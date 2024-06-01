# Comparing `tmp/crackerjack-0.7.9.tar.gz` & `tmp/crackerjack-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.7.9.tar", last modified: Sat Nov  4 14:26:39 2023, max compression
+gzip compressed data, was "crackerjack-0.8.0.tar", last modified: Sat Jun  1 11:10:25 2024, max compression
```

## Comparing `crackerjack-0.7.9.tar` & `crackerjack-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,26 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.7.9/LICENSE
--rw-r--r--   0        0        0     5853 2023-09-28 08:22:56.721114 crackerjack-0.7.9/README.md
--rw-r--r--   0        0        0      197 2023-11-04 14:26:23.730744 crackerjack-0.7.9/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-11-04 14:26:23.732926 crackerjack-0.7.9/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2452 2023-11-04 14:26:23.731823 crackerjack-0.7.9/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.7.9/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      248 2023-11-04 14:25:36.771278 crackerjack-0.7.9/crackerjack/.ruff_cache/0.1.4/10355199064880463147
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.7.9/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.7.9/crackerjack/__init__.py
--rw-r--r--   0        0        0     1567 2023-10-13 04:57:56.888743 crackerjack-0.7.9/crackerjack/__main__.py
--rw-r--r--   0        0        0     8152 2023-10-17 08:39:56.127703 crackerjack-0.7.9/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     2565 2023-11-04 14:26:24.821869 crackerjack-0.7.9/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2565 2023-11-04 14:26:39.922172 crackerjack-0.7.9/pyproject.toml
--rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 crackerjack-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6261 2024-06-01 11:05:46.530942 crackerjack-0.8.0/README.md
+-rw-r--r--   0        0        0      197 2024-06-01 11:09:57.660429 crackerjack-0.8.0/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2024-06-01 11:09:57.667134 crackerjack-0.8.0/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2264 2024-06-01 11:09:57.663819 crackerjack-0.8.0/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.8.0/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      248 2024-01-06 07:37:34.391552 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.11/3256171999636029978
+-rw-r--r--   0        0        0      248 2024-01-24 12:53:52.172690 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.14/602324811142551221
+-rw-r--r--   0        0        0      248 2023-11-06 09:35:44.665597 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.4/10355199064880463147
+-rw-r--r--   0        0        0      248 2023-11-30 19:47:12.985430 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.6/15140459877605758699
+-rw-r--r--   0        0        0      248 2023-12-09 08:32:10.697985 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.7/1790508110482614856
+-rw-r--r--   0        0        0      248 2023-12-25 16:57:47.788926 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.9/17041001205004563469
+-rw-r--r--   0        0        0      248 2024-02-04 19:42:45.746383 crackerjack-0.8.0/crackerjack/.ruff_cache/0.2.0/10047773857155985907
+-rw-r--r--   0        0        0      248 2024-02-08 21:29:34.013736 crackerjack-0.8.0/crackerjack/.ruff_cache/0.2.1/8522267973936635051
+-rw-r--r--   0        0        0      248 2024-02-19 14:09:40.345898 crackerjack-0.8.0/crackerjack/.ruff_cache/0.2.2/18053836298936336950
+-rw-r--r--   0        0        0      248 2024-03-02 11:27:50.943765 crackerjack-0.8.0/crackerjack/.ruff_cache/0.3.0/12548816621480535786
+-rw-r--r--   0        0        0      248 2024-03-18 07:54:31.415399 crackerjack-0.8.0/crackerjack/.ruff_cache/0.3.3/11081883392474770722
+-rw-r--r--   0        0        0      248 2024-03-27 22:01:10.025644 crackerjack-0.8.0/crackerjack/.ruff_cache/0.3.4/676973378459347183
+-rw-r--r--   0        0        0      248 2024-04-02 07:04:47.506968 crackerjack-0.8.0/crackerjack/.ruff_cache/0.3.5/16311176246009842383
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.8.0/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.8.0/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1767 2024-06-01 09:32:10.833253 crackerjack-0.8.0/crackerjack/__main__.py
+-rw-r--r--   0        0        0     7906 2024-06-01 10:39:46.039848 crackerjack-0.8.0/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     2776 2024-06-01 11:09:59.406480 crackerjack-0.8.0/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2775 2024-06-01 11:10:25.704923 crackerjack-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7760 1970-01-01 00:00:00.000000 crackerjack-0.8.0/PKG-INFO
```

### Comparing `crackerjack-0.7.9/LICENSE` & `crackerjack-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.7.9/README.md` & `crackerjack-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Crackerjack Python
 
-[![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
+[![Python: 3.12](https://img.shields.io/badge/python-3.12%2B-blue)](https://docs.python.org/3/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 Crackerjack is a python coding style which uses a minimalist approach to produce elegant, easy to read, code.
@@ -54,25 +55,25 @@
 
 - streamlines and standardizes code style across numerous packages
 
 - installs, or updates, a project's pre-commit tools as well as .gitignore & other config files
   to comply with evolving crackerjack standards
 
 - runs the following pre-commit hooks (in order):
-  * various core pre-commit hooks
-  * [black](https://github.com/ambv/black)
-  * ruff
-  * creosote
-  * bandit
-  * flynt
-  * autotyping
-  * refurb
-  * pyright
-  * ruff (again for sanity checking)
-  * black (again for sanity checking)
+  * [pdm-lock-check](https://github.com/pdm-project/pdm)
+  * various core [pre-commit-hooks](https://github.com/pre-commit/pre-commit-hooks)
+  * [ruff](https://github.com/charliermarsh/ruff-pre-commit)
+  * [creosote](https://github.com/fredrikaverpil/creosote)
+  * [flynt](https://github.com/ikamensh/flynt/)
+  * [codespell](https://github.com/codespell-project/codespell)
+  * [autotyping](https://github.com/JelleZijlstra/autotyping)
+  * [refurb](https://github.com/dosisod/refurb)
+  * [bandit](https://github.com/PyCQA/bandit)
+  * [pyright](https://github.com/RobertCraigie/pyright-python)
+  * [ruff](https://github.com/charliermarsh/ruff-pre-commit) (again for sanity checking)
 
 - converts/creates documentation in Markdown (md) (work in progress)
 
 - runs tests and generates pytest mock stubs if needed (work in progress)
 
 - bumps the project version and publishes it to PyPI
 
@@ -82,30 +83,24 @@
 
 (...more what you'd call "guidelines" than actual rules. -Captain Barbossa )
 
 - code is statically typed
 
 - all docstrings, README's, and other documentation is to be done in Markdown (md)
 
-- format with black
-
 - use aiopath.AsyncPath or pathlib.Path not os.path
 
 - import typing as t
 
 - do not capitalize all letters in configuration settings or constants (we diverge from PEP-8 here
  for not other reason than it looks ugly)
 
 - functions that deal with path operations should get passed AsyncPaths or Paths - not strings
 
-- if a class can be a dataclasses.dataclass, pydantic.BaseModel, or msgspec.Struct it should be
-
-- force single line imports (will support isort Vertical Hanging Indent when ruff does)
-
-- use PDM and PEP-582 for dependency management and package building/publishing
+- use PDM and PEP-582(proposed) for dependency management and package building/publishing
 
 - use pdoc and mkdocs for producing documentation
 
 - use pytest for testing
 
 - be compliant with the latest python version within 2 months after release
```

### Comparing `crackerjack-0.7.9/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.8.0/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.7.9/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.8.0/crackerjack/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 repos:
   - repo: https://github.com/pdm-project/pdm
-    rev: 2.10.0  # a PDM release exposing the hook
+    rev: 2.15.4  # a PDM release exposing the hook
     hooks:
       - id: pdm-lock-check
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
-        name: trailing-whitspace
+        name: trailing-whitespace
       - id: end-of-file-fixer
         name: end-of-file-fixer
       - id: check-yaml
         name: check-yaml
       - id: check-toml
         name: check-toml
       - id: check-added-large-files
         name: check-added-large-files
-  - repo: https://github.com/psf/black
-    rev: '23.10.1'
-    hooks:
-      - id: black
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.1.4
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.7
     hooks:
+      - id: ruff-format
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
     rev: v3.0.0
     hooks:
       - id: creosote
   - repo: https://github.com/ikamensh/flynt/
     rev: '1.0.1'
     hooks:
       - id: flynt
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.6
+    rev: v2.3.0
     hooks:
       - id: codespell
         additional_dependencies:
           - tomli
-        args: [--ignore-words-list, "crate,uptodate"]
   - repo: local
     hooks:
       - id: autotyping
         name: autotyping
         entry: python -m libcst.tool codemod autotyping.AutotypeCommand
         args:
           - --aggressive
@@ -54,37 +50,34 @@
         types_or: [ python, pyi ]
         language: python
         files: \.py$
         additional_dependencies:
           - autotyping>=23.3.0
           - libcst>=0.4.9
   - repo: https://github.com/dosisod/refurb
-    rev: v1.22.1
+    rev: v2.0.0
     hooks:
       - id: refurb
   - repo: https://github.com/PyCQA/bandit
-    rev: '1.7.5'
+    rev: '1.7.8'
     hooks:
       - id: bandit
         args: ["-c", "pyproject.toml"]
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.334
+    rev: v1.1.365
     hooks:
       - id: pyright
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.7
+    hooks:
+      - id: ruff
+      - id: ruff-format
   #  - repo: https://github.com/pdoc3/pdoc
   #    rev: master
   #    hooks:
   #      - id: pdoc
   #        name: pdoc
   #        entry: pdoc --html -f -o docs module1 module2 module3
   #        language_version: python3.11
   #        require_serial: true
   #        types: [ python ]
   #        always_run: true
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.1.4
-    hooks:
-      - id: ruff
-  - repo: https://github.com/psf/black
-    rev: '23.10.1'
-    hooks:
-      - id: black
```

### Comparing `crackerjack-0.7.9/crackerjack/__main__.py` & `crackerjack-0.8.0/crackerjack/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
 import typing as t
 
-from click import command
-from click import help_option
-from click import option
-from crackerjack import crackerjack_it
+from click import command, help_option, option
 from pydantic import BaseModel
 
+from crackerjack import crackerjack_it
+
 
 class Options(BaseModel):
     commit: bool = False
     interactive: bool = False
     doc: bool = False
     do_not_update_configs: bool = False
     publish: t.Literal["micro", "minor", "major"] | bool = False
+    bump: t.Literal["micro", "minor", "major"] | bool = False
     verbose: bool = False
     update_precommit: bool = False
 
 
 options = Options()
 
 
@@ -25,37 +25,41 @@
 @help_option("-h", is_flag=True, help="help")
 @option("-c", is_flag=True, help="commit")
 @option("-i", is_flag=True, help="interactive")
 @option("-d", is_flag=True, help="doc")
 @option("-x", is_flag=True, help="do not update configs")
 @option("-u", is_flag=True, help="update pre-commit")
 @option("-v", is_flag=True, help="verbose")
-@option("-p", help="publish: -p [micro, minor, major]")
+@option("-p", help="bump version and publish: -p [micro, minor, major]")
+@option("-b", help="bump version: -b [micro, minor, major]")
 # @option("-f", help="format: -f [module]")
 def crackerjack(
     c: bool = False,
     i: bool = False,
     d: bool = False,
     u: bool = False,
     v: bool = False,
     x: bool = False,
     p: str | bool = False,
+    b: str | bool = False,
 ) -> None:
     if c:
         options.commit = c
     if i:
         options.interactive = i
     if d:
         options.doc = d
     if u:
         options.update_precommit = u
     if x:
         options.do_not_update_configs = x
     if p in ("micro", "minor", "major"):
         options.publish = p
+    if b in ("micro", "minor", "major"):
+        options.bump = b
     if v:
         print("-v not currently implemented")
         options.verbose = v
     asyncio.run(crackerjack_it(options=options))
 
 
 if __name__ == "__main__":
```

### Comparing `crackerjack-0.7.9/crackerjack/crackerjack.py` & `crackerjack-0.8.0/crackerjack/crackerjack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import asyncio
 import re
 import sys
 import typing as t
 from pathlib import Path
 from subprocess import run
 
-from acb.actions.encode import dump
-from acb.actions.encode import load
-from aioconsole import ainput
-from aioconsole import aprint
+from acb.actions.encode import dump, load
+from aioconsole import ainput, aprint
 from aiopath import AsyncPath
 from inflection import underscore
 from pydantic import BaseModel
 
 
 class Config(BaseModel):
     python_version: t.Optional[str] = None
     pre_commit_path: t.Optional[Path] = None
     git_path: t.Optional[Path] = None
     pdm_path: t.Optional[Path] = None
     zshenv_path: t.Optional[Path] = None
 
 
-class Crakerjack(BaseModel, arbitrary_types_allowed=True):
+class Crackerjack(BaseModel, arbitrary_types_allowed=True):
     our_path: AsyncPath = AsyncPath(__file__).parent
     pkg_path: AsyncPath = AsyncPath(Path.cwd())
     settings_path: AsyncPath = pkg_path / ".crackerjack.yaml"
     pkg_dir: t.Optional[AsyncPath] = None
     pkg_name: str = "crackerjack"
     our_toml: t.Optional[dict[str, t.Any]] = None
     pkg_toml: t.Optional[dict[str, t.Any]] = None
@@ -54,14 +52,15 @@
                         value = value.replace("crackerjack", self.pkg_name)
                     settings[setting] = value
                 if setting in (
                     "exclude-deps",
                     "exclude",
                     "excluded",
                     "skips",
+                    "ignore",
                 ) and isinstance(value, list):
                     settings[setting] = set(
                         pkg_toml_config["tool"][tool][setting] + value
                     )
             pkg_toml_config["tool"][tool] = settings
         pkg_toml_config["tool"]["pdm"]["dev-dependencies"] = pkg_deps
         python_version_pattern = r"\s*W*(\d\.\d*)"
@@ -73,32 +72,23 @@
             )
             classifiers.append(classifier)
         pkg_toml_config["project"]["classifiers"] = classifiers
         pkg_toml_config["project"]["requires-python"] = requires_python
         await dump.toml(pkg_toml_config, self.pkg_toml_path)  # type: ignore
 
     async def copy_configs(self) -> None:
-        config_files = (
-            ".gitignore",
-            ".pre-commit-config.yaml",
-            ".libcst.codemod.yaml",
-        )
+        config_files = (".gitignore", ".pre-commit-config.yaml", ".libcst.codemod.yaml")
         for config in config_files:
             config_path = self.our_path / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
             if self.pkg_path.stem == "crackerjack":
                 await config_path.write_text(await pkg_config_path.read_text())
                 continue
-            config_text = await config_path.read_text()
-            if config == ".gitignore":
-                await pkg_config_path.write_text(
-                    config_text.replace("crackerjack", self.pkg_name)
-                )
-            run([str(str(self.config.git_path)), "add", config])
+            run([str(self.config.git_path), "add", config])
 
     async def run_interactive(self, hook: str) -> None:
         success: bool = False
         while not success:
             fail = run(
                 [str(self.config.pre_commit_path), "run", hook.lower(), "--all-files"]
             )
@@ -109,84 +99,85 @@
                     continue
                 sys.exit()
             success = True
 
     async def update_pkg_configs(self) -> None:
         await self.copy_configs()
         installed_pkgs = run(
-            [str(str(self.config.pdm_path)), "list", "--freeze"],
+            [str(self.config.pdm_path), "list", "--freeze"],
             capture_output=True,
             text=True,
         ).stdout.splitlines()
         if not len([pkg for pkg in installed_pkgs if "pre-commit" in pkg]):
             print('Installing "pre-commit"...')
             run([str(self.config.pdm_path), "self", "add", "keyring"])
             run([str(self.config.pdm_path), "config", "python.use_venv", "false"])
             run([str(self.config.git_path), "init"])
             run([str(self.config.git_path), "branch", "-m", "main"])
             run([str(self.config.git_path), "add", "pyproject.toml"])
             run([str(self.config.git_path), "add", "pdm.lock"])
             run([str(self.config.pre_commit_path), "install"])
-            run(
-                [
-                    str(str(self.config.git_path)),
-                    "config",
-                    "advice.addIgnoredFile",
-                    "false",
-                ]
-            )
+            run([str(self.config.git_path), "config", "advice.addIgnoredFile", "false"])
         await self.update_pyproject_configs()
 
-    async def process(self, options: t.Any) -> None:
+    async def load_config(self) -> None:
         await self.settings_path.touch(exist_ok=True)
         try:
             self.config = Config(**await load.yaml(self.settings_path))
         except TypeError:
             self.config = Config()
             await dump.yaml(self.config.model_dump(), self.settings_path)
             raise SystemExit("\nPlease configure '.crackerjack.yaml' and try again\n")
+
+    async def run_pre_commit(self) -> None:
+        check_all = run([str(self.config.pre_commit_path), "run", "--all-files"])
+        if check_all.returncode > 0:
+            check_all = run([str(self.config.pre_commit_path), "run", "--all-files"])
+            if check_all.returncode > 0:
+                await aprint("\n\nPre-commit failed. Please fix errors.\n")
+                raise SystemExit()
+
+    async def process(self, options: t.Any) -> None:
+        await self.load_config()
         imp_dir = self.pkg_path / "__pypackages__" / self.config.python_version / "lib"
         sys.path.append(str(imp_dir))
         self.pkg_name = underscore(self.pkg_path.stem.lower())
         self.pkg_dir = self.pkg_path / self.pkg_name
         await self.pkg_dir.mkdir(exist_ok=True)
         await aprint("\nCrackerjacking...\n")
         if not options.do_not_update_configs:
             await self.update_pkg_configs()
-            run([str(str(self.config.pdm_path)), "install"])
+            run([str(self.config.pdm_path), "install"])
         if self.pkg_path.stem == "crackerjack" and options.update_precommit:
             run([str(self.config.pre_commit_path), "autoupdate"])
         if options.interactive:
             for hook in ("refurb", "bandit", "pyright"):
                 await self.run_interactive(hook)
-        check_all = run([str(self.config.pre_commit_path), "run", "--all-files"])
-        if check_all.returncode > 0:
-            check_all = run([str(self.config.pre_commit_path), "run", "--all-files"])
-            if check_all.returncode > 0:
-                await aprint("\n\nPre-commit failed. Please fix errors.\n")
-                raise SystemExit()
-        if options.publish:
-            run([str(str(self.config.pdm_path)), "bump", options.publish])
+        await self.run_pre_commit()
+        for option in (options.publish, options.bump):
+            if option:
+                run([str(self.config.pdm_path), "bump", option])
+                break
         if options.publish:
-            run([str(str(self.config.pdm_path)), "publish"])
+            run([str(self.config.pdm_path), "publish"])
         if options.commit:
             commit_msg = await ainput("\nCommit message: ")
             run(
                 [
-                    str(str(self.config.git_path)),
+                    str(self.config.git_path),
                     "commit",
                     "-m",
-                    f"{commit_msg}",
+                    str(commit_msg),
                     "--no-verify",
                     "--",
                     ".",
                 ]
             )
-            run([str(str(self.config.git_path)), "push", "origin", "main"])
+            run([str(self.config.git_path), "push", "origin", "main"])
         await aprint("\nCrackerjack complete!\n")
 
     async def run(self, options: t.Any) -> None:
         process = asyncio.create_task(self.process(options))
         await process
 
 
-crackerjack_it = Crakerjack().run
+crackerjack_it = Crackerjack().run
```

### Comparing `crackerjack-0.7.9/crackerjack/pyproject.toml` & `crackerjack-0.8.0/crackerjack/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,45 +3,59 @@
     "python.use_venv",
     "true",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = []
 
+[tool.codespell]
+skip = "*/data/*"
+quiet-level = 3
+ignore-words-list = "crate,uptodate"
+
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
-show-source = true
+output-format = "full"
 
-[tool.ruff.isort]
-force-single-line = true
+[tool.ruff.format]
+docstring-code-format = true
 
-[tool.ruff.mccabe]
-max-complexity = 10
+[tool.ruff.lint]
+ignore = [
+    "F821",
+    "D100",
+    "D101",
+    "D102",
+    "D103",
+    "D104",
+    "D107",
+]
+extend-select = [
+    "I",
+    "C901",
+    "D",
+]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.black]
-target-version = [
-    "py312",
-]
-
 [tool.creosote]
 paths = [
     "crackerjack",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
     "pdm-bump",
     "autotyping",
     "pre-commit",
     "pytest",
+    "pdm",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
@@ -69,15 +83,15 @@
 reportUnknownArgumentType = false
 reportPrivateUsage = "warning"
 pythonVersion = "3.12"
 pythonPlatform = "Darwin"
 
 [project]
 name = "Crackerjack"
-version = "0.7.8"
+version = "0.7.36"
 description = "Crackerjack code style"
 requires-python = ">=3.12"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -96,23 +110,24 @@
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: BSD License",
     "Typing :: Typed",
 ]
 dependencies = [
     "click>=8.1.7",
-    "aioconsole>=0.6.2",
+    "aioconsole>=0.7.1",
     "inflection>=0.5.1",
-    "autotyping>=23.3.0",
-    "pre-commit>=3.4.0",
-    "pytest>=7.4.2",
-    "pydantic>=2.4.0",
-    "aiopath>=0.7.5",
-    "acb>=0.3.4",
-    "pdm-bump>=0.7.3",
+    "autotyping>=24.3.0",
+    "pre-commit>=3.7.1",
+    "pytest>=8.2.1",
+    "pydantic>=2.7.1",
+    "aiopath>=0.7.7",
+    "acb>=0.6.0",
+    "pdm-bump>=0.9.0",
+    "pdm>=2.15.2",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.7.9/pyproject.toml` & `crackerjack-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,45 +3,59 @@
     "python.use_venv",
     "true",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = []
 
+[tool.codespell]
+skip = "*/data/*"
+quiet-level = 3
+ignore-words-list = "crate,uptodate"
+
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
-show-source = true
+output-format = "full"
 
-[tool.ruff.isort]
-force-single-line = true
+[tool.ruff.format]
+docstring-code-format = true
 
-[tool.ruff.mccabe]
-max-complexity = 10
+[tool.ruff.lint]
+ignore = [
+    "F821",
+    "D100",
+    "D101",
+    "D102",
+    "D103",
+    "D104",
+    "D107",
+]
+extend-select = [
+    "I",
+    "C901",
+    "D",
+]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.black]
-target-version = [
-    "py312",
-]
-
 [tool.creosote]
 paths = [
     "crackerjack",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
     "pdm-bump",
     "autotyping",
     "pre-commit",
     "pytest",
+    "pdm",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
@@ -69,15 +83,15 @@
 reportUnknownArgumentType = false
 reportPrivateUsage = "warning"
 pythonVersion = "3.12"
 pythonPlatform = "Darwin"
 
 [project]
 name = "Crackerjack"
-version = "0.7.9"
+version = "0.8.0"
 description = "Crackerjack code style"
 requires-python = ">=3.12"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -96,23 +110,24 @@
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: BSD License",
     "Typing :: Typed",
 ]
 dependencies = [
     "click>=8.1.7",
-    "aioconsole>=0.6.2",
+    "aioconsole>=0.7.1",
     "inflection>=0.5.1",
-    "autotyping>=23.3.0",
-    "pre-commit>=3.4.0",
-    "pytest>=7.4.2",
-    "pydantic>=2.4.0",
-    "aiopath>=0.7.5",
-    "acb>=0.3.4",
-    "pdm-bump>=0.7.3",
+    "autotyping>=24.3.0",
+    "pre-commit>=3.7.1",
+    "pytest>=8.2.1",
+    "pydantic>=2.7.1",
+    "aiopath>=0.7.7",
+    "acb>=0.6.0",
+    "pdm-bump>=0.9.0",
+    "pdm>=2.15.2",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.7.9/PKG-INFO` & `crackerjack-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.7.9
+Version: 0.8.0
 Summary: Crackerjack code style
-Keywords: black ruff mypy creosote refurb
+Keywords: black,ruff,mypy,creosote,refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -20,28 +20,30 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://github.com/lesleslie/crackerjack
 Project-URL: Documentation, https://github.com/lesleslie/crackerjack
 Project-URL: Repository, https://github.com/lesleslie/crackerjack
 Requires-Python: >=3.12
 Requires-Dist: click>=8.1.7
-Requires-Dist: aioconsole>=0.6.2
+Requires-Dist: aioconsole>=0.7.1
 Requires-Dist: inflection>=0.5.1
-Requires-Dist: autotyping>=23.3.0
-Requires-Dist: pre-commit>=3.4.0
-Requires-Dist: pytest>=7.4.2
-Requires-Dist: pydantic>=2.4.0
-Requires-Dist: aiopath>=0.7.5
-Requires-Dist: acb>=0.3.4
-Requires-Dist: pdm-bump>=0.7.3
+Requires-Dist: autotyping>=24.3.0
+Requires-Dist: pre-commit>=3.7.1
+Requires-Dist: pytest>=8.2.1
+Requires-Dist: pydantic>=2.7.1
+Requires-Dist: aiopath>=0.7.7
+Requires-Dist: acb>=0.6.0
+Requires-Dist: pdm-bump>=0.9.0
+Requires-Dist: pdm>=2.15.2
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
 
-[![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
+[![Python: 3.12](https://img.shields.io/badge/python-3.12%2B-blue)](https://docs.python.org/3/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 Crackerjack is a python coding style which uses a minimalist approach to produce elegant, easy to read, code.
@@ -91,25 +93,25 @@
 
 - streamlines and standardizes code style across numerous packages
 
 - installs, or updates, a project's pre-commit tools as well as .gitignore & other config files
   to comply with evolving crackerjack standards
 
 - runs the following pre-commit hooks (in order):
-  * various core pre-commit hooks
-  * [black](https://github.com/ambv/black)
-  * ruff
-  * creosote
-  * bandit
-  * flynt
-  * autotyping
-  * refurb
-  * pyright
-  * ruff (again for sanity checking)
-  * black (again for sanity checking)
+  * [pdm-lock-check](https://github.com/pdm-project/pdm)
+  * various core [pre-commit-hooks](https://github.com/pre-commit/pre-commit-hooks)
+  * [ruff](https://github.com/charliermarsh/ruff-pre-commit)
+  * [creosote](https://github.com/fredrikaverpil/creosote)
+  * [flynt](https://github.com/ikamensh/flynt/)
+  * [codespell](https://github.com/codespell-project/codespell)
+  * [autotyping](https://github.com/JelleZijlstra/autotyping)
+  * [refurb](https://github.com/dosisod/refurb)
+  * [bandit](https://github.com/PyCQA/bandit)
+  * [pyright](https://github.com/RobertCraigie/pyright-python)
+  * [ruff](https://github.com/charliermarsh/ruff-pre-commit) (again for sanity checking)
 
 - converts/creates documentation in Markdown (md) (work in progress)
 
 - runs tests and generates pytest mock stubs if needed (work in progress)
 
 - bumps the project version and publishes it to PyPI
 
@@ -119,30 +121,24 @@
 
 (...more what you'd call "guidelines" than actual rules. -Captain Barbossa )
 
 - code is statically typed
 
 - all docstrings, README's, and other documentation is to be done in Markdown (md)
 
-- format with black
-
 - use aiopath.AsyncPath or pathlib.Path not os.path
 
 - import typing as t
 
 - do not capitalize all letters in configuration settings or constants (we diverge from PEP-8 here
  for not other reason than it looks ugly)
 
 - functions that deal with path operations should get passed AsyncPaths or Paths - not strings
 
-- if a class can be a dataclasses.dataclass, pydantic.BaseModel, or msgspec.Struct it should be
-
-- force single line imports (will support isort Vertical Hanging Indent when ruff does)
-
-- use PDM and PEP-582 for dependency management and package building/publishing
+- use PDM and PEP-582(proposed) for dependency management and package building/publishing
 
 - use pdoc and mkdocs for producing documentation
 
 - use pytest for testing
 
 - be compliant with the latest python version within 2 months after release
```

