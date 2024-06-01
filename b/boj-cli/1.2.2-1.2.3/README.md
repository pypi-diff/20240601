# Comparing `tmp/boj-cli-1.2.2.tar.gz` & `tmp/boj-cli-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boj-cli-1.2.2.tar", last modified: Fri Feb 23 21:16:52 2024, max compression
+gzip compressed data, was "boj-cli-1.2.3.tar", last modified: Sat Jun  1 08:17:37 2024, max compression
```

## Comparing `boj-cli-1.2.2.tar` & `boj-cli-1.2.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.801716 boj-cli-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.785716 boj-cli-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.github/major-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.github/minor-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.github/patch-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.github/release-template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.785716 boj-cli-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.github/workflows/run-test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.785716 boj-cli-1.2.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.idea/boj-cli.iml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.785716 boj-cli-1.2.2/.idea/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.idea/dictionaries/jerry.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.785716 boj-cli-1.2.2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-23 21:16:32.000000 boj-cli-1.2.2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-23 21:16:32.000000 boj-cli-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-02-23 21:16:52.801716 boj-cli-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-02-23 21:16:32.000000 boj-cli-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/args_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/browsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/browsers/login_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/add/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/add/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/case/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/case/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/clean/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/clean/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/init/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/init/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/login/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/login/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/open/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/open/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/open/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/random/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/random/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.789716 boj-cli-1.2.2/boj/commands/run/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/run/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/run/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.793716 boj-cli-1.2.2/boj/commands/submit/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/submit/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/submit/progress_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/commands/submit/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.793716 boj-cli-1.2.2/boj/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.793716 boj-cli-1.2.2/boj/core/fs/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/fs/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/fs/file_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/fs/file_search_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/fs/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/fs/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/fs/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/core/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.797716 boj-cli-1.2.2/boj/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/data/boj_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/data/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/data/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/data/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/data/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.797716 boj-cli-1.2.2/boj/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/web/boj_main_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/web/boj_problem_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/web/boj_status_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/web/boj_submit_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-23 21:16:32.000000 boj-cli-1.2.2/boj/web/solved_ac_search_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.797716 boj-cli-1.2.2/boj_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-02-23 21:16:52.000000 boj-cli-1.2.2/boj_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-02-23 21:16:52.000000 boj-cli-1.2.2/boj_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 21:16:52.000000 boj-cli-1.2.2/boj_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 21:16:52.000000 boj-cli-1.2.2/boj_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-23 21:16:52.000000 boj-cli-1.2.2/boj_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-23 21:16:52.000000 boj-cli-1.2.2/boj_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-02-23 21:16:32.000000 boj-cli-1.2.2/config_example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-23 21:16:32.000000 boj-cli-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-23 21:16:32.000000 boj-cli-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-23 21:16:52.801716 boj-cli-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-23 21:16:32.000000 boj-cli-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.797716 boj-cli-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.781716 boj-cli-1.2.2/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.797716 boj-cli-1.2.2/tests/assets/config/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/assets/config/test_filetype_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/assets/config/test_filetype_no_lang_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/assets/config/test_filetype_no_run_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.781716 boj-cli-1.2.2/tests/assets/problems/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.801716 boj-cli-1.2.2/tests/assets/problems/3052/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/assets/problems/3052/.boj-info.json
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/assets/problems/3052/compile_flags.txt
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/assets/problems/3052/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/assets/problems/3052/testcase.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.801716 boj-cli-1.2.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/core/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/core/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/test_args_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:16:52.801716 boj-cli-1.2.2/tests/web/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-23 21:16:32.000000 boj-cli-1.2.2/tests/web/test_solved_ac_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-23 21:16:32.000000 boj-cli-1.2.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.539514 boj-cli-1.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/major-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/minor-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/patch-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/release-template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.539514 boj-cli-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.github/workflows/run-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/boj-cli.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/.idea/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/dictionaries/jerry.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/material_theme_project_new.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-01 08:17:18.000000 boj-cli-1.2.3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-06-01 08:17:18.000000 boj-cli-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-06-01 08:17:37.555514 boj-cli-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-06-01 08:17:18.000000 boj-cli-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/args_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/browsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/browsers/login_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/add/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/add/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/case/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/case/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/clean/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/clean/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.543514 boj-cli-1.2.3/boj/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/init/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/login/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/login/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/open/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/open/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/open/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/random/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/random/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/run/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/run/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/commands/submit/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/submit/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/submit/progress_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/commands/submit/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.547514 boj-cli-1.2.3/boj/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.551514 boj-cli-1.2.3/boj/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/file_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/file_search_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/fs/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/core/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.551514 boj-cli-1.2.3/boj/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/boj_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/data/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.551514 boj-cli-1.2.3/boj/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/boj_main_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/boj_problem_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/boj_status_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/boj_submit_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-06-01 08:17:18.000000 boj-cli-1.2.3/boj/web/solved_ac_search_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/boj_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 08:17:37.000000 boj-cli-1.2.3/boj_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-06-01 08:17:18.000000 boj-cli-1.2.3/config_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-06-01 08:17:18.000000 boj-cli-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-06-01 08:17:18.000000 boj-cli-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 08:17:37.555514 boj-cli-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-01 08:17:18.000000 boj-cli-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.539514 boj-cli-1.2.3/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/assets/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/config/test_filetype_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/config/test_filetype_no_lang_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/config/test_filetype_no_run_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.539514 boj-cli-1.2.3/tests/assets/problems/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/assets/problems/3052/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/problems/3052/.boj-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/problems/3052/compile_flags.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/problems/3052/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/assets/problems/3052/testcase.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/core/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/core/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/test_args_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:17:37.555514 boj-cli-1.2.3/tests/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-06-01 08:17:18.000000 boj-cli-1.2.3/tests/web/test_solved_ac_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-01 08:17:18.000000 boj-cli-1.2.3/version.py
```

### Comparing `boj-cli-1.2.2/.github/release-template.yaml` & `boj-cli-1.2.3/.github/release-template.yaml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/.github/workflows/release.yaml` & `boj-cli-1.2.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/.gitignore` & `boj-cli-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/.idea/boj-cli.iml` & `boj-cli-1.2.3/.idea/boj-cli.iml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/LICENSE` & `boj-cli-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/PKG-INFO` & `boj-cli-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: boj-cli
-Version: 1.2.2
-Summary: Command line interface for BOJ
-Author: xvzc
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # boj-cli
 
 <div align="center">
   <h1 align="center">BOJ-CLI</h2>
 </div>
 <br>
 <div align="center">
@@ -28,17 +19,19 @@
       * [add](#add)
       * [run](#run)
       * [submit](#submit)
       * [clean](#clean)
       * [open](#open)
       * [random](#random)
       * [case](#case)
+   * [Supported languages](#supported-languages)
+
 <!--te-->
 # Requirements
-- `Python <= 3.12`
+- `Python <= 3.11`
 - `MacOS`, `Linux`, `Windows`
 
 # Installation
 
 ```sh
 $ pip install boj-cli
 ```
@@ -243,80 +236,18 @@
 ```
 --edit $TESTCASE_ID, -e $TESTACSE_ID: 주어진 id에 해당하는 테스트케이스 파일들을 편집합니다.
 --new, -n: 새로운 테스트케이스를 생성하고 편집합니다. TESTCASE_ID는 자동부여 됩니다.
 ```
 
 # Supported languages
 
-- `c++17`
-- `python3`
-- `pypy3`
-- `c11`
-- `text`
-- `golfscript`
-- `java8`
-- `c++98`
-- `ruby`
-- `c99`
-- `c++11`
-- `java11`
-- `kotlin(jvm)`
-- `c++14`
-- `swift`
-- `java8(openjdk)`
-- `c++20`
-- `c#`
-- `node.js`
-- `go`
-- `d`
-- `rust2018`
-- `go(gccgo)`
-- `c++17(clang)`
-- `java15`
-- `d(ldc)`
-- `php`
-- `rust2015`
-- `pascal`
-- `lua`
-- `perl`
-- `f#`
-- `visual-basic`
-- `objective-c`
-- `objective-c++`
-- `c99(clang)`
-- `c++98(clang)`
-- `c++11(clang)`
-- `c++14(clang)`
-- `c11(clang)`
-- `c++20(clang)`
-- `c90`
-- `c2x`
-- `c90(clang)`
-- `c2x(clang)`
-- `typescript`
-- `assembly(32bit)`
-- `assembly(64bit)`
-- `bash`
-- `fortran`
-- `scheme`
-- `ada`
-- `awk`
-- `o-caml`
-- `brainf**k`
-- `whitespace`
-- `tcl`
-- `rhino`
-- `cobol`
-- `pike`
-- `sed`
-- `intercal`
-- `bc`
-- `algol68`
-- `befunge`
-- `free-basic`
-- `haxe`
-- `lolcode`
-- `아희`
-- `system-verilog`
-- `rust2021`
-- `scala`
+`c++17` `python3` `pypy3` `c99` `c11` `text` `golfscript` `java8` `c++98` `ruby`  
+`c++11`  `java11` `kotlin(jvm)` `c++14` `swift` `java8(openjdk)` `c++20`  `c#`  
+`node.js` `go` `d` `rust2018` `go(gccgo)` `c++17(clang)` `java15` `d(ldc)` `php`  
+`rust2015` `pascal` `lua`  `perl` `f#` `visual-basic` `objective-c` `c99(clang)`  
+`c++98(clang)` `c++11(clang)` `c++14(clang)` `objective-c++` `c11(clang)` `c90`  
+`c90(clang)` `c2x(clang)` `typescript` `c++20(clang)` `bash` `fortran` `scheme`  
+`awk` `c2x` `assembly(32bit)` `assembly(64bit)` `o-caml` `whitespace` `lolcode`  
+`intercal` `rhino` `cobol` `pike` `sed` `tcl` `brainf**k` `ada` `system-verilog`  
+`algol68` `befunge` `haxe` `아희`  `bc` `free-basic` `rust2021` `scala`  
+
```

### Comparing `boj-cli-1.2.2/README.md` & `boj-cli-1.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: boj-cli
+Version: 1.2.3
+Summary: Command line interface for BOJ
+Author: xvzc
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # boj-cli
 
 <div align="center">
   <h1 align="center">BOJ-CLI</h2>
 </div>
 <br>
 <div align="center">
@@ -19,17 +28,19 @@
       * [add](#add)
       * [run](#run)
       * [submit](#submit)
       * [clean](#clean)
       * [open](#open)
       * [random](#random)
       * [case](#case)
+   * [Supported languages](#supported-languages)
+
 <!--te-->
 # Requirements
-- `Python <= 3.12`
+- `Python <= 3.11`
 - `MacOS`, `Linux`, `Windows`
 
 # Installation
 
 ```sh
 $ pip install boj-cli
 ```
@@ -234,80 +245,18 @@
 ```
 --edit $TESTCASE_ID, -e $TESTACSE_ID: 주어진 id에 해당하는 테스트케이스 파일들을 편집합니다.
 --new, -n: 새로운 테스트케이스를 생성하고 편집합니다. TESTCASE_ID는 자동부여 됩니다.
 ```
 
 # Supported languages
 
-- `c++17`
-- `python3`
-- `pypy3`
-- `c11`
-- `text`
-- `golfscript`
-- `java8`
-- `c++98`
-- `ruby`
-- `c99`
-- `c++11`
-- `java11`
-- `kotlin(jvm)`
-- `c++14`
-- `swift`
-- `java8(openjdk)`
-- `c++20`
-- `c#`
-- `node.js`
-- `go`
-- `d`
-- `rust2018`
-- `go(gccgo)`
-- `c++17(clang)`
-- `java15`
-- `d(ldc)`
-- `php`
-- `rust2015`
-- `pascal`
-- `lua`
-- `perl`
-- `f#`
-- `visual-basic`
-- `objective-c`
-- `objective-c++`
-- `c99(clang)`
-- `c++98(clang)`
-- `c++11(clang)`
-- `c++14(clang)`
-- `c11(clang)`
-- `c++20(clang)`
-- `c90`
-- `c2x`
-- `c90(clang)`
-- `c2x(clang)`
-- `typescript`
-- `assembly(32bit)`
-- `assembly(64bit)`
-- `bash`
-- `fortran`
-- `scheme`
-- `ada`
-- `awk`
-- `o-caml`
-- `brainf**k`
-- `whitespace`
-- `tcl`
-- `rhino`
-- `cobol`
-- `pike`
-- `sed`
-- `intercal`
-- `bc`
-- `algol68`
-- `befunge`
-- `free-basic`
-- `haxe`
-- `lolcode`
-- `아희`
-- `system-verilog`
-- `rust2021`
-- `scala`
+`c++17` `python3` `pypy3` `c99` `c11` `text` `golfscript` `java8` `c++98` `ruby`  
+`c++11`  `java11` `kotlin(jvm)` `c++14` `swift` `java8(openjdk)` `c++20`  `c#`  
+`node.js` `go` `d` `rust2018` `go(gccgo)` `c++17(clang)` `java15` `d(ldc)` `php`  
+`rust2015` `pascal` `lua`  `perl` `f#` `visual-basic` `objective-c` `c99(clang)`  
+`c++98(clang)` `c++11(clang)` `c++14(clang)` `objective-c++` `c11(clang)` `c90`  
+`c90(clang)` `c2x(clang)` `typescript` `c++20(clang)` `bash` `fortran` `scheme`  
+`awk` `c2x` `assembly(32bit)` `assembly(64bit)` `o-caml` `whitespace` `lolcode`  
+`intercal` `rhino` `cobol` `pike` `sed` `tcl` `brainf**k` `ada` `system-verilog`  
+`algol68` `befunge` `haxe` `아희`  `bc` `free-basic` `rust2021` `scala`  
+
```

### Comparing `boj-cli-1.2.2/boj/args_resolver.py` & `boj-cli-1.2.3/boj/args_resolver.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/browsers/login_browser.py` & `boj-cli-1.2.3/boj/browsers/login_browser.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/commands/add/command.py` & `boj-cli-1.2.3/boj/commands/add/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from pathlib import Path
 
 from rich.console import Console
 
 from boj.core import http
 from boj.core.command import Command
-from boj.core.error import IllegalStatementError, ResourceNotFoundError
+from boj.core.error import IllegalStatementError, ResourceNotFoundError, FatalError
 from boj.core.fs.repository import Repository, ReadOnlyRepository
 from boj.core.fs.file_object import TextFile
 from boj.core.html import HtmlParser
 from boj.core.http import HtmlResponse
 from boj.core.fs.util import file_exists
 from boj.data.config import Config
 from boj.data.testcase import Testcase
@@ -32,15 +32,15 @@
     def execute(self, args):
         config = self.config_repository.find()
 
         with self.console.status("Checking for status..") as status:
             filetype = args.filetype or config.general.default_filetype
             if not filetype:
                 message = "missing required argument '--type' or 'config.general.default_filetype'"
-                raise IllegalStatementError(message)
+                raise FatalError(message)
 
             # Get HTML content of given problem id from BOJ
             status.update("Crawling testcases..")
             problem_page = HtmlResponse(
                 http.get(BojProblemPageRequest(args.problem_id))
             )
```

### Comparing `boj-cli-1.2.2/boj/commands/case/command.py` & `boj-cli-1.2.3/boj/commands/case/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 import os
 
 from rich.console import Console
 
 from boj.core.command import Command
-from boj.core.error import IllegalStatementError, ParsingConfigError
+from boj.core.error import IllegalStatementError, FatalError
 from boj.core.fs.file_object import FileMetadata, TextFile
 from boj.core.fs.repository import ReadOnlyRepository, Repository
 from boj.data.boj_info import BojInfo
 from boj.data.config import Config
 
 
 def _open_files(command: str, input_: TextFile, output: TextFile):
@@ -32,15 +32,15 @@
     def execute(self, args):
         config = self.config_repository.find()
         cwd, query, search_strategy = BojInfo.query_factory(
             config.workspace.ongoing_dir(abs_=True),
             args.problem_id,
         )
         if not config.general.editor_command:
-            raise ParsingConfigError("'config.general.editor_command' is not specified")
+            raise FatalError("'config.general.editor_command' is not specified")
 
         self.boj_info_repository.search_strategy = search_strategy
         boj_info = self.boj_info_repository.find(cwd, query)
 
         tc_dir = boj_info.testcase_dir(abs_=True)
         if args.new:
             new_id = "1"
```

### Comparing `boj-cli-1.2.2/boj/commands/clean/command.py` & `boj-cli-1.2.3/boj/commands/clean/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/commands/init/command.py` & `boj-cli-1.2.3/boj/commands/init/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/commands/login/command.py` & `boj-cli-1.2.3/boj/commands/login/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 import os
 
 from rich.console import Console
 
 from boj.browsers.login_browser import LoginBrowser
-from boj.core.error import ParsingConfigError
+from boj.core.error import FatalError
 from boj.core.fs.file_object import FileMetadata
 from boj.core.fs.repository import Repository, ReadOnlyRepository
 from boj.data.config import Config
 from boj.data.credential import Credential
 from boj.core import constant
 from boj.core.command import Command
 
@@ -18,15 +18,15 @@
     console: Console
     config_repository: ReadOnlyRepository[Config]
     credential_repository: Repository[Credential]
 
     def execute(self, args):
         config = self.config_repository.find()
         if not config.general.selenium_browser:
-            raise ParsingConfigError("Please specify 'config.general.login_browser'")
+            raise FatalError("invalid value for 'config.general.login_browser'")
 
         with self.console.status("Preparing login browser...") as status:
             browser = LoginBrowser(
                 constant.boj_login_url(),
                 config.general.selenium_browser,
             )
```

### Comparing `boj-cli-1.2.2/boj/commands/open/command.py` & `boj-cli-1.2.3/boj/commands/open/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/commands/random/command.py` & `boj-cli-1.2.3/boj/commands/random/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import boj.core.crypto
 import boj.core.constant
 from boj.core import constant
 from boj.core.command import Command
 
 from boj.core import http
-from boj.core.error import IllegalStatementError
+from boj.core.error import IllegalStatementError, FatalError
 from boj.web.solved_ac_search_api import (
     SolvedAcSearchApiRequest,
     make_solved_ac_search_api_params,
 )
 from boj.core.fs.repository import Repository
 from boj.core.http import JsonResponse
 from boj.data.credential import Credential
@@ -41,18 +41,18 @@
                         )
                     )
                 )
             )
 
             json = response.json
             if not json or ("items" not in json):
-                raise IllegalStatementError("Error while calling solve.ac API.")
+                raise FatalError("error while calling solve.ac API.")
 
             if len(json["items"]) == 0:
-                raise IllegalStatementError("No matching problem found.")
+                raise FatalError("no matching problem found.")
 
             items = json["items"]
             selected_tag = None
             if args.tags:
                 selected_tag = random.choice(args.tags)
 
             for item in items:
```

### Comparing `boj-cli-1.2.2/boj/commands/run/command.py` & `boj-cli-1.2.3/boj/commands/run/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/commands/run/runner.py` & `boj-cli-1.2.3/boj/commands/run/runner.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/commands/submit/command.py` & `boj-cli-1.2.3/boj/commands/submit/command.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/commands/submit/progress_message.py` & `boj-cli-1.2.3/boj/commands/submit/progress_message.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/commands/submit/websocket.py` & `boj-cli-1.2.3/boj/commands/submit/websocket.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/containers.py` & `boj-cli-1.2.3/boj/containers.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/browser.py` & `boj-cli-1.2.3/boj/core/browser.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/console.py` & `boj-cli-1.2.3/boj/core/console.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/constant.py` & `boj-cli-1.2.3/boj/core/constant.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/error.py` & `boj-cli-1.2.3/boj/core/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 class BojError(BaseException):
     def __init__(self, msg):
         super().__init__(msg)
 
 
+class FatalError(BojError):
+    def __init__(self, msg):
+        super().__init__("fatal: " + msg)
+
+
 class AuthenticationError(BojError):
     def __init__(self, msg):
         super().__init__(msg)
 
 
 class DeprecatedError(BojError):
     def __init__(self, msg):
```

### Comparing `boj-cli-1.2.2/boj/core/fs/file_io.py` & `boj-cli-1.2.3/boj/core/fs/file_io.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/fs/file_object.py` & `boj-cli-1.2.3/boj/core/fs/file_object.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/fs/file_search_strategy.py` & `boj-cli-1.2.3/boj/core/fs/file_search_strategy.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/fs/repository.py` & `boj-cli-1.2.3/boj/core/fs/repository.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/fs/serializer.py` & `boj-cli-1.2.3/boj/core/fs/serializer.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/core/http.py` & `boj-cli-1.2.3/boj/core/http.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/data/boj_info.py` & `boj-cli-1.2.3/boj/data/boj_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Optional, Type, Self
 
 from boj.core import constant
-from boj.core.error import IllegalStatementError, ResourceNotFoundError
+from boj.core.error import IllegalStatementError, ResourceNotFoundError, FatalError
 import json
 
 from boj.core.fs.file_search_strategy import (
     FileSearchStrategy,
     StaticSearchStrategy,
     UpwardSearchStrategy,
 )
@@ -172,13 +172,13 @@
 class BojInfoRepository(Repository[BojInfo]):
     def find(self, cwd: str = os.getcwd(), query: Optional[str] = None) -> BojInfo:
         try:
             path = self._search_strategy.find(query=query, cwd=cwd)
             metadata = FileMetadata.of(path)
             return self._serializer.marshal(self._file_io.read(path), metadata)
         except ResourceNotFoundError:
-            raise ResourceNotFoundError(
-                "Can not find '.boj-info.json'. did you run 'boj add $problem_id'?"
+            raise FatalError(
+                "can not find '.boj-info.json'. did you run 'boj add $problem_id'?"
             )
 
     def save(self, obj: T) -> None:
         self._file_io.write(self._serializer.unmarshal(obj), obj.metadata.path)
```

### Comparing `boj-cli-1.2.2/boj/data/config.py` & `boj-cli-1.2.3/boj/data/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from boj.core.fs.repository import ReadOnlyRepository, T
 from boj.core.fs.serializer import Serializer
 from boj.core.fs.file_object import FileMetadata, FileObject
 from boj.core.error import (
     ParsingConfigError,
     IllegalStatementError,
+    ResourceNotFoundError,
+    FatalError,
 )
 
 
 class GeneralConfig:
     def __init__(
         self,
         default_filetype: Optional[str],
@@ -290,13 +292,19 @@
 
 class ConfigRepository(ReadOnlyRepository[Config]):
     def find(
         self,
         cwd: str = os.getcwd(),
         query: Optional[str] = None,
     ) -> Config:
-        path = self._search_strategy.find(
-            cwd=cwd,
-            query=os.path.join(".boj", "config.yaml"),
-        )
+        try:
+            path = self._search_strategy.find(
+                cwd=cwd,
+                query=os.path.join(".boj", "config.yaml"),
+            )
+        except ResourceNotFoundError:
+            raise FatalError(
+                "not a boj directory (or any of the parent directories): .boj/config.yaml"
+            )
+
         file = self._file_io.read(path)
         return self._serializer.marshal(file, FileMetadata.of(path))
```

### Comparing `boj-cli-1.2.2/boj/data/credential.py` & `boj-cli-1.2.3/boj/data/credential.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/data/session.py` & `boj-cli-1.2.3/boj/data/session.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/data/testcase.py` & `boj-cli-1.2.3/boj/data/testcase.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/entry.py` & `boj-cli-1.2.3/boj/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     try:
         container = Container()
         dispatcher = container.dispatcher_factory()
         mkdir(constant.boj_cli_path(), True)
         dispatcher.modules[args.command].execute(args)
     except BojError as e:
         SystemExit(e)
-        console.log("Error: " + str(e))
+        console.log(str(e))
         # print(str(e))
         exit(1)
     except BaseException as e:
         console.log(e.args)
         traceback.print_exc()
         exit(1)
```

### Comparing `boj-cli-1.2.2/boj/web/boj_problem_page.py` & `boj-cli-1.2.3/boj/web/boj_problem_page.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/web/boj_submit_page.py` & `boj-cli-1.2.3/boj/web/boj_submit_page.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj/web/solved_ac_search_api.py` & `boj-cli-1.2.3/boj/web/solved_ac_search_api.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/boj_cli.egg-info/PKG-INFO` & `boj-cli-1.2.3/boj_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boj-cli
-Version: 1.2.2
+Version: 1.2.3
 Summary: Command line interface for BOJ
 Author: xvzc
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # boj-cli
@@ -28,17 +28,19 @@
       * [add](#add)
       * [run](#run)
       * [submit](#submit)
       * [clean](#clean)
       * [open](#open)
       * [random](#random)
       * [case](#case)
+   * [Supported languages](#supported-languages)
+
 <!--te-->
 # Requirements
-- `Python <= 3.12`
+- `Python <= 3.11`
 - `MacOS`, `Linux`, `Windows`
 
 # Installation
 
 ```sh
 $ pip install boj-cli
 ```
@@ -243,80 +245,18 @@
 ```
 --edit $TESTCASE_ID, -e $TESTACSE_ID: 주어진 id에 해당하는 테스트케이스 파일들을 편집합니다.
 --new, -n: 새로운 테스트케이스를 생성하고 편집합니다. TESTCASE_ID는 자동부여 됩니다.
 ```
 
 # Supported languages
 
-- `c++17`
-- `python3`
-- `pypy3`
-- `c11`
-- `text`
-- `golfscript`
-- `java8`
-- `c++98`
-- `ruby`
-- `c99`
-- `c++11`
-- `java11`
-- `kotlin(jvm)`
-- `c++14`
-- `swift`
-- `java8(openjdk)`
-- `c++20`
-- `c#`
-- `node.js`
-- `go`
-- `d`
-- `rust2018`
-- `go(gccgo)`
-- `c++17(clang)`
-- `java15`
-- `d(ldc)`
-- `php`
-- `rust2015`
-- `pascal`
-- `lua`
-- `perl`
-- `f#`
-- `visual-basic`
-- `objective-c`
-- `objective-c++`
-- `c99(clang)`
-- `c++98(clang)`
-- `c++11(clang)`
-- `c++14(clang)`
-- `c11(clang)`
-- `c++20(clang)`
-- `c90`
-- `c2x`
-- `c90(clang)`
-- `c2x(clang)`
-- `typescript`
-- `assembly(32bit)`
-- `assembly(64bit)`
-- `bash`
-- `fortran`
-- `scheme`
-- `ada`
-- `awk`
-- `o-caml`
-- `brainf**k`
-- `whitespace`
-- `tcl`
-- `rhino`
-- `cobol`
-- `pike`
-- `sed`
-- `intercal`
-- `bc`
-- `algol68`
-- `befunge`
-- `free-basic`
-- `haxe`
-- `lolcode`
-- `아희`
-- `system-verilog`
-- `rust2021`
-- `scala`
+`c++17` `python3` `pypy3` `c99` `c11` `text` `golfscript` `java8` `c++98` `ruby`  
+`c++11`  `java11` `kotlin(jvm)` `c++14` `swift` `java8(openjdk)` `c++20`  `c#`  
+`node.js` `go` `d` `rust2018` `go(gccgo)` `c++17(clang)` `java15` `d(ldc)` `php`  
+`rust2015` `pascal` `lua`  `perl` `f#` `visual-basic` `objective-c` `c99(clang)`  
+`c++98(clang)` `c++11(clang)` `c++14(clang)` `objective-c++` `c11(clang)` `c90`  
+`c90(clang)` `c2x(clang)` `typescript` `c++20(clang)` `bash` `fortran` `scheme`  
+`awk` `c2x` `assembly(32bit)` `assembly(64bit)` `o-caml` `whitespace` `lolcode`  
+`intercal` `rhino` `cobol` `pike` `sed` `tcl` `brainf**k` `ada` `system-verilog`  
+`algol68` `befunge` `haxe` `아희`  `bc` `free-basic` `rust2021` `scala`  
+
```

### Comparing `boj-cli-1.2.2/boj_cli.egg-info/SOURCES.txt` & `boj-cli-1.2.3/boj_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 .github/minor-release.yaml
 .github/patch-release.yaml
 .github/release-template.yaml
 .github/workflows/release.yaml
 .github/workflows/run-test.yaml
 .idea/.gitignore
 .idea/boj-cli.iml
-.idea/misc.xml
+.idea/material_theme_project_new.xml
 .idea/modules.xml
 .idea/vcs.xml
 .idea/dictionaries/jerry.xml
 .idea/inspectionProfiles/profiles_settings.xml
 boj/__init__.py
 boj/__main__.py
 boj/args_resolver.py
```

### Comparing `boj-cli-1.2.2/config_example.yaml` & `boj-cli-1.2.3/config_example.yaml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/pyproject.toml` & `boj-cli-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/requirements.txt` & `boj-cli-1.2.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/tests/assets/problems/3052/main.cpp` & `boj-cli-1.2.3/tests/assets/problems/3052/main.cpp`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/tests/core/test_constant.py` & `boj-cli-1.2.3/tests/core/test_constant.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/tests/test_args_resolver.py` & `boj-cli-1.2.3/tests/test_args_resolver.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/tests/web/test_solved_ac_search_api.py` & `boj-cli-1.2.3/tests/web/test_solved_ac_search_api.py`

 * *Files identical despite different names*

### Comparing `boj-cli-1.2.2/version.py` & `boj-cli-1.2.3/version.py`

 * *Files identical despite different names*

