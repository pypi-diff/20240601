# Comparing `tmp/playwright_html_renderer-0.1.tar.gz` & `tmp/playwright_html_renderer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright_html_renderer-0.1.tar", last modified: Sat Jun  1 18:51:32 2024, max compression
+gzip compressed data, was "playwright_html_renderer-0.2.tar", last modified: Sat Jun  1 19:29:51 2024, max compression
```

## Comparing `playwright_html_renderer-0.1.tar` & `playwright_html_renderer-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:51:32.939615 playwright_html_renderer-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-06-01 18:51:18.000000 playwright_html_renderer-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-06-01 18:51:32.939615 playwright_html_renderer-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-06-01 18:51:18.000000 playwright_html_renderer-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:51:32.939615 playwright_html_renderer-0.1/playwright_html_renderer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 18:51:18.000000 playwright_html_renderer-0.1/playwright_html_renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 18:51:18.000000 playwright_html_renderer-0.1/playwright_html_renderer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-06-01 18:51:18.000000 playwright_html_renderer-0.1/playwright_html_renderer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:51:32.939615 playwright_html_renderer-0.1/playwright_html_renderer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-06-01 18:51:32.000000 playwright_html_renderer-0.1/playwright_html_renderer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-01 18:51:32.000000 playwright_html_renderer-0.1/playwright_html_renderer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 18:51:32.000000 playwright_html_renderer-0.1/playwright_html_renderer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 18:51:32.000000 playwright_html_renderer-0.1/playwright_html_renderer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 18:51:32.000000 playwright_html_renderer-0.1/playwright_html_renderer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 18:51:32.000000 playwright_html_renderer-0.1/playwright_html_renderer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:51:32.939615 playwright_html_renderer-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 18:51:18.000000 playwright_html_renderer-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:29:51.531174 playwright_html_renderer-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-06-01 19:29:43.000000 playwright_html_renderer-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-06-01 19:29:51.531174 playwright_html_renderer-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-06-01 19:29:43.000000 playwright_html_renderer-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:29:51.531174 playwright_html_renderer-0.2/playwright_html_renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 19:29:43.000000 playwright_html_renderer-0.2/playwright_html_renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 19:29:43.000000 playwright_html_renderer-0.2/playwright_html_renderer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-06-01 19:29:43.000000 playwright_html_renderer-0.2/playwright_html_renderer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:29:51.531174 playwright_html_renderer-0.2/playwright_html_renderer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-06-01 19:29:51.000000 playwright_html_renderer-0.2/playwright_html_renderer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-01 19:29:51.000000 playwright_html_renderer-0.2/playwright_html_renderer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 19:29:51.000000 playwright_html_renderer-0.2/playwright_html_renderer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 19:29:51.000000 playwright_html_renderer-0.2/playwright_html_renderer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 19:29:51.000000 playwright_html_renderer-0.2/playwright_html_renderer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 19:29:51.000000 playwright_html_renderer-0.2/playwright_html_renderer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 19:29:51.531174 playwright_html_renderer-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 19:29:43.000000 playwright_html_renderer-0.2/setup.py
```

### Comparing `playwright_html_renderer-0.1/LICENSE` & `playwright_html_renderer-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright_html_renderer-0.1/PKG-INFO` & `playwright_html_renderer-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwright-html-renderer
-Version: 0.1
+Version: 0.2
 Summary: CLI tool to render HTML using Playwright
 Home-page: https://github.com/custom-packages/playwright-html-renderer
 Author: Stefan Kühnel
 License: European Union Public License 1.2
 Project-URL: Documentation, https://github.com/custom-packages/playwright-html-renderer
 Project-URL: Source code, https://github.com/custom-packages/playwright-html-renderer
 Project-URL: Issues, https://github.com/custom-packages/playwright-html-renderer/issues
```

### Comparing `playwright_html_renderer-0.1/README.md` & `playwright_html_renderer-0.2/README.md`

 * *Files identical despite different names*

### Comparing `playwright_html_renderer-0.1/playwright_html_renderer/cli.py` & `playwright_html_renderer-0.2/playwright_html_renderer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
-import pkg_resources
 import sys
 
 from playwright.sync_api import sync_playwright
 
 
-VERSION = pkg_resources.get_distribution("playwright-html-renderer").version
+VERSION = "0.2"
 
 
 def get_raw_html_content(filepath: str) -> str:
     """Retrieve raw HTML content from a file or STDIN.
 
     Args:
         filepath: Path to the file containing HTML content, or '-' for STDIN.
```

### Comparing `playwright_html_renderer-0.1/playwright_html_renderer.egg-info/PKG-INFO` & `playwright_html_renderer-0.2/playwright_html_renderer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwright-html-renderer
-Version: 0.1
+Version: 0.2
 Summary: CLI tool to render HTML using Playwright
 Home-page: https://github.com/custom-packages/playwright-html-renderer
 Author: Stefan Kühnel
 License: European Union Public License 1.2
 Project-URL: Documentation, https://github.com/custom-packages/playwright-html-renderer
 Project-URL: Source code, https://github.com/custom-packages/playwright-html-renderer
 Project-URL: Issues, https://github.com/custom-packages/playwright-html-renderer/issues
```

### Comparing `playwright_html_renderer-0.1/setup.py` & `playwright_html_renderer-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import os
 
 from setuptools import setup, find_packages
 
-VERSION = "0.1"
+VERSION = "0.2"
 
 
 def get_long_description():
     with io.open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

