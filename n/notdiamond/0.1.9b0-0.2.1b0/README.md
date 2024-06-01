# Comparing `tmp/notdiamond-0.1.9b0.tar.gz` & `tmp/notdiamond-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notdiamond-0.1.9b0.tar", max compression
+gzip compressed data, was "notdiamond-0.2.1b0.tar", max compression
```

## Comparing `notdiamond-0.1.9b0.tar` & `notdiamond-0.2.1b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     5862 2024-04-22 18:39:28.549020 notdiamond-0.1.9b0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.9b0/notdiamond/__init__.py
--rw-r--r--   0        0        0      831 2024-04-22 18:35:58.307978 notdiamond-0.1.9b0/notdiamond/callbacks.py
--rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.9b0/notdiamond/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.9b0/notdiamond/llms/__init__.py
--rw-r--r--   0        0        0    39818 2024-04-26 15:44:03.491985 notdiamond-0.1.9b0/notdiamond/llms/llm.py
--rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.9b0/notdiamond/llms/provider.py
--rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.9b0/notdiamond/llms/providers.py
--rw-r--r--   0        0        0    11705 2024-04-26 15:44:03.492337 notdiamond-0.1.9b0/notdiamond/llms/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.9b0/notdiamond/metrics/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.9b0/notdiamond/metrics/metric.py
--rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.9b0/notdiamond/metrics/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.9b0/notdiamond/prompts/__init__.py
--rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.9b0/notdiamond/prompts/hash.py
--rw-r--r--   0        0        0     6415 2024-04-26 15:44:03.492739 notdiamond-0.1.9b0/notdiamond/prompts/prompt.py
--rw-r--r--   0        0        0     2482 2024-04-26 15:44:03.493687 notdiamond-0.1.9b0/notdiamond/settings.py
--rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.9b0/notdiamond/types.py
--rw-r--r--   0        0        0     1580 2024-04-26 15:48:16.880555 notdiamond-0.1.9b0/pyproject.toml
--rw-r--r--   0        0        0     6974 1970-01-01 00:00:00.000000 notdiamond-0.1.9b0/PKG-INFO
+-rw-r--r--   0        0        0     5862 2024-04-26 13:35:55.983756 notdiamond-0.2.1b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 13:35:56.000431 notdiamond-0.2.1b0/notdiamond/__init__.py
+-rw-r--r--   0        0        0      831 2024-04-26 13:35:56.000431 notdiamond-0.2.1b0/notdiamond/callbacks.py
+-rw-r--r--   0        0        0      440 2024-04-26 13:35:56.000431 notdiamond-0.2.1b0/notdiamond/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:35:56.000431 notdiamond-0.2.1b0/notdiamond/llms/__init__.py
+-rw-r--r--   0        0        0    58577 2024-05-31 20:25:16.037554 notdiamond-0.2.1b0/notdiamond/llms/llm.py
+-rw-r--r--   0        0        0     4849 2024-05-31 12:59:46.696552 notdiamond-0.2.1b0/notdiamond/llms/provider.py
+-rw-r--r--   0        0        0     4854 2024-05-31 20:25:16.037554 notdiamond-0.2.1b0/notdiamond/llms/providers.py
+-rw-r--r--   0        0        0    12146 2024-05-31 13:08:17.130478 notdiamond-0.2.1b0/notdiamond/llms/request.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:35:56.003765 notdiamond-0.2.1b0/notdiamond/metrics/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-26 13:35:56.003765 notdiamond-0.2.1b0/notdiamond/metrics/metric.py
+-rw-r--r--   0        0        0     1100 2024-04-26 13:35:56.003765 notdiamond-0.2.1b0/notdiamond/metrics/request.py
+-rw-r--r--   0        0        0        0 2024-04-26 13:35:56.003765 notdiamond-0.2.1b0/notdiamond/prompts/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-26 13:35:56.003765 notdiamond-0.2.1b0/notdiamond/prompts/hash.py
+-rw-r--r--   0        0        0     7396 2024-05-31 12:59:46.696552 notdiamond-0.2.1b0/notdiamond/prompts/prompt.py
+-rw-r--r--   0        0        0     6031 2024-05-31 20:25:16.037554 notdiamond-0.2.1b0/notdiamond/settings.py
+-rw-r--r--   0        0        0      972 2024-04-26 13:35:56.003765 notdiamond-0.2.1b0/notdiamond/types.py
+-rw-r--r--   0        0        0     1633 2024-06-01 00:03:59.996705 notdiamond-0.2.1b0/pyproject.toml
+-rw-r--r--   0        0        0     7023 1970-01-01 00:00:00.000000 notdiamond-0.2.1b0/PKG-INFO
```

### Comparing `notdiamond-0.1.9b0/README.md` & `notdiamond-0.2.1b0/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.9b0/notdiamond/callbacks.py` & `notdiamond-0.2.1b0/notdiamond/callbacks.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.9b0/notdiamond/llms/provider.py` & `notdiamond-0.2.1b0/notdiamond/llms/provider.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     Attributes:
         provider (str): The name of the LLM provider (e.g., "openai", "anthropic"). Must be one of the
                         predefined providers in `POSSIBLE_PROVIDERS`.
         model (str): The name of the LLM model to use (e.g., "gpt-3.5-turbo").
                         Must be one of the predefined models in `POSSIBLE_MODELS`.
         api_key (Optional[str], optional): The API key for accessing the LLM provider's services.
                                             Defaults to None, in which case it tries to fetch from the settings.
+        openrouter_model (str): The OpenRouter model equivalent for this provider / model
         **kwargs: Additional keyword arguments that might be necessary for specific providers or models.
 
     Raises:
         UnsupportedLLMProvider: If the `provider` or `model` specified is not supported.
     """
 
     def __init__(
@@ -65,24 +66,33 @@
         if model not in POSSIBLE_MODELS:
             raise UnsupportedLLMProvider(
                 f"Given LLM model {model} is not in the list of supported models."
             )
 
         self.provider = provider
         self.model = model
+        self._openrouter_model = settings.PROVIDERS[provider][
+            "openrouter_identifier"
+        ].get(model, None)
         self.api_key = (
             api_key
             if api_key is not None
             else settings.PROVIDERS[provider]["api_key"]
         )
         self.kwargs = kwargs
 
     def __repr__(self) -> str:
         return f"{self.provider}/{self.model}"
 
+    @property
+    def openrouter_model(self):
+        if self._openrouter_model is None:
+            print("WARNING: this model is not available via OpenRouter")
+        return self._openrouter_model
+
     def prepare_for_request(self):
         """
         Converts the NDLLMProvider object to a dict in the format accepted by
         the NotDiamond API.
 
         Returns:
             dict
```

### Comparing `notdiamond-0.1.9b0/notdiamond/llms/providers.py` & `notdiamond-0.2.1b0/notdiamond/llms/providers.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,52 +9,70 @@
     It allows developers to easily specify available LLM providers for the router.
 
     Attributes:
         GPT_3_5_TURBO (NDLLMProvider): refers to 'gpt-3.5-turbo' model by OpenAI
         GPT_4 (NDLLMProvider): refers to 'gpt-4' model by OpenAI
         GPT_4_1106_PREVIEW (NDLLMProvider): refers to 'gpt-4-1106-preview' model by OpenAI
         GPT_4_TURBO_PREVIEW (NDLLMProvider): refers to 'gpt-4-turbo-preview' model by OpenAI
+        GPT_4_TURBO_2024_04_09 (NDLLMProvider): refers to 'gpt-4-turbo-2024-04-09' model by OpenAI
+        GPT_4o_2024_05_13 (NDLLMProvider): refers to 'gpt-4o-2024-05-13' model by OpenAI
         CLAUDE_2_1 (NDLLMProvider): refers to 'claude-2.1' model by Anthropic
         CLAUDE_3_OPUS_20240229 (NDLLMProvider): refers to 'claude-3-opus-20240229' model by Anthropic
         CLAUDE_3_SONNET_20240229 (NDLLMProvider): refers to 'claude-3-sonnet-20240229' model by Anthropic
         CLAUDE_3_HAIKU_20240307 (NDLLMProvider): refers to 'claude-3-haiku-20240307' model by Anthropic
         GEMINI_PRO (NDLLMProvider): refers to 'gemini-pro' model by Google
+        GEMINI_1_PRO_LATEST (NDLLMProvider): refers to 'gemini-1.0-pro-latest' model by Google
+        GEMINI_15_PRO_LATEST (NDLLMProvider): refers to 'gemini-1.5-pro-latest' model by Google
         COMMAND (NDLLMProvider): refers to 'command' model by Cohere
         COMMAND_R (NDLLMProvider): refers to 'command-r' model by Cohere
         MISTRAL_LARGE_LATEST (NDLLMProvider): refers to 'mistral-large-latest' model by Mistral AI
         MISTRAL_MEDIUM_LATEST (NDLLMProvider): refers to 'mistral-medium-latest' model by Mistral AI
         MISTRAL_SMALL_LATEST (NDLLMProvider): refers to 'mistral-small-latest' model by Mistral AI
         OPEN_MISTRAL_7B (NDLLMProvider): refers to 'open-mistral-7b' model by Mistral AI
         OPEN_MIXTRAL_8X7B (NDLLMProvider): refers to 'open-mixtral-8x7b' model by Mistral AI
+        OPEN_MIXTRAL_8X22B (NDLLMProvider): refers to 'open-mixtral-8x22b' model by Mistral AI
         CODELLAMA_34B_INSTRUCT_HF (NDLLMProvider): refers to 'CodeLlama-34b-Instruct-hf' model served via TogetherAI
         PHIND_CODELLAMA_34B_V2 (NDLLMProvider): refers to 'Phind-CodeLlama-34B-v2' model served via TogetherAI
         MISTRAL_7B_INSTRUCT_V0_2 (NDLLMProvider): refers to 'Mistral-7B-Instruct-v0.2' model served via TogetherAI
         MIXTRAL_8X7B_INSTRUCT_V0_1 (NDLLMProvider): refers to 'Mixtral-8x7B-Instruct-v0.1' model served via TogetherAI
+        MIXTRAL_8X22B_INSTRUCT_V0_1 (NDLLMProvider): refers to 'Mixtral-8x22B-Instruct-v0.1' model served via TogetherAI
 
     Note:
         This class is static and designed to be used without instantiation.
         Access its attributes directly to obtain configurations for specific LLM providers.
     """
 
     GPT_3_5_TURBO = ("openai", "gpt-3.5-turbo")
     GPT_4 = ("openai", "gpt-4")
     GPT_4_1106_PREVIEW = ("openai", "gpt-4-1106-preview")
     GPT_4_TURBO_PREVIEW = ("openai", "gpt-4-turbo-preview")
+    GPT_4_TURBO_2024_04_09 = ("openai", "gpt-4-turbo-2024-04-09")
+    GPT_4o_2024_05_13 = ("openai", "gpt-4o-2024-05-13")
     CLAUDE_2_1 = ("anthropic", "claude-2.1")
     CLAUDE_3_OPUS_20240229 = ("anthropic", "claude-3-opus-20240229")
     CLAUDE_3_SONNET_20240229 = ("anthropic", "claude-3-sonnet-20240229")
     CLAUDE_3_HAIKU_20240307 = ("anthropic", "claude-3-haiku-20240307")
     GEMINI_PRO = ("google", "gemini-pro")
+    GEMINI_1_PRO_LATEST = ("google", "gemini-1.0-pro-latest")
+    GEMINI_15_PRO_LATEST = ("google", "gemini-1.5-pro-latest")
     COMMAND = ("cohere", "command")
     COMMAND_R = ("cohere", "command-r")
     MISTRAL_LARGE_LATEST = ("mistral", "mistral-large-latest")
     MISTRAL_MEDIUM_LATEST = ("mistral", "mistral-medium-latest")
     MISTRAL_SMALL_LATEST = ("mistral", "mistral-small-latest")
     OPEN_MISTRAL_7B = ("mistral", "open-mistral-7b")
     OPEN_MIXTRAL_8X7B = ("mistral", "open-mixtral-8x7b")
+    OPEN_MIXTRAL_8X22B = ("mistral", "open-mixtral-8x22b")
     CODELLAMA_34B_INSTRUCT_HF = ("togetherai", "CodeLlama-34b-Instruct-hf")
     PHIND_CODELLAMA_34B_V2 = ("togetherai", "Phind-CodeLlama-34B-v2")
     MISTRAL_7B_INSTRUCT_V0_2 = ("togetherai", "Mistral-7B-Instruct-v0.2")
     MIXTRAL_8X7B_INSTRUCT_V0_1 = ("togetherai", "Mixtral-8x7B-Instruct-v0.1")
+    MIXTRAL_8X22B_INSTRUCT_V0_1 = ("togetherai", "Mixtral-8x22B-Instruct-v0.1")
+    LLAMA_3_70B_CHAT_HF = ("togetherai", "Llama-3-70b-chat-hf")
+    LLAMA_3_8B_CHAT_HF = ("togetherai", "Llama-3-8b-chat-hf")
+    LLAMA_3_SONAR_LARGE_32K_ONLINE = (
+        "perplexity",
+        "llama-3-sonar-large-32k-online",
+    )
 
     def __new__(cls, provider, model):
         return NDLLMProvider(provider=provider, model=model)
```

### Comparing `notdiamond-0.1.9b0/notdiamond/llms/request.py` & `notdiamond-0.2.1b0/notdiamond/llms/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,52 +14,57 @@
 
 def model_select_prepare(
     prompt_template: Optional[Union[NDPromptTemplate, NDChatPromptTemplate]],
     llm_providers: List[NDLLMProvider],
     metric: NDMetric,
     notdiamond_api_key: str,
     max_model_depth: int,
+    hash_content: bool,
     preference_weights: Optional[Dict[str, float]] = None,
     preference_id: Optional[str] = None,
     tools: Optional[Sequence[Union[Dict[str, Any], Callable]]] = [],
 ):
     """
     This is the core method for the model_select endpoint.
     It returns the best fitting LLM to call and a session ID that can be used for feedback.
 
     Parameters:
         prompt_template (Optional[Union[NDPromptTemplate, NDChatPromptTemplate]]): prompt template for the LLM call
         llm_providers (List[NDLLMProvider]): a list of available LLM providers that the router can decide from
         metric (NDMetric): metric based off which the router makes the decision. As of now only 'accuracy' supported.
         notdiamond_api_key (str): API key generated via the NotDiamond dashboard.
         max_model_depth (int): if your top recommended model is down, specify up to which depth of routing you're willing to go.
+        hash_content (Optional[bool]): Flag for hashing content before sending to NotDiamond API.
         preference_weights (Optional[Dict[str, float]], optional): Define the quality, cost and latency weights of importance
                                                                     for the router. Defaults to None.
         preference_id (Optional[str], optional): The ID of the router preference that was configured via the Dashboard.
                                                     Defaults to None.
         async_mode (bool, optional): whether to run the request in async mode. Defaults to False.
 
     Returns:
         tuple(url, payload, headers): returns data to be used for the API call of modelSelect
     """
 
     url = f"{settings.ND_BASE_URL}/v2/optimizer/modelSelect"
     tools_dict = get_tools_in_openai_format(tools)
 
     payload: ModelSelectRequestPayload = {
-        "messages": prompt_template.prepare_for_request(),
-        "hash_digest": prompt_template.get_hash_digest(tools_dict),
+        "messages": prompt_template.prepare_for_request(hash_content),
         "llm_providers": [
             llm_provider.prepare_for_request()
             for llm_provider in llm_providers
         ],
         "metric": metric.metric,
         "max_model_depth": max_model_depth,
+        "hash_content": hash_content,
     }
 
+    if hash_content:
+        payload["hash_digest"] = prompt_template.get_hash_digest(tools_dict)
+
     if tools_dict:
         payload["tools"] = tools_dict
     if preference_weights is not None:
         payload["preference_weights"] = preference_weights
     if preference_id is not None:
         payload["preference_id"] = preference_id
 
@@ -68,15 +73,15 @@
         "Authorization": f"Bearer {notdiamond_api_key}",
     }
 
     return url, payload, headers
 
 
 def get_tools_in_openai_format(
-    tools: Optional[Sequence[Union[Dict[str, Any], Callable]]]
+    tools: Optional[Sequence[Union[Dict[str, Any], Callable]]],
 ):
     """
     This function converts the tools list into the format that OpenAI expects.
     Does this by using langchains Model that automatically creates the dictionary on bind_tools
 
     Parameters:
         tools (Optional[Sequence[Union[Dict[str, Any], Callable]]]): list of tools to be converted
@@ -102,43 +107,42 @@
             filter(
                 lambda x: (x.model == top_provider["model"])
                 & (x.provider == top_provider["provider"]),
                 llm_providers,
             )
         )[0]
         return best_llm, session_id
-    if response_code == 401:
-        print(
-            f"ND API error: {response_code}. Make sure you have a valid NotDiamond API Key."
-        )
-    else:
-        print(f"ND API error: {response_code}")
+
+    error_message = response_json["detail"]
+    print(f"ND API error: {response_code}. {error_message}")
     return None, "NO-SESSION-ID"
 
 
 def model_select(
     prompt_template: Optional[Union[NDPromptTemplate, NDChatPromptTemplate]],
     llm_providers: List[NDLLMProvider],
     metric: NDMetric,
     notdiamond_api_key: str,
     max_model_depth: int,
+    hash_content: bool,
     preference_weights: Optional[Dict[str, float]] = None,
     preference_id: Optional[str] = None,
     tools: Optional[Sequence[Union[Dict[str, Any], Callable]]] = [],
 ):
     """
     This endpoint receives the prompt and routing settings, and makes a call to the NotDiamond API.
     It returns the best fitting LLM to call and a session ID that can be used for feedback.
 
     Parameters:
         prompt_template (Optional[Union[NDPromptTemplate, NDChatPromptTemplate]]): prompt template for the LLM call
         llm_providers (List[NDLLMProvider]): a list of available LLM providers that the router can decide from
         metric (NDMetric): metric based off which the router makes the decision. As of now only 'accuracy' supported.
         notdiamond_api_key (str): API key generated via the NotDiamond dashboard.
         max_model_depth (int): if your top recommended model is down, specify up to which depth of routing you're willing to go.
+        hash_content (Optional[bool]): Flag for hashing content before sending to NotDiamond API.
         preference_weights (Optional[Dict[str, float]], optional): Define the quality, cost and latency weights of importance
                                                                     for the router. Defaults to None.
         preference_id (Optional[str], optional): The ID of the router preference that was configured via the Dashboard.
                                                     Defaults to None.
 
     Returns:
         tuple(NDLLMProvider, string): returns a tuple of the chosen NDLLMProvider to call and a session ID string.
@@ -147,22 +151,23 @@
     """
     url, payload, headers = model_select_prepare(
         prompt_template=prompt_template,
         llm_providers=llm_providers,
         metric=metric,
         notdiamond_api_key=notdiamond_api_key,
         max_model_depth=max_model_depth,
+        hash_content=hash_content,
         preference_weights=preference_weights,
         preference_id=preference_id,
         tools=tools,
     )
 
     try:
         response = requests.post(
-            url, data=json.dumps(payload), headers=headers
+            url, data=json.dumps(payload), headers=headers, timeout=5
         )
         response_code = response.status_code
         response_json = response.json()
     except Exception as e:
         print(f"ND API error: {e}")
         return None, "NO-SESSION-ID"
 
@@ -175,28 +180,30 @@
 
 async def amodel_select(
     prompt_template: Optional[Union[NDPromptTemplate, NDChatPromptTemplate]],
     llm_providers: List[NDLLMProvider],
     metric: NDMetric,
     notdiamond_api_key: str,
     max_model_depth: int,
+    hash_content: bool,
     preference_weights: Optional[Dict[str, float]] = None,
     preference_id: Optional[str] = None,
     tools: Optional[Sequence[Union[Dict[str, Any], Callable]]] = [],
 ):
     """
     This endpoint receives the prompt and routing settings, and makes a call to the NotDiamond API.
     It returns the best fitting LLM to call and a session ID that can be used for feedback.
 
     Parameters:
         prompt_template (Optional[Union[NDPromptTemplate, NDChatPromptTemplate]]): prompt template for the LLM call
         llm_providers (List[NDLLMProvider]): a list of available LLM providers that the router can decide from
         metric (NDMetric): metric based off which the router makes the decision. As of now only 'accuracy' supported.
         notdiamond_api_key (str): API key generated via the NotDiamond dashboard.
         max_model_depth (int): if your top recommended model is down, specify up to which depth of routing you're willing to go.
+        hash_content (Optional[bool]): Flag for hashing content before sending to NotDiamond API.
         preference_weights (Optional[Dict[str, float]], optional): Define the quality, cost and latency weights of importance
                                                                     for the router. Defaults to None.
         preference_id (Optional[str], optional): The ID of the router preference that was configured via the Dashboard.
                                                     Defaults to None.
 
     Returns:
         tuple(NDLLMProvider, string): returns a tuple of the chosen NDLLMProvider to call and a session ID string.
@@ -205,23 +212,24 @@
     """
     url, payload, headers = model_select_prepare(
         prompt_template=prompt_template,
         llm_providers=llm_providers,
         metric=metric,
         notdiamond_api_key=notdiamond_api_key,
         max_model_depth=max_model_depth,
+        hash_content=hash_content,
         preference_weights=preference_weights,
         preference_id=preference_id,
         tools=tools,
     )
 
     try:
         async with aiohttp.ClientSession() as session:
             async with session.post(
-                url, data=json.dumps(payload), headers=headers
+                url, data=json.dumps(payload), headers=headers, timeout=5
             ) as response:
                 response_code = response.status
                 response_json = await response.json()
     except Exception as e:
         print(f"ND API error: {e}")
         return None, "NO-SESSION-ID"
```

### Comparing `notdiamond-0.1.9b0/notdiamond/metrics/metric.py` & `notdiamond-0.2.1b0/notdiamond/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.9b0/notdiamond/metrics/request.py` & `notdiamond-0.2.1b0/notdiamond/metrics/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.9b0/notdiamond/prompts/prompt.py` & `notdiamond-0.2.1b0/notdiamond/prompts/prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.prompts import PromptTemplate
 from langchain_core.messages import AIMessage, HumanMessage, SystemMessage
+from langchain_core.output_parsers import JsonOutputParser
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.prompts.string import get_template_variables
 
 from notdiamond.prompts.hash import nd_hash
 
 
 class NDPromptTemplate(PromptTemplate):
@@ -44,30 +45,42 @@
     def format(self, **kwargs: Any) -> str:
         """Format the prompt template with the given variables and convert it to NDPromptTemplate."""
         return super(NDPromptTemplate, self).format(**kwargs)
 
     def optimize(self):
         print("Not yet implemented!")
 
-    def prepare_for_request(self):
-        messages = [{"role": "user", "content": nd_hash(self.format())}]
+    def prepare_for_request(self, hash_content: bool):
+        content = self.format()
+        if hash_content:
+            content = nd_hash(content)
+        messages = [{"role": "user", "content": content}]
 
         return messages
 
     def get_hash_digest(self, tools_dict: Dict[str, Any] = None) -> str:
         current_prompt = self.format()
         if tools_dict:
             functions = json.dumps(tools_dict)
             hash_digest_with_tools = f"""
     {current_prompt}\nHere is a list of functions in JSON format that you can invoke:\n{functions}.
 """
             return nd_hash(hash_digest_with_tools)
 
         return nd_hash(current_prompt)
 
+    def inject_model_instruction(self, parser: JsonOutputParser):
+        format_instructions = parser.get_format_instructions()
+        format_instructions = format_instructions.replace("{", "{{").replace(
+            "}", "}}"
+        )
+        self.template = format_instructions + "\n" + self.template
+
+        return self
+
 
 class NDChatPromptTemplate(ChatPromptTemplate):
     """
     Starting reference is from
     here:https://api.python.langchain.com/en/latest/prompts/langchain_core.prompts.chat.ChatPromptTemplate.html
     """
 
@@ -143,28 +156,31 @@
             return "system"
         if isinstance(message, AIMessage):
             return "assistant"
         if isinstance(message, HumanMessage):
             return "user"
         raise ValueError(f"Unsupported message type: {type(message)}")
 
-    def prepare_for_request(self):
+    def prepare_for_request(self, hash_content):
         formated_messages = self.format_messages(**self.partial_variables)
         messages = []
 
         for message in formated_messages:
             if (
                 isinstance(message, SystemMessage)
                 or isinstance(message, AIMessage)
                 or isinstance(message, HumanMessage)
             ):
+                content = message.content
+                if hash_content:
+                    content = nd_hash(content)
                 messages.append(
                     {
                         "role": self.get_role_of_message(message),
-                        "content": nd_hash(message.content),
+                        "content": content,
                     }
                 )
 
         return messages
 
     def get_hash_digest(self, tools_dict: Dict[str, Any] = None) -> str:
         formated_messages = self.format_messages(**self.partial_variables)
@@ -178,7 +194,18 @@
             functions = json.dumps(tools_dict)
             hash_digest_with_tools = f"""
     {message_to_hash}\nHere is a list of functions in JSON format that you can invoke:\n{functions}.
 """
             return nd_hash(hash_digest_with_tools)
 
         return nd_hash(message_to_hash)
+
+    def inject_model_instruction(self, parser: JsonOutputParser):
+        format_instructions = parser.get_format_instructions()
+        format_instructions = format_instructions.replace("{", "{{").replace(
+            "}", "}}"
+        )
+        self.messages[0].content = (
+            format_instructions + "\n" + self.messages[0].content
+        )
+
+        return self
```

### Comparing `notdiamond-0.1.9b0/notdiamond/types.py` & `notdiamond-0.2.1b0/notdiamond/types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.9b0/pyproject.toml` & `notdiamond-0.2.1b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notdiamond"
-version = "0.1.9-beta"
+version = "0.2.1-beta"
 description = "Not Diamond Python Library"
 authors = ["Not Diamond <t5@notdiamond.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 langchain = ">=0.1.16"
@@ -17,18 +17,20 @@
 langchain-anthropic = "^0.1.8"
 langchain-community = "^0.0.32"
 langchain-mistralai = "^0.0.5"
 together = "^0.2.11"
 langchain-together = "^0.0.2.post1"
 aiohttp = "^3.9.3"
 langchain-cohere = "^0.1.2"
+pydantic-partial = "^0.5.5"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-asyncio = "^0.23.6"
+llama-index = "^0.10.34"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.1"
 pydantic = "^2.5.3"
 pre-commit = "^3.7.0"
 black = "^24.3.0"
 flake8 = "^7.0.0"
```

### Comparing `notdiamond-0.1.9b0/PKG-INFO` & `notdiamond-0.2.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notdiamond
-Version: 0.1.9b0
+Version: 0.2.1b0
 Summary: Not Diamond Python Library
 Author: Not Diamond
 Author-email: t5@notdiamond.ai
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,14 +18,15 @@
 Requires-Dist: langchain-google-genai (>=0.0.2)
 Requires-Dist: langchain-mistralai (>=0.0.5,<0.0.6)
 Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
 Requires-Dist: langchain-together (>=0.0.2.post1,<0.0.3)
 Requires-Dist: litellm (>=1.34.40,<2.0.0)
 Requires-Dist: openai (>=1.0.0)
 Requires-Dist: ppdeep (>=20200505,<20200506)
+Requires-Dist: pydantic-partial (>=0.5.5,<0.6.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: together (>=0.2.11,<0.3.0)
 Description-Content-Type: text/markdown
 
 # Getting started with Not Diamond
 
 Not Diamond automatically determines which model is best-suited to respond to any query, **drastically improving LLM output quality** while reducing costs and latency and avoiding vendor lock-in. Unlike any other model router, Not Diamond is **100% privacy-preserving** and **continuously adapts to your preferences** ([demo video](https://www.loom.com/share/6e5dee9d99434de6bafbcd96ff5d663c?sid=d771348d-e9e5-49f9-9f21-6310d12541ec)).
```

