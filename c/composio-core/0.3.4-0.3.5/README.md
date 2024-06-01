# Comparing `tmp/composio_core-0.3.4.tar.gz` & `tmp/composio_core-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.3.4.tar", last modified: Sat Jun  1 00:39:12 2024, max compression
+gzip compressed data, was "composio_core-0.3.5.tar", last modified: Sat Jun  1 01:15:45 2024, max compression
```

## Comparing `composio_core-0.3.4.tar` & `composio_core-0.3.5.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.756622 composio_core-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-01 00:38:03.000000 composio_core-0.3.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 00:39:12.756622 composio_core-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-06-01 00:38:03.000000 composio_core-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.740622 composio_core-0.3.4/composio/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/add.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8536 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/cli/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/client/
--rw-r--r--   0 runner    (1001) docker     (127)    32419 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)   316458 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/client/local_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/file/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/file/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/actions/read_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/file/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/greptile/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/greptile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/greptile/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/greptile/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/greptile/actions/codequery.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/greptile/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/local_workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.744622 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/command_runner_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/get_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/history_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/local_docker_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/local_workspace/workspace/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.748622 composio_core-0.3.4/composio/local_tools/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/mathematical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/mathematical/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/local_tools/ragtool/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/local_tools/ragtool/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/actions/rag_add_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/actions/rag_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/ragtool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/local_tools/webtool/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/local_tools/webtool/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/actions/scrape_website_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/actions/scrape_website_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/local_tools/webtool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/storage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/tools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.752622 composio_core-0.3.4/composio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 00:38:03.000000 composio_core-0.3.4/composio/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:39:12.756622 composio_core-0.3.4/composio_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 00:39:12.000000 composio_core-0.3.4/composio_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:39:12.756622 composio_core-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-01 00:38:03.000000 composio_core-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.684438 composio_core-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-01 01:15:28.000000 composio_core-0.3.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 01:15:45.684438 composio_core-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-06-01 01:15:28.000000 composio_core-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.668438 composio_core-0.3.5/composio/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.668438 composio_core-0.3.5/composio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/add.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8536 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/cli/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.672438 composio_core-0.3.5/composio/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    32419 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)   316458 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/client/local_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.672438 composio_core-0.3.5/composio/local_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.672438 composio_core-0.3.5/composio/local_tools/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.672438 composio_core-0.3.5/composio/local_tools/file/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/file/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/file/actions/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/file/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/file/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.672438 composio_core-0.3.5/composio/local_tools/greptile/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/greptile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.672438 composio_core-0.3.5/composio/local_tools/greptile/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/greptile/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/greptile/actions/codequery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/greptile/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.672438 composio_core-0.3.5/composio/local_tools/local_workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.672438 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.676438 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.676438 composio_core-0.3.5/composio/local_tools/local_workspace/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/commons/command_runner_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/commons/get_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/commons/history_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/commons/local_docker_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/commons/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.676438 composio_core-0.3.5/composio/local_tools/local_workspace/history_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/history_keeper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.676438 composio_core-0.3.5/composio/local_tools/local_workspace/history_keeper/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/history_keeper/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.676438 composio_core-0.3.5/composio/local_tools/local_workspace/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.676438 composio_core-0.3.5/composio/local_tools/local_workspace/workspace/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/workspace/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/local_workspace/workspace/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.676438 composio_core-0.3.5/composio/local_tools/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/mathematical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/mathematical/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.680438 composio_core-0.3.5/composio/local_tools/ragtool/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/ragtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.680438 composio_core-0.3.5/composio/local_tools/ragtool/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/ragtool/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/ragtool/actions/rag_add_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/ragtool/actions/rag_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/ragtool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.680438 composio_core-0.3.5/composio/local_tools/webtool/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/webtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.680438 composio_core-0.3.5/composio/local_tools/webtool/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/webtool/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/webtool/actions/scrape_website_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/webtool/actions/scrape_website_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/local_tools/webtool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.680438 composio_core-0.3.5/composio/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/storage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.680438 composio_core-0.3.5/composio/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.680438 composio_core-0.3.5/composio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/utils/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-01 01:15:28.000000 composio_core-0.3.5/composio/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:45.684438 composio_core-0.3.5/composio_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-06-01 01:15:45.000000 composio_core-0.3.5/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-06-01 01:15:45.000000 composio_core-0.3.5/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:15:45.000000 composio_core-0.3.5/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 01:15:45.000000 composio_core-0.3.5/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 01:15:45.000000 composio_core-0.3.5/composio_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 01:15:45.000000 composio_core-0.3.5/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:15:45.684438 composio_core-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-01 01:15:28.000000 composio_core-0.3.5/setup.py
```

### Comparing `composio_core-0.3.4/PKG-INFO` & `composio_core-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.4
+Version: 0.3.5
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.4/README.md` & `composio_core-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/__init__.py` & `composio_core-0.3.5/composio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/actions.py` & `composio_core-0.3.5/composio/cli/actions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/add.py` & `composio_core-0.3.5/composio/cli/add.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/apps.py` & `composio_core-0.3.5/composio/cli/apps.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/connections.py` & `composio_core-0.3.5/composio/cli/connections.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/context.py` & `composio_core-0.3.5/composio/cli/context.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/integrations.py` & `composio_core-0.3.5/composio/cli/integrations.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/login.py` & `composio_core-0.3.5/composio/cli/login.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/cli/triggers.py` & `composio_core-0.3.5/composio/cli/triggers.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/client/__init__.py` & `composio_core-0.3.5/composio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/client/endpoints.py` & `composio_core-0.3.5/composio/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/client/enums.py` & `composio_core-0.3.5/composio/client/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/client/exceptions.py` & `composio_core-0.3.5/composio/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/client/http.py` & `composio_core-0.3.5/composio/client/http.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/client/local_handler.py` & `composio_core-0.3.5/composio/client/local_handler.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/constants.py` & `composio_core-0.3.5/composio/constants.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/exceptions.py` & `composio_core-0.3.5/composio/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/file/actions/read_file.py` & `composio_core-0.3.5/composio/local_tools/file/actions/read_file.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/file/actions/write_file.py` & `composio_core-0.3.5/composio/local_tools/file/actions/write_file.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/greptile/actions/codequery.py` & `composio_core-0.3.5/composio/local_tools/greptile/actions/codequery.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/base_class.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/clone_github.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/cmd_manager/tool.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/cmd_manager/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/commons/command_runner_model.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/commons/command_runner_model.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/commons/history_processor.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/commons/history_processor.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/commons/local_docker_workspace.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/commons/local_docker_workspace.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/commons/parsing.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/commons/parsing.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/commons/utils.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/commons/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/history_keeper/tool.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/history_keeper/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/workspace/actions/base_workspace_action.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/create_workspace.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/workspace/actions/create_workspace.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/workspace/actions/workspace_status.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/workspace/actions/workspace_status.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/local_workspace/workspace/tool.py` & `composio_core-0.3.5/composio/local_tools/local_workspace/workspace/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/ragtool/actions/rag_add_request.py` & `composio_core-0.3.5/composio/local_tools/ragtool/actions/rag_add_request.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/ragtool/actions/rag_query.py` & `composio_core-0.3.5/composio/local_tools/ragtool/actions/rag_query.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/webtool/actions/scrape_website_content.py` & `composio_core-0.3.5/composio/local_tools/webtool/actions/scrape_website_content.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/local_tools/webtool/actions/scrape_website_element.py` & `composio_core-0.3.5/composio/local_tools/webtool/actions/scrape_website_element.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/storage/base.py` & `composio_core-0.3.5/composio/storage/base.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/tools/__init__.py` & `composio_core-0.3.5/composio/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/tools/schema.py` & `composio_core-0.3.5/composio/tools/schema.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/utils/decorators.py` & `composio_core-0.3.5/composio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/utils/git.py` & `composio_core-0.3.5/composio/utils/git.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/utils/shared.py` & `composio_core-0.3.5/composio/utils/shared.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio/utils/url.py` & `composio_core-0.3.5/composio/utils/url.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/composio_core.egg-info/PKG-INFO` & `composio_core-0.3.5/composio_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.4
+Version: 0.3.5
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.4/composio_core.egg-info/SOURCES.txt` & `composio_core-0.3.5/composio_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.4/setup.py` & `composio_core-0.3.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="composio_core",
-    version="0.3.4",
+    version="0.3.5",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

