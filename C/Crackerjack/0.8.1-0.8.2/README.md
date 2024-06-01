# Comparing `tmp/crackerjack-0.8.1.tar.gz` & `tmp/crackerjack-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.8.1.tar", last modified: Sat Jun  1 14:15:39 2024, max compression
+gzip compressed data, was "crackerjack-0.8.2.tar", last modified: Sat Jun  1 18:12:30 2024, max compression
```

## Comparing `crackerjack-0.8.1.tar` & `crackerjack-0.8.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.8.1/LICENSE
--rw-r--r--   0        0        0     6261 2024-06-01 11:05:46.530942 crackerjack-0.8.1/README.md
--rw-r--r--   0        0        0      197 2024-06-01 14:15:14.232808 crackerjack-0.8.1/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2024-06-01 14:15:14.239850 crackerjack-0.8.1/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2264 2024-06-01 14:15:14.236144 crackerjack-0.8.1/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.8.1/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      248 2024-01-06 07:37:34.391552 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.11/3256171999636029978
--rw-r--r--   0        0        0      248 2024-01-24 12:53:52.172690 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.14/602324811142551221
--rw-r--r--   0        0        0      248 2023-11-06 09:35:44.665597 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.4/10355199064880463147
--rw-r--r--   0        0        0      248 2023-11-30 19:47:12.985430 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.6/15140459877605758699
--rw-r--r--   0        0        0      248 2023-12-09 08:32:10.697985 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.7/1790508110482614856
--rw-r--r--   0        0        0      248 2023-12-25 16:57:47.788926 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.9/17041001205004563469
--rw-r--r--   0        0        0      248 2024-02-04 19:42:45.746383 crackerjack-0.8.1/crackerjack/.ruff_cache/0.2.0/10047773857155985907
--rw-r--r--   0        0        0      248 2024-02-08 21:29:34.013736 crackerjack-0.8.1/crackerjack/.ruff_cache/0.2.1/8522267973936635051
--rw-r--r--   0        0        0      248 2024-02-19 14:09:40.345898 crackerjack-0.8.1/crackerjack/.ruff_cache/0.2.2/18053836298936336950
--rw-r--r--   0        0        0      248 2024-03-02 11:27:50.943765 crackerjack-0.8.1/crackerjack/.ruff_cache/0.3.0/12548816621480535786
--rw-r--r--   0        0        0      248 2024-03-18 07:54:31.415399 crackerjack-0.8.1/crackerjack/.ruff_cache/0.3.3/11081883392474770722
--rw-r--r--   0        0        0      248 2024-03-27 22:01:10.025644 crackerjack-0.8.1/crackerjack/.ruff_cache/0.3.4/676973378459347183
--rw-r--r--   0        0        0      248 2024-04-02 07:04:47.506968 crackerjack-0.8.1/crackerjack/.ruff_cache/0.3.5/16311176246009842383
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.8.1/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.8.1/crackerjack/__init__.py
--rw-r--r--   0        0        0     1767 2024-06-01 09:32:10.833253 crackerjack-0.8.1/crackerjack/__main__.py
--rw-r--r--   0        0        0     7906 2024-06-01 10:39:46.039848 crackerjack-0.8.1/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     2799 2024-06-01 14:15:15.801398 crackerjack-0.8.1/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2799 2024-06-01 14:15:39.847169 crackerjack-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     7760 1970-01-01 00:00:00.000000 crackerjack-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.8.2/LICENSE
+-rw-r--r--   0        0        0     6261 2024-06-01 11:05:46.530942 crackerjack-0.8.2/README.md
+-rw-r--r--   0        0        0      197 2024-06-01 18:12:04.564476 crackerjack-0.8.2/crackerjack/.gitignore
+-rw-r--r--   0        0        0      772 2024-06-01 18:12:04.568718 crackerjack-0.8.2/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2167 2024-06-01 18:12:04.566679 crackerjack-0.8.2/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.8.2/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      248 2024-01-06 07:37:34.391552 crackerjack-0.8.2/crackerjack/.ruff_cache/0.1.11/3256171999636029978
+-rw-r--r--   0        0        0      248 2024-01-24 12:53:52.172690 crackerjack-0.8.2/crackerjack/.ruff_cache/0.1.14/602324811142551221
+-rw-r--r--   0        0        0      248 2023-11-06 09:35:44.665597 crackerjack-0.8.2/crackerjack/.ruff_cache/0.1.4/10355199064880463147
+-rw-r--r--   0        0        0      248 2023-11-30 19:47:12.985430 crackerjack-0.8.2/crackerjack/.ruff_cache/0.1.6/15140459877605758699
+-rw-r--r--   0        0        0      248 2023-12-09 08:32:10.697985 crackerjack-0.8.2/crackerjack/.ruff_cache/0.1.7/1790508110482614856
+-rw-r--r--   0        0        0      248 2023-12-25 16:57:47.788926 crackerjack-0.8.2/crackerjack/.ruff_cache/0.1.9/17041001205004563469
+-rw-r--r--   0        0        0      248 2024-02-04 19:42:45.746383 crackerjack-0.8.2/crackerjack/.ruff_cache/0.2.0/10047773857155985907
+-rw-r--r--   0        0        0      248 2024-02-08 21:29:34.013736 crackerjack-0.8.2/crackerjack/.ruff_cache/0.2.1/8522267973936635051
+-rw-r--r--   0        0        0      248 2024-02-19 14:09:40.345898 crackerjack-0.8.2/crackerjack/.ruff_cache/0.2.2/18053836298936336950
+-rw-r--r--   0        0        0      248 2024-03-02 11:27:50.943765 crackerjack-0.8.2/crackerjack/.ruff_cache/0.3.0/12548816621480535786
+-rw-r--r--   0        0        0      248 2024-03-18 07:54:31.415399 crackerjack-0.8.2/crackerjack/.ruff_cache/0.3.3/11081883392474770722
+-rw-r--r--   0        0        0      248 2024-03-27 22:01:10.025644 crackerjack-0.8.2/crackerjack/.ruff_cache/0.3.4/676973378459347183
+-rw-r--r--   0        0        0      248 2024-04-02 07:04:47.506968 crackerjack-0.8.2/crackerjack/.ruff_cache/0.3.5/16311176246009842383
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.8.2/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.8.2/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1766 2024-06-01 16:17:09.941534 crackerjack-0.8.2/crackerjack/__main__.py
+-rw-r--r--   0        0        0     8052 2024-06-01 17:29:48.590452 crackerjack-0.8.2/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     2896 2024-06-01 18:12:06.118742 crackerjack-0.8.2/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2907 2024-06-01 18:12:30.011464 crackerjack-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     7760 1970-01-01 00:00:00.000000 crackerjack-0.8.2/PKG-INFO
```

### Comparing `crackerjack-0.8.1/LICENSE` & `crackerjack-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.8.1/README.md` & `crackerjack-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.8.1/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.8.2/crackerjack/.libcst.codemod.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # String that LibCST should look for in code which indicates that the
 # module is generated code.
 generated_code_marker: '@generated'
 # Command line and arguments for invoking a code formatter. Anything
 # specified here must be capable of taking code via stdin and returning
 # formatted code via stdout.
-formatter: [ 'black', '-' ]
+formatter: [ 'ruff', 'format' ]
 # List of regex patterns which LibCST will evaluate against filenames to
 # determine if the module should be touched.
 blacklist_patterns: [ ]
 # List of modules that contain codemods inside of them.
 modules:
   - 'libcst.codemod.commands'
   - 'autotyping'
```

### Comparing `crackerjack-0.8.1/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.8.2/crackerjack/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         name: check-added-large-files
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: v0.4.7
     hooks:
       - id: ruff-format
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
-    rev: v3.0.0
+    rev: v3.0.1
     hooks:
       - id: creosote
   - repo: https://github.com/ikamensh/flynt/
     rev: '1.0.1'
     hooks:
       - id: flynt
   - repo: https://github.com/codespell-project/codespell
@@ -35,28 +35,26 @@
       - id: codespell
         additional_dependencies:
           - tomli
   - repo: local
     hooks:
       - id: autotyping
         name: autotyping
-        entry: python -m libcst.tool codemod autotyping.AutotypeCommand
+        entry: python -m autotyping
         args:
           - --aggressive
           - --only-without-imports
-          - --show-successes
-          - --include-generated
           - --guess-common-names
           - crackerjack
         types_or: [ python, pyi ]
         language: python
         files: \.py$
         additional_dependencies:
-          - autotyping>=23.3.0
-          - libcst>=0.4.9
+          - autotyping>=24.3.0
+          - libcst>=1.1.0
   - repo: https://github.com/dosisod/refurb
     rev: v2.0.0
     hooks:
       - id: refurb
   - repo: https://github.com/PyCQA/bandit
     rev: '1.7.8'
     hooks:
```

### Comparing `crackerjack-0.8.1/crackerjack/__main__.py` & `crackerjack-0.8.2/crackerjack/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import typing as t
 
 from click import command, help_option, option
 from pydantic import BaseModel
-
 from crackerjack import crackerjack_it
 
 
 class Options(BaseModel):
     commit: bool = False
     interactive: bool = False
     doc: bool = False
```

### Comparing `crackerjack-0.8.1/crackerjack/crackerjack.py` & `crackerjack-0.8.2/crackerjack/crackerjack.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,17 @@
         for config in config_files:
             config_path = self.our_path / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
             if self.pkg_path.stem == "crackerjack":
                 await config_path.write_text(await pkg_config_path.read_text())
                 continue
+            await pkg_config_path.write_text(
+                (await config_path.read_text()).replace("crackerjack", self.pkg_name)
+            )
             run([str(self.config.git_path), "add", config])
 
     async def run_interactive(self, hook: str) -> None:
         success: bool = False
         while not success:
             fail = run(
                 [str(self.config.pre_commit_path), "run", hook.lower(), "--all-files"]
```

### Comparing `crackerjack-0.8.1/crackerjack/pyproject.toml` & `crackerjack-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,21 @@
 ]
 extend-select = [
     "I",
     "C901",
     "D",
 ]
 
+[tool.ruff.lint.isort]
+no-lines-before = [
+    "first-party",
+    "local-folder",
+]
+case-sensitive = false
+
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.creosote]
 paths = [
     "crackerjack",
 ]
@@ -85,15 +92,15 @@
 reportUnknownArgumentType = false
 reportPrivateUsage = "warning"
 pythonVersion = "3.12"
 pythonPlatform = "Darwin"
 
 [project]
 name = "Crackerjack"
-version = "0.8.0"
+version = "0.8.2"
 description = "Crackerjack code style"
 requires-python = ">=3.12"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -117,19 +124,19 @@
 dependencies = [
     "click>=8.1.7",
     "aioconsole>=0.7.1",
     "inflection>=0.5.1",
     "autotyping>=24.3.0",
     "pre-commit>=3.7.1",
     "pytest>=8.2.1",
-    "pydantic>=2.7.1",
+    "pydantic>=2.7.2",
     "aiopath>=0.7.7",
-    "acb>=0.6.0",
+    "acb>=0.6.2",
     "pdm-bump>=0.9.0",
-    "pdm>=2.15.2",
+    "pdm>=2.15.4",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.8.1/pyproject.toml` & `crackerjack-0.8.2/crackerjack/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 fix = true
 show-fixes = true
 output-format = "full"
 
 [tool.ruff.format]
 docstring-code-format = true
 
+[tool.ruff.lint.isort]
+no-lines-before = ["first-party", "local-folder"]
+case-sensitive = false
+
 [tool.ruff.lint]
 ignore = [
     "F821",
     "D100",
     "D101",
     "D102",
     "D103",
@@ -117,19 +121,19 @@
 dependencies = [
     "click>=8.1.7",
     "aioconsole>=0.7.1",
     "inflection>=0.5.1",
     "autotyping>=24.3.0",
     "pre-commit>=3.7.1",
     "pytest>=8.2.1",
-    "pydantic>=2.7.1",
+    "pydantic>=2.7.2",
     "aiopath>=0.7.7",
-    "acb>=0.6.0",
+    "acb>=0.6.2",
     "pdm-bump>=0.9.0",
-    "pdm>=2.15.2",
+    "pdm>=2.15.4",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.8.1/PKG-INFO` & `crackerjack-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.8.1
+Version: 0.8.2
 Summary: Crackerjack code style
 Keywords: black,ruff,mypy,creosote,refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
@@ -25,19 +25,19 @@
 Requires-Python: >=3.12
 Requires-Dist: click>=8.1.7
 Requires-Dist: aioconsole>=0.7.1
 Requires-Dist: inflection>=0.5.1
 Requires-Dist: autotyping>=24.3.0
 Requires-Dist: pre-commit>=3.7.1
 Requires-Dist: pytest>=8.2.1
-Requires-Dist: pydantic>=2.7.1
+Requires-Dist: pydantic>=2.7.2
 Requires-Dist: aiopath>=0.7.7
-Requires-Dist: acb>=0.6.0
+Requires-Dist: acb>=0.6.2
 Requires-Dist: pdm-bump>=0.9.0
-Requires-Dist: pdm>=2.15.2
+Requires-Dist: pdm>=2.15.4
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
 
 [![Python: 3.12](https://img.shields.io/badge/python-3.12%2B-blue)](https://docs.python.org/3/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

