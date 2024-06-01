# Comparing `tmp/css_colors_stats-0.0.2.tar.gz` & `tmp/css_colors_stats-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "css_colors_stats-0.0.2.tar", max compression
+gzip compressed data, was "css_colors_stats-0.0.3.tar", max compression
```

## Comparing `css_colors_stats-0.0.2.tar` & `css_colors_stats-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      822 2024-06-01 16:36:41.900781 css_colors_stats-0.0.2/README.md
--rw-r--r--   0        0        0      376 2024-06-01 16:36:41.900781 css_colors_stats-0.0.2/css_colors_stats/__init__.py
--rw-r--r--   0        0        0     1343 2024-06-01 16:36:41.900781 css_colors_stats-0.0.2/css_colors_stats/core.py
--rw-r--r--   0        0        0     1166 2024-06-01 16:36:41.900781 css_colors_stats-0.0.2/css_colors_stats/html.py
--rw-r--r--   0        0        0     3026 2024-06-01 16:36:41.900781 css_colors_stats-0.0.2/css_colors_stats/parser.py
--rw-r--r--   0        0        0      544 2024-06-01 16:36:41.900781 css_colors_stats-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 css_colors_stats-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      904 2024-06-01 16:55:04.557760 css_colors_stats-0.0.3/README.md
+-rw-r--r--   0        0        0      376 2024-06-01 16:55:04.557760 css_colors_stats-0.0.3/css_colors_stats/__init__.py
+-rw-r--r--   0        0        0     1343 2024-06-01 16:55:04.557760 css_colors_stats-0.0.3/css_colors_stats/core.py
+-rw-r--r--   0        0        0     1166 2024-06-01 16:55:04.557760 css_colors_stats-0.0.3/css_colors_stats/html.py
+-rw-r--r--   0        0        0     3026 2024-06-01 16:55:04.557760 css_colors_stats-0.0.3/css_colors_stats/parser.py
+-rw-r--r--   0        0        0      544 2024-06-01 16:55:04.561760 css_colors_stats-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 css_colors_stats-0.0.3/PKG-INFO
```

### Comparing `css_colors_stats-0.0.2/README.md` & `css_colors_stats-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # css-colors-stats
-
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/css-colors-stats) ![PyPI - Version](https://img.shields.io/pypi/v/css-colors-stats)
 [![Deployment](https://github.com/giocaizzi/css-colors-stats/actions/workflows/deployment.yml/badge.svg)](https://github.com/giocaizzi/css-colors-stats/actions/workflows/deployment.yml)
 
 Quickly **extract and count colors from CSS files** using a *python CLI tool*.
 
 Export result to:
 - `json`
 - `html`
@@ -16,17 +16,15 @@
 - `hsla`
 
 ## Installation
 
 Clone this repo and install it with *pip*.
 
 ```shell
-git clone https://github.com/giocaizzi/css-colors-stats
-pip install .
-rm -rf css-colors-stats
+pip install css-colors-stats
 ```
 
 ## Usage
 
 ```shell
 css-colors-stats [-h] [--html] filepath
 ```
```

### Comparing `css_colors_stats-0.0.2/css_colors_stats/core.py` & `css_colors_stats-0.0.3/css_colors_stats/core.py`

 * *Files identical despite different names*

### Comparing `css_colors_stats-0.0.2/css_colors_stats/html.py` & `css_colors_stats-0.0.3/css_colors_stats/html.py`

 * *Files identical despite different names*

### Comparing `css_colors_stats-0.0.2/css_colors_stats/parser.py` & `css_colors_stats-0.0.3/css_colors_stats/parser.py`

 * *Files identical despite different names*

### Comparing `css_colors_stats-0.0.2/pyproject.toml` & `css_colors_stats-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "css-colors-stats"
-version = "0.0.2"
+version = "0.0.3"
 description = "Quickly extract and count colors from CSS files."
 authors = ["Giorgio Caizzi <giorgio.caizzi@jakala.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `css_colors_stats-0.0.2/PKG-INFO` & `css_colors_stats-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: css-colors-stats
-Version: 0.0.2
+Version: 0.0.3
 Summary: Quickly extract and count colors from CSS files.
 Author: Giorgio Caizzi
 Author-email: giorgio.caizzi@jakala.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # css-colors-stats
-
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/css-colors-stats) ![PyPI - Version](https://img.shields.io/pypi/v/css-colors-stats)
 [![Deployment](https://github.com/giocaizzi/css-colors-stats/actions/workflows/deployment.yml/badge.svg)](https://github.com/giocaizzi/css-colors-stats/actions/workflows/deployment.yml)
 
 Quickly **extract and count colors from CSS files** using a *python CLI tool*.
 
 Export result to:
 - `json`
 - `html`
@@ -30,17 +30,15 @@
 - `hsla`
 
 ## Installation
 
 Clone this repo and install it with *pip*.
 
 ```shell
-git clone https://github.com/giocaizzi/css-colors-stats
-pip install .
-rm -rf css-colors-stats
+pip install css-colors-stats
 ```
 
 ## Usage
 
 ```shell
 css-colors-stats [-h] [--html] filepath
 ```
```

