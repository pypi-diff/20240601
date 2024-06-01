# Comparing `tmp/ollama_instructor-0.1.2.tar.gz` & `tmp/ollama_instructor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama_instructor-0.1.2.tar", max compression
+gzip compressed data, was "ollama_instructor-0.1.3.tar", max compression
```

## Comparing `ollama_instructor-0.1.2.tar` & `ollama_instructor-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-30 06:53:56.160597 ollama_instructor-0.1.2/LICENSE
--rw-r--r--   0        0        0     5624 2024-05-30 13:38:56.481958 ollama_instructor-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-30 14:12:52.173166 ollama_instructor-0.1.2/ollama_instructor/__init__.py
--rw-r--r--   0        0        0     3803 2024-05-30 06:53:56.162638 ollama_instructor-0.1.2/ollama_instructor/cleaner.py
--rw-r--r--   0        0        0    19217 2024-05-30 06:53:56.162850 ollama_instructor-0.1.2/ollama_instructor/ollama_instructor_client.py
--rw-r--r--   0        0        0     3500 2024-05-30 06:53:56.163045 ollama_instructor-0.1.2/ollama_instructor/prompt_manager.py
--rw-r--r--   0        0        0     6693 2024-05-30 14:12:28.282021 ollama_instructor-0.1.2/ollama_instructor/validation_manager.py
--rw-r--r--   0        0        0     1032 2024-05-30 14:15:17.954556 ollama_instructor-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 ollama_instructor-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-30 06:53:56.160597 ollama_instructor-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5818 2024-06-01 12:30:26.356002 ollama_instructor-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 14:12:52.173166 ollama_instructor-0.1.3/ollama_instructor/__init__.py
+-rw-r--r--   0        0        0     3803 2024-05-30 06:53:56.162638 ollama_instructor-0.1.3/ollama_instructor/cleaner.py
+-rw-r--r--   0        0        0    15757 2024-05-30 14:23:44.226694 ollama_instructor-0.1.3/ollama_instructor/ollama_instructor_client.py
+-rw-r--r--   0        0        0     3500 2024-05-30 06:53:56.163045 ollama_instructor-0.1.3/ollama_instructor/prompt_manager.py
+-rw-r--r--   0        0        0     6693 2024-05-30 14:12:28.282021 ollama_instructor-0.1.3/ollama_instructor/validation_manager.py
+-rw-r--r--   0        0        0     1032 2024-06-01 12:46:45.368228 ollama_instructor-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7203 1970-01-01 00:00:00.000000 ollama_instructor-0.1.3/PKG-INFO
```

### Comparing `ollama_instructor-0.1.2/LICENSE` & `ollama_instructor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama_instructor-0.1.2/README.md` & `ollama_instructor-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # ollama-instructor
 
 `ollama-instructor` is a lightweight Python library that provides a convenient wrapper around the Client of the renowned Ollama repository, extending it with validation features for obtaining valid JSON responses from a Large Language Model (LLM). Utilizing Pydantic, `ollama-instructor` allows users to specify models for JSON schemas and data validation, ensuring that responses from LLMs adhere to the defined schema.
 
-> **Note**: This library has a native support for the Ollamas Python client. If you want to have more flexibility with other providers like Groq, OpenAI, Perplexity and more, have a look into the great library of [instrutor](https://github.com/jxnl/instructor) of Jason Lui.
+> **Note 1**: This library has a native support for the Ollamas Python client. If you want to have more flexibility with other providers like Groq, OpenAI, Perplexity and more, have a look into the great library of [instrutor](https://github.com/jxnl/instructor) of Jason Lui.
 
+> **Note 2**: This library depends on having [Ollama](https://ollama.com) installed and running. For more information, please refer to the official website of Ollama.
 
 ## Features
 
 - Easy integration with the Ollama repository for running open-source LLMs locally. See: 
     - https://github.com/ollama/ollama
     - https://github.com/ollama/ollama-python
 - Data validation using Pydantic models to ensure the JSON response from a LLM meets the specified schema. See:
     - https://docs.pydantic.dev/latest/
 - Retries with error guidance if the LLM returns invalid responses. You can set the maxium number of retries.
 - Allow partial responses to be returned by setting the `allow_partial` flag to True. This will try to clean set invalid data within the response and set it to `None`. Unsetted data (not part of the Pydantic model) will be deleted from the response.
 
 `ollama-instructor` can help you to get structured and reliable JSON from local LLMs like:
-- Llama3
+- llama3
 - phi3
 - mistral
-- Gemma
+- gemma
+- ...
 
 `ollama-instructor` can be your starting point to build agents by your self. Have full control over agent flows without relying on complex agent framework.
 
 
 ## Installation
 
 To install `ollama-instructor`, run the following command in your terminal:
@@ -101,17 +103,17 @@
 ### chat_completion & chat_completion_with_stream
 
 The `chat_completion` and `chat_completion_with_stream` methods are the main methods of the library. They are used to generate text completions from a given prompt.
 
 `ollama-instructor` uses `chat_completion` and `chat_completion_with_stream` to expand the `chat` method of `Ollama`. For all available arguments of `chat` see the [Ollama documentation](https://github.com/ollama/ollama).
 
 The following arguments are added to the `chat` method within `chat_completion` and `chat_completion_with_stream`:
-- `pydantic_model`: a `pydantic.BaseModel` class that is used to firstly instruct the LLM with the JSON schema of the `pydantic.BaseModel` and secondly to validate the response of the LLM with the built-in validation of `pydantic`.
+- `pydantic_model`: a class of Pydantic's `BaseModel` class that is used to firstly instruct the LLM with the JSON schema of the `BaseModel` and secondly to validate the response of the LLM with the built-in validation of [Pydantic](https://docs.pydantic.dev/latest/).
 - `retries`: the number of retries if the LLM fails to generate a valid response (default: `3`). If a LLM fails the retry will provide the last response of the LLM with the given `ValidationError` and insructs it to generate a valid response.
-- `allow_partial`: If set to `True` `ollama-instructor` will modify the `pydantic.BaseModel` to allow partial responses. In this case it makes sure to provide the correct instance of the JSON schema but with default or None values. Therefore, it is useful to provide default values within the `pydantic.BaseModel`. With the improvement of this library you will find examples and best practice guides on that topic in the [docs](/docs/) folder.
+- `allow_partial`: If set to `True` `ollama-instructor` will modify the `BaseModel` to allow partial responses. In this case it makes sure to provide the correct instance of the JSON schema but with default or None values. Therefore, it is useful to provide default values within the `BaseModel`. With the improvement of this library you will find examples and best practice guides on that topic in the [docs](/docs/) folder.
 
 
 ## Documentation and examples
 - It was always my goal to have a well documented library. Therefore, have a look into the repositorys code to get an idea how to use it.
 - There will be a great bunch of how-to-use guides and examples in the [docs](/docs/) folder (coming soon).
 - If you need more information about the library, please feel free to open an issue.
```

### Comparing `ollama_instructor-0.1.2/ollama_instructor/cleaner.py` & `ollama_instructor-0.1.3/ollama_instructor/cleaner.py`

 * *Files identical despite different names*

### Comparing `ollama_instructor-0.1.2/ollama_instructor/ollama_instructor_client.py` & `ollama_instructor-0.1.3/ollama_instructor/ollama_instructor_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     The ollama instructor will return a modified version of Ollama's response dict. The modifications are as follows:
     - `validation_errors`: This will contain the `ValidationError`raised during Pydantic's validation, if the response of the LLM is invalid.
     - `raw_response`: This will contain the raw response from the LLM.
 
     
     Example:
     ```Python
-    from ollama_instructor import OllamaInstructorClient
+    from ollama_instructor.ollama_instructor_client import OllamaInstructorClient
     from pydantic import BaseModel
 
     class Person(BaseModel):
         name: str
         age: int
 
     client = OllamaInstructorClient(host="http://localhost:11434") # by default the host is http://localhost:11434
@@ -95,15 +95,15 @@
             Dict[str, Any]: The Dict contains all key-value-pairs known from `Ollama` and some additional like:
                 - the last validation error if there is one
                 - the left retries
                 - the raw response (the dictionary of 'message') of the LLM before the validation does it's magic
 
         Example:
             ```Python
-            from ollama_instructor import OllamaInstructorClient
+            from ollama_instructor.ollama_instructor_client import OllamaInstructorClient
             from pydantic import BaseModel
             from enum import Enum
 
             client = OllamaInstructorClient(host='http://localhost:11434')
 
             class Gender(Enum):
                 MALE = 'male'
@@ -225,15 +225,15 @@
             **kwargs: Additional arguments to pass to the LLM client of `Ollama`.
 
         Returns:
             Generator[Dict[str, Any], None, None]: The generated response.
 
         Example:
             ```Python
-            from ollama_instructor import OllamaInstructorClient
+            from ollama_instructor.ollama_instructor_client import OllamaInstructorClient
             from pydantic import BaseModel
             from enum import Enum
 
             client = OllamaInstructorClient(host='http://localhost:11434')
 
             class Gender(Enum):
                 MALE = 'male'
@@ -334,95 +334,8 @@
                     yield chunk
                     return chunk
                    
             except Exception as e:
                 ic()
                 ic(e)
                 raise e
-            
-
-    ####################
-    # DEPRECATED
-    ####################
-    def chat_completion_with_stream_old(self, pydantic_model: Type[BaseModel], messages: List[Dict[str, Any]], model: str, retries: int = 3, format: Literal['', 'json'] = 'json', **kwargs) -> Generator[Dict[str, Any], None, None]: 
-        '''
-        ATTENTION: This method is deprecated. Use `chat_completion_with_stream` instead.
-
-
-        Chat with the model and validate the response with the provided Pydantic model.
-
-        **This method is for streaming.** Use `chat_completion` instead.
-
-        Args:
-            pydantic_model (Type[BaseModel]): The Pydantic model for validation.
-            messages (List[Dict[str, Any]]): The chat messages.
-            model (str): The LLM model.
-            retries (int): The number of retries if the response is not valid.
-            format (Literal['', 'json']): The format of the response.
-            **kwargs: Additional arguments to pass to the LLM client of `Ollama`.
-
-        Returns:
-            Generator[Dict[str, Any], None, None]: The generated response.
-
-        Example:
-            ```Python
-            from ollama_instructor import OllamaInstructorClient
-            from pydantic import BaseModel
-            from enum import Enum
-
-            client = OllamaInstructorClient(host='http://localhost:11434')
-
-            class Gender(Enum):
-                MALE = 'male'
-                FEMALE = 'female'
-
-            class Person(BaseModel):
-                name: str
-                age: int
-                gender: Gender
-
-            response = client.chat_completion_with_stream_old(
-                pydantic_model=Person,
-                messages=[
-                    {
-                        'role': 'user',
-                        'content': 'Jason is 45 years old.'
-                    }
-                ],
-                model='mistral:7b-instruct',
-            )
-            
-            for chunk in response:
-                print(chunk['message']['content'])
-            # >>> Output example:
-            # {'name': 'Jason', 'age': 45, 'gender': 'male'}
-        '''
-        self.retry_counter = retries
-        if self.retry_counter == retries:
-            messages = self.chat_prompt_manager.create_chat_prompt_for_json(pydantic_model=pydantic_model, messages=messages)
-            self.chat_history = messages
-        expanding_response = ""
-        response = self.ollama_client.chat(
-            model=model,
-            messages=messages,
-            format=format,
-            stream=True,
-            **kwargs
-        )
-        try:
-            ic()
-            for chunk in response:
-                if self.chat_history != []:
-                    self.chat_history.pop(-1)
-                
-                expanding_response += chunk['message']['content']
-                chunk['message']['content'] = expanding_response
-                # Validation block
-                chunk = self.validation_manager.validate_chat_completion_with_stream(chunk=chunk, pydantic_model=pydantic_model)
-                validation_result = self.validation_manager.validate_for_error_message(response=chunk, pydantic_model=pydantic_model)
-                chunk = self.validation_manager.add_error_log_to_final_response(response=chunk, error_message=validation_result, raw_message=expanding_response)
-                # Append chat_history
-                self.chat_history += [chunk['message']]
-                yield chunk
-        except Exception as e:
-            ic()
-            raise e
+
```

### Comparing `ollama_instructor-0.1.2/ollama_instructor/prompt_manager.py` & `ollama_instructor-0.1.3/ollama_instructor/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `ollama_instructor-0.1.2/ollama_instructor/validation_manager.py` & `ollama_instructor-0.1.3/ollama_instructor/validation_manager.py`

 * *Files identical despite different names*

### Comparing `ollama_instructor-0.1.2/pyproject.toml` & `ollama_instructor-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ollama-instructor"
-version = "0.1.2"
+version = "0.1.3"
 description = "Instruct and validate structured outputs from LLMs with Ollama."
 authors = ["Lennart Pollvogt"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/lennartpollvogt/ollama-instructor"
 repository = "https://github.com/lennartpollvogt/ollama-instructor"
 documentation = "https://github.com/lennartpollvogt/ollama-instructor/tree/main/docs"
```

### Comparing `ollama_instructor-0.1.2/PKG-INFO` & `ollama_instructor-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-instructor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Instruct and validate structured outputs from LLMs with Ollama.
 Home-page: https://github.com/lennartpollvogt/ollama-instructor
 License: MIT
 Keywords: ollama,pydantic,validation,json-schema,json,instructor,prompting,local-llm,llm
 Author: Lennart Pollvogt
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -28,32 +28,34 @@
 Project-URL: Repository, https://github.com/lennartpollvogt/ollama-instructor
 Description-Content-Type: text/markdown
 
 # ollama-instructor
 
 `ollama-instructor` is a lightweight Python library that provides a convenient wrapper around the Client of the renowned Ollama repository, extending it with validation features for obtaining valid JSON responses from a Large Language Model (LLM). Utilizing Pydantic, `ollama-instructor` allows users to specify models for JSON schemas and data validation, ensuring that responses from LLMs adhere to the defined schema.
 
-> **Note**: This library has a native support for the Ollamas Python client. If you want to have more flexibility with other providers like Groq, OpenAI, Perplexity and more, have a look into the great library of [instrutor](https://github.com/jxnl/instructor) of Jason Lui.
+> **Note 1**: This library has a native support for the Ollamas Python client. If you want to have more flexibility with other providers like Groq, OpenAI, Perplexity and more, have a look into the great library of [instrutor](https://github.com/jxnl/instructor) of Jason Lui.
 
+> **Note 2**: This library depends on having [Ollama](https://ollama.com) installed and running. For more information, please refer to the official website of Ollama.
 
 ## Features
 
 - Easy integration with the Ollama repository for running open-source LLMs locally. See: 
     - https://github.com/ollama/ollama
     - https://github.com/ollama/ollama-python
 - Data validation using Pydantic models to ensure the JSON response from a LLM meets the specified schema. See:
     - https://docs.pydantic.dev/latest/
 - Retries with error guidance if the LLM returns invalid responses. You can set the maxium number of retries.
 - Allow partial responses to be returned by setting the `allow_partial` flag to True. This will try to clean set invalid data within the response and set it to `None`. Unsetted data (not part of the Pydantic model) will be deleted from the response.
 
 `ollama-instructor` can help you to get structured and reliable JSON from local LLMs like:
-- Llama3
+- llama3
 - phi3
 - mistral
-- Gemma
+- gemma
+- ...
 
 `ollama-instructor` can be your starting point to build agents by your self. Have full control over agent flows without relying on complex agent framework.
 
 
 ## Installation
 
 To install `ollama-instructor`, run the following command in your terminal:
@@ -131,17 +133,17 @@
 ### chat_completion & chat_completion_with_stream
 
 The `chat_completion` and `chat_completion_with_stream` methods are the main methods of the library. They are used to generate text completions from a given prompt.
 
 `ollama-instructor` uses `chat_completion` and `chat_completion_with_stream` to expand the `chat` method of `Ollama`. For all available arguments of `chat` see the [Ollama documentation](https://github.com/ollama/ollama).
 
 The following arguments are added to the `chat` method within `chat_completion` and `chat_completion_with_stream`:
-- `pydantic_model`: a `pydantic.BaseModel` class that is used to firstly instruct the LLM with the JSON schema of the `pydantic.BaseModel` and secondly to validate the response of the LLM with the built-in validation of `pydantic`.
+- `pydantic_model`: a class of Pydantic's `BaseModel` class that is used to firstly instruct the LLM with the JSON schema of the `BaseModel` and secondly to validate the response of the LLM with the built-in validation of [Pydantic](https://docs.pydantic.dev/latest/).
 - `retries`: the number of retries if the LLM fails to generate a valid response (default: `3`). If a LLM fails the retry will provide the last response of the LLM with the given `ValidationError` and insructs it to generate a valid response.
-- `allow_partial`: If set to `True` `ollama-instructor` will modify the `pydantic.BaseModel` to allow partial responses. In this case it makes sure to provide the correct instance of the JSON schema but with default or None values. Therefore, it is useful to provide default values within the `pydantic.BaseModel`. With the improvement of this library you will find examples and best practice guides on that topic in the [docs](/docs/) folder.
+- `allow_partial`: If set to `True` `ollama-instructor` will modify the `BaseModel` to allow partial responses. In this case it makes sure to provide the correct instance of the JSON schema but with default or None values. Therefore, it is useful to provide default values within the `BaseModel`. With the improvement of this library you will find examples and best practice guides on that topic in the [docs](/docs/) folder.
 
 
 ## Documentation and examples
 - It was always my goal to have a well documented library. Therefore, have a look into the repositorys code to get an idea how to use it.
 - There will be a great bunch of how-to-use guides and examples in the [docs](/docs/) folder (coming soon).
 - If you need more information about the library, please feel free to open an issue.
```

