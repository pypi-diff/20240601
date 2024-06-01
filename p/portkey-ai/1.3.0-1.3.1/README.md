# Comparing `tmp/portkey_ai-1.3.0.tar.gz` & `tmp/portkey_ai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portkey_ai-1.3.0.tar", last modified: Fri May 31 15:23:52 2024, max compression
+gzip compressed data, was "portkey_ai-1.3.1.tar", last modified: Fri May 31 16:42:58 2024, max compression
```

## Comparing `portkey_ai-1.3.0.tar` & `portkey_ai-1.3.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.579394 portkey_ai-1.3.0/
--rw-r--r--   0 visargdesai   (501) staff       (20)     1067 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/LICENSE
--rw-r--r--   0 visargdesai   (501) staff       (20)     5319 2024-05-31 15:23:52.579286 portkey_ai-1.3.0/PKG-INFO
--rw-r--r--   0 visargdesai   (501) staff       (20)     4240 2024-04-05 10:21:35.000000 portkey_ai-1.3.0/README.md
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.476666 portkey_ai-1.3.0/portkey_ai/
--rw-r--r--   0 visargdesai   (501) staff       (20)     2816 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      380 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/_portkey_scripts.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.480650 portkey_ai-1.3.0/portkey_ai/api_resources/
--rw-r--r--   0 visargdesai   (501) staff       (20)     2520 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/__init__.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.488632 portkey_ai-1.3.0/portkey_ai/api_resources/apis/
--rw-r--r--   0 visargdesai   (501) staff       (20)     2324 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1180 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/api_resource.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3662 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/assistants.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     6417 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/audio.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3971 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/batches.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     6707 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/chat_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     6026 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1139 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/create_headers.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2177 2024-04-13 08:51:10.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/embeddings.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3795 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/feedback.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     8416 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/fine_tuning.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    10091 2024-04-05 10:21:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/generation.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     5679 2024-04-13 08:51:10.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/images.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4432 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/main_files.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2639 2024-04-13 08:51:10.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/models.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1574 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/moderations.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2493 2024-02-13 17:21:25.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/post.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    40728 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/threads.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    24230 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/apis/vector_stores.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    29119 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/base_client.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    14130 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/client.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      903 2024-04-05 10:21:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/common_types.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4020 2024-01-12 13:07:25.000000 portkey_ai-1.3.0/portkey_ai/api_resources/exceptions.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1164 2024-03-21 12:59:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/global_constants.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7058 2024-02-13 17:21:25.000000 portkey_ai-1.3.0/portkey_ai/api_resources/streaming.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.494855 portkey_ai-1.3.0/portkey_ai/api_resources/types/
--rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-03-21 12:59:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3612 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/assistant_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1173 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/audio_types.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2159 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/batches_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3568 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/chat_complete_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2413 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/complete_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1163 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/embeddings_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      212 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/feedback_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4872 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/fine_tuning_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3420 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/generation_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      858 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/image_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1978 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/main_file_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     1675 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/models_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      793 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/moderations_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3415 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_message_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     6102 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_run_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      965 2024-04-13 13:30:23.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      426 2024-03-21 12:59:35.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/utils.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3417 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/portkey_ai/api_resources/types/vector_stores_type.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    12969 2024-05-31 14:38:31.000000 portkey_ai-1.3.0/portkey_ai/api_resources/utils.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.495043 portkey_ai-1.3.0/portkey_ai/llms/
--rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/__init__.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.495689 portkey_ai-1.3.0/portkey_ai/llms/langchain/
--rw-r--r--   0 visargdesai   (501) staff       (20)      106 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/langchain/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7232 2024-05-31 15:19:33.000000 portkey_ai-1.3.0/portkey_ai/llms/langchain/chat.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4771 2024-05-31 15:19:33.000000 portkey_ai-1.3.0/portkey_ai/llms/langchain/completion.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.534356 portkey_ai-1.3.0/portkey_ai/llms/llama_index/
--rw-r--r--   0 visargdesai   (501) staff       (20)       62 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/llama_index/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7253 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/llama_index/completions.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     3277 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/llms/llama_index/utils.py
--rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/portkey_ai/py.typed
--rw-r--r--   0 visargdesai   (501) staff       (20)       18 2024-05-31 15:22:36.000000 portkey_ai-1.3.0/portkey_ai/version.py
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.577669 portkey_ai-1.3.0/portkey_ai.egg-info/
--rw-r--r--   0 visargdesai   (501) staff       (20)     5319 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/PKG-INFO
--rw-r--r--   0 visargdesai   (501) staff       (20)     3178 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/SOURCES.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)        1 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/dependency_links.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)       64 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/entry_points.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)      263 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/requires.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)       17 2024-05-31 15:23:52.000000 portkey_ai-1.3.0/portkey_ai.egg-info/top_level.txt
--rw-r--r--   0 visargdesai   (501) staff       (20)        1 2024-01-08 09:37:18.000000 portkey_ai-1.3.0/portkey_ai.egg-info/zip-safe
--rw-r--r--   0 visargdesai   (501) staff       (20)       80 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/pyproject.toml
--rw-r--r--   0 visargdesai   (501) staff       (20)     1155 2024-05-31 15:23:52.586785 portkey_ai-1.3.0/setup.cfg
-drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 15:23:52.577261 portkey_ai-1.3.0/tests/
--rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.0/tests/__init__.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4668 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_assistants.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4609 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_async_audio_speech.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4618 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_async_audio_transcript.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4627 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_async_audio_translation.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    15529 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_async_chat_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    14317 2024-05-31 14:40:38.000000 portkey_ai-1.3.0/tests/test_async_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7609 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_async_images.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4400 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_async_moderations.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4468 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_audio_speech.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4476 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_audio_transcript.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4486 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_audio_translation.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    14966 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_chat_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)    13730 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_complete.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     7246 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_images.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     4259 2024-05-31 14:29:48.000000 portkey_ai-1.3.0/tests/test_moderations.py
--rw-r--r--   0 visargdesai   (501) staff       (20)     2536 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/test_threads.py
--rw-r--r--   0 visargdesai   (501) staff       (20)      497 2024-03-21 14:00:19.000000 portkey_ai-1.3.0/tests/utils.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.997795 portkey_ai-1.3.1/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1067 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/LICENSE
+-rw-r--r--   0 visargdesai   (501) staff       (20)     5319 2024-05-31 16:42:58.997708 portkey_ai-1.3.1/PKG-INFO
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4240 2024-04-05 10:21:35.000000 portkey_ai-1.3.1/README.md
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.973475 portkey_ai-1.3.1/portkey_ai/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2816 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      380 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/portkey_ai/_portkey_scripts.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.976812 portkey_ai-1.3.1/portkey_ai/api_resources/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2520 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/__init__.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.982642 portkey_ai-1.3.1/portkey_ai/api_resources/apis/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2324 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1180 2024-05-31 14:38:31.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/api_resource.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3662 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/assistants.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     6417 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/audio.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3971 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/batches.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     6707 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/chat_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     6026 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1116 2024-05-31 16:38:29.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/create_headers.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2177 2024-04-13 08:51:10.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/embeddings.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3795 2024-05-31 14:38:31.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/feedback.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     8416 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/fine_tuning.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    10091 2024-04-05 10:21:35.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/generation.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     5679 2024-04-13 08:51:10.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/images.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4432 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/main_files.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2639 2024-04-13 08:51:10.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/models.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1574 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/moderations.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2493 2024-02-13 17:21:25.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/post.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    40728 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/threads.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    24230 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/apis/vector_stores.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    29119 2024-05-31 14:38:31.000000 portkey_ai-1.3.1/portkey_ai/api_resources/base_client.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    14130 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/client.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      903 2024-04-05 10:21:35.000000 portkey_ai-1.3.1/portkey_ai/api_resources/common_types.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4020 2024-01-12 13:07:25.000000 portkey_ai-1.3.1/portkey_ai/api_resources/exceptions.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1164 2024-03-21 12:59:35.000000 portkey_ai-1.3.1/portkey_ai/api_resources/global_constants.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7058 2024-02-13 17:21:25.000000 portkey_ai-1.3.1/portkey_ai/api_resources/streaming.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.989014 portkey_ai-1.3.1/portkey_ai/api_resources/types/
+-rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-03-21 12:59:35.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3612 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/assistant_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1173 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/audio_types.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2159 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/batches_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3568 2024-04-13 13:30:23.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/chat_complete_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2413 2024-04-13 13:30:23.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/complete_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1163 2024-04-13 13:30:23.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/embeddings_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      212 2024-05-31 14:38:31.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/feedback_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4872 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/fine_tuning_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3420 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/generation_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      858 2024-04-13 13:30:23.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/image_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1978 2024-04-13 13:30:23.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/main_file_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1675 2024-04-13 13:30:23.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/models_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      793 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/moderations_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3415 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/thread_message_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     6102 2024-04-13 13:30:23.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/thread_run_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      965 2024-04-13 13:30:23.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/thread_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      426 2024-03-21 12:59:35.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/utils.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3417 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/portkey_ai/api_resources/types/vector_stores_type.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    12969 2024-05-31 14:38:31.000000 portkey_ai-1.3.1/portkey_ai/api_resources/utils.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.989205 portkey_ai-1.3.1/portkey_ai/llms/
+-rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/portkey_ai/llms/__init__.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.990022 portkey_ai-1.3.1/portkey_ai/llms/langchain/
+-rw-r--r--   0 visargdesai   (501) staff       (20)      106 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/portkey_ai/llms/langchain/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7232 2024-05-31 15:19:33.000000 portkey_ai-1.3.1/portkey_ai/llms/langchain/chat.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4771 2024-05-31 15:19:33.000000 portkey_ai-1.3.1/portkey_ai/llms/langchain/completion.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.991018 portkey_ai-1.3.1/portkey_ai/llms/llama_index/
+-rw-r--r--   0 visargdesai   (501) staff       (20)       62 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/portkey_ai/llms/llama_index/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7253 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/portkey_ai/llms/llama_index/completions.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3277 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/portkey_ai/llms/llama_index/utils.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/portkey_ai/py.typed
+-rw-r--r--   0 visargdesai   (501) staff       (20)       18 2024-05-31 16:41:59.000000 portkey_ai-1.3.1/portkey_ai/version.py
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.996590 portkey_ai-1.3.1/portkey_ai.egg-info/
+-rw-r--r--   0 visargdesai   (501) staff       (20)     5319 2024-05-31 16:42:58.000000 portkey_ai-1.3.1/portkey_ai.egg-info/PKG-INFO
+-rw-r--r--   0 visargdesai   (501) staff       (20)     3178 2024-05-31 16:42:58.000000 portkey_ai-1.3.1/portkey_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)        1 2024-05-31 16:42:58.000000 portkey_ai-1.3.1/portkey_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)       64 2024-05-31 16:42:58.000000 portkey_ai-1.3.1/portkey_ai.egg-info/entry_points.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)      263 2024-05-31 16:42:58.000000 portkey_ai-1.3.1/portkey_ai.egg-info/requires.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)       17 2024-05-31 16:42:58.000000 portkey_ai-1.3.1/portkey_ai.egg-info/top_level.txt
+-rw-r--r--   0 visargdesai   (501) staff       (20)        1 2024-01-08 09:37:18.000000 portkey_ai-1.3.1/portkey_ai.egg-info/zip-safe
+-rw-r--r--   0 visargdesai   (501) staff       (20)       80 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/pyproject.toml
+-rw-r--r--   0 visargdesai   (501) staff       (20)     1155 2024-05-31 16:42:58.998173 portkey_ai-1.3.1/setup.cfg
+drwxr-xr-x   0 visargdesai   (501) staff       (20)        0 2024-05-31 16:42:58.996262 portkey_ai-1.3.1/tests/
+-rw-r--r--   0 visargdesai   (501) staff       (20)        0 2024-01-08 09:33:02.000000 portkey_ai-1.3.1/tests/__init__.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4668 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_assistants.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4609 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_async_audio_speech.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4618 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_async_audio_transcript.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4627 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_async_audio_translation.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    15529 2024-03-21 14:00:19.000000 portkey_ai-1.3.1/tests/test_async_chat_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    14317 2024-05-31 14:40:38.000000 portkey_ai-1.3.1/tests/test_async_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7609 2024-03-21 14:00:19.000000 portkey_ai-1.3.1/tests/test_async_images.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4400 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_async_moderations.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4468 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_audio_speech.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4476 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_audio_transcript.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4486 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_audio_translation.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    14966 2024-03-21 14:00:19.000000 portkey_ai-1.3.1/tests/test_chat_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)    13730 2024-03-21 14:00:19.000000 portkey_ai-1.3.1/tests/test_complete.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     7246 2024-03-21 14:00:19.000000 portkey_ai-1.3.1/tests/test_images.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     4259 2024-05-31 14:29:48.000000 portkey_ai-1.3.1/tests/test_moderations.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)     2536 2024-03-21 14:00:19.000000 portkey_ai-1.3.1/tests/test_threads.py
+-rw-r--r--   0 visargdesai   (501) staff       (20)      497 2024-03-21 14:00:19.000000 portkey_ai-1.3.1/tests/utils.py
```

### Comparing `portkey_ai-1.3.0/LICENSE` & `portkey_ai-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/PKG-INFO` & `portkey_ai-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portkey-ai
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client library for the Portkey API
 Home-page: https://github.com/Portkey-AI/portkey-python-sdk
 Author: Portkey.ai
 Author-email: support@portkey.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `portkey_ai-1.3.0/README.md` & `portkey_ai-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/__init__.py` & `portkey_ai-1.3.1/portkey_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/__init__.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/__init__.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/api_resource.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/api_resource.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/assistants.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/assistants.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/audio.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/audio.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/batches.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/batches.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/chat_complete.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/chat_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/complete.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/create_headers.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/create_headers.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,13 +25,12 @@
                     headers[get_portkey_header(k)] = str(v)
                 else:
                     headers[k] = str("Bearer " + v)
 
                 # logic for List of str to comma separated string
                 if k == "forward-headers":
                     headers[get_portkey_header(k)] = ",".join(v)
-        print(headers)
         return headers
 
 
 def createHeaders(**kwargs):
     return CreateHeaders(**kwargs).json()
```

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/embeddings.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/embeddings.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/feedback.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/feedback.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/fine_tuning.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/generation.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/generation.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/images.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/images.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/main_files.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/main_files.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/models.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/models.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/moderations.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/moderations.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/post.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/post.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/threads.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/threads.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/apis/vector_stores.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/apis/vector_stores.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/base_client.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/base_client.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/client.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/client.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/common_types.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/common_types.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/exceptions.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/exceptions.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/global_constants.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/global_constants.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/streaming.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/streaming.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/assistant_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/assistant_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/audio_types.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/audio_types.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/batches_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/batches_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/chat_complete_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/chat_complete_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/complete_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/complete_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/embeddings_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/embeddings_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/fine_tuning_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/fine_tuning_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/generation_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/generation_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/image_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/image_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/main_file_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/main_file_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/models_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/models_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/moderations_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/moderations_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_message_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/thread_message_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_run_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/thread_run_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/thread_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/thread_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/types/vector_stores_type.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/types/vector_stores_type.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/api_resources/utils.py` & `portkey_ai-1.3.1/portkey_ai/api_resources/utils.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/llms/langchain/chat.py` & `portkey_ai-1.3.1/portkey_ai/llms/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/llms/langchain/completion.py` & `portkey_ai-1.3.1/portkey_ai/llms/langchain/completion.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/llms/llama_index/completions.py` & `portkey_ai-1.3.1/portkey_ai/llms/llama_index/completions.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai/llms/llama_index/utils.py` & `portkey_ai-1.3.1/portkey_ai/llms/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/portkey_ai.egg-info/PKG-INFO` & `portkey_ai-1.3.1/portkey_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portkey-ai
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python client library for the Portkey API
 Home-page: https://github.com/Portkey-AI/portkey-python-sdk
 Author: Portkey.ai
 Author-email: support@portkey.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `portkey_ai-1.3.0/portkey_ai.egg-info/SOURCES.txt` & `portkey_ai-1.3.1/portkey_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/setup.cfg` & `portkey_ai-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_assistants.py` & `portkey_ai-1.3.1/tests/test_assistants.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_async_audio_speech.py` & `portkey_ai-1.3.1/tests/test_async_audio_speech.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_async_audio_transcript.py` & `portkey_ai-1.3.1/tests/test_async_audio_transcript.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_async_audio_translation.py` & `portkey_ai-1.3.1/tests/test_async_audio_translation.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_async_chat_complete.py` & `portkey_ai-1.3.1/tests/test_async_chat_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_async_complete.py` & `portkey_ai-1.3.1/tests/test_async_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_async_images.py` & `portkey_ai-1.3.1/tests/test_async_images.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_async_moderations.py` & `portkey_ai-1.3.1/tests/test_async_moderations.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_audio_speech.py` & `portkey_ai-1.3.1/tests/test_audio_speech.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_audio_transcript.py` & `portkey_ai-1.3.1/tests/test_audio_transcript.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_audio_translation.py` & `portkey_ai-1.3.1/tests/test_audio_translation.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_chat_complete.py` & `portkey_ai-1.3.1/tests/test_chat_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_complete.py` & `portkey_ai-1.3.1/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_images.py` & `portkey_ai-1.3.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_moderations.py` & `portkey_ai-1.3.1/tests/test_moderations.py`

 * *Files identical despite different names*

### Comparing `portkey_ai-1.3.0/tests/test_threads.py` & `portkey_ai-1.3.1/tests/test_threads.py`

 * *Files identical despite different names*

