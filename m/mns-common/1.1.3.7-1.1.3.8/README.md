# Comparing `tmp/mns_common-1.1.3.7.tar.gz` & `tmp/mns_common-1.1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.1.3.7.tar", last modified: Fri May 31 16:10:13 2024, max compression
+gzip compressed data, was "mns_common-1.1.3.8.tar", last modified: Sat Jun  1 14:25:33 2024, max compression
```

## Comparing `mns_common-1.1.3.7.tar` & `mns_common-1.1.3.8.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.179244 mns_common-1.1.3.7/
--rw-rw-rw-   0        0        0       59 2024-05-31 16:10:13.178247 mns_common-1.1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.142343 mns_common-1.1.3.7/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.3.7/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.144338 mns_common-1.1.3.7/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.3.7/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.147330 mns_common-1.1.3.7/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.3.7/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.3.7/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.3.7/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.149324 mns_common-1.1.3.7/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.3.7/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.3.7/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.3.7/mns_common/api/em/east_money_stock_hk_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.3.7/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.150322 mns_common-1.1.3.7/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.150322 mns_common-1.1.3.7/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.3.7/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.151319 mns_common-1.1.3.7/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.152317 mns_common-1.1.3.7/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      235 2024-05-24 10:14:14.000000 mns_common-1.1.3.7/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.153314 mns_common-1.1.3.7/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.154311 mns_common-1.1.3.7/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.3.7/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.155308 mns_common-1.1.3.7/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.3.7/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.3.7/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.3.7/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.156306 mns_common-1.1.3.7/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.3.7/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.158300 mns_common-1.1.3.7/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.3.7/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.3.7/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.3.7/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.3.7/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.159298 mns_common-1.1.3.7/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.3.7/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.160295 mns_common-1.1.3.7/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.3.7/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.3.7/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.161292 mns_common-1.1.3.7/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-05-31 16:09:35.000000 mns_common-1.1.3.7/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-05-31 09:03:19.000000 mns_common-1.1.3.7/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-05-31 09:03:19.000000 mns_common-1.1.3.7/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     4896 2024-05-22 14:19:44.000000 mns_common-1.1.3.7/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.162289 mns_common-1.1.3.7/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     7992 2024-05-25 06:17:07.000000 mns_common-1.1.3.7/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.163287 mns_common-1.1.3.7/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.3.7/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9682 2024-05-31 08:28:58.000000 mns_common-1.1.3.7/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.164284 mns_common-1.1.3.7/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.3.7/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.3.7/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.165282 mns_common-1.1.3.7/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.3.7/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.3.7/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.165282 mns_common-1.1.3.7/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.166279 mns_common-1.1.3.7/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.3.7/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.3.7/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.3.7/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.167276 mns_common-1.1.3.7/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.3.7/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4770 2024-05-20 14:28:57.000000 mns_common-1.1.3.7/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.168274 mns_common-1.1.3.7/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.3.7/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.3.7/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.3.7/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.169271 mns_common-1.1.3.7/mns_common/component/qmt/
--rw-rw-rw-   0        0        0      163 2024-05-23 13:30:35.000000 mns_common-1.1.3.7/mns_common/component/qmt/__init__.py
--rw-rw-rw-   0        0        0     7540 2024-05-23 14:38:14.000000 mns_common-1.1.3.7/mns_common/component/qmt/qmt_buy_service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.170268 mns_common-1.1.3.7/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.171265 mns_common-1.1.3.7/mns_common/component/self_choose/
--rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.3.7/mns_common/component/self_choose/__init__.py
--rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.3.7/mns_common/component/self_choose/black_list_service_api.py
--rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.3.7/mns_common/component/self_choose/self_choose_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.172263 mns_common-1.1.3.7/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.3.7/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.3.7/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.173260 mns_common-1.1.3.7/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     3032 2024-05-31 09:01:38.000000 mns_common-1.1.3.7/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.174258 mns_common-1.1.3.7/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.7/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     9927 2024-05-22 08:23:47.000000 mns_common-1.1.3.7/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.175255 mns_common-1.1.3.7/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.3.7/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     2283 2024-05-24 22:26:12.000000 mns_common-1.1.3.7/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0      492 2024-05-24 09:42:58.000000 mns_common-1.1.3.7/mns_common/constant/self_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.176252 mns_common-1.1.3.7/mns_common/db/
--rw-rw-rw-   0        0        0    11520 2024-05-27 11:15:24.000000 mns_common-1.1.3.7/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.3.7/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.178247 mns_common-1.1.3.7/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.3.7/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.3.7/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.3.7/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2024-05-29 15:15:49.000000 mns_common-1.1.3.7/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.3.7/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:10:13.178247 mns_common-1.1.3.7/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-31 16:10:13.000000 mns_common-1.1.3.7/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3843 2024-05-31 16:10:13.000000 mns_common-1.1.3.7/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 16:10:13.000000 mns_common-1.1.3.7/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-31 16:10:13.000000 mns_common-1.1.3.7/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 16:10:13.179244 mns_common-1.1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-31 16:09:59.000000 mns_common-1.1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.523970 mns_common-1.1.3.8/
+-rw-rw-rw-   0        0        0       59 2024-06-01 14:25:33.522972 mns_common-1.1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.486550 mns_common-1.1.3.8/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.3.8/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.488547 mns_common-1.1.3.8/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.3.8/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.491539 mns_common-1.1.3.8/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.3.8/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.3.8/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.3.8/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.493533 mns_common-1.1.3.8/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.3.8/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.3.8/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.3.8/mns_common/api/em/east_money_stock_hk_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.3.8/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.494531 mns_common-1.1.3.8/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.494531 mns_common-1.1.3.8/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.3.8/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.495528 mns_common-1.1.3.8/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.496526 mns_common-1.1.3.8/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-05-24 10:14:14.000000 mns_common-1.1.3.8/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.497523 mns_common-1.1.3.8/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.498520 mns_common-1.1.3.8/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.3.8/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.499517 mns_common-1.1.3.8/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.3.8/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.3.8/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.3.8/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.500515 mns_common-1.1.3.8/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.3.8/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.502509 mns_common-1.1.3.8/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.3.8/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.3.8/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.3.8/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.3.8/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.503507 mns_common-1.1.3.8/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.3.8/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.504504 mns_common-1.1.3.8/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.3.8/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.3.8/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.505501 mns_common-1.1.3.8/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-05-31 16:09:35.000000 mns_common-1.1.3.8/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0     4342 2024-06-01 14:25:23.000000 mns_common-1.1.3.8/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0      736 2024-06-01 14:25:23.000000 mns_common-1.1.3.8/mns_common/component/classify/symbol_classify_param.py
+-rw-rw-rw-   0        0        0     4896 2024-05-22 14:19:44.000000 mns_common-1.1.3.8/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.506501 mns_common-1.1.3.8/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     7992 2024-05-25 06:17:07.000000 mns_common-1.1.3.8/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.507497 mns_common-1.1.3.8/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.3.8/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9682 2024-05-31 08:28:58.000000 mns_common-1.1.3.8/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.508522 mns_common-1.1.3.8/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.3.8/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.3.8/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.509491 mns_common-1.1.3.8/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.3.8/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.3.8/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.509491 mns_common-1.1.3.8/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.511485 mns_common-1.1.3.8/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.3.8/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.3.8/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.3.8/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.511485 mns_common-1.1.3.8/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.3.8/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4770 2024-05-20 14:28:57.000000 mns_common-1.1.3.8/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.513480 mns_common-1.1.3.8/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.3.8/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.3.8/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.3.8/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.513480 mns_common-1.1.3.8/mns_common/component/qmt/
+-rw-rw-rw-   0        0        0      163 2024-05-23 13:30:35.000000 mns_common-1.1.3.8/mns_common/component/qmt/__init__.py
+-rw-rw-rw-   0        0        0     7540 2024-05-23 14:38:14.000000 mns_common-1.1.3.8/mns_common/component/qmt/qmt_buy_service.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.514478 mns_common-1.1.3.8/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.515989 mns_common-1.1.3.8/mns_common/component/self_choose/
+-rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.3.8/mns_common/component/self_choose/__init__.py
+-rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.3.8/mns_common/component/self_choose/black_list_service_api.py
+-rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.3.8/mns_common/component/self_choose/self_choose_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.516989 mns_common-1.1.3.8/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.3.8/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.3.8/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.517986 mns_common-1.1.3.8/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     3032 2024-05-31 09:01:38.000000 mns_common-1.1.3.8/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.517986 mns_common-1.1.3.8/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.8/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     9927 2024-05-22 08:23:47.000000 mns_common-1.1.3.8/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.519981 mns_common-1.1.3.8/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.3.8/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     2283 2024-05-24 22:26:12.000000 mns_common-1.1.3.8/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0      492 2024-05-24 09:42:58.000000 mns_common-1.1.3.8/mns_common/constant/self_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.520978 mns_common-1.1.3.8/mns_common/db/
+-rw-rw-rw-   0        0        0    11520 2024-05-27 11:15:24.000000 mns_common-1.1.3.8/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.3.8/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.522972 mns_common-1.1.3.8/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.3.8/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.3.8/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.3.8/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2024-05-29 15:15:49.000000 mns_common-1.1.3.8/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.3.8/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:33.522972 mns_common-1.1.3.8/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-06-01 14:25:33.000000 mns_common-1.1.3.8/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3847 2024-06-01 14:25:33.000000 mns_common-1.1.3.8/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 14:25:33.000000 mns_common-1.1.3.8/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 14:25:33.000000 mns_common-1.1.3.8/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 14:25:33.523970 mns_common-1.1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-06-01 14:24:56.000000 mns_common-1.1.3.8/setup.py
```

### Comparing `mns_common-1.1.3.7/README.md` & `mns_common-1.1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/akshare/k_line_api.py` & `mns_common-1.1.3.8/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.1.3.8/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.1.3.8/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.1.3.8/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.1.3.8/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.1.3.8/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.1.3.8/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.1.3.8/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/em/east_money_stock_hk_api.py` & `mns_common-1.1.3.8/mns_common/api/em/east_money_stock_hk_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.1.3.8/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.1.3.8/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.1.3.8/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.1.3.8/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.1.3.8/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.1.3.8/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.1.3.8/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.1.3.8/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.1.3.8/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/msg/push_msg_api.py` & `mns_common-1.1.3.8/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.1.3.8/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.1.3.8/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.1.3.8/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/cache/cache_service.py` & `mns_common-1.1.3.8/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.1.3.8/mns_common/component/classify/symbol_classify_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 import os
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 16
 project_path = file_path[0:end]
 sys.path.append(project_path)
-from mns_common.component.classify.classify_constant import stock_type_param
 import mns_common.utils.data_frame_util as data_frame_util
+from mns_common.component.classify.symbol_classify_param import stock_type_classify_param
 
 
 # 深沪普通股票  选择 10cm涨幅的
 def choose_sh_symbol(realtime_quotes_now):
     return realtime_quotes_now.loc[
         (realtime_quotes_now['classification'].isin(['S', 'H']))]
 
@@ -23,88 +23,96 @@
 
 # 选择北交所的 30厘米的
 def choose_bjs_symbol(realtime_quotes_now):
     return realtime_quotes_now.loc[
         realtime_quotes_now['classification'].isin(['X'])]
 
 
-# 新上市注册股票,不限制涨幅的
-def choose_new_sub_c_symbol(realtime_quotes_now):
-    return realtime_quotes_now.loc[realtime_quotes_now['name'].str.startswith('C')]
-
-
 # 设置新股次新标记
 def set_stock_type(real_time_quotes_now_init):
     if data_frame_util.is_empty(real_time_quotes_now_init):
         return None
     real_time_quotes_now = real_time_quotes_now_init.copy()
-    real_time_quotes_now.loc[:, "stock_type"] = stock_type_param['normal_stock']
+    real_time_quotes_now.loc[:, "stock_type"] = stock_type_classify_param['normal_stock']
     # 上市五个交易日的股票
-    real_time_quotes_now.loc[real_time_quotes_now['name'].str.startswith('C'), "stock_type"] = stock_type_param[
-        'new_stock']
+    real_time_quotes_now.loc[real_time_quotes_now['name'].str.startswith('C'), "stock_type"] = \
+        stock_type_classify_param[
+            'new_stock']
+    # 交易上市6-70天的次新股票
+    real_time_quotes_now.loc[
+        (real_time_quotes_now['stock_type'] != stock_type_classify_param['new_stock'])
+        & (real_time_quotes_now['deal_days'] <= stock_type_classify_param['sub_stock_new_max_deal_days']),
+        "stock_type"] = stock_type_classify_param['sub_stock_new']
 
+    # 上市次新股 70-365
     real_time_quotes_now.loc[
-        (real_time_quotes_now['stock_type'] != stock_type_param['new_stock'])
-        & (real_time_quotes_now['diff_days'] <= stock_type_param['sub_stock_max_days']),
-        "stock_type"] = stock_type_param['sub_stock']
+        (real_time_quotes_now['deal_days'] >= stock_type_classify_param['sub_stock_new_max_deal_days'])
+        & (real_time_quotes_now['deal_days'] <= stock_type_classify_param['sub_stock_max_days']),
+        "stock_type"] = stock_type_classify_param['sub_stock']
 
     return real_time_quotes_now
 
 
 # 新上市注册股票
 def choose_new_stock(real_time_quotes_now):
     real_time_quotes_now = real_time_quotes_now.loc[
-        real_time_quotes_now['stock_type'] == stock_type_param['new_stock']]
+        real_time_quotes_now['stock_type'] == stock_type_classify_param['new_stock']]
 
     return real_time_quotes_now
 
 
 # 排除新股
 def exclude_new_stock(real_time_quotes_now):
     real_time_quotes_now = real_time_quotes_now.loc[
-        real_time_quotes_now['stock_type'] != stock_type_param['new_stock']]
+        real_time_quotes_now['stock_type'] != stock_type_classify_param['new_stock']]
+    return real_time_quotes_now
+
+
+# 选择次新new     # 交易上市6-70天的次新股票
+def choose_sub_new(real_time_quotes_now):
+    real_time_quotes_now = real_time_quotes_now.loc[
+        real_time_quotes_now['stock_type'] == stock_type_classify_param['sub_stock_new']]
+
     return real_time_quotes_now
 
 
-# 选择次新
+# 排除次新new      # 交易上市6-70天的次新股票
+def exclude_sub_new(real_time_quotes_now):
+    real_time_quotes_now = real_time_quotes_now.loc[
+        real_time_quotes_now['stock_type'] != stock_type_classify_param['sub_stock_new']]
+    return real_time_quotes_now
+
+
+# 选择次新 71-365
 def choose_sub_stock(real_time_quotes_now):
     real_time_quotes_now = real_time_quotes_now.loc[
-        real_time_quotes_now['stock_type'] == stock_type_param['sub_stock']]
+        real_time_quotes_now['stock_type'] == stock_type_classify_param['sub_stock']]
 
     return real_time_quotes_now
 
 
-# 排除次新
+# 排除次新  71-365
 def exclude_sub_stock(real_time_quotes_now):
     real_time_quotes_now = real_time_quotes_now.loc[
-        real_time_quotes_now['stock_type'] != stock_type_param['sub_stock']]
+        real_time_quotes_now['stock_type'] != stock_type_classify_param['sub_stock']]
     return real_time_quotes_now
 
 
 # 选择普通
 def choose_normal_stock(real_time_quotes_now):
     real_time_quotes_now = real_time_quotes_now.loc[
-        real_time_quotes_now['stock_type'] == stock_type_param['normal_stock']]
+        real_time_quotes_now['stock_type'] == stock_type_classify_param['normal_stock']]
 
     return real_time_quotes_now
 
 
 # 排除普通
 def exclude_normal_stock(real_time_quotes_now):
     real_time_quotes_now = real_time_quotes_now.loc[
-        real_time_quotes_now['stock_type'] != stock_type_param['normal_stock']]
+        real_time_quotes_now['stock_type'] != stock_type_classify_param['normal_stock']]
     return real_time_quotes_now
 
 
-# 选择普通和次新
-def choose_normal_and_sub_stock(real_time_quotes_now):
+# 根据类型列表选择
+def choose_stock_by_type_list(real_time_quotes_now, type_list):
     return real_time_quotes_now.loc[
-        real_time_quotes_now['stock_type'].isin([stock_type_param['normal_stock'],
-                                                 stock_type_param['sub_stock']])]
-
-
-# 选择科创 创业板 注册制以后主板 前五个交易日不设涨幅限制
-def choose_kc_symbol_and_sub(realtime_quotes_now):
-    real_time_quotes_now = realtime_quotes_now.loc[
-        (realtime_quotes_now['classification'].isin(['K', 'C', 'X']))
-        | (realtime_quotes_now['name'].str.startswith('C'))]
-    return real_time_quotes_now
+        real_time_quotes_now['stock_type'].isin(type_list)]
```

### Comparing `mns_common-1.1.3.7/mns_common/component/common_service_fun_api.py` & `mns_common-1.1.3.8/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/company/company_common_service_api.py` & `mns_common-1.1.3.8/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.1.3.8/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.1.3.8/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/data/data_init_api.py` & `mns_common-1.1.3.8/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.1.3.8/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.1.3.8/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.1.3.8/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.1.3.8/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/qmt/qmt_buy_service.py` & `mns_common-1.1.3.8/mns_common/component/qmt/qmt_buy_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.1.3.8/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/self_choose/black_list_service_api.py` & `mns_common-1.1.3.8/mns_common/component/self_choose/black_list_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/self_choose/self_choose_service_api.py` & `mns_common-1.1.3.8/mns_common/component/self_choose/self_choose_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/trade/trade_service_api.py` & `mns_common-1.1.3.8/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.1.3.8/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.1.3.8/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/constant/db_name_constant.py` & `mns_common-1.1.3.8/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/db/MongodbUtil.py` & `mns_common-1.1.3.8/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/utils/data_frame_util.py` & `mns_common-1.1.3.8/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common/utils/date_handle_util.py` & `mns_common-1.1.3.8/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.7/mns_common.egg-info/SOURCES.txt` & `mns_common-1.1.3.8/mns_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 mns_common/api/ths/ths_stock_api.py
 mns_common/api/ths/ths_stock_zt_pool_api.py
 mns_common/component/__init__.py
 mns_common/component/common_service_fun_api.py
 mns_common/component/cache/__init__.py
 mns_common/component/cache/cache_service.py
 mns_common/component/classify/__init__.py
-mns_common/component/classify/classify_constant.py
 mns_common/component/classify/symbol_classify_api.py
+mns_common/component/classify/symbol_classify_param.py
 mns_common/component/company/__init__.py
 mns_common/component/company/company_common_service_api.py
 mns_common/component/concept/__init__.py
 mns_common/component/concept/kpl_concept_common_service_api.py
 mns_common/component/concept/ths_concept_common_service_api.py
 mns_common/component/data/__init__.py
 mns_common/component/data/data_init_api.py
```

