# Comparing `tmp/investorzilla-3.3.tar.gz` & `tmp/investorzilla-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investorzilla-3.3.tar", last modified: Sun Apr  7 12:32:26 2024, max compression
+gzip compressed data, was "investorzilla-3.4.tar", last modified: Fri May 31 23:16:22 2024, max compression
```

## Comparing `investorzilla-3.3.tar` & `investorzilla-3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 12:32:26.000000 investorzilla-3.3/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    35149 2023-11-22 08:46:03.000000 investorzilla-3.3/LICENSE
--rw-r--r--   0 aviram    (1000) aviram    (1000)    46319 2024-04-07 12:32:26.000000 investorzilla-3.3/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)     4470 2023-12-12 11:07:53.000000 investorzilla-3.3/README.md
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 12:32:23.000000 investorzilla-3.3/investorzilla/
--rw-r--r--   0 aviram    (1000) aviram    (1000)      582 2024-03-10 10:12:17.000000 investorzilla-3.3/investorzilla/__init__.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1324 2023-11-22 08:43:50.000000 investorzilla-3.3/investorzilla/__main__.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 12:32:24.000000 investorzilla-3.3/investorzilla/currency/
--rw-r--r--   0 aviram    (1000) aviram    (1000)     2944 2023-12-15 20:49:46.000000 investorzilla-3.3/investorzilla/currency/brasil_banco_central.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     2374 2023-11-22 08:44:44.000000 investorzilla-3.3/investorzilla/currency/cryptocompare.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    12863 2024-02-10 08:46:46.000000 investorzilla-3.3/investorzilla/datacache.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    68186 2024-03-27 19:54:05.000000 investorzilla-3.3/investorzilla/fund.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     9784 2024-04-07 10:26:30.000000 investorzilla-3.3/investorzilla/investor.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 12:32:25.000000 investorzilla-3.3/investorzilla/marketindex/
--rw-r--r--   0 aviram    (1000) aviram    (1000)     3913 2023-11-20 22:28:04.000000 investorzilla-3.3/investorzilla/marketindex/brasil_banco_central.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1464 2023-11-22 08:44:43.000000 investorzilla-3.3/investorzilla/marketindex/federal_reserve.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     2906 2023-12-16 08:53:09.000000 investorzilla-3.3/investorzilla/marketindex/yahoo_finance.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    11871 2023-12-16 08:31:42.000000 investorzilla-3.3/investorzilla/monetary_time_series.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    16852 2024-03-27 19:52:35.000000 investorzilla-3.3/investorzilla/portfolio.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 12:32:26.000000 investorzilla-3.3/investorzilla/portfolios/
--rw-r--r--   0 aviram    (1000) aviram    (1000)      515 2023-11-22 08:44:43.000000 investorzilla-3.3/investorzilla/portfolios/app-credentials-for-google-sheets.json
--rw-r--r--   0 aviram    (1000) aviram    (1000)    12780 2024-03-27 19:39:50.000000 investorzilla-3.3/investorzilla/portfolios/google_sheets.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)     8472 2024-03-27 19:41:19.000000 investorzilla-3.3/investorzilla/portfolios/uri.py
--rw-r--r--   0 aviram    (1000) aviram    (1000)    28862 2024-04-07 12:29:19.000000 investorzilla-3.3/investorzilla/streamlit_ui.py
-drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-04-07 12:32:24.000000 investorzilla-3.3/investorzilla.egg-info/
--rw-r--r--   0 aviram    (1000) aviram    (1000)    46319 2024-04-07 12:32:19.000000 investorzilla-3.3/investorzilla.egg-info/PKG-INFO
--rw-r--r--   0 aviram    (1000) aviram    (1000)      841 2024-04-07 12:32:20.000000 investorzilla-3.3/investorzilla.egg-info/SOURCES.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2024-04-07 12:32:19.000000 investorzilla-3.3/investorzilla.egg-info/dependency_links.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       62 2024-04-07 12:32:19.000000 investorzilla-3.3/investorzilla.egg-info/entry_points.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)      159 2024-04-07 12:32:19.000000 investorzilla-3.3/investorzilla.egg-info/requires.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)       14 2024-04-07 12:32:19.000000 investorzilla-3.3/investorzilla.egg-info/top_level.txt
--rw-r--r--   0 aviram    (1000) aviram    (1000)     1494 2024-04-07 12:29:29.000000 investorzilla-3.3/pyproject.toml
--rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2024-04-07 12:32:26.000000 investorzilla-3.3/setup.cfg
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-05-31 23:16:22.000000 investorzilla-3.4/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    35149 2023-11-22 08:46:03.000000 investorzilla-3.4/LICENSE
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    46319 2024-05-31 23:16:22.000000 investorzilla-3.4/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     4470 2023-12-12 11:07:53.000000 investorzilla-3.4/README.md
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-05-31 23:16:19.000000 investorzilla-3.4/investorzilla/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      582 2024-03-10 10:12:17.000000 investorzilla-3.4/investorzilla/__init__.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1324 2023-11-22 08:43:50.000000 investorzilla-3.4/investorzilla/__main__.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-05-31 23:16:20.000000 investorzilla-3.4/investorzilla/currency/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     2944 2023-12-15 20:49:46.000000 investorzilla-3.4/investorzilla/currency/brasil_banco_central.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     2374 2023-11-22 08:44:44.000000 investorzilla-3.4/investorzilla/currency/cryptocompare.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    12863 2024-02-10 08:46:46.000000 investorzilla-3.4/investorzilla/datacache.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    68186 2024-03-27 19:54:05.000000 investorzilla-3.4/investorzilla/fund.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     9784 2024-04-07 10:26:30.000000 investorzilla-3.4/investorzilla/investor.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-05-31 23:16:21.000000 investorzilla-3.4/investorzilla/marketindex/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     3913 2023-11-20 22:28:04.000000 investorzilla-3.4/investorzilla/marketindex/brasil_banco_central.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1464 2023-11-22 08:44:43.000000 investorzilla-3.4/investorzilla/marketindex/federal_reserve.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     2906 2023-12-16 08:53:09.000000 investorzilla-3.4/investorzilla/marketindex/yahoo_finance.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    11871 2023-12-16 08:31:42.000000 investorzilla-3.4/investorzilla/monetary_time_series.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    16852 2024-03-27 19:52:35.000000 investorzilla-3.4/investorzilla/portfolio.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-05-31 23:16:22.000000 investorzilla-3.4/investorzilla/portfolios/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      515 2023-11-22 08:44:43.000000 investorzilla-3.4/investorzilla/portfolios/app-credentials-for-google-sheets.json
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    12780 2024-03-27 19:39:50.000000 investorzilla-3.4/investorzilla/portfolios/google_sheets.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     8472 2024-03-27 19:41:19.000000 investorzilla-3.4/investorzilla/portfolios/uri.py
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    29762 2024-05-31 23:13:58.000000 investorzilla-3.4/investorzilla/streamlit_ui.py
+drwxr-xr-x   0 aviram    (1000) aviram    (1000)        0 2024-05-31 23:16:20.000000 investorzilla-3.4/investorzilla.egg-info/
+-rw-r--r--   0 aviram    (1000) aviram    (1000)    46319 2024-05-31 23:16:13.000000 investorzilla-3.4/investorzilla.egg-info/PKG-INFO
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      841 2024-05-31 23:16:15.000000 investorzilla-3.4/investorzilla.egg-info/SOURCES.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)        1 2024-05-31 23:16:13.000000 investorzilla-3.4/investorzilla.egg-info/dependency_links.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       62 2024-05-31 23:16:14.000000 investorzilla-3.4/investorzilla.egg-info/entry_points.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)      159 2024-05-31 23:16:14.000000 investorzilla-3.4/investorzilla.egg-info/requires.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       14 2024-05-31 23:16:14.000000 investorzilla-3.4/investorzilla.egg-info/top_level.txt
+-rw-r--r--   0 aviram    (1000) aviram    (1000)     1494 2024-05-31 23:15:42.000000 investorzilla-3.4/pyproject.toml
+-rw-r--r--   0 aviram    (1000) aviram    (1000)       38 2024-05-31 23:16:22.000000 investorzilla-3.4/setup.cfg
```

### Comparing `investorzilla-3.3/LICENSE` & `investorzilla-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/PKG-INFO` & `investorzilla-3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investorzilla
-Version: 3.3
+Version: 3.4
 Summary: Manage your investments like a data scientist
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `investorzilla-3.3/README.md` & `investorzilla-3.4/README.md`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/__init__.py` & `investorzilla-3.4/investorzilla/__init__.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/__main__.py` & `investorzilla-3.4/investorzilla/__main__.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/currency/brasil_banco_central.py` & `investorzilla-3.4/investorzilla/currency/brasil_banco_central.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/currency/cryptocompare.py` & `investorzilla-3.4/investorzilla/currency/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/datacache.py` & `investorzilla-3.4/investorzilla/datacache.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/fund.py` & `investorzilla-3.4/investorzilla/fund.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/investor.py` & `investorzilla-3.4/investorzilla/investor.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/marketindex/brasil_banco_central.py` & `investorzilla-3.4/investorzilla/marketindex/brasil_banco_central.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/marketindex/federal_reserve.py` & `investorzilla-3.4/investorzilla/marketindex/federal_reserve.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/marketindex/yahoo_finance.py` & `investorzilla-3.4/investorzilla/marketindex/yahoo_finance.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/monetary_time_series.py` & `investorzilla-3.4/investorzilla/monetary_time_series.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/portfolio.py` & `investorzilla-3.4/investorzilla/portfolio.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/portfolios/app-credentials-for-google-sheets.json` & `investorzilla-3.4/investorzilla/portfolios/app-credentials-for-google-sheets.json`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/portfolios/google_sheets.py` & `investorzilla-3.4/investorzilla/portfolios/google_sheets.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/portfolios/uri.py` & `investorzilla-3.4/investorzilla/portfolios/uri.py`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/investorzilla/streamlit_ui.py` & `investorzilla-3.4/investorzilla/streamlit_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import logging
 import copy
+import textwrap
 
 # Dependencies available via OS packages:
 # pip3 install pandas pyyaml sqlalchemy pandas_datareader
 
 # Other dependencies:
 # pip3 install streamlit google-api-python-client
 
@@ -395,14 +396,31 @@
                     kpi=investorzilla.KPI.MOVEMENTS,
                     periodPair=streamlit.session_state.interact_periods,
                     type='altair',
                     precomputedReport=self.reportPeriodic
                 ).interactive()
             )
 
+            # Render 4% Rule text
+            streamlit.header('[4% Rule](https://www.investopedia.com/terms/f/four-percent-rule.asp)')
+            rule_4_percent=textwrap.dedent("""\
+                If you retire today, you would be able to withdraw
+                **{withdraw_per_year:0,.2f} {currency}** per year or
+                **{withdraw_per_month:0,.2f} {currency}** per month, based on your
+                total assets and a withdrawal rate of 4%.
+            """)
+            streamlit.markdown(
+                rule_4_percent.format(
+                    withdraw_per_year = 0.04 * self.reportPeriodic.iloc[-1][investorzilla.KPI.BALANCE],
+                    withdraw_per_month = (0.04 * self.reportPeriodic.iloc[-1][investorzilla.KPI.BALANCE])/12,
+                    currency = streamlit.session_state.fund.name.split('@')[1].strip()
+                )
+            )
+
+
         table_styles=[
             dict(selector="td", props="font-size: 0.8em; text-align: right"),
             dict(selector="th", props="font-size: 0.8em; "),
             dict(selector='tr:hover', props='background-color: yellow')
         ]
 
         streamlit.header('Wealth Evolution')
```

### Comparing `investorzilla-3.3/investorzilla.egg-info/PKG-INFO` & `investorzilla-3.4/investorzilla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investorzilla
-Version: 3.3
+Version: 3.4
 Summary: Manage your investments like a data scientist
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `investorzilla-3.3/investorzilla.egg-info/SOURCES.txt` & `investorzilla-3.4/investorzilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `investorzilla-3.3/pyproject.toml` & `investorzilla-3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "investorzilla"
-version = '3.3'
+version = '3.4'
 description = "Manage your investments like a data scientist"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 authors = [
     { name = "Avi Alkalay", email = "avi@unix.sh" },
 ]
```

