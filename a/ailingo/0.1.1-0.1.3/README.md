# Comparing `tmp/ailingo-0.1.1.tar.gz` & `tmp/ailingo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailingo-0.1.1.tar", max compression
+gzip compressed data, was "ailingo-0.1.3.tar", max compression
```

## Comparing `ailingo-0.1.1.tar` & `ailingo-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-05-27 15:01:46.422200 ailingo-0.1.1/LICENSE
--rw-r--r--   0        0        0     7749 2024-05-27 15:01:46.422200 ailingo-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-27 15:01:46.422200 ailingo-0.1.1/ailingo/__init__.py
--rw-r--r--   0        0        0     4476 2024-05-27 15:01:46.422200 ailingo-0.1.1/ailingo/cli.py
--rw-r--r--   0        0        0     2200 2024-05-27 15:01:46.422200 ailingo-0.1.1/ailingo/file_manager.py
--rw-r--r--   0        0        0     1010 2024-05-27 15:01:46.422200 ailingo-0.1.1/ailingo/llm.py
--rw-r--r--   0        0        0     6837 2024-05-27 15:01:46.422200 ailingo-0.1.1/ailingo/translator.py
--rw-r--r--   0        0        0      487 2024-05-27 15:01:46.422200 ailingo-0.1.1/ailingo/utils.py
--rw-r--r--   0        0        0      938 2024-05-27 15:01:46.426200 ailingo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8651 1970-01-01 00:00:00.000000 ailingo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-06-01 05:37:11.106830 ailingo-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7891 2024-06-01 05:37:11.106830 ailingo-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-06-01 05:37:11.106830 ailingo-0.1.3/ailingo/__init__.py
+-rw-r--r--   0        0        0     4962 2024-06-01 05:37:11.106830 ailingo-0.1.3/ailingo/cli.py
+-rw-r--r--   0        0        0     2200 2024-06-01 05:37:11.106830 ailingo-0.1.3/ailingo/file_manager.py
+-rw-r--r--   0        0        0     1010 2024-06-01 05:37:11.106830 ailingo-0.1.3/ailingo/llm.py
+-rw-r--r--   0        0        0     7016 2024-06-01 05:37:11.106830 ailingo-0.1.3/ailingo/translator.py
+-rw-r--r--   0        0        0      269 2024-06-01 05:37:11.106830 ailingo-0.1.3/ailingo/utils.py
+-rw-r--r--   0        0        0     1061 2024-06-01 05:37:11.110830 ailingo-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8969 1970-01-01 00:00:00.000000 ailingo-0.1.3/PKG-INFO
```

### Comparing `ailingo-0.1.1/LICENSE` & `ailingo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ailingo-0.1.1/README.md` & `ailingo-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,18 @@
   <a href="./README.md">English</a> |
   <a href="./README.ja.md">日本語</a> |
   <a href="./README.zh-CN.md">简体中文</a> |
   <a href="./README.zh-TW.md">繁体中文</a> |
   <a href="./README.es.md">Español</a>
 </p>
 
+<p align="center">
+    <img alt="example" src="https://github.com/yamitzky/ailingo/assets/623449/faae1265-9ab6-4df5-a787-23e73fff9778">
+</p>
+
 NOTICE: This document was automatically generated using ailingo.
 
 ## Overview
 
 It is designed to enable developers, translators, and content creators to efficiently localize their files.
 
 **Key Features:**
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 # ailingo: A CLI tool for translating local files using generative AI (LLM)
 **ailingo** is a command-line interface (CLI) tool that uses generative AI to
 translate local files into various languages.
                           _[_R_e_l_e_a_s_e_s_]_[_C_I_]_[_M_I_T_ _L_i_c_e_n_s_e_]
          _E_n_g_l_i_s_h | _æ__¥_æ__¬_è_ª_ | _ç_®__ä_½__ä_¸_­_æ__ | _ç_¹__ä_½__ä_¸_­_æ__ | _E_s_p_a_Ã_±_o_l
+                                   [example]
 NOTICE: This document was automatically generated using ailingo. ## Overview It
 is designed to enable developers, translators, and content creators to
 efficiently localize their files. **Key Features:** - **Flexible file handling:
 ** Translate multiple files at once. - **Wide language support:** Freely
 specify the source and target languages. - **Generative AI model selection:**
 Choose from various generative AI models available through litellm, including
 ChatGPT, Gemini, and Anthropic. - **Customizable output:** Control the names
```

### Comparing `ailingo-0.1.1/ailingo/cli.py` & `ailingo-0.1.3/ailingo/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import logging
+from logging import getLogger
 import os
 import subprocess
 import tempfile
 
 import typer
 from ailingo.translator import DEFAULT_OUTPUT_PATTERN, Translator
+from ailingo.utils import setup_logger
 from rich import print
 from rich.console import Console
 
 app = typer.Typer()
 
 err_console = Console(stderr=True)
+logger = getLogger(__name__)
 
 
 @app.command()
 def translate(
     file_paths: list[str] = typer.Argument(
         default=None, help="Input file(s) to translate."
     ),
@@ -52,18 +56,25 @@
     edit: bool = typer.Option(False, "-e", "--edit", help="Edit mode."),
     dryrun: bool = typer.Option(
         False, "--dry-run", help="Perform a trial run with no changes made."
     ),
     quiet: bool = typer.Option(
         False, "-q", "--quiet", help="Suppress all output messages."
     ),
+    debug: bool = typer.Option(False, "--debug", help="Enable debug mode."),
 ) -> None:
     """
     Translates the specified files.
     """
+    setup_logger(logging.DEBUG if debug else None)
+    if debug:
+        logger.debug("Debug mode enabled.")
+    if dryrun:
+        logger.debug("Dry run enabled.")
+
     if target_languages_str:
         target_languages = target_languages_str.split(",")
     else:
         target_languages = []
 
     translator = Translator(model_name=model_name)
 
@@ -75,14 +86,15 @@
     if edit and len(target_languages) > 1:
         raise typer.BadParameter(
             "Multiple target languages cannot be specified in edit mode."
         )
 
     # edit mode
     if edit:
+        logger.debug("Edit mode enabled.")
         no_temp_file = bool(dryrun or output_pattern)
         with (
             tempfile.NamedTemporaryFile(mode="w+", suffix=".txt") as input,
             tempfile.NamedTemporaryFile(
                 mode="w+", suffix=".txt", delete=no_temp_file
             ) as output,
         ):
@@ -100,28 +112,30 @@
             )
             output.seek(0)
             print(output.read())
         return
 
     # rewrite mode
     if not target_languages:
+        logger.debug("Rewrite mode enabled.")
         for file_path in file_paths:
             translator.translate(
                 file_path=file_path,
                 source_language=source_language,
                 target_language=None,
                 output_pattern=output_pattern,
                 overwrite=overwrite,
                 dryrun=dryrun,
                 request=request,
                 quiet=quiet,
             )
         return
 
     # normal mode
+    logger.debug("Normal mode enabled.")
     for file_path in file_paths:
         for target_language in target_languages:
             translator.translate(
                 file_path=file_path,
                 source_language=source_language,
                 target_language=target_language,
                 output_pattern=output_pattern,
```

### Comparing `ailingo-0.1.1/ailingo/file_manager.py` & `ailingo-0.1.3/ailingo/file_manager.py`

 * *Files identical despite different names*

### Comparing `ailingo-0.1.1/ailingo/llm.py` & `ailingo-0.1.3/ailingo/llm.py`

 * *Files identical despite different names*

### Comparing `ailingo-0.1.1/ailingo/translator.py` & `ailingo-0.1.3/ailingo/translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from pathlib import Path
+from logging import getLogger
 
 from ailingo.file_manager import FileManager
 from ailingo.llm import LLM
-from ailingo.utils import setup_logger
 from rich import print
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.prompt import Confirm
 
-logger = setup_logger(__name__)
+logger = getLogger(__name__)
 
 
 DEFAULT_OUTPUT_PATTERN = "{parent}/{stem}.{target}{suffix}"
 
 
 class Translator:
     def __init__(
         self,
         model_name: str,
         file_manager: FileManager | None = None,
         llm: LLM | None = None,
     ) -> None:
         self.file_manager = file_manager or FileManager()
         self.llm = llm or LLM(model_name)
+        self.model_name = model_name
 
     def translate(
         self,
         file_path: str,
         target_language: str | None = None,
         output_pattern: str | None = None,
         source_language: str | None = None,
@@ -173,14 +174,18 @@
                 "You are a writer who rewrites text.\n"
                 "Please rewrite the provided text to make it more natural without changing the original meaning.\n"
                 "As a native speaker, correct any spelling, grammar, or terminology errors.\n"
                 "Only output the result. Do not output any related comments and code blocks.\n"
                 "Never translate. Don't change the language. Please respect the original language.\n"
                 "Please follow the information below for reference.\n"
             )
+        prompt = base_prompt + "\n".join(hints)
+        logger.debug(f"Model: {self.model_name}")
+        logger.debug(f"Prompt: {prompt}")
+        logger.debug(f"Text: {text}")
         response = self.llm.completion(
             [
-                {"role": "system", "content": base_prompt + "\n".join(hints)},
+                {"role": "system", "content": prompt},
                 {"role": "user", "content": text},
             ],
         )
         return response
```

### Comparing `ailingo-0.1.1/pyproject.toml` & `ailingo-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "ailingo"
-version = "0.1.1"
+version = "0.1.3"
 description = "A CLI Tool for Local File Translation Using Generative AI(LLMs)"
 authors = ["Mitsuki Ogasahara <negiga@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 litellm = "^1.38.8"
 typer = "^0.12.3"
 rich = "^13.7.1"
 google-cloud-aiplatform = { version = "^1.52.0", optional = true }
 google-generativeai = { version = "^0.5.4", optional = true }
 boto3 = { version = ">=1.28.57", optional = true }
 
+instructor = "^1.3.2"
+anthropic = {extras = ["vertex"], version = "^0.28.0", optional = true }
 [tool.poetry.extras]
 google = ["google-cloud-aiplatform", "google-generativeai"]
+anthropic-vertex = ["anthropic"]
 aws = ["boto3"]
-all = ["google-cloud-aiplatform", "google-generativeai", "boto3"]
+all = ["google-cloud-aiplatform", "google-generativeai", "boto3", "anthropic"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.5"
 pyright = "^1.1.364"
 pytest = "^8.2.1"
 
 pytest-cov = "^5.0.0"
-black = "^24.4.2"
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ailingo = "ailingo.cli:app"
```

### Comparing `ailingo-0.1.1/PKG-INFO` & `ailingo-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: ailingo
-Version: 0.1.1
+Version: 0.1.3
 Summary: A CLI Tool for Local File Translation Using Generative AI(LLMs)
 License: MIT
 Author: Mitsuki Ogasahara
 Author-email: negiga@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
+Provides-Extra: anthropic-vertex
 Provides-Extra: aws
 Provides-Extra: google
+Requires-Dist: anthropic[vertex] (>=0.28.0,<0.29.0) ; extra == "anthropic-vertex" or extra == "all"
 Requires-Dist: boto3 (>=1.28.57) ; extra == "aws" or extra == "all"
 Requires-Dist: google-cloud-aiplatform (>=1.52.0,<2.0.0) ; extra == "google" or extra == "all"
 Requires-Dist: google-generativeai (>=0.5.4,<0.6.0) ; extra == "google" or extra == "all"
+Requires-Dist: instructor (>=1.3.2,<2.0.0)
 Requires-Dist: litellm (>=1.38.8,<2.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 # ailingo: A CLI tool for translating local files using generative AI (LLM)
 
@@ -38,14 +41,18 @@
   <a href="./README.md">English</a> |
   <a href="./README.ja.md">日本語</a> |
   <a href="./README.zh-CN.md">简体中文</a> |
   <a href="./README.zh-TW.md">繁体中文</a> |
   <a href="./README.es.md">Español</a>
 </p>
 
+<p align="center">
+    <img alt="example" src="https://github.com/yamitzky/ailingo/assets/623449/faae1265-9ab6-4df5-a787-23e73fff9778">
+</p>
+
 NOTICE: This document was automatically generated using ailingo.
 
 ## Overview
 
 It is designed to enable developers, translators, and content creators to efficiently localize their files.
 
 **Key Features:**
```

#### html2text {}

```diff
@@ -1,24 +1,28 @@
-Metadata-Version: 2.1 Name: ailingo Version: 0.1.1 Summary: A CLI Tool for
+Metadata-Version: 2.1 Name: ailingo Version: 0.1.3 Summary: A CLI Tool for
 Local File Translation Using Generative AI(LLMs) License: MIT Author: Mitsuki
 Ogasahara Author-email: negiga@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: all
-Provides-Extra: aws Provides-Extra: google Requires-Dist: boto3 (>=1.28.57) ;
-extra == "aws" or extra == "all" Requires-Dist: google-cloud-aiplatform
-(>=1.52.0,<2.0.0) ; extra == "google" or extra == "all" Requires-Dist: google-
-generativeai (>=0.5.4,<0.6.0) ; extra == "google" or extra == "all" Requires-
-Dist: litellm (>=1.38.8,<2.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: typer (>=0.12.3,<0.13.0) Description-Content-Type: text/markdown
-# ailingo: A CLI tool for translating local files using generative AI (LLM)
-**ailingo** is a command-line interface (CLI) tool that uses generative AI to
-translate local files into various languages.
+Provides-Extra: anthropic-vertex Provides-Extra: aws Provides-Extra: google
+Requires-Dist: anthropic[vertex] (>=0.28.0,<0.29.0) ; extra == "anthropic-
+vertex" or extra == "all" Requires-Dist: boto3 (>=1.28.57) ; extra == "aws" or
+extra == "all" Requires-Dist: google-cloud-aiplatform (>=1.52.0,<2.0.0) ; extra
+== "google" or extra == "all" Requires-Dist: google-generativeai
+(>=0.5.4,<0.6.0) ; extra == "google" or extra == "all" Requires-Dist:
+instructor (>=1.3.2,<2.0.0) Requires-Dist: litellm (>=1.38.8,<2.0.0) Requires-
+Dist: rich (>=13.7.1,<14.0.0) Requires-Dist: typer (>=0.12.3,<0.13.0)
+Description-Content-Type: text/markdown # ailingo: A CLI tool for translating
+local files using generative AI (LLM) **ailingo** is a command-line interface
+(CLI) tool that uses generative AI to translate local files into various
+languages.
                           _[_R_e_l_e_a_s_e_s_]_[_C_I_]_[_M_I_T_ _L_i_c_e_n_s_e_]
          _E_n_g_l_i_s_h | _æ__¥_æ__¬_è_ª_ | _ç_®__ä_½__ä_¸_­_æ__ | _ç_¹__ä_½__ä_¸_­_æ__ | _E_s_p_a_Ã_±_o_l
+                                   [example]
 NOTICE: This document was automatically generated using ailingo. ## Overview It
 is designed to enable developers, translators, and content creators to
 efficiently localize their files. **Key Features:** - **Flexible file handling:
 ** Translate multiple files at once. - **Wide language support:** Freely
 specify the source and target languages. - **Generative AI model selection:**
 Choose from various generative AI models available through litellm, including
 ChatGPT, Gemini, and Anthropic. - **Customizable output:** Control the names
```

