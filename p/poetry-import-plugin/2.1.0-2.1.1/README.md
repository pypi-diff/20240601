# Comparing `tmp/poetry_import_plugin-2.1.0.tar.gz` & `tmp/poetry_import_plugin-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_import_plugin-2.1.0.tar", max compression
+gzip compressed data, was "poetry_import_plugin-2.1.1.tar", max compression
```

## Comparing `poetry_import_plugin-2.1.0.tar` & `poetry_import_plugin-2.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-20 13:45:56.845976 poetry_import_plugin-2.1.0/LICENSE
--rw-r--r--   0        0        0     3034 2024-05-20 13:45:56.845976 poetry_import_plugin-2.1.0/README.md
--rw-r--r--   0        0        0     1241 2024-05-20 13:45:56.929977 poetry_import_plugin-2.1.0/poetry_import/__init__.py
--rw-r--r--   0        0        0     2077 2024-05-20 13:45:56.929977 poetry_import_plugin-2.1.0/poetry_import/backport.py
--rw-r--r--   0        0        0    15218 2024-05-20 13:45:56.929977 poetry_import_plugin-2.1.0/poetry_import/command.py
--rw-r--r--   0        0        0     4115 2024-05-20 13:46:27.550040 poetry_import_plugin-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4033 1970-01-01 00:00:00.000000 poetry_import_plugin-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-06-01 18:28:27.386900 poetry_import_plugin-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3834 2024-06-01 18:28:27.386900 poetry_import_plugin-2.1.1/README.md
+-rw-r--r--   0        0        0     1241 2024-06-01 18:28:28.882918 poetry_import_plugin-2.1.1/poetry_import/__init__.py
+-rw-r--r--   0        0        0     2077 2024-06-01 18:28:28.882918 poetry_import_plugin-2.1.1/poetry_import/backport.py
+-rw-r--r--   0        0        0    15218 2024-06-01 18:28:28.882918 poetry_import_plugin-2.1.1/poetry_import/command.py
+-rw-r--r--   0        0        0     4122 2024-06-01 18:29:07.775371 poetry_import_plugin-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4847 1970-01-01 00:00:00.000000 poetry_import_plugin-2.1.1/PKG-INFO
```

### Comparing `poetry_import_plugin-2.1.0/LICENSE` & `poetry_import_plugin-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_import_plugin-2.1.0/poetry_import/__init__.py` & `poetry_import_plugin-2.1.1/poetry_import/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_import_plugin-2.1.0/poetry_import/backport.py` & `poetry_import_plugin-2.1.1/poetry_import/backport.py`

 * *Files identical despite different names*

### Comparing `poetry_import_plugin-2.1.0/poetry_import/command.py` & `poetry_import_plugin-2.1.1/poetry_import/command.py`

 * *Files identical despite different names*

### Comparing `poetry_import_plugin-2.1.0/pyproject.toml` & `poetry_import_plugin-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "poetry-import-plugin"
-version = "2.1.0"
+version = "2.1.1"
 description = "Convert requirements.txt to pyproject.toml"
 authors = ["Ben Chen <benbenbang@github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-repository = "https://github.com/benbenbang/poetry-import"
+repository = "https://github.com/benbenbang/poetry-import-plugin"
 keywords = ["poetry", "pyproject", "toml", "requirements", "import"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.7",
```

### Comparing `poetry_import_plugin-2.1.0/PKG-INFO` & `poetry_import_plugin-2.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: poetry-import-plugin
-Version: 2.1.0
+Version: 2.1.1
 Summary: Convert requirements.txt to pyproject.toml
-Home-page: https://github.com/benbenbang/poetry-import
+Home-page: https://github.com/benbenbang/poetry-import-plugin
 License: Apache-2.0
 Keywords: poetry,pyproject,toml,requirements,import
 Author: Ben Chen
 Author-email: benbenbang@github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,19 +15,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Project-URL: Repository, https://github.com/benbenbang/poetry-import
+Project-URL: Repository, https://github.com/benbenbang/poetry-import-plugin
 Description-Content-Type: text/markdown
 
 # Poetry Import Plugin
 
+ [![PyPI version](https://badge.fury.io/py/poetry-import-plugin.svg)](https://badge.fury.io/py/poetry-import-plugin) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-import-plugin) [![GitHub issues](https://img.shields.io/github/issues/benbenbang/poetry-import-plugin)](https://github.com/benbenbang/poetry-import-plugin/issues) ![pre-commit enable](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white) [![main](https://github.com/benbenbang/poetry-import-plugin/actions/workflows/main.yml/badge.svg)](https://github.com/benbenbang/poetry-import-plugin/actions/workflows/main.yml) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://semver.org/)
+
+
 `poetry-import-plugin` is a Python plugin for Poetry that simplifies the process of importing dependencies from `requirements.txt` files into a Poetry project. It allows you to integrate dependencies into specified dependency groups within the project's `pyproject.toml` file, optionally applying constraints from a constraints file. This plugin also supports updating the Poetry lock file and installing dependencies.
 
 ps. It is renamed from `Req2Toml`
 
 
 
 
@@ -44,18 +47,18 @@
 
 Currently (as of 2024), poetry provides three ways to install the plugin:
 
 #### With `pipx inject`
 
 ```bash
 # To install
-pipx inject poetry-import-plugin
+pipx inject poetry poetry-import-plugin
 
 # To uninstall
-pipx uninject poetry-import-plugin
+pipx uninject poetry poetry-import-plugin
 ```
 
 
 
 #### With `pip`
 
 ```bash
@@ -71,15 +74,15 @@
 #### The `self add` command (not recommended for Windows users)
 
 ```bash
 # To install
 poetry self add poetry-import-plugin
 
 # To uninstall
-poetry self remove poetry-plugin
+poetry self remove poetry-import-plugin
 ```
 
 
 
 ## Usage
 
 The `import` command can be used to import dependencies from `requirements.txt` files into your Poetry project. Below are the available options and arguments:
```

