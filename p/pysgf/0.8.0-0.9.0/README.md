# Comparing `tmp/pysgf-0.8.0.tar.gz` & `tmp/pysgf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysgf-0.8.0.tar", last modified: Mon Jun  8 16:13:01 2020, max compression
+gzip compressed data, was "pysgf-0.9.0.tar", max compression
```

## Comparing `pysgf-0.8.0.tar` & `pysgf-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1068 2020-06-08 16:12:14.212464 pysgf-0.8.0/LICENSE
--rw-r--r--   0        0        0      713 2020-06-08 16:12:14.212464 pysgf-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       56 2020-06-08 16:12:14.212464 pysgf-0.8.0/pysgf/__init__.py
--rw-r--r--   0        0        0    11824 2020-06-08 16:12:14.216464 pysgf-0.8.0/pysgf/parser.py
--rw-r--r--   0        0        0      489 2020-06-08 16:13:01.678970 pysgf-0.8.0/setup.py
--rw-r--r--   0        0        0      322 2020-06-08 16:13:01.679285 pysgf-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-06-01 10:11:33.089737 pysgf-0.9.0/LICENSE
+-rw-r--r--   0        0        0      735 2024-06-01 10:11:33.089737 pysgf-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-06-01 10:11:33.089737 pysgf-0.9.0/pysgf/__init__.py
+-rw-r--r--   0        0        0    11824 2024-06-01 10:11:33.089737 pysgf-0.9.0/pysgf/parser.py
+-rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 pysgf-0.9.0/PKG-INFO
```

### Comparing `pysgf-0.8.0/LICENSE` & `pysgf-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysgf-0.8.0/pyproject.toml` & `pysgf-0.9.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "pysgf"
-version = "0.8.0"
+version = "0.9.0"
 description = "Simple SGF parser"
 authors = ["Sander Land"]
 
 [tool.black]
 line-length=120
-target_version = ['py37']
+target_version = ['py39']
 include = '\.py$'
 
 [tool.isort]
 line_length=120                # corresponds to -w  flag
 multi_line_output=3            # corresponds to -m  flag
 include_trailing_comma=true    # corresponds to -tc flag
 skip_glob = '^((?!py$).)*$'    # sort all Python files
 known_third_party = []
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.9"
 
-[tool.poetry.dev-dependencies]
-black = "^19.10b0"
-isort = "^4.3"
-pytest = "^5.2"
-sphinx = "^2.4.4"
-sphinx-rtd-theme = "^0.4.3"
-twine = "^3.1.1"
+[tool.poetry.group.dev.dependencies]
+black = "^24.4.2"
+isort = "^5.13.2"
+pytest = "^8.2.1"
+sphinx = "^7.3.7"
+sphinx-rtd-theme = "^2.0.0"
+twine = "^5.1.0"
 
 [build-system]
-requires = ["poetry>=1.0"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.1.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pysgf-0.8.0/pysgf/parser.py` & `pysgf-0.9.0/pysgf/parser.py`

 * *Files identical despite different names*

