# Comparing `tmp/py_alpaca_api-0.6.3.tar.gz` & `tmp/py_alpaca_api-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.6.3.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.6.4.tar", max compression
```

## Comparing `py_alpaca_api-0.6.3.tar` & `py_alpaca_api-0.6.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1066 2024-05-25 20:54:28.642031 py_alpaca_api-0.6.3/LICENSE
--rw-r--r--   0        0        0    17780 2024-05-28 01:41:42.529974 py_alpaca_api-0.6.3/README.md
--rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.3/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2275 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.3/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.3/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     6777 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.3/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     2898 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.3/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    11730 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.3/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     7469 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.3/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2984 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.3/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    20152 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.3/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0     9323 2024-05-28 01:32:55.543711 py_alpaca_api-0.6.3/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     9600 2024-05-30 22:46:51.399125 py_alpaca_api-0.6.3/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    14988 2024-05-28 23:39:58.663626 py_alpaca_api-0.6.3/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1344 2024-05-30 22:46:51.399125 py_alpaca_api-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    18582 1970-01-01 00:00:00.000000 py_alpaca_api-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.6.4/LICENSE
+-rw-r--r--   0        0        0    17780 2024-06-01 03:16:13.087825 py_alpaca_api-0.6.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.6.4/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2275 2024-06-01 03:16:13.097825 py_alpaca_api-0.6.4/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:57:11.657657 py_alpaca_api-0.6.4/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     6313 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     2640 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    11730 2024-06-01 03:16:13.097825 py_alpaca_api-0.6.4/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7360 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2945 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    18520 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0     8869 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     2106 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/requests.py
+-rw-r--r--   0        0        0     9400 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    14784 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1344 2024-06-01 00:51:31.644447 py_alpaca_api-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    18582 1970-01-01 00:00:00.000000 py_alpaca_api-0.6.4/PKG-INFO
```

### Comparing `py_alpaca_api-0.6.3/LICENSE` & `py_alpaca_api-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.3/README.md` & `py_alpaca_api-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.6.4/py_alpaca_api/alpaca.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/account.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/account.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from typing import Dict
 
 import pandas as pd
 import pendulum
-import requests
 
 from .data_classes import AccountClass, account_class_from_dict
+from .requests import Requests
 
 
 class Account:
     def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
         """
         Args:
             trade_url: The URL for the trade.
@@ -44,19 +44,20 @@
             raise ValueError("One of the Date and Until Date are required, not both or neither.")
 
         params = {
             "date": date if date else None,
             "until_date": until_date if until_date else None,
         }
 
-        request = requests.get(url=url, headers=self.headers, params=params)
+        # request = requests.get(url=url, headers=self.headers, params=params)
 
-        if request.status_code != 200:
-            raise Exception(f"Failed to get account activities. Response: {request.text}")
+        # if request.status_code != 200:
+        #     raise Exception(f"Failed to get account activities. Response: {request.text}")
 
+        request = Requests().get(url=url, headers=self.headers, params=params)
         response = json.loads(request.text)
 
         activity_df = pd.DataFrame()
         activity_df.assign(
             symbol="NAN",
             activity_type="NAN",
             id="NAN",
@@ -120,24 +121,18 @@
 
             Example:
                 >>> account = account.get()
         """
         # Alpaca API URL for account information
         url = f"{self.trade_url}/account"
         # Get request to Alpaca API for account information
-        response = requests.get(url, headers=self.headers)
-        # Check if response is successful
-        if response.status_code == 200:
-            # Convert JSON response to dictionary
-            res = json.loads(response.text)
-            # Return account information as an AccountClass object
-            return account_class_from_dict(res)
-        # If response is not successful, raise an exception
-        else:
-            raise Exception(f"Failed to get account information. Response: {response.text}")
+        request = Requests().get(url=url, headers=self.headers)
+        response = json.loads(request.text)
+
+        return account_class_from_dict(response)
 
     ########################################################
     # \\\\\\\\\\\\\  Get Portfolio History ///////////////#
     ########################################################
     def portfolio_history(
         self,
         period: str = "1W",
@@ -156,38 +151,33 @@
         Raises:
             Exception: If the request to the Alpaca API fails.
 
         """
 
         url = f"{self.trade_url}/account/portfolio/history"
 
-        response = requests.get(
-            url,
-            headers=self.headers,
-            params={
-                "period": period,
-                "timeframe": timeframe,
-                "intraday_reporting": intraday_reporting,
-            },
+        params = {
+            "period": period,
+            "timeframe": timeframe,
+            "intraday_reporting": intraday_reporting,
+        }
+
+        request = Requests().get(url=url, headers=self.headers, params=params)
+        response = json.loads(request.text)
+
+        portfolio_df = pd.DataFrame(
+            response,
+            columns=[
+                "timestamp",
+                "equity",
+                "profit_loss",
+                "profit_loss_pct",
+                "base_value",
+            ],
         )
 
-        if response.status_code == 200:
-            res = json.loads(response.text)
-            res_df = pd.DataFrame(
-                res,
-                columns=[
-                    "timestamp",
-                    "equity",
-                    "profit_loss",
-                    "profit_loss_pct",
-                    "base_value",
-                ],
-            )
-
-            timestamp_transformed = (
-                pd.to_datetime(res_df["timestamp"], unit="s").dt.tz_localize("America/New_York").dt.tz_convert("UTC").apply(lambda x: x.date())
-            )
-            res_df["timestamp"] = timestamp_transformed
-            res_df["profit_loss_pct"] = res_df["profit_loss_pct"] * 100
-            return res_df
-        else:
-            raise Exception(f"Failed to get portfolio information. Response: {response.text}")
+        timestamp_transformed = (
+            pd.to_datetime(portfolio_df["timestamp"], unit="s").dt.tz_localize("America/New_York").dt.tz_convert("UTC").apply(lambda x: x.date())
+        )
+        portfolio_df["timestamp"] = timestamp_transformed
+        portfolio_df["profit_loss_pct"] = portfolio_df["profit_loss_pct"] * 100
+        return portfolio_df
```

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/asset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Dict
 
 import pandas as pd
-import requests
 
 from .data_classes import AssetClass, asset_class_from_dict
+from .requests import Requests
 
 
 class Asset:
     def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
         """
         Initialize a new Asset object.
 
@@ -46,28 +46,25 @@
         url = f"{self.trade_url}/assets"
         params = {
             "status": status,
             "asset_class": asset_class,
             "exchange": exchange,
         }
 
-        response = requests.get(url, headers=self.headers, params=params)
+        request = Requests().get(url, headers=self.headers, params=params)
 
-        if response.status_code == 200:
-            res_df = pd.json_normalize(json.loads(response.text))
+        assets_df = pd.json_normalize(json.loads(request.text))
 
-            res_df = res_df[res_df["status"] == "active"]
-            res_df = res_df[res_df["fractionable"]]
-            res_df = res_df[res_df["tradable"]]
-            res_df = res_df[res_df["exchange"] != "OTC"]
-            res_df.reset_index(drop=True, inplace=True)
-
-            return res_df
-        else:
-            raise ValueError(f"Failed to get asset information. Response: {response.text}")
+        assets_df = assets_df[assets_df["status"] == "active"]
+        assets_df = assets_df[assets_df["fractionable"]]
+        assets_df = assets_df[assets_df["tradable"]]
+        assets_df = assets_df[assets_df["exchange"] != "OTC"]
+        assets_df.reset_index(drop=True, inplace=True)
+
+        return assets_df
 
     #####################################################
     # \\\\\\\\\\\\\\\\\\\  Get Asset ////////////////////#
     #####################################################
     def get(self, symbol: str) -> AssetClass:
         """
         Retrieves asset information for a given symbol.
@@ -77,16 +74,13 @@
 
         Returns:
             AssetClass: An object representing the asset information.
 
         Raises:
             ValueError: If the request to the Alpaca API fails.
         """
-
         url = f"{self.trade_url}/assets/{symbol}"
-        response = requests.get(url, headers=self.headers)
 
-        if response.status_code == 200:
-            res = json.loads(response.text)
-            return asset_class_from_dict(res)
-        else:
-            raise ValueError(f"Failed to get asset information. Response: {response.text}")
+        request = Requests().get(url, headers=self.headers)
+
+        response = json.loads(request.text)
+        return asset_class_from_dict(response)
```

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/data_classes.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/history.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import json
 from collections import defaultdict
 from typing import Dict
 
 import pandas as pd
-import requests
 
 from .asset import Asset
 from .data_classes import AssetClass
+from .requests import Requests
 
 
 class History:
     def __init__(self, data_url: str, headers: Dict[str, str], asset: Asset) -> None:
         """
         Args:
             data_url: A string representing the URL of the data.
@@ -184,16 +183,16 @@
         This function fetches historical data for a given symbol by making requests to the specified API endpoint.
         It uses a page token to paginate through the response data and retrieves all available historical bars.
         """
         page_token = None
         symbols_data = defaultdict(list)
         while True:
             params["page_token"] = page_token
-            response = requests.get(url, headers=self.headers, params=params)
-            if response.status_code != 200:
-                raise Exception(json.loads(response.text)["message"])
-            res_data = response.json()
+
+            request = Requests().get(url, headers=self.headers, params=params)
+
+            res_data = request.json()
             symbols_data[symbol].extend(res_data.get("bars", []))
             page_token = res_data.get("next_page_token", "")
             if not page_token:
                 break
         return symbols_data[symbol]
```

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/market.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/market.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Dict
 
 import pandas as pd
-import requests
 
 from .data_classes import ClockClass, clock_class_from_dict
+from .requests import Requests
 
 
 class Market:
     def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
         """
         Initialize the Trade class with the provided trade URL and headers.
 
@@ -20,18 +20,17 @@
         self.headers = headers
 
     ########################################################
     # \\\\\\\\\\\\\\\\ Get API Response ///////////////////#
     ########################################################
     @staticmethod
     def get_api_response(url: str, headers: Dict[str, str], params: Dict[str, str] = None) -> Dict:
-        response = requests.get(url, headers=headers, params=params)
-        data = json.loads(response.text)
-        if response.status_code != 200:
-            raise Exception(f'Failed to get data from API. Response: {data["message"]}')
+        # response = requests.get(url, headers=headers, params=params)
+        request = Requests().get(url=url, headers=headers, params=params)
+        data = json.loads(request.text)
         return data
 
     ########################################################
     # \\\\\\\\\\\\\\\\\ Market Calender ///////////////////#
     ########################################################
     def calender(self, start_date: str, end_date: str) -> pd.DataFrame:
         """
```

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/order.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/order.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from typing import Dict
 
-import requests
-
 from .data_classes import OrderClass, order_class_from_dict
+from .requests import Requests
 
 
 class Order:
     def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
         """
         Initializes a new instance of the Order class.
 
@@ -34,31 +33,21 @@
 
         Returns:
             OrderClass: An object representing the order information.
 
         Raises:
             ValueError: If the request to retrieve order information fails.
         """
-
-        # Parameters for the request
         params = {"nested": nested}
-        # Alpaca API URL for order information
         url = f"{self.trade_url}/orders/{order_id}"
-        # Get request to Alpaca API for order information
-        response = requests.get(url, headers=self.headers, params=params)
-        # Check if response is successful
-        if response.status_code == 200:
-            # Convert JSON response to dictionary
-            res = json.loads(response.text)
-            # Return order information as an OrderClass object
-            return order_class_from_dict(res)
-        # If response is not successful, raise an exception
-        else:
-            res = json.loads(response.text)
-            raise ValueError(f'Failed to get order information. Response: {res["message"]}')
+
+        request = Requests().get(url=url, headers=self.headers, params=params)
+
+        response = json.loads(request.text)
+        return order_class_from_dict(response)
 
     ########################################################
     # \\\\\\\\\\\\\\\\\ Cancel Order By ID /////////////////#
     ########################################################
     def cancel_by_id(self, order_id: str) -> str:
         """
         Cancel an order by its ID.
@@ -68,54 +57,38 @@
 
         Returns:
             str: A message indicating the status of the cancellation.
 
         Raises:
             Exception: If the cancellation request fails, an exception is raised with the error message.
         """
-
-        # Alpaca API URL for canceling an order
         url = f"{self.trade_url}/orders/{order_id}"
-        # Delete request to Alpaca API for canceling an order
-        response = requests.delete(url, headers=self.headers)
-        # Check if response is successful
-        if response.status_code == 204:
-            # Convert JSON response to dictionary
-            return f"Order {order_id} has been cancelled"
-        # If response is not successful, raise an exception
-        else:
-            res = json.loads(response.text)
-            raise Exception(f'Failed to cancel order {order_id}, Response: {res["message"]}')
+
+        Requests().delete(url=url, headers=self.headers)
+
+        return f"Order {order_id} has been cancelled"
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Cancel All Orders //////////////////#
     ########################################################
     def cancel_all(self) -> str:
         """
         Cancels all open orders.
 
         Returns:
             str: A message indicating the number of orders that have been cancelled.
 
         Raises:
             Exception: If the request to cancel orders is not successful, an exception is raised with the error message.
         """
-        # Alpaca API URL for canceling all orders
         url = f"{self.trade_url}/orders"
-        # Delete request to Alpaca API for canceling all orders
-        response = requests.delete(url, headers=self.headers)
-        # Check if response is successful
-        if response.status_code == 207:
-            # Convert JSON response to dictionary
-            res = json.loads(response.text)
-            return f"{len(res)} orders have been cancelled"
-        # If response is not successful, raise an exception
-        else:
-            res = json.loads(response.text)
-            raise Exception(f'Failed to cancel orders. Response: {res["message"]}')
+        request = Requests().delete(url=url, headers=self.headers)
+
+        response = json.loads(request.text)
+        return f"{len(response)} orders have been cancelled"
 
     @staticmethod
     def check_for_order_errors(
         symbol: str,
         qty: float = None,
         notional: float = None,
         take_profit: float = None,
@@ -485,15 +458,11 @@
             "type": entry_type,
             "time_in_force": time_in_force,
             "extended_hours": extended_hours,
         }
 
         url = f"{self.trade_url}/orders"
 
-        response = requests.post(url, headers=self.headers, json=payload)
+        request = Requests().post(url=url, headers=self.headers, payload=payload)
 
-        if response.status_code == 200:
-            res = json.loads(response.text)
-            return order_class_from_dict(res)
-        else:
-            res = json.loads(response.text)
-            raise Exception(f'Failed to submit order. Code: {response.status_code}, Response: {res["message"]}')
+        response = json.loads(request.text)
+        return order_class_from_dict(response)
```

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/position.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/position.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import pandas as pd
-import requests
 
 from .account import Account
 from .data_classes import PositionClass, position_class_from_dict
+from .requests import Requests
 
 
 class Position:
     def __init__(self, trade_url: str, headers: dict[str, str], account: Account) -> None:
         """
         Initializes a Position object.
 
@@ -35,20 +35,18 @@
             pd.DataFrame: A DataFrame containing the positions data.
 
         Raises:
             Exception: If the API response is not successful.
         """
 
         url = f"{self.trade_url}/positions"
-        response = requests.get(url, headers=self.headers)
+        request = Requests().get(url=url, headers=self.headers)
+        # response = requests.get(url, headers=self.headers)
 
-        if response.status_code != 200:
-            raise Exception(response.text)
-
-        res_data_df = pd.json_normalize(json.loads(response.text))
+        res_data_df = pd.json_normalize(json.loads(request.text))
 
         pos_data_df = pd.DataFrame(
             {
                 "asset_id": "",
                 "symbol": "Cash",
                 "exchange": "",
                 "asset_class": "",
@@ -144,20 +142,17 @@
         if symbol and symbol_dict:
             raise ValueError("Symbol or symbol_dict is required, not both.")
 
         if symbol_dict:
             return position_class_from_dict(symbol_dict)
 
         url = f"{self.trade_url}/positions/{symbol}"
-        response = requests.get(url, headers=self.headers)
-
-        if response.status_code != 200:
-            raise ValueError(response.text)
+        request = Requests().get(url=url, headers=self.headers)
 
-        res_dict = json.loads(response.text)
+        res_dict = json.loads(request.text)
 
         equity = self.account.get().equity
         res_dict["portfolio_pct"] = round(float(res_dict["market_value"]) / equity, 4)
 
         res_dict["profit_dol"] = round(float(res_dict["unrealized_pl"]), 2)
         del res_dict["unrealized_pl"]
 
@@ -189,22 +184,19 @@
         Raises:
             Exception: If the request to close positions is not successful, an exception is raised with
                 the error message from the API response.
         """
 
         url = f"{self.trade_url}/positions"
         params = {"cancel_orders": cancel_orders}
-        response = requests.delete(url, headers=self.headers, params=params)
 
-        if response.status_code == 207:
-            res = json.loads(response.text)
-            return f"{len(res)} positions have been closed"
-        else:
-            res = json.loads(response.text)
-            raise Exception(f'Failed to close positions. Response: {res["message"]}')
+        request = Requests().delete(url=url, headers=self.headers, params=params)
+
+        response = json.loads(request.text)
+        return f"{len(response)} positions have been closed"
 
     ########################################################
     # \\\\\\\\\\\\\\\\\\ Close Position ///////////////////#
     ########################################################
     def close(self, symbol_or_id: str, qty: float = None, percentage: int = None) -> str:
         """
         Closes a position for a given symbol or asset ID.
@@ -232,14 +224,10 @@
         if percentage and (percentage < 0 or percentage > 100):
             raise ValueError("Percentage must be between 0 and 100.")
         if not symbol_or_id:
             raise ValueError("Symbol or asset_id is required.")
 
         url = f"{self.trade_url}/positions/{symbol_or_id}"
         params = {"qty": qty, "percentage": percentage}
-        response = requests.delete(url, headers=self.headers, params=params)
+        Requests().delete(url=url, headers=self.headers, params=params)
 
-        if response.status_code == 200:
-            return f"Position {symbol_or_id} has been closed"
-        else:
-            res = json.loads(response.text)
-            raise Exception(f'Failed to close position. Response: {res["message"]}')
+        return f"Position {symbol_or_id} has been closed"
```

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/screener.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from typing import Dict
 
 import pandas as pd
 import pendulum
-import requests
 
 from .asset import Asset
 from .market import Market
+from .requests import Requests
 
 
 class Screener:
     def __init__(
         self,
         data_url: str,
         headers: Dict[str, str],
@@ -186,61 +186,58 @@
             "end": end,
             "feed": "sip",
             "currency": "USD",
             "page_token": "",
             "sort": "asc",
         }
 
-        response = requests.get(url, headers=self.headers, params=params)
+        request = Requests().get(url=url, headers=self.headers, params=params)
 
-        if response.status_code == 200:
-            res = json.loads(response.text)
+        res = json.loads(request.text)
 
-            bars_df = pd.DataFrame.from_dict(res["bars"], orient="index")
+        bars_df = pd.DataFrame.from_dict(res["bars"], orient="index")
+        page_token = res["next_page_token"]
+
+        while page_token:
+            params["page_token"] = page_token
+            request = Requests().get(url=url, headers=self.headers, params=params)
+            res = json.loads(request.text)
+            bars_df = pd.concat(
+                [
+                    bars_df,
+                    pd.DataFrame.from_dict(res["bars"], orient="index"),
+                ]
+            )
             page_token = res["next_page_token"]
 
-            while page_token:
-                params["page_token"] = page_token
-                response = requests.get(url, headers=self.headers, params=params)
-                res = json.loads(response.text)
-                bars_df = pd.concat(
-                    [
-                        bars_df,
-                        pd.DataFrame.from_dict(res["bars"], orient="index"),
-                    ]
-                )
-                page_token = res["next_page_token"]
+        bars_df.reset_index()
 
-            bars_df.reset_index()
+        all_bars_df = pd.DataFrame()
 
-            all_bars_df = pd.DataFrame()
+        for bar in bars_df.iterrows():
+            try:
+                change = round(
+                    ((bar[1][1]["c"] - bar[1][0]["c"]) / bar[1][0]["c"]) * 100,
+                    2,
+                )
+                symbol = bar[0]
 
-            for bar in bars_df.iterrows():
-                try:
-                    change = round(
-                        ((bar[1][1]["c"] - bar[1][0]["c"]) / bar[1][0]["c"]) * 100,
-                        2,
-                    )
-                    symbol = bar[0]
-
-                    sym_data = {
-                        "symbol": symbol,
-                        "change": change,
-                        "price": bar[1][1]["c"],
-                        "volume": bar[1][1]["v"],
-                        "trades": bar[1][1]["n"],
-                    }
-                    all_bars_df = pd.concat([all_bars_df, pd.DataFrame([sym_data])])
-
-                except TypeError or KeyError:
-                    pass
-            all_bars_df.reset_index(drop=True, inplace=True)
-            return all_bars_df
-        else:
-            raise ValueError(f"Failed to get assets. Response: {response.text}")
+                sym_data = {
+                    "symbol": symbol,
+                    "change": change,
+                    "price": bar[1][1]["c"],
+                    "volume": bar[1][1]["v"],
+                    "trades": bar[1][1]["n"],
+                }
+                all_bars_df = pd.concat([all_bars_df, pd.DataFrame([sym_data])])
+
+            except TypeError or KeyError:
+                pass
+        all_bars_df.reset_index(drop=True, inplace=True)
+        return all_bars_df
 
     ##################################################
     # ///////////////// Set Dates \\\\\\\\\\\\\\\\\\ #
     ##################################################
     def set_dates(self):
         """
         Sets the dates for the screener.
@@ -256,11 +253,12 @@
         calender = (
             self.market.calender(
                 start_date=today.subtract(days=7).format("YYYY-MM-DD"),
                 end_date=today.subtract(days=1).format("YYYY-MM-DD"),
             )
             .tail(2)
             .reset_index(drop=True)
+            .sort_values(by="date", ascending=True)
         )
 
         self.yesterday = calender.iloc[1]["date"].strftime("%Y-%m-%d")
         self.day_before_yesterday = calender.iloc[0]["date"].strftime("%Y-%m-%d")
```

### Comparing `py_alpaca_api-0.6.3/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.6.4/py_alpaca_api/src/watchlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from typing import Dict, Union
 
-import requests
-
 from .data_classes import WatchlistClass, watchlist_class_from_dict
+from .requests import Requests
 
 
 class Watchlist:
     def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
         """
         Initialize a Watchlist object.
 
@@ -57,27 +56,25 @@
 
         Returns:
             dict: The response data as a dictionary.
 
         Raises:
             Exception: If the response status code is not 200 or 204.
         """
-        response = requests.request(
+        request = Requests().request(
             method=method,
             url=url,
             headers=self.headers,
             json=payload,
             params=params,
         )
-        if response.status_code in {200, 204}:
-            if response.text:
-                return json.loads(response.text)
-            return {}
-        else:
-            raise Exception(response.text)
+
+        if request.text:
+            return json.loads(request.text)
+        return {}
 
     ########################################################
     # //////////////// Get a  watchlist ///////////////////#
     ########################################################
     def get(self, watchlist_id: str = None, watchlist_name: str = None) -> WatchlistClass:
         """
         Retrieves a watchlist based on the provided watchlist ID or name.
@@ -116,25 +113,23 @@
         Returns:
             A list of WatchlistClass objects representing all the watchlists.
 
         Raises:
             Exception: If the API request fails.
         """
         url = f"{self.trade_url}/watchlists"
-        response = requests.get(url, headers=self.headers)
-        res = json.loads(response.text)
+        request = Requests().get(url, headers=self.headers)
+
+        response = json.loads(request.text)
 
         watchlists = []
-        if response.status_code == 200:
-            if res:
-                for watchlist in res:
-                    watchlists.append(self.get(watchlist_id=watchlist["id"]))
-            return watchlists
-        else:
-            raise Exception(response.text)
+        if response:
+            for watchlist in response:
+                watchlists.append(self.get(watchlist_id=watchlist["id"]))
+        return watchlists
 
     ########################################################
     # ///////////// Create a new watchlist ////////////////#
     ########################################################
     def create(self, name: str, symbols: Union[list, str] = None) -> WatchlistClass:
         """
         Creates a new watchlist with the given name and symbols.
```

### Comparing `py_alpaca_api-0.6.3/pyproject.toml` & `py_alpaca_api-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.6.3"
+version = "0.6.4"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.6.3/PKG-INFO` & `py_alpaca_api-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

