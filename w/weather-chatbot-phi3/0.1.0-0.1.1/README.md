# Comparing `tmp/weather_chatbot_phi3-0.1.0.tar.gz` & `tmp/weather_chatbot_phi3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_chatbot_phi3-0.1.0.tar", max compression
+gzip compressed data, was "weather_chatbot_phi3-0.1.1.tar", max compression
```

## Comparing `weather_chatbot_phi3-0.1.0.tar` & `weather_chatbot_phi3-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0        0 2024-06-01 13:36:28.802748 weather_chatbot_phi3-0.1.0/README.md
--rw-r--r--   0        0        0      624 2024-06-01 14:03:03.269675 weather_chatbot_phi3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 13:49:27.073368 weather_chatbot_phi3-0.1.0/weather_chatbot/__init__.py
--rw-r--r--   0        0        0     3147 2024-06-01 13:36:28.802748 weather_chatbot_phi3-0.1.0/weather_chatbot/app.py
--rw-r--r--   0        0        0      994 2024-06-01 13:36:28.804747 weather_chatbot_phi3-0.1.0/weather_chatbot/push_model.py
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 weather_chatbot_phi3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-06-01 13:36:28.802748 weather_chatbot_phi3-0.1.1/README.md
+-rw-r--r--   0        0        0      624 2024-06-01 19:23:20.665655 weather_chatbot_phi3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-06-01 19:12:51.845137 weather_chatbot_phi3-0.1.1/weather_chatbot/__init__.py
+-rw-r--r--   0        0        0     2938 2024-06-01 19:13:13.282549 weather_chatbot_phi3-0.1.1/weather_chatbot/app.py
+-rw-r--r--   0        0        0      423 2024-06-01 19:12:34.753201 weather_chatbot_phi3-0.1.1/weather_chatbot/download_model.py
+-rw-r--r--   0        0        0     1094 2024-06-01 18:29:15.517301 weather_chatbot_phi3-0.1.1/weather_chatbot/push_model.py
+-rw-r--r--   0        0        0       34 2024-06-01 18:29:15.518301 weather_chatbot_phi3-0.1.1/weather_chatbot/requirements.txt
+-rw-r--r--   0        0        0      196 2024-06-01 18:29:15.518301 weather_chatbot_phi3-0.1.1/weather_chatbot/style.css
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 weather_chatbot_phi3-0.1.1/PKG-INFO
```

### Comparing `weather_chatbot_phi3-0.1.0/pyproject.toml` & `weather_chatbot_phi3-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weather-chatbot-phi3"
-version = "0.1.0"
+version = "0.1.1"
 description = "An LLM Chatbot integrated with Open Weather API for Real-Time Weather Information."
 authors = ["Vatsal Patel <vatsal1804@gmail.com>"]
 license = "CC-BY-NC-SA-4.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `weather_chatbot_phi3-0.1.0/weather_chatbot/app.py` & `weather_chatbot_phi3-0.1.1/weather_chatbot/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,14 @@
 import gradio as gr
 from llama_cpp import Llama
 import requests
 import huggingface_hub
 
 # Download model from Hugging Face if not already present
 model_path = "./model/phi-3-gguf/Phi-3-mini-4k-instruct-q4.gguf"
-if not os.path.exists(model_path):
-    huggingface_hub.hf_hub_download(
-        repo_id="VatsalPatel18/phi3-mini-WeatherBot",
-        filename="Phi-3-mini-4k-instruct-gguf",
-        local_dir=model_path
-    )
 
 # Initialize the Llama model
 llm = Llama(
     model_path=model_path,
     n_ctx=4096,
     n_threads=8,
     n_gpu_layers=0,
```

### Comparing `weather_chatbot_phi3-0.1.0/weather_chatbot/push_model.py` & `weather_chatbot_phi3-0.1.1/weather_chatbot/push_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from huggingface_hub import HfApi, create_repo, upload_file
 
 # Set your repository details
 repo_name = "phi3-mini-WeatherBot"
 repo_id = f"VatsalPatel18/{repo_name}"
-local_dir = "./model/phi-3-gguf"
+local_dir = "../model/phi-3-gguf"
 
 # Authenticate using the token from the environment variable
 token = os.getenv("HUGGINGFACE_HUB_TOKEN")
 
 if not token:
     raise ValueError("The Hugging Face token is not set in the environment variable.")
 
@@ -17,17 +17,21 @@
 
 # Create the repository if it doesn't exist
 create_repo(repo_id, token=token, exist_ok=True)
 
 # Upload each file in the local directory
 for root, dirs, files in os.walk(local_dir):
     for file in files:
+        if file.startswith("."):
+            # Skip hidden files and folders
+            continue
         local_file_path = os.path.join(root, file)
         repo_file_path = os.path.relpath(local_file_path, local_dir)
         upload_file(
             path_or_fileobj=local_file_path,
             path_in_repo=repo_file_path,
             repo_id=repo_id,
             token=token
         )
 
 print("Files uploaded successfully.")
+
```

### Comparing `weather_chatbot_phi3-0.1.0/PKG-INFO` & `weather_chatbot_phi3-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-chatbot-phi3
-Version: 0.1.0
+Version: 0.1.1
 Summary: An LLM Chatbot integrated with Open Weather API for Real-Time Weather Information.
 License: CC-BY-NC-SA-4.0
 Author: Vatsal Patel
 Author-email: vatsal1804@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

