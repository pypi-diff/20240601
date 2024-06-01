# Comparing `tmp/pr_pilot_cli-1.4.1.tar.gz` & `tmp/pr_pilot_cli-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.4.1.tar", last modified: Sat Jun  1 01:03:41 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.4.2.tar", last modified: Sat Jun  1 05:01:05 2024, max compression
```

## Comparing `pr_pilot_cli-1.4.1.tar` & `pr_pilot_cli-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:03:41.043411 pr_pilot_cli-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 01:03:41.043411 pr_pilot_cli-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:03:41.043411 pr_pilot_cli-1.4.1/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/detect_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/status_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/cli/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:03:41.043411 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 01:03:41.000000 pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:03:41.047412 pr_pilot_cli-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-01 01:03:36.000000 pr_pilot_cli-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/detect_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/status_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/cli/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 05:01:05.000000 pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 05:01:05.593724 pr_pilot_cli-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-01 05:01:01.000000 pr_pilot_cli-1.4.2/setup.py
```

### Comparing `pr_pilot_cli-1.4.1/LICENSE` & `pr_pilot_cli-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.1/PKG-INFO` & `pr_pilot_cli-1.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.4.1
+Version: 1.4.2
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -95,18 +95,29 @@
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
 ## Installation
 
-I't simple:
+Prerequisites:
 1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
 2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
 
+Install via pip:
+```
+pip install --upgrade pr-pilot-cli
+```
+
+Install via Homebrew:
+```
+brew tap PR-Pilot-AI/pr-pilot-homebrew
+brew install pr-pilot-cli
+```
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
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.1 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.2 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
@@ -29,15 +29,18 @@
 TEXT Github repository in the format owner/repo. --spinner / --no-spinner
 Display a loading indicator --quiet No pretty-print, no status indicator or
 messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
 prompt and settings for generating code -f, --file PATH Load prompt from a
 template file. --direct Do not feed the rendered template as a prompt into PR
 Pilot, but render it directly as output. -o, --output PATH Output file for the
 result. --model TEXT GPT model to use. --debug Display debug information. --
-help Show this message and exit. ``` ## Installation I't simple: 1. **[Install
-the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on
-your Github repository 2. **[Generate an API key](https://app.pr-pilot.ai/
-dashboard/api-keys/)** in the dashboard ## Configuration The configuration file
-is located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
-improve the CLI by submitting pull requests or reporting issues. For more
-details, check the project's GitHub repository. ## License The PR Pilot CLI is
-open-source software licensed under the GPL-3 license.
+help Show this message and exit. ``` ## Installation Prerequisites: 1. **
+[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/
+new)** on your Github repository 2. **[Generate an API key](https://app.pr-
+pilot.ai/dashboard/api-keys/)** in the dashboard Install via pip: ``` pip
+install --upgrade pr-pilot-cli ``` Install via Homebrew: ``` brew tap PR-Pilot-
+AI/pr-pilot-homebrew brew install pr-pilot-cli ``` ## Configuration The
+configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
+Contributors are welcome to improve the CLI by submitting pull requests or
+reporting issues. For more details, check the project's GitHub repository. ##
+License The PR Pilot CLI is open-source software licensed under the GPL-
+3 license.
```

### Comparing `pr_pilot_cli-1.4.1/README.md` & `pr_pilot_cli-1.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -78,18 +78,29 @@
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
 ## Installation
 
-I't simple:
+Prerequisites:
 1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
 2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
 
+Install via pip:
+```
+pip install --upgrade pr-pilot-cli
+```
+
+Install via Homebrew:
+```
+brew tap PR-Pilot-AI/pr-pilot-homebrew
+brew install pr-pilot-cli
+```
+
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
 
 ## License
```

#### html2text {}

```diff
@@ -22,15 +22,18 @@
 TEXT Github repository in the format owner/repo. --spinner / --no-spinner
 Display a loading indicator --quiet No pretty-print, no status indicator or
 messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
 prompt and settings for generating code -f, --file PATH Load prompt from a
 template file. --direct Do not feed the rendered template as a prompt into PR
 Pilot, but render it directly as output. -o, --output PATH Output file for the
 result. --model TEXT GPT model to use. --debug Display debug information. --
-help Show this message and exit. ``` ## Installation I't simple: 1. **[Install
-the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on
-your Github repository 2. **[Generate an API key](https://app.pr-pilot.ai/
-dashboard/api-keys/)** in the dashboard ## Configuration The configuration file
-is located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
-improve the CLI by submitting pull requests or reporting issues. For more
-details, check the project's GitHub repository. ## License The PR Pilot CLI is
-open-source software licensed under the GPL-3 license.
+help Show this message and exit. ``` ## Installation Prerequisites: 1. **
+[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/
+new)** on your Github repository 2. **[Generate an API key](https://app.pr-
+pilot.ai/dashboard/api-keys/)** in the dashboard Install via pip: ``` pip
+install --upgrade pr-pilot-cli ``` Install via Homebrew: ``` brew tap PR-Pilot-
+AI/pr-pilot-homebrew brew install pr-pilot-cli ``` ## Configuration The
+configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
+Contributors are welcome to improve the CLI by submitting pull requests or
+reporting issues. For more details, check the project's GitHub repository. ##
+License The PR Pilot CLI is open-source software licensed under the GPL-
+3 license.
```

### Comparing `pr_pilot_cli-1.4.1/cli/cli.py` & `pr_pilot_cli-1.4.2/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.1/cli/detect_repository.py` & `pr_pilot_cli-1.4.2/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.1/cli/status_indicator.py` & `pr_pilot_cli-1.4.2/cli/status_indicator.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.1/cli/task_handler.py` & `pr_pilot_cli-1.4.2/cli/task_handler.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.4.1/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.4.2/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.4.1
+Version: 1.4.2
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -95,18 +95,29 @@
   --debug                   Display debug information.
   --help                    Show this message and exit.
 
 ```
 
 ## Installation
 
-I't simple:
+Prerequisites:
 1. **[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on your Github repository
 2. **[Generate an API key](https://app.pr-pilot.ai/dashboard/api-keys/)** in the dashboard
 
+Install via pip:
+```
+pip install --upgrade pr-pilot-cli
+```
+
+Install via Homebrew:
+```
+brew tap PR-Pilot-AI/pr-pilot-homebrew
+brew install pr-pilot-cli
+```
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
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.1 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.4.2 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
@@ -29,15 +29,18 @@
 TEXT Github repository in the format owner/repo. --spinner / --no-spinner
 Display a loading indicator --quiet No pretty-print, no status indicator or
 messages. --cheap Use the cheapest GPT model (gpt-3.5-turbo) --code Optimize
 prompt and settings for generating code -f, --file PATH Load prompt from a
 template file. --direct Do not feed the rendered template as a prompt into PR
 Pilot, but render it directly as output. -o, --output PATH Output file for the
 result. --model TEXT GPT model to use. --debug Display debug information. --
-help Show this message and exit. ``` ## Installation I't simple: 1. **[Install
-the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/new)** on
-your Github repository 2. **[Generate an API key](https://app.pr-pilot.ai/
-dashboard/api-keys/)** in the dashboard ## Configuration The configuration file
-is located at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to
-improve the CLI by submitting pull requests or reporting issues. For more
-details, check the project's GitHub repository. ## License The PR Pilot CLI is
-open-source software licensed under the GPL-3 license.
+help Show this message and exit. ``` ## Installation Prerequisites: 1. **
+[Install the PR Pilot app](https://github.com/apps/pr-pilot-ai/installations/
+new)** on your Github repository 2. **[Generate an API key](https://app.pr-
+pilot.ai/dashboard/api-keys/)** in the dashboard Install via pip: ``` pip
+install --upgrade pr-pilot-cli ``` Install via Homebrew: ``` brew tap PR-Pilot-
+AI/pr-pilot-homebrew brew install pr-pilot-cli ``` ## Configuration The
+configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
+Contributors are welcome to improve the CLI by submitting pull requests or
+reporting issues. For more details, check the project's GitHub repository. ##
+License The PR Pilot CLI is open-source software licensed under the GPL-
+3 license.
```

### Comparing `pr_pilot_cli-1.4.1/setup.py` & `pr_pilot_cli-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.4.1',
+    version='1.4.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

