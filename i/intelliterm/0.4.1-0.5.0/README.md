# Comparing `tmp/intelliterm-0.4.1.tar.gz` & `tmp/intelliterm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelliterm-0.4.1.tar", max compression
+gzip compressed data, was "intelliterm-0.5.0.tar", max compression
```

## Comparing `intelliterm-0.4.1.tar` & `intelliterm-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-09-03 04:07:04.571987 intelliterm-0.4.1/LICENSE.txt
--rw-r--r--   0        0        0     7545 2023-10-06 00:04:55.717569 intelliterm-0.4.1/README.md
--rw-r--r--   0        0        0      368 2023-09-03 04:07:04.572627 intelliterm-0.4.1/intelliterm/__init__.py
--rw-r--r--   0        0        0    18458 2023-11-12 21:17:07.065061 intelliterm-0.4.1/intelliterm/chat.py
--rw-r--r--   0        0        0     1304 2023-09-05 00:01:59.839495 intelliterm-0.4.1/intelliterm/code.py
--rw-r--r--   0        0        0    17768 2023-11-12 21:19:18.502627 intelliterm-0.4.1/intelliterm/command_palette.py
--rw-r--r--   0        0        0     7143 2023-11-12 21:18:18.837177 intelliterm-0.4.1/intelliterm/config.py
--rw-r--r--   0        0        0     2479 2023-11-12 21:10:16.816084 intelliterm-0.4.1/intelliterm/console.py
--rw-r--r--   0        0        0      406 2023-09-05 04:05:50.741419 intelliterm-0.4.1/intelliterm/constants.py
--rw-r--r--   0        0        0     4125 2023-10-05 22:58:55.786426 intelliterm-0.4.1/intelliterm/main.py
--rw-r--r--   0        0        0      695 2023-11-12 21:10:54.586769 intelliterm-0.4.1/intelliterm/notifications.py
--rw-r--r--   0        0        0     5187 2023-10-07 20:39:28.835358 intelliterm-0.4.1/intelliterm/prompt.py
--rw-r--r--   0        0        0      708 2023-11-12 20:50:48.989909 intelliterm-0.4.1/intelliterm/styling.py
--rw-r--r--   0        0        0      284 2023-09-05 00:11:16.033316 intelliterm-0.4.1/intelliterm/types.py
--rw-r--r--   0        0        0     2248 2023-09-05 04:53:47.743699 intelliterm-0.4.1/intelliterm/utils.py
--rw-r--r--   0        0        0     1607 2023-11-12 21:25:48.645488 intelliterm-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8466 1970-01-01 00:00:00.000000 intelliterm-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-09-03 04:07:04.571987 intelliterm-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     7545 2023-10-06 00:04:55.717569 intelliterm-0.5.0/README.md
+-rw-r--r--   0        0        0     6148 2023-06-30 08:41:58.414379 intelliterm-0.5.0/intelliterm/.DS_Store
+-rw-r--r--   0        0        0       37 2023-06-30 08:07:56.945449 intelliterm-0.5.0/intelliterm/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-06-30 08:07:56.945515 intelliterm-0.5.0/intelliterm/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2023-06-30 08:07:56.945341 intelliterm-0.5.0/intelliterm/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-06-30 08:26:53.968443 intelliterm-0.5.0/intelliterm/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-06-30 08:26:53.968595 intelliterm-0.5.0/intelliterm/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      368 2023-09-03 04:07:04.572627 intelliterm-0.5.0/intelliterm/__init__.py
+-rw-r--r--   0        0        0    17700 2024-06-01 00:32:45.970235 intelliterm-0.5.0/intelliterm/chat.py
+-rw-r--r--   0        0        0     4928 2024-06-01 00:35:25.642256 intelliterm-0.5.0/intelliterm/client.py
+-rw-r--r--   0        0        0     1304 2023-09-05 00:01:59.839495 intelliterm-0.5.0/intelliterm/code.py
+-rw-r--r--   0        0        0    17634 2024-05-31 04:36:20.058461 intelliterm-0.5.0/intelliterm/command_palette.py
+-rw-r--r--   0        0        0     7224 2024-05-30 22:39:50.364742 intelliterm-0.5.0/intelliterm/config.py
+-rw-r--r--   0        0        0     2499 2024-06-01 00:27:07.352931 intelliterm-0.5.0/intelliterm/console.py
+-rw-r--r--   0        0        0      406 2023-09-05 04:05:50.741419 intelliterm-0.5.0/intelliterm/constants.py
+-rw-r--r--   0        0        0     4190 2024-05-31 04:59:11.773656 intelliterm-0.5.0/intelliterm/main.py
+-rw-r--r--   0        0        0      695 2023-11-12 21:10:54.586769 intelliterm-0.5.0/intelliterm/notifications.py
+-rw-r--r--   0        0        0     5261 2024-06-01 00:43:07.607872 intelliterm-0.5.0/intelliterm/prompt.py
+-rw-r--r--   0        0        0     9037 2024-06-01 00:45:59.108584 intelliterm-0.5.0/intelliterm/setup.py
+-rw-r--r--   0        0        0      708 2023-11-12 20:50:48.989909 intelliterm-0.5.0/intelliterm/styling.py
+-rw-r--r--   0        0        0      284 2023-09-05 00:11:16.033316 intelliterm-0.5.0/intelliterm/types.py
+-rw-r--r--   0        0        0     2248 2023-09-05 04:53:47.743699 intelliterm-0.5.0/intelliterm/utils.py
+-rw-r--r--   0        0        0     1648 2024-06-01 00:45:53.998213 intelliterm-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8601 1970-01-01 00:00:00.000000 intelliterm-0.5.0/PKG-INFO
```

### Comparing `intelliterm-0.4.1/LICENSE.txt` & `intelliterm-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `intelliterm-0.4.1/README.md` & `intelliterm-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `intelliterm-0.4.1/intelliterm/chat.py` & `intelliterm-0.5.0/intelliterm/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,37 +4,46 @@
 import subprocess
 import time
 import uuid
 from datetime import datetime
 from string import punctuation
 from typing import Any, Optional, Union
 
+import anthropic
 import openai
-from emoji import emojize
 from pick import pick
-from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 import intelliterm
+from intelliterm.client import Backend, Client
 from intelliterm.command_palette import CommandPalette, prompt
 from intelliterm.config import config
 from intelliterm.console import console
 from intelliterm.constants import CODE_THEME, SAVED_CHATS_DIR
 from intelliterm.notifications import notification
 from intelliterm.prompt import SPECIAL_PROMPTS, Prompt
 from intelliterm.types import AutoCopy
 from intelliterm.utils import get_file_info, logger, pretty_dict
 
 if "OPENAI_API_KEY" not in os.environ:
     console.error("Missing OPENAI_API_KEY")
     console.print("Add \texport OPENAI_API_KEY = 'API-KEY'\t to your .zshrc or .bashrc")
     quit()
 
+if "ANTHROPIC_API_KEY" not in os.environ:
+    console.error("Missing ANTHROPIC_API_KEY")
+    console.print(
+        "Add \texport ANTHROPIC_API_KEY = 'API-KEY'\t to your .zshrc or .bashrc"
+    )
+    quit()
+
 openai.api_key = os.getenv("OPENAI_API_KEY")
+anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
+
 
 class Chat:
     """Class representing a chat client.
 
     Attributes:
         config (Config): Configuration manager.
         _oneshot (bool): If True, exits intelliterm after completion.
@@ -71,26 +80,27 @@
         load() -> None:
             Load saved chat.
         ask(prompt: ChatPrompt, show_input: bool = True) -> None:
             Call model completion on a prompt.
         listen() -> None:
             Listen for new prompts/commands.
     """
+
     def __init__(
         self,
         oneshot: bool = False,
         autocopy: AutoCopy = "off",
     ):
         self._oneshot: bool = oneshot
         self.autocopy: AutoCopy = autocopy
         self._history: list[str] = []
         self.is_completing: bool = False
         self.chat_id: str = str(uuid.uuid4())
         self._context: list[Prompt] = [
-            Prompt(content=SPECIAL_PROMPTS['SYSTEM'], role="system")
+            Prompt(content=SPECIAL_PROMPTS["SYSTEM"], role="system")
         ]
 
     def history(self, input: str) -> None:
         """Add user input to history.
 
         Args:
             input (str)
@@ -109,30 +119,30 @@
             self._context.append(prompt)
 
     def serialize(self) -> dict[str, Any]:
         context = [prompt.serialize() for prompt in self._context]
         obj = {
             "chat_id": self.chat_id,
             "timestamp": str(datetime.now()),
-            "_context": context
+            "_context": context,
         }
         return obj
 
     @classmethod
-    def deserialize(cls, json_str: str) -> 'Chat':
-        # TODO: sdosdo 
+    def deserialize(cls, json_str: str) -> "Chat":
         dict = json.loads(json_str)
 
-        dict.pop('timestamp', None)
+        dict.pop("timestamp", None)
+        client = Client(Backend(config.get("backend")))
         chat = Chat()
         chat.__dict__.update(dict)
 
         new_context: list[Prompt] = []
 
-        for p in dict['_context']:
+        for p in dict["_context"]:
             prompt = Prompt()
             prompt.__dict__.update(p)
             new_context.append(prompt)
 
         chat._context = new_context
         return chat
 
@@ -170,17 +180,16 @@
 
         Returns:
             Optional[ChatPrompt]: Last prompt in chat. Defaults to None.
         """
         return self._context[-1] if len(self._context) > 1 else None
 
     def new(self) -> None:
-        """Start a new chat (clear context).
-        """
-        self._context = self._context[:1]     # keep system prompt
+        """Start a new chat (clear context)."""
+        self._context = self._context[:1]  # keep system prompt
         self.chat_id = str(uuid.uuid4())
         console.info("[black]Started new chat")
 
     def total_tokens(self) -> int:
         """Return total number of tokens in current chat's context.
 
         Returns:
@@ -195,42 +204,44 @@
             str: Chat info.
         """
         info = ""
         last_prompt = self.last_prompt()
         total_tokens = self.total_tokens()
 
         if last_prompt:
-            info += f"[bold][{config.get('accent_color')}]:gear: {config.active().name} "
+            info += (
+                f"[bold][{config.get('accent_color')}]:gear: {config.active().name} "
+            )
             info += f"[reset]([bold]{last_prompt.token_count()} "
             info += f"[reset]token{'s' if last_prompt.token_count() > 1 else ''}, "
             info += f"[bold]{total_tokens} [reset]total)"
         return info
 
     def file(self, path: str, prompt: Prompt) -> None:
         """Handle file input.
-        
+
         Args:
             path (str): Path to file.
             prompt (ChatPrompt): (ie: what to do with file)
         """
-        path = path.replace("~", os.environ['HOME'])
+        path = path.replace("~", os.environ["HOME"])
 
-        if os.environ['HOME'] not in path:
+        if os.environ["HOME"] not in path:
             # use cwd
             path = os.path.join(os.getcwd(), path)
 
         if os.path.exists(path):
             if os.path.isfile(path):
                 with open(path, "r") as file:
                     file_info = get_file_info(path)
                     console.print(
                         Panel(
                             pretty_dict(file_info),
                             title="[bold]:open_file_folder: file",
-                            border_style="black"
+                            border_style="black",
                         )
                     )
                     prompt.content += file.read()
                     self.ask(prompt, show_input=False)
             else:
                 # is a dir / not a file
                 return
@@ -241,19 +252,21 @@
         """Create a title for the current chat's context.
 
         Returns:
             str: Generated title.
         """
         response = openai.ChatCompletion.create(
             model=config.get("model"),
-            messages=([prompt.to_message() for prompt in self._context[1:]] +
-                      [Prompt(content=SPECIAL_PROMPTS['CHAT_TITLE']).to_message()]),
+            messages=(
+                [prompt.get_message() for prompt in self._context[1:]]
+                + [Prompt(content=SPECIAL_PROMPTS["CHAT_TITLE"]).get_message()]
+            ),
             temperature=float(config.get("temperature")),
             presence_penalty=float(config.get("presence_penalty")),
-            frequency_penalty=float(config.get("frequency_penalty"))
+            frequency_penalty=float(config.get("frequency_penalty")),
         )
         title: str = str(response.choices[0].message.content).strip(punctuation)
         title = re.sub(r'[\\/*?:"<>|]', "", title)
 
         # Duplicate check
         existing_titles = set()
         for filename in os.listdir(SAVED_CHATS_DIR):
@@ -269,23 +282,23 @@
                     highest_num = max(highest_num, number)
 
             title = f"{title}_{highest_num + 1}"
 
         return title
 
     def save(self) -> None:
-        """Save current chat.
-        """
+        """Save current chat."""
+
         def check_if_saved() -> tuple[bool, Optional[str]]:
             for file_name in os.listdir(SAVED_CHATS_DIR):
                 if file_name.endswith(".json"):
                     file_path = os.path.join(SAVED_CHATS_DIR, file_name)
                     with open(file_path) as file:
                         chat = json.loads(file.read())
-                        if chat['chat_id'] == self.chat_id:
+                        if chat["chat_id"] == self.chat_id:
                             return (True, file_name)
             return (False, None)
 
         chat_empty = len(self._context) == 1
 
         if chat_empty:
             notification.emit("Nothing to save (chat empty)")
@@ -302,22 +315,21 @@
             file_name = f"{title}.json"
             file_path = os.path.join(SAVED_CHATS_DIR, file_name)
 
         with open(file_path, "w+") as file:
             chat_dict = self.serialize()
             json.dump(chat_dict, file, indent=4)
 
-            file_path = file_path.replace(os.environ['HOME'], '~')
+            file_path = file_path.replace(os.environ["HOME"], "~")
             logger.info(f"Saved chat ${self.chat_id}: ${file_path}")
             notification.emit(f"[black]Saved chat to: ${file_path}")
 
     # TODO(add test)
     def load(self) -> None:
-        """Load a saved chat.
-        """
+        """Load a saved chat."""
         file_names: list[str] = []
         chats: list[str] = []
 
         if os.path.exists(SAVED_CHATS_DIR):
             for file_name in os.listdir(SAVED_CHATS_DIR):
                 file_path = os.path.join(SAVED_CHATS_DIR, file_name)
 
@@ -345,82 +357,52 @@
     def ask(self, prompt: Prompt, show_input: bool = True) -> None:
         """Call model completion on a prompt.
 
         Args:
             prompt (ChatPrompt)
             show_input (bool): Show/hide input before completion. Defaults to True.
         """
-        prompt_message = prompt.to_message()
+        client = Client(Backend(config.get("backend")))
+        prompt_message = prompt.get_message()
 
         console.clear()
         logger.info(prompt_message)
 
         self.context(prompt)
 
         if not self._oneshot and show_input:
             console.print(
                 Panel(
                     Markdown(prompt.content, code_theme=CODE_THEME),
                     title=self.info(),
                     title_align="right",
-                    border_style="black"
+                    border_style="black",
                 )
             )
 
-        markdown = Markdown("", code_theme=CODE_THEME)
         full_content = ""
+        markdown = Markdown("", code_theme=CODE_THEME)
 
         try:
             self.is_completing = True
             start_time = time.time()
-            response = openai.ChatCompletion.create(
-                model=config.get("model"),
-                messages=[prompt.to_message() for prompt in self._context],
-                temperature=float(config.get("temperature")),
-                presence_penalty=float(config.get("presence_penalty")),
-                frequency_penalty=float(config.get("frequency_penalty")),
-                stream=True,
-            )
-
-            messages = []
-
-            with Live(
-                markdown,
-                console=console,
-                transient=True,
-                refresh_per_second=40,
-                vertical_overflow="visible"
-            ) as live:
-                for chunk in response:
-                    message = chunk['choices'][0]['delta']
-                    messages.append(message)
-
-                    full_content = "".join([m.get("content", "") for m in messages])
-                    markdown = Markdown(
-                        full_content,
-                        code_theme=CODE_THEME,
-                    )
-                    live.update(markdown)
-            response.close()
-        except openai.InvalidRequestError as e:
-            console.print("openai:", e)
-            return None
-        except Exception as e:
-            console.print(e)
+            full_content = client.get_response(prompt, self._context, markdown) or ""
         except (KeyboardInterrupt, EOFError):
             if self.is_completing:
                 console.with_divider(":stop_button: aborted")
                 return None
+        except Exception as e:
+            console.print(e)
         finally:
             self.is_completing = False
             self.context(
                 Prompt(
                     content=full_content,
                     role="assistant",
-                    took=time.time() - start_time
+                    took=time.time() - start_time,
                 )
             )
             console.print(markdown)
 
         last_prompt = self.last_prompt()
 
         if last_prompt:
@@ -434,16 +416,15 @@
         else:
             console.with_divider()
 
         if not self._oneshot:
             self.listen()
 
     def listen(self) -> None:
-        """Listen for new prompts/commands.
-        """
+        """Listen for new prompts/commands."""
         while True:
             try:
                 input = prompt()
 
                 if input is not None and len(input) > 0:
                     self.history(input)
 
@@ -481,15 +462,15 @@
                                             last_prompt.parse_code()[0].run()
                                     else:
                                         notification.emit("No code to run")
                                 case "file":
                                     if len(options) > 0:
                                         self.file(
                                             options[0],
-                                            Prompt(content="".join(options[1:]))
+                                            Prompt(content="".join(options[1:])),
                                         )
                                     else:
                                         console.error("No file specified")
                                         console.print(command.hint())
                                 case "new":
                                     self.new()
                                 case "shell":
```

### Comparing `intelliterm-0.4.1/intelliterm/code.py` & `intelliterm-0.5.0/intelliterm/code.py`

 * *Files identical despite different names*

### Comparing `intelliterm-0.4.1/intelliterm/command_palette.py` & `intelliterm-0.5.0/intelliterm/command_palette.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 from intelliterm.console import console
 from intelliterm.notifications import notification
 
 key_bindings = KeyBindings()
 
 
 # TODO(implement): add useful bindings
-@key_bindings.add("escape", "c")     # option + c
+@key_bindings.add("escape", "c")  # option + c
 def exit_(event: Any) -> None:
     """
-        Pressing Ctrl-d will exit the user interface.
-        """
+    Pressing Ctrl-d will exit the user interface.
+    """
     event.app.exit()
 
 
 # TODO(possibly): persist prompt history across sessions
 def get_history() -> None:
     pass
 
 
-session: PromptSession = PromptSession()     #history=)
+session: PromptSession = PromptSession()  # history=)
 
 
 def bottom_toolbar() -> Any:
     from intelliterm.config import config
 
     buffer = session.default_buffer
     input = buffer.text
@@ -63,71 +63,75 @@
                         arg.name if arg.is_option else f"&lt;{arg.name}&gt;"
                         for arg in command.args
                     )
             if output.startswith(CommandPalette.TRIGGER):
                 output_groups = output.split(" ", 1)
 
                 try:
-                    output_groups[curr_index
-                                  ] = f"<strong>{output_groups[curr_index]}</strong>"
+                    output_groups[curr_index] = (
+                        f"<strong>{output_groups[curr_index]}</strong>"
+                    )
                     output = " ".join(output_groups)
                 except IndexError:
                     pass
         else:
             if input != CommandPalette.TRIGGER:
                 output = f"Unknown command: <strong><style color='ansired'>{input.strip()}</style></strong>"
     return HTML(output)
 
 
 def rprompt() -> str:
     from intelliterm.config import config
+
     return f"[{config.active().name}]"
 
 
 def prompt() -> str:
     """Prompt for user input.
-    
+
     Returns:
         str: User input.
     """
     from intelliterm.config import config
 
-    style: Style = Style.from_dict({
-        "": "",
-        "caret": f"fg:ansi{config.get('accent_color')}",
-        "bottom-toolbar": "fg:ansiblack bg:black",
-    })
+    style: Style = Style.from_dict(
+        {
+            "": "",
+            "caret": f"fg:ansi{config.get('accent_color')}",
+            "bottom-toolbar": "fg:ansiblack bg:black",
+        }
+    )
 
     return session.prompt(
         message=[
             ("class:caret", ">"),
             ("class:input", " "),
         ],
         auto_suggest=AutoSuggestFromHistory(),
         completer=FuzzyCompleter(CommandCompleter()),
         mouse_support=False,
         key_bindings=key_bindings,
         validator=validator,
         validate_while_typing=False,
         bottom_toolbar=bottom_toolbar,
         placeholder=HTML(f"<ansiblack>  ({config.active().name})</ansiblack>"),
-     # rprompt=rprompt,
+        # rprompt=rprompt,
         style=style,
     )
 
 
 class CommandArgument:
     """Class defining a command argument/option.
-    
+
     Attributes:
         name (str): Argument name.
         pos (Optional[int]): Argument position.
         is_option (bool): Argument is an option for a command. Defaults to False.
             (ex: "edit" in: !config edit)
-    
+
     """
 
     # TODO(refactor): remove `is_option` (ie: improve logic separation)
     def __init__(
         self,
         name: str,
         pos: Optional[int] = None,
@@ -136,61 +140,64 @@
         self.name = name
         self.pos = pos
         self.is_option = is_option
 
 
 class CommandExample:
     """Class defining a command usage CommandExample.
-    
+
     Attributes:
         command (str): Command name.
         args (Optional[list[Argument]]): List of command arguments/options.
     """
+
     def __init__(self, command: str, args: Optional[list[CommandArgument]]) -> None:
         self.command = command
         self.args = args
 
 
 class CommandUsage:
     """Class defining a usage CommandExample for a `Command`.
-    
+
     Attributes:
         command (str): Command name.
         description (str): Usage description.
         args (list[Argument]): List of arguments. Defaults to empty list.
         examples (list[CommandExample]): List of examples. Defaults to empty list.
-        
+
     Methods:
         hint() -> str:
             Returns a helpful hint explaining how to use a command.
     """
+
     def __init__(
         self,
         command: str,
         description: str,
         args: list[CommandArgument] = [],
         examples: list[CommandExample] = [],
     ):
         self.command = command
         self.args = args
         self.description = description
         self.examples = examples
 
     def hint(self) -> str:
         """Returns a helpful hint explaining how to use a command.
-        
+
         Returns:
             str
         """
         hint = f"[command]{CommandPalette.TRIGGER}{self.command}[reset]"
 
         for arg in self.args:
             hint += (
                 f" [option]{arg.name}[reset]"
-                if arg.is_option else f" [arg]<{arg.name}>[reset]"
+                if arg.is_option
+                else f" [arg]<{arg.name}>[reset]"
             )
         hint += f"\n\t\t{self.description}\n"
 
         if self.examples:
             hint += "\t\t[bold italic]example:[reset] "
 
             for example in self.examples:
@@ -201,26 +208,27 @@
                         hint += f"[arg] {arg.name}"
         hint += "[reset]\n\n"
         return hint
 
 
 class Command:
     """Class defining a CommandPalette command.
-    
+
     Attributes:
         name (str): Command name.
         description (str): Command description.
         aliases (list[str]): Command aliases.
         args (Optional[list[Argument]]): Command arguments. Defaults to None.
         usage (Optional[list[Usage]]): Command usage template. Defaults to None.
-            
+
     Methods:
         hint() -> str:
             Return documentation hint (command options, usage and examples).
     """
+
     def __init__(
         self,
         name: str,
         description: str,
         aliases: list[str],
         args: Optional[list[CommandArgument]] = None,
         usage: Optional[list[CommandUsage]] = None,
@@ -229,57 +237,59 @@
         self.description = description
         self.aliases = aliases
         self.args = args
         self.usage = usage
 
     def hint(self) -> str:
         """Return documentation hint (command options, usage and examples).
-        
-        Returns: 
+
+        Returns:
             str
         """
         hint = ""
 
         if self.args:
             args = [a for a in self.args if not a.is_option]
             options = [a for a in self.args if a.is_option]
 
             if args:
                 hint += "  [bold italic]args:[reset]\n"
                 hint += "\n".join(f"\t[arg]<{arg.name}>[reset]" for arg in args) + "\n"
             if options:
                 hint += "  [bold italic]options:[reset]\n"
-                hint += "\n".join(
-                    f"\t[option]{option.name}[reset]" for option in options
-                ) + "\n"
+                hint += (
+                    "\n".join(f"\t[option]{option.name}[reset]" for option in options)
+                    + "\n"
+                )
         if self.usage:
             hint += "  [bold italic]usage:[reset]\n\t"
             hint += "\t".join(u.hint() for u in self.usage)
 
         return hint
 
 
 class CommandPalette:
     """Class representing a command manager that handles intelliterm-specific commands.
-    
+
     Methods:
         get_command(alias: str) -> Optional[Command]:
-            Get command matching alias.  
+            Get command matching alias.
         help() -> None:
             Show available commands and how to use them.
         is_command(input: str) -> bool:
             Utility to check if input starts with the command trigger.
         is_valid_input(input: str) -> bool:
             Check if input matches a valid command alias.
         is_secondary_alias(alias: str) -> bool:
-            Check if alias is not a primary alias 
+            Check if alias is not a primary alias
             (ie: is shortened variant, like `h` for `help`).
         unrecognized(alias: str) -> None:
             Handle unrecognized command alias.
     """
+
     TRIGGER: str = "!"
     COMMAND_REGEX = r"^!(\w+)(?:\s{0,1}(.*))?"
 
     AVAILABLE_COMMANDS: list[Command] = [
         Command(
             name="help",
             description="Show available commands",
@@ -296,39 +306,35 @@
             args=[
                 CommandArgument("name"),
                 CommandArgument("edit", is_option=True),
                 CommandArgument("reset", is_option=True),
             ],
             aliases=["u", "use", "cfg", "switch", "config"],
             usage=[
-                CommandUsage(
-                    command="config",
-                    description="Show active configuration",
-                ),
+                CommandUsage(command="config", description="Show active configuration"),
                 CommandUsage(
                     command="use",
                     args=[CommandArgument("name")],
-                    description=
-                    "[reset]Use / switch to another configuration (case-insensitive)",
+                    description="[reset]Use / switch to another configuration (case-insensitive)",
                     examples=[
                         CommandExample(command="use", args=[CommandArgument("gpt3")])
                     ],
                 ),
                 CommandUsage(
                     command="config",
                     args=[CommandArgument("edit", is_option=True)],
                     description=(
-                        "Edit configurations file " +
-                        f"(via {os.environ.get('EDITOR', 'nano')})"
-                    )
+                        "Edit configurations file "
+                        + f"(via {os.environ.get('EDITOR', 'nano')})"
+                    ),
                 ),
                 CommandUsage(
                     command="config",
                     args=[CommandArgument("reset", is_option=True)],
-                    description="Reset configuration to defaults"
+                    description="Reset configuration to defaults",
                 ),
             ],
         ),
         Command(
             name="info",
             description="Show chat info",
             aliases=["i", "info"],
@@ -348,15 +354,15 @@
             description="Load chat",
             aliases=["l", "load"],
         ),
         Command(
             name="copy",
             description="Copy response",
             aliases=["c", "copy"],
-            args=[CommandArgument("code", is_option=True)]
+            args=[CommandArgument("code", is_option=True)],
         ),
         Command(
             name="run",
             description="Run code block in response",
             aliases=["r", "run"],
         ),
         Command(
@@ -377,123 +383,121 @@
                     description="Input file with prompt",
                     examples=[
                         CommandExample(
                             command="file",
                             args=[
                                 CommandArgument("file.txt"),
                                 CommandArgument("explain this file"),
-                            ]
+                            ],
                         )
-                    ]
+                    ],
                 ),
             ],
         ),
         Command(
             name="shell",
             description="Run a shell command",
             aliases=["os", "shell"],
             args=[CommandArgument("command")],
             usage=[
                 CommandUsage(
                     command="shell",
                     args=[CommandArgument("command")],
-                    description=
-                    f"Run basic shell commands within {intelliterm.__name__}",
+                    description=f"Run basic shell commands within {intelliterm.__name__}",
                     examples=[
                         CommandExample(command="shell", args=[CommandArgument("ls")])
-                    ]
+                    ],
                 ),
             ],
         ),
         Command(
             name="quit",
             description=f"Quit {intelliterm.__name__}",
             aliases=["q", "quit"],
-        )
+        ),
     ]
 
     GROUPED_ALIASES = [command.aliases for command in AVAILABLE_COMMANDS]
     PRIMARY_ALIASES = [
         command.name if command.name in command.aliases else command.aliases[0]
         for command in AVAILABLE_COMMANDS
     ]
     ALL_ALIASES = [alias for command in AVAILABLE_COMMANDS for alias in command.aliases]
 
     @staticmethod
     def get_command(alias: str) -> Optional[Command]:
         """Get command matching alias.
-        
-        Args: 
+
+        Args:
             alias (str): Command alias.
-            
+
         Returns:
             Optional(Command): Command if it exists, otherwise None.
         """
         alias = alias.replace(CommandPalette.TRIGGER, "")
         return next(
             (
-                command for command in CommandPalette.AVAILABLE_COMMANDS
+                command
+                for command in CommandPalette.AVAILABLE_COMMANDS
                 if alias in command.aliases
             ),
             None,
         )
 
     @staticmethod
     def get_aliases(command_name: str) -> list[str]:
         """Get all aliases for command with name.
-        
+
         Args:
             command_name (str): Command name.
-            
+
         Returns:
             list[str]: List of aliases associated with command.
         """
         aliases = []
         command = CommandPalette.get_command(command_name)
 
         if command:
             aliases = command.aliases
         return aliases
 
     @staticmethod
     def help() -> None:
-        """Show available commands and how to use them.
-        """
+        """Show available commands and how to use them."""
         help_message = ""
 
         for i, command in enumerate(CommandPalette.AVAILABLE_COMMANDS):
             aliases = [CommandPalette.TRIGGER + alias for alias in command.aliases]
             help_message += f"[command]{', '.join(aliases)}"
             help_message += f"[reset] : {command.description}"
-            help_message += "\n" if i != len(
-                CommandPalette.AVAILABLE_COMMANDS
-            ) - 1 else ""
+            help_message += (
+                "\n" if i != len(CommandPalette.AVAILABLE_COMMANDS) - 1 else ""
+            )
             help_message += command.hint()
         console.print(Panel(help_message, title="Commands", border_style="black"))
 
     @staticmethod
     def is_valid_input(input: str) -> bool:
         """Check if input matches a valid command alias.
-        
+
         Args:
             input (str): User input.
-            
+
         Returns:
             bool
         """
         if input.startswith(CommandPalette.TRIGGER):
-            match = re.match(CommandPalette.COMMAND_REGEX, input)     # is command
+            match = re.match(CommandPalette.COMMAND_REGEX, input)  # is command
             return match.group(1) in CommandPalette.ALL_ALIASES if match else False
         else:
-            return True     # is regular text
+            return True  # is regular text
 
     @staticmethod
     def unrecognized(alias: str) -> None:
-        """Handle unrecognized command alias.
-        """
+        """Handle unrecognized command alias."""
         grouped_commands = [
             " ".join(["!" + alias for alias in command.aliases])
             for command in CommandPalette.AVAILABLE_COMMANDS
         ]
         columns = [Panel(group) for group in grouped_commands]
         console.print(Columns(columns))
 
@@ -503,27 +507,27 @@
         error += "[reset] or [command]!h[reset] "
         error += "to see available commands."
 
         console.error(error)
 
     @staticmethod
     def is_secondary_alias(alias: str) -> bool:
-        """Check if alias is not a primary alias 
-            (ie: is shortened variant, like `h` for `help`).
-           
-            Returns:
-                bool
+        """Check if alias is not a primary alias
+        (ie: is shortened variant, like `h` for `help`).
+
+        Returns:
+            bool
 
         """
         return alias not in CommandPalette.PRIMARY_ALIASES
 
 
 class CommandCompleter(Completer):
-    """Auto-completion for CommandPalette.
-    """
+    """Auto-completion for CommandPalette."""
+
     def get_completions(self, document: Any, complete_event: Any) -> Generator:
         from intelliterm.config import config
 
         # current_position: Point = document.get_menu_position()
         # print(current_position)
 
         word: str = document.current_line.replace(CommandPalette.TRIGGER, "")
@@ -535,19 +539,20 @@
             for command in CommandPalette.AVAILABLE_COMMANDS:
                 for alias in command.aliases:
                     if alias.startswith(word):
                         yield Completion(
                             CommandPalette.TRIGGER + alias,
                             start_position=document.get_start_of_document_position(),
                             style=f"fg:ansi{config.get('accent_color')} bg:black",
-                        # selected_style="fg:black bg:red ",
-                            display_meta=
-                            f"(aliased: {CommandPalette.TRIGGER + command.name})"
-                            if CommandPalette.is_secondary_alias(alias) else
-                            command.description,
+                            # selected_style="fg:black bg:red ",
+                            display_meta=(
+                                f"(aliased: {CommandPalette.TRIGGER + command.name})"
+                                if CommandPalette.is_secondary_alias(alias)
+                                else command.description
+                            ),
                         )
 
 
 validator = Validator.from_callable(
     CommandPalette.is_valid_input,
     error_message="Invalid command",
 )
```

### Comparing `intelliterm-0.4.1/intelliterm/config.py` & `intelliterm-0.5.0/intelliterm/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,190 +13,190 @@
 from intelliterm.constants import USER_DATA_DIR
 from intelliterm.notifications import notification
 from intelliterm.utils import TIPS, logger, longest_line, pretty_dict
 
 
 class Config:
     """Intelliterm configurations manager.
-    
+
     Methods:
         exists() -> bool:
             Check if configuration file exists.
         default() -> ConfigParser:
             Get default configuration.
         active() -> SectionProxy:
             Get active configuration.
         show() -> None:
             Display active and available configurations.
-        get(property: Optional[str] = None) -> str:    
+        get(property: Optional[str] = None) -> str:
             Get property in active configuration.
         edit() -> None:
             Edit configurations file.
         load() -> None:
-            Load configurations file. 
+            Load configurations file.
         use(config_name: str) -> None:
             Use a different configuration.
         reset() -> None:
             Reset to default configurations file.
     """
 
     CONFIG_PATH = os.path.join(USER_DATA_DIR, "config.ini")
 
     def __init__(self) -> None:
         self.config: ConfigParser = ConfigParser()
         self.load()
 
     @staticmethod
     def exists() -> bool:
-        """Check if configuration file exists.
-        """
+        """Check if configuration file exists."""
         return os.path.exists(Config.CONFIG_PATH) and os.path.isfile(Config.CONFIG_PATH)
 
     @staticmethod
     def default() -> ConfigParser:
-        """Get default configuration.
-        """        
-        default_config = ConfigParser(default_section='GPT3')
-        default_config['DEFAULT'] = {
+        """Get default configuration."""
+        default_config = ConfigParser(default_section="GPT3")
+        default_config["DEFAULT"] = {
+            "backend": "openai",
             "model": "gpt-3.5-turbo",
             "temperature": "0",
             "presence_penalty": "0",
             "frequency_penalty": "0",
-            "accent_color": "blue"
+            "accent_color": "blue",
         }
-        default_config['GPT3'] = {
+        default_config["GPT3"] = {
             "model": "gpt-3.5-turbo",
         }
-        default_config['GPT4'] = {
+        default_config["GPT4"] = {
             "model": "gpt-4",
         }
-        default_config['CONFIG'] = {
-            "active": 'GPT3',
+        default_config["CONFIG"] = {
+            "active": "GPT3",
         }
 
         return default_config
 
     def active(self) -> SectionProxy:
-        """Get active configuration.
-        """
-        return self.config[self.config['CONFIG']['active']]
+        """Get active configuration."""
+        return self.config[self.config["CONFIG"]["active"]]
 
     def show(self) -> None:
-        """Display active and available configurations.
-        """
+        """Display active and available configurations."""
         panels: list[Panel] = []
 
         for section in self.config:
             if section != "CONFIG" and section != "DEFAULT":
                 pretty_config = pretty_dict(
                     dict(self.config[section]),
                     colors=section == self.active().name,
                 )
 
                 if section == self.active().name:
                     content = (
-                        f"[{self.get('accent_color')}][bold]{section}[reset]" + "\n" +
-                        ("-" * longest_line(pretty_config) + "\n") + pretty_config
+                        f"[{self.get('accent_color')}][bold]{section}[reset]"
+                        + "\n"
+                        + ("-" * longest_line(pretty_config) + "\n")
+                        + pretty_config
                     )
 
                     panels.append(
                         Panel(
                             content,
-                            border_style=self.get('accent_color'),
+                            border_style=self.get("accent_color"),
                             title="(active)",
-                            title_align="right"
+                            title_align="right",
                         )
                     )
                 else:
                     panels.append(
-                        Panel((
-                            section + "\n" + ("-" * longest_line(pretty_config)) + "\n"                            
-                        ) + pretty_config,
-                            border_style="black")
+                        Panel(
+                            (
+                                section
+                                + "\n"
+                                + ("-" * longest_line(pretty_config))
+                                + "\n"
+                            )
+                            + pretty_config,
+                            border_style="black",
+                        )
                     )
 
-        config_command = CommandPalette.get_command('config')
+        config_command = CommandPalette.get_command("config")
 
         if config_command:
             if config_command and config_command.args:
                 console.print(
                     Panel(
                         Columns(panels),
                         title="[bold]:gear: Configurations",
-                        subtitle=(random.choice(TIPS['config'])),
+                        subtitle=(random.choice(TIPS["config"])),
                         title_align="left",
                         subtitle_align="left",
-                        border_style="black"
+                        border_style="black",
                     )
                 )
 
     def get(self, property: str) -> str:
         """Get property in active configuration.
-        
+
         Args:
             property (str): Property to get from active configuration.
-            
+
         Returns:
             str: Value for property if not None, else, name of active configuration.
         """
         return self.active()[property]
 
     def edit(self) -> None:
-        """Edit configurations file.
-        """
+        """Edit configurations file."""
         subprocess.run([os.environ.get("EDITOR", "nano"), Config.CONFIG_PATH])
         self.load()
         self.show()
 
     def validate(self) -> None:
         # TODO(finish)
-        required_values: dict[str, Any] = {
-            "": {}
-        }
+        required_values: dict[str, Any] = {"": {}}
 
         for section, keys in required_values.items():
             if section not in self.config:
                 raise Exception(f"Missing section {section} in config")
 
     def load(self) -> None:
-        """Load configurations file.
-        """
+        """Load configurations file."""
         if not self.exists():
             os.makedirs(os.path.dirname(Config.CONFIG_PATH), exist_ok=True)
             with open(Config.CONFIG_PATH, "w+") as file:
                 self.default().write(file)
                 logger.info("Configurations file not found, set to default")
         self.config.read(Config.CONFIG_PATH)
 
     def use(self, config_name: str) -> None:
         """Use a different configuration.
-        
+
         Args:
             config_name (str): Name of configuration to set as active.
         """
-        config_name = config_name.upper()     # case-insensitive
+        config_name = config_name.upper()  # case-insensitive
 
         self.config.read(Config.CONFIG_PATH)
 
         if config_name != "CONFIG" and self.config.has_section(config_name):
             self.config.set("CONFIG", "active", config_name)
 
             with open(Config.CONFIG_PATH, "w+") as config_file:
                 self.config.write(config_file)
                 self.load()
-                notification.emit(f"Switched to <strong>{self.active().name}</strong>")
+                notification.emit(f"Switched to {self.active().name}")
                 logger.info(f"{self.active().name} {dict( self.active())}")
         else:
             console.error(f"No configuration named {config_name}")
             logger.info(f"No configuration named {config_name}")
             self.show()
 
     def reset(self) -> None:
-        """Reset to default configurations file.
-        """
+        """Reset to default configurations file."""
         yes: bool = confirm("Reset to default configuration?")
 
         if yes:
             with open(Config.CONFIG_PATH, "w+") as config_file:
                 self.default().write(config_file)
                 logger.info(f"{Config.CONFIG_PATH} reset to defaults")
             self.load()
@@ -205,13 +205,12 @@
     def to_dict(self) -> dict:
         """Transform config to dictionary.
 
         Returns:
             dict[str, str]
         """
         return {
-            section: dict(self.config[section])
-            for section in self.config.sections()
+            section: dict(self.config[section]) for section in self.config.sections()
         }
 
 
 config = Config()
```

### Comparing `intelliterm-0.4.1/intelliterm/console.py` & `intelliterm-0.5.0/intelliterm/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,64 +13,65 @@
     """A class for printing formatted messages to the console.
 
     Inherits from rich.console's `Console`.
 
     Methods:
         info(*objects: Any) -> None:
             Prints the given objects to the console as information.
-        warning(*objects: Any) -> None: 
+        warning(*objects: Any) -> None:
             Prints the given objects to the console as a warning.
-        error(*objects: Any) -> None: 
+        error(*objects: Any) -> None:
             Prints the given objects to the console as an error.
-        divider(*objects: Any) -> None:  
+        divider(*objects: Any) -> None:
             Prints a divider as wide as the terminal window.
     """
+
     def info(self, *objects: Any, sep: str = " ", end: str = "\n") -> None:
-        """Print to console as info.
-        """
+        """Print to console as info."""
         message = " ".join(str(o) for o in objects)
         self.print(
             f"[bold blue]i [info][not bold]{message}",
             style=INFO_STYLE,
         )
 
     def warning(self, *objects: Any, sep: str = " ", end: str = "\n") -> None:
-        """Print to console as warning.
-        """
+        """Print to console as warning."""
         message = " ".join(str(o) for o in objects)
         self.print(
             f":warning: {message}",
             sep=sep,
             end=end,
             style=WARNING_STYLE,
         )
 
     def error(self, *objects: Any, sep: str = " ", end: str = "\n") -> None:
-        """Print to console as error.
-        """
+        """Print to console as error."""
         message = " ".join(str(o) for o in objects)
         self.print(
             f":warning: {message}",
             sep=sep,
             end=end,
             style=DANGER_STYLE,
         )
 
     def with_divider(self, title: Optional[str] = None) -> None:
         """Print a divider as wide as the terminal window.
-        
+
         Args:
             title (Optional[str]): Title to center in divider. Defaults to None.
         """
         if title:
             has_emoji = re.search(r":\w+:", title)
             emoji_offset = len(has_emoji.group()) if has_emoji else 0
             offset = (len(title) - emoji_offset + 2) // 2
 
             self.print(
-                (f"[black]{title} " + "-" * (os.get_terminal_size().columns - len(title))),
+                (
+                    f"[black]{title} "
+                    + "-" * (os.get_terminal_size().columns - len(title))
+                ),
             )
         else:
-            self.print('-' * os.get_terminal_size().columns)
+            self.print("-" * os.get_terminal_size().columns)
 
 
 console = Console(theme=Theme(cast(Mapping[str, StyleType] | None, COLORS)))
```

### Comparing `intelliterm-0.4.1/intelliterm/main.py` & `intelliterm-0.5.0/intelliterm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 import logging
 import os
 import sys
 from typing import NoReturn, Optional
 
 from intelliterm import __version__
 from intelliterm.chat import Chat
+from intelliterm.client import Backend, Client
+from intelliterm.config import config
 from intelliterm.console import console
 from intelliterm.prompt import SPECIAL_PROMPTS, Prompt
 from intelliterm.utils import (
     intelliterm,
     is_git_diff,
     logger,
     setup_dirs,
     setup_logging,
 )
 
-
 __author__ = "Yulian Kraynyak"
 __copyright__ = "Yulian Kraynyak"
 __license__ = "MIT"
 
 _logger = logging.getLogger(__name__)
 
 
@@ -47,18 +48,18 @@
             raise argparse.ArgumentTypeError(f"[danger]{path} [reset]is not a file")
         else:
             return path
 
 
 def parse_args(args: list[str]) -> argparse.Namespace:
     """Parse command line parameters.
-    
+
     Args:
         args (list[str]): CLI parameters as list of strings (for example  `["--help"]`).
-            
+
     Returns:
         argparse.Namespace: CLI parameters namespace.
     """
     parser = ArgParser()
     parser.add_argument(
         "-v",
         "-V",
@@ -70,15 +71,15 @@
     parser.add_argument(
         dest="prompt",
         help="prompt",
         nargs="*",
         type=str,
         metavar="STR",
     )
-    parser.add_argument(     # TODO(unfinished)
+    parser.add_argument(  # TODO(unfinished)
         "-f",
         "--file",
         dest="file",
         help="input a file",
         type=ArgParser.validate_file,
     )
     parser.add_argument(
@@ -144,15 +145,15 @@
             prompt = Prompt(content=" ".join(args.prompt) + sys.stdin.read().strip())
             chat.ask(prompt)
         else:
             prompt = Prompt(content=sys.stdin.read().strip())
 
             if len(prompt.content) > 0:
                 if is_git_diff(prompt.content):
-                    prompt.content = SPECIAL_PROMPTS['GIT_DIFF'] + prompt.content
+                    prompt.content = SPECIAL_PROMPTS["GIT_DIFF"] + prompt.content
                 chat.oneshot(True)
                 chat.ask(prompt)
             else:
                 console.error("Empty input")
 
 
 def run() -> None:
```

### Comparing `intelliterm-0.4.1/intelliterm/notifications.py` & `intelliterm-0.5.0/intelliterm/notifications.py`

 * *Files identical despite different names*

### Comparing `intelliterm-0.4.1/intelliterm/prompt.py` & `intelliterm-0.5.0/intelliterm/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,117 +1,126 @@
 # ruff: noqa: E501
 
 import json
+import os
 import platform
 import re
-from typing import Any, Literal, Optional, cast
+from typing import Any, Literal, Optional, TypedDict, cast
 
 import pyperclip
 import tiktoken
 
 import intelliterm
 from intelliterm.code import Code
 from intelliterm.config import config
 from intelliterm.console import console
 from intelliterm.notifications import notification
 
-# TODO(improve): extend `bio` with helpful, general info about self for better responses
 bio = {
     "os": platform.system(),
+    "config": config.to_dict(),
 }
 
+DEFAULT_ENCODING = "gpt-3.5-turbo"
 SPECIAL_PROMPTS = {
-    "SYSTEM":
-        f"""
+    "SYSTEM": f"""
         You are {intelliterm.__name__}, 
         a general knowledge and code assistant running via CLI and specializing in short, straight-to-the-point, intuitive answers.
         
-        My bio: {bio}
+        Use this context for questions about config, environment you are running in: {bio}
         
-        If I ask anything that involves my bio make sure to make clear
-        that all information is general/approximate/non-identifying.
+        If I ask anything that involves who you are, clarify that all information is general/approximate/non-identifying.
         
         If input is a concept: use analogies to related concepts.
         Edit every response to ensure the following rules are always satisfied:
             - Style the following terms as bold in markdown:
                 - names of individuals
                 - names of companies and corporations
                 - names of company products                
                 - stock tickers
             - Code snippets must support syntax highlighting
             - Do not explain code that is short or simple, simply 
               respond with the code itself
         Input:
         """.strip(),
-    "GIT_DIFF":
-        """
+    "GIT_DIFF": """
         Generate a commit message, max 50 characters, in conventional format:
         """.strip(),
-    "CHAT_TITLE":
-        """Summarize this in a maximum of 20 characters"""
+    "CHAT_TITLE": """Summarize this in a maximum of 20 characters""",
 }
 
 Role = Literal["system", "assistant", "user"]
 
 
+class Message(TypedDict, total=False):
+    content: Any  # TODO: add multi-modal support
+    role: Role
+
+
 class Prompt:
     """Class representing a chat prompt.
-    
+
     Attributes:
         role (Role): Role to assume. Defaults to "user".
         content (str): Prompt content.
         is_file (bool): File input flag.
-        
+
     Methods:
         copy(options: Optional[list[str]] = None) -> None:
             Copy prompt content/code to the clipboard.
-        to_message() -> dict[str, str]:  
+        to_message() -> dict[str, str]:
             Transform to OpenAI Chat Completion message.
         token_count() -> int:
             Count number of tokens in prompt content.
         get_code() -> Optional[Code]:
             Extract code from prompt content.
     """
+
     def __init__(
         self,
         is_file: bool = False,
         content: str = "",
         role: Role = "user",
-        took: Optional[float] = None
+        took: Optional[float] = None,
     ) -> None:
         self.is_file: bool = is_file
         self.content: str = content
         self.role: Role = role
         self.took: float = 0
 
     def serialize(self) -> dict[str, Any]:
         return self.__dict__
 
     @classmethod
-    def deserialize(cls, json_str: str) -> 'Prompt':
+    def deserialize(cls, json_str: str) -> "Prompt":
         dict = json.loads(json_str)
         return cast(Prompt, dict)
 
     def token_count(self) -> int:
         """Count number of tokens in prompt content.
 
         Returns:
             int: Number of tokens in prompt content.
         """
-        encoding = tiktoken.encoding_for_model(config.get("model"))
+        encoding = tiktoken.encoding_for_model(
+            config.get("model")
+            if config.get("model").startswith("gpt")
+            else DEFAULT_ENCODING
+        )
         num_tokens = len(encoding.encode(self.content))
         return num_tokens
 
     def copy(self, options: Optional[list[str]] = None) -> None:
         """Copy prompt content or code to clipboard.
 
         Args:
-            options (Optional[list[str]]): 
+            options (Optional[list[str]]):
                 Copy command options. Defaults to None.
         """
+
         def _copy_to_clipboard(text: str) -> None:
             if len(text) == 0:
                 console.print("Nothing to copy")
                 return
             pyperclip.copy(text)
 
         if options is not None and len(options) > 0:
@@ -125,38 +134,29 @@
                         _copy_to_clipboard(code_blocks[0].code)
                         console.with_divider(":clipboard: code copied!")
                     elif len(code_blocks) > 1:
                         # TODO(implement): handle multiple code blocks
                         pass
                     else:
                         notification.emit("No code to copy")
-
         else:
             # > !c
             # Copy all content.
             if len(self.content) > 0:
                 _copy_to_clipboard(self.content)
                 console.with_divider(":clipboard: copied!")
 
-    def to_message(self) -> dict[str, Any]:
-        """Transform to OpenAI Chat Completion message.
-
-        Returns:
-            dict[str, Any]
-        """
-        return {
-            "content": self.content,
-            "role": self.role
-        }
+    def get_message(self) -> Message:
+        return {"role": self.role, "content": self.content}
 
     def parse_code(self) -> list[Code]:
         """Extract code blocks from prompt content.
 
-        Returns: 
-            list[Code] 
+        Returns:
+            list[Code]
         """
         found_code_blocks = re.findall(r"```(\w+)\n([\s\S]*?)\n```", self.content)
         code_blocks: list[Code] = []
 
         for found in found_code_blocks:
             language = found[0]
             code = found[1]
```

### Comparing `intelliterm-0.4.1/intelliterm/styling.py` & `intelliterm-0.5.0/intelliterm/styling.py`

 * *Files identical despite different names*

### Comparing `intelliterm-0.4.1/intelliterm/utils.py` & `intelliterm-0.5.0/intelliterm/utils.py`

 * *Files identical despite different names*

### Comparing `intelliterm-0.4.1/pyproject.toml` & `intelliterm-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "intelliterm"
-version = "0.4.1"
+version = "0.5.0"
 description = "Chat with AI from your terminal!"
 authors = ["Yulian Kraynyak <yulian@yulian.codes>"]
 repository = "https://github.com/ykrx/intelliterm"
 readme = "README.md"
 license = "LICENSE.txt"
 packages = [{ include = "intelliterm" }]
 
@@ -16,14 +16,16 @@
 prompt-toolkit = "^3.0.38"
 tiktoken = "^0.4.0"
 setuptools = "^68.0.0"
 pyperclip = "^1.8.2"
 pygments = "^2.15.1"
 rich = "^13.4.2"
 emoji = "^2.8.0"
+aiohttp = "^3.9.0"
+anthropic = "^0.23.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 mypy = "^1.4.1"
 
 [build-system]
```

### Comparing `intelliterm-0.4.1/PKG-INFO` & `intelliterm-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: intelliterm
-Version: 0.4.1
+Version: 0.5.0
 Summary: Chat with AI from your terminal!
 Home-page: https://github.com/ykrx/intelliterm
 License: LICENSE.txt
 Author: Yulian Kraynyak
 Author-email: yulian@yulian.codes
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.0,<4.0.0)
+Requires-Dist: anthropic (>=0.23.1,<0.24.0)
 Requires-Dist: emoji (>=2.8.0,<3.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pick (>=2.2.0,<3.0.0)
 Requires-Dist: platformdirs (>=3.8.0,<4.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
-Metadata-Version: 2.1 Name: intelliterm Version: 0.4.1 Summary: Chat with AI
+Metadata-Version: 2.1 Name: intelliterm Version: 0.5.0 Summary: Chat with AI
 from your terminal! Home-page: https://github.com/ykrx/intelliterm License:
 LICENSE.txt Author: Yulian Kraynyak Author-email: yulian@yulian.codes Requires-
 Python: >=3.11,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: emoji (>=2.8.0,<3.0.0) Requires-Dist:
-openai (>=0.27.8,<0.28.0) Requires-Dist: pick (>=2.2.0,<3.0.0) Requires-Dist:
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.0,<4.0.0) Requires-Dist: anthropic
+(>=0.23.1,<0.24.0) Requires-Dist: emoji (>=2.8.0,<3.0.0) Requires-Dist: openai
+(>=0.27.8,<0.28.0) Requires-Dist: pick (>=2.2.0,<3.0.0) Requires-Dist:
 platformdirs (>=3.8.0,<4.0.0) Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0) Requires-Dist: pyperclip
 (>=1.8.2,<2.0.0) Requires-Dist: rich (>=13.4.2,<14.0.0) Requires-Dist:
 setuptools (>=68.0.0,<69.0.0) Requires-Dist: tiktoken (>=0.4.0,<0.5.0) Project-
 URL: Repository, https://github.com/ykrx/intelliterm Description-Content-Type:
 text/markdown # Intelliterm > Chat with AI from your terminal! > **Note**
 > This is a side project I occasionally work on in my free time, [report]
```

