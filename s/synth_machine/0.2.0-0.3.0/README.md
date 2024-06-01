# Comparing `tmp/synth_machine-0.2.0.tar.gz` & `tmp/synth_machine-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_machine-0.2.0.tar", max compression
+gzip compressed data, was "synth_machine-0.3.0.tar", max compression
```

## Comparing `synth_machine-0.2.0.tar` & `synth_machine-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0    35149 2024-05-13 16:56:20.221981 synth_machine-0.2.0/LICENSE
--rw-r--r--   0        0        0      492 2024-05-13 16:56:20.221981 synth_machine-0.2.0/README.md
--rw-r--r--   0        0        0     1221 2024-05-13 16:56:20.225981 synth_machine-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      335 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/__init__.py
--rw-r--r--   0        0        0     3949 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/config.py
--rw-r--r--   0        0        0      454 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/cost.py
--rw-r--r--   0        0        0      436 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/executor_factory.py
--rw-r--r--   0        0        0      266 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/executors/__init__.py
--rw-r--r--   0        0        0     4421 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/executors/anthropic.py
--rw-r--r--   0        0        0      732 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/executors/base.py
--rw-r--r--   0        0        0     3636 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/executors/openai.py
--rw-r--r--   0        0        0     3803 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/executors/togetherai.py
--rw-r--r--   0        0        0    22726 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/machine.py
--rw-r--r--   0        0        0      919 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/machine_config.py
--rw-r--r--   0        0        0     1508 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/runners.py
--rw-r--r--   0        0        0     3070 2024-05-13 16:56:20.225981 synth_machine-0.2.0/synth_machine/safety.py
--rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 synth_machine-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-01 21:03:53.658851 synth_machine-0.3.0/LICENSE
+-rw-r--r--   0        0        0      492 2024-06-01 21:03:53.658851 synth_machine-0.3.0/README.md
+-rw-r--r--   0        0        0     1222 2024-06-01 21:03:53.662851 synth_machine-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       75 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/__init__.py
+-rw-r--r--   0        0        0     4278 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/config.py
+-rw-r--r--   0        0        0      454 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/cost.py
+-rw-r--r--   0        0        0      830 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/executor_factory.py
+-rw-r--r--   0        0        0      203 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/executors/__init__.py
+-rw-r--r--   0        0        0     4385 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/executors/anthropic.py
+-rw-r--r--   0        0        0      710 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/executors/base.py
+-rw-r--r--   0        0        0     3144 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/executors/lorem.py
+-rw-r--r--   0        0        0     3600 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/executors/openai.py
+-rw-r--r--   0        0        0     3765 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/executors/togetherai.py
+-rw-r--r--   0        0        0    23932 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/machine.py
+-rw-r--r--   0        0        0      973 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/machine_config.py
+-rw-r--r--   0        0        0     1853 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/runners.py
+-rw-r--r--   0        0        0     3085 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/safety.py
+-rw-r--r--   0        0        0     3511 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/synth_definition.py
+-rw-r--r--   0        0        0      198 2024-06-01 21:03:53.662851 synth_machine-0.3.0/synth_machine/tools.py
+-rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 synth_machine-0.3.0/PKG-INFO
```

### Comparing `synth_machine-0.2.0/LICENSE` & `synth_machine-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_machine-0.2.0/pyproject.toml` & `synth_machine-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "synth_machine"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = [
   "CTO <cto@hiresynth.ai>",
   "CEO <ceo@hiresynth.ai>",
   "COO <coo@hiresynth.ai>"
 ]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
-anthropic = "^0.25.1"
+anthropic = "^0.26.0"
 jinja2 = "^3.1.2"
 jq = "^1.6.0"
 jsonschema = "^4.19.2"
 object-store-python = "^0.1.10"
 opa-python-client = "^1.3.6"
 openai = "1.28.1"
 partial_json_parser = "*"
 pydantic = "^2.7.1"
 requests = "^2.31.0"
 tiktoken = "0.6.0"
 transitions = "^0.9.0"
 urllib3 = "*"
 
 [tool.poetry.group.dev.dependencies]
-commitizen = "^3.8.0"
+commitizen = "^3.26.0"
 coverage = "^7.5.1"
 deptry = "^0.16.1"
 pre-commit = "^3.6.2"
 pyright = "^1.1.326"
 pyyaml = "^6.0.1"
 ruff = "^0.4.3"
```

### Comparing `synth_machine-0.2.0/synth_machine/config.py` & `synth_machine-0.3.0/synth_machine/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 import logging
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import Optional, Tuple
-
 from jinja2 import Template, StrictUndefined
 
 from synth_machine.executor_factory import get_executor
 from synth_machine.executors.base import BaseExecutor
 from synth_machine.machine_config import ModelConfig
-
+from synth_machine.synth_definition import Output, Input
 import tiktoken
 
 enc = tiktoken.get_encoding("cl100k_base")
 
 
 @dataclass
 class SynthConfig:
     executor: BaseExecutor
     model_config: ModelConfig
     system_prompt: Optional[str]
     user_prompt: str
 
 
 async def tool_setup(
-    output_definition: dict, inputs: dict, id: str, owner: str, tools: list
+    output_definition: Output, inputs: dict, id: str, user: str, tools: list
 ) -> dict:
-    tool_search = [tool for tool in tools if tool.name == output_definition.get("tool")]
+    tool_search = [tool for tool in tools if tool.name == output_definition.tool]
     if not tool_search:
+        logging.warning(
+            f"Tool not found: '{output_definition.tool}'. Available tools: {[tool.name for tool in tools]}"
+        )
         return {}
     tool = tool_search[0]
-    tool_path = f"{tool.api_endpoint}{output_definition['route']}"
+    tool_path = f"{tool.api_endpoint}{output_definition.route}"
     output_mime_types = [
         response_mime
-        for response_mime in tool.api_spec["paths"][output_definition["route"]]["post"][
+        for response_mime in tool.api_spec["paths"][output_definition.route]["post"][
             "responses"
         ]["200"]["content"].keys()
         if response_mime != "application/json"
     ]
     # TODO: add back in validation using the api spec response schema.
 
     tool_payload = {
         key: (
             inputs[value]
             if value in inputs.keys()
             else Template(value, undefined=StrictUndefined).render(**inputs)
         )
-        for key, value in output_definition.get("input_name_map").items()  # type: ignore
+        for key, value in output_definition.input_name_map.items()  # type: ignore
     }
 
     if tool.token_multiplier != 0:
         raw_tokens = sum([len(enc.encode(value)) for value in tool_payload.values()])
         tokens_multiplied = raw_tokens * tool.token_multiplier
     else:
         tokens_multiplied = 0
 
     logging.debug(f"Tool payload: {tool_payload}")
     return {
-        "id": id,
         "tool_id": tool.id,  # type: ignore
-        "owner": owner,
+        "owner": user,
         "payload": tool_payload,
         "output_mime_types": output_mime_types,
         "tool_path": tool_path,
         "tokens": {
             "execution": tool.tokens_per_execution,
             "multiplier": tokens_multiplied,
         },
@@ -86,36 +87,43 @@
             logging.warning(f"Undefined variable in prompt: {e}")
             return ("", str(e))
         return (dedent(prompt).strip(), None)
     return ("", f"Prompt template not provided, got {prompt_template}")
 
 
 async def prompt_setup(
-    output_definition: dict, inputs: dict, default_model_config: dict
+    output_definition: Output, inputs: Input, default_model_config: dict
 ) -> Tuple[Optional[SynthConfig], Optional[str]]:
-    user_prompt_template = output_definition.get("prompt")
+    user_prompt_template = output_definition.prompt
     user_prompt, prompt_err = prompt_for_transition(
         inputs=inputs,
         prompt_template=user_prompt_template,
     )
     if prompt_err:
         return (None, prompt_err)
     logging.debug(f"""User PROMPT: <<<{user_prompt}>>>""")
 
-    system_prompt_template = output_definition.get("system_prompt", "")
-    system_prompt, system_err = prompt_for_transition(
-        inputs=inputs,
-        prompt_template=system_prompt_template,
-    )
-    if system_err:
-        return (None, system_err)
+    system_prompt_template = output_definition.system_prompt
+    if system_prompt_template:
+        system_prompt, system_err = prompt_for_transition(
+            inputs=inputs,
+            prompt_template=system_prompt_template,
+        )
+        if system_err:
+            return (None, system_err)
+    else:
+        system_prompt = None
     logging.debug(f"""System PROMPT: <<<{system_prompt}>>>""")
 
     model_config = ModelConfig(
-        **(default_model_config | output_definition.get("model_config", {}))
+        **(
+            default_model_config | output_definition.config.dict()
+            if output_definition.config
+            else default_model_config
+        )
     )
 
     logging.debug(f"Model config {model_config}")
     executor = get_executor(name=model_config.executor)
 
     return (
         SynthConfig(
```

### Comparing `synth_machine-0.2.0/synth_machine/executors/anthropic.py` & `synth_machine-0.3.0/synth_machine/executors/anthropic.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,22 @@
         self.enc = tiktoken.get_encoding("cl100k_base")
         self.client = anthropic.AsyncAnthropic(api_key=ANTHROPIC_API_KEY)  # type: ignore
 
     @staticmethod
     def post_process(output: dict) -> dict:
         return output
 
-    async def generate(  # type: ignore
+    async def generate(
         self,
         user_prompt: Optional[str],
         system_prompt: Optional[str],
         json_schema: Optional[dict],
         model_config: ModelConfig,
-        user: Optional[str],
-    ) -> AsyncGenerator[str, dict]:
+        user: str = "",
+    ) -> AsyncGenerator:
         messages = [{"role": "user", "content": user_prompt}]
         if model_config.assistant_partial != "":
             # Anthropic supports assistant prefilling instead of system prompt
             messages.append(
                 {"role": "assistant", "content": model_config.assistant_partial}
             )
 
@@ -68,15 +68,15 @@
                         "input_schema": json_schema,
                     }
                 ]
             else:
                 tools = model_config.tool_options
 
             tool_response = await self.client.beta.tools.messages.create(
-                model=model_config.model_name,
+                model=model_config.llm_name,
                 system=system_prompt,
                 max_tokens=model_config.max_tokens,
                 messages=messages,
                 tools=tools,
             )
             response_content = tool_response.content
 
@@ -95,15 +95,15 @@
                 {
                     "tokens": calculate_input_tokens(str(output), cot_response),
                     "token_type": "output",
                 },
             )  # type: ignore
         else:
             response = await self.client.messages.create(
-                model=model_config.model_name,
+                model=model_config.llm_name,
                 system=system_prompt,
                 messages=messages,  # type: ignore
                 max_tokens=model_config.max_tokens,
                 stream=True,
                 metadata={"user_id": user},
                 stop_sequences=model_config.stop,
             )  # type: ignore
```

### Comparing `synth_machine-0.2.0/synth_machine/executors/base.py` & `synth_machine-0.3.0/synth_machine/executors/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 
 class BaseExecutor:
     @staticmethod
     def post_process(output: dict) -> dict:
         raise NotImplementedError
 
-    async def generate(
+    def generate(
         self,
         user_prompt: Optional[str],
         system_prompt: Optional[str],
         json_schema: Optional[dict],
         model_config: ModelConfig,
-        user: Optional[str],
-    ) -> AsyncGenerator[str, dict]:
+        user: str = "",
+    ) -> AsyncGenerator:
         raise NotImplementedError
```

### Comparing `synth_machine-0.2.0/synth_machine/executors/openai.py` & `synth_machine-0.3.0/synth_machine/executors/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,22 @@
     def __init__(self) -> None:
         self.client = AsyncOpenAI(api_key=OPENAI_API_KEY)  # type: ignore
 
     @staticmethod
     def post_process(output: dict) -> dict:
         return output.get("output", {})
 
-    async def generate(  # type: ignore
+    async def generate(
         self,
         user_prompt: Optional[str],
         system_prompt: Optional[str],
         json_schema: Optional[dict],
         model_config: ModelConfig,
-        user: Optional[str],
-    ) -> AsyncGenerator[str, dict]:
+        user: str = "",
+    ) -> AsyncGenerator:
         # PyRight doesn't understand the openai library has been updated
         messages = (
             [
                 {"role": "system", "content": system_prompt},
             ]
             if system_prompt
             else []
@@ -61,26 +61,26 @@
                 )
             ]
             tool_choice = ChatCompletionNamedToolChoiceParam(
                 {"type": "function", "function": {"name": "output"}}
             )
 
             response = await self.client.chat.completions.create(
-                model=model_config.model_name,
+                model=model_config.llm_name,
                 messages=messages,  # type: ignore
                 temperature=model_config.temperature,
                 stream=True,
                 tools=tools,
                 max_tokens=model_config.max_tokens,
                 tool_choice=tool_choice,
                 user=user,
             )
         else:
             response = await self.client.chat.completions.create(
-                model=model_config.model_name,
+                model=model_config.llm_name,
                 messages=messages,  # type: ignore
                 temperature=model_config.temperature,
                 stream=True,
                 max_tokens=model_config.max_tokens,
                 user=user,
             )
```

### Comparing `synth_machine-0.2.0/synth_machine/executors/togetherai.py` & `synth_machine-0.3.0/synth_machine/executors/togetherai.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,22 +21,22 @@
             api_key=TOGETHER_API_KEY, base_url="https://api.together.xyz"
         )  # type: ignore
 
     @staticmethod
     def post_process(output: dict) -> dict:
         return output[0]["arguments"].get("output", {})
 
-    async def generate(  # type: ignore
+    async def generate(
         self,
         user_prompt: Optional[str],
         system_prompt: Optional[str],
         json_schema: Optional[dict],
         model_config: ModelConfig,
-        user: Optional[str],
-    ) -> AsyncGenerator[str, dict]:
+        user: str = "",
+    ) -> AsyncGenerator:
         # PyRight doesn't understand the openai library has been updated
         messages = (
             [
                 {"role": "system", "content": system_prompt},
             ]
             if system_prompt
             else []
@@ -44,15 +44,15 @@
         messages.append(
             {"role": "user", "content": str(user_prompt)},
         )
 
         if (
             json_schema
             and json_schema.get("type") != "string"
-            and model_config.model_name
+            and model_config.llm_name
             in [
                 "mistralai/Mixtral-8x7B-Instruct-v0.1",
                 "mistralai/Mistral-7B-Instruct-v0.1",
                 "togethercomputer/CodeLlama-34b-Instruct",
             ]
         ):
             tools = [
@@ -71,26 +71,26 @@
                 )
             ]
             tool_choice = ChatCompletionNamedToolChoiceParam(
                 {"type": "function", "function": {"name": "output"}}
             )
 
             response = await self.client.chat.completions.create(
-                model=model_config.model_name,
+                model=model_config.llm_name,
                 messages=messages,  # type: ignore
                 temperature=model_config.temperature,
                 stream=True,
                 tools=tools,
                 max_tokens=model_config.max_tokens,
                 tool_choice=tool_choice,
                 user=user,
             )
         else:
             response = await self.client.chat.completions.create(
-                model=model_config.model_name,
+                model=model_config.llm_name,
                 messages=messages,  # type: ignore
                 temperature=model_config.temperature,
                 stream=True,
                 max_tokens=model_config.max_tokens,
                 user=user,
             )
```

### Comparing `synth_machine-0.2.0/synth_machine/machine.py` & `synth_machine-0.3.0/synth_machine/machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import itertools
+import uuid
 from enum import StrEnum
 from json.decoder import JSONDecodeError
 from typing import List, Optional
 
 from jsonschema import validate  # type: ignore
 from jsonschema.exceptions import ValidationError  # type: ignore
 from object_store import ObjectStore
@@ -13,24 +14,33 @@
 
 from synth_machine.safety import Safety, SafetyInput, SAFETY_DEFAULTS
 from synth_machine.config import (
     prompt_setup,
     prompt_for_transition,
     tool_setup,
 )
-from synth_machine.runners import jq_runner, tool_runner
+from synth_machine.runners import (
+    jq_runner,
+    tool_runner,
+    STORAGE_PREFIX,
+    STORAGE_OPTIONS,
+)
 from synth_machine.cost import BaseCost
-
-from synth_machine import STORAGE_OPTIONS, STORAGE_PREFIX, TOOLS
+from synth_machine.tools import Tool
+from synth_machine.synth_definition import SynthDefinition, Output, Input, Transition
 
 
 class Model:
     pass
 
 
+class TransitionError(Exception):
+    pass
+
+
 class YieldTasks(StrEnum):
     CHUNK = "CHUNK"
     MODEL_CONFIG = "MODEL_CONFIG"
     SET_MEMORY = "SET_MEMORY"
     SET_ACTIVE_OUTPUT = "SET_ACTIVE_OUTPUT"
 
 
@@ -55,48 +65,44 @@
 
 
 class Synth(BaseCost):
     JSONSCHEMA_PRELUDE = {"$schema": "http://json-schema.org/draft-04/schema#"}
 
     def __init__(
         self,
-        session_id: int,
-        synth_id: int,
-        owner: int,
-        initial_state: str,
-        states: List[dict],
-        transitions: List[dict],
-        default_model_config: dict = {},
-        safety_thresholds: Optional[SafetyInput] = None,
+        config: dict,
         memory: dict = {},
+        safety_thresholds: Optional[SafetyInput] = None,
         store: ObjectStore = ObjectStore(STORAGE_PREFIX, STORAGE_OPTIONS),
-        tools: list = TOOLS,
+        user: str = str(uuid.uuid4()),
+        session_id: str = str(uuid.uuid4()),
+        tools: List[Tool] = [],
     ) -> None:
+        config = SynthDefinition(**config)
+        self.user = user
         self.session_id = session_id
-        self.synth_id = synth_id
-        self.owner = owner
-        self.raw_transitions = transitions
+        self.raw_transitions = config.transitions
         self.transitions = list(
             map(
                 lambda t: {
-                    "trigger": t["trigger"],
-                    "source": t["source"],
-                    "dest": t["dest"],
+                    "trigger": t.trigger,
+                    "source": t.source,
+                    "dest": t.dest,
                 },
-                transitions,
+                self.raw_transitions,
             )
         )
-        self.raw_states = states
-        self.state_names = list(map(lambda s: s["name"], self.raw_states))
-        self.memory: dict = memory
+        self.raw_states = config.states
+        self.state_names = list(map(lambda s: s.name, self.raw_states))
+        self.memory: dict = config.initial_memory | memory
         self._model = Model()
-        self.default_model_config = default_model_config
+        self.default_model_config = config.default_model_config
         self._machine = Machine(
             auto_transitions=False,
-            initial=initial_state,
+            initial=config.initial_state,
             model=self._model,
             states=self.state_names,
             transitions=self.transitions,
         )
         self.safety = Safety(
             thresholds=(safety_thresholds if safety_thresholds else SAFETY_DEFAULTS),
         )
@@ -105,77 +111,77 @@
         self.tools = tools
 
     def current_state(self) -> str:
         return self._model.state  # type: ignore
 
     def interfaces_for_available_triggers(
         self, state: Optional[str] = None
-    ) -> List[dict]:
+    ) -> List[Transition]:
         return [
             transition
             for transition in self.raw_transitions
-            if transition["trigger"]
+            if transition.trigger
             in self._machine.get_triggers(state or self.current_state())
         ]
 
     def get_raw_state(self, state: str):
-        return [s for s in self.raw_states if s["name"] == state][0]
+        return [s for s in self.raw_states if s.name == state][0]
 
     def machine_update(self, transition, set_active_trigger=False, state=None):
         return [
             "MACHINE_UPDATE",
-            self.interfaces_for_available_triggers(state=state or transition["dest"]),
+            self.interfaces_for_available_triggers(state=state or transition.dest),
             self.memory,
             self.current_state(),
-            transition["trigger"] if set_active_trigger else "",
+            transition.trigger if set_active_trigger else "",
         ]
 
-    async def post_process(self, output_key: str, output_definition: dict, chunk: str):
+    async def post_process(
+        self, output_key: str, output_definition: Output, chunk: str
+    ):
         new_buffer = f"{self.buffer.get(output_key, "")}{chunk}"
         if new_buffer != self.buffer.get(output_key, ""):
             self.buffer[output_key] = new_buffer
             try:
-                result = self.memory | loads(str(self.buffer[output_key]), OBJ).get(  # type: ignore
-                    "output", {}
-                )
+                result = self.memory | loads(str(self.buffer[output_key]), OBJ).output
             except Exception:
                 result = self.memory
         else:
             result = self.memory
         operation_list = [
             operation
             for operation in PostProcessTasks
-            if output_definition.get(operation)
+            if getattr(output_definition, operation, None)
         ]
         operation = operation_list[0] if operation_list else None
         match operation:
             case PostProcessTasks.JQ:
                 jq_result = jq_runner(
-                    output_definition.get(operation, ""),
+                    getattr(output_definition, operation),
                     result,
-                    output_definition.get("schema", {}),
+                    output_definition.schema_dict,
                 )
                 if jq_result:
                     self.memory[output_key] = jq_result
                     yield [PostProcessTasks.JQ, output_key, jq_result]
                 yield []
             case _:
                 yield []
 
     async def run_task(
         self,
-        inputs: dict,
-        transition: dict,
+        inputs: Input,
+        transition: Transition,
         output_key: str,
-        output_definition: dict,
+        output_definition: Output,
         retries: int = 3,
         loop: bool = False,
     ):
         yield [YieldTasks.SET_ACTIVE_OUTPUT, output_key]
-        schema: dict = output_definition.get("schema", {})
+        schema = output_definition.schema_dict
 
         # TODO: find a nicer way to ensure tests don't reference the finished memory object out of order
         yield [
             YieldTasks.SET_MEMORY,
             output_key,
             json.loads(json.dumps(self.memory.get(output_key, {}))),
         ]
@@ -183,33 +189,35 @@
         config = {}
         predicted = ""
         predicted_json = ""
 
         operation_list = [
             operation
             for operation in OperationPriority
-            if output_definition.get(operation)
+            if getattr(output_definition, operation, None)
         ]
         operation = operation_list[0] if operation_list else None
         logging.debug(f"operation: {operation}")
         match operation:
             case OperationPriority.JINJA:
-                template = prompt_for_transition(
-                    inputs=inputs, prompt_template=output_definition.get("template")
+                template, _ = prompt_for_transition(
+                    inputs=inputs, prompt_template=output_definition.jinja
                 )
                 self.memory[output_key] = template
                 yield [
                     YieldTasks.SET_MEMORY,
                     output_key,
                     json.loads(json.dumps(template)),
                 ]
             case OperationPriority.INTERLEAVE:
                 keys = [
                     self.memory.get(x)
-                    for x in output_definition.get(OperationPriority.INTERLEAVE, "")
+                    for x in getattr(
+                        output_definition, OperationPriority.INTERLEAVE, ""
+                    )
                     if self.memory.get(x)
                 ]
                 output = []
                 for zipped in itertools.zip_longest(*keys):  # type: ignore
                     temp = {}
                     for key in zipped:
                         if key is None:
@@ -227,34 +235,39 @@
                 ]
             case OperationPriority.TOOL:
                 config = await tool_setup(
                     tools=self.tools,
                     output_definition=output_definition,
                     inputs=inputs,
                     id=str(self.session_id),
-                    owner=str(self.owner),
-                )
-                predicted_json = await tool_runner(
-                    store=self.store,
-                    config=config,
-                    return_key=output_definition.get("return_key"),
+                    user=self.user,
                 )
+                logging.info(f"Tool config: {config}")
+                predicted_json = await tool_runner(store=self.store, config=config)
 
                 if not predicted_json:
                     yield [
                         FailureState.FAILED,
                         output_key,
                         f"Failed to call tool {config}",
                     ]
 
                 logging.debug(f"Tool output: {predicted_json}")
-                if isinstance(self.memory.get(output_key, {}), list):
+                if loop:
                     self.memory[output_key].append(predicted_json)
+                    logging.debug(
+                        f"➕ Tool Appended {output_key}:{self.memory[output_key]}"
+                    )
+
                 else:
                     self.memory[output_key] = predicted_json
+                    logging.debug(
+                        f"💾 Tool Saved {output_key}:{self.memory[output_key]}"
+                    )
+
                 token_cost = config["tokens"]["execution"]
                 token_usage = await self.calculate_tool_token_usage(config, token_cost)
                 yield [
                     "TOOL_OUTPUT",
                     output_key,
                     token_usage,
                     config.get("tool_id"),
@@ -264,16 +277,16 @@
                     output_key,
                     json.loads(json.dumps(predicted_json)),
                 ]
             case OperationPriority.PROMPT:
                 config, err = await prompt_setup(
                     output_definition=output_definition,
                     inputs=inputs,
-                    default_model_config=self.default_model_config
-                    | transition.get("model_config", {}),
+                    default_model_config=self.default_model_config.dict(by_alias=True)  # type: ignore
+                    | transition.model_config,
                 )
                 if err or not config:
                     logging.error(err)
                     yield [FailureState.FAILED, output_key, err]
                     return
 
                 prompt_safety = self.safety.check(
@@ -305,45 +318,46 @@
                 ]
                 while True:
                     executor = {"executor": config.model_config.executor}
                     yield [YieldTasks.MODEL_CONFIG, output_key, executor]
                     logging.debug(
                         f"🤖 Execution started ({config.model_config.executor})"
                     )
-                    llm_name = config.model_config.model_name
+                    llm_name = config.model_config.llm_name
                     tokens = {
                         "input": 0,
                         "output": 0,
                     }
                     async for token, token_info in config.executor.generate(
-                        config.user_prompt,
-                        config.system_prompt,
-                        schema,
-                        config.model_config,
-                        str(self.owner),
-                    ):  # type: ignore
+                        user_prompt=config.user_prompt,
+                        system_prompt=config.system_prompt,
+                        json_schema=schema,
+                        model_config=config.model_config,
+                        user=self.user,
+                    ):
                         predicted = f"{predicted}{str(token)}"
-                        stage = token_info["token_type"]
+                        stage = token_info.get("token_type", "output")
+                        tokens_used = token_info.get("tokens")
                         token_cost_per_chunk = self.calculate_chunk_cost(
-                            config, token_info["tokens"]
+                            config, tokens_used
                         )
                         tokens[stage] += token_cost_per_chunk
                         yield [
                             str(YieldTasks.CHUNK),
                             output_key,
                             token,
                             token_cost_per_chunk,
-                            token_info["tokens"],
+                            tokens_used,
                             stage,
                             llm_name,
                         ]
                     await self.calculate_prompt_token_usage(
                         llm_name,
-                        input_tokens=tokens["input"],
-                        output_tokens=tokens["output"],
+                        input_tokens=tokens.get("input", 0),
+                        output_tokens=tokens.get("output", 0),
                     )  # type: ignore
                     logging.debug("🤖 Execution complete")
 
                     response_safety = self.safety.check(
                         text=predicted, provider=config.model_config.executor
                     )
                     if response_safety is None:
@@ -368,24 +382,24 @@
                     yield [
                         "SAFETY",
                         "SUCCESS",
                         "RESPONSE",
                         json.dumps(response_safety),
                     ]
 
-                    if schema.get("type") == "string":
+                    if schema and schema.get("type") == "string":
                         predicted_json = predicted
                     else:
                         try:
                             predicted_json = config.executor.post_process(
                                 json.loads(predicted.strip())
                             )  # type: ignore
                             validate(
                                 instance=predicted_json,
-                                schema=self.JSONSCHEMA_PRELUDE | schema,
+                                schema=self.JSONSCHEMA_PRELUDE | schema,  # type: ignore
                             )
 
                         except (
                             ValidationError,
                             JSONDecodeError,
                         ) as e:
                             logging.error(f"❌ Failed validation with {e}")
@@ -395,34 +409,34 @@
                                 predicted_json = ""
                                 retries -= 1
                                 continue
                             yield [
                                 FailureState.OUTPUT_VALIDATION_FAILED,
                                 output_key,
                             ]
-                            self._model.state = transition["source"]  # type: ignore
+                            self._model.state = transition.source  # type: ignore
                             return
                     logging.debug("✅ Validated")
                     yield [
                         "OUTPUT_VALIDATION_SUCCEEDED",
                         output_key,
                     ]
                     if loop:
                         self.memory[output_key].append(predicted_json)
                         logging.debug(
-                            f"➕ Appended {output_key}:{self.memory[output_key]}"
+                            f"➕ LLM Appended {output_key}:{self.memory[output_key]}"
                         )
                     else:
                         self.memory[output_key] = predicted_json
                         logging.debug(
-                            f"💾 Saved {output_key}:{self.memory[output_key]}"
+                            f"💾 LLM Saved {output_key}:{self.memory[output_key]}"
                         )
                     return
             case OperationPriority.APPEND:
-                memory_keys = output_definition.get(operation, [])
+                memory_keys = getattr(output_definition, operation, [])
 
                 if self.memory.get(output_key) is None:
                     self.memory[output_key] = []
                 for memory_key in memory_keys:
                     item = self.memory.get(memory_key)
                     if item is not None:
                         self.memory[output_key].append(item)
@@ -477,29 +491,29 @@
         transition = self._transition_for_trigger(initial_trigger)
         # State-level loop, facilitates 'after' on transition
         while True:
             # Show interface for the *next* state
             yield self.machine_update(transition=transition, set_active_trigger=True)
 
             post_process_tasks = [
-                (output_definition.get("key"), output_definition)
-                for output_definition in transition.get("outputs", [])
+                (output_definition.key, output_definition)
+                for output_definition in transition.outputs
                 for post_processing_task in PostProcessTasks
-                if output_definition.get(post_processing_task)
+                if getattr(output_definition, post_processing_task, None)
             ]
-            for output_definition in transition.get("outputs", []):
-                output_key = output_definition.get("key")
+            for output_definition in transition.outputs:
+                output_key = output_definition.key
                 inputs = {
-                    input_item.get("key"): self.memory.get(input_item.get("key"))
-                    for input_item in transition.get("inputs", [])
+                    input_item.key: self.memory.get(input_item.key)
+                    for input_item in transition.inputs
                 }
-                loop = output_definition.get("loop")
+                loop = output_definition.loop
                 if loop is not None:
                     self.memory[output_key] = []
-                    for matrix in loop.get("matrix", []):
+                    for matrix in loop.matrix:
                         for loop_var, memory_key_looped in matrix.items():
                             if isinstance(memory_key_looped, list):
                                 loop = memory_key_looped
                             else:
                                 loop = self.memory.get(memory_key_looped, [])
                             for item in loop:
                                 loop_inputs = {
@@ -547,18 +561,18 @@
                         output_definition=post_process_definition,
                         chunk="",
                     )
                     if post_process:
                         async for post_process_event in post_process:
                             yield post_process_event
 
-            self._model.trigger(transition["trigger"])  # type: ignore
-            yield ["TRANSITION_COMPLETED", transition["trigger"]]
+            self._model.trigger(transition.trigger)  # type: ignore
+            yield ["TRANSITION_COMPLETED", transition.trigger]
 
-            if after := transition.get("after"):
+            if after := transition.after:
                 if "memory_key:" in after:
                     memory_key = after.split(":")[1]
                     if self.memory.get(memory_key):
                         transition = self._transition_for_trigger(
                             self.memory[memory_key]
                         )
                     else:
@@ -569,16 +583,37 @@
                 break
         yield self.machine_update(transition=transition)
 
     def _transition_for_trigger(self, trigger: str):
         return [
             transition
             for transition in self.raw_transitions
-            if transition["trigger"] == trigger
+            if transition.trigger == trigger
         ][0]
 
     async def streaming_trigger(self, trigger: str, params: Optional[dict] = None):
         if params is not None and len(params) > 0:
             self.memory = self.memory | params
 
         async for event in self.execute_for_trigger(initial_trigger=trigger):  # type: ignore
             yield event
+
+    async def trigger(self, trigger: str, inputs: dict = {}):
+        filtered_transition = list(
+            filter(
+                lambda transition: transition.trigger == trigger,
+                self.interfaces_for_available_triggers(),
+            )
+        )
+        if not len(filtered_transition):
+            raise TransitionError(
+                f"No transition: {trigger} exists at state: {self.current_state()}"
+            )
+
+        transition_outputs = [val.key for val in filtered_transition[0].outputs]  # type: ignore
+
+        async for value in self.streaming_trigger(trigger, params=inputs):
+            logging.debug(value)
+            if value[0] == FailureState.FAILED:
+                logging.error(f"Failure: {value}")
+
+        return {output: self.memory[output] for output in transition_outputs}
```

### Comparing `synth_machine-0.2.0/synth_machine/machine_config.py` & `synth_machine-0.3.0/synth_machine/machine_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from typing import List, Optional
 import tiktoken
 
 
 class ModelConfig(BaseModel):
     executor: str = "togetherai"
-    model_name: str = "mistralai/Mixtral-8x7B-Instruct-v0.1"
+    llm_name: str = Field(
+        alias="model_name", default="mistralai/Mixtral-8x7B-Instruct-v0.1"
+    )
     max_tokens: int = 1024
     temperature: float = 0.8
     assistant_partial: str = ""
     partial_input: Optional[str] = None
     stop: List[str] = []
     tool_use: bool = False
     tool_options: Optional[List[dict]] = None
```

### Comparing `synth_machine-0.2.0/synth_machine/runners.py` & `synth_machine-0.3.0/synth_machine/runners.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,49 +2,60 @@
 from io import BytesIO
 from typing import Optional
 from uuid import uuid4
 
 import jq
 import requests  # type: ignore
 from object_store import ObjectStore
+import json
+import os
 
-from synth_machine import STORAGE_PREFIX
 
+STORAGE_OPTIONS = json.loads(os.environ.get("STORAGE_OPTIONS", "{}"))
+STORAGE_PREFIX = os.environ.get("STORAGE_PREFIX", "memory://")
 
-async def tool_runner(
-    store: ObjectStore, config: dict, return_key: Optional[str]
-) -> Optional[dict | str]:
+
+async def tool_runner(store: ObjectStore, config: dict) -> Optional[dict | str]:
     try:
         response = requests.post(
             config["tool_path"],
             json=config["payload"],
         )
+        response_headers = {
+            "response_headers": {
+                "status": response.status_code,
+                "success": response.ok,
+            }
+        }
     except Exception as e:
-        logging.warn(f"Error in running tool {e}")
-        return None
+        logging.error(f"Error in running tool {e}")
+        return
 
     if config["output_mime_types"]:
         output_format = response.headers["content-type"].split("/")[1]
         file_name = f"{uuid4()}.{output_format}"
         store.put(file_name, BytesIO(response.content))
         return {
             "file_name": file_name,
             "mime_type": output_format,
             "url": f"{STORAGE_PREFIX}/{file_name}",
+            "response_headers": response_headers["response_headers"],
         }
     else:
-        output = response.json()
-        return output if not return_key else output[return_key]
+        output = response.json() | response_headers
+        return output
 
 
-def jq_runner(jq_command: str, data: dict = {}, schema: dict = {}) -> list:
+def jq_runner(jq_command: str, data: dict = {}, schema: Optional[dict] = {}) -> list:
     if not jq_command:
         return []
     try:
         intermediate_result = jq.compile(jq_command).input_value(data)
-        if schema.get("type") == "object" or schema.get("type") == "string":
+        if schema and (
+            schema.get("type") == "object" or schema.get("type") == "string"
+        ):
             return intermediate_result.first()
         else:
             return intermediate_result.all()
     except Exception as e:
         logging.warn(f"Error in post processing task {e}")
         return []
```

### Comparing `synth_machine-0.2.0/synth_machine/safety.py` & `synth_machine-0.3.0/synth_machine/safety.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 from enum import Enum
 from typing import TypedDict
 
 from openai import OpenAI, RateLimitError
 from opa_client.opa import OpaClient
 from urllib3.exceptions import LocationValueError, MaxRetryError
-from synth_machine import SAFETY_URL
+import os
 
+SAFETY_URL = os.environ.get("SAFETY_URL")
 if SAFETY_URL:
     opa_client = OpaClient(host=SAFETY_URL, port=8181)
 
 
 class Threshold(Enum):
     high = "high"
     moderate = "moderate"
```

### Comparing `synth_machine-0.2.0/PKG-INFO` & `synth_machine-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: synth_machine
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: GPL-3.0-or-later
 Author: CTO
 Author-email: cto@hiresynth.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anthropic (>=0.25.1,<0.26.0)
+Requires-Dist: anthropic (>=0.26.0,<0.27.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jq (>=1.6.0,<2.0.0)
 Requires-Dist: jsonschema (>=4.19.2,<5.0.0)
 Requires-Dist: object-store-python (>=0.1.10,<0.2.0)
 Requires-Dist: opa-python-client (>=1.3.6,<2.0.0)
 Requires-Dist: openai (==1.28.1)
 Requires-Dist: partial_json_parser
```

