# Comparing `tmp/docstub-0.1.0.tar.gz` & `tmp/docstub-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstub-0.1.0.tar", last modified: Mon Apr 29 14:43:15 2024, max compression
+gzip compressed data, was "docstub-0.2.1.tar", last modified: Fri May 31 23:40:04 2024, max compression
```

## Comparing `docstub-0.1.0.tar` & `docstub-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,42 @@
-drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-04-29 14:43:15.040340 docstub-0.1.0/
--rw-r--r--   0 lg        (1000) lg        (1000)      944 2024-04-29 14:26:40.000000 docstub-0.1.0/.gitignore
--rw-r--r--   0 lg        (1000) lg        (1000)     1469 2024-04-29 14:30:02.000000 docstub-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 lg        (1000) lg        (1000)     1522 2024-04-29 13:14:59.000000 docstub-0.1.0/LICENSE
--rw-r--r--   0 lg        (1000) lg        (1000)     3096 2024-04-29 14:43:15.040340 docstub-0.1.0/PKG-INFO
--rw-r--r--   0 lg        (1000) lg        (1000)      435 2024-04-29 14:24:09.000000 docstub-0.1.0/README.md
--rw-r--r--   0 lg        (1000) lg        (1000)     1836 2024-04-29 14:24:09.000000 docstub-0.1.0/pyproject.toml
--rw-r--r--   0 lg        (1000) lg        (1000)       38 2024-04-29 14:43:15.040340 docstub-0.1.0/setup.cfg
-drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-04-29 14:43:15.037006 docstub-0.1.0/src/
-drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-04-29 14:43:15.037006 docstub-0.1.0/src/docstub/
--rw-r--r--   0 lg        (1000) lg        (1000)      194 2024-04-29 14:24:09.000000 docstub-0.1.0/src/docstub/__init__.py
--rw-r--r--   0 lg        (1000) lg        (1000)      411 2024-04-29 14:43:14.000000 docstub-0.1.0/src/docstub/_version.py
-drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-04-29 14:43:15.037006 docstub-0.1.0/src/docstub.egg-info/
--rw-r--r--   0 lg        (1000) lg        (1000)     3096 2024-04-29 14:43:14.000000 docstub-0.1.0/src/docstub.egg-info/PKG-INFO
--rw-r--r--   0 lg        (1000) lg        (1000)      289 2024-04-29 14:43:15.000000 docstub-0.1.0/src/docstub.egg-info/SOURCES.txt
--rw-r--r--   0 lg        (1000) lg        (1000)        1 2024-04-29 14:43:14.000000 docstub-0.1.0/src/docstub.egg-info/dependency_links.txt
--rw-r--r--   0 lg        (1000) lg        (1000)       23 2024-04-29 14:43:14.000000 docstub-0.1.0/src/docstub.egg-info/requires.txt
--rw-r--r--   0 lg        (1000) lg        (1000)        8 2024-04-29 14:43:14.000000 docstub-0.1.0/src/docstub.egg-info/top_level.txt
+drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-05-31 23:40:04.388698 docstub-0.2.1/
+-rw-r--r--   0 lg        (1000) lg        (1000)      944 2024-04-29 14:26:40.000000 docstub-0.2.1/.gitignore
+-rw-r--r--   0 lg        (1000) lg        (1000)     1529 2024-05-31 23:18:11.000000 docstub-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 lg        (1000) lg        (1000)     1522 2024-04-29 13:14:59.000000 docstub-0.2.1/LICENSE
+-rw-r--r--   0 lg        (1000) lg        (1000)     4758 2024-05-31 23:40:04.388698 docstub-0.2.1/PKG-INFO
+-rw-r--r--   0 lg        (1000) lg        (1000)     1742 2024-05-31 22:55:39.000000 docstub-0.2.1/README.md
+drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-05-31 23:40:04.382032 docstub-0.2.1/examples/
+-rw-r--r--   0 lg        (1000) lg        (1000)      670 2024-05-31 22:49:02.000000 docstub-0.2.1/examples/docstub.toml
+drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-05-31 23:40:04.385365 docstub-0.2.1/examples/example_pkg/
+-rw-r--r--   0 lg        (1000) lg        (1000)      167 2024-05-31 22:49:02.000000 docstub-0.2.1/examples/example_pkg/__init__.py
+-rw-r--r--   0 lg        (1000) lg        (1000)     2021 2024-05-31 22:49:02.000000 docstub-0.2.1/examples/example_pkg/_basic.py
+-rw-r--r--   0 lg        (1000) lg        (1000)      115 2024-05-31 22:49:02.000000 docstub-0.2.1/examples/example_pkg/_compiled.pyi
+-rw-r--r--   0 lg        (1000) lg        (1000)      896 2024-05-31 23:28:48.000000 docstub-0.2.1/examples/example_pkg/_numpy.py
+drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-05-31 23:40:04.385365 docstub-0.2.1/examples/example_pkg-stubs/
+-rw-r--r--   0 lg        (1000) lg        (1000)      135 2024-05-31 23:38:38.000000 docstub-0.2.1/examples/example_pkg-stubs/__init__.pyi
+-rw-r--r--   0 lg        (1000) lg        (1000)      974 2024-05-31 23:38:38.000000 docstub-0.2.1/examples/example_pkg-stubs/_basic.pyi
+-rw-r--r--   0 lg        (1000) lg        (1000)      115 2024-05-31 23:38:38.000000 docstub-0.2.1/examples/example_pkg-stubs/_compiled.pyi
+-rw-r--r--   0 lg        (1000) lg        (1000)      511 2024-05-31 23:38:38.000000 docstub-0.2.1/examples/example_pkg-stubs/_numpy.pyi
+-rw-r--r--   0 lg        (1000) lg        (1000)     2150 2024-05-31 23:11:43.000000 docstub-0.2.1/pyproject.toml
+-rw-r--r--   0 lg        (1000) lg        (1000)       38 2024-05-31 23:40:04.388698 docstub-0.2.1/setup.cfg
+drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-05-31 23:40:04.382032 docstub-0.2.1/src/
+drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-05-31 23:40:04.385365 docstub-0.2.1/src/docstub/
+-rw-r--r--   0 lg        (1000) lg        (1000)      194 2024-04-29 14:24:09.000000 docstub-0.2.1/src/docstub/__init__.py
+-rw-r--r--   0 lg        (1000) lg        (1000)       62 2024-05-31 22:49:02.000000 docstub-0.2.1/src/docstub/__main__.py
+-rw-r--r--   0 lg        (1000) lg        (1000)     3938 2024-05-31 22:49:02.000000 docstub-0.2.1/src/docstub/_analysis.py
+-rw-r--r--   0 lg        (1000) lg        (1000)     2765 2024-05-31 22:49:02.000000 docstub-0.2.1/src/docstub/_cli.py
+-rw-r--r--   0 lg        (1000) lg        (1000)      971 2024-05-31 22:49:02.000000 docstub-0.2.1/src/docstub/_config.py
+-rw-r--r--   0 lg        (1000) lg        (1000)     8892 2024-05-31 23:31:57.000000 docstub-0.2.1/src/docstub/_docstrings.py
+-rw-r--r--   0 lg        (1000) lg        (1000)     8265 2024-05-31 22:49:02.000000 docstub-0.2.1/src/docstub/_stubs.py
+-rw-r--r--   0 lg        (1000) lg        (1000)        0 2024-05-31 22:49:02.000000 docstub-0.2.1/src/docstub/_utils.py
+-rw-r--r--   0 lg        (1000) lg        (1000)      411 2024-05-31 23:40:03.000000 docstub-0.2.1/src/docstub/_version.py
+-rw-r--r--   0 lg        (1000) lg        (1000)     4311 2024-05-31 22:49:02.000000 docstub-0.2.1/src/docstub/default_config.toml
+-rw-r--r--   0 lg        (1000) lg        (1000)     1474 2024-05-31 22:49:02.000000 docstub-0.2.1/src/docstub/doctype.lark
+drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-05-31 23:40:04.385365 docstub-0.2.1/src/docstub.egg-info/
+-rw-r--r--   0 lg        (1000) lg        (1000)     4758 2024-05-31 23:40:04.000000 docstub-0.2.1/src/docstub.egg-info/PKG-INFO
+-rw-r--r--   0 lg        (1000) lg        (1000)      874 2024-05-31 23:40:04.000000 docstub-0.2.1/src/docstub.egg-info/SOURCES.txt
+-rw-r--r--   0 lg        (1000) lg        (1000)        1 2024-05-31 23:40:04.000000 docstub-0.2.1/src/docstub.egg-info/dependency_links.txt
+-rw-r--r--   0 lg        (1000) lg        (1000)       50 2024-05-31 23:40:04.000000 docstub-0.2.1/src/docstub.egg-info/entry_points.txt
+-rw-r--r--   0 lg        (1000) lg        (1000)      156 2024-05-31 23:40:04.000000 docstub-0.2.1/src/docstub.egg-info/requires.txt
+-rw-r--r--   0 lg        (1000) lg        (1000)        8 2024-05-31 23:40:04.000000 docstub-0.2.1/src/docstub.egg-info/top_level.txt
+drwxr-xr-x   0 lg        (1000) lg        (1000)        0 2024-05-31 23:40:04.385365 docstub-0.2.1/tests/
+-rw-r--r--   0 lg        (1000) lg        (1000)        0 2024-05-31 22:49:02.000000 docstub-0.2.1/tests/test_dev.py
```

### Comparing `docstub-0.1.0/.gitignore` & `docstub-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `docstub-0.1.0/.pre-commit-config.yaml` & `docstub-0.2.1/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Install pre-commit hooks via "pre-commit install"
 
+exclude: |
+    (?x)^(
+        examples/.*-stubs/.*|
+    )$
+
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "2c9f875913ee60ca25ce70243dc24d5b6415598c"  # frozen: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-ast
       - id: check-builtin-literals
```

### Comparing `docstub-0.1.0/LICENSE` & `docstub-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docstub-0.1.0/pyproject.toml` & `docstub-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,39 +22,53 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
-dependencies = []
+dependencies = [
+  "numpydoc >=1.7.0",
+  "click >=8.1.7",
+  "libcst >=1.3.1",
+  "lark >=1.1.9",
+]
 
 [project.optional-dependencies]
+optional = [
+  "black >=24.4.2",
+  "isort >=5.13.2",
+]
 dev = [
   "pre-commit >=3.7",
 ]
+test = [
+  "pytest >=5.0.0",
+  "coverage >=7.5.0",
+]
 
 [project.urls]
 Home = "https://github.com/lagru/docstub"
 
+[project.scripts]
+docstub = "docstub.__main__:main"
+
 
 [tool.setuptools_scm]
 write_to = "src/docstub/_version.py"
 
 
 [tool.ruff]
 src = ["src"]
 
 [tool.ruff.lint]
 extend-select = [
   "B",        # flake8-bugbear
   "I",        # isort
-  "ARG",      # flake8-unused-arguments
   "C4",       # flake8-comprehensions
-  "EM",       # flake8-errmsg
   "ICN",      # flake8-import-conventions
   "G",        # flake8-logging-format
   "PGH",      # pygrep-hooks
   "PIE",      # flake8-pie
   "PL",       # pylint
   "PT",       # flake8-pytest-style
   "PTH",      # flake8-use-pathlib
@@ -66,8 +80,10 @@
   "YTT",      # flake8-2020
   "EXE",      # flake8-executable
 ]
 ignore = [
   "PLR09",    # Too many <...>
   "PLR2004",  # Magic value used in comparison
   "ISC001",   # Conflicts with formatter
+  "RET504",   # Assignment before `return` statement facilitates debugging
+  "PTH123",   # Using builtin open() instead of Path.open() is fine
 ]
```

