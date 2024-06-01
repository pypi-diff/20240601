# Comparing `tmp/FLUTE-LLM-0.1.4.tar.gz` & `tmp/FLUTE-LLM-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLUTE-LLM-0.1.4.tar", last modified: Thu May 30 11:52:40 2024, max compression
+gzip compressed data, was "FLUTE-LLM-0.1.5.tar", last modified: Sat Jun  1 13:12:12 2024, max compression
```

## Comparing `FLUTE-LLM-0.1.4.tar` & `FLUTE-LLM-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 11:52:40.990638 FLUTE-LLM-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-05-30 11:52:40.958278 FLUTE-LLM-0.1.4/FLUTE_LLM.egg-info/
--rw-rw-rw-   0        0        0     4111 2024-05-30 11:52:40.000000 FLUTE-LLM-0.1.4/FLUTE_LLM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2024-05-30 11:52:40.000000 FLUTE-LLM-0.1.4/FLUTE_LLM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 11:52:40.000000 FLUTE-LLM-0.1.4/FLUTE_LLM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-30 11:52:40.000000 FLUTE-LLM-0.1.4/FLUTE_LLM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-30 11:52:40.000000 FLUTE-LLM-0.1.4/FLUTE_LLM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 FLUTE-LLM-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4111 2024-05-30 11:52:40.989442 FLUTE-LLM-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3704 2024-05-30 11:50:55.000000 FLUTE-LLM-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 11:52:40.958784 FLUTE-LLM-0.1.4/flute/
-drwxrwxrwx   0        0        0        0 2024-05-30 11:52:40.966186 FLUTE-LLM-0.1.4/flute/Modules/
--rw-rw-rw-   0        0        0     2606 2024-05-28 13:00:12.000000 FLUTE-LLM-0.1.4/flute/Modules/AbstractPromptProcessor.py
--rw-rw-rw-   0        0        0     2478 2024-05-30 11:46:57.000000 FLUTE-LLM-0.1.4/flute/Modules/ClaudePromptProcessor.py
--rw-rw-rw-   0        0        0     3020 2024-05-30 11:47:07.000000 FLUTE-LLM-0.1.4/flute/Modules/GPTPromptProcessor.py
--rw-rw-rw-   0        0        0     3690 2024-05-30 11:46:55.000000 FLUTE-LLM-0.1.4/flute/Modules/GeminiPromptProcessor.py
--rw-rw-rw-   0        0        0     1894 2024-05-30 11:45:52.000000 FLUTE-LLM-0.1.4/flute/Modules/PromptProcessorFactory.py
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.4/flute/Modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:52:40.979535 FLUTE-LLM-0.1.4/flute/Modules/__pycache__/
--rw-rw-rw-   0        0        0     4286 2024-05-28 13:00:25.000000 FLUTE-LLM-0.1.4/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4188 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.4/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4912 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.4/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4565 2024-05-28 13:29:45.000000 FLUTE-LLM-0.1.4/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     2263 2024-05-30 11:47:26.000000 FLUTE-LLM-0.1.4/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc
--rw-rw-rw-   0        0        0      178 2024-05-28 11:35:01.000000 FLUTE-LLM-0.1.4/flute/Modules/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 11:52:40.981312 FLUTE-LLM-0.1.4/flute/Test/
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.4/flute/Test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:52:40.984776 FLUTE-LLM-0.1.4/flute/Test/__pycache__/
--rw-rw-rw-   0        0        0      175 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.4/flute/Test/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    14769 2024-05-30 11:03:19.000000 FLUTE-LLM-0.1.4/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc
--rw-rw-rw-   0        0        0     2786 2024-05-30 11:03:01.000000 FLUTE-LLM-0.1.4/flute/Test/test_prompt_processors.py
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.4/flute/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:52:40.986590 FLUTE-LLM-0.1.4/flute/__pycache__/
--rw-rw-rw-   0        0        0      170 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.4/flute/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       42 2024-05-30 11:52:40.990638 FLUTE-LLM-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      842 2024-05-30 11:51:16.000000 FLUTE-LLM-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:12:12.028775 FLUTE-LLM-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-06-01 13:12:11.955573 FLUTE-LLM-0.1.5/FLUTE_LLM.egg-info/
+-rw-rw-rw-   0        0        0     4470 2024-06-01 13:12:11.000000 FLUTE-LLM-0.1.5/FLUTE_LLM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2024-06-01 13:12:11.000000 FLUTE-LLM-0.1.5/FLUTE_LLM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:12:11.000000 FLUTE-LLM-0.1.5/FLUTE_LLM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-06-01 13:12:11.000000 FLUTE-LLM-0.1.5/FLUTE_LLM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-01 13:12:11.000000 FLUTE-LLM-0.1.5/FLUTE_LLM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 FLUTE-LLM-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4470 2024-06-01 13:12:12.027768 FLUTE-LLM-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4063 2024-06-01 13:03:27.000000 FLUTE-LLM-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:12:11.957220 FLUTE-LLM-0.1.5/flute/
+drwxrwxrwx   0        0        0        0 2024-06-01 13:12:12.003650 FLUTE-LLM-0.1.5/flute/Modules/
+-rw-rw-rw-   0        0        0     2606 2024-05-28 13:00:12.000000 FLUTE-LLM-0.1.5/flute/Modules/AbstractPromptProcessor.py
+-rw-rw-rw-   0        0        0     2478 2024-05-30 11:46:57.000000 FLUTE-LLM-0.1.5/flute/Modules/ClaudePromptProcessor.py
+-rw-rw-rw-   0        0        0     3020 2024-05-30 11:47:07.000000 FLUTE-LLM-0.1.5/flute/Modules/GPTPromptProcessor.py
+-rw-rw-rw-   0        0        0     3690 2024-05-30 11:46:55.000000 FLUTE-LLM-0.1.5/flute/Modules/GeminiPromptProcessor.py
+-rw-rw-rw-   0        0        0     2042 2024-06-01 12:42:05.000000 FLUTE-LLM-0.1.5/flute/Modules/PromptProcessorFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.5/flute/Modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:12:12.018336 FLUTE-LLM-0.1.5/flute/Modules/__pycache__/
+-rw-rw-rw-   0        0        0     4286 2024-05-28 13:00:25.000000 FLUTE-LLM-0.1.5/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4188 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.5/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4912 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.5/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4565 2024-05-28 13:29:45.000000 FLUTE-LLM-0.1.5/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2350 2024-06-01 13:10:23.000000 FLUTE-LLM-0.1.5/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc
+-rw-rw-rw-   0        0        0      178 2024-05-28 11:35:01.000000 FLUTE-LLM-0.1.5/flute/Modules/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-06-01 13:12:12.021280 FLUTE-LLM-0.1.5/flute/Test/
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.5/flute/Test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:12:12.024279 FLUTE-LLM-0.1.5/flute/Test/__pycache__/
+-rw-rw-rw-   0        0        0      175 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.5/flute/Test/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14794 2024-06-01 13:10:23.000000 FLUTE-LLM-0.1.5/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc
+-rw-rw-rw-   0        0        0     2779 2024-06-01 13:06:04.000000 FLUTE-LLM-0.1.5/flute/Test/test_prompt_processors.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.5/flute/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:12:12.026765 FLUTE-LLM-0.1.5/flute/__pycache__/
+-rw-rw-rw-   0        0        0      170 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.5/flute/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       42 2024-06-01 13:12:12.028775 FLUTE-LLM-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      842 2024-06-01 13:10:35.000000 FLUTE-LLM-0.1.5/setup.py
```

### Comparing `FLUTE-LLM-0.1.4/FLUTE_LLM.egg-info/PKG-INFO` & `FLUTE-LLM-0.1.5/FLUTE_LLM.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUTE-LLM
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for prompt processing and language model interaction
 Home-page: https://github.com/thepioneerjp/FLUTE
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -94,14 +94,22 @@
     class PromptProcessorFactory {
         +create_prompt_processor(model_name: str, api_key: Optional[str]) AbstractPromptProcessor
     }
 ```
 
 The class diagram shows the inheritance relationship between the abstract base class `AbstractPromptProcessor` and its concrete implementations `ClaudePromptProcessor`, `GPTPromptProcessor`, and `GeminiPromptProcessor`. The `PromptProcessorFactory` class is responsible for creating instances of the appropriate prompt processor based on the provided model name.
 
+### Supported models
+Those listed in [PromptProcessorFactory.py](/flute/Modules/PromptProcessorFactory.py) are currently supported.
+
+In brief, they consist of:
+- GPT-4 models (GPT-4, GPT-4-turbo, GPT-4o and most of their different versions)
+- Claude 3 models (Haiku, Sonnet, and Opus)
+- Gemini models(1.0 Pro, 1.0 Pro-vision, 1.5 Flash, and 1.5 Pro)
+
 # LICENSE
 The repository is licensed under the latest version of Modular and Inclusive Software Advancement License Classic (MISA-CLASSIC License).
 
 There are 4 main policies that consist of this license.
 1. Disclaimer of Liability
 2. Naming Continuity Obligation
 3. Waiver of Other Copyrights
```

### Comparing `FLUTE-LLM-0.1.4/FLUTE_LLM.egg-info/SOURCES.txt` & `FLUTE-LLM-0.1.5/FLUTE_LLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/LICENSE` & `FLUTE-LLM-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/PKG-INFO` & `FLUTE-LLM-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUTE-LLM
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for prompt processing and language model interaction
 Home-page: https://github.com/thepioneerjp/FLUTE
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -94,14 +94,22 @@
     class PromptProcessorFactory {
         +create_prompt_processor(model_name: str, api_key: Optional[str]) AbstractPromptProcessor
     }
 ```
 
 The class diagram shows the inheritance relationship between the abstract base class `AbstractPromptProcessor` and its concrete implementations `ClaudePromptProcessor`, `GPTPromptProcessor`, and `GeminiPromptProcessor`. The `PromptProcessorFactory` class is responsible for creating instances of the appropriate prompt processor based on the provided model name.
 
+### Supported models
+Those listed in [PromptProcessorFactory.py](/flute/Modules/PromptProcessorFactory.py) are currently supported.
+
+In brief, they consist of:
+- GPT-4 models (GPT-4, GPT-4-turbo, GPT-4o and most of their different versions)
+- Claude 3 models (Haiku, Sonnet, and Opus)
+- Gemini models(1.0 Pro, 1.0 Pro-vision, 1.5 Flash, and 1.5 Pro)
+
 # LICENSE
 The repository is licensed under the latest version of Modular and Inclusive Software Advancement License Classic (MISA-CLASSIC License).
 
 There are 4 main policies that consist of this license.
 1. Disclaimer of Liability
 2. Naming Continuity Obligation
 3. Waiver of Other Copyrights
```

### Comparing `FLUTE-LLM-0.1.4/README.md` & `FLUTE-LLM-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,22 @@
     class PromptProcessorFactory {
         +create_prompt_processor(model_name: str, api_key: Optional[str]) AbstractPromptProcessor
     }
 ```
 
 The class diagram shows the inheritance relationship between the abstract base class `AbstractPromptProcessor` and its concrete implementations `ClaudePromptProcessor`, `GPTPromptProcessor`, and `GeminiPromptProcessor`. The `PromptProcessorFactory` class is responsible for creating instances of the appropriate prompt processor based on the provided model name.
 
+### Supported models
+Those listed in [PromptProcessorFactory.py](/flute/Modules/PromptProcessorFactory.py) are currently supported.
+
+In brief, they consist of:
+- GPT-4 models (GPT-4, GPT-4-turbo, GPT-4o and most of their different versions)
+- Claude 3 models (Haiku, Sonnet, and Opus)
+- Gemini models(1.0 Pro, 1.0 Pro-vision, 1.5 Flash, and 1.5 Pro)
+
 # LICENSE
 The repository is licensed under the latest version of Modular and Inclusive Software Advancement License Classic (MISA-CLASSIC License).
 
 There are 4 main policies that consist of this license.
 1. Disclaimer of Liability
 2. Naming Continuity Obligation
 3. Waiver of Other Copyrights
```

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/AbstractPromptProcessor.py` & `FLUTE-LLM-0.1.5/flute/Modules/AbstractPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/ClaudePromptProcessor.py` & `FLUTE-LLM-0.1.5/flute/Modules/ClaudePromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/GPTPromptProcessor.py` & `FLUTE-LLM-0.1.5/flute/Modules/GPTPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/GeminiPromptProcessor.py` & `FLUTE-LLM-0.1.5/flute/Modules/GeminiPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/PromptProcessorFactory.py` & `FLUTE-LLM-0.1.5/flute/Modules/PromptProcessorFactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,17 +37,21 @@
             "gpt-4-0613",
             "gpt-4-32k",
             "gpt-4-32k-0613",
         ]:
             api_key = os.getenv("OPENAI_API_KEY")
             return GPTPromptProcessor(api_key=api_key)
         elif model_name in [
+            "gemini-1.5-pro-latest", 
+            "gemini-1.5-flash-latest",
+            "gemini-1.0-pro",
+            "gemini-pro-vision",
             "models/gemini-1.5-pro-latest", 
             "models/gemini-1.5-flash-latest",
-            "models/gemini-pro",
+            "models/gemini-1.0-pro",
             "models/gemini-pro-vision",
         ]:
             api_key = os.getenv("GOOGLE_API_KEY")
             return GeminiPromptProcessor(api_key=api_key, model=model_name)
         ## TODO: Groq, Local LLMs, Brain Computer Interface, etc...
         else:
             return None
```

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.5/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.5/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.5/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.5/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.4/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc` & `FLUTE-LLM-0.1.5/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf0665866 (Thu May 30 11:45:52 2024 UTC)
-files sz: 1894
+moddate:  0x1d175b66 (Sat Jun  1 12:42:05 2024 UTC)
+files sz: 2042
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -186,53 +186,53 @@
                            176 LOAD_FAST                1 (api_key)
                            178 KW_NAMES                 6
                            180 PRECALL                  1
                            184 CALL                     1
                            194 RETURN_VALUE
                
                 43     >>  196 LOAD_FAST                0 (model_name)
-                           198 LOAD_CONST               7 (('models/gemini-1.5-pro-latest', 'models/gemini-1.5-flash-latest', 'models/gemini-pro', 'models/gemini-pro-vision'))
+                           198 LOAD_CONST               7 (('gemini-1.5-pro-latest', 'gemini-1.5-flash-latest', 'gemini-1.0-pro', 'gemini-pro-vision', 'models/gemini-1.5-pro-latest', 'models/gemini-1.5-flash-latest', 'models/gemini-1.0-pro', 'models/gemini-pro-vision'))
                            200 CONTAINS_OP              0
                            202 POP_JUMP_FORWARD_IF_FALSE    37 (to 278)
                
-                49         204 LOAD_GLOBAL              3 (NULL + os)
+                53         204 LOAD_GLOBAL              3 (NULL + os)
                            216 LOAD_ATTR                2 (getenv)
                            226 LOAD_CONST               8 ('GOOGLE_API_KEY')
                            228 PRECALL                  1
                            232 CALL                     1
                            242 STORE_FAST               1 (api_key)
                
-                50         244 LOAD_GLOBAL             11 (NULL + GeminiPromptProcessor)
+                54         244 LOAD_GLOBAL             11 (NULL + GeminiPromptProcessor)
                            256 LOAD_FAST                1 (api_key)
                            258 LOAD_FAST                0 (model_name)
                            260 KW_NAMES                 3
                            262 PRECALL                  2
                            266 CALL                     2
                            276 RETURN_VALUE
                
-                53     >>  278 LOAD_CONST               0 (None)
+                57     >>  278 LOAD_CONST               0 (None)
                            280 RETURN_VALUE
                consts
                   None
                   ('claude-3-opus-20240229', 'claude-3-sonnet-20240229', 'claude-3-haiku-20240307')
                   'ANTHROPIC_API_KEY'
                   ('api_key', 'model')
                   ('gpt-4o', 'gpt-4o-2024-05-13', 'gpt-4-turbo', 'gpt-4-turbo-2024-04-09', 'gpt-4-turbo-preview', 'gpt-4-0125-preview', 'gpt-4-1106-preview', 'gpt-4-vision-preview', 'gpt-4-1106-vision-preview', 'gpt-4', 'gpt-4-0613', 'gpt-4-32k', 'gpt-4-32k-0613')
                   'OPENAI_API_KEY'
                   ('api_key',)
-                  ('models/gemini-1.5-pro-latest', 'models/gemini-1.5-flash-latest', 'models/gemini-pro', 'models/gemini-pro-vision')
+                  ('gemini-1.5-pro-latest', 'gemini-1.5-flash-latest', 'gemini-1.0-pro', 'gemini-pro-vision', 'models/gemini-1.5-pro-latest', 'models/gemini-1.5-flash-latest', 'models/gemini-1.0-pro', 'models/gemini-pro-vision')
                   'GOOGLE_API_KEY'
                names      ('load_dotenv', 'os', 'getenv', 'ClaudePromptProcessor', 'GPTPromptProcessor', 'GeminiPromptProcessor')
                varnames   ('model_name', 'api_key')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\j_matsumoto\\Documents\\GitHub\\FLUTE\\flute\\Test\\..\\Modules\\PromptProcessorFactory.py'
                name       'create_prompt_processor'
                firstlineno 14
-               lnotab 0x020204011c02080528012201080f28012001080628012203
+               lnotab 0x020204011c02080528012201080f28012001080a28012203
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'str', 'Optional', 'create_prompt_processor')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\j_matsumoto\\Documents\\GitHub\\FLUTE\\flute\\Test\\..\\Modules\\PromptProcessorFactory.py'
          name       'PromptProcessorFactory'
```

### Comparing `FLUTE-LLM-0.1.4/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc` & `FLUTE-LLM-0.1.5/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe55c5866 (Thu May 30 11:03:01 2024 UTC)
-files sz: 2786
+moddate:  0xbc1c5b66 (Sat Jun  1 13:06:04 2024 UTC)
+files sz: 2779
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a01640064016c026d03630201006d045a05010064
@@ -1616,85 +1616,85 @@
          argcount  : 0
          nlocals   : 9
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000006401a60100
             00ab0100000000000000007d007c006a0200000000000000007d017c016a
-            0300000000000000007d0264017d037c027c036b02000000007d047c0473
-            bd7409000000000000000000006a05000000000000000064027c04660164
-            037c027c036602a6040000ab0400000000000000006404740d0000000000
+            0300000000000000007d0264027d037c027c036b02000000007d047c0473
+            bd7409000000000000000000006a05000000000000000064037c04660164
+            047c027c036602a6040000ab0400000000000000006405740d0000000000
             00000000006a070000000000000000a6000000ab00000000000000000076
             0073147409000000000000000000006a0800000000000000007c00a60100
             00ab01000000000000000072147409000000000000000000006a09000000
-            00000000007c00a6010000ab0100000000000000006e0164047409000000
+            00000000007c00a6010000ab0100000000000000006e0164057409000000
             000000000000006a0900000000000000007c01a6010000ab010000000000
             0000007409000000000000000000006a0900000000000000007c02a60100
             00ab0100000000000000007409000000000000000000006a090000000000
-            0000007c03a6010000ab01000000000000000064059c047a0600007d0564
-            0664077c0569017a0600007d067415000000000000000000007409000000
+            0000007c03a6010000ab01000000000000000064069c047a0600007d0564
+            0764087c0569017a0600007d067415000000000000000000007409000000
             000000000000006a0b00000000000000007c06a6010000ab010000000000
             000000a6010000ab0100000000000000008201640078017d0178017d0278
             017d047d037c00a00c000000000000000000000000000000000000000064
-            086409640a640b640cac0da6050000ab0500000000000000007d07741b00
+            09640a640b640c640dac0ea6050000ab0500000000000000007d07741b00
             0000000000000000007c07741c00000000000000000000a6020000ab0200
-            000000000000007d027c0290017308640e640f740d000000000000000000
+            000000000000007d027c0290017308640f6410740d000000000000000000
             006a070000000000000000a6000000ab0000000000000000007600731974
             09000000000000000000006a080000000000000000741a00000000000000
             000000a6010000ab01000000000000000072197409000000000000000000
             006a090000000000000000741a00000000000000000000a6010000ab0100
-            000000000000006e01640f6410740d000000000000000000006a07000000
+            000000000000006e0164106411740d000000000000000000006a07000000
             0000000000a6000000ab0000000000000000007600731474090000000000
             00000000006a0800000000000000007c07a6010000ab0100000000000000
             0072147409000000000000000000006a0900000000000000007c07a60100
-            00ab0100000000000000006e0164106411740d000000000000000000006a
+            00ab0100000000000000006e0164116412740d000000000000000000006a
             070000000000000000a6000000ab00000000000000000076007319740900
             0000000000000000006a080000000000000000741c000000000000000000
             00a6010000ab01000000000000000072197409000000000000000000006a
             090000000000000000741c00000000000000000000a6010000ab01000000
-            00000000006e0164117409000000000000000000006a0900000000000000
-            007c02a6010000ab01000000000000000064129c047a0600007d08741500
+            00000000006e0164127409000000000000000000006a0900000000000000
+            007c02a6010000ab01000000000000000064139c047a0600007d08741500
             0000000000000000007409000000000000000000006a0b00000000000000
             007c08a6010000ab010000000000000000a6010000ab0100000000000000
             00820164007d0264005300
           53           0 RESUME                   0
          
           54           2 LOAD_GLOBAL              1 (NULL + PromptProcessorFactory)
                       14 LOAD_ATTR                1 (create_prompt_processor)
-                      24 LOAD_CONST               1 ('models/gemini-1.5-flash-latest')
+                      24 LOAD_CONST               1 ('gemini-1.5-flash-latest')
                       26 PRECALL                  1
                       30 CALL                     1
                       40 STORE_FAST               0 (processor)
          
           55          42 LOAD_FAST                0 (processor)
                       44 LOAD_ATTR                2 (model)
                       54 STORE_FAST               1 (@py_assert1)
                       56 LOAD_FAST                1 (@py_assert1)
                       58 LOAD_ATTR                3 (model_name)
                       68 STORE_FAST               2 (@py_assert3)
-                      70 LOAD_CONST               1 ('models/gemini-1.5-flash-latest')
+                      70 LOAD_CONST               2 ('models/gemini-1.5-flash-latest')
                       72 STORE_FAST               3 (@py_assert6)
                       74 LOAD_FAST                2 (@py_assert3)
                       76 LOAD_FAST                3 (@py_assert6)
                       78 COMPARE_OP               2 (==)
                       84 STORE_FAST               4 (@py_assert5)
                       86 LOAD_FAST                4 (@py_assert5)
                       88 POP_JUMP_FORWARD_IF_TRUE   189 (to 468)
                       90 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      102 LOAD_ATTR                5 (_call_reprcompare)
-                     112 LOAD_CONST               2 (('==',))
+                     112 LOAD_CONST               3 (('==',))
                      114 LOAD_FAST                4 (@py_assert5)
                      116 BUILD_TUPLE              1
-                     118 LOAD_CONST               3 (('%(py4)s\n{%(py4)s = %(py2)s\n{%(py2)s = %(py0)s.model\n}.model_name\n} == %(py7)s',))
+                     118 LOAD_CONST               4 (('%(py4)s\n{%(py4)s = %(py2)s\n{%(py2)s = %(py0)s.model\n}.model_name\n} == %(py7)s',))
                      120 LOAD_FAST                2 (@py_assert3)
                      122 LOAD_FAST                3 (@py_assert6)
                      124 BUILD_TUPLE              2
                      126 PRECALL                  4
                      130 CALL                     4
-                     140 LOAD_CONST               4 ('processor')
+                     140 LOAD_CONST               5 ('processor')
                      142 LOAD_GLOBAL             13 (NULL + @py_builtins)
                      154 LOAD_ATTR                7 (locals)
                      164 PRECALL                  0
                      168 CALL                     0
                      178 CONTAINS_OP              0
                      180 POP_JUMP_FORWARD_IF_TRUE    20 (to 222)
                      182 LOAD_GLOBAL              9 (NULL + @pytest_ar)
@@ -1705,15 +1705,15 @@
                      220 POP_JUMP_FORWARD_IF_FALSE    20 (to 262)
                  >>  222 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      234 LOAD_ATTR                9 (_saferepr)
                      244 LOAD_FAST                0 (processor)
                      246 PRECALL                  1
                      250 CALL                     1
                      260 JUMP_FORWARD             1 (to 264)
-                 >>  262 LOAD_CONST               4 ('processor')
+                 >>  262 LOAD_CONST               5 ('processor')
                  >>  264 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      276 LOAD_ATTR                9 (_saferepr)
                      286 LOAD_FAST                1 (@py_assert1)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      314 LOAD_ATTR                9 (_saferepr)
@@ -1721,20 +1721,20 @@
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      352 LOAD_ATTR                9 (_saferepr)
                      362 LOAD_FAST                3 (@py_assert6)
                      364 PRECALL                  1
                      368 CALL                     1
-                     378 LOAD_CONST               5 (('py0', 'py2', 'py4', 'py7'))
+                     378 LOAD_CONST               6 (('py0', 'py2', 'py4', 'py7'))
                      380 BUILD_CONST_KEY_MAP      4
                      382 BINARY_OP                6 (%)
                      386 STORE_FAST               5 (@py_format8)
-                     388 LOAD_CONST               6 ('assert %(py9)s')
-                     390 LOAD_CONST               7 ('py9')
+                     388 LOAD_CONST               7 ('assert %(py9)s')
+                     390 LOAD_CONST               8 ('py9')
                      392 LOAD_FAST                5 (@py_format8)
                      394 BUILD_MAP                1
                      396 BINARY_OP                6 (%)
                      400 STORE_FAST               6 (@py_format10)
                      402 LOAD_GLOBAL             21 (NULL + AssertionError)
                      414 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      426 LOAD_ATTR               11 (_format_explanation)
@@ -1751,35 +1751,35 @@
                      476 STORE_FAST               2 (@py_assert3)
                      478 COPY                     1
                      480 STORE_FAST               4 (@py_assert5)
                      482 STORE_FAST               3 (@py_assert6)
          
           57         484 LOAD_FAST                0 (processor)
                      486 LOAD_METHOD             12 (generate_response)
-                     508 LOAD_CONST               8 ('Hello, how are you?')
-                     510 LOAD_CONST               9 (4096)
-                     512 LOAD_CONST              10 (1.0)
-                     514 LOAD_CONST              11 (1)
-                     516 LOAD_CONST              12 ('You are an assistant')
-                     518 KW_NAMES                13
+                     508 LOAD_CONST               9 ('Hello, how are you?')
+                     510 LOAD_CONST              10 (4096)
+                     512 LOAD_CONST              11 (1.0)
+                     514 LOAD_CONST              12 (1)
+                     516 LOAD_CONST              13 ('You are an assistant')
+                     518 KW_NAMES                14
                      520 PRECALL                  5
                      524 CALL                     5
                      534 STORE_FAST               7 (response)
          
           58         536 LOAD_GLOBAL             27 (NULL + isinstance)
                      548 LOAD_FAST                7 (response)
                      550 LOAD_GLOBAL             28 (str)
                      562 PRECALL                  2
                      566 CALL                     2
                      576 STORE_FAST               2 (@py_assert3)
                      578 LOAD_FAST                2 (@py_assert3)
                      580 EXTENDED_ARG             1
                      582 POP_JUMP_FORWARD_IF_TRUE   264 (to 1112)
-                     584 LOAD_CONST              14 ('assert %(py4)s\n{%(py4)s = %(py0)s(%(py1)s, %(py2)s)\n}')
-                     586 LOAD_CONST              15 ('isinstance')
+                     584 LOAD_CONST              15 ('assert %(py4)s\n{%(py4)s = %(py0)s(%(py1)s, %(py2)s)\n}')
+                     586 LOAD_CONST              16 ('isinstance')
                      588 LOAD_GLOBAL             13 (NULL + @py_builtins)
                      600 LOAD_ATTR                7 (locals)
                      610 PRECALL                  0
                      614 CALL                     0
                      624 CONTAINS_OP              0
                      626 POP_JUMP_FORWARD_IF_TRUE    25 (to 678)
                      628 LOAD_GLOBAL              9 (NULL + @pytest_ar)
@@ -1790,16 +1790,16 @@
                      676 POP_JUMP_FORWARD_IF_FALSE    25 (to 728)
                  >>  678 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      690 LOAD_ATTR                9 (_saferepr)
                      700 LOAD_GLOBAL             26 (isinstance)
                      712 PRECALL                  1
                      716 CALL                     1
                      726 JUMP_FORWARD             1 (to 730)
-                 >>  728 LOAD_CONST              15 ('isinstance')
-                 >>  730 LOAD_CONST              16 ('response')
+                 >>  728 LOAD_CONST              16 ('isinstance')
+                 >>  730 LOAD_CONST              17 ('response')
                      732 LOAD_GLOBAL             13 (NULL + @py_builtins)
                      744 LOAD_ATTR                7 (locals)
                      754 PRECALL                  0
                      758 CALL                     0
                      768 CONTAINS_OP              0
                      770 POP_JUMP_FORWARD_IF_TRUE    20 (to 812)
                      772 LOAD_GLOBAL              9 (NULL + @pytest_ar)
@@ -1810,16 +1810,16 @@
                      810 POP_JUMP_FORWARD_IF_FALSE    20 (to 852)
                  >>  812 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      824 LOAD_ATTR                9 (_saferepr)
                      834 LOAD_FAST                7 (response)
                      836 PRECALL                  1
                      840 CALL                     1
                      850 JUMP_FORWARD             1 (to 854)
-                 >>  852 LOAD_CONST              16 ('response')
-                 >>  854 LOAD_CONST              17 ('str')
+                 >>  852 LOAD_CONST              17 ('response')
+                 >>  854 LOAD_CONST              18 ('str')
                      856 LOAD_GLOBAL             13 (NULL + @py_builtins)
                      868 LOAD_ATTR                7 (locals)
                      878 PRECALL                  0
                      882 CALL                     0
                      892 CONTAINS_OP              0
                      894 POP_JUMP_FORWARD_IF_TRUE    25 (to 946)
                      896 LOAD_GLOBAL              9 (NULL + @pytest_ar)
@@ -1830,21 +1830,21 @@
                      944 POP_JUMP_FORWARD_IF_FALSE    25 (to 996)
                  >>  946 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                      958 LOAD_ATTR                9 (_saferepr)
                      968 LOAD_GLOBAL             28 (str)
                      980 PRECALL                  1
                      984 CALL                     1
                      994 JUMP_FORWARD             1 (to 998)
-                 >>  996 LOAD_CONST              17 ('str')
+                 >>  996 LOAD_CONST              18 ('str')
                  >>  998 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                     1010 LOAD_ATTR                9 (_saferepr)
                     1020 LOAD_FAST                2 (@py_assert3)
                     1022 PRECALL                  1
                     1026 CALL                     1
-                    1036 LOAD_CONST              18 (('py0', 'py1', 'py2', 'py4'))
+                    1036 LOAD_CONST              19 (('py0', 'py1', 'py2', 'py4'))
                     1038 BUILD_CONST_KEY_MAP      4
                     1040 BINARY_OP                6 (%)
                     1044 STORE_FAST               8 (@py_format5)
                     1046 LOAD_GLOBAL             21 (NULL + AssertionError)
                     1058 LOAD_GLOBAL              9 (NULL + @pytest_ar)
                     1070 LOAD_ATTR               11 (_format_explanation)
                     1080 LOAD_FAST                8 (@py_format5)
@@ -1855,14 +1855,15 @@
                     1110 RAISE_VARARGS            1
                  >> 1112 LOAD_CONST               0 (None)
                     1114 STORE_FAST               2 (@py_assert3)
                     1116 LOAD_CONST               0 (None)
                     1118 RETURN_VALUE
          consts
             None
+            'gemini-1.5-flash-latest'
             'models/gemini-1.5-flash-latest'
             ('==',)
             ('%(py4)s\n{%(py4)s = %(py2)s\n{%(py2)s = %(py0)s.model\n}.model_name\n} == %(py7)s',)
             'processor'
             ('py0', 'py2', 'py4', 'py7')
             'assert %(py9)s'
             'py9'
```

### Comparing `FLUTE-LLM-0.1.4/flute/Test/test_prompt_processors.py` & `FLUTE-LLM-0.1.5/flute/Test/test_prompt_processors.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,12 +47,12 @@
     assert processor.api_key == api_key
     assert processor.model.model_name == "models/gemini-1.5-flash-latest"
 
     response = processor.generate_response("Hello, how are you?", max_tokens=4096, temperature=1.0, top_p=1, system="You are an assistant")
     assert isinstance(response, str)
 
 def test_create_gemini_prompt_processor_without_api_key():
-    processor = PromptProcessorFactory.create_prompt_processor("models/gemini-1.5-flash-latest")
+    processor = PromptProcessorFactory.create_prompt_processor("gemini-1.5-flash-latest")
     assert processor.model.model_name == "models/gemini-1.5-flash-latest"
 
     response = processor.generate_response("Hello, how are you?", max_tokens=4096, temperature=1.0, top_p=1, system="You are an assistant")
     assert isinstance(response, str)
```

### Comparing `FLUTE-LLM-0.1.4/setup.py` & `FLUTE-LLM-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FLUTE-LLM',
-    version='0.1.4',
+    version='0.1.5',
     description='A package for prompt processing and language model interaction',
     author='The Pioneer',
     url='https://github.com/thepioneerjp/FLUTE',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

