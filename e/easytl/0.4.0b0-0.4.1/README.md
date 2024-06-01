# Comparing `tmp/easytl-0.4.0b0.tar.gz` & `tmp/easytl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.4.0b0.tar", last modified: Fri May 24 01:30:57 2024, max compression
+gzip compressed data, was "easytl-0.4.1.tar", last modified: Sat Jun  1 01:46:05 2024, max compression
```

## Comparing `easytl-0.4.0b0.tar` & `easytl-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.740841 easytl-0.4.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.740841 easytl-0.4.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-24 01:28:55.000000 easytl-0.4.0b0/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-24 01:28:55.000000 easytl-0.4.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-24 01:28:55.000000 easytl-0.4.0b0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-24 01:30:57.744840 easytl-0.4.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-24 01:28:55.000000 easytl-0.4.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-24 01:28:55.000000 easytl-0.4.0b0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-24 01:28:55.000000 easytl-0.4.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-24 01:28:55.000000 easytl-0.4.0b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:30:57.744840 easytl-0.4.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.740841 easytl-0.4.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.740841 easytl-0.4.0b0/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)   105332 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/src/easytl/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/anthropic_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/azure_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/googletl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/services/openai_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/src/easytl/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/util/llm_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-24 01:28:55.000000 easytl-0.4.0b0/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 01:30:57.000000 easytl-0.4.0b0/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:30:57.744840 easytl-0.4.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-24 01:28:55.000000 easytl-0.4.0b0/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    19390 2024-05-24 01:28:55.000000 easytl-0.4.0b0/tests/passing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-24 01:28:55.000000 easytl-0.4.0b0/tests/simple_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.833641 easytl-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.829641 easytl-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.829641 easytl-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-06-01 01:44:34.000000 easytl-0.4.1/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-06-01 01:44:34.000000 easytl-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-06-01 01:44:34.000000 easytl-0.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-06-01 01:46:05.833641 easytl-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-06-01 01:44:34.000000 easytl-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-06-01 01:44:34.000000 easytl-0.4.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-06-01 01:44:34.000000 easytl-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 01:44:34.000000 easytl-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:46:05.833641 easytl-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.829641 easytl-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.829641 easytl-0.4.1/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105910 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.833641 easytl-0.4.1/src/easytl/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/services/anthropic_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/services/azure_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/services/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/services/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/services/googletl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/services/openai_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.833641 easytl-0.4.1/src/easytl/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14635 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/util/llm_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-01 01:44:34.000000 easytl-0.4.1/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.833641 easytl-0.4.1/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-06-01 01:46:05.000000 easytl-0.4.1/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-06-01 01:46:05.000000 easytl-0.4.1/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:46:05.000000 easytl-0.4.1/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-01 01:46:05.000000 easytl-0.4.1/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 01:46:05.000000 easytl-0.4.1/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:05.833641 easytl-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-06-01 01:44:34.000000 easytl-0.4.1/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-06-01 01:44:34.000000 easytl-0.4.1/tests/passing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-06-01 01:44:34.000000 easytl-0.4.1/tests/simple_test.py
```

### Comparing `easytl-0.4.0b0/.github/workflows/workflow.yml` & `easytl-0.4.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0b0/.gitignore` & `easytl-0.4.1/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -166,9 +166,9 @@
 tests/deepl.txt
 tests/easytl-log.txt
 tests/google_translate_key.json
 tests/anthropic.txt
 tests/azure.txt
 tests/azure_region.txt
 
-# For MacOS
+## For MacOS
 .DS_Store
```

### Comparing `easytl-0.4.0b0/LICENSE.md` & `easytl-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0b0/PKG-INFO` & `easytl-0.4.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,39 @@
-Metadata-Version: 2.1
-Name: easytl
-Version: 0.4.0b0
-Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini, Google Translate and More.
-Author-email: "Kaden Bilyeu (Bikatr7)" <Bikatr7@proton.me>, Alejandro Mata <alemalvarez@icloud.com>
-Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
-Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: google-generativeai==0.5.4
-Requires-Dist: deepl==1.16.1
-Requires-Dist: openai==1.29.0
-Requires-Dist: backoff==2.2.1
-Requires-Dist: tiktoken==0.6.0
-Requires-Dist: google-cloud-translate==3.15.3
-Requires-Dist: anthropic==0.26.0
-Requires-Dist: requests>=2.31.0
-
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
-- [Quick Start](#quick-start)
-- [Installation](#installation)
-- [Features](#features)
-- [API Usage](#api-usage)
-- [License](#license)
-- [Contact](#contact)
-- [Contribution](#contribution)
-- [Notes](#notes)
+- [**Notes**](#notes)
+- [**Quick Start**](#quick-start)
+- [**Installation**](#installation)
+- [**Features**](#features)
+- [**API Usage**](#api-usage)
+  - [Translating Text](#translating-text)
+  - [Generic Translation Methods](#generic-translation-methods)
+  - [Cost Calculation](#cost-calculation)
+  - [Credentials Management](#credentials-management)
+- [**License**](#license)
+- [**Contact**](#contact)
+- [**Contribution**](#contribution)
+- [**Acknowledgements**](#acknowledgements)
 
----------------------------------------------------------------------------------------------------------------------------------------------------
+--------------------------------------------------------------------------------------------------------------------------------------------------
+
+## **Notes**<a name="notes"></a>
 
-## EasyTL
+Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini, Google Translate and More! 
 
-Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
+EasyTL has a [Trello board](https://trello.com/b/Td555CoW/easytl) for tracking planned features and issues:
 
-EasyTL has a Trello board for tracking planned features and issues:
-https://trello.com/b/Td555CoW/easytl
+We've compiled a repository of examples and use cases for EasyTL at this [GitHub repository](https://github.com/Bikatr7/easytl-demo)
+
+> [!TIP]
+> You can find the full documentation [here](https://easytl.readthedocs.io/en/latest/index.html)! (work in progress)
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
-**Quick Start**<a name="quick-start"></a>
+## **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
 ```
 
@@ -56,25 +41,49 @@
 
 For example, with DeepL:
 
 ```python
 from easytl import EasyTL
 
 ## Set your API key
-EasyTL.credentials("deepl", "your_api_key_here")
+EasyTL.set_credentials("deepl", "YOUR_API_KEY")
 
 ## You can also validate your API keys; translation functions will do this automatically
-is_valid, e = EasyTL.validate_credentials("deepl")
+is_valid, e = EasyTL.test_credentials("deepl")
 
 translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN-US") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality and other services.
+
+print(translated_text) ## Output: "I can speak Japanese"
+```
+
+or with OpenAI:
+
+```python
+from easytl import EasyTL
+
+import asyncio
+
+async def main():
+
+    ## Set your API key
+    EasyTL.set_credentials("openai", "YOUR_API_KEY")
+
+    ## Get's the raw response from the API, allowing you to access the full response object
+    raw_response = await EasyTL.openai_translate_async("I can speak Japanese", model="gpt-4o", translation_instructions="Translate this text to Japanese.", response_type="raw") 
+
+    print(raw_response.choices[0].message.content) ## Output: "私は日本語が話せます" or something similar
+
+if(__name__ == "__main__"):
+    asyncio.run(main())
+
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Installation**<a name="installation"></a>
+## **Installation**<a name="installation"></a>
 
 Python 3.10+
 
 EasyTL can be installed using pip:
 
 ```bash
 pip install easytl
@@ -84,96 +93,109 @@
 
 These are the dependencies/requirements that will be installed:
 ```bash
 setuptools>=61.0
 wheel
 setuptools_scm>=6.0
 tomli
-google-generativeai==0.5.1
+requests>=2.31.0
+google-generativeai==0.5.4
 deepl==1.16.1
-openai==1.13.3
+openai==1.29.0
 backoff==2.2.1
-tiktoken==0.6.0
+tiktoken==0.7.0
 google-cloud-translate==3.15.3
+anthropic==0.26.1
 ```
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Features**<a name="features"></a>
+## **Features**<a name="features"></a>
 
 EasyTL offers seamless integration with several translation APIs, allowing users to easily switch between services based on their needs. Key features include:
 
-- Support for multiple translation APIs including OpenAI, DeepL, Gemini, and Google Translate.
-- Simple API key and credential management.
-- Methods to validate credentials before usage.
+- Support for multiple translation APIs including OpenAI, DeepL, Gemini, Google Translate, Microsoft Azure Translate, and Anthropic.
+- Simple API key and credential management and validation.
 - Cost estimation tools to help manage usage based on text length, translation instructions for LLMs, and translation services.
-- Highly customizable translation options, with the API's original features.
+- Highly customizable translation options, with each API's original features and more. 
 - Lots of optional arguments for additional functionality. Such as decorators, semaphores, and rate-limit delays.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**API Usage**<a name="api-usage"></a>
+## **API Usage**<a name="api-usage"></a>
 
 ### Translating Text
 
-Use `deepl_translate`, `googletl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+Translate functions can be broken down into two categories: LLM and non-LLM. LLM ones can take instructions, while non-LLM ones require a target language. 
+
+`deepl_translate`, `googletl_translate`, and `azure_translate` are non-LLM functions, while `openai_translate`, `gemini_translate`, and `anthropic_translate` are LLM functions.
+
+Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature. However these vary wildly between services, so it is recommended to check the documentation for each service for more information.
 
 All services offer asynchronous translation methods that return a future object for concurrent processing. These methods are suffixed with `_async` and can be awaited to retrieve the translated text.
 
-Instead of receiving the translated text directly, you can also use the `response` parameter to get the full response object from the API.
+Instead of receiving the translated text directly, you can also use the `response_type` parameter to get the raw response object, specify a json response where available, or both.
+  
+  `text` - Default. Returns the translated text.
+
+  `json` - Returns the response as a JSON object. Not all services support this.
+
+  `raw` - Returns the raw response object from the API. This can be useful for accessing additional information or debugging.
+  
+  `raw_json` - Returns the raw response object with the text but with the response also a json object. Again, not all services support this.
 
-## Generic Translation Methods
+### Generic Translation Methods
 
 EasyTL has generic translation methods `translate` and `translate_async` that can be used to translate text with any of the supported services. These methods accept the text, service, and kwargs of the respective service as parameters.
 
 ### Cost Calculation
 
 The `calculate_cost` method provides an estimate of the cost associated with translating a given text with specified settings for each supported service.
 
-characters or tokens depending on the service.
+These are characters or tokens depending on the type of translate function used.
 
 ```python
 num_characters, cost, model = EasyTL.calculate_cost("This has a lot of characters", "deepl")
 ```
 
 or 
 
 ```python
 num_tokens, cost, model = EasyTL.calculate_cost("This has a lot of tokens.", "openai", model="gpt-4", translation_instructions="Translate this text to Japanese.")
 ```
 
 ### Credentials Management
 
-Credentials can be set and validated using `set_credentials` and `validate_credentials` methods to ensure they are active and correct before submitting translation requests.
+Credentials can be set and validated using `set_credentials` and `test_credentials` methods to ensure they are active and correct before submitting translation requests.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**License**<a name="license"></a>
+## **License**<a name="license"></a>
 
 This project, EasyTL, is licensed under the GNU Lesser General Public License v2.1 (LGPLv2.1) - see the LICENSE file for complete details.
 
 The LGPL is a permissive copyleft license that enables this software to be freely used, modified, and distributed. It is particularly designed for libraries, allowing them to be included in both open source and proprietary software. When using or modifying EasyTL, you can choose to release your work under the LGPLv2.1 to contribute back to the community or incorporate it into proprietary software as per the license's permissions.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Contact**<a name="contact"></a>
+## **Contact**<a name="contact"></a>
 
 If you have any questions or suggestions, feel free to reach out to me at [Bikatr7@proton.me](mailto:Bikatr7@proton.me)
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/EasyTL) for this project.
 
 Or the issue tracker [here](https://github.com/Bikatr7/EasyTL/issues).
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Contribution**<a name="contribution"></a>
+## **Contribution**<a name="contribution"></a>
 
 Contributions are welcome! I don't have a specific format for contributions, but please feel free to submit a pull request or open an issue if you have any suggestions or improvements.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Notes**<a name="notes"></a>
+## **Acknowledgements**<a name="acknowledgements"></a>
 
 EasyTL was originally developed as a part of [Kudasai](https://github.com/Bikatr7/Kudasai), a Japanese preprocessor later turned Machine Translator. It was later split off into its own package to be used independently of Kudasai for multiple reasons.
 
 This package is also my second serious attempt at creating a Python package, so I'm sure there are some things that could be improved. Feedback is welcomed.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `easytl-0.4.0b0/SECURITY.md` & `easytl-0.4.1/SECURITY.md`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Security Policy
 
 ## Introduction
 
 I take the security of the EasyTL library very seriously. I appreciate your efforts to responsibly disclose your findings and will make every effort to acknowledge your contributions.
 
+Please note: Public disclosure of the vulnerability without prior agreement is not recommended, as it could put the wider user community at risk.
+
 ## Reporting a Vulnerability
 
 Please report (suspected) security vulnerabilities to **[Bikatr7@proton.me](mailto:Bikatr7@proton.me)**. You should receive a response within 48 hours. If the issue is confirmed, I will release a patch as soon as possible depending on the complexity but typically within a few days.
 
 ### What to include in a security report
 
 - The version of EasyTL you are using
@@ -39,10 +41,8 @@
 
 ## Policy on Security Updates
 
 I will keep you informed of the progress towards fixing the vulnerability and announce the patched version once it is available.
 
 ## Acknowledgements
 
-Individuals who report security vulnerabilities responsibly will be acknowledged in the project documentation. If you would like to be acknowledged, please include a name or alias in your report.
-
-Please note: Public disclosure of the vulnerability without prior agreement is not recommended, as it could put the wider user community at risk.
+Individuals who report security vulnerabilities responsibly will be acknowledged in the project documentation. If you would like to be acknowledged, please include a name or alias in your report.
```

### Comparing `easytl-0.4.0b0/pyproject.toml` & `easytl-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 [project]
 dependencies = [
     "google-generativeai==0.5.4",
     "deepl==1.16.1",
     "openai==1.29.0",
     "backoff==2.2.1",
-    "tiktoken==0.6.0",
+    "tiktoken==0.7.0",
     "google-cloud-translate==3.15.3",
-    "anthropic==0.26.0",
+    "anthropic==0.26.1",
     "requests>=2.31.0",
 ]
 
 name = "easytl"
-version = "v0.4.0-beta"
+version = "v0.4.1"
 authors = [
   { name="Kaden Bilyeu (Bikatr7)", email="Bikatr7@proton.me"},
   { name="Alejandro Mata", email="alemalvarez@icloud.com"},
 ] 
 description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini, Google Translate and More."
 readme = "README.md"
 requires-python = ">=3.10"
@@ -36,7 +36,8 @@
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Bikatr7/EasyTL"
 Issues = "https://github.com/Bikatr7/EasyTL/issues"
+Documentation = "https://easytl.readthedocs.io/en/latest/index.html"
```

### Comparing `easytl-0.4.0b0/src/easytl/__init__.py` & `easytl-0.4.1/src/easytl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
 ## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 from .version import VERSION as __version__  # noqa
 
-__author__ = "Bikatr7 <Tetralon07@gmail.com>"
+__author__ = "Kaden Bilyeu (Bikatr7) <Bikatr7@proton.me>"
 
 from .easytl import EasyTL
 
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
 from .classes import Message, SystemTranslationMessage, ModelTranslationMessage
 from .classes import ChatCompletion
 from .classes import GenerateContentResponse, AsyncGenerateContentResponse, GenerationConfig
@@ -33,14 +33,15 @@
 from .exceptions import RequestException
 
 ## service specific exceptions
 from .exceptions import OpenAIAPIError, OpenAIConflictError, OpenAINotFoundError, OpenAIAPIStatusError, OpenAIRateLimitError, OpenAIAPITimeoutError, OpenAIBadRequestError, OpenAIAPIConnectionError, OpenAIAuthenticationError, OpenAIInternalServerError, OpenAIPermissionDeniedError, OpenAIUnprocessableEntityError, OpenAIAPIResponseValidationError
 from .exceptions import DeepLAuthorizationException, DeepLQuotaExceededException, DeepLConnectionException, DeepLTooManyRequestsException, DeepLDocumentNotReadyException, DeepLGlossaryNotFoundException, DeepLDocumentTranslationException
 from .exceptions import GoogleAuthError, GoogleDefaultCredentialsError
 from .exceptions import AnthropicAPIError, AnthropicConflictError, AnthropicNotFoundError, AnthropicAPIStatusError, AnthropicRateLimitError, AnthropicAPITimeoutError, AnthropicBadRequestError, AnthropicAPIConnectionError, AnthropicAuthenticationError, AnthropicInternalServerError, AnthropicPermissionDeniedError, AnthropicUnprocessableEntityError, AnthropicAPIResponseValidationError
+from .exceptions import BadAzureRegionException, InvalidAPIKeyException, InvalidEasyTLSettingsException
 
 __all__ = [
     "EasyTL",
     "Language", "SplitSentences", "Formality", "GlossaryInfo", "TextResult",
     "Message", "SystemTranslationMessage", "ModelTranslationMessage",
     "ChatCompletion",
     "GenerateContentResponse", "AsyncGenerateContentResponse", "GenerationConfig",
@@ -51,9 +52,10 @@
     "GoogleAPIError",
     "OpenAIError",
     "AnthropicError",
     "RequestException",
     "OpenAIAPIError", "OpenAIConflictError", "OpenAINotFoundError", "OpenAIAPIStatusError", "OpenAIRateLimitError", "OpenAIAPITimeoutError", "OpenAIBadRequestError", "OpenAIAPIConnectionError", "OpenAIAuthenticationError", "OpenAIInternalServerError", "OpenAIPermissionDeniedError", "OpenAIUnprocessableEntityError", "OpenAIAPIResponseValidationError",
     "DeepLAuthorizationException", "DeepLQuotaExceededException", "DeepLConnectionException", "DeepLTooManyRequestsException", "DeepLDocumentNotReadyException", "DeepLGlossaryNotFoundException", "DeepLDocumentTranslationException",
     "GoogleAuthError", "GoogleDefaultCredentialsError",
-    "AnthropicAPIError", "AnthropicConflictError", "AnthropicNotFoundError", "AnthropicAPIStatusError", "AnthropicRateLimitError", "AnthropicAPITimeoutError", "AnthropicBadRequestError", "AnthropicAPIConnectionError", "AnthropicAuthenticationError", "AnthropicInternalServerError", "AnthropicPermissionDeniedError", "AnthropicUnprocessableEntityError", "AnthropicAPIResponseValidationError"
+    "AnthropicAPIError", "AnthropicConflictError", "AnthropicNotFoundError", "AnthropicAPIStatusError", "AnthropicRateLimitError", "AnthropicAPITimeoutError", "AnthropicBadRequestError", "AnthropicAPIConnectionError", "AnthropicAuthenticationError", "AnthropicInternalServerError", "AnthropicPermissionDeniedError", "AnthropicUnprocessableEntityError", "AnthropicAPIResponseValidationError",
+    "BadAzureRegionException", "InvalidAPIKeyException", "InvalidEasyTLSettingsException"
 ]
```

### Comparing `easytl-0.4.0b0/src/easytl/classes.py` & `easytl-0.4.1/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0b0/src/easytl/decorators.py` & `easytl-0.4.1/src/easytl/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 ## Copyright (C) 2024 Kaden Bilyeu (Bikatr7) (https://github.com/Bikatr7), Alejandro Mata (https://github.com/alemalvarez)
 ## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
+## One day this absolute disaster of a file will break and I will have to fix it. But today is not that day.
+
 ## built-in libraries
 from functools import wraps
 
 import datetime
 import os
 
 ## custom modules
```

### Comparing `easytl-0.4.0b0/src/easytl/easytl.py` & `easytl-0.4.1/src/easytl/easytl.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 ## Use of this source code is governed by an GNU Lesser General Public License v2.1
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 
-import warnings
-
 ## third-party libraries
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, NOT_GIVEN, NotGiven
 
 ## custom modules
 from .services.deepl_service import DeepLService
 from .services.gemini_service import GeminiService
 from .services.openai_service import OpenAIService
 from .services.googletl_service import GoogleTLService
 from .services.anthropic_service import AnthropicService
 from .services.azure_service import AzureService
 
 from. classes import ModelTranslationMessage, SystemTranslationMessage, TextResult, GenerateContentResponse, AsyncGenerateContentResponse, ChatCompletion, AnthropicMessage, AnthropicToolsBetaMessage, AnthropicTextBlock, AnthropicToolUseBlock
-from .exceptions import DeepLException, GoogleAPIError, OpenAIError, InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException, AnthropicError, RequestException
+from .exceptions import InvalidAPITypeException, InvalidResponseFormatException, InvalidTextInputException, EasyTLException
 
 from .util.util import _is_iterable_of_strings
 from .util.llm_util import _validate_easytl_llm_translation_settings, _return_curated_gemini_settings, _return_curated_openai_settings, _validate_stop_sequences, _validate_response_schema,  _return_curated_anthropic_settings, _validate_text_length 
 
 class EasyTL:
 
     """
@@ -49,16 +47,16 @@
     def set_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic", "azure"], credentials:str) -> None:
 
         """
 
         Sets the credentials for the specified API type.
 
         Parameters:
-        api_type (literal["deepl", "gemini", "openai", "google translate", "anthropic"]) : The API type to set the credentials for.
-        credentials (string) : The credentials to set. This is an api key for deepl, gemini, anthropic, and openai. For google translate, this is a path to your json that has your service account key.
+        api_type (literal["deepl", "gemini", "openai", "google translate", "anthropic", "azure"]) : The API type to set the credentials for.
+        credentials (string) : The credentials to set. This is an api key for deepl, gemini, anthropic, azure and openai. For google translate, this is a path to your json that has your service account key.
 
         """
 
         service_map = {
             "deepl": DeepLService._set_api_key,
             "gemini": GeminiService._set_api_key,
             "openai": OpenAIService._set_api_key,
@@ -71,46 +69,48 @@
         assert api_type in service_map, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai', 'google translate', 'anthropic' and 'azure'.")
 
         service_map[api_type](credentials)
 
 ##-------------------start-of-test_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def test_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic", "azure"]) -> typing.Tuple[bool, typing.Optional[Exception]]:
+    def test_credentials(api_type:typing.Literal["deepl", "gemini", "openai", "google translate", "anthropic", "azure"], azure_region:str = "westus") -> typing.Tuple[bool, typing.Optional[Exception]]:
 
         """
 
         Tests the validity of the credentials for the specified API type.
 
         Parameters:
-        api_type (literal["deepl", "gemini", "openai", "google translate", "anthropic"]) : The API type to test the credentials for.
+        api_type (literal["deepl", "gemini", "openai", "google translate", "anthropic", "azure"]) : The API type to test the credentials for.
+        azure_region (string) : The Azure region to test the credentials for. Default is 'westus'. Can be omitted for other services.
 
         Returns:
         (bool) : Whether the credentials are valid.
         (Exception) : The exception that was raised, if any. None otherwise.
 
         """
 
         api_services = {
-            "deepl": {"service": DeepLService, "exception": DeepLException, "test_func": DeepLService._test_api_key_validity},
-            "gemini": {"service": GeminiService, "exception": GoogleAPIError, "test_func": GeminiService._test_api_key_validity},
-            "openai": {"service": OpenAIService, "exception": OpenAIError, "test_func": OpenAIService._test_api_key_validity},
-            "google translate": {"service": GoogleTLService, "exception": GoogleAPIError, "test_func": GoogleTLService._test_credentials},
-            "anthropic": {"service": AnthropicService, "exception": AnthropicError, "test_func": AnthropicService._test_api_key_validity},
-            "azure": {"service": AzureService, "exception": RequestException, "test_func": AzureService._test_credentials}
+            "deepl": {"service": DeepLService, "test_func": DeepLService._test_api_key_validity},
+            "gemini": {"service": GeminiService, "test_func": GeminiService._test_api_key_validity},
+            "openai": {"service": OpenAIService, "test_func": OpenAIService._test_api_key_validity},
+            "google translate": {"service": GoogleTLService, "test_func": GoogleTLService._test_credentials},
+            "anthropic": {"service": AnthropicService, "test_func": AnthropicService._test_api_key_validity},
+            "azure": {"service": AzureService, "test_func": AzureService._test_credentials}
         }
 
         assert api_type in api_services, InvalidAPITypeException("Invalid API type specified. Supported types are 'deepl', 'gemini', 'openai', 'google translate', 'anthropic' and 'azure'.")
 
-        _is_valid, _e = api_services[api_type]["test_func"]()
+        if(api_type == "azure"):
+            _, _e = api_services[api_type]["test_func"](azure_region)
+        else:
+            _, _e = api_services[api_type]["test_func"]()
 
-        if(not _is_valid):
-            ## Done to make sure the exception is due to the specified API type and not the fault of EasyTL
-            assert isinstance(_e, api_services[api_type]["exception"]), _e
-            return False, _e
+        if(_e is not None):
+            raise _e
 
         return True, None
     
 ##-------------------start-of-googletl_translate()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def googletl_translate(text:typing.Union[str, typing.Iterable[str]],
@@ -730,30 +730,32 @@
                         override_previous_settings:bool = True,
                         decorator:typing.Callable | None = None,
                         logging_directory:str | None = None,
                         response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                         translation_delay:float | None = None,
                         translation_instructions:str | SystemTranslationMessage | None = None,
                         model:str="gpt-4",
-                        temperature:float=0.3,
-                        top_p:float=1.0,
-                        stop:typing.List[str] | None=None,
-                        max_tokens:int | None=None,
-                        presence_penalty:float=0.0,
-                        frequency_penalty:float=0.0
+                        temperature:float | None | NotGiven = NOT_GIVEN,
+                        top_p:float | None | NotGiven = NOT_GIVEN,
+                        stop:typing.List[str] | None | NotGiven = NOT_GIVEN,
+                        max_tokens:int | None | NotGiven = NOT_GIVEN,
+                        presence_penalty:float | None | NotGiven = NOT_GIVEN,
+                        frequency_penalty:float | None | NotGiven = NOT_GIVEN
                         ) -> typing.Union[typing.List[str], str, typing.List[ChatCompletion], ChatCompletion]:
         
         """
 
         Translates the given text using OpenAI.
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
+        Due to how OpenAI's API works, NOT_GIVEN is treated differently than None. If a parameter is set to NOT_GIVEN, it is not passed to the API. If it is set to None, it is passed to the API as None.
+        
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, OpenAI will retry the request twice if it fails.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
@@ -839,33 +841,35 @@
                                     decorator:typing.Callable | None = None,
                                     logging_directory:str | None = None,
                                     response_type:typing.Literal["text", "raw", "json", "raw_json"] | None = "text",
                                     semaphore:int | None = 5,
                                     translation_delay:float | None = None,
                                     translation_instructions:str | SystemTranslationMessage | None = None,
                                     model:str="gpt-4",
-                                    temperature:float=0.3,
-                                    top_p:float=1.0,
-                                    stop:typing.List[str] | None=None,
-                                    max_tokens:int | None=None,
-                                    presence_penalty:float=0.0,
-                                    frequency_penalty:float=0.0
+                                    temperature:float | None | NotGiven = NOT_GIVEN,
+                                    top_p:float | None | NotGiven = NOT_GIVEN,
+                                    stop:typing.List[str] | None | NotGiven = NOT_GIVEN,
+                                    max_tokens:int | None | NotGiven = NOT_GIVEN,
+                                    presence_penalty:float | None | NotGiven = NOT_GIVEN,
+                                    frequency_penalty:float | None | NotGiven = NOT_GIVEN
                                     ) -> typing.Union[typing.List[str], str, typing.List[ChatCompletion], ChatCompletion]:
         
         """
 
         Asynchronous version of openai_translate().
         Will generally be faster for iterables. Order is preserved.
 
         Translates the given text using OpenAI.
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
+        Due to how OpenAI's API works, NOT_GIVEN is treated differently than None. If a parameter is set to NOT_GIVEN, it is not passed to the API. If it is set to None, it is passed to the API as None.
+
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
         decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, OpenAI will retry the request twice if it fails.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
@@ -1238,15 +1242,16 @@
         Returns:
         result (string or list - string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
 
         """
 
         assert response_type in ["text", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'json'.")
 
-        EasyTL.test_credentials("azure")
+
+        EasyTL.test_credentials("azure", azure_region=azure_region)
 
         if(override_previous_settings == True):
             AzureService._set_attributes(target_language=target_lang,
                                         api_version=api_version,
                                         azure_region=azure_region,
                                         azure_endpoint=azure_endpoint,
                                         source_language=source_lang,
@@ -1333,15 +1338,15 @@
         Returns:
         result (string or list - string) : The translation result. A list of strings if the input was an iterable, a string otherwise.
         
         """
 
         assert response_type in ["text", "json"], InvalidResponseFormatException("Invalid response type specified. Must be 'text' or 'json'.")
 
-        EasyTL.test_credentials("azure")
+        EasyTL.test_credentials("azure", azure_region=azure_region)
 
         if(override_previous_settings == True):
             AzureService._set_attributes(target_language=target_lang,
                                         api_version=api_version,
                                         azure_region=azure_region,
                                         azure_endpoint=azure_endpoint,
                                         source_language=source_lang,
@@ -1526,18 +1531,18 @@
         
         """
 
         Calculates the cost of translating the given text using the specified service.
 
         For LLMs, the cost is based on the default model unless specified.
 
-        Model and Translation Instructions are ignored for DeepL and Google Translate.
+        Model and Translation Instructions are ignored for DeepL, Google Translate and Azure.
+
+        For DeepL, Azure and Google Translate, the number of tokens is the number of characters in the text. The returned model is the name of the service.
 
-        For deepl, number of tokens is the number of characters, the returned model is always "deepl".
-        The same applies for google translate, but the model is "google translate".
 
         Note that Anthropic's cost estimate is pretty sketchy and can be inaccurate. Refer to the actual response object for the cost or the API panel. This is because their tokenizer is not public and we're forced to estimate.
 
         Parameters:
         text (string or iterable) : The text to translate.
         service (string) : The service to use for translation.
         model (string or None) : The model to use for translation. If None, the default model is used.
@@ -1546,15 +1551,15 @@
         Returns:
         num_tokens (int) : The number of tokens/characters in the text.
         cost (float) : The cost of translating the text.
         model (string) : The model used for translation.
 
         """
 
-        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic", "azure"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate' or 'anthropic'.")
+        assert service in ["deepl", "openai", "gemini", "google translate", "anthropic", "azure"], InvalidAPITypeException("Invalid service specified. Must be 'deepl', 'openai', 'gemini', 'google translate', 'anthropic' or 'azure'.")
 
         if(service == "deepl"):
             return DeepLService._calculate_cost(text)
         
         elif(service == "openai"):
             return OpenAIService._calculate_cost(text, translation_instructions, model)
```

### Comparing `easytl-0.4.0b0/src/easytl/exceptions.py` & `easytl-0.4.1/src/easytl/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 ## service specific exceptions
 from openai import APIError as OpenAIAPIError, ConflictError as OpenAIConflictError, NotFoundError as OpenAINotFoundError, APIStatusError as OpenAIAPIStatusError, RateLimitError as OpenAIRateLimitError, APITimeoutError as OpenAIAPITimeoutError, BadRequestError as OpenAIBadRequestError, APIConnectionError as OpenAIAPIConnectionError, AuthenticationError as OpenAIAuthenticationError, InternalServerError as OpenAIInternalServerError, PermissionDeniedError as OpenAIPermissionDeniedError, UnprocessableEntityError as OpenAIUnprocessableEntityError, APIResponseValidationError as OpenAIAPIResponseValidationError
 from deepl.exceptions import AuthorizationException as DeepLAuthorizationException, QuotaExceededException as DeepLQuotaExceededException, ConnectionException as DeepLConnectionException, TooManyRequestsException as DeepLTooManyRequestsException, DocumentNotReadyException as DeepLDocumentNotReadyException, GlossaryNotFoundException as DeepLGlossaryNotFoundException, DocumentTranslationException as DeepLDocumentTranslationException
 from google.auth.exceptions import GoogleAuthError, DefaultCredentialsError as GoogleDefaultCredentialsError
 from anthropic import APIError as AnthropicAPIError, ConflictError as AnthropicConflictError, NotFoundError as AnthropicNotFoundError, APIStatusError as AnthropicAPIStatusError, RateLimitError as AnthropicRateLimitError, APITimeoutError as AnthropicAPITimeoutError, BadRequestError as AnthropicBadRequestError, APIConnectionError as AnthropicAPIConnectionError, AuthenticationError as AnthropicAuthenticationError, InternalServerError as AnthropicInternalServerError, PermissionDeniedError as AnthropicPermissionDeniedError, UnprocessableEntityError as AnthropicUnprocessableEntityError, APIResponseValidationError as AnthropicAPIResponseValidationError
 
+##-------------------start-of-EasyTLException--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
 class EasyTLException(Exception):
 
     """
 
     EasyTLException is the base exception class for all exceptions in the EasyTL package.
 
     """
@@ -148,13 +150,34 @@
 
     """
 
     def __init__(self, message:str) -> None:
 
         """
 
+        Parameters:
+        message (string) : The message to display when the exception is raised.
+
+        """
+
+        self.message = message
+
+##-------------------start-of-BadAzureRegionException--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+class BadAzureRegionException(EasyTLException):
+
+    """
+
+    BadAzureRegionException is an exception that is raised when the Azure region is invalid.
+
+    """
+
+    def __init__(self, message:str) -> None:
+
+        """
+
         Parameters:
         message (string) : The message to display when the exception is raised.
 
         """
 
         self.message = message
```

### Comparing `easytl-0.4.0b0/src/easytl/services/anthropic_service.py` & `easytl-0.4.1/src/easytl/services/anthropic_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,32 +264,30 @@
 
         """
         
         attributes = ["temperature", "top_p", "top_k", "stream", "stop_sequences", "max_tokens"]
         message_args = {
             "model": AnthropicService._model,
             "system": instructions,
-            "messages": [prompt.to_dict()],  # type: ignore
+            "messages": [prompt.to_dict()],
+            ## scary looking dict comprehension to get the attributes that are not NOT_GIVEN
+            **{attr: getattr(AnthropicService, f"_{attr}") for attr in attributes if getattr(AnthropicService, f"_{attr}") != NOT_GIVEN}
         }
         
-        for attr in attributes:
-            value = getattr(AnthropicService, f"_{attr}")
-            if(value != NOT_GIVEN):
-                message_args[attr] = value
-        
-        # Special case for max_tokens
-        if("max_tokens" not in message_args):
-            message_args["max_tokens"] = 4096
+        ## Special case for max_tokens
+        message_args["max_tokens"] = message_args.get("max_tokens", 4096)
         
         if(AnthropicService._json_mode and AnthropicService._model in VALID_JSON_ANTHROPIC_MODELS):
-            message_args["tools"] = [AnthropicService._json_tool]
-            message_args["tool_choice"] = {"type": "tool", "name": "format_to_json"}
+            message_args.update({
+                "tools": [AnthropicService._json_tool],
+                "tool_choice": {"type": "tool", "name": "format_to_json"}
+            })
         
         response = AnthropicService._sync_client.beta.tools.messages.create(**message_args)
-
+        
         return response
     
 ##-------------------start-of- __translate_text_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     async def __translate_text_async(instructions:str, prompt:ModelTranslationMessage) -> AnthropicMessage | AnthropicToolsBetaMessage:
 
@@ -311,29 +309,27 @@
             if(AnthropicService._rate_limit_delay is not None):
                 await asyncio.sleep(AnthropicService._rate_limit_delay)
 
             attributes = ["temperature", "top_p", "top_k", "stream", "stop_sequences", "max_tokens"]
             message_args = {
                 "model": AnthropicService._model,
                 "system": instructions,
-                "messages": [prompt.to_dict()],  # type: ignore
+                "messages": [prompt.to_dict()],
+                ## scary looking dict comprehension to get the attributes that are not NOT_GIVEN
+                **{attr: getattr(AnthropicService, f"_{attr}") for attr in attributes if getattr(AnthropicService, f"_{attr}") != NOT_GIVEN}
             }
             
-            for attr in attributes:
-                value = getattr(AnthropicService, f"_{attr}")
-                if(value != NOT_GIVEN):
-                    message_args[attr] = value
-            
-            # Special case for max_tokens
-            if("max_tokens" not in message_args):
-                message_args["max_tokens"] = 4096
+            ## Special case for max_tokens
+            message_args["max_tokens"] = message_args.get("max_tokens", 4096)
             
             if(AnthropicService._json_mode and AnthropicService._model in VALID_JSON_ANTHROPIC_MODELS):
-                message_args["tools"] = [AnthropicService._json_tool]
-                message_args["tool_choice"] = {"type": "tool", "name": "format_to_json"}
+                message_args.update({
+                    "tools": [AnthropicService._json_tool],
+                    "tool_choice": {"type": "tool", "name": "format_to_json"}
+                })
 
             response = await AnthropicService._async_client.beta.tools.messages.create(**message_args)
 
             return response
     
 ##-------------------start-of-test_api_key_validity()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `easytl-0.4.0b0/src/easytl/services/azure_service.py` & `easytl-0.4.1/src/easytl/services/azure_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # third-party libraries
 import requests
 
 ## custom modules
 from ..util.util import _convert_iterable_to_str
 from ..decorators import _async_logging_decorator, _sync_logging_decorator
+from ..exceptions import BadAzureRegionException
 
 class AzureService:
 
     _api_key:str = ""
     _location:str = ""
     _endpoint:str = ""
 
@@ -147,14 +148,17 @@
             }]
 
             url = AzureService._endpoint + AzureService._path
 
             request = requests.post(url, params=params, headers=headers, json=body)
             response = request.json()
 
+            if('error' in response):
+                raise BadAzureRegionException(f"{response['error']['message']}\n\nTip: Double check API key, region and endpoint :)")
+
             return response
 
         except Exception as _e:
             raise _e
         
 ##-------------------start-of-_translate_text_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
@@ -181,26 +185,28 @@
 
             loop = asyncio.get_running_loop()
             return await loop.run_in_executor(None, lambda: AzureService._translate_text(text))
             
 ##-------------------start-of-_test_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def _test_credentials() -> typing.Tuple[bool, typing.Union[Exception, None]]:
+    def _test_credentials(azure_region: str) -> typing.Tuple[bool, typing.Union[Exception, None]]:
 
         """
 
         Tests the credentials for the Azure service.
 
         Returns:
         success (bool): True if the credentials are valid, False otherwise.
         error (Exception): The error that occurred during the test.
 
         """
 
+        AzureService._set_attributes(azure_region=azure_region)
+
         try:
             AzureService._translate_text('Hola')
             return True, None
 
         except Exception as _e:
             return False, _e
```

### Comparing `easytl-0.4.0b0/src/easytl/services/deepl_service.py` & `easytl-0.4.1/src/easytl/services/deepl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0b0/src/easytl/services/gemini_service.py` & `easytl-0.4.1/src/easytl/services/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0b0/src/easytl/services/googletl_service.py` & `easytl-0.4.1/src/easytl/services/googletl_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from google.cloud import translate_v2 as translate
 from google.cloud.translate_v2 import Client
 
 from google.oauth2 import service_account
 from google.oauth2.service_account import Credentials
 
 ## custom modules
-from ..version import VERSION
 from ..util.util import _convert_iterable_to_str
 from ..decorators import _sync_logging_decorator, _async_logging_decorator
 
 class GoogleTLService:
 
     _translator:Client
     _credentials:Credentials
```

### Comparing `easytl-0.4.0b0/src/easytl/services/openai_service.py` & `easytl-0.4.1/src/easytl/services/openai_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing
 import asyncio
 
 ## third-party libraries
 from openai import AsyncOpenAI, OpenAI
 
 ## custom modules
-from ..classes import SystemTranslationMessage, ModelTranslationMessage, ChatCompletion
+from ..classes import SystemTranslationMessage, ModelTranslationMessage, ChatCompletion, NOT_GIVEN, NotGiven
 from ..decorators import _async_logging_decorator, _sync_logging_decorator
 from ..exceptions import EasyTLException
 
 from ..util.util import _convert_iterable_to_str, _estimate_cost, _is_iterable_of_strings
 from ..util.constants import VALID_JSON_OPENAI_MODELS
 
 
@@ -22,23 +22,23 @@
 
     _default_model:str = "gpt-4"
     _default_translation_instructions:SystemTranslationMessage = SystemTranslationMessage("Please translate the following text into English.")
 
     _system_message:typing.Optional[typing.Union[SystemTranslationMessage, str]] = _default_translation_instructions
 
     _model:str = _default_model
-    _temperature:float = 0.3
-    _logit_bias:typing.Dict[str, int] | None
-    _top_p:float = 1.0
-    _n:int = 1
+    _temperature:float | None | NotGiven = NOT_GIVEN
+    _logit_bias:typing.Dict[str, int] | None | NotGiven = NOT_GIVEN
+    _top_p:float | None | NotGiven = NOT_GIVEN
+    _n:int | None | NotGiven = 1
     _stream:bool = False
-    _stop:typing.List[str] | None = None
-    _max_tokens:int | None = None
-    _presence_penalty:float = 0.0
-    _frequency_penalty:float = 0.0
+    _stop:typing.List[str] | None | NotGiven = NOT_GIVEN
+    _max_tokens:int | None | NotGiven = NOT_GIVEN
+    _presence_penalty:float | None | NotGiven = NOT_GIVEN
+    _frequency_penalty:float | None | NotGiven = NOT_GIVEN
 
     _semaphore_value:int = 5
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
     _sync_client = OpenAI(api_key="DummyKey")
     _async_client = AsyncOpenAI(api_key="DummyKey")
 
@@ -67,23 +67,23 @@
         OpenAIService._async_client.api_key = api_key
         OpenAIService._sync_client.api_key = api_key
 
 ##-------------------start-of-set_attributes()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     def _set_attributes(model:str = _default_model,
-                        temperature:float = 0.3,
-                        logit_bias:typing.Dict[str, int] | None = None,
-                        top_p:float = 1.0,
-                        n:int = 1,
+                        temperature:float | None | NotGiven = NOT_GIVEN,
+                        logit_bias:typing.Dict[str, int] | None | NotGiven = NOT_GIVEN,
+                        top_p:float | None | NotGiven = NOT_GIVEN,
+                        n:int | None | NotGiven = 1,
                         stream:bool = False,
-                        stop:typing.List[str] | None = None,
-                        max_tokens:int | None = None,
-                        presence_penalty:float = 0.0,
-                        frequency_penalty:float = 0.0,
+                        stop:typing.List[str] | None | NotGiven = NOT_GIVEN,
+                        max_tokens:int | None | NotGiven = NOT_GIVEN,
+                        presence_penalty:float | None | NotGiven = NOT_GIVEN,
+                        frequency_penalty:float | None | NotGiven = NOT_GIVEN,
                         decorator:typing.Union[typing.Callable, None]=None,
                         logging_directory:str | None=None,
                         semaphore:int | None=None,
                         rate_limit_delay:float | None=None,
                         json_mode:bool=False
                         ) -> None:
     
@@ -252,81 +252,63 @@
         Returns:
         response (ChatCompletion) : The response from the API.
 
         """
 
         response_format = "json_object" if OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS else "text"
 
-        response = OpenAIService._sync_client.chat.completions.create(
-            response_format={ "type": response_format },
-            messages=[ 
-                instructions.to_dict(),
-                prompt.to_dict()
-            ], # type: ignore
-
-            model=OpenAIService._model,
-            temperature=OpenAIService._temperature,
-            logit_bias=OpenAIService._logit_bias,
-            top_p=OpenAIService._top_p,
-            n=OpenAIService._n,
-            stream=OpenAIService._stream,
-            stop=OpenAIService._stop,
-            presence_penalty=OpenAIService._presence_penalty,
-            frequency_penalty=OpenAIService._frequency_penalty,
-            max_tokens=OpenAIService._max_tokens
-            
-        ) 
+        attributes = ["temperature", "logit_bias", "top_p", "n", "stream", "stop", "presence_penalty", "frequency_penalty", "max_tokens"]
+        message_args = {
+            "response_format": { "type": response_format },
+            "model": OpenAIService._model,
+            "messages": [instructions.to_dict(), prompt.to_dict()],
+            ## scary looking dict comprehension to get the attributes that are not NOT_GIVEN
+            **{attr: getattr(OpenAIService, f"_{attr}") for attr in attributes if getattr(OpenAIService, f"_{attr}") != NOT_GIVEN}
+        }
+
+        response = OpenAIService._sync_client.chat.completions.create(**message_args)
         
         return response
     
 ##-------------------start-of- __translate_text_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    async def __translate_text_async(instruction:SystemTranslationMessage, prompt:ModelTranslationMessage) -> ChatCompletion:
+    async def __translate_text_async(instructions:SystemTranslationMessage, prompt:ModelTranslationMessage) -> ChatCompletion:
 
         """
 
         Asynchronously translates the text using the OpenAI API.
 
         Parameters:
         instruction (SystemTranslationMessage) : The instructions to use for the translation.
         prompt (ModelTranslationMessage) : The text to translate.
 
         Returns:
         response (ChatCompletion) : The response from the API.
 
         """
 
-        response_format = "json_object" if OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS else "text"
-
         async with OpenAIService._semaphore:
 
+            response_format = "json_object" if OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS else "text"
+
             if(OpenAIService._rate_limit_delay is not None):
                 await asyncio.sleep(OpenAIService._rate_limit_delay)
 
-            response = await OpenAIService._async_client.chat.completions.create(
-                response_format={ "type": response_format },
-                messages=[
-                    instruction.to_dict(),
-                    prompt.to_dict()
-                ],  # type: ignore
-
-                model=OpenAIService._model,
-                temperature=OpenAIService._temperature,
-                logit_bias=OpenAIService._logit_bias,
-                top_p=OpenAIService._top_p,
-                n=OpenAIService._n,
-                stream=OpenAIService._stream,
-                stop=OpenAIService._stop,
-                presence_penalty=OpenAIService._presence_penalty,
-                frequency_penalty=OpenAIService._frequency_penalty,
-                max_tokens=OpenAIService._max_tokens
-                
-            ) 
+            attributes = ["temperature", "logit_bias", "top_p", "n", "stream", "stop", "presence_penalty", "frequency_penalty", "max_tokens"]
+            message_args = {
+                "response_format": { "type": response_format },
+                "model": OpenAIService._model,
+                "messages": [instructions.to_dict(), prompt.to_dict()],
+                ## scary looking dict comprehension to get the attributes that are not NOT_GIVEN
+                **{attr: getattr(OpenAIService, f"_{attr}") for attr in attributes if getattr(OpenAIService, f"_{attr}") != NOT_GIVEN}
+            }
 
+            response = await OpenAIService._async_client.chat.completions.create(**message_args)
+            
             return response
 
 ##-------------------start-of-test_api_key_validity()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
     def _test_api_key_validity() -> typing.Tuple[bool, typing.Union[Exception, None]]:
```

### Comparing `easytl-0.4.0b0/src/easytl/util/constants.py` & `easytl-0.4.1/src/easytl/util/constants.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0b0/src/easytl/util/llm_util.py` & `easytl-0.4.1/src/easytl/util/llm_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import typing
 
 ## third-party libraries
 import tiktoken
 
 ## custom modules
 from ..util.constants import ALLOWED_OPENAI_MODELS, ALLOWED_GEMINI_MODELS, ALLOWED_ANTHROPIC_MODELS, MODEL_MAX_TOKENS
-from ..util.util import _convert_iterable_to_str, _convert_to_correct_type
+from ..util.util import _convert_iterable_to_str, _convert_to_correct_type, _update_model_name
 
 from ..exceptions import InvalidEasyTLSettingsException, TooManyInputTokensException
 from ..classes import ModelTranslationMessage, NotGiven, NOT_GIVEN
 
 ##-------------------start-of-_return_curated_anthropic_settings()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def _return_curated_anthropic_settings(local_settings:dict[str, typing.Any]) -> dict:
@@ -161,29 +161,33 @@
 
         if(isinstance(text, ModelTranslationMessage)):
             text = str(text)
 
         text = _convert_iterable_to_str(text) 
 
         if(service == "openai"):
+
+            ## this just gets the latest model if they passed in a generic model name
+            model = _update_model_name(model)
+            
             _encoding = tiktoken.encoding_for_model(model)
             _num_tokens = len(_encoding.encode(text))
 
             _max_tokens_allowed = MODEL_MAX_TOKENS.get(model, {}).get("max_input_tokens")
 
             ## silently return if the model is not in the list of models with a max token limit
             if(not _max_tokens_allowed):
                 return
 
             ## we can do a hard error with openai since we can accurately count tokens
             if(_num_tokens > _max_tokens_allowed):
                 raise TooManyInputTokensException(f"Input text exceeds the maximum token limit of {model}.")
             
         else:
-            _encoding = tiktoken.encoding_for_model("gpt-4")
+            _encoding = tiktoken.encoding_for_model("gpt-4-turbo-2024-04-09")
             _num_tokens = len(_encoding.encode(text))
 
             _max_tokens_allowed = MODEL_MAX_TOKENS.get(model, {}).get("max_input_tokens")
 
             ## silently return if the model is not in the list of models with a max token limit
             if(not _max_tokens_allowed):
                 return
```

### Comparing `easytl-0.4.0b0/src/easytl/util/util.py` & `easytl-0.4.1/src/easytl/util/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,14 @@
     if("constraints" in _setting_info and not _setting_info["constraints"](_converted_value)):
         raise ValueError(f"{setting_name} out of range")
 
     return _converted_value
 
 ##-------------------start-of-_estimate_cost()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-@staticmethod
 def _estimate_cost(text:str | typing.Iterable, model:str, price_case:int | None = None) -> typing.Tuple[int, float, str]:
 
     """
 
     Attempts to estimate cost.
 
     Parameters:
@@ -338,8 +337,40 @@
         _min_cost_for_input = (_num_tokens / 1000) * _input_cost
         _min_cost_for_output = (_num_tokens / 1000) * _output_cost
         _min_cost = _min_cost_for_input + _min_cost_for_output
 
         return _num_tokens, _min_cost, model
     
     ## type checker doesn't like the chance of None being returned, so we raise an exception here if it gets to this point, which it shouldn't
-    raise Exception("An unknown error occurred while calculating the minimum cost of translation.")
+    raise Exception("An unknown error occurred while calculating the minimum cost of translation.")
+
+##-------------------start-of-_update_model_name()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+def _update_model_name(model: str) -> str:
+
+    """
+    
+    Updates the model name to the most recent version.
+
+    Parameters:
+    model (string) : the model to update.
+
+    Returns:
+    model (string) : the updated model name.
+
+    """
+
+    model_updates = {
+        "gpt-3.5-turbo": "gpt-3.5-turbo-0125",
+        "gpt-3.5-turbo-16k": "gpt-3.5-turbo-16k-0613",
+        "gpt-4": "gpt-4-0613",
+        "gpt-4-32k": "gpt-4-32k-0613",
+        "gpt-4-turbo": "gpt-4-turbo-2024-04-09",
+        "gpt-4-turbo-preview": "gpt-4-0125-preview",
+        "gpt-4-vision-preview": "gpt-4-1106-vision-preview",
+        "gpt-4o": "gpt-4o-2024-05-13"
+    }
+
+    if(model in model_updates):
+        return model_updates[model]
+
+    return model
```

### Comparing `easytl-0.4.0b0/src/easytl.egg-info/PKG-INFO` & `easytl-0.4.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.4.0b0
+Version: 0.4.1
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini, Google Translate and More.
 Author-email: "Kaden Bilyeu (Bikatr7)" <Bikatr7@proton.me>, Alejandro Mata <alemalvarez@icloud.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
+Project-URL: Documentation, https://easytl.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: google-generativeai==0.5.4
 Requires-Dist: deepl==1.16.1
 Requires-Dist: openai==1.29.0
 Requires-Dist: backoff==2.2.1
-Requires-Dist: tiktoken==0.6.0
+Requires-Dist: tiktoken==0.7.0
 Requires-Dist: google-cloud-translate==3.15.3
-Requires-Dist: anthropic==0.26.0
+Requires-Dist: anthropic==0.26.1
 Requires-Dist: requests>=2.31.0
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 **Table of Contents**
 
-- [Quick Start](#quick-start)
-- [Installation](#installation)
-- [Features](#features)
-- [API Usage](#api-usage)
-- [License](#license)
-- [Contact](#contact)
-- [Contribution](#contribution)
-- [Notes](#notes)
+- [**Notes**](#notes)
+- [**Quick Start**](#quick-start)
+- [**Installation**](#installation)
+- [**Features**](#features)
+- [**API Usage**](#api-usage)
+  - [Translating Text](#translating-text)
+  - [Generic Translation Methods](#generic-translation-methods)
+  - [Cost Calculation](#cost-calculation)
+  - [Credentials Management](#credentials-management)
+- [**License**](#license)
+- [**Contact**](#contact)
+- [**Contribution**](#contribution)
+- [**Acknowledgements**](#acknowledgements)
 
----------------------------------------------------------------------------------------------------------------------------------------------------
+--------------------------------------------------------------------------------------------------------------------------------------------------
+
+## **Notes**<a name="notes"></a>
+
+Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini, Google Translate and More! 
 
-## EasyTL
+EasyTL has a [Trello board](https://trello.com/b/Td555CoW/easytl) for tracking planned features and issues:
 
-Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
+We've compiled a repository of examples and use cases for EasyTL at this [GitHub repository](https://github.com/Bikatr7/easytl-demo)
 
-EasyTL has a Trello board for tracking planned features and issues:
-https://trello.com/b/Td555CoW/easytl
+> [!TIP]
+> You can find the full documentation [here](https://easytl.readthedocs.io/en/latest/index.html)! (work in progress)
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
-**Quick Start**<a name="quick-start"></a>
+## **Quick Start**<a name="quick-start"></a>
 
 To get started with EasyTL, install the package via pip:
 
 ```bash
 pip install easytl
 ```
 
@@ -56,25 +66,49 @@
 
 For example, with DeepL:
 
 ```python
 from easytl import EasyTL
 
 ## Set your API key
-EasyTL.credentials("deepl", "your_api_key_here")
+EasyTL.set_credentials("deepl", "YOUR_API_KEY")
 
 ## You can also validate your API keys; translation functions will do this automatically
-is_valid, e = EasyTL.validate_credentials("deepl")
+is_valid, e = EasyTL.test_credentials("deepl")
 
 translated_text = EasyTL.deepl_translate("私は日本語が話せます", "EN-US") ## Text to translate, language to translate to, only two "required" arguments but there are more optional arguments for additional functionality and other services.
+
+print(translated_text) ## Output: "I can speak Japanese"
+```
+
+or with OpenAI:
+
+```python
+from easytl import EasyTL
+
+import asyncio
+
+async def main():
+
+    ## Set your API key
+    EasyTL.set_credentials("openai", "YOUR_API_KEY")
+
+    ## Get's the raw response from the API, allowing you to access the full response object
+    raw_response = await EasyTL.openai_translate_async("I can speak Japanese", model="gpt-4o", translation_instructions="Translate this text to Japanese.", response_type="raw") 
+
+    print(raw_response.choices[0].message.content) ## Output: "私は日本語が話せます" or something similar
+
+if(__name__ == "__main__"):
+    asyncio.run(main())
+
 ```
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Installation**<a name="installation"></a>
+## **Installation**<a name="installation"></a>
 
 Python 3.10+
 
 EasyTL can be installed using pip:
 
 ```bash
 pip install easytl
@@ -84,96 +118,109 @@
 
 These are the dependencies/requirements that will be installed:
 ```bash
 setuptools>=61.0
 wheel
 setuptools_scm>=6.0
 tomli
-google-generativeai==0.5.1
+requests>=2.31.0
+google-generativeai==0.5.4
 deepl==1.16.1
-openai==1.13.3
+openai==1.29.0
 backoff==2.2.1
-tiktoken==0.6.0
+tiktoken==0.7.0
 google-cloud-translate==3.15.3
+anthropic==0.26.1
 ```
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Features**<a name="features"></a>
+## **Features**<a name="features"></a>
 
 EasyTL offers seamless integration with several translation APIs, allowing users to easily switch between services based on their needs. Key features include:
 
-- Support for multiple translation APIs including OpenAI, DeepL, Gemini, and Google Translate.
-- Simple API key and credential management.
-- Methods to validate credentials before usage.
+- Support for multiple translation APIs including OpenAI, DeepL, Gemini, Google Translate, Microsoft Azure Translate, and Anthropic.
+- Simple API key and credential management and validation.
 - Cost estimation tools to help manage usage based on text length, translation instructions for LLMs, and translation services.
-- Highly customizable translation options, with the API's original features.
+- Highly customizable translation options, with each API's original features and more. 
 - Lots of optional arguments for additional functionality. Such as decorators, semaphores, and rate-limit delays.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**API Usage**<a name="api-usage"></a>
+## **API Usage**<a name="api-usage"></a>
 
 ### Translating Text
 
-Use `deepl_translate`, `googletl_translate`, `openai_translate`, or `gemini_translate` to translate text using the respective services. Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature for creative outputs.
+Translate functions can be broken down into two categories: LLM and non-LLM. LLM ones can take instructions, while non-LLM ones require a target language. 
+
+`deepl_translate`, `googletl_translate`, and `azure_translate` are non-LLM functions, while `openai_translate`, `gemini_translate`, and `anthropic_translate` are LLM functions.
+
+Each method accepts various parameters to customize the translation process, such as language, text format, and API-specific features like formality level or temperature. However these vary wildly between services, so it is recommended to check the documentation for each service for more information.
 
 All services offer asynchronous translation methods that return a future object for concurrent processing. These methods are suffixed with `_async` and can be awaited to retrieve the translated text.
 
-Instead of receiving the translated text directly, you can also use the `response` parameter to get the full response object from the API.
+Instead of receiving the translated text directly, you can also use the `response_type` parameter to get the raw response object, specify a json response where available, or both.
+  
+  `text` - Default. Returns the translated text.
+
+  `json` - Returns the response as a JSON object. Not all services support this.
+
+  `raw` - Returns the raw response object from the API. This can be useful for accessing additional information or debugging.
+  
+  `raw_json` - Returns the raw response object with the text but with the response also a json object. Again, not all services support this.
 
-## Generic Translation Methods
+### Generic Translation Methods
 
 EasyTL has generic translation methods `translate` and `translate_async` that can be used to translate text with any of the supported services. These methods accept the text, service, and kwargs of the respective service as parameters.
 
 ### Cost Calculation
 
 The `calculate_cost` method provides an estimate of the cost associated with translating a given text with specified settings for each supported service.
 
-characters or tokens depending on the service.
+These are characters or tokens depending on the type of translate function used.
 
 ```python
 num_characters, cost, model = EasyTL.calculate_cost("This has a lot of characters", "deepl")
 ```
 
 or 
 
 ```python
 num_tokens, cost, model = EasyTL.calculate_cost("This has a lot of tokens.", "openai", model="gpt-4", translation_instructions="Translate this text to Japanese.")
 ```
 
 ### Credentials Management
 
-Credentials can be set and validated using `set_credentials` and `validate_credentials` methods to ensure they are active and correct before submitting translation requests.
+Credentials can be set and validated using `set_credentials` and `test_credentials` methods to ensure they are active and correct before submitting translation requests.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**License**<a name="license"></a>
+## **License**<a name="license"></a>
 
 This project, EasyTL, is licensed under the GNU Lesser General Public License v2.1 (LGPLv2.1) - see the LICENSE file for complete details.
 
 The LGPL is a permissive copyleft license that enables this software to be freely used, modified, and distributed. It is particularly designed for libraries, allowing them to be included in both open source and proprietary software. When using or modifying EasyTL, you can choose to release your work under the LGPLv2.1 to contribute back to the community or incorporate it into proprietary software as per the license's permissions.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Contact**<a name="contact"></a>
+## **Contact**<a name="contact"></a>
 
 If you have any questions or suggestions, feel free to reach out to me at [Bikatr7@proton.me](mailto:Bikatr7@proton.me)
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/EasyTL) for this project.
 
 Or the issue tracker [here](https://github.com/Bikatr7/EasyTL/issues).
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Contribution**<a name="contribution"></a>
+## **Contribution**<a name="contribution"></a>
 
 Contributions are welcome! I don't have a specific format for contributions, but please feel free to submit a pull request or open an issue if you have any suggestions or improvements.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
-**Notes**<a name="notes"></a>
+## **Acknowledgements**<a name="acknowledgements"></a>
 
 EasyTL was originally developed as a part of [Kudasai](https://github.com/Bikatr7/Kudasai), a Japanese preprocessor later turned Machine Translator. It was later split off into its own package to be used independently of Kudasai for multiple reasons.
 
 This package is also my second serious attempt at creating a Python package, so I'm sure there are some things that could be improved. Feedback is welcomed.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `easytl-0.4.0b0/src/easytl.egg-info/SOURCES.txt` & `easytl-0.4.1/src/easytl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0b0/tests/issue_template.py` & `easytl-0.4.1/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.4.0b0/tests/passing.py` & `easytl-0.4.1/tests/passing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-from easytl import EasyTL
-
+## built-in libraries
 import asyncio
 import os
 import time
 import logging
 
+## third-party libraries
 import backoff
 
+## custom modules
+from easytl import EasyTL
+
 from easytl.exceptions import DeepLException, GoogleAPIError, OpenAIError, AnthropicAPIError
 
 ##-------------------start-of-read_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def read_api_key(filename):
+
     try:
         with open(filename, 'r') as file:
             return file.read().strip()
-        
     except:
         pass
 
 ##-------------------start-of-setup_preconditions()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def setup_preconditions():
 
+    ## default values, assuming github actions environment
     gemini_time_delay = 30
 
     deepl_api_key = os.environ.get('DEEPL_API_KEY')
     gemini_api_key = os.environ.get('GEMINI_API_KEY')
     openai_api_key = os.environ.get('OPENAI_API_KEY')
-    anthropic_api_key = os.environ.get('ANTHROPIC_API_KEY')
     json_value = os.environ.get('GOOGLE_TRANSLATE_SERVICE_KEY_VALUE')
+    anthropic_api_key = os.environ.get('ANTHROPIC_API_KEY')
     azure_api_key = os.environ.get('AZURE_API_KEY')
     azure_region = os.environ.get('AZURE_REGION')
 
+    ## this dumps the json value to a file as that's what the google translate service expects
     if(json_value is not None):
 
         with open("json_value.txt", "w") as file:
             file.write(json_value)
 
         google_tl_key_path = "json_value.txt"
 
+    ## the following will replace the keys with local test keys if the environment variables are not set (not a github actions environment)
     logging_directory = os.getenv('LOGGING_DIRECTORY', '/tmp/')
 
     if(deepl_api_key is None):
         deepl_api_key = read_api_key("tests/deepl.txt")
     if(gemini_api_key is None):
         gemini_api_key = read_api_key("tests/gemini.txt")
     if(openai_api_key is None):
@@ -51,35 +57,43 @@
     if(anthropic_api_key is None):
         anthropic_api_key = read_api_key("tests/anthropic.txt")
     if(azure_api_key is None):
         azure_api_key = read_api_key("tests/azure.txt")
     if(azure_region is None):
         azure_region = read_api_key("tests/azure_region.txt")
 
+    ## last json failure clarifies that this is not a github actions environment
     if(json_value is None):
         google_tl_key_path = "tests/google_translate_key.json"
         
         logging_directory = "tests/"
         gemini_time_delay = 5
 
+    ## if any of these trigger, something is wrong (not in local test environment or github actions environment)
     assert deepl_api_key is not None, "DEEPL_API_KEY environment variable must be set"
     assert gemini_api_key is not None, "GEMINI_API_KEY environment variable must be set"
     assert openai_api_key is not None, "OPENAI_API_KEY environment variable must be set"
     assert anthropic_api_key is not None, "ANTHROPIC_API_KEY environment variable must be set"
     assert azure_api_key is not None, "AZURE_API_KEY environment variable must be set"
-    assert azure_region is not None, "AZURE_REGION environment variable must be set"
+    #assert azure_region is not None, "AZURE_REGION environment variable must be set" 
+    # we can set a default for the region
+    if azure_region is None:
+        azure_region = "westus"
+        print(f"Using default Azure region: {azure_region}")
     assert google_tl_key_path is not None, "GOOGLE_TRANSLATE_SERVICE_KEY_VALUE environment variable must be set"
 
+    ## set the credentials for the services
     EasyTL.set_credentials("deepl", deepl_api_key)
     EasyTL.set_credentials("gemini", gemini_api_key)
     EasyTL.set_credentials("openai", openai_api_key)
     EasyTL.set_credentials("anthropic", anthropic_api_key)
     EasyTL.set_credentials("google translate", google_tl_key_path)
     EasyTL.set_credentials("azure", azure_api_key)
 
+    ## schema for gemini & anthropic
     schema = {
         "type": "object",
         "properties": {
             "input": {
                 "type": "string",
                 "description": "The text you were given to translate"
             },
@@ -95,28 +109,25 @@
 
 ##-------------------start-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def main():
 
     gemini_time_delay, logging_directory, schema, azure_region = setup_preconditions()
 
+    ## probably self explanatory from this point on
+
     decorator = backoff.on_exception(backoff.expo, exception=(DeepLException, GoogleAPIError, OpenAIError, AnthropicAPIError), logger=logging.getLogger())
 
     print("------------------------------------------------Deepl------------------------------------------------")
 
     print("------------------------------------------------Text response------------------------------------------------")
 
     print(EasyTL.deepl_translate(text="Hello, world!", target_lang="DE", logging_directory=logging_directory, decorator=decorator))
     print(await EasyTL.deepl_translate_async(text="Hello, world!", target_lang="DE", logging_directory=logging_directory,decorator=decorator))
 
-    print(EasyTL.deepl_translate("Hello, world!", target_lang="DE", response_type="raw", logging_directory=logging_directory, decorator=decorator).text) # type: ignore
-    result = await EasyTL.deepl_translate_async("Hello, world!", target_lang="DE", response_type="raw", logging_directory=logging_directory, decorator=decorator)
-
-    print(result.text) # type: ignore
-
     print("------------------------------------------------Raw response------------------------------------------------")
 
     results = EasyTL.deepl_translate(text=["Hello, world!", "Goodbye, world!"], target_lang="DE", response_type="raw", logging_directory=logging_directory, decorator=decorator)
     async_results = await EasyTL.deepl_translate_async(text=["Hello, world!", "Goodbye, world!"], target_lang="DE", response_type="raw", logging_directory=logging_directory, decorator=decorator)
 
     for result in results: # type: ignore
         print(result.text) # type: ignore
@@ -133,47 +144,38 @@
     print("------------------------------------------------Google Translate------------------------------------------------")
 
     print("------------------------------------------------Text response------------------------------------------------")
 
     print(EasyTL.googletl_translate("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator))
     print(await EasyTL.googletl_translate_async("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator))
 
-    print(EasyTL.googletl_translate("Hello, world!", target_lang="de", response_type="raw", logging_directory=logging_directory, decorator=decorator)["translatedText"]) # type: ignore
-    result = await EasyTL.googletl_translate_async("Hello, world!", target_lang="de", response_type="raw", logging_directory=logging_directory, decorator=decorator)
-
-    print(result["translatedText"]) # type: ignore
-
     print("------------------------------------------------Raw response------------------------------------------------")
 
     results = EasyTL.googletl_translate(text=["Hello, world!", "Goodbye, world!"], target_lang="de", response_type="raw", logging_directory=logging_directory, decorator=decorator)
     async_results = await EasyTL.googletl_translate_async(text=["Hello, world!", "Goodbye, world!"], target_lang="de", response_type="raw", logging_directory=logging_directory, decorator=decorator)
 
     for result in results: # type: ignore
         print(result["translatedText"]) # type: ignore
 
     for result in async_results: # type: ignore
         print(result["translatedText"]) # type: ignore
+
     print("------------------------------------------------Cost calculation------------------------------------------------")
 
     characters, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="google translate", model=None, translation_instructions=None)
 
     print(f"Characters: {characters}, Cost: {cost}, Model: {model}")
 
     print("------------------------------------------------Gemini------------------------------------------------")
 
     print("-----------------------------------------------Text response-----------------------------------------------")
 
     print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
     print(await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
 
-    print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator).text) # type: ignore
-    result = await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
-
-    print(result.text) # type: ignore
-
     print("-----------------------------------------------Raw response-----------------------------------------------")
 
     results = EasyTL.gemini_translate(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
     async_results = await EasyTL.gemini_translate_async(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory, translation_delay=5,decorator=decorator)
 
     for result in results: # type: ignore
         print(result.text) # type: ignore
@@ -198,19 +200,14 @@
     print("------------------------------------------------OpenAI------------------------------------------------")
 
     print("-----------------------------------------------Text response-----------------------------------------------")
 
     print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
     print(await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
 
-    print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator).choices[0].message.content) # type: ignore
-    result = await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
-
-    print(result.choices[0].message.content) # type: ignore
-
     print("-----------------------------------------------Raw response-----------------------------------------------")
 
     results = EasyTL.openai_translate(text=["Hello, world!", "Goodbye, world!"], model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
     async_results = await EasyTL.openai_translate_async(text=["Hello, world!", "Goodbye, world!"], model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
 
     for result in results: # type: ignore
         print(result.choices[0].message.content) # type: ignore
@@ -232,19 +229,14 @@
     print("------------------------------------------------Anthropic------------------------------------------------")
 
     print("-----------------------------------------------Text response-----------------------------------------------")
 
     print(EasyTL.anthropic_translate("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
     print(await EasyTL.anthropic_translate_async("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
 
-    print(EasyTL.anthropic_translate("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator).content[0].text) # type: ignore
-    result = await EasyTL.anthropic_translate_async("Hello, world!", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
-
-    print(result.content[0].text) # type: ignore
-
     print("-----------------------------------------------Raw response-----------------------------------------------")
 
     results = EasyTL.anthropic_translate(text=["Hello, world!", "Goodbye, world!"], model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
     async_results = await EasyTL.anthropic_translate_async(text=["Hello, world!", "Goodbye, world!"], model="claude-3-haiku-20240307", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
 
     for result in results: # type: ignore
         print(result.content[0].text) # type: ignore
@@ -279,16 +271,14 @@
 
     characters, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="azure", model=None, translation_instructions=None)
 
     print(f"Characters: {characters}, Cost: {cost}, Model: {model}")   
 
 ##-------------------end-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-
-
 if(__name__ == "__main__"):
     ## setup logging
     logging.basicConfig(level=logging.DEBUG, 
                         filename='passing.log',
                         filemode='w', 
                         format='[%(asctime)s] [%(levelname)s] [%(filename)s] %(message)s', 
                         datefmt='%Y-%m-%d %H:%M:%S')
```

### Comparing `easytl-0.4.0b0/tests/simple_test.py` & `easytl-0.4.1/tests/simple_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,31 +18,34 @@
     except:
         pass
 
 ##-------------------start-of-setup_preconditions()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def setup_preconditions():
 
+    ## default values, assuming github actions environment
     gemini_time_delay = 30
 
     deepl_api_key = os.environ.get('DEEPL_API_KEY')
     gemini_api_key = os.environ.get('GEMINI_API_KEY')
     openai_api_key = os.environ.get('OPENAI_API_KEY')
-    anthropic_api_key = os.environ.get('ANTHROPIC_API_KEY')
     json_value = os.environ.get('GOOGLE_TRANSLATE_SERVICE_KEY_VALUE')
+    anthropic_api_key = os.environ.get('ANTHROPIC_API_KEY')
     azure_api_key = os.environ.get('AZURE_API_KEY')
     azure_region = os.environ.get('AZURE_REGION')
 
+    ## this dumps the json value to a file as that's what the google translate service expects
     if(json_value is not None):
 
         with open("json_value.txt", "w") as file:
             file.write(json_value)
 
         google_tl_key_path = "json_value.txt"
 
+    ## the following will replace the keys with local test keys if the environment variables are not set (not a github actions environment)
     logging_directory = os.getenv('LOGGING_DIRECTORY', '/tmp/')
 
     if(deepl_api_key is None):
         deepl_api_key = read_api_key("tests/deepl.txt")
     if(gemini_api_key is None):
         gemini_api_key = read_api_key("tests/gemini.txt")
     if(openai_api_key is None):
@@ -50,35 +53,39 @@
     if(anthropic_api_key is None):
         anthropic_api_key = read_api_key("tests/anthropic.txt")
     if(azure_api_key is None):
         azure_api_key = read_api_key("tests/azure.txt")
     if(azure_region is None):
         azure_region = read_api_key("tests/azure_region.txt")
 
+    ## last json failure clarifies that this is not a github actions environment
     if(json_value is None):
         google_tl_key_path = "tests/google_translate_key.json"
         
         logging_directory = "tests/"
         gemini_time_delay = 5
 
+    ## if any of these trigger, something is wrong (not in local test environment or github actions environment)
     assert deepl_api_key is not None, "DEEPL_API_KEY environment variable must be set"
     assert gemini_api_key is not None, "GEMINI_API_KEY environment variable must be set"
     assert openai_api_key is not None, "OPENAI_API_KEY environment variable must be set"
     assert anthropic_api_key is not None, "ANTHROPIC_API_KEY environment variable must be set"
     assert azure_api_key is not None, "AZURE_API_KEY environment variable must be set"
     assert azure_region is not None, "AZURE_REGION environment variable must be set"
     assert google_tl_key_path is not None, "GOOGLE_TRANSLATE_SERVICE_KEY_VALUE environment variable must be set"
 
+    ## set the credentials for the services
     EasyTL.set_credentials("deepl", deepl_api_key)
     EasyTL.set_credentials("gemini", gemini_api_key)
     EasyTL.set_credentials("openai", openai_api_key)
     EasyTL.set_credentials("anthropic", anthropic_api_key)
     EasyTL.set_credentials("google translate", google_tl_key_path)
     EasyTL.set_credentials("azure", azure_api_key)
 
+    ## schema for gemini & anthropic
     schema = {
         "type": "object",
         "properties": {
             "input": {
                 "type": "string",
                 "description": "The text you were given to translate"
             },
@@ -112,29 +119,16 @@
                 "description": "The translated text"
             }
         },
         "required": ["input", "output"]
     }
 
     # print(EasyTL.anthropic_translate("Hello, world!", translation_instructions="Translate this to German.", response_type="json", logging_directory=logging_directory,decorator=decorator, response_schema=schema))
-    # print(await EasyTL.anthropic_translate_async("Hello, world!", translation_instructions="Translate this to German.", response_type="json", logging_directory=logging_directory,decorator=decorator, response_schema=schema))
-
-    #tokens, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="anthropic", model="claude-3-haiku-20240307", translation_instructions="Translate this to German.")
-
-    print("------------------------------------------------Azure------------------------------------------------")
-    
-    print("-----------------------------------------------Text response-----------------------------------------------")
-
-    print(EasyTL.azure_translate("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator, azure_region=azure_region))
-    print(await EasyTL.azure_translate_async("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator, azure_region=azure_region))
-
-    print("-----------------------------------------------JSON response-----------------------------------------------")
 
-    print(EasyTL.azure_translate("Hello, world!", target_lang="de", response_type="json", logging_directory=logging_directory,decorator=decorator, azure_region=azure_region))
-    print(await EasyTL.azure_translate_async("Hello, world!", target_lang="de", response_type="json", logging_directory=logging_directory,decorator=decorator, azure_region=azure_region))
+    ## print(EasyTL.azure_translate("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator, azure_region=azure_region))
 
  ##   print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo-0125", translation_instructions="Translate this to German in json format.", response_type="json", logging_directory=logging_directory,decorator=decorator))
 
 ##    print(EasyTL.deepl_translate("Hello, world!", target_lang="DE", response_type="text", logging_directory=logging_directory,decorator=decorator))
 
  ##   print(EasyTL.googletl_translate("Hello, world!", target_lang="de", response_type="text", logging_directory=logging_directory,decorator=decorator))
```

