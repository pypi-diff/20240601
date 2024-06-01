# Comparing `tmp/ragtime-0.0.39.tar.gz` & `tmp/ragtime-0.0.40.tar.gz`

## Comparing `ragtime-0.0.39.tar` & `ragtime-0.0.40.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 ragtime-0.0.39/CHANGELOG.md
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 ragtime-0.0.39/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.39/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.39/img/Ragtime_logo.png
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/__init__.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base.py
--rw-r--r--   0        0        0     8910 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/config.py
--rw-r--r--   0        0        0    23158 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/expe.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/pipeline.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
--rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
--rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
--rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/__init__.py
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/answer_generator.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/eval_generator.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/fact_generator.py
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/generators/text_generator.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/llms/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/llms/lite_llm.py
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/llms/llm.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/__init__.py
--rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/answer_prompters.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/eval_prompters.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/fact_prompters.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/prompters/prompter.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/retrievers/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ragtime-0.0.39/src/ragtime/retrievers/retriever.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.39/tests/full_test.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.39/tests/run_tests.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.39/tests/test_quest.json
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.39/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.39/LICENSE
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.39/README.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ragtime-0.0.39/pyproject.toml
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 ragtime-0.0.39/PKG-INFO
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 ragtime-0.0.40/CHANGELOG.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 ragtime-0.0.40/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.40/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.40/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base.py
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/config.py
+-rw-r--r--   0        0        0    23173 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/expe.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/pipeline.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
+-rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
+-rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
+-rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/generators/__init__.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/generators/answer_generator.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/generators/eval_generator.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/generators/fact_generator.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/generators/question_generator.py
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/generators/text_generator.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/llms/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/llms/lite_llm.py
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/llms/llm.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/prompters/__init__.py
+-rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/prompters/answer_prompters.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/prompters/eval_prompters.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/prompters/fact_prompters.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/prompters/prompter.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/prompters/question_prompters.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/retrievers/__init__.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/retrievers/indexer.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ragtime-0.0.40/src/ragtime/retrievers/retriever.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.40/tests/full_test.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.40/tests/run_tests.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.40/tests/test_quest.json
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.40/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.40/LICENSE
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.40/README.md
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ragtime-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 ragtime-0.0.40/PKG-INFO
```

### Comparing `ragtime-0.0.39/CHANGELOG.md` & `ragtime-0.0.40/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# v0.0.40 - June 1st 2024
+- updated prompt in FactPrompterFR to make facts more atomic - seems to work better after a sanity check on Google NQ
+
 # v0.0.39
 - packages hierarchy updated
 - prompters renamed
 - pipeline in progress
 
 # v0.0.38
 - Fully functionnal pipeline described as a dictionary
```

### Comparing `ragtime-0.0.39/CONTRIBUTING.md` & `ragtime-0.0.40/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/img/Ragtime_logo.png` & `ragtime-0.0.40/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/__init__.py` & `ragtime-0.0.40/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base.py` & `ragtime-0.0.40/src/ragtime/base.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/config.py` & `ragtime-0.0.40/src/ragtime/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 #################################
 
 # # # FOLDERS
 QUESTIONS_FOLDER_NAME: str = "01. Questions"
 ANSWERS_FOLDER_NAME: str = "02. Answers"
 FACTS_FOLDER_NAME: str = "03. Facts"
 EVALS_FOLDER_NAME: str = "04. Evals"
+DATASETS_FOLDER_NAME : str = "datasets"
+DOCUMENTS_FOLDER_NAME : str = "documents"
 ROOT_FOLDER: Path = ROOT_FOLDER if "ROOT_FOLDER" in globals() else None
 FOLDER_EXPE: Path = FOLDER_EXPE if "FOLDER_EXPE" in globals() else None
 FOLDER_QUESTIONS: Path = FOLDER_QUESTIONS if "FOLDER_QUESTIONS" in globals() else None
 FOLDER_ANSWERS: Path = FOLDER_ANSWERS if "FOLDER_ANSWERS" in globals() else None
 FOLDER_FACTS: Path = FOLDER_FACTS if "FOLDER_FACTS" in globals() else None
 FOLDER_EVALS: Path = FOLDER_EVALS if "FOLDER_EVALS" in globals() else None
 FOLDER_TEMPLATES: Path = FOLDER_TEMPLATES if "FOLDER_TEMPLATES" in globals() else None
```

### Comparing `ragtime-0.0.39/src/ragtime/expe.py` & `ragtime-0.0.40/src/ragtime/expe.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,14 @@
 
 from enum import Enum, IntEnum
 from datetime import datetime
 from typing import Any, Generic, Optional, TypeVar, Union
 from enum import IntEnum
 
 
-class Question(RagtimeText):
-    pass
-
-
-class Questions(RagtimeList[Question]):
-    pass
-
 
 class Prompt(RagtimeBase):
     user: Optional[str] = ""
     system: Optional[str] = ""
 
 
 class LLMAnswer(RagtimeText):
@@ -63,14 +56,21 @@
     duration: Optional[float] = None  # time to get the answer in seconds
     cost: Optional[float] = None
 
 
 class WithLLMAnswer(BaseModel):
     llm_answer: Optional[LLMAnswer] = None
 
+class Question(RagtimeText, WithLLMAnswer):
+    pass
+
+
+class Questions(RagtimeList[Question]):
+    pass
+
 
 class Eval(RagtimeText, WithLLMAnswer):
     """At first an Eval is made by a human, and then automatically generated from an LLM Answer"""
 
     human: Optional[float] = None
     auto: Optional[float] = None
```

### Comparing `ragtime-0.0.39/src/ragtime/pipeline.py` & `ragtime-0.0.40/src/ragtime/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from ragtime.llms import LLM, LiteLLM
 from ragtime.prompters.prompter import Prompter
 from ragtime.retrievers.retriever import Retriever
 from ragtime.generators import AnsGenerator, FactGenerator, EvalGenerator
 from ragtime.expe import StartFrom
 
-# from ragtime.generators import *
+from ragtime.base import RagtimeException
 from ragtime.expe import Expe
 from ragtime.config import (
-    RagtimeException,
     FOLDER_ANSWERS,
     FOLDER_FACTS,
     FOLDER_EVALS,
     DEFAULT_HTML_TEMPLATE,
     DEFAULT_SPREADSHEET_TEMPLATE,
 )
 
@@ -36,19 +35,18 @@
 def run_pipeline(
     configuration: dict, start_from: str = None, stop_after: str = None
 ) -> dict:
     # Check if there is a folder and file name for a starting point
     # TODO: refacto the error handling + check if the folder and the file exist
     input_folder: Union[Path, str] = configuration.get("folder_name", None)
     if not input_folder:
-        raise Exception("You must provide starting point folder")
+        raise Exception("You must provide a starting point folder")
     file_name: str = configuration.get("file_name", None)
     if not file_name:
-        raise Exception("You must provide starting point file name")
-    output_folder: Union[Path, str]
+        raise Exception("You must provide a starting point file name")
 
     # This table HO function are helper to instanciate the classe and methode call from a dictionary
     # TODO: break down this implementation to a PipelineConfiguration class
     #       to split the error handling from the config file and the implementation details
     #       of the pipeline implementation
     generator_table: dict[str, dict] = {
         "answers": {
@@ -72,16 +70,17 @@
     # Check is the generator suite is present
     # TODO: refacto error handling
     if not configuration.get("generate", None):
         raise Exception("The pipeline must provide a generator suite")
 
     steps: list[str] = ["answers", "facts", "evals"]
     b = steps.index(start_from if start_from in steps else steps[0])
-    e = steps.index(stop_after if stop_after in steps else steps[-1], b)
+    e = steps.index(stop_after if stop_after in steps else steps[-1], b) + 1
 
+    output_folder: Union[Path, str]
     # loop through the step of the pipeline in this specific order
     for step in steps[b:e]:
         # Skip if the step is not defined
         # NOTE: I think there is a better way to express this behavior
         step_conf: dict = configuration["generate"].get(step, None)
         if not step_conf:
             continue
@@ -115,42 +114,35 @@
             expe,
             only_llms=step_conf.get("only_llms", None),
             save_every=step_conf.get("save_every", 0),
             start_from=step_conf.get("start_from", StartFrom.beginning),
             b_missing_only=step_conf.get("b_missing_only", False),
         )
 
+        written_at: Path = expe.save_to_json(path=output_folder / file_name)
+
         # Check if export is provided
         exports_format = step_conf.get("export", None)
-        if not exports_format:
-            continue
-
-        exporter_table = {
-            "json": (
-                lambda template_path: expe.save_to_json(path=output_folder / file_name)
-            ),
-            "html": (
-                lambda template_path: expe.save_to_html(
-                    path=output_folder / file_name,
-                    template_path=(DEFAULT_HTML_TEMPLATE, template_path)[
-                        bool(template_path)
-                    ],
-                )
-            ),
-            "spreadsheet": (
-                lambda template_path: expe.save_to_spreadsheet(
-                    path=output_folder / file_name,
-                    template_path=(DEFAULT_SPREADSHEET_TEMPLATE, template_path)[
-                        bool(template_path)
-                    ],
-                )
-            ),
-        }
-        # Run the export with the parameter provided
-        for fmt in ["json", "html", "spreadsheet"]:
-            fmt_parameters = exports_format.get(fmt, None)
-            if fmt_parameters is None:
-                continue
-            exporter_table[fmt](fmt_parameters.get("path", None))
-
+        if exports_format:
+            exporter_table = {
+                "html": (
+                    lambda template_path: expe.save_to_html(
+                        path=output_folder / file_name,
+                        template_path=(template_path or DEFAULT_HTML_TEMPLATE),
+                    )
+                ),
+                "spreadsheet": (
+                    lambda template_path: expe.save_to_spreadsheet(
+                        path=output_folder / file_name,
+                        template_path=(template_path or DEFAULT_SPREADSHEET_TEMPLATE),
+                    )
+                ),
+            }
+            # Run the export with the parameter provided
+            for fmt in ["html", "spreadsheet"]:
+                fmt_parameters = exports_format.get(fmt, None)
+                if fmt_parameters is None:
+                    continue
+                exporter_table[fmt](fmt_parameters.get("path", None))
         # Update the next input folder with the current output folder
-        input_folder = output_folder
+        input_folder = written_at.parent
+        file_name = written_at.name
```

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.40/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.40/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/classes.py` & `ragtime-0.0.40/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/main.py` & `ragtime-0.0.40/src/ragtime/base_folder/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.40/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.40/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx` & `ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx` & `ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx` & `ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx` & `ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx` & `ragtime-0.0.40/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/generators/answer_generator.py` & `ragtime-0.0.40/src/ragtime/generators/answer_generator.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/generators/eval_generator.py` & `ragtime-0.0.40/src/ragtime/generators/eval_generator.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/generators/fact_generator.py` & `ragtime-0.0.40/src/ragtime/generators/fact_generator.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/generators/text_generator.py` & `ragtime-0.0.40/src/ragtime/generators/text_generator.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/llms/llm.py` & `ragtime-0.0.40/src/ragtime/llms/llm.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/prompters/answer_prompters.py` & `ragtime-0.0.40/src/ragtime/prompters/answer_prompters.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/prompters/eval_prompters.py` & `ragtime-0.0.40/src/ragtime/prompters/eval_prompters.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 class EvalPrompterFR(Prompter):
     """
     Prompt: FAITS and REPONSE - expect the REPONSE to be rewritten including the FACTS in the text
     Post_process: analyse cited factsfacts not cited, and facts invented (?)
     """
 
-    system:str = """Tu dois comparer une liste numérotée de FAITS avec une REPONSE.
+    system: str = """Tu dois comparer une liste numérotée de FAITS avec une REPONSE.
         Tu dois reprendre exactement la REPONSE en insérant dans le texte le numéro du FAIT auquel correspond exactement le passage ou la phrase.
         Si la phrase correspond à plusieurs FAITS, indique les entre parenthèses.
         Il ne faut pas insérer le FAIT s'il est en contradiction avec le passage ou la phrase.
         Si un passage ou une phrase dans la REPONSE ne correspond à aucun FAIT il faut mettre un point d'interrogation entre parenthèses (?)
         sauf si ce passage fait référence à un emplacement dans le document, auquel cas il ne faut rien indiquer."""
-    
+
     def get_prompt(self, answer: Answer, facts: Facts) -> Prompt:
         result: Prompt = Prompt()
         facts_as_str: str = "\n".join(
             f"{i}. {fact.text}" for i, fact in enumerate(facts, start=1)
         )
         result.user = f"-- FAITS --\n{facts_as_str}\n\n-- REPONSE --\n{answer.text}"
         result.system = self.system
@@ -56,12 +56,12 @@
         precision: float = div0(
             len(true_facts_in_answer), len(facts_in_answer) + nb_false_facts_in_answer
         )
         recall: float = div0(len(true_facts_in_answer), len(true_facts))
         cur_obj.meta["precision"] = precision
         cur_obj.meta["recall"] = recall
         cur_obj.meta["hallus"] = nb_false_facts_in_answer
-        cur_obj.meta["missing"] = ", ".join(list(true_facts_not_in_answer))
+        cur_obj.meta["missing"] = ", ".join([str(v) for v in true_facts_not_in_answer])
         cur_obj.meta["nb_missing"] = len(cur_obj.meta["missing"])
         cur_obj.meta["facts_in_ans"] = str(sorted(facts_in_answer))
         cur_obj.auto = div0(2 * precision * recall, precision + recall)
         cur_obj.text = answer
```

### Comparing `ragtime-0.0.39/src/ragtime/prompters/fact_prompters.py` & `ragtime-0.0.40/src/ragtime/prompters/fact_prompters.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 class FactPrompterFR(Prompter):
     """
     New version of Facts Prompters
     Asks for 1 to 5 facts in French
     """
 
     system:str = """Génère un minimum de phrases numérotées courtes et simples qui décrivent ce paragraphe.
-        Chaque phrase doit être indépendante et aucune phrase ne doit contenir la même information qu'une autre phrase.
-        Les phrases ne doivent pas contenir de référence au document source ni à sa page.
-        Les phrases doivent être compréhensibles seules et donc ne pas contenir de référence aux autres phrases ni nécessiter les autres phrases pour être comprises."""
+# Chaque phrase ne doit contenir qu'une seule information.
+# Chaque phrase doit être indépendante et aucune phrase ne doit contenir la même information qu'une autre phrase.
+# Les phrases ne doivent pas contenir de référence au document source ni à sa page.
+# Les phrases doivent être compréhensibles seules et donc ne pas contenir de référence aux autres phrases ni nécessiter les autres phrases pour être comprises."""
 
     def get_prompt(self, answer: Answer) -> Prompt:
         result: Prompt = Prompt()
         result.user = f"{answer.text}"
         result.system = self.system
         return result
```

### Comparing `ragtime-0.0.39/src/ragtime/prompters/prompter.py` & `ragtime-0.0.40/src/ragtime/prompters/prompter.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/src/ragtime/retrievers/retriever.py` & `ragtime-0.0.40/src/ragtime/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/tests/full_test.py` & `ragtime-0.0.40/tests/full_test.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/tests/run_tests.py` & `ragtime-0.0.40/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/tests/test_quest.json` & `ragtime-0.0.40/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/.gitignore` & `ragtime-0.0.40/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/LICENSE` & `ragtime-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/README.md` & `ragtime-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.39/pyproject.toml` & `ragtime-0.0.40/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.39"
+version = "0.0.40"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
@@ -21,12 +21,12 @@
     "Operating System :: OS Independent",
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["RAG", "LLM", "Evaluation"]
 dependencies = ['requests', 'retry', 'pathlib', 'openpyxl', 'langdetect',
 'pydantic', 'jinja2', 'tabulate', 'unidecode', 'litellm', 'setenv', 'py_setenv', 'lazy_import',
-'asyncio', 'toml']
+'asyncio', 'llama_index']
 
 [project.urls]
 Homepage = "https://github.com/recitalAI/ragtime-package"
 Issues = "https://github.com/recitalAI/ragtime-package/issues"
```

### Comparing `ragtime-0.0.39/PKG-INFO` & `ragtime-0.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.39
+Version: 0.0.40
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
         
@@ -35,23 +35,23 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: asyncio
 Requires-Dist: jinja2
 Requires-Dist: langdetect
 Requires-Dist: lazy-import
 Requires-Dist: litellm
+Requires-Dist: llama-index
 Requires-Dist: openpyxl
 Requires-Dist: pathlib
 Requires-Dist: py-setenv
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: retry
 Requires-Dist: setenv
 Requires-Dist: tabulate
-Requires-Dist: toml
 Requires-Dist: unidecode
 Description-Content-Type: text/markdown
 
 <img src="img/Ragtime_logo.png" alt="Ragtime 🎹 LLM Ops for all">
 
 # Presentation
 **Ragtime** 🎹 is an LLMOps framework which allows you to automatically:
```

