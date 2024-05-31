# Comparing `tmp/myeia-0.3.5.tar.gz` & `tmp/myeia-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myeia-0.3.5.tar", last modified: Fri Sep  8 13:39:54 2023, max compression
+gzip compressed data, was "myeia-0.3.6.tar", last modified: Fri May 31 22:00:09 2024, max compression
```

## Comparing `myeia-0.3.5.tar` & `myeia-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:39:54.707308 myeia-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-08 13:39:33.000000 myeia-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2023-09-08 13:39:54.707308 myeia-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2023-09-08 13:39:33.000000 myeia-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:39:54.707308 myeia-0.3.5/myeia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 13:39:33.000000 myeia-0.3.5/myeia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2023-09-08 13:39:33.000000 myeia-0.3.5/myeia/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-08 13:39:33.000000 myeia-0.3.5/myeia/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:39:54.707308 myeia-0.3.5/myeia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2023-09-08 13:39:54.000000 myeia-0.3.5/myeia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-09-08 13:39:54.000000 myeia-0.3.5/myeia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 13:39:54.000000 myeia-0.3.5/myeia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-08 13:39:54.000000 myeia-0.3.5/myeia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-08 13:39:54.000000 myeia-0.3.5/myeia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-08 13:39:33.000000 myeia-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-08 13:39:54.707308 myeia-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-09-08 13:39:33.000000 myeia-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:00:09.889812 myeia-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-31 21:59:53.000000 myeia-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-31 22:00:09.889812 myeia-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-31 21:59:53.000000 myeia-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:00:09.889812 myeia-0.3.6/myeia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:59:53.000000 myeia-0.3.6/myeia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-31 21:59:53.000000 myeia-0.3.6/myeia/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 21:59:53.000000 myeia-0.3.6/myeia/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:00:09.889812 myeia-0.3.6/myeia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-31 22:00:09.000000 myeia-0.3.6/myeia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-31 22:00:09.000000 myeia-0.3.6/myeia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:00:09.000000 myeia-0.3.6/myeia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 22:00:09.000000 myeia-0.3.6/myeia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 22:00:09.000000 myeia-0.3.6/myeia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 21:59:53.000000 myeia-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 22:00:09.889812 myeia-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-31 21:59:53.000000 myeia-0.3.6/setup.py
```

### Comparing `myeia-0.3.5/LICENSE` & `myeia-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myeia-0.3.5/PKG-INFO` & `myeia-0.3.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: myeia
-Version: 0.3.5
+Version: 0.3.6
 Summary: UNKNOWN
 Home-page: https://github.com/philsv/myeia
 Author: philsv
 Author-email: frphsv@gmail.com
 License: MIT
 Description: # myeia
         
-        [![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&r=r&ts=1683906897&type=6e&v=0.3.5&x2=0)](https://badge.fury.io/py/myeia)
+        [![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&r=r&ts=1683906897&type=6e&v=0.3.6&x2=0)](https://badge.fury.io/py/myeia)
         [![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://github.com/philsv/myeia/blob/main/LICENSE)
         [![Weekly Downloads](https://static.pepy.tech/personalized-badge/myeia?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week)](https://pepy.tech/project/myeia)
         [![Monthly Downloads](https://static.pepy.tech/personalized-badge/myeia?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/myeia)
         [![Downloads](https://static.pepy.tech/personalized-badge/myeia?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/myeia)
         
         myeia is a simple Python wrapper for the U.S. Energy Information Administration (EIA) APIv2. It is designed to be simple to use and to provide a consistent interface for accessing EIA data.
         
@@ -40,14 +40,21 @@
         
         ```python
         from myeia.api import API
         
         eia = API()
         ```
         
+        ## Prerequisites
+        
+        ```bash
+        # Create your personal .env file in your projects root directory
+        touch .env
+        ```
+        
         By Default the EIA class will look for your API `EIA_TOKEN`.
         
         If you have registered for an API key you can set it in your `.env` file.
         
         ```ini
         EIA_TOKEN=YOUR_TOKEN_HERE
         ```
@@ -75,15 +82,15 @@
                     Natural Gas Futures Contract 1 (Dollars per Million Btu)
         Date
         2022-09-13                                              8.284
         2022-09-12                                              8.249
         2022-09-09                                              7.996
         2022-09-08                                              7.915
         2022-09-07                                              7.842
-        ...
+        ...                                                       ...
         ```
         
         ## Different Facets
         
         Lets look at another example the *Total OPEC Petroleum Supply* where the facet is available as `seriesId`. By Default it is set as `series` but we can define the facet as `seriesId`.
         
         ```python
@@ -105,14 +112,15 @@
                     Total OPEC Petroleum Supply
         Date
         2023-12-01                    34.517314
         2023-11-01                    34.440397
         2023-10-01                    34.376971
         2023-09-01                    34.416242
         2023-08-01                    34.451823
+        ...                                 ...
         ```
         
         ## Get Multiple Series
         
         You can also get a list of series for a specific route.
         
         You have to make sure they are both in the same frequency and facet type.
@@ -161,15 +169,15 @@
                     Natural Gas Futures Contract 1 (Dollars per Million Btu)
         Date                                                                
         2021-01-29                                              2.564       
         2021-01-28                                              2.664       
         2021-01-27                                              2.760       
         2021-01-26                                              2.656       
         2021-01-25                                              2.602       
-        ...                                                     ...       
+        ...                                                       ...       
         ```
         
         This also works for the `get_series_via_route` method.
         
         ```python
         df = eia.get_series_via_route(
             route="natural-gas/pri/fut",
```

### Comparing `myeia-0.3.5/README.md` & `myeia-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # myeia
 
-[![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&r=r&ts=1683906897&type=6e&v=0.3.5&x2=0)](https://badge.fury.io/py/myeia)
+[![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&r=r&ts=1683906897&type=6e&v=0.3.6&x2=0)](https://badge.fury.io/py/myeia)
 [![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://github.com/philsv/myeia/blob/main/LICENSE)
 [![Weekly Downloads](https://static.pepy.tech/personalized-badge/myeia?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week)](https://pepy.tech/project/myeia)
 [![Monthly Downloads](https://static.pepy.tech/personalized-badge/myeia?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/myeia)
 [![Downloads](https://static.pepy.tech/personalized-badge/myeia?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/myeia)
 
 myeia is a simple Python wrapper for the U.S. Energy Information Administration (EIA) APIv2. It is designed to be simple to use and to provide a consistent interface for accessing EIA data.
 
@@ -32,14 +32,21 @@
 
 ```python
 from myeia.api import API
 
 eia = API()
 ```
 
+## Prerequisites
+
+```bash
+# Create your personal .env file in your projects root directory
+touch .env
+```
+
 By Default the EIA class will look for your API `EIA_TOKEN`.
 
 If you have registered for an API key you can set it in your `.env` file.
 
 ```ini
 EIA_TOKEN=YOUR_TOKEN_HERE
 ```
@@ -67,15 +74,15 @@
             Natural Gas Futures Contract 1 (Dollars per Million Btu)
 Date
 2022-09-13                                              8.284
 2022-09-12                                              8.249
 2022-09-09                                              7.996
 2022-09-08                                              7.915
 2022-09-07                                              7.842
-...
+...                                                       ...
 ```
 
 ## Different Facets
 
 Lets look at another example the *Total OPEC Petroleum Supply* where the facet is available as `seriesId`. By Default it is set as `series` but we can define the facet as `seriesId`.
 
 ```python
@@ -97,14 +104,15 @@
             Total OPEC Petroleum Supply
 Date
 2023-12-01                    34.517314
 2023-11-01                    34.440397
 2023-10-01                    34.376971
 2023-09-01                    34.416242
 2023-08-01                    34.451823
+...                                 ...
 ```
 
 ## Get Multiple Series
 
 You can also get a list of series for a specific route.
 
 You have to make sure they are both in the same frequency and facet type.
@@ -153,15 +161,15 @@
             Natural Gas Futures Contract 1 (Dollars per Million Btu)
 Date                                                                
 2021-01-29                                              2.564       
 2021-01-28                                              2.664       
 2021-01-27                                              2.760       
 2021-01-26                                              2.656       
 2021-01-25                                              2.602       
-...                                                     ...       
+...                                                       ...       
 ```
 
 This also works for the `get_series_via_route` method.
 
 ```python
 df = eia.get_series_via_route(
     route="natural-gas/pri/fut",
```

### Comparing `myeia-0.3.5/myeia/api.py` & `myeia-0.3.6/myeia/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,46 @@
+import logging
 import os
 import warnings
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
+import logging
 from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 import requests
 from dotenv import load_dotenv
+from requests.exceptions import JSONDecodeError
 
 try:
     from pandas.errors import SettingWithCopyWarning
 except ImportError as e:
     raise ImportError("Please upgrade your version of pandas to 1.5.3 or higher.") from e
 
 warnings.simplefilter(action="ignore", category=SettingWithCopyWarning)
 
 load_dotenv()
 
+logging.basicConfig(
+    level=logging.INFO, format="%(asctime)s - %(message)s", datefmt="%d-%b-%y %H:%M:%S"
+)
+
+
 
 def get_json_response(url: str, headers: dict) -> pd.DataFrame:
     """
     Helper function to get JSON response from API.
     """
     response = requests.get(url, headers=headers)
     response.raise_for_status()
-    json_response = response.json()
+    try:
+        json_response = response.json()
+    except JSONDecodeError as e:
+        logging.error(f"Response: {response.text}")
+        raise ValueError(f"Error decoding JSON response ({e}). Data might be incomplete or missing. Chunking your request might help.") from e
     return pd.DataFrame(json_response["response"]["data"])
 
 
 def format_time_series_data(df: pd.DataFrame) -> pd.DataFrame:
     """
     Helper function to format time series data.
     """
@@ -150,16 +162,16 @@
             base_df = get_json_response(url, headers=self.header)
 
             if base_df.empty:
                 raise ValueError(f"Error getting data for series: {series}. Please check your request.")
 
             if facet == "series":
                 df = base_df[["period", "value", "series-description", "series"]]
-            elif facet == "seriesId":
-                df = base_df[["period", "value", "seriesDescription", "seriesId"]]
+            else:
+                df = base_df[["period", "value", "seriesDescription", facet]]
 
             df.reset_index(drop=True, inplace=True)
             df.rename(columns={df.columns[1]: df[df.columns[2]][0]}, inplace=True)
             df = df.iloc[:, :2]  # Keep only the date and value columns
             df.rename(columns={df.columns[0]: "Date"}, inplace=True)
             df = format_time_series_data(df)
             data.append(df)
```

### Comparing `myeia-0.3.5/myeia.egg-info/PKG-INFO` & `myeia-0.3.6/myeia.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: myeia
-Version: 0.3.5
+Version: 0.3.6
 Summary: UNKNOWN
 Home-page: https://github.com/philsv/myeia
 Author: philsv
 Author-email: frphsv@gmail.com
 License: MIT
 Description: # myeia
         
-        [![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&r=r&ts=1683906897&type=6e&v=0.3.5&x2=0)](https://badge.fury.io/py/myeia)
+        [![PyPI version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=py&r=r&ts=1683906897&type=6e&v=0.3.6&x2=0)](https://badge.fury.io/py/myeia)
         [![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://github.com/philsv/myeia/blob/main/LICENSE)
         [![Weekly Downloads](https://static.pepy.tech/personalized-badge/myeia?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week)](https://pepy.tech/project/myeia)
         [![Monthly Downloads](https://static.pepy.tech/personalized-badge/myeia?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/myeia)
         [![Downloads](https://static.pepy.tech/personalized-badge/myeia?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/myeia)
         
         myeia is a simple Python wrapper for the U.S. Energy Information Administration (EIA) APIv2. It is designed to be simple to use and to provide a consistent interface for accessing EIA data.
         
@@ -40,14 +40,21 @@
         
         ```python
         from myeia.api import API
         
         eia = API()
         ```
         
+        ## Prerequisites
+        
+        ```bash
+        # Create your personal .env file in your projects root directory
+        touch .env
+        ```
+        
         By Default the EIA class will look for your API `EIA_TOKEN`.
         
         If you have registered for an API key you can set it in your `.env` file.
         
         ```ini
         EIA_TOKEN=YOUR_TOKEN_HERE
         ```
@@ -75,15 +82,15 @@
                     Natural Gas Futures Contract 1 (Dollars per Million Btu)
         Date
         2022-09-13                                              8.284
         2022-09-12                                              8.249
         2022-09-09                                              7.996
         2022-09-08                                              7.915
         2022-09-07                                              7.842
-        ...
+        ...                                                       ...
         ```
         
         ## Different Facets
         
         Lets look at another example the *Total OPEC Petroleum Supply* where the facet is available as `seriesId`. By Default it is set as `series` but we can define the facet as `seriesId`.
         
         ```python
@@ -105,14 +112,15 @@
                     Total OPEC Petroleum Supply
         Date
         2023-12-01                    34.517314
         2023-11-01                    34.440397
         2023-10-01                    34.376971
         2023-09-01                    34.416242
         2023-08-01                    34.451823
+        ...                                 ...
         ```
         
         ## Get Multiple Series
         
         You can also get a list of series for a specific route.
         
         You have to make sure they are both in the same frequency and facet type.
@@ -161,15 +169,15 @@
                     Natural Gas Futures Contract 1 (Dollars per Million Btu)
         Date                                                                
         2021-01-29                                              2.564       
         2021-01-28                                              2.664       
         2021-01-27                                              2.760       
         2021-01-26                                              2.656       
         2021-01-25                                              2.602       
-        ...                                                     ...       
+        ...                                                       ...       
         ```
         
         This also works for the `get_series_via_route` method.
         
         ```python
         df = eia.get_series_via_route(
             route="natural-gas/pri/fut",
```

### Comparing `myeia-0.3.5/setup.py` & `myeia-0.3.6/setup.py`

 * *Files identical despite different names*

