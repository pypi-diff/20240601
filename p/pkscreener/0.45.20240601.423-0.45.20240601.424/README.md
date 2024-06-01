# Comparing `tmp/pkscreener-0.45.20240601.423.tar.gz` & `tmp/pkscreener-0.45.20240601.424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240601.423.tar", last modified: Sat Jun  1 08:56:09 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240601.424.tar", last modified: Sat Jun  1 10:57:26 2024, max compression
```

## Comparing `pkscreener-0.45.20240601.423.tar` & `pkscreener-0.45.20240601.424.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:56:09.559430 pkscreener-0.45.20240601.423/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-01 08:54:10.000000 pkscreener-0.45.20240601.423/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 08:54:10.000000 pkscreener-0.45.20240601.423/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-01 08:56:09.559430 pkscreener-0.45.20240601.423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-06-01 08:54:10.000000 pkscreener-0.45.20240601.423/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:56:09.555430 pkscreener-0.45.20240601.423/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:56:09.559430 pkscreener-0.45.20240601.423/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    34830 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    47230 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   163367 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    56446 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 08:56:02.000000 pkscreener-0.45.20240601.423/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   146905 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    60753 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    34702 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:56:09.555430 pkscreener-0.45.20240601.423/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-01 08:56:09.000000 pkscreener-0.45.20240601.423/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-01 08:56:09.000000 pkscreener-0.45.20240601.423/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:56:09.000000 pkscreener-0.45.20240601.423/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-01 08:56:09.000000 pkscreener-0.45.20240601.423/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:56:09.000000 pkscreener-0.45.20240601.423/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-01 08:56:09.000000 pkscreener-0.45.20240601.423/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 08:56:09.000000 pkscreener-0.45.20240601.423/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 08:56:09.563430 pkscreener-0.45.20240601.423/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-06-01 08:54:11.000000 pkscreener-0.45.20240601.423/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:57:26.515632 pkscreener-0.45.20240601.424/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-01 10:57:26.515632 pkscreener-0.45.20240601.424/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:57:26.511632 pkscreener-0.45.20240601.424/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:57:26.515632 pkscreener-0.45.20240601.424/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34830 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47230 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   163367 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56446 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 10:57:20.000000 pkscreener-0.45.20240601.424/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   146905 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    60748 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34702 2024-06-01 10:55:37.000000 pkscreener-0.45.20240601.424/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:57:26.511632 pkscreener-0.45.20240601.424/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-01 10:57:26.000000 pkscreener-0.45.20240601.424/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-01 10:57:26.000000 pkscreener-0.45.20240601.424/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:57:26.000000 pkscreener-0.45.20240601.424/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-01 10:57:26.000000 pkscreener-0.45.20240601.424/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:57:26.000000 pkscreener-0.45.20240601.424/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-01 10:57:26.000000 pkscreener-0.45.20240601.424/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 10:57:26.000000 pkscreener-0.45.20240601.424/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 10:57:26.515632 pkscreener-0.45.20240601.424/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-06-01 10:55:38.000000 pkscreener-0.45.20240601.424/setup.py
```

### Comparing `pkscreener-0.45.20240601.423/LICENSE` & `pkscreener-0.45.20240601.424/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/LICENSE-Others` & `pkscreener-0.45.20240601.424/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/PKG-INFO` & `pkscreener-0.45.20240601.424/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240601.423
+Version: 0.45.20240601.424
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240601.423.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240601.424.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240601.423/README.md` & `pkscreener-0.45.20240601.424/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240601.423/pkscreener/__init__.py` & `pkscreener-0.45.20240601.424/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/classes/keys.py` & `pkscreener-0.45.20240601.424/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/courbd.ttf` & `pkscreener-0.45.20240601.424/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/globals.py` & `pkscreener-0.45.20240601.424/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240601.424/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240601.424/pkscreener/pkscreenerbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 except ImportError:
     import _thread as thread
 
 import traceback
 from datetime import datetime
 from time import sleep
 from telegram import __version__ as TG_VER
-from telegram.constants import PARSEMODE_HTML
+from telegram.constants import ParseMode
 
 start_time = datetime.now()
 MINUTES_2_IN_SECONDS = 120
 OWNER_USER = "Itsonlypk"
 
 from PKDevTools.classes.Telegram import get_secrets
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
@@ -224,15 +224,15 @@
         await update.message.reply_text(
             menuText,
             reply_markup=reply_markup,
         )
     await context.bot.send_message(
         chat_id=int(f"-{Channel_Id}"),
         text=f"Name: {user.first_name}, Username:@{user.username} with ID: {str(user.id)} started using the bot!\n{chosenBotMenuOption}",
-        parse_mode=PARSEMODE_HTML,
+        parse_mode=ParseMode.HTML,
     )
     # Tell ConversationHandler that we're in state `FIRST` now
     return START_ROUTES
 
 def removeMonitorFile():
     from PKDevTools.classes import Archiver
     configManager.getConfig(ConfigManager.parser)
@@ -561,15 +561,15 @@
             update=update,
         )
     try:
         if optionChoices != "":
             await context.bot.send_message(
                 chat_id=int(f"-{Channel_Id}"),
                 text=f"Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> submitted scan request <b>{optionChoices}</b> to the bot!",
-                parse_mode=PARSEMODE_HTML,
+                parse_mode=ParseMode.HTML,
             )
     except Exception:# pragma: no cover
         await start(update, context)
     menuText =  menuText.replace("\n     ","\n").replace("\n    ","\n").replace(colorText.FAIL,"").replace(colorText.END,"")
     if not str(optionChoices.upper()).startswith("B"):
         await sendUpdatedMenu(
             menuText=menuText, update=update, context=context, reply_markup=reply_markup
@@ -756,23 +756,23 @@
         f"<pre>{html.escape(tb_string)}</pre>"
     )
 
     try:
         # Finally, send the message
         if "telegram.error.Conflict" not in message:
             await context.bot.send_message(
-                chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=PARSEMODE_HTML
+                chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
             )
     except Exception:# pragma: no cover
         try:
             if "telegram.error.Conflict" not in tb_string:
                 await context.bot.send_message(
                     chat_id=int(f"-{Channel_Id}"),
                     text=tb_string,
-                    parse_mode=PARSEMODE_HTML,
+                    parse_mode=ParseMode.HTML,
                 )
         except Exception:# pragma: no cover
             print(tb_string)
 
 
 async def command_handler(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     if _shouldAvoidResponse(update):
@@ -1095,15 +1095,15 @@
     )
 
 
 async def shareUpdateWithChannel(update, context, optionChoices=""):
     query = update.message or update.callback_query
     message = f"Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> began using ({optionChoices}) the bot!"
     await context.bot.send_message(
-        chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=PARSEMODE_HTML
+        chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
     )
 
 
 async def help_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     if _shouldAvoidResponse(update):
         return
     global bot_available
@@ -1125,15 +1125,15 @@
     if update is not None and update.message is not None:
         await update.message.reply_text(
             f"You can begin by typing in /start (Recommended) and hit send!\n\nOR\n\nChoose an option:\n{cmdText}\n\nWe recommend you start by clicking on this /start"
         )  #  \n\nThis bot restarts every hour starting at 5:30am IST until 10:30pm IST to keep it running on free servers. If it does not respond, please try again in a minutes to avoid the restart duration!
         query = update.message
         message = f"Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> began using the bot!"
         await context.bot.send_message(
-            chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=PARSEMODE_HTML
+            chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
         )
 
 
 def _shouldAvoidResponse(update):
     sentFrom = []
     if update.callback_query is not None:
         sentFrom.append(abs(update.callback_query.from_user.id))
```

### Comparing `pkscreener-0.45.20240601.423/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240601.424/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240601.424/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240601.423
+Version: 0.45.20240601.424
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240601.423.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240601.424.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240529.422/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.423/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240601.423/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240601.424/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240601.423/setup.py` & `pkscreener-0.45.20240601.424/setup.py`

 * *Files identical despite different names*

