# Comparing `tmp/qteasy-1.2.6.tar.gz` & `tmp/qteasy-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qteasy-1.2.6.tar", last modified: Tue May  7 01:13:52 2024, max compression
+gzip compressed data, was "qteasy-1.2.7.tar", last modified: Sat Jun  1 15:55:00 2024, max compression
```

## Comparing `qteasy-1.2.6.tar` & `qteasy-1.2.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-07 01:13:52.997615 qteasy-1.2.6/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.6/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-05-07 01:13:52.997530 qteasy-1.2.6/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    24211 2024-05-06 15:43:04.000000 qteasy-1.2.6/README.md
--rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-05-06 15:43:04.000000 qteasy-1.2.6/pyproject.toml
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-07 01:13:52.984206 qteasy-1.2.6/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-05-06 15:43:04.000000 qteasy-1.2.6/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-05-05 10:05:28.000000 qteasy-1.2.6/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.6/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-05-05 10:05:28.000000 qteasy-1.2.6/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142516 2024-05-05 14:24:46.000000 qteasy-1.2.6/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   111306 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   390940 2024-05-06 15:43:04.000000 qteasy-1.2.6/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.6/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34874 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-05-05 10:05:28.000000 qteasy-1.2.6/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   110944 2024-05-06 04:13:52.000000 qteasy-1.2.6/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-05-04 08:19:36.000000 qteasy-1.2.6/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107890 2024-05-06 15:43:04.000000 qteasy-1.2.6/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.6/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-05-05 10:05:28.000000 qteasy-1.2.6/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   156164 2024-05-05 14:35:57.000000 qteasy-1.2.6/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/trader_cli.py
--rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/trader_tui.py
--rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-05-05 10:05:28.000000 qteasy-1.2.6/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.6/qteasy/tsfuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)      840 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/tui_style.tcss
--rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-05-04 09:08:45.000000 qteasy-1.2.6/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.6/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-07 01:13:52.996942 qteasy-1.2.6/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    27935 2024-05-07 01:13:52.000000 qteasy-1.2.6/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-05-07 01:13:52.000000 qteasy-1.2.6/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-05-07 01:13:52.000000 qteasy-1.2.6/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.6/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      195 2024-05-07 01:13:52.000000 qteasy-1.2.6/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-05-07 01:13:52.000000 qteasy-1.2.6/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-05-07 01:13:52.997902 qteasy-1.2.6/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.6/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-05-07 01:13:52.996557 qteasy-1.2.6/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-05-05 10:05:28.000000 qteasy-1.2.6/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.6/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.6/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.6/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-05-05 10:05:28.000000 qteasy-1.2.6/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   123545 2024-05-06 15:43:04.000000 qteasy-1.2.6/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.6/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73624 2024-04-05 14:28:39.000000 qteasy-1.2.6/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.6/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.6/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.6/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.6/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-05-06 14:14:27.000000 qteasy-1.2.6/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    44521 2024-05-05 14:36:45.000000 qteasy-1.2.6/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.6/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    40814 2024-05-06 04:13:52.000000 qteasy-1.2.6/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-05-04 09:08:45.000000 qteasy-1.2.6/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-05-04 09:08:45.000000 qteasy-1.2.6/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.6/tests/test_trading.py
--rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-05-04 09:08:45.000000 qteasy-1.2.6/tests/test_tui.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.6/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.6/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.6/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-06-01 15:55:00.192462 qteasy-1.2.7/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.2.7/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    27987 2024-06-01 15:55:00.192370 qteasy-1.2.7/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    24263 2024-05-31 06:41:22.000000 qteasy-1.2.7/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2304 2024-05-31 06:41:22.000000 qteasy-1.2.7/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-06-01 15:55:00.179329 qteasy-1.2.7/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8588 2024-05-31 06:41:22.000000 qteasy-1.2.7/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    68549 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    53075 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.2.7/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30260 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142516 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   114508 2024-05-31 06:50:26.000000 qteasy-1.2.7/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   391054 2024-05-31 06:41:22.000000 qteasy-1.2.7/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.2.7/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34312 2024-05-31 06:41:22.000000 qteasy-1.2.7/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    38585 2024-05-29 11:59:46.000000 qteasy-1.2.7/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   110944 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-05-04 08:19:36.000000 qteasy-1.2.7/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107890 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    34029 2024-04-05 14:28:39.000000 qteasy-1.2.7/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88071 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   156164 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    51352 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)    98512 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    93193 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/trader_cli.py
+-rw-r--r--   0 jackie     (501) staff       (20)    18205 2024-05-31 06:41:22.000000 qteasy-1.2.7/qteasy/trader_tui.py
+-rw-r--r--   0 jackie     (501) staff       (20)    68078 2024-05-29 11:59:46.000000 qteasy-1.2.7/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   131527 2024-04-21 23:36:55.000000 qteasy-1.2.7/qteasy/tsfuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)      840 2024-05-31 06:41:22.000000 qteasy-1.2.7/qteasy/tui_style.tcss
+-rwxr-xr-x   0 jackie     (501) staff       (20)    75175 2024-05-29 11:59:51.000000 qteasy-1.2.7/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79918 2024-04-21 23:36:55.000000 qteasy-1.2.7/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-06-01 15:55:00.191593 qteasy-1.2.7/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    27987 2024-06-01 15:55:00.000000 qteasy-1.2.7/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1274 2024-06-01 15:55:00.000000 qteasy-1.2.7/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-06-01 15:55:00.000000 qteasy-1.2.7/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.2.7/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      195 2024-06-01 15:55:00.000000 qteasy-1.2.7/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-06-01 15:55:00.000000 qteasy-1.2.7/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1627 2024-06-01 15:55:00.192773 qteasy-1.2.7/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.2.7/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-06-01 15:55:00.191284 qteasy-1.2.7/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-05-05 10:05:28.000000 qteasy-1.2.7/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8078 2024-04-05 14:28:39.000000 qteasy-1.2.7/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.2.7/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-03 01:57:25.000000 qteasy-1.2.7/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    19818 2024-05-05 10:05:28.000000 qteasy-1.2.7/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   123545 2024-05-29 11:59:51.000000 qteasy-1.2.7/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.2.7/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73630 2024-05-31 06:41:22.000000 qteasy-1.2.7/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.2.7/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.2.7/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.2.7/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   304019 2024-04-05 14:28:39.000000 qteasy-1.2.7/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169228 2024-05-29 11:59:51.000000 qteasy-1.2.7/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44521 2024-05-29 11:59:51.000000 qteasy-1.2.7/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.2.7/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    40814 2024-05-29 11:59:51.000000 qteasy-1.2.7/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43397 2024-05-29 11:59:51.000000 qteasy-1.2.7/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    45317 2024-05-29 11:59:51.000000 qteasy-1.2.7/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   168527 2024-04-21 23:36:55.000000 qteasy-1.2.7/tests/test_trading.py
+-rw-r--r--   0 jackie     (501) staff       (20)     2670 2024-05-29 11:59:51.000000 qteasy-1.2.7/tests/test_tui.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.2.7/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43279 2024-04-05 14:28:39.000000 qteasy-1.2.7/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.2.7/tests/test_visual.py
```

### Comparing `qteasy-1.2.6/LICENSE` & `qteasy-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/PKG-INFO` & `qteasy-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.6
+Version: 1.2.7
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -58,14 +58,16 @@
 Provides-Extra: feather
 Requires-Dist: pyarrow>=3; extra == "feather"
 Provides-Extra: dev
 Requires-Dist: ta-lib; extra == "dev"
 Requires-Dist: pymysql>=1.0.0; extra == "dev"
 Requires-Dist: pyarrow>=3; extra == "dev"
 
+![png](docs/source/img/qteasy_logo_horizontal.png)
+
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
 [![Build Status](https://app.travis-ci.com/shepherdpp/qteasy.svg?branch=master)](https://app.travis-ci.com/shepherdpp/qteasy)
 [![Documentation Status](https://readthedocs.org/projects/qteasy/badge/?version=latest)](https://qteasy.readthedocs.io/zh/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/shepherdpp/qteasy)
@@ -106,15 +108,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.6`
+- Latest Version: `1.2.7`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.6/README.md` & `qteasy-1.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![png](docs/source/img/qteasy_logo_horizontal.png)
+
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
 [![Build Status](https://app.travis-ci.com/shepherdpp/qteasy.svg?branch=master)](https://app.travis-ci.com/shepherdpp/qteasy)
 [![Documentation Status](https://readthedocs.org/projects/qteasy/badge/?version=latest)](https://qteasy.readthedocs.io/zh/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/shepherdpp/qteasy)
@@ -42,15 +44,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.6`
+- Latest Version: `1.2.7`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.6/pyproject.toml` & `qteasy-1.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 build-backend = "setuptools.build_meta"
 
 #[tool.setuptools.package.find]
 #where = "qteasy/"
 
 [project]
 name = "qteasy"
-version = "1.2.6"
+version = "1.2.7"
 authors = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 maintainers = [
   {name="jackie PENG", email="jackie.pengzhao@gmail.com" },
 ]
 description = "A fast quantitative investment tool kit"
```

### Comparing `qteasy-1.2.6/qteasy/__init__.py` & `qteasy-1.2.7/qteasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 from .visual import candle
 from .finance import CashPlan, set_cost, update_cost
 from .database import DataSource, find_history_data
 from ._arg_validators import QT_CONFIG, ConfigDict
 
 
 # qteasy版本信息
-__version__ = '1.2.6'
+__version__ = '1.2.7'
 version_info = Namespace(
         major=1,
         minor=2,
-        patch=6,
+        patch=7,
         short=(1, 2),
-        full=(1, 2, 6),
-        string='1.2.6',
-        tuple=('1', '2', '6'),
+        full=(1, 2, 7),
+        string='1.2.7',
+        tuple=('1', '2', '7'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
```

### Comparing `qteasy-1.2.6/qteasy/_arg_validators.py` & `qteasy-1.2.7/qteasy/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/backtest.py` & `qteasy-1.2.7/qteasy/backtest.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/blender.py` & `qteasy-1.2.7/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/broker.py` & `qteasy-1.2.7/qteasy/broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/built_in.py` & `qteasy-1.2.7/qteasy/built_in.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/core.py` & `qteasy-1.2.7/qteasy/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
     Returns
     -------
     list, 股票代码清单
 
     See Also
     --------
-    filter_stock()
+    filter_stocks()
     """
     share_basics = filter_stocks(date=date, **kwargs)
     return share_basics.index.to_list()
 
 
 def get_basic_info(code_or_name: str, asset_types=None, match_full_name=False, printout=True, verbose=False):
     """ 等同于get_stock_info()
@@ -462,23 +462,20 @@
          pk_count2:     int，数据表第二个主键记录
          pk_min2:       obj，数据表主键2起始记录
          pk_max2:       obj，数据表主键2最终记录)
 
     Examples
     --------
     >>> get_table_info('STOCK_BASIC')
-
-    Out:
     <stock_basic>, 1.5MB/5K records on disc
     primary keys:
     -----------------------------------
     1:  ts_code:
         <unknown> entries
         starts: 000001.SZ, end: 873527.BJ
-
     columns of table:
     ------------------------------------
             columns       dtypes remarks
     0       ts_code   varchar(9)    证券代码
     1        symbol   varchar(6)    股票代码
     2          name  varchar(20)    股票名称
     3          area  varchar(10)      地域
@@ -497,15 +494,15 @@
     if data_source is None:
         data_source = qteasy.QT_DATA_SOURCE
     if not isinstance(data_source, qteasy.DataSource):
         raise TypeError(f'data_source should be a DataSource, got {type(data_source)} instead.')
     return data_source.get_table_info(table=table_name, verbose=verbose)
 
 
-def get_table_overview(data_source=None, tables=None, include_sys_tables=False):
+def get_table_overview(data_source=None, tables=None, include_sys_tables=False) -> None:
     """ 显示默认数据源或指定数据源的数据总览
 
     Parameters
     ----------
     data_source: Object
         一个data_source 对象,默认为None，如果为None，则显示默认数据源的overview
     tables: str or list of str, Default: None
@@ -523,18 +520,19 @@
     """
 
     from .database import DataSource
     if data_source is None:
         data_source = qteasy.QT_DATA_SOURCE
     if not isinstance(data_source, DataSource):
         raise TypeError(f'A DataSource object must be passed, got {type(data_source)} instead.')
-    return data_source.overview(tables=tables, include_sys_tables=include_sys_tables)
 
+    data_source.overview(tables=tables, include_sys_tables=include_sys_tables)
 
-def get_data_overview(data_source=None, tables=None, include_sys_tables=False):
+
+def get_data_overview(data_source=None, tables=None, include_sys_tables=False) -> None:
     """ 显示数据源的数据总览，等同于get_table_overview()
 
     获取的信息包括所有数据表的数据量、占用磁盘空间、主键名称、内容等
 
     Parameters
     ----------
     data_source: Object
@@ -546,18 +544,16 @@
 
     Returns
     -------
     None
 
     Examples
     --------
-    >>> get_data_overview()  # 获取当前默认数据源的数据总览
-
-    Out:
-
+    >>> import qteasy as qt
+    >>> qt.get_data_overview()  # 获取当前默认数据源的数据总览
     Analyzing local data source tables... depending on size of tables, it may take a few minutes
     [########################################]62/62-100.0%  Analyzing completed!
     db:mysql://localhost@3306/ts_db
     Following tables contain local data, to view complete list, print returned DataFrame
                      Has_data Size_on_disk Record_count Record_start  Record_end
     table
     trade_calendar     True        2.5MB         73K     1990-10-12   2023-12-31
@@ -612,96 +608,96 @@
     express            True        3.5MB         23K     2004-12-31   2023-06-30
     shibor             True         16KB         212           None         None
     """
 
     return get_table_overview(data_source=data_source, tables=tables, include_sys_tables=include_sys_tables)
 
 
-def refill_data_source(data_source=None, **kwargs):
+def refill_data_source(*, data_source=None, **kwargs) -> None:
     """ 填充数据数据源
 
     Parameters
     ----------
     data_source: DataSource, Default None
         需要填充数据的DataSource, 如果为None，则填充数据源到QT_DATA_SOURCE
-    **kwargs
-        DataSource.refill_local_source()的数据下载参数：
-        tables: str or list of str, default: None
-            需要补充的本地数据表，可以同时给出多个table的名称，逗号分隔字符串和字符串列表都合法：
-            例如，下面两种方式都合法且相同：
-                table='stock_indicator, stock_daily, income, stock_adj_factor'
-                table=['stock_indicator', 'stock_daily', 'income', 'stock_adj_factor']
-            除了直接给出表名称以外，还可以通过表类型指明多个表，可以同时输入多个类型的表：
-                - 'all'     : 所有的表
-                - 'cal'     : 交易日历表
-                - 'basics'  : 所有的基础信息表
-                - 'adj'     : 所有的复权因子表
-                - 'data'    : 所有的历史数据表
-                - 'events'  : 所有的历史事件表(如股票更名、更换基金经理、基金份额变动等)
-                - 'report'  : 财务报表
-                - 'comp'    : 指数成分表
-        dtypes: str or list of str, default: None
-            通过指定dtypes来确定需要更新的表单，只要包含指定的dtype的数据表都会被选中
-            如果给出了tables，则dtypes参数会被忽略
-        freqs: str, default: None
-            通过指定tables或dtypes来确定需要更新的表单时，指定freqs可以限定表单的范围
-            如果tables != all时，给出freq会排除掉freq与之不符的数据表
-        asset_types: Str of List of Str, default: None
-            通过指定tables或dtypes来确定需要更新的表单时，指定asset_types可以限定表单的范围
-            如果tables != all时，给出asset_type会排除掉与之不符的数据表
-        start_date: DateTime Like, default: None
-            限定数据下载的时间范围，如果给出start_date/end_date，只有这个时间段内的数据会被下载
-        end_date: DateTime Like, default: None
-            限定数据下载的时间范围，如果给出start_date/end_date，只有这个时间段内的数据会被下载
-        list_arg_filter: str or list of str, default: None  **注意，不是所有情况下该参数都有效**
-            限定下载数据时的筛选参数，某些数据表以列表的形式给出可筛选参数，如stock_basic表，它有一个可筛选
-            参数"exchange"，选项包含 'SSE', 'SZSE', 'BSE'，可以通过此参数限定下载数据的范围。
-            如果filter_arg为None，则下载所有数据。
-            例如，下载stock_basic表数据时，下载以下输入均为合法输入：
-            - 'SZSE'
-                仅下载深圳交易所的股票数据
-            - ['SSE', 'SZSE']
-            - 'SSE, SZSE'
-                上面两种写法等效，下载上海和深圳交易所的股票数据
-        symbols: str or list of str, default: None  **注意，不是所有情况下该参数都有效**
-            限定下载数据的证券代码范围，代码不需要给出类型后缀，只需要给出数字代码即可。
-            可以多种形式确定范围，以下输入均为合法输入：
-            - '000001'
-                没有指定asset_types时，000001.SZ, 000001.SH ... 等所有代码都会被选中下载
-                如果指定asset_types，只有符合类型的证券数据会被下载
-            - '000001, 000002, 000003'
-            - ['000001', '000002', '000003']
-                两种写法等效，列表中列举出的证券数据会被下载
-            - '000001:000300'
-                从'000001'开始到'000300'之间的所有证券数据都会被下载
-        merge_type: str, default: 'ignore'
-            数据混合方式，当获取的数据与本地数据的key重复时，如何处理重复的数据：
-            - 'ignore' 默认值，不下载重复的数据
-            - 'update' 下载并更新本地数据的重复部分
-        reversed_par_seq: Bool, default: False
-            是否逆序参数下载数据， 默认False
-            - True:  逆序参数下载数据
-            - False: 顺序参数下载数据
-        parallel: Bool, default: True
-            是否启用多线程下载数据，默认True
-            - True:  启用多线程下载数据
-            - False: 禁用多线程下载
-        process_count: int, default: None
-            启用多线程下载时，同时开启的线程数，默认值为设备的CPU核心数
-        chunk_size: int, default: 100
-            保存数据到本地时，为了减少文件/数据库读取次数，将下载的数据累计一定数量后
-            再批量保存到本地，chunk_size即批量，默认值100
+    **kwargs:
+     tables: str or list of str, default: None
+         需要补充的本地数据表，可以同时给出多个table的名称，逗号分隔字符串和字符串列表都合法：
+         例如，下面两种方式都合法且相同：
+             table='stock_indicator, stock_daily, income, stock_adj_factor'
+             table=['stock_indicator', 'stock_daily', 'income', 'stock_adj_factor']
+         除了直接给出表名称以外，还可以通过表类型指明多个表，可以同时输入多个类型的表：
+             - 'all'     : 所有的表
+             - 'cal'     : 交易日历表
+             - 'basics'  : 所有的基础信息表
+             - 'adj'     : 所有的复权因子表
+             - 'data'    : 所有的历史数据表
+             - 'events'  : 所有的历史事件表(如股票更名、更换基金经理、基金份额变动等)
+             - 'report'  : 财务报表
+             - 'comp'    : 指数成分表
+     dtypes: str or list of str, default: None
+         通过指定dtypes来确定需要更新的表单，只要包含指定的dtype的数据表都会被选中
+         如果给出了tables，则dtypes参数会被忽略
+     freqs: str, default: None
+         通过指定tables或dtypes来确定需要更新的表单时，指定freqs可以限定表单的范围
+         如果tables != all时，给出freq会排除掉freq与之不符的数据表
+     asset_types: Str of List of Str, default: None
+         通过指定tables或dtypes来确定需要更新的表单时，指定asset_types可以限定表单的范围
+         如果tables != all时，给出asset_type会排除掉与之不符的数据表
+     start_date: DateTime Like, default: None
+         限定数据下载的时间范围，如果给出start_date/end_date，只有这个时间段内的数据会被下载
+     end_date: DateTime Like, default: None
+         限定数据下载的时间范围，如果给出start_date/end_date，只有这个时间段内的数据会被下载
+     list_arg_filter: str or list of str, default: None  **注意，不是所有情况下该参数都有效**
+         限定下载数据时的筛选参数，某些数据表以列表的形式给出可筛选参数，如stock_basic表，它有一个可筛选
+         参数"exchange"，选项包含 'SSE', 'SZSE', 'BSE'，可以通过此参数限定下载数据的范围。
+         如果filter_arg为None，则下载所有数据。
+         例如，下载stock_basic表数据时，下载以下输入均为合法输入：
+         - 'SZSE'
+             仅下载深圳交易所的股票数据
+         - ['SSE', 'SZSE']
+         - 'SSE, SZSE'
+             上面两种写法等效，下载上海和深圳交易所的股票数据
+     symbols: str or list of str, default: None  **注意，不是所有情况下该参数都有效**
+         限定下载数据的证券代码范围，代码不需要给出类型后缀，只需要给出数字代码即可。
+         可以多种形式确定范围，以下输入均为合法输入：
+         - '000001'
+             没有指定asset_types时，000001.SZ, 000001.SH ... 等所有代码都会被选中下载
+             如果指定asset_types，只有符合类型的证券数据会被下载
+         - '000001, 000002, 000003'
+         - ['000001', '000002', '000003']
+             两种写法等效，列表中列举出的证券数据会被下载
+         - '000001:000300'
+             从'000001'开始到'000300'之间的所有证券数据都会被下载
+     merge_type: str, default: 'ignore'
+         数据混合方式，当获取的数据与本地数据的key重复时，如何处理重复的数据：
+         - 'ignore' 默认值，不下载重复的数据
+         - 'update' 下载并更新本地数据的重复部分
+     reversed_par_seq: Bool, default: False
+         是否逆序参数下载数据， 默认False
+         - True:  逆序参数下载数据
+         - False: 顺序参数下载数据
+     parallel: Bool, default: True
+         是否启用多线程下载数据，默认True
+         - True:  启用多线程下载数据
+         - False: 禁用多线程下载
+     process_count: int, default: None
+         启用多线程下载时，同时开启的线程数，默认值为设备的CPU核心数
+     chunk_size: int, default: 100
+         保存数据到本地时，为了减少文件/数据库读取次数，将下载的数据累计一定数量后
+         再批量保存到本地，chunk_size即批量，默认值100
 
     Returns
     -------
     None
 
     Examples
     --------
-    >>> refill_data_source(tables='stock_basic')
+    >>> import qteasy as qt
+    >>> qt.refill_data_source(tables='stock_basic')
 
     """
     from .database import DataSource
     if data_source is None:
         data_source = qteasy.QT_DATA_SOURCE
     if not isinstance(data_source, DataSource):
         raise TypeError(f'A DataSource object must be passed, got {type(data_source)} instead.')
@@ -738,16 +734,15 @@
     Parameters
     ----------
     htypes: [str, list]
         需要获取的历史数据类型集合，可以是以逗号分隔的数据类型字符串或者数据类型字符列表，
         如以下两种输入方式皆合法且等效：
          - str:     'open, high, low, close'
          - list:    ['open', 'high', 'low', 'close']
-        特殊htypes的处理：
-        以下特殊htypes将被特殊处理"
+        特殊htypes的处理，以下特殊htypes将被特殊处理，返回特定的数，详见示例
          - wt-000300.SH:
             指数权重数据，如果htype是一个wt开头的复合体，则获取该指数的股票权重数据
             获取的数据的htypes同样为wt-000300.SH型
          - close-000300.SH:
             给出一个htype和ts_code的复合体，且shares为None时，返回不含任何share
             的参考数据
     shares: [str, list] 等同于symbols
@@ -786,16 +781,14 @@
          - forward / fw / f: 前复权
     as_data_frame: bool, Default: False
         是否返回DataFrame对象，True时返回HistoryPanel对象
     group_by: str, 默认'shares'
         如果返回DataFrame对象，设置dataframe的分组策略
         - 'shares' / 'share' / 's': 每一个share组合为一个dataframe
         - 'htypes' / 'htype' / 'h': 每一个htype组合为一个dataframe
-    flatten: bool, 默认False # TODO: new in next version
-        是否返回平坦的数据，即数据的列名为htype的组合
     **kwargs:
         用于生成trade_time_index的参数，包括：
         drop_nan: bool
             是否保留全NaN的行
         resample_method: str
             如果数据需要升频或降频时，调整频率的方法
             调整数据频率分为数据降频和升频，在两种不同情况下，可用的method不同：
@@ -829,100 +822,176 @@
             - 'zero': 使用0值填充缺失数据：
                 [1, 2, 3] 填充后变为: [0, 1, 0, 2, 0, 3, 0]
         b_days_only: bool 默认True
             是否强制转换自然日频率为工作日，即：
             'D' -> 'B'
             'W' -> 'W-FRI'
             'M' -> 'BM'
-        trade_time_only: bool, 默认True
+        trade_time_only: bool, default True
             为True时 仅生成交易时间段内的数据，交易时间段的参数通过**kwargs设定
-        include_start:
+        include_start: bool, default True
             日期时间序列是否包含开始日期/时间
-        include_end:
+        include_end: bool, default True
             日期时间序列是否包含结束日期/时间
-        start_am:
+        start_am:, str
             早晨交易时段的开始时间
-        end_am:
+        end_am:, str
             早晨交易时段的结束时间
-        include_start_am:
+        include_start_am: bool
             早晨交易时段是否包括开始时间
-        include_end_am:
+        include_end_am: bool
             早晨交易时段是否包括结束时间
-        start_pm:
+        start_pm: str
             下午交易时段的开始时间
-        end_pm:
+        end_pm: str
             下午交易时段的结束时间
-        include_start_pm
+        include_start_pm: bool
             下午交易时段是否包含开始时间
-        include_end_pm
+        include_end_pm: bool
             下午交易时段是否包含结束时间
 
     Returns
     -------
     HistoryPanel:
         如果设置as_data_frame为False，则返回一个HistoryPanel对象
     Dict of DataFrame:
         如果设置as_data_frame为True，则返回一个Dict，其值为多个DataFrames
 
     Examples
     --------
     >>> import qteasy as qt
+    # 给出历史数据类型和证券代码，起止时间，可以获取该时间段内该股票的历史数据
     >>> qt.get_history_data(htypes='open, high, low, close, vol', shares='000001.SZ', start='20191225', end='20200110')
     {'000001.SZ':
                   open   high    low  close         vol
-     2019-12-25  16.45  16.56  16.24  16.30   414917.98
-     2019-12-26  16.34  16.48  16.32  16.47   372033.86
-     2019-12-27  16.53  16.93  16.43  16.63  1042574.72
-     2019-12-30  16.46  16.63  16.10  16.57   976970.31
-     2019-12-31  16.57  16.63  16.31  16.45   704442.25
-     2020-01-02  16.65  16.95  16.55  16.87  1530231.87
-     2020-01-03  16.94  17.31  16.92  17.18  1116194.81
-     2020-01-06  17.01  17.34  16.91  17.07   862083.50
-     2020-01-07  17.13  17.28  16.95  17.15   728607.56
-     2020-01-08  17.00  17.05  16.63  16.66   847824.12
-     2020-01-09  16.81  16.93  16.53  16.79  1031636.65
-     2020-01-10  16.79  16.81  16.52  16.69   585548.45
-     }
-     # data can be extracted in different frequency, and also adjusted
-     >>> qt.get_history_data(htypes='open, high, low, close', shares='000001.SZ', start='20191229', end='20200106', freq='H', adj='b', asset_type='E')
+    2019-12-25  16.45  16.56  16.24  16.30   414917.98
+    2019-12-26  16.34  16.48  16.32  16.47   372033.86
+    2019-12-27  16.53  16.93  16.43  16.63  1042574.72
+    2019-12-30  16.46  16.63  16.10  16.57   976970.31
+    2019-12-31  16.57  16.63  16.31  16.45   704442.25
+    2020-01-02  16.65  16.95  16.55  16.87  1530231.87
+    2020-01-03  16.94  17.31  16.92  17.18  1116194.81
+    2020-01-06  17.01  17.34  16.91  17.07   862083.50
+    2020-01-07  17.13  17.28  16.95  17.15   728607.56
+    2020-01-08  17.00  17.05  16.63  16.66   847824.12
+    2020-01-09  16.81  16.93  16.53  16.79  1031636.65
+    2020-01-10  16.79  16.81  16.52  16.69   585548.45
+    }
+
+    >>> # 除了股票的价格数据以外，也可以获取基金、指数的价格数据，如下面的代码获取000300.SH的指数价格数
+    >>> qt.get_history_data(htypes='close', shares='000300.SH', start='20191225', end='20200105')
+    {'000300.SH':
+                  close
+    2019-12-25  3990.87
+    2019-12-26  4025.99
+    2019-12-27  4022.03
+    2019-12-30  4081.63
+    2019-12-31  4096.58
+    2020-01-02  4152.24
+    2020-01-03  4144.96
+    }
+    # 以及基金的净值数据
+    >>> qt.get_history_data(htypes='unit_nav, accum_nav', shares='000001.OF', start='20191225', end='20200105')
+    {'000001.OF':
+                unit_nav  accum_nav
+    2019-12-25     1.086      3.547
+    2019-12-26     1.096      3.557
+    2019-12-27     1.091      3.552
+    2019-12-30     1.100      3.561
+    2019-12-31     1.105      3.566
+    2020-01-02     1.123      3.584
+    2020-01-03     1.127      3.588
+    }
+
+    >>> # 不光价格数据，其他类型的数据也可以同时获取：
+    >>> qt.get_history_data(htypes='close, pe, pb', shares='000001.SZ', start='20191225', end='20200105')
+    {'000001.SZ':
+                close       pe      pb
+    2019-12-25  16.30  12.7454  1.1798
+    2019-12-26  16.47  12.8784  1.1921
+    2019-12-27  16.63  13.0035  1.2036
+    2019-12-30  16.57  12.9566  1.1993
+    2019-12-31  16.45  12.8627  1.1906
+    2020-01-02  16.87  13.1911  1.2210
+    2020-01-03  17.18  13.4335  1.2434
+    }
+    # 可以同时混合获取多只股票、指数、多种数据类型的数据，如果某些数据类型缺失，会用NaN填充，注意000001.SZ是股票平安银行，000001.SH是上证指数
+    >>> qt.get_history_data(htypes='close, pe, pb, total_mv, eps', shares='000001.SZ, 000001.SH', start='20191225', end='20200105')
+    {'000001.SZ':
+                close       pe      pb      total_mv   eps
+    2019-12-25  16.30  12.7454  1.1798  3.163165e+07   NaN
+    2019-12-26  16.47  12.8784  1.1921  3.196155e+07   NaN
+    2019-12-27  16.63  13.0035  1.2036  3.227204e+07   NaN
+    2019-12-30  16.57  12.9566  1.1993  3.215561e+07   NaN
+    2019-12-31  16.45  12.8627  1.1906  3.192274e+07  1.54
+    2020-01-02  16.87  13.1911  1.2210  3.273778e+07  1.54
+    2020-01-03  17.18  13.4335  1.2434  3.333937e+07  1.54,
+    '000001.SH':
+                  close     pe    pb      total_mv  eps
+    2019-12-25  2981.88  13.74  1.38  3.987686e+13  NaN
+    2019-12-26  3007.35  13.85  1.39  4.020871e+13  NaN
+    2019-12-27  3005.04  13.85  1.39  4.019086e+13  NaN
+    2019-12-30  3040.02  14.00  1.40  4.064796e+13  NaN
+    2019-12-31  3050.12  14.05  1.41  4.079249e+13  NaN
+    2020-01-02  3085.20  14.22  1.42  4.128453e+13  NaN
+    2020-01-03  3083.79  14.22  1.42  4.127933e+13  NaN
+    }
+
+    >>> # 通过设置freq参数，可以获取不同频率的K线数据，如设置freq='H'可以获取1小时频率的数据
+    >>> qt.get_history_data(htypes='open, high, low, close', shares='000001.SZ', start='20191229', end='20200106', freq='H', adj='b', asset_type='E')
      {'000001.SZ':
                                 open        high         low       close
-     2019-12-30 10:00:00  1796.92174  1796.92174  1796.92174  1796.92174
-     2019-12-30 11:00:00  1790.37160  1800.19681  1758.71259  1786.00484
-     2019-12-30 14:00:00  1811.11371  1813.29709  1795.83005  1806.74695
-     2019-12-30 15:00:00  1805.65526  1808.93033  1793.64667  1808.93033
-     2019-12-31 10:00:00  1808.93033  1808.93033  1808.93033  1808.93033
-     2019-12-31 11:00:00  1806.74695  1806.74695  1780.54639  1788.18822
-     2019-12-31 14:00:00  1786.00484  1788.18822  1781.63808  1786.00484
-     2019-12-31 15:00:00  1786.00484  1796.92174  1783.82146  1795.83005
-     2020-01-02 10:00:00  1817.66385  1817.66385  1817.66385  1817.66385
-     2020-01-02 11:00:00  1819.84723  1848.23117  1807.83864  1840.58934
-     2020-01-02 14:00:00  1842.77272  1847.13948  1828.58075  1843.86441
-     2020-01-02 15:00:00  1843.86441  1844.95610  1836.22258  1841.68103
-     2020-01-03 10:00:00  1849.32286  1849.32286  1849.32286  1849.32286
-     2020-01-03 11:00:00  1849.32286  1879.89018  1849.32286  1877.70680
-     2020-01-03 14:00:00  1863.51483  1889.71539  1863.51483  1884.25694
-     2020-01-03 15:00:00  1884.25694  1884.25694  1872.24835  1875.52342
-     }
-     # if you want data to be filled also in non-trading days
-     >>> qt.get_history_data(htypes='open, high, low, close, vol', shares='000001.SZ', start='20191225', end='20200105', b_days_only=False)
+    2019-12-30 10:00:00  1796.92174  1796.92174  1796.92174  1796.92174
+    2019-12-30 11:00:00  1790.37160  1800.19681  1758.71259  1786.00484
+    2019-12-30 14:00:00  1811.11371  1813.29709  1795.83005  1806.74695
+    2019-12-30 15:00:00  1805.65526  1808.93033  1793.64667  1808.93033
+    2019-12-31 10:00:00  1808.93033  1808.93033  1808.93033  1808.93033
+    2019-12-31 11:00:00  1806.74695  1806.74695  1780.54639  1788.18822
+    2019-12-31 14:00:00  1786.00484  1788.18822  1781.63808  1786.00484
+    2019-12-31 15:00:00  1786.00484  1796.92174  1783.82146  1795.83005
+    2020-01-02 10:00:00  1817.66385  1817.66385  1817.66385  1817.66385
+    2020-01-02 11:00:00  1819.84723  1848.23117  1807.83864  1840.58934
+    2020-01-02 14:00:00  1842.77272  1847.13948  1828.58075  1843.86441
+    2020-01-02 15:00:00  1843.86441  1844.95610  1836.22258  1841.68103
+    2020-01-03 10:00:00  1849.32286  1849.32286  1849.32286  1849.32286
+    2020-01-03 11:00:00  1849.32286  1879.89018  1849.32286  1877.70680
+    2020-01-03 14:00:00  1863.51483  1889.71539  1863.51483  1884.25694
+    2020-01-03 15:00:00  1884.25694  1884.25694  1872.24835  1875.52342
+    }
+
+    >>> # 可以设置b_days_only参数来将价格填充到非交易日，形成完整的日期序列
+    >>> qt.get_history_data(htypes='open, high, low, close, vol', shares='000001.SZ', start='20191225', end='20200105', b_days_only=False)
     {'000001.SZ':
                   open   high    low  close         vol
      2019-12-25  16.45  16.56  16.24  16.30   414917.98
      2019-12-26  16.34  16.48  16.32  16.47   372033.86
      2019-12-27  16.53  16.93  16.43  16.63  1042574.72
      2019-12-28  16.53  16.93  16.43  16.63  1042574.72
      2019-12-29  16.53  16.93  16.43  16.63  1042574.72
      2019-12-30  16.46  16.63  16.10  16.57   976970.31
      2019-12-31  16.57  16.63  16.31  16.45   704442.25
      2020-01-01  16.57  16.63  16.31  16.45   704442.25
      2020-01-02  16.65  16.95  16.55  16.87  1530231.87
      2020-01-03  16.94  17.31  16.92  17.18  1116194.81
      2020-01-04  16.94  17.31  16.92  17.18  1116194.81
-     2020-01-05  16.94  17.31  16.92  17.18  1116194.81}
+     2020-01-05  16.94  17.31  16.92  17.18  1116194.81
+     }
+
+    >>> # 使用特殊的htypes，可以获取特定的数据，如指数权重数据，下面的代码获取000001.SZ在HS300指数重的权重数据，单位为百分比
+    >>> qt.get_history_data(htypes='wt-000300.SH', shares='000001.SZ, 000002.SZ', start='20191225', end='20200105')
+    {'000001.SZ':
+                wt-000300.SH
+    2020-01-02        1.1714
+    2020-01-03        1.1714,
+    '000002.SZ':
+                wt-000300.SH
+    2020-01-02        1.3595
+    2020-01-03        1.3595
+    }
+
     """
 
     if htypes is None:
         raise ValueError(f'htype should not be None')
     if symbols is not None and shares is None:
         shares = symbols
     if shares is None:
```

### Comparing `qteasy-1.2.6/qteasy/database.py` & `qteasy-1.2.7/qteasy/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -2576,15 +2576,15 @@
         """ 格式化打印database对象的各种主要信息
 
         Returns
         -------
         """
         raise NotImplementedError
 
-    def overview(self, tables=None, print_out=True, include_sys_tables=False):
+    def overview(self, tables=None, print_out=True, include_sys_tables=False) -> pd.DataFrame:
         """ 以表格形式列出所有数据表的当前数据状态
 
         Parameters
         ----------
         tables: str or list of str, Default None
             指定要列出的数据表，如果为None则列出所有数据表
         print_out: bool, Default True
@@ -4108,15 +4108,15 @@
         if not string_form:
             return size, rows
         if human:
             return f'{human_file_size(size)}', f'{human_units(rows)}'
         else:
             return f'{size}', f'{rows}'
 
-    def get_table_info(self, table, verbose=True, print_info=True, human=True):
+    def get_table_info(self, table, verbose=True, print_info=True, human=True) -> tuple:
         """ 获取并打印数据表的相关信息，包括数据表是否已有数据，数据量大小，占用磁盘空间、数据覆盖范围，
             以及数据下载方法
 
         Parameters:
         -----------
         table: str
             数据表名称
@@ -4989,17 +4989,19 @@
             # 检查trade_calendar中是否有足够的数据，如果没有，需要包含trade_calendar表：
             if 'trade_calendar' not in tables_to_refill:
                 if refresh_trade_calendar:
                     tables_to_refill.add('trade_calendar')
                 else:
                     # 检查trade_calendar中是否已有数据，且最新日期是否足以覆盖今天，如果没有数据或数据不足，也需要添加该表
                     latest_calendar_date = self.get_table_info('trade_calendar', print_info=False)[11]
-                    if latest_calendar_date == 'N/A':
-                        tables_to_refill.add('trade_calendar')
-                    elif pd.to_datetime('today') >= pd.to_datetime(latest_calendar_date):
+                    try:
+                        latest_calendar_date = pd.to_datetime(latest_calendar_date)
+                        if pd.to_datetime('today') >= pd.to_datetime(latest_calendar_date):
+                            tables_to_refill.add('trade_calendar')
+                    except:
                         tables_to_refill.add('trade_calendar')
 
         # 开始逐个下载清单中的表数据
         table_count = 0
         import time
         for table in table_master.index:
             # 逐个下载数据并写入本地数据表中
```

### Comparing `qteasy-1.2.6/qteasy/emfuncs.py` & `qteasy-1.2.7/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/evaluate.py` & `qteasy-1.2.7/qteasy/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     return res
 
 
 def evaluate(looped_values: pd.DataFrame,
              hist_benchmark: pd.DataFrame,
              benchmark_data: str,
              cash_plan,
-             indicators: str = 'final_value')->dict:
+             indicators: str = 'final_value') -> dict:
     """ 根据args获取相应的性能指标，所谓性能指标是指根据生成的交易清单、回测结果、参考数据类型及投资计划输出各种性能指标
         返回一个dict，包含所有需要的indicators
 
     这里生成的indicators包含：
     - final_value:        回测区间最后一天的总资产金额
     - loop_start:        回测区间起始日
     - loop_end:          回测区间终止日
@@ -150,17 +150,17 @@
     - months:            回测历史周期总月数
     - years:             回测历史周期年份数
     - oper_count         操作数量
     - total_invest       总投入资金数量
     - total_fee          总交易费用
     - rtn:               回测的总回报率
     - annual_rtn:        回测的年均回报率
-    - mdd:               最大回测
-    - peak_date:         最大回测峰值日期
-    - valley_date:       最大回测谷值日期
+    - mdd:               最大回撤（从前期最高点开始计算最大跌幅）
+    - peak_date:         最大回撤峰值日期（前期高点日期）
+    - valley_date:       最大回撤谷值日期（最大跌幅日期）
     - volatility:        回测区间波动率（最后一日波动率）
     - ref_rtn:           benchmark参照指标的回报率
     - ref_annual_rtn:    benchmark参照指标的年均回报率
     - beta:              回测区间的beta值
     - sharp:             回测区间的夏普率
     - alpha:             回测区间的阿尔法值
     - info:              回测区间的信息比率
@@ -180,14 +180,25 @@
     indicators: str, Default: 'final_value'
         评价指标，逗号分隔的多个评价指标
 
     Returns
     -------
     performance_dict: dict: 一个字典，每个指标的各种值
     """
+    # validate input
+
+    if not isinstance(hist_benchmark, pd.DataFrame):
+        raise TypeError(f'reference value should be pandas DataFrame, got {type(hist_benchmark)} instead!')
+    if not isinstance(looped_values, pd.DataFrame):
+        raise TypeError(f'looped value should be pandas DataFrame, got {type(looped_values)} instead')
+    if benchmark_data not in hist_benchmark.columns:
+        raise KeyError(f'reference data type \'{benchmark_data}\' can not be found in reference data')
+    if not isinstance(cash_plan, qteasy.CashPlan):
+        raise TypeError(f'Cash plan is not valid, got {type(cash_plan)} instead')
+
     indicator_list = str_to_list(indicators)
     performance_dict = dict()
     # 评价回测结果——计算回测终值，这是默认输出结果
     performance_dict['final_value'] = eval_fv(looped_val=looped_values)
     performance_dict['loop_start'] = looped_values.index[0]
     performance_dict['loop_end'] = looped_values.index[-1]
     performance_dict['complete_values'] = looped_values
@@ -240,15 +251,14 @@
         performance_dict['info'] = eval_calmar(looped_values)
     if bool(performance_dict):
         return performance_dict
     else:
         return performance_dict
 
 
-# TODO: move all variable validations from evaluation sub functions to evaluate() function -> 2020/11/11
 def _get_yearly_span(value_df: pd.DataFrame) -> float:
     """ 计算回测结果的时间跨度，单位为年。一年按照365天计算
 
     Parameters
     ----------
     value_df: pd.DataFrame
         回测结果
@@ -269,33 +279,33 @@
         except:
             raise ValueError(f'The yearly time span of the looped value can not be calculated, '
                              f'DataFrame index should be time or number format!, '
                              f'got {type(first_day)} and {type(last_day)}')
     return total_year
 
 
-def eval_benchmark(looped_value, reference_value, reference_data):
+def eval_benchmark(looped_values, hist_benchmark, benchmark_data):
     """ 参考标准年化收益率。具体计算方式为 （(参考标准最终指数 / 参考标准初始指数) ** 1 / 回测交易年数 - 1）
 
     Parameters
     ----------
-    looped_value: pd.DataFrame
-    reference_value: pd.DataFrame
-    reference_data: str
+    looped_values: pd.DataFrame
+    hist_benchmark: pd.DataFrame
+    benchmark_data: str
 
     Returns
     -------
     tuple: (total_rtn, annual_rtn)
     """
-    total_year = _get_yearly_span(looped_value)
+    total_year = _get_yearly_span(looped_values)
     try:
-        rtn_data = reference_value[reference_data]
-        rtn = (rtn_data[looped_value.index[-1]] / rtn_data[looped_value.index[0]])
+        rtn_data = hist_benchmark[benchmark_data]
+        rtn = (rtn_data[looped_values.index[-1]] / rtn_data[looped_values.index[0]])
         return rtn - 1, rtn ** (1 / total_year) - 1.
-    except:
+    except Exception:
         pass
         return 0., 0.
 
 
 def eval_alpha(looped_value, total_invest, reference_value, reference_data, risk_free_ror: float = 0.0035):
     """ 回测结果评价函数：alpha系数
     阿尔法系数(α)是基金的超额收益和按照β系数计算的期望收益之间的差额。 其计算方法如下：超额收益是基金的实际收益减去无
@@ -370,20 +380,15 @@
     reference_data: str:
         参考结果的数据类型，如close, open, low 等
 
     Returns
     -------
     beta: float
     """
-    if not isinstance(reference_value, pd.DataFrame):
-        raise TypeError(f'reference value should be pandas DataFrame, got {type(reference_value)} instead!')
-    if not isinstance(looped_value, pd.DataFrame):
-        raise TypeError(f'looped value should be pandas DataFrame, got {type(looped_value)} instead')
-    if reference_data not in reference_value.columns:
-        raise KeyError(f'reference data type \'{reference_data}\' can not be found in reference data')
+
     # 计算或获取每日收益率
     if 'pct_change' not in looped_value.columns:
         looped_value['pct_change'] = (looped_value['value'] / looped_value['value'].shift(1)) - 1
     ref = reference_value[reference_data]
     ref_ret = (ref / ref.shift(1)) - 1
     if len(looped_value) > 250:
         ret_dev = looped_value['pct_change'].rolling(250).var()
@@ -438,16 +443,14 @@
     logarithm: bool, Default: True
         是否计算指数收益率，默认为True，计算对数收益率，为False时计算常规收益率
 
     Returns
     -------
     volatility: float
     """
-    assert isinstance(looped_value, pd.DataFrame), \
-        f'TypeError, looped value should be pandas DataFrame, got {type(looped_value)} instead'
     if looped_value.empty:
         return -np.inf
     if logarithm:
         ret = np.log(looped_value['value'] / looped_value['value'].shift(1))
     else:
         ret = (looped_value['value'] / looped_value['value'].shift(1)) - 1
     if len(ret) > 250:
@@ -526,16 +529,14 @@
     tuple: (max_drawdown, peak_date, valley_date, recover_date, dd_df)
     max_drawdown: 最大回撤
     peak_date: 峰值日期
     valley_date: 谷值日期
     recover_date: 回撤恢复日期
     dd_df:   完整的DataFrame，包含最大的五个回撤区间的全部信息
     """
-    assert isinstance(looped_value, pd.DataFrame), \
-        f'TypeError, looped value should be pandas DataFrame, got {type(looped_value)} instead'
     if looped_value.empty:
         return -np.inf
     cummax = looped_value['value'].cummax()
     looped_value['underwater'] = (looped_value['value'] - cummax) / cummax
     drawdown_sign = np.sign(looped_value.underwater)
     diff = drawdown_sign - drawdown_sign.shift(1)
     drawdown_starts = np.where(diff == -1)[0]
@@ -581,16 +582,14 @@
         回测器生成输出的交易模拟记录
 
     Returns
     -------
     perf: float，应用该评价方法对回测模拟结果的评价分数
 
     """
-    if not isinstance(looped_val, pd.DataFrame):
-        raise TypeError(f'looped value should be pandas DataFrame, got {type(looped_val)} instead')
     if looped_val.empty:
         return -np.inf
     if 'value' not in looped_val:
         raise KeyError(f'the key \'value\' can not be found in given looped value!')
 
     perf = looped_val.at[looped_val.index[-1], 'value']
     return perf
@@ -620,18 +619,14 @@
     tuple: (perf, annual_perf, skew, kurtosis, looped_val)
     perf: float，应用该评价方法对回测模拟结果的评价分数
     annual_perf: float，应用该评价方法对回测模拟结果的评价分数
     skew: float，应用该评价方法对回测模拟结果的评价分数
     kurtosis: float，应用该评价方法对回测模拟结果的评价分数
     looped_val: pd.DataFrame，回测器生成输出的交易模拟记录
     """
-    assert isinstance(looped_val, pd.DataFrame), \
-        f'TypeError, looped value should be pandas DataFrame, got {type(looped_val)} instead'
-    assert isinstance(cash_plan, qteasy.CashPlan), \
-        f'TypeError, cash plan type not valid, got {type(cash_plan)} instead'
     if looped_val.empty:
         return -np.inf, -np.inf, np.nan, np.nan, pd.DataFrame()
     invest_plan = cash_plan.plan
     looped_val['invest'] = invest_plan.amount
     looped_val = looped_val.fillna(0)
     looped_val['invest'] = looped_val.invest.cumsum()
     looped_val['rtn'] = looped_val.value / looped_val['invest'] - 1
```

### Comparing `qteasy-1.2.6/qteasy/finance.py` & `qteasy-1.2.7/qteasy/finance.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/history.py` & `qteasy-1.2.7/qteasy/history.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/optimization.py` & `qteasy-1.2.7/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/qt_operator.py` & `qteasy-1.2.7/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/space.py` & `qteasy-1.2.7/qteasy/space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/strategy.py` & `qteasy-1.2.7/qteasy/strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/tafuncs.py` & `qteasy-1.2.7/qteasy/tafuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/trade_recording.py` & `qteasy-1.2.7/qteasy/trade_recording.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/trader.py` & `qteasy-1.2.7/qteasy/trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/trader_cli.py` & `qteasy-1.2.7/qteasy/trader_cli.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/trader_tui.py` & `qteasy-1.2.7/qteasy/trader_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/trading_util.py` & `qteasy-1.2.7/qteasy/trading_util.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/tsfuncs.py` & `qteasy-1.2.7/qteasy/tsfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/tui_style.tcss` & `qteasy-1.2.7/qteasy/tui_style.tcss`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/utilfuncs.py` & `qteasy-1.2.7/qteasy/utilfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy/visual.py` & `qteasy-1.2.7/qteasy/visual.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/qteasy.egg-info/PKG-INFO` & `qteasy-1.2.7/qteasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.2.6
+Version: 1.2.7
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
 Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
 Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
 License: Copyright <2019> <JACKIE PENG>
@@ -58,14 +58,16 @@
 Provides-Extra: feather
 Requires-Dist: pyarrow>=3; extra == "feather"
 Provides-Extra: dev
 Requires-Dist: ta-lib; extra == "dev"
 Requires-Dist: pymysql>=1.0.0; extra == "dev"
 Requires-Dist: pyarrow>=3; extra == "dev"
 
+![png](docs/source/img/qteasy_logo_horizontal.png)
+
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
 [![Build Status](https://app.travis-ci.com/shepherdpp/qteasy.svg?branch=master)](https://app.travis-ci.com/shepherdpp/qteasy)
 [![Documentation Status](https://readthedocs.org/projects/qteasy/badge/?version=latest)](https://qteasy.readthedocs.io/zh/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/shepherdpp/qteasy)
@@ -106,15 +108,15 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.2.6`
+- Latest Version: `1.2.7`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
```

### Comparing `qteasy-1.2.6/qteasy.egg-info/SOURCES.txt` & `qteasy-1.2.7/qteasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/setup.cfg` & `qteasy-1.2.7/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qteasy
-version = 1.2.6
+version = 1.2.7
 author = Jackie PENG
 author_email = jackie.pengzhao@gmail.com
 maintainer = Jackie PENG
 description = A fast quantitative investment tool kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shepherdpp/qteasy
```

### Comparing `qteasy-1.2.6/tests/test_broker.py` & `qteasy-1.2.7/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_cashplan.py` & `qteasy-1.2.7/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_config.py` & `qteasy-1.2.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_core_sub_funcs.py` & `qteasy-1.2.7/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_cost.py` & `qteasy-1.2.7/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_datasource.py` & `qteasy-1.2.7/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_eastmoney.py` & `qteasy-1.2.7/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_evaluations.py` & `qteasy-1.2.7/tests/test_evaluations.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         self.assertAlmostEqual(eval_fv(self.test_data3), 6.95068113)
         self.assertAlmostEqual(eval_fv(self.test_data4), 8.86508591)
         self.assertAlmostEqual(eval_fv(self.test_data5), 4.58627048)
         self.assertAlmostEqual(eval_fv(self.test_data6), 4.10346795)
         self.assertAlmostEqual(eval_fv(self.test_data7), 2.92532313)
         self.assertAlmostEqual(eval_fv(pd.DataFrame()), -np.inf)
         print(f'Error testing')
-        self.assertRaises(TypeError, eval_fv, 15)
+        self.assertRaises(AttributeError, eval_fv, 15)
         self.assertRaises(KeyError,
                           eval_fv,
                           pd.DataFrame([1, 2, 3], columns=['non_value']))
 
     # noinspection PyTypeChecker
     def test_max_drawdown(self):
         print(f'test with test arr and empty DataFrame')
@@ -361,15 +361,15 @@
         self.assertTrue(np.isnan(eval_max_drawdown(self.test_data6)[3]))
         self.assertAlmostEqual(eval_max_drawdown(self.test_data7)[0], 0.783577449)
         self.assertEqual(eval_max_drawdown(self.test_data7)[1], 17)
         self.assertEqual(eval_max_drawdown(self.test_data7)[2], 51)
         self.assertTrue(np.isnan(eval_max_drawdown(self.test_data7)[3]))
         self.assertEqual(eval_max_drawdown(pd.DataFrame()), -np.inf)
         print(f'Error testing')
-        self.assertRaises(TypeError, eval_fv, 15)
+        self.assertRaises(Exception, eval_fv, 15)
         self.assertRaises(KeyError,
                           eval_fv,
                           pd.DataFrame([1, 2, 3], columns=['non_value']))
         # test max drawdown == 0:
         # TODO: investigate: how does divide by zero change?
         self.assertAlmostEqual(eval_max_drawdown(self.test_data4 - 5)[0], 1.0770474121951792)
         self.assertEqual(eval_max_drawdown(self.test_data4 - 5)[1], 14)
@@ -398,15 +398,15 @@
         self.assertAlmostEqual(eval_volatility(self.test_data3, logarithm=False), 0.655331424)
         self.assertAlmostEqual(eval_volatility(self.test_data4, logarithm=False), 0.692683021)
         self.assertAlmostEqual(eval_volatility(self.test_data5, logarithm=False), 1.09602969)
         self.assertAlmostEqual(eval_volatility(self.test_data6, logarithm=False), 1.774789504)
         self.assertAlmostEqual(eval_volatility(self.test_data7, logarithm=False), 2.003329156)
 
         self.assertEqual(eval_volatility(pd.DataFrame()), -np.inf)
-        self.assertRaises(AssertionError, eval_volatility, [1, 2, 3])
+        self.assertRaises(AttributeError, eval_volatility, [1, 2, 3])
 
         # 测试长数据的Volatility计算
         expected_volatility = np.array([np.nan, np.nan, np.nan, np.nan, np.nan,
                                         np.nan, np.nan, np.nan, np.nan, np.nan,
                                         np.nan, np.nan, np.nan, np.nan, np.nan,
                                         np.nan, np.nan, np.nan, np.nan, np.nan,
                                         np.nan, np.nan, np.nan, np.nan, np.nan,
@@ -631,17 +631,17 @@
         self.assertAlmostEqual(eval_beta(self.test_data2, reference, 'value'), -0.017148939)
         self.assertAlmostEqual(eval_beta(self.test_data3, reference, 'value'), -0.042204233)
         self.assertAlmostEqual(eval_beta(self.test_data4, reference, 'value'), -0.15652986)
         self.assertAlmostEqual(eval_beta(self.test_data5, reference, 'value'), -0.049195532)
         self.assertAlmostEqual(eval_beta(self.test_data6, reference, 'value'), -0.026995082)
         self.assertAlmostEqual(eval_beta(self.test_data7, reference, 'value'), -0.01147809)
 
-        self.assertRaises(TypeError, eval_beta, [1, 2, 3], reference, 'value')
-        self.assertRaises(TypeError, eval_beta, self.test_data3, [1, 2, 3], 'value')
-        self.assertRaises(KeyError, eval_beta, self.test_data3, reference, 'not_found_value')
+        self.assertRaises(Exception, eval_beta, [1, 2, 3], reference, 'value')
+        self.assertRaises(Exception, eval_beta, self.test_data3, [1, 2, 3], 'value')
+        self.assertRaises(Exception, eval_beta, self.test_data3, reference, 'not_found_value')
 
         # 测试长数据的beta计算
         expected_beta = np.array([np.nan, np.nan, np.nan, np.nan, np.nan,
                                   np.nan, np.nan, np.nan, np.nan, np.nan,
                                   np.nan, np.nan, np.nan, np.nan, np.nan,
                                   np.nan, np.nan, np.nan, np.nan, np.nan,
                                   np.nan, np.nan, np.nan, np.nan, np.nan,
```

### Comparing `qteasy-1.2.6/tests/test_fast_experiments.py` & `qteasy-1.2.7/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_historypanel.py` & `qteasy-1.2.7/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_loop.py` & `qteasy-1.2.7/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_operator_and_strategy.py` & `qteasy-1.2.7/tests/test_operator_and_strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_qt.py` & `qteasy-1.2.7/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_space.py` & `qteasy-1.2.7/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_ta_funcs.py` & `qteasy-1.2.7/tests/test_ta_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_trader.py` & `qteasy-1.2.7/tests/test_trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_trader_shell.py` & `qteasy-1.2.7/tests/test_trader_shell.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_trading.py` & `qteasy-1.2.7/tests/test_trading.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_tui.py` & `qteasy-1.2.7/tests/test_tui.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_tushare.py` & `qteasy-1.2.7/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_utilityfuncs.py` & `qteasy-1.2.7/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.2.6/tests/test_visual.py` & `qteasy-1.2.7/tests/test_visual.py`

 * *Files identical despite different names*

