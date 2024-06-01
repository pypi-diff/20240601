# Comparing `tmp/developergpt-0.7.4.tar.gz` & `tmp/developergpt-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.7.4.tar", last modified: Tue May 21 02:16:10 2024, max compression
+gzip compressed data, was "developergpt-0.7.5.tar", last modified: Sat Jun  1 20:25:03 2024, max compression
```

## Comparing `developergpt-0.7.4.tar` & `developergpt-0.7.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:16:10.138103 developergpt-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 02:16:00.000000 developergpt-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 02:16:00.000000 developergpt-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-21 02:16:10.138103 developergpt-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-21 02:16:00.000000 developergpt-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:16:10.134103 developergpt-0.7.4/developergpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/anthropic_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/few_shot_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/gemini_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-21 02:16:00.000000 developergpt-0.7.4/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:16:10.134103 developergpt-0.7.4/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-05-21 02:16:10.000000 developergpt-0.7.4/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-21 02:16:10.000000 developergpt-0.7.4/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:16:10.000000 developergpt-0.7.4/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 02:16:10.000000 developergpt-0.7.4/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-21 02:16:10.000000 developergpt-0.7.4/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 02:16:10.000000 developergpt-0.7.4/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:16:10.138103 developergpt-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-21 02:16:00.000000 developergpt-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:16:10.134103 developergpt-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:16:00.000000 developergpt-0.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-21 02:16:00.000000 developergpt-0.7.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 02:16:00.000000 developergpt-0.7.4/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:03.887435 developergpt-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-01 20:24:55.000000 developergpt-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 20:24:55.000000 developergpt-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-06-01 20:25:03.887435 developergpt-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-06-01 20:24:55.000000 developergpt-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:03.887435 developergpt-0.7.5/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/anthropic_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/few_shot_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/gemini_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-06-01 20:24:55.000000 developergpt-0.7.5/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:03.887435 developergpt-0.7.5/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-06-01 20:25:03.000000 developergpt-0.7.5/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-06-01 20:25:03.000000 developergpt-0.7.5/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:25:03.000000 developergpt-0.7.5/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 20:25:03.000000 developergpt-0.7.5/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-06-01 20:25:03.000000 developergpt-0.7.5/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 20:25:03.000000 developergpt-0.7.5/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:25:03.887435 developergpt-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-06-01 20:24:55.000000 developergpt-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:03.887435 developergpt-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:24:55.000000 developergpt-0.7.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-01 20:24:55.000000 developergpt-0.7.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 20:24:55.000000 developergpt-0.7.5/tests/test_cli.py
```

### Comparing `developergpt-0.7.4/LICENSE` & `developergpt-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/PKG-INFO` & `developergpt-0.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.7.4
+Version: 0.7.5
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -36,77 +36,68 @@
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.0 Pro by default but also supports OpenAI GPT LLMs, Anthropic Claude 3 LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.5 Flash by default but also supports Google Gemini 1.0 Pro, OpenAI GPT-3.5 & GPT-4, Anthropic Claude 3 Haiku & Sonnet, open LLMs (Zephyr, Gemma, Mistral) hosted on Hugging Face, and quantized Mistral-7B-Instruct running offline on-device.
 
-As of May 2024, DeveloperGPT is completely free to use when using Google Gemini 1.0 Pro (used by default) or Google Gemini 1.5 Flash at up to 15 requests per minute.
-
-Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
+As of June 2024, DeveloperGPT is completely free to use when using Google Gemini 1.5 Pro (used by default) or Google Gemini 1.0 Pro at up to 15 requests per minute.
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
-| Model(s)                        | Source                                                                                                                       | Details                                                  |
-| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default), **Flash** | [Google Gemini 1.0 Pro, Gemini 1.5 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**                 | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Haiku, Sonnet**               | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
-| **Zephyr**                      | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
-| **Gemma, Gemma-Base**           | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
-| **Mistral-Q6, Mistral-Q4**      | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
-| **Mistral**                     | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
+| Model(s)                                   | Source                                                                                                                       | Details                                                  |
+| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini Pro**, **Gemini Flash** (default) | [Google Gemini 1.0 Pro, Gemini 1.5 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**                          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
+| **Zephyr**                                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**                      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4**                 | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
-- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
+- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively). These LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details. 
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
 # Example
 $ developergpt cmd list all git commits that contain the word llm
 ```
 
 ![Natural Language Example 1](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmd_demo.gif)
 
-Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
-```bash
-# Fast Mode: Commands are given without explanation (may be less accurate)
-$ developergpt cmd --fast [your natural language command request]
-```
+Use `developergpt cmd --fast` to get commands faster without any explanations (~1.6 seconds with `--fast` vs. ~3.2 seconds with regular on average). Commands provided by DeveloperGPT in `--fast` mode may be less accurate - see [DeveloperGPT Natural Language to Terminal Command Accuracy](#developergpt-natural-language-to-terminal-command-accuracy) for more details.
 
-Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
-# Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
-$ developergpt --offline cmd [your natural language command request]
+# Fast Mode: Commands are given without explanation for faster response
+$ developergpt cmd --fast [your natural language command request]
 ```
 
-Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Pro (used by default).  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Flash (used by default).  
 ```bash
-# Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
+# Example: Natural Language to Terminal Commands using the GPT-3.5 instead of Gemini Flash
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
 **Usage:** `developergpt chat`
 ```bash
-# Chat with DeveloperGPT using Gemini Pro (default)
+# Chat with DeveloperGPT using Gemini 1.5 Flash (default)
 $ developergpt chat
 ```
 
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
-Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
-
-Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
+Use `developergpt --model [model_name] chat` to use a different LLM.  
 ```bash
 # Example
 $ developergpt --model mistral chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
@@ -120,88 +111,70 @@
 
 ### Basic Usage
 ```bash
 # see available commands
 $ developergpt 
 ```
 
+### DeveloperGPT Natural Language to Terminal Command Accuracy
+Accuracy of DeveloperGPT varies depending on the LLM used as well as the mode (`--fast` vs. regular). Shown below are Top@1 Accuracy of different LLMs on a set of [85 natural language command requests](https://github.com/luo-anthony/DeveloperGPT/blob/evaluation_v2/evaluation/85_command_requests.txt) (this isn't a rigorous evaluation, but it gives a rough sense of accuracy). Github CoPilot in the CLI v1.0.1 is also included for comparison. 
+
+![DeveloperGPT LLM Accuracy](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/evaluation.png)
+
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini 1.0 Pro. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini 1.5 Flash. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
-2. Set your Google API Key as an environment variable. You only need to do this once. 
+2. Set your Google API Key as the `GOOGLE_API_KEY` environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 #### Using Hugging Face Inference API Open LLMs
-To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
-See https://huggingface.co/docs/api-inference/index for more details. 
-
-```bash
-# [OPTIONAL] set Hugging Face token (using zsh for example)
-$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as the `HUGGING_FACE_API_KEY` environment variable. See https://huggingface.co/docs/api-inference/index for more details. 
 
-#### Using Mistral-7B-Instruct (Offline)
-To use Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
+#### Using Quantized Mistral-7B-Instruct Offline On-Device
+To use quantized Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
 ```bash
 developergpt --offline chat
 ```
 
 #### Using OpenAI GPT LLMs
-To use GPT3.5 or GPT4, you will need an OpenAI API key.
+To use GPT-3.5 or GPT-4, you will need an OpenAI API key.
 
 1. Get your own OpenAI API Key and setup billing: https://platform.openai.com/account/api-keys
-2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
-```bash
-# set OpenAI API Key (using zsh for example)
-$ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+2. Set your OpenAI API Key as the `OPENAI_API_KEY` environment variable. You only need to do this once. 
 
 #### Using Anthropic LLMs
 To use Anthropic Claude 3 Sonnet or Haiku, you will need an Anthropic API key.
 
 1. Get your own Anthropic API Key: https://www.anthropic.com/api
-2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
-```bash
-# set Anthropic API Key (using zsh for example)
-$ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+2. Set your Anthropic API Key as the `ANTHROPIC_API_KEY` environment variable. You only need to do this once. 
 
 
-### Usage and Cost 
+### LLM Cost
 #### Google Gemini LLMs
-As of May 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of June 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash are free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### Hugging Face Hosted Open LLMs 
-As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
+As of June 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.0001 cents. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.1 cents. Using GPT-4 is not recommended as GPT-3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Anthropic Claude LLMs
-You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.0001 cents. See https://www.anthropic.com/api for pricing details. 
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.1 cents. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini API free tier.
```

### Comparing `developergpt-0.7.4/README.md` & `developergpt-0.7.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,66 @@
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.0 Pro by default but also supports OpenAI GPT LLMs, Anthropic Claude 3 LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.5 Flash by default but also supports Google Gemini 1.0 Pro, OpenAI GPT-3.5 & GPT-4, Anthropic Claude 3 Haiku & Sonnet, open LLMs (Zephyr, Gemma, Mistral) hosted on Hugging Face, and quantized Mistral-7B-Instruct running offline on-device.
 
-As of May 2024, DeveloperGPT is completely free to use when using Google Gemini 1.0 Pro (used by default) or Google Gemini 1.5 Flash at up to 15 requests per minute.
-
-Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
+As of June 2024, DeveloperGPT is completely free to use when using Google Gemini 1.5 Pro (used by default) or Google Gemini 1.0 Pro at up to 15 requests per minute.
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
-| Model(s)                        | Source                                                                                                                       | Details                                                  |
-| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default), **Flash** | [Google Gemini 1.0 Pro, Gemini 1.5 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**                 | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Haiku, Sonnet**               | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
-| **Zephyr**                      | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
-| **Gemma, Gemma-Base**           | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
-| **Mistral-Q6, Mistral-Q4**      | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
-| **Mistral**                     | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
+| Model(s)                                   | Source                                                                                                                       | Details                                                  |
+| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini Pro**, **Gemini Flash** (default) | [Google Gemini 1.0 Pro, Gemini 1.5 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**                          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
+| **Zephyr**                                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**                      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4**                 | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
-- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
+- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively). These LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details. 
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
 # Example
 $ developergpt cmd list all git commits that contain the word llm
 ```
 
 ![Natural Language Example 1](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmd_demo.gif)
 
-Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
-```bash
-# Fast Mode: Commands are given without explanation (may be less accurate)
-$ developergpt cmd --fast [your natural language command request]
-```
+Use `developergpt cmd --fast` to get commands faster without any explanations (~1.6 seconds with `--fast` vs. ~3.2 seconds with regular on average). Commands provided by DeveloperGPT in `--fast` mode may be less accurate - see [DeveloperGPT Natural Language to Terminal Command Accuracy](#developergpt-natural-language-to-terminal-command-accuracy) for more details.
 
-Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
-# Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
-$ developergpt --offline cmd [your natural language command request]
+# Fast Mode: Commands are given without explanation for faster response
+$ developergpt cmd --fast [your natural language command request]
 ```
 
-Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Pro (used by default).  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Flash (used by default).  
 ```bash
-# Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
+# Example: Natural Language to Terminal Commands using the GPT-3.5 instead of Gemini Flash
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
 **Usage:** `developergpt chat`
 ```bash
-# Chat with DeveloperGPT using Gemini Pro (default)
+# Chat with DeveloperGPT using Gemini 1.5 Flash (default)
 $ developergpt chat
 ```
 
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
-Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
-
-Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
+Use `developergpt --model [model_name] chat` to use a different LLM.  
 ```bash
 # Example
 $ developergpt --model mistral chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
@@ -83,88 +74,70 @@
 
 ### Basic Usage
 ```bash
 # see available commands
 $ developergpt 
 ```
 
+### DeveloperGPT Natural Language to Terminal Command Accuracy
+Accuracy of DeveloperGPT varies depending on the LLM used as well as the mode (`--fast` vs. regular). Shown below are Top@1 Accuracy of different LLMs on a set of [85 natural language command requests](https://github.com/luo-anthony/DeveloperGPT/blob/evaluation_v2/evaluation/85_command_requests.txt) (this isn't a rigorous evaluation, but it gives a rough sense of accuracy). Github CoPilot in the CLI v1.0.1 is also included for comparison. 
+
+![DeveloperGPT LLM Accuracy](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/evaluation.png)
+
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini 1.0 Pro. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini 1.5 Flash. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
-2. Set your Google API Key as an environment variable. You only need to do this once. 
+2. Set your Google API Key as the `GOOGLE_API_KEY` environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 #### Using Hugging Face Inference API Open LLMs
-To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
-See https://huggingface.co/docs/api-inference/index for more details. 
-
-```bash
-# [OPTIONAL] set Hugging Face token (using zsh for example)
-$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as the `HUGGING_FACE_API_KEY` environment variable. See https://huggingface.co/docs/api-inference/index for more details. 
 
-#### Using Mistral-7B-Instruct (Offline)
-To use Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
+#### Using Quantized Mistral-7B-Instruct Offline On-Device
+To use quantized Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
 ```bash
 developergpt --offline chat
 ```
 
 #### Using OpenAI GPT LLMs
-To use GPT3.5 or GPT4, you will need an OpenAI API key.
+To use GPT-3.5 or GPT-4, you will need an OpenAI API key.
 
 1. Get your own OpenAI API Key and setup billing: https://platform.openai.com/account/api-keys
-2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
-```bash
-# set OpenAI API Key (using zsh for example)
-$ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+2. Set your OpenAI API Key as the `OPENAI_API_KEY` environment variable. You only need to do this once. 
 
 #### Using Anthropic LLMs
 To use Anthropic Claude 3 Sonnet or Haiku, you will need an Anthropic API key.
 
 1. Get your own Anthropic API Key: https://www.anthropic.com/api
-2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
-```bash
-# set Anthropic API Key (using zsh for example)
-$ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+2. Set your Anthropic API Key as the `ANTHROPIC_API_KEY` environment variable. You only need to do this once. 
 
 
-### Usage and Cost 
+### LLM Cost
 #### Google Gemini LLMs
-As of May 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of June 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash are free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### Hugging Face Hosted Open LLMs 
-As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
+As of June 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.0001 cents. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.1 cents. Using GPT-4 is not recommended as GPT-3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Anthropic Claude LLMs
-You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.0001 cents. See https://www.anthropic.com/api for pricing details. 
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.1 cents. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini API free tier.
```

### Comparing `developergpt-0.7.4/developergpt/anthropic_adapter.py` & `developergpt-0.7.5/developergpt/anthropic_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/developergpt/cli.py` & `developergpt-0.7.5/developergpt/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 @click.option(
     "--temperature",
     default=0.2,
     help="The temperature of the model response for chat (higher means more creative, lower means more predictable)",
 )
 @click.option(
     "--model",
-    default="gemini",
+    default="flash",
     help=f"The LLM to use. Options: {', '.join(config.SUPPORTED_MODELS)}",
 )
 @click.option(
     "--offline",
     is_flag=True,
     default=False,
     help=f"Use DeveloperGPT with a quantized LLM running on-device (offline). Options: {', '.join(config.OFFLINE_MODELS)}",
```

### Comparing `developergpt-0.7.4/developergpt/config.py` & `developergpt-0.7.5/developergpt/config.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/developergpt/few_shot_prompts.py` & `developergpt-0.7.5/developergpt/few_shot_prompts.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/developergpt/gemini_adapter.py` & `developergpt-0.7.5/developergpt/gemini_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/developergpt/huggingface_adapter.py` & `developergpt-0.7.5/developergpt/huggingface_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/developergpt/openai_adapter.py` & `developergpt-0.7.5/developergpt/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/developergpt/utils.py` & `developergpt-0.7.5/developergpt/utils.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/developergpt.egg-info/PKG-INFO` & `developergpt-0.7.5/developergpt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.7.4
+Version: 0.7.5
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
@@ -36,77 +36,68 @@
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20Zephyr,%20Claude-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 
-DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.0 Pro by default but also supports OpenAI GPT LLMs, Anthropic Claude 3 LLMs, open LLMs hosted on Hugging Face, and offline quantized on-device LLMs.
+DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini 1.5 Flash by default but also supports Google Gemini 1.0 Pro, OpenAI GPT-3.5 & GPT-4, Anthropic Claude 3 Haiku & Sonnet, open LLMs (Zephyr, Gemma, Mistral) hosted on Hugging Face, and quantized Mistral-7B-Instruct running offline on-device.
 
-As of May 2024, DeveloperGPT is completely free to use when using Google Gemini 1.0 Pro (used by default) or Google Gemini 1.5 Flash at up to 15 requests per minute.
-
-Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
+As of June 2024, DeveloperGPT is completely free to use when using Google Gemini 1.5 Pro (used by default) or Google Gemini 1.0 Pro at up to 15 requests per minute.
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [llm_name] [cmd, chat]`
-| Model(s)                        | Source                                                                                                                       | Details                                                  |
-| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
-| **Gemini** (default), **Flash** | [Google Gemini 1.0 Pro, Gemini 1.5 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
-| **GPT35, GPT4**                 | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
-| **Haiku, Sonnet**               | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
-| **Zephyr**                      | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
-| **Gemma, Gemma-Base**           | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
-| **Mistral-Q6, Mistral-Q4**      | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
-| **Mistral**                     | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
+| Model(s)                                   | Source                                                                                                                       | Details                                                  |
+| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini Pro**, **Gemini Flash** (default) | [Google Gemini 1.0 Pro, Gemini 1.5 Flash](https://deepmind.google/technologies/gemini/)                                      | Free (up to 15 requests/min), Google AI API Key Required |
+| **GPT35, GPT4**                            | [OpenAI](https://platform.openai.com/docs/models)                                                                            | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Haiku, Sonnet**                          | [Anthropic (Claude 3)](https://docs.anthropic.com/claude/docs/models-overview)                                               | Pay-Per-Usage, Anthropic API Key Required                |
+| **Zephyr**                                 | [Zephyr7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                                         | Free, Open LLM, Hugging Face Inference API               |
+| **Gemma, Gemma-Base**                      | [Gemma-1.1-7B-Instruct](https://huggingface.co/google/gemma-1.1-7b-it), [Gemma-Base](https://huggingface.co/google/gemma-7b) | Free, Open LLM, Hugging Face Inference API               |
+| **Mistral-Q6, Mistral-Q4**                 | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)                          | Free, Open LLM, OFFLINE, ON-DEVICE                       |
+| **Mistral**                                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                             | Free, Open LLM, Hugging Face Inference API               |
 
-- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
+- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively). These LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details. 
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
 # Example
 $ developergpt cmd list all git commits that contain the word llm
 ```
 
 ![Natural Language Example 1](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmd_demo.gif)
 
-Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
-```bash
-# Fast Mode: Commands are given without explanation (may be less accurate)
-$ developergpt cmd --fast [your natural language command request]
-```
+Use `developergpt cmd --fast` to get commands faster without any explanations (~1.6 seconds with `--fast` vs. ~3.2 seconds with regular on average). Commands provided by DeveloperGPT in `--fast` mode may be less accurate - see [DeveloperGPT Natural Language to Terminal Command Accuracy](#developergpt-natural-language-to-terminal-command-accuracy) for more details.
 
-Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
-# Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
-$ developergpt --offline cmd [your natural language command request]
+# Fast Mode: Commands are given without explanation for faster response
+$ developergpt cmd --fast [your natural language command request]
 ```
 
-Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Pro (used by default).  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini Flash (used by default).  
 ```bash
-# Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
+# Example: Natural Language to Terminal Commands using the GPT-3.5 instead of Gemini Flash
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
 **Usage:** `developergpt chat`
 ```bash
-# Chat with DeveloperGPT using Gemini Pro (default)
+# Chat with DeveloperGPT using Gemini 1.5 Flash (default)
 $ developergpt chat
 ```
 
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
-Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
-
-Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
+Use `developergpt --model [model_name] chat` to use a different LLM.  
 ```bash
 # Example
 $ developergpt --model mistral chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
@@ -120,88 +111,70 @@
 
 ### Basic Usage
 ```bash
 # see available commands
 $ developergpt 
 ```
 
+### DeveloperGPT Natural Language to Terminal Command Accuracy
+Accuracy of DeveloperGPT varies depending on the LLM used as well as the mode (`--fast` vs. regular). Shown below are Top@1 Accuracy of different LLMs on a set of [85 natural language command requests](https://github.com/luo-anthony/DeveloperGPT/blob/evaluation_v2/evaluation/85_command_requests.txt) (this isn't a rigorous evaluation, but it gives a rough sense of accuracy). Github CoPilot in the CLI v1.0.1 is also included for comparison. 
+
+![DeveloperGPT LLM Accuracy](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/evaluation.png)
+
 ### Setup
 #### Using Google Gemini (Default)
-By default, DeveloperGPT uses Google Gemini 1.0 Pro. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
+By default, DeveloperGPT uses Google Gemini 1.5 Flash. To use Gemini 1.0 Pro or Gemini 1.5 Flash, you will need an API key (free to use up to 15 queries per minute).
 
 1. Get your own Google AI Studio API Key: https://makersuite.google.com/app/apikey
-2. Set your Google API Key as an environment variable. You only need to do this once. 
+2. Set your Google API Key as the `GOOGLE_API_KEY` environment variable. You only need to do this once. 
 ```bash
 # set Google API Key (using zsh for example)
 $ echo 'export GOOGLE_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
 #### Using Hugging Face Inference API Open LLMs
-To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as an environment variable using the steps below. 
-See https://huggingface.co/docs/api-inference/index for more details. 
-
-```bash
-# [OPTIONAL] set Hugging Face token (using zsh for example)
-$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+To use open LLMs such as Gemma or Mistral hosted on Hugging Face, you can optionally set up a [Hugging Face Inference API](https://huggingface.co/settings/tokens) token as the `HUGGING_FACE_API_KEY` environment variable. See https://huggingface.co/docs/api-inference/index for more details. 
 
-#### Using Mistral-7B-Instruct (Offline)
-To use Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
+#### Using Quantized Mistral-7B-Instruct Offline On-Device
+To use quantized Mistral-7B-Instruct, just run DeveloperGPT with the `--offline` flag. This will download the model on first run and use it locally in any future runs (no internet connection is required after the first use). No special setup is required. 
 ```bash
 developergpt --offline chat
 ```
 
 #### Using OpenAI GPT LLMs
-To use GPT3.5 or GPT4, you will need an OpenAI API key.
+To use GPT-3.5 or GPT-4, you will need an OpenAI API key.
 
 1. Get your own OpenAI API Key and setup billing: https://platform.openai.com/account/api-keys
-2. Set your OpenAI API Key as an environment variable. You only need to do this once. 
-```bash
-# set OpenAI API Key (using zsh for example)
-$ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+2. Set your OpenAI API Key as the `OPENAI_API_KEY` environment variable. You only need to do this once. 
 
 #### Using Anthropic LLMs
 To use Anthropic Claude 3 Sonnet or Haiku, you will need an Anthropic API key.
 
 1. Get your own Anthropic API Key: https://www.anthropic.com/api
-2. Set your Anthropic API Key as an environment variable. You only need to do this once. 
-```bash
-# set Anthropic API Key (using zsh for example)
-$ echo 'export ANTHROPIC_API_KEY=[your_key_here]' >> ~/.zshenv
-
-# reload the environment (or just quit and open a new terminal)
-$ source ~/.zshenv
-```
+2. Set your Anthropic API Key as the `ANTHROPIC_API_KEY` environment variable. You only need to do this once. 
 
 
-### Usage and Cost 
+### LLM Cost
 #### Google Gemini LLMs
-As of May 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of June 2024, Google Gemini 1.0 Pro and Gemini 1.5 Flash are free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### Hugging Face Hosted Open LLMs 
-As of April 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
+As of June 2024, using Hugging Face Inference API hosted LLMs is free but rate limited. See https://huggingface.co/docs/api-inference/index for more details.
 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.0001 cents. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. The average cost per query using GPT-3.5 is < 0.1 cents. Using GPT-4 is not recommended as GPT-3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Anthropic Claude LLMs
-You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.0001 cents. See https://www.anthropic.com/api for pricing details. 
+You can monitor your Anthropic API usage here: https://console.anthropic.com/settings/plans. The average cost per query using Claude 3 Haiku is < 0.1 cents. See https://www.anthropic.com/api for pricing details. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Credit
 - Thanks to Hugging Face and the NLP/LLM community for open LLMs, generous free hosted inference APIs, tools, quantization, and other resources! 
 - Thanks to Google for the generous Gemini API free tier.
```

### Comparing `developergpt-0.7.4/developergpt.egg-info/SOURCES.txt` & `developergpt-0.7.5/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.7.4/setup.py` & `developergpt-0.7.5/setup.py`

 * *Files identical despite different names*

