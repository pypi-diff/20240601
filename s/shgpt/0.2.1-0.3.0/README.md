# Comparing `tmp/shgpt-0.2.1.tar.gz` & `tmp/shgpt-0.3.0.tar.gz`

## Comparing `shgpt-0.2.1.tar` & `shgpt-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 shgpt-0.2.1/Makefile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/__main__.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/app.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/version.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/api/ollama.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/tui/app.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/tui/app.tcss
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/utils/common.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/utils/conf.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 shgpt-0.2.1/shgpt/utils/http.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 shgpt-0.2.1/.gitignore
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 shgpt-0.2.1/README.md
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 shgpt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 shgpt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 shgpt-0.3.0/Makefile
+-rw-r--r--   0        0        0    83463 2020-02-02 00:00:00.000000 shgpt-0.3.0/roles.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/__main__.py
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/app.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/version.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/api/history.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/api/ollama.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/tui/app.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/tui/app.tcss
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/utils/common.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/utils/conf.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/utils/http.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 shgpt-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 shgpt-0.3.0/README.md
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 shgpt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 shgpt-0.3.0/PKG-INFO
```

### Comparing `shgpt-0.2.1/shgpt/app.py` & `shgpt-0.3.0/shgpt/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,122 @@
-import argparse, sys
-from os import environ, makedirs
-from smartinput import sinput, Shell, Fore
+import argparse, sys, readline
+from os import makedirs
 from .api.ollama import Ollama
 from .version import __version__
 from .utils.conf import *
 from .utils.common import *
 from .tui.app import ShellGPTApp
 from functools import partial
 
-
-def repl_handler(llm, prompt, shell):
-    if prompt != "":
-        try:
-            for r in llm.generate(prompt):
-                print(r, end='')
-            print()
-        except Exception as e:
-            shell.out(f"Error when infer: ${e}")
+def init_app():
+    print(f'Create {CONF_PATH}...')
+    makedirs(CONF_PATH, exist_ok=True)
+
+def read_action(cmd):
+    if IS_TTY:
+        action = input("(E)xecute, (Y)ank or (C)ontinue(default): ")
+        action = action.upper()
+        if action == "E":
+            print(execute_cmd(cmd))
+        elif action == "Y":
+            copy_text(cmd)
 
 
 class ShellGPT(object):
     def __init__(self, url, model, role, timeout):
-        makedirs(CONF_PATH, exist_ok=True)
+        self.role = role
         self.llm = Ollama(url, model, role, timeout)
 
-    def tui(self):
-        app = ShellGPTApp(self.llm)
+    def tui(self, initial_prompt):
+        app = ShellGPTApp(self.llm, initial_prompt)
         app.run()
 
-    def repl(self):
+    def repl(self, initial_prompt):
         print(r'''
 __      __   _                    _         ___ _        _ _  ___ ___ _____
 \ \    / /__| |__ ___ _ __  ___  | |_ ___  / __| |_  ___| | |/ __| _ \_   _|
  \ \/\/ / -_) / _/ _ \ '  \/ -_) |  _/ _ \ \__ \ ' \/ -_) | | (_ |  _/ | |
   \_/\_/\___|_\__\___/_|_|_\___|  \__\___/ |___/_||_\___|_|_|\___|_|   |_|
 ''')
-        shell = Shell(callback=partial(repl_handler, self.llm), intitle="shellgpt> ", outtitle="", alertcolor=Fore.RED, exiton="exit")
-        shell.start()
-        return
+        self.infer(initial_prompt)
+        while True:
+            prompt = input("> ")
+            if 'exit' == prompt:
+                sys.exit(0)
+
+            self.infer(prompt)
+
 
     def infer(self, prompt):
-        for r in self.llm.generate(prompt):
-            print(r, end='')
-        print()
+        if prompt == "":
+            return
+
+        buf = ''
+        try:
+            for r in self.llm.generate(prompt):
+                buf += r
+                print(r, end='')
+
+            print()
+            if self.role == 'shell':
+                read_action(buf)
+        except Exception as e:
+            print(f"Error when infer: ${e}")
 
 
 def main():
     prog = sys.argv[0]
     parser = argparse.ArgumentParser(
         prog=prog,
         description='Make Shell easy to use with power of LLM!')
     parser.add_argument('-V', '--version', action='version', version='%(prog)s ' + __version__)
     parser.add_argument('-s', '--shell', action='store_true', help='Infer shell command')
     parser.add_argument('-r', '--role', default='default', help='System role message')
     parser.add_argument('-l', '--repl', action='store_true', help='Start interactive REPL')
+    parser.add_argument('-t', '--tui', action='store_true', help='Start TUI')
+    parser.add_argument('--init', action='store_true', help='Init config')
     parser.add_argument('--timeout', type=int, help='Timeout for each inference request', default=INFER_TIMEOUT)
     parser.add_argument('--ollama-url', default=OLLAMA_URL, help='Ollama URL')
     parser.add_argument('-m', '--ollama-model', default='llama3', help='Ollama model')
     parser.add_argument('-v', '--verbose', action='store_true', help='verbose mode')
     parser.add_argument('prompt', metavar='<prompt>', nargs='*')
     args = parser.parse_args()
     set_verbose(args.verbose)
 
+    if args.init:
+        init_app()
+        sys.exit(0)
+
     sin = read_stdin()
     prompt = ' '.join(args.prompt)
     if sin is not None:
         prompt = f'{sin}\n\n{prompt}'
 
+    if args.repl:
+        app_mode = AppMode.REPL
+    elif args.tui:
+        app_mode = AppMode.TUI
+    else:
+        app_mode = AppMode.TUI if len(prompt) == 0 else AppMode.Direct
+
     role = args.role
-    if args.shell:
-        role = 'shell'
-    elif args.repl:
-        pass
-    elif len(prompt) == 0:
-        # tui default to shell role
+    # tui default to shell role
+    if args.shell or app_mode == AppMode.TUI:
         role = 'shell'
 
-    sg = ShellGPT(args.ollama_url, args.ollama_model, role, args.timeout)
-    if args.repl:
-        sg.repl()
-    elif len(prompt) == 0:
-        sg.tui()
-    else:
-        sg.infer(prompt)
+    if role not in ROLE_CONTENT:
+        try:
+            load_roles_from_config()
+        except Exception as e:
+            debug_print(f"Error when load roles: ${e}")
 
+    if role not in ROLE_CONTENT:
+        print(f"Error: role '{role}' not found in config!")
+        sys.exit(1)
 
-if __name__ == '__main__':
-    main()
+    sg = ShellGPT(args.ollama_url, args.ollama_model, role, args.timeout)
+    if app_mode == AppMode.Direct:
+        sg.infer(prompt)
+    elif app_mode == AppMode.TUI:
+        sg.tui(prompt)
+    else:
+        sg.repl(prompt)
```

### Comparing `shgpt-0.2.1/shgpt/tui/app.py` & `shgpt-0.3.0/shgpt/tui/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from textual.app import App, ComposeResult
 from textual.widgets import Header, Footer, Static, TextArea, Button
 from typing import Optional
-import pyperclip
-import subprocess
 from ..utils.common import *
-from ..utils.common import debug_print
 
 class PromptInput(Static):
+    def __init__(self, prompt):
+        self.initial_prompt = prompt
+        super().__init__()
+
     def compose(self) -> ComposeResult:
-        yield TextArea(id="prompt_input")
+        yield TextArea(self.initial_prompt, id="prompt_input")
 
 
 class AnswerOutput(Static):
     def compose(self) -> ComposeResult:
         yield TextArea(id="answer_output")
 
 
@@ -44,23 +45,24 @@
     BINDINGS = [
         ("ctrl+j", "infer", "Infer answer"),
         ("ctrl+d", "toggle_dark", "Toggle dark mode"),
         ("ctrl+y", "Yank", "Yank code block"),
         ("ctrl+r", "run", "Run code block"),
     ]
 
-    def __init__(self, llm):
+    def __init__(self, llm, initial_prompt):
         self.llm = llm
         self.has_inflight_req = False
+        self.initial_prompt = initial_prompt
         super().__init__()
 
     def compose(self) -> ComposeResult:
         """Create child widgets for the app."""
         yield Header()
-        yield PromptInput()
+        yield PromptInput(self.initial_prompt)
         yield AnswerOutput()
         yield ButtonDispatch(
             lambda: self.action_copy(),
             lambda: self.action_run(),
         )
         yield CommandOutput()
         yield Footer()
@@ -110,20 +112,19 @@
         answer_output.load_text(buf)
 
     def action_copy(self) -> None:
         text = self.get_answer_output()
         if text is None:
             return
 
-        cmd = text
-        pyperclip.copy(cmd)
+        copy_text(text)
 
 
     def action_run(self) -> None:
         text = self.get_answer_output()
         if text is None:
             return
 
         cmd = text
-        output = subprocess.getoutput(cmd)
+        output = execute_cmd(cmd)
         command_output = self.query_one("#command_output")
         command_output.load_text(output)
```

### Comparing `shgpt-0.2.1/shgpt/utils/common.py` & `shgpt-0.3.0/shgpt/utils/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from enum import Enum
 from typing import Optional
 from datetime import datetime
-import re, platform, os, fileinput, sys
+import re, platform, os, subprocess, sys
+import pyperclip
 
 IS_VERBOSE = False
-TEST_PROMPT = "tell me how to get current disk usage by shell command"
 OS_NAME = platform.system()
+IS_TTY = sys.stdin.isatty()
 
 def get_shell_type():
     if OS_NAME in ("Windows", "nt"):
-        is_powershell = len(getenv("PSModulePath", "").split(pathsep)) >= 3
+        is_powershell = len(os.getenv("PSModulePath", "").split(os.pathsep)) >= 3
         return "powershell.exe" if is_powershell else "cmd.exe"
     return os.path.basename(os.getenv("SHELL", "/bin/sh"))
 
 SHELL = get_shell_type()
 
 def set_verbose(v):
     global IS_VERBOSE
@@ -35,15 +36,29 @@
 
 
 def now_ms():
     return int(datetime.now().timestamp() * 1000)
 
 
 def read_stdin():
-    if sys.stdin.isatty() is False:
+    if IS_TTY:
+        return None
+    else:
         buf = ''
         for line in sys.stdin:
             buf += line
 
         return buf
-    else:
-        return None
+
+
+def copy_text(text):
+    pyperclip.copy(text)
+
+
+def execute_cmd(cmd):
+    return subprocess.getoutput(cmd)
+
+
+class AppMode(Enum):
+    Direct = 1,
+    TUI = 2,
+    REPL = 3,
```

### Comparing `shgpt-0.2.1/README.md` & `shgpt-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 # ShellGPT
 
 [![](https://img.shields.io/pypi/v/shgpt)](https://pypi.org/project/shgpt/)
 
-Generate shell command you want with power of LLM, without leaving your terminal!
+Chat with LLM for anything you like, be it shell generator, story teller, linux-terminal, etc. All without leaving your terminal!
 
 # Install
 ```
-pip install shgpt
+pip install -U shgpt
 ```
 
-This will install two commands: `sg` and `shgpt`.
+This will install two commands: `sg` and `shgpt`, which are identical.
+
+After install, use `sg --init` to create required directories(mainly `~/.shellgpt`).
 
 # Usage
 
 ShellGPT has three modes to use:
-- Direct mode, `sg [question]` or `echo question | sg`.
-- `sg`, Enter TUI mode, tailored for infer shell command
-- `sg -l`, Enter an interactive REPL.
+- Direct mode, `sg [question]` or pipeline like `echo question | sg`.
+- TUI mode, `sg`, tailored for infer shell command.
+- REPL mode, `sg -l`, chat with LLM.
+
+See [conf.py](https://github.com/jiacai2050/shellgpt/blob/main/shgpt/utils/conf.py) for configs.
+
+## TUI
+
+There are some key bindings to use in TUI: option
+- `ctrl+j`, Infer answer
+- `ctrl+r`, Run command
+- `ctrl+y`, Yank command
 
-See [conf.py](shgpt/utils/conf.py) for configs.
+![TUI screenshot](https://github.com/jiacai2050/shellgpt/raw/main/assets/shellgpt-tui.jpg)
 
 ## Role
 
 There are some built-in roles in shellgpt:
 - `default`, used for ask general questions
 - `code`, used for ask programming questions
 - `shell`, used for infer shell command
-- `cm`, used for generate git commit message
+- `cm`, used for generate git commit message, like `git diff | sg -r cm`
 
-```bash
-git diff | sg -r cm
-```
-
-Users can provide their own role with `-r` option.
+Users can define their own roles in `~/.shellgpt/roles.json`, it a JSON map with
+- key being role name and
+- value being role content
 
-## TUI generate git commit message
+Or you can just copy [roles.json](https://github.com/jiacai2050/shellgpt/blob/main/roles.json) to play with, it's generated from [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts/blob/main/prompts.csv).
 
-Users can provide their own role with `-r`There are some key bindings to use in TUI: option
-- `ctrl+j`, Infer answer
-- `ctrl+r`, Run command
-- `ctrl+y`, Yank command
+```bash
+$ shgpt -r linux-terminal pwd
+/home/user
 
-![TUI screenshot](./assets/shellgpt-tui.jpg)
+$ shgpt -r javascript-console 0.1 + 0.2
+0.3
 
+```
 # Requirements
 - [Ollama](https://ollama.com/), you need to download models before try shellgpt.
 
 # License
 
 [GPL-3.0](https://opensource.org/license/GPL-3.0)
```

### Comparing `shgpt-0.2.1/pyproject.toml` & `shgpt-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "shgpt"
 dynamic = ["version"]
 authors = [{name = "Jiacai Liu", email="dev@liujiacai.net"}]
-description = "Generate shell command you want with power of LLM, without leaving your terminal."
+description = "Chat with LLM for anything you like, be it shell generator, story teller, linux-terminal, etc. All without leaving your terminal!"
 readme = "README.md"
 keywords = ["llm", "shell", "gpt"]
 license = "GPL-3.0"
 dependencies = [
   "requests",
-  "smartinput",
   "pyperclip",
   "textual",
 ]
 
 [project.urls]
 Repository = "https://github.com/jiacai2050/shellgpt"
 Issues = "https://github.com/jiacai2050/shellgpt/issues"
@@ -30,14 +29,15 @@
 
 [tool.hatch.build.targets.sdist]
 include = [
   "shgpt",
   "pyproject.toml",
   "README.md",
   "Makefile",
+  "roles.json",
 ]
 
 [tool.hatch.build.targets.wheel]
 include = [
   "shgpt",
 ]
```

### Comparing `shgpt-0.2.1/PKG-INFO` & `shgpt-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,75 @@
 Metadata-Version: 2.3
 Name: shgpt
-Version: 0.2.1
-Summary: Generate shell command you want with power of LLM, without leaving your terminal.
+Version: 0.3.0
+Summary: Chat with LLM for anything you like, be it shell generator, story teller, linux-terminal, etc. All without leaving your terminal!
 Project-URL: Repository, https://github.com/jiacai2050/shellgpt
 Project-URL: Issues, https://github.com/jiacai2050/shellgpt/issues
 Author-email: Jiacai Liu <dev@liujiacai.net>
 License-Expression: GPL-3.0
 Keywords: gpt,llm,shell
 Requires-Dist: pyperclip
 Requires-Dist: requests
-Requires-Dist: smartinput
 Requires-Dist: textual
 Description-Content-Type: text/markdown
 
 # ShellGPT
 
 [![](https://img.shields.io/pypi/v/shgpt)](https://pypi.org/project/shgpt/)
 
-Generate shell command you want with power of LLM, without leaving your terminal!
+Chat with LLM for anything you like, be it shell generator, story teller, linux-terminal, etc. All without leaving your terminal!
 
 # Install
 ```
-pip install shgpt
+pip install -U shgpt
 ```
 
-This will install two commands: `sg` and `shgpt`.
+This will install two commands: `sg` and `shgpt`, which are identical.
+
+After install, use `sg --init` to create required directories(mainly `~/.shellgpt`).
 
 # Usage
 
 ShellGPT has three modes to use:
-- Direct mode, `sg [question]` or `echo question | sg`.
-- `sg`, Enter TUI mode, tailored for infer shell command
-- `sg -l`, Enter an interactive REPL.
+- Direct mode, `sg [question]` or pipeline like `echo question | sg`.
+- TUI mode, `sg`, tailored for infer shell command.
+- REPL mode, `sg -l`, chat with LLM.
+
+See [conf.py](https://github.com/jiacai2050/shellgpt/blob/main/shgpt/utils/conf.py) for configs.
+
+## TUI
+
+There are some key bindings to use in TUI: option
+- `ctrl+j`, Infer answer
+- `ctrl+r`, Run command
+- `ctrl+y`, Yank command
 
-See [conf.py](shgpt/utils/conf.py) for configs.
+![TUI screenshot](https://github.com/jiacai2050/shellgpt/raw/main/assets/shellgpt-tui.jpg)
 
 ## Role
 
 There are some built-in roles in shellgpt:
 - `default`, used for ask general questions
 - `code`, used for ask programming questions
 - `shell`, used for infer shell command
-- `cm`, used for generate git commit message
+- `cm`, used for generate git commit message, like `git diff | sg -r cm`
 
-```bash
-git diff | sg -r cm
-```
-
-Users can provide their own role with `-r` option.
+Users can define their own roles in `~/.shellgpt/roles.json`, it a JSON map with
+- key being role name and
+- value being role content
 
-## TUI generate git commit message
+Or you can just copy [roles.json](https://github.com/jiacai2050/shellgpt/blob/main/roles.json) to play with, it's generated from [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts/blob/main/prompts.csv).
 
-Users can provide their own role with `-r`There are some key bindings to use in TUI: option
-- `ctrl+j`, Infer answer
-- `ctrl+r`, Run command
-- `ctrl+y`, Yank command
+```bash
+$ shgpt -r linux-terminal pwd
+/home/user
 
-![TUI screenshot](./assets/shellgpt-tui.jpg)
+$ shgpt -r javascript-console 0.1 + 0.2
+0.3
 
+```
 # Requirements
 - [Ollama](https://ollama.com/), you need to download models before try shellgpt.
 
 # License
 
 [GPL-3.0](https://opensource.org/license/GPL-3.0)
```

