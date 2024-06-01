# Comparing `tmp/composio_core-0.3.3.tar.gz` & `tmp/composio_core-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.3.3.tar", last modified: Fri May 31 15:19:55 2024, max compression
+gzip compressed data, was "composio_core-0.3.4.tar", last modified: Sat Jun  1 00:39:12 2024, max compression
```

## Comparing `composio_core-0.3.3.tar` & `composio_core-0.3.4.tar`

### file list

```diff
@@ -1,99 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.446807 composio_core-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 15:19:19.000000 composio_core-0.3.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-31 15:19:55.446807 composio_core-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-31 15:19:19.000000 composio_core-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.430807 composio_core-0.3.3/composio/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.434807 composio_core-0.3.3/composio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/add.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8106 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/client/
--rw-r--r--   0 runner    (1001) docker     (127)    31369 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)   316153 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/local_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/file/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/file/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/local_workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19278 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/commons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/command_runner_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/get_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/history_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/local_docker_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/workspace_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/mathematical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/mathematical/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/mathematical/mathematical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/storage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.446807 composio_core-0.3.3/composio/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/tools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.446807 composio_core-0.3.3/composio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.446807 composio_core-0.3.3/composio_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:19:55.446807 composio_core-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-31 15:19:19.000000 composio_core-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.756622 composio_core-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-01 00:38:03.000000 composio_core-0.3.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 00:39:12.756622 composio_core-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-06-01 00:38:03.000000 composio_core-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.740622 composio_core-0.3.4/composio/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/add.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8536 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    32419 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)   316458 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/local_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/file/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/actions/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/greptile/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/greptile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/greptile/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/greptile/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/greptile/actions/codequery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/greptile/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/local_workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/command_runner_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/get_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/history_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/local_docker_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/mathematical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/mathematical/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/local_tools/ragtool/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/local_tools/ragtool/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/actions/rag_add_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/actions/rag_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/local_tools/webtool/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/local_tools/webtool/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/actions/scrape_website_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/actions/scrape_website_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/storage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.756622 composio_core-0.3.4/composio_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:39:12.756622 composio_core-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-01 00:38:03.000000 composio_core-0.3.4/setup.py
```

### Comparing `composio_core-0.3.3/PKG-INFO` & `composio_core-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.3
+Version: 0.3.4
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.3/README.md` & `composio_core-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/cli/__init__.py` & `composio_core-0.3.4/composio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/cli/actions.py` & `composio_core-0.3.4/composio/cli/actions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/cli/add.py` & `composio_core-0.3.4/composio/cli/add.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/cli/apps.py` & `composio_core-0.3.4/composio/cli/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,20 +172,31 @@
         )
         triggers = sorted(
             context.client.triggers.get(),
             key=lambda x: x.appKey,
         )
         if not beta:
             c = []
-            for app in apps:
-                if app.name.lower().endswith("beta"):
-                    continue
-                c.append(app)
-            apps = c
-            # apps = list(set([app for app in apps if not app.name.lower().endswith("beta")]))
+            def filter_non_beta_items(items):
+                filtered_items = []
+                for item in items:
+                    if not item.name.lower().endswith("beta"):
+                        filtered_items.append(item)
+                
+                seen = set()
+                unique_items = []
+                for item in filtered_items:
+                    if item.name not in seen:
+                        unique_items.append(item)
+                        seen.add(item.name)
+                return unique_items
+
+            apps = filter_non_beta_items(apps)
+            actions = filter_non_beta_items(actions)
+            triggers = filter_non_beta_items(triggers)
 
         enum_module = MODULE_TEMPLATE.format(
             tag_enum=_get_tag_enum(apps=apps, actions=actions),
             app_enum=_get_app_enum(apps=apps),
             action_enum=_get_action_enum(apps=apps, actions=actions),
             trigger_enum=_get_trigger_enum(apps=apps, triggers=triggers),
         )
```

### Comparing `composio_core-0.3.3/composio/cli/connections.py` & `composio_core-0.3.4/composio/cli/connections.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/cli/context.py` & `composio_core-0.3.4/composio/cli/context.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/cli/integrations.py` & `composio_core-0.3.4/composio/cli/integrations.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/cli/login.py` & `composio_core-0.3.4/composio/cli/login.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/cli/triggers.py` & `composio_core-0.3.4/composio/cli/triggers.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/client/__init__.py` & `composio_core-0.3.4/composio/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -724,15 +724,23 @@
     def execute(
         self,
         action: Action,
         params: t.Dict,
         entity_id: str,
         connected_account: t.Optional[str] = None,
     ) -> t.Dict:
-        """Execute an action."""
+        """
+        Execute an action on the specified entity with optional connected account.
+
+        :param action: The Action object to be executed.
+        :param params: A dictionary of parameters to be passed to the action.
+        :param entity_id: The unique identifier of the entity on which the action is executed.
+        :param connected_account: Optional connected account ID if required for the action.
+        :return: A dictionary containing the response from the executed action.
+        """
         if action.is_local:
             return self.local_handler.execute_local_action(
                 action=action,
                 request_data=params,
             )
         if action.no_auth:
             return self._raise_if_required(
@@ -1007,15 +1015,24 @@
         self,
         app_name: t.Union[str, App],
         auth_mode: t.Optional[str] = None,
         auth_config: t.Optional[t.Dict[str, t.Any]] = None,
         redirect_url: t.Optional[str] = None,
         integration: t.Optional[IntegrationModel] = None,
     ) -> ConnectionRequestModel:
-        """Initiate integration connection."""
+        """
+        Initiate an integration connection process for a specified application.
+
+        :param app_name: The name of the application or an App enum instance.
+        :param auth_mode: Optional authentication mode to be used.
+        :param auth_config: Optional dictionary containing authentication configuration details.
+        :param redirect_url: Optional URL to which a user will be redirected after authentication.
+        :param integration: Optional existing IntegrationModel instance to be used.
+        :return: A ConnectionRequestModel instance representing the initiated connection.
+        """
         if isinstance(app_name, App):
             app_name = app_name.value
 
         app = self.client.apps.get(name=app_name)
         timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
         if integration is None and auth_mode is not None:
             integration = self.client.integrations.create(
```

### Comparing `composio_core-0.3.3/composio/client/endpoints.py` & `composio_core-0.3.4/composio/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/client/enums.py` & `composio_core-0.3.4/composio/client/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,360 +12,360 @@
 
     @property
     def name(self) -> str:
         """Returns trigger name."""
         return self.value[0]
 
     IMPORTANT = ("default", "important")
-    ASANA_PROJECT_MEMBERSHIPS = ("asana", "Project memberships")
-    ASANA_WEBHOOKS = ("asana", "Webhooks")
-    ASANA_AUDIT_LOG_API = ("asana", "Audit log API")
-    ASANA_TYPEAHEAD = ("asana", "Typeahead")
-    ASANA_WORKSPACES = ("asana", "Workspaces")
-    ASANA_PROJECT_BRIEFS = ("asana", "Project briefs")
-    ASANA_PROJECT_STATUSES = ("asana", "Project statuses")
-    ASANA_EVENTS = ("asana", "Events")
-    ASANA_STATUS_UPDATES = ("asana", "Status updates")
-    ASANA_TEAMS = ("asana", "Teams")
-    ASANA_BATCH_API = ("asana", "Batch API")
-    ASANA_ATTACHMENTS = ("asana", "Attachments")
-    ASANA_ORGANIZATION_EXPORTS = ("asana", "Organization exports")
+    ASANA_PORTFOLIOS = ("asana", "Portfolios")
     ASANA_PORTFOLIO_MEMBERSHIPS = ("asana", "Portfolio memberships")
-    ASANA_PROJECTS = ("asana", "Projects")
-    ASANA_USER_TASK_LISTS = ("asana", "User task lists")
-    ASANA_USERS = ("asana", "Users")
+    ASANA_EVENTS = ("asana", "Events")
+    ASANA_RULES = ("asana", "Rules")
     ASANA_MEMBERSHIPS = ("asana", "Memberships")
+    ASANA_PROJECT_BRIEFS = ("asana", "Project briefs")
+    ASANA_TEAMS = ("asana", "Teams")
     ASANA_ALLOCATIONS = ("asana", "Allocations")
+    ASANA_TYPEAHEAD = ("asana", "Typeahead")
+    ASANA_TASKS = ("asana", "Tasks")
+    ASANA_WORKSPACE_MEMBERSHIPS = ("asana", "Workspace memberships")
+    ASANA_WEBHOOKS = ("asana", "Webhooks")
+    ASANA_PROJECTS = ("asana", "Projects")
+    ASANA_PROJECT_TEMPLATES = ("asana", "Project templates")
+    ASANA_STORIES = ("asana", "Stories")
+    ASANA_ORGANIZATION_EXPORTS = ("asana", "Organization exports")
     ASANA_TEAM_MEMBERSHIPS = ("asana", "Team memberships")
+    ASANA_AUDIT_LOG_API = ("asana", "Audit log API")
+    ASANA_TASK_TEMPLATES = ("asana", "Task templates")
     ASANA_GOALS = ("asana", "Goals")
-    ASANA_JOBS = ("asana", "Jobs")
-    ASANA_PORTFOLIOS = ("asana", "Portfolios")
-    ASANA_STORIES = ("asana", "Stories")
+    ASANA_GOAL_RELATIONSHIPS = ("asana", "Goal relationships")
+    ASANA_BATCH_API = ("asana", "Batch API")
+    ASANA_PROJECT_MEMBERSHIPS = ("asana", "Project memberships")
     ASANA_TAGS = ("asana", "Tags")
-    ASANA_TASK_TEMPLATES = ("asana", "Task templates")
     ASANA_CUSTOM_FIELDS = ("asana", "Custom fields")
     ASANA_TIME_PERIODS = ("asana", "Time periods")
-    ASANA_RULES = ("asana", "Rules")
-    ASANA_WORKSPACE_MEMBERSHIPS = ("asana", "Workspace memberships")
-    ASANA_TASKS = ("asana", "Tasks")
+    ASANA_ATTACHMENTS = ("asana", "Attachments")
+    ASANA_USER_TASK_LISTS = ("asana", "User task lists")
     ASANA_CUSTOM_FIELD_SETTINGS = ("asana", "Custom field settings")
-    ASANA_SECTIONS = ("asana", "Sections")
+    ASANA_USERS = ("asana", "Users")
+    ASANA_STATUS_UPDATES = ("asana", "Status updates")
     ASANA_TIME_TRACKING_ENTRIES = ("asana", "Time tracking entries")
-    ASANA_PROJECT_TEMPLATES = ("asana", "Project templates")
-    ASANA_GOAL_RELATIONSHIPS = ("asana", "Goal relationships")
-    ATTIO_THREADS = ("attio", "Threads")
-    ATTIO_NOTES = ("attio", "Notes")
-    ATTIO_WEBHOOKS = ("attio", "Webhooks")
-    ATTIO_LISTS = ("attio", "Lists")
-    ATTIO_TASKS = ("attio", "Tasks")
-    ATTIO_OBJECTS = ("attio", "Objects")
+    ASANA_SECTIONS = ("asana", "Sections")
+    ASANA_JOBS = ("asana", "Jobs")
+    ASANA_PROJECT_STATUSES = ("asana", "Project statuses")
+    ASANA_WORKSPACES = ("asana", "Workspaces")
     ATTIO_ATTRIBUTES = ("attio", "Attributes")
+    ATTIO_OBJECTS = ("attio", "Objects")
+    ATTIO_WEBHOOKS = ("attio", "Webhooks")
+    ATTIO_THREADS = ("attio", "Threads")
     ATTIO_META = ("attio", "Meta")
-    ATTIO_ENTRIES = ("attio", "Entries")
+    ATTIO_WORKSPACE_MEMBERS = ("attio", "Workspace members")
+    ATTIO_NOTES = ("attio", "Notes")
     ATTIO_COMMENTS = ("attio", "Comments")
     ATTIO_RECORDS = ("attio", "Records")
-    ATTIO_WORKSPACE_MEMBERS = ("attio", "Workspace members")
-    BREVO_WHATSAPP_CAMPAIGNS = ("brevo", "WhatsApp Campaigns")
-    BREVO_WEBHOOKS = ("brevo", "Webhooks")
-    BREVO_EVENT = ("brevo", "Event")
-    BREVO_SENDERS = ("brevo", "Senders")
+    ATTIO_TASKS = ("attio", "Tasks")
+    ATTIO_ENTRIES = ("attio", "Entries")
+    ATTIO_LISTS = ("attio", "Lists")
+    BREVO_COMPANIES = ("brevo", "Companies")
+    BREVO_EXTERNAL_FEEDS = ("brevo", "External Feeds")
+    BREVO_INBOUND_PARSING = ("brevo", "Inbound Parsing")
     BREVO_ACCOUNT = ("brevo", "Account")
-    BREVO_TRANSACTIONAL_WHATSAPP = ("brevo", "Transactional WhatsApp")
     BREVO_CONVERSATIONS = ("brevo", "Conversations")
+    BREVO_RESELLER = ("brevo", "Reseller")
     BREVO_USER = ("brevo", "User")
-    BREVO_TRANSACTIONAL_SMS = ("brevo", "Transactional SMS")
-    BREVO_EMAIL_CAMPAIGNS = ("brevo", "Email Campaigns")
     BREVO_SMS_CAMPAIGNS = ("brevo", "SMS Campaigns")
-    BREVO_RESELLER = ("brevo", "Reseller")
-    BREVO_CONTACTS = ("brevo", "Contacts")
-    BREVO_INBOUND_PARSING = ("brevo", "Inbound Parsing")
-    BREVO_ECOMMERCE = ("brevo", "Ecommerce")
-    BREVO_DEALS = ("brevo", "Deals")
+    BREVO_NOTES = ("brevo", "Notes")
+    BREVO_TASKS = ("brevo", "Tasks")
+    BREVO_WHATSAPP_CAMPAIGNS = ("brevo", "WhatsApp Campaigns")
+    BREVO_WEBHOOKS = ("brevo", "Webhooks")
+    BREVO_TRANSACTIONAL_WHATSAPP = ("brevo", "Transactional WhatsApp")
     BREVO_COUPONS = ("brevo", "Coupons")
-    BREVO_TRANSACTIONAL_EMAILS = ("brevo", "Transactional emails")
-    BREVO_COMPANIES = ("brevo", "Companies")
     BREVO_DOMAINS = ("brevo", "Domains")
+    BREVO_EVENT = ("brevo", "Event")
+    BREVO_EMAIL_CAMPAIGNS = ("brevo", "Email Campaigns")
+    BREVO_TRANSACTIONAL_EMAILS = ("brevo", "Transactional emails")
+    BREVO_SENDERS = ("brevo", "Senders")
+    BREVO_TRANSACTIONAL_SMS = ("brevo", "Transactional SMS")
     BREVO_PROCESS = ("brevo", "Process")
-    BREVO_FILES = ("brevo", "Files")
+    BREVO_DEALS = ("brevo", "Deals")
+    BREVO_CONTACTS = ("brevo", "Contacts")
     BREVO_MASTER_ACCOUNT = ("brevo", "Master account")
-    BREVO_NOTES = ("brevo", "Notes")
-    BREVO_TASKS = ("brevo", "Tasks")
-    BREVO_EXTERNAL_FEEDS = ("brevo", "External Feeds")
+    BREVO_ECOMMERCE = ("brevo", "Ecommerce")
+    BREVO_FILES = ("brevo", "Files")
+    CLICKUP_MEMBERS = ("clickup", "Members")
+    CLICKUP_GUESTS = ("clickup", "Guests")
+    CLICKUP_SPACES = ("clickup", "Spaces")
+    CLICKUP_FOLDERS = ("clickup", "Folders")
+    CLICKUP_TEAMS___WORKSPACES = ("clickup", "Teams - Workspaces")
+    CLICKUP_TIME_TRACKING__LEGACY_ = ("clickup", "Time Tracking (Legacy)")
     CLICKUP_ROLES = ("clickup", "Roles")
-    CLICKUP_SHARED_HIERARCHY = ("clickup", "Shared Hierarchy")
+    CLICKUP_TASK_CHECKLISTS = ("clickup", "Task Checklists")
+    CLICKUP_TASKS = ("clickup", "Tasks")
+    CLICKUP_LISTS = ("clickup", "Lists")
+    CLICKUP_CUSTOM_FIELDS = ("clickup", "Custom Fields")
+    CLICKUP_TIME_TRACKING = ("clickup", "Time Tracking")
     CLICKUP_WEBHOOKS = ("clickup", "Webhooks")
-    CLICKUP_CUSTOM_TASK_TYPES = ("clickup", "Custom Task Types")
     CLICKUP_AUTHORIZATION = ("clickup", "Authorization")
-    CLICKUP_CUSTOM_FIELDS = ("clickup", "Custom Fields")
-    CLICKUP_ATTACHMENTS = ("clickup", "Attachments")
-    CLICKUP_USERS = ("clickup", "Users")
-    CLICKUP_TIME_TRACKING__LEGACY_ = ("clickup", "Time Tracking (Legacy)")
-    CLICKUP_GUESTS = ("clickup", "Guests")
+    CLICKUP_CUSTOM_TASK_TYPES = ("clickup", "Custom Task Types")
     CLICKUP_GOALS = ("clickup", "Goals")
-    CLICKUP_TEAMS___WORKSPACES = ("clickup", "Teams - Workspaces")
-    CLICKUP_COMMENTS = ("clickup", "Comments")
-    CLICKUP_MEMBERS = ("clickup", "Members")
-    CLICKUP_FOLDERS = ("clickup", "Folders")
-    CLICKUP_SPACES = ("clickup", "Spaces")
+    CLICKUP_TASK_RELATIONSHIPS = ("clickup", "Task Relationships")
     CLICKUP_TAGS = ("clickup", "Tags")
-    CLICKUP_TEAMS___USER_GROUPS = ("clickup", "Teams - User Groups")
     CLICKUP_VIEWS = ("clickup", "Views")
-    CLICKUP_TASK_RELATIONSHIPS = ("clickup", "Task Relationships")
+    CLICKUP_ATTACHMENTS = ("clickup", "Attachments")
+    CLICKUP_USERS = ("clickup", "Users")
+    CLICKUP_COMMENTS = ("clickup", "Comments")
+    CLICKUP_SHARED_HIERARCHY = ("clickup", "Shared Hierarchy")
     CLICKUP_TASK_TEMPLATES = ("clickup", "Task Templates")
-    CLICKUP_LISTS = ("clickup", "Lists")
-    CLICKUP_TASKS = ("clickup", "Tasks")
-    CLICKUP_TASK_CHECKLISTS = ("clickup", "Task Checklists")
-    CLICKUP_TIME_TRACKING = ("clickup", "Time Tracking")
-    ELEVENLABS_VOICE_GENERATION = ("elevenlabs", "voice-generation")
+    CLICKUP_TEAMS___USER_GROUPS = ("clickup", "Teams - User Groups")
+    ELEVENLABS_SAMPLES = ("elevenlabs", "samples")
     ELEVENLABS_SPEECH_TO_SPEECH = ("elevenlabs", "speech-to-speech")
-    ELEVENLABS_SPEECH_HISTORY = ("elevenlabs", "speech-history")
-    ELEVENLABS_MODELS = ("elevenlabs", "models")
+    ELEVENLABS_VOICE_GENERATION = ("elevenlabs", "voice-generation")
+    ELEVENLABS_TEXT_TO_SPEECH = ("elevenlabs", "text-to-speech")
     ELEVENLABS_PROJECTS = ("elevenlabs", "projects")
-    ELEVENLABS_AUDIO_NATIVE = ("elevenlabs", "audio-native")
     ELEVENLABS_WORKSPACE = ("elevenlabs", "workspace")
-    ELEVENLABS_PRONUNCIATION_DICTIONARY = ("elevenlabs", "Pronunciation Dictionary")
-    ELEVENLABS_TEXT_TO_SPEECH = ("elevenlabs", "text-to-speech")
-    ELEVENLABS_SAMPLES = ("elevenlabs", "samples")
-    ELEVENLABS_DUBBING = ("elevenlabs", "dubbing")
+    ELEVENLABS_AUDIO_NATIVE = ("elevenlabs", "audio-native")
+    ELEVENLABS_SPEECH_HISTORY = ("elevenlabs", "speech-history")
     ELEVENLABS_USER = ("elevenlabs", "user")
+    ELEVENLABS_DUBBING = ("elevenlabs", "dubbing")
+    ELEVENLABS_PRONUNCIATION_DICTIONARY = ("elevenlabs", "Pronunciation Dictionary")
     ELEVENLABS_VOICES = ("elevenlabs", "voices")
-    FIGMA_FILES = ("figma", "Files")
-    FIGMA_WEBHOOKS = ("figma", "Webhooks")
-    FIGMA_USERS = ("figma", "Users")
-    FIGMA_PROJECTS = ("figma", "Projects")
-    FIGMA_COMPONENT_SETS = ("figma", "Component Sets")
+    ELEVENLABS_MODELS = ("elevenlabs", "models")
     FIGMA_PAYMENTS = ("figma", "Payments")
-    FIGMA_VARIABLES = ("figma", "Variables")
-    FIGMA_STYLES = ("figma", "Styles")
-    FIGMA_COMMENT_REACTIONS = ("figma", "Comment Reactions")
-    FIGMA_COMMENTS = ("figma", "Comments")
     FIGMA_ACTIVITY_LOGS = ("figma", "Activity Logs")
     FIGMA_DEV_RESOURCES = ("figma", "Dev Resources")
+    FIGMA_VARIABLES = ("figma", "Variables")
+    FIGMA_USERS = ("figma", "Users")
+    FIGMA_COMMENTS = ("figma", "Comments")
+    FIGMA_COMMENT_REACTIONS = ("figma", "Comment Reactions")
+    FIGMA_FILES = ("figma", "Files")
+    FIGMA_STYLES = ("figma", "Styles")
     FIGMA_COMPONENTS = ("figma", "Components")
-    GITHUB_SECRET_SCANNING = ("github", "secret-scanning")
-    GITHUB_GIT = ("github", "git")
-    GITHUB_COPILOT = ("github", "copilot")
-    GITHUB_PROJECTS = ("github", "projects")
-    GITHUB_CHECKS = ("github", "checks")
-    GITHUB_ORGS = ("github", "orgs")
-    GITHUB_MIGRATIONS = ("github", "migrations")
-    GITHUB_RATE_LIMIT = ("github", "rate-limit")
-    GITHUB_CLASSROOM = ("github", "classroom")
+    FIGMA_WEBHOOKS = ("figma", "Webhooks")
+    FIGMA_COMPONENT_SETS = ("figma", "Component Sets")
+    FIGMA_PROJECTS = ("figma", "Projects")
+    GITHUB_GITIGNORE = ("github", "gitignore")
+    GITHUB_CODE = ("github", "code")
     GITHUB_GISTS = ("github", "gists")
-    GITHUB_TEAMS = ("github", "teams")
-    GITHUB_PULLS = ("github", "pulls")
+    GITHUB_CODESPACES = ("github", "codespaces")
+    GITHUB_APPS = ("github", "apps")
     GITHUB_SECURITY_ADVISORIES = ("github", "security-advisories")
-    GITHUB_ISSUES = ("github", "issues")
-    GITHUB_INTERACTIONS = ("github", "interactions")
+    GITHUB_DEPENDENCY_GRAPH = ("github", "dependency-graph")
+    GITHUB_META = ("github", "meta")
     GITHUB_LICENSES = ("github", "licenses")
-    GITHUB_MARKDOWN = ("github", "markdown")
-    GITHUB_BILLING = ("github", "billing")
     GITHUB_REPOS = ("github", "repos")
-    GITHUB_ACTIVITY = ("github", "activity")
     GITHUB_ACTIONS = ("github", "actions")
-    GITHUB_CODE = ("github", "code")
-    GITHUB_CODE_SCANNING = ("github", "code-scanning")
-    GITHUB_CODESPACES = ("github", "codespaces")
-    GITHUB_DEPENDENCY_GRAPH = ("github", "dependency-graph")
-    GITHUB_CODES_OF_CONDUCT = ("github", "codes-of-conduct")
-    GITHUB_USERS = ("github", "users")
-    GITHUB_OIDC = ("github", "oidc")
-    GITHUB_APPS = ("github", "apps")
+    GITHUB_PROJECTS = ("github", "projects")
     GITHUB_REACTIONS = ("github", "reactions")
-    GITHUB_SEARCH = ("github", "search")
+    GITHUB_CODES_OF_CONDUCT = ("github", "codes-of-conduct")
+    GITHUB_INTERACTIONS = ("github", "interactions")
     GITHUB_PACKAGES = ("github", "packages")
-    GITHUB_META = ("github", "meta")
-    GITHUB_EMOJIS = ("github", "emojis")
+    GITHUB_PULLS = ("github", "pulls")
+    GITHUB_RATE_LIMIT = ("github", "rate-limit")
+    GITHUB_TEAMS = ("github", "teams")
+    GITHUB_BILLING = ("github", "billing")
+    GITHUB_CLASSROOM = ("github", "classroom")
+    GITHUB_MIGRATIONS = ("github", "migrations")
+    GITHUB_MARKDOWN = ("github", "markdown")
+    GITHUB_GIT = ("github", "git")
+    GITHUB_SECRET_SCANNING = ("github", "secret-scanning")
+    GITHUB_CHECKS = ("github", "checks")
+    GITHUB_USERS = ("github", "users")
     GITHUB_IMPORTANT = ("github", "important")
-    GITHUB_GITIGNORE = ("github", "gitignore")
     GITHUB_DEPENDABOT = ("github", "dependabot")
-    LISTENNOTES_SEARCH_API = ("listennotes", "Search API")
-    LISTENNOTES_PODCASTER_API = ("listennotes", "Podcaster API")
+    GITHUB_ACTIVITY = ("github", "activity")
+    GITHUB_CODE_SCANNING = ("github", "code-scanning")
+    GITHUB_ISSUES = ("github", "issues")
+    GITHUB_OIDC = ("github", "oidc")
+    GITHUB_EMOJIS = ("github", "emojis")
+    GITHUB_ORGS = ("github", "orgs")
+    GITHUB_COPILOT = ("github", "copilot")
+    GITHUB_SEARCH = ("github", "search")
     LISTENNOTES_DIRECTORY_API = ("listennotes", "Directory API")
     LISTENNOTES_PLAYLIST_API = ("listennotes", "Playlist API")
+    LISTENNOTES_SEARCH_API = ("listennotes", "Search API")
+    LISTENNOTES_PODCASTER_API = ("listennotes", "Podcaster API")
     LISTENNOTES_INSIGHTS_API = ("listennotes", "Insights API")
     NASA_PROJECT = ("nasa", "Project")
     NASA_ORGANIZATION = ("nasa", "Organization")
     NASA_RESOURCE = ("nasa", "Resource")
     OKTA_USERTYPE = ("okta", "UserType")
-    OKTA_GROUPSCHEMA = ("okta", "GroupSchema")
-    OKTA_AUTHORIZATIONSERVER = ("okta", "AuthorizationServer")
-    OKTA_FEATURE = ("okta", "Feature")
-    OKTA_GROUP = ("okta", "Group")
-    OKTA_SESSION = ("okta", "Session")
     OKTA_INLINEHOOK = ("okta", "InlineHook")
-    OKTA_THREATINSIGHT = ("okta", "ThreatInsight")
-    OKTA_LOG = ("okta", "Log")
+    OKTA_GROUP = ("okta", "Group")
+    OKTA_LINKEDOBJECT = ("okta", "LinkedObject")
     OKTA_USERSCHEMA = ("okta", "UserSchema")
-    OKTA_IDENTITYPROVIDER = ("okta", "IdentityProvider")
-    OKTA_AUTHENTICATOR = ("okta", "Authenticator")
+    OKTA_AUTHORIZATIONSERVER = ("okta", "AuthorizationServer")
+    OKTA_USERFACTOR = ("okta", "UserFactor")
+    OKTA_BRAND = ("okta", "Brand")
     OKTA_USER = ("okta", "User")
-    OKTA_LINKEDOBJECT = ("okta", "LinkedObject")
-    OKTA_APPLICATION = ("okta", "Application")
-    OKTA_SUBSCRIPTION = ("okta", "Subscription")
     OKTA_TRUSTEDORIGIN = ("okta", "TrustedOrigin")
-    OKTA_ORG = ("okta", "Org")
+    OKTA_LOG = ("okta", "Log")
     OKTA_NETWORKZONE = ("okta", "NetworkZone")
+    OKTA_GROUPSCHEMA = ("okta", "GroupSchema")
+    OKTA_THREATINSIGHT = ("okta", "ThreatInsight")
+    OKTA_FEATURE = ("okta", "Feature")
+    OKTA_ORG = ("okta", "Org")
+    OKTA_SUBSCRIPTION = ("okta", "Subscription")
+    OKTA_APPLICATION = ("okta", "Application")
     OKTA_PROFILEMAPPING = ("okta", "ProfileMapping")
+    OKTA_SESSION = ("okta", "Session")
+    OKTA_POLICY = ("okta", "Policy")
+    OKTA_IDENTITYPROVIDER = ("okta", "IdentityProvider")
+    OKTA_EVENTHOOK = ("okta", "EventHook")
+    OKTA_AUTHENTICATOR = ("okta", "Authenticator")
     OKTA_DOMAIN = ("okta", "Domain")
-    OKTA_BRAND = ("okta", "Brand")
     OKTA_TEMPLATE = ("okta", "Template")
-    OKTA_EVENTHOOK = ("okta", "EventHook")
-    OKTA_POLICY = ("okta", "Policy")
-    OKTA_USERFACTOR = ("okta", "UserFactor")
     SLACK_TEAM_PROFILE = ("slack", "team.profile")
+    SLACK_BOTS = ("slack", "bots")
+    SLACK_OAUTH_V2 = ("slack", "oauth.v2")
+    SLACK_RTM = ("slack", "rtm")
+    SLACK_ADMIN_INVITEREQUESTS_APPROVED = ("slack", "admin.inviteRequests.approved")
+    SLACK_APPS = ("slack", "apps")
+    SLACK_ADMIN_TEAMS = ("slack", "admin.teams")
+    SLACK_APPS_PERMISSIONS = ("slack", "apps.permissions")
+    SLACK_ADMIN_APPS = ("slack", "admin.apps")
+    SLACK_ADMIN_TEAMS_SETTINGS = ("slack", "admin.teams.settings")
+    SLACK_CALLS_PARTICIPANTS = ("slack", "calls.participants")
+    SLACK_STARS = ("slack", "stars")
+    SLACK_ADMIN_CONVERSATIONS_RESTRICTACCESS = ("slack", "admin.conversations.restrictAccess")
+    SLACK_WORKFLOWS = ("slack", "workflows")
+    SLACK_ADMIN_USERGROUPS = ("slack", "admin.usergroups")
+    SLACK_ADMIN_CONVERSATIONS = ("slack", "admin.conversations")
+    SLACK_ADMIN_TEAMS_OWNERS = ("slack", "admin.teams.owners")
+    SLACK_CALLS = ("slack", "calls")
+    SLACK_FILES = ("slack", "files")
+    SLACK_REACTIONS = ("slack", "reactions")
     SLACK_APPS_PERMISSIONS_USERS = ("slack", "apps.permissions.users")
+    SLACK_ADMIN_USERS_SESSION = ("slack", "admin.users.session")
+    SLACK_APPS_PERMISSIONS_RESOURCES = ("slack", "apps.permissions.resources")
     SLACK_DND = ("slack", "dnd")
     SLACK_ADMIN_APPS_RESTRICTED = ("slack", "admin.apps.restricted")
-    SLACK_ADMIN_CONVERSATIONS_RESTRICTACCESS = ("slack", "admin.conversations.restrictAccess")
-    SLACK_ADMIN_TEAMS_OWNERS = ("slack", "admin.teams.owners")
-    SLACK_USERS_PROFILE = ("slack", "users.profile")
-    SLACK_ADMIN_CONVERSATIONS = ("slack", "admin.conversations")
-    SLACK_STARS = ("slack", "stars")
+    SLACK_CONVERSATIONS = ("slack", "conversations")
+    SLACK_EMOJI = ("slack", "emoji")
+    SLACK_ADMIN_INVITEREQUESTS = ("slack", "admin.inviteRequests")
     SLACK_USERGROUPS = ("slack", "usergroups")
-    SLACK_APPS_PERMISSIONS_SCOPES = ("slack", "apps.permissions.scopes")
-    SLACK_CALLS_PARTICIPANTS = ("slack", "calls.participants")
     SLACK_ADMIN_APPS_APPROVED = ("slack", "admin.apps.approved")
-    SLACK_CHAT_SCHEDULEDMESSAGES = ("slack", "chat.scheduledMessages")
-    SLACK_DIALOG = ("slack", "dialog")
-    SLACK_ADMIN_CONVERSATIONS_EKM = ("slack", "admin.conversations.ekm")
-    SLACK_ADMIN_APPS_REQUESTS = ("slack", "admin.apps.requests")
-    SLACK_CHAT = ("slack", "chat")
-    SLACK_ADMIN_EMOJI = ("slack", "admin.emoji")
-    SLACK_REMINDERS = ("slack", "reminders")
-    SLACK_BOTS = ("slack", "bots")
-    SLACK_ADMIN_INVITEREQUESTS = ("slack", "admin.inviteRequests")
     SLACK_TEAM = ("slack", "team")
-    SLACK_USERGROUPS_USERS = ("slack", "usergroups.users")
     SLACK_FILES_REMOTE = ("slack", "files.remote")
-    SLACK_VIEWS = ("slack", "views")
-    SLACK_CALLS = ("slack", "calls")
+    SLACK_ADMIN_APPS_REQUESTS = ("slack", "admin.apps.requests")
+    SLACK_DIALOG = ("slack", "dialog")
     SLACK_FILES_COMMENTS = ("slack", "files.comments")
-    SLACK_API = ("slack", "api")
-    SLACK_OAUTH = ("slack", "oauth")
+    SLACK_APPS_EVENT_AUTHORIZATIONS = ("slack", "apps.event.authorizations")
     SLACK_ADMIN = ("slack", "admin")
+    SLACK_CHAT_SCHEDULEDMESSAGES = ("slack", "chat.scheduledMessages")
     SLACK_USERS = ("slack", "users")
-    SLACK_CONVERSATIONS = ("slack", "conversations")
-    SLACK_APPS = ("slack", "apps")
-    SLACK_ADMIN_INVITEREQUESTS_APPROVED = ("slack", "admin.inviteRequests.approved")
-    SLACK_REACTIONS = ("slack", "reactions")
-    SLACK_SEARCH = ("slack", "search")
-    SLACK_FILES = ("slack", "files")
-    SLACK_APPS_PERMISSIONS_RESOURCES = ("slack", "apps.permissions.resources")
+    SLACK_VIEWS = ("slack", "views")
+    SLACK_IMPORTANT = ("slack", "important")
+    SLACK_CHAT = ("slack", "chat")
+    SLACK_OAUTH = ("slack", "oauth")
     SLACK_AUTH = ("slack", "auth")
-    SLACK_ADMIN_TEAMS_ADMINS = ("slack", "admin.teams.admins")
-    SLACK_ADMIN_USERGROUPS = ("slack", "admin.usergroups")
-    SLACK_PINS = ("slack", "pins")
     SLACK_ADMIN_USERS = ("slack", "admin.users")
-    SLACK_ADMIN_USERS_SESSION = ("slack", "admin.users.session")
-    SLACK_IMPORTANT = ("slack", "important")
-    SLACK_APPS_EVENT_AUTHORIZATIONS = ("slack", "apps.event.authorizations")
-    SLACK_EMOJI = ("slack", "emoji")
-    SLACK_ADMIN_TEAMS_SETTINGS = ("slack", "admin.teams.settings")
-    SLACK_APPS_PERMISSIONS = ("slack", "apps.permissions")
-    SLACK_ADMIN_TEAMS = ("slack", "admin.teams")
-    SLACK_MIGRATION = ("slack", "migration")
-    SLACK_RTM = ("slack", "rtm")
-    SLACK_ADMIN_APPS = ("slack", "admin.apps")
-    SLACK_OAUTH_V2 = ("slack", "oauth.v2")
-    SLACK_WORKFLOWS = ("slack", "workflows")
     SLACK_ADMIN_INVITEREQUESTS_DENIED = ("slack", "admin.inviteRequests.denied")
+    SLACK_USERGROUPS_USERS = ("slack", "usergroups.users")
+    SLACK_API = ("slack", "api")
+    SLACK_REMINDERS = ("slack", "reminders")
+    SLACK_ADMIN_EMOJI = ("slack", "admin.emoji")
+    SLACK_PINS = ("slack", "pins")
+    SLACK_MIGRATION = ("slack", "migration")
+    SLACK_ADMIN_CONVERSATIONS_EKM = ("slack", "admin.conversations.ekm")
+    SLACK_USERS_PROFILE = ("slack", "users.profile")
+    SLACK_ADMIN_TEAMS_ADMINS = ("slack", "admin.teams.admins")
+    SLACK_APPS_PERMISSIONS_SCOPES = ("slack", "apps.permissions.scopes")
+    SLACK_SEARCH = ("slack", "search")
     SLACKBOT_TEAM_PROFILE = ("slackbot", "team.profile")
+    SLACKBOT_BOTS = ("slackbot", "bots")
+    SLACKBOT_OAUTH_V2 = ("slackbot", "oauth.v2")
+    SLACKBOT_APPS = ("slackbot", "apps")
+    SLACKBOT_APPS_PERMISSIONS = ("slackbot", "apps.permissions")
+    SLACKBOT_CALLS_PARTICIPANTS = ("slackbot", "calls.participants")
+    SLACKBOT_STARS = ("slackbot", "stars")
+    SLACKBOT_WORKFLOWS = ("slackbot", "workflows")
+    SLACKBOT_CALLS = ("slackbot", "calls")
+    SLACKBOT_FILES = ("slackbot", "files")
+    SLACKBOT_REACTIONS = ("slackbot", "reactions")
     SLACKBOT_APPS_PERMISSIONS_USERS = ("slackbot", "apps.permissions.users")
+    SLACKBOT_APPS_PERMISSIONS_RESOURCES = ("slackbot", "apps.permissions.resources")
     SLACKBOT_DND = ("slackbot", "dnd")
-    SLACKBOT_USERS_PROFILE = ("slackbot", "users.profile")
-    SLACKBOT_STARS = ("slackbot", "stars")
+    SLACKBOT_EMOJI = ("slackbot", "emoji")
+    SLACKBOT_CONVERSATIONS = ("slackbot", "conversations")
     SLACKBOT_USERGROUPS = ("slackbot", "usergroups")
-    SLACKBOT_APPS_PERMISSIONS_SCOPES = ("slackbot", "apps.permissions.scopes")
-    SLACKBOT_CALLS_PARTICIPANTS = ("slackbot", "calls.participants")
-    SLACKBOT_CHAT_SCHEDULEDMESSAGES = ("slackbot", "chat.scheduledMessages")
-    SLACKBOT_DIALOG = ("slackbot", "dialog")
-    SLACKBOT_CHAT = ("slackbot", "chat")
-    SLACKBOT_REMINDERS = ("slackbot", "reminders")
-    SLACKBOT_BOTS = ("slackbot", "bots")
     SLACKBOT_TEAM = ("slackbot", "team")
-    SLACKBOT_USERGROUPS_USERS = ("slackbot", "usergroups.users")
     SLACKBOT_FILES_REMOTE = ("slackbot", "files.remote")
-    SLACKBOT_VIEWS = ("slackbot", "views")
-    SLACKBOT_CALLS = ("slackbot", "calls")
     SLACKBOT_FILES_COMMENTS = ("slackbot", "files.comments")
-    SLACKBOT_API = ("slackbot", "api")
-    SLACKBOT_OAUTH = ("slackbot", "oauth")
+    SLACKBOT_DIALOG = ("slackbot", "dialog")
+    SLACKBOT_APPS_EVENT_AUTHORIZATIONS = ("slackbot", "apps.event.authorizations")
     SLACKBOT_USERS = ("slackbot", "users")
-    SLACKBOT_CONVERSATIONS = ("slackbot", "conversations")
-    SLACKBOT_APPS = ("slackbot", "apps")
-    SLACKBOT_REACTIONS = ("slackbot", "reactions")
-    SLACKBOT_FILES = ("slackbot", "files")
+    SLACKBOT_VIEWS = ("slackbot", "views")
+    SLACKBOT_IMPORTANT = ("slackbot", "important")
+    SLACKBOT_CHAT = ("slackbot", "chat")
+    SLACKBOT_OAUTH = ("slackbot", "oauth")
     SLACKBOT_AUTH = ("slackbot", "auth")
-    SLACKBOT_APPS_PERMISSIONS_RESOURCES = ("slackbot", "apps.permissions.resources")
+    SLACKBOT_USERGROUPS_USERS = ("slackbot", "usergroups.users")
+    SLACKBOT_API = ("slackbot", "api")
+    SLACKBOT_REMINDERS = ("slackbot", "reminders")
     SLACKBOT_PINS = ("slackbot", "pins")
-    SLACKBOT_IMPORTANT = ("slackbot", "important")
-    SLACKBOT_APPS_EVENT_AUTHORIZATIONS = ("slackbot", "apps.event.authorizations")
-    SLACKBOT_EMOJI = ("slackbot", "emoji")
     SLACKBOT_MIGRATION = ("slackbot", "migration")
-    SLACKBOT_APPS_PERMISSIONS = ("slackbot", "apps.permissions")
     SLACKBOT_RTM = ("slackbot", "rtm")
-    SLACKBOT_OAUTH_V2 = ("slackbot", "oauth.v2")
-    SLACKBOT_WORKFLOWS = ("slackbot", "workflows")
-    SPOTIFY_TRACKS = ("spotify", "Tracks")
-    SPOTIFY_CATEGORIES = ("spotify", "Categories")
-    SPOTIFY_EPISODES = ("spotify", "Episodes")
-    SPOTIFY_USERS = ("spotify", "Users")
-    SPOTIFY_PLAYER = ("spotify", "Player")
-    SPOTIFY_SEARCH = ("spotify", "Search")
-    SPOTIFY_AUDIOBOOKS = ("spotify", "Audiobooks")
+    SLACKBOT_USERS_PROFILE = ("slackbot", "users.profile")
+    SLACKBOT_CHAT_SCHEDULEDMESSAGES = ("slackbot", "chat.scheduledMessages")
+    SLACKBOT_APPS_PERMISSIONS_SCOPES = ("slackbot", "apps.permissions.scopes")
+    SPOTIFY_GENRES = ("spotify", "Genres")
     SPOTIFY_MARKETS = ("spotify", "Markets")
-    SPOTIFY_CHAPTERS = ("spotify", "Chapters")
+    SPOTIFY_USERS = ("spotify", "Users")
     SPOTIFY_ARTISTS = ("spotify", "Artists")
-    SPOTIFY_LIBRARY = ("spotify", "Library")
+    SPOTIFY_AUDIOBOOKS = ("spotify", "Audiobooks")
     SPOTIFY_ALBUMS = ("spotify", "Albums")
-    SPOTIFY_SHOWS = ("spotify", "Shows")
-    SPOTIFY_GENRES = ("spotify", "Genres")
+    SPOTIFY_TRACKS = ("spotify", "Tracks")
+    SPOTIFY_CHAPTERS = ("spotify", "Chapters")
+    SPOTIFY_SEARCH = ("spotify", "Search")
     SPOTIFY_PLAYLISTS = ("spotify", "Playlists")
+    SPOTIFY_PLAYER = ("spotify", "Player")
+    SPOTIFY_EPISODES = ("spotify", "Episodes")
+    SPOTIFY_CATEGORIES = ("spotify", "Categories")
+    SPOTIFY_SHOWS = ("spotify", "Shows")
+    SPOTIFY_LIBRARY = ("spotify", "Library")
     TASKADE_FOLDER = ("taskade", "Folder")
     TASKADE_ME = ("taskade", "Me")
-    TASKADE_WORKSPACE = ("taskade", "Workspace")
     TASKADE_TASK = ("taskade", "Task")
-    TASKADE_AGENT = ("taskade", "Agent")
+    TASKADE_WORKSPACE = ("taskade", "Workspace")
     TASKADE_PROJECT = ("taskade", "Project")
-    WHATSAPP_GROUPS = ("whatsapp", "Groups")
+    TASKADE_AGENT = ("taskade", "Agent")
+    WHATSAPP_HEALTH = ("whatsapp", "Health")
     WHATSAPP_BUSINESS_PROFILE = ("whatsapp", "Business Profile")
     WHATSAPP_USERS = ("whatsapp", "Users")
-    WHATSAPP_HEALTH = ("whatsapp", "Health")
-    WHATSAPP_MESSAGES = ("whatsapp", "Messages")
+    WHATSAPP_CERTIFICATES = ("whatsapp", "Certificates")
+    WHATSAPP_CONTACTS = ("whatsapp", "Contacts")
+    WHATSAPP_PROFILE = ("whatsapp", "Profile")
     WHATSAPP_APPLICATION = ("whatsapp", "Application")
-    WHATSAPP_REGISTRATION = ("whatsapp", "Registration")
+    WHATSAPP_GROUPS = ("whatsapp", "Groups")
     WHATSAPP_BACKUP_RESTORE = ("whatsapp", "Backup/Restore")
-    WHATSAPP_PROFILE = ("whatsapp", "Profile")
-    WHATSAPP_CONTACTS = ("whatsapp", "Contacts")
-    WHATSAPP_CERTIFICATES = ("whatsapp", "Certificates")
-    WHATSAPP_TWO_STEP_VERIFICATION = ("whatsapp", "Two-Step Verification")
+    WHATSAPP_REGISTRATION = ("whatsapp", "Registration")
     WHATSAPP_MEDIA = ("whatsapp", "Media")
-    ZOOM_PAC = ("zoom", "PAC")
-    ZOOM_DEVICES = ("zoom", "Devices")
-    ZOOM_MEETINGS = ("zoom", "Meetings")
+    WHATSAPP_MESSAGES = ("whatsapp", "Messages")
+    WHATSAPP_TWO_STEP_VERIFICATION = ("whatsapp", "Two-Step Verification")
+    ZOOM_WEBINARS = ("zoom", "Webinars")
     ZOOM_REPORTS = ("zoom", "Reports")
-    ZOOM_TRACKING_FIELD = ("zoom", "Tracking Field")
+    ZOOM_SIP_PHONE = ("zoom", "SIP Phone")
     ZOOM_TSP = ("zoom", "TSP")
-    ZOOM_H323_DEVICES = ("zoom", "H323 Devices")
     ZOOM_ARCHIVING = ("zoom", "Archiving")
-    ZOOM_WEBINARS = ("zoom", "Webinars")
-    ZOOM_SIP_PHONE = ("zoom", "SIP Phone")
+    ZOOM_MEETINGS = ("zoom", "Meetings")
+    ZOOM_DEVICES = ("zoom", "Devices")
+    ZOOM_H323_DEVICES = ("zoom", "H323 Devices")
     ZOOM_CLOUD_RECORDING = ("zoom", "Cloud Recording")
+    ZOOM_PAC = ("zoom", "PAC")
+    ZOOM_TRACKING_FIELD = ("zoom", "Tracking Field")
 
 
 
 
 class App(str, Enum):
     """Composio App."""
 
     @property
     def is_local(self) -> bool:
         """If the app is local."""
-        return self.value.lower() in ["mathematical", "localworkspace", "cmdmanagertool", "historykeeper"]
+        return self.value.lower() in ["mathematical", "localworkspace", "cmdmanagertool", "historykeeper", "ragtool", "webtool", "greptile"]
 
     ABLY = "ably"
     ACCELO = "accelo"
     ACTIVE_COMPAIGN = "active-compaign"
     ADOBE = "adobe"
     AERO_WORKFLOW = "aero-workflow"
     ALCHEMY = "alchemy"
@@ -464,15 +464,14 @@
     JIRA = "jira"
     KEAP = "keap"
     KLAVIYO = "klaviyo"
     KLIPFOLIO = "klipfolio"
     LASTPASS = "lastpass"
     LAUNCH_DARKLY = "launch-darkly"
     LEVER = "lever"
-    LEVER_SANDBOX = "lever-sandbox"
     LEXOFFICE = "lexoffice"
     LINEAR = "linear"
     LINKHUT = "linkhut"
     LISTENNOTES = "listennotes"
     MAILCHIMP = "mailchimp"
     MAINTAINX = "maintainx"
     MBOUM = "mboum"
@@ -566,14 +565,17 @@
     ZOHO_INVOICE = "zoho-invoice"
     ZOHO_MAIL = "zoho-mail"
     ZOOM = "zoom"
     MATHEMATICAL = "mathematical"
     LOCALWORKSPACE = "localworkspace"
     CMDMANAGERTOOL = "cmdmanagertool"
     HISTORYKEEPER = "historykeeper"
+    RAGTOOL = "ragtool"
+    WEBTOOL = "webtool"
+    GREPTILE = "greptile"
 
 
 
 class Action(tuple, Enum):
     """App action."""
 
     @property
@@ -3534,30 +3536,33 @@
     ZOOM_WEB_IN_ARS_UPDATE_STATUS = ("zoom", "zoom_web_in_ars_update_status", False)
     ZOOM_WEB_IN_ARS_GET_SURVEY = ("zoom", "zoom_web_in_ars_get_survey", False)
     ZOOM_WEB_IN_ARS_DELETE_SURVEY = ("zoom", "zoom_web_in_ars_delete_survey", False)
     ZOOM_WEB_IN_ARS_UPDATE_SURVEY = ("zoom", "zoom_web_in_ars_update_survey", False)
     ZOOM_WEB_IN_ARS_GET_WEB_IN_ART_OKEN = ("zoom", "zoom_web_in_ars_get_web_in_art_oken", False)
     ZOOM_WEB_IN_ARS_LIST_TRACKING_SOURCES = ("zoom", "zoom_web_in_ars_list_tracking_sources", False)
     CALCULATOR = ("mathematical", "mathematical_calculator", True, True)
-    WORKSPACESTATUS = ("localworkspace", "localworkspace_workspacestatus", True, True)
-    SETUPWORKSPACE = ("localworkspace", "localworkspace_setupworkspace", True, True)
-    SETUPGITHUBREPO = ("localworkspace", "localworkspace_setupgithubrepo", True, True)
+    WORKSPACESTATUSACTION = ("localworkspace", "localworkspace_workspacestatusaction", True, True)
     CREATEWORKSPACEACTION = ("localworkspace", "localworkspace_createworkspaceaction", True, True)
     FINDFILECMD = ("cmdmanagertool", "cmdmanagertool_findfilecmd", True, True)
     CREATEFILECMD = ("cmdmanagertool", "cmdmanagertool_createfilecmd", True, True)
     GOTOLINENUMINOPENFILE = ("cmdmanagertool", "cmdmanagertool_gotolinenuminopenfile", True, True)
     OPENFILE = ("cmdmanagertool", "cmdmanagertool_openfile", True, True)
-    SCROLLUP = ("cmdmanagertool", "cmdmanagertool_scrollup", True, True)
-    SCROLLDOWN = ("cmdmanagertool", "cmdmanagertool_scrolldown", True, True)
+    SCROLL = ("cmdmanagertool", "cmdmanagertool_scroll", True, True)
     SEARCHFILECMD = ("cmdmanagertool", "cmdmanagertool_searchfilecmd", True, True)
     SEARCHDIRCMD = ("cmdmanagertool", "cmdmanagertool_searchdircmd", True, True)
-    SETCURSORS = ("cmdmanagertool", "cmdmanagertool_setcursors", True, True)
     EDITFILE = ("cmdmanagertool", "cmdmanagertool_editfile", True, True)
     RUNCOMMANDONWORKSPACE = ("cmdmanagertool", "cmdmanagertool_runcommandonworkspace", True, True)
+    GETCURRENTDIRCMD = ("cmdmanagertool", "cmdmanagertool_getcurrentdircmd", True, True)
+    GITHUBCLONECMD = ("cmdmanagertool", "cmdmanagertool_githubclonecmd", True, True)
     GETWORKSPACEHISTORY = ("historykeeper", "historykeeper_getworkspacehistory", True, True)
+    RAGTOOLQUERY = ("ragtool", "ragtool_ragtoolquery", True, True)
+    ADDCONTENTTORAGTOOL = ("ragtool", "ragtool_addcontenttoragtool", True, True)
+    SCRAPEWEBSITECONTENT = ("webtool", "webtool_scrapewebsitecontent", True, True)
+    SCRAPEWEBSITEELEMENT = ("webtool", "webtool_scrapewebsiteelement", True, True)
+    CODEQUERY = ("greptile", "greptile_codequery", True, True)
 
 
 
 class Trigger(tuple, Enum):
     """App trigger."""
 
     @property
```

### Comparing `composio_core-0.3.3/composio/client/exceptions.py` & `composio_core-0.3.4/composio/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/client/http.py` & `composio_core-0.3.4/composio/client/http.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/client/local_handler.py` & `composio_core-0.3.4/composio/client/local_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from composio.local_tools.local_workspace.cmd_manager.cmd_manager_tool import (
+from composio.local_tools.local_workspace.cmd_manager.tool import (
     CmdManagerTool,
 )
 from composio.local_tools.local_workspace.commons.history_processor import (
     HistoryProcessor,
 )
 from composio.local_tools.local_workspace.commons.local_docker_workspace import (
     WorkspaceManagerFactory,
 )
-from composio.local_tools.local_workspace.history_keeper.history_keeper_tool import (
+from composio.local_tools.local_workspace.history_keeper import (
     HistoryKeeper,
 )
-from composio.local_tools.local_workspace.workspace.workspace_tool import LocalWorkspace
+from composio.local_tools.local_workspace.workspace import LocalWorkspace
 
-from ..local_tools import Mathematical
+from composio.local_tools.ragtool import RagTool
+from composio.local_tools import Mathematical
+from composio.local_tools.webtool import WebTool
+from composio.local_tools.greptile.tool import Greptile
 
 
 class LocalToolHandler:
     def __init__(self):
         self.registered_tools = self.register_local_tools()
         self.tool_map = {tool.tool_name: tool for tool in self.registered_tools}
 
@@ -36,14 +39,17 @@
         h_keeper_tool.set_workspace_factory(w)
         h_keeper_tool.set_history_processor(h)
         return [
             Mathematical(),
             workspace_tool,
             cmd_manager_tool,
             h_keeper_tool,
+            RagTool(),
+            WebTool(),
+            Greptile(),
         ]
 
     def get_list_of_action_schemas(self, apps=[], actions=[], tags=[]):
         tag_values = [tag if isinstance(tag, str) else tag.value for tag in tags]
 
         all_action_objs = []
```

### Comparing `composio_core-0.3.3/composio/constants.py` & `composio_core-0.3.4/composio/constants.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/exceptions.py` & `composio_core-0.3.4/composio/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/local_tools/file/tool.py` & `composio_core-0.3.4/composio/local_tools/file/actions/write_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,11 @@
-"""
-File I/O tool for Composio.
-"""
-
 import typing as t
 from pathlib import Path
-
 from pydantic import BaseModel, Field
-
-
-class Action:
-    """Local action abstraction."""
-
-
-class Tool:
-    """Local tool abstraction."""
-
+from composio.core.local import Action
 
 class WriteFileRequest(BaseModel):
     """Safe file request schema."""
 
     base_dir: str = Field(
         default=".",
         description="Directory where the file will be saved.",
@@ -32,67 +19,32 @@
         description="File name to be saved.",
     )
     overwrite: bool = Field(
         ...,
         description="Whether to overwrite a file if it exists or not.",
     )
 
-
 class WriteFileResponse(BaseModel):
     """Save file response schema."""
 
     filename: str = Field(
         ...,
         description="Path of the saved file.",
     )
 
-
-class ReadFileRequest(BaseModel):
-    """Read file request schema."""
-
-    base_dir: str = Field(
-        default=".",
-        description="Directory where the file will be saved.",
-    )
-    filename: str = Field(
-        ...,
-        description="File name to be saved.",
-    )
-
-
-class ReadFileResponse(BaseModel):
-    """Read file response schema."""
-
-    contents: str = Field(
-        ...,
-        description="Content read from the file.",
-    )
-
-
-class ReadFile(Action):
-    """Read file tool."""
-
-    def read_file(self, request: ReadFileRequest) -> ReadFileResponse:
-        """
-        Reads the contents of the file `file_name` and returns the contents
-        if successful.
-        """
-        try:
-            return ReadFileResponse(
-                contents=Path(request.base_dir, request.filename).read_text(
-                    encoding="utf-8"
-                )
-            )
-        except Exception as e:  # pylint: disable=broad-exception-caught
-            return ReadFileResponse(contents=f"Error reading file: {e}")
-
-
 class WriteFile(Action):
     """Write file tool."""
 
+    _display_name = "Write file"
+    _description = "Write file to a file."
+    _request = WriteFileRequest
+    _response = WriteFileResponse
+    _tags = ["file", "write"]
+    _tool_name = "file"
+
     def execute(self, request: WriteFileRequest) -> WriteFileResponse:
         """
         Saves the contents to a file called `file_name` and returns the
         file name if successful.
         """
         try:
             file = Path(request.base_dir, request.filename)
@@ -100,15 +52,7 @@
                 file.parent.mkdir(parents=True)
             if file.exists() and not request.overwrite:
                 return WriteFileResponse(filename=f"File {file} already exists")
             file.write_text(request.contents, encoding="utf-8")
             return WriteFileResponse(filename=str(file))
         except Exception as e:  # pylint: disable=broad-exception-caught
             return WriteFileResponse(filename=f"Error saving to file: {e}")
-
-
-class FileTool(Tool):
-    """File I/O tool."""
-
-    def actions(self) -> t.List[t.Type[Action]]:
-        """Return the list of actions."""
-        return [ReadFile, WriteFile]
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,181 +1,189 @@
-from pydantic import BaseModel, Field
+from pydantic import Field
 
-from composio.local_tools.action import Action
 from composio.local_tools.local_workspace.commons.get_logger import get_logger
 from composio.local_tools.local_workspace.commons.history_processor import (
-    HistoryProcessor,
     history_recorder,
 )
 from composio.local_tools.local_workspace.commons.local_docker_workspace import (
-    KEY_CONTAINER_NAME,
-    KEY_IMAGE_NAME,
-    KEY_PARENT_PIDS,
-    KEY_WORKSPACE_MANAGER,
-    WorkspaceManagerFactory,
     communicate,
-    get_container_process,
-    get_workspace_meta_from_manager,
-)
-from composio.local_tools.local_workspace.commons.utils import (
-    get_container_by_container_name,
 )
+from composio.local_tools.local_workspace.commons.utils import process_output
 
-from .const import SCRIPT_CURSOR_DEFAULT
+from .base_class import BaseAction, BaseRequest, BaseResponse
+from .const import SCRIPT_SEARCH
 
 
 logger = get_logger()
 
 
-class ScrollDownRequest(BaseModel):
-    workspace_id: str = Field(
-        ..., description="workspace-id to get the running workspace-manager"
+class SearchDirRequest(BaseRequest):
+    search_term: str = Field(..., description="search term to search in the directory")
+    directory: str = Field(
+        default=".",
+        description="The directory to search in (if not provided, searches in the current directory)",
     )
 
 
-class ScrollDownResponse(BaseModel):
-    output: str = Field(..., description="output of the command")
-    return_code: int = Field(..., description="return code for the command")
-
-
-class ScrollDown(Action):
-    """
-    Moves the window down 100 lines.
-    """
-
-    _display_name = "Scroll down command on workspace"
-    _request_schema = ScrollDownRequest  # Reusing the request schema from SetCursors
-    _response_schema = ScrollDownResponse  # Reusing the response schema from SetCursors
-    _tags = ["workspace"]
-    _tool_name = "cmdmanagertool"
-    script_file = SCRIPT_CURSOR_DEFAULT
-    command = "scroll_down"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
-
-    def __init__(self):
-        super().__init__()
-        self.logger = logger
-        self.args = None
-        self.workspace_id = ""
-        self.image_name = ""
-        self.container_name = ""
-        self.container_process = None
-        self.parent_pids = []
-        self.container_obj = None
-
-    def set_workspace_and_history(
-        self,
-        workspace_factory: WorkspaceManagerFactory,
-        history_processor: HistoryProcessor,
-    ):
-        self.workspace_factory = workspace_factory
-        self.history_processor = history_processor
-
-    def _setup(self, args: ScrollDownRequest):
-        self.args = args
-        self.workspace_id = args.workspace_id
-        workspace_meta = get_workspace_meta_from_manager(
-            self.workspace_factory, self.workspace_id
-        )
-        self.image_name = workspace_meta[KEY_IMAGE_NAME]
-        self.container_name = workspace_meta[KEY_CONTAINER_NAME]
-        self.container_process = get_container_process(
-            workspace_meta[KEY_WORKSPACE_MANAGER]
-        )
-        self.parent_pids = workspace_meta[KEY_PARENT_PIDS]
-        self.container_obj = get_container_by_container_name(
-            self.container_name, self.image_name
-        )
-        if not self.container_obj:
-            raise ValueError(
-                f"container-name {self.container_name} is not a valid docker-container"
-            )
-        self.logger = logger
+class SearchDirResponse(BaseResponse):
+    pass
+
+
+class SearchDirCmd(BaseAction):
+    """
+    Searches for search_term in all files in dir. If dir is not provided, searches in the current directory.
+    """
+
+    _display_name = "Search Directory Action"
+    _request_schema = SearchDirRequest
+    _response_schema = SearchDirResponse
 
     @history_recorder()
     def execute(
-        self, request_data: ScrollDownRequest, authorisation_data: dict
-    ) -> ScrollDownResponse:
+        self, request_data: SearchDirRequest, authorisation_data: dict
+    ) -> SearchDirResponse:
+        if not request_data.directory or not request_data.directory.strip():
+            raise ValueError(
+                "dir can not be null. Give a directory-name in which to search"
+            )
         self._setup(request_data)
-        command = f"{self.command}"  # Command to scroll down 100 lines
-        full_command = f"source {self.script_file} && {command}"
+        self.script_file = SCRIPT_SEARCH
+        self.command = "search_dir"
+        if self.container_process is None:
+            raise ValueError("Container process is not set")
+        full_command = f"{self.command} '{request_data.search_term}' {request_data.directory}"  # Command to scroll down 100 lines
+        print(f"Running command: {full_command}")
         output, return_code = communicate(
             self.container_process, self.container_obj, full_command, self.parent_pids
         )
-        return ScrollDownResponse(output=output, return_code=return_code)
+        output, return_code = process_output(output, return_code)
+        return SearchDirResponse(output=output, return_code=return_code)
+
 
+class SearchFileRequest(BaseRequest):
+    search_term: str = Field(..., description="search term to search in the file")
+    file_name: str = Field(
+        ..., description="name of the file in which search needs to be done"
+    )
 
-class ScrollUpRequest(BaseModel):
-    workspace_id: str = Field(..., description="moves the window up 100 lines")
 
+class SearchFileResponse(BaseResponse):
+    pass
 
-class ScrollUpResponse(BaseModel):
-    output: str = Field(..., description="output of the command")
-    return_code: int = Field(..., description="return code for the command")
-
-
-class ScrollUp(Action):
-    """
-    Moves the window up 100 lines.
-    """
-
-    _display_name = "Scroll up command on workspace"
-    _request_schema = ScrollUpRequest  # Reusing the request schema from SetCursors
-    _response_schema = ScrollUpResponse  # Reusing the response schema from SetCursors
-    _tags = ["workspace"]
-    _tool_name = "cmdmanagertool"
-    script_file = SCRIPT_CURSOR_DEFAULT
-    command = "scroll_up"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
-
-    def __init__(self):
-        super().__init__()
-        self.logger = logger
-        self.args = None
-        self.workspace_id = ""
-        self.image_name = ""
-        self.container_name = ""
-        self.container_process = None
-        self.parent_pids = []
-        self.container_obj = None
-
-    def set_workspace_and_history(
-        self,
-        workspace_factory: WorkspaceManagerFactory,
-        history_processor: HistoryProcessor,
-    ):
-        self.workspace_factory = workspace_factory
-        self.history_processor = history_processor
-
-    def _setup(self, args: ScrollDownRequest):
-        self.args = args
-        self.workspace_id = args.workspace_id
-        workspace_meta = get_workspace_meta_from_manager(
-            self.workspace_factory, self.workspace_id
-        )
-        self.image_name = workspace_meta[KEY_IMAGE_NAME]
-        self.container_name = workspace_meta[KEY_CONTAINER_NAME]
-        self.container_process = get_container_process(
-            workspace_meta[KEY_WORKSPACE_MANAGER]
+
+class SearchFileCmd(BaseAction):
+    """
+    Searches for a specified term within a specified file or the current open file if none is specified.
+    """
+
+    _display_name = "Search file Action"
+    _request_schema = SearchFileRequest
+    _response_schema = SearchFileResponse
+
+    @history_recorder()
+    def execute(
+        self, request_data: SearchFileRequest, authorisation_data: dict
+    ) -> SearchFileResponse:
+        if not request_data.file_name or not request_data.file_name.strip():
+            raise ValueError(
+                "file-name can not be null. Give a file-name in which to search"
+            )
+        self._setup(request_data)
+        self.script_file = SCRIPT_SEARCH
+        self.command = "search_file"
+        if self.container_process is None:
+            raise ValueError("Container process is not set")
+        full_command = (
+            f"{self.command} '{request_data.search_term}' {request_data.file_name}"
         )
-        self.parent_pids = workspace_meta[KEY_PARENT_PIDS]
-        self.container_obj = get_container_by_container_name(
-            self.container_name, self.image_name
+        print(f"Running command: {full_command}")
+        output, return_code = communicate(
+            self.container_process, self.container_obj, full_command, self.parent_pids
         )
-        if not self.container_obj:
+        output, return_code = process_output(output, return_code)
+        return SearchFileResponse(output=output, return_code=return_code)
+
+
+class FindFileRequest(BaseRequest):
+    file_name: str = Field(
+        ...,
+        description="The name of the file to be searched for within the specified directory or the current directory if none is specified.",
+    )
+    dir: str = Field(
+        default=".",
+        description="The directory within which to search for the file. If not provided, the search will default to the current directory.",
+    )
+
+
+class FindFileResponse(BaseResponse):
+    pass
+
+
+class FindFileCmd(BaseAction):
+    """
+    Searches for files by name within a specified directory or the current directory if none is specified.
+    Example:
+        - To find a file, provide the workspace ID, the file name, and optionally a directory.
+        - The response will list any files found and indicate whether the search was successful.
+    """
+
+    _display_name = "Find File Action"
+    _request_schema = FindFileRequest
+    _response_schema = FindFileResponse
+
+    @history_recorder()
+    def execute(
+        self, request_data: FindFileRequest, authorisation_data: dict
+    ) -> FindFileResponse:
+        if not request_data.file_name or not request_data.file_name.strip():
+            raise ValueError("file-name can not be null. Give a file-name to find")
+        if not request_data.dir or not request_data.dir.strip():
             raise ValueError(
-                f"container-name {self.container_name} is not a valid docker-container"
+                "directory in which file-name needs to be searched cant be empty. Give a directory name"
             )
+        self._setup(request_data)
+        self.script_file = SCRIPT_SEARCH
+        self.command = "find_file"
+        full_command = f"{self.command} {request_data.file_name} {request_data.dir}"
+        print(f"Running command: {full_command}")
+        if self.container_process is None:
+            raise ValueError("Container process is not set")
+        output, return_code = communicate(
+            self.container_process, self.container_obj, full_command, self.parent_pids
+        )
+        output, return_code = process_output(output, return_code)
+        return FindFileResponse(output=output, return_code=return_code)
+
+
+class GetCurrentDirRequest(BaseRequest):
+    pass
+
+
+class GetCurrentDirResponse(BaseResponse):
+    pass
+
+
+class GetCurrentDirCmd(BaseAction):
+    """
+    Gets the current directory.
+    """
+
+    _display_name = "Get Current Directory Action"
+    _request_schema = GetCurrentDirRequest
+    _response_schema = GetCurrentDirResponse
+    script_file = SCRIPT_SEARCH
+    command = "pwd"
 
     @history_recorder()
     def execute(
-        self, request_data: ScrollDownRequest, authorisation_data: dict
-    ) -> ScrollDownResponse:
+        self, request_data: GetCurrentDirRequest, authorisation_data: dict
+    ) -> GetCurrentDirResponse:
         self._setup(request_data)
-        command = f"{self.command}"  # Command to scroll down 100 lines
-        full_command = f"source {self.script_file} && {command}"
+        full_command = f"{self.command}"
+        print(f"Running command: {full_command}")
+        if self.container_process is None:
+            raise ValueError("Container process is not set")
         output, return_code = communicate(
             self.container_process, self.container_obj, full_command, self.parent_pids
         )
-        return ScrollDownResponse(output=output, return_code=return_code)
+        output, return_code = process_output(output, return_code)
+        return GetCurrentDirResponse(output=output, return_code=return_code)
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/commons/local_docker_workspace.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,287 +1,328 @@
-from pydantic import BaseModel, Field
+import datetime
+import hashlib
+import os
+import subprocess
+import time
+import typing as t
+from typing import Any, Dict, List, Optional, Tuple
+from uuid import uuid4
+
+import docker
+import gymnasium as gym
+from pydantic import BaseModel
 
-from composio.local_tools.action import Action
 from composio.local_tools.local_workspace.commons.get_logger import get_logger
-from composio.local_tools.local_workspace.commons.history_processor import (
-    HistoryProcessor,
-    history_recorder,
-)
-from composio.local_tools.local_workspace.commons.local_docker_workspace import (
-    KEY_CONTAINER_NAME,
-    KEY_IMAGE_NAME,
-    KEY_PARENT_PIDS,
-    KEY_WORKSPACE_MANAGER,
-    WorkspaceManagerFactory,
-    communicate,
-    get_container_process,
-    get_workspace_meta_from_manager,
-)
 from composio.local_tools.local_workspace.commons.utils import (
-    get_container_by_container_name,
+    communicate,
+    get_container,
+    process_output,
+    read_with_timeout,
 )
 
-from .const import SCRIPT_SEARCH
-
 
 logger = get_logger()
 
+COMMANDS_CONFIG_PATH = "../config/commands.yaml"
+TYPE_WORKSPACE_LOCAL_DOCKER = "local_docker"
 
-class SearchDirRequest(BaseModel):
-    workspace_id: str = Field(
-        ..., description="workspace-id to get the running workspace-manager"
-    )
-    search_term: str = Field(..., description="search term to search in the directory")
-    dir: str = Field(..., description="directory in which search needs to be done")
-
-
-class SearchDirResponse(BaseModel):
-    output: str = Field(..., description="output of the command")
-    return_code: int = Field(..., description="return code for the command")
-
-
-class SearchDirCmd(Action):
-    """
-    search the given term in the given directory
-    """
-
-    _display_name = "Scroll down command on workspace"
-    _request_schema = SearchDirRequest
-    _response_schema = SearchDirResponse
-    _tags = ["workspace"]
-    _tool_name = "cmdmanagertool"
-    script_file = SCRIPT_SEARCH
-    command = "search_dir"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
+KEY_WORKSPACE_MANAGER = "workspace"
+KEY_CONTAINER_NAME = "container_name"
+KEY_PARENT_PIDS = "parent_pids"
+KEY_IMAGE_NAME = "image_name"
+KEY_WORKSPACE_ID = "workspace_id"
 
-    def __init__(self):
-        super().__init__()
-        self.args = None
-        self.workspace_id = ""
-        self.image_name = ""
-        self.container_name = ""
-        self.container_process = None
-        self.parent_pids = []
-        self.container_obj = None
-        self.logger = logger
 
-    def set_workspace_and_history(
-        self,
-        workspace_factory: WorkspaceManagerFactory,
-        history_processor: HistoryProcessor,
-    ):
-        self.workspace_factory = workspace_factory
-        self.history_processor = history_processor
+class LocalDockerArgumentsModel(BaseModel):
+    image_name: str
+    timeout: int = 35
+    verbose: bool = False
+    environment_setup: Optional[str] = None
 
-    def _setup(self, args: SearchDirRequest):
-        self.args = args
-        self.workspace_id = args.workspace_id
-        workspace_meta = get_workspace_meta_from_manager(
-            self.workspace_factory, self.workspace_id
-        )
-        self.image_name = workspace_meta[KEY_IMAGE_NAME]
-        self.container_name = workspace_meta[KEY_CONTAINER_NAME]
-        self.container_process = get_container_process(
-            workspace_meta[KEY_WORKSPACE_MANAGER]
-        )
-        self.parent_pids = workspace_meta[KEY_PARENT_PIDS]
-        self.container_obj = get_container_by_container_name(
-            self.container_name, self.image_name
-        )
-        if not self.container_obj:
-            raise ValueError(
-                f"container-name {self.container_name} is not a valid docker-container"
-            )
-        self.logger = logger
-
-    @history_recorder()
-    def execute(
-        self, request_data: SearchDirRequest, authorisation_data: dict
-    ) -> SearchDirResponse:
-        if not request_data.dir or not request_data.dir.strip():
-            raise ValueError(
-                "dir can not be null. Give a directory-name in which to search"
-            )
-        self._setup(request_data)
-        command = f"{self.command} '{request_data.search_term}' {request_data.dir}"  # Command to scroll down 100 lines
-        full_command = f"source {self.script_file} && {command}"
-        output, return_code = communicate(
-            self.container_process, self.container_obj, full_command, self.parent_pids
-        )
-        return SearchDirResponse(output=output, return_code=return_code)
 
+class LocalDockerWorkspace(gym.Env):
+    """Gym environment for SWE-bench. This class should handle all communication with the docker container."""
 
-class SearchFileRequest(BaseModel):
-    workspace_id: str = Field(
-        ..., description="workspace-id to get the running workspace-manager"
-    )
-    search_term: str = Field(..., description="search term to search in the directory")
-    file_name: str = Field(
-        ..., description="name of the file in which search needs to be done"
-    )
-
-
-class SearchFileResponse(BaseModel):
-    output: str = Field(..., description="output of the command")
-    return_code: int = Field(..., description="return code for the command")
-
-
-class SearchFileCmd(Action):
-    """
-    searches for search_term in file. If file is not provided, searches in the current open file
-    """
-
-    _display_name = "Search term in file"
-    _request_schema = SearchFileRequest
-    _response_schema = SearchFileResponse
-    _tags = ["workspace"]
-    _tool_name = "cmdmanagertool"
-    script_file = SCRIPT_SEARCH
-    command = "search_file"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
+    name = "swe_main"
 
-    def __init__(self):
+    def __init__(self, args: LocalDockerArgumentsModel):
         super().__init__()
-        self.args = None
-        self.workspace_id = ""
-        self.image_name = ""
-        self.container_name = ""
-        self.container_process = None
-        self.parent_pids = []
-        self.container_obj = None
-        self.logger = logger
-
-    def set_workspace_and_history(
-        self,
-        workspace_factory: WorkspaceManagerFactory,
-        history_processor: HistoryProcessor,
-    ):
-        self.workspace_factory = workspace_factory
-        self.history_processor = history_processor
-
-    def _setup(self, args: SearchFileRequest):
         self.args = args
-        self.workspace_id = args.workspace_id
-        workspace_meta = get_workspace_meta_from_manager(
-            self.workspace_factory, self.workspace_id
-        )
-        self.image_name = workspace_meta[KEY_IMAGE_NAME]
-        self.container_name = workspace_meta[KEY_CONTAINER_NAME]
-        self.container_process = get_container_process(
-            workspace_meta[KEY_WORKSPACE_MANAGER]
-        )
-        self.parent_pids = workspace_meta[KEY_PARENT_PIDS]
-        self.container_obj = get_container_by_container_name(
-            self.container_name, self.image_name
-        )
-        if not self.container_obj:
-            raise ValueError(
-                f"container-name {self.container_name} is not a valid docker-container"
-            )
-
-    @history_recorder()
-    def execute(
-        self, request_data: SearchFileRequest, authorisation_data: dict
-    ) -> SearchDirResponse:
-        if not request_data.file_name or not request_data.file_name.strip():
-            raise ValueError(
-                "dir can not be null. Give a directory-name in which to search"
+        self.base_commit = None
+        self.communicate_output = None
+        # self.install_environment = args.install_environment
+        self.logger = logger
+        # self.persistent = args.container_name is not None
+        self.returncode = None
+        self.container_name: str = ""
+        self.container: t.Optional[subprocess.Popen] = None
+        self.container_obj = None
+        self.persistent = False
+        self.container_pid = None
+        self.parent_pids: t.Set[str] = set()
+        if not self.args.verbose:
+            self.logger.disabled = True
+
+        # Establish connection with execution container
+        self.image_name = args.image_name
+        self._reset_container()
+
+        # Set timeout
+        self.timeout = self.args.timeout
+        self.idx = 0
+        self.clean_multi_line_functions = lambda x: x
+        self.hooks: List[Any] = []
+
+    def _reset_container(self) -> None:
+        if hasattr(self, "container"):
+            try:
+                if self.container is None:
+                    raise ValueError("Container is None")
+                self.container.terminate()
+            except KeyboardInterrupt:
+                logger.error("handling keyboard interrupt")
+                raise
+            except Exception as e:
+                logger.error(f"reset container exception: {e}")
+        self._init_container()
+        self._init_scripts()
+
+    def _init_container(self) -> None:
+        """
+        Handles container initialization. Defines container name and creates it
+        """
+        if not self.container_name:
+            process_id = str(os.getpid())
+            current_time = str(datetime.datetime.now())
+            unique_string = current_time + process_id
+            hash_object = hashlib.sha256(unique_string.encode())
+            # Cannot have colons/slashes in container name, but those are important in image names
+            # i.e., when we want swe-agent to pull the image from dockerhub
+            image_name_sanitized = self.image_name.replace("/", "-")
+            image_name_sanitized = image_name_sanitized.replace(":", "-")
+            self.container_name = (
+                f"{image_name_sanitized}-{hash_object.hexdigest()[:10]}"
             )
-        self._setup(request_data)
-        command = (
-            f"{self.command} '{request_data.search_term}' {request_data.file_name}"
+        self.container, self.parent_pids = get_container(
+            self.container_name, self.image_name, persistent=self.persistent
         )
-        full_command = f"source {self.script_file} && {command}"
-        output, return_code = communicate(
-            self.container_process, self.container_obj, full_command, self.parent_pids
-        )
-        return SearchDirResponse(output=output, return_code=return_code)
-
+        self.container_pid = self.container.pid
 
-class FindFileRequest(BaseModel):
-    workspace_id: str = Field(
-        ..., description="workspace-id to get the running workspace-manager"
-    )
-    file_name: str = Field(..., description="file-name to search for")
-    dir: str = Field(
-        ..., description="name of the directory in which search needs to be done"
-    )
-
-
-class FindFileResponse(BaseModel):
-    output: str = Field(..., description="output of the command")
-    return_code: int = Field(..., description="return code for the command")
-
-
-class FindFileCmd(Action):
-    """
-    finds all files with the given name in dir.
-    """
-
-    _display_name = "finds file in directory"
-    _request_schema = FindFileRequest
-    _response_schema = FindFileResponse
-    _tags = ["workspace"]
-    _tool_name = "cmdmanagertool"
-    script_file = SCRIPT_SEARCH
-    command = "find_file"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
+        client = None
 
-    def __init__(self):
-        super().__init__()
-        self.args = None
-        self.workspace_id = ""
-        self.image_name = ""
-        self.container_name = ""
-        self.container_process = None
-        self.parent_pids = []
-        self.container_obj = None
-        self.logger = logger
-
-    def set_workspace_and_history(
-        self,
-        workspace_factory: WorkspaceManagerFactory,
-        history_processor: HistoryProcessor,
-    ):
-        self.workspace_factory = workspace_factory
-        self.history_processor = history_processor
-
-    def _setup(self, args: FindFileRequest):
-        self.args = args
-        self.workspace_id = args.workspace_id
-        workspace_meta = get_workspace_meta_from_manager(
-            self.workspace_factory, self.workspace_id
-        )
-        self.image_name = workspace_meta[KEY_IMAGE_NAME]
-        self.container_name = workspace_meta[KEY_CONTAINER_NAME]
-        self.container_process = get_container_process(
-            workspace_meta[KEY_WORKSPACE_MANAGER]
-        )
-        self.parent_pids = workspace_meta[KEY_PARENT_PIDS]
-        self.container_obj = get_container_by_container_name(
-            self.container_name, self.image_name
-        )
-        if not self.container_obj:
-            raise ValueError(
-                f"container-name {self.container_name} is not a valid docker-container"
+        try:
+            client = docker.from_env()
+            self.container_obj = client.containers.get(self.container_name)
+        except docker.errors.DockerException as e:
+            if "Error while fetching server API version" in str(e):
+                raise RuntimeError(
+                    "Docker is not running. Please start Docker and try again."
+                ) from e
+
+        except docker.errors.NotFound:
+            logger.debug("Couldn't find container. Let's wait and retry.")
+            time.sleep(3)
+            if client is not None:
+                self.container_obj = client.containers.get(self.container_name)
+            else:
+                raise ValueError("Client is None")
+
+        self.logger.info("🌱 Environment Initialized")
+
+    def _init_scripts(self):
+        """
+        Initialize custom commands within container
+        """
+        self.communicate_with_handling(
+            "source /root/.bashrc",
+            error_msg="Failed to source .bashrc",
+        )
+        self.communicate_with_handling(
+            "mkdir -p /root/commands",
+            error_msg="Failed to create commands directory",
+        )
+        self.communicate_with_handling(
+            "touch /root/commands/__init__.py",
+            error_msg="Failed to create __init__.py",
+        )
+        self.communicate_with_handling(
+            "export PATH=$PATH:/root/commands",
+            error_msg="Failed to add commands directory to PATH",
+        )
+
+    def reset_container(self):
+        pass
+
+    def communicate_with_handling(
+        self, input: str, error_msg: str, timeout_duration=25
+    ) -> str:
+        """
+        Wrapper for communicate function that raises error if return code is non-zero
+        """
+        if self.container is None:
+            raise ValueError("Container is None")
+
+        logs, self.returncode = communicate(
+            self.container,
+            self.container_obj,
+            input,
+            list(self.parent_pids),
+            timeout_duration=timeout_duration,
+        )
+        if self.returncode != 0:
+            self.logger.error(f"{error_msg}: {logs}")
+            self.close()
+            raise RuntimeError(f"{error_msg}: {logs}")
+        return logs
+
+    def communicate(self, input: str, timeout_duration=25) -> Tuple[str, int]:
+        if self.container is None:
+            raise ValueError("Container is None")
+        output, return_code = communicate(
+            self.container,
+            self.container_obj,
+            input,
+            list(self.parent_pids),
+            timeout_duration,
+        )
+        output, return_code = process_output(output, return_code)
+        return output, return_code
+
+    def interrupt(self):
+        """
+        Send interrupt signal to container and exhaust stdout buffer with a communicate call
+        """
+        pids = self.get_pids()
+        if self.container_obj is None:
+            raise ValueError("Container is None")
+        for pid, cmd in pids:
+            if pid not in self.parent_pids and cmd != "ps":
+                self.container_obj.exec_run(f"kill -9 {pid}")
+        try:
+            _ = read_with_timeout(
+                self.container, self.container_obj, self.get_pids, self.parent_pids, 20
             )
-
-    @history_recorder()
-    def execute(
-        self, request_data: FindFileRequest, authorisation_data: dict
-    ) -> FindFileResponse:
-        if not request_data.file_name or not request_data.file_name.strip():
-            raise ValueError("file-name can not be null. Give a file-name to find")
-        if not request_data.dir or not request_data.dir.strip():
-            raise ValueError(
-                "directory in which file-name needs to be searched cant be empty. Give a directory name"
+        except TimeoutError:
+            pass
+        try:
+            output, return_code = self.communicate(
+                input="echo 'interrupted'", timeout_duration=5
             )
-        self._setup(request_data)
-        command = f"{self.command} {request_data.file_name} {request_data.dir}"
-        full_command = f"source {self.script_file} && {command}"
-        output, return_code = communicate(
-            self.container_process, self.container_obj, full_command, self.parent_pids
-        )
-        return FindFileResponse(output=output, return_code=return_code)
+            assert output.strip().endswith(
+                "interrupted"
+            ), "container health check failed"
+        except TimeoutError as exc:
+            raise RuntimeError("Failed to interrupt container") from exc
+
+    def get_pids(self, all_pids=False) -> list[str]:
+        """
+        Gets list of processes running inside docker container
+        """
+        if self.container_obj is None:
+            raise ValueError("Container is None")
+
+        pids = (
+            self.container_obj.exec_run("ps -eo pid,comm --no-headers")
+            .output.decode()
+            .split("\n")
+        )
+        pids = [x.split() for x in pids if x]
+        if not all_pids:
+            pids = [x for x in pids if x[1] != "ps" and x[0] not in self.parent_pids]
+        return pids
+
+    def close(self):
+        """
+        Handle environment shutdown
+        """
+        self.logger.info("Beginning environment shutdown...")
+        try:
+            if self.container is None:
+                raise ValueError("Container is None")
+            communicate(
+                self.container,
+                self.container_obj,
+                "exit",
+                parent_pids=list(self.parent_pids),
+            )
+        except KeyboardInterrupt:
+            logger.error("handling keyboard interrupt")
+            raise
+        except Exception as e:
+            logger.error(f"docker close exception: {e}")
+        assert self.container is not None
+        assert self.container_obj is not None
+        self.container.terminate()
+        if self.persistent:
+            if self.container_obj.status not in {"paused", "exited"}:
+                self.container_obj.pause()
+                self.logger.info("Agent container paused")
+            else:
+                self.logger.info(f"Agent container status: {self.container_obj.status}")
+        else:
+            try:
+                self.container_obj.remove(force=True)
+            except KeyboardInterrupt:
+                logger.error("handling keyboard interrupt")
+                raise
+            except Exception as e:
+                logger.error(f"docker close exception: {e}")
+            self.logger.info("Agent container stopped")
+        # todo: implement these hooks
+        for hook in self.hooks:
+            hook.on_close()
+
+
+class WorkspaceManagerFactory:
+    _registry: Dict[str, Dict[str, Any]] = {}
+
+    def get_workspace_manager(self, args: LocalDockerArgumentsModel) -> str:
+        # currently we only support local docker
+        workspace_type = TYPE_WORKSPACE_LOCAL_DOCKER
+        if workspace_type == TYPE_WORKSPACE_LOCAL_DOCKER:
+            workspace_manager = LocalDockerWorkspace(args)
+            container_name = workspace_manager.container_name
+            parent_pids = workspace_manager.parent_pids
+            workspace_id = str(uuid4())
+            self._registry[workspace_id] = {
+                KEY_WORKSPACE_MANAGER: workspace_manager,
+                KEY_CONTAINER_NAME: container_name,
+                KEY_PARENT_PIDS: parent_pids,
+                KEY_IMAGE_NAME: args.image_name,
+            }
+            return workspace_id
+
+        raise ValueError(f"Unknown workspace manager type: {workspace_type}")
+
+    def get_registered_manager(self, workspace_id: str) -> Optional[Dict[str, Any]]:
+        return self._registry.get(workspace_id)
+
+    def remove_workspace_manager(self, workspace_id: str) -> None:
+        if workspace_id in WorkspaceManagerFactory._registry:
+            del self._registry[workspace_id]
+
+    def list_workspace_managers(self) -> Dict[str, Any]:
+        return self._registry
+
+
+def get_workspace_meta_from_manager(
+    workspace_factory: WorkspaceManagerFactory, workspace_id: str
+) -> dict:
+    workspace_meta = workspace_factory.get_registered_manager(workspace_id)
+    if workspace_meta is None:
+        raise ValueError(f"Workspace manager not found: {workspace_id}")
+    return workspace_meta
+
+
+def get_container_name_from_workspace_id(
+    workspace_factory: WorkspaceManagerFactory, workspace_id: str
+) -> str:
+    workspace_meta = workspace_factory.get_registered_manager(workspace_id)
+    if workspace_meta is None:
+        raise ValueError(f"Workspace manager not found: {workspace_id}")
+    return workspace_meta[KEY_CONTAINER_NAME]
+
+
+def get_container_process(workspace: LocalDockerWorkspace):
+    if not workspace or not workspace.container:
+        raise ValueError("workspace null, or not running any container process")
+    return workspace.container
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,99 @@
+from abc import ABC, abstractmethod
+from pathlib import Path
+from typing import Optional
+
 from pydantic import BaseModel, Field
 
-from composio.local_tools.action import Action
-from composio.local_tools.local_workspace.commons.get_logger import get_logger
-from composio.local_tools.local_workspace.commons.history_processor import (
+from composio.core.local import Action
+from composio.local_tools.local_workspace.commons import (
+    get_logger,
     HistoryProcessor,
-    history_recorder,
 )
 from composio.local_tools.local_workspace.commons.local_docker_workspace import (
     KEY_CONTAINER_NAME,
     KEY_IMAGE_NAME,
     KEY_PARENT_PIDS,
     KEY_WORKSPACE_MANAGER,
     WorkspaceManagerFactory,
-    communicate,
     get_container_process,
     get_workspace_meta_from_manager,
 )
 from composio.local_tools.local_workspace.commons.utils import (
     get_container_by_container_name,
 )
 
-from .const import SCRIPT_CURSOR_DEFAULT
-
 
 logger = get_logger()
+script_path = Path(__file__).resolve()
+script_dir = script_path.parent
+CONFIG_FILE_PATH = script_dir / Path("../../config/default.yaml")
 
 
-class SetCursorsRequest(BaseModel):
+class BaseRequest(BaseModel):
     workspace_id: str = Field(
         ..., description="workspace-id to get the running workspace-manager"
     )
-    start_line: int = Field(..., description="start line of the cursor")
-    end_line: int = Field(..., description="end line of the cursor")
 
 
-class SetCursorsResponse(BaseModel):
+class BaseResponse(BaseModel):
     output: str = Field(..., description="output of the command")
-    return_code: int = Field(..., description="return code for the command")
+    return_code: int = Field(
+        ..., description="Any output or errors that occurred during the file edit."
+    )
 
 
-class SetCursors(Action):
+class BaseAction(Action, ABC):
     """
-    Sets the start and end cursors based on the provided line numbers, with checks to ensure the file is open,
-    the arguments are numbers, and the start line is less than or equal to the end line.
-
-    Raises:
-    - ValueError: If start_line or end_line are not integers, or if start_line > end_line.
-    - RuntimeError: If no file is currently open.
+    Base class for all actions
     """
 
-    _display_name = "Run command on workspace"
-    _request_schema = SetCursorsRequest
-    _response_schema = SetCursorsResponse
+    _history_maintains = True
+    _display_name = ""
     _tags = ["workspace"]
     _tool_name = "cmdmanagertool"
-    script_file = SCRIPT_CURSOR_DEFAULT
-    command = "set_cursors"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
+    script_file = ""
+    command = ""
+    workspace_factory: Optional[WorkspaceManagerFactory] = None
+    history_processor: Optional[HistoryProcessor] = None
 
     def __init__(self):
         super().__init__()
+        self.name = "agent"
+        self.logger = logger
+        self.config_file_path = ""
         self.args = None
         self.workspace_id = ""
+        self.command = ""
         self.image_name = ""
         self.container_name = ""
         self.container_process = None
         self.parent_pids = []
         self.container_obj = None
         self.logger = logger
+        self.return_code = None
+        self.config = None
+        self.command_patterns = None
+        self.subroutine_patterns = None
 
     def set_workspace_and_history(
         self,
         workspace_factory: WorkspaceManagerFactory,
         history_processor: HistoryProcessor,
     ):
         self.workspace_factory = workspace_factory
         self.history_processor = history_processor
 
-    def _setup(self, args: SetCursorsRequest):
+    def _setup(self, args: BaseRequest):
         self.args = args
+        self.config_file_path = Path(CONFIG_FILE_PATH)
         self.workspace_id = args.workspace_id
-        self.start_line = args.start_line
-        self.end_line = args.end_line
+        if self.workspace_factory is None:
+            logger.error("workspace_factory is not set")
+            raise ValueError("workspace_factory is not set")
         workspace_meta = get_workspace_meta_from_manager(
             self.workspace_factory, self.workspace_id
         )
         self.image_name = workspace_meta[KEY_IMAGE_NAME]
         self.container_name = workspace_meta[KEY_CONTAINER_NAME]
         self.container_process = get_container_process(
             workspace_meta[KEY_WORKSPACE_MANAGER]
@@ -96,24 +103,17 @@
             self.container_name, self.image_name
         )
         if not self.container_obj:
             raise ValueError(
                 f"container-name {self.container_name} is not a valid docker-container"
             )
 
-    @history_recorder()
+    def validate_file_name(self, file_name):
+        if file_name is None or file_name.strip() == "":
+            return "Exception: file-name can not be empty", 1
+        return None, 0
+
+    @abstractmethod
     def execute(
-        self, request_data: SetCursorsRequest, authorisation_data: dict
-    ) -> SetCursorsResponse:
-        """Executes a shell script command inside the Docker container."""
-        self._setup(request_data)
-        command = (
-            f"{self.command} {' '.join([str(self.start_line), str(self.end_line)])}"
-        )
-        full_command = f"source {self.script_file} && {command}"
-        output, return_code = communicate(
-            self.container_process,
-            self.container_obj,
-            full_command,
-            self.parent_pids,
-        )
-        return SetCursorsResponse(output=output, return_code=return_code)
+        self, request_data: BaseRequest, authorisation_data: dict
+    ) -> BaseResponse:
+        pass
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/workspace/tool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,38 @@
-from composio.local_tools.local_workspace.cmd_manager.actions import (
-    CreateFileCmd,
-    EditFile,
-    FindFileCmd,
-    GoToLineNumInOpenFile,
-    OpenFile,
-    RunCommandOnWorkspace,
-    ScrollDown,
-    ScrollUp,
-    SearchDirCmd,
-    SearchFileCmd,
-    SetCursors,
-)
-from composio.local_tools.local_workspace.commons.history_processor import (
+import typing as t
+from composio.core.local import Tool, Action
+
+from composio.local_tools.local_workspace.commons import (
     HistoryProcessor,
-)
-from composio.local_tools.local_workspace.commons.local_docker_workspace import (
     WorkspaceManagerFactory,
 )
-from composio.local_tools.tool import Tool
-
+from composio.local_tools.local_workspace.workspace.actions import (
+    WorkspaceStatusAction,
+    CreateWorkspaceAction,
+)
 
-class CmdManagerTool(Tool):
+class LocalWorkspace(Tool):
     """
-    command manager tool for workspace
+    Use this action to create a workspace and get workspace ID in return.
+    this is a tool for creating local workspace
     """
 
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
+    workspace_factory: t.Optional[WorkspaceManagerFactory] = None
+    history_processor: t.Optional[HistoryProcessor] = None
 
-    def actions(self) -> list:
-        return [
-            FindFileCmd,
-            CreateFileCmd,
-            GoToLineNumInOpenFile,
-            OpenFile,
-            ScrollUp,
-            ScrollDown,
-            SearchFileCmd,
-            SearchDirCmd,
-            SetCursors,
-            EditFile,
-            RunCommandOnWorkspace,
-        ]
+    def actions(self) -> list[t.Type[Action]]:
+        return [WorkspaceStatusAction, CreateWorkspaceAction]
 
     def triggers(self) -> list:
         return []
 
     def set_workspace_factory(self, workspace_factory: WorkspaceManagerFactory):
         self.workspace_factory = workspace_factory
 
-    def get_workspace_factory(self) -> WorkspaceManagerFactory:
+    def get_workspace_factory(self) -> t.Optional[WorkspaceManagerFactory]:
         return self.workspace_factory
 
     def set_history_processor(self, history_processor: HistoryProcessor):
         self.history_processor = history_processor
 
-    def get_history_processor(self) -> HistoryProcessor:
+    def get_history_processor(self) -> t.Optional[HistoryProcessor]:
         return self.history_processor
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/commons/command_runner_model.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/commons/command_runner_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,7 +80,8 @@
         code="""state() {
             echo '{"working_dir": "'$(realpath --relative-to=$ROOT/.. $PWD)'"}';
         };""",
     )
     _commands: list[Command] = field(default_factory=list)
     _subroutines: dict[str, Subroutine] = field(default_factory=dict)
     subroutine_types: list[Subroutine] = field(default_factory=list)
+    multi_line_command_endings: dict[str, str] = field(default_factory=dict)
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/commons/parsing.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/commons/parsing.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/commons/utils.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/commons/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import tarfile
 import tempfile
 import time
 import traceback
 from io import BytesIO
 from subprocess import PIPE, STDOUT
-from typing import List, Set, Tuple
+from typing import List, Optional, Set, Tuple
 
 import docker
 
 from composio.local_tools.local_workspace.commons.get_logger import get_logger
 
 
 START_UP_DELAY = 5
@@ -343,14 +343,21 @@
         logger.error(traceback.format_exc())
     finally:
         # Cleanup: Remove the temporary file if it was created
         if temp_file_name and os.path.exists(temp_file_name):
             os.remove(temp_file_name)
 
 
+def process_output(output: str, return_code: Optional[int]):
+    if return_code is None:
+        return_code = 1
+        output = "Exception: " + output
+    return output, return_code
+
+
 def communicate(
     container: subprocess.Popen,
     container_obj,
     input_cmd: str,
     parent_pids: List[str],
     timeout_duration=25,
 ):
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
+from typing import Optional
+
 from pydantic import BaseModel, Field
 
-from composio.local_tools.action import Action
+from composio.core.local import Action
 from composio.local_tools.local_workspace.commons.get_logger import get_logger
 from composio.local_tools.local_workspace.commons.history_processor import (
     HistoryProcessor,
 )
 from composio.local_tools.local_workspace.commons.local_docker_workspace import (
     WorkspaceManagerFactory,
 )
 
-
 STATUS_RUNNING = "running"
 STATUS_STOPPED = "stopped"
 logger = get_logger()
 
-
 class GetWorkspaceHistoryRequest(BaseModel):
     workspace_id: str = Field(
         ..., description="workspace-id will be used to get status of the workspace"
     )
 
-
 class GetWorkspaceHistoryResponse(BaseModel):
     workspace_history: dict = Field(
         ..., description="history of last n commands on the workspace"
     )
 
-
 class GetWorkspaceHistory(Action):
     """
     returns history for workspace.
     History includes -
             - state of the environment
             - last executed n commands
             - output from last n commands
     """
 
+    _history_maintains = True
     _display_name = "Get workspace history"
     _request_schema = GetWorkspaceHistoryRequest
     _response_schema = GetWorkspaceHistoryRequest
     _tags = ["workspace"]
+    _tool_name = "historykeeper"
     _history_len = 5
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
+    workspace_factory: Optional[WorkspaceManagerFactory] = None
+    history_processor: Optional[HistoryProcessor] = None
 
     def set_workspace_and_history(
         self,
         workspace_factory: WorkspaceManagerFactory,
         history_processor: HistoryProcessor,
     ):
         self.workspace_factory = workspace_factory
         self.history_processor = history_processor
 
     def execute(
         self, request_data: GetWorkspaceHistoryRequest, authorisation_data: dict = {}
-    ):
-        return self.history_processor.get_history(
-            workspace_id=request_data.workspace_id, n=self._history_len
-        )
-
-    def get_history_n(self):
-        """
-        Returns:
-        """
-        return
+    ) -> dict:
+        if self.history_processor is None:
+            logger.error("History processor is not set")
+            raise ValueError("History processor is not set")
+
+        return {
+            "workspace_history": self.history_processor.get_history(
+                workspace_id=request_data.workspace_id, n=self._history_len
+            )
+        }
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/tool.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-from composio.local_tools.local_workspace.commons.history_processor import (
-    HistoryProcessor,
-)
-from composio.local_tools.local_workspace.commons.local_docker_workspace import (
+import typing as t
+from typing import Optional
+from composio.core.local import Tool, Action
+
+from composio.local_tools.local_workspace.commons.get_logger import get_logger
+from composio.local_tools.local_workspace.commons import (
     WorkspaceManagerFactory,
+    HistoryProcessor
 )
-from composio.local_tools.local_workspace.history_keeper.actions.get_workspace_history import (
-    GetWorkspaceHistory,
-)
-from composio.local_tools.tool import Tool
+from .actions import GetWorkspaceHistory
 
+logger = get_logger()
 
 class HistoryKeeper(Tool):
     """
-    local workspace tool for creating local workspace
+    local workspace tool which can maintain history across commands.
     """
 
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
+    workspace_factory: Optional[WorkspaceManagerFactory] = None
+    history_processor: Optional[HistoryProcessor] = None
 
-    def actions(self) -> list:
+    def actions(self) -> list[t.Type[Action]]:
         return [GetWorkspaceHistory]
 
     def triggers(self) -> list:
         return []
 
     def set_workspace_factory(self, workspace_factory: WorkspaceManagerFactory):
         self.workspace_factory = workspace_factory
 
-    def get_workspace_factory(self) -> WorkspaceManagerFactory:
+    def get_workspace_factory(self) -> Optional[WorkspaceManagerFactory]:
         return self.workspace_factory
 
     def set_history_processor(self, history_processor: HistoryProcessor):
         self.history_processor = history_processor
 
-    def get_history_processor(self) -> HistoryProcessor:
+    def get_history_processor(self) -> Optional[HistoryProcessor]:
         return self.history_processor
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,151 +1,156 @@
-import os
+from pydantic import Field
 
-from pydantic import BaseModel, Field
-
-from composio.local_tools.action import Action
 from composio.local_tools.local_workspace.commons.get_logger import get_logger
 from composio.local_tools.local_workspace.commons.history_processor import (
-    HistoryProcessor,
+    history_recorder,
 )
 from composio.local_tools.local_workspace.commons.local_docker_workspace import (
-    KEY_CONTAINER_NAME,
-    KEY_IMAGE_NAME,
-    KEY_PARENT_PIDS,
-    KEY_WORKSPACE_MANAGER,
-    WorkspaceManagerFactory,
-    get_container_process,
-    get_workspace_meta_from_manager,
-)
-from composio.local_tools.local_workspace.commons.utils import (
     communicate,
-    communicate_with_handling,
-    get_container_by_container_name,
 )
+from composio.local_tools.local_workspace.commons.utils import process_output
 
+from .base_class import BaseAction, BaseRequest, BaseResponse
+from .const import SCRIPT_CURSOR_DEFAULT
 
-LONG_TIMEOUT = 200
-logger = get_logger()
 
-REPO_NAME = os.environ.get("REPO_NAME", "princeton-nlp/SWE-bench")
+logger = get_logger()
 
 
-class SetupGithubRepoRequest(BaseModel):
-    workspace_id: str = Field(
-        ..., description="workspace-id to get the running workspace-manager"
+class GoToRequest(BaseRequest):
+    line_number: int = Field(
+        ..., description="The line number to which the view should be moved."
     )
-    # repo_name: str = Field(..., description="github repo-name for which issue needs to be solved")
 
 
-class SetupGithubRepoResponse(BaseModel):
-    github_repo_copy_resp: str = Field(..., description="response of github repo copy")
+class GoToResponse(BaseResponse):
+    pass
 
 
-class SetupGithubRepo(Action):
+class GoToLineNumInOpenFile(BaseAction):
     """
-    clones github repo in the workspace
-    """
-
-    _display_name = "Clone github repo on workspace"
-    _request_schema = SetupGithubRepoRequest
-    _response_schema = SetupGithubRepoResponse
-    _tags = ["workspace"]
-    _tool_name = "localworkspace"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
-
-    def __init__(self):
-        super().__init__()
-        self.args = None
-        self.workspace_id = ""
-        self.repo_name = REPO_NAME
-        self.image_name = ""
-        self.container_name = ""
-        self.container_process = None
-        self.parent_pids = []
-        self.container_obj = None
-        self.logger = logger
-        self.repo_type = "not_local"
-
-    def _setup(self, args: SetupGithubRepoRequest):
-        self.args = args
-        self.workspace_id = args.workspace_id
-        workspace_meta = get_workspace_meta_from_manager(
-            self.workspace_factory, self.workspace_id
-        )
-        self.image_name = workspace_meta[KEY_IMAGE_NAME]
-        self.container_name = workspace_meta[KEY_CONTAINER_NAME]
-        self.container_process = get_container_process(
-            workspace_meta[KEY_WORKSPACE_MANAGER]
-        )
-        self.parent_pids = workspace_meta[KEY_PARENT_PIDS]
-        self.container_obj = self.get_container_by_container_name()
-        if not self.container_obj:
-            raise ValueError(
-                f"container-name {self.container_name} is not a valid docker-container"
-            )
-        self._github_token = self.load_github_token_from_host_env()
-
-    def set_workspace_and_history(
-        self,
-        workspace_factory: WorkspaceManagerFactory,
-        history_processor: HistoryProcessor,
-    ):
-        self.workspace_factory = workspace_factory
-        self.history_processor = history_processor
-
-    def get_container_by_container_name(self):
-        container_obj = get_container_by_container_name(
-            self.container_name, self.image_name
+    Navigates to a specific line number in the open file, with checks to ensure the file is open
+    and the line number is a valid number.
+
+    Args:
+    - line_number (int): The line number to navigate to.
+
+    Raises:
+    - ValueError: If line_number is not an integer.
+    - RuntimeError: If no file is currently open.
+    """
+
+    _display_name = "Goto Line Action"
+    _request_schema = GoToRequest
+    _response_schema = GoToResponse
+
+    @history_recorder()
+    def execute(
+        self, request_data: GoToRequest, authorisation_data: dict
+    ) -> GoToResponse:
+        self._setup(request_data)
+        self.script_file = SCRIPT_CURSOR_DEFAULT
+        self.command = "goto"
+        if self.container_process is None:
+            raise ValueError("Container process is not set")
+        command = f"{self.command} {str(request_data.line_number)}"
+        full_command = f"{command}"
+        output, return_code = communicate(
+            self.container_process, self.container_obj, full_command, self.parent_pids
         )
-        return container_obj
+        output, return_code = process_output(output, return_code)
+        return GoToResponse(output=output, return_code=return_code)
+
+
+class CreateFileRequest(BaseRequest):
+    file_name: str = Field(
+        ...,
+        description="The name of the new file to be created within the shell session",
+    )
+
+
+class CreateFileResponse(BaseResponse):
+    pass
 
-    def load_github_token_from_host_env(self):
-        # Retrieve the token from an environment variable
-        access_token = os.getenv("GITHUB_ACCESS_TOKEN")
-
-        # Check if the token is available
-        if access_token is None:
-            raise ValueError(
-                "GitHub access token is not set in the environment variables"
-            )
-        return access_token
-
-    def reset(self):
-        # Clone repository if not already cloned
-        folders = communicate(
-            self.container_process, self.container_obj, "ls", self.parent_pids
-        ).split("\n")
-        if self.repo_name not in folders:
-            raise ValueError(f"repo name {self.repo_name} is not found in workspace")
-
-        # Clean repository of any modifications + Checkout base commit
-        for cmd in [
-            f"cd {self.repo_name}",
-            "export ROOT=$(pwd -P)",
-        ]:
-            communicate_with_handling(
-                self.container_process,
-                self.container_obj,
-                cmd,
-                self.parent_pids,
-                error_msg="Failed to clean repository",
-            )
 
+class CreateFileCmd(BaseAction):
+    """
+    Creates a new file within a shell session.
+    Example:
+        - To create a file, provide the shell ID and the name of the new file.
+        - The response will indicate whether the file was created successfully and list any errors.
+    Raises:
+    - ValueError: If line_number is not an integer.
+    - RuntimeError: If no file is currently open.
+    """
+
+    _display_name = "Create and open a new file"
+    _request_schema = CreateFileRequest
+    _response_schema = CreateFileResponse
+
+    @history_recorder()
     def execute(
-        self, request_data: SetupGithubRepoRequest, authorisation_data: dict = {}
-    ):
+        self, request_data: CreateFileRequest, authorisation_data: dict
+    ) -> CreateFileResponse:
         self._setup(request_data)
-        token_prefix = ""
-        if self._github_token:
-            token_prefix = f"{self._github_token}@"
-        communicate_with_handling(
-            self.container_process,
-            self.container_obj,
-            f"git clone https://{token_prefix}github.com/{self.repo_name}.git",
-            self.parent_pids,
-            error_msg="Failed to clone repository from mirror",
-            timeout_duration=LONG_TIMEOUT,
+        self.script_file = SCRIPT_CURSOR_DEFAULT
+        self.command = "create"
+        if self.container_process is None:
+            raise ValueError("Container process is not set")
+        file_name = request_data.file_name
+        output, return_code = self.validate_file_name(file_name)
+        if output is not None:
+            return CreateFileResponse(output=output, return_code=return_code)
+        command = f"{self.command} {str(request_data.file_name)}"
+        print(f"Running command: {command}")
+        full_command = f"{command}"
+        output, return_code = communicate(
+            self.container_process, self.container_obj, full_command, self.parent_pids
         )
-        return SetupGithubRepoResponse(
-            github_repo_copy_resp=f"repo: {self.repo_name} is cloned to container"
+        output, return_code = process_output(output, return_code)
+        return CreateFileResponse(output=output, return_code=return_code)
+
+
+class OpenCmdRequest(BaseRequest):
+    file_name: str = Field(..., description="file path to open in the editor")
+    line_number: int = Field(
+        default=0,
+        description="if file-number is given, file will be open from that line number",
+    )
+
+
+class OpenCmdResponse(BaseResponse):
+    pass
+
+
+class OpenFile(BaseAction):
+    """
+    Opens a file in the editor based on the provided file path,
+    If line_number is provided, the window will be move to include that line
+
+    Can result in:
+    - ValueError: If file_path is not a string or if the file does not exist.
+    - RuntimeError: If no file is currently open.
+    """
+
+    _display_name = "Open File on workspace"
+    _request_schema = OpenCmdRequest
+    _response_schema = OpenCmdResponse
+
+    @history_recorder()
+    def execute(
+        self, request_data: OpenCmdRequest, authorisation_data: dict
+    ) -> OpenCmdResponse:
+        self._setup(request_data)
+        self.script_file = SCRIPT_CURSOR_DEFAULT
+        self.command = "open"
+        if self.container_process is None:
+            raise ValueError("Container process is not set")
+        command = f"{self.command} {request_data.file_name}"
+        if request_data.line_number != 0:
+            command += f"{request_data.line_number}"
+        full_command = f"{command}"
+        output, return_code = communicate(
+            self.container_process, self.container_obj, full_command, self.parent_pids
         )
+        output, return_code = process_output(output, return_code)
+        return OpenCmdResponse(output=output, return_code=return_code)
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/create_workspace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,153 +1,120 @@
-import logging
 from pathlib import Path
 
-from pydantic import BaseModel, Field
-from rich.logging import RichHandler
+from pydantic import Field
 
-from composio.local_tools.action import Action
 from composio.local_tools.local_workspace.commons.command_runner_model import (
     AgentConfig,
 )
-from composio.local_tools.local_workspace.commons.history_processor import (
-    HistoryProcessor,
-)
+from composio.local_tools.local_workspace.commons.get_logger import get_logger
 from composio.local_tools.local_workspace.commons.local_docker_workspace import (
     KEY_CONTAINER_NAME,
     KEY_IMAGE_NAME,
     KEY_PARENT_PIDS,
     KEY_WORKSPACE_MANAGER,
-    WorkspaceManagerFactory,
+    LocalDockerArgumentsModel,
     get_container_process,
     get_workspace_meta_from_manager,
 )
 from composio.local_tools.local_workspace.commons.utils import (
     communicate,
     communicate_with_handling,
     copy_file_to_container,
     get_container_by_container_name,
 )
 
+from .base_workspace_action import (
+    BaseWorkspaceAction,
+    BaseWorkspaceRequest,
+    BaseWorkspaceResponse,
+)
 
-LOGGER_NAME = "composio_logger"
-
-handler = RichHandler(show_time=False, show_path=False)
-handler.setLevel(logging.DEBUG)
-logger = logging.getLogger(LOGGER_NAME)
-logger.setLevel(logging.DEBUG)
-logger.addHandler(handler)
-logger.propagate = False
 
+logger = get_logger()
 STATUS_RUNNING = "running"
 STATUS_STOPPED = "stopped"
 
 script_path = Path(__file__).resolve()
 script_dir = script_path.parent
 
 
-class WorkspaceSetupRequest(BaseModel):
-    workspace_id: str = Field(
-        ..., description="workspace-id will be used to get status of the workspace"
+class CreateWorkspaceRequest(BaseWorkspaceRequest):
+    image_name: str = Field(
+        default="sweagent/swe-agent:latest",
+        description="""The workspace is a docker container.
+        Use docker image sweagent/swe-agent:latest it works for most use cases.
+        Only use a different docker image if you have a good reason.
+        Ex. image names ubuntu:22.04
+        """,
+        examples=["sweagent/swe-agent:latest", "ubuntu:22.04"],
     )
 
 
-class WorkspaceSetupResponse(BaseModel):
-    workspace_status: str = Field(
-        ..., description="status of the workspace given in request"
-    )
+class CreateWorkspaceResponse(BaseWorkspaceResponse):
+    workspace_id: str = Field(..., description="workspace-id for the created workspace")
 
 
-class SetupWorkspace(Action):
+class CreateWorkspaceAction(BaseWorkspaceAction):
     """
-    setsup workspace with the environment variables, scripts.
-    sets the path, and sources necessary scripts
+    Creates a workspace, and returns workspace-id
     """
 
-    _display_name = "Setup workspace"
-    _request_schema = WorkspaceSetupRequest
-    _response_schema = WorkspaceSetupResponse
-    _tags = ["workspace"]
-    _tool_name = "localworkspace"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
-
-    def __init__(self):
-        super().__init__()
-        self.args = None
-        self.workspace_id = ""
-        self.container_name = ""
-        self.image_name = ""
-        self.container_process = None
-        self.parent_pids = []
-        self.container_obj = None
-        self.return_code = None
-        self.logger = logger
-        self.config = None
-        self.config_file_path = None
+    _display_name = "Create workspace"
+    _request_schema = CreateWorkspaceRequest
+    _response_schema = CreateWorkspaceResponse
 
-    def _setup(self, args: WorkspaceSetupRequest):
-        self.args = args
-        self.workspace_id = args.workspace_id
+    def execute(
+        self, request_data: CreateWorkspaceRequest, authorisation_data: dict
+    ) -> CreateWorkspaceResponse:
+        if self.workspace_factory is None:
+            raise ValueError("Workspace factory is not set")
+
+        if request_data.image_name == "":
+            request_data.image_name = "sweagent/swe-agent:latest"
+
+        args: LocalDockerArgumentsModel = LocalDockerArgumentsModel(
+            image_name=request_data.image_name
+        )
+        workspace_id = self.workspace_factory.get_workspace_manager(args)
+        self.workspace_id = workspace_id
         workspace_meta = get_workspace_meta_from_manager(
             self.workspace_factory, self.workspace_id
         )
         if not workspace_meta:
             raise ValueError(
                 f"workspace not found, invalid workspace-id: {self.workspace_id}"
             )
         self.container_name = workspace_meta[KEY_CONTAINER_NAME]
         self.image_name = workspace_meta[KEY_IMAGE_NAME]
         self.container_process = get_container_process(
             workspace_meta[KEY_WORKSPACE_MANAGER]
         )
         self.parent_pids = workspace_meta[KEY_PARENT_PIDS]
-        self.container_obj = self.get_container_by_container_name()
+        self.container_obj = get_container_by_container_name(
+            self.container_name, self.image_name
+        )
         self.return_code = None
         self.logger = logger
-        self.config = None
         self.config_file_path = script_dir / Path("../../config/default.yaml")
-        self.load_config_from_path()
+        self.config = AgentConfig.load_yaml(self.config_file_path)
         if not self.container_obj:
             raise ValueError(
                 f"container-name {self.container_name} is not a valid docker-container"
             )
-
-    def set_workspace_and_history(
-        self,
-        workspace_factory: WorkspaceManagerFactory,
-        history_processor: HistoryProcessor,
-    ):
-        self.workspace_factory = workspace_factory
-        self.history_processor = history_processor
-
-    def execute(
-        self, request_data: WorkspaceSetupRequest, authorisation_data: dict = {}
-    ):
-        self._setup(request_data)
         self.set_env_variables()
         env_vars = "\n".join(self.config.env_variables)
-        return {"message": f"environment is set with variables: {env_vars}"}
-
-    def get_container_by_container_name(self):
-        container_obj = get_container_by_container_name(
-            self.container_name, self.image_name
-        )
-        return container_obj
-
-    def load_config_from_path(self):
-        if not self.config and self.config_file_path is not None:
-            # If unassigned, we load the config from the file to store its contents with the overall arguments
-            config = AgentConfig.load_yaml(self.config_file_path)
-            object.__setattr__(self, "config", config)
-        assert self.config is not None  # mypy
+        print(f"environment is set with variables: {env_vars}")
+        return CreateWorkspaceResponse(workspace_id=workspace_id)
 
     def set_env_variables(self):
-        commands_to_execute = [self.config.state_command.code] + [
-            f"{k}={v}" for k, v in self.config.env_variables.items()
-        ]
+        commands_to_execute = (
+            [self.config.state_command.code]
+            + ["pip install flake8"]
+            + [f"{k}={v}" for k, v in self.config.env_variables.items()]
+        )
         commands = "\n".join(commands_to_execute)
         return_code = 0
         output = None
         try:
             output, return_code = communicate(
                 self.container_process, self.container_obj, commands, self.parent_pids
             )
@@ -188,14 +155,29 @@
                     )
             else:
                 # scripts are made executable
                 datum["name"] = Path(file).name.rsplit(".", 1)[0]
                 datum["type"] = "script"
             command_files.append(datum)
         self.add_commands(command_files)
+        # create home directory and cd into it
+        communicate_with_handling(
+            self.container_process,
+            self.container_obj,
+            "mkdir -p /home/swe-agent",
+            self.parent_pids,
+            error_msg="Failed to create home directory",
+        )
+        communicate_with_handling(
+            self.container_process,
+            self.container_obj,
+            "cd /home/swe-agent",
+            self.parent_pids,
+            error_msg="Failed to cd to home directory",
+        )
 
     def add_commands(self, commands: list[dict]) -> None:
         """
         Adds custom commands to container
         """
         for command in commands:
             name = command["name"]
```

### Comparing `composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/workspace_status.py` & `composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/workspace_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,56 @@
 import docker
-from pydantic import BaseModel, Field
+from pydantic import Field
 
-from composio.local_tools.action import Action
 from composio.local_tools.local_workspace.commons.get_logger import get_logger
-from composio.local_tools.local_workspace.commons.history_processor import (
-    HistoryProcessor,
-)
 from composio.local_tools.local_workspace.commons.local_docker_workspace import (
-    WorkspaceManagerFactory,
     get_container_name_from_workspace_id,
 )
 
+from .base_workspace_action import (
+    BaseWorkspaceAction,
+    BaseWorkspaceRequest,
+    BaseWorkspaceResponse,
+)
+
 
 STATUS_RUNNING = "running"
 STATUS_STOPPED = "stopped"
 logger = get_logger()
 
 
-class WorkspaceStatusRequest(BaseModel):
+class WorkspaceStatusRequest(BaseWorkspaceRequest):
     workspace_id: str = Field(
         ..., description="workspace-id will be used to get status of the workspace"
     )
 
 
-class WorkspaceStatusResponse(BaseModel):
+class WorkspaceStatusResponse(BaseWorkspaceResponse):
     workspace_status: str = Field(
         ..., description="status of the workspace given in request"
     )
 
 
-class WorkspaceStatus(Action):
+class WorkspaceStatusAction(BaseWorkspaceAction):
     """
-    returns the status of workspace given in the request
+    Returns the status of workspace given in the request
     """
 
     _display_name = "Get workspace status"
     _request_schema = WorkspaceStatusRequest
     _response_schema = WorkspaceStatusResponse
-    _tags = ["workspace"]
-    _tool_name = "localworkspace"
-    workspace_factory: WorkspaceManagerFactory = None
-    history_processor: HistoryProcessor = None
-
-    def set_workspace_and_history(
-        self,
-        workspace_factory: WorkspaceManagerFactory,
-        history_processor: HistoryProcessor,
-    ):
-        self.workspace_factory = workspace_factory
-        self.history_processor = history_processor
-
-    def __init__(self):
-        super().__init__()
-        self.container_name = ""
-
-    def _setup(self, args: WorkspaceStatusRequest):
-        self.container_name = get_container_name_from_workspace_id(
-            self.workspace_factory, args.workspace_id
-        )
 
     def execute(
         self, request_data: WorkspaceStatusRequest, authorisation_data: dict = {}
     ):
-        self._setup(request_data)
+        if self.workspace_factory is None:
+            raise ValueError("Workspace factory is not set")
+        self.container_name = get_container_name_from_workspace_id(
+            self.workspace_factory, request_data.workspace_id
+        )
         client = docker.from_env()
         try:
             container = client.containers.get(self.container_name)
             if container.status == STATUS_RUNNING:
                 return WorkspaceStatusResponse(workspace_status=STATUS_RUNNING)
             return WorkspaceStatusResponse(workspace_status=STATUS_STOPPED)
         except docker.errors.NotFound:
```

### Comparing `composio_core-0.3.3/composio/storage/base.py` & `composio_core-0.3.4/composio/storage/base.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/tools/__init__.py` & `composio_core-0.3.4/composio/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/tools/schema.py` & `composio_core-0.3.4/composio/tools/schema.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/utils/decorators.py` & `composio_core-0.3.4/composio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/utils/git.py` & `composio_core-0.3.4/composio/utils/git.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/utils/shared.py` & `composio_core-0.3.4/composio/utils/shared.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio/utils/url.py` & `composio_core-0.3.4/composio/utils/url.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.3/composio_core.egg-info/PKG-INFO` & `composio_core-0.3.4/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.3
+Version: 0.3.4
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.3/composio_core.egg-info/SOURCES.txt` & `composio_core-0.3.4/composio_core.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,50 +20,64 @@
 composio/client/__init__.py
 composio/client/endpoints.py
 composio/client/enums.py
 composio/client/exceptions.py
 composio/client/http.py
 composio/client/local_handler.py
 composio/local_tools/__init__.py
-composio/local_tools/action.py
-composio/local_tools/tool.py
 composio/local_tools/file/__init__.py
 composio/local_tools/file/tool.py
+composio/local_tools/file/actions/__init__.py
+composio/local_tools/file/actions/read_file.py
+composio/local_tools/file/actions/write_file.py
+composio/local_tools/greptile/__init__.py
+composio/local_tools/greptile/tool.py
+composio/local_tools/greptile/actions/__init__.py
+composio/local_tools/greptile/actions/codequery.py
 composio/local_tools/local_workspace/__init__.py
 composio/local_tools/local_workspace/cmd_manager/__init__.py
-composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py
+composio/local_tools/local_workspace/cmd_manager/tool.py
 composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
+composio/local_tools/local_workspace/cmd_manager/actions/base_class.py
+composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py
 composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
 composio/local_tools/local_workspace/cmd_manager/actions/const.py
 composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
 composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
 composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
 composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
-composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py
 composio/local_tools/local_workspace/commons/__init__.py
 composio/local_tools/local_workspace/commons/command_runner_model.py
 composio/local_tools/local_workspace/commons/get_logger.py
 composio/local_tools/local_workspace/commons/history_processor.py
 composio/local_tools/local_workspace/commons/local_docker_workspace.py
 composio/local_tools/local_workspace/commons/parsing.py
 composio/local_tools/local_workspace/commons/utils.py
 composio/local_tools/local_workspace/history_keeper/__init__.py
-composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py
+composio/local_tools/local_workspace/history_keeper/tool.py
 composio/local_tools/local_workspace/history_keeper/actions/__init__.py
 composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
 composio/local_tools/local_workspace/workspace/__init__.py
-composio/local_tools/local_workspace/workspace/workspace_tool.py
+composio/local_tools/local_workspace/workspace/tool.py
 composio/local_tools/local_workspace/workspace/actions/__init__.py
+composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py
 composio/local_tools/local_workspace/workspace/actions/create_workspace.py
-composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py
-composio/local_tools/local_workspace/workspace/actions/workspace_setup.py
 composio/local_tools/local_workspace/workspace/actions/workspace_status.py
 composio/local_tools/mathematical/__init__.py
-composio/local_tools/mathematical/calculator.py
-composio/local_tools/mathematical/mathematical.py
+composio/local_tools/mathematical/tool.py
+composio/local_tools/ragtool/__init__.py
+composio/local_tools/ragtool/tool.py
+composio/local_tools/ragtool/actions/__init__.py
+composio/local_tools/ragtool/actions/rag_add_request.py
+composio/local_tools/ragtool/actions/rag_query.py
+composio/local_tools/webtool/__init__.py
+composio/local_tools/webtool/tool.py
+composio/local_tools/webtool/actions/__init__.py
+composio/local_tools/webtool/actions/scrape_website_content.py
+composio/local_tools/webtool/actions/scrape_website_element.py
 composio/storage/__init__.py
 composio/storage/base.py
 composio/storage/user.py
 composio/tools/__init__.py
 composio/tools/schema.py
 composio/utils/__init__.py
 composio/utils/decorators.py
```

### Comparing `composio_core-0.3.3/setup.py` & `composio_core-0.3.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Setup configuration for compsio core.
 """
 
 import os
 from pathlib import Path
-from setuptools import setup
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
+
 
 setup(
     name="composio_core",
-    version="0.3.3",
+    version="0.3.4",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

