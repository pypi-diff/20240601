# Comparing `tmp/vscode_task_runner-1.1.0.tar.gz` & `tmp/vscode_task_runner-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vscode_task_runner-1.1.0.tar", max compression
+gzip compressed data, was "vscode_task_runner-1.2.0.tar", max compression
```

## Comparing `vscode_task_runner-1.1.0.tar` & `vscode_task_runner-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2024-02-18 03:23:53.818490 vscode_task_runner-1.1.0/LICENSE
--rw-r--r--   0        0        0     9230 2024-02-18 03:23:53.818490 vscode_task_runner-1.1.0/README.md
--rw-r--r--   0        0        0     1434 2024-02-18 03:23:53.818490 vscode_task_runner-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-18 03:23:53.818490 vscode_task_runner-1.1.0/vtr/__init__.py
--rw-r--r--   0        0        0       39 2024-02-18 03:23:53.818490 vscode_task_runner-1.1.0/vtr/__main__.py
--rw-r--r--   0        0        0     3186 2024-02-18 03:23:53.818490 vscode_task_runner-1.1.0/vtr/console.py
--rw-r--r--   0        0        0     1308 2024-02-18 03:23:53.818490 vscode_task_runner-1.1.0/vtr/constants.py
--rw-r--r--   0        0        0      929 2024-02-18 03:23:53.818490 vscode_task_runner-1.1.0/vtr/exceptions.py
--rw-r--r--   0        0        0     1501 2024-02-18 03:23:53.822490 vscode_task_runner-1.1.0/vtr/executor.py
--rw-r--r--   0        0        0     4187 2024-02-18 03:23:53.822490 vscode_task_runner-1.1.0/vtr/helpers.py
--rw-r--r--   0        0        0     1489 2024-02-18 03:23:53.822490 vscode_task_runner-1.1.0/vtr/models.py
--rw-r--r--   0        0        0      620 2024-02-18 03:23:53.822490 vscode_task_runner-1.1.0/vtr/parser.py
--rw-r--r--   0        0        0    10190 2024-02-18 03:23:53.822490 vscode_task_runner-1.1.0/vtr/task.py
--rw-r--r--   0        0        0     7523 2024-02-18 03:23:53.822490 vscode_task_runner-1.1.0/vtr/terminal_task_system.py
--rw-r--r--   0        0        0     5382 2024-02-18 03:23:53.822490 vscode_task_runner-1.1.0/vtr/variables.py
--rw-r--r--   0        0        0    10389 1970-01-01 00:00:00.000000 vscode_task_runner-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/LICENSE
+-rw-r--r--   0        0        0     9230 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/README.md
+-rw-r--r--   0        0        0     1438 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/__init__.py
+-rw-r--r--   0        0        0       39 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/__main__.py
+-rw-r--r--   0        0        0     3186 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/console.py
+-rw-r--r--   0        0        0     1308 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/constants.py
+-rw-r--r--   0        0        0      929 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/exceptions.py
+-rw-r--r--   0        0        0     1501 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/executor.py
+-rw-r--r--   0        0        0     4187 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/helpers.py
+-rw-r--r--   0        0        0     1489 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/models.py
+-rw-r--r--   0        0        0      620 2024-06-01 15:07:54.477779 vscode_task_runner-1.2.0/vtr/parser.py
+-rw-r--r--   0        0        0    10190 2024-06-01 15:07:54.481779 vscode_task_runner-1.2.0/vtr/task.py
+-rw-r--r--   0        0        0     7236 2024-06-01 15:07:54.481779 vscode_task_runner-1.2.0/vtr/terminal_task_system.py
+-rw-r--r--   0        0        0     5382 2024-06-01 15:07:54.481779 vscode_task_runner-1.2.0/vtr/variables.py
+-rw-r--r--   0        0        0    10389 1970-01-01 00:00:00.000000 vscode_task_runner-1.2.0/PKG-INFO
```

### Comparing `vscode_task_runner-1.1.0/LICENSE` & `vscode_task_runner-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/README.md` & `vscode_task_runner-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/pyproject.toml` & `vscode_task_runner-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "vscode-task-runner"
-    version = "1.1.0"
+    version = "1.2.0"
     description = "Task runner for VS Code tasks.json"
     license = "MIT"
     readme = "README.md"
     homepage = "https://github.com/NathanVaughn/vscode-task-runner"
     repository = "https://github.com/NathanVaughn/vscode-task-runner.git"
     authors = ["Nathan Vaughn <nvaughn51@gmail.com>"]
     classifiers = [
@@ -24,15 +24,15 @@
     dacite      = "^1.8.1"
     questionary = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
     pre-commit  = "^3.2.0"
     pytest      = ">=7.3.1,<9.0.0"
     pytest-mock = "^3.10.0"
-    pytest-cov  = "^4.1.0"
+    pytest-cov  = ">=4.1,<6.0"
 
 [tool.poetry.scripts]
     vtr                = "vtr.console:run"
     vscode-task-runner = "vtr.console:run"
 
 [tool.pyright]
     typeCheckingMode           = "basic"
```

### Comparing `vscode_task_runner-1.1.0/vtr/console.py` & `vscode_task_runner-1.2.0/vtr/console.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/vtr/constants.py` & `vscode_task_runner-1.2.0/vtr/constants.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/vtr/exceptions.py` & `vscode_task_runner-1.2.0/vtr/exceptions.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/vtr/executor.py` & `vscode_task_runner-1.2.0/vtr/executor.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/vtr/helpers.py` & `vscode_task_runner-1.2.0/vtr/helpers.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/vtr/models.py` & `vscode_task_runner-1.2.0/vtr/models.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/vtr/parser.py` & `vscode_task_runner-1.2.0/vtr/parser.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/vtr/task.py` & `vscode_task_runner-1.2.0/vtr/task.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/vtr/terminal_task_system.py` & `vscode_task_runner-1.2.0/vtr/terminal_task_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,46 +64,36 @@
 
 def create_shell_launch_config(
     shell_type: ShellType, shell_args: Union[List[str], str], command_line: str
 ) -> List[str]:
     # https://github.com/microsoft/vscode/blob/eef30e7165e19b33daa1e15e92fa34ff4a5df0d3/src/vs/workbench/contrib/tasks/browser/terminalTaskSystem.ts#L1107-L1177
 
     # manually converted and simplified
-
     # convert a single shell args string into a list
     if isinstance(shell_args, str):
         shell_args = [shell_args]
 
     to_add: List[str] = []
 
     # skip all this if the user has already manually specific arguments
     if not shell_args:
-        # this cannot happen in our case, since we don't have default
-        # arguments loaded from settings.
-
-        # Under Mac remove -l to not start it as a login shell.
-        # if vtr.constants.PLATFORM_KEY == "osx" and "-l" in shell_args:
-        #     shell_args.remove("-l")
-
         if shell_type == ShellType.PowerShell:
             to_add.append("-Command")
         elif shell_type == ShellType.SH:
             to_add.append("-c")
         elif shell_type == ShellType.WSL:
             to_add.append("-e")
         elif shell_type == ShellType.CMD:
             to_add.extend(["/d", "/c"])
+        elif shell_type == ShellType.Unknown:
+            # default to a -c, works for most shells
+            to_add.append("-c")
 
     combined_shell_args = _add_all_argument(to_add, shell_args)
     combined_shell_args.append(command_line)
-
-    # if windows_shell_args:
-    #     return [" ".join(combined_shell_args)]
-    # else:
-    #     return combined_shell_args
     return combined_shell_args
 
 
 def build_shell_command_line(
     shell_type: ShellType,
     shell_quoting_options: ShellQuotingOptions,
     task_command: CommandString,
```

### Comparing `vscode_task_runner-1.1.0/vtr/variables.py` & `vscode_task_runner-1.2.0/vtr/variables.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-1.1.0/PKG-INFO` & `vscode_task_runner-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vscode-task-runner
-Version: 1.1.0
+Version: 1.2.0
 Summary: Task runner for VS Code tasks.json
 Home-page: https://github.com/NathanVaughn/vscode-task-runner
 License: MIT
 Author: Nathan Vaughn
 Author-email: nvaughn51@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

