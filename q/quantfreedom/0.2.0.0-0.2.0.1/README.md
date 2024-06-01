# Comparing `tmp/quantfreedom-0.2.0.0.tar.gz` & `tmp/quantfreedom-0.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfreedom-0.2.0.0.tar", max compression
+gzip compressed data, was "quantfreedom-0.2.0.1.tar", max compression
```

## Comparing `quantfreedom-0.2.0.0.tar` & `quantfreedom-0.2.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11558 2023-12-05 17:44:20.643060 quantfreedom-0.2.0.0/LICENSE
--rw-r--r--   0        0        0     2134 2024-05-19 15:27:32.666161 quantfreedom-0.2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1363 2024-05-19 14:11:30.926838 quantfreedom-0.2.0.0/quantfreedom/__init__.py
--rw-r--r--   0        0        0      222 2024-05-16 14:35:07.370622 quantfreedom-0.2.0.0/quantfreedom/backtesters/__init__.py
--rw-r--r--   0        0        0    11920 2024-05-22 16:37:44.092927 quantfreedom-0.2.0.0/quantfreedom/backtesters/bt_live.py
--rw-r--r--   0        0        0    26622 2024-05-22 16:38:16.972085 quantfreedom-0.2.0.0/quantfreedom/backtesters/bt_regular.py
--rw-r--r--   0        0        0        0 2024-05-05 13:17:05.091942 quantfreedom-0.2.0.0/quantfreedom/core/__init__.py
--rw-r--r--   0        0        0    12777 2024-05-19 14:11:08.879829 quantfreedom-0.2.0.0/quantfreedom/core/enums.py
--rw-r--r--   0        0        0    21711 2024-05-17 14:31:43.097467 quantfreedom-0.2.0.0/quantfreedom/core/plotting_base.py
--rw-r--r--   0        0        0    11179 2024-05-22 15:39:50.177126 quantfreedom-0.2.0.0/quantfreedom/core/strategy.py
--rw-r--r--   0        0        0      294 2024-05-14 13:37:33.155122 quantfreedom-0.2.0.0/quantfreedom/exchanges/__init__.py
--rw-r--r--   0        0        0     6099 2024-05-19 14:14:16.992505 quantfreedom-0.2.0.0/quantfreedom/exchanges/binance_usdm.py
--rw-r--r--   0        0        0    38437 2024-05-14 16:11:25.497110 quantfreedom-0.2.0.0/quantfreedom/exchanges/bybit.py
--rw-r--r--   0        0        0     6870 2024-05-16 19:00:06.369046 quantfreedom-0.2.0.0/quantfreedom/exchanges/exchange.py
--rw-r--r--   0        0        0    41125 2024-05-06 16:11:37.496638 quantfreedom-0.2.0.0/quantfreedom/exchanges/mufex.py
--rw-r--r--   0        0        0        0 2024-05-05 13:45:24.956684 quantfreedom-0.2.0.0/quantfreedom/helpers/__init__.py
--rw-r--r--   0        0        0     7914 2024-05-05 13:17:05.095785 quantfreedom-0.2.0.0/quantfreedom/helpers/bsc_scan.py
--rw-r--r--   0        0        0     2078 2024-05-15 14:15:07.568687 quantfreedom-0.2.0.0/quantfreedom/helpers/custom_logger.py
--rw-r--r--   0        0        0     2687 2024-05-17 15:07:48.934089 quantfreedom-0.2.0.0/quantfreedom/helpers/email_sender.py
--rw-r--r--   0        0        0    12014 2024-05-24 16:31:44.154454 quantfreedom-0.2.0.0/quantfreedom/helpers/helper_funcs.py
--rw-r--r--   0        0        0     3794 2024-05-17 15:07:55.283120 quantfreedom-0.2.0.0/quantfreedom/helpers/utils.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.699807 quantfreedom-0.2.0.0/quantfreedom/indicators/__init__.py
--rw-r--r--   0        0        0    22925 2024-05-22 14:26:53.128699 quantfreedom-0.2.0.0/quantfreedom/indicators/tv_indicators.py
--rw-r--r--   0        0        0        0 2023-12-05 17:44:20.704775 quantfreedom-0.2.0.0/quantfreedom/order_handler/__init__.py
--rw-r--r--   0        0        0    28538 2024-05-19 14:14:54.910441 quantfreedom-0.2.0.0/quantfreedom/order_handler/increase_position.py
--rw-r--r--   0        0        0     9848 2024-05-17 15:08:35.463005 quantfreedom-0.2.0.0/quantfreedom/order_handler/leverage.py
--rw-r--r--   0        0        0    17107 2024-05-17 15:08:53.075942 quantfreedom-0.2.0.0/quantfreedom/order_handler/order.py
--rw-r--r--   0        0        0    10626 2024-05-17 15:08:55.366393 quantfreedom-0.2.0.0/quantfreedom/order_handler/stop_loss.py
--rw-r--r--   0        0        0     5671 2024-05-17 15:08:56.215120 quantfreedom-0.2.0.0/quantfreedom/order_handler/take_profit.py
--rw-r--r--   0        0        0      203 2024-04-04 19:41:17.532684 quantfreedom-0.2.0.0/README.md
--rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 quantfreedom-0.2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-12-05 17:44:20.643060 quantfreedom-0.2.0.1/LICENSE
+-rw-r--r--   0        0        0     2136 2024-06-01 19:22:50.808165 quantfreedom-0.2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1363 2024-05-24 18:22:01.689363 quantfreedom-0.2.0.1/quantfreedom/__init__.py
+-rw-r--r--   0        0        0      222 2024-05-24 18:22:01.690361 quantfreedom-0.2.0.1/quantfreedom/backtesters/__init__.py
+-rw-r--r--   0        0        0    11920 2024-05-24 18:22:01.691364 quantfreedom-0.2.0.1/quantfreedom/backtesters/bt_live.py
+-rw-r--r--   0        0        0    27589 2024-06-01 14:44:59.014989 quantfreedom-0.2.0.1/quantfreedom/backtesters/bt_regular.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:22:01.691364 quantfreedom-0.2.0.1/quantfreedom/core/__init__.py
+-rw-r--r--   0        0        0    12969 2024-05-27 19:09:21.252998 quantfreedom-0.2.0.1/quantfreedom/core/enums.py
+-rw-r--r--   0        0        0    21711 2024-05-24 18:22:01.693361 quantfreedom-0.2.0.1/quantfreedom/core/plotting_base.py
+-rw-r--r--   0        0        0    11443 2024-05-27 19:09:21.253974 quantfreedom-0.2.0.1/quantfreedom/core/strategy.py
+-rw-r--r--   0        0        0      294 2024-05-24 18:22:01.693361 quantfreedom-0.2.0.1/quantfreedom/exchanges/__init__.py
+-rw-r--r--   0        0        0     6099 2024-05-24 18:22:01.694361 quantfreedom-0.2.0.1/quantfreedom/exchanges/binance_usdm.py
+-rw-r--r--   0        0        0    38437 2024-06-01 14:09:05.800700 quantfreedom-0.2.0.1/quantfreedom/exchanges/bybit.py
+-rw-r--r--   0        0        0     6870 2024-05-24 18:22:01.695361 quantfreedom-0.2.0.1/quantfreedom/exchanges/exchange.py
+-rw-r--r--   0        0        0    41144 2024-06-01 14:08:52.651575 quantfreedom-0.2.0.1/quantfreedom/exchanges/mufex.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:22:01.696361 quantfreedom-0.2.0.1/quantfreedom/helpers/__init__.py
+-rw-r--r--   0        0        0     7914 2024-05-24 18:22:01.697362 quantfreedom-0.2.0.1/quantfreedom/helpers/bsc_scan.py
+-rw-r--r--   0        0        0     2078 2024-05-24 18:22:01.697362 quantfreedom-0.2.0.1/quantfreedom/helpers/custom_logger.py
+-rw-r--r--   0        0        0     2687 2024-05-24 18:22:01.698361 quantfreedom-0.2.0.1/quantfreedom/helpers/email_sender.py
+-rw-r--r--   0        0        0    12014 2024-05-24 20:38:00.847760 quantfreedom-0.2.0.1/quantfreedom/helpers/helper_funcs.py
+-rw-r--r--   0        0        0     3794 2024-05-24 18:22:01.699361 quantfreedom-0.2.0.1/quantfreedom/helpers/utils.py
+-rw-r--r--   0        0        0        0 2023-12-05 17:44:20.699807 quantfreedom-0.2.0.1/quantfreedom/indicators/__init__.py
+-rw-r--r--   0        0        0    22925 2024-05-24 18:22:01.699361 quantfreedom-0.2.0.1/quantfreedom/indicators/tv_indicators.py
+-rw-r--r--   0        0        0        0 2023-12-05 17:44:20.704775 quantfreedom-0.2.0.1/quantfreedom/order_handler/__init__.py
+-rw-r--r--   0        0        0    28538 2024-05-24 18:22:01.700362 quantfreedom-0.2.0.1/quantfreedom/order_handler/increase_position.py
+-rw-r--r--   0        0        0     9848 2024-05-24 18:22:01.701362 quantfreedom-0.2.0.1/quantfreedom/order_handler/leverage.py
+-rw-r--r--   0        0        0    17131 2024-05-27 19:09:21.253974 quantfreedom-0.2.0.1/quantfreedom/order_handler/order.py
+-rw-r--r--   0        0        0    13829 2024-05-27 19:09:21.254974 quantfreedom-0.2.0.1/quantfreedom/order_handler/stop_loss.py
+-rw-r--r--   0        0        0     5671 2024-05-24 18:22:01.702362 quantfreedom-0.2.0.1/quantfreedom/order_handler/take_profit.py
+-rw-r--r--   0        0        0      203 2024-04-04 19:41:17.532684 quantfreedom-0.2.0.1/README.md
+-rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 quantfreedom-0.2.0.1/PKG-INFO
```

### Comparing `quantfreedom-0.2.0.0/LICENSE` & `quantfreedom-0.2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/pyproject.toml` & `quantfreedom-0.2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 [tool.poetry]
 name = "quantfreedom"
-version = "0.2.0.0"
-description = "I don't want to put a description here So I wont"
+version = "0.2.0.1"
+description = "I don't want to put a description here, so I wont"
 authors = ["Neo <quantfreedom1022@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-dash = "2.9.1"
-dash-bootstrap-templates = "1.1.1"
-ipykernel = "6.25.0"
-ipywidgets = "8.1.1"
+dash = "2.17.0"
+dash-bootstrap-templates = "1.1.2"
+ipykernel = "6.29.4"
+ipywidgets = "8.1.3"
 jupyter-dash = "0.4.2"
-notebook = "6.5.6"
-numba = "0.58.1"
-numpy = "1.26.1"
-pandas = "2.1.1"
-plotly = "5.17.0"
+notebook = "7.2.0"
+numpy = "1.26.4"
+pandas = "2.2.2"
+plotly = "5.22.0"
+poetry = "1.8.3"
 tables = "3.9.2"
 kaleido = [
 {version="0.1.0.post1", markers="sys_platform == 'win32'", source = "pypi"},
 {version="0.2.1", markers="sys_platform == 'darwin'", source = "pypi"},
 {version="0.2.1", markers="sys_platform == 'linux'", source = "pypi"},
 ]
 
-aws-cdk-lib = { version = "2.139.0", optional = true }
-bcrypt = {version = "4.1.2", optional = true}
-cryptography = {version = "42.0.5", optional = true}
-fastapi = { version = "0.110.0", optional = true }
+aws-cdk-lib = { version = "2.143.0", optional = true }
+bcrypt = {version = "4.1.3", optional = true}
+cryptography = {version = "42.0.7", optional = true}
+fastapi = { version = "0.111.0", optional = true }
 httpx = { version = "0.27.0", optional = true }
 mangum = { version = "0.17.0", optional = true }
-mysql-connector-python = { version = "8.3.0", optional = true }
+mysql-connector-python = { version = "8.4.0", optional = true }
 pyjwt = {version = "2.8.0", optional = true}
-uvicorn = { version = "0.29.0", optional = true}
+uvicorn = { version = "0.30.0", optional = true}
 
-griffe = { version = "0.38.0", optional = true }
-mkdocs = { version = "1.5.3", optional = true }
-mkdocstrings = {version = "0.24.0", optional = true, extras = ["python"]}
+griffe = { version = "0.45.2", optional = true }
+mkdocs = { version = "1.6.0", optional = true }
 mkdocs-gen-files = { version = "0.5.0", optional = true }
 mkdocs-literate-nav = {version = "0.6.1", optional = true}
-mkdocs-material = { version = "9.4.14", optional = true }
+mkdocs-material = { version = "9.5.25", optional = true }
 mkdocs-open-in-new-tab = { version = "1.0.3", optional = true }
 mkdocs-redirects = { version = "1.2.1", optional = true }
+mkdocstrings = {version = "0.25.1", optional = true, extras = ["python"]}
 python-multipart = {version = "0.0.9", optional = true}
 
 [tool.poetry.extras]
 dev = ["aws-cdk-lib", "bcrypt", "cryptography", "fastapi", "httpx", "mangum", "mysql-connector-python", "pyjwt", "uvicorn"]
-docs = ["griffe", "mkdocs", "mkdocstrings", "mkdocs-gen-files", "mkdocs-literate-nav", "mkdocs-material", "mkdocs-open-in-new-tab", "mkdocs-redirects", "python-multipart"]
+docs = ["griffe", "mkdocs", "mkdocs-gen-files", "mkdocs-literate-nav", "mkdocs-material", "mkdocs-open-in-new-tab", "mkdocs-redirects", "mkdocstrings", "python-multipart"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `quantfreedom-0.2.0.0/quantfreedom/__init__.py` & `quantfreedom-0.2.0.1/quantfreedom/__init__.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/backtesters/bt_live.py` & `quantfreedom-0.2.0.1/quantfreedom/backtesters/bt_live.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/backtesters/bt_regular.py` & `quantfreedom-0.2.0.1/quantfreedom/backtesters/bt_regular.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from quantfreedom.core.enums import (
     CurrentFootprintCandleTuple,
     DecreasePosition,
     FootprintCandlesTuple,
     OrderStatus,
     RejectedOrder,
     or_dt,
+    TrailingSLStrategyType,
 )
 from quantfreedom.helpers.utils import pretty_qf
 
 logger = getLogger()
 
 
 def run_df_backtest(
@@ -45,14 +46,16 @@
     # Creating Settings Vars
     total_bars = candles.candle_open_timestamps.size
     step_by_settings = strategy.total_filtered_settings // step_by
     chunk_process = step_by_settings // threads
 
     print("Starting the backtest now ... and also here are some stats for your backtest.")
 
+    # TODO total settings combinations to test is wrong because we need to take into account the filtering in creating dos tuple
+
     print("\n" + f"Total threads to use: {threads:,}")
     print(f"Total indicator settings to test: {strategy.total_indicator_settings:,}")
     print(f"Total order settings to test: {strategy.total_order_settings:,}")
     print(f"Total settings combinations to test: {strategy.total_order_settings * strategy.total_indicator_settings:,}")
     print(f"Total settings combination to test after filtering: {strategy.total_filtered_settings:,}")
     print(f"Total settings combination with step by: {step_by_settings:,}")
     print(f"Total settings combination to process per chunk: {chunk_process:,}")
@@ -93,18 +96,21 @@
             ],
             callback=proc_results,
             error_callback=handler,
         )
         results.append(r)
 
     print("\n" + "looping through results")
-    for r in results:
+    for idx, r in enumerate(results):
+        print(idx, end=", ")
         r.wait()
 
+    print("\n" + "closing")
     p.close()
+    print("joining")
     p.join()
     print("creating datafram")
 
     backtest_df = make_bt_df(
         strategy=strategy,
         strategy_result_records=strategy_result_records,
     )
@@ -160,14 +166,15 @@
             logger.debug(
                 f"set_idx= {strategy.cur_dos_tuple.settings_index} loop_idx = {set_idx} bar_idx= {bar_index} datetime= {candles.candle_open_datetimes[bar_index]}"
             )
 
             if order.position_size_usd > 0:
                 try:
                     current_candle = CurrentFootprintCandleTuple(
+                        open_timestamp=candles.candle_open_timestamps[bar_index],
                         open_price=candles.candle_open_prices[bar_index],
                         high_price=candles.candle_high_prices[bar_index],
                         low_price=candles.candle_low_prices[bar_index],
                         close_price=candles.candle_close_prices[bar_index],
                     )
                     logger.debug("Checking stop loss hit")
                     order.check_stop_loss_hit(
@@ -216,14 +223,17 @@
                     pnl_array[filled_pnl_counter] = realized_pnl
                     filled_pnl_counter += 1
                     total_fees_paid += fees_paid
                     logger.debug("Filled pnl array and updated total fees paid")
 
                     order.set_order_variables(equity=equity)
                     logger.debug("reset order variables")
+                    if strategy.static_os_tuple.trailing_sl_strategy_type == TrailingSLStrategyType.PctAboveBelow:
+                        order.obj_stop_loss.checker_tsl = order.obj_stop_loss.init_check_move_tsl_pct
+                        logger.debug("reset checker_tsl to init_check_move_tsl_pct")
 
                 except Exception as e:
                     logger.error(f"Exception checking sl liq tp and move -> {e}")
                     raise Exception(f"Exception checking sl liq tp  and move -> {e}")
             else:
                 logger.debug("Not in a pos so not checking SL Liq or TP")
 
@@ -366,14 +376,15 @@
                         + strategy.cur_ind_set_tuple
                     )
                     record_results[rec_idx] = tuple_results
                     rec_idx += 1
         logger.debug(
             f"Starting New Loop\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n"
         )
+
     return range_start, range_end, record_results
 
 
 def proc_results(
     results: tuple,
 ):
     start = results[0]
@@ -534,14 +545,18 @@
                     realized_pnl=realized_pnl,
                 )
                 or_filled += 1
                 logger.debug(f"Filled decrease postiion order records for {OrderStatus._fields[e.order_status]}")
 
                 order.set_order_variables(equity=equity)
                 logger.debug("reset order variables")
+                
+                if strategy.static_os_tuple.trailing_sl_strategy_type == TrailingSLStrategyType.PctAboveBelow:
+                        order.obj_stop_loss.checker_tsl = order.obj_stop_loss.init_check_move_tsl_pct
+                        logger.debug("reset checker_tsl to init_check_move_tsl_pct")
 
             except Exception as e:
                 logger.error(f"Exception checking sl liq tp and move -> {e}")
                 raise Exception(f"Exception checking sl liq tp and move -> {e}")
         else:
             logger.debug("Not in a pos so not checking SL Liq or TP")
```

### Comparing `quantfreedom-0.2.0.0/quantfreedom/core/enums.py` & `quantfreedom-0.2.0.1/quantfreedom/core/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,23 @@
     Nothing: int = 0
     SLBasedOnCandleBody: int = 1
 
 
 StopLossStrategyType = StopLossStrategyTypeT()
 
 
+class TrailingSLStrategyTypeT(NamedTuple):
+    Nothing: int = 0
+    CBAboveBelow: int = 1
+    PctAboveBelow: int = 2
+
+
+TrailingSLStrategyType = TrailingSLStrategyTypeT()
+
+
 class TakeProfitStrategyTypeT(NamedTuple):
     """
     How you want to process the take profit
 
     Parameters
     ----------
     RiskReward : int = 0
@@ -310,21 +319,21 @@
 
 
 class StaticOrderSettings(NamedTuple):
     increase_position_type: int
     leverage_strategy_type: int
     pg_min_max_sl_bcb: str
     sl_strategy_type: int
+    trailing_sl_strategy_type: int
     sl_to_be_bool: bool
     starting_bar: int
     starting_equity: float
     static_leverage: float
     tp_fee_type: str
     tp_strategy_type: int
-    trail_sl_bool: bool
     z_or_e_type: str
 
 
 class RejectedOrder(Exception):
     def __init__(
         self,
         msg: str = None,
```

### Comparing `quantfreedom-0.2.0.0/quantfreedom/core/plotting_base.py` & `quantfreedom-0.2.0.1/quantfreedom/core/plotting_base.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/core/strategy.py` & `quantfreedom-0.2.0.1/quantfreedom/core/strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,23 @@
         for k in range(len(the_tuple) - 2, -1, -1):
             array_size *= the_tuple[k].size
             m = int(array_size / the_tuple[k].size)
             for j in range(1, the_tuple[k].size):
                 cart_prod_array[j * m : (j + 1) * m, k + 1 :] = cart_prod_array[0:m, k + 1 :]
 
         logger.debug("cart_prod_array")
-        return cart_prod_array.T
+        trail_sl_by_pct = 9
+        trail_sl_when_pct = 10
+        cart_prod_array = cart_prod_array.T
+
+        filter_tf = cart_prod_array[trail_sl_when_pct] > cart_prod_array[trail_sl_by_pct]
+
+        filtered_cart_prod = cart_prod_array[:, filter_tf]
+
+        return filtered_cart_prod
 
     def get_og_dos_tuple(
         self,
         final_cart_prod_array: np.ndarray,
     ) -> DynamicOrderSettings:
 
         dos_tuple = DynamicOrderSettings(*tuple(final_cart_prod_array[:12]))
```

### Comparing `quantfreedom-0.2.0.0/quantfreedom/exchanges/binance_usdm.py` & `quantfreedom-0.2.0.1/quantfreedom/exchanges/binance_usdm.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/exchanges/bybit.py` & `quantfreedom-0.2.0.1/quantfreedom/exchanges/bybit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -743,24 +743,24 @@
             else:
                 raise Exception
         except Exception as e:
             raise Exception(f"bybit adjust_order message = {response['retMsg']} -> {e}")
 
     def move_stop_order(
         self,
-        symbol: str,
-        order_id: str,
-        new_price: float,
         asset_size: float,
+        new_price: float,
+        order_id: str,
+        symbol: str,
     ):
         return self.adjust_order(
+            asset_size=asset_size,
             symbol=symbol,
             order_id=order_id,
             triggerPrice=new_price,
-            asset_size=asset_size,
         )
 
     def get_risk_limit_info(
         self,
         symbol: str,
         category: str = "linear",
     ):
```

### Comparing `quantfreedom-0.2.0.0/quantfreedom/exchanges/exchange.py` & `quantfreedom-0.2.0.1/quantfreedom/exchanges/exchange.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/exchanges/mufex.py` & `quantfreedom-0.2.0.1/quantfreedom/exchanges/mufex.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,18 +666,18 @@
         params["orderId"] = order_id
         params["qty"] = str(asset_size)
         params["price"] = str(new_price)
         return self.adjust_order(params=params)
 
     def move_stop_order(
         self,
-        symbol: str,
-        order_id: str,
-        new_price: float,
         asset_size: float,
+        new_price: float,
+        order_id: str,
+        symbol: str,
     ):
         params = {}
         params["symbol"] = symbol
         params["orderId"] = order_id
         params["qty"] = str(asset_size)
         params["triggerPrice"] = str(new_price)
         return self.adjust_order(params=params)
@@ -916,15 +916,15 @@
         )
 
     def set_and_get_exchange_settings_tuple(
         self,
         leverage_mode: LeverageModeType,  # type: ignore
         position_mode: PositionModeType,  # type: ignore
         symbol: str,
-    ):
+    )-> ExchangeSettings:
         self.position_mode = position_mode
         if position_mode == PositionModeType.HedgeMode:
             self.set_position_mode_as_hedge_mode(symbol=symbol)
         else:
             self.set_position_mode_as_one_way_mode(symbol=symbol)
 
         if leverage_mode == LeverageModeType.Isolated:
```

### Comparing `quantfreedom-0.2.0.0/quantfreedom/helpers/bsc_scan.py` & `quantfreedom-0.2.0.1/quantfreedom/helpers/bsc_scan.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/helpers/custom_logger.py` & `quantfreedom-0.2.0.1/quantfreedom/helpers/custom_logger.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/helpers/email_sender.py` & `quantfreedom-0.2.0.1/quantfreedom/helpers/email_sender.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/helpers/helper_funcs.py` & `quantfreedom-0.2.0.1/quantfreedom/helpers/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/helpers/utils.py` & `quantfreedom-0.2.0.1/quantfreedom/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/indicators/tv_indicators.py` & `quantfreedom-0.2.0.1/quantfreedom/indicators/tv_indicators.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/order_handler/increase_position.py` & `quantfreedom-0.2.0.1/quantfreedom/order_handler/increase_position.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/order_handler/leverage.py` & `quantfreedom-0.2.0.1/quantfreedom/order_handler/leverage.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/quantfreedom/order_handler/order.py` & `quantfreedom-0.2.0.1/quantfreedom/order_handler/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
         self.obj_stop_loss = StopLoss(
             long_short=long_short,
             market_fee_pct=exchange_settings_tuple.market_fee_pct,
             pg_min_max_sl_bcb=static_os_tuple.pg_min_max_sl_bcb,
             price_tick_step=exchange_settings_tuple.price_tick_step,
             sl_strategy_type=static_os_tuple.sl_strategy_type,
+            trailing_sl_strategy_type=static_os_tuple.trailing_sl_strategy_type,
             sl_to_be_bool=static_os_tuple.sl_to_be_bool,
-            trail_sl_bool=static_os_tuple.trail_sl_bool,
             z_or_e_type=static_os_tuple.z_or_e_type,
         )
         self.obj_inc_pos = IncreasePosition(
             asset_tick_step=exchange_settings_tuple.asset_tick_step,
             increase_position_type=static_os_tuple.increase_position_type,
             long_short=long_short,
             market_fee_pct=exchange_settings_tuple.market_fee_pct,
```

### Comparing `quantfreedom-0.2.0.0/quantfreedom/order_handler/stop_loss.py` & `quantfreedom-0.2.0.1/quantfreedom/order_handler/stop_loss.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 from logging import getLogger
 
 from quantfreedom.helpers.helper_funcs import round_size_by_tick_step
 from quantfreedom.core.enums import (
-    CandleBodyType,
     CurrentFootprintCandleTuple,
     DecreasePosition,
     FootprintCandlesTuple,
     OrderStatus,
     StopLossStrategyType,
+    TrailingSLStrategyType,
 )
 
 logger = getLogger()
 
 
 class StopLoss:
     sl_based_on_add_pct: float
@@ -26,32 +26,32 @@
 
     def __init__(
         self,
         long_short: str,
         market_fee_pct: float,
         pg_min_max_sl_bcb: str,
         price_tick_step: float,
-        sl_strategy_type: StopLossStrategyType,  # type: ignore
+        sl_strategy_type: int,
+        trailing_sl_strategy_type: int,
         sl_to_be_bool: bool,
-        trail_sl_bool: bool,
         z_or_e_type: str,
     ) -> None:
         self.market_fee_pct = market_fee_pct
         self.price_tick_step = price_tick_step
 
         if long_short.lower() == "long":
             self.sl_to_zero_price = self.long_sl_to_zero_price
             self.get_sl_hit = self.long_sl_hit_bool
             self.move_sl_bool = self.num_greater_than_num
-            self.sl_price_calc = self.long_sl_price_calc
+            self.sl_price_calc = self.decrease_sl_price
         elif long_short.lower() == "short":
             self.sl_to_zero_price = self.short_sl_to_zero_price
             self.get_sl_hit = self.short_sl_hit_bool
             self.move_sl_bool = self.num_less_than_num
-            self.sl_price_calc = self.short_sl_price_calc
+            self.sl_price_calc = self.increase_sl_price
         else:
             raise Exception("long or short are the only options for long_short")
 
         # stop loss calulator
         if sl_strategy_type == StopLossStrategyType.SLBasedOnCandleBody:
             self.sl_calculator = self.sl_based_on_candle_body
             self.checker_sl_hit = self.check_sl_hit
@@ -76,29 +76,44 @@
             else:
                 raise Exception("zero or entry are the only options for z_or_e_type")
         else:
             self.checker_sl_to_be = self.pass_func
             self.zero_or_entry_calc = self.pass_func
 
         # Trailing stop loss
-        if trail_sl_bool:
-            self.checker_tsl = self.check_move_tsl
+        if trailing_sl_strategy_type == TrailingSLStrategyType.CBAboveBelow:
+            self.checker_tsl = self.check_move_tsl_close
+        elif trailing_sl_strategy_type == TrailingSLStrategyType.PctAboveBelow:
+            self.checker_tsl = self.init_check_move_tsl_pct
+            if long_short.lower() == "long":
+                self.tsl_mover = self.increase_sl_price
+            else:
+                pass
+
         else:
             self.checker_tsl = self.pass_func
 
-    # Long Functions
+    def decrease_sl_price(
+        self,
+        price: float,
+        add_pct: float,
+    ):
+        sl_price = price - (price * add_pct)
+        return sl_price
 
-    def long_sl_price_calc(
+    def increase_sl_price(
         self,
-        candle_body: float,
+        price: float,
         add_pct: float,
     ):
-        sl_price = candle_body - (candle_body * add_pct)
+        sl_price = price + (price * add_pct)
         return sl_price
 
+    # Long Functions
+
     def long_sl_hit_bool(
         self,
         current_candle: CurrentFootprintCandleTuple,
         sl_price: float,
     ):
         logger.debug("Starting")
         candle_low = current_candle.low_price
@@ -120,22 +135,14 @@
         sl_price: float,
     ):
         logger.debug("Starting")
         candle_high = current_candle.high_price
         logger.debug(f"candle_high= {candle_high}")
         return sl_price < candle_high
 
-    def short_sl_price_calc(
-        self,
-        candle_body: float,
-        add_pct: float,
-    ):
-        sl_price = candle_body + (candle_body * add_pct)
-        return sl_price
-
     def short_sl_to_zero_price(
         self,
         average_entry: float,
     ):
         numerator = average_entry - self.market_fee_pct * average_entry
         denominator = 1 + self.market_fee_pct
         sl_price = numerator / denominator
@@ -186,15 +193,15 @@
             candles=candles,
             candle_body_type=self.sl_bcb_type,
             lookback=lookback,
         )
         logger.debug(f"candle_body= {candle_body}")
 
         sl_price = self.sl_price_calc(
-            candle_body=candle_body,
+            price=candle_body,
             add_pct=self.sl_based_on_add_pct,
         )
         sl_price = round_size_by_tick_step(
             user_num=sl_price,
             exchange_num=self.price_tick_step,
         )
         logger.debug(f"sl_price= {sl_price}")
@@ -246,30 +253,37 @@
             else:
                 logger.debug("not moving sl to be")
                 return None, None
         else:
             logger.debug("can't move sl to be")
             return None, None
 
-    def check_move_tsl(
+    def check_move_tsl_close(
         self,
         average_entry: float,
         current_candle: CurrentFootprintCandleTuple,
         sl_price: float,
     ):
         """
         Checking to see if we move the trailing stop loss
         """
         candle_body = current_candle[self.trail_sl_bcb_type]
         pct_from_ae = abs(candle_body - average_entry) / average_entry
         logger.debug(f"pct_from_ae= {round(pct_from_ae * 100, 2)}")
-        possible_move_tsl = self.move_sl_bool(num_1=pct_from_ae, num_2=self.trail_sl_when_pct)
+        possible_move_tsl = self.move_sl_bool(
+            num_1=pct_from_ae,
+            num_2=self.trail_sl_when_pct,
+        )
+
         if possible_move_tsl:
             logger.debug("Maybe move tsl")
-            temp_sl_price = self.sl_price_calc(candle_body=candle_body, add_pct=self.trail_sl_by_pct)
+            temp_sl_price = self.sl_price_calc(
+                price=candle_body,
+                add_pct=self.trail_sl_by_pct,
+            )
             temp_sl_price = round_size_by_tick_step(
                 user_num=temp_sl_price,
                 exchange_num=self.price_tick_step,
             )
             logger.debug(f"temp sl= {temp_sl_price}")
             if self.move_sl_bool(num_1=temp_sl_price, num_2=sl_price):
                 sl_pct = round(abs(average_entry - temp_sl_price) / average_entry, 2)
@@ -278,14 +292,84 @@
             else:
                 logger.debug("Wont move tsl")
                 return None, None
         else:
             logger.debug("Not moving tsl")
             return None, None
 
+    def init_check_move_tsl_pct(
+        self,
+        average_entry: float,
+        current_candle: CurrentFootprintCandleTuple,
+        sl_price: float,
+    ):
+        """
+        Checking to see if we move the trailing stop loss
+        """
+        candle_body = current_candle[self.trail_sl_bcb_type]
+        pct_from_ae = abs(candle_body - average_entry) / average_entry
+        logger.debug(f"pct_from_ae= {round(pct_from_ae * 100, 2)}")
+        possible_move_tsl = self.move_sl_bool(
+            num_1=pct_from_ae,
+            num_2=self.trail_sl_when_pct,
+        )
+
+        if possible_move_tsl:
+            logger.debug("Move tsl")
+            new_sl_price = self.tsl_mover(
+                price=average_entry,
+                add_pct=self.trail_sl_by_pct,
+            )
+            round_size_by_tick_step(
+                user_num=new_sl_price,
+                exchange_num=self.price_tick_step,
+            )
+            sl_pct = round(abs(average_entry - new_sl_price) / average_entry, 2)
+            self.checker_tsl = self.check_move_tsl_pct
+            return new_sl_price, sl_pct
+        else:
+            logger.debug("Not moving tsl")
+            return None, None
+
+    def check_move_tsl_pct(
+        self,
+        average_entry: float,
+        current_candle: CurrentFootprintCandleTuple,
+        sl_price: float,
+    ):
+        """
+        Checking to see if we move the trailing stop loss
+        """
+        candle_body = current_candle[self.trail_sl_bcb_type]
+        pct_from_sl = abs(candle_body - sl_price) / sl_price
+        logger.debug(f"pct_from_sl = {round(pct_from_sl * 100, 2)}")
+
+        possible_move_tsl = self.move_sl_bool(
+            num_1=pct_from_sl,
+            num_2=self.trail_sl_when_pct,
+        )
+
+        # TODO once possible_move_tsl is True, we don't need to check it again
+
+        if possible_move_tsl:
+            logger.debug("Move tsl")
+            new_sl_price = self.tsl_mover(
+                price=sl_price,
+                add_pct=self.trail_sl_by_pct,
+            )
+            round_size_by_tick_step(
+                user_num=new_sl_price,
+                exchange_num=self.price_tick_step,
+            )
+            sl_pct = round(abs(sl_price - new_sl_price) / sl_price, 2)
+            return new_sl_price, sl_pct
+        else:
+            logger.debug("Not moving tsl")
+            return None, None
+
     def min_price_getter(
         self,
         bar_index: int,
         candles: FootprintCandlesTuple,
         lookback: int,
         candle_body_type: int,
     ) -> float:
@@ -307,7 +391,29 @@
         return final_the_prices
 
     def pass_func(self, **kwargs):
         return None, None
 
     def sl_to_zero_price(self, **kwargs):
         pass
+
+    def checker_tsl(
+        self,
+        average_entry: float,
+        current_candle: CurrentFootprintCandleTuple,
+        sl_price: float,
+    ):
+        pass
+
+    def move_sl_bool(
+        self,
+        num1: float,
+        num2: float,
+    ):
+        pass
+
+    def sl_price_calc(
+        self,
+        price: float,
+        add_pct: float,
+    ):
+        pass
```

### Comparing `quantfreedom-0.2.0.0/quantfreedom/order_handler/take_profit.py` & `quantfreedom-0.2.0.1/quantfreedom/order_handler/take_profit.py`

 * *Files identical despite different names*

### Comparing `quantfreedom-0.2.0.0/PKG-INFO` & `quantfreedom-0.2.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 Metadata-Version: 2.1
 Name: quantfreedom
-Version: 0.2.0.0
-Summary: I don't want to put a description here So I wont
+Version: 0.2.0.1
+Summary: I don't want to put a description here, so I wont
 Author: Neo
 Author-email: quantfreedom1022@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Provides-Extra: docs
-Requires-Dist: aws-cdk-lib (==2.139.0) ; extra == "dev"
-Requires-Dist: bcrypt (==4.1.2) ; extra == "dev"
-Requires-Dist: cryptography (==42.0.5) ; extra == "dev"
-Requires-Dist: dash (==2.9.1)
-Requires-Dist: dash-bootstrap-templates (==1.1.1)
-Requires-Dist: fastapi (==0.110.0) ; extra == "dev"
-Requires-Dist: griffe (==0.38.0) ; extra == "docs"
+Requires-Dist: aws-cdk-lib (==2.143.0) ; extra == "dev"
+Requires-Dist: bcrypt (==4.1.3) ; extra == "dev"
+Requires-Dist: cryptography (==42.0.7) ; extra == "dev"
+Requires-Dist: dash (==2.17.0)
+Requires-Dist: dash-bootstrap-templates (==1.1.2)
+Requires-Dist: fastapi (==0.111.0) ; extra == "dev"
+Requires-Dist: griffe (==0.45.2) ; extra == "docs"
 Requires-Dist: httpx (==0.27.0) ; extra == "dev"
-Requires-Dist: ipykernel (==6.25.0)
-Requires-Dist: ipywidgets (==8.1.1)
+Requires-Dist: ipykernel (==6.29.4)
+Requires-Dist: ipywidgets (==8.1.3)
 Requires-Dist: jupyter-dash (==0.4.2)
 Requires-Dist: kaleido (==0.1.0.post1) ; sys_platform == "win32"
 Requires-Dist: kaleido (==0.2.1) ; sys_platform == "darwin"
 Requires-Dist: kaleido (==0.2.1) ; sys_platform == "linux"
 Requires-Dist: mangum (==0.17.0) ; extra == "dev"
-Requires-Dist: mkdocs (==1.5.3) ; extra == "docs"
+Requires-Dist: mkdocs (==1.6.0) ; extra == "docs"
 Requires-Dist: mkdocs-gen-files (==0.5.0) ; extra == "docs"
 Requires-Dist: mkdocs-literate-nav (==0.6.1) ; extra == "docs"
-Requires-Dist: mkdocs-material (==9.4.14) ; extra == "docs"
+Requires-Dist: mkdocs-material (==9.5.25) ; extra == "docs"
 Requires-Dist: mkdocs-open-in-new-tab (==1.0.3) ; extra == "docs"
 Requires-Dist: mkdocs-redirects (==1.2.1) ; extra == "docs"
-Requires-Dist: mkdocstrings[python] (==0.24.0) ; extra == "docs"
-Requires-Dist: mysql-connector-python (==8.3.0) ; extra == "dev"
-Requires-Dist: notebook (==6.5.6)
-Requires-Dist: numba (==0.58.1)
-Requires-Dist: numpy (==1.26.1)
-Requires-Dist: pandas (==2.1.1)
-Requires-Dist: plotly (==5.17.0)
+Requires-Dist: mkdocstrings[python] (==0.25.1) ; extra == "docs"
+Requires-Dist: mysql-connector-python (==8.4.0) ; extra == "dev"
+Requires-Dist: notebook (==7.2.0)
+Requires-Dist: numpy (==1.26.4)
+Requires-Dist: pandas (==2.2.2)
+Requires-Dist: plotly (==5.22.0)
+Requires-Dist: poetry (==1.8.3)
 Requires-Dist: pyjwt (==2.8.0) ; extra == "dev"
 Requires-Dist: python-multipart (==0.0.9) ; extra == "docs"
 Requires-Dist: tables (==3.9.2)
-Requires-Dist: uvicorn (==0.29.0) ; extra == "dev"
+Requires-Dist: uvicorn (==0.30.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 I am terrible at updating this readme file so please go to the website for installation instructions beyond pip install
 https://quantfreedom.github.io/QuantFreedom/
 ```
 pip install quantfreedom
 ```
```

