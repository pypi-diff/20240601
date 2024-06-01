# Comparing `tmp/composio_core-0.3.6.tar.gz` & `tmp/composio_core-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.3.6.tar", last modified: Sat Jun  1 01:49:54 2024, max compression
+gzip compressed data, was "composio_core-0.3.7.tar", last modified: Sat Jun  1 03:17:50 2024, max compression
```

## Comparing `composio_core-0.3.6.tar` & `composio_core-0.3.7.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.038567 composio_core-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-01 01:49:33.000000 composio_core-0.3.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 01:49:54.038567 composio_core-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-06-01 01:49:33.000000 composio_core-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.022568 composio_core-0.3.6/composio/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.022568 composio_core-0.3.6/composio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2549 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/add.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8565 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/cli/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/client/
--rw-r--r--   0 runner    (1001) docker     (127)    32419 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/client/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)   316458 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/client/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/client/local_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/core/local/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/core/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/core/local/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/core/local/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/local_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/local_tools/file/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/local_tools/file/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/file/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/file/actions/read_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/file/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/file/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/local_tools/greptile/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/greptile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/local_tools/greptile/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/greptile/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/greptile/actions/codequery.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/greptile/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/local_tools/local_workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.026568 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.030568 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.030568 composio_core-0.3.6/composio/local_tools/local_workspace/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/commons/command_runner_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/commons/get_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/commons/history_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/commons/local_docker_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/commons/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.030568 composio_core-0.3.6/composio/local_tools/local_workspace/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.030568 composio_core-0.3.6/composio/local_tools/local_workspace/history_keeper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/history_keeper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.030568 composio_core-0.3.6/composio/local_tools/local_workspace/history_keeper/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/history_keeper/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.030568 composio_core-0.3.6/composio/local_tools/local_workspace/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/local_tools/local_workspace/workspace/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/workspace/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/local_workspace/workspace/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/local_tools/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/mathematical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/local_tools/mathematical/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/mathematical/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/mathematical/actions/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/mathematical/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/local_tools/ragtool/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/ragtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/local_tools/ragtool/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/ragtool/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/ragtool/actions/rag_add_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/ragtool/actions/rag_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/ragtool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/local_tools/webtool/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/webtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/local_tools/webtool/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/webtool/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/webtool/actions/scrape_website_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/webtool/actions/scrape_website_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/local_tools/webtool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/storage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.034567 composio_core-0.3.6/composio/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/tools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.038567 composio_core-0.3.6/composio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/utils/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 01:49:33.000000 composio_core-0.3.6/composio/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:54.038567 composio_core-0.3.6/composio_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 01:49:54.000000 composio_core-0.3.6/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-06-01 01:49:54.000000 composio_core-0.3.6/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:49:54.000000 composio_core-0.3.6/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 01:49:54.000000 composio_core-0.3.6/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 01:49:54.000000 composio_core-0.3.6/composio_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 01:49:54.000000 composio_core-0.3.6/composio_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:49:54.038567 composio_core-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-01 01:49:33.000000 composio_core-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.141311 composio_core-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-01 03:17:23.000000 composio_core-0.3.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 03:17:50.141311 composio_core-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-06-01 03:17:23.000000 composio_core-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.121310 composio_core-0.3.7/composio/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.125310 composio_core-0.3.7/composio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2549 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/add.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8583 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/cli/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.125310 composio_core-0.3.7/composio/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    32419 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)   316721 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/client/local_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.125310 composio_core-0.3.7/composio/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.129310 composio_core-0.3.7/composio/core/local/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/core/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/core/local/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/core/local/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.129310 composio_core-0.3.7/composio/local_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.129310 composio_core-0.3.7/composio/local_tools/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.129310 composio_core-0.3.7/composio/local_tools/file/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/file/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/file/actions/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/file/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/file/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.129310 composio_core-0.3.7/composio/local_tools/greptile/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/greptile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.129310 composio_core-0.3.7/composio/local_tools/greptile/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/greptile/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/greptile/actions/codequery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/greptile/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.129310 composio_core-0.3.7/composio/local_tools/local_workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.129310 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.133310 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.133310 composio_core-0.3.7/composio/local_tools/local_workspace/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/commons/command_runner_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/commons/get_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/commons/history_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/commons/local_docker_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/commons/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.133310 composio_core-0.3.7/composio/local_tools/local_workspace/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.133310 composio_core-0.3.7/composio/local_tools/local_workspace/history_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/history_keeper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.133310 composio_core-0.3.7/composio/local_tools/local_workspace/history_keeper/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/history_keeper/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.133310 composio_core-0.3.7/composio/local_tools/local_workspace/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.133310 composio_core-0.3.7/composio/local_tools/local_workspace/workspace/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/workspace/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/local_workspace/workspace/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.133310 composio_core-0.3.7/composio/local_tools/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/mathematical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.137310 composio_core-0.3.7/composio/local_tools/mathematical/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/mathematical/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/mathematical/actions/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/mathematical/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.137310 composio_core-0.3.7/composio/local_tools/ragtool/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/ragtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.137310 composio_core-0.3.7/composio/local_tools/ragtool/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/ragtool/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/ragtool/actions/rag_add_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/ragtool/actions/rag_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/ragtool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.137310 composio_core-0.3.7/composio/local_tools/webtool/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/webtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.137310 composio_core-0.3.7/composio/local_tools/webtool/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/webtool/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/webtool/actions/scrape_website_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/webtool/actions/scrape_website_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/local_tools/webtool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.137310 composio_core-0.3.7/composio/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/storage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.137310 composio_core-0.3.7/composio/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.137310 composio_core-0.3.7/composio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/utils/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 03:17:23.000000 composio_core-0.3.7/composio/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:50.141311 composio_core-0.3.7/composio_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 03:17:50.000000 composio_core-0.3.7/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-06-01 03:17:50.000000 composio_core-0.3.7/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:17:50.000000 composio_core-0.3.7/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 03:17:50.000000 composio_core-0.3.7/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 03:17:50.000000 composio_core-0.3.7/composio_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 03:17:50.000000 composio_core-0.3.7/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:17:50.141311 composio_core-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-01 03:17:23.000000 composio_core-0.3.7/setup.py
```

### Comparing `composio_core-0.3.6/PKG-INFO` & `composio_core-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.6
+Version: 0.3.7
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.6/README.md` & `composio_core-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/cli/__init__.py` & `composio_core-0.3.7/composio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/cli/actions.py` & `composio_core-0.3.7/composio/cli/actions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/cli/add.py` & `composio_core-0.3.7/composio/cli/add.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/cli/apps.py` & `composio_core-0.3.7/composio/cli/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         for action in app_actions:
             enum_name = f"{_get_enum_key(action.name)}"
             enum_value = f'("{app.key}", "{action.name}", {app.no_auth})'
             action_enums += f"    {enum_name} = {enum_value}\n"
     local_tool_handler = LocalToolHandler()
     for tool in local_tool_handler.registered_tools:
         for action in tool.actions():
-            enum_name = f"{_get_enum_key(action().action_name)}"
+            enum_name = f"{_get_enum_key(action().get_tool_merged_action_name())}"
             enum_value = f'("{tool.tool_name}", "{tool.tool_name}_{action().action_name}", True, True)'
             action_enums += f"    {enum_name} = {enum_value}\n"
     return ACTION_ENUM_TEMPLATE.format(actions=action_enums)
 
 
 def _get_trigger_enum(
     apps: t.List[AppModel],
```

### Comparing `composio_core-0.3.6/composio/cli/connections.py` & `composio_core-0.3.7/composio/cli/connections.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/cli/context.py` & `composio_core-0.3.7/composio/cli/context.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/cli/integrations.py` & `composio_core-0.3.7/composio/cli/integrations.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/cli/login.py` & `composio_core-0.3.7/composio/cli/login.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/cli/triggers.py` & `composio_core-0.3.7/composio/cli/triggers.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/client/__init__.py` & `composio_core-0.3.7/composio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/client/endpoints.py` & `composio_core-0.3.7/composio/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/client/enums.py` & `composio_core-0.3.7/composio/client/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,349 +12,349 @@
 
     @property
     def name(self) -> str:
         """Returns trigger name."""
         return self.value[0]
 
     IMPORTANT = ("default", "important")
-    ASANA_PORTFOLIOS = ("asana", "Portfolios")
-    ASANA_PORTFOLIO_MEMBERSHIPS = ("asana", "Portfolio memberships")
+    ASANA_GOAL_RELATIONSHIPS = ("asana", "Goal relationships")
+    ASANA_BATCH_API = ("asana", "Batch API")
+    ASANA_TEAMS = ("asana", "Teams")
+    ASANA_PROJECT_TEMPLATES = ("asana", "Project templates")
+    ASANA_TASKS = ("asana", "Tasks")
+    ASANA_WORKSPACE_MEMBERSHIPS = ("asana", "Workspace memberships")
+    ASANA_PROJECT_BRIEFS = ("asana", "Project briefs")
     ASANA_EVENTS = ("asana", "Events")
+    ASANA_TIME_TRACKING_ENTRIES = ("asana", "Time tracking entries")
+    ASANA_ORGANIZATION_EXPORTS = ("asana", "Organization exports")
+    ASANA_STATUS_UPDATES = ("asana", "Status updates")
     ASANA_RULES = ("asana", "Rules")
     ASANA_MEMBERSHIPS = ("asana", "Memberships")
-    ASANA_PROJECT_BRIEFS = ("asana", "Project briefs")
-    ASANA_TEAMS = ("asana", "Teams")
-    ASANA_ALLOCATIONS = ("asana", "Allocations")
     ASANA_TYPEAHEAD = ("asana", "Typeahead")
-    ASANA_TASKS = ("asana", "Tasks")
-    ASANA_WORKSPACE_MEMBERSHIPS = ("asana", "Workspace memberships")
     ASANA_WEBHOOKS = ("asana", "Webhooks")
-    ASANA_PROJECTS = ("asana", "Projects")
-    ASANA_PROJECT_TEMPLATES = ("asana", "Project templates")
-    ASANA_STORIES = ("asana", "Stories")
-    ASANA_ORGANIZATION_EXPORTS = ("asana", "Organization exports")
+    ASANA_PORTFOLIOS = ("asana", "Portfolios")
+    ASANA_JOBS = ("asana", "Jobs")
     ASANA_TEAM_MEMBERSHIPS = ("asana", "Team memberships")
     ASANA_AUDIT_LOG_API = ("asana", "Audit log API")
+    ASANA_USERS = ("asana", "Users")
+    ASANA_USER_TASK_LISTS = ("asana", "User task lists")
+    ASANA_PORTFOLIO_MEMBERSHIPS = ("asana", "Portfolio memberships")
+    ASANA_PROJECTS = ("asana", "Projects")
+    ASANA_CUSTOM_FIELD_SETTINGS = ("asana", "Custom field settings")
+    ASANA_ALLOCATIONS = ("asana", "Allocations")
+    ASANA_TAGS = ("asana", "Tags")
+    ASANA_ATTACHMENTS = ("asana", "Attachments")
     ASANA_TASK_TEMPLATES = ("asana", "Task templates")
     ASANA_GOALS = ("asana", "Goals")
-    ASANA_GOAL_RELATIONSHIPS = ("asana", "Goal relationships")
-    ASANA_BATCH_API = ("asana", "Batch API")
-    ASANA_PROJECT_MEMBERSHIPS = ("asana", "Project memberships")
-    ASANA_TAGS = ("asana", "Tags")
     ASANA_CUSTOM_FIELDS = ("asana", "Custom fields")
-    ASANA_TIME_PERIODS = ("asana", "Time periods")
-    ASANA_ATTACHMENTS = ("asana", "Attachments")
-    ASANA_USER_TASK_LISTS = ("asana", "User task lists")
-    ASANA_CUSTOM_FIELD_SETTINGS = ("asana", "Custom field settings")
-    ASANA_USERS = ("asana", "Users")
-    ASANA_STATUS_UPDATES = ("asana", "Status updates")
-    ASANA_TIME_TRACKING_ENTRIES = ("asana", "Time tracking entries")
+    ASANA_STORIES = ("asana", "Stories")
+    ASANA_WORKSPACES = ("asana", "Workspaces")
     ASANA_SECTIONS = ("asana", "Sections")
-    ASANA_JOBS = ("asana", "Jobs")
     ASANA_PROJECT_STATUSES = ("asana", "Project statuses")
-    ASANA_WORKSPACES = ("asana", "Workspaces")
-    ATTIO_ATTRIBUTES = ("attio", "Attributes")
-    ATTIO_OBJECTS = ("attio", "Objects")
-    ATTIO_WEBHOOKS = ("attio", "Webhooks")
+    ASANA_TIME_PERIODS = ("asana", "Time periods")
+    ASANA_PROJECT_MEMBERSHIPS = ("asana", "Project memberships")
+    ATTIO_LISTS = ("attio", "Lists")
     ATTIO_THREADS = ("attio", "Threads")
+    ATTIO_ENTRIES = ("attio", "Entries")
+    ATTIO_WEBHOOKS = ("attio", "Webhooks")
+    ATTIO_OBJECTS = ("attio", "Objects")
+    ATTIO_TASKS = ("attio", "Tasks")
     ATTIO_META = ("attio", "Meta")
-    ATTIO_WORKSPACE_MEMBERS = ("attio", "Workspace members")
-    ATTIO_NOTES = ("attio", "Notes")
     ATTIO_COMMENTS = ("attio", "Comments")
+    ATTIO_ATTRIBUTES = ("attio", "Attributes")
     ATTIO_RECORDS = ("attio", "Records")
-    ATTIO_TASKS = ("attio", "Tasks")
-    ATTIO_ENTRIES = ("attio", "Entries")
-    ATTIO_LISTS = ("attio", "Lists")
+    ATTIO_NOTES = ("attio", "Notes")
+    ATTIO_WORKSPACE_MEMBERS = ("attio", "Workspace members")
+    BREVO_TASKS = ("brevo", "Tasks")
+    BREVO_FILES = ("brevo", "Files")
     BREVO_COMPANIES = ("brevo", "Companies")
-    BREVO_EXTERNAL_FEEDS = ("brevo", "External Feeds")
-    BREVO_INBOUND_PARSING = ("brevo", "Inbound Parsing")
-    BREVO_ACCOUNT = ("brevo", "Account")
     BREVO_CONVERSATIONS = ("brevo", "Conversations")
-    BREVO_RESELLER = ("brevo", "Reseller")
-    BREVO_USER = ("brevo", "User")
+    BREVO_EMAIL_CAMPAIGNS = ("brevo", "Email Campaigns")
     BREVO_SMS_CAMPAIGNS = ("brevo", "SMS Campaigns")
-    BREVO_NOTES = ("brevo", "Notes")
-    BREVO_TASKS = ("brevo", "Tasks")
-    BREVO_WHATSAPP_CAMPAIGNS = ("brevo", "WhatsApp Campaigns")
     BREVO_WEBHOOKS = ("brevo", "Webhooks")
+    BREVO_CONTACTS = ("brevo", "Contacts")
+    BREVO_INBOUND_PARSING = ("brevo", "Inbound Parsing")
+    BREVO_USER = ("brevo", "User")
+    BREVO_ACCOUNT = ("brevo", "Account")
+    BREVO_MASTER_ACCOUNT = ("brevo", "Master account")
     BREVO_TRANSACTIONAL_WHATSAPP = ("brevo", "Transactional WhatsApp")
+    BREVO_DEALS = ("brevo", "Deals")
     BREVO_COUPONS = ("brevo", "Coupons")
     BREVO_DOMAINS = ("brevo", "Domains")
-    BREVO_EVENT = ("brevo", "Event")
-    BREVO_EMAIL_CAMPAIGNS = ("brevo", "Email Campaigns")
-    BREVO_TRANSACTIONAL_EMAILS = ("brevo", "Transactional emails")
+    BREVO_WHATSAPP_CAMPAIGNS = ("brevo", "WhatsApp Campaigns")
+    BREVO_NOTES = ("brevo", "Notes")
     BREVO_SENDERS = ("brevo", "Senders")
+    BREVO_EXTERNAL_FEEDS = ("brevo", "External Feeds")
+    BREVO_RESELLER = ("brevo", "Reseller")
+    BREVO_ECOMMERCE = ("brevo", "Ecommerce")
     BREVO_TRANSACTIONAL_SMS = ("brevo", "Transactional SMS")
+    BREVO_TRANSACTIONAL_EMAILS = ("brevo", "Transactional emails")
+    BREVO_EVENT = ("brevo", "Event")
     BREVO_PROCESS = ("brevo", "Process")
-    BREVO_DEALS = ("brevo", "Deals")
-    BREVO_CONTACTS = ("brevo", "Contacts")
-    BREVO_MASTER_ACCOUNT = ("brevo", "Master account")
-    BREVO_ECOMMERCE = ("brevo", "Ecommerce")
-    BREVO_FILES = ("brevo", "Files")
-    CLICKUP_MEMBERS = ("clickup", "Members")
-    CLICKUP_GUESTS = ("clickup", "Guests")
+    CLICKUP_CUSTOM_TASK_TYPES = ("clickup", "Custom Task Types")
+    CLICKUP_TASKS = ("clickup", "Tasks")
     CLICKUP_SPACES = ("clickup", "Spaces")
+    CLICKUP_GUESTS = ("clickup", "Guests")
+    CLICKUP_MEMBERS = ("clickup", "Members")
     CLICKUP_FOLDERS = ("clickup", "Folders")
+    CLICKUP_WEBHOOKS = ("clickup", "Webhooks")
+    CLICKUP_VIEWS = ("clickup", "Views")
     CLICKUP_TEAMS___WORKSPACES = ("clickup", "Teams - Workspaces")
-    CLICKUP_TIME_TRACKING__LEGACY_ = ("clickup", "Time Tracking (Legacy)")
-    CLICKUP_ROLES = ("clickup", "Roles")
-    CLICKUP_TASK_CHECKLISTS = ("clickup", "Task Checklists")
-    CLICKUP_TASKS = ("clickup", "Tasks")
-    CLICKUP_LISTS = ("clickup", "Lists")
     CLICKUP_CUSTOM_FIELDS = ("clickup", "Custom Fields")
-    CLICKUP_TIME_TRACKING = ("clickup", "Time Tracking")
-    CLICKUP_WEBHOOKS = ("clickup", "Webhooks")
+    CLICKUP_USERS = ("clickup", "Users")
+    CLICKUP_COMMENTS = ("clickup", "Comments")
+    CLICKUP_ROLES = ("clickup", "Roles")
     CLICKUP_AUTHORIZATION = ("clickup", "Authorization")
-    CLICKUP_CUSTOM_TASK_TYPES = ("clickup", "Custom Task Types")
-    CLICKUP_GOALS = ("clickup", "Goals")
-    CLICKUP_TASK_RELATIONSHIPS = ("clickup", "Task Relationships")
     CLICKUP_TAGS = ("clickup", "Tags")
-    CLICKUP_VIEWS = ("clickup", "Views")
     CLICKUP_ATTACHMENTS = ("clickup", "Attachments")
-    CLICKUP_USERS = ("clickup", "Users")
-    CLICKUP_COMMENTS = ("clickup", "Comments")
+    CLICKUP_LISTS = ("clickup", "Lists")
+    CLICKUP_TIME_TRACKING = ("clickup", "Time Tracking")
+    CLICKUP_GOALS = ("clickup", "Goals")
     CLICKUP_SHARED_HIERARCHY = ("clickup", "Shared Hierarchy")
-    CLICKUP_TASK_TEMPLATES = ("clickup", "Task Templates")
+    CLICKUP_TASK_RELATIONSHIPS = ("clickup", "Task Relationships")
     CLICKUP_TEAMS___USER_GROUPS = ("clickup", "Teams - User Groups")
-    ELEVENLABS_SAMPLES = ("elevenlabs", "samples")
+    CLICKUP_TASK_CHECKLISTS = ("clickup", "Task Checklists")
+    CLICKUP_TIME_TRACKING__LEGACY_ = ("clickup", "Time Tracking (Legacy)")
+    CLICKUP_TASK_TEMPLATES = ("clickup", "Task Templates")
+    ELEVENLABS_WORKSPACE = ("elevenlabs", "workspace")
     ELEVENLABS_SPEECH_TO_SPEECH = ("elevenlabs", "speech-to-speech")
-    ELEVENLABS_VOICE_GENERATION = ("elevenlabs", "voice-generation")
-    ELEVENLABS_TEXT_TO_SPEECH = ("elevenlabs", "text-to-speech")
     ELEVENLABS_PROJECTS = ("elevenlabs", "projects")
-    ELEVENLABS_WORKSPACE = ("elevenlabs", "workspace")
+    ELEVENLABS_VOICES = ("elevenlabs", "voices")
+    ELEVENLABS_TEXT_TO_SPEECH = ("elevenlabs", "text-to-speech")
+    ELEVENLABS_VOICE_GENERATION = ("elevenlabs", "voice-generation")
+    ELEVENLABS_DUBBING = ("elevenlabs", "dubbing")
     ELEVENLABS_AUDIO_NATIVE = ("elevenlabs", "audio-native")
+    ELEVENLABS_SAMPLES = ("elevenlabs", "samples")
+    ELEVENLABS_MODELS = ("elevenlabs", "models")
+    ELEVENLABS_PRONUNCIATION_DICTIONARY = ("elevenlabs", "Pronunciation Dictionary")
     ELEVENLABS_SPEECH_HISTORY = ("elevenlabs", "speech-history")
     ELEVENLABS_USER = ("elevenlabs", "user")
-    ELEVENLABS_DUBBING = ("elevenlabs", "dubbing")
-    ELEVENLABS_PRONUNCIATION_DICTIONARY = ("elevenlabs", "Pronunciation Dictionary")
-    ELEVENLABS_VOICES = ("elevenlabs", "voices")
-    ELEVENLABS_MODELS = ("elevenlabs", "models")
-    FIGMA_PAYMENTS = ("figma", "Payments")
-    FIGMA_ACTIVITY_LOGS = ("figma", "Activity Logs")
     FIGMA_DEV_RESOURCES = ("figma", "Dev Resources")
-    FIGMA_VARIABLES = ("figma", "Variables")
-    FIGMA_USERS = ("figma", "Users")
-    FIGMA_COMMENTS = ("figma", "Comments")
-    FIGMA_COMMENT_REACTIONS = ("figma", "Comment Reactions")
+    FIGMA_WEBHOOKS = ("figma", "Webhooks")
+    FIGMA_PROJECTS = ("figma", "Projects")
     FIGMA_FILES = ("figma", "Files")
+    FIGMA_COMMENT_REACTIONS = ("figma", "Comment Reactions")
+    FIGMA_COMMENTS = ("figma", "Comments")
+    FIGMA_COMPONENT_SETS = ("figma", "Component Sets")
     FIGMA_STYLES = ("figma", "Styles")
+    FIGMA_USERS = ("figma", "Users")
+    FIGMA_VARIABLES = ("figma", "Variables")
+    FIGMA_PAYMENTS = ("figma", "Payments")
     FIGMA_COMPONENTS = ("figma", "Components")
-    FIGMA_WEBHOOKS = ("figma", "Webhooks")
-    FIGMA_COMPONENT_SETS = ("figma", "Component Sets")
-    FIGMA_PROJECTS = ("figma", "Projects")
-    GITHUB_GITIGNORE = ("github", "gitignore")
-    GITHUB_CODE = ("github", "code")
-    GITHUB_GISTS = ("github", "gists")
+    FIGMA_ACTIVITY_LOGS = ("figma", "Activity Logs")
+    GITHUB_BILLING = ("github", "billing")
     GITHUB_CODESPACES = ("github", "codespaces")
-    GITHUB_APPS = ("github", "apps")
+    GITHUB_PROJECTS = ("github", "projects")
     GITHUB_SECURITY_ADVISORIES = ("github", "security-advisories")
-    GITHUB_DEPENDENCY_GRAPH = ("github", "dependency-graph")
-    GITHUB_META = ("github", "meta")
+    GITHUB_MIGRATIONS = ("github", "migrations")
+    GITHUB_APPS = ("github", "apps")
+    GITHUB_DEPENDABOT = ("github", "dependabot")
+    GITHUB_EMOJIS = ("github", "emojis")
     GITHUB_LICENSES = ("github", "licenses")
-    GITHUB_REPOS = ("github", "repos")
-    GITHUB_ACTIONS = ("github", "actions")
-    GITHUB_PROJECTS = ("github", "projects")
-    GITHUB_REACTIONS = ("github", "reactions")
-    GITHUB_CODES_OF_CONDUCT = ("github", "codes-of-conduct")
-    GITHUB_INTERACTIONS = ("github", "interactions")
-    GITHUB_PACKAGES = ("github", "packages")
-    GITHUB_PULLS = ("github", "pulls")
-    GITHUB_RATE_LIMIT = ("github", "rate-limit")
+    GITHUB_DEPENDENCY_GRAPH = ("github", "dependency-graph")
     GITHUB_TEAMS = ("github", "teams")
-    GITHUB_BILLING = ("github", "billing")
-    GITHUB_CLASSROOM = ("github", "classroom")
-    GITHUB_MIGRATIONS = ("github", "migrations")
-    GITHUB_MARKDOWN = ("github", "markdown")
-    GITHUB_GIT = ("github", "git")
-    GITHUB_SECRET_SCANNING = ("github", "secret-scanning")
-    GITHUB_CHECKS = ("github", "checks")
-    GITHUB_USERS = ("github", "users")
     GITHUB_IMPORTANT = ("github", "important")
-    GITHUB_DEPENDABOT = ("github", "dependabot")
-    GITHUB_ACTIVITY = ("github", "activity")
-    GITHUB_CODE_SCANNING = ("github", "code-scanning")
+    GITHUB_PULLS = ("github", "pulls")
     GITHUB_ISSUES = ("github", "issues")
+    GITHUB_ACTIONS = ("github", "actions")
+    GITHUB_CODES_OF_CONDUCT = ("github", "codes-of-conduct")
+    GITHUB_USERS = ("github", "users")
+    GITHUB_SECRET_SCANNING = ("github", "secret-scanning")
+    GITHUB_META = ("github", "meta")
+    GITHUB_REACTIONS = ("github", "reactions")
+    GITHUB_GITIGNORE = ("github", "gitignore")
+    GITHUB_MARKDOWN = ("github", "markdown")
+    GITHUB_RATE_LIMIT = ("github", "rate-limit")
+    GITHUB_COPILOT = ("github", "copilot")
     GITHUB_OIDC = ("github", "oidc")
-    GITHUB_EMOJIS = ("github", "emojis")
+    GITHUB_INTERACTIONS = ("github", "interactions")
+    GITHUB_ACTIVITY = ("github", "activity")
+    GITHUB_CLASSROOM = ("github", "classroom")
+    GITHUB_PACKAGES = ("github", "packages")
     GITHUB_ORGS = ("github", "orgs")
-    GITHUB_COPILOT = ("github", "copilot")
+    GITHUB_GIT = ("github", "git")
+    GITHUB_CODE = ("github", "code")
     GITHUB_SEARCH = ("github", "search")
+    GITHUB_CODE_SCANNING = ("github", "code-scanning")
+    GITHUB_CHECKS = ("github", "checks")
+    GITHUB_GISTS = ("github", "gists")
+    GITHUB_REPOS = ("github", "repos")
+    LISTENNOTES_PODCASTER_API = ("listennotes", "Podcaster API")
+    LISTENNOTES_SEARCH_API = ("listennotes", "Search API")
     LISTENNOTES_DIRECTORY_API = ("listennotes", "Directory API")
     LISTENNOTES_PLAYLIST_API = ("listennotes", "Playlist API")
-    LISTENNOTES_SEARCH_API = ("listennotes", "Search API")
-    LISTENNOTES_PODCASTER_API = ("listennotes", "Podcaster API")
     LISTENNOTES_INSIGHTS_API = ("listennotes", "Insights API")
-    NASA_PROJECT = ("nasa", "Project")
-    NASA_ORGANIZATION = ("nasa", "Organization")
     NASA_RESOURCE = ("nasa", "Resource")
-    OKTA_USERTYPE = ("okta", "UserType")
-    OKTA_INLINEHOOK = ("okta", "InlineHook")
-    OKTA_GROUP = ("okta", "Group")
-    OKTA_LINKEDOBJECT = ("okta", "LinkedObject")
-    OKTA_USERSCHEMA = ("okta", "UserSchema")
-    OKTA_AUTHORIZATIONSERVER = ("okta", "AuthorizationServer")
-    OKTA_USERFACTOR = ("okta", "UserFactor")
-    OKTA_BRAND = ("okta", "Brand")
-    OKTA_USER = ("okta", "User")
+    NASA_ORGANIZATION = ("nasa", "Organization")
+    NASA_PROJECT = ("nasa", "Project")
     OKTA_TRUSTEDORIGIN = ("okta", "TrustedOrigin")
-    OKTA_LOG = ("okta", "Log")
-    OKTA_NETWORKZONE = ("okta", "NetworkZone")
-    OKTA_GROUPSCHEMA = ("okta", "GroupSchema")
+    OKTA_SESSION = ("okta", "Session")
     OKTA_THREATINSIGHT = ("okta", "ThreatInsight")
+    OKTA_EVENTHOOK = ("okta", "EventHook")
     OKTA_FEATURE = ("okta", "Feature")
-    OKTA_ORG = ("okta", "Org")
+    OKTA_USERSCHEMA = ("okta", "UserSchema")
     OKTA_SUBSCRIPTION = ("okta", "Subscription")
     OKTA_APPLICATION = ("okta", "Application")
-    OKTA_PROFILEMAPPING = ("okta", "ProfileMapping")
-    OKTA_SESSION = ("okta", "Session")
-    OKTA_POLICY = ("okta", "Policy")
-    OKTA_IDENTITYPROVIDER = ("okta", "IdentityProvider")
-    OKTA_EVENTHOOK = ("okta", "EventHook")
+    OKTA_GROUP = ("okta", "Group")
+    OKTA_USERTYPE = ("okta", "UserType")
+    OKTA_BRAND = ("okta", "Brand")
+    OKTA_LINKEDOBJECT = ("okta", "LinkedObject")
+    OKTA_USER = ("okta", "User")
+    OKTA_GROUPSCHEMA = ("okta", "GroupSchema")
     OKTA_AUTHENTICATOR = ("okta", "Authenticator")
-    OKTA_DOMAIN = ("okta", "Domain")
+    OKTA_ORG = ("okta", "Org")
+    OKTA_IDENTITYPROVIDER = ("okta", "IdentityProvider")
+    OKTA_AUTHORIZATIONSERVER = ("okta", "AuthorizationServer")
+    OKTA_INLINEHOOK = ("okta", "InlineHook")
+    OKTA_PROFILEMAPPING = ("okta", "ProfileMapping")
     OKTA_TEMPLATE = ("okta", "Template")
-    SLACK_TEAM_PROFILE = ("slack", "team.profile")
+    OKTA_DOMAIN = ("okta", "Domain")
+    OKTA_USERFACTOR = ("okta", "UserFactor")
+    OKTA_POLICY = ("okta", "Policy")
+    OKTA_LOG = ("okta", "Log")
+    OKTA_NETWORKZONE = ("okta", "NetworkZone")
     SLACK_BOTS = ("slack", "bots")
-    SLACK_OAUTH_V2 = ("slack", "oauth.v2")
-    SLACK_RTM = ("slack", "rtm")
-    SLACK_ADMIN_INVITEREQUESTS_APPROVED = ("slack", "admin.inviteRequests.approved")
+    SLACK_CONVERSATIONS = ("slack", "conversations")
+    SLACK_CHAT = ("slack", "chat")
+    SLACK_ADMIN_APPS = ("slack", "admin.apps")
+    SLACK_ADMIN_APPS_REQUESTS = ("slack", "admin.apps.requests")
+    SLACK_ADMIN_INVITEREQUESTS_DENIED = ("slack", "admin.inviteRequests.denied")
     SLACK_APPS = ("slack", "apps")
+    SLACK_ADMIN_USERS = ("slack", "admin.users")
+    SLACK_CALLS = ("slack", "calls")
+    SLACK_ADMIN = ("slack", "admin")
+    SLACK_RTM = ("slack", "rtm")
+    SLACK_TEAM = ("slack", "team")
+    SLACK_USERGROUPS_USERS = ("slack", "usergroups.users")
+    SLACK_APPS_PERMISSIONS_RESOURCES = ("slack", "apps.permissions.resources")
+    SLACK_APPS_PERMISSIONS_USERS = ("slack", "apps.permissions.users")
+    SLACK_USERGROUPS = ("slack", "usergroups")
+    SLACK_IMPORTANT = ("slack", "important")
+    SLACK_AUTH = ("slack", "auth")
+    SLACK_ADMIN_CONVERSATIONS_EKM = ("slack", "admin.conversations.ekm")
+    SLACK_ADMIN_CONVERSATIONS_RESTRICTACCESS = ("slack", "admin.conversations.restrictAccess")
+    SLACK_ADMIN_TEAMS_SETTINGS = ("slack", "admin.teams.settings")
+    SLACK_CHAT_SCHEDULEDMESSAGES = ("slack", "chat.scheduledMessages")
     SLACK_ADMIN_TEAMS = ("slack", "admin.teams")
+    SLACK_API = ("slack", "api")
+    SLACK_ADMIN_INVITEREQUESTS_APPROVED = ("slack", "admin.inviteRequests.approved")
     SLACK_APPS_PERMISSIONS = ("slack", "apps.permissions")
-    SLACK_ADMIN_APPS = ("slack", "admin.apps")
-    SLACK_ADMIN_TEAMS_SETTINGS = ("slack", "admin.teams.settings")
-    SLACK_CALLS_PARTICIPANTS = ("slack", "calls.participants")
-    SLACK_STARS = ("slack", "stars")
-    SLACK_ADMIN_CONVERSATIONS_RESTRICTACCESS = ("slack", "admin.conversations.restrictAccess")
-    SLACK_WORKFLOWS = ("slack", "workflows")
-    SLACK_ADMIN_USERGROUPS = ("slack", "admin.usergroups")
-    SLACK_ADMIN_CONVERSATIONS = ("slack", "admin.conversations")
+    SLACK_USERS = ("slack", "users")
+    SLACK_ADMIN_TEAMS_ADMINS = ("slack", "admin.teams.admins")
+    SLACK_FILES_REMOTE = ("slack", "files.remote")
     SLACK_ADMIN_TEAMS_OWNERS = ("slack", "admin.teams.owners")
-    SLACK_CALLS = ("slack", "calls")
-    SLACK_FILES = ("slack", "files")
     SLACK_REACTIONS = ("slack", "reactions")
-    SLACK_APPS_PERMISSIONS_USERS = ("slack", "apps.permissions.users")
+    SLACK_DIALOG = ("slack", "dialog")
+    SLACK_APPS_PERMISSIONS_SCOPES = ("slack", "apps.permissions.scopes")
+    SLACK_TEAM_PROFILE = ("slack", "team.profile")
+    SLACK_PINS = ("slack", "pins")
     SLACK_ADMIN_USERS_SESSION = ("slack", "admin.users.session")
-    SLACK_APPS_PERMISSIONS_RESOURCES = ("slack", "apps.permissions.resources")
-    SLACK_DND = ("slack", "dnd")
-    SLACK_ADMIN_APPS_RESTRICTED = ("slack", "admin.apps.restricted")
-    SLACK_CONVERSATIONS = ("slack", "conversations")
     SLACK_EMOJI = ("slack", "emoji")
-    SLACK_ADMIN_INVITEREQUESTS = ("slack", "admin.inviteRequests")
-    SLACK_USERGROUPS = ("slack", "usergroups")
-    SLACK_ADMIN_APPS_APPROVED = ("slack", "admin.apps.approved")
-    SLACK_TEAM = ("slack", "team")
-    SLACK_FILES_REMOTE = ("slack", "files.remote")
-    SLACK_ADMIN_APPS_REQUESTS = ("slack", "admin.apps.requests")
-    SLACK_DIALOG = ("slack", "dialog")
     SLACK_FILES_COMMENTS = ("slack", "files.comments")
-    SLACK_APPS_EVENT_AUTHORIZATIONS = ("slack", "apps.event.authorizations")
-    SLACK_ADMIN = ("slack", "admin")
-    SLACK_CHAT_SCHEDULEDMESSAGES = ("slack", "chat.scheduledMessages")
-    SLACK_USERS = ("slack", "users")
-    SLACK_VIEWS = ("slack", "views")
-    SLACK_IMPORTANT = ("slack", "important")
-    SLACK_CHAT = ("slack", "chat")
     SLACK_OAUTH = ("slack", "oauth")
-    SLACK_AUTH = ("slack", "auth")
-    SLACK_ADMIN_USERS = ("slack", "admin.users")
-    SLACK_ADMIN_INVITEREQUESTS_DENIED = ("slack", "admin.inviteRequests.denied")
-    SLACK_USERGROUPS_USERS = ("slack", "usergroups.users")
-    SLACK_API = ("slack", "api")
+    SLACK_STARS = ("slack", "stars")
+    SLACK_MIGRATION = ("slack", "migration")
+    SLACK_DND = ("slack", "dnd")
     SLACK_REMINDERS = ("slack", "reminders")
     SLACK_ADMIN_EMOJI = ("slack", "admin.emoji")
-    SLACK_PINS = ("slack", "pins")
-    SLACK_MIGRATION = ("slack", "migration")
-    SLACK_ADMIN_CONVERSATIONS_EKM = ("slack", "admin.conversations.ekm")
-    SLACK_USERS_PROFILE = ("slack", "users.profile")
-    SLACK_ADMIN_TEAMS_ADMINS = ("slack", "admin.teams.admins")
-    SLACK_APPS_PERMISSIONS_SCOPES = ("slack", "apps.permissions.scopes")
+    SLACK_APPS_EVENT_AUTHORIZATIONS = ("slack", "apps.event.authorizations")
+    SLACK_ADMIN_USERGROUPS = ("slack", "admin.usergroups")
+    SLACK_ADMIN_APPS_APPROVED = ("slack", "admin.apps.approved")
+    SLACK_ADMIN_APPS_RESTRICTED = ("slack", "admin.apps.restricted")
+    SLACK_CALLS_PARTICIPANTS = ("slack", "calls.participants")
+    SLACK_OAUTH_V2 = ("slack", "oauth.v2")
+    SLACK_VIEWS = ("slack", "views")
+    SLACK_FILES = ("slack", "files")
     SLACK_SEARCH = ("slack", "search")
-    SLACKBOT_TEAM_PROFILE = ("slackbot", "team.profile")
+    SLACK_USERS_PROFILE = ("slack", "users.profile")
+    SLACK_ADMIN_INVITEREQUESTS = ("slack", "admin.inviteRequests")
+    SLACK_ADMIN_CONVERSATIONS = ("slack", "admin.conversations")
+    SLACK_WORKFLOWS = ("slack", "workflows")
     SLACKBOT_BOTS = ("slackbot", "bots")
-    SLACKBOT_OAUTH_V2 = ("slackbot", "oauth.v2")
+    SLACKBOT_CONVERSATIONS = ("slackbot", "conversations")
+    SLACKBOT_CHAT = ("slackbot", "chat")
     SLACKBOT_APPS = ("slackbot", "apps")
-    SLACKBOT_APPS_PERMISSIONS = ("slackbot", "apps.permissions")
-    SLACKBOT_CALLS_PARTICIPANTS = ("slackbot", "calls.participants")
-    SLACKBOT_STARS = ("slackbot", "stars")
-    SLACKBOT_WORKFLOWS = ("slackbot", "workflows")
     SLACKBOT_CALLS = ("slackbot", "calls")
-    SLACKBOT_FILES = ("slackbot", "files")
-    SLACKBOT_REACTIONS = ("slackbot", "reactions")
-    SLACKBOT_APPS_PERMISSIONS_USERS = ("slackbot", "apps.permissions.users")
+    SLACKBOT_RTM = ("slackbot", "rtm")
+    SLACKBOT_TEAM = ("slackbot", "team")
+    SLACKBOT_USERGROUPS_USERS = ("slackbot", "usergroups.users")
     SLACKBOT_APPS_PERMISSIONS_RESOURCES = ("slackbot", "apps.permissions.resources")
-    SLACKBOT_DND = ("slackbot", "dnd")
-    SLACKBOT_EMOJI = ("slackbot", "emoji")
-    SLACKBOT_CONVERSATIONS = ("slackbot", "conversations")
+    SLACKBOT_APPS_PERMISSIONS_USERS = ("slackbot", "apps.permissions.users")
     SLACKBOT_USERGROUPS = ("slackbot", "usergroups")
-    SLACKBOT_TEAM = ("slackbot", "team")
-    SLACKBOT_FILES_REMOTE = ("slackbot", "files.remote")
-    SLACKBOT_FILES_COMMENTS = ("slackbot", "files.comments")
-    SLACKBOT_DIALOG = ("slackbot", "dialog")
-    SLACKBOT_APPS_EVENT_AUTHORIZATIONS = ("slackbot", "apps.event.authorizations")
-    SLACKBOT_USERS = ("slackbot", "users")
-    SLACKBOT_VIEWS = ("slackbot", "views")
     SLACKBOT_IMPORTANT = ("slackbot", "important")
-    SLACKBOT_CHAT = ("slackbot", "chat")
-    SLACKBOT_OAUTH = ("slackbot", "oauth")
     SLACKBOT_AUTH = ("slackbot", "auth")
-    SLACKBOT_USERGROUPS_USERS = ("slackbot", "usergroups.users")
+    SLACKBOT_CHAT_SCHEDULEDMESSAGES = ("slackbot", "chat.scheduledMessages")
     SLACKBOT_API = ("slackbot", "api")
-    SLACKBOT_REMINDERS = ("slackbot", "reminders")
+    SLACKBOT_USERS = ("slackbot", "users")
+    SLACKBOT_APPS_PERMISSIONS = ("slackbot", "apps.permissions")
+    SLACKBOT_FILES_REMOTE = ("slackbot", "files.remote")
+    SLACKBOT_REACTIONS = ("slackbot", "reactions")
+    SLACKBOT_DIALOG = ("slackbot", "dialog")
+    SLACKBOT_APPS_PERMISSIONS_SCOPES = ("slackbot", "apps.permissions.scopes")
+    SLACKBOT_TEAM_PROFILE = ("slackbot", "team.profile")
     SLACKBOT_PINS = ("slackbot", "pins")
+    SLACKBOT_EMOJI = ("slackbot", "emoji")
+    SLACKBOT_FILES_COMMENTS = ("slackbot", "files.comments")
+    SLACKBOT_OAUTH = ("slackbot", "oauth")
+    SLACKBOT_STARS = ("slackbot", "stars")
     SLACKBOT_MIGRATION = ("slackbot", "migration")
-    SLACKBOT_RTM = ("slackbot", "rtm")
+    SLACKBOT_DND = ("slackbot", "dnd")
+    SLACKBOT_REMINDERS = ("slackbot", "reminders")
+    SLACKBOT_APPS_EVENT_AUTHORIZATIONS = ("slackbot", "apps.event.authorizations")
+    SLACKBOT_CALLS_PARTICIPANTS = ("slackbot", "calls.participants")
+    SLACKBOT_VIEWS = ("slackbot", "views")
+    SLACKBOT_OAUTH_V2 = ("slackbot", "oauth.v2")
+    SLACKBOT_FILES = ("slackbot", "files")
     SLACKBOT_USERS_PROFILE = ("slackbot", "users.profile")
-    SLACKBOT_CHAT_SCHEDULEDMESSAGES = ("slackbot", "chat.scheduledMessages")
-    SLACKBOT_APPS_PERMISSIONS_SCOPES = ("slackbot", "apps.permissions.scopes")
+    SLACKBOT_WORKFLOWS = ("slackbot", "workflows")
+    SPOTIFY_PLAYER = ("spotify", "Player")
+    SPOTIFY_LIBRARY = ("spotify", "Library")
     SPOTIFY_GENRES = ("spotify", "Genres")
-    SPOTIFY_MARKETS = ("spotify", "Markets")
-    SPOTIFY_USERS = ("spotify", "Users")
-    SPOTIFY_ARTISTS = ("spotify", "Artists")
     SPOTIFY_AUDIOBOOKS = ("spotify", "Audiobooks")
     SPOTIFY_ALBUMS = ("spotify", "Albums")
-    SPOTIFY_TRACKS = ("spotify", "Tracks")
-    SPOTIFY_CHAPTERS = ("spotify", "Chapters")
-    SPOTIFY_SEARCH = ("spotify", "Search")
+    SPOTIFY_MARKETS = ("spotify", "Markets")
+    SPOTIFY_SHOWS = ("spotify", "Shows")
     SPOTIFY_PLAYLISTS = ("spotify", "Playlists")
-    SPOTIFY_PLAYER = ("spotify", "Player")
-    SPOTIFY_EPISODES = ("spotify", "Episodes")
+    SPOTIFY_ARTISTS = ("spotify", "Artists")
     SPOTIFY_CATEGORIES = ("spotify", "Categories")
-    SPOTIFY_SHOWS = ("spotify", "Shows")
-    SPOTIFY_LIBRARY = ("spotify", "Library")
-    TASKADE_FOLDER = ("taskade", "Folder")
+    SPOTIFY_EPISODES = ("spotify", "Episodes")
+    SPOTIFY_USERS = ("spotify", "Users")
+    SPOTIFY_SEARCH = ("spotify", "Search")
+    SPOTIFY_TRACKS = ("spotify", "Tracks")
+    SPOTIFY_CHAPTERS = ("spotify", "Chapters")
+    TASKADE_WORKSPACE = ("taskade", "Workspace")
+    TASKADE_AGENT = ("taskade", "Agent")
     TASKADE_ME = ("taskade", "Me")
+    TASKADE_FOLDER = ("taskade", "Folder")
     TASKADE_TASK = ("taskade", "Task")
-    TASKADE_WORKSPACE = ("taskade", "Workspace")
     TASKADE_PROJECT = ("taskade", "Project")
-    TASKADE_AGENT = ("taskade", "Agent")
-    WHATSAPP_HEALTH = ("whatsapp", "Health")
-    WHATSAPP_BUSINESS_PROFILE = ("whatsapp", "Business Profile")
-    WHATSAPP_USERS = ("whatsapp", "Users")
-    WHATSAPP_CERTIFICATES = ("whatsapp", "Certificates")
-    WHATSAPP_CONTACTS = ("whatsapp", "Contacts")
-    WHATSAPP_PROFILE = ("whatsapp", "Profile")
     WHATSAPP_APPLICATION = ("whatsapp", "Application")
-    WHATSAPP_GROUPS = ("whatsapp", "Groups")
-    WHATSAPP_BACKUP_RESTORE = ("whatsapp", "Backup/Restore")
     WHATSAPP_REGISTRATION = ("whatsapp", "Registration")
-    WHATSAPP_MEDIA = ("whatsapp", "Media")
+    WHATSAPP_USERS = ("whatsapp", "Users")
+    WHATSAPP_GROUPS = ("whatsapp", "Groups")
+    WHATSAPP_CONTACTS = ("whatsapp", "Contacts")
     WHATSAPP_MESSAGES = ("whatsapp", "Messages")
+    WHATSAPP_HEALTH = ("whatsapp", "Health")
+    WHATSAPP_PROFILE = ("whatsapp", "Profile")
     WHATSAPP_TWO_STEP_VERIFICATION = ("whatsapp", "Two-Step Verification")
-    ZOOM_WEBINARS = ("zoom", "Webinars")
-    ZOOM_REPORTS = ("zoom", "Reports")
-    ZOOM_SIP_PHONE = ("zoom", "SIP Phone")
-    ZOOM_TSP = ("zoom", "TSP")
-    ZOOM_ARCHIVING = ("zoom", "Archiving")
-    ZOOM_MEETINGS = ("zoom", "Meetings")
-    ZOOM_DEVICES = ("zoom", "Devices")
+    WHATSAPP_CERTIFICATES = ("whatsapp", "Certificates")
+    WHATSAPP_MEDIA = ("whatsapp", "Media")
+    WHATSAPP_BACKUP_RESTORE = ("whatsapp", "Backup/Restore")
+    WHATSAPP_BUSINESS_PROFILE = ("whatsapp", "Business Profile")
     ZOOM_H323_DEVICES = ("zoom", "H323 Devices")
-    ZOOM_CLOUD_RECORDING = ("zoom", "Cloud Recording")
     ZOOM_PAC = ("zoom", "PAC")
+    ZOOM_MEETINGS = ("zoom", "Meetings")
+    ZOOM_CLOUD_RECORDING = ("zoom", "Cloud Recording")
+    ZOOM_SIP_PHONE = ("zoom", "SIP Phone")
     ZOOM_TRACKING_FIELD = ("zoom", "Tracking Field")
+    ZOOM_ARCHIVING = ("zoom", "Archiving")
+    ZOOM_TSP = ("zoom", "TSP")
+    ZOOM_REPORTS = ("zoom", "Reports")
+    ZOOM_DEVICES = ("zoom", "Devices")
+    ZOOM_WEBINARS = ("zoom", "Webinars")
 
 
 
 
 class App(str, Enum):
     """Composio App."""
 
@@ -3535,34 +3535,34 @@
     ZOOM_WEB_IN_ARS_GETS_IP_URI_WITH_PASS_CODE = ("zoom", "zoom_web_in_ars_gets_ip_uri_with_pass_code", False)
     ZOOM_WEB_IN_ARS_UPDATE_STATUS = ("zoom", "zoom_web_in_ars_update_status", False)
     ZOOM_WEB_IN_ARS_GET_SURVEY = ("zoom", "zoom_web_in_ars_get_survey", False)
     ZOOM_WEB_IN_ARS_DELETE_SURVEY = ("zoom", "zoom_web_in_ars_delete_survey", False)
     ZOOM_WEB_IN_ARS_UPDATE_SURVEY = ("zoom", "zoom_web_in_ars_update_survey", False)
     ZOOM_WEB_IN_ARS_GET_WEB_IN_ART_OKEN = ("zoom", "zoom_web_in_ars_get_web_in_art_oken", False)
     ZOOM_WEB_IN_ARS_LIST_TRACKING_SOURCES = ("zoom", "zoom_web_in_ars_list_tracking_sources", False)
-    CALCULATOR = ("mathematical", "mathematical_calculator", True, True)
-    WORKSPACESTATUSACTION = ("localworkspace", "localworkspace_workspacestatusaction", True, True)
-    CREATEWORKSPACEACTION = ("localworkspace", "localworkspace_createworkspaceaction", True, True)
-    FINDFILECMD = ("cmdmanagertool", "cmdmanagertool_findfilecmd", True, True)
-    CREATEFILECMD = ("cmdmanagertool", "cmdmanagertool_createfilecmd", True, True)
-    GOTOLINENUMINOPENFILE = ("cmdmanagertool", "cmdmanagertool_gotolinenuminopenfile", True, True)
-    OPENFILE = ("cmdmanagertool", "cmdmanagertool_openfile", True, True)
-    SCROLL = ("cmdmanagertool", "cmdmanagertool_scroll", True, True)
-    SEARCHFILECMD = ("cmdmanagertool", "cmdmanagertool_searchfilecmd", True, True)
-    SEARCHDIRCMD = ("cmdmanagertool", "cmdmanagertool_searchdircmd", True, True)
-    EDITFILE = ("cmdmanagertool", "cmdmanagertool_editfile", True, True)
-    RUNCOMMANDONWORKSPACE = ("cmdmanagertool", "cmdmanagertool_runcommandonworkspace", True, True)
-    GETCURRENTDIRCMD = ("cmdmanagertool", "cmdmanagertool_getcurrentdircmd", True, True)
-    GITHUBCLONECMD = ("cmdmanagertool", "cmdmanagertool_githubclonecmd", True, True)
-    GETWORKSPACEHISTORY = ("historykeeper", "historykeeper_getworkspacehistory", True, True)
-    RAGTOOLQUERY = ("ragtool", "ragtool_ragtoolquery", True, True)
-    ADDCONTENTTORAGTOOL = ("ragtool", "ragtool_addcontenttoragtool", True, True)
-    SCRAPEWEBSITECONTENT = ("webtool", "webtool_scrapewebsitecontent", True, True)
-    SCRAPEWEBSITEELEMENT = ("webtool", "webtool_scrapewebsiteelement", True, True)
-    CODEQUERY = ("greptile", "greptile_codequery", True, True)
+    MATHEMATICAL_CALCULATOR = ("mathematical", "mathematical_calculator", True, True)
+    LOCALWORKSPACE_WORKSPACESTATUSACTION = ("localworkspace", "localworkspace_workspacestatusaction", True, True)
+    LOCALWORKSPACE_CREATEWORKSPACEACTION = ("localworkspace", "localworkspace_createworkspaceaction", True, True)
+    CMDMANAGERTOOL_FINDFILECMD = ("cmdmanagertool", "cmdmanagertool_findfilecmd", True, True)
+    CMDMANAGERTOOL_CREATEFILECMD = ("cmdmanagertool", "cmdmanagertool_createfilecmd", True, True)
+    CMDMANAGERTOOL_GOTOLINENUMINOPENFILE = ("cmdmanagertool", "cmdmanagertool_gotolinenuminopenfile", True, True)
+    CMDMANAGERTOOL_OPENFILE = ("cmdmanagertool", "cmdmanagertool_openfile", True, True)
+    CMDMANAGERTOOL_SCROLL = ("cmdmanagertool", "cmdmanagertool_scroll", True, True)
+    CMDMANAGERTOOL_SEARCHFILECMD = ("cmdmanagertool", "cmdmanagertool_searchfilecmd", True, True)
+    CMDMANAGERTOOL_SEARCHDIRCMD = ("cmdmanagertool", "cmdmanagertool_searchdircmd", True, True)
+    CMDMANAGERTOOL_EDITFILE = ("cmdmanagertool", "cmdmanagertool_editfile", True, True)
+    CMDMANAGERTOOL_RUNCOMMANDONWORKSPACE = ("cmdmanagertool", "cmdmanagertool_runcommandonworkspace", True, True)
+    CMDMANAGERTOOL_GETCURRENTDIRCMD = ("cmdmanagertool", "cmdmanagertool_getcurrentdircmd", True, True)
+    CMDMANAGERTOOL_GITHUBCLONECMD = ("cmdmanagertool", "cmdmanagertool_githubclonecmd", True, True)
+    HISTORYKEEPER_GETWORKSPACEHISTORY = ("historykeeper", "historykeeper_getworkspacehistory", True, True)
+    RAGTOOL_RAGTOOLQUERY = ("ragtool", "ragtool_ragtoolquery", True, True)
+    RAGTOOL_ADDCONTENTTORAGTOOL = ("ragtool", "ragtool_addcontenttoragtool", True, True)
+    WEBTOOL_SCRAPEWEBSITECONTENT = ("webtool", "webtool_scrapewebsitecontent", True, True)
+    WEBTOOL_SCRAPEWEBSITEELEMENT = ("webtool", "webtool_scrapewebsiteelement", True, True)
+    GREPTILE_CODEQUERY = ("greptile", "greptile_codequery", True, True)
 
 
 
 class Trigger(tuple, Enum):
     """App trigger."""
 
     @property
```

### Comparing `composio_core-0.3.6/composio/client/exceptions.py` & `composio_core-0.3.7/composio/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/client/http.py` & `composio_core-0.3.7/composio/client/http.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/client/local_handler.py` & `composio_core-0.3.7/composio/client/local_handler.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/constants.py` & `composio_core-0.3.7/composio/constants.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/core/local/action.py` & `composio_core-0.3.7/composio/core/local/action.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/core/local/tool.py` & `composio_core-0.3.7/composio/core/local/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/exceptions.py` & `composio_core-0.3.7/composio/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/file/actions/read_file.py` & `composio_core-0.3.7/composio/local_tools/file/actions/read_file.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/file/actions/write_file.py` & `composio_core-0.3.7/composio/local_tools/file/actions/write_file.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/greptile/actions/codequery.py` & `composio_core-0.3.7/composio/local_tools/greptile/actions/codequery.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/cmd_manager/tool.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/cmd_manager/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/commons/command_runner_model.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/commons/command_runner_model.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/commons/history_processor.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/commons/history_processor.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/commons/local_docker_workspace.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/commons/local_docker_workspace.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/commons/parsing.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/commons/parsing.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/commons/utils.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/commons/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/history_keeper/tool.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/history_keeper/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/workspace/actions/create_workspace.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/workspace/actions/create_workspace.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/workspace/actions/workspace_status.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/workspace/actions/workspace_status.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/local_workspace/workspace/tool.py` & `composio_core-0.3.7/composio/local_tools/local_workspace/workspace/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/mathematical/actions/calculator.py` & `composio_core-0.3.7/composio/local_tools/mathematical/actions/calculator.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/ragtool/actions/rag_add_request.py` & `composio_core-0.3.7/composio/local_tools/ragtool/actions/rag_add_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Tool for adding content to the knowledge base
     """
 
     _display_name = "Add Content to Rag Tool"
     _request_schema = RagToolAddRequest
     _response_schema = RagToolAddResponse
     _tags = ["Knowledge Base"]
-    _tool_name = "ragtoolactions"
+    _tool_name = "ragtool"
 
     def execute(self, request: RagToolAddRequest, authorisation_data: dict = {}):
         """Add content to the knowledge base"""
         try:
             from embedchain import App
         except ImportError as e:
             raise ImportError(f"Failed to import App from embedchain: {e}")
```

### Comparing `composio_core-0.3.6/composio/local_tools/ragtool/actions/rag_query.py` & `composio_core-0.3.7/composio/local_tools/ragtool/actions/rag_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     this can only be performed after AddContentToRagTool
     """
 
     _display_name = "Rag Tool"
     _request_schema = RagToolQueryRequest
     _response_schema = RagToolQueryResponse
     _tags = ["Knowledge Base"]
-    _tool_name = "ragtoolactions"
+    _tool_name = "ragtool"
 
 
     def execute(self, request: RagToolQueryRequest, authorisation_data: dict = {}):
         """Query the knowledge base and return the response"""
         try:
             from embedchain import App
         except ImportError as e:
```

### Comparing `composio_core-0.3.6/composio/local_tools/webtool/actions/scrape_website_content.py` & `composio_core-0.3.7/composio/local_tools/webtool/actions/scrape_website_content.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/local_tools/webtool/actions/scrape_website_element.py` & `composio_core-0.3.7/composio/local_tools/webtool/actions/scrape_website_element.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/storage/base.py` & `composio_core-0.3.7/composio/storage/base.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/tools/__init__.py` & `composio_core-0.3.7/composio/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/tools/schema.py` & `composio_core-0.3.7/composio/tools/schema.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/utils/decorators.py` & `composio_core-0.3.7/composio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/utils/git.py` & `composio_core-0.3.7/composio/utils/git.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/utils/shared.py` & `composio_core-0.3.7/composio/utils/shared.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio/utils/url.py` & `composio_core-0.3.7/composio/utils/url.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/composio_core.egg-info/PKG-INFO` & `composio_core-0.3.7/composio_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.6
+Version: 0.3.7
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.6/composio_core.egg-info/SOURCES.txt` & `composio_core-0.3.7/composio_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.6/setup.py` & `composio_core-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="composio_core",
-    version="0.3.6",
+    version="0.3.7",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

