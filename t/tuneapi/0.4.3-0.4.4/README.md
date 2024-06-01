# Comparing `tmp/tuneapi-0.4.3.tar.gz` & `tmp/tuneapi-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.4.3.tar", max compression
+gzip compressed data, was "tuneapi-0.4.4.tar", max compression
```

## Comparing `tuneapi-0.4.3.tar` & `tuneapi-0.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.4.3/LICENSE
--rw-r--r--   0        0        0      184 2024-05-13 05:27:01.434096 tuneapi-0.4.3/README.md
--rw-r--r--   0        0        0      770 2024-05-30 12:40:20.107474 tuneapi-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       78 2024-05-30 12:39:50.633839 tuneapi-0.4.3/tuneapi/__init__.py
--rw-r--r--   0        0        0      351 2024-05-21 04:32:29.030680 tuneapi-0.4.3/tuneapi/__main__.py
--rw-r--r--   0        0        0     6012 2024-05-21 06:57:23.060317 tuneapi-0.4.3/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     8812 2024-05-30 12:03:04.615930 tuneapi-0.4.3/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     8131 2024-05-23 12:07:04.181995 tuneapi-0.4.3/tuneapi/apis/model_gemini.py
--rw-r--r--   0        0        0     5897 2024-05-30 06:57:07.159092 tuneapi-0.4.3/tuneapi/apis/model_groq.py
--rw-r--r--   0        0        0     6065 2024-05-30 06:57:07.179854 tuneapi-0.4.3/tuneapi/apis/model_mistral.py
--rw-r--r--   0        0        0     7750 2024-05-30 09:57:47.403200 tuneapi-0.4.3/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     6479 2024-05-30 10:03:03.860013 tuneapi-0.4.3/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0     5393 2024-05-24 03:47:21.853954 tuneapi-0.4.3/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      220 2024-05-23 09:12:22.307150 tuneapi-0.4.3/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    18250 2024-05-30 07:03:24.320899 tuneapi-0.4.3/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1247 2024-05-21 04:49:29.146672 tuneapi-0.4.3/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0     9846 2024-05-21 05:00:43.950665 tuneapi-0.4.3/tuneapi/utils/code.py
--rw-r--r--   0        0        0      345 2024-05-12 08:34:03.731467 tuneapi-0.4.3/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2987 2024-05-12 08:34:17.889266 tuneapi-0.4.3/tuneapi/utils/fs.py
--rw-r--r--   0        0        0     1024 2024-05-13 05:28:35.812363 tuneapi-0.4.3/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33527 2024-05-12 08:34:20.152416 tuneapi-0.4.3/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3778 2024-05-12 08:34:28.068601 tuneapi-0.4.3/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2131 2024-05-12 08:34:30.772098 tuneapi-0.4.3/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4883 2024-05-12 08:34:35.753162 tuneapi-0.4.3/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0     1220 2024-05-12 08:34:38.734730 tuneapi-0.4.3/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     2496 2024-05-12 08:34:41.922150 tuneapi-0.4.3/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5838 2024-05-12 08:34:44.657582 tuneapi-0.4.3/tuneapi/utils/subway.py
--rw-r--r--   0        0        0     1430 2024-05-13 05:28:59.510065 tuneapi-0.4.3/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 tuneapi-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.4.4/LICENSE
+-rw-r--r--   0        0        0      184 2024-05-13 05:27:01.434096 tuneapi-0.4.4/README.md
+-rw-r--r--   0        0        0      787 2024-06-01 16:21:28.115393 tuneapi-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-06-01 16:20:52.321722 tuneapi-0.4.4/tuneapi/__init__.py
+-rw-r--r--   0        0        0      351 2024-06-01 14:39:34.984592 tuneapi-0.4.4/tuneapi/__main__.py
+-rw-r--r--   0        0        0     6012 2024-05-21 06:57:23.060317 tuneapi-0.4.4/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     8812 2024-06-01 09:26:15.931242 tuneapi-0.4.4/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     8131 2024-05-23 12:07:04.181995 tuneapi-0.4.4/tuneapi/apis/model_gemini.py
+-rw-r--r--   0        0        0     5897 2024-05-30 06:57:07.159092 tuneapi-0.4.4/tuneapi/apis/model_groq.py
+-rw-r--r--   0        0        0     6065 2024-05-30 06:57:07.179854 tuneapi-0.4.4/tuneapi/apis/model_mistral.py
+-rw-r--r--   0        0        0     7750 2024-05-30 09:57:47.403200 tuneapi-0.4.4/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     6479 2024-05-30 10:03:03.860013 tuneapi-0.4.4/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0     5393 2024-05-24 03:47:21.853954 tuneapi-0.4.4/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      236 2024-06-01 14:37:34.211853 tuneapi-0.4.4/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    26878 2024-06-01 16:19:58.032422 tuneapi-0.4.4/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1247 2024-05-21 04:49:29.146672 tuneapi-0.4.4/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0     9846 2024-05-21 05:00:43.950665 tuneapi-0.4.4/tuneapi/utils/code.py
+-rw-r--r--   0        0        0      345 2024-05-12 08:34:03.731467 tuneapi-0.4.4/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2987 2024-05-12 08:34:17.889266 tuneapi-0.4.4/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0     1024 2024-05-13 05:28:35.812363 tuneapi-0.4.4/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33527 2024-05-12 08:34:20.152416 tuneapi-0.4.4/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3778 2024-05-12 08:34:28.068601 tuneapi-0.4.4/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2131 2024-05-12 08:34:30.772098 tuneapi-0.4.4/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4883 2024-05-12 08:34:35.753162 tuneapi-0.4.4/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0     1326 2024-06-01 14:07:45.554825 tuneapi-0.4.4/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2496 2024-05-12 08:34:41.922150 tuneapi-0.4.4/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5838 2024-05-12 08:34:44.657582 tuneapi-0.4.4/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0     1430 2024-05-13 05:28:59.510065 tuneapi-0.4.4/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tuneapi-0.4.4/PKG-INFO
```

### Comparing `tuneapi-0.4.3/LICENSE` & `tuneapi-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/pyproject.toml` & `tuneapi-0.4.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.4.3"
+version = "0.4.4"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
@@ -12,14 +12,15 @@
 fire = "0.5.0"
 requests = "^2.31.0"
 cloudpickle = "3.0.0"
 protobuf = "^4.25.3"
 cryptography = ">=42.0.5"
 tqdm = "^4.66.1"
 snowflake_id = "1.0.2"
+nutree = "0.8.0"
 boto3 = { version = "1.29.6", optional = true }
 
 [tool.poetry.extras]
 boto3 = ["boto3"]
 
 [tool.poetry.scripts]
 tuneapi = "tuneapi.__main__:main"
```

### Comparing `tuneapi-0.4.3/tuneapi/apis/__init__.py` & `tuneapi-0.4.4/tuneapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/apis/model_anthropic.py` & `tuneapi-0.4.4/tuneapi/apis/model_anthropic.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/apis/model_gemini.py` & `tuneapi-0.4.4/tuneapi/apis/model_gemini.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/apis/model_groq.py` & `tuneapi-0.4.4/tuneapi/apis/model_groq.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/apis/model_mistral.py` & `tuneapi-0.4.4/tuneapi/apis/model_mistral.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/apis/model_openai.py` & `tuneapi-0.4.4/tuneapi/apis/model_openai.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/apis/model_tune.py` & `tuneapi-0.4.4/tuneapi/apis/model_tune.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/apis/threads.py` & `tuneapi-0.4.4/tuneapi/apis/threads.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/types/chats.py` & `tuneapi-0.4.4/tuneapi/types/chats.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright © 2023- Frello Technology Private Limited
 
+import io
 import os
 import json
+import copy
 import random
 from functools import partial
 from collections.abc import Iterable
 from typing import Dict, List, Any, Tuple, Optional, Generator, Union
+import nutree as nt
 
 import tuneapi.utils as tu
-from tuneapi.utils import to_json, get_random_string, logger, from_json
 
 
 class Tool:
 
     class Prop:
         def __init__(
             self,
@@ -26,14 +28,17 @@
             self.name = name
             self.description = description
             self.required = required
             self.type = type
             self.items = items
             self.enum = enum
 
+        def __repr__(self) -> str:
+            return f"<Tool.Prop: " + ("*" if self.required else "") + f"{self.name}>"
+
     def __init__(
         self,
         name: str,
         description: str,
         parameters: List["Tool.Prop"],
     ):
         self.name = name
@@ -83,15 +88,14 @@
 class Message:
     # names that are our standards roles
     SYSTEM = "system"
     HUMAN = "human"
     GPT = "gpt"
     FUNCTION_CALL = "function_call"
     FUNCTION_RESP = "function_resp"
-    TOOLS = "tools"
 
     # mapping from known roles to our standard roles
     KNOWN_ROLES = {
         # system
         "system": SYSTEM,
         "sys": SYSTEM,
         # user
@@ -110,41 +114,51 @@
 
     # start initialization here
     def __init__(
         self,
         value: str | float | List[Dict[str, Any]],
         role: str,
         id: str = None,
+        fn_pairs: Optional[Tuple["Message", "Message"]] = None,
         **kwargs,
     ):
         if role not in self.KNOWN_ROLES:
             raise ValueError(f"Unknown role: {role}. Update dictionary `KNOWN_ROLES`")
         if value is None:
             raise ValueError("value cannot be None")
 
         self.role = self.KNOWN_ROLES[role]
         self.value = value
-        self.id = id or tu.get_snowflake()
+        self.id = id or "msg_" + str(tu.get_snowflake())
         self.metadata = kwargs
+        self.fn_pairs = fn_pairs
 
     def __str__(self) -> str:
         try:
             idx = max(os.get_terminal_size().columns - len(self.role) - 40, 10)
         except OSError:
             idx = 50
         return f"<{self.role}: {json.dumps(self.value)[:idx]}>"
 
-    def __radd__(self, other):
+    def __radd__(self, other: str):
         return Message(self.value + other, self.role)
 
-    def __add__(self, other):
+    def __add__(self, other: str):
         return Message(self.value + other, self.role)
 
     def __repr__(self) -> str:
-        return str(self.value)
+        out = ""
+        if self.fn_pairs:
+            for fc, fr in self.fn_pairs:
+                out += f"[[FC] {fc} => [FR] {fr}]"
+        if out:
+            out += " " + str(self.value)
+        else:
+            out = str(self.value)
+        return out
 
     def __getitem__(self, x):
         if x == "content":
             return self.value
         return getattr(self, x)
 
     def to_dict(
@@ -192,14 +206,15 @@
         return chat_message
 
     @classmethod
     def from_dict(cls, data):
         return cls(
             value=data.get("value") or data.get("content"),
             role=data.get("from") or data.get("role"),
+            id=data.get("id"),
             **data.get("metadata", {}),
         )  # type: ignore
 
 
 ### Aliases
 human = partial(Message, role=Message.HUMAN)
 system = partial(Message, role=Message.SYSTEM)
@@ -226,15 +241,15 @@
         title: str = "",
         tools: List[Tool] = [],
         **kwargs,
     ):
         self.chats = list(chats)
         self.jl = jl
         self.model = model
-        self.id = id
+        self.id = id or "thread_" + str(tu.get_snowflake())
         self.title = title
         self.tools = tools
 
         #
         kwargs = {k: v for k, v in sorted(kwargs.items())}
         self.meta = kwargs
         self.keys = list(kwargs.keys())
@@ -302,15 +317,15 @@
         )
 
     def to_ft(
         self, id: Any = None, drop_last: bool = False
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         chats = self.chats if not drop_last else self.chats[:-1]
         ft_dict = {
-            "id": id or get_random_string(6),
+            "id": id or tu.get_random_string(6),
             "conversations": [x.to_dict(format="ft") for x in chats],
         }
         if drop_last:
             ft_dict["last"] = self.chats[-1].to_dict(format="ft")
         return ft_dict, self.meta
 
     # modifications
@@ -327,25 +342,249 @@
     def add(self, message: Message):
         self.chats.append(message)
 
     def append(self, message: Message):
         self.chats.append(message)
 
 
-class ThreadTree:
-    """This is the tree representation of a thread, where each leaf is a Message object."""
+class TreeThread:
+    """
+    This is the tree representation of a thread, where each node is a Message object. Useful for regeneration and
+    searching through a tree of conversations. This is a container providing all the necessary APIs.
+    """
 
     def __init__(
+        self, *msgs: Union[List[Union[List, Message]], Message], id: str = None
+    ):
+        system = ""
+        if (
+            len(msgs)
+            and isinstance(msgs[0], Message)
+            and msgs[0].role == Message.SYSTEM
+        ):
+            system = msgs[0].value
+        if system:
+            msgs = msgs[1:]
+
+        self.id = id or "tree_" + str(tu.get_snowflake())
+        self.system = system
+        self.msg_counter = 0  # monotonically increasing counter
+        self.messages_map = {}
+        self.messages = {}
+
+        self.tree = nt.Tree(name=self.id)
+        if msgs:
+            self._add_children_to_parent(self.tree, msgs)
+
+    def __repr__(self) -> str:
+        if self.system and " <system>" not in self.tree.name:
+            self.tree.name += " <system>"
+        elif not self.system and self.tree.name.endswith(" <system>"):
+            self.tree.name = self.tree.name[:-9]
+        return self.tree.format()
+
+    def __getitem__(self, x) -> Message:
+        try:
+            if type(x) == int:
+                return self.messages[self.messages_map[x]]
+            elif type(x) == str:
+                return self.messages[x]
+            elif isinstance(x, Message):
+                return self.messages[x.id]
+            elif isinstance(x, nt.Node):
+                return self.messages[x.data_id]
+        except KeyError:
+            raise ValueError(f"Message with id '{x}' not found")
+        raise ValueError(f"Unknown type: {type(x)}")
+
+    def _get_parent_message(self, message: Message) -> Message:
+        if not isinstance(message, Message):
+            message = self[message]
+        parent_node = self.tree.find(data_id=message.id).parent
+        return self.messages[parent_node.data_id]
+
+    def _get_parent_node(self, message: Message) -> nt.Node:
+        message = self._get_parent_message(message)
+        return self.tree.find(data_id=message.id).parent
+
+    def _add_children_to_parent(
         self,
-        message: Message,
-        parent_message: Message,
+        parent_node: Union[nt.Tree, nt.Node],
+        children: List[Union[List, Message]],
+    ) -> None:
+        for child in children:
+            if isinstance(child, Message):
+                if not isinstance(parent_node, nt.Tree):
+                    lm = self.messages[parent_node.data_id]
+                    if lm.role == child.role:
+                        raise ValueError(
+                            f"Same consecutive roles: {self.latest_message.role} -> {child.role}"
+                        )
+
+                parent_node = parent_node.add(
+                    f"[{self.msg_counter:02d}] " + str(child),
+                    data_id=child.id,
+                )
+                self.messages_map[self.msg_counter] = child.id
+                self.messages[child.id] = child
+                self.msg_counter += 1
+            if isinstance(child, list):
+                # if this is a list then there are two possibilities:
+                # - regeneration: all items are assistant type
+                # - reprompt: all items are human type
+                self._add_children_to_parent(parent_node, child)
+
+    @property
+    def latest_node(self) -> nt.Node:
+        done = False
+        cntr = copy.deepcopy(self.msg_counter)
+        while not done:
+            try:
+                return self.tree.find(data_id=self.messages_map[cntr - 1])
+            except KeyError:
+                cntr -= 1
+                if cntr == 0:
+                    done = True
+        raise ValueError("No latest node found")
+
+    @property
+    def latest_message(self) -> Message:
+        return self.messages[self.latest_node.data_id]
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            "id": self.id,
+            "system": self.system,
+            "messages": [x.to_dict(format="full") for x in self.messages.values()],
+            "tree": self.tree.to_dict_list(),
+            "messages_map": self.messages_map,
+        }
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]) -> "TreeThread":
+        tree = cls()
+        tree.id = data["id"]
+        tree.system = data["system"]
+        tree.tree = nt.Tree.from_dict(data["tree"])
+        messages = [Message.from_dict(x) for x in data["messages"]]
+        tree.messages = {x.id: x for x in messages}
+        tree.messages_map = data["messages_map"]
+        tree.msg_counter = len(tree.messages) + 1
+        return tree
+
+    def add(self, child: Message, to: Message = None) -> "TreeThread":
+        if child.id in self.messages:
+            raise ValueError(
+                f"Message with id '{child.id}' already exists. Cycle detected."
+            )
+        if to is None:
+            # find the latest inserted message and just add this as a child
+            to = self.latest_message
+        to = self[to]
+        if to.id not in self.messages:
+            raise ValueError(f"Parent with id {to.id} not found. Insert parent first.")
+
+        self._add_children_to_parent(
+            self.tree.find(data_id=to.id),  # find the actual nutree.Node
+            [child],
+        )
+        return self
+
+    def delete(self, from_: Message) -> "TreeThread":
+        from_ = self[from_]
+        if from_.id not in self.messages:
+            raise ValueError(
+                f"Parent with id {from_.id} not found. Insert parent first."
+            )
+        from_node = self.tree.find(data_id=from_.id)
+
+        messages_map_inv = {v: k for k, v in self.messages_map.items()}
+
+        def _cleanup(node, _):
+            del self.messages[node.data_id]
+            del self.messages_map[messages_map_inv[node.data_id]]
+
+        if from_node.children:
+            from_node.visit(_cleanup, add_self=True)
+        else:
+            del self.messages[from_node.data_id]
+            del self.messages_map[messages_map_inv[from_node.data_id]]
+        from_node.remove(keep_children=False)
+        return self
+
+    def undo(self) -> "TreeThread":
+        return self.delete(self.latest_message)
+
+    def regenerate_stream(
+        self,
+        from_: Message,
+        api: object,
+        prompt: str = None,
+        dry: bool = False,
+        **api_kwargs,
+    ):
+        # validation on inputs for regeneration
+        from_ = self[from_]
+
+        if from_.role == Message.HUMAN:
+            # if we are regenerating for a human, then we need to add a prompt to the tree and then regenerate
+            if not prompt:
+                raise ValueError(
+                    f"Regenerating for role 'human' but no `prompt` provided. pass `prompt`"
+                )
+            if type(prompt) == str:
+                prompt = human(prompt)
+            self.add(prompt, to=self._get_parent_message(from_))
+            thread = Thread()
+            for x in self.tree.find(data_id=prompt.id).get_parent_list():
+                thread.append(self.messages[x.data_id])
+            thread.append(prompt)
+        else:
+            # if regenerating AI response then we just need to get till the parent message because that is guaranteed
+            # to be a human
+            if prompt:
+                raise ValueError(
+                    f"Regenerating for role 'gpt' but `prompt` provided. remove `prompt`"
+                )
+            thread = Thread()
+            for x in self.tree.find(data_id=from_.id).get_parent_list():
+                thread.append(self.messages[x.data_id])
+
+        if dry:
+            stream = (x + " " for x in "... I have been generated ...".split())
+        else:
+            stream = api.stream_chat(thread, **api_kwargs)
+
+        full_str = ""
+        for token in stream:
+            yield token
+            if isinstance(token, dict):
+                raise ValueError("Function call occured, not sure what to do")
+            full_str += token
+        self.add(assistant(full_str), to=thread.chats[-1])
+
+    def regenerate(
+        self,
+        from_: Message,
+        api: object,
+        prompt: str = None,
+        dry: bool = False,
+        **api_kwargs,
     ):
-        self.children = []
-        self.parent_id = parent_message.id or tu.get_snowflake()
-        self.id = message.id or tu.get_snowflake()
+        return "".join(
+            list(
+                self.regenerate_stream(
+                    from_,
+                    api,
+                    prompt=prompt,
+                    dry=dry,
+                    **api_kwargs,
+                )
+            )
+        )
 
 
 # these are the classes that we use for tune datasets from r-stack
 
 
 class ThreadsList(list):
     """This class implements some basic container methods for a list of Chat objects"""
@@ -473,27 +712,27 @@
         bench_dataset = cls()
         for item in data["items"]:
             bench_dataset.append(Thread.from_dict(item))
         return bench_dataset
 
     def to_disk(self, folder: str, fmt: Optional[str] = None):
         if fmt:
-            logger.warn(
+            tu.logger.warn(
                 f"exporting to {fmt} format, you cannot recreate the dataset from this."
             )
         os.makedirs(folder)
         with open(f"{folder}/tuneds.jsonl", "w") as f:
             for sample in self.items:
                 if fmt == "sharegpt":
                     item, _ = sample.to_ft()
                 elif fmt is None:
                     item = sample.to_dict()
                 else:
                     raise ValueError(f"Unknown format: {fmt}")
-                f.write(to_json(item, tight=True) + "\n")  # type: ignore
+                f.write(tu.to_json(item, tight=True) + "\n")  # type: ignore
 
     @classmethod
     def from_disk(cls, folder: str):
         bench_dataset = cls()
         with open(f"{folder}/tuneds.jsonl", "r") as f:
             for line in f:
                 item = json.loads(line)
@@ -555,26 +794,26 @@
     def to_disk(self, folder: str, fmt: Optional[str] = None):
         config = {}
         config["type"] = "tune"
         config["hf_type"] = fmt
         os.makedirs(folder)
         self.train_ds.to_disk(f"{folder}/train", fmt=fmt)
         self.eval_ds.to_disk(f"{folder}/eval", fmt=fmt)
-        to_json(config, fp=f"{folder}/tune_config.json", tight=True)
+        tu.to_json(config, fp=f"{folder}/tune_config.json", tight=True)
 
     @classmethod
     def from_disk(cls, folder: str):
         if not os.path.exists(folder):
             raise ValueError(f"Folder '{folder}' does not exist")
         if not os.path.exists(f"{folder}/train"):
             raise ValueError(f"Folder '{folder}/train' does not exist")
         if not os.path.exists(f"{folder}/eval"):
             raise ValueError(f"Folder '{folder}/eval' does not exist")
         if not os.path.exists(f"{folder}/tune_config.json"):
             raise ValueError(f"File '{folder}/tune_config.json' does not exist")
 
         # not sure what to do with these
-        config = from_json(f"{folder}/tune_config.json")
+        config = tu.from_json(f"{folder}/tune_config.json")
         return cls(
             train=ThreadsList.from_disk(f"{folder}/train"),
             eval=ThreadsList.from_disk(f"{folder}/eval"),
         )
```

### Comparing `tuneapi-0.4.3/tuneapi/utils/__init__.py` & `tuneapi-0.4.4/tuneapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/code.py` & `tuneapi-0.4.4/tuneapi/utils/code.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/fs.py` & `tuneapi-0.4.4/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/logger.py` & `tuneapi-0.4.4/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/mime.py` & `tuneapi-0.4.4/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/misc.py` & `tuneapi-0.4.4/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/networking.py` & `tuneapi-0.4.4/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/parallel.py` & `tuneapi-0.4.4/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/randomness.py` & `tuneapi-0.4.4/tuneapi/utils/randomness.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,13 +24,16 @@
         if instance is None:
             # largest value of instance has to be <1024, so we randomly create one when initialising ie. < `0x400`
             instance = "0x3" + "".join(random.choices("0123456789abcedf", k=2))
             instance = int(instance, 16)
         self.gen = SnowflakeGenerator(instance, epoch=epoch)
         self.lock = Lock()
 
-    def __call__(self) -> int:
+    def __call__(self, as_int=False) -> int:
         with self.lock:
-            return next(self.gen)
+            if as_int:
+                return next(self.gen)
+            else:
+                return f"{next(self.gen):17d}"
 
 
 get_snowflake = SFGen()
```

### Comparing `tuneapi-0.4.3/tuneapi/utils/serdeser.py` & `tuneapi-0.4.4/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/subway.py` & `tuneapi-0.4.4/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/tuneapi/utils/terminal.py` & `tuneapi-0.4.4/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.3/PKG-INFO` & `tuneapi-0.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.4.3
+Version: 0.4.4
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: MIT
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: boto3
 Requires-Dist: boto3 (==1.29.6) ; extra == "boto3"
 Requires-Dist: cloudpickle (==3.0.0)
 Requires-Dist: cryptography (>=42.0.5)
 Requires-Dist: fire (==0.5.0)
+Requires-Dist: nutree (==0.8.0)
 Requires-Dist: protobuf (>=4.25.3,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: snowflake_id (==1.0.2)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/NimbleBoxAI/tuneapi
 Description-Content-Type: text/markdown
```

