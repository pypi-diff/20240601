# Comparing `tmp/req_update-2.6.0.tar.gz` & `tmp/req_update-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "req_update-2.6.0.tar", last modified: Mon May 27 00:43:25 2024, max compression
+gzip compressed data, was "req_update-2.7.0.tar", last modified: Sat Jun  1 14:35:23 2024, max compression
```

## Comparing `req_update-2.6.0.tar` & `req_update-2.7.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 00:43:25.524181 req_update-2.6.0/
--rw-r--r--   0 root         (0) root         (0)     6337 2024-05-27 00:41:46.000000 req_update-2.6.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1068 2024-05-27 00:41:46.000000 req_update-2.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-27 00:41:46.000000 req_update-2.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3428 2024-05-27 00:43:25.520181 req_update-2.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2291 2024-05-27 00:41:46.000000 req_update-2.6.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1751 2024-05-27 00:41:46.000000 req_update-2.6.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 00:43:25.520181 req_update-2.6.0/req_update/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4359 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/docker.py
--rw-r--r--   0 root         (0) root         (0)      154 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/drone.py
--rw-r--r--   0 root         (0) root         (0)     5343 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/gitsubmodule.py
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/go.py
--rw-r--r--   0 root         (0) root         (0)     5800 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/node.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/py.typed
--rw-r--r--   0 root         (0) root         (0)     8506 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/python.py
--rwxr-xr-x   0 root         (0) root         (0)     4362 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/req_update.py
--rw-r--r--   0 root         (0) root         (0)     7610 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 00:43:25.520181 req_update-2.6.0/req_update.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3428 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 00:43:25.524181 req_update-2.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 14:35:23.166483 req_update-2.7.0/
+-rw-r--r--   0 root         (0) root         (0)     6484 2024-06-01 14:34:08.000000 req_update-2.7.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-06-01 14:34:08.000000 req_update-2.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2024-06-01 14:34:08.000000 req_update-2.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3428 2024-06-01 14:35:23.166483 req_update-2.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-06-01 14:34:08.000000 req_update-2.7.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1721 2024-06-01 14:34:08.000000 req_update-2.7.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 14:35:23.162483 req_update-2.7.0/req_update/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4623 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/docker.py
+-rw-r--r--   0 root         (0) root         (0)      182 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/drone.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/githubworkflow.py
+-rw-r--r--   0 root         (0) root         (0)     5343 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/gitsubmodule.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/go.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/node.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9846 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/python.py
+-rwxr-xr-x   0 root         (0) root         (0)     4443 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/req_update.py
+-rw-r--r--   0 root         (0) root         (0)     7610 2024-06-01 14:34:08.000000 req_update-2.7.0/req_update/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 14:35:23.166483 req_update-2.7.0/req_update.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3428 2024-06-01 14:35:23.000000 req_update-2.7.0/req_update.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2024-06-01 14:35:23.000000 req_update-2.7.0/req_update.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 14:35:23.000000 req_update-2.7.0/req_update.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-06-01 14:35:23.000000 req_update-2.7.0/req_update.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-06-01 14:35:23.000000 req_update-2.7.0/req_update.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-06-01 14:35:23.000000 req_update-2.7.0/req_update.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 14:35:23.166483 req_update-2.7.0/setup.cfg
```

### Comparing `req_update-2.6.0/CHANGELOG.md` & `req_update-2.7.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGELOG
 =========
 
+2.7.0 (2024-06-01)
+------------------
+
+ - Support updating github actions
+ - Vertically align comments for python updates
+ - Update dependencies
+
+
 2.6.0 (2024-05-26)
 ------------------
 
  - Change check_repository_cleanliness to return a bool rather than raise an exception
  - Add a ignore-cleanliness CLI flag
  - Fix update warnings in dry-mode
  - Update dependencies
```

### Comparing `req_update-2.6.0/LICENSE` & `req_update-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `req_update-2.6.0/PKG-INFO` & `req_update-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: req-update
-Version: 2.6.0
+Version: 2.7.0
 Summary: Update python, node, go, docker, and other dependencies
 Author-email: Albert Wang <git@albertyw.com>
 License: MIT
 Project-URL: Homepage, https://github.com/albertyw/req-update
 Keywords: dependencies
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
-Requires-Dist: coverage==7.5.2; extra == "test"
-Requires-Dist: ruff==0.4.5; extra == "test"
+Requires-Dist: coverage==7.5.3; extra == "test"
+Requires-Dist: ruff==0.4.7; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 
 # req-update
 
 [![PyPI](https://img.shields.io/pypi/v/req-update)](https://pypi.org/project/req-update/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/req-update)
 ![PyPI - License](https://img.shields.io/pypi/l/req-update)
```

### Comparing `req_update-2.6.0/README.md` & `req_update-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `req_update-2.6.0/pyproject.toml` & `req_update-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 ]
 dependencies = []
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 test = [
     # Testing
-    "coverage==7.5.2",                  # Test coverage
-    "ruff==0.4.5",                      # Python linter
+    "coverage==7.5.3",        # Test coverage
+    "ruff==0.4.7",            # Python linter
 
     # Types
-    "mypy==1.10.0",                     # Static typing
+    "mypy==1.10.0",           # Static typing
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/albertyw/req-update"
 
 [project.scripts]
 req_update = "req_update.req_update:main"
```

### Comparing `req_update-2.6.0/req_update/docker.py` & `req_update-2.7.0/req_update/docker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 import json
 from pathlib import Path
+import re
 import subprocess
 from urllib import request
 from urllib.error import HTTPError
 
 from req_update.util import Updater
 
 
 class Docker(Updater):
-    UPDATE_FILE = 'Dockerfile'
+    UPDATE_FILE = re.compile(r'Dockerfile$')
     LINE_HEADER = 'FROM'
+    DEPENDENCY_VERSION_SEPARATOR = ':'
 
     def check_applicable(self) -> bool:
         return len(self.get_update_files()) > 0
 
     def get_update_files(self) -> list[Path]:
         command = ['git', 'ls-files']
         try:
             shell = self.util.execute_shell(command, True)
         except subprocess.CalledProcessError:
             return []
         files = [Path(f) for f in shell.stdout.split('\n')]
-        files = [f for f in files if f.name == self.UPDATE_FILE]
+        files = [f for f in files if self.UPDATE_FILE.match(str(f))]
         return files
 
     def update_dependencies(self) -> bool:
         """
         Update dependencies
         Return if updates were made
         """
@@ -57,21 +59,24 @@
         lines = [line.strip('\n') for line in lines]
         return lines
 
     def attempt_update_image(self, line: str) -> tuple[str, str, str]:
         if not line.strip().startswith(self.LINE_HEADER):
             return line, '', ''
         base_image = line.split()[1]
-        if base_image.count(':') != 1:
+        if base_image.count(self.DEPENDENCY_VERSION_SEPARATOR) != 1:
             return line, base_image, ''
-        dependency = base_image.split(':')[0]
-        version = base_image.split(':')[1]
+        dependency = base_image.split(self.DEPENDENCY_VERSION_SEPARATOR)[0]
+        version = base_image.split(self.DEPENDENCY_VERSION_SEPARATOR)[1]
         new_version = self.find_updated_version(dependency, version)
         if new_version:
-            line = line.replace(':' + version, ':' + new_version)
+            line = line.replace(
+                self.DEPENDENCY_VERSION_SEPARATOR + version,
+                self.DEPENDENCY_VERSION_SEPARATOR + new_version,
+            )
         return line, dependency, new_version
 
     def find_updated_version(self, dependency: str, original_version: str) -> str:
         if original_version == 'latest':
             self.util.warn('Cannot update docker image when using "latest"')
             return ''
         if dependency.count('/') == 1:
```

### Comparing `req_update-2.6.0/req_update/gitsubmodule.py` & `req_update-2.7.0/req_update/gitsubmodule.py`

 * *Files identical despite different names*

### Comparing `req_update-2.6.0/req_update/go.py` & `req_update-2.7.0/req_update/go.py`

 * *Files identical despite different names*

### Comparing `req_update-2.6.0/req_update/node.py` & `req_update-2.7.0/req_update/node.py`

 * *Files identical despite different names*

### Comparing `req_update-2.6.0/req_update/python.py` & `req_update-2.7.0/req_update/python.py`

 * *Files 18% similar despite different names*

```diff
@@ -153,51 +153,61 @@
         boolean for whether the lines have been updated
         """
         if file_type == REQUIREMENTS:
             line_regex = PYTHON_REQUIREMENTS_LINE_REGEX
         elif file_type == PYPROJECT:
             line_regex = PYTHON_PYPROJECT_LINE_REGEX
         dependency = dependency.replace('_', '-')
+        updated = False
         for i, line in enumerate(lines):
             match = line_regex.match(line.strip())
             if not match:
                 continue
             dependency_file = match.group('name').replace('_', '-').lower()
             dependency_update = dependency.lower()
             if dependency_file != dependency_update:
                 continue
             old_version = match.group('version')
             old_spacer = match.group('spacer')
-            if old_spacer:
-                spacing = len(old_version) + len(old_spacer) - len(version)
-                if spacing <= 1:
-                    spacing = 10 - len(version) % 10 + 1
-                spacer = ' ' * (spacing - 1) + '#'
-            else:
-                spacer = ''
             if file_type == PYPROJECT:
-                spacer = ',' + spacer[1:]
+                old_spacer = ',' + old_spacer[1:]
             if file_type == REQUIREMENTS:
                 new_line = line_regex.sub(
-                    r'\g<1>\g<2>%s%s' % (version, spacer),
+                    r'\g<1>\g<2>%s%s' % (version, old_spacer),
                     line,
                 )
             elif file_type == PYPROJECT:
                 new_line = line_regex.sub(
-                    r'"\g<1>\g<2>%s"%s' % (version, spacer),
+                    r'"\g<1>\g<2>%s"%s' % (version, old_spacer),
                     line,
                 )
             if line == new_line:
                 continue
             self.util.check_major_version_update(
                 dependency, old_version, version,
             )
             lines[i] = new_line
-            return True
-        return False
+            updated = True
+        if not updated:
+            return updated
+        # Vertically align comments
+        comment_alignment = Python.get_comment_alignment(lines, file_type)
+        for i, line in enumerate(lines):
+            if '#' not in line:
+                continue
+            if line_regex.search(line) is None:
+                continue
+            new_line = line
+            while new_line.find('#') != comment_alignment:
+                if new_line.find('#') < comment_alignment:
+                    new_line = new_line.replace('#', ' #')
+                else:
+                    new_line = new_line.replace(' #', '#')
+            lines[i] = new_line
+        return updated
 
     def install_updates(self) -> None:
         """Install requirements updates"""
         for updated_file in self.updated_files:
             if updated_file in REQUIREMENTS_FILES:
                 command = ['pip', 'install', '-r', updated_file]
                 self.util.execute_shell(command, False)
@@ -220,7 +230,30 @@
                     match = PYPROJECT_OPTIONAL_DEPS_REGEX.match(line)
                     if not match:
                         continue
                     optional = match.group(1)
                     command = ['pip', 'install', '-e', '.[%s]' % optional]
                     self.util.execute_shell(command, False)
             self.util.log('Installing updated packages in %s' % updated_file)
+
+    @staticmethod
+    def get_comment_alignment(lines: list[str], file_type: str) -> int:
+        max_length = 0
+        for line in lines:
+            if '#' not in line:
+                continue
+            length = 1 # One whitespace before comments
+            if file_type == REQUIREMENTS:
+                match = PYTHON_REQUIREMENTS_LINE_REGEX.search(line)
+            elif file_type == PYPROJECT:
+                match = PYTHON_PYPROJECT_LINE_REGEX.search(line)
+                length += 3 # Account for additional quotes and comma
+            if not match:
+                continue
+            length += match.start() # Account for indentation
+            length += len(match.group(1) + match.group(2) + match.group(3))
+            if length > max_length:
+                max_length = length
+        alignment = max_length
+        if alignment % 10 != 0:
+            alignment += 10 - alignment % 10
+        return alignment
```

### Comparing `req_update-2.6.0/req_update/req_update.py` & `req_update-2.7.0/req_update/req_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,33 +9,35 @@
 
 current_path = pathlib.Path(os.path.dirname(os.path.abspath(__file__)))
 parent_path = current_path.parent.resolve()
 sys.path.insert(0, str(parent_path))
 
 from req_update.docker import Docker  # NOQA
 from req_update.drone import Drone  # NOQA
+from req_update.githubworkflow import GithubWorkflow  # NOQA
 from req_update.gitsubmodule import GitSubmodule  # NOQA
 from req_update.go import Go  # NOQA
 from req_update.node import Node  # NOQA
 from req_update.python import Python  # NOQA
 from req_update.util import Updater, Util  # NOQA
 
 
-VERSION = (2, 6, 0)
+VERSION = (2, 7, 0)
 __version__ = '.'.join(map(str, VERSION))
 
 
 DESCRIPTION = (
     'Update python, go, node, and git submodule dependencies for your '
     'project with git integration\n\n'
     'https://github.com/albertyw/req-update'
 )
 UPDATERS: list[type[Updater]] = [
     Docker,
     Drone,
+    GithubWorkflow,
     GitSubmodule,
     Go,
     Node,
     Python,
 ]
```

### Comparing `req_update-2.6.0/req_update/util.py` & `req_update-2.7.0/req_update/util.py`

 * *Files identical despite different names*

### Comparing `req_update-2.6.0/req_update.egg-info/PKG-INFO` & `req_update-2.7.0/req_update.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: req-update
-Version: 2.6.0
+Version: 2.7.0
 Summary: Update python, node, go, docker, and other dependencies
 Author-email: Albert Wang <git@albertyw.com>
 License: MIT
 Project-URL: Homepage, https://github.com/albertyw/req-update
 Keywords: dependencies
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
-Requires-Dist: coverage==7.5.2; extra == "test"
-Requires-Dist: ruff==0.4.5; extra == "test"
+Requires-Dist: coverage==7.5.3; extra == "test"
+Requires-Dist: ruff==0.4.7; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 
 # req-update
 
 [![PyPI](https://img.shields.io/pypi/v/req-update)](https://pypi.org/project/req-update/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/req-update)
 ![PyPI - License](https://img.shields.io/pypi/l/req-update)
```

