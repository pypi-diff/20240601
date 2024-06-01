# Comparing `tmp/kabutobashi-0.7.2.tar.gz` & `tmp/kabutobashi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kabutobashi-0.7.2.tar", max compression
+gzip compressed data, was "kabutobashi-0.8.0.tar", max compression
```

## Comparing `kabutobashi-0.7.2.tar` & `kabutobashi-0.8.0.tar`

### file list

```diff
@@ -1,48 +1,87 @@
--rw-r--r--   0        0        0     1046 2023-08-26 13:57:06.613903 kabutobashi-0.7.2/LICENSE
--rw-r--r--   0        0        0     2430 2023-08-26 13:57:06.613903 kabutobashi-0.7.2/README.md
--rw-r--r--   0        0        0     1578 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/__init__.py
--rw-r--r--   0        0        0      118 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/application/__init__.py
--rw-r--r--   0        0        0     1101 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/application/applications.py
--rw-r--r--   0        0        0     1281 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/application/crawl_application.py
--rw-r--r--   0        0        0     1679 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/application/di_container.py
--rw-r--r--   0        0        0      467 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/__init__.py
--rw-r--r--   0        0        0       50 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/aggregates/__init__.py
--rw-r--r--   0        0        0     4659 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/aggregates/single_code.py
--rw-r--r--   0        0        0       25 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/entity/__init__.py
--rw-r--r--   0        0        0    14511 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/entity/stock.py
--rw-r--r--   0        0        0      799 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/errors.py
--rw-r--r--   0        0        0      591 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/serialize.py
--rw-r--r--   0        0        0      244 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/services/__init__.py
--rw-r--r--   0        0        0     1742 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/services/analyze.py
--rw-r--r--   0        0        0       38 2023-08-26 13:57:06.621903 kabutobashi-0.7.2/kabutobashi/domain/services/converter/__init__.py
--rw-r--r--   0        0        0     2705 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/converter/to_entity.py
--rw-r--r--   0        0        0      141 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/decode_html/__init__.py
--rw-r--r--   0        0        0     7272 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/decode_html/html_info.py
--rw-r--r--   0        0        0     2086 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/decode_html/utils.py
--rw-r--r--   0        0        0      947 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/__init__.py
--rw-r--r--   0        0        0     6390 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/adx.py
--rw-r--r--   0        0        0     1594 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/basic.py
--rw-r--r--   0        0        0     3535 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/bollinger_bands.py
--rw-r--r--   0        0        0     3045 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/fitting.py
--rw-r--r--   0        0        0     2397 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/ichimoku.py
--rw-r--r--   0        0        0     3182 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/industry_cat.py
--rw-r--r--   0        0        0     2379 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/macd.py
--rw-r--r--   0        0        0    10660 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/method.py
--rw-r--r--   0        0        0     1522 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/momentum.py
--rw-r--r--   0        0        0     1471 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/pct_change.py
--rw-r--r--   0        0        0     2042 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/psycho_logical.py
--rw-r--r--   0        0        0     2684 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/sma.py
--rw-r--r--   0        0        0     5415 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/stochastics.py
--rw-r--r--   0        0        0     1363 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/services/method/volatility.py
--rw-r--r--   0        0        0      491 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/values/__init__.py
--rw-r--r--   0        0        0     4319 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/values/decoded_html_pages.py
--rw-r--r--   0        0        0     1652 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/values/raw_html_pages.py
--rw-r--r--   0        0        0     1690 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/values/stock_data.py
--rw-r--r--   0        0        0     2001 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/domain/values/user_agent.py
--rw-r--r--   0        0        0      536 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/example_data.py
--rw-r--r--   0        0        0        0 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/infrastructure/__init__.py
--rw-r--r--   0        0        0      177 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/infrastructure/repository/__init__.py
--rw-r--r--   0        0        0     3413 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/infrastructure/repository/html_page_repository.py
--rw-r--r--   0        0        0     3194 2023-08-26 13:57:06.625903 kabutobashi-0.7.2/kabutobashi/utilities.py
--rw-r--r--   0        0        0     1832 2023-08-26 13:57:06.629903 kabutobashi-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 kabutobashi-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1046 2021-11-16 15:11:13.718673 kabutobashi-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5420 2024-06-01 02:10:09.626156 kabutobashi-0.8.0/README.md
+-rw-r--r--   0        0        0     1657 2024-06-01 02:10:09.704313 kabutobashi-0.8.0/kabutobashi/__init__.py
+-rw-r--r--   0        0        0      118 2024-04-26 12:24:27.332999 kabutobashi-0.8.0/kabutobashi/application/__init__.py
+-rw-r--r--   0        0        0     1148 2024-06-01 02:10:09.626829 kabutobashi-0.8.0/kabutobashi/application/applications.py
+-rw-r--r--   0        0        0     1281 2023-01-09 02:04:19.887157 kabutobashi-0.8.0/kabutobashi/application/crawl_application.py
+-rw-r--r--   0        0        0     1679 2023-01-09 02:04:19.887273 kabutobashi-0.8.0/kabutobashi/application/di_container.py
+-rw-r--r--   0        0        0      467 2023-01-06 23:35:53.082753 kabutobashi-0.8.0/kabutobashi/domain/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-26 12:24:27.333933 kabutobashi-0.8.0/kabutobashi/domain/aggregates/__init__.py
+-rw-r--r--   0        0        0     4659 2024-04-26 12:24:27.334665 kabutobashi-0.8.0/kabutobashi/domain/aggregates/single_code.py
+-rw-r--r--   0        0        0       25 2023-01-06 23:35:53.082870 kabutobashi-0.8.0/kabutobashi/domain/entity/__init__.py
+-rw-r--r--   0        0        0       99 2024-06-01 02:10:09.626925 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/__init__.py
+-rw-r--r--   0        0        0     3101 2024-06-01 02:10:09.627024 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/abc_block.py
+-rw-r--r--   0        0        0      192 2024-06-01 02:10:09.627120 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/crawl_blocks/__init__.py
+-rw-r--r--   0        0        0      365 2024-06-01 02:10:09.627234 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/crawl_blocks/abc_crawl_block.py
+-rw-r--r--   0        0        0      757 2024-06-01 02:10:09.627328 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/crawl_blocks/crawl_stock_info_block.py
+-rw-r--r--   0        0        0      983 2024-06-01 02:10:09.627434 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/crawl_blocks/crawl_stock_info_multiple_days_block.py
+-rw-r--r--   0        0        0      665 2024-06-01 02:10:09.627535 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/crawl_blocks/crawl_stock_ipo_block.py
+-rw-r--r--   0        0        0    13932 2024-06-01 02:10:09.627664 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/decorator.py
+-rw-r--r--   0        0        0      204 2024-06-01 02:10:09.627758 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/extract_blocks/__init__.py
+-rw-r--r--   0        0        0     4699 2024-06-01 02:10:09.627889 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/extract_blocks/extract_stock_info_block.py
+-rw-r--r--   0        0        0     2395 2024-06-01 02:10:09.628012 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/extract_blocks/extract_stock_info_multiple_days_block.py
+-rw-r--r--   0        0        0     1576 2024-06-01 02:10:09.628126 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/extract_blocks/extract_stock_ipo_block.py
+-rw-r--r--   0        0        0     4506 2024-06-01 02:10:09.628273 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/hub_block.py
+-rw-r--r--   0        0        0      471 2024-06-01 02:10:09.628491 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/__init__.py
+-rw-r--r--   0        0        0     1188 2024-06-01 02:10:09.628590 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/abc_parameterize_block.py
+-rw-r--r--   0        0        0      830 2024-06-01 02:10:09.628690 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/parameterize_adx_block.py
+-rw-r--r--   0        0        0     1151 2024-06-01 02:10:09.628800 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/parameterize_bollinger_bands_block.py
+-rw-r--r--   0        0        0      804 2024-06-01 02:10:09.628903 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/parameterize_macd_block.py
+-rw-r--r--   0        0        0      686 2024-06-01 02:10:09.629009 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/parameterize_momentum_block.py
+-rw-r--r--   0        0        0      838 2024-06-01 02:10:09.629111 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/parameterize_psycho_logical_block.py
+-rw-r--r--   0        0        0     1498 2024-06-01 02:10:09.629226 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/parameterize_sma_block.py
+-rw-r--r--   0        0        0      892 2024-06-01 02:10:09.629332 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/parameterize_blocks/parameterize_stochastics_block.py
+-rw-r--r--   0        0        0       56 2024-06-01 02:10:09.629537 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/pre_process_blocks/__init__.py
+-rw-r--r--   0        0        0      635 2024-06-01 02:10:09.629653 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/pre_process_blocks/default_pre_process.py
+-rw-r--r--   0        0        0      401 2024-06-01 02:10:09.629866 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/__init__.py
+-rw-r--r--   0        0        0     1224 2024-06-01 02:10:09.629962 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/abc_process_block.py
+-rw-r--r--   0        0        0     5793 2024-06-01 02:10:09.630119 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/process_adx_block.py
+-rw-r--r--   0        0        0     2238 2024-06-01 02:10:09.630232 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/process_bollinger_bands_block.py
+-rw-r--r--   0        0        0     1358 2024-06-01 02:10:09.630336 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/process_macd_block.py
+-rw-r--r--   0        0        0      998 2024-06-01 02:10:09.630437 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/process_momentum_block.py
+-rw-r--r--   0        0        0     1585 2024-06-01 02:10:09.630543 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/process_psycho_logical_block.py
+-rw-r--r--   0        0        0     1187 2024-06-01 02:10:09.630640 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/process_sma_block.py
+-rw-r--r--   0        0        0     4260 2024-06-01 02:10:09.630778 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/process_blocks/process_stochastics_block.py
+-rw-r--r--   0        0        0       49 2024-06-01 02:10:09.631048 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/read_blocks/__init__.py
+-rw-r--r--   0        0        0      709 2024-06-01 02:10:09.631146 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/read_blocks/read_example_block.py
+-rw-r--r--   0        0        0       51 2024-06-01 02:10:09.631410 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/reduce_blocks/__init__.py
+-rw-r--r--   0        0        0     1087 2024-06-01 02:10:09.631521 kabutobashi-0.8.0/kabutobashi/domain/entity/blocks/reduce_blocks/fully_connect_block.py
+-rw-r--r--   0        0        0    14519 2024-06-01 02:10:09.631974 kabutobashi-0.8.0/kabutobashi/domain/entity/stock.py
+-rw-r--r--   0        0        0     1867 2024-06-01 02:10:09.632102 kabutobashi-0.8.0/kabutobashi/domain/errors.py
+-rw-r--r--   0        0        0      591 2023-01-09 02:04:19.887916 kabutobashi-0.8.0/kabutobashi/domain/serialize.py
+-rw-r--r--   0        0        0      244 2023-01-06 23:35:53.083402 kabutobashi-0.8.0/kabutobashi/domain/services/__init__.py
+-rw-r--r--   0        0        0     1742 2023-01-03 08:30:17.876611 kabutobashi-0.8.0/kabutobashi/domain/services/analyze.py
+-rw-r--r--   0        0        0       38 2023-01-06 23:35:53.083638 kabutobashi-0.8.0/kabutobashi/domain/services/converter/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-26 12:24:27.336091 kabutobashi-0.8.0/kabutobashi/domain/services/converter/to_entity.py
+-rw-r--r--   0        0        0      141 2023-01-03 08:30:17.876814 kabutobashi-0.8.0/kabutobashi/domain/services/decode_html/__init__.py
+-rw-r--r--   0        0        0     7272 2023-01-09 02:04:19.888243 kabutobashi-0.8.0/kabutobashi/domain/services/decode_html/html_info.py
+-rw-r--r--   0        0        0     2086 2023-01-03 08:30:17.877049 kabutobashi-0.8.0/kabutobashi/domain/services/decode_html/utils.py
+-rw-r--r--   0        0        0       33 2024-06-01 02:10:09.632387 kabutobashi-0.8.0/kabutobashi/domain/services/flow/__init__.py
+-rw-r--r--   0        0        0     7213 2024-06-01 02:10:09.632644 kabutobashi-0.8.0/kabutobashi/domain/services/flow/flow.py
+-rw-r--r--   0        0        0      948 2024-06-01 02:10:09.632940 kabutobashi-0.8.0/kabutobashi/domain/services/method/__init__.py
+-rw-r--r--   0        0        0     6390 2023-07-18 04:44:29.984705 kabutobashi-0.8.0/kabutobashi/domain/services/method/adx.py
+-rw-r--r--   0        0        0     1594 2023-07-18 04:44:29.984945 kabutobashi-0.8.0/kabutobashi/domain/services/method/basic.py
+-rw-r--r--   0        0        0     3535 2023-08-26 13:49:54.265668 kabutobashi-0.8.0/kabutobashi/domain/services/method/bollinger_bands.py
+-rw-r--r--   0        0        0     3045 2023-07-18 04:44:29.985376 kabutobashi-0.8.0/kabutobashi/domain/services/method/fitting.py
+-rw-r--r--   0        0        0     2397 2023-07-18 04:44:29.985532 kabutobashi-0.8.0/kabutobashi/domain/services/method/ichimoku.py
+-rw-r--r--   0        0        0     3182 2023-07-18 04:44:29.985771 kabutobashi-0.8.0/kabutobashi/domain/services/method/industry_cat.py
+-rw-r--r--   0        0        0     2379 2023-08-26 13:49:54.265558 kabutobashi-0.8.0/kabutobashi/domain/services/method/macd.py
+-rw-r--r--   0        0        0    10660 2023-08-26 13:54:05.350319 kabutobashi-0.8.0/kabutobashi/domain/services/method/method.py
+-rw-r--r--   0        0        0     1522 2023-07-18 04:44:29.986426 kabutobashi-0.8.0/kabutobashi/domain/services/method/momentum.py
+-rw-r--r--   0        0        0     1471 2023-07-18 04:44:29.986590 kabutobashi-0.8.0/kabutobashi/domain/services/method/pct_change.py
+-rw-r--r--   0        0        0     2042 2023-07-18 04:44:29.986741 kabutobashi-0.8.0/kabutobashi/domain/services/method/psycho_logical.py
+-rw-r--r--   0        0        0     2684 2023-08-26 13:49:54.265339 kabutobashi-0.8.0/kabutobashi/domain/services/method/sma.py
+-rw-r--r--   0        0        0     5415 2023-07-18 04:44:29.987035 kabutobashi-0.8.0/kabutobashi/domain/services/method/stochastics.py
+-rw-r--r--   0        0        0     1363 2023-07-18 04:44:29.987176 kabutobashi-0.8.0/kabutobashi/domain/services/method/volatility.py
+-rw-r--r--   0        0        0      491 2023-01-09 02:04:19.888346 kabutobashi-0.8.0/kabutobashi/domain/values/__init__.py
+-rw-r--r--   0        0        0     4319 2023-07-14 03:41:24.936146 kabutobashi-0.8.0/kabutobashi/domain/values/decoded_html_pages.py
+-rw-r--r--   0        0        0     1652 2023-07-14 03:41:24.936438 kabutobashi-0.8.0/kabutobashi/domain/values/raw_html_pages.py
+-rw-r--r--   0        0        0     1690 2023-07-14 03:41:24.936681 kabutobashi-0.8.0/kabutobashi/domain/values/stock_data.py
+-rw-r--r--   0        0        0     2001 2022-07-23 12:18:17.215670 kabutobashi-0.8.0/kabutobashi/domain/values/user_agent.py
+-rw-r--r--   0        0        0      536 2023-01-03 08:30:17.877878 kabutobashi-0.8.0/kabutobashi/example_data.py
+-rw-r--r--   0        0        0        0 2022-05-18 14:35:16.310647 kabutobashi-0.8.0/kabutobashi/infrastructure/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-14 03:41:24.936950 kabutobashi-0.8.0/kabutobashi/infrastructure/repository/__init__.py
+-rw-r--r--   0        0        0     3413 2023-01-09 02:04:19.888724 kabutobashi-0.8.0/kabutobashi/infrastructure/repository/html_page_repository.py
+-rw-r--r--   0        0        0     3194 2023-01-03 08:30:17.878499 kabutobashi-0.8.0/kabutobashi/utilities.py
+-rw-r--r--   0        0        0     1452 2024-06-01 02:10:09.704437 kabutobashi-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6558 1970-01-01 00:00:00.000000 kabutobashi-0.8.0/PKG-INFO
```

### Comparing `kabutobashi-0.7.2/LICENSE` & `kabutobashi-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/__init__.py` & `kabutobashi-0.8.0/kabutobashi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from .application import crawl_info, crawl_info_multiple, crawl_ipo, decode_brand_list
 from .domain import errors
 from .domain.aggregates import StockCodeSingleAggregate
 from .domain.entity import Stock
+from .domain.entity.blocks import block
 from .domain.services import SaFundamental, SaVolume, StockAnalysis
+from .domain.services.flow import Flow
 
 # methods to analysis
 from .domain.services.method import (
     Method,
     adx,
     basic,
     bollinger_bands,
@@ -41,15 +43,15 @@
 # estimate filters
 sa_fundamental = SaFundamental()
 sa_volume = SaVolume()
 
 stock_analysis = [sa_fundamental, sa_volume]
 
 # comparable tuple
-VERSION = (0, 7, 2)
+VERSION = (0, 8, 0)
 # generate __version__ via VERSION tuple
 __version__ = ".".join(map(str, VERSION))
 
 # module level doc-string
 __doc__ = """
 kabutobashi
 ===========
```

### Comparing `kabutobashi-0.7.2/kabutobashi/application/applications.py` & `kabutobashi-0.8.0/kabutobashi/application/applications.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 
 
 def decode_brand_list(path: str) -> List[Stock]:
     """
     See Also: https://www.jpx.co.jp/markets/statistics-equities/misc/01.html
     """
     df = pd.read_excel(path)
-    column_renames = {"日付": "dt", "コード": "code", "銘柄名": "name", "市場・商品区分": "market", "33業種区分": "industry_type"}
+    column_renames = {
+        "日付": "dt",
+        "コード": "code",
+        "銘柄名": "name",
+        "市場・商品区分": "market",
+        "33業種区分": "industry_type",
+    }
     df = df.rename(columns=column_renames)
     df = df[column_renames.values()]
     df["market"] = df["market"].apply(lambda x: x.replace("（内国株式）", ""))
     prime_df = df[df["market"] == "プライム"]
     standard_df = df[df["market"] == "スタンダード"]
     growth_df = df[df["market"] == "グロース"]
     merged_df = pd.concat([prime_df, standard_df, growth_df]).reset_index()
```

### Comparing `kabutobashi-0.7.2/kabutobashi/application/crawl_application.py` & `kabutobashi-0.8.0/kabutobashi/application/crawl_application.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/application/di_container.py` & `kabutobashi-0.8.0/kabutobashi/application/di_container.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/aggregates/single_code.py` & `kabutobashi-0.8.0/kabutobashi/domain/aggregates/single_code.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/entity/stock.py` & `kabutobashi-0.8.0/kabutobashi/domain/entity/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,17 +112,17 @@
         if self.code != other.code:
             raise KabutobashiEntityError()
         return StockBrand(
             code=self.code if self.code is not None else other.code,
             unit=self.unit if self.unit is not None else other.unit,
             market=self.market if self.market is not None else other.market,
             industry_type=self.industry_type if self.industry_type is not None else other.industry_type,
-            market_capitalization=self.market_capitalization
-            if self.market_capitalization is not None
-            else other.market_capitalization,
+            market_capitalization=(
+                self.market_capitalization if self.market_capitalization is not None else other.market_capitalization
+            ),
             name=self.name if self.name is not None else other.name,
             issued_shares=self.issued_shares if self.issued_shares is not None else other.issued_shares,
             is_delisting=self.is_delisting or other.is_delisting,
         )
 
     # TODO modify
     # class Config:
```

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/serialize.py` & `kabutobashi-0.8.0/kabutobashi/domain/serialize.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/analyze.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/analyze.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/converter/to_entity.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/converter/to_entity.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/decode_html/html_info.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/decode_html/html_info.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/decode_html/utils.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/decode_html/utils.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/__init__.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   - Stochastics
 
 - other
 
   - Basic: only used `parameterize`
 
 """
+
 from .adx import AdxProcess, adx
 from .basic import BasicProcess, basic
 from .bollinger_bands import BollingerBandsProcess, bollinger_bands
 from .fitting import FittingProcess, fitting
 from .ichimoku import IchimokuProcess, ichimoku
 from .industry_cat import IndustryCategoriesProcess, industry_categories
 from .macd import MacdProcess, macd
```

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/adx.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/adx.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/basic.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/basic.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/bollinger_bands.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/fitting.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/fitting.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/ichimoku.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/ichimoku.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/industry_cat.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/industry_cat.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/macd.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/macd.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/method.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/method.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/momentum.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/momentum.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/pct_change.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/pct_change.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/psycho_logical.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/psycho_logical.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/sma.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/sma.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/stochastics.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/stochastics.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/services/method/volatility.py` & `kabutobashi-0.8.0/kabutobashi/domain/services/method/volatility.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/values/decoded_html_pages.py` & `kabutobashi-0.8.0/kabutobashi/domain/values/decoded_html_pages.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/values/raw_html_pages.py` & `kabutobashi-0.8.0/kabutobashi/domain/values/raw_html_pages.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/values/stock_data.py` & `kabutobashi-0.8.0/kabutobashi/domain/values/stock_data.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/domain/values/user_agent.py` & `kabutobashi-0.8.0/kabutobashi/domain/values/user_agent.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/example_data.py` & `kabutobashi-0.8.0/kabutobashi/example_data.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/infrastructure/repository/html_page_repository.py` & `kabutobashi-0.8.0/kabutobashi/infrastructure/repository/html_page_repository.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.2/kabutobashi/utilities.py` & `kabutobashi-0.8.0/kabutobashi/utilities.py`

 * *Files identical despite different names*

