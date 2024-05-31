# Comparing `tmp/pr_pilot_cli-1.3.3.tar.gz` & `tmp/pr_pilot_cli-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.3.3.tar", last modified: Fri May 31 00:34:31 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.3.4.tar", last modified: Fri May 31 01:00:33 2024, max compression
```

## Comparing `pr_pilot_cli-1.3.3.tar` & `pr_pilot_cli-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:34:31.894970 pr_pilot_cli-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-31 00:34:31.894970 pr_pilot_cli-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:34:31.890970 pr_pilot_cli-1.3.3/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/cli/detect_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/cli/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/cli/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:34:31.894970 pr_pilot_cli-1.3.3/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-31 00:34:31.000000 pr_pilot_cli-1.3.3/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-31 00:34:31.000000 pr_pilot_cli-1.3.3/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:34:31.000000 pr_pilot_cli-1.3.3/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 00:34:31.000000 pr_pilot_cli-1.3.3/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 00:34:31.000000 pr_pilot_cli-1.3.3/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 00:34:31.000000 pr_pilot_cli-1.3.3/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:34:31.894970 pr_pilot_cli-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-31 00:34:27.000000 pr_pilot_cli-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:00:33.877976 pr_pilot_cli-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-31 01:00:33.877976 pr_pilot_cli-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:00:33.873976 pr_pilot_cli-1.3.4/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/detect_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/cli/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:00:33.877976 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 01:00:33.000000 pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:00:33.877976 pr_pilot_cli-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-31 01:00:29.000000 pr_pilot_cli-1.3.4/setup.py
```

### Comparing `pr_pilot_cli-1.3.3/LICENSE` & `pr_pilot_cli-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.3/PKG-INFO` & `pr_pilot_cli-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.3.3
+Version: 1.3.4
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.3 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.4 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
```

### Comparing `pr_pilot_cli-1.3.3/README.md` & `pr_pilot_cli-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.3/cli/cli.py` & `pr_pilot_cli-1.3.4/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.3/cli/detect_repository.py` & `pr_pilot_cli-1.3.4/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.3/cli/prompt_template.py` & `pr_pilot_cli-1.3.4/cli/prompt_template.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.3.3/cli/task_handler.py` & `pr_pilot_cli-1.3.4/cli/task_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 class TaskHandler:
     def __init__(self, task: Task, show_spinner=True):
         self.task = task
         self.dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{task.id}"
         self.console = Console()
         self.spinner = yaspin()
-        if not show_spinner:
-            self.spinner.hide()
+        self.show_spinner = show_spinner
 
     def wait_for_result(self, output_file=None, raw=False) -> str:
         """
         Wait for the task to finish and display the result.
         :param output_file: Optional file to save the result.
         :param raw: If true, print the raw result without formatting or status indicator.
         :return:
         """
-        self.spinner.start()
-        self.spinner.text = f"Running task: {self.dashboard_url}"
+        if self.show_spinner:
+            self.spinner.start()
+            self.spinner.text = f"Running task: {self.dashboard_url}"
         try:
             result = wait_for_result(self.task, poll_interval=POLL_INTERVAL)
 
             self.console.line()
             if output_file:
                 with open(output_file, "w") as f:
                     f.write(result)
@@ -37,12 +37,13 @@
             elif raw:
                 self.console.print(result)
             else:
                 self.console.print(Markdown(result))
             self.console.line()
             return result
         except Exception as e:
-            self.spinner.fail("💥")
+            if self.show_spinner:
+                self.spinner.fail("💥")
             self.console.print(f"Error: {e}")
         finally:
-            self.spinner.stop()
-            self.spinner.hide()
+            if self.show_spinner:
+                self.spinner.stop()
```

### Comparing `pr_pilot_cli-1.3.3/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.3.4/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.3.3
+Version: 1.3.4
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.3 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.3.4 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.1 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1 Requires-Dist: jinja2==3.1.4
                                 [PR Pilot Logo]
```

### Comparing `pr_pilot_cli-1.3.3/setup.py` & `pr_pilot_cli-1.3.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.3.3',
+    version='1.3.4',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

