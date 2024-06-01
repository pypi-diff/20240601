# Comparing `tmp/clonellm-0.0.2.tar.gz` & `tmp/clonellm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonellm-0.0.2.tar", max compression
+gzip compressed data, was "clonellm-0.0.3.tar", max compression
```

## Comparing `clonellm-0.0.2.tar` & `clonellm-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2024-05-24 08:18:44.196305 clonellm-0.0.2/LICENSE
--rw-r--r--   0        0        0     9668 2024-05-24 08:18:44.200305 clonellm-0.0.2/README.md
--rw-r--r--   0        0        0     1274 2024-05-24 08:18:44.200305 clonellm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      209 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/__init__.py
--rw-r--r--   0        0        0      745 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/_base.py
--rw-r--r--   0        0        0     2038 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/_prompt.py
--rw-r--r--   0        0        0     1119 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/_typing.py
--rw-r--r--   0        0        0    10078 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/core.py
--rw-r--r--   0        0        0     3190 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/embed.py
--rw-r--r--   0        0        0     1205 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/memory.py
--rw-r--r--   0        0        0        0 2024-05-24 08:18:44.200305 clonellm-0.0.2/src/clonellm/py.typed
--rw-r--r--   0        0        0    10510 1970-01-01 00:00:00.000000 clonellm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-01 01:45:57.209604 clonellm-0.0.3/LICENSE
+-rw-r--r--   0        0        0     9851 2024-06-01 01:45:57.209604 clonellm-0.0.3/README.md
+-rw-r--r--   0        0        0     1326 2024-06-01 01:45:57.213604 clonellm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      209 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/__init__.py
+-rw-r--r--   0        0        0      745 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/_base.py
+-rw-r--r--   0        0        0     1525 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/_prompt.py
+-rw-r--r--   0        0        0     1217 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/_typing.py
+-rw-r--r--   0        0        0     9553 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/core.py
+-rw-r--r--   0        0        0     3220 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/embed.py
+-rw-r--r--   0        0        0     1205 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/memory.py
+-rw-r--r--   0        0        0        0 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/py.typed
+-rw-r--r--   0        0        0    10693 1970-01-01 00:00:00.000000 clonellm-0.0.3/PKG-INFO
```

### Comparing `clonellm-0.0.2/LICENSE` & `clonellm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.2/README.md` & `clonellm-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 </h1>
 <p align="center">
     <p align="center">Create an AI clone of yourself using LLMs.</p>
 </p>   
 
 <h4 align="center">
     <a href="https://pypi.org/project/clonellm/" target="_blank">
-        <img src="https://img.shields.io/badge/release-v0.0.2-green" alt="Latest Release">
+        <img src="https://img.shields.io/badge/release-v0.0.3-green" alt="Latest Release">
     </a>
     <a href="https://pypi.org/project/clonellm/" target="_blank">
         <img src="https://img.shields.io/pypi/v/clonellm.svg" alt="PyPI Version">
     </a>
     <a target="_blank">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" alt="Python Versions">
     </a>
     <a target="_blank">
         <img src="https://img.shields.io/pypi/l/clonellm" alt="PyPI License">
     </a>
 </h4>
 
 ## Introduction
-A minimal Python package that enables you to create an AI clone of yourself using LLMs. Built on top of LiteLLM and Langchain, CloneLLM utilizes the Retrieval-Augmented Generation (RAG) to tailor AI responses as if you are answering the questions.
+A minimal Python package that enables you to create an AI clone of yourself using LLMs. Built on top of LiteLLM and LangChain, CloneLLM utilizes the Retrieval-Augmented Generation (RAG) to tailor AI responses as if you are answering the questions.
 
 You can input texts and documents about yourself — including personal information, professional experience, educational background, etc. — which are then embedded into a vector space for dynamic retrieval. This AI clone can act as a virtual assistant or digital representation, capable of handling queries and tasks in a manner that reflects the your own knowledge, tone, style and mannerisms.
 
 ## Installation
 
 ### Prerequisites
 Before installing CloneLLM, make sure you have Python 3.9 or newer installed on your machine. 
@@ -65,15 +65,15 @@
 
 documents = [
     Document(page_content="My name is Mehdi Samsami."),
     open("cv.txt", "r").read(),
 ]
 ```
 
-**Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings` or Langchain's embeddings. Then, initialize a clone with your documents, embedding model, and your referred LLM.
+**Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings` or LangChain's embeddings. Then, initialize a clone with your documents, embedding model, and your referred LLM.
 ```python
 from clonellm import CloneLLM, LiteLLMEmbeddings
 
 embedding = LiteLLMEmbeddings(model="text-embedding-ada-002")
 clone = CloneLLM(model="gpt-4-turbo", documents=documents, embedding=embedding)
 ```
 
@@ -94,15 +94,15 @@
 # Response: My name is Mehdi Samsami. How can I help you?
 ```
 
 ### Models
 At its core, CloneLLM utilizes LiteLLM for interactions with various LLMs. This is why you can choose from many different providers (100+ LLMs) supported by LiteLLM, including Bedrock, Azure, OpenAI, Cohere, Anthropic, Ollama, Sagemaker, HuggingFace, Replicate, etc.
 
 ### Document loaders
-You can use Langchain's document loaders to seamlessly import data from various sources into `Document` format. Take, for example, text and HTML loaders:
+You can use LangChain's document loaders to seamlessly import data from various sources into `Document` format. Take, for example, text and HTML loaders:
 ```python
 # !pip install unstructured
 from langchain_community.document_loaders import TextLoader, UnstructuredHTMLLoader
 
 documents = TextLoader("cv.txt").load() + UnstructuredHTMLLoader("linkedin.html").load()
 ```
 
@@ -115,15 +115,15 @@
     file_path='chat.json',
     jq_schema='.messages[].content',
     text_content=False
 ).load()
 ```
 
 ### Embeddings
-With `LiteLLMEmbeddings`, CloneLLM allows you to utilize embedding models from a variety of providers supported by LiteLLM. Additionally, you can select any preferred embedding model from Langchain's extensive range. Take, for example, the Hugging Face embedding:
+With `LiteLLMEmbeddings`, CloneLLM allows you to utilize embedding models from a variety of providers supported by LiteLLM. Additionally, you can select any preferred embedding model from LangChain's extensive range. Take, for example, the Hugging Face embedding:
 ```python
 # !pip install --upgrade --quiet sentence_transformers
 from langchain_community.embeddings import HuggingFaceEmbeddings
 from clonellm import CloneLLM
 import os
 
 os.environ["COHERE_API_KEY"] = "cohere-api-key"
@@ -276,14 +276,17 @@
 - [x] Add support for conversation history
 - [ ] Add support for RAG with no embedding (ingest the entire context into the prompt)
 - [x] Add support for string documents
 - [x] Fix mypy errors
 - [x] Rename `completion` methods to `invoke`
 - [x] Add support for streaming completion
 - [ ] Add support for custom system prompts
-- [ ] Add an attribute to return supported models
+- [x] Make `LiteLLMEmbeddings.all_embedding_models` a property
+- [ ] Add an attribute to `CloneLLM` to return supported models
 - [x] Add initial version of README
+- [ ] Describe `CloneLLM.clear_memory` method in README
 - [ ] Add documents
-- [ ] Add usage examples
-- [ ] Add initial unit tests
+- [x] Add usage examples
+- [x] Add unit tests for non-core modules
+- [ ] Add unit tests for core module
 - [x] Add GitHub workflow to run tests on PR
 - [x] Add GitHub workflow to publish to PyPI on release
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                                     [Logo]
                             ************ CClloonneeLLLLMM ************
                   Create an AI clone of yourself using LLMs.
      ****** _[[_LL_aa_tt_ee_ss_tt_ _RR_ee_ll_ee_aa_ss_ee_]]_[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]][[PPyytthhoonn VVeerrssiioonnss]][[PPyyPPII LLiicceennssee]] ******
 ## Introduction A minimal Python package that enables you to create an AI clone
-of yourself using LLMs. Built on top of LiteLLM and Langchain, CloneLLM
+of yourself using LLMs. Built on top of LiteLLM and LangChain, CloneLLM
 utilizes the Retrieval-Augmented Generation (RAG) to tailor AI responses as if
 you are answering the questions. You can input texts and documents about
 yourself â including personal information, professional experience,
 educational background, etc. â which are then embedded into a vector space
 for dynamic retrieval. This AI clone can act as a virtual assistant or digital
 representation, capable of handling queries and tasks in a manner that reflects
 the your own knowledge, tone, style and mannerisms. ## Installation ###
@@ -18,38 +18,38 @@
 the project directory cd clonellm # Install the package pip install . ``` ##
 Usage ### Getting started **Step 1**. Gather documents that contain relavant
 information about you. These documents form the base from which your AI clone
 will learn to mimic your tone, style, and expertise. ```python from
 langchain_core.documents import Document documents = [ Document
 (page_content="My name is Mehdi Samsami."), open("cv.txt", "r").read(), ] ```
 **Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings`
-or Langchain's embeddings. Then, initialize a clone with your documents,
+or LangChain's embeddings. Then, initialize a clone with your documents,
 embedding model, and your referred LLM. ```python from clonellm import
 CloneLLM, LiteLLMEmbeddings embedding = LiteLLMEmbeddings(model="text-
 embedding-ada-002") clone = CloneLLM(model="gpt-4-turbo", documents=documents,
 embedding=embedding) ``` **Step 3**. Configure environment variables to store
 API keys for embedding and LLM models. ```bash export OPENAI_API_KEY=sk-... ```
 **Step 4**. Fit the clone to the data (documents). ```python clone.fit() ```
 **Step 5**. Invoke the clone to ask questions. ```python clone.invoke("What's
 your name?") # Response: My name is Mehdi Samsami. How can I help you? ``` ###
 Models At its core, CloneLLM utilizes LiteLLM for interactions with various
 LLMs. This is why you can choose from many different providers (100+ LLMs)
 supported by LiteLLM, including Bedrock, Azure, OpenAI, Cohere, Anthropic,
 Ollama, Sagemaker, HuggingFace, Replicate, etc. ### Document loaders You can
-use Langchain's document loaders to seamlessly import data from various sources
+use LangChain's document loaders to seamlessly import data from various sources
 into `Document` format. Take, for example, text and HTML loaders: ```python #
 !pip install unstructured from langchain_community.document_loaders import
 TextLoader, UnstructuredHTMLLoader documents = TextLoader("cv.txt").load() +
 UnstructuredHTMLLoader("linkedin.html").load() ``` Or JSON loader: ```python #
 !pip install jq from langchain_community.document_loaders import JSONLoader
 documents = JSONLoader( file_path='chat.json', jq_schema='.messages[].content',
 text_content=False ).load() ``` ### Embeddings With `LiteLLMEmbeddings`,
 CloneLLM allows you to utilize embedding models from a variety of providers
 supported by LiteLLM. Additionally, you can select any preferred embedding
-model from Langchain's extensive range. Take, for example, the Hugging Face
+model from LangChain's extensive range. Take, for example, the Hugging Face
 embedding: ```python # !pip install --upgrade --quiet sentence_transformers
 from langchain_community.embeddings import HuggingFaceEmbeddings from clonellm
 import CloneLLM import os os.environ["COHERE_API_KEY"] = "cohere-api-key"
 embedding = HuggingFaceEmbeddings(model_name="sentence-transformers/all-mpnet-
 base-v2") clone = CloneLLM(model="command-xlarge-beta", documents=documents,
 embedding=embedding) ``` Or, the Llama-cpp embedding: ```python # !pip install
 --upgrade --quiet llama-cpp-python from langchain_community.embeddings import
@@ -107,12 +107,14 @@
 bugs, or improving documentation. - ð° **Share:** Post about CloneLLM on
 LinkedIn or other social platforms. Thank you for your interest in CloneLLM. We
 look forward to seeing what you'll create with your AI clone! ## TODO - [x] Add
 pre commit configuration file - [x] Add setup.py script - [x] Add support for
 conversation history - [ ] Add support for RAG with no embedding (ingest the
 entire context into the prompt) - [x] Add support for string documents - [x]
 Fix mypy errors - [x] Rename `completion` methods to `invoke` - [x] Add support
-for streaming completion - [ ] Add support for custom system prompts - [ ] Add
-an attribute to return supported models - [x] Add initial version of README -
-[ ] Add documents - [ ] Add usage examples - [ ] Add initial unit tests - [x]
-Add GitHub workflow to run tests on PR - [x] Add GitHub workflow to publish to
-PyPI on release
+for streaming completion - [ ] Add support for custom system prompts - [x] Make
+`LiteLLMEmbeddings.all_embedding_models` a property - [ ] Add an attribute to
+`CloneLLM` to return supported models - [x] Add initial version of README - [ ]
+Describe `CloneLLM.clear_memory` method in README - [ ] Add documents - [x] Add
+usage examples - [x] Add unit tests for non-core modules - [ ] Add unit tests
+for core module - [x] Add GitHub workflow to run tests on PR - [x] Add GitHub
+workflow to publish to PyPI on release
```

### Comparing `clonellm-0.0.2/pyproject.toml` & `clonellm-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "clonellm"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python package to create an AI clone of yourself using LLMs."
 packages = [{ from = "src", include = "clonellm" }]
 license = "MIT"
 authors = ["Mehdi Samsami <mehdisamsami@live.com>"]
 readme = "README.md"
 keywords = ["llm", "language models", "nlp", "rag", "ai", "ai clone"]
 repository = "https://github.com/msamsami/clonellm"
@@ -23,14 +23,15 @@
 pytest = "*"
 mypy = "*"
 pytest-asyncio = "*"
 ruff = "^0.4"
 types-setuptools = "^69.0.0.20240106"
 
 [tool.mypy]
+exclude=["tests", "examples"]
 namespace_packages = false
 files = ["src/clonellm/**/*.py"]
 check_untyped_defs = true
 disable_error_code = ["empty-body"]
 disallow_untyped_defs = false
 strict = true
 
@@ -38,14 +39,15 @@
 module = [
     "litellm",
     "openai.lib.streaming",
 ]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
+testpaths = ["tests"]
 filterwarnings = ["ignore"]
 
 [tool.ruff]
 include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
 line-length = 130
 # Use `ruff linter` to list available linters
 # https://beta.ruff.rs/docs/rules/
```

### Comparing `clonellm-0.0.2/src/clonellm/_base.py` & `clonellm-0.0.3/src/clonellm/_base.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.2/src/clonellm/_prompt.py` & `clonellm-0.0.3/src/clonellm/_prompt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
 
-__all__ = ("context_prompt", "user_profile_prompt", "contextualize_question_prompt", "history_prompt", "question_prompt")
+__all__ = ("context_prompt", "user_profile_prompt", "history_prompt", "question_prompt")
 
 
 context_prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are my human clone. Act as I would. Do not ask questions about me. If anyone asks, you are me."),
         ("system", "You are having a conversation with someone who wants to learn more about you."),
         ("system", "You MUST speak in first person. If you do not, you will be terminated."),
@@ -23,27 +23,14 @@
 
 user_profile_prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "Here is all the known information about me: {user_profile}"),
     ]
 )
 
-contextualize_question_prompt = ChatPromptTemplate.from_messages(
-    [
-        (
-            "system",
-            (
-                "Given a chat history and the latest user question hich might reference context in the chat history, "
-                "formulate a standalone question which can be understood without the chat history. "
-                "Do NOT answer the question, just reformulate it if needed and otherwise return it as is."
-            ),
-        ),
-    ]
-)
-
 history_prompt = ChatPromptTemplate.from_messages(
     [
         MessagesPlaceholder(variable_name="chat_history"),
     ]
 )
 
 question_prompt = ChatPromptTemplate.from_messages(
```

### Comparing `clonellm-0.0.2/src/clonellm/_typing.py` & `clonellm-0.0.3/src/clonellm/_typing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import datetime
 from typing import Any, Optional
 
 from pydantic import BaseModel
 
 __all__ = ("UserProfile",)
 
@@ -15,17 +16,17 @@
     birth_date: Optional[datetime.date | str] = None
     gender: Optional[str] = None
     city: Optional[str] = None
     state: Optional[str] = None
     country: Optional[str] = None
     phone_number: Optional[str] = None
     email: Optional[str] = None
-    education_experience: Optional[dict[str, Any]] = None
-    work_experience: Optional[dict[str, Any]] = None
-    expertise: Optional[list[str]] = None
+    education_experience: Optional[dict[str, Any] | list[dict[str, Any]]] = None
+    work_experience: Optional[dict[str, Any] | list[dict[str, Any]]] = None
+    expertise: Optional[list[str] | dict[str, Any]] = None
     home_page: Optional[str] = None
     github_page: Optional[str] = None
     linkedin_page: Optional[str] = None
 
     @property
     def full_name(self) -> str:
         return " ".join([self.first_name, self.middle_name or "", self.last_name])
```

### Comparing `clonellm-0.0.2/src/clonellm/core.py` & `clonellm-0.0.3/src/clonellm/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import annotations
 import json
 import logging
-from typing import Any, AsyncIterator, Iterator, Optional
+from operator import itemgetter
+from typing import Any, AsyncIterator, cast, Iterator, Optional
 from typing_extensions import Self
 import uuid
 
-from langchain.chains.combine_documents import create_stuff_documents_chain
-from langchain.chains.history_aware_retriever import create_history_aware_retriever
-from langchain.chains.retrieval import create_retrieval_chain
 from langchain.text_splitter import CharacterTextSplitter, TextSplitter
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.runnables import RunnablePassthrough, RunnableSerializable
 from langchain_core.runnables.history import RunnableWithMessageHistory
 from langchain_core.vectorstores import VectorStoreRetriever
 from langchain_community.chat_models import ChatLiteLLM
 from langchain_community.vectorstores import Chroma
 
 from ._base import LiteLLMMixin
-from ._prompt import context_prompt, user_profile_prompt, history_prompt, contextualize_question_prompt, question_prompt
+from ._prompt import context_prompt, user_profile_prompt, history_prompt, question_prompt
 from ._typing import UserProfile
 from .embed import LiteLLMEmbeddings
 from .memory import get_session_history, clear_session_history
 
 logging.getLogger("langchain_core").setLevel(logging.ERROR)
 
 __all__ = ("CloneLLM",)
@@ -154,79 +152,77 @@
         prompt = context_prompt.copy()
         if self.user_profile:
             prompt += user_profile_prompt.format_messages(user_profile=self._user_profile)
         prompt += question_prompt
         return {"context": self._get_retriever(), "input": RunnablePassthrough()} | prompt | self._llm | StrOutputParser()
 
     def _get_rag_chain_with_history(self) -> RunnableWithMessageHistory:
-        contextualize_system_prompt = contextualize_question_prompt + history_prompt + question_prompt
-        history_aware_retriever = create_history_aware_retriever(self._llm, self._get_retriever(), contextualize_system_prompt)
-
         prompt = context_prompt
         if self.user_profile:
             prompt += user_profile_prompt.format_messages(user_profile=self._user_profile)
         prompt += history_prompt
         prompt += question_prompt
-        question_answer_chain = create_stuff_documents_chain(self._llm, prompt)
 
-        rag_chain = create_retrieval_chain(history_aware_retriever, question_answer_chain)
+        context = itemgetter("input") | self._get_retriever()
+        first_step = RunnablePassthrough.assign(context=context)
+        rag_chain = first_step | prompt | self._llm | StrOutputParser()
+
         return RunnableWithMessageHistory(
-            rag_chain,
+            rag_chain,  # type: ignore[arg-type]
             get_session_history,
             input_messages_key="input",
             history_messages_key="chat_history",
-            output_messages_key="answer",
             output_parser=StrOutputParser(),
         )
 
     def invoke(self, prompt: str) -> str:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             response = rag_chain_with_history.invoke({"input": prompt}, config={"configurable": {"session_id": self._session_id}})
-            return response["answer"]  # type: ignore[no-any-return]
+            return cast(str, response.content)
         rag_chain = self._get_rag_chain()
         return rag_chain.invoke(prompt)
 
     async def ainvoke(self, prompt: str) -> str:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             response = await rag_chain_with_history.ainvoke(
                 {"input": prompt}, config={"configurable": {"session_id": self._session_id}}
             )
-            return response["answer"]  # type: ignore[no-any-return]
+            return cast(str, response.content)
         rag_chain = self._get_rag_chain()
         return await rag_chain.ainvoke(prompt)
 
     def stream(self, prompt: str) -> Iterator[str]:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
-            iterator = rag_chain_with_history.stream({"input": prompt}, config={"configurable": {"session_id": self._session_id}})
-            for chunk in iterator:
-                if "answer" in chunk:
-                    yield chunk["answer"]
-                else:
-                    yield ""
-        rag_chain = self._get_rag_chain()
-        for chunk in rag_chain.stream(prompt):
-            yield chunk
+            for chunk in rag_chain_with_history.stream(
+                {"input": prompt}, config={"configurable": {"session_id": self._session_id}}
+            ):
+                yield chunk.content
+        else:
+            rag_chain = self._get_rag_chain()
+            for chunk in rag_chain.stream(prompt):
+                yield chunk
 
     async def astream(self, prompt: str) -> AsyncIterator[str]:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             async for chunk in rag_chain_with_history.astream(
                 {"input": prompt}, config={"configurable": {"session_id": self._session_id}}
             ):
-                yield chunk["answer"]
-        rag_chain = self._get_rag_chain()
-        async for chunk in rag_chain.astream(prompt):
-            yield chunk
+                yield chunk.content
+        else:
+            rag_chain = self._get_rag_chain()
+            async for chunk in rag_chain.astream(prompt):
+                yield chunk
 
     def clear_memory(self) -> None:
         clear_session_history(self._session_id)
         self._session_id = str(uuid.uuid4())
 
     def __repr__(self) -> str:
         return f"CloneLLM<(model='{self.model}', memory={self.memory})>"
```

### Comparing `clonellm-0.0.2/src/clonellm/embed.py` & `clonellm-0.0.3/src/clonellm/embed.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,29 +20,29 @@
     """
 
     def __init__(self, model: str, api_key: Optional[str] = None, dimensions: Optional[int] = None, **kwargs: Any) -> None:
         super().__init__(model, api_key, **kwargs)
         self.dimensions = dimensions
 
     def embed_documents(self, texts: list[str]) -> list[list[float]]:
-        """Call out to LLM's embedding endpoint for embedding search docs.
+        """Call out to LLM's embedding endpoint for embedding a list of documents.
 
         Args:
             texts (list[str]): The list of texts to embed.
 
         Returns:
             list[list[float]]: List of embeddings, one for each text.
         """
         response = embedding(
             model=self.model, input=texts, api_key=self.api_key, dimensions=self.dimensions, **self._litellm_kwargs
         )
         return [r["embedding"] for r in response.data]
 
     async def aembed_documents(self, texts: list[str]) -> list[list[float]]:
-        """Call out to LLM's embedding endpoint async for embedding search docs.
+        """Call out to LLM's embedding endpoint async for embedding a list of documents.
 
         Args:
             texts (list[str]): The list of texts to embed.
 
         Returns:
             list[list[float]]: List of embeddings, one for each text.
         """
@@ -70,14 +70,15 @@
 
         Returns:
             list[float]: Embedding for the text.
         """
         embeddings = await self.aembed_documents([text])
         return embeddings[0]
 
+    @property
     def all_embedding_models(self) -> list[str]:
         """
         Returns the names of supported embedding models.
         """
         return cast(list[str], all_embedding_models)
 
     def __repr__(self) -> str:
```

### Comparing `clonellm-0.0.2/src/clonellm/memory.py` & `clonellm-0.0.3/src/clonellm/memory.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.2/PKG-INFO` & `clonellm-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonellm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package to create an AI clone of yourself using LLMs.
 Home-page: https://github.com/msamsami/clonellm
 License: MIT
 Keywords: llm,language models,nlp,rag,ai,ai clone
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Requires-Python: >=3.9,<3.13
@@ -28,29 +28,29 @@
 </h1>
 <p align="center">
     <p align="center">Create an AI clone of yourself using LLMs.</p>
 </p>   
 
 <h4 align="center">
     <a href="https://pypi.org/project/clonellm/" target="_blank">
-        <img src="https://img.shields.io/badge/release-v0.0.2-green" alt="Latest Release">
+        <img src="https://img.shields.io/badge/release-v0.0.3-green" alt="Latest Release">
     </a>
     <a href="https://pypi.org/project/clonellm/" target="_blank">
         <img src="https://img.shields.io/pypi/v/clonellm.svg" alt="PyPI Version">
     </a>
     <a target="_blank">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" alt="Python Versions">
     </a>
     <a target="_blank">
         <img src="https://img.shields.io/pypi/l/clonellm" alt="PyPI License">
     </a>
 </h4>
 
 ## Introduction
-A minimal Python package that enables you to create an AI clone of yourself using LLMs. Built on top of LiteLLM and Langchain, CloneLLM utilizes the Retrieval-Augmented Generation (RAG) to tailor AI responses as if you are answering the questions.
+A minimal Python package that enables you to create an AI clone of yourself using LLMs. Built on top of LiteLLM and LangChain, CloneLLM utilizes the Retrieval-Augmented Generation (RAG) to tailor AI responses as if you are answering the questions.
 
 You can input texts and documents about yourself — including personal information, professional experience, educational background, etc. — which are then embedded into a vector space for dynamic retrieval. This AI clone can act as a virtual assistant or digital representation, capable of handling queries and tasks in a manner that reflects the your own knowledge, tone, style and mannerisms.
 
 ## Installation
 
 ### Prerequisites
 Before installing CloneLLM, make sure you have Python 3.9 or newer installed on your machine. 
@@ -87,15 +87,15 @@
 
 documents = [
     Document(page_content="My name is Mehdi Samsami."),
     open("cv.txt", "r").read(),
 ]
 ```
 
-**Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings` or Langchain's embeddings. Then, initialize a clone with your documents, embedding model, and your referred LLM.
+**Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings` or LangChain's embeddings. Then, initialize a clone with your documents, embedding model, and your referred LLM.
 ```python
 from clonellm import CloneLLM, LiteLLMEmbeddings
 
 embedding = LiteLLMEmbeddings(model="text-embedding-ada-002")
 clone = CloneLLM(model="gpt-4-turbo", documents=documents, embedding=embedding)
 ```
 
@@ -116,15 +116,15 @@
 # Response: My name is Mehdi Samsami. How can I help you?
 ```
 
 ### Models
 At its core, CloneLLM utilizes LiteLLM for interactions with various LLMs. This is why you can choose from many different providers (100+ LLMs) supported by LiteLLM, including Bedrock, Azure, OpenAI, Cohere, Anthropic, Ollama, Sagemaker, HuggingFace, Replicate, etc.
 
 ### Document loaders
-You can use Langchain's document loaders to seamlessly import data from various sources into `Document` format. Take, for example, text and HTML loaders:
+You can use LangChain's document loaders to seamlessly import data from various sources into `Document` format. Take, for example, text and HTML loaders:
 ```python
 # !pip install unstructured
 from langchain_community.document_loaders import TextLoader, UnstructuredHTMLLoader
 
 documents = TextLoader("cv.txt").load() + UnstructuredHTMLLoader("linkedin.html").load()
 ```
 
@@ -137,15 +137,15 @@
     file_path='chat.json',
     jq_schema='.messages[].content',
     text_content=False
 ).load()
 ```
 
 ### Embeddings
-With `LiteLLMEmbeddings`, CloneLLM allows you to utilize embedding models from a variety of providers supported by LiteLLM. Additionally, you can select any preferred embedding model from Langchain's extensive range. Take, for example, the Hugging Face embedding:
+With `LiteLLMEmbeddings`, CloneLLM allows you to utilize embedding models from a variety of providers supported by LiteLLM. Additionally, you can select any preferred embedding model from LangChain's extensive range. Take, for example, the Hugging Face embedding:
 ```python
 # !pip install --upgrade --quiet sentence_transformers
 from langchain_community.embeddings import HuggingFaceEmbeddings
 from clonellm import CloneLLM
 import os
 
 os.environ["COHERE_API_KEY"] = "cohere-api-key"
@@ -298,15 +298,18 @@
 - [x] Add support for conversation history
 - [ ] Add support for RAG with no embedding (ingest the entire context into the prompt)
 - [x] Add support for string documents
 - [x] Fix mypy errors
 - [x] Rename `completion` methods to `invoke`
 - [x] Add support for streaming completion
 - [ ] Add support for custom system prompts
-- [ ] Add an attribute to return supported models
+- [x] Make `LiteLLMEmbeddings.all_embedding_models` a property
+- [ ] Add an attribute to `CloneLLM` to return supported models
 - [x] Add initial version of README
+- [ ] Describe `CloneLLM.clear_memory` method in README
 - [ ] Add documents
-- [ ] Add usage examples
-- [ ] Add initial unit tests
+- [x] Add usage examples
+- [x] Add unit tests for non-core modules
+- [ ] Add unit tests for core module
 - [x] Add GitHub workflow to run tests on PR
 - [x] Add GitHub workflow to publish to PyPI on release
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clonellm Version: 0.0.2 Summary: Python package to
+Metadata-Version: 2.1 Name: clonellm Version: 0.0.3 Summary: Python package to
 create an AI clone of yourself using LLMs. Home-page: https://github.com/
 msamsami/clonellm License: MIT Keywords: llm,language models,nlp,rag,ai,ai
 clone Author: Mehdi Samsami Author-email: mehdisamsami@live.com Requires-
 Python: >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -11,15 +11,15 @@
 Repository, https://github.com/msamsami/clonellm Description-Content-Type:
 text/markdown
                                     [Logo]
                             ************ CClloonneeLLLLMM ************
                   Create an AI clone of yourself using LLMs.
      ****** _[[_LL_aa_tt_ee_ss_tt_ _RR_ee_ll_ee_aa_ss_ee_]]_[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]][[PPyytthhoonn VVeerrssiioonnss]][[PPyyPPII LLiicceennssee]] ******
 ## Introduction A minimal Python package that enables you to create an AI clone
-of yourself using LLMs. Built on top of LiteLLM and Langchain, CloneLLM
+of yourself using LLMs. Built on top of LiteLLM and LangChain, CloneLLM
 utilizes the Retrieval-Augmented Generation (RAG) to tailor AI responses as if
 you are answering the questions. You can input texts and documents about
 yourself â including personal information, professional experience,
 educational background, etc. â which are then embedded into a vector space
 for dynamic retrieval. This AI clone can act as a virtual assistant or digital
 representation, capable of handling queries and tasks in a manner that reflects
 the your own knowledge, tone, style and mannerisms. ## Installation ###
@@ -30,38 +30,38 @@
 the project directory cd clonellm # Install the package pip install . ``` ##
 Usage ### Getting started **Step 1**. Gather documents that contain relavant
 information about you. These documents form the base from which your AI clone
 will learn to mimic your tone, style, and expertise. ```python from
 langchain_core.documents import Document documents = [ Document
 (page_content="My name is Mehdi Samsami."), open("cv.txt", "r").read(), ] ```
 **Step 2**. Initialize an embedding model using CloneLLM's `LiteLLMEmbeddings`
-or Langchain's embeddings. Then, initialize a clone with your documents,
+or LangChain's embeddings. Then, initialize a clone with your documents,
 embedding model, and your referred LLM. ```python from clonellm import
 CloneLLM, LiteLLMEmbeddings embedding = LiteLLMEmbeddings(model="text-
 embedding-ada-002") clone = CloneLLM(model="gpt-4-turbo", documents=documents,
 embedding=embedding) ``` **Step 3**. Configure environment variables to store
 API keys for embedding and LLM models. ```bash export OPENAI_API_KEY=sk-... ```
 **Step 4**. Fit the clone to the data (documents). ```python clone.fit() ```
 **Step 5**. Invoke the clone to ask questions. ```python clone.invoke("What's
 your name?") # Response: My name is Mehdi Samsami. How can I help you? ``` ###
 Models At its core, CloneLLM utilizes LiteLLM for interactions with various
 LLMs. This is why you can choose from many different providers (100+ LLMs)
 supported by LiteLLM, including Bedrock, Azure, OpenAI, Cohere, Anthropic,
 Ollama, Sagemaker, HuggingFace, Replicate, etc. ### Document loaders You can
-use Langchain's document loaders to seamlessly import data from various sources
+use LangChain's document loaders to seamlessly import data from various sources
 into `Document` format. Take, for example, text and HTML loaders: ```python #
 !pip install unstructured from langchain_community.document_loaders import
 TextLoader, UnstructuredHTMLLoader documents = TextLoader("cv.txt").load() +
 UnstructuredHTMLLoader("linkedin.html").load() ``` Or JSON loader: ```python #
 !pip install jq from langchain_community.document_loaders import JSONLoader
 documents = JSONLoader( file_path='chat.json', jq_schema='.messages[].content',
 text_content=False ).load() ``` ### Embeddings With `LiteLLMEmbeddings`,
 CloneLLM allows you to utilize embedding models from a variety of providers
 supported by LiteLLM. Additionally, you can select any preferred embedding
-model from Langchain's extensive range. Take, for example, the Hugging Face
+model from LangChain's extensive range. Take, for example, the Hugging Face
 embedding: ```python # !pip install --upgrade --quiet sentence_transformers
 from langchain_community.embeddings import HuggingFaceEmbeddings from clonellm
 import CloneLLM import os os.environ["COHERE_API_KEY"] = "cohere-api-key"
 embedding = HuggingFaceEmbeddings(model_name="sentence-transformers/all-mpnet-
 base-v2") clone = CloneLLM(model="command-xlarge-beta", documents=documents,
 embedding=embedding) ``` Or, the Llama-cpp embedding: ```python # !pip install
 --upgrade --quiet llama-cpp-python from langchain_community.embeddings import
@@ -119,12 +119,14 @@
 bugs, or improving documentation. - ð° **Share:** Post about CloneLLM on
 LinkedIn or other social platforms. Thank you for your interest in CloneLLM. We
 look forward to seeing what you'll create with your AI clone! ## TODO - [x] Add
 pre commit configuration file - [x] Add setup.py script - [x] Add support for
 conversation history - [ ] Add support for RAG with no embedding (ingest the
 entire context into the prompt) - [x] Add support for string documents - [x]
 Fix mypy errors - [x] Rename `completion` methods to `invoke` - [x] Add support
-for streaming completion - [ ] Add support for custom system prompts - [ ] Add
-an attribute to return supported models - [x] Add initial version of README -
-[ ] Add documents - [ ] Add usage examples - [ ] Add initial unit tests - [x]
-Add GitHub workflow to run tests on PR - [x] Add GitHub workflow to publish to
-PyPI on release
+for streaming completion - [ ] Add support for custom system prompts - [x] Make
+`LiteLLMEmbeddings.all_embedding_models` a property - [ ] Add an attribute to
+`CloneLLM` to return supported models - [x] Add initial version of README - [ ]
+Describe `CloneLLM.clear_memory` method in README - [ ] Add documents - [x] Add
+usage examples - [x] Add unit tests for non-core modules - [ ] Add unit tests
+for core module - [x] Add GitHub workflow to run tests on PR - [x] Add GitHub
+workflow to publish to PyPI on release
```

