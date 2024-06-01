# Comparing `tmp/langfun-0.0.2.dev20240530.tar.gz` & `tmp/langfun-0.0.2.dev20240531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240530.tar", last modified: Thu May 30 08:04:10 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240531.tar", last modified: Fri May 31 08:04:22 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240530.tar` & `langfun-0.0.2.dev20240531.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.801158 langfun-0.0.2.dev20240530/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-30 08:04:10.801158 langfun-0.0.2.dev20240530/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.781158 langfun-0.0.2.dev20240530/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.789158 langfun-0.0.2.dev20240530/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.789158 langfun-0.0.2.dev20240530/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.789158 langfun-0.0.2.dev20240530/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.793158 langfun-0.0.2.dev20240530/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.793158 langfun-0.0.2.dev20240530/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.793158 langfun-0.0.2.dev20240530/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/openai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/llms/vertexai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.797158 langfun-0.0.2.dev20240530/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.797158 langfun-0.0.2.dev20240530/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/audio_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/ms_office.py
--rw-r--r--   0 runner    (1001) docker     (127)    85434 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/ms_office_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/pdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.801158 langfun-0.0.2.dev20240530/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19281 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.801158 langfun-0.0.2.dev20240530/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:10.801158 langfun-0.0.2.dev20240530/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-30 08:04:10.000000 langfun-0.0.2.dev20240530/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-30 08:04:10.000000 langfun-0.0.2.dev20240530/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:04:10.000000 langfun-0.0.2.dev20240530/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 08:04:10.000000 langfun-0.0.2.dev20240530/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 08:04:10.000000 langfun-0.0.2.dev20240530/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:04:10.801158 langfun-0.0.2.dev20240530/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-30 08:03:29.000000 langfun-0.0.2.dev20240530/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.482950 langfun-0.0.2.dev20240531/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.486950 langfun-0.0.2.dev20240531/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.486950 langfun-0.0.2.dev20240531/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.490950 langfun-0.0.2.dev20240531/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.490950 langfun-0.0.2.dev20240531/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.494950 langfun-0.0.2.dev20240531/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.494950 langfun-0.0.2.dev20240531/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/openai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/vertexai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.494950 langfun-0.0.2.dev20240531/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.494950 langfun-0.0.2.dev20240531/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/audio_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/ms_office.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85434 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/ms_office_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/pdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.498950 langfun-0.0.2.dev20240531/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19281 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27664 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/setup.py
```

### Comparing `langfun-0.0.2.dev20240530/LICENSE` & `langfun-0.0.2.dev20240531/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/PKG-INFO` & `langfun-0.0.2.dev20240531/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240530
+Version: 0.0.2.dev20240531
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240530/README.md` & `langfun-0.0.2.dev20240531/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/__init__.py` & `langfun-0.0.2.dev20240531/langfun/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from langfun.core import *
 from langfun.core import structured
 
 Schema = structured.Schema
 MISSING = structured.MISSING
 UNKNOWN = structured.UNKNOWN
 
+include_method_in_prompt = structured.include_method_in_prompt
+
 MappingExample = structured.MappingExample
 
 call = structured.call
 parse = structured.parse
 query = structured.query
 describe = structured.describe
 complete = structured.complete
```

### Comparing `langfun-0.0.2.dev20240530/langfun/core/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240531/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/component.py` & `langfun-0.0.2.dev20240531/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/component_test.py` & `langfun-0.0.2.dev20240531/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240531/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240531/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/console.py` & `langfun-0.0.2.dev20240531/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/console_test.py` & `langfun-0.0.2.dev20240531/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240531/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240531/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240531/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/language_model.py` & `langfun-0.0.2.dev20240531/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240531/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/vertexai.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/llms/vertexai_test.py` & `langfun-0.0.2.dev20240531/langfun/core/llms/vertexai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240531/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240531/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/memory.py` & `langfun-0.0.2.dev20240531/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/message.py` & `langfun-0.0.2.dev20240531/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/message_test.py` & `langfun-0.0.2.dev20240531/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/audio.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/audio.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/audio_test.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/audio_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/ms_office.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/ms_office.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/ms_office_test.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/ms_office_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/pdf.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/pdf.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/pdf_test.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/pdf_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240531/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modality.py` & `langfun-0.0.2.dev20240531/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240531/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240531/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240531/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/sampling.py` & `langfun-0.0.2.dev20240531/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240531/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Common langfun templates."""
 
 # pylint: disable=g-bad-import-order
 # pylint: disable=g-importing-member
 
+from langfun.core.structured.schema import include_method_in_prompt
+
 from langfun.core.structured.schema import Missing
 from langfun.core.structured.schema import MISSING
 from langfun.core.structured.schema import Unknown
 from langfun.core.structured.schema import UNKNOWN
 
 from langfun.core.structured.schema import Schema
 from langfun.core.structured.schema import SchemaProtocol
```

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,17 @@
     value_specs = tuple(
         [v.value_spec for v in schema_lib.Missing.find_missing(value).values()]
     )
     return schema_lib.class_dependencies(value_specs, include_subclasses=True)
 
   def class_defs_repr(self, value: Any) -> str | None:
     return schema_lib.class_definitions(
-        self.missing_type_dependencies(value), markdown=True
+        self.missing_type_dependencies(value),
+        markdown=True,
+        allowed_dependencies=set()
     )
 
   def postprocess_result(self, result: Any) -> Any:
     """Postprocess result."""
     # Try restore modality objects from the input value to output value.
     modalities = self.modalities(self.input)
     if modalities:
```

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
       {{ modality_refs_title }}:
       {{ modality_refs_repr(example.input) | indent(2, True) }}
 
       {% endif -%}
 
       {%- if example.schema -%}
       {{ schema_title }}:
-      {{ example.schema_repr(protocol, include_methods=include_methods) | indent(2, True) }}
+      {{ example.schema_repr(protocol) | indent(2, True) }}
 
       {% endif -%}
 
       {{ output_title }}:
       {%- if example.has_output %}
       {{ example.output_repr(protocol, compact=False) | indent(2, True) }}
       {% endif -%}
@@ -275,18 +275,14 @@
   ] = 'MODALITY_REFERENCES'
 
   protocol: Annotated[
       schema_lib.SchemaProtocol,
       'The protocol for representing the schema and value.',
   ] = 'python'
 
-  include_methods: Annotated[
-      bool, 'If True, include method definitions in the schema.'
-  ] = False
-
   #
   # Other user-provided flags.
   #
 
   examples: Annotated[
       list[MappingExample] | None,
       'Fewshot examples for improving the quality of mapping.',
```

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/prompting.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,14 @@
     lm: lf.LanguageModel | None = None,
     examples: list[mapping.MappingExample] | None = None,
     cache_seed: int | None = 0,
     response_postprocess: Callable[[str], str] | None = None,
     autofix: int = 0,
     autofix_lm: lf.LanguageModel | None = None,
     protocol: schema_lib.SchemaProtocol = 'python',
-    include_methods: bool = False,
     returns_message: bool = False,
     skip_lm: bool = False,
     **kwargs,
 ) -> Any:
   """Parse a natural langugage message based on schema.
 
   Examples:
@@ -170,16 +169,14 @@
     autofix: Number of attempts to auto fix the generated code. If 0, autofix is
       disabled. Auto-fix is not supported for 'json' protocol.
     autofix_lm: The language model to use for autofix. If not specified, the
       `autofix_lm` from `lf.context` context manager will be used. Otherwise it
       will use `lm`.
     protocol: The protocol for schema/value representation. Applicable values
       are 'json' and 'python'. By default `python` will be used.
-    include_methods: If True, include method definitions in the output type
-      during prompting.
     returns_message: If True, returns `lf.Message` as the output, instead of
       returning the structured `message.result`.
     skip_lm: If True, returns the rendered prompt as a UserMessage object.
       otherwise return the LLM response based on the rendered prompt.
     **kwargs: Keyword arguments passed to render the prompt or configure the 
       `lf.structured.Mapping` class. Notable kwargs are:
       - template_str: Change the root template for query.
@@ -221,15 +218,14 @@
     prompt = schema_lib.mark_missing(prompt)
 
   output = _query_structure_cls(protocol)(
       input=prompt,
       schema=schema,
       default=default,
       examples=examples,
-      include_methods=include_methods,
       response_postprocess=response_postprocess,
       autofix=autofix if protocol == 'python' else 0,
       **kwargs,
   )(
       lm=lm,
       autofix_lm=autofix_lm or lm,
       cache_seed=cache_seed,
```

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Schema for structured data."""
 
 import abc
 import inspect
 import io
+import re
 import textwrap
 import typing
 from typing import Any, Literal, Sequence, Type, Union
 import langfun.core as lf
 from langfun.core.coding.python import correction
 import pyglove as pg
 
 
+def include_method_in_prompt(method):
+  """Decorator to include a method in the class definition of the prompt."""
+  setattr(method, '__show_in_prompt__', True)
+  return method
+
+
+def should_include_method_in_prompt(method):
+  """Returns true if the method should be shown in the prompt."""
+  return getattr(method, '__show_in_prompt__', False)
+
+
 def parse_value_spec(value) -> pg.typing.ValueSpec:
   """Parses a PyGlove ValueSpec equivalence into a ValueSpec."""
   if isinstance(value, pg.typing.ValueSpec):
     return value
 
   if isinstance(value, dict) and len(value) == 1 and 'result' in value:
     value = value['result']
@@ -159,17 +171,20 @@
           'Unsupported value spec being used as the schema for '
           f'structured data: {vs}.')
 
     return {'result': _node(self.spec)}
 
   def class_dependencies(
       self,
+      include_base_classes: bool = True,
       include_subclasses: bool = True) -> list[Type[Any]]:
     """Returns a list of class dependencies for current schema."""
-    return class_dependencies(self.spec, include_subclasses)
+    return class_dependencies(
+        self.spec, include_base_classes, include_subclasses
+    )
 
   @classmethod
   def from_value(cls, value) -> 'Schema':
     """Creates a schema from an equivalent representation."""
     if isinstance(value, Schema):
       return value
     return cls(parse_value_spec(value))
@@ -194,19 +209,20 @@
     value_or_spec: Union[
         pg.Symbolic,
         Schema,
         pg.typing.ValueSpec,
         Type[pg.Object],
         tuple[Union[pg.typing.ValueSpec, Type[pg.Object]], ...],
     ],
+    include_base_classes: bool = True,
     include_subclasses: bool = True,
 ) -> list[Type[Any]]:
   """Returns a list of class dependencies from a value or specs."""
   if isinstance(value_or_spec, Schema):
-    return value_or_spec.class_dependencies(include_subclasses)
+    value_or_spec = value_or_spec.spec
 
   if inspect.isclass(value_or_spec) or isinstance(
       value_or_spec, pg.typing.ValueSpec
   ):
     value_or_spec = (value_or_spec,)
 
   if isinstance(value_or_spec, tuple):
@@ -232,21 +248,22 @@
         dependencies.append(cls)
 
   def _fill_dependencies(vs: pg.typing.ValueSpec, include_subclasses: bool):
     if isinstance(vs, pg.typing.Object):
       if vs.cls not in seen:
         seen.add(vs.cls)
 
-        # Add base classes as dependencies.
-        for base_cls in vs.cls.__bases__:
-          # We only keep track of user-defined symbolic classes.
-          if base_cls is not object and base_cls is not pg.Object:
-            _fill_dependencies(
-                pg.typing.Object(base_cls), include_subclasses=False
-            )
+        if include_base_classes:
+          # Add base classes as dependencies.
+          for base_cls in vs.cls.__bases__:
+            # We only keep track of user-defined symbolic classes.
+            if base_cls is not object and base_cls is not pg.Object:
+              _fill_dependencies(
+                  pg.typing.Object(base_cls), include_subclasses=False
+              )
 
         # Add members as dependencies.
         for field in _pg_schema(vs.cls).values():
           _fill_dependencies(field.value, include_subclasses)
       _add_dependency(vs.cls)
 
       # Check subclasses if available.
@@ -297,83 +314,91 @@
   """Python-representation for a schema."""
 
   def repr(
       self,
       schema: Schema,
       *,
       include_result_definition: bool = True,
-      include_methods: bool = False,
       markdown: bool = True,
       **kwargs,
   ) -> str:
     ret = ''
     if include_result_definition:
       ret += self.result_definition(schema)
     class_definition_str = self.class_definitions(
-        schema, markdown=markdown, include_methods=include_methods, **kwargs
+        schema, markdown=markdown, **kwargs
     )
     if class_definition_str:
       ret += f'\n\n{class_definition_str}'
     return ret.strip()
 
-  def class_definitions(self, schema: Schema, **kwargs) -> str | None:
-    deps = schema.class_dependencies(include_subclasses=True)
-    return class_definitions(deps, **kwargs)
+  def class_definitions(
+      self,
+      schema: Schema,
+      additional_dependencies: list[Type[Any]] | None = None,
+      **kwargs
+  ) -> str | None:
+    """Returns a string containing of class definitions from a schema."""
+    deps = schema.class_dependencies(
+        include_base_classes=False, include_subclasses=True
+    )
+    allowed_dependencies = set(deps)
+    if additional_dependencies:
+      allowed_dependencies.update(additional_dependencies)
+    return class_definitions(
+        deps, allowed_dependencies=allowed_dependencies, **kwargs)
 
   def result_definition(self, schema: Schema) -> str:
     return annotation(schema.spec)
 
 
 def source_form(value, markdown: bool = False) -> str:
   """Returns the source code form of an object."""
   return ValuePythonRepr().repr(value, markdown=markdown)
 
 
 def class_definitions(
     classes: Sequence[Type[Any]],
     *,
-    include_pg_object_as_base: bool = False,
-    include_methods: bool = False,
+    allowed_dependencies: set[Type[Any]] | None = None,
     strict: bool = False,
     markdown: bool = False,
 ) -> str | None:
   """Returns a str for class definitions."""
   if not classes:
     return None
   def_str = io.StringIO()
   for i, cls in enumerate(classes):
     if i > 0:
       def_str.write('\n')
     def_str.write(
         class_definition(
             cls,
             strict=strict,
-            include_pg_object_as_base=include_pg_object_as_base,
-            include_methods=include_methods,
+            allowed_dependencies=allowed_dependencies,
         )
     )
   ret = def_str.getvalue()
   if markdown and ret:
     ret = f'```python\n{ret}```'
   return ret
 
 
 def class_definition(
     cls,
     strict: bool = False,
-    include_pg_object_as_base: bool = False,
-    include_methods: bool = False,
+    allowed_dependencies: set[Type[Any]] | None = None,
 ) -> str:
   """Returns the Python class definition."""
   out = io.StringIO()
   schema = _pg_schema(cls)
   eligible_bases = []
   for base_cls in cls.__bases__:
     if base_cls is not object:
-      if include_pg_object_as_base or base_cls is not pg.Object:
+      if allowed_dependencies is None or base_cls in allowed_dependencies:
         eligible_bases.append(base_cls.__name__)
 
   if eligible_bases:
     base_cls_str = ', '.join(eligible_bases)
     out.write(f'class {cls.__name__}({base_cls_str}):\n')
   else:
     out.write(f'class {cls.__name__}:\n')
@@ -402,58 +427,71 @@
       # Write field doc string as comments before the field definition.
       if field.description:
         for line in field.description.split('\n'):
           if line:
             out.write('  # ')
             out.write(line)
             out.write('\n')
-      out.write(f'  {field.key}: {annotation(field.value, strict=strict)}')
-      out.write('\n')
-      empty_class = False
 
-  if include_methods:
-    for method in _iter_newly_defined_methods(cls):
-      out.write('\n')
-      out.write(
-          textwrap.indent(
-              inspect.cleandoc('\n' + inspect.getsource(method)), ' ' * 2)
+      annotation_str = annotation(
+          field.value, strict=strict, allowed_dependencies=allowed_dependencies
       )
+      out.write(f'  {field.key}: {annotation_str}')
       out.write('\n')
       empty_class = False
 
+  for method in _iter_newly_defined_methods(cls, allowed_dependencies):
+    source = inspect.getsource(method)
+    # Remove decorators from the method definition.
+    source = re.sub(r'\s*@.*\.include_method_in_prompt.*\n', '', source)
+    out.write('\n')
+    out.write(
+        textwrap.indent(
+            inspect.cleandoc('\n' + source), ' ' * 2)
+    )
+    out.write('\n')
+    empty_class = False
+
   if empty_class:
     out.write('  pass\n')
   return out.getvalue()
 
 
-def _iter_newly_defined_methods(cls):
-  names = set(dir(cls))
+def _iter_newly_defined_methods(
+    cls, allowed_dependencies: set[Type[Any]] | None):
+  names = {attr_name: True for attr_name in dir(cls)}
   for base in cls.__bases__:
-    names -= set(dir(base))
-  for name in names:
+    if allowed_dependencies is None or base in allowed_dependencies:
+      for name in dir(base):
+        names.pop(name, None)
+  for name in names.keys():
     attr = getattr(cls, name)
-    if callable(attr):
+    if callable(attr) and should_include_method_in_prompt(attr):
       yield attr
 
 
 def annotation(
     vs: pg.typing.ValueSpec,
     annotate_optional: bool = True,
     strict: bool = False,
+    allowed_dependencies: set[Type[Any]] | None = None,
 ) -> str:
   """Returns the annotation string for a value spec."""
+  child_annotation_kwargs = dict(
+      strict=strict, allowed_dependencies=allowed_dependencies
+  )
   if isinstance(vs, pg.typing.Any):
     return 'Any'
   elif isinstance(vs, pg.typing.Enum):
     candidate_str = ', '.join([repr(v) for v in vs.values])
     return f'Literal[{candidate_str}]'
   elif isinstance(vs, pg.typing.Union):
     candidate_str = ', '.join(
         [
-            annotation(c, annotate_optional=False, strict=strict)
+            annotation(c, annotate_optional=False, **child_annotation_kwargs)
             for c in vs.candidates
         ]
     )
     if vs.is_noneable:
       candidate_str += ', None'
     return f'Union[{candidate_str}]'
 
@@ -481,39 +519,42 @@
         x = (
             'pg.typing.Int'
             if isinstance(vs, pg.typing.Int)
             else 'pg.typing.Float'
         )
       x += '(' + ', '.join(constraints) + ')'
   elif isinstance(vs, pg.typing.Object):
-    x = vs.cls.__name__
+    if allowed_dependencies is None or vs.cls in allowed_dependencies:
+      x = vs.cls.__name__
+    else:
+      x = 'Any'
   elif isinstance(vs, pg.typing.List):
-    item_str = annotation(vs.element.value, strict=strict)
+    item_str = annotation(vs.element.value, **child_annotation_kwargs)
     x = f'list[{item_str}]'
   elif isinstance(vs, pg.typing.Tuple):
     elem_str = ', '.join(
-        [annotation(el.value, strict=strict) for el in vs.elements]
+        [annotation(el.value, **child_annotation_kwargs) for el in vs.elements]
     )
     x = f'tuple[{elem_str}]'
   elif isinstance(vs, pg.typing.Dict):
     kv_pairs = None
     if vs.schema is not None:
       kv_pairs = [
-          (k, annotation(f.value, strict=strict))
+          (k, annotation(f.value, **child_annotation_kwargs))
           for k, f in vs.schema.items()
           if isinstance(k, pg.typing.ConstStrKey)
       ]
 
     if kv_pairs:
       kv_str = ', '.join(f"'{k}': {v}" for k, v in kv_pairs)
       x = '{' + kv_str + '}'
       if strict:
         x = f'pg.typing.Dict({x})'
     elif vs.schema and vs.schema.dynamic_field:
-      v = annotation(vs.schema.dynamic_field.value, strict=strict)
+      v = annotation(vs.schema.dynamic_field.value, **child_annotation_kwargs)
       x = f'dict[str, {v}]'
     else:
       x = 'dict[str, Any]'
 
   else:
     raise TypeError(f'Unsupported value spec being used as schema: {vs}.')
 
@@ -600,15 +641,20 @@
            markdown: bool = True,
            **kwargs) -> str:
     del schema
     if inspect.isclass(value):
       cls_schema = Schema.from_value(value)
       if isinstance(cls_schema.spec, pg.typing.Object):
         object_code = SchemaPythonRepr().class_definitions(
-            cls_schema, markdown=markdown, include_pg_object_as_base=True
+            cls_schema,
+            markdown=markdown,
+            # We add `pg.Object` as additional dependencies to the class
+            # definition so exemplars for class generation could show
+            # pg.Object as their bases.
+            additional_dependencies=[pg.Object]
         )
         assert object_code is not None
         return object_code
       else:
         object_code = SchemaPythonRepr().result_definition(cls_schema)
     else:
       object_code = pg.format(
```

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/schema_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -279,17 +279,18 @@
 class SchemaPythonReprTest(unittest.TestCase):
 
   def assert_annotation(
       self,
       value_spec: pg.typing.ValueSpec,
       expected_annotation: str,
       strict: bool = False,
+      **kwargs,
   ) -> None:
     self.assertEqual(
-        schema_lib.annotation(value_spec, strict=strict),
+        schema_lib.annotation(value_spec, strict=strict, **kwargs),
         expected_annotation,
     )
 
   def test_annotation(self):
     # Bool.
     self.assert_annotation(pg.typing.Bool(), 'bool')
     self.assert_annotation(pg.typing.Bool().noneable(), 'bool | None')
@@ -357,40 +358,75 @@
     )
 
     # Object.
     self.assert_annotation(pg.typing.Object(Activity), 'Activity')
     self.assert_annotation(
         pg.typing.Object(Activity).noneable(), 'Activity | None'
     )
+    self.assert_annotation(
+        pg.typing.Object(Activity).noneable(), 'Activity | None',
+        allowed_dependencies=set([Activity]),
+    )
+    self.assert_annotation(
+        pg.typing.Object(Activity).noneable(), 'Any | None',
+        allowed_dependencies=set(),
+    )
 
     # List.
     self.assert_annotation(
         pg.typing.List(pg.typing.Object(Activity)), 'list[Activity]'
     )
     self.assert_annotation(
+        pg.typing.List(pg.typing.Object(Activity)), 'list[Activity]',
+        allowed_dependencies=set([Activity]),
+    )
+    self.assert_annotation(
+        pg.typing.List(pg.typing.Object(Activity)), 'list[Any]',
+        allowed_dependencies=set(),
+    )
+    self.assert_annotation(
         pg.typing.List(pg.typing.Object(Activity)).noneable(),
         'list[Activity] | None',
     )
     self.assert_annotation(
         pg.typing.List(pg.typing.Object(Activity).noneable()),
         'list[Activity | None]',
     )
 
     # Tuple.
     self.assert_annotation(
-        pg.typing.Tuple([pg.typing.Int(), pg.typing.Str()]), 'tuple[int, str]'
+        pg.typing.Tuple([Activity, pg.typing.Str()]), 'tuple[Activity, str]'
+    )
+    self.assert_annotation(
+        pg.typing.Tuple([Activity, pg.typing.Str()]), 'tuple[Activity, str]',
+        allowed_dependencies=set([Activity]),
     )
     self.assert_annotation(
-        pg.typing.Tuple([pg.typing.Int(), pg.typing.Str()]).noneable(),
-        'tuple[int, str] | None',
+        pg.typing.Tuple([Activity, pg.typing.Str()]), 'tuple[Any, str]',
+        allowed_dependencies=set(),
+    )
+    self.assert_annotation(
+        pg.typing.Tuple([Activity, pg.typing.Str()]).noneable(),
+        'tuple[Activity, str] | None',
     )
 
     # Dict.
     self.assert_annotation(
-        pg.typing.Dict({'x': int, 'y': str}), '{\'x\': int, \'y\': str}'
+        pg.typing.Dict({'x': Activity, 'y': str}),
+        '{\'x\': Activity, \'y\': str}'
+    )
+    self.assert_annotation(
+        pg.typing.Dict({'x': Activity, 'y': str}),
+        '{\'x\': Activity, \'y\': str}',
+        allowed_dependencies=set([Activity]),
+    )
+    self.assert_annotation(
+        pg.typing.Dict({'x': Activity, 'y': str}),
+        '{\'x\': Any, \'y\': str}',
+        allowed_dependencies=set(),
     )
     self.assert_annotation(
         pg.typing.Dict({'x': int, 'y': str}),
         'pg.typing.Dict({\'x\': int, \'y\': str})',
         strict=True,
     )
     self.assert_annotation(
@@ -416,38 +452,47 @@
     # Union.
     self.assert_annotation(
         pg.typing.Union(
             [pg.typing.Object(Activity), pg.typing.Object(Itinerary)]
         ).noneable(),
         'Union[Activity, Itinerary, None]',
     )
+    self.assert_annotation(
+        pg.typing.Union(
+            [pg.typing.Object(Activity), pg.typing.Object(Itinerary)]
+        ).noneable(),
+        'Union[Activity, Any, None]',
+        allowed_dependencies=set([Activity]),
+    )
 
     # Any.
     self.assert_annotation(pg.typing.Any(), 'Any')
     self.assert_annotation(pg.typing.Any().noneable(), 'Any')
 
   def test_class_definition(self):
     self.assertEqual(
-        schema_lib.class_definition(Activity),
+        schema_lib.class_definition(Activity, allowed_dependencies=set()),
         'class Activity:\n  description: str\n',
     )
     self.assertEqual(
         schema_lib.class_definition(Itinerary),
         inspect.cleandoc("""
-            class Itinerary:
+            class Itinerary(Object):
               \"\"\"A travel itinerary for a day.\"\"\"
               day: int(min=1)
               type: Literal['daytime', 'nighttime']
               activities: list[Activity]
               # Hotel to stay if applicable.
               hotel: str(regex='.*Hotel') | None
             """) + '\n',
     )
     self.assertEqual(
-        schema_lib.class_definition(PlaceOfInterest),
+        schema_lib.class_definition(
+            PlaceOfInterest, allowed_dependencies=set()
+        ),
         inspect.cleandoc("""
             class PlaceOfInterest:
               \"\"\"The name of a place of interest.
 
               A place of interest is a place that people ususally visit during their
               travels.
               \"\"\"
@@ -455,38 +500,41 @@
             """) + '\n',
     )
 
     class A(pg.Object):
       pass
 
     self.assertEqual(
-        schema_lib.class_definition(A),
+        schema_lib.class_definition(A, allowed_dependencies=set()),
         'class A:\n  pass\n',
     )
     self.assertEqual(
-        schema_lib.class_definition(A, include_pg_object_as_base=True),
+        schema_lib.class_definition(A),
         'class A(Object):\n  pass\n',
     )
 
     class C(pg.Object):
       x: str
       __kwargs__: typing.Any
 
-    self.assertEqual(schema_lib.class_definition(C), 'class C:\n  x: str\n')
+    self.assertEqual(
+        schema_lib.class_definition(C), 'class C(Object):\n  x: str\n'
+    )
 
     class D(pg.Object):
       x: str
+      @schema_lib.include_method_in_prompt
       def __call__(self, y: int) -> int:
         return len(self.x) + y
 
     self.assertEqual(
-        schema_lib.class_definition(D, include_methods=True),
+        schema_lib.class_definition(D),
         inspect.cleandoc(
             """
-            class D:
+            class D(Object):
               x: str
 
               def __call__(self, y: int) -> int:
                 return len(self.x) + y
             """) + '\n'
     )
 
@@ -502,54 +550,54 @@
     @dataclasses.dataclass(frozen=True)
     class Baz(Bar):  # pylint: disable=unused-variable
       pass
 
     class A(pg.Object):
       foo: Foo
 
+      @schema_lib.include_method_in_prompt
       def foo_value(self) -> int:
         return self.foo.x
 
+      def baz_value(self) -> str:
+        return 'baz'
+
     class B(A):
       bar: Bar
       foo2: Foo
 
+      @schema_lib.include_method_in_prompt
       def bar_value(self) -> str:
         return self.bar.y
 
     schema = schema_lib.Schema([B])
     self.assertEqual(
-        schema_lib.SchemaPythonRepr().class_definitions(
-            schema, include_methods=True
-        ),
+        schema_lib.SchemaPythonRepr().class_definitions(schema),
         inspect.cleandoc('''
             class Foo:
               x: int
 
-            class A:
-              foo: Foo
-
-              def foo_value(self) -> int:
-                return self.foo.x
-
             class Bar:
               """Class Bar."""
               y: str
 
             class Baz(Bar):
               """Baz(y: str)"""
               y: str
 
-            class B(A):
+            class B:
               foo: Foo
               bar: Bar
               foo2: Foo
 
               def bar_value(self) -> str:
                 return self.bar.y
+
+              def foo_value(self) -> int:
+                return self.foo.x
             ''') + '\n',
     )
 
     self.assertEqual(
         schema_lib.SchemaPythonRepr().result_definition(schema), 'list[B]'
     )
 
@@ -558,58 +606,63 @@
         inspect.cleandoc('''
             list[B]
 
             ```python
             class Foo:
               x: int
 
-            class A:
-              foo: Foo
-
             class Bar:
               """Class Bar."""
               y: str
 
             class Baz(Bar):
               """Baz(y: str)"""
               y: str
 
-            class B(A):
+            class B:
               foo: Foo
               bar: Bar
               foo2: Foo
+
+              def bar_value(self) -> str:
+                return self.bar.y
+
+              def foo_value(self) -> int:
+                return self.foo.x
             ```
             '''),
     )
     self.assertEqual(
         schema_lib.SchemaPythonRepr().repr(
             schema,
             include_result_definition=False,
-            include_pg_object_as_base=True,
             markdown=False,
         ),
         inspect.cleandoc('''
-            class Foo(Object):
+            class Foo:
               x: int
 
-            class A(Object):
-              foo: Foo
-
             class Bar:
               """Class Bar."""
               y: str
 
             class Baz(Bar):
               """Baz(y: str)"""
               y: str
 
-            class B(A):
+            class B:
               foo: Foo
               bar: Bar
               foo2: Foo
+
+              def bar_value(self) -> str:
+                return self.bar.y
+
+              def foo_value(self) -> int:
+                return self.foo.x
             '''),
     )
 
 
 class SchemaJsonReprTest(unittest.TestCase):
 
   def test_repr(self):
@@ -649,15 +702,15 @@
     )
     self.assertEqual(
         schema_lib.ValuePythonRepr().repr(A),
         inspect.cleandoc("""
             ```python
             class Foo(Object):
               x: int
-            
+
             class A(Object):
               foo: list[Foo]
               y: str | None
             ```
             """),
     )
     self.assertEqual(schema_lib.source_form(int), 'int')
```

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240531/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/subscription.py` & `langfun-0.0.2.dev20240531/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240531/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/template.py` & `langfun-0.0.2.dev20240531/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/template_test.py` & `langfun-0.0.2.dev20240531/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240531/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240531/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240531/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240531/langfun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240530
+Version: 0.0.2.dev20240531
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240530/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240531/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240530/setup.py` & `langfun-0.0.2.dev20240531/setup.py`

 * *Files identical despite different names*

