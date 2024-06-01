# Comparing `tmp/gersemi-0.9.3.tar.gz` & `tmp/gersemi-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gersemi-0.9.3.tar", last modified: Wed Oct 18 16:17:20 2023, max compression
+gzip compressed data, was "gersemi-0.9.4.tar", last modified: Sun Dec 17 16:11:21 2023, max compression
```

## Comparing `gersemi-0.9.3.tar` & `gersemi-0.9.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:20.592738 gersemi-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2023-10-18 16:17:04.000000 gersemi-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16657 2023-10-18 16:17:20.592738 gersemi-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2023-10-18 16:17:04.000000 gersemi-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:20.584738 gersemi-0.9.3/gersemi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/ast_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/base_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/base_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10717 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/builtin_commands
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/cmake.lark
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:20.588738 gersemi-0.9.3/gersemi/command_invocation_dumpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/ctest_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24458 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/module_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18273 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/project_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    33017 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/scripting_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/specialized_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/command_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/custom_command_definition_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/formatted_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/keyword_with_pairs_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/parsing_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/result.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/sanity_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/task_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:20.588738 gersemi-0.9.3/gersemi/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/tasks/check_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/tasks/format_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/tasks/forward_to_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/tasks/rewrite_in_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/tasks/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-10-18 16:17:04.000000 gersemi-0.9.3/gersemi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:20.584738 gersemi-0.9.3/gersemi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16657 2023-10-18 16:17:20.000000 gersemi-0.9.3/gersemi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-10-18 16:17:20.000000 gersemi-0.9.3/gersemi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 16:17:20.000000 gersemi-0.9.3/gersemi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-18 16:17:20.000000 gersemi-0.9.3/gersemi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-18 16:17:20.000000 gersemi-0.9.3/gersemi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-18 16:17:20.000000 gersemi-0.9.3/gersemi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 16:17:20.592738 gersemi-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-10-18 16:17:04.000000 gersemi-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 16:17:20.588738 gersemi-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-10-18 16:17:04.000000 gersemi-0.9.3/tests/test_custom_command_dumper_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-10-18 16:17:04.000000 gersemi-0.9.3/tests/test_custom_command_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    29786 2023-10-18 16:17:05.000000 gersemi-0.9.3/tests/test_executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-10-18 16:17:05.000000 gersemi-0.9.3/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-10-18 16:17:05.000000 gersemi-0.9.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-10-18 16:17:05.000000 gersemi-0.9.3/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2023-10-18 16:17:05.000000 gersemi-0.9.3/tests/tests_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:21.094103 gersemi-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2023-12-17 16:11:13.000000 gersemi-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16657 2023-12-17 16:11:21.094103 gersemi-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2023-12-17 16:11:13.000000 gersemi-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:21.086103 gersemi-0.9.4/gersemi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/ast_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/base_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/base_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/builtin_commands
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/cmake.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:21.090103 gersemi-0.9.4/gersemi/command_invocation_dumpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/ctest_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24740 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/module_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18435 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/project_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33167 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/scripting_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/specialized_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/command_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/custom_command_definition_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/formatted_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/keyword_with_pairs_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/parsing_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/sanity_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/task_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:21.094103 gersemi-0.9.4/gersemi/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/tasks/check_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/tasks/format_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/tasks/forward_to_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/tasks/rewrite_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/tasks/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-12-17 16:11:13.000000 gersemi-0.9.4/gersemi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:21.094103 gersemi-0.9.4/gersemi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16657 2023-12-17 16:11:21.000000 gersemi-0.9.4/gersemi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-12-17 16:11:21.000000 gersemi-0.9.4/gersemi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 16:11:21.000000 gersemi-0.9.4/gersemi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-17 16:11:21.000000 gersemi-0.9.4/gersemi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-17 16:11:21.000000 gersemi-0.9.4/gersemi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-17 16:11:21.000000 gersemi-0.9.4/gersemi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 16:11:21.094103 gersemi-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-12-17 16:11:13.000000 gersemi-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 16:11:21.094103 gersemi-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-17 16:11:13.000000 gersemi-0.9.4/tests/test_custom_command_dumper_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-12-17 16:11:13.000000 gersemi-0.9.4/tests/test_custom_command_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29786 2023-12-17 16:11:13.000000 gersemi-0.9.4/tests/test_executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-12-17 16:11:13.000000 gersemi-0.9.4/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-12-17 16:11:13.000000 gersemi-0.9.4/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-17 16:11:13.000000 gersemi-0.9.4/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2023-12-17 16:11:13.000000 gersemi-0.9.4/tests/tests_generator.py
```

### Comparing `gersemi-0.9.3/LICENSE` & `gersemi-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/PKG-INFO` & `gersemi-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gersemi
-Version: 0.9.3
+Version: 0.9.4
 Summary: A formatter to make your CMake code the real treasure
 Home-page: https://github.com/BlankSpruce/gersemi
 Author: Blank Spruce
 Author-email: blankspruce@protonmail.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -93,15 +93,15 @@
 
 ### [pre-commit](https://pre-commit.com/) hook
 
 You can use gersemi with a pre-commit hook by adding the following to `.pre-commit-config.yaml` of your repository:
 ```yaml
 repos:
 - repo: https://github.com/BlankSpruce/gersemi
-  rev: 0.9.3
+  rev: 0.9.4
   hooks:
   - id: gersemi
 ```
 
 Update `rev` to relevant version used in your repository. For more details refer to https://pre-commit.com/#using-the-latest-version-for-a-repository
 
 ## Formatting
```

### Comparing `gersemi-0.9.3/README.md` & `gersemi-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 ### [pre-commit](https://pre-commit.com/) hook
 
 You can use gersemi with a pre-commit hook by adding the following to `.pre-commit-config.yaml` of your repository:
 ```yaml
 repos:
 - repo: https://github.com/BlankSpruce/gersemi
-  rev: 0.9.3
+  rev: 0.9.4
   hooks:
   - id: gersemi
 ```
 
 Update `rev` to relevant version used in your repository. For more details refer to https://pre-commit.com/#using-the-latest-version-for-a-repository
 
 ## Formatting
```

### Comparing `gersemi-0.9.3/gersemi/__main__.py` & `gersemi-0.9.4/gersemi/__main__.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/ast_helpers.py` & `gersemi-0.9.4/gersemi/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/base_command_invocation_dumper.py` & `gersemi-0.9.4/gersemi/base_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/base_dumper.py` & `gersemi-0.9.4/gersemi/base_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/builtin_commands` & `gersemi-0.9.4/gersemi/builtin_commands`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/cache.py` & `gersemi-0.9.4/gersemi/cache.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/cmake.lark` & `gersemi-0.9.4/gersemi/cmake.lark`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumper.py` & `gersemi-0.9.4/gersemi/command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/ctest_command_dumpers.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/ctest_command_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/module_command_dumpers.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/module_command_dumpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,15 @@
         "CMAKE_GENERATOR_TOOLSET",
         "CMAKE_GENERATOR_INSTANCE",
         "SOURCE_SUBDIR",
         "CONFIGURE_HANDLED_BY_BUILD",
         # Build Step
         "BUILD_IN_SOURCE",
         "BUILD_ALWAYS",
+        "BUILD_JOB_SERVER_AWARE",
         # Install Step
         # Test Step
         "TEST_BEFORE_INSTALL",
         "TEST_AFTER_INSTALL",
         "TEST_EXCLUDE_FROM_MAIN",
         # Output Logging
         "LOG_DOWNLOAD",
@@ -371,15 +372,15 @@
 
 
 class SetPackageProperties(ArgumentAwareCommandInvocationDumper):
     one_value_keywords = ["URL", "DESCRIPTION", "TYPE", "PURPOSE"]
 
 
 class FetchContentDeclare(CommandLineFormatter, ArgumentAwareCommandInvocationDumper):
-    options = ["SYSTEM", "OVERRIDE_FIND_PACKAGE"]
+    options = ["SYSTEM", "OVERRIDE_FIND_PACKAGE", "EXCLUDE_FROM_ALL"]
     one_value_keywords = [
         # Download Step
         "URL_HASH",
         "URL_MD5",
         "DOWNLOAD_NAME",
         "DOWNLOAD_NO_EXTRACT",
         "TIMEOUT",
@@ -718,14 +719,19 @@
         "NO_CMAKE_ENVIRONMENT_PATH",
         "IMPORTED_TARGET",
         "GLOBAL",
         "STATIC_TARGET",
     ]
 
 
+class PkgGetVariable(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<resultVar>", "<moduleName>", "<varName>"]
+    multi_value_keywords = ["DEFINE_VARIABLES"]
+
+
 class PkgSearchModule(ArgumentAwareCommandInvocationDumper):
     options = [
         "REQUIRED",
         "QUIET",
         "NO_CMAKE_PATH",
         "NO_CMAKE_ENVIRONMENT_PATH",
         "IMPORTED_TARGET",
@@ -840,14 +846,15 @@
     "flex_target": FlexTarget,
     "gettext_create_translations": GettextCreateTranslations,
     "gettext_process_pot_file": GettextProcessPotFile,
     "gettext_process_po_files": GettextProcessPoFiles,
     "matlab_add_unit_test": MatlabAddUnitTest,
     "matlab_add_mex": MatlabAddMex,
     "pkg_check_modules": PkgCheckModules,
+    "pkg_get_variable": PkgGetVariable,
     "pkg_search_module": PkgSearchModule,
     "protobuf_generate_cpp": ProtobufGenerateCpp,
     "qt4_wrap_cpp": Qt4WrapCpp,
     "qt4_wrap_ui": Qt4WrapUi,
     "qt4_add_resources": Qt4AddResources,
     "qt4_generate_moc": Qt4GenerateMoc,
     "qt4_generate_dbus_interface": Qt4GenerateDbusInterface,
```

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/project_command_dumpers.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/project_command_dumpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             ],
             one_value_keywords=[
                 "MAIN_DEPENDENCY",
                 "WORKING_DIRECTORY",
                 "COMMENT",
                 "DEPFILE",
                 "JOB_POOL",
+                "JOB_SERVER_AWARE",
             ],
             multi_value_keywords=[
                 "OUTPUT",
                 "COMMAND",
                 "ARGS",
                 "DEPENDS",
                 "BYPRODUCTS",
@@ -56,15 +57,20 @@
         "ARGS": "_format_command_line",
     }
 
 
 class AddCustomTarget(CommandLineFormatter, ArgumentAwareCommandInvocationDumper):
     front_positional_arguments = ["Name", "ALL"]
     options = ["VERBATIM", "USES_TERMINAL", "COMMAND_EXPAND_LISTS"]
-    one_value_keywords = ["WORKING_DIRECTORY", "COMMENT", "JOB_POOL"]
+    one_value_keywords = [
+        "WORKING_DIRECTORY",
+        "COMMENT",
+        "JOB_POOL",
+        "JOB_SERVER_AWARE",
+    ]
     multi_value_keywords = ["COMMAND", "DEPENDS", "BYPRODUCTS", "SOURCES"]
     keyword_formatters = {"COMMAND": "_format_command_line"}
 
     def _format_positional_arguments_group(self, group):
         if len(group) > 1:
             if group[0].children[0] == "ALL":
                 first, *rest = group
@@ -177,15 +183,16 @@
 
 
 class GetTargetProperty(ArgumentAwareCommandInvocationDumper):
     front_positional_arguments = ["<VAR>", "target", "property"]
 
 
 class GetTestProperty(ArgumentAwareCommandInvocationDumper):
-    front_positional_arguments = ["<VAR>", "target", "property"]
+    front_positional_arguments = ["test", "property"]
+    one_value_keywords = ["DIRECTORY"]
 
 
 class IncludeDirectories(ArgumentAwareCommandInvocationDumper):
     options = ["AFTER", "BEFORE", "SYSTEM"]
 
 
 class IncludeExternalMsProject(ArgumentAwareCommandInvocationDumper):
@@ -509,14 +516,15 @@
     multi_value_keywords = ["PROPERTIES"]
     keyword_formatters = {"PROPERTIES": "_format_keyword_with_pairs"}
 
 
 class SetTestsProperties(
     KeywordWithPairsFormatter, ArgumentAwareCommandInvocationDumper
 ):
+    one_value_keywords = ["DIRECTORY"]
     multi_value_keywords = ["PROPERTIES"]
     keyword_formatters = {"PROPERTIES": "_format_keyword_with_pairs"}
 
 
 project_command_mapping = {
     "add_custom_command": AddCustomCommand,
     "add_custom_target": AddCustomTarget,
```

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/scripting_command_dumpers.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/scripting_command_dumpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -633,16 +633,24 @@
     ]
     one_value_keywords = ["BASE_DIR", "PROGRAM_ARGS"]
 
 
 class GetProperty(ArgumentAwareCommandInvocationDumper):
     front_positional_arguments = ["<variable>"]
     options = ["GLOBAL", "VARIABLE", "SET", "DEFINED", "BRIEF_DOCS", "FULL_DOCS"]
-    one_value_keywords = ["TARGET", "INSTALL", "TEST", "CACHE", "PROPERTY"]
-    multi_value_keywords = ["DIRECTORY", "SOURCE"]
+    one_value_keywords = [
+        "TARGET",
+        "INSTALL",
+        "TEST",
+        "CACHE",
+        "PROPERTY",
+        "TARGET_DIRECTORY",
+        "SOURCE",
+    ]
+    multi_value_keywords = ["DIRECTORY"]
 
 
 class GetSourceFileProperty(ArgumentAwareCommandInvocationDumper):
     one_value_keywords = ["DIRECTORY", "TARGET_DIRECTORY"]
 
 
 class Include(ArgumentAwareCommandInvocationDumper):
@@ -749,16 +757,24 @@
 class SeparateArguments(ArgumentAwareCommandInvocationDumper):
     front_positional_arguments = ["<variable>", "<mode>"]
     options = ["PROGRAM", "SEPARATE_ARGS"]
 
 
 class SetProperty(ArgumentAwareCommandInvocationDumper):
     options = ["GLOBAL", "APPEND", "APPEND_STRING"]
-    one_value_keywords = ["DIRECTORY"]
-    multi_value_keywords = ["TARGET", "SOURCE", "INSTALL", "TEST", "CACHE", "PROPERTY"]
+    multi_value_keywords = [
+        "TARGET",
+        "SOURCE",
+        "INSTALL",
+        "TEST",
+        "CACHE",
+        "PROPERTY",
+        "TARGET_DIRECTORIES",
+        "DIRECTORY",
+    ]
     keyword_formatters = {"PROPERTY": "_format_property"}
 
     def _format_property(self, args):
         result = self._try_to_format_into_single_line(
             args, separator=" ", prefix="(", postfix=")"
         )
         if result is not None:
```

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/specialized_dumpers.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/specialized_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py` & `gersemi-0.9.4/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/command_line_formatter.py` & `gersemi-0.9.4/gersemi/command_line_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/configuration.py` & `gersemi-0.9.4/gersemi/configuration.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/custom_command_definition_finder.py` & `gersemi-0.9.4/gersemi/custom_command_definition_finder.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/dumper.py` & `gersemi-0.9.4/gersemi/dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/exceptions.py` & `gersemi-0.9.4/gersemi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/formatter.py` & `gersemi-0.9.4/gersemi/formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/keyword_with_pairs_formatter.py` & `gersemi-0.9.4/gersemi/keyword_with_pairs_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/parser.py` & `gersemi-0.9.4/gersemi/parser.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/parsing_transformer.py` & `gersemi-0.9.4/gersemi/parsing_transformer.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/postprocessor.py` & `gersemi-0.9.4/gersemi/postprocessor.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/result.py` & `gersemi-0.9.4/gersemi/result.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/runner.py` & `gersemi-0.9.4/gersemi/runner.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/sanity_checker.py` & `gersemi-0.9.4/gersemi/sanity_checker.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/tasks/check_formatting.py` & `gersemi-0.9.4/gersemi/tasks/check_formatting.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/tasks/format_file.py` & `gersemi-0.9.4/gersemi/tasks/format_file.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/tasks/rewrite_in_place.py` & `gersemi-0.9.4/gersemi/tasks/rewrite_in_place.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/tasks/show_diff.py` & `gersemi-0.9.4/gersemi/tasks/show_diff.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi/utils.py` & `gersemi-0.9.4/gersemi/utils.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/gersemi.egg-info/PKG-INFO` & `gersemi-0.9.4/gersemi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gersemi
-Version: 0.9.3
+Version: 0.9.4
 Summary: A formatter to make your CMake code the real treasure
 Home-page: https://github.com/BlankSpruce/gersemi
 Author: Blank Spruce
 Author-email: blankspruce@protonmail.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -93,15 +93,15 @@
 
 ### [pre-commit](https://pre-commit.com/) hook
 
 You can use gersemi with a pre-commit hook by adding the following to `.pre-commit-config.yaml` of your repository:
 ```yaml
 repos:
 - repo: https://github.com/BlankSpruce/gersemi
-  rev: 0.9.3
+  rev: 0.9.4
   hooks:
   - id: gersemi
 ```
 
 Update `rev` to relevant version used in your repository. For more details refer to https://pre-commit.com/#using-the-latest-version-for-a-repository
 
 ## Formatting
```

### Comparing `gersemi-0.9.3/gersemi.egg-info/SOURCES.txt` & `gersemi-0.9.4/gersemi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/setup.py` & `gersemi-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/tests/test_custom_command_dumper_generation.py` & `gersemi-0.9.4/tests/test_custom_command_dumper_generation.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/tests/test_custom_command_formatting.py` & `gersemi-0.9.4/tests/test_custom_command_formatting.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/tests/test_executable.py` & `gersemi-0.9.4/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/tests/test_formatter.py` & `gersemi-0.9.4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/tests/test_parser.py` & `gersemi-0.9.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.3/tests/tests_generator.py` & `gersemi-0.9.4/tests/tests_generator.py`

 * *Files identical despite different names*

