# Comparing `tmp/statelint-0.2.0.tar.gz` & `tmp/statelint-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statelint-0.2.0.tar", last modified: Sat May 27 00:27:37 2023, max compression
+gzip compressed data, was "statelint-1.0.0.tar", last modified: Sat Jun  1 03:14:40 2024, max compression
```

## Comparing `statelint-0.2.0.tar` & `statelint-1.0.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.045829 statelint-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 00:27:25.000000 statelint-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-27 00:27:37.045829 statelint-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-27 00:27:25.000000 statelint-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-27 00:27:37.045829 statelint-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 00:27:25.000000 statelint-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.037829 statelint-0.2.0/statelint/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.037829 statelint-0.2.0/statelint/fields/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/any_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/bool_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/list_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/num_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/object_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/pattern_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/str_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/fields/timestamp_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/linter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/choice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/container_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/nodes/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/factory/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/fail_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/map_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/nodes/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/catcher_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/choices_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/payload_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/result_path_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/mixins/retrier_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/parallel_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/pass_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/succeed_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/task_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/unknown_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/nodes/wait_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/problem/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/problem/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/problem/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/problem/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.041829 statelint-0.2.0/statelint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-27 00:27:25.000000 statelint-0.2.0/statelint/utils/re_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.037829 statelint-0.2.0/statelint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 00:27:37.000000 statelint-0.2.0/statelint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:27:37.045829 statelint-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_catcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_choice_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_choice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_linter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_map_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_parallel_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_pass_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_ref_pattern_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_retrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_task_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_terminal_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-27 00:27:25.000000 statelint-0.2.0/tests/test_wait_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.729137 statelint-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 03:14:29.000000 statelint-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-06-01 03:14:40.729137 statelint-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-06-01 03:14:29.000000 statelint-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-06-01 03:14:40.729137 statelint-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:14:29.000000 statelint-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.717137 statelint-1.0.0/statelint/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.721137 statelint-1.0.0/statelint/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/any_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/bool_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/list_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/num_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/object_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/pattern_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/str_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/fields/timestamp_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/linter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.721137 statelint-1.0.0/statelint/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/choice_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/container_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.721137 statelint-1.0.0/statelint/nodes/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/factory/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/fail_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/map_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.721137 statelint-1.0.0/statelint/nodes/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/mixins/catcher_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/mixins/choices_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/mixins/payload_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/mixins/result_path_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/mixins/retrier_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/parallel_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/pass_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/succeed_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/unknown_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/nodes/wait_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.725137 statelint-1.0.0/statelint/problem/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/problem/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/problem/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/problem/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.725137 statelint-1.0.0/statelint/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-06-01 03:14:29.000000 statelint-1.0.0/statelint/utils/re_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.725137 statelint-1.0.0/statelint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-06-01 03:14:40.000000 statelint-1.0.0/statelint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-06-01 03:14:40.000000 statelint-1.0.0/statelint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:14:40.000000 statelint-1.0.0/statelint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 03:14:40.000000 statelint-1.0.0/statelint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 03:14:40.000000 statelint-1.0.0/statelint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 03:14:40.000000 statelint-1.0.0/statelint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:14:40.725137 statelint-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_catcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_choice_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_choice_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_fail_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_map_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_parallel_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_pass_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_ref_pattern_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_retrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_terminal_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-06-01 03:14:29.000000 statelint-1.0.0/tests/test_wait_state.py
```

### Comparing `statelint-0.2.0/LICENSE` & `statelint-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/PKG-INFO` & `statelint-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: statelint
-Version: 0.2.0
+Version: 1.0.0
 Summary: command-line validator for Amazon States Language
 Home-page: https://github.com/taro-kayo/statelint
 Author: taro-kayo
 License: Apache License 2.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Provides-Extra: yaml
 License-File: LICENSE
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: regex>=2023.5.5
+Provides-Extra: yaml
+Requires-Dist: PyYAML>=6.0; extra == "yaml"
 
 # statelint
 <a href="https://github.com/taro-kayo/statelint/actions"><img alt="Actions Status" src="https://github.com/taro-kayo/statelint/workflows/Test/badge.svg"></a>
 <a href="https://coveralls.io/github/taro-kayo/statelint?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/taro-kayo/statelint/badge.svg?branch=main"></a>
 <a href="https://github.com/taro-kayo/statelint/blob/main/LICENSE"><img alt="License: Apache License 2.0" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg"></a>
 <a href="https://pypi.org/project/statelint/"><img alt="PyPI" src="https://img.shields.io/pypi/v/statelint"></a>
-<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+[![Downloads](https://static.pepy.tech/badge/statelint/month)](https://pepy.tech/project/statelint)
 
 A PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
 
 This package is based on Amazon Web Services Labs' [awslabs/statelint](https://github.com/awslabs/statelint).
 
 ## Installation
 
@@ -70,13 +74,7 @@
 ```
 
 You can pass both parameters at the same time.
 
 ```shell
 statelint --ignore=FLOAT,URI fancy-state-machine-spec.json
 ```
-
-## TODO
-
-- [reference path with dash doesn't validate](https://github.com/awslabs/statelint/issues/17)
-- [Reference Path with unicode doesn't validate](https://github.com/awslabs/statelint/issues/23)
-- [Does not catch Duplicated State names](https://github.com/awslabs/statelint/issues/39)
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: statelint Version: 0.2.0 Summary: command-line
+Metadata-Version: 2.1 Name: statelint Version: 1.0.0 Summary: command-line
 validator for Amazon States Language Home-page: https://github.com/taro-kayo/
 statelint Author: taro-kayo License: Apache License 2.0 Classifier: Development
-Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
-Audience :: Developers Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.8.0 Description-Content-Type: text/markdown Provides-Extra: yaml
-License-File: LICENSE # statelint _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:
-_A_p_a_c_h_e_ _L_i_c_e_n_s_e_ _2_._0_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]A PyPI package providing a
-validator for [Amazon States Language](https://states-language.net/spec.html)
-JSON/YAML files. This package is based on Amazon Web Services Labs' [awslabs/
-statelint](https://github.com/awslabs/statelint). ## Installation ```shell pip
-install statelint ``` ## Usage ```shell statelint fancy-state-machine-spec.json
-``` If you prefer YAML, you need to install [PyYaml](https://pypi.org/project/
-PyYAML/). ```shell pip install PyYAML ``` Then, run command with a `--yaml`
-parameter. ```shell statelint --yaml fancy-state-machine-spec.yaml ``` If you
-don't like to be complained that `BackoffRate` doesn't end with ".0", pass a `-
--ignore=FLOAT` parameter. ```shell statelint --ignore=FLOAT fancy-state-
-machine-spec.json ``` If your `Resource` doesn't contain URI string, pass a `--
-ignore=URI` parameter. ```shell statelint --ignore=URI fancy-state-machine-
-spec.json ``` You can pass both parameters at the same time. ```shell statelint
---ignore=FLOAT,URI fancy-state-machine-spec.json ``` ## TODO - [reference path
-with dash doesn't validate](https://github.com/awslabs/statelint/issues/17) -
-[Reference Path with unicode doesn't validate](https://github.com/awslabs/
-statelint/issues/23) - [Does not catch Duplicated State names](https://
-github.com/awslabs/statelint/issues/39)
+Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+python-dateutil>=2.8.2 Requires-Dist: regex>=2023.5.5 Provides-Extra: yaml
+Requires-Dist: PyYAML>=6.0; extra == "yaml" # statelint _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]
+_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _L_i_c_e_n_s_e_ _2_._0_]_[_P_y_P_I_][![Downloads](https://
+static.pepy.tech/badge/statelint/month)](https://pepy.tech/project/statelint) A
+PyPI package providing a validator for [Amazon States Language](https://states-
+language.net/spec.html) JSON/YAML files. This package is based on Amazon Web
+Services Labs' [awslabs/statelint](https://github.com/awslabs/statelint). ##
+Installation ```shell pip install statelint ``` ## Usage ```shell statelint
+fancy-state-machine-spec.json ``` If you prefer YAML, you need to install
+[PyYaml](https://pypi.org/project/PyYAML/). ```shell pip install PyYAML ```
+Then, run command with a `--yaml` parameter. ```shell statelint --yaml fancy-
+state-machine-spec.yaml ``` If you don't like to be complained that
+`BackoffRate` doesn't end with ".0", pass a `--ignore=FLOAT` parameter.
+```shell statelint --ignore=FLOAT fancy-state-machine-spec.json ``` If your
+`Resource` doesn't contain URI string, pass a `--ignore=URI` parameter.
+```shell statelint --ignore=URI fancy-state-machine-spec.json ``` You can pass
+both parameters at the same time. ```shell statelint --ignore=FLOAT,URI fancy-
+state-machine-spec.json ```
```

### Comparing `statelint-0.2.0/README.md` & `statelint-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # statelint
 <a href="https://github.com/taro-kayo/statelint/actions"><img alt="Actions Status" src="https://github.com/taro-kayo/statelint/workflows/Test/badge.svg"></a>
 <a href="https://coveralls.io/github/taro-kayo/statelint?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/taro-kayo/statelint/badge.svg?branch=main"></a>
 <a href="https://github.com/taro-kayo/statelint/blob/main/LICENSE"><img alt="License: Apache License 2.0" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg"></a>
 <a href="https://pypi.org/project/statelint/"><img alt="PyPI" src="https://img.shields.io/pypi/v/statelint"></a>
-<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+[![Downloads](https://static.pepy.tech/badge/statelint/month)](https://pepy.tech/project/statelint)
 
 A PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
 
 This package is based on Amazon Web Services Labs' [awslabs/statelint](https://github.com/awslabs/statelint).
 
 ## Installation
 
@@ -48,13 +48,7 @@
 ```
 
 You can pass both parameters at the same time.
 
 ```shell
 statelint --ignore=FLOAT,URI fancy-state-machine-spec.json
 ```
-
-## TODO
-
-- [reference path with dash doesn't validate](https://github.com/awslabs/statelint/issues/17)
-- [Reference Path with unicode doesn't validate](https://github.com/awslabs/statelint/issues/23)
-- [Does not catch Duplicated State names](https://github.com/awslabs/statelint/issues/39)
```

#### html2text {}

```diff
@@ -1,19 +1,16 @@
 # statelint _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _L_i_c_e_n_s_e_ _2_._0_]
-_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]A PyPI package providing a validator for [Amazon
+_[_P_y_P_I_][![Downloads](https://static.pepy.tech/badge/statelint/month)](https://
+pepy.tech/project/statelint) A PyPI package providing a validator for [Amazon
 States Language](https://states-language.net/spec.html) JSON/YAML files. This
 package is based on Amazon Web Services Labs' [awslabs/statelint](https://
 github.com/awslabs/statelint). ## Installation ```shell pip install statelint
 ``` ## Usage ```shell statelint fancy-state-machine-spec.json ``` If you prefer
 YAML, you need to install [PyYaml](https://pypi.org/project/PyYAML/). ```shell
 pip install PyYAML ``` Then, run command with a `--yaml` parameter. ```shell
 statelint --yaml fancy-state-machine-spec.yaml ``` If you don't like to be
 complained that `BackoffRate` doesn't end with ".0", pass a `--ignore=FLOAT`
 parameter. ```shell statelint --ignore=FLOAT fancy-state-machine-spec.json ```
 If your `Resource` doesn't contain URI string, pass a `--ignore=URI` parameter.
 ```shell statelint --ignore=URI fancy-state-machine-spec.json ``` You can pass
 both parameters at the same time. ```shell statelint --ignore=FLOAT,URI fancy-
-state-machine-spec.json ``` ## TODO - [reference path with dash doesn't
-validate](https://github.com/awslabs/statelint/issues/17) - [Reference Path
-with unicode doesn't validate](https://github.com/awslabs/statelint/issues/23)
-- [Does not catch Duplicated State names](https://github.com/awslabs/statelint/
-issues/39)
+state-machine-spec.json ```
```

### Comparing `statelint-0.2.0/setup.cfg` & `statelint-1.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taro-kayo/statelint
 author = taro-kayo
 license = Apache License 2.0
 license_file = LICENSE
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 packages = find:
 install_requires = 
 	python-dateutil>=2.8.2
 	regex>=2023.5.5
 python_requires = >=3.8.0
```

### Comparing `statelint-0.2.0/statelint/cli.py` & `statelint-1.0.0/statelint/cli.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/fields/__init__.py` & `statelint-1.0.0/statelint/fields/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .num_field import FloatField as _FloatField
 from .num_field import IntegerField as _IntegerField
 from .num_field import NumericField as _NumericField
 from .object_field import ObjectField as _ObjectField
 from .pattern_field import JsonPathField as _JsonPathField
 from .pattern_field import NullableRefPathField as _NullableRefPathField
 from .pattern_field import RefPathField as _RefPathField
+from .pattern_field import RefPathOrFuncField as _RefPathOrFuncField
 from .pattern_field import UriField as _UriField
 from .str_field import EnumStrField as _EnumStrField
 from .str_field import NullableStrField as _NullableStrField
 from .str_field import StrField as _StrField
 from .timestamp_field import TimestampField as _TimestampField
 
 VERSION = _StrField("Version")
@@ -24,15 +25,17 @@
 
 SECONDS = _IntegerField("Seconds", 0, inclusive=False)
 SECONDS_PATH = _RefPathField("SecondsPath")
 TIMESTAMP = _TimestampField("Timestamp")
 TIMESTAMP_PATH = _RefPathField("TimestampPath")
 
 CAUSE = _StrField("Cause")
+CAUSE_PATH = _RefPathOrFuncField("CausePath")
 ERROR = _StrField("Error")
+ERROR_PATH = _RefPathOrFuncField("ErrorPath")
 
 RESULT = _AnyField("Result")
 RESULT_SELECTOR = _AnyField("ResultSelector")
 RESULT_PATH = _NullableRefPathField("ResultPath")
 PARAMETERS = _AnyField("Parameters")
 
 NEXT = _StrField("Next")
@@ -41,28 +44,31 @@
 STATES = _ObjectField("States")
 START_AT = _StrField("StartAt")
 
 TIMEOUT_SECONDS = _IntegerField("TimeoutSeconds", 0, 99999999)
 HEARTBEAT_SECONDS = _IntegerField("HeartbeatSeconds", 0, 99999999)
 TIMEOUT_SECONDS_PATH = _RefPathField("TimeoutSecondsPath")
 HEARTBEAT_SECONDS_PATH = _RefPathField("HeartbeatSecondsPath")
+CREDENTIALS = _ObjectField("Credentials")
 
 TYPE = _EnumStrField("Type", [t.value for t in StateType])
 
 INPUT_PATH = _NullableStrField("InputPath")
 OUTPUT_PATH = _NullableStrField("OutputPath")
 
 RESOURCE = _UriField("Resource")
 
 CATCH = _ListField("Catch", _ObjectField)
 RETRY = _ListField("Retry", _ObjectField)
 ERROR_EQUALS = _NonEmptyListField("ErrorEquals", _StrField)
 INTERVAL_SECONDS = _IntegerField("IntervalSeconds", 0)
 MAX_ATTEMPTS = _IntegerField("MaxAttempts", -1, 99999999)
 BACKOFF_RATE = _FloatField("BackoffRate", 1, inclusive=False)
+MAX_DELAY_SECONDS = _IntegerField("MaxDelaySeconds", 0)
+JITTER_STRATEGY = _EnumStrField("JitterStrategy", ["FULL", "NONE"])
 
 
 CHOICES = _NonEmptyListField("Choices", _ObjectField)
 DEFAULT = _StrField("Default")
 
 AND = _NonEmptyListField("And", _ObjectField)
 OR = _NonEmptyListField("Or", _ObjectField)
@@ -110,8 +116,30 @@
 IS_TIMESTAMP = _BoolField("IsTimestamp")
 STRING_MATCHES = _StrField("StringMatches")
 
 BRANCHES = _ListField("Branches", _ObjectField)
 
 ITERATOR = _ObjectField("Iterator")
 ITEMS_PATH = _JsonPathField("ItemsPath")
-MAX_CONCURRENCY = _NumericField("MaxConcurrency")
+MAX_CONCURRENCY = _NumericField("MaxConcurrency", 0, inclusive=False)
+MAX_CONCURRENCY_PATH = _RefPathField("MaxConcurrencyPath")
+
+ITEM_PROCESSOR = _ObjectField("ItemProcessor")
+PROCESSOR_CONFIG = _ObjectField("ProcessorConfig")
+ITEM_SELECTOR = _AnyField("ItemSelector")
+TOLERATED_FAILURE_COUNT = _IntegerField("ToleratedFailureCount", 0, inclusive=False)
+TOLERATED_FAILURE_COUNT_PATH = _RefPathField("ToleratedFailureCountPath")
+ITEM_READER = _ObjectField("ItemReader")
+READER_CONFIG = _ObjectField("ReaderConfig")
+MAX_ITEMS = _IntegerField("MaxItems", 0)
+MAX_ITEMS_PATH = _RefPathField("MaxItemsPath")
+RESULT_WRITER = _ObjectField("ResultWriter")
+ITEM_BATCHER = _ObjectField("ItemBatcher")
+BATCH_INPUT = _AnyField("BatchInput")
+MAX_ITEMS_PER_BATCH = _IntegerField("MaxItemsPerBatch", 0)
+MAX_ITEMS_PER_BATCH_PATH = _RefPathField("MaxItemsPerBatchPath")
+MAX_INPUT_BYTES_PER_BATCH = _IntegerField("MaxInputBytesPerBatch", 0)
+MAX_INPUT_BYTES_PER_BATCH_PATH = _RefPathField("MaxInputBytesPerBatchPath")
+TOLERATED_FAILURE_PERCENTAGE = _IntegerField(
+    "ToleratedFailurePercentage", 0, 100, inclusive=False
+)
+TOLERATED_FAILURE_PERCENTAGE_PATH = _RefPathField("ToleratedFailurePercentagePath")
```

### Comparing `statelint-0.2.0/statelint/fields/base.py` & `statelint-1.0.0/statelint/fields/base.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/fields/common.py` & `statelint-1.0.0/statelint/fields/common.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/fields/container.py` & `statelint-1.0.0/statelint/fields/container.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/fields/list_field.py` & `statelint-1.0.0/statelint/fields/list_field.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/fields/num_field.py` & `statelint-1.0.0/statelint/fields/num_field.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/fields/pattern_field.py` & `statelint-1.0.0/statelint/fields/pattern_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Any, Callable, List
 
 from ..problem import ProblemPredicate, ProblemType
-from ..utils.re_helper import is_path, is_reference_path
+from ..utils.re_helper import is_intrinsic_invocation, is_path, is_reference_path
 from .base import NonNullMixin
 from .str_field import NullableStrField
 
 
 class PatternField(NullableStrField, ABC):
     def __init__(self, name: str, is_match: Callable[[str], bool]) -> None:
         super().__init__(name)
@@ -50,14 +50,29 @@
         return ProblemType.REFERENCE_PATH
 
 
 class RefPathField(NonNullMixin, NullableRefPathField):
     pass
 
 
+class NullableRefPathOrFuncField(PatternField):
+    def __init__(self, name: str) -> None:
+        super().__init__(
+            name, lambda v: is_reference_path(v) or is_intrinsic_invocation(v)
+        )
+
+    @property
+    def problem_type(self) -> ProblemType:
+        return ProblemType.REFERENCE_PATH_OR_FUNC
+
+
+class RefPathOrFuncField(NonNullMixin, NullableRefPathOrFuncField):
+    pass
+
+
 class JsonPathField(NonNullMixin, PatternField):
     def __init__(self, name: str) -> None:
         super().__init__(name, lambda x: is_path(x, True))
 
     @property
     def problem_type(self) -> ProblemType:
         return ProblemType.JSON_PATH
```

### Comparing `statelint-0.2.0/statelint/fields/str_field.py` & `statelint-1.0.0/statelint/fields/str_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,17 @@
 class EnumStrField(StrField):
     def __init__(self, name: str, choices: List[str]):
         super().__init__(name)
         self.choices = choices
 
     def validate(self, value: Any) -> List[ProblemPredicate]:
         problems = super().validate(value)
-        if problems:
-            return problems
-        if value not in self.choices:
+        str_val = "" if value is None else str(value)
+        if str_val not in self.choices:
             choices = ", ".join(f'"{c}"' for c in self.choices)
-            return [
+            problems += [
                 ProblemPredicate(
-                    f' is "{value}", not one of the allowed values [{choices}]'
+                    f' is "{str_val}", not one of the allowed values [{choices}]'
                 )
             ]
 
-        return []
+        return problems
```

### Comparing `statelint-0.2.0/statelint/fields/timestamp_field.py` & `statelint-1.0.0/statelint/fields/timestamp_field.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/linter.py` & `statelint-1.0.0/statelint/linter.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/nodes/container_state.py` & `statelint-1.0.0/statelint/nodes/container_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/nodes/factory/factory.py` & `statelint-1.0.0/statelint/nodes/factory/factory.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/nodes/mixins/__init__.py` & `statelint-1.0.0/statelint/nodes/mixins/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import List
 
 from ...fields import END, NEXT, RESULT, TIMEOUT_SECONDS, Field
 from ..node import Node
 from .catcher_mixin import CatchMixin
 from .choices_mixin import ChoicesMixin
-from .payload_template_mixin import ParametersMixin, ResultSelectorMixin
+from .payload_template_mixin import (
+    BatchInputMixin,
+    ItemSelectorMixin,
+    ParametersMixin,
+    ResultSelectorMixin,
+)
 from .result_path_mixin import ResultPathMixin
 from .retrier_mixin import RetryMixin
 
 
 class ResultMixin(Node):
     @property
     def optional_fields(self) -> List[Field]:
```

### Comparing `statelint-0.2.0/statelint/nodes/mixins/catcher_mixin.py` & `statelint-1.0.0/statelint/nodes/mixins/catcher_mixin.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/nodes/mixins/choices_mixin.py` & `statelint-1.0.0/statelint/nodes/mixins/choices_mixin.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/nodes/mixins/payload_template_mixin.py` & `statelint-1.0.0/statelint/nodes/mixins/payload_template_mixin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import itertools
 from typing import Any, List
 
-from ...fields import PARAMETERS, RESULT_SELECTOR, Field
+from ...fields import (
+    BATCH_INPUT,
+    ITEM_SELECTOR,
+    PARAMETERS,
+    RESULT_SELECTOR,
+    Field,
+    OneOfField,
+)
 from ...problem import Problem
 from ...utils.re_helper import is_intrinsic_invocation, is_path
 from ..node import Node, StatePath
 
 
 class ParametersMixin(Node):
     @property
@@ -18,14 +25,30 @@
             return problems
 
         return problems + _validate_payload(
             PARAMETERS, self.state_path, self._state[PARAMETERS.name]
         )
 
 
+class ItemSelectorMixin(Node):
+    @property
+    def optional_fields(self) -> List[Field]:
+        return [*super().optional_fields, OneOfField(PARAMETERS, ITEM_SELECTOR)]
+
+    def validate(self) -> List[Problem]:
+        problems = [*super().validate()]
+        for field in (PARAMETERS, ITEM_SELECTOR):
+            if isinstance(self._state.get(field.name), dict):
+                problems += _validate_payload(
+                    field, self.state_path, self._state[field.name]
+                )
+
+        return problems
+
+
 class ResultSelectorMixin(Node):
     @property
     def optional_fields(self) -> List[Field]:
         return [*super().optional_fields, RESULT_SELECTOR]
 
     def validate(self) -> List[Problem]:
         problems = [*super().validate()]
@@ -33,14 +56,28 @@
             return problems
 
         return problems + _validate_payload(
             RESULT_SELECTOR, self.state_path, self._state[RESULT_SELECTOR.name]
         )
 
 
+class BatchInputMixin(Node):
+    @property
+    def optional_fields(self) -> List[Field]:
+        return [*super().optional_fields, BATCH_INPUT]
+
+    def validate(self) -> List[Problem]:
+        problems = super().validate()
+        batch_input = self._state.get(BATCH_INPUT.name)
+        if not isinstance(batch_input, dict):
+            return problems
+
+        return problems + _validate_payload(BATCH_INPUT, self.state_path, batch_input)
+
+
 def _validate_payload(
     field: Field, current_path: StatePath, param: Any
 ) -> List[Problem]:
     problems = []
     if isinstance(param, list):
         return list(
             itertools.chain.from_iterable(
```

### Comparing `statelint-0.2.0/statelint/nodes/node.py` & `statelint-1.0.0/statelint/nodes/node.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/nodes/parallel_state.py` & `statelint-1.0.0/statelint/nodes/parallel_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/nodes/state_machine.py` & `statelint-1.0.0/statelint/nodes/state_machine.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/nodes/task_state.py` & `statelint-1.0.0/statelint/nodes/task_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List
 
 from ..fields import (
+    CREDENTIALS,
     HEARTBEAT_SECONDS,
     HEARTBEAT_SECONDS_PATH,
     RESOURCE,
     TIMEOUT_SECONDS,
     TIMEOUT_SECONDS_PATH,
     Field,
     OneOfField,
@@ -34,8 +35,9 @@
     @property
     def optional_fields(self) -> List[Field]:
         return [
             *super().optional_fields,
             RESOURCE,
             OneOfField(TIMEOUT_SECONDS, TIMEOUT_SECONDS_PATH),
             OneOfField(HEARTBEAT_SECONDS, HEARTBEAT_SECONDS_PATH),
+            CREDENTIALS,
         ]
```

### Comparing `statelint-0.2.0/statelint/nodes/wait_state.py` & `statelint-1.0.0/statelint/nodes/wait_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint/utils/re_helper.py` & `statelint-1.0.0/statelint/utils/re_helper.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/statelint.egg-info/PKG-INFO` & `statelint-1.0.0/statelint.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: statelint
-Version: 0.2.0
+Version: 1.0.0
 Summary: command-line validator for Amazon States Language
 Home-page: https://github.com/taro-kayo/statelint
 Author: taro-kayo
 License: Apache License 2.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Provides-Extra: yaml
 License-File: LICENSE
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: regex>=2023.5.5
+Provides-Extra: yaml
+Requires-Dist: PyYAML>=6.0; extra == "yaml"
 
 # statelint
 <a href="https://github.com/taro-kayo/statelint/actions"><img alt="Actions Status" src="https://github.com/taro-kayo/statelint/workflows/Test/badge.svg"></a>
 <a href="https://coveralls.io/github/taro-kayo/statelint?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/taro-kayo/statelint/badge.svg?branch=main"></a>
 <a href="https://github.com/taro-kayo/statelint/blob/main/LICENSE"><img alt="License: Apache License 2.0" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg"></a>
 <a href="https://pypi.org/project/statelint/"><img alt="PyPI" src="https://img.shields.io/pypi/v/statelint"></a>
-<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+[![Downloads](https://static.pepy.tech/badge/statelint/month)](https://pepy.tech/project/statelint)
 
 A PyPI package providing a validator for [Amazon States Language](https://states-language.net/spec.html) JSON/YAML files.
 
 This package is based on Amazon Web Services Labs' [awslabs/statelint](https://github.com/awslabs/statelint).
 
 ## Installation
 
@@ -70,13 +74,7 @@
 ```
 
 You can pass both parameters at the same time.
 
 ```shell
 statelint --ignore=FLOAT,URI fancy-state-machine-spec.json
 ```
-
-## TODO
-
-- [reference path with dash doesn't validate](https://github.com/awslabs/statelint/issues/17)
-- [Reference Path with unicode doesn't validate](https://github.com/awslabs/statelint/issues/23)
-- [Does not catch Duplicated State names](https://github.com/awslabs/statelint/issues/39)
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: statelint Version: 0.2.0 Summary: command-line
+Metadata-Version: 2.1 Name: statelint Version: 1.0.0 Summary: command-line
 validator for Amazon States Language Home-page: https://github.com/taro-kayo/
 statelint Author: taro-kayo License: Apache License 2.0 Classifier: Development
-Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
-Audience :: Developers Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.8.0 Description-Content-Type: text/markdown Provides-Extra: yaml
-License-File: LICENSE # statelint _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:
-_A_p_a_c_h_e_ _L_i_c_e_n_s_e_ _2_._0_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]A PyPI package providing a
-validator for [Amazon States Language](https://states-language.net/spec.html)
-JSON/YAML files. This package is based on Amazon Web Services Labs' [awslabs/
-statelint](https://github.com/awslabs/statelint). ## Installation ```shell pip
-install statelint ``` ## Usage ```shell statelint fancy-state-machine-spec.json
-``` If you prefer YAML, you need to install [PyYaml](https://pypi.org/project/
-PyYAML/). ```shell pip install PyYAML ``` Then, run command with a `--yaml`
-parameter. ```shell statelint --yaml fancy-state-machine-spec.yaml ``` If you
-don't like to be complained that `BackoffRate` doesn't end with ".0", pass a `-
--ignore=FLOAT` parameter. ```shell statelint --ignore=FLOAT fancy-state-
-machine-spec.json ``` If your `Resource` doesn't contain URI string, pass a `--
-ignore=URI` parameter. ```shell statelint --ignore=URI fancy-state-machine-
-spec.json ``` You can pass both parameters at the same time. ```shell statelint
---ignore=FLOAT,URI fancy-state-machine-spec.json ``` ## TODO - [reference path
-with dash doesn't validate](https://github.com/awslabs/statelint/issues/17) -
-[Reference Path with unicode doesn't validate](https://github.com/awslabs/
-statelint/issues/23) - [Does not catch Duplicated State names](https://
-github.com/awslabs/statelint/issues/39)
+Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+python-dateutil>=2.8.2 Requires-Dist: regex>=2023.5.5 Provides-Extra: yaml
+Requires-Dist: PyYAML>=6.0; extra == "yaml" # statelint _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]
+_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _L_i_c_e_n_s_e_ _2_._0_]_[_P_y_P_I_][![Downloads](https://
+static.pepy.tech/badge/statelint/month)](https://pepy.tech/project/statelint) A
+PyPI package providing a validator for [Amazon States Language](https://states-
+language.net/spec.html) JSON/YAML files. This package is based on Amazon Web
+Services Labs' [awslabs/statelint](https://github.com/awslabs/statelint). ##
+Installation ```shell pip install statelint ``` ## Usage ```shell statelint
+fancy-state-machine-spec.json ``` If you prefer YAML, you need to install
+[PyYaml](https://pypi.org/project/PyYAML/). ```shell pip install PyYAML ```
+Then, run command with a `--yaml` parameter. ```shell statelint --yaml fancy-
+state-machine-spec.yaml ``` If you don't like to be complained that
+`BackoffRate` doesn't end with ".0", pass a `--ignore=FLOAT` parameter.
+```shell statelint --ignore=FLOAT fancy-state-machine-spec.json ``` If your
+`Resource` doesn't contain URI string, pass a `--ignore=URI` parameter.
+```shell statelint --ignore=URI fancy-state-machine-spec.json ``` You can pass
+both parameters at the same time. ```shell statelint --ignore=FLOAT,URI fancy-
+state-machine-spec.json ```
```

### Comparing `statelint-0.2.0/statelint.egg-info/SOURCES.txt` & `statelint-1.0.0/statelint.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 statelint/problem/problem_type.py
 statelint/utils/__init__.py
 statelint/utils/re_helper.py
 tests/test_catcher.py
 tests/test_choice_rule.py
 tests/test_choice_state.py
 tests/test_cli.py
+tests/test_fail_state.py
 tests/test_fields.py
 tests/test_linter.py
 tests/test_map_state.py
 tests/test_parallel_state.py
 tests/test_parameters.py
 tests/test_pass_state.py
 tests/test_ref_pattern_field.py
```

### Comparing `statelint-0.2.0/tests/test_catcher.py` & `statelint-1.0.0/tests/test_catcher.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_choice_rule.py` & `statelint-1.0.0/tests/test_choice_rule.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_choice_state.py` & `statelint-1.0.0/tests/test_choice_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_cli.py` & `statelint-1.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_fields.py` & `statelint-1.0.0/tests/test_fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from statelint.linter import Linter
 
 
 def test_null_type():
     state_machine = {"StartAt": "x", "States": {"x": {"Type": None, "End": True}}}
     assert Linter.validate(state_machine) == [
         "State Machine.States.x.Type should be non-null",
+        'State Machine.States.x.Type is "", not one of the allowed values '
+        '["Pass", "Succeed", "Fail", "Task", "Choice", "Wait", "Parallel", "Map"]',
         'Field "End" not allowed in State Machine.States.x',
     ]
 
 
 def test_illegal_type():
     state_machine = {"StartAt": "x", "States": {"x": {"Type": "?", "End": True}}}
     assert Linter.validate(state_machine) == [
```

### Comparing `statelint-0.2.0/tests/test_linter.py` & `statelint-1.0.0/tests/test_linter.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_parallel_state.py` & `statelint-1.0.0/tests/test_parallel_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_parameters.py` & `statelint-1.0.0/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_pass_state.py` & `statelint-1.0.0/tests/test_pass_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_ref_pattern_field.py` & `statelint-1.0.0/tests/test_ref_pattern_field.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_retrier.py` & `statelint-1.0.0/tests/test_task_state.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,118 @@
+import pytest
+
 from statelint.linter import Linter
 
 
 def test_ok():
     state_machine = {
         "States": {
             "x": {
                 "Type": "Task",
                 "End": True,
+                "ResultPath": None,
                 "Resource": "arn:x",
-                "Retry": [
-                    {
-                        "ErrorEquals": ["E"],
-                        "IntervalSeconds": 99999999,
-                        "MaxAttempts": 99999998,
-                        "BackoffRate": 1.0,
-                    }
-                ],
-            },
+                "TimeoutSeconds": 1,
+                "ResultSelector": {},
+                "Parameters": {},
+                "Credentials": {},
+                "Catch": [],
+            }
+        },
+        "StartAt": "x",
+    }
+    assert Linter.validate(state_machine) == []
+
+
+def test_ok_min():
+    state_machine = {
+        "States": {
+            "x": {
+                "Type": "Task",
+                "End": True,
+                "Resource": "arn:x",
+            }
         },
         "StartAt": "x",
     }
     assert Linter.validate(state_machine) == []
 
 
 def test_bad_fields():
     state_machine = {
         "States": {
             "x": {
                 "Type": "Task",
                 "End": True,
+                "ResultPath": ".x",
+                "Resource": "xxx",
+                "TimeoutSeconds": 0,
+                "ResultSelector": None,
+                "Parameters": "x",
+            }
+        },
+        "StartAt": "x",
+    }
+    assert Linter.validate(state_machine) == [
+        'State Machine.States.x.ResultPath is ".x" but should be a Reference Path',
+        'State Machine.States.x.Resource is "xxx" but should be A URI',
+        "State Machine.States.x.TimeoutSeconds is 0 but allowed floor is 0",
+    ]
+
+
+@pytest.mark.parametrize("name", ["TimeoutSeconds", "HeartbeatSeconds"])
+def test_one_of_fields(name):
+    state_machine = {
+        "States": {
+            "x": {
+                "Type": "Task",
+                "End": True,
+                "Resource": "arn:x",
+                name: 1,
+                f"{name}Path": "$",
+            }
+        },
+        "StartAt": "x",
+    }
+    assert Linter.validate(state_machine) == [
+        f'State Machine.States.x may have only one of ["{name}", "{name}Path"]',
+    ]
+
+
+def test_catch():
+    state_machine = {
+        "States": {"x": {"Type": "Task", "End": True, "Resource": "arn:x", "Catch": 1}},
+        "StartAt": "x",
+    }
+    assert Linter.validate(state_machine) == [
+        "State Machine.States.x.Catch is 1 but should be an Array"
+    ]
+
+
+def test_catch_null():
+    state_machine = {
+        "States": {
+            "x": {"Type": "Task", "End": True, "Resource": "arn:x", "Catch": None}
+        },
+        "StartAt": "x",
+    }
+    assert Linter.validate(state_machine) == [
+        "State Machine.States.x.Catch should be non-null"
+    ]
+
+
+def test_catch_element():
+    state_machine = {
+        "States": {
+            "x": {
+                "Type": "Task",
+                "End": True,
                 "Resource": "arn:x",
-                "Retry": [
-                    {
-                        "ErrorEquals": [],
-                        "IntervalSeconds": -1,
-                        "MaxAttempts": 0,
-                        "BackoffRate": 1,
-                    }
-                ],
+                "Catch": [1, "x"],
             },
         },
         "StartAt": "x",
     }
     assert Linter.validate(state_machine) == [
-        "State Machine.States.x.Retry[0].ErrorEquals is empty, non-empty required",
-        "State Machine.States.x.Retry[0].IntervalSeconds is -1 but allowed floor is 0",
-        "State Machine.States.x.Retry[0].BackoffRate is 1 but should be a Float",
+        "State Machine.States.x.Catch[0] is 1 but should be an Object",
+        'State Machine.States.x.Catch[1] is "x" but should be an Object',
     ]
```

### Comparing `statelint-0.2.0/tests/test_state_machine.py` & `statelint-1.0.0/tests/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_terminal_state.py` & `statelint-1.0.0/tests/test_terminal_state.py`

 * *Files identical despite different names*

### Comparing `statelint-0.2.0/tests/test_wait_state.py` & `statelint-1.0.0/tests/test_wait_state.py`

 * *Files identical despite different names*

