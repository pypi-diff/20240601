# Comparing `tmp/pr_pilot_cli-1.4.0.tar.gz` & `tmp/pr_pilot_cli-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.4.0.tar", last modified: Fri May 31 23:56:03 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.4.1.tar", last modified: Sat Jun  1 01:03:41 2024, max compression
```

## Comparing `pr_pilot_cli-1.4.0.tar` & `pr_pilot_cli-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:56:03.765395 pr_pilot_cli-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-31 23:56:03.765395 pr_pilot_cli-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:56:03.761394 pr_pilot_cli-1.4.0/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/detect_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/status_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:56:03.765395 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 23:56:03.765395 pr_pilot_cli-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:03:41.043411 pr_pilot_cli-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 01:03:41.043411 pr_pilot_cli-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:03:41.043411 pr_pilot_cli-1.4.1/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/detect_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/status_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:03:41.043411 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:03:41.047412 pr_pilot_cli-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/setup.py
```

### Comparing `pr_pilot_cli-1.4.0/LICENSE` & `pr_pilot_cli-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.0/PKG-INFO` & `pr_pilot_cli-1.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.4.0
+Version: 1.4.1
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,29 +40,35 @@
 Open a terminal and `ls` into a repository you have [installed](https://github.com/apps/pr-pilot-ai/installations/new) PR Pilot.
 
 ### Examples
 
 You can run a prompt directly on the command line:
 
 ```bash
-pilot --raw "translate the README into German" > README_German.md
+pilot -o README_German.md "translate the README into German"
 ```
 
 Generate code quickly:
 
 ```bash
 pilot -o test_utils.py --code "Write some unit tests for the utils.py file."
 ```
 
 Get an organized view of your Github issues:
 
 ```bash
 pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
 ```
 
+Get some advice on your code:
+
+```bash
+pilot "The 'TaskEngine' class is too complex. Read it and suggest refactoring options."
+```
+
 Generate parts of your README with a [template](./prompts/README.md.jinja2):
 
 ```bash
 pilot --direct -f prompts/README.md.jinja2 -o README.md
 ```
 
 For more examples, check out the [prompts](./prompts) directory in this repository.
@@ -87,14 +93,20 @@
   -o, --output PATH         Output file for the result.
   --model TEXT              GPT model to use.
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
+## Installation
+
+I't simple:
+1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
+2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
+
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.0 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.1 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
@@ -10,30 +10,34 @@
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
 [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
 powerful, reusable commands that can be executed by PR Pilot. ## Usage Open a
 terminal and `ls` into a repository you have [installed](https://github.com/
 apps/pr-pilot-ai/installations/new) PR Pilot. ### Examples You can run a prompt
-directly on the command line: ```bash pilot --raw "translate the README into
-German" > README_German.md ``` Generate code quickly: ```bash pilot -
-o test_utils.py --code "Write some unit tests for the utils.py file." ``` Get
-an organized view of your Github issues: ```bash pilot "Find all open Github
-issues labeled as 'bug', categorize and prioritize them" ``` Generate parts of
-your README with a [template](./prompts/README.md.jinja2): ```bash pilot --
-direct -f prompts/README.md.jinja2 -o README.md ``` For more examples, check
-out the [prompts](./prompts) directory in this repository. ### Options and
-Parameters You can change the default settings with parameters and options:
-```bash Usage: python -m cli.cli [OPTIONS] [PROMPT]... Options: --wait / --no-
-wait Wait for the result. --repo TEXT Github repository in the format owner/
-repo. --spinner / --no-spinner Display a loading indicator --quiet No pretty-
-print, no status indicator or messages. --cheap Use the cheapest GPT model
-(gpt-3.5-turbo) --code Optimize prompt and settings for generating code -f, --
-file PATH Load prompt from a template file. --direct Do not feed the rendered
-template as a prompt into PR Pilot, but render it directly as output. -o, --
-output PATH Output file for the result. --model TEXT GPT model to use. --debug
-Display debug information. --help Show this message and exit. ``` ##
-Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
-Contributing Contributors are welcome to improve the CLI by submitting pull
-requests or reporting issues. For more details, check the project's GitHub
-repository. ## License The PR Pilot CLI is open-source software licensed under
-the GPL-3 license.
+directly on the command line: ```bash pilot -o README_German.md "translate the
+README into German" ``` Generate code quickly: ```bash pilot -o test_utils.py -
+-code "Write some unit tests for the utils.py file." ``` Get an organized view
+of your Github issues: ```bash pilot "Find all open Github issues labeled as
+'bug', categorize and prioritize them" ``` Get some advice on your code:
+```bash pilot "The 'TaskEngine' class is too complex. Read it and suggest
+refactoring options." ``` Generate parts of your README with a [template](./
+prompts/README.md.jinja2): ```bash pilot --direct -f prompts/README.md.jinja2 -
+o README.md ``` For more examples, check out the [prompts](./prompts) directory
+in this repository. ### Options and Parameters You can change the default
+settings with parameters and options: ```bash Usage: python -m cli.cli
+[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
+TEXT Github repository in the format owner/repo. --spinner / --no-spinner
+Display a loading indicator --quiet No pretty-print, no status indicator or
+messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
+prompt and settings for generating code -f, --file PATH Load prompt from a
+template file. --direct Do not feed the rendered template as a prompt into PR
+Pilot, but render it directly as output. -o, --output PATH Output file for the
+result. --model TEXT GPT model to use. --debug Display debug information. --
+help Show this message and exit. ``` ## Installation I't simple: 1. **[Install
+the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on
+your Github repository 2. **[Generate an API key](https://app.pr-pilot.ai/
+dashboard/api-keys/)** in the dashboard ## Configuration The configuration file
+is located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
+improve the CLI by submitting pull requests or reporting issues. For more
+details, check the project's GitHub repository. ## License The PR Pilot CLI is
+open-source software licensed under the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.4.0/README.md` & `pr_pilot_cli-1.4.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,29 +23,35 @@
 Open a terminal and `ls` into a repository you have [installed](https://github.com/apps/pr-pilot-ai/installations/new) PR Pilot.
 
 ### Examples
 
 You can run a prompt directly on the command line:
 
 ```bash
-pilot --raw "translate the README into German" > README_German.md
+pilot -o README_German.md "translate the README into German"
 ```
 
 Generate code quickly:
 
 ```bash
 pilot -o test_utils.py --code "Write some unit tests for the utils.py file."
 ```
 
 Get an organized view of your Github issues:
 
 ```bash
 pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
 ```
 
+Get some advice on your code:
+
+```bash
+pilot "The 'TaskEngine' class is too complex. Read it and suggest refactoring options."
+```
+
 Generate parts of your README with a [template](./prompts/README.md.jinja2):
 
 ```bash
 pilot --direct -f prompts/README.md.jinja2 -o README.md
 ```
 
 For more examples, check out the [prompts](./prompts) directory in this repository.
@@ -70,14 +76,20 @@
   -o, --output PATH         Output file for the result.
   --model TEXT              GPT model to use.
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
+## Installation
+
+I't simple:
+1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
+2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
+
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
 
 ## License
```

#### html2text {}

```diff
@@ -3,30 +3,34 @@
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
 [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
 powerful, reusable commands that can be executed by PR Pilot. ## Usage Open a
 terminal and `ls` into a repository you have [installed](https://github.com/
 apps/pr-pilot-ai/installations/new) PR Pilot. ### Examples You can run a prompt
-directly on the command line: ```bash pilot --raw "translate the README into
-German" > README_German.md ``` Generate code quickly: ```bash pilot -
-o test_utils.py --code "Write some unit tests for the utils.py file." ``` Get
-an organized view of your Github issues: ```bash pilot "Find all open Github
-issues labeled as 'bug', categorize and prioritize them" ``` Generate parts of
-your README with a [template](./prompts/README.md.jinja2): ```bash pilot --
-direct -f prompts/README.md.jinja2 -o README.md ``` For more examples, check
-out the [prompts](./prompts) directory in this repository. ### Options and
-Parameters You can change the default settings with parameters and options:
-```bash Usage: python -m cli.cli [OPTIONS] [PROMPT]... Options: --wait / --no-
-wait Wait for the result. --repo TEXT Github repository in the format owner/
-repo. --spinner / --no-spinner Display a loading indicator --quiet No pretty-
-print, no status indicator or messages. --cheap Use the cheapest GPT model
-(gpt-3.5-turbo) --code Optimize prompt and settings for generating code -f, --
-file PATH Load prompt from a template file. --direct Do not feed the rendered
-template as a prompt into PR Pilot, but render it directly as output. -o, --
-output PATH Output file for the result. --model TEXT GPT model to use. --debug
-Display debug information. --help Show this message and exit. ``` ##
-Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
-Contributing Contributors are welcome to improve the CLI by submitting pull
-requests or reporting issues. For more details, check the project's GitHub
-repository. ## License The PR Pilot CLI is open-source software licensed under
-the GPL-3 license.
+directly on the command line: ```bash pilot -o README_German.md "translate the
+README into German" ``` Generate code quickly: ```bash pilot -o test_utils.py -
+-code "Write some unit tests for the utils.py file." ``` Get an organized view
+of your Github issues: ```bash pilot "Find all open Github issues labeled as
+'bug', categorize and prioritize them" ``` Get some advice on your code:
+```bash pilot "The 'TaskEngine' class is too complex. Read it and suggest
+refactoring options." ``` Generate parts of your README with a [template](./
+prompts/README.md.jinja2): ```bash pilot --direct -f prompts/README.md.jinja2 -
+o README.md ``` For more examples, check out the [prompts](./prompts) directory
+in this repository. ### Options and Parameters You can change the default
+settings with parameters and options: ```bash Usage: python -m cli.cli
+[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
+TEXT Github repository in the format owner/repo. --spinner / --no-spinner
+Display a loading indicator --quiet No pretty-print, no status indicator or
+messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
+prompt and settings for generating code -f, --file PATH Load prompt from a
+template file. --direct Do not feed the rendered template as a prompt into PR
+Pilot, but render it directly as output. -o, --output PATH Output file for the
+result. --model TEXT GPT model to use. --debug Display debug information. --
+help Show this message and exit. ``` ## Installation I't simple: 1. **[Install
+the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on
+your Github repository 2. **[Generate an API key](https://app.pr-pilot.ai/
+dashboard/api-keys/)** in the dashboard ## Configuration The configuration file
+is located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
+improve the CLI by submitting pull requests or reporting issues. For more
+details, check the project's GitHub repository. ## License The PR Pilot CLI is
+open-source software licensed under the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.4.0/cli/cli.py` & `pr_pilot_cli-1.4.1/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.0/cli/detect_repository.py` & `pr_pilot_cli-1.4.1/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.0/cli/prompt_template.py` & `pr_pilot_cli-1.4.1/cli/prompt_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import os
 import subprocess
-import time
 
 import click
 import jinja2
 from pr_pilot.util import create_task
-from yaspin import yaspin
 
 from cli.task_handler import TaskHandler
 
 
-
 def sh(shell_command, status):
     status.update(f"Running shell command: {shell_command}")
     try:
         process = subprocess.Popen(shell_command.split(), stdout=subprocess.PIPE)
         output, error = process.communicate()
         status.success()
         return output.decode('utf-8')
@@ -43,18 +40,18 @@
         self.model = model
         self.status = status
 
     def render(self):
 
         def subtask(prompt, status):
             try:
-                status.update("Creating new task")
+                status.update("Creating sub-task ...")
                 task = create_task(self.repo, prompt, log=False, gpt_model=self.model)
                 task_handler = TaskHandler(task, status)
-                return task_handler.wait_for_result()
+                return task_handler.wait_for_result(quiet=True)
             except Exception as e:
                 return f"Error: {e}"
 
         env = jinja2.Environment(loader=jinja2.FileSystemLoader(os.getcwd()))
         env.globals.update(env=read_env_var)
         env.globals.update(subtask=wrap_function_with_status(subtask, self.status))
         env.globals.update(sh=wrap_function_with_status(sh, self.status))
```

### Comparing `pr_pilot_cli-1.4.0/cli/status_indicator.py` & `pr_pilot_cli-1.4.1/cli/status_indicator.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.0/cli/task_handler.py` & `pr_pilot_cli-1.4.1/cli/task_handler.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.4.0
+Version: 1.4.1
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,29 +40,35 @@
 Open a terminal and `ls` into a repository you have [installed](https://github.com/apps/pr-pilot-ai/installations/new) PR Pilot.
 
 ### Examples
 
 You can run a prompt directly on the command line:
 
 ```bash
-pilot --raw "translate the README into German" > README_German.md
+pilot -o README_German.md "translate the README into German"
 ```
 
 Generate code quickly:
 
 ```bash
 pilot -o test_utils.py --code "Write some unit tests for the utils.py file."
 ```
 
 Get an organized view of your Github issues:
 
 ```bash
 pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
 ```
 
+Get some advice on your code:
+
+```bash
+pilot "The 'TaskEngine' class is too complex. Read it and suggest refactoring options."
+```
+
 Generate parts of your README with a [template](./prompts/README.md.jinja2):
 
 ```bash
 pilot --direct -f prompts/README.md.jinja2 -o README.md
 ```
 
 For more examples, check out the [prompts](./prompts) directory in this repository.
@@ -87,14 +93,20 @@
   -o, --output PATH         Output file for the result.
   --model TEXT              GPT model to use.
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
+## Installation
+
+I't simple:
+1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
+2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
+
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.0 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.1 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
@@ -10,30 +10,34 @@
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
 [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
 powerful, reusable commands that can be executed by PR Pilot. ## Usage Open a
 terminal and `ls` into a repository you have [installed](https://github.com/
 apps/pr-pilot-ai/installations/new) PR Pilot. ### Examples You can run a prompt
-directly on the command line: ```bash pilot --raw "translate the README into
-German" > README_German.md ``` Generate code quickly: ```bash pilot -
-o test_utils.py --code "Write some unit tests for the utils.py file." ``` Get
-an organized view of your Github issues: ```bash pilot "Find all open Github
-issues labeled as 'bug', categorize and prioritize them" ``` Generate parts of
-your README with a [template](./prompts/README.md.jinja2): ```bash pilot --
-direct -f prompts/README.md.jinja2 -o README.md ``` For more examples, check
-out the [prompts](./prompts) directory in this repository. ### Options and
-Parameters You can change the default settings with parameters and options:
-```bash Usage: python -m cli.cli [OPTIONS] [PROMPT]... Options: --wait / --no-
-wait Wait for the result. --repo TEXT Github repository in the format owner/
-repo. --spinner / --no-spinner Display a loading indicator --quiet No pretty-
-print, no status indicator or messages. --cheap Use the cheapest GPT model
-(gpt-3.5-turbo) --code Optimize prompt and settings for generating code -f, --
-file PATH Load prompt from a template file. --direct Do not feed the rendered
-template as a prompt into PR Pilot, but render it directly as output. -o, --
-output PATH Output file for the result. --model TEXT GPT model to use. --debug
-Display debug information. --help Show this message and exit. ``` ##
-Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
-Contributing Contributors are welcome to improve the CLI by submitting pull
-requests or reporting issues. For more details, check the project's GitHub
-repository. ## License The PR Pilot CLI is open-source software licensed under
-the GPL-3 license.
+directly on the command line: ```bash pilot -o README_German.md "translate the
+README into German" ``` Generate code quickly: ```bash pilot -o test_utils.py -
+-code "Write some unit tests for the utils.py file." ``` Get an organized view
+of your Github issues: ```bash pilot "Find all open Github issues labeled as
+'bug', categorize and prioritize them" ``` Get some advice on your code:
+```bash pilot "The 'TaskEngine' class is too complex. Read it and suggest
+refactoring options." ``` Generate parts of your README with a [template](./
+prompts/README.md.jinja2): ```bash pilot --direct -f prompts/README.md.jinja2 -
+o README.md ``` For more examples, check out the [prompts](./prompts) directory
+in this repository. ### Options and Parameters You can change the default
+settings with parameters and options: ```bash Usage: python -m cli.cli
+[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
+TEXT Github repository in the format owner/repo. --spinner / --no-spinner
+Display a loading indicator --quiet No pretty-print, no status indicator or
+messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
+prompt and settings for generating code -f, --file PATH Load prompt from a
+template file. --direct Do not feed the rendered template as a prompt into PR
+Pilot, but render it directly as output. -o, --output PATH Output file for the
+result. --model TEXT GPT model to use. --debug Display debug information. --
+help Show this message and exit. ``` ## Installation I't simple: 1. **[Install
+the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on
+your Github repository 2. **[Generate an API key](https://app.pr-pilot.ai/
+dashboard/api-keys/)** in the dashboard ## Configuration The configuration file
+is located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
+improve the CLI by submitting pull requests or reporting issues. For more
+details, check the project's GitHub repository. ## License The PR Pilot CLI is
+open-source software licensed under the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.4.0/setup.py` & `pr_pilot_cli-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.4.0',
+    version='1.4.1',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

