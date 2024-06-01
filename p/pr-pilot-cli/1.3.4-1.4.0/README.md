# Comparing `tmp/pr_pilot_cli-1.3.4.tar.gz` & `tmp/pr_pilot_cli-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.3.4.tar", last modified: Fri May 31 01:00:33 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.4.0.tar", last modified: Fri May 31 23:56:03 2024, max compression
```

## Comparing `pr_pilot_cli-1.3.4.tar` & `pr_pilot_cli-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:00:33.877976 pr_pilot_cli-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-31 01:00:33.877976 pr_pilot_cli-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:00:33.873976 pr_pilot_cli-1.3.4/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/detect_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:00:33.877976 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:00:33.877976 pr_pilot_cli-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:56:03.765395 pr_pilot_cli-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-31 23:56:03.765395 pr_pilot_cli-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:56:03.761394 pr_pilot_cli-1.4.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/detect_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/status_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/cli/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:56:03.765395 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 23:56:03.000000 pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 23:56:03.765395 pr_pilot_cli-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-31 23:55:59.000000 pr_pilot_cli-1.4.0/setup.py
```

### Comparing `pr_pilot_cli-1.3.4/LICENSE` & `pr_pilot_cli-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.4/PKG-INFO` & `pr_pilot_cli-1.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.3.4
+Version: 1.4.0
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,115 +17,83 @@
 
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
   <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
-  <a href="https://docs.pr-pilot.ai">Documentation</a> | 
-  <a href="https://www.pr-pilot.ai/blog">Blog</a> | 
+  <a href="https://docs.pr-pilot.ai">Documentation</a> |
+  <a href="https://www.pr-pilot.ai/blog">Blog</a> |
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
 # PR Pilot CLI
 
 PR Pilot gives you a natural language interface for your Github projects.
 Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
 and Github issues.
 
-Using templates, you can create powerful, reusable commands that can be executed by PR Pilot. Here is how it works:
+Using [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create powerful,
+reusable commands that can be executed by PR Pilot.
 
-Write a template file:
-
-```markdown
-Take a look at our test results:
-
----
-{{ sh('pytest') }}
----
-
-Understand why the tests are failing by reading the relevant code files. 
-Give a short, concise, structured analysis of the test results.
-```
-
-Execute the file:
-
-`pilot -f analyze_test_results.md.jinja2`
-
-For more examples, check out the [prompts](./prompts) directory in this repository.
-
-### 
+## Usage
 
-## Installation
+Open a terminal and `ls` into a repository you have [installed](https://github.com/apps/pr-pilot-ai/installations/new) PR Pilot.
 
- > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
+### Examples
 
-To install the CLI, run the following command:
+You can run a prompt directly on the command line:
 
 ```bash
-pip install --upgrade pr-pilot-cli
+pilot --raw "translate the README into German" > README_German.md
 ```
 
-By default, the CLI will prompt you to input your API key if it is not already configured.
-
-## Usage
-
-After installation, open a terminal and `ls` into a repository you have installed PR Pilot in and talk to PR Pilot:
-
-### Examples
-
-Translate a file:
+Generate code quickly:
 
 ```bash
-pilot --raw "translate the README into German" > README_German.md
+pilot -o test_utils.py --code "Write some unit tests for the utils.py file."
 ```
 
-Let it write some unit tests:
+Get an organized view of your Github issues:
 
 ```bash
-pilot "Write some unit tests for the utils.py file."
+pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
 ```
 
-Find some information in your Github issues:
+Generate parts of your README with a [template](./prompts/README.md.jinja2):
 
 ```bash
-pilot "Do we have any open Github issues regarding the AuthenticationView class?"
+pilot --direct -f prompts/README.md.jinja2 -o README.md
 ```
 
-For more information, check out our [User Guide](https://docs.pr-pilot.ai/user_guide.html).
+For more examples, check out the [prompts](./prompts) directory in this repository.
 
 ### Options and Parameters
 
 You can change the default settings with parameters and options:
 
 ```bash
-Usage: pilot [OPTIONS] [PROMPT]...
+Usage: python -m cli.cli [OPTIONS] [PROMPT]...
 
 Options:
-  --wait / --no-wait  Wait for the result.
-  --repo TEXT         Github repository in the format owner/repo.
-  --chatty            Print more information.
-  --raw               For piping. No pretty-print, no status indicator.
-  --code              Disable formatting, enable RAW mode, use GPT-4 model.
-  -f, --file PATH     Load prompt from a template file.
-  --direct            Do not use the rendered template as a prompt for PR
-                      Pilot, but render it directly as output.
-  -o, --output PATH   Output file for the result.
-  --model TEXT        GPT model to use.
-  --debug             Display debug information.
-  --help              Show this message and exit.
-```
-
-
-## Features
-- **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
-- **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
-- **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
-- **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
+  --wait / --no-wait        Wait for the result.
+  --repo TEXT               Github repository in the format owner/repo.
+  --spinner / --no-spinner  Display a loading indicator
+  --quiet                   No pretty-print, no status indicator or messages.
+  --cheap                   Use the cheapest GPT model (gpt-3.5-turbo)
+  --code                    Optimize prompt and settings for generating code
+  -f, --file PATH           Load prompt from a template file.
+  --direct                  Do not feed the rendered template as a prompt into
+                            PR Pilot, but render it directly as output.
+  -o, --output PATH         Output file for the result.
+  --model TEXT              GPT model to use.
+  --debug                   Display debug information.
+  --help                    Show this message and exit.
 
+```
 
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
```

#### html2text {}

```diff
@@ -1,51 +1,39 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.4 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.0 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
-templates, you can create powerful, reusable commands that can be executed by
-PR Pilot. Here is how it works: Write a template file: ```markdown Take a look
-at our test results: --- {{ sh('pytest') }} --- Understand why the tests are
-failing by reading the relevant code files. Give a short, concise, structured
-analysis of the test results. ``` Execute the file: `pilot -
-f analyze_test_results.md.jinja2` For more examples, check out the [prompts](./
-prompts) directory in this repository. ### ## Installation > Make sure you have
-PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/
-installations/new) To install the CLI, run the following command: ```bash pip
-install --upgrade pr-pilot-cli ``` By default, the CLI will prompt you to input
-your API key if it is not already configured. ## Usage After installation, open
-a terminal and `ls` into a repository you have installed PR Pilot in and talk
-to PR Pilot: ### Examples Translate a file: ```bash pilot --raw "translate the
-README into German" > README_German.md ``` Let it write some unit tests:
-```bash pilot "Write some unit tests for the utils.py file." ``` Find some
-information in your Github issues: ```bash pilot "Do we have any open Github
-issues regarding the AuthenticationView class?" ``` For more information, check
-out our [User Guide](https://docs.pr-pilot.ai/user_guide.html). ### Options and
+[Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
+powerful, reusable commands that can be executed by PR Pilot. ## Usage Open a
+terminal and `ls` into a repository you have [installed](https://github.com/
+apps/pr-pilot-ai/installations/new) PR Pilot. ### Examples You can run a prompt
+directly on the command line: ```bash pilot --raw "translate the README into
+German" > README_German.md ``` Generate code quickly: ```bash pilot -
+o test_utils.py --code "Write some unit tests for the utils.py file." ``` Get
+an organized view of your Github issues: ```bash pilot "Find all open Github
+issues labeled as 'bug', categorize and prioritize them" ``` Generate parts of
+your README with a [template](./prompts/README.md.jinja2): ```bash pilot --
+direct -f prompts/README.md.jinja2 -o README.md ``` For more examples, check
+out the [prompts](./prompts) directory in this repository. ### Options and
 Parameters You can change the default settings with parameters and options:
-```bash Usage: pilot [OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for
-the result. --repo TEXT Github repository in the format owner/repo. --chatty
-Print more information. --raw For piping. No pretty-print, no status indicator.
---code Disable formatting, enable RAW mode, use GPT-4 model. -f, --file PATH
-Load prompt from a template file. --direct Do not use the rendered template as
-a prompt for PR Pilot, but render it directly as output. -o, --output PATH
-Output file for the result. --model TEXT GPT model to use. --debug Display
-debug information. --help Show this message and exit. ``` ## Features -
-**Configuration Management**: Automatically manages API key configuration by
-prompting the user to input their API key if not already configured. - **Task
-Creation**: Users can create tasks by specifying a repository and a prompt. The
-CLI handles task creation and optionally waits for the result. - **Result
-Retrieval**: If the `--wait` option is used, the CLI waits for the task to
-complete and displays the result directly in the terminal. - **Dashboard
-Link**: For tasks that are not awaited, the CLI provides a link to the task's
-dashboard for further monitoring. ## Configuration The configuration file is
-located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
-improve the CLI by submitting pull requests or reporting issues. For more
-details, check the project's GitHub repository. ## License The PR Pilot CLI is
-open-source software licensed under the GPL-3 license.
+```bash Usage: python -m cli.cli [OPTIONS] [PROMPT]... Options: --wait / --no-
+wait Wait for the result. --repo TEXT Github repository in the format owner/
+repo. --spinner / --no-spinner Display a loading indicator --quiet No pretty-
+print, no status indicator or messages. --cheap Use the cheapest GPT model
+(gpt-3.5-turbo) --code Optimize prompt and settings for generating code -f, --
+file PATH Load prompt from a template file. --direct Do not feed the rendered
+template as a prompt into PR Pilot, but render it directly as output. -o, --
+output PATH Output file for the result. --model TEXT GPT model to use. --debug
+Display debug information. --help Show this message and exit. ``` ##
+Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## License The PR Pilot CLI is open-source software licensed under
+the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.3.4/README.md` & `pr_pilot_cli-1.4.0/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,99 @@
+Metadata-Version: 2.1
+Name: pr-pilot-cli
+Version: 1.4.0
+Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
+Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
+Author: Marco Lamina
+Author-email: marco@pr-pilot.ai
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click==8.1.7
+Requires-Dist: pr-pilot==1.4.1
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: yaspin==3.0.2
+Requires-Dist: rich==13.7.1
+Requires-Dist: jinja2==3.1.4
+
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
   <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
-  <a href="https://docs.pr-pilot.ai">Documentation</a> | 
-  <a href="https://www.pr-pilot.ai/blog">Blog</a> | 
+  <a href="https://docs.pr-pilot.ai">Documentation</a> |
+  <a href="https://www.pr-pilot.ai/blog">Blog</a> |
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
 # PR Pilot CLI
 
 PR Pilot gives you a natural language interface for your Github projects.
 Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
 and Github issues.
 
-Using templates, you can create powerful, reusable commands that can be executed by PR Pilot. Here is how it works:
-
-Write a template file:
-
-```markdown
-Take a look at our test results:
-
----
-{{ sh('pytest') }}
----
-
-Understand why the tests are failing by reading the relevant code files. 
-Give a short, concise, structured analysis of the test results.
-```
-
-Execute the file:
+Using [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create powerful,
+reusable commands that can be executed by PR Pilot.
 
-`pilot -f analyze_test_results.md.jinja2`
-
-For more examples, check out the [prompts](./prompts) directory in this repository.
-
-### 
+## Usage
 
-## Installation
+Open a terminal and `ls` into a repository you have [installed](https://github.com/apps/pr-pilot-ai/installations/new) PR Pilot.
 
- > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
+### Examples
 
-To install the CLI, run the following command:
+You can run a prompt directly on the command line:
 
 ```bash
-pip install --upgrade pr-pilot-cli
+pilot --raw "translate the README into German" > README_German.md
 ```
 
-By default, the CLI will prompt you to input your API key if it is not already configured.
-
-## Usage
-
-After installation, open a terminal and `ls` into a repository you have installed PR Pilot in and talk to PR Pilot:
-
-### Examples
-
-Translate a file:
+Generate code quickly:
 
 ```bash
-pilot --raw "translate the README into German" > README_German.md
+pilot -o test_utils.py --code "Write some unit tests for the utils.py file."
 ```
 
-Let it write some unit tests:
+Get an organized view of your Github issues:
 
 ```bash
-pilot "Write some unit tests for the utils.py file."
+pilot "Find all open Github issues labeled as 'bug', categorize and prioritize them"
 ```
 
-Find some information in your Github issues:
+Generate parts of your README with a [template](./prompts/README.md.jinja2):
 
 ```bash
-pilot "Do we have any open Github issues regarding the AuthenticationView class?"
+pilot --direct -f prompts/README.md.jinja2 -o README.md
 ```
 
-For more information, check out our [User Guide](https://docs.pr-pilot.ai/user_guide.html).
+For more examples, check out the [prompts](./prompts) directory in this repository.
 
 ### Options and Parameters
 
 You can change the default settings with parameters and options:
 
 ```bash
-Usage: pilot [OPTIONS] [PROMPT]...
+Usage: python -m cli.cli [OPTIONS] [PROMPT]...
 
 Options:
-  --wait / --no-wait  Wait for the result.
-  --repo TEXT         Github repository in the format owner/repo.
-  --chatty            Print more information.
-  --raw               For piping. No pretty-print, no status indicator.
-  --code              Disable formatting, enable RAW mode, use GPT-4 model.
-  -f, --file PATH     Load prompt from a template file.
-  --direct            Do not use the rendered template as a prompt for PR
-                      Pilot, but render it directly as output.
-  -o, --output PATH   Output file for the result.
-  --model TEXT        GPT model to use.
-  --debug             Display debug information.
-  --help              Show this message and exit.
-```
-
-
-## Features
-- **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
-- **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
-- **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
-- **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
+  --wait / --no-wait        Wait for the result.
+  --repo TEXT               Github repository in the format owner/repo.
+  --spinner / --no-spinner  Display a loading indicator
+  --quiet                   No pretty-print, no status indicator or messages.
+  --cheap                   Use the cheapest GPT model (gpt-3.5-turbo)
+  --code                    Optimize prompt and settings for generating code
+  -f, --file PATH           Load prompt from a template file.
+  --direct                  Do not feed the rendered template as a prompt into
+                            PR Pilot, but render it directly as output.
+  -o, --output PATH         Output file for the result.
+  --model TEXT              GPT model to use.
+  --debug                   Display debug information.
+  --help                    Show this message and exit.
 
+```
 
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
```

#### html2text {}

```diff
@@ -1,44 +1,39 @@
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.0 Summary: CLI for PR
+Pilot, a text-to-task automation platform for Github. Home-page: https://
+github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
+marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
+pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
+Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI PR Pilot gives you a natural language interface for your Github
 projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
 fulfill tasks by interacting with your code base and Github issues. Using
-templates, you can create powerful, reusable commands that can be executed by
-PR Pilot. Here is how it works: Write a template file: ```markdown Take a look
-at our test results: --- {{ sh('pytest') }} --- Understand why the tests are
-failing by reading the relevant code files. Give a short, concise, structured
-analysis of the test results. ``` Execute the file: `pilot -
-f analyze_test_results.md.jinja2` For more examples, check out the [prompts](./
-prompts) directory in this repository. ### ## Installation > Make sure you have
-PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/
-installations/new) To install the CLI, run the following command: ```bash pip
-install --upgrade pr-pilot-cli ``` By default, the CLI will prompt you to input
-your API key if it is not already configured. ## Usage After installation, open
-a terminal and `ls` into a repository you have installed PR Pilot in and talk
-to PR Pilot: ### Examples Translate a file: ```bash pilot --raw "translate the
-README into German" > README_German.md ``` Let it write some unit tests:
-```bash pilot "Write some unit tests for the utils.py file." ``` Find some
-information in your Github issues: ```bash pilot "Do we have any open Github
-issues regarding the AuthenticationView class?" ``` For more information, check
-out our [User Guide](https://docs.pr-pilot.ai/user_guide.html). ### Options and
+[Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/), you can create
+powerful, reusable commands that can be executed by PR Pilot. ## Usage Open a
+terminal and `ls` into a repository you have [installed](https://github.com/
+apps/pr-pilot-ai/installations/new) PR Pilot. ### Examples You can run a prompt
+directly on the command line: ```bash pilot --raw "translate the README into
+German" > README_German.md ``` Generate code quickly: ```bash pilot -
+o test_utils.py --code "Write some unit tests for the utils.py file." ``` Get
+an organized view of your Github issues: ```bash pilot "Find all open Github
+issues labeled as 'bug', categorize and prioritize them" ``` Generate parts of
+your README with a [template](./prompts/README.md.jinja2): ```bash pilot --
+direct -f prompts/README.md.jinja2 -o README.md ``` For more examples, check
+out the [prompts](./prompts) directory in this repository. ### Options and
 Parameters You can change the default settings with parameters and options:
-```bash Usage: pilot [OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for
-the result. --repo TEXT Github repository in the format owner/repo. --chatty
-Print more information. --raw For piping. No pretty-print, no status indicator.
---code Disable formatting, enable RAW mode, use GPT-4 model. -f, --file PATH
-Load prompt from a template file. --direct Do not use the rendered template as
-a prompt for PR Pilot, but render it directly as output. -o, --output PATH
-Output file for the result. --model TEXT GPT model to use. --debug Display
-debug information. --help Show this message and exit. ``` ## Features -
-**Configuration Management**: Automatically manages API key configuration by
-prompting the user to input their API key if not already configured. - **Task
-Creation**: Users can create tasks by specifying a repository and a prompt. The
-CLI handles task creation and optionally waits for the result. - **Result
-Retrieval**: If the `--wait` option is used, the CLI waits for the task to
-complete and displays the result directly in the terminal. - **Dashboard
-Link**: For tasks that are not awaited, the CLI provides a link to the task's
-dashboard for further monitoring. ## Configuration The configuration file is
-located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
-improve the CLI by submitting pull requests or reporting issues. For more
-details, check the project's GitHub repository. ## License The PR Pilot CLI is
-open-source software licensed under the GPL-3 license.
+```bash Usage: python -m cli.cli [OPTIONS] [PROMPT]... Options: --wait / --no-
+wait Wait for the result. --repo TEXT Github repository in the format owner/
+repo. --spinner / --no-spinner Display a loading indicator --quiet No pretty-
+print, no status indicator or messages. --cheap Use the cheapest GPT model
+(gpt-3.5-turbo) --code Optimize prompt and settings for generating code -f, --
+file PATH Load prompt from a template file. --direct Do not feed the rendered
+template as a prompt into PR Pilot, but render it directly as output. -o, --
+output PATH Output file for the result. --model TEXT GPT model to use. --debug
+Display debug information. --help Show this message and exit. ``` ##
+Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## License The PR Pilot CLI is open-source software licensed under
+the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.3.4/cli/cli.py` & `pr_pilot_cli-1.4.0/cli/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 
 import click
 import yaml
-from pr_pilot.util import create_task, wait_for_result, get_task
+from pr_pilot.util import create_task
 from rich.console import Console
 from rich.markdown import Markdown
-from yaspin import yaspin
 
 from cli.detect_repository import detect_repository
-from cli.task_handler import TaskHandler
 from cli.prompt_template import PromptTemplate
+from cli.status_indicator import StatusIndicator
+from cli.task_handler import TaskHandler
 
 CONFIG_LOCATION = os.path.expanduser('~/.pr-pilot.yaml')
 CONFIG_API_KEY = "api_key"
-CODE_MODEL = "gpt-4"
+CODE_MODEL = "gpt-4o"
+CHEAP_MODEL = "gpt-3.5-turbo"
 POLL_INTERVAL = 2
 
 
 def load_config():
     """Load the configuration from the default location. If it doesn't exist,
     ask user to enter API key and save config."""
     if not os.path.exists(CONFIG_LOCATION):
@@ -35,69 +36,77 @@
         config = yaml.safe_load(f)
     return config
 
 
 @click.command()
 @click.option('--wait/--no-wait', is_flag=True, default=True, help='Wait for the result.')
 @click.option('--repo', help='Github repository in the format owner/repo.', required=False)
-@click.option('--chatty', is_flag=True, default=False, help='Print more information.')
-@click.option('--raw', is_flag=True, default=False, help='For piping. No pretty-print, no status indicator.')
-@click.option('--code', is_flag=True, default=False, help='Disable formatting, enable RAW mode, use GPT-4 model.')
+@click.option('--spinner/--no-spinner', is_flag=True, default=True, help='Display a loading indicator')
+@click.option('--quiet', is_flag=True, default=False, help='No pretty-print, no status indicator or messages.')
+@click.option('--cheap', is_flag=True, default=False, help=f'Use the cheapest GPT model ({CHEAP_MODEL})')
+@click.option('--code', is_flag=True, default=False, help='Optimize prompt and settings for generating code')
 @click.option('--file', '-f', type=click.Path(exists=True), help='Load prompt from a template file.')
 @click.option('--direct', is_flag=True, default=False,
-              help='Do not use the rendered template as a prompt for PR Pilot, but render it directly as output.')
+              help='Do not feed the rendered template as a prompt into PR Pilot, but render it directly as output.')
 @click.option('--output', '-o', type=click.Path(exists=False), help='Output file for the result.')
 @click.option('--model', help='GPT model to use.', default='gpt-4-turbo')
 @click.option('--debug', is_flag=True, default=False, help='Display debug information.')
 @click.argument('prompt', nargs=-1)
-def main(wait, repo, chatty, raw, code, file, direct, output, model, debug, prompt):
+def main(wait, repo, spinner, quiet, cheap, code, file, direct, output, model, debug, prompt):
     prompt = ' '.join(prompt)
     config = load_config()
     console = Console()
+    show_spinner = spinner and not quiet
+    status = StatusIndicator(spinner=show_spinner, messages=not quiet, console=console)
 
-    if debug:
-        chatty = True
     if not os.getenv("PR_PILOT_API_KEY"):
         os.environ["PR_PILOT_API_KEY"] = config[CONFIG_API_KEY]
     if not repo:
         # No repository provided, try to detect it
         repo = detect_repository()
     if not repo:
         # Current directory is not a git repository, see if there is a default repo in the config
         repo = config.get("default_repo")
     if not repo:
         console.print(f"No Github repository provided. Use --repo or set 'default_repo' in {CONFIG_LOCATION}.")
         return
     if file:
-        renderer = PromptTemplate(file, repo, model)
-        prompt = renderer.render(show_spinner=not raw)
+        status.start()
+        renderer = PromptTemplate(file, repo, model, status)
+        prompt = renderer.render()
     if not prompt:
         prompt = click.edit("", extension=".md")
         if not prompt:
             console.print("No prompt provided.")
             return
+    if cheap:
+        model = CHEAP_MODEL
     if code:
-        raw = True
         prompt += "\n\nONLY respond with the code, no other text. Do not wrap it in triple backticks."
-        model = CODE_MODEL
+        if not model:
+            model = CODE_MODEL
 
     if direct:
         # Do not send the prompt, just return it as the result
         if output:
             with open(output, "w") as f:
                 f.write(prompt)
-            console.print(Markdown(f"Rendered template `{file}` into `{output}`"))
+            if not quiet:
+                console.print(Markdown(f"Rendered template `{file}` into `{output}`"))
             return
-
+    status.start()
+    status.update("Creating new task")
     task = create_task(repo, prompt, log=False, gpt_model=model)
-
-    if not wait:
-        if chatty:
-            console.print(f"✅ Task created: https://app.pr-pilot.ai/dashboard/tasks/{task.id}")
-        return
-
-    task_handler = TaskHandler(task, show_spinner=not raw)
-    task_handler.wait_for_result(output, raw)
+    status.update(f"Task created: https://app.pr-pilot.ai/dashboard/tasks/{task.id}")
+    status.success()
+    if debug:
+        console.print(task)
+    if wait:
+        task_handler = TaskHandler(task, status)
+        task_handler.wait_for_result(output, quiet)
+    status.stop()
+    if debug:
+        console.print(task)
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pr_pilot_cli-1.3.4/cli/detect_repository.py` & `pr_pilot_cli-1.4.0/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.4/cli/prompt_template.py` & `pr_pilot_cli-1.4.0/cli/prompt_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 import os
 import subprocess
 import time
 
+import click
 import jinja2
 from pr_pilot.util import create_task
 from yaspin import yaspin
 
 from cli.task_handler import TaskHandler
 
 
 
-def sh(shell_command, spinner=None):
-    if spinner:
-        spinner.text = f"Running shell command: {shell_command}"
-    process = subprocess.Popen(shell_command.split(), stdout=subprocess.PIPE)
-    time.sleep(5)
-    output, error = process.communicate()
-    return output.decode('utf-8')
+def sh(shell_command, status):
+    status.update(f"Running shell command: {shell_command}")
+    try:
+        process = subprocess.Popen(shell_command.split(), stdout=subprocess.PIPE)
+        output, error = process.communicate()
+        status.success()
+        return output.decode('utf-8')
+    except Exception as e:
+        click.echo(str(e))
+        status.fail()
+
 
 def read_env_var(variable, default=None):
     """Get the value of an environment variable, with a default value."""
     return os.environ.get(variable, default)
 
 
-def wrap_function_with_spinner(func, show_spinner=True):
+def wrap_function_with_status(func, status):
     def wrapper(*args, **kwargs):
-        if not show_spinner:
-            return func(*args, **kwargs)
-        with yaspin() as spinner:
-            kwargs['spinner'] = spinner
-            return func(*args, **kwargs)
+        kwargs['status'] = status
+        return func(*args, **kwargs)
 
     return wrapper
 
+
 class PromptTemplate:
-    def __init__(self, template_file_path, repo, model):
+    def __init__(self, template_file_path, repo, model, status):
         self.template_file_path = template_file_path
         self.repo = repo
         self.model = model
+        self.status = status
+
+    def render(self):
 
-    def render(self, show_spinner=True):
-        def subtask(prompt, spinner=None):
+        def subtask(prompt, status):
             try:
+                status.update("Creating new task")
                 task = create_task(self.repo, prompt, log=False, gpt_model=self.model)
-                task_handler = TaskHandler(task, show_spinner)
-                return task_handler.wait_for_result(None, False)
+                task_handler = TaskHandler(task, status)
+                return task_handler.wait_for_result()
             except Exception as e:
                 return f"Error: {e}"
 
         env = jinja2.Environment(loader=jinja2.FileSystemLoader(os.getcwd()))
         env.globals.update(env=read_env_var)
-        env.globals.update(subtask=subtask)
-        env.globals.update(sh=wrap_function_with_spinner(sh, show_spinner))
+        env.globals.update(subtask=wrap_function_with_status(subtask, self.status))
+        env.globals.update(sh=wrap_function_with_status(sh, self.status))
         template = env.get_template(self.template_file_path)
         return template.render()
```

### Comparing `pr_pilot_cli-1.3.4/cli/task_handler.py` & `pr_pilot_cli-1.4.0/cli/task_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,63 @@
+import time
+
 from pr_pilot import Task
-from pr_pilot.util import wait_for_result, get_task
+from pr_pilot.util import get_task
 from rich.console import Console
 from rich.markdown import Markdown
-from yaspin import yaspin
 
+from cli.status_indicator import StatusIndicator
 
 POLL_INTERVAL = 2  # seconds
+MAX_RESULT_WAIT_TIME = 60 * 4  # 4 minutes
 
 
 class TaskHandler:
-    def __init__(self, task: Task, show_spinner=True):
+    def __init__(self, task: Task, status_indicator: StatusIndicator):
         self.task = task
         self.dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{task.id}"
         self.console = Console()
-        self.spinner = yaspin()
-        self.show_spinner = show_spinner
+        self.status = status_indicator
 
-    def wait_for_result(self, output_file=None, raw=False) -> str:
+    def wait_for_result(self, output_file=None, quiet=False) -> str:
         """
         Wait for the task to finish and display the result.
         :param output_file: Optional file to save the result.
-        :param raw: If true, print the raw result without formatting or status indicator.
+        :param quiet: If True, nothing will be printed on the command line.
         :return:
         """
-        if self.show_spinner:
-            self.spinner.start()
-            self.spinner.text = f"Running task: {self.dashboard_url}"
+
+        self.status.update("Waiting for task result")
+        self.status.start()
         try:
-            result = wait_for_result(self.task, poll_interval=POLL_INTERVAL)
+            start_time = time.time()
+            task_title = None
+            while self.task.status not in ["completed", "failed"]:
+                if time.time() - start_time > MAX_RESULT_WAIT_TIME:
+                    raise TimeoutError("The task took too long to complete.")
+                self.task = get_task(self.task.id)
+                if self.task.title and not self.task.title == "A title" and not task_title == self.task.title:
+                    task_title = self.task.title
+                    self.status.update(self.task.title)
+                time.sleep(POLL_INTERVAL)
+            if self.task.status == "failed":
+                raise ValueError(f"Task failed: {self.task.result}")
+
+            result = self.task.result
 
-            self.console.line()
             if output_file:
                 with open(output_file, "w") as f:
                     f.write(result)
-                self.console.print(f"Result saved in {output_file}")
-            elif raw:
-                self.console.print(result)
+                self.status.update(f"Result saved in {output_file}")
+                self.status.success()
             else:
-                self.console.print(Markdown(result))
-            self.console.line()
+                self.status.success()
+                self.status.stop()
+                if not quiet:
+                    self.console.line()
+                    self.console.print(Markdown(result))
+                    self.console.line()
+
             return result
         except Exception as e:
-            if self.show_spinner:
-                self.spinner.fail("💥")
-            self.console.print(f"Error: {e}")
-        finally:
-            if self.show_spinner:
-                self.spinner.stop()
+            self.status.update(f"Error: {e}")
+            self.status.fail()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pr_pilot_cli-1.3.4/setup.py` & `pr_pilot_cli-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.3.4',
+    version='1.4.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

