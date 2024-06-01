# Comparing `tmp/anipy_cli-3.1.2.tar.gz` & `tmp/anipy_cli-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_cli-3.1.2.tar", max compression
+gzip compressed data, was "anipy_cli-3.1.3.tar", max compression
```

## Comparing `anipy_cli-3.1.2.tar` & `anipy_cli-3.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2308 2024-05-30 12:07:29.289708 anipy_cli-3.1.2/README.md
--rw-r--r--   0        0        0      855 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/__init__.py
--rw-r--r--   0        0        0     5288 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/arg_parser.py
--rw-r--r--   0        0        0     1922 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/cli.py
--rw-r--r--   0        0        0      411 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/__init__.py
--rw-r--r--   0        0        0      817 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/base_cli.py
--rw-r--r--   0        0        0     2281 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/binge_cli.py
--rw-r--r--   0        0        0     2806 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/default_cli.py
--rw-r--r--   0        0        0     3187 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/download_cli.py
--rw-r--r--   0        0        0     2863 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/history_cli.py
--rw-r--r--   0        0        0     2258 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/mal_cli.py
--rw-r--r--   0        0        0      616 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/seasonal_cli.py
--rw-r--r--   0        0        0      916 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/colors.py
--rw-r--r--   0        0        0    15422 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/config.py
--rw-r--r--   0        0        0     1160 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/discord.py
--rw-r--r--   0        0        0     6981 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/mal_proxy.py
--rw-r--r--   0        0        0      185 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/__init__.py
--rw-r--r--   0        0        0     1140 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/base_menu.py
--rw-r--r--   0        0        0    24105 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/mal_menu.py
--rw-r--r--   0        0        0     7860 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/menu.py
--rw-r--r--   0        0        0     9097 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/seasonal_menu.py
--rw-r--r--   0        0        0     7564 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/prompts.py
--rw-r--r--   0        0        0     7684 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/util.py
--rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 anipy_cli-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2308 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/README.md
+-rw-r--r--   0        0        0      855 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/__init__.py
+-rw-r--r--   0        0        0     5288 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/arg_parser.py
+-rw-r--r--   0        0        0     1922 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/cli.py
+-rw-r--r--   0        0        0      411 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/clis/__init__.py
+-rw-r--r--   0        0        0      817 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/clis/base_cli.py
+-rw-r--r--   0        0        0     2281 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/clis/binge_cli.py
+-rw-r--r--   0        0        0     2806 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/clis/default_cli.py
+-rw-r--r--   0        0        0     3187 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/clis/download_cli.py
+-rw-r--r--   0        0        0     2863 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/clis/history_cli.py
+-rw-r--r--   0        0        0     2258 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/clis/mal_cli.py
+-rw-r--r--   0        0        0      616 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/clis/seasonal_cli.py
+-rw-r--r--   0        0        0      916 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/colors.py
+-rw-r--r--   0        0        0    15422 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/config.py
+-rw-r--r--   0        0        0     1160 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/discord.py
+-rw-r--r--   0        0        0     6981 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/mal_proxy.py
+-rw-r--r--   0        0        0      185 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/menus/__init__.py
+-rw-r--r--   0        0        0     1140 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/menus/base_menu.py
+-rw-r--r--   0        0        0    24105 2024-06-01 13:03:33.405826 anipy_cli-3.1.3/src/anipy_cli/menus/mal_menu.py
+-rw-r--r--   0        0        0     7860 2024-06-01 13:03:33.409826 anipy_cli-3.1.3/src/anipy_cli/menus/menu.py
+-rw-r--r--   0        0        0     9097 2024-06-01 13:03:33.409826 anipy_cli-3.1.3/src/anipy_cli/menus/seasonal_menu.py
+-rw-r--r--   0        0        0     7564 2024-06-01 13:03:33.409826 anipy_cli-3.1.3/src/anipy_cli/prompts.py
+-rw-r--r--   0        0        0     7684 2024-06-01 13:03:33.409826 anipy_cli-3.1.3/src/anipy_cli/util.py
+-rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 anipy_cli-3.1.3/PKG-INFO
```

### Comparing `anipy_cli-3.1.2/README.md` & `anipy_cli-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/pyproject.toml` & `anipy_cli-3.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-cli"
-version = "3.1.2"
+version = "3.1.3"
 description = "Watch and Download anime from the comfort of your Terminal"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-cli"
 keywords = ["anime", "cli"]
@@ -16,15 +16,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0.1"
 yaspin = "^3.0.2"
 inquirerpy = "^0.3.4"
 appdirs = "^1.4.4"
 pypresence = "^4.3.0"
-anipy-api = "^3.1.2"
+anipy-api = "^3.1.3"
 
 [tool.poetry.scripts]
 anipy-cli = "anipy_cli.cli:run_cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/sdaqo/anipy-cli/issues"
```

### Comparing `anipy_cli-3.1.2/src/anipy_cli/arg_parser.py` & `anipy_cli-3.1.3/src/anipy_cli/arg_parser.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/cli.py` & `anipy_cli-3.1.3/src/anipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/clis/base_cli.py` & `anipy_cli-3.1.3/src/anipy_cli/clis/base_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/clis/binge_cli.py` & `anipy_cli-3.1.3/src/anipy_cli/clis/binge_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/clis/default_cli.py` & `anipy_cli-3.1.3/src/anipy_cli/clis/default_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/clis/download_cli.py` & `anipy_cli-3.1.3/src/anipy_cli/clis/download_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/clis/history_cli.py` & `anipy_cli-3.1.3/src/anipy_cli/clis/history_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/clis/mal_cli.py` & `anipy_cli-3.1.3/src/anipy_cli/clis/mal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/clis/seasonal_cli.py` & `anipy_cli-3.1.3/src/anipy_cli/clis/seasonal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/colors.py` & `anipy_cli-3.1.3/src/anipy_cli/colors.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/config.py` & `anipy_cli-3.1.3/src/anipy_cli/config.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/discord.py` & `anipy_cli-3.1.3/src/anipy_cli/discord.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/mal_proxy.py` & `anipy_cli-3.1.3/src/anipy_cli/mal_proxy.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/menus/base_menu.py` & `anipy_cli-3.1.3/src/anipy_cli/menus/base_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/menus/mal_menu.py` & `anipy_cli-3.1.3/src/anipy_cli/menus/mal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/menus/menu.py` & `anipy_cli-3.1.3/src/anipy_cli/menus/menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/menus/seasonal_menu.py` & `anipy_cli-3.1.3/src/anipy_cli/menus/seasonal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/prompts.py` & `anipy_cli-3.1.3/src/anipy_cli/prompts.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/src/anipy_cli/util.py` & `anipy_cli-3.1.3/src/anipy_cli/util.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.2/PKG-INFO` & `anipy_cli-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: anipy-cli
-Version: 3.1.2
+Version: 3.1.3
 Summary: Watch and Download anime from the comfort of your Terminal
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,cli
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anipy-api (>=3.1.2,<4.0.0)
+Requires-Dist: anipy-api (>=3.1.3,<4.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pypresence (>=4.3.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: yaspin (>=3.0.2,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/sdaqo/anipy-cli/issues
 Project-URL: Documentation, https://sdaqo.github.io/anipy-cli/getting-started-cli
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: anipy-cli Version: 3.1.2 Summary: Watch and
+Metadata-Version: 2.1 Name: anipy-cli Version: 3.1.3 Summary: Watch and
 Download anime from the comfort of your Terminal Home-page: https://
 sdaqo.github.io/anipy-cli License: GPL-3.0 Keywords: anime,cli Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: anipy-api (>=3.1.2,<4.0.0) Requires-Dist: appdirs
+Python :: 3.12 Requires-Dist: anipy-api (>=3.1.3,<4.0.0) Requires-Dist: appdirs
 (>=1.4.4,<2.0.0) Requires-Dist: inquirerpy (>=0.3.4,<0.4.0) Requires-Dist:
 pypresence (>=4.3.0,<5.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
 Dist: yaspin (>=3.0.2,<4.0.0) Project-URL: Bug Tracker, https://github.com/
 sdaqo/anipy-cli/issues Project-URL: Documentation, https://sdaqo.github.io/
 anipy-cli/getting-started-cli Project-URL: Repository, https://github.com/
 sdaqo/anipy-cli Description-Content-Type: text/markdown # ANIPY-CLI **Anime
 from the comfort of your Terminal**
```

