# Comparing `tmp/makex-20240401.tar.gz` & `tmp/makex-20240601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makex-20240401.tar", last modified: Fri Apr 26 20:00:55 2024, max compression
+gzip compressed data, was "makex-20240601.tar", last modified: Sat Jun  1 21:19:56 2024, max compression
```

## Comparing `makex-20240401.tar` & `makex-20240601.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.538812 makex-20240401/
--rw-r--r--   0 nate      (1000) nate      (1000)     3232 2024-04-26 20:00:55.537812 makex-20240401/PKG-INFO
--rw-r--r--   0 nate      (1000) nate      (1000)     1912 2024-04-26 20:00:53.000000 makex-20240401/README.md
--rw-r--r--   0 nate      (1000) nate      (1000)     2126 2024-04-26 20:00:53.000000 makex-20240401/pyproject.toml
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.530812 makex-20240401/python/
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.531812 makex-20240401/python/benchmarks/
--rw-r--r--   0 nate      (1000) nate      (1000)     1518 2024-04-26 20:00:53.000000 makex-20240401/python/benchmarks/hashing_benchmark_test.py
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.535812 makex-20240401/python/makex/
--rw-r--r--   0 nate      (1000) nate      (1000)    43219 2024-04-26 20:00:53.000000 makex-20240401/python/makex/__main__.py
--rw-r--r--   0 nate      (1000) nate      (1000)     2126 2024-04-26 20:00:53.000000 makex-20240401/python/makex/_logging.py
--rw-r--r--   0 nate      (1000) nate      (1000)     6016 2024-04-26 20:00:53.000000 makex-20240401/python/makex/_shtab.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      693 2024-04-26 20:00:53.000000 makex-20240401/python/makex/api.py
--rw-r--r--   0 nate      (1000) nate      (1000)    15755 2024-04-26 20:00:53.000000 makex-20240401/python/makex/build_path.py
--rw-r--r--   0 nate      (1000) nate      (1000)      945 2024-04-26 20:00:53.000000 makex-20240401/python/makex/colors.py
--rw-r--r--   0 nate      (1000) nate      (1000)     9448 2024-04-26 20:00:53.000000 makex-20240401/python/makex/configuration.py
--rw-r--r--   0 nate      (1000) nate      (1000)     4919 2024-04-26 20:00:53.000000 makex-20240401/python/makex/constants.py
--rw-r--r--   0 nate      (1000) nate      (1000)     6558 2024-04-26 20:00:53.000000 makex-20240401/python/makex/context.py
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.530812 makex-20240401/python/makex/data/
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.536811 makex-20240401/python/makex/data/completions/
--rw-r--r--   0 nate      (1000) nate      (1000)     9618 2024-04-26 20:00:53.000000 makex-20240401/python/makex/data/completions/makex.bash
--rw-r--r--   0 nate      (1000) nate      (1000)     6146 2024-04-26 20:00:53.000000 makex-20240401/python/makex/data/completions/makex.zsh
--rw-rw-r--   0 nate      (1000) nate      (1000)     2411 2024-04-26 20:00:53.000000 makex-20240401/python/makex/errors.py
--rw-r--r--   0 nate      (1000) nate      (1000)    50541 2024-04-26 20:00:53.000000 makex-20240401/python/makex/executor.py
--rw-r--r--   0 nate      (1000) nate      (1000)     7517 2024-04-26 20:00:53.000000 makex-20240401/python/makex/executor_test.py
--rw-r--r--   0 nate      (1000) nate      (1000)    11770 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_checksum.py
--rw-rw-r--   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_checksum_test.py
--rw-r--r--   0 nate      (1000) nate      (1000)     6332 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_cloning.py
--rw-r--r--   0 nate      (1000) nate      (1000)      228 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_cloning_test.py
--rw-r--r--   0 nate      (1000) nate      (1000)     3656 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_system.py
--rw-r--r--   0 nate      (1000) nate      (1000)     3806 2024-04-26 20:00:53.000000 makex-20240401/python/makex/flags.py
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.536811 makex-20240401/python/makex/integrations/
--rw-r--r--   0 nate      (1000) nate      (1000)      774 2024-04-26 20:00:53.000000 makex-20240401/python/makex/integrations/intellij.py
--rw-r--r--   0 nate      (1000) nate      (1000)      484 2024-04-26 20:00:53.000000 makex-20240401/python/makex/integrations/vscode.py
--rw-r--r--   0 nate      (1000) nate      (1000)    83180 2024-04-26 20:00:53.000000 makex-20240401/python/makex/makex_file.py
--rw-r--r--   0 nate      (1000) nate      (1000)    36614 2024-04-26 20:00:53.000000 makex-20240401/python/makex/makex_file_parser.py
--rw-r--r--   0 nate      (1000) nate      (1000)     6970 2024-04-26 20:00:53.000000 makex-20240401/python/makex/makex_file_parser_test.py
--rw-r--r--   0 nate      (1000) nate      (1000)    11283 2024-04-26 20:00:53.000000 makex-20240401/python/makex/makex_file_types.py
--rw-r--r--   0 nate      (1000) nate      (1000)     5654 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     2879 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata_file.py
--rw-r--r--   0 nate      (1000) nate      (1000)     5519 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata_sqlite.py
--rw-r--r--   0 nate      (1000) nate      (1000)      487 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata_sqlite_test.py
--rw-r--r--   0 nate      (1000) nate      (1000)      671 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     3157 2024-04-26 20:00:53.000000 makex-20240401/python/makex/patterns.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      600 2024-04-26 20:00:53.000000 makex-20240401/python/makex/patterns_test.py
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.536811 makex-20240401/python/makex/platform_object/
--rw-rw-r--   0 nate      (1000) nate      (1000)       43 2024-04-26 20:00:53.000000 makex-20240401/python/makex/platform_object/__init__.py
--rw-r--r--   0 nate      (1000) nate      (1000)     4960 2024-04-26 20:00:53.000000 makex-20240401/python/makex/platform_object/platform_object.py
--rw-r--r--   0 nate      (1000) nate      (1000)      484 2024-04-26 20:00:53.000000 makex-20240401/python/makex/platform_object/platform_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     2216 2024-04-26 20:00:53.000000 makex-20240401/python/makex/protocols.py
--rw-r--r--   0 nate      (1000) nate      (1000)    25641 2024-04-26 20:00:53.000000 makex-20240401/python/makex/python_script.py
--rw-r--r--   0 nate      (1000) nate      (1000)     3962 2024-04-26 20:00:53.000000 makex-20240401/python/makex/run.py
--rw-r--r--   0 nate      (1000) nate      (1000)    13762 2024-04-26 20:00:53.000000 makex-20240401/python/makex/target.py
--rw-r--r--   0 nate      (1000) nate      (1000)     4109 2024-04-26 20:00:53.000000 makex-20240401/python/makex/ui.py
--rw-rw-r--   0 nate      (1000) nate      (1000)       19 2024-04-26 20:00:53.000000 makex-20240401/python/makex/version.py
--rw-r--r--   0 nate      (1000) nate      (1000)     9577 2024-04-26 20:00:53.000000 makex-20240401/python/makex/workspace.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1054 2024-04-26 20:00:53.000000 makex-20240401/python/makex/workspace_test.py
-drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.536811 makex-20240401/python/makex.egg-info/
--rw-r--r--   0 nate      (1000) nate      (1000)     3232 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/PKG-INFO
--rw-r--r--   0 nate      (1000) nate      (1000)     1596 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/SOURCES.txt
--rw-r--r--   0 nate      (1000) nate      (1000)        1 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/dependency_links.txt
--rw-r--r--   0 nate      (1000) nate      (1000)       71 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/entry_points.txt
--rw-r--r--   0 nate      (1000) nate      (1000)      210 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/requires.txt
--rw-r--r--   0 nate      (1000) nate      (1000)       17 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/top_level.txt
--rw-r--r--   0 nate      (1000) nate      (1000)       38 2024-04-26 20:00:55.538812 makex-20240401/setup.cfg
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.295574 makex-20240601/
+-rw-r--r--   0 nate      (1000) nate      (1000)     3435 2024-06-01 21:19:56.294574 makex-20240601/PKG-INFO
+-rw-r--r--   0 nate      (1000) nate      (1000)     2009 2024-06-01 21:19:54.000000 makex-20240601/README.md
+-rw-r--r--   0 nate      (1000) nate      (1000)     2283 2024-06-01 21:19:54.000000 makex-20240601/pyproject.toml
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.288574 makex-20240601/python/
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.288574 makex-20240601/python/benchmarks/
+-rw-r--r--   0 nate      (1000) nate      (1000)     1518 2024-06-01 21:19:54.000000 makex-20240601/python/benchmarks/hashing_benchmark_test.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.292574 makex-20240601/python/makex/
+-rw-r--r--   0 nate      (1000) nate      (1000)    43404 2024-06-01 21:19:54.000000 makex-20240601/python/makex/__main__.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     2126 2024-06-01 21:19:54.000000 makex-20240601/python/makex/_logging.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     6016 2024-06-01 21:19:54.000000 makex-20240601/python/makex/_shtab.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)      693 2024-06-01 21:19:54.000000 makex-20240601/python/makex/api.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    15755 2024-06-01 21:19:54.000000 makex-20240601/python/makex/build_path.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      945 2024-06-01 21:19:54.000000 makex-20240601/python/makex/colors.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    10662 2024-06-01 21:19:54.000000 makex-20240601/python/makex/configuration.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     5054 2024-06-01 21:19:54.000000 makex-20240601/python/makex/constants.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     6558 2024-06-01 21:19:54.000000 makex-20240601/python/makex/context.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.288574 makex-20240601/python/makex/data/
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.293574 makex-20240601/python/makex/data/completions/
+-rw-r--r--   0 nate      (1000) nate      (1000)     9618 2024-06-01 21:19:54.000000 makex-20240601/python/makex/data/completions/makex.bash
+-rw-r--r--   0 nate      (1000) nate      (1000)     6146 2024-06-01 21:19:54.000000 makex-20240601/python/makex/data/completions/makex.zsh
+-rw-r--r--   0 nate      (1000) nate      (1000)     2427 2024-06-01 21:19:54.000000 makex-20240601/python/makex/errors.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    50638 2024-06-01 21:19:54.000000 makex-20240601/python/makex/executor.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     7696 2024-06-01 21:19:54.000000 makex-20240601/python/makex/executor_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    11853 2024-06-01 21:19:54.000000 makex-20240601/python/makex/file_checksum.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:54.000000 makex-20240601/python/makex/file_checksum_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     6332 2024-06-01 21:19:54.000000 makex-20240601/python/makex/file_cloning.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      228 2024-06-01 21:19:54.000000 makex-20240601/python/makex/file_cloning_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     3656 2024-06-01 21:19:54.000000 makex-20240601/python/makex/file_system.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     4245 2024-06-01 21:19:54.000000 makex-20240601/python/makex/flags.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.293574 makex-20240601/python/makex/integrations/
+-rw-r--r--   0 nate      (1000) nate      (1000)      774 2024-06-01 21:19:54.000000 makex-20240601/python/makex/integrations/intellij.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      484 2024-06-01 21:19:54.000000 makex-20240601/python/makex/integrations/vscode.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    89646 2024-06-01 21:19:54.000000 makex-20240601/python/makex/makex_file.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    36579 2024-06-01 21:19:54.000000 makex-20240601/python/makex/makex_file_parser.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     6970 2024-06-01 21:19:54.000000 makex-20240601/python/makex/makex_file_parser_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    11566 2024-06-01 21:19:54.000000 makex-20240601/python/makex/makex_file_types.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     5654 2024-06-01 21:19:54.000000 makex-20240601/python/makex/metadata.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     2879 2024-06-01 21:19:54.000000 makex-20240601/python/makex/metadata_file.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     5519 2024-06-01 21:19:54.000000 makex-20240601/python/makex/metadata_sqlite.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      487 2024-06-01 21:19:54.000000 makex-20240601/python/makex/metadata_sqlite_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      671 2024-06-01 21:19:54.000000 makex-20240601/python/makex/metadata_test.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     3157 2024-06-01 21:19:54.000000 makex-20240601/python/makex/patterns.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      900 2024-06-01 21:19:54.000000 makex-20240601/python/makex/patterns_test.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.293574 makex-20240601/python/makex/platform_object/
+-rw-rw-r--   0 nate      (1000) nate      (1000)       43 2024-06-01 21:19:54.000000 makex-20240601/python/makex/platform_object/__init__.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     4960 2024-06-01 21:19:54.000000 makex-20240601/python/makex/platform_object/platform_object.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      484 2024-06-01 21:19:54.000000 makex-20240601/python/makex/platform_object/platform_test.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     2216 2024-06-01 21:19:54.000000 makex-20240601/python/makex/protocols.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    24454 2024-06-01 21:19:54.000000 makex-20240601/python/makex/python_script.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     3962 2024-06-01 21:19:54.000000 makex-20240601/python/makex/run.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    13762 2024-06-01 21:19:54.000000 makex-20240601/python/makex/target.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     4444 2024-06-01 21:19:54.000000 makex-20240601/python/makex/test_actions.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     4110 2024-06-01 21:19:54.000000 makex-20240601/python/makex/ui.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)       19 2024-06-01 21:19:54.000000 makex-20240601/python/makex/version.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     9577 2024-06-01 21:19:54.000000 makex-20240601/python/makex/workspace.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1054 2024-06-01 21:19:54.000000 makex-20240601/python/makex/workspace_test.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-01 21:19:56.293574 makex-20240601/python/makex.egg-info/
+-rw-r--r--   0 nate      (1000) nate      (1000)     3435 2024-06-01 21:19:56.000000 makex-20240601/python/makex.egg-info/PKG-INFO
+-rw-r--r--   0 nate      (1000) nate      (1000)     1625 2024-06-01 21:19:56.000000 makex-20240601/python/makex.egg-info/SOURCES.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)        1 2024-06-01 21:19:56.000000 makex-20240601/python/makex.egg-info/dependency_links.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       71 2024-06-01 21:19:56.000000 makex-20240601/python/makex.egg-info/entry_points.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)      252 2024-06-01 21:19:56.000000 makex-20240601/python/makex.egg-info/requires.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       17 2024-06-01 21:19:56.000000 makex-20240601/python/makex.egg-info/top_level.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       38 2024-06-01 21:19:56.295574 makex-20240601/setup.cfg
```

### Comparing `makex-20240401/PKG-INFO` & `makex-20240601/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: makex
-Version: 20240401
+Version: 20240601
 Summary: Build tool
 Author: Nate Skulic, MetaCompany
 Keywords: build,make,automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: toml>=0.10.2
-Requires-Dist: progressbar2>=4.3.2
+Provides-Extra: use-reflink
+Provides-Extra: use-xattr
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: shtab; extra == "build"
 Requires-Dist: pex; extra == "build"
 Requires-Dist: nuitka; extra == "build"
 Requires-Dist: pytest; extra == "build"
 Requires-Dist: shtab; extra == "build"
@@ -28,14 +29,16 @@
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
 Provides-Extra: documents
 Requires-Dist: sphinx; extra == "documents"
 Requires-Dist: sphinx-better-theme; extra == "documents"
 Requires-Dist: sphinx-notfound-page; extra == "documents"
 Requires-Dist: myst-parser; extra == "documents"
 Requires-Dist: markdown-it-py[linkify,plugins]; extra == "documents"
+Provides-Extra: typechecking
+Requires-Dist: typing_extensions; extra == "typechecking"
 
 # makex
 
 <!-- heading -->
 
 Makex is a new and simplified build and automation tool, similar to the original [Make](https://en.wikipedia.org/wiki/Make_(software)).
 
@@ -48,30 +51,30 @@
 
 - Compiling software/applications/firmware
 - Building filesystems/trees/file archives
 - Building and deploying websites and web applications
 - Running things in a repeatable manner
 - Replacing most or all of the other build systems
 
-## Features
+## Features 🍩
 
 - Familiar Syntax
 - File Hashing and Checksums
 - Dependency Graphs
 - Caching
 - Workspaces
 - Copy on Write
 
 <!-- links -->
 
-## Links
+## Links 🔗
 
 - [Documentation](https://meta.company/go/makex)
-- [Installation Instructions](https://meta.company/go/makex/install)
-- [Troubleshooting](https://meta.company/go/makex/trouble)
+- [Installation Instructions](https://documents.meta.company/makex/latest/install)
+- [Troubleshooting](https://documents.meta.company/makex/latest/trouble)
 - Support: [Google Groups](http://groups.google.com/group/makex) or [makex@googlegroups.com](mailto://makex@googlegroups.com)
 
 <!-- quick-start -->
 
 
 ## Quick Start
 
@@ -79,17 +82,15 @@
 
   ```shell
   pip install makex
   ```
 
 2. Define a Makex file (name it `Makexfile`):
 
-  ```python
-  #!makex
-  
+  ```python 
   task(
       name="hello-world",
       steps=[
           write("hello-world.txt", "Hello World!"),
   
           # or, you can use the shell, but it's not recommended:
           # shell(f"echo 'Hello World!' > {path('hello-world')}/hello-world.txt"),
@@ -102,27 +103,30 @@
 
 3. Run makex and the target:
 
   ```shell
   makex run :hello-world
   ```
  
+```{todo}
+Use the path command to show getting an output path.
+```
+
 4. A file at `_output_/hello-world/hello-world.txt` will have the following contents:
 
   ```
   Hello World!
   ```
 
-
 ## Limitations
 
 - Mac support is not tested.
 - Windows is not tested or supported (yet).
 
 ```{note}
 This is an early release of Makex. Things may change. If you have any problems, feel free to contact us. 
 ```
 
-## Pronunciation
+## Pronunciation 🗣
 
-Makex is pronounced "makes", ˈmeɪks, ˈmeɪkˈɛks (or just "make" 🙂).
+Makex is pronounced "makes", ˈmeɪks, ˈmeɪkˈɛks (or just "make" 🙂)
```

### Comparing `makex-20240401/README.md` & `makex-20240601/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 
 - Compiling software/applications/firmware
 - Building filesystems/trees/file archives
 - Building and deploying websites and web applications
 - Running things in a repeatable manner
 - Replacing most or all of the other build systems
 
-## Features
+## Features 🍩
 
 - Familiar Syntax
 - File Hashing and Checksums
 - Dependency Graphs
 - Caching
 - Workspaces
 - Copy on Write
 
 <!-- links -->
 
-## Links
+## Links 🔗
 
 - [Documentation](https://meta.company/go/makex)
-- [Installation Instructions](https://meta.company/go/makex/install)
-- [Troubleshooting](https://meta.company/go/makex/trouble)
+- [Installation Instructions](https://documents.meta.company/makex/latest/install)
+- [Troubleshooting](https://documents.meta.company/makex/latest/trouble)
 - Support: [Google Groups](http://groups.google.com/group/makex) or [makex@googlegroups.com](mailto://makex@googlegroups.com)
 
 <!-- quick-start -->
 
 
 ## Quick Start
 
@@ -44,17 +44,15 @@
 
   ```shell
   pip install makex
   ```
 
 2. Define a Makex file (name it `Makexfile`):
 
-  ```python
-  #!makex
-  
+  ```python 
   task(
       name="hello-world",
       steps=[
           write("hello-world.txt", "Hello World!"),
   
           # or, you can use the shell, but it's not recommended:
           # shell(f"echo 'Hello World!' > {path('hello-world')}/hello-world.txt"),
@@ -67,27 +65,30 @@
 
 3. Run makex and the target:
 
   ```shell
   makex run :hello-world
   ```
  
+```{todo}
+Use the path command to show getting an output path.
+```
+
 4. A file at `_output_/hello-world/hello-world.txt` will have the following contents:
 
   ```
   Hello World!
   ```
 
-
 ## Limitations
 
 - Mac support is not tested.
 - Windows is not tested or supported (yet).
 
 ```{note}
 This is an early release of Makex. Things may change. If you have any problems, feel free to contact us. 
 ```
 
-## Pronunciation
+## Pronunciation 🗣
 
-Makex is pronounced "makes", ˈmeɪks, ˈmeɪkˈɛks (or just "make" 🙂).
+Makex is pronounced "makes", ˈmeɪks, ˈmeɪkˈɛks (or just "make" 🙂)
```

### Comparing `makex-20240401/pyproject.toml` & `makex-20240601/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,48 +2,54 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "makex"
 dynamic = ["version"]
 description = "Build tool"
-readme = { file = "README.md", content-type="text/markdown" }
-license = { file = "LICENSE.md", content-type="text/markdown" }
+readme = { file = "README.md", content-type = "text/markdown" }
+license = { file = "LICENSE.md", content-type = "text/markdown" }
 requires-python = ">=3.9"
 dependencies = [
-    # XXX: We don't need this anymore but we can fall back if ours doesn't work.
-    #"reflink>=0.2.2",
-    # XXX: We don't need this anymore but we can fall back. This xattr package doesn't emit auditing events unlike the builtin.
-    #"xattr>=1.0.0",
+    # XXX: We may revert to this:
+    #"progressbar2>=4.3.2",
+    # TODO: remove this dependency.
     "toml>=0.10.2",
-    "progressbar2>=4.3.2",
 ]
 authors = [
-    {name = "Nate Skulic"},
-    {name = "MetaCompany" },
+    { name = "Nate Skulic" },
+    { name = "MetaCompany" },
 ]
 keywords = ["build", "make", "automation"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     #"License :: OSI Approved :: Apache Software License",
     "Operating System :: Unix",
     "Operating System :: POSIX :: Linux",
-   # "Operating System :: MacOS :: MacOS X",
+    # "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Utilities",
 ]
 
 
 [tool.setuptools.dynamic]
 version = { attr = "makex.version.VERSION" }
 
 [project.optional-dependencies]
+use-reflink = [
+    # XXX: We don't need this anymore but we can fall back if ours doesn't work.
+    #"reflink>=0.2.2",
+]
+use-xattr = [
+    # XXX: We don't need this anymore but we can fall back. This xattr package doesn't emit auditing events unlike the builtin.
+    #"xattr>=1.0.0",
+]
 build = [
     "build",
     "shtab",
     "pex",
     "nuitka",
     "pytest",
     "shtab",
@@ -55,25 +61,28 @@
 documents = [
     "sphinx",
     "sphinx-better-theme",
     "sphinx-notfound-page",
     "myst-parser",
     "markdown-it-py[linkify,plugins]"
 ]
+typechecking = [
+    "typing_extensions"
+]
 
 [project.scripts]
 makex = "makex.__main__:main"
 mx = "makex.__main__:main"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 namespaces = true
 
 [tool.setuptools.package-data]
-"makex.data.completions" =[
+"makex.data.completions" = [
     "*.bash",
     "*.zsh",
 ]
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "5"
```

### Comparing `makex-20240401/python/benchmarks/hashing_benchmark_test.py` & `makex-20240601/python/benchmarks/hashing_benchmark_test.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/__main__.py` & `makex-20240601/python/makex/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 )
 from makex.context import Context
 from makex.errors import (
     CacheError,
     Error,
     ExecutionError,
     GenericSyntaxError,
+    MultipleErrors,
 )
 from makex.executor import Executor
 from makex.flags import VARIANTS_ENABLED
 from makex.makex_file import MakexFileCycleError
 from makex.makex_file_parser import (
     TargetGraph,
     parse_makefile_into_graph,
@@ -570,27 +571,31 @@
 
     if not path.exists():
         raise Exception(f"Path in scope {scope} does not exist (Expected: {path}).")
 
     return ParsedScope(path, type)
 
 
-def print_errors(ctx: Context, errors):
+def print_errors(ctx: Context, errors: Union[Exception, MultipleErrors]):
     if errors:
         print(f"{ctx.colors.ERROR+ctx.colors.BOLD}The execution had errors:{ctx.colors.RESET}\n")
+
     for error in errors:
         print("---------------")
         print_error(ctx, error)
 
 
 def print_error(ctx: Context, error):
     if isinstance(error, (PythonScriptFileError, PythonScriptError)):
         print(pretty_makex_file_exception(error, error.location, colors=ctx.colors))
     elif isinstance(error, MakexFileCycleError):
         print(error.pretty(ctx))
+    elif isinstance(error, MultipleErrors):
+        for error in error.errors:
+            print_error(ctx, error)
     elif isinstance(error, ExecutionError):
         if error.location:
             print(pretty_makex_file_exception(error.error, error.location, colors=ctx.colors))
         else:
             print("Execution Error:", error)
     else:
         print(f"{type(error)} Error:")
@@ -886,15 +891,15 @@
 
     if args.real:
         workspace = which_workspace(workspace.path, target_input)
 
     obj = get_build_path(
         objective_name=ref.name,
         variants=[],
-        input_directory=target_input,
+        input_directory=target_input.parent,
         build_root=ctx.cache,
         workspace=workspace.path,
         workspace_id=workspace.id,
         output_folder=ctx.output_folder_name,
     )
 
     path, link = obj
@@ -1357,14 +1362,17 @@
 
     # XXX: Currently set to one to avoid much breakage. Things are fast enough, for now.
     workers = 1 or args.threads
     executor = Executor(ctx, workers=workers, force=args.force)
 
     try:
         executed, errors = executor.execute_targets(*targets_to_run)
+
+        if len(errors):
+            print_errors(ctx, errors)
     except KeyboardInterrupt as e:
         executor.stop.set()
         _kill_running_processes()
         sys.exit(-1)
 
     except IOError as e:
         exc_info = sys.exc_info()
@@ -1373,17 +1381,14 @@
         sys.exit(-1)
 
     except Exception as e:
         exc_info = sys.exc_info()
         traceback.print_exception(*exc_info)
         sys.exit(-1)
 
-    if len(errors):
-        print_errors(ctx, errors)
-
 
 COMMANDS = {
     "run": main_run,
     "path": main_get_path,
     "targets": main_targets,
     "workspace": main_workspace,
     "complete": main_complete,
```

### Comparing `makex-20240401/python/makex/_logging.py` & `makex-20240601/python/makex/_logging.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/_shtab.py` & `makex-20240601/python/makex/_shtab.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/api.py` & `makex-20240601/python/makex/api.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/build_path.py` & `makex-20240601/python/makex/build_path.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/colors.py` & `makex-20240601/python/makex/colors.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/configuration.py` & `makex-20240601/python/makex/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,46 @@
+import json
 import os
 from dataclasses import (
     dataclass,
     field,
 )
 from io import StringIO
 from pathlib import Path
 from typing import (
     Callable,
     Optional,
     Protocol,
     Union,
 )
 
-import toml as toml
 from makex.constants import (
     CONFIG_NAME_1,
     CONFIG_NAME_2,
     OUTPUT_FOLDER_CONFIGURATION_ENABLED,
     WORKSPACE_FILE_NAME,
 )
 from makex.errors import (
     GenericFileLocation,
     GenericSyntaxError,
     MakexError,
 )
 
+_HAS_TOML = False
+try:
+    import tomllib as toml
+    _HAS_TOML = True
+except ImportError:
+    try:
+        import toml as toml
+        _HAS_TOML = True
+    except ImportError:
+        _HAS_TOML = False
+
+
 
 class ConfigurationError(MakexError):
     def __init__(self, message, location: GenericFileLocation):
         super().__init__(message)
         self.location = location
 
 
@@ -185,15 +197,14 @@
         if isinstance(value, dict):
             script = value.get("shell", None)
             if script is not None:
 
                 read, write = os.pipe()
                 os.write(write, script.encode("utf-8"))
                 os.close(write)
-                print(shell, script)
                 process = run(
                     shell,
                     env=current_enviroment,
                     capture=True,
                     shell=False,
                     print=False,
                     cwd=cwd,
@@ -250,14 +261,26 @@
         except toml.TomlDecodeError as e:
             l = GenericFileLocation(path, e.lineno, e.colno)
             raise GenericSyntaxError(str(e), location=l, type="Configuration") from e
         except Exception as e:
             raise Exception(f"Error loading configuration file at {path}: {e} {type(e)}")
 
 
+def read_configuration_json(path: Path) -> Configuration:
+    with path.open("r") as f:
+        try:
+            d = json.load(f)
+            return Configuration.from_json(d)
+        except json.JSONDecodeError as e:
+            l = GenericFileLocation(path, e.lineno, e.colno)
+            raise GenericSyntaxError(e.msg, location=l, type="Configuration") from e
+        except Exception as e:
+            raise Exception(f"Error loading configuration file at {path}: {e} {type(e)}")
+
+
 def collect_configurations(
     cwd: Path, parents=True, verbose: Callable[[str], None] = lambda x: None
 ) -> ConfigurationFiles:
     """ An expensive (IO) routine to collect all related configuration/marker files for makex.
 
         We search for workspaces and configurations both so we don't need to do it twice separately.
 
@@ -275,14 +298,28 @@
             workspace_file = parent / WORKSPACE_FILE_NAME
             config_file1 = parent / CONFIG_NAME_1
             config_file2 = parent / CONFIG_NAME_2
 
             if workspace_file.exists():
                 workspace_files_found.append(workspace_file)
 
+            if False:
+                for config_file_type, config_file_name in CONFIG_FILE_NAMES:
+                    path = parent / config_file_name
+
+                    if path.exists() is False:
+                        continue
+
+                    if config_file_type == "toml":
+                        config_files_found.append(read_configuration(path))
+                    elif config_file_type == "json":
+                        config_files_found.append(read_configuration(path))
+                    else:
+                        raise NotImplementedError
+
             if config_file1.exists():
                 verbose(f"Reading configuration file at {config_file1}")
                 config_files_found.append(read_configuration(config_file1))
             elif config_file2.exists():
                 verbose(f"Reading configuration file at {config_file2}")
                 config_files_found.append(read_configuration(config_file2))
             parent = parent.parent
```

### Comparing `makex-20240401/python/makex/constants.py` & `makex-20240601/python/makex/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 """
 # higher priority config file name
 CONFIG_NAME_1 = "makex.toml"
 
 # lower priority/hidden config file name
 CONFIG_NAME_2 = ".makex.toml"
 
+CONFIG_FILE_NAMES = [
+    ("toml","makex.toml"),
+    ("toml",".makex.toml"),
+    ("json","makex.json"),
+    ("json",".makex.json"),
+]
+
 WORKSPACE_FILE_NAME = "WORKSPACE"
 
 MAKEX_FILE_NAMES = {"Makexfile", "makexfile"} #"Build",
 
 OUTPUT_DIRECTORY_NAME = "_output_"
 
 # Flags we don't want to wire into configuration/enviroment/context (yet):
```

### Comparing `makex-20240401/python/makex/context.py` & `makex-20240601/python/makex/context.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/data/completions/makex.bash` & `makex-20240601/python/makex/data/completions/makex.bash`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/data/completions/makex.zsh` & `makex-20240601/python/makex/data/completions/makex.zsh`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/errors.py` & `makex-20240601/python/makex/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,9 +94,9 @@
     location: FileLocation
 
     def __init__(self, message, location):
         pass
 
 
 class MultipleErrors(MakexError):
-    def __init__(self, erorrs: list[Exception]):
-        pass
+    def __init__(self, errors: list[Exception]):
+        self.errors = errors
```

### Comparing `makex-20240401/python/makex/executor.py` & `makex-20240601/python/makex/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     find_makex_files,
     resolve_find_files,
     resolve_glob,
     resolve_path_element_workspace,
     resolve_string_path_workspace,
     resolve_target_output_path,
 )
+from makex.makex_file_parser import TargetGraph
 from makex.makex_file_types import (
     FindFiles,
     Glob,
     ListTypes,
     PathElement,
     PathObject,
     ResolvedTargetReference,
@@ -77,15 +78,15 @@
 
     def __init__(self, target, output=None, errors=None):
         self.target = target
         self.output = output or ""
         self.errors = errors or []
 
 
-_XATTR_OUTPUT_TARGET_HASH = b"user.makex.target_hash"
+_XATTR_OUTPUT_TARGET_HASH = b"user.makex.task_hash"
 
 from os import (
     getxattr,
     removexattr,
     setxattr,
 )
 
@@ -173,22 +174,22 @@
     # queue of object we need to write to database. doing this because of sqlite issues...
     # sqlite objects can't be accessed from a different thread, so we'd need to recreate connections per each, or,
     # keep a queue.
     _database_queue: deque[EvaluatedTarget]
 
     _executed_keys: set[str]
 
-    def __init__(self, ctx: "Context", workers=1, force=False):
+    def __init__(self, ctx: "Context", workers=1, force=False, graph=None):
         self.ctx = ctx
         self._workers = workers
         self.force = force
         self.analysis_mode = False
 
         # our input
-        self._graph_1 = ctx.graph
+        self._graph_1 = graph or ctx.graph or TargetGraph()
 
         self.stop = threading.Event()
 
         self._target_hash = {}
 
         self._disk_metadata = SqliteMetadataBackend(ctx.cache / DATABASE_FILE_NAME)
 
@@ -215,15 +216,15 @@
         except MakexFileCycleError as e:
             self.errors.append(e)
             self.stop.set()
             return False
 
         if True:
             requires = list(requires)
-            debug("Check target requires ready: %s", requires)
+            debug("Check task requires ready: %s", requires)
 
         statuses = []
         for target in requires:
             statuses.append(self._target_status.get(target.key(), False))
 
         return all(statuses)
 
@@ -250,15 +251,15 @@
     def _store_database(self, target):
         if self.ctx.dry_run:
             return
 
         if DATABASE_ENABLED:
             key = target.key()
             hash = self._get_target_hash(target)
-            trace("Storing target in database %s (%s)", key, hash)
+            trace("Storing task in database %s (%s)", key, hash)
             self._disk_metadata.put_target(key, hash)
 
     def execute_targets(self, *targets: TargetObject) -> ExecuteResult:
         """
 
         This will block/loop in a thread until all the targets are finished.
 
@@ -313,15 +314,15 @@
 
         trace("waiting: %s", self.waiting)
         i = 0
         try:
             while self.stop.is_set() is False:
                 # loop until we wait on nothing
                 if len(self.waiting) == 0:
-                    debug("No more targets waiting for processing.")
+                    debug("No more tasks waiting for processing.")
                     self.stop.set()
                     continue
 
                 while len(self.queued) == self._workers:
                     #trace("Queue wait")
                     time.sleep(0.1)
 
@@ -341,15 +342,15 @@
                 if isinstance(target, ResolvedTargetReference):
                     resolved_target = self._graph_1.get_target(target)
 
                     if resolved_target is None:
                         #raise Exception(f"Could not find target {target.name} in file {target.path}: {target.location}")
                         self.errors.append(
                             ExecutionError(
-                                f"Could not find target {target.name} in file {target.path}",
+                                f"Could not find task {target.name} in file {target.path}",
                                 target,
                                 target.location
                             )
                         )
                         self.stop.set()
                         break
 
@@ -404,15 +405,15 @@
         return self.finished, self.errors
 
     def _checksum_file(self, path: Path) -> FileChecksum:
         if self._supports_extended_attribute is False:
             # we need to store the checksum in a database sidecar
             # store the checksum in the database
             if DATABASE_ENABLED is False:
-                raise NotImplementedError("No where to store file checksum.")
+                raise NotImplementedError("Nowhere to store file checksum.")
 
             fingerprint = FileChecksum.get_fingerprint(path)
 
             string_path = str(path)
 
             checksum = self._disk_metadata.get_file_checksum(string_path, fingerprint)
 
@@ -435,15 +436,15 @@
             status = self.metadata.get_file_status(path)
             if status.checksum == checksum:
                 return False
 
         if self._supports_extended_attribute is False:
             # XXX: FS doesn't support xattr. Use the database to store/retrieve checksums.
             if DATABASE_ENABLED is False:
-                raise NotImplementedError("No where to check file checksum validity.")
+                raise NotImplementedError("Nowhere to check file checksum validity.")
 
             fingerprint = FileChecksum.get_fingerprint(path)
             string_path = str(path)
 
             database_checksum = self._disk_metadata.get_file_checksum(string_path, fingerprint)
             if database_checksum is None:
                 return True
@@ -552,15 +553,15 @@
             #trace("Process requirement %r", node)
             if isinstance(node, PathElement):
                 path = resolve_path_element_workspace(
                     ctx, target.workspace, node, target_input_path
                 )
 
                 if not path.exists():
-                    error = ExecutionError("Missing input file: {node}", target, node.location)
+                    error = ExecutionError(f"Missing input file: {path}", target, node.location)
                     errors.append(error)
 
                     inputs.append(FileStatus(path=path, error=error))
                 else:
                     if path.is_dir():
                         continue
 
@@ -636,15 +637,15 @@
                     )
 
                     # find the makex file inside of path
                     makex_file = find_makex_files(_path, ctx.makex_file_names)
 
                     if makex_file is None:
                         error = ExecutionError(
-                            f"No makex files found in path {_path} for the target's requirements.",
+                            f"No makex files found in path {_path} for the task's requirements.",
                             target,
                             path.location
                         )
                         #stop_and_error(error)
                         raise error
 
                     ref = ResolvedTargetReference(name, makex_file, location=path.location)
@@ -657,37 +658,37 @@
                     )
 
                     # find the makex file inside of path
                     makex_file = find_makex_files(_path, ctx.makex_file_names)
 
                     if makex_file is None:
                         error = ExecutionError(
-                            f"No makex files found in path {_path} for the target's requirements.",
+                            f"No makex files found in path {_path} for the task's requirements.",
                             target,
                             path.location
                         )
                         #stop_and_error(error)
                         raise error
 
                     ref = ResolvedTargetReference(name, makex_file, location=path.location)
                 else:
                     raise NotImplementedError(
-                        f"Invalid path in Target Reference. Got {type(path)}: {path}: node={node}"
+                        f"Invalid path in Task Reference. Got {type(path)}: {path}: node={node}"
                     )
 
                 requirement = self.graph_2.get_target(ref)
 
                 if requirement is None:
                     raise ExecutionError(
                         f"Missing requirement in graph: {ref}", target, target.location
                     )
                 requires.append(requirement)
             else:
                 raise ExecutionError(
-                    f"Invalid requirement in target {target.key()} {type(node)}",
+                    f"Invalid requirement in task {target.key()} {type(node)}",
                     target,
                     target.location
                 )
 
         outputs: list[FileStatus] = []
 
         unnamed_outputs: list[FileStatus] = []
@@ -702,25 +703,25 @@
             #debug("Rewrite output path %r %r %s", target_output_path, target.path, target)
             # TODO: use a method on TargetObject to get/transform outputs
             for k, path_like in target.outputs_dict.items():
 
                 if isinstance(path_like, list):
                     for value in path_like:
                         path = _transform_output_to_path(ctx, target, target_output_path, value)
-                        trace("Check target output: %s", path)
+                        trace("Check task output: %s", path)
                         status = self._get_output_file_status(path)
                         if k is None:
                             unnamed_outputs.append(status)
                         else:
                             output_dict.setdefault(k, []).append(status)
 
                         outputs.append(status)
                 else:
                     path = _transform_output_to_path(ctx, target, target_output_path, path_like)
-                    trace("Check target output: %s", path)
+                    trace("Check task output: %s", path)
                     status = self._get_output_file_status(path)
                     if k is None:
                         unnamed_outputs.append(status)
                     else:
                         output_dict[k] = status
 
                     outputs.append(status)
@@ -760,38 +761,41 @@
         )
 
         # TODO: queue target transformation in a separate pool and return a future here (once evaluated)
 
         if target.commands is not None and isinstance(target.commands, ListTypes) is False:
             location = figure_out_location(target.commands, target.location)
             err = PythonScriptError(
-                f"Target actions argument must be a list. Got {target.commands!r}", location
+                f"Task actions argument must be a list. Got {target.commands!r}", location
             )
             raise err
 
         for command in target.commands:
             # TODO: check we actually got a Action
             if isinstance(command, ListTypes):
                 for c in command:
                     if isinstance(c, InternalActionBase) is False:
                         location = figure_out_location(c, target.location)
 
                         err = PythonScriptError(
-                            f"Invalid action in target {target}: {c!r}",
+                            f"Invalid action in task {target}: {c!r}",
                             location,
                         )
                         raise err
                     else:
                         arguments = c.transform_arguments(ctx, evaluated)
                         actions.append(InternalAction(c, arguments))
+            elif command is None:
+                # XXX: skip None values in steps/actions lists.
+                continue
             elif isinstance(command, InternalActionBase) is False:
                 location = figure_out_location(command, target.location)
 
                 err = PythonScriptError(
-                    f"Invalid action in target {target}: {command!r}",
+                    f"Invalid action in task {target}: {command!r}",
                     location,
                 )
                 raise err
             else:
                 arguments = command.transform_arguments(ctx, evaluated)
                 actions.append(InternalAction(command, arguments))
 
@@ -805,37 +809,37 @@
         evaluated: EvaluatedTarget,
         h=None,
     ) -> tuple[bool, list[Exception]]:
 
         h = h or self._get_target_hash(evaluated)
         target_key = evaluated.key()
 
-        trace(f"Target hash is: %s of %r (exists=%s)", h, target_key, h in self._target_hash)
+        trace(f"Task hash is: %s of %r (exists=%s)", h, target_key, h in self._target_hash)
 
         if target_key in self._executed_keys:
             # we just executed this target, report it as dirty.
             # TODO: determine if this is correct.
-            trace(f"Target is dirty because it was just executed in this process. (%s)", target_key)
+            trace(f"Task is dirty because it was just executed in this process. (%s)", target_key)
             return True, []
 
         # TODO: we need to cache dirty checking so this doesn't go too deep.
         for require in evaluated.requires:
             dirty, _ = self._check_target_dirty(require)
             if dirty:
                 trace("Requirement of %s is dirty: %s", evaluated.key(), require.key())
                 return True, []
 
         # XXX: Targets without any outputs are always dirty. We can't compare the outputs.
         if len(evaluated.outputs) == 0:
-            trace(f"Target is dirty because it has no declared outputs. (%s)", target_key)
+            trace(f"Task is dirty because it has no declared outputs. (%s)", target_key)
             return True, []
 
         # XXX: Targets with outputs, but without any input files or requirements are always dirty.
         if len(evaluated.inputs) == 0 and len(evaluated.requires) == 0:
-            trace(f"Target is dirty because it has no requirements or inputs. (%s)", target_key)
+            trace(f"Task is dirty because it has no requirements or inputs. (%s)", target_key)
             return True, []
 
         # First, Check the in-memory cache
         target_dirty = self._memory_has_target(h) is False
 
         errors = []
 
@@ -844,31 +848,29 @@
         if DATABASE_ENABLED:
             if True: # only check if the in memory is empty
                 db_has_target = self._disk_metadata.has_target(target_key, h)
 
                 # We need to verify the outputs here because it's possible they are missing/screwed up, and we were not the ones who produced the target.
                 if db_has_target is True:
                     debug(
-                        f"Target in database. Checking outputs... (%r, hash=%r).",
-                        evaluated.key(),
-                        h
+                        f"Task in database. Checking outputs... (%r, hash=%r).", evaluated.key(), h
                     )
 
                     if self._check_outputs_stale_or_missing(evaluated, h):
                         # db has a target produced with the specified hash. outputs are still valid.
-                        debug(f"Target is dirty because the outputs are stale (%r).", target_key)
+                        debug(f"Task is dirty because the outputs are stale (%r).", target_key)
                         target_dirty = True
                     else:
-                        debug(f"Outputs of target are not stale (%r, hash=%r).", target_key, h)
+                        debug(f"Outputs of task are not stale (%r, hash=%r).", target_key, h)
                         target_dirty = False
 
                     _outputs_checked = True
                 else:
                     debug(
-                        f"Target is dirty because the database doesn't have the target (%r, hash=%r).",
+                        f"Task is dirty because the database doesn't have the target (%r, hash=%r).",
                         target_key,
                         h
                     )
                     target_dirty = True
 
                 if target_dirty is True:
                     return target_dirty, errors
@@ -876,15 +878,15 @@
         if target_dirty is False:
             # memory or db has the target
             #debug(f"Skipping target. Not dirty. (%r, hash=%r).", evaluated.key(), h)
             return target_dirty, errors
         else:
             # neither have the target
             debug(
-                "Target is dirty because hash isn't in memory or database: (%r, hash=%r)",
+                "Task is dirty because hash isn't in memory or database: (%r, hash=%r)",
                 target_key,
                 h,
             )
 
         if False:
             #hash = evaluated.hash(self.ctx)
 
@@ -964,21 +966,21 @@
                 # TODO: we should remove this branch once we remove use of Target.path
                 delete_output = False
             else:
                 delete_output = True
         else:
             delete_output = True
 
-        debug(f"Begin evaluate target {target}...")
+        debug(f"Begin evaluate task {target}...")
         # queue the requirements for execution if all dependencies are completed
         try:
             evaluated, errors = self._evaluate_target(target)
 
             if errors:
-                raise MultipleErrors(errors)
+                return None, [MultipleErrors(errors)]
         except (PythonScriptError, ExecutionError) as e:
             #logging.exception(e)
             #self.errors.append(e)
             # XXX: target evaluation errors must stop all execution.
             #self.stop.set()
             return None, [e]
 
@@ -1037,15 +1039,15 @@
         execute_list = [d, c, b, a]
         
         Execute list is ordered correctly, but it is not topographic/parallelized.
         The execute_list/queue is processed similarly; waiting for target dependants to finish before starting the target.
         """
 
         #self.ctx.ui.print(f"Evaluated target: {target.key()}")
-        debug("Evaluated target: %s", evaluated.key())
+        debug("Evaluated task: %s", evaluated.key())
 
         self.graph_2.add_target(evaluated)
 
         target_dirty, errors = self._check_target_dirty(evaluated)
 
         # all([]) -> True
         #target_dirty = all(checksums)
@@ -1064,18 +1066,18 @@
             self._queue_target_on_pool(evaluated, delete_output, hash)
             return evaluated, None
 
         # dirty checking applicable
         if target_dirty is False:
             self._mark_target_complete(evaluated)
             #self._queue_for_database(evaluated)
-            debug("Skipping target. Not dirty: %s", evaluated.key())
+            debug("Skipping task. Not dirty: %s", evaluated.key())
             return evaluated, None
 
-        info("Target has been deemed dirty. Queueing for execution: %s", evaluated.key())
+        info("Task has been deemed dirty. Queueing for execution: %s", evaluated.key())
         self._queue_target_on_pool(evaluated, delete_output, hash)
         return evaluated, None
 
     def _queue_target_on_pool(self, evaluated: EvaluatedTarget, delete_output, hash) -> None:
         # TODO: we should get a future here.
         #  if there was an exception, stop everything, both execution and evaluation.
         #  if all the requirements have evaluated (or no requirements), execute.
@@ -1085,30 +1087,30 @@
         #   if none or only some of the deps have evaluated, keep it waiting
         #info(f"Queue target for execution {evaluated}")
 
         cache_exists = evaluated.cache_path.exists()
         if cache_exists:
             if REMOVE_CACHE_DIRTY_TARGETS_ENABLED and delete_output:
                 debug(
-                    "Removing cache of %s (%s) because target is dirty.",
+                    "Removing cache of %s (%s) because task is dirty.",
                     evaluated.key(),
                     evaluated.cache_path
                 )
                 # remove the cache if the target is dirty
                 rmtree(evaluated.cache_path)
                 evaluated.cache_path.unlink(missing_ok=True)
 
                 logging.debug("Creating output directory %s", evaluated.cache_path)
                 evaluated.cache_path.mkdir(parents=True, exist_ok=True)
         # create a single link from _output_ to cache's _output_
         elif cache_exists is False:
             logging.debug("Creating output directory %s", evaluated.cache_path)
             evaluated.cache_path.mkdir(parents=True, exist_ok=True)
 
-        debug("Output2 %s", list(evaluated.input_path.iterdir()))
+        #debug("Output2 %s", list(evaluated.input_path.iterdir()))
         # autogenerated path
         if SYMLINK_PER_TARGET_ENABLED is False:
             # create link Target.input_path / _output_ -> Target.cache_path.parent (_output_)
             self._create_output_link(evaluated, evaluated.cache_path.parent)
         else:
             # create a link from Target.input_path / _output_ / Target.id - > Target.cache_path
             raise NotImplementedError()
@@ -1123,15 +1125,15 @@
         if metadata is None:
             return []
         return metadata.inputs
 
     def _check_output_hash_valid(self, path: Path, hash: str):
         # check the hash stored in the output file matches our target
         if hash != _get_xattr(path, _XATTR_OUTPUT_TARGET_HASH).decode("ascii"):
-            trace("Target.hash != output.hash: %s %s", path, hash)
+            trace("Task.hash != output.hash: %s %s", path, hash)
             return False
 
         return True
 
     def _check_outputs_stale_or_missing(self, target: EvaluatedTarget, target_hash: str):
         # Return True if any outputs are missing or stale
         dirty = True
@@ -1172,15 +1174,15 @@
 
         errors = []
         for output in target.outputs:
             path = output.path
             if not path.exists():
                 errors.append(
                     ExecutionError(
-                        f"Target failed to create output file. Missing file at: {path}",
+                        f"Task failed to create output file. Missing file at: {path}",
                         target,
                         target.location
                     )
                 )
         return errors
 
     def _get_target_hash(self, target: EvaluatedTarget):
@@ -1188,25 +1190,25 @@
         hash = self._hash_cache.get(key, None)
         if hash is None:
             hash = self._hash_cache[key] = target.hash(self.ctx, hash_cache=self._target_hash)
 
         return hash
 
     def _put_target_hash(self, target: EvaluatedTarget, hash):
-        trace("Store target hash %s %s", target.key(), hash)
+        trace("Store task hash %s %s", target.key(), hash)
         self._target_hash[target.key()] = hash
 
     def _target_completed(self, target: EvaluatedTarget, result: Future[TargetResult]):
         # Called after the Future is completed.
         # Called in *this* thread (not the thread in which the target was executed).
         assert isinstance(target, EvaluatedTarget)
 
         self._mark_target_executed(target)
 
-        debug("Target complete %s", target)
+        debug("Task complete %s", target)
 
         # store the hash in the cache for later.
         h = self._get_target_hash(target)
         self._put_target_hash(target, h)
 
         exc = result.exception()
         if exc:
@@ -1239,27 +1241,27 @@
 
     def _write_queued_to_database(self):
         if self.ctx.dry_run is True:
             return None
 
         while self._database_queue:
             target = self._database_queue.popleft()
-            trace("Writing queue target %r to database", target.key())
+            trace("Writing queued task %r to database", target.key())
             self._store_database(target)
 
     def _write_target_hash_to_outputs(self, target_hash: bytes, outputs: list[FileStatus]):
         #target_hash_bytes = target_hash.encode("utf-8")
         for output in outputs:
             _set_xattr(output.path, _XATTR_OUTPUT_TARGET_HASH, target_hash)
 
     def _execute_target_thread(self, ctx: Context, target: EvaluatedTarget, target_hash):
         # this is run in a separate thread...
-        debug(f"Begin execution of target: {target} [thread={threading.current_thread().ident}]")
+        debug(f"Begin execution of task: {target} [thread={threading.current_thread().ident}]")
 
-        ctx.ui.print(f"Execute target: {target.key()}")
+        ctx.ui.print(f"Execute task: {target.key()}")
         output = StringIO()
 
         # create a copy of the ctx.environment, so we can set ctx.environment variables throughout the process.
         with ctx.new_environment() as subcontext:
             #context = ctx or subcontext
             context = subcontext
             for command in target.actions or []:
@@ -1277,15 +1279,15 @@
                     raise ExecutionError(message, target, command.location or target.location)
 
                 trace("Execution return status: %s", execution)
 
                 if execution.status != 0: #not in {0, CORRECTED_RETURN_CODE}:
                     # \n\n {execution.output} \n\n {execution.error}
                     string = [
-                        f"Error running the action for target ",
+                        f"Error running the action for task ",
                         f"{brief_target_name(context, target, color=True)}:{target.location.line} (exit={execution.status}) \n",
                         f"\tThe process had an error and returned non-zero status code ({execution.status}). See above for any error output."
                     ]
                     raise ExecutionError(
                         "".join(string), target, command.location or target.location
                     )
 
@@ -1293,13 +1295,13 @@
                     # XXX: not required as execution dumps stdout. we may want to capture
                     output.write(execution.output)
 
                 #except Exception as e:
                 #    logging.exception(e)
                 #   pass
 
-        debug(f"Finished execution of target: {target}")
+        debug(f"Finished execution of task: {target}")
 
         if STORE_TASK_HASH_IN_OUTPUT_FILES:
             self._write_target_hash_to_outputs(target_hash, target.outputs)
 
         return TargetResult(target, output=output.getvalue())
```

### Comparing `makex-20240401/python/makex/executor_test.py` & `makex-20240601/python/makex/executor_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,28 +30,40 @@
 from makex.workspace import Workspace
 
 
 class PathMaker:
     def __init__(self, root=None):
         self.root = root or Path.cwd()
 
+    def __truediv__(self, other):
+        path = Path(other)
+        parent = self.root
+
+        if not path.is_absolute():
+            path = parent / path
+        else:
+            path = path
+
+        return PathElement(*path.parts, resolved=path)
+
     def path(self, *args):
         path = Path(*args)
         #if not args:
         #    return PathElement(*args, resolved=path)
 
         parent = self.root
 
         if not path.is_absolute():
             path = parent / path
         else:
             path = path
 
         return PathElement(*path.parts, resolved=path)
 
+    __call__ = path
 
 def test_sort(tmp_path):
     """
     diamond:
     a
     /\
     bc
@@ -90,16 +102,15 @@
     bc
     \/
     d
 
 
     """
 
-    pathmaker = PathMaker()
-    path = pathmaker.path
+    path = PathMaker(tmp_path)
 
     l = fake_location(tmp_path / "Makefilex")
 
     assert TargetObject("d", location=l) == TargetObject("d", location=l)
     assert TargetObject("a", location=l) != TargetObject("d", location=l)
 
     assert TargetObject(
@@ -202,19 +213,17 @@
     input.joinpath("a").write_text("a")
     input.joinpath("b").write_text("b")
     input.joinpath("c").write_text("c")
     input.joinpath("d").write_text("d")
 
     location = fake_location(input_make_file)
 
-    o_pathmaker = PathMaker(output)
-    opath = o_pathmaker.path
+    opath = PathMaker(output)
 
-    i_pathmaker = PathMaker(input)
-    ipath = i_pathmaker.path
+    ipath = PathMaker(input)
 
     debug("$SSSSS %s", opath())
 
     makex_file = MakexFile(None, input_make_file)
     d = TargetObject(
         "d",
         path=opath(),
```

### Comparing `makex-20240401/python/makex/file_checksum.py` & `makex-20240601/python/makex/file_checksum.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
 INODE_IN_FINGERPRINT = False
 
 # must be prefixed with user. otherwise we will get OSError, Operation not supported
 TEST_KEY = b"user.test"
 TEST_VALUE = b"test"
 
+# hash will be stored in XATTR_PREFIX.algorithm
+XATTR_PREFIX="user.checksum"
 
 def get_digest_data(data: BinaryIO, hash_func=hashlib.sha256):
     h = hash_func()
     while True:
         # Reading is buffered, so we can read smaller chunks.
         chunk = data.read(h.block_size)
         if not chunk:
@@ -161,15 +163,15 @@
         if not os.access(path, os.W_OK):
             st = os.stat(path)
             new_mode = st.st_mode | stat.S_IXUSR | stat.S_IWGRP | stat.S_IWGRP | stat.S_IWRITE
             LOGGER.debug(f"Updating file mode {new_mode}: %s", path)
             os.chmod(path, new_mode)
 
         try:
-            set_xattr(path, f"user.checksum.{type.value}", bytes(f"{d}:{fingerprint}", "ascii"))
+            set_xattr(path, f"{XATTR_PREFIX}.{type.value}", bytes(f"{d}:{fingerprint}", "ascii"))
         except OSError as e:
             logging.error(e)
             pass
 
         return cls(type, d, fingerprint)
 
     @classmethod
@@ -251,15 +253,15 @@
         # inodes (may/likely) change when files are copied, no matter copy on write.
         csum, csum_fingerprint = get_filechecksum_xattr(path, type)
 
         if csum is None:
             return False
 
         fingerprint = get_fingerprint(path)
-        set_xattr(path, f"user.checksum.{type.value}", bytes(f"{csum}:{fingerprint}", "ascii"))
+        set_xattr(path, f"{XATTR_PREFIX}.{type.value}", bytes(f"{csum}:{fingerprint}", "ascii"))
         return True
 
     @classmethod
     def compare(cls, a, b, type: Type = Type.SHA256):
         """
         Compare the xattrs of a and b and
 
@@ -314,15 +316,15 @@
 
         if INODE_IN_FINGERPRINT:
             # regenerate a fingerprint when copying with inodes in the fingerprint
             # inodes (may/likely) change when files are copied, no matter copy on write.
             fingerprint = get_fingerprint(destination).encode("ascii")
 
         set_xattr(
-            destination, f"user.checksum.{type.value}", bytes(f"{csum}:{fingerprint}", "ascii")
+            destination, f"{XATTR_PREFIX}.{type.value}", bytes(f"{csum}:{fingerprint}", "ascii")
         )
 
     @staticmethod
     def get_fingerprint(path: Path, type: Type = Type.SHA256) -> Optional[str]:
         return get_fingerprint(path)
 
 
@@ -331,15 +333,15 @@
     #shutil.copystat(source, destination)
     FileChecksum.copy(source, destination)
 
 
 def get_filechecksum_xattr(path: Path, type: FileChecksum.Type) -> tuple[str, str]:
     assert isinstance(type, FileChecksum.Type)
     try:
-        csum = get_xattr(path, f"user.checksum.{type.value}").decode("ascii")
+        csum = get_xattr(path, f"{XATTR_PREFIX}.{type.value}").decode("ascii")
         csum, csum_fingerprint = csum.split(":")
 
     except ValueError:
         return None, None
     except IOError as e:
         #logging.exception(e)
         return None, None
@@ -370,16 +372,17 @@
     # check if still valid
 
     fingerprint = get_fingerprint(path)
     csum = None
     csum_fingerpint = None
 
     try:
-        csum = get_xattr(path, f"user.checksum.{type.value}").decode("ascii")
+        csum = get_xattr(path, f"{XATTR_PREFIX}.{type.value}").decode("ascii")
         csum, csum_fingerpint = csum.split(":")#x.get(f"user.checksum.{type.value}.fingerprint").decode("ascii")
     except ValueError:
         return None, None, None
     except IOError:
         # xattr raises exceptions if the file doesn't have the properties
         pass
 
     return csum, csum_fingerpint, fingerprint
+
```

### Comparing `makex-20240401/python/makex/file_cloning.py` & `makex-20240601/python/makex/file_cloning.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/file_system.py` & `makex-20240601/python/makex/file_system.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/flags.py` & `makex-20240601/python/makex/flags.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,25 @@
 
     if v in {"true", "1", "on"}:
         return True
     else:
         return False
 
 
+
+def _get_string(name, default: bool = _SENTINEL, prefix="MAKEX_", environ=environ) -> bool:
+    v = environ.get(f"{prefix}{name}", None)
+    if v is None:
+        if default is not _SENTINEL:
+            return default
+        return None
+
+    return name
+
+
 # Enable/disable all features in development, which may not be documented.
 DEVELOPMENT_ENABLED = _get_bool("DEVELOPER", False)
 
 # Enable detection of nested Workspaces
 NESTED_WORKSPACES_ENABLED = _get_bool("NESTED_WORKSPACES_ENABLED", True)
 
 # Enable the `find() function in makex files. Default to True.
@@ -83,14 +94,19 @@
 INCLUDE_ENABLED = _get_bool("INCLUDE_ENABLED", True)
 
 # allow includes to make an `include()` call.
 INCLUDE_MULTIPLE_LEVEL_ENABLED = False
 
 IMPORT_ENABLED = _get_bool("IMPORT_ENABLED", False)
 
+
+# Allow explicitly specifying the configuration file name. This will skip use of
+# the builtin file names.
+CONFIGURATION_FILE_NAME = _get_string("CONFIGURATION_FILE_NAME", None)
+
 # Strict mode
 # - Disable the shell (unless really explicit)
 # - Make sure all used files are declared (or just handle this implicitly)
 # - Disable globs/finds
 # - Using paths of another target should be prohibited unless it is an internal (copy/sync/write).
 #   - Any paths of required targets become a dependency and would break composition.
 # - If shell must be enabled, disable __str__ on any PathObject so they can't be hidden in shell strings.
```

### Comparing `makex-20240401/python/makex/integrations/intellij.py` & `makex-20240601/python/makex/integrations/intellij.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/makex_file.py` & `makex-20240601/python/makex/makex_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import ast
 import logging
 import os
 import re
 import shlex
 import shutil
 import types
+import typing
+import zipfile
 from abc import (
     ABC,
     abstractmethod,
 )
 from dataclasses import dataclass
 from io import StringIO
 from itertools import chain
@@ -85,41 +87,38 @@
     make_glob_pattern,
 )
 from makex.protocols import (
     CommandOutput,
     StringHashFunction,
 )
 from makex.python_script import (
+    FILE_LOCATION_ARGUMENT_NAME,
     GLOBALS_NAME,
     FileLocation,
     ListValue,
     PythonScriptError,
     PythonScriptFile,
     ScriptEnvironment,
     StringValue,
-    _create_file_location_call,
+    add_location_keyword_argument,
     call_function,
+    create_file_location_call,
     is_function_call,
     wrap_script_function,
 )
 from makex.run import run
 from makex.target import (
     ArgumentData,
     EvaluatedTarget,
     format_hash_key,
     target_hash,
 )
 from makex.ui import pretty_file
 from makex.version import VERSION
 from makex.workspace import Workspace
-from typing_extensions import (
-    NotRequired,
-    Required,
-    Unpack,
-)
 
 _TARGET_REFERENCE_NAME = "Reference"
 _MACRO_DECORATOR_NAME = "macro"
 
 TARGETS_MODULE_VARIABLE = "_TARGETS_"
 MACROS_MODULE_VARIABLE = "__macros__"
 MACRO_NAMES_MODULE_VARIABLE = "__macro_names__"
@@ -155,16 +154,14 @@
     "home",
     "archive",
     "mirror",
     "sync",
     "include",
 }
 
-# TODO: move these to makex_file_types
-
 
 def _validate_path(
     parts: Union[list[StringValue], tuple[StringValue]],
     location: FileLocation,
     absolute=ABSOLUTE_PATHS_ENABLED,
 ):
     if ".." in parts:
@@ -177,26 +174,30 @@
 VALID_NAME_RE = r"^[a-zA-Z][a-zA-Z0-9\-._@]*"
 VALID_NAME_PATTERN = re.compile(VALID_NAME_RE, re.U)
 
 
 def _validate_target_name(name: StringValue, location: FileLocation):
     if not VALID_NAME_PATTERN.match(name):
         raise PythonScriptError(
-            f"Target has an invalid name {name!r}. Must be {VALID_NAME_RE!r} (regular expression).",
+            f"Task has an invalid name {name!r}. Must be {VALID_NAME_RE!r} (regular expression).",
             location
         )
     return True
 
 
 def resolve_string_path_workspace(
     ctx: Context,
     workspace: Workspace,
     element: StringValue,
     base: Path,
 ) -> Path:
+
+    if element.value == ".":
+        return base
+
     _path = path = Path(element.value)
 
     _validate_path(path.parts, element.location)
 
     if path.parts[0] == "//":
         #trace("Workspace path: %s %s", workspace, element)
         if WORKSPACES_IN_PATHS_ENABLED:
@@ -293,18 +294,30 @@
                 raise ExecutionError(
                     f"Globs are not allowed in the {name} property.", target, value.location
                 )
             # TODO: handle find() here as well
             # todo: use glob cache from ctx for multiples of the same glob during a run
             #pattern = make_glob_pattern(value.pattern)
             #pattern = re.compile(pattern)
+            # TODO: Handle ignores
             ignore = {ctx.output_folder_name}
             #yield from find_files(base, pattern, ignore_names=ignore)
 
             yield from resolve_glob(ctx, target, base, value, ignore_names=ignore)
+        elif isinstance(value, FindFiles):
+            # find(path, pattern, type=file|symlink)
+            if value.path:
+                path = resolve_path_element_workspace(ctx, target.workspace, value.path, base)
+            else:
+                path = base
+
+            # TODO: Handle ignores
+            debug("Searching for files %s: %s", path, value.pattern)
+            ignore = {ctx.output_folder_name}
+            yield from resolve_find_files(ctx, target, path, value.pattern, ignore_names=ignore)
         elif isinstance(value, PathObject):
             yield value.path
         elif IGNORE_NONE_VALUES_IN_LISTS and value is None:
             continue
 
         else:
             #raise ExecutionError(f"{type(value)} {value!r}", target, getattr(value, "location", target))
@@ -454,17 +467,15 @@
     else:
         path_string = f"{base}:{path_string}"
 
     # XXX: prepend the current folder to the path so executables are found next to the makex file.
     _path = shutil.which(name, path=path_string)
 
     if _path is None:
-        error(
-            "Which could not find the executable for %r: PATH=%s", name, os.environ.get("PATH", "")
-        )
+        error("Which could not find the executable for %r: PATH=%s", name, path_string)
         raise ExecutionError(
             f"Could not find the executable for {name}. Please install whatever it "
             f"is that provides the command {name!r}, or modify your PATH environment variable "
             f"to include the path to the {name!r} executable.",
             target
         )
 
@@ -742,14 +753,30 @@
         return {output_folder_name}
 
     return f
 
 
 @dataclass
 class Copy(InternalActionBase):
+    """
+    Copies files/folders.
+
+    #  copy(items) will always use the file/folder name in the items list
+    #  copy(file)
+    #  copy(files)
+    #  copy(folder)
+    #  copy(folders)
+    # with destination:
+    #  copy(file, folder) copy a file to specified folder.
+    #  copy(files, folder) copies a set of files to the specified folder.
+    #  copy(folder, folder) copy a folder to the inside of specified folder.
+    #  copy(folders, folder) copies a set of folders to the specified folder..
+
+    # TODO: rename argument?
+    """
     source: Union[list[AllPathLike], PathLikeTypes]
     destination: PathLikeTypes
     exclude: list[AllPathLike]
     location: FileLocation
     destination_is_subdirectory: bool = False
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function):
@@ -801,15 +828,14 @@
                     name="source",
                     base=target.input_path,
                     value=self.source
                 )
             ]
 
         if self.destination:
-
             if not isinstance(self.destination, (str, PathObject, PathElement)):
                 raise PythonScriptError("Destination must be a string or path.", self.location)
 
             if isinstance(self.destination, str):
                 if "/" in self.destination:
                     self.destination_is_subdirectory = True
 
@@ -854,19 +880,16 @@
         self, ctx: Context, target: EvaluatedTarget, arguments: ArgumentData
     ) -> CommandOutput:
         sources = arguments.get("sources")
         destination: Path = arguments.get("destination")
         excludes: Pattern = arguments.get("excludes")
 
         destination_specified = destination is not None
-        if destination_specified:
-            destination_is_folder = destination.is_dir()
-        else:
+        if destination_specified is False:
             destination = target.path
-            destination_is_folder = True
 
         copy_file = ctx.copy_file_function
 
         if destination.exists() is False:
             debug("Create destination %s", destination)
             if ctx.dry_run is False:
                 destination.mkdir(parents=True)
@@ -892,63 +915,35 @@
                     trace("Copy/ignore: %s", path)
                     _names.add(name)
                 elif excludes and excludes.match(path):
                     trace("Copy/exclude: %s", path)
                     _names.add(name)
             return _names
 
-        # XXX: keep n sources so we can determine which form of copy() we have (8 forms).
-        #  copy(items) will always use the file/folder name in the items list
-        #  copy(files)
-        #  copy(file)
-        #  copy(folders)
-        #  copy(folder)
-        # with destination:
-        #  copy(file, file) copy a file to specified file path. TODO: this doesn't work. remove this. suggest install()
-        #  copy(file, folder) copy a file to specified folder.
-        #  copy(folder, folder) allows renaming or mirroring a folder.
-        #  copy(folders, folder) copies a set of folders to the specified folder..
-        #  copy(files, folder) copies a set of files to the specified folder.
-
-        #  copy(file, "folder" / file) allows renaming a file and prefixing it into a folder. TODO: remove this. suggest install()
-        n_sources = len(sources)
-
         for source in sources:
-
             if not source.exists():
                 raise ExecutionError(
                     f"Missing source file {source} in copy list",
                     target,
                     getattr(source, "location", target.location)
                 )
 
             if ignore_pattern.match(source.as_posix()):
                 trace("File copy ignored %s", source)
                 continue
 
-            #trace("Copy source %s", source)
-            if destination_specified:
-                # destination was specified, one of:
-                # copy(folder, folder)
-                # copy(folders, folder)
-                # copy(file, file)
-                # copy(files, destination)
-                if n_sources == 1:
-                    _destination = destination
-                else:
-                    _destination = destination / source.name
-            else:
-                # destination not specified, one of:
+            source_is_dir = source.is_dir()
+            _destination = destination / source.name
+
+            if source_is_dir:
                 # copy(folder)
                 # copy(folders)
-                # copy(file)
-                # copy(files)
-                _destination = destination / source.name
+                # copy(folder, folder)
+                # copy(folders, folder)
 
-            if source.is_dir():
                 debug("Copy tree %s <- %s", _destination, source)
 
                 if ctx.dry_run is False:
                     try:
                         # copy recursive
                         shutil.copytree(
                             source,
@@ -974,14 +969,18 @@
                     except OSError as e:
                         string = [
                             f"Error copying tree {source} to {destination}:\n  Error to {e.filename} from {e.filename2}: {type(e)}: {e.args[0]} {e} "
                         ]
 
                         raise ExecutionError("\n".join(string), target, target.location) from e
             else:
+                # copy(file)
+                # copy(files)
+                # copy(file, folder)
+                # copy(files, folder)
                 trace("Copy file %s <- %s", _destination, source)
                 if ctx.dry_run is False:
                     try:
                         copy_file(source.as_posix(), _destination.as_posix())
                     except (OSError, shutil.Error) as e:
                         raise ExecutionError(
                             f"Error copying file {source} to {_destination}: {e}",
@@ -1007,14 +1006,23 @@
         - sub/directory
 
         destination argument (e.g. "source" or "source/") will prefix the paths with the destination:
 
         - source/directory1
         - source/file1
         - source/sub/directory
+
+        mirror(file, file): mirror a file into output with a new name
+        mirror(folder, folder): mirror a folder into output with a new name
+
+        mirror(file): mirror a file into output (redundant with copy)
+        mirror(folder): mirror a folder into output (redundant with copy)
+
+        mirror(files, folder): mirror files into folder (redundant with copy)
+        mirror(folders, folder): mirror folders into folder (redundant with copy)
     """
     source: Union[list[AllPathLike], AllPathLike]
     destination: PathLikeTypes
     exclude: list[MultiplePathLike]
     location: FileLocation
     symlinks = False
 
@@ -1251,14 +1259,164 @@
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
         environment = arguments.get("environment")
         environment_string = ";".join(f"{k}={v}" for k, v in environment.items())
         return hash_function(environment_string)
 
 
+class ArchiveCommand(InternalActionBase):
+    """
+     TODO:
+    archive(
+        path=task_path("rpm") / "SOURCES/makex-source.zip",
+        type=None, # automatically inferred from extension
+        root=".", # base/path which all items should be relative to.
+        files=[
+            find()
+        ]
+    ),
+    """
+    path: PathLikeTypes
+    type: typing.Literal["zip", "tar.gz"]
+    root: PathLikeTypes
+    prefix: PathLikeTypes
+    options: dict
+    files: list[AllPathLike]
+    location: FileLocation
+
+    environment: dict[StringValue, Union[StringValue, PathLikeTypes]]
+
+    def __init__(
+        self,
+        path: PathLikeTypes,
+        root,
+        type,
+        options,
+        files,
+        prefix=None,
+        location: FileLocation = None
+    ):
+        self.path = path
+        self.root = root
+        self.type = type
+        self.options = options
+        self.files = files
+        self.prefix = prefix
+        self.location = location
+
+    def transform_arguments(self, ctx: Context, target: EvaluatedTarget) -> ArgumentData:
+        files = list(
+            resolve_pathlike_list(
+                ctx=ctx,
+                target=target,
+                name="files",
+                base=target.input_path,
+                values=self.files or [],
+            )
+        )
+        path = _resolve_pathlike(ctx, target, target.input_path, "path", self.path)
+        if self.root:
+            root = _resolve_pathlike(ctx, target, target.input_path, "path", self.root)
+        else:
+            root = target.input_path
+
+        options = self.options
+        type = self.type
+
+        if self.type is None:
+            if path.suffix == ".zip":
+                type = "zip"
+            elif path.suffix == ".tar.gz":
+                type = "tar.gz"
+            else:
+                raise PythonScriptError(
+                    "Could not detect archive type from filename. Specify type=zip|tar.gz",
+                    self.location
+                )
+
+        return ArgumentData(
+            {
+                "path": path,
+                "type": type,
+                "prefix": self.prefix,
+                "root": root,
+                "options": options,
+                "files": files,
+            }
+        )
+
+    def run_with_arguments(self, ctx: Context, target: EvaluatedTarget, arguments) -> CommandOutput:
+        type = arguments.get("type")
+
+        if type == "zip":
+            return self._run_zip(ctx, target, arguments)
+        elif type == "tar.gz":
+            raise NotImplementedError(type)
+            return self._run_tar_gz(ctx, target, arguments)
+        else:
+            raise NotImplementedError(type)
+
+    def scantree(self, path):
+        """Recursively yield DirEntry objects for given directory."""
+        for entry in os.scandir(path):
+            if entry.is_dir(follow_symlinks=False):
+                yield from self.scantree(entry.path) # see below for Python 2.x
+            else:
+                yield entry
+
+    def _run_zip(self, ctx, target, arguments) -> CommandOutput:
+        path = arguments.get("path")
+        root = arguments.get("root")
+        prefix = arguments.get("prefix")
+        if prefix:
+            prefix = Path(prefix)
+
+        zipobj = zipfile.ZipFile(path, 'w', zipfile.ZIP_DEFLATED)
+        files: list[Path] = arguments.get("files")
+
+        for file in files:
+
+            if file.is_relative_to(root):
+                is_relative = True
+                file_relative = file.relative_to(root)
+            else:
+                is_relative = False
+                file_relative = file
+
+            if file.is_dir():
+                for direntry in self.scantree(file):
+                    #if direntry.is_dir():
+                    #    continue
+                    arcpath = Path(direntry.path
+                                   ).relative_to(root) if is_relative else direntry.path
+
+                    if prefix:
+                        arcpath = prefix / arcpath
+
+                    zipobj.write(direntry.path, arcpath)
+            else:
+
+                zipobj.write(file, file_relative)
+
+        return CommandOutput(0)
+
+    def _run_tar_gz(self, ctx, target, arguments):
+        return CommandOutput(0)
+
+    def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
+        parts = []
+        parts.append(str(arguments.get("path")))
+        parts.append(arguments.get("type"))
+        parts.append(str(arguments.get("options")))
+        parts.append(str(arguments.get("root")))
+        parts.append(str(arguments.get("files")))
+        string = "".join(parts)
+        return hash_function(string)
+
+
 class InsertAST(ast.NodeTransformer):
     def __init__(self, path, asts: list[ast.AST]):
         self.path = path
         self.asts = asts
 
     def visit_Module(self, node: ast.Module) -> Any:
         node.body = self.asts + node.body
@@ -1336,16 +1494,15 @@
         line = node.lineno
         offset = node.col_offset
         slice: ast.Slice = node.slice
 
         lower = slice.lower or ast.Constant(None, lineno=line, col_offset=offset)
         upper = slice.upper or ast.Constant(None, lineno=line, col_offset=offset)
         step = slice.step or ast.Constant(None, lineno=line, col_offset=offset)
-
-        file_location = _create_file_location_call(self.path, line, offset)
+        file_location = create_file_location_call(self.path, line, offset)
 
         reference_call = ast.Call(
             func=ast.Name(
                 id=_TARGET_REFERENCE_NAME,
                 ctx=ast.Load(),
                 lineno=line,
                 col_offset=offset,
@@ -1361,15 +1518,15 @@
                 ast.keyword(
                     arg='path',
                     value=lower,
                     lineno=line,
                     col_offset=offset,
                 ),
                 ast.keyword(
-                    arg='location',
+                    arg=FILE_LOCATION_ARGUMENT_NAME,
                     value=file_location,
                     lineno=line,
                     col_offset=offset,
                 ),
             ],
             lineno=line,
             col_offset=offset,
@@ -1593,21 +1750,14 @@
     for name in names:
         check = path / name
         if check.exists():
             return check
     return None
 
 
-@dataclass
-class ArchiveCommand:
-    path: PathLike
-    prefix: PathLike
-    location: FileLocation
-
-
 class IncludeFunction(Protocol):
     def __call__(
         self,
         ctx: Context,
         workspace: Workspace,
         base: Path,
         search_path: str,
@@ -1635,19 +1785,56 @@
         return output
     elif isinstance(output, PathObject):
         return output
     elif isinstance(output, PathElement):
         return output
     else:
         raise PythonScriptError(
-            f"Invalid output type {type(output)} in output list for target {target_name}: {output}",
+            f"Invalid output type {type(output)} in output list for task {target_name}: {output}",
             location
         )
 
 
+if typing.TYPE_CHECKING:
+
+    from typing_extensions import (
+        NotRequired,
+        Required,
+        Unpack,
+    )
+
+    # TODO: remove this in the future when >=3.12 is expected
+    class TargetArguments(TypedDict):
+        name: str
+        label: str
+        path: NotRequired[Path]
+        requires: NotRequired[list[str]]
+        runs: NotRequired[list]
+        actions: NotRequired[list]
+        outputs: NotRequired[list]
+        inputs: NotRequired[dict]
+        location: Required[FileLocation]
+
+    #**kwargs: Unpack[TargetArguments]
+    # NotRequired
+    #
+else:
+
+    class TargetArguments(TypedDict):
+        name: str
+        label: str
+        path: Path
+        requires: list[str]
+        runs: list
+        actions: list
+        outputs: list
+        inputs: dict
+        location: FileLocation
+
+
 class MakexFileScriptEnvironment(ScriptEnvironment):
     class Task:
         def __init__(self, env):
             self.env = env
 
         def __getitem__(self, item):
             if item not in {"path"}:
@@ -1698,23 +1885,19 @@
 
         g = {
             #**self._globals,
             **parent,
             TARGETS_MODULE_VARIABLE: self.targets,
             MACROS_MODULE_VARIABLE: self.macros,
             "Environment": self.environment, #"pattern": wrap_script_function(self._pattern),
-            "ENVIRONMENT": self.environment,
+            "ENVIRONMENT": self.environment, # TODO: deprecate this:
             "target": wrap_script_function(self._function_target),
-
- # TODO: declare new aliases:
             "Task": wrap_script_function(self._function_task),
             "task": wrap_script_function(self._function_task),
             _TARGET_REFERENCE_NAME: wrap_script_function(self._function_Target),
-            #TODO: define a Target object for type references
-            #"Target": wrap_script_function(self._function_Target),
             _MACRO_DECORATOR_NAME: self._decorator_macro, #"macro": Decorator,
         }
 
         if INCLUDE_ENABLED:
             g["include"] = self._function_include
 
         # path utilities
@@ -1738,16 +1921,15 @@
         if FIND_FUNCTION_ENABLED:
             g["find"] = wrap_script_function(self._function_find)
 
         # Actions
         g.update(
             {
                 "print": wrap_script_function(self._function_print),
-                "shell": wrap_script_function(self._function_shell),
-                # TODO: deprecate sync
+                "shell": wrap_script_function(self._function_shell), # TODO: deprecate sync
                 "sync": wrap_script_function(self._function_sync),
                 "mirror": wrap_script_function(self._function_sync),
                 "execute": wrap_script_function(self._function_execute),
                 "copy": wrap_script_function(self._function_copy),
                 "write": wrap_script_function(self._function_write),
                 "environment": wrap_script_function(self._function_environment),
             }
@@ -1842,30 +2024,30 @@
         debug("Importing macros from %s: %s", path, _macros.keys())
 
         _globals.update(_macros)
 
         self.includes.add(file)
 
         if tasks:
-            trace("Adding targets from included file: %s", module._TARGETS_.keys())
+            trace("Adding tasks from included file: %s", module._TARGETS_.keys())
             self.targets.update(module._TARGETS_)
 
     def _function_expand(self, string: StringValue, location: FileLocation):
         return Expansion(context=self.ctx, string=string, location=location)
 
     def _function_home(self, *path, user=None, location=None):
         if user:
             arg = f"~{user}"
         else:
             arg = "~"
         home = expanduser(arg)
 
         _path = Path(home)
         if path:
-            _path =  _path.joinpath(*path)
+            _path = _path.joinpath(*path)
 
         return PathElement(arg, resolved=_path, location=location)
 
     def _function_find(
         self, path: PathLikeTypes, expr: Union[Glob, RegularExpression] = None, location=None
     ):
 
@@ -1928,23 +2110,45 @@
         )
 
     def _function_source(self, *path: StringValue, location=None):
         if not path:
             # XXX: No path. Return the source directory.
             return PathElement(*self.directory.parts, resolved=self.directory, location=location)
 
+        # OPTIMIZATION: fast path for sources with a single Path() argument
+        if len(path) == 1:
+            path0 = path[0]
+            if isinstance(path0, PathElement):
+                _parts = self.directory.parts + path0.parts
+                resolved = self.directory / path0._as_path()
+                return PathElement(*_parts, resolved=resolved, location=location)
+            elif isinstance(path0, StringValue):
+                resolved = self.directory / path0
+                return PathElement(path0, resolved=resolved, location=location)
+            else:
+                raise PythonScriptError(
+                    f"Invalid path part type in source() function. Expected string. Got {type(path0)}: {path0!r}",
+                    getattr(path0, "location", location)
+                )
+
+        _parts = []
         for part in path:
-            if not isinstance(part, StringValue):
+            if isinstance(part, PathElement):
+                _parts += part.parts
+
+            elif isinstance(part, StringValue):
+                _parts.append(part)
+            else:
                 raise PythonScriptError(
                     f"Invalid path part type in source() function. Expected string. Got {type(part)}: {part!r}",
                     getattr(part, "location", location)
                 )
 
         _path = resolve_path_parts_workspace(
-            self.ctx, self.workspace, path, self.directory, location
+            self.ctx, self.workspace, _parts, self.directory, location
         )
 
         # XXX: all of _path.parts is used, so it's fully absolute
         return PathElement(*path, resolved=_path, location=location)
 
     def _function_Path(self, *path: StringValue, location=None):
         for part in path:
@@ -1961,16 +2165,31 @@
             # TODO: handle resolving workspace paths here
             _path = resolve_path_parts_workspace(
                 self.ctx, self.workspace, path, self.directory, location
             )
 
         return PathElement(*path, resolved=_path, location=location)
 
-    def _function_archive(self, path: PathLikeTypes = None, *, prefix=None, location=None):
-        return ArchiveCommand(path, prefix=prefix, location=location)
+    def _function_archive(self, **kwargs):
+        location = kwargs.pop(FILE_LOCATION_ARGUMENT_NAME, None)
+        path = kwargs.pop("path", None)
+        root = kwargs.pop("root", None)
+        type = kwargs.pop("type", None)
+        options = kwargs.pop("options", None)
+        prefix = kwargs.pop("prefix", None)
+        files = kwargs.pop("files", None)
+        return ArchiveCommand(
+            path=path,
+            root=root,
+            type=type,
+            options=options,
+            files=files,
+            prefix=prefix,
+            location=location,
+        )
 
     def _function_shell(self, *script: tuple[StringValue, ...], location=None):
         for part in script:
             if not isinstance(part, StringValue):
                 raise PythonScriptError(
                     f"Invalid script in shell function. Expected string. Got {type(part)}: {part!r}",
                     getattr(part, "location", location)
@@ -2083,67 +2302,54 @@
             elif isinstance(require, TargetReferenceElement):
                 # append references which will be evaluated later
                 yield require
             elif isinstance(require, FindFiles):
                 # append internal objects referring to files such as is find(), glob() and Target(); these will be expanded later
                 if FIND_IN_INPUTS_ENABLED is False:
                     raise PythonScriptError(
-                        "The find function (find()) is not allowed in the target's requires list.",
+                        "The find function (find()) is not allowed in the task's requires list.",
                         require.location
                     )
 
                 yield require
             elif isinstance(require, Glob):
                 # append internal objects referring to files such as is find(), glob() and Target(); these will be expanded later
                 if GLOBS_IN_INPUTS_ENABLED is False:
                     raise PythonScriptError(
-                        "The glob function (glob) is not allowed in the target's requires list.",
+                        "The glob function (glob) is not allowed in the task's requires list.",
                         require.location
                     )
                 yield require
             elif isinstance(require, PathElement):
                 yield require
             elif isinstance(require, TargetObject):
-                raise PythonScriptError("Invalid use of target() for the requires args. ", location)
+                raise PythonScriptError("Invalid use of task() for the requires args. ", location)
             elif isinstance(require, ListTypes):
                 # TODO: wrap lists so we can get a precise location.
                 # TODO: limit list depth.
                 yield from self._target_requires(require, location)
             else:
                 raise PythonScriptError(
                     f"Invalid type {type(require)} in requires list. Got {require!r}.", location
                 )
 
-    class TargetArguments(TypedDict):
-        name: str
-        path: NotRequired[Path]
-        requires: NotRequired[list[str]]
-        runs: NotRequired[list]
-        actions: NotRequired[list]
-        outputs: NotRequired[list]
-        inputs: NotRequired[dict]
-        location: Required[FileLocation]
-        #**kwargs: Unpack[TargetArguments]
-        # NotRequired
-        #
-
     def _function_target(
         self, #*args,
-        **kwargs: Unpack[TargetArguments],
+        **kwargs: TargetArguments, #Unpack[TargetArguments],
     ):
         location = kwargs.get("location", None)
         self.ctx.ui.warn(
             f"The target() function is deprecated. It will be removed by 2024-06. Please change to using task(steps=[]) instead. {location}"
         )
         steps = kwargs.pop("runs", None)
         return self._function_task(steps=steps, **kwargs)
 
     def _function_task(
         self, #*args,
-        **kwargs: Unpack[TargetArguments],
+        **kwargs: TargetArguments, #Unpack[TargetArguments],
     ):
         location = kwargs.pop("location", None)
 
         if False:
             arglen = len(args)
             if not arglen:
                 pass
@@ -2154,42 +2360,42 @@
                 name, path = args
                 return TargetReferenceElement(name, path, location=location)
             elif arglen == 1:
                 name = args[0]
                 return TargetReferenceElement(name, location=location)
             else:
                 raise PythonScriptError(
-                    "Invalid number of arguments to create Target Reference. Expected name and optional path.",
+                    "Invalid number of arguments to create Task Reference. Expected name and optional path.",
                     location=location
                 )
 
         if self.block_registration:
-            trace("Registration of target blocked at %s", location)
+            trace("Registration of task blocked at %s", location)
             return
 
         #trace("Calling target() from %s", self.makex_file)
         name = kwargs.pop("name", None)
         path = kwargs.pop("path", None)
         requires = kwargs.pop("requires", None)
-        runs = kwargs.pop("actions", None) or kwargs.pop("steps", None)
+        steps = kwargs.pop("steps", None)
+        runs = kwargs.pop("actions", None) or steps
         outputs = kwargs.pop("outputs", None)
 
         if kwargs:
             raise PythonScriptError(f"Unknown arguments to task(): {kwargs}", location)
 
         if name is None or name == "":
-            raise PythonScriptError(f"Invalid target name {name!r}.", location)
+            raise PythonScriptError(f"Invalid task name {name!r}.", location)
 
         _validate_target_name(name, getattr(name, "location", location))
 
         existing: TargetObject = self.targets.get(name, None)
         if existing:
             raise PythonScriptError(
-                f"Duplicate target name {name!r}. Already defined at {existing.location}.",
-                location
+                f"Duplicate task name {name!r}. Already defined at {existing.location}.", location
             )
 
         if requires:
             _requires = list(self._target_requires(requires, location))
         else:
             _requires = []
 
@@ -2233,15 +2439,15 @@
             outputs_dict=outputs_dict,
             workspace=self.workspace,
             makex_file=self.makex_file,
             location=location,
         )
 
         self.targets[name] = target
-        trace("Registered target %s in makexfile %s. %s ", target.name, self.makex_file, location)
+        trace("Registered task %s in makexfile %s. %s ", target.name, self.makex_file, location)
         return None
 
 
 class MakexFile:
     # to the makefile
     path: Path
 
@@ -2426,15 +2632,15 @@
             usages = env.environment._usages()
             if usages:
                 makefile.environment_hash = target_hash(
                     "".join(f"{k}={v}" for k, v in sorted(usages.items()))
                 )
 
         debug(
-            "Finished parsing makefile %s: Macros: %s | Targets: %s",
+            "Finished parsing makefile %s: Macros: %s | Tasks: %s",
             path,
             makefile.macros.keys(),
             _globals[TARGETS_MODULE_VARIABLE].keys()
         )
         makefile.targets = _globals[TARGETS_MODULE_VARIABLE]
         return makefile
```

### Comparing `makex-20240401/python/makex/makex_file_parser.py` & `makex-20240601/python/makex/makex_file_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,28 +172,28 @@
                     _path = makex_file_path
                 elif isinstance(path, str):
                     # XXX: this is used for testing only. we should not be dealing with str (instead we should a StringValues)
                     location = FileLocation(None, None, target.location)
                     _path = Path(path)
                 else:
                     raise ExecutionError(
-                        f"Invalid target reference path: Type: {type(path)} {path}",
+                        f"Invalid task reference path: Type: {type(path)} {path}",
                         target,
                         getattr(path, "location", None)
                     )
 
                 if not _path.is_absolute():
                     _path = target_input_path / _path
 
                 if _path.is_dir():
                     # find the makexfile it's referring to
                     file = find_makex_files(_path, ctx.makex_file_names)
                     if file is None:
                         raise ExecutionError(
-                            f"No makex file found at {_path}. Invalid target reference.",
+                            f"No makex file found at {_path}. Invalid task reference.",
                             target,
                             path.location
                         )
                 else:
                     file = _path
 
                 trace("Got reference %r %r", name, file)
@@ -334,16 +334,14 @@
                 for child in self.get_requires_detect_cycles(v):
                     indegree_map[child] -= 1
                     if not indegree_map[child]:
                         new_zero_indegree.append(child)
             zero_indegree = new_zero_indegree
 
 
-
-
 def parse_target_string_reference(
     ctx: Context,
     base,
     string,
     check=True,
 ) -> Optional[ResolvedTargetReference]:
     # resolve the path/makefile?:target_or_build_path name
@@ -480,15 +478,15 @@
                             raise error
                     #trace("Searching path for makex files: %s", search_path)
                     makex_file = find_makex_files(search_path, ctx.makex_file_names)
 
                     trace("Resolved makex file from string %s: %s", path, makex_file)
                     if makex_file is None:
                         error = ExecutionError(
-                            f"No makex files found in path {search_path} {path!r} for the target's requirements."
+                            f"No makex files found in path {search_path} {path!r} for the task's requirements."
                             f" Tried: {ctx.makex_file_names!r} {target}",
                             target,
                             path.location
                         )
                         stop_and_error(error)
                         raise error
                     yield ResolvedTargetReference(target_name, makex_file, path.location)
@@ -517,15 +515,15 @@
                             break
 
                     makex_file = find_makex_files(search_path, ctx.makex_file_names)
 
                     trace("Resolved makex file from pathelement %s: %s", path, makex_file)
                     if makex_file is None:
                         error = ExecutionError(
-                            f"No makex files found in path {search_path} for the target's requirements.",
+                            f"No makex files found in path {search_path} for the task's requirements.",
                             target,
                             path.location
                         )
                         stop_and_error(error)
                         raise error
 
                     yield ResolvedTargetReference(target_name, makex_file, path.location)
@@ -558,22 +556,22 @@
 
         _makefile = makefile.result()
 
         _finished[makefile_path] = _makefile
 
         if _makefile.targets:
             trace(
-                "Adding %d targets from makefile: %s...",
+                "Adding %d tasks from makefile: %s...",
                 len(_makefile.targets),
                 _makefile.targets.keys(), #[:min(3, len(makefile.targets))]
             )
 
             # we're done. add the target references to the parsing input queue
             for target_name, target in _makefile.targets.items():
-                trace("Add target to graph %s %s ", target, target.key())
+                trace("Add task to graph %s %s ", target, target.key())
                 try:
                     graph.add_target(ctx, target)
                 except ExecutionError as e:
                     stop_and_error(e)
                     mark_path_finished(makefile_path)
                     return
 
@@ -619,21 +617,20 @@
 
     def mark_path_finished(makefile_path: Path):
         completed.append(makefile_path)
 
         if makefile_path in executing:
             executing.remove(makefile_path)
 
-
     def search_makex_file(
-            ctx: Context,
-            workspace: Workspace,
-            base: Path,
-            search_path: str,
-            search_parents=True,
+        ctx: Context,
+        workspace: Workspace,
+        base: Path,
+        search_path: str,
+        search_parents=True,
     ):
         if search_path.startswith("//"):
             full_path = workspace.path / search_path[2:]
 
             if not full_path.exists():
                 return None
             return full_path
```

### Comparing `makex-20240401/python/makex/makex_file_parser_test.py` & `makex-20240601/python/makex/makex_file_parser_test.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/makex_file_types.py` & `makex-20240601/python/makex/makex_file_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,21 @@
 
         parts = self.parts + other.parts
         return PathElement(*parts, resolved=resolved, location=other.location)
 
     def __repr__(self):
         return f'PathElement({self._as_path()})'
 
+    def with_suffix(self, suffix, **kwargs):
+        location = kwargs.pop("_location_")
+        _path = self._as_path()
+        _path = _path.with_suffix(suffix)
+        return PathElement(*_path.parts, base=self.base, location=location)
+
+
     def __str__(self):
         if self.resolved:
             return str(self.resolved)
         else:
             raise Exception("Can't use unresolved path here.")
 
 
@@ -381,16 +388,19 @@
     def __init__(self, env: dict[str, str]):
         self.__env = env
         # record usages of environment variables so we can include it as part of the hashing of targets/makex files.
         self.__usages: dict[str, str] = {}
 
     def get(self, key, default=SENTINEL, _location_: FileLocation = None) -> StringValue:
         item = self.__env.get(key, default)
-        if item is None or item is SENTINEL:
+        if item is SENTINEL:
             raise PythonScriptError(f"Environment variable {key} not defined.", _location_)
 
+        if item in {None,False}:
+            return item
+
         self.__usages[key] = item
 
         return StringValue(item, location=_location_)
 
     def _usages(self):
         return self.__usages
```

### Comparing `makex-20240401/python/makex/metadata.py` & `makex-20240601/python/makex/metadata.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/metadata_file.py` & `makex-20240601/python/makex/metadata_file.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/metadata_sqlite.py` & `makex-20240601/python/makex/metadata_sqlite.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/metadata_test.py` & `makex-20240601/python/makex/metadata_test.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/patterns.py` & `makex-20240601/python/makex/patterns.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/patterns_test.py` & `makex-20240601/python/makex/patterns_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from makex.patterns import (
     combine_patterns,
     make_glob_pattern,
 )
 
 
 def test():
@@ -18,7 +20,17 @@
     assert not pattern.match("1hgignore")
     assert pattern.match(".hgignore")
     assert pattern.match(".p4ignore")
     assert not pattern.match("hgignore")
     assert pattern.match("test/test.py")
     assert pattern.match("/test/test.py")
     assert pattern.match("test.py")
+
+
+def test_recursive():
+    pattern = re.compile(make_glob_pattern("**.py"))
+    assert pattern.match("/test/test.py")
+    assert pattern.match("test.py")
+
+    pattern = re.compile(make_glob_pattern("*.py"))
+    assert pattern.match("test.py")
+    assert not pattern.match("/test/test.py")
```

### Comparing `makex-20240401/python/makex/platform_object/platform_object.py` & `makex-20240601/python/makex/platform_object/platform_object.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/protocols.py` & `makex-20240601/python/makex/protocols.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/python_script.py` & `makex-20240601/python/makex/python_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 - Do not split items in this file into separate modules/packages.
 
 """
 import ast
 import logging
 import sys
 import traceback
-import types
 from abc import (
     ABC,
     abstractmethod,
 )
 from collections import deque
 from copy import copy
-from importlib.machinery import ModuleSpec
 from io import StringIO
 from os import PathLike
 from pathlib import Path
 from typing import (
     Any,
     BinaryIO,
+    Callable,
     Optional,
     Protocol,
     Union,
 )
 
 LOGGER = logging.getLogger("python-script")
 STRING_VALUE_NAME = "_STRING_"
@@ -121,15 +120,15 @@
             STRING_VALUE_NAME: StringValue,
             LIST_VALUE_NAME: ListValue,
             GLOBALS_NAME: globals,
             FILE_LOCATION_NAME: FileLocation
         }
 
 
-Globals = dict[str, str]
+Globals = dict[str, Any]
 
 
 class BaseScriptEnvironment(ABC):
     def exit(self):
         # exit the script
         raise StopPythonScript("Script Stopped/Exited by request.")
 
@@ -152,15 +151,14 @@
         c = copy(self)
         c.path = path
         c.wrap = self.wraps
         return c
 
     def pretty(self):
         return pretty_exception(self.wraps, self.location)
-        #return pretty_exception(self, Path(self.location.path), color=color)
 
 
 class StopPythonScript(PythonScriptError):
     pass
 
 
 class PythonScriptFileError(PythonScriptError):
@@ -188,15 +186,15 @@
     def wrapper(*args, **kwargs):
         location = kwargs.pop(FILE_LOCATION_ARGUMENT_NAME)
         return f(*args, **kwargs, location=location)
 
     return wrapper
 
 
-# TODO: Track other primitive types: None/bool/list/dict/int/float
+# TODO: Track other primitive types: None/bool/dict/int/float
 class StringValue(str):
     """
         This is a special type.
 
         We're doing weird things here.
 
         Track string value locations because they are usually a source of problems, and we want to refer to that location
@@ -219,44 +217,39 @@
 
     def __add__(self, other):
         return StringValue(self.value + other.value, getattr(other, "location", self.location))
 
     # TODO: __add__ with a non-string should return an internal JoinedString
 
 
-class DisableImports(ast.NodeVisitor):
-    # TODO: disable imports
-
+class _DisableImports(ast.NodeVisitor):
+    """
+        Disables import statements in the two forms.
+    """
     def __init__(self, path: PathLike):
         self.path = path
 
     def visit_Import(self, node):
-        print(
-            f"""Line {node.lineno} imports modules {
-        ', '.join(alias.name for alias in node.names)
-        }"""
-        )
+        names = ', '.join(alias.name for alias in node.names)
+        print(f"""Line {node.lineno} imports modules {names}""")
         raise PythonScriptError(
             "Invalid syntax (Imports are not allowed):",
             FileLocation.from_ast_node(node, self.path)
         )
 
     def visit_ImportFrom(self, node):
-        print(
-            f"""Line {node.lineno} imports from module {node.module} the names {
-        ', '.join(alias.name for alias in node.names)
-        }"""
-        )
+        names = ', '.join(alias.name for alias in node.names)
+        logging.error(f"""Line {node.lineno} imports from module {node.module} the names {names}""")
         raise PythonScriptError(
             "Invalid syntax (Imports are not allowed):",
             FileLocation.from_ast_node(node, self.path)
         )
 
 
-def _create_file_location_call(path, line, column):
+def create_file_location_call(path, line, column):
     file_location_call = ast.Call(
         func=ast.Name(
             id=FILE_LOCATION_NAME,
             ctx=ast.Load(lineno=line, col_offset=column),
             lineno=line,
             col_offset=column
         ),
@@ -268,14 +261,26 @@
         keywords=[],
         lineno=line,
         col_offset=column,
     )
     return file_location_call
 
 
+def add_location_keyword_argument(node: ast.Call, path, line, column):
+    file_location = create_file_location_call(path, line, column)
+    node.keywords.append(
+        ast.keyword(
+            arg=FILE_LOCATION_ARGUMENT_NAME,
+            value=file_location,
+            lineno=line,
+            col_offset=column,
+        )
+    )
+
+
 class _DisableAssignments(ast.NodeVisitor):
     """
     Disable assignments:
     - to anything non-script (globals)
     - to specified variables.
 
     a,b = item
@@ -344,15 +349,15 @@
 
     def visit_Constant(self, node: ast.Constant) -> Any:
         if isinstance(node.value, str):
             line = node.lineno
             offset = node.col_offset
 
             #logging.debug("Got string cnst %s %s", node.value, node.lineno)
-            file_location = _create_file_location_call(self.path, line, offset)
+            file_location = create_file_location_call(self.path, line, offset)
 
             # TODO: separate the values into JoinedString class so we can evaluate later.
             strcall = ast.Call(
                 func=ast.Name(
                     id=STRING_VALUE_NAME,
                     ctx=ast.Load(),
                     lineno=line,
@@ -375,15 +380,15 @@
             #logging.debug("Got other const %r", node.value)
             return node
 
     def visit_JoinedStr(self, node: ast.JoinedStr) -> Any:
         line = node.lineno
         offset = node.col_offset
 
-        file_location = _create_file_location_call(self.path, line, offset)
+        file_location = create_file_location_call(self.path, line, offset)
 
         # TODO: separate the values into JoinedString class so we can evaluate later.
         strcall = ast.Call(
             func=ast.Name(id=STRING_VALUE_NAME, ctx=ast.Load()),
             args=[node],
             keywords=[
                 ast.keyword(arg='location', value=file_location),
@@ -399,15 +404,15 @@
     # XXX: Deprecated in 3.8 and unused past that version.
     def visit_Str(self, node):
         self.generic_visit(node)
 
         line = node.lineno
         offset = node.col_offset
 
-        file_location = _create_file_location_call(self.path, line, offset)
+        file_location = create_file_location_call(self.path, line, offset)
         strcall = ast.Call(
             func=ast.Name(id=STRING_VALUE_NAME, ctx=ast.Load()),
             args=[ast.Str(node.s)],
             keywords=[
                 ast.keyword(arg='location', value=file_location),
             ],
             lineno=line,
@@ -437,15 +442,14 @@
         func = node.func
 
         if isinstance(func, ast.Attribute):
             attr_name = func.attr
             attr_of = func.value
             if not (isinstance(attr_of, ast.Name) and isinstance(attr_of.ctx, ast.Load)):
                 # could/probably have a str.method e.g. "".join()
-
                 #for child in ast.iter_child_nodes(node):
                 #    self.generic_visit(child)
                 self.generic_visit(node)
                 return node
         elif isinstance(func, ast.Name):
             function_name = func.id
 
@@ -458,15 +462,15 @@
             # user is doing something unexpected.
             # TODO: we should raise a PythonScriptError here.
             self.generic_visit(node)
             return node
         self.generic_visit(node)
 
         #debug(f">Transform fileloction {node.func.id}")
-        file_location = _create_file_location_call(self.path, node.lineno, node.col_offset)
+        file_location = create_file_location_call(self.path, node.lineno, node.col_offset)
         node.keywords = node.keywords or []
         node.keywords.append(ast.keyword(arg=FILE_LOCATION_ARGUMENT_NAME, value=file_location))
 
         ast.fix_missing_locations(node)
         return node
 
 
@@ -498,18 +502,16 @@
     def __getitem__(self, index):
         return self.appended_values[index]
 
     def __radd__(self, other):
         if isinstance(other, list):
             self.appended_values.extendleft(other)
         #elif isinstance(other, GlobValue):
-        #
         #    for i in other:
         #        self.appended_values.insert(0, i)
-        #
         #    self.prepended_values.extend(other._pieces)
         #    self.appended_values.appendleft(other)
         #elif isinstance(other, StringValue):
         #    self.appended_values.appendleft(other)
         elif isinstance(other, ListValue):
             self.appended_values.appendleft(*other.appended_values)
             #self.prepended_values.extend(other.appended_values)
@@ -567,15 +569,15 @@
             func=ast.Name(id=LIST_VALUE_NAME, ctx=ast.Load(), lineno=line, col_offset=offset),
             args=[node],
             keywords=[],
             lineno=line,
             col_offset=offset,
         )
 
-        file_location = _create_file_location_call(self.path, line, offset)
+        file_location = create_file_location_call(self.path, line, offset)
         _node.keywords.append(
             ast.keyword(
                 arg=FILE_LOCATION_ARGUMENT_NAME,
                 value=file_location,
                 lineno=line,
                 col_offset=offset
             )
@@ -587,58 +589,57 @@
         #ast.fix_missing_locations(_node)
         self.generic_visit(node)
         return _node
 
     visit_ListComp = visit_List
 
 
+class Options:
+    pre_visitors: list
+    post_visitors: list
+
+    imports_enabled: bool
+    import_function: Callable
+    disable_assigment_names: set
+
+
 class PythonScriptFile:
     def __init__(
         self,
         path: PathLike,
-        globals: Globals = None,
+        globals: Optional[Globals] = None,
+        # TODO: split these into a options class
         importer=None,
         pre_visitors=None,
         extra_visitors=None,
         enable_imports=False,
     ):
         #self._env = env
         self.path = str(path)
         self.globals = globals or {}
         self.disable_assignment_names = set()
         self.extra_visitors = extra_visitors or []
         self.pre_visitors = pre_visitors or []
         self.enable_imports = enable_imports
         self.importer = importer or self._importer
 
-        # transform attribute calls to have line/column information
-        #self._all_globals = self._env.globals()
-        #self._all_globals.update(self.globals)
-
     def _ast_parse(self, f: BinaryIO):
         # XXX: must be binary due to the way hash_contents works
         buildfile_contents = f.read()
         f.seek(0)
         # transform to ast
         tree = ast.parse(buildfile_contents, filename=self.path, mode='exec')
         return tree
 
     def set_disabled_assignment_names(self, names: set):
         self.disable_assignment_names = names
 
-    #def _get_env_attr(self, name):
-    #    if self._env.has_global(name):
-    #        return self._env.get_global(name)
-
-    #    try:
-    #        return self._all_globals.get(name)
-    #    except ValueError as e:
-    #        raise PythonScriptError(f"{name} not defined in global scope.")
-
     def parse(self, file: Union[BinaryIO]) -> ast.AST:
+        # TODO: use hasattr(file, "read") instead of isinstance
+
         # parse and process the ast.
         # TODO: prefix the modules to execute with the ast to include
         try:
             tree = self._ast_parse(file)
         except SyntaxError as e:
             exc_type, exc_message, exc_traceback = sys.exc_info()
             l = FileLocation(e.lineno, e.offset, self.path)
@@ -649,16 +650,17 @@
         return tree
 
     def _parse(self, tree: ast.AST):
         # set of names to ignore
         ignore = {STRING_VALUE_NAME, FILE_LOCATION_NAME, LIST_VALUE_NAME, GLOBALS_NAME}
 
         # Catch some early errors
+        # TODO: enable this once we have options
         if False:
-            t = DisableImports(self.path)
+            t = _DisableImports(self.path)
             t.visit(tree)
 
         t = _DisableAssignments(self.path, self.disable_assignment_names)
         t.visit(tree)
 
         for visitor in self.pre_visitors:
             visitor.visit(tree)
@@ -679,61 +681,26 @@
 
     def _importer(self, name, globals=None, locals=None, fromlist=(), level=0):
         # level = 1 if relative import. e.g from .module import item
         # TODO: improve this error location
         raise ImportError("Imports are disabled here.")
 
     def execute(self, tree: ast.AST):
+        #print(ast.dump(tree, indent=2))
+
         if not isinstance(tree, ast.AST):
             raise ValueError(f"Expected AST argument. Got {type(tree)}")
-            # TODO: use hasattr(file, "read") instead of isinstance
-            #tree = file
-        #else:
-        #    tree = self.parse(file)
-        from importlib.abc import Loader
-
-        class CustomModule(types.ModuleType):
-            def __init__(self, name):
-                super().__init__(name)
-                self.macros = {}
-
-            def __getattribute__(self, item):
-                if item == "__dict__":
-                    return self.__dict__
-
-                macro = self.macros.get(item, None)
-
-                if macro is None:
-                    raise PythonScriptError(
-                        f"Can't import {item} from {self.name}", FileLocation(0, 0, "//")
-                    )
-                return macro
-
-        class MakexLoader(Loader):
-            def create_module(self, spec: ModuleSpec) -> Union[types.ModuleType, None]:
-                print("CREATING MODULE", spec)
-                module = types.ModuleType(spec.name)
-                #exec(code, module.__dict__)
-
-                return module
-
-            def exec_module(self, module: types.ModuleType) -> None:
-                print("Exec module", module)
-                pass
 
-        #scope = self._env.globals()
-        #scope.update(self.globals)
         scope = self.globals
-        #scope["__getattr__"] = self._get_env_attr
 
+        # TODO: make this line optional, default true
         scope["__builtins__"] = {}
 
         if self.enable_imports:
             scope["__builtins__"] = {"__import__": self.importer}
-        #print(ast.dump(tree, indent=2))
 
         scope[STRING_VALUE_NAME] = StringValue
         scope[FILE_LOCATION_NAME] = FileLocation
         scope[LIST_VALUE_NAME] = ListValue
         scope[GLOBALS_NAME] = globals
 
         try:
```

### Comparing `makex-20240401/python/makex/run.py` & `makex-20240601/python/makex/run.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/target.py` & `makex-20240601/python/makex/target.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/ui.py` & `makex-20240601/python/makex/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import random
 import re
 import sys
 from io import StringIO
 from pathlib import Path
 
-import progressbar
+#import progressbar
 from makex.colors import (
     ColorsNames,
     NoColors,
 )
 from makex.python_script import FileLocation
```

### Comparing `makex-20240401/python/makex/workspace.py` & `makex-20240601/python/makex/workspace.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex/workspace_test.py` & `makex-20240601/python/makex/workspace_test.py`

 * *Files identical despite different names*

### Comparing `makex-20240401/python/makex.egg-info/PKG-INFO` & `makex-20240601/python/makex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: makex
-Version: 20240401
+Version: 20240601
 Summary: Build tool
 Author: Nate Skulic, MetaCompany
 Keywords: build,make,automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: toml>=0.10.2
-Requires-Dist: progressbar2>=4.3.2
+Provides-Extra: use-reflink
+Provides-Extra: use-xattr
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: shtab; extra == "build"
 Requires-Dist: pex; extra == "build"
 Requires-Dist: nuitka; extra == "build"
 Requires-Dist: pytest; extra == "build"
 Requires-Dist: shtab; extra == "build"
@@ -28,14 +29,16 @@
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
 Provides-Extra: documents
 Requires-Dist: sphinx; extra == "documents"
 Requires-Dist: sphinx-better-theme; extra == "documents"
 Requires-Dist: sphinx-notfound-page; extra == "documents"
 Requires-Dist: myst-parser; extra == "documents"
 Requires-Dist: markdown-it-py[linkify,plugins]; extra == "documents"
+Provides-Extra: typechecking
+Requires-Dist: typing_extensions; extra == "typechecking"
 
 # makex
 
 <!-- heading -->
 
 Makex is a new and simplified build and automation tool, similar to the original [Make](https://en.wikipedia.org/wiki/Make_(software)).
 
@@ -48,30 +51,30 @@
 
 - Compiling software/applications/firmware
 - Building filesystems/trees/file archives
 - Building and deploying websites and web applications
 - Running things in a repeatable manner
 - Replacing most or all of the other build systems
 
-## Features
+## Features 🍩
 
 - Familiar Syntax
 - File Hashing and Checksums
 - Dependency Graphs
 - Caching
 - Workspaces
 - Copy on Write
 
 <!-- links -->
 
-## Links
+## Links 🔗
 
 - [Documentation](https://meta.company/go/makex)
-- [Installation Instructions](https://meta.company/go/makex/install)
-- [Troubleshooting](https://meta.company/go/makex/trouble)
+- [Installation Instructions](https://documents.meta.company/makex/latest/install)
+- [Troubleshooting](https://documents.meta.company/makex/latest/trouble)
 - Support: [Google Groups](http://groups.google.com/group/makex) or [makex@googlegroups.com](mailto://makex@googlegroups.com)
 
 <!-- quick-start -->
 
 
 ## Quick Start
 
@@ -79,17 +82,15 @@
 
   ```shell
   pip install makex
   ```
 
 2. Define a Makex file (name it `Makexfile`):
 
-  ```python
-  #!makex
-  
+  ```python 
   task(
       name="hello-world",
       steps=[
           write("hello-world.txt", "Hello World!"),
   
           # or, you can use the shell, but it's not recommended:
           # shell(f"echo 'Hello World!' > {path('hello-world')}/hello-world.txt"),
@@ -102,27 +103,30 @@
 
 3. Run makex and the target:
 
   ```shell
   makex run :hello-world
   ```
  
+```{todo}
+Use the path command to show getting an output path.
+```
+
 4. A file at `_output_/hello-world/hello-world.txt` will have the following contents:
 
   ```
   Hello World!
   ```
 
-
 ## Limitations
 
 - Mac support is not tested.
 - Windows is not tested or supported (yet).
 
 ```{note}
 This is an early release of Makex. Things may change. If you have any problems, feel free to contact us. 
 ```
 
-## Pronunciation
+## Pronunciation 🗣
 
-Makex is pronounced "makes", ˈmeɪks, ˈmeɪkˈɛks (or just "make" 🙂).
+Makex is pronounced "makes", ˈmeɪks, ˈmeɪkˈɛks (or just "make" 🙂)
```

### Comparing `makex-20240401/python/makex.egg-info/SOURCES.txt` & `makex-20240601/python/makex.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 python/makex/metadata_test.py
 python/makex/patterns.py
 python/makex/patterns_test.py
 python/makex/protocols.py
 python/makex/python_script.py
 python/makex/run.py
 python/makex/target.py
+python/makex/test_actions.py
 python/makex/ui.py
 python/makex/version.py
 python/makex/workspace.py
 python/makex/workspace_test.py
 python/makex.egg-info/PKG-INFO
 python/makex.egg-info/SOURCES.txt
 python/makex.egg-info/dependency_links.txt
```

