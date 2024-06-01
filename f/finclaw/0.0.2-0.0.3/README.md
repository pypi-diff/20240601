# Comparing `tmp/finclaw-0.0.2.tar.gz` & `tmp/finclaw-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finclaw-0.0.2.tar", max compression
+gzip compressed data, was "finclaw-0.0.3.tar", max compression
```

## Comparing `finclaw-0.0.2.tar` & `finclaw-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,44 @@
--rw-r--r--   0        0        0      397 2023-09-06 01:47:11.345740 finclaw-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/__init__.py
--rw-r--r--   0        0        0     5105 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/__main__.py
--rw-r--r--   0        0        0     1041 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/config.py
--rw-r--r--   0        0        0        0 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/data_store/__init__.py
--rw-r--r--   0        0        0     4656 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/data_store/data_portal.py
--rw-r--r--   0        0        0     8411 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/data_store/schema.py
--rw-r--r--   0        0        0    10255 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/data_store/store.py
--rw-r--r--   0        0        0      183 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/data_store/validators.py
--rw-r--r--   0        0        0        0 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/utils/__init__.py
--rw-r--r--   0        0        0     2361 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/utils/cli_utils.py
--rw-r--r--   0        0        0      101 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/utils/list_utils.py
--rw-r--r--   0        0        0       31 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/__init__.py
--rw-r--r--   0        0        0       85 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/exceptions.py
--rw-r--r--   0        0        0        0 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/__init__.py
--rw-r--r--   0        0        0     9354 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/finnhub_client.py
--rw-r--r--   0        0        0    14571 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/finnhub_to_table.py
--rw-r--r--   0        0        0    10044 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/models.py
--rw-r--r--   0        0        0     1231 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/pull_dividends.py
--rw-r--r--   0        0        0     3224 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/pull_financials.py
--rw-r--r--   0        0        0     1023 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/pull_insider_information.py
--rw-r--r--   0        0        0     4189 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/pull_ohcl.py
--rw-r--r--   0        0        0     2401 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/pull_ownership.py
--rw-r--r--   0        0        0      969 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/pull_splits.py
--rw-r--r--   0        0        0      853 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/finnhub/symbols.py
--rw-r--r--   0        0        0      222 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/fmp/__init__.py
--rw-r--r--   0        0        0     3356 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/fmp/fmp.py
--rw-r--r--   0        0        0     1341 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/fmp/fmp_client.py
--rw-r--r--   0        0        0        0 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/kraken/__init__.py
--rw-r--r--   0        0        0     5296 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/kraken/exchange.py
--rw-r--r--   0        0        0        0 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/polygone/__init__.py
--rw-r--r--   0        0        0      281 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/twelvedata/__init__.py
--rw-r--r--   0        0        0     3862 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/twelvedata/twelve.py
--rw-r--r--   0        0        0     2119 2023-09-06 01:47:11.345740 finclaw-0.0.2/finclaw/vendor/twelvedata/twelve_client.py
--rw-r--r--   0        0        0      607 2023-09-06 01:47:11.349740 finclaw-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 finclaw-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1657 2024-06-01 16:47:33.703543 finclaw-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-06-01 16:47:33.703543 finclaw-0.0.3/finclaw/__init__.py
+-rw-r--r--   0        0        0     7348 2024-06-01 16:47:33.703543 finclaw-0.0.3/finclaw/__main__.py
+-rw-r--r--   0        0        0     1336 2024-06-01 16:47:33.703543 finclaw-0.0.3/finclaw/config.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:47:33.703543 finclaw-0.0.3/finclaw/data_store/__init__.py
+-rw-r--r--   0        0        0     5202 2024-06-01 16:47:33.703543 finclaw-0.0.3/finclaw/data_store/data_portal.py
+-rw-r--r--   0        0        0    14164 2024-06-01 16:47:33.703543 finclaw-0.0.3/finclaw/data_store/schema.py
+-rw-r--r--   0        0        0     1572 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/data_store/storage_clients/LocalStoreClient.py
+-rw-r--r--   0        0        0     2294 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/data_store/storage_clients/S3Client.py
+-rw-r--r--   0        0        0      749 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/data_store/storage_clients/StoreClient.py
+-rw-r--r--   0        0        0       69 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/data_store/storage_clients/__init__.py
+-rw-r--r--   0        0        0    10841 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/data_store/store.py
+-rw-r--r--   0        0        0     8341 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/data_store/storeV2.py
+-rw-r--r--   0        0        0      183 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/data_store/validators.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/utils/__init__.py
+-rw-r--r--   0        0        0     2361 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/utils/cli_utils.py
+-rw-r--r--   0        0        0      101 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/utils/list_utils.py
+-rw-r--r--   0        0        0      719 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/utils/progress_bar.py
+-rw-r--r--   0        0        0       31 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/__init__.py
+-rw-r--r--   0        0        0     6012 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/constants/mic.py
+-rw-r--r--   0        0        0       85 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/__init__.py
+-rw-r--r--   0        0        0     9354 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/finnhub_client.py
+-rw-r--r--   0        0        0    14571 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/finnhub_to_table.py
+-rw-r--r--   0        0        0    10044 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/models.py
+-rw-r--r--   0        0        0     1327 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/pull_dividends.py
+-rw-r--r--   0        0        0     3295 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/pull_financials.py
+-rw-r--r--   0        0        0     1069 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/pull_insider_information.py
+-rw-r--r--   0        0        0     4287 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/pull_ohcl.py
+-rw-r--r--   0        0        0     2387 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/pull_ownership.py
+-rw-r--r--   0        0        0     1043 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/pull_splits.py
+-rw-r--r--   0        0        0      853 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/finnhub/symbols.py
+-rw-r--r--   0        0        0      222 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/fmp/__init__.py
+-rw-r--r--   0        0        0     5599 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/fmp/fmp.py
+-rw-r--r--   0        0        0     2354 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/fmp/fmp_client.py
+-rw-r--r--   0        0        0     6873 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/fmp/models.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/kraken/__init__.py
+-rw-r--r--   0        0        0     5296 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/kraken/exchange.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/polygone/__init__.py
+-rw-r--r--   0        0        0      281 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/twelvedata/__init__.py
+-rw-r--r--   0        0        0     3884 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/twelvedata/twelve.py
+-rw-r--r--   0        0        0     2902 2024-06-01 16:47:33.707543 finclaw-0.0.3/finclaw/vendor/twelvedata/twelve_client.py
+-rw-r--r--   0        0        0      632 2024-06-01 16:47:33.711543 finclaw-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2462 1970-01-01 00:00:00.000000 finclaw-0.0.3/PKG-INFO
```

### Comparing `finclaw-0.0.2/finclaw/config.py` & `finclaw-0.0.3/finclaw/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import logging
 import os
 
 from pydantic import BaseSettings
 from dotenv import load_dotenv
 
+logger = logging.getLogger()
+logging.basicConfig(level=logging.DEBUG)
+
 
 def is_running_in_jupyter():
     try:
+        # get_ipython is defined when this is called from inside Jupyter
         shell = get_ipython().__class__.__name__
-        if shell == 'ZMQInteractiveShell':
+        if shell == "ZMQInteractiveShell":
             return True  # Jupyter Notebook
-        elif shell == 'TerminalInteractiveShell':
+        elif shell == "TerminalInteractiveShell":
             return False  # Terminal running IPython
         else:
             return False  # Other type, assume not a Jupyter Notebook
     except NameError:
         return False  # Probably standard Python interpreter
 
 
@@ -28,18 +32,21 @@
 
     # TwelveData creds
     TWELVEDATA_API_KEY: str = ""
 
     # Kraken creds
     KRAKEN_API_KEY: str
     KRAKEN_API_SECRET: str
+    USE_TQDM: bool = False
+
+    # It can be set when using AWS
+    S3_BUCKET_NAME: str = ""
 
 
 if is_running_in_jupyter():
+    logger.info("Running inside Jupyter")
+    logger.info("Note that .env file should be in the same directory as this notebook")
     load_dotenv()
     settings = Settings()
 else:
     load_dotenv()
     settings = Settings()
-
-logger = logging.getLogger()
-logging.basicConfig(level=logging.DEBUG)
```

### Comparing `finclaw-0.0.2/finclaw/data_store/data_portal.py` & `finclaw-0.0.3/finclaw/data_store/data_portal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 from collections import namedtuple
 from datetime import timedelta
 from typing import List, Optional, Union, Dict
 
 import pandas as pd
 import pyarrow as pa
-from tqdm import tqdm
+
+from finclaw.data_store.storeV2 import PriceStoreV2
+from finclaw.utils.progress_bar import progress_bar
 
 from finclaw.config import settings
 from finclaw.data_store.store import PriceStore
 from finclaw.data_store.validators import validate_vendor
 
 DataChunk = namedtuple("DataChunk", ["current_date", "price_ohcl_daily"])
 
@@ -20,43 +22,45 @@
 
     def history(self, days: int):
         """
         Get dataframe for the last n days
         :param days:
         :return:
         """
-        return self.data[(self.data.index.max() - pd.Timedelta(days=days)) <= self.data.index]
+        return self.data[
+            (self.data.index.max() - pd.Timedelta(days=days)) <= self.data.index
+        ]
 
 
 class DataPortal:
     """
     This is used by the simulation runner to answer questions about the data,
     like getting the prices of assets on a given day or to service history
     calls.
     """
 
     def __init__(
-            self,
-            price_store: PriceStore,
-            start: pd.Timestamp,
-            end: pd.Timestamp,
-            step
+        self, price_store: PriceStore, start: pd.Timestamp, end: pd.Timestamp, step
     ):
         self.price_data: Optional[pd.DataFrame] = None
         self._price_store = price_store
         self.current_date: pd.Timestamp = start
         self.start = start
         self.end = end
         self.step = step
 
-    def load_price_data(self, *, start: pd.Timestamp, end: pd.Timestamp, frequency: str, vendor: str) -> pa.Table:
-        return self._price_store.load_prices(start=start, end=end, frequency=frequency, vendor=vendor)
+    def load_price_data(
+        self, *, start: pd.Timestamp, end: pd.Timestamp, frequency: str, vendor: str
+    ) -> pa.Table:
+        return self._price_store.load_prices(start=start, end=end, frequency=frequency)
 
     def init(self):
-        price = self.load_price_data(start=self.start, end=self.end, frequency="D", vendor="finnhub")
+        price = self.load_price_data(
+            start=self.start, end=self.end, frequency="D", vendor="finnhub"
+        )
         df = price.to_pandas()
         df.index = df.timestamp
         self.price_data = df
 
     def get_simulation_data_frames(self):
         end = self.end
         while self.current_date < end:
@@ -66,84 +70,103 @@
     def get_snapshot(self, *, current_date: pd.Timestamp):
         if self.price_data is None:
             raise ValueError("You need to call initialize")
 
         # Note, we want a copy
         price_df = self.price_data[self.price_data.index <= current_date]
 
-        return DataChunk(current_date=self.current_date,
-                         price_ohcl_daily=Snapshot(price_df))
+        return DataChunk(
+            current_date=self.current_date, price_ohcl_daily=Snapshot(price_df)
+        )
 
 
-def list_stores(path=settings.TRADE_ENGINE_DATA, is_dict=False) -> Union[List[PriceStore], Dict[str, PriceStore]]:
+def list_stores(
+    path=settings.TRADE_ENGINE_DATA, is_dict=False
+) -> Union[List[PriceStore], Dict[str, PriceStore]]:
     if not is_dict:
         return [PriceStore(path + "/" + ps_path) for ps_path in os.listdir(path)]
     result = {}
     for ps_path in os.listdir(path):
         ps = PriceStore(path + "/" + ps_path)
         result[f"{repr(ps)}"] = ps
     return result
 
 
-def get_ohclv(store: Union[PriceStore, List[PriceStore]], *, frequency: str, vendor: str) -> pa.Table:
+def list_stores_s3(
+    storage_client, path=settings.TRADE_ENGINE_DATA, is_dict=False
+) -> Union[List[PriceStoreV2], Dict[str, PriceStoreV2]]:
+    if not is_dict:
+        return [
+            PriceStoreV2(path + "/" + ps_path, storage_client)
+            for ps_path in storage_client.listdir(path)
+        ]
+    result = {}
+    for ps_path in storage_client.listdir(path):
+        ps = PriceStoreV2(path + "/" + ps_path, storage_client)
+        result[f"{repr(ps)}"] = ps
+    return result
+
+
+def get_ohclv(
+    store: Union[PriceStore, List[PriceStore]], *, frequency: str, vendor: str
+) -> pa.Table:
     """
     Args:
         vendor:
         store:
         frequency:
     """
     validate_vendor(vendor)
 
     if isinstance(store, PriceStore):
-        price = store.load_prices(frequency=frequency, vendor=vendor)
+        price = store.load_prices(frequency=frequency)
 
     elif isinstance(store, list):
         price = pa.concat_tables(
             [
                 get_ohclv(
                     s,
                     frequency=frequency,
                     vendor=vendor,
                 )
-                for s in tqdm(store)
+                for s in progress_bar(store)
             ]
         )
     else:
         raise ValueError("store needs to be a PriceStore or a List[PriceStore]")
 
     return price
 
 
-def get_financials(store: Union[PriceStore, List[PriceStore]], *, vendor: str, statement_type: str) -> pa.Table:
+def get_financials(
+    store: Union[PriceStore, List[PriceStore]], *, vendor: str, statement_type: str
+) -> pa.Table:
     validate_vendor(vendor)
     if isinstance(store, PriceStore):
         financials = store.load_financials(vendor=vendor, statement_type=statement_type)
     elif isinstance(store, list):
         financials = pa.concat_tables(
             [
                 get_financials(
                     s,
                     vendor=vendor,
                     statement_type=statement_type,
                 )
-                for s in tqdm(store)
+                for s in progress_bar(store)
             ]
         )
     else:
         raise ValueError("store needs to be a PriceStore or a List[PriceStore]")
     return financials
 
 
 def get_insiders(store: Union[PriceStore, List[PriceStore]], *, vendor) -> pa.Table:
     validate_vendor(vendor)
     if isinstance(store, PriceStore):
         insiders = store.load_insiders(vendor=vendor)
     elif isinstance(store, list):
         insiders = pa.concat_tables(
-            [
-                get_insiders(s, vendor=vendor)
-                for s in tqdm(store)
-            ]
+            [get_insiders(s, vendor=vendor) for s in progress_bar(store)]
         )
     else:
         raise ValueError("store needs to be a PriceStore or a List[PriceStore]")
     return insiders
```

### Comparing `finclaw-0.0.2/finclaw/data_store/schema.py` & `finclaw-0.0.3/finclaw/data_store/schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -234,7 +234,148 @@
 OWNER = pa.schema([
     ('shares_traded', pa.float64()),
     ('filing_date', pa.timestamp('s', tz='UTC')),
     ('name', pa.string()),
     ('shares_owned', pa.float64()),
     ('symbol', pa.string())
 ])
+
+BALANCE_SHEET_V2 = pa.schema([
+    ('date', pa.timestamp('ns')),
+    ('symbol', pa.string()),
+    ('reported_currency', pa.string()),
+    ('cik', pa.string()),
+    ('filling_date', pa.timestamp('ns')),
+    ('accepted_date', pa.timestamp('ns')),
+    ('calendar_year', pa.timestamp('ns')),
+    ('period', pa.string()),
+    ('cash_and_cash_equivalents', pa.float64()),
+    ('short_term_investments', pa.float64()),
+    ('cash_and_short_term_investments', pa.float64()),
+    ('net_receivables', pa.float64()),
+    ('inventory', pa.float64()),
+    ('other_current_assets', pa.float64()),
+    ('total_current_assets', pa.float64()),
+    ('property_plant_equipment_net', pa.float64()),
+    ('goodwill', pa.float64()),
+    ('intangible_assets', pa.float64()),
+    ('goodwill_and_intangible_assets', pa.float64()),
+    ('long_term_investments', pa.float64()),
+    ('tax_assets', pa.float64()),
+    ('other_non_current_assets', pa.float64()),
+    ('total_non_current_assets', pa.float64()),
+    ('other_assets', pa.float64()),
+    ('total_assets', pa.float64()),
+    ('account_payables', pa.float64()),
+    ('short_term_debt', pa.float64()),
+    ('tax_payables', pa.float64()),
+    ('deferred_revenue', pa.float64()),
+    ('other_current_liabilities', pa.float64()),
+    ('total_current_liabilities', pa.float64()),
+    ('long_term_debt', pa.float64()),
+    ('deferred_revenue_non_current', pa.float64()),
+    ('deferred_tax_liabilities_non_current', pa.float64()),
+    ('other_non_current_liabilities', pa.float64()),
+    ('total_non_current_liabilities', pa.float64()),
+    ('other_liabilities', pa.float64()),
+    ('capital_lease_obligations', pa.float64()),
+    ('total_liabilities', pa.float64()),
+    ('preferred_stock', pa.float64()),
+    ('common_stock', pa.float64()),
+    ('retained_earnings', pa.float64()),
+    ('accumulated_other_comprehensive_income_loss', pa.float64()),
+    ('othertotal_stockholders_equity', pa.float64()),
+    ('total_stockholders_equity', pa.float64()),
+    ('total_equity', pa.float64()),
+    ('total_liabilities_and_stockholders_equity', pa.float64()),
+    ('minority_interest', pa.float64()),
+    ('total_liabilities_and_total_equity', pa.float64()),
+    ('total_investments', pa.float64()),
+    ('total_debt', pa.float64()),
+    ('net_debt', pa.float64()),
+    ('link', pa.string()),
+    ('final_link', pa.string())
+])
+
+INCOME_STATEMENT_V2 = pa.schema([
+    ('date', pa.timestamp('ns')),
+    ('symbol', pa.string()),
+    ('reported_currency', pa.string()),
+    ('cik', pa.string()),
+    ('filling_date', pa.timestamp('ns')),
+    ('accepted_date', pa.timestamp('ns')),
+    ('calendar_year', pa.timestamp('ns')),
+    ('period', pa.string()),
+    ('revenue', pa.float64()),
+    ('cost_of_revenue', pa.float64()),
+    ('gross_profit', pa.float64()),
+    ('gross_profit_ratio', pa.float64()),
+    ('research_and_development_expenses', pa.float64()),
+    ('general_and_administrative_expenses', pa.float64()),
+    ('selling_and_marketing_expenses', pa.float64()),
+    ('selling_general_and_administrative_expenses', pa.float64()),
+    ('other_expenses', pa.float64()),
+    ('operating_expenses', pa.float64()),
+    ('cost_and_expenses', pa.float64()),
+    ('interest_income', pa.float64()),
+    ('interest_expense', pa.float64()),
+    ('depreciation_and_amortization', pa.float64()),
+    ('ebitda', pa.float64()),
+    ('ebitda_ratio', pa.float64()),
+    ('operating_income', pa.float64()),
+    ('operating_income_ratio', pa.float64()),
+    ('total_other_income_expenses_net', pa.float64()),
+    ('income_before_tax', pa.float64()),
+    ('income_before_tax_ratio', pa.float64()),
+    ('income_tax_expense', pa.float64()),
+    ('net_income', pa.float64()),
+    ('net_income_ratio', pa.float64()),
+    ('eps', pa.float64()),
+    ('eps_diluted', pa.float64()),
+    ('weighted_average_shs_out', pa.float64()),
+    ('weighted_average_shs_out_dil', pa.float64()),
+    ('link', pa.string()),
+    ('final_link', pa.string())
+])
+
+CASHFLOW_STATEMENT_V2 = pa.schema([
+    ('date', pa.timestamp('ns')),
+    ('symbol', pa.string()),
+    ('reported_currency', pa.string()),
+    ('cik', pa.string()),
+    ('filling_date', pa.timestamp('ns')),
+    ('accepted_date', pa.timestamp('ns')),
+    ('calendar_year', pa.timestamp('ns')),
+    ('period', pa.string()),
+    ('net_income', pa.float64()),
+    ('depreciation_and_amortization', pa.float64()),
+    ('deferred_income_tax', pa.float64()),
+    ('stock_based_compensation', pa.float64()),
+    ('change_in_working_capital', pa.float64()),
+    ('accounts_receivables', pa.float64()),
+    ('inventory', pa.float64()),
+    ('accounts_payables', pa.float64()),
+    ('other_working_capital', pa.float64()),
+    ('other_non_cash_items', pa.float64()),
+    ('net_cash_provided_by_operating_activities', pa.float64()),
+    ('investments_in_property_plant_and_equipment', pa.float64()),
+    ('acquisitions_net', pa.float64()),
+    ('purchases_of_investments', pa.float64()),
+    ('sales_maturities_of_investments', pa.float64()),
+    ('other_investing_activities', pa.float64()),
+    ('net_cash_used_for_investing_activities', pa.float64()),
+    ('debt_repayment', pa.float64()),
+    ('common_stock_issued', pa.float64()),
+    ('common_stock_repurchased', pa.float64()),
+    ('dividends_paid', pa.float64()),
+    ('other_financing_activities', pa.float64()),
+    ('net_cash_used_provided_by_financing_activities', pa.float64()),
+    ('effect_of_forex_changes_on_cash', pa.float64()),
+    ('net_change_in_cash', pa.float64()),
+    ('cash_at_end_of_period', pa.float64()),
+    ('cash_at_beginning_of_period', pa.float64()),
+    ('operating_cash_flow', pa.float64()),
+    ('capital_expenditure', pa.float64()),
+    ('free_cash_flow', pa.float64()),
+    ('link', pa.string()),
+    ('final_link', pa.string())
+])
```

### Comparing `finclaw-0.0.2/finclaw/data_store/store.py` & `finclaw-0.0.3/finclaw/data_store/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,81 +2,95 @@
 from typing import List, Optional
 
 import pandas as pd
 import pyarrow as pa
 from pyarrow import parquet as pq
 from pathlib import Path
 from google.cloud import storage
+import boto3
 import os
-
+from pyarrow import fs
 from finclaw.data_store.schema import OHCL
 
 """
-These are the stores that are responsible for storing normalized data
+These are the storage_clients that are responsible for storing normalized data
 """
 
 
 class VendorStore:
     def __init__(self, vendor_path):
         self._vendor_path = vendor_path
         self._company_description = "company_descriptions"
 
     def list_company_descriptions(self) -> List[str]:
         return list(os.listdir(self._vendor_path / self._company_description))
 
     def get_company_description_table(self) -> pd.DataFrame:
         for f in self.list_company_descriptions():
-            return pq.read_table(self._vendor_path / self._company_description / f).to_pandas()
+            return pq.read_table(
+                self._vendor_path / self._company_description / f
+            ).to_pandas()
 
     def list_available_resources(self):
         return list(os.listdir(self._vendor_path))
 
     def get_symbol_table(self):
         pass
 
 
 class PriceStore:
     def __init__(self, path_to_price_store: str):
         self._price_path: Path = Path(path_to_price_store)
-        date_of_store = path_to_price_store.split("/")[-1]
+
+    def list_datasets(self):
+        return os.listdir(self._price_path)
 
     # Loading logic
-    def load_prices(self, *, start: Optional[pd.Timestamp] = None, end: Optional[pd.Timestamp] = None, frequency: str,
-                    vendor: str) -> pa.Table:
+    def load_prices(
+        self,
+        *,
+        start: Optional[pd.Timestamp] = None,
+        end: Optional[pd.Timestamp] = None,
+        frequency: str,
+    ) -> pa.Table:
         # sourcery skip: inline-immediately-returned-variable
         """
             Load prices from storage from start and end if exist
         :return:
         """
         if start is not None and end is not None:
             assert start < end
         self.path_exists()
 
         # Note: we can update this later to add filtering
-        price_store = self.get_ohclv_price_store_path(frequency=frequency, vendor=vendor)
+        price_store = self.get_ohclv_price_store_path(frequency=frequency)
 
         if start and end:
             price_dataset_name = PriceStore.get_dataset_name(start=start, end=end)
             return self.load_table(price_dataset_name, price_store, schema=OHCL)
         else:
             tables = []
             for table_name in os.listdir(price_store):
-                table_for_one_freq = self.load_table(table_name, price_store, schema=OHCL)
+                table_for_one_freq = self.load_table(
+                    table_name, price_store, schema=OHCL
+                )
                 tables.append(table_for_one_freq)
             return pa.concat_tables(tables)
 
     def load_table(self, price_dataset, price_store, *, schema: pa.Schema) -> pa.Table:
         price_path = price_store / price_dataset
         if not price_path.exists():
             raise ValueError(f"{price_path} does not exist")
         dataset = pq.ParquetDataset(price_path, use_legacy_dataset=False, schema=schema)
         table: pa.Table = dataset.read()
         return table
 
-    def load_symbols(self, *, start: pd.Timestamp, end: pd.Timestamp, vendor: str) -> pa.Table:
+    def load_symbols(
+        self, *, start: pd.Timestamp, end: pd.Timestamp, vendor: str
+    ) -> pa.Table:
         assert start < end
         self.path_exists()
 
         # Note: we can update this later to add filtering
         symbol_store_path = self.get_symbol_store_path(vendor=vendor)
         symbol_dataset = PriceStore.get_dataset_name(start=start, end=end)
 
@@ -84,18 +98,20 @@
 
         if not symbol_path.exists():
             raise ValueError(f"{symbol_path} does not exist")
 
         dataset = pq.ParquetDataset(symbol_path, use_legacy_dataset=False)
         return dataset.read()
 
-    def load_financials(self, vendor: str, statement_type: str):
+    def load_financials(self, statement_type: str):
         self.path_exists()
 
-        financial_store_path = self.get_financial_statement_store_path(vendor=vendor, statement_type=statement_type)
+        financial_store_path = self.get_financial_statement_store_path(
+            statement_type=statement_type
+        )
         dataset = pq.ParquetDataset(financial_store_path, use_legacy_dataset=False)
         return dataset.read()
 
     def load_insiders(self, vendor):
         self.path_exists()
 
         insider_store_path = self.get_insider_store_path(vendor=vendor)
@@ -103,86 +119,122 @@
         return dataset.read()
 
     def path_exists(self):
         if not self._price_path.exists():
             raise ValueError(f"{self._price_path} does not exist")
 
     ## Store logic
-    def store(self, *, symbol_table: pa.Table, price_table: pa.Table,
-              start: pd.Timestamp,
-              end: pd.Timestamp,
-              frequency: str, vendor: str,
-              company_table: Optional[pa.Table] = None):
+    def store(
+        self,
+        *,
+        symbol_table: pa.Table,
+        price_table: pa.Table,
+        start: pd.Timestamp,
+        end: pd.Timestamp,
+        frequency: str,
+        vendor: str,
+        company_table: Optional[pa.Table] = None,
+    ):
         # Need to store symbols into a table as well
-        self.store_prices(end=end, frequency=frequency, price_table=price_table, start=start, vendor=vendor)
-        self.store_symbols(symbol_table=symbol_table, start=start, end=end, vendor=vendor)
+        self.store_prices(
+            end=end,
+            frequency=frequency,
+            price_table=price_table,
+            start=start,
+            vendor=vendor,
+        )
+        self.store_symbols(
+            symbol_table=symbol_table, start=start, end=end, vendor=vendor
+        )
         if company_table:
-            self.store_company_descriptions(company_table=company_table, start=start, end=end, vendor=vendor)
+            self.store_company_descriptions(
+                company_table=company_table, start=start, end=end, vendor=vendor
+            )
 
     def store_prices(self, *, end, frequency, price_table, start, vendor):
-        price_store_ds = self.get_ohclv_price_store_path(frequency, vendor)
+        price_store_ds = self.get_ohclv_price_store_path(frequency)
         self._save_table(price_store_ds, price_table, start, end)
 
-    def store_symbols(self, *, symbol_table, start: pd.Timestamp, end: pd.Timestamp, vendor):
+    def store_symbols(
+        self, *, symbol_table, start: pd.Timestamp, end: pd.Timestamp, vendor
+    ):
+        processing_date = pd.Timestamp.utcnow()
+        n_rows = symbol_table.shape[0]
+        symbol_table.add_column(
+            0, "meta_storage_date", [[processing_date for i in range(n_rows)]]
+        )
+
         symbol_store_ds = self.get_symbol_store_path(vendor=vendor)
         self._save_table(symbol_store_ds, symbol_table, start, end)
 
     def store_company_descriptions(self, *, company_table, start, end, vendor: str):
         company_descriptions = self.get_company_descriptions(vendor=vendor)
         self._save_table(company_descriptions, company_table, start, end)
 
-    def store_ownership(self, *, institutional_ownership_table: pa.Table,
-                        fund_ownership_table: pa.Table, all_owners_table: pa.Table,
-                        start, end,
-                        vendor: str):
+    def store_ownership(
+        self,
+        *,
+        institutional_ownership_table: pa.Table,
+        fund_ownership_table: pa.Table,
+        all_owners_table: pa.Table,
+        start,
+        end,
+        vendor: str,
+    ):
         fund_ownership_path = self.get_ownership_store_path("fund", vendor)
         self._save_table(fund_ownership_path, fund_ownership_table, start, end)
 
-        institutional_ownership_path = self.get_ownership_store_path("institutional", vendor)
-        self._save_table(institutional_ownership_path, institutional_ownership_table, start, end)
+        institutional_ownership_path = self.get_ownership_store_path(
+            "institutional", vendor
+        )
+        self._save_table(
+            institutional_ownership_path, institutional_ownership_table, start, end
+        )
 
         all_owners_path = self.get_ownership_store_path("all_owners", vendor)
         self._save_table(all_owners_path, all_owners_table, start, end)
 
     def store_insider_information(self, *, insider_table, start, end, vendor):
         insider_store_path = self.get_insider_store_path(vendor)
         self._save_table(insider_store_path, insider_table, start, end)
 
     def store_dividends(self, *, dividend_table, start, end, vendor):
         dividend_store_path = self.get_dividend_store_path(vendor)
         self._save_table(dividend_store_path, dividend_table, start, end)
 
     def store_financials(self, statement, financials_table, start, end, vendor):
-        statement_store_path = self.get_financial_statement_store_path(vendor, statement)
+        statement_store_path = self.get_financial_statement_store_path(
+            vendor, statement
+        )
         self._save_table(statement_store_path, financials_table, start, end)
 
     def store_splits(self, split_table, start, end, vendor):
         split_store_path = self.get_split_store_path(vendor)
         self._save_table(split_store_path, split_table, start, end)
 
     def get_symbol_store_path(self, *, vendor: str):
         return self._price_path / vendor / "symbols"
 
     def get_company_descriptions(self, *, vendor: str):
         return self._price_path / vendor / "company_descriptions"
 
-    def get_ohclv_price_store_path(self, frequency, vendor):
-        return self._price_path / vendor / "ohclv" / f"frequency_{frequency}"
+    def get_ohclv_price_store_path(self, frequency):
+        return self._price_path / "ohclv" / f"frequency_{frequency}"
 
     def get_ownership_store_path(self, ownership_type, vendor):
         return self._price_path / vendor / "ownership" / ownership_type
 
     def get_insider_store_path(self, vendor):
         return self._price_path / vendor / "insider"
 
     def get_dividend_store_path(self, vendor):
         return self._price_path / vendor / "dividends"
 
-    def get_financial_statement_store_path(self, vendor, statement_type):
-        return self._price_path / vendor / statement_type
+    def get_financial_statement_store_path(self, statement_type):
+        return self._price_path / statement_type
 
     def get_split_store_path(self, vendor):
         return self._price_path / vendor / "splits"
 
     @staticmethod
     def _save_table(path_to_ds: Path, table, start: pd.Timestamp, end: pd.Timestamp):
         path_to_ds.mkdir(parents=True, exist_ok=True)
@@ -208,42 +260,51 @@
     """
     Google Storage Price Store
     """
 
     def __init__(self, bucket_name: str, path_to_price_store: str):
         super().__init__(path_to_price_store)
         if path_to_price_store.startswith("/"):
-            raise ValueError(f"{path_to_price_store} cannot start with / for Google Storage")
+            raise ValueError(
+                f"{path_to_price_store} cannot start with / for Google Storage"
+            )
         self.client = storage.Client()
         self.bucket = self.client.get_bucket(bucket_name)
 
     @staticmethod
     def _save_table(path_to_ds: str, table, start: pd.Timestamp, end: pd.Timestamp):
         raise NotImplementedError()
 
     def path_exists(self):
         blobs = self.bucket.list_blobs(prefix=str(self._price_path), max_results=1)
         for _ in blobs:
             return True
 
         return False
 
-    def load_prices(self, *, start: Optional[pd.Timestamp] = None, end: Optional[pd.Timestamp] = None, frequency: str,
-                    vendor: str) -> pa.Table:
+    def load_prices(
+        self,
+        *,
+        start: Optional[pd.Timestamp] = None,
+        end: Optional[pd.Timestamp] = None,
+        frequency: str,
+    ) -> pa.Table:
         # sourcery skip: inline-immediately-returned-variable
         """
             Load prices from storage from start and end if exist
         :return:
         """
         if start is not None and end is not None:
             assert start < end
         if not self.path_exists():
             raise ValueError(f"{self._price_path} does not exist")
 
         # Note: we can update this later to add filtering
-        price_store = self.get_ohclv_price_store_path(frequency=frequency, vendor=vendor)
+        price_store = self.get_ohclv_price_store_path(frequency=frequency)
 
         if start and end:
             price_dataset_name = PriceStore.get_dataset_name(start=start, end=end)
             return self.load_table(price_dataset_name, price_store, OHCL)
         else:
-            return pq.read_table(f"gs://{self.bucket.name}/{self._price_path}", schema=OHCL)
+            return pq.read_table(
+                f"gs://{self.bucket.name}/{self._price_path}", schema=OHCL
+            )
```

### Comparing `finclaw-0.0.2/finclaw/utils/cli_utils.py` & `finclaw-0.0.3/finclaw/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/finnhub_client.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/finnhub_client.py`

 * *Files identical despite different names*

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/finnhub_to_table.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/finnhub_to_table.py`

 * *Files identical despite different names*

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/models.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/models.py`

 * *Files identical despite different names*

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/pull_dividends.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/pull_dividends.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import asyncio
 from typing import List
 
 import aiohttp
 import pandas as pd
 import pyarrow as pa
 from pandas import Timestamp
-from tqdm import tqdm
+from finclaw.utils.progress_bar import progress_bar
 
 from finclaw.config import logger
 from finclaw.vendor.finnhub import models
 from finclaw.vendor.finnhub.finnhub_client import get_dividend
 
 
-async def get_dividends(symbols: List[str], start: pd.Timestamp, end: pd.Timestamp) -> pa.Table:
+async def get_dividends(
+    symbols: List[str], start: pd.Timestamp, end: pd.Timestamp
+) -> pa.Table:
     start = start.strftime("%Y-%m-%d")
     end = end.strftime("%Y-%m-%d")
 
     result = []
-    for symbol in tqdm(symbols, desc="Pulling dividend information"):
+    for symbol in progress_bar(symbols, desc="Pulling dividend information"):
         try:
             async with aiohttp.ClientSession() as session:
-                symbol_dividend_records = await get_dividend(session, symbol=symbol, from_=start, to=end)
+                symbol_dividend_records = await get_dividend(
+                    session, symbol=symbol, from_=start, to=end
+                )
                 if table := models.to_dividend_table(symbol_dividend_records):
                     result.append(table)
         except Exception as e:
             logger.info(f"Error pulling dividend data for {symbol} {e}")
 
     return pa.concat_tables(result)
 
 
 def pull_dividend_data(*, store, symbols, start: Timestamp, end: Timestamp):
     dividend_table = asyncio.run(get_dividends(symbols, start, end))
-    store.store_dividends(dividend_table=dividend_table, start=start, end=end, vendor="finnhub")
+    store.store_dividends(
+        dividend_table=dividend_table, start=start, end=end, vendor="finnhub"
+    )
```

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/pull_financials.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/pull_financials.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,68 +7,90 @@
 from pandas import Timestamp
 
 from finclaw.config import settings, logger
 from finclaw.data_store.store import PriceStore
 from finclaw.vendor.finnhub.finnhub_client import get_financials_for
 from finclaw.vendor.finnhub import models
 from finclaw.vendor.finnhub.symbols import get_symbols_for
-from tqdm import tqdm
+from finclaw.utils.progress_bar import progress_bar
 
 
-async def get_financials(symbols: List[str], start: pd.Timestamp, end: pd.Timestamp, statement, freq) -> pa.Table:
+async def get_financials(
+    symbols: List[str], start: pd.Timestamp, end: pd.Timestamp, statement, freq
+) -> pa.Table:
     start = start.strftime("%Y-%m-%d")
     end = end.strftime("%Y-%m-%d")
     #  TODO:  This is going to be different for each symbol
     #  because the financials are different for each symbol
     result = []
-    for symbol in tqdm(symbols, desc="Pulling financials"):
+    for symbol in progress_bar(symbols, desc="Pulling financials"):
         async with aiohttp.ClientSession() as session:
-            financial_records = await get_financials_for(session, symbol=symbol, statement=statement, freq=freq)
+            financial_records = await get_financials_for(
+                session, symbol=symbol, statement=statement, freq=freq
+            )
 
             if statement == "bs":
                 try:
-                    if table := models.to_balance_sheet_financial_data(financial_records):
+                    if table := models.to_balance_sheet_financial_data(
+                        financial_records
+                    ):
                         result.append(table)
                 except Exception as e:
                     logger.error(f"Error pulling balance sheet data for {symbol} {e}")
                     raise e
-            elif statement == 'ic':
+            elif statement == "ic":
                 try:
-                    if table := models.to_income_statement_financial_data(financial_records):
+                    if table := models.to_income_statement_financial_data(
+                        financial_records
+                    ):
                         result.append(table)
                 except Exception as e:
-                    logger.error(f"Error pulling income statement data for {symbol} {e}")
+                    logger.error(
+                        f"Error pulling income statement data for {symbol} {e}"
+                    )
                     raise e
-            elif statement == 'cf':
+            elif statement == "cf":
                 try:
                     if table := models.to_cash_flow_financial_data(financial_records):
                         result.append(table)
                 except Exception as e:
                     logger.error(f"Error pulling cash flow data for {symbol} {e}")
                     raise e
             else:
                 raise ValueError(f"Unknown statement type {statement}")
 
     return pa.concat_tables(result)
 
 
 def pull_financials(*, store, symbols, start: Timestamp, end: Timestamp):
-    balance_sheet_table = asyncio.run(get_financials(symbols, start, end, "bs", "quarterly"))
-    store.store_financials(statement="balance_sheet",
-                           financials_table=balance_sheet_table,
-                           start=start,
-                           end=end,
-                           vendor="finnhub")
-
-    income_statement_table = asyncio.run(get_financials(symbols, start, end, "ic", "quarterly"))
-    store.store_financials(statement="income_statement",
-                           financials_table=income_statement_table,
-                           start=start,
-                           end=end,
-                           vendor="finnhub")
-
-    cashflow_statements = asyncio.run(get_financials(symbols, start, end, "cf", "quarterly"))
-    store.store_financials(statement="cashflow_statement",
-                           financials_table=cashflow_statements,
-                           start=start,
-                           end=end,
-                           vendor="finnhub")
+    balance_sheet_table = asyncio.run(
+        get_financials(symbols, start, end, "bs", "quarterly")
+    )
+    store.store_financials(
+        statement="balance_sheet",
+        financials_table=balance_sheet_table,
+        start=start,
+        end=end,
+        vendor="finnhub",
+    )
+
+    income_statement_table = asyncio.run(
+        get_financials(symbols, start, end, "ic", "quarterly")
+    )
+    store.store_financials(
+        statement="income_statement",
+        financials_table=income_statement_table,
+        start=start,
+        end=end,
+        vendor="finnhub",
+    )
+
+    cashflow_statements = asyncio.run(
+        get_financials(symbols, start, end, "cf", "quarterly")
+    )
+    store.store_financials(
+        statement="cashflow_statement",
+        financials_table=cashflow_statements,
+        start=start,
+        end=end,
+        vendor="finnhub",
+    )
```

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/pull_insider_information.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/pull_insider_information.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import asyncio
 from typing import List
 
 import aiohttp
 import pyarrow as pa
-from tqdm import tqdm
+from finclaw.utils.progress_bar import progress_bar
 
 from finclaw.vendor.finnhub import models
 from finclaw.vendor.finnhub.finnhub_client import get_insider_transactions
 
 
 async def get_insider_information_table(symbols: List[str]) -> pa.Table:
     result = []
-    for symbol in tqdm(symbols, desc="Pulling insider information"):
+    for symbol in progress_bar(symbols, desc="Pulling insider information"):
         async with aiohttp.ClientSession() as session:
-            insider_transaction_records = await get_insider_transactions(session, symbol=symbol)
+            insider_transaction_records = await get_insider_transactions(
+                session, symbol=symbol
+            )
             data_to_process = insider_transaction_records["data"]
             if table := models.to_insider_table(data_to_process):
                 result.append(table)
 
     return pa.concat_tables(result)
 
 
 def pull_insider_information(*, store, symbols, start, end):
     insider_information = asyncio.run(get_insider_information_table(symbols))
 
-    store.store_insider_information(insider_table=insider_information,
-                                    start=start, end=end, vendor="finnhub")
+    store.store_insider_information(
+        insider_table=insider_information, start=start, end=end, vendor="finnhub"
+    )
```

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/pull_ohcl.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/pull_ohcl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import asyncio
 from datetime import datetime
 from typing import List
 
 import aiohttp
 import pandas as pd
 import pyarrow as pa
+
 # from google.cloud import storage
 import pytz
 from pandas import Timestamp
-from tqdm import tqdm
+from finclaw.utils.progress_bar import progress_bar
 
 from finclaw.config import logger
 from finclaw.data_store.schema import STOCK_SYMBOL
 from finclaw.vendor.finnhub.finnhub_client import get_company_profile, get_stock_candle
 from finclaw.vendor.finnhub.models import to_company_description_table, to_ohcl_table
 from finclaw.vendor.finnhub.symbols import get_symbols_for
 
@@ -20,73 +21,79 @@
 # bucket = storage_client.bucket("social-signals-datalake")
 
 VENDOR = "finnhub"
 
 
 def data_to_df(data):
     df = pd.DataFrame(data=data)
-    df.index = pd.to_datetime(df.t, unit='s')
+    df.index = pd.to_datetime(df.t, unit="s")
     return df
 
 
 TIME_TEMPLATE = "%Y-%m-%d_%H%M%S"
 
 
 def get_human_time() -> str:
     created_at = datetime.now(tz=pytz.UTC)
     return created_at.strftime(TIME_TEMPLATE)
 
 
 def store_df_in_gs(symbol, df):
     day = datetime.now(tz=pytz.UTC).strftime("%Y-%m-%d")
-    blob = bucket.blob(f"finnhub/common_stocks/ohcl_daily/{day}/{symbol}_{get_human_time()}")
+    blob = bucket.blob(
+        f"finnhub/common_stocks/ohcl_daily/{day}/{symbol}_{get_human_time()}"
+    )
     blob.upload_from_string(df.to_csv())
 
 
 async def get_ohcl_data_for(session, start, end, symbol: str, frequency: str = "D"):
     try:
         data = await get_ohcl_data_(session, start, end, frequency, symbol)
         if data is not None:
             return to_ohcl_table(data, symbol)
     except Exception as e:
         logger.exception(e)
         return
 
 
 async def get_ohcl_data_(session, start: int, end: int, frequency, symbol):
-    data = await get_stock_candle(session=session, symbol=symbol, resolution=frequency, from_=start, to=end)
+    data = await get_stock_candle(
+        session=session, symbol=symbol, resolution=frequency, from_=start, to=end
+    )
 
-    return None if data['s'] == "no_data" else data
+    return None if data["s"] == "no_data" else data
 
 
 async def get_ohcl_table_for(start: int, end: int, symbols: List[str], frequency: str):
     logger.info("Start fetching OHLC data")
     tables = []
     symbols_n = len(symbols)
     # Partition symbols into groups of 3 and then do concurrent call
     async with aiohttp.ClientSession() as session:
-        for idx, symbol in tqdm(enumerate(symbols), total=symbols_n):
+        for idx, symbol in progress_bar(enumerate(symbols), total=symbols_n):
             if idx % 100 == 0:
                 logger.info(f"Remaining: {symbols_n - idx}")
 
-            table = await get_ohcl_data_for(session, start, end, symbol, frequency=frequency)
+            table = await get_ohcl_data_for(
+                session, start, end, symbol, frequency=frequency
+            )
             if isinstance(table, pa.Table):
                 tables.append(table)
             else:
                 logger.info(f"Skipping {symbol}")
         return pa.concat_tables(tables)
 
 
 async def get_company_table_for(symbols: List[str]) -> pa.Table:
     logger.info("Start fetching company descriptions data")
     tables = []
     symbols_n = len(symbols)
     # Partition symbols into groups of 3 and then do concurrent call
     async with aiohttp.ClientSession() as session:
-        for idx, symbol in tqdm(enumerate(symbols), total=symbols_n):
+        for idx, symbol in progress_bar(enumerate(symbols), total=symbols_n):
             if idx % 100 == 0:
                 logger.info(f"Remaining: {symbols_n - idx}")
 
             data = await get_company_profile(session, symbol)
             if data:
                 table = to_company_description_table(data)
             else:
@@ -95,29 +102,40 @@
             if isinstance(table, pa.Table):
                 tables.append(table)
             else:
                 logger.info(f"Skipping {symbol}")
         return pa.concat_tables(tables)
 
 
-def pull_ohcl_data(*, store, start: Timestamp, end: Timestamp, market: str, frequency: str,
-                   include_company_information: bool = True):
+def pull_ohcl_data(
+    *,
+    store,
+    start: Timestamp,
+    end: Timestamp,
+    market: str,
+    frequency: str,
+    include_company_information: bool = True,
+):
     company_table = None
 
     df_symbols, symbols = get_symbols_for(market)
     symbol_table = pa.Table.from_pandas(df_symbols, schema=STOCK_SYMBOL)
 
     start_timestamp = int(start.timestamp())
     end_timestamp = int(end.timestamp())
 
     if include_company_information:
         company_table = asyncio.run(get_company_table_for(symbols=symbols))
 
-    table = asyncio.run(get_ohcl_table_for(start_timestamp, end_timestamp, symbols, frequency))
-
-    store.store(symbol_table=symbol_table,
-                price_table=table,
-                company_table=company_table,
-                start=start,
-                end=end,
-                frequency=frequency,
-                vendor=VENDOR)
+    table = asyncio.run(
+        get_ohcl_table_for(start_timestamp, end_timestamp, symbols, frequency)
+    )
+
+    store.store(
+        symbol_table=symbol_table,
+        price_table=table,
+        company_table=company_table,
+        start=start,
+        end=end,
+        frequency=frequency,
+        vendor=VENDOR,
+    )
```

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/pull_ownership.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/pull_ownership.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 import asyncio
 from typing import List
 
 import aiohttp
 import pandas as pd
 import pyarrow as pa
-from tqdm import tqdm
+from finclaw.utils.progress_bar import progress_bar
 
 import finclaw.vendor.finnhub.finnhub_client as fc
 from finclaw.vendor.finnhub import models
 
 
-async def get_institutional_ownership_table(symbols: List[str], start: pd.Timestamp, end: pd.Timestamp) -> pa.Table:
+async def get_institutional_ownership_table(
+    symbols: List[str], start: pd.Timestamp, end: pd.Timestamp
+) -> pa.Table:
     start = start.strftime("%Y-%m-%d")
     end = end.strftime("%Y-%m-%d")
 
     result = []
-    for symbol in tqdm(symbols, desc="Pulling institutional ownership information"):
+    for symbol in progress_bar(
+        symbols, desc="Pulling institutional ownership information"
+    ):
         async with aiohttp.ClientSession() as session:
-            insider_transaction_records = await fc.get_institutional_ownership(session, symbol=symbol, from_=start,
-                                                                               to=end)
+            insider_transaction_records = await fc.get_institutional_ownership(
+                session, symbol=symbol, from_=start, to=end
+            )
 
             if table := models.to_institutional_ownership_table(
-                    insider_transaction_records
+                insider_transaction_records
             ):
                 result.append(table)
 
     return pa.concat_tables(result)
 
 
 async def get_fund_ownership_table(symbols: List[str]) -> pa.Table:
     result = []
-    for symbol in tqdm(symbols, desc="Pulling fund ownership information"):
+    for symbol in progress_bar(symbols, desc="Pulling fund ownership information"):
         async with aiohttp.ClientSession() as session:
             fund_ownership_record = await fc.get_fund_ownership(session, symbol=symbol)
             if table := models.to_fund_ownership_table(fund_ownership_record):
                 result.append(table)
 
     return pa.concat_tables(result)
 
 
 async def get_all_owners_table(symbols: List[str]) -> pa.Table:
     result = []
-    for symbol in tqdm(symbols, desc="Pull all owners data"):
+    for symbol in progress_bar(symbols, desc="Pull all owners data"):
         async with aiohttp.ClientSession() as session:
             all_owners_table = await fc.get_all_owners(session, symbol=symbol)
             if table := models.to_all_owners_table(all_owners_table):
                 result.append(table)
     return pa.concat_tables(result)
 
 
 def pull_ownership_data_for(*, store, symbols, start, end):
-    institutional_ownership = asyncio.run(get_institutional_ownership_table(symbols, start, end))
+    institutional_ownership = asyncio.run(
+        get_institutional_ownership_table(symbols, start, end)
+    )
     fund_ownership = asyncio.run(get_fund_ownership_table(symbols))
     all_owners = asyncio.run(get_all_owners_table(symbols))
 
-    store.store_ownership(institutional_ownership_table=institutional_ownership,
-                          fund_ownership_table=fund_ownership,
-                          all_owners_table=all_owners,
-                          start=start, end=end, vendor="finnhub")
+    store.store_ownership(
+        institutional_ownership_table=institutional_ownership,
+        fund_ownership_table=fund_ownership,
+        all_owners_table=all_owners,
+        start=start,
+        end=end,
+    )
```

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/pull_splits.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/pull_splits.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import asyncio
 from typing import List
 
 import aiohttp
 import pandas as pd
 import pyarrow as pa
-from tqdm import tqdm
+from finclaw.utils.progress_bar import progress_bar
 
 import finclaw.vendor.finnhub.finnhub_client as fc
 from finclaw.vendor.finnhub import models
 
 
-async def get_splits(symbols: List[str], start: pd.Timestamp, end: pd.Timestamp) -> pa.Table:
+async def get_splits(
+    symbols: List[str], start: pd.Timestamp, end: pd.Timestamp
+) -> pa.Table:
     start = start.strftime("%Y-%m-%d")
     end = end.strftime("%Y-%m-%d")
 
     result = []
-    for symbol in tqdm(symbols, desc="Pulling splits information:"):
+    for symbol in progress_bar(symbols, desc="Pulling splits information:"):
         async with aiohttp.ClientSession() as session:
-            split_records = await fc.get_stock_splits(session, symbol=symbol, from_=start, to=end)
+            split_records = await fc.get_stock_splits(
+                session, symbol=symbol, from_=start, to=end
+            )
 
             if table := models.to_split_data(split_records, symbol):
                 result.append(table)
 
     return pa.concat_tables(result)
```

### Comparing `finclaw-0.0.2/finclaw/vendor/finnhub/symbols.py` & `finclaw-0.0.3/finclaw/vendor/finnhub/symbols.py`

 * *Files identical despite different names*

### Comparing `finclaw-0.0.2/finclaw/vendor/fmp/fmp_client.py` & `finclaw-0.0.3/finclaw/vendor/fmp/fmp_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,81 @@
 import asyncio
-import re
-from typing import Optional, List
 
 import aiohttp
 
 from finclaw.config import logger
 from finclaw.config import settings
-from finclaw.vendor.exceptions import NotSuccessfull
 
 API_BASE = "https://financialmodelingprep.com/api/v3/"
 
 
 # 30 API/Seconds limit
 
-async def _call_api(session, url: str, payload: str, querystring: dict, error_count=0) -> dict:
+
+async def _call_api(
+    session, url: str, payload: str, querystring: dict, error_count=0
+) -> dict:
     if settings.FMP_API_KEY == "":
         raise ValueError("You need to specify FMP_API_KEY")
     querystring["apikey"] = settings.FMP_API_KEY
+
     async with session.get(url, data=payload, params=querystring) as resp:
+        if error_count >= 4:
+            raise ValueError(f"Too many errors: {resp.status}")
+        if resp.status != 200:
+            logger.info("Rate limit reached going to sleep")
+            await asyncio.sleep(60)
+            return await _call_api(session, url, payload, querystring, error_count + 1)
         try:
             json_response = await resp.json()
         except aiohttp.ContentTypeError as e:
             logger.exception("Could not parse response")
         return json_response
 
 
 async def get_symbols(session: aiohttp.ClientSession):
     querystring = {}
     return await _call_api(
         session,
-        f"{API_BASE}symbol/available-tsx",
+        f"{API_BASE}stock/list",
         payload="",
         querystring={},
     )
 
 
-async def get_stock_candle(session: aiohttp.ClientSession, symbol: str, resolution: str):
+async def get_stock_candle(
+    session: aiohttp.ClientSession, symbol: str, resolution: str
+):
     if resolution == "1":
         return await _call_api(
-            session, f"{API_BASE}historical-chart/1min/{symbol}", payload="", querystring={}
+            session,
+            f"{API_BASE}historical-chart/1min/{symbol}",
+            payload="",
+            querystring={},
         )
     else:
         raise NotImplementedError("Only 1 minute resolution is supported")
+
+
+async def get_financials_for(
+    session: aiohttp.ClientSession, symbol: str, statement: str, freq: str
+):
+    """
+    https://site.financialmodelingprep.com/developer/docs#financial-statements
+    """
+    endpoint_map = {
+        "bs": "balance-sheet-statement",
+        "ic": "income-statement",
+        "cf": "cash-flow-statement",
+    }
+    periods = ["annual", "quarter"]
+    if statement not in endpoint_map:
+        raise ValueError(f"statement:{statement} should be one of bs, ic, cf")
+    if freq not in periods:
+        raise ValueError(f"freq:{freq} should be one of {periods}")
+
+    return await _call_api(
+        session,
+        f"{API_BASE}{endpoint_map[statement]}/{symbol}",
+        payload="",
+        querystring={"period": freq},
+    )
```

### Comparing `finclaw-0.0.2/finclaw/vendor/kraken/exchange.py` & `finclaw-0.0.3/finclaw/vendor/kraken/exchange.py`

 * *Files identical despite different names*

### Comparing `finclaw-0.0.2/finclaw/vendor/twelvedata/twelve.py` & `finclaw-0.0.3/finclaw/vendor/twelvedata/twelve.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,129 @@
 import asyncio
-from typing import Tuple, Any, List, Optional
+from typing import List, Optional
 
 import aiohttp
 import pandas as pd
+import pyarrow as pa
 import pytz
-from pandas import DataFrame, Timestamp
-from tqdm import tqdm
+from pandas import Timestamp
 
+from finclaw.config import logger
 from finclaw.data_store.schema import OHCL, STOCK_SYMBOL
 from finclaw.data_store.store import PriceStore
+from finclaw.data_store.storeV2 import PriceStoreV2
+from finclaw.utils.progress_bar import progress_bar
 from finclaw.vendor.twelvedata import twelve_client as twclient
-import pyarrow as pa
 
 VENDOR = "twelvedata"
 
 
 async def get_symbols(session: aiohttp.ClientSession, market: str) -> pd.DataFrame:
-    async with aiohttp.ClientSession() as session:
-        symbols = await twclient.get_symbols(session=session)
-        data = filter(lambda x: x["mic_code"] == market, symbols["data"])
-        df = pd.DataFrame(data=data)
-        df = df.rename(
-            columns={"symbol": "ticker", "name": "description", "currency": "currency_name", "mic_code": "mic"})
-        df["figi"] = None
+    symbols = await twclient.get_symbols(session=session)
+    data = filter(lambda x: x["mic_code"] == market, symbols["data"])
+    df = pd.DataFrame(data=data)
+    df = df.rename(
+        columns={
+            "symbol": "ticker",
+            "name": "description",
+            "currency": "currency_name",
+            "mic_code": "mic",
+        }
+    )
+    df["figi"] = None
     return df[STOCK_SYMBOL.names]
 
 
-async def get_ohcl_for_symbol(session: aiohttp.ClientSession, *, symbol: str,
-                              resolution: str, mic_code: str) -> Optional[pd.DataFrame]:
-    ohcl_json = await twclient.get_stock_candle(session=session, symbol=symbol, resolution=resolution,
-                                                mic_code=mic_code)
+async def get_ohcl_for_symbol(
+    session: aiohttp.ClientSession, *, symbol: str, resolution: str, mic_code: str
+) -> Optional[pd.DataFrame]:
+    ohcl_json = await twclient.get_stock_candle(
+        session=session, symbol=symbol, resolution=resolution, mic_code=mic_code
+    )
     if not ohcl_json:
         return None
     df = pd.DataFrame(data=ohcl_json["values"])
-    df["timestamp"] = pd.to_datetime(df["datetime"]).dt.tz_localize('America/New_york')
+    df["timestamp"] = pd.to_datetime(df["datetime"]).dt.tz_localize("America/New_york")
     df["timestamp"] = df["timestamp"].dt.tz_convert("UTC")
     df["symbol"] = symbol
 
-    df[["open", "high", "close", "low"]] = df[["open", "high", "close", "low"]].astype(float)
+    df[["open", "high", "close", "low"]] = df[["open", "high", "close", "low"]].astype(
+        float
+    )
     df["volume"] = df["volume"].astype(int)
 
     return df[OHCL.names]
 
 
-async def get_ohcl_data(session: aiohttp.ClientSession,
-                        *,
-                        start: Timestamp,
-                        end: Timestamp,
-                        symbols: List[str],
-                        frequency: str,
-                        mic_code: str) -> pd.DataFrame:
+async def get_ohcl_data(
+    session: aiohttp.ClientSession,
+    *,
+    start: Timestamp,
+    end: Timestamp,
+    symbols: List[str],
+    frequency: str,
+    mic_code: str,
+) -> pd.DataFrame:
     if start > end:
         raise ValueError("Start date cannot be greater than end date")
     if start.tz != pytz.UTC or end.tz != pytz.UTC:
         raise ValueError("Start and end dates must be UTC")
 
     dfs = []
-    for symbol in tqdm(symbols):
-        symbol_df = await get_ohcl_for_symbol(session=session, symbol=symbol, resolution=frequency, mic_code=mic_code)
+    for symbol in progress_bar(symbols):
+        symbol_df = await get_ohcl_for_symbol(
+            session=session, symbol=symbol, resolution=frequency, mic_code=mic_code
+        )
         if symbol_df is not None:
             dfs.append(symbol_df)
 
     result_df = pd.concat(dfs)
     return result_df[(result_df.timestamp >= start) & (result_df.timestamp <= end)]
 
 
 async def get_symbol_table(market_id_code: str) -> pa.Table:
     async with aiohttp.ClientSession() as session:
         symbol_df = await get_symbols(session=session, market=market_id_code)
         return pa.Table.from_pandas(symbol_df, schema=STOCK_SYMBOL)
 
 
-async def get_ohcl_table_for(start: Timestamp, end: Timestamp, symbols: List[str], frequency: str,
-                             market_id_code: str) -> pa.Table:
+async def get_ohcl_table_for(
+    start: Timestamp,
+    end: Timestamp,
+    symbols: List[str],
+    frequency: str,
+    market_id_code: str,
+) -> pa.Table:
     async with aiohttp.ClientSession() as session:
-        ohcl_df = await get_ohcl_data(session=session, start=start, end=end, symbols=symbols, frequency=frequency,
-                                      mic_code=market_id_code)
+        ohcl_df = await get_ohcl_data(
+            session=session,
+            start=start,
+            end=end,
+            symbols=symbols,
+            frequency=frequency,
+            mic_code=market_id_code,
+        )
         return pa.Table.from_pandas(ohcl_df, schema=OHCL)
 
 
-def pull_symbols(*, store: PriceStore, market_id_code: str, start: pd.Timestamp, end: pd.Timestamp):
+def pull_symbols(
+    *, store: PriceStoreV2, market_id_code: str, start: pd.Timestamp, end: pd.Timestamp
+):
     symbol_table = asyncio.run(get_symbol_table(market_id_code=market_id_code))
-    store.store_symbols(symbol_table=symbol_table, start=start, end=end, vendor=VENDOR)
+    store.store_symbols(symbol_table=symbol_table, start=start, end=end)
 
 
-def pull_ohcl_data(*, store: PriceStore, symbols: List[str], start: Timestamp, end: Timestamp, frequency: str,
-                   market_id_code: str):
-    table = asyncio.run(get_ohcl_table_for(start, end, symbols, frequency, market_id_code=market_id_code))
-    store.store_prices(price_table=table, start=start, end=end, vendor=VENDOR, frequency=frequency)
+def pull_ohcl_data(
+    *,
+    store: PriceStoreV2,
+    symbols: List[str],
+    start: Timestamp,
+    end: Timestamp,
+    frequency: str,
+    market_id_code: str,
+):
+    table = asyncio.run(
+        get_ohcl_table_for(
+            start, end, symbols, frequency, market_id_code=market_id_code
+        )
+    )
+    store.store_prices(price_table=table, start=start, end=end, frequency=frequency)
```

### Comparing `finclaw-0.0.2/finclaw/vendor/twelvedata/twelve_client.py` & `finclaw-0.0.3/finclaw/vendor/twelvedata/twelve_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,37 @@
 from finclaw.vendor.exceptions import NotSuccessfull
 
 API_BASE = "https://api.twelvedata.com/"
 
 
 # 30 API/Seconds limit
 
-async def _call_api(session, url: str, payload: str, querystring: dict, error_count=0) -> Optional[dict]:
+
+async def _call_api(
+    session, url: str, payload: str, querystring: dict, error_count=0
+) -> Optional[dict]:
     if settings.FMP_API_KEY == "":
         raise ValueError("You need to specify TWELVEDATA_API_KEY")
     querystring["apikey"] = settings.TWELVEDATA_API_KEY
+    logger.debug(f"Calling {url} with {querystring}")
+    del querystring["mic_code"]
     async with session.get(url, data=payload, params=querystring) as resp:
+        logger.debug(f"Calling {url} with {querystring}")
         try:
             json_response = await resp.json()
+            logger.debug(f"Response: {json_response}")
             if return_code := json_response.get("code", None):
                 if return_code == 429:
                     if error_count > 5:
                         raise NotSuccessfull("Too many errors")
                     logger.warning("Rate limit reached going to sleep")
                     await asyncio.sleep(60)
-                    return await _call_api(session, url, payload, querystring, error_count=error_count + 1)
+                    return await _call_api(
+                        session, url, payload, querystring, error_count=error_count + 1
+                    )
                 elif return_code == 404:
                     logger.warning(f"Not found:{json_response}")
                     return None
                 else:
                     raise NotSuccessfull(f"Error code: {return_code}")
 
         except aiohttp.ContentTypeError as e:
@@ -44,18 +53,47 @@
         session,
         f"{API_BASE}stocks",
         payload="",
         querystring={},
     )
 
 
-async def get_stock_candle(session: aiohttp.ClientSession, *, symbol: str, resolution: str, mic_code: str):
+async def get_stock_candle(
+    session: aiohttp.ClientSession, *, symbol: str, resolution: str, mic_code: str
+):
+    """
+    5min, 15min, 30min, 45min, 1h, 2h, 4h, 1day, 1week, 1month
+    Parameters
+    ----------
+    session
+    symbol
+    resolution
+    mic_code
+
+    Returns
+    -------
+
+    """
     if resolution == "1":
         return await _call_api(
-            session, f"{API_BASE}time_series", payload="", querystring={
+            session,
+            f"{API_BASE}time_series",
+            payload="",
+            querystring={
                 "interval": "1min",
                 "symbol": symbol,
                 "mic_code": mic_code,
-            }
+            },
+        )
+    elif resolution == "D":
+        return await _call_api(
+            session,
+            f"{API_BASE}time_series",
+            payload="",
+            querystring={
+                "interval": "1day",
+                "symbol": symbol,
+                "mic_code": mic_code,
+            },
         )
     else:
         raise NotImplementedError("Only 1 minute resolution is supported")
```

### Comparing `finclaw-0.0.2/pyproject.toml` & `finclaw-0.0.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "finclaw"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["bobrinik <bobrinik@pm.me>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
-greet = "finclaw.main:main"
+finclaw = "finclaw.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^1.5.2"
 click = "^8.1.3"
 pydantic = { extras = ["dotenv"], version = "^1.10.4" }
-pyarrow = "^10.0.1"
+pyarrow = "^14.0.0"
 aiohttp = "^3.8.3"
 tqdm = "^4.64.1"
 matplotlib = "^3.6.3"
 requests = "^2.28.2"
 google-cloud-storage = "^2.10.0"
+boto3 = "^1.34.24"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 jupyter = "^1.0.0"
 
 [build-system]
```

