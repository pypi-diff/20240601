# Comparing `tmp/lambda_genai_util-0.0.4.tar.gz` & `tmp/lambda_genai_util-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_genai_util-0.0.4.tar", last modified: Fri May 31 12:32:04 2024, max compression
+gzip compressed data, was "lambda_genai_util-0.0.5.tar", last modified: Sat Jun  1 18:45:17 2024, max compression
```

## Comparing `lambda_genai_util-0.0.4.tar` & `lambda_genai_util-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 12:32:04.936710 lambda_genai_util-0.0.4/
--rw-rw-rw-   0        0        0     1089 2024-05-30 13:47:39.000000 lambda_genai_util-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1712 2024-05-31 12:32:04.936710 lambda_genai_util-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      611 2024-05-31 12:29:11.000000 lambda_genai_util-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 12:32:04.937710 lambda_genai_util-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 12:32:04.908848 lambda_genai_util-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 12:32:04.921710 lambda_genai_util-0.0.4/src/lambda_genai_util/
--rw-rw-rw-   0        0        0     1483 2024-05-31 12:29:02.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/AnthropicBedrockUtil.py
--rw-rw-rw-   0        0        0     1690 2024-05-31 12:28:59.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/AwsTitanBedrockUtil.py
--rw-rw-rw-   0        0        0      182 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/BedrockUtil.py
--rw-rw-rw-   0        0        0     1420 2024-05-31 12:28:54.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/CohereBedrockUtil.py
--rw-rw-rw-   0        0        0     1263 2024-05-31 12:28:51.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/MetaBedrockUtil.py
--rw-rw-rw-   0        0        0     1205 2024-05-31 12:28:48.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/MistralBedrockUtil.py
--rw-rw-rw-   0        0        0     1525 2024-05-31 12:28:36.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/TextCompletionUtil.py
--rw-rw-rw-   0        0        0        0 2024-05-31 10:47:21.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/__init__.py
--rw-rw-rw-   0        0        0     1039 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/model_map.py
--rw-rw-rw-   0        0        0     2086 2024-05-31 12:28:43.000000 lambda_genai_util-0.0.4/src/lambda_genai_util/prompt_service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:32:04.934709 lambda_genai_util-0.0.4/src/lambda_genai_util.egg-info/
--rw-rw-rw-   0        0        0     1712 2024-05-31 12:32:04.000000 lambda_genai_util-0.0.4/src/lambda_genai_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2024-05-31 12:32:04.000000 lambda_genai_util-0.0.4/src/lambda_genai_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 12:32:04.000000 lambda_genai_util-0.0.4/src/lambda_genai_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-31 12:32:04.000000 lambda_genai_util-0.0.4/src/lambda_genai_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 12:32:04.000000 lambda_genai_util-0.0.4/src/lambda_genai_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 18:45:17.311266 lambda_genai_util-0.0.5/
+-rw-rw-rw-   0        0        0     1089 2024-05-30 13:47:39.000000 lambda_genai_util-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1712 2024-06-01 18:45:17.310266 lambda_genai_util-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2024-06-01 18:45:02.000000 lambda_genai_util-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 18:45:17.311266 lambda_genai_util-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 18:45:17.282268 lambda_genai_util-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 18:45:17.294265 lambda_genai_util-0.0.5/src/lambda_genai_util/
+-rw-rw-rw-   0        0        0     1916 2024-06-01 18:01:07.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/AnthropicBedrockUtil.py
+-rw-rw-rw-   0        0        0     2142 2024-06-01 18:01:07.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/AwsTitanBedrockUtil.py
+-rw-rw-rw-   0        0        0      233 2024-06-01 17:00:09.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/BedrockUtil.py
+-rw-rw-rw-   0        0        0     1825 2024-06-01 17:59:53.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/CohereBedrockUtil.py
+-rw-rw-rw-   0        0        0     1694 2024-06-01 18:01:07.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/MetaBedrockUtil.py
+-rw-rw-rw-   0        0        0     1688 2024-06-01 18:01:07.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/MistralBedrockUtil.py
+-rw-rw-rw-   0        0        0     1693 2024-06-01 18:01:58.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/TextCompletionUtil.py
+-rw-rw-rw-   0        0        0        0 2024-05-31 10:47:21.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/__init__.py
+-rw-rw-rw-   0        0        0     1039 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/model_map.py
+-rw-rw-rw-   0        0        0     2390 2024-06-01 18:09:43.000000 lambda_genai_util-0.0.5/src/lambda_genai_util/prompt_service.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:45:17.309272 lambda_genai_util-0.0.5/src/lambda_genai_util.egg-info/
+-rw-rw-rw-   0        0        0     1712 2024-06-01 18:45:17.000000 lambda_genai_util-0.0.5/src/lambda_genai_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2024-06-01 18:45:17.000000 lambda_genai_util-0.0.5/src/lambda_genai_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 18:45:17.000000 lambda_genai_util-0.0.5/src/lambda_genai_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-06-01 18:45:17.000000 lambda_genai_util-0.0.5/src/lambda_genai_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-01 18:45:17.000000 lambda_genai_util-0.0.5/src/lambda_genai_util.egg-info/top_level.txt
```

### Comparing `lambda_genai_util-0.0.4/LICENSE.txt` & `lambda_genai_util-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.4/PKG-INFO` & `lambda_genai_util-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda_genai_util
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for GenAI Utility for AWS Based development
 Author-email: Biprajeet Kar <biprokvs@gmail.com>
 Maintainer-email: Biprajeet Kar <biprokvs@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Biprajeet Kar
```

### Comparing `lambda_genai_util-0.0.4/pyproject.toml` & `lambda_genai_util-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lambda_genai_util"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Biprajeet Kar", email="biprokvs@gmail.com" },
 ]
 maintainers = [
   {name="Biprajeet Kar", email="biprokvs@gmail.com"}
 ]
 description = "Library for GenAI Utility for AWS Based development"
```

### Comparing `lambda_genai_util-0.0.4/src/lambda_genai_util/AnthropicBedrockUtil.py` & `lambda_genai_util-0.0.5/src/lambda_genai_util/CohereBedrockUtil.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 import json
 import logging
 from lambda_util.lambda_genai_util.BedrockUtil import BedrockUtil
 
 logger = logging.getLogger(__name__)
 
-class AnthropicBedrockUtil(BedrockUtil):
+class CohereBedrockUtil(BedrockUtil):
 
-    def text_completion(self, bedrock_client, model, prompt, **model_kwargs):
+    def text_completion(self, bedrock_client, model, prompt,guardrail_identifier=None, guardrail_version=None, **model_kwargs):
         prompt_request = {}
         prompt_response = {}
-        model_id = model
 
         if prompt:
+            if "command-r" in model:
+                prompt_request['message'] = prompt
+            else:
+                prompt_request["prompt"] = prompt
+
+            prompt_request.update(model_kwargs)
+
+            body = json.dumps(prompt_request)
+            accept = "application/json"
+            content_type = "application/json"
+
             try:
-                prompt_request['anthropic_version'] = 'bedrock-2023-05-31'
-                prompt_request["messages"] = [{"role": "user", "content": prompt}]
-                prompt_request.update(model_kwargs)
-                prompt_request.setdefault("max_tokens", 4000)
-
-                body = json.dumps(prompt_request)
-                accept = "application/json"
-                content_type = "application/json"
-
-                response = bedrock_client.invoke_model(
-                    body=body, modelId=model_id, accept=accept, contentType=content_type
-                )
+                if guardrail_identifier is None and guardrail_version is None:
+                    response = bedrock_client.invoke_model(
+                        body=body, modelId=model, accept=accept, contentType=content_type
+                    )
+                else:
+                    response = bedrock_client.invoke_model(
+                        body=body, modelId=model, accept=accept, contentType=content_type,
+                        guardrailIdentifier=guardrail_identifier, guardrailVersion=guardrail_version
+                    )
                 response_body = json.loads(response.get("body").read())
 
-                prompt_response['output'] = response_body['content'][0]['text']
-
-            except (KeyError, IndexError) as e:
-                logger.error(f"Error occurred while processing response: {e}")
-                prompt_response['output'] = None
+                if "command-r" in model:
+                    prompt_response['output'] = response_body.get('text', '')
+                else:
+                    prompt_response['output'] = response_body.get('generations', [{}])[0].get('text', '')
 
             except Exception as e:
-                logger.exception(f"An unexpected error occurred: {e}")
+                logger.exception(f"Error in text_completion for model {model}: {str(e)}")
                 raise
 
         return prompt_response
```

### Comparing `lambda_genai_util-0.0.4/src/lambda_genai_util/AwsTitanBedrockUtil.py` & `lambda_genai_util-0.0.5/src/lambda_genai_util/AwsTitanBedrockUtil.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 import json
 import logging
 
 from lambda_util.lambda_genai_util.BedrockUtil import BedrockUtil
 
 logger = logging.getLogger(__name__)
 
+
 class AwsTitanBedrockUtil(BedrockUtil):
 
-    def text_completion(self, bedrock_client, model, prompt, **model_kwargs):
+    def text_completion(self, bedrock_client, model, prompt, guardrail_identifier=None, guardrail_version=None,**model_kwargs):
         prompt_request = {}
         prompt_response = {}
         model_id = model
 
         if prompt:
             prompt_request["inputText"] = prompt
 
             text_config = {
                 'temperature': model_kwargs.get("temperature"),
                 'topP': model_kwargs.get("top_p"),
                 'maxTokenCount': model_kwargs.get("max_token")
             }
             stop_sequences = model_kwargs.get('stop_sequences')
-            
+
             if stop_sequences:
                 text_config['stopSequences'] = [seq.strip() for seq in stop_sequences.split(',') if seq.strip()]
 
             text_config = {k: v for k, v in text_config.items() if v}
 
             if text_config:
                 prompt_request['textGenerationConfig'] = text_config
 
             body = json.dumps(prompt_request)
             accept = "application/json"
             content_type = "application/json"
 
             try:
-                response = bedrock_client.invoke_model(
-                    body=body, modelId=model_id, accept=accept, contentType=content_type
-                )
+
+                if guardrail_identifier is None and guardrail_version is None:
+                    response = bedrock_client.invoke_model(
+                        body=body, modelId=model, accept=accept, contentType=content_type
+                    )
+                else:
+                    response = bedrock_client.invoke_model(
+                        body=body, modelId=model, accept=accept, contentType=content_type,
+                        guardrailIdentifier=guardrail_identifier, guardrailVersion=guardrail_version
+                    )
                 response_body = json.loads(response.get("body").read())
                 prompt_response['output'] = response_body['results'][0]['outputText']
             except Exception as e:
-                logger.error(f"Error in text_completion: {str(e)}")
+                logger.exception(f"Error in text_completion for model {model}: {str(e)}")
                 raise
 
-        return prompt_response
+        return prompt_response
```

### Comparing `lambda_genai_util-0.0.4/src/lambda_genai_util/MetaBedrockUtil.py` & `lambda_genai_util-0.0.5/src/lambda_genai_util/MetaBedrockUtil.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,37 +3,42 @@
 
 from lambda_util.lambda_genai_util.BedrockUtil import BedrockUtil
 
 logger = logging.getLogger(__name__)
 
 class MetaBedrockUtil(BedrockUtil):
 
-    def text_completion(self, bedrock_client, model, prompt, **model_kwargs):
+    def text_completion(self, bedrock_client, model, prompt, guardrail_identifier=None, guardrail_version=None,**model_kwargs):
         prompt_request = {}
         prompt_response = {}
-        model_id = model
 
         if prompt:
             prompt_request["prompt"] = prompt
             prompt_request.update(model_kwargs)
 
             try:
                 body = json.dumps(prompt_request)
                 accept = "application/json"
                 content_type = "application/json"
 
-                response = bedrock_client.invoke_model(
-                    body=body, modelId=model_id, accept=accept, contentType=content_type
-                )
+                if guardrail_identifier is None and guardrail_version is None:
+                    response = bedrock_client.invoke_model(
+                        body=body, modelId=model, accept=accept, contentType=content_type
+                    )
+                else:
+                    response = bedrock_client.invoke_model(
+                        body=body, modelId=model, accept=accept, contentType=content_type,
+                        guardrailIdentifier=guardrail_identifier, guardrailVersion=guardrail_version
+                    )
                 response_body = json.loads(response["body"].read())
 
                 prompt_response['output'] = response_body['generation']
 
             except (KeyError, json.JSONDecodeError) as e:
                 logger.error(f"Error processing response: {str(e)}")
                 raise
 
             except Exception as e:
-                logger.exception(f"Unexpected error occurred: {str(e)}")
+                logger.exception(f"Error in text_completion for model {model}: {str(e)}")
                 raise
 
         return prompt_response
```

### Comparing `lambda_genai_util-0.0.4/src/lambda_genai_util/TextCompletionUtil.py` & `lambda_genai_util-0.0.5/src/lambda_genai_util/TextCompletionUtil.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from lambda_util.lambda_genai_util.AnthropicBedrockUtil import AnthropicBedrockUtil
 from lambda_util.lambda_genai_util.CohereBedrockUtil import CohereBedrockUtil
 from lambda_util.lambda_genai_util.model_map import model_map
 
 bedrock = boto3.client(service_name='bedrock-runtime')
 logger = logging.getLogger(__name__)
 
-def generate_text_completion(model: str, prompt, **model_kwargs):
+def generate_text_completion(model: str, prompt, guardrail_identifier=None, guardrail_version=None, **model_kwargs):
     if model is None or model_map.get(model) is None:
         logger.warning(f"Invalid model: {model}")
         return None
 
     fm_provider = model_map[model]
     fm_utils = {
         "Amazon": AwsTitanBedrockUtil,
@@ -22,15 +22,16 @@
         "Cohere": CohereBedrockUtil,
         "Meta": MetaBedrockUtil,
         "Mistral AI": MistralBedrockUtil
     }
 
     try:
         fm = fm_utils[fm_provider]()
-        result = fm.text_completion(bedrock_client=bedrock, model=model, prompt=prompt, **model_kwargs)
+        result = fm.text_completion(bedrock_client=bedrock, model=model, prompt=prompt, guardrail_identifier=guardrail_identifier,
+                                    guardrail_version=guardrail_version, **model_kwargs)
         logger.info(f"Text completion generated for model: {model}")
         return result
     except KeyError:
         logger.error(f"Unsupported provider: {fm_provider}")
     except Exception as e:
         logger.exception(f"Error generating text completion for model: {model}")
```

### Comparing `lambda_genai_util-0.0.4/src/lambda_genai_util/model_map.py` & `lambda_genai_util-0.0.5/src/lambda_genai_util/model_map.py`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.4/src/lambda_genai_util/prompt_service.py` & `lambda_genai_util-0.0.5/src/lambda_genai_util/prompt_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 import logging
 from lambda_util import yaml
 from lambda_util.lambda_genai_util.TextCompletionUtil import generate_text_completion
 from lambda_util.lambda_genai_util.model_map import model_map
 
-
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
-def read_prompt_config(file_path):
+
+def __read_prompt_config(file_path):
     try:
         with open(file_path, "r") as file:
             return yaml.safe_load(file)
     except FileNotFoundError:
         logger.error(f"The file {file_path} does not exist.")
     except Exception as e:
         logger.exception(f"Error decoding YAML in file {file_path}: {e}")
     return None
 
-def validate_model(service_id, model):
+
+def __validate_model(service_id, model):
     if service_map.get("PromptServices", {}).get(service_id):
         service = service_map["PromptServices"][service_id]
         allowed_providers = service.get("allowedFoundationModelProviders")
         if allowed_providers and model_map.get(model) in allowed_providers:
             return True
     logger.warning(f"Model ID {model} not allowed for service {service_id}")
     return False
 
-def validate_prompt_inputs(service_id, prompt_inputs):
+
+def __validate_prompt_inputs(service_id, prompt_inputs):
     if service_map.get("PromptServices", {}).get(service_id):
         service = service_map["PromptServices"][service_id]
         input_variables = service.get("inputVariables")
         if (not input_variables and not prompt_inputs) or (
-            input_variables and prompt_inputs and sorted(input_variables) == sorted(prompt_inputs.keys())
+                input_variables and prompt_inputs and sorted(input_variables) == sorted(prompt_inputs.keys())
         ):
             return True
     logger.warning(f"Invalid inputs provided for service ID {service_id}")
     return False
 
+
 def run_service(service_id, model_id, prompt_input_variables=None, **model_kwargs):
-    if validate_model(service_id, model_id) and validate_prompt_inputs(service_id, prompt_input_variables):
+    if __validate_model(service_id, model_id) and __validate_prompt_inputs(service_id, prompt_input_variables):
         prompt = service_map["PromptServices"][service_id]["prompt"]
+        guardrail_identifier = service_map["PromptServices"][service_id].get("guardrailIdentifier")
+        guardrail_version = service_map["PromptServices"][service_id].get("guardrailVersion")
         formatted_prompt = prompt.format(**(prompt_input_variables or {}))
-        return generate_text_completion(model_id, formatted_prompt, **model_kwargs)
+        return generate_text_completion(model_id, formatted_prompt, guardrail_identifier, guardrail_version,
+                                        **model_kwargs)
+
 
-service_map = read_prompt_config("prompt_store.yaml")
+service_map = __read_prompt_config("prompt_store.yaml")
```

### Comparing `lambda_genai_util-0.0.4/src/lambda_genai_util.egg-info/PKG-INFO` & `lambda_genai_util-0.0.5/src/lambda_genai_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda_genai_util
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for GenAI Utility for AWS Based development
 Author-email: Biprajeet Kar <biprokvs@gmail.com>
 Maintainer-email: Biprajeet Kar <biprokvs@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Biprajeet Kar
```

### Comparing `lambda_genai_util-0.0.4/src/lambda_genai_util.egg-info/SOURCES.txt` & `lambda_genai_util-0.0.5/src/lambda_genai_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

