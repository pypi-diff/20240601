# Comparing `tmp/composio_core-0.3.2.tar.gz` & `tmp/composio_core-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.3.2.tar", last modified: Thu May 30 15:24:18 2024, max compression
+gzip compressed data, was "composio_core-0.3.3.tar", last modified: Fri May 31 15:19:55 2024, max compression
```

## Comparing `composio_core-0.3.2.tar` & `composio_core-0.3.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.485798 composio_core-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 15:23:58.000000 composio_core-0.3.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-30 15:24:18.485798 composio_core-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-30 15:23:58.000000 composio_core-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.473798 composio_core-0.3.2/composio/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.473798 composio_core-0.3.2/composio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/add.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7910 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/client/
--rw-r--r--   0 runner    (1001) docker     (127)    31185 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)   235201 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/local_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/file/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/file/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/local_workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19278 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/commons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/command_runner_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/get_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/history_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/local_docker_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/workspace_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/mathematical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/mathematical/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/mathematical/mathematical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/storage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/tools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.485798 composio_core-0.3.2/composio_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:24:18.485798 composio_core-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-30 15:23:58.000000 composio_core-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.446807 composio_core-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 15:19:19.000000 composio_core-0.3.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-31 15:19:55.446807 composio_core-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-31 15:19:19.000000 composio_core-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.430807 composio_core-0.3.3/composio/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.434807 composio_core-0.3.3/composio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/add.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8106 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/cli/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    31369 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)   316153 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/client/local_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/file/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/local_workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.438807 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19278 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/command_runner_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/get_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/history_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/local_docker_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/local_workspace/workspace/workspace_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/local_tools/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/mathematical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/mathematical/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/mathematical/mathematical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/local_tools/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.442807 composio_core-0.3.3/composio/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/storage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.446807 composio_core-0.3.3/composio/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.446807 composio_core-0.3.3/composio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-31 15:19:19.000000 composio_core-0.3.3/composio/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.446807 composio_core-0.3.3/composio_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:19:55.000000 composio_core-0.3.3/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:19:55.446807 composio_core-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-31 15:19:19.000000 composio_core-0.3.3/setup.py
```

### Comparing `composio_core-0.3.2/PKG-INFO` & `composio_core-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.2
+Version: 0.3.3
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.2/README.md` & `composio_core-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/cli/__init__.py` & `composio_core-0.3.3/composio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/cli/actions.py` & `composio_core-0.3.3/composio/cli/actions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/cli/add.py` & `composio_core-0.3.3/composio/cli/add.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/cli/apps.py` & `composio_core-0.3.3/composio/cli/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,22 @@
             key=lambda x: x.appKey,
         )
         triggers = sorted(
             context.client.triggers.get(),
             key=lambda x: x.appKey,
         )
         if not beta:
-            apps = [app for app in apps if not app.name.lower().endswith("beta")]
+            c = []
+            for app in apps:
+                if app.name.lower().endswith("beta"):
+                    continue
+                c.append(app)
+            apps = c
+            # apps = list(set([app for app in apps if not app.name.lower().endswith("beta")]))
+
         enum_module = MODULE_TEMPLATE.format(
             tag_enum=_get_tag_enum(apps=apps, actions=actions),
             app_enum=_get_app_enum(apps=apps),
             action_enum=_get_action_enum(apps=apps, actions=actions),
             trigger_enum=_get_trigger_enum(apps=apps, triggers=triggers),
         )
         with open(enums.__file__, "w", encoding="utf-8") as file:
```

### Comparing `composio_core-0.3.2/composio/cli/connections.py` & `composio_core-0.3.3/composio/cli/connections.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/cli/context.py` & `composio_core-0.3.3/composio/cli/context.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/cli/integrations.py` & `composio_core-0.3.3/composio/cli/integrations.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/cli/login.py` & `composio_core-0.3.3/composio/cli/login.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/cli/triggers.py` & `composio_core-0.3.3/composio/cli/triggers.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/client/__init__.py` & `composio_core-0.3.3/composio/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,22 +699,24 @@
         response_json = response.json()
         items = [self.model(**action) for action in response_json.get("items")]
         if len(actions) > 0:
             required_triggers = [action.action for action in actions]
             items = [item for item in items if item.name in required_triggers]
 
         if len(tags) > 0:
-            required_triggers = [
+            required_tags = [
                 tag.name if isinstance(tag, Tag) else tag for tag in tags
             ]
-            items = [
-                item
-                for item in items
-                if any(tag in required_triggers for tag in item.tags)
-            ]
+            should_not_filter_using_tags = len(items) < 15 and len(required_tags) == 1 and required_tags[0] == "important"
+            if not should_not_filter_using_tags:
+                items = [
+                    item
+                    for item in items
+                    if any(tag in required_tags for tag in item.tags)
+                ]
 
         if len(local_apps) > 0 or len(local_actions) > 0:
             local_items = self.local_handler.get_list_of_action_schemas(
                 apps=local_apps, actions=local_actions, tags=tags
             )
             items = [self.model(**item) for item in local_items] + items
         return items
```

### Comparing `composio_core-0.3.2/composio/client/endpoints.py` & `composio_core-0.3.3/composio/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/client/exceptions.py` & `composio_core-0.3.3/composio/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/client/http.py` & `composio_core-0.3.3/composio/client/http.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/client/local_handler.py` & `composio_core-0.3.3/composio/client/local_handler.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/constants.py` & `composio_core-0.3.3/composio/constants.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/exceptions.py` & `composio_core-0.3.3/composio/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/action.py` & `composio_core-0.3.3/composio/local_tools/action.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/file/tool.py` & `composio_core-0.3.3/composio/local_tools/file/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/commons/command_runner_model.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/commons/command_runner_model.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/commons/history_processor.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/commons/history_processor.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/commons/local_docker_workspace.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/commons/local_docker_workspace.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/commons/parsing.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/commons/parsing.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/commons/utils.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/commons/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/create_workspace.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/create_workspace.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/workspace_status.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/workspace/actions/workspace_status.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/workspace_tool.py` & `composio_core-0.3.3/composio/local_tools/local_workspace/workspace/workspace_tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/mathematical/calculator.py` & `composio_core-0.3.3/composio/local_tools/mathematical/calculator.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/local_tools/tool.py` & `composio_core-0.3.3/composio/local_tools/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/storage/base.py` & `composio_core-0.3.3/composio/storage/base.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/tools/__init__.py` & `composio_core-0.3.3/composio/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/tools/schema.py` & `composio_core-0.3.3/composio/tools/schema.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/utils/decorators.py` & `composio_core-0.3.3/composio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/utils/git.py` & `composio_core-0.3.3/composio/utils/git.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/utils/shared.py` & `composio_core-0.3.3/composio/utils/shared.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio/utils/url.py` & `composio_core-0.3.3/composio/utils/url.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/composio_core.egg-info/PKG-INFO` & `composio_core-0.3.3/composio_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.2
+Version: 0.3.3
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.2/composio_core.egg-info/SOURCES.txt` & `composio_core-0.3.3/composio_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.2/setup.py` & `composio_core-0.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from pathlib import Path
 from setuptools import setup
 from setuptools import setup, find_packages
 
 setup(
     name="composio_core",
-    version="0.3.2",
+    version="0.3.3",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

