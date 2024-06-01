# Comparing `tmp/wujing-0.1.0.tar.gz` & `tmp/wujing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wujing-0.1.0.tar", max compression
+gzip compressed data, was "wujing-0.1.1.tar", max compression
```

## Comparing `wujing-0.1.0.tar` & `wujing-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      511 2024-06-01 16:20:02.752311 wujing-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        8 2024-06-01 15:43:38.836867 wujing-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-06-01 12:55:11.416512 wujing-0.1.0/toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 12:55:11.601734 wujing-0.1.0/toolkit/plot/__init__.py
--rw-r--r--   0        0        0     3020 2024-06-01 12:55:11.735762 wujing-0.1.0/toolkit/plot/plot_log_scaled_histogram.py
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 wujing-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-06-01 16:42:47.519526 wujing-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       16 2024-06-01 16:40:18.653371 wujing-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-06-01 16:38:12.496816 wujing-0.1.1/toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:38:12.496816 wujing-0.1.1/toolkit/plot/__init__.py
+-rw-r--r--   0        0        0     3020 2024-06-01 16:38:12.496816 wujing-0.1.1/toolkit/plot/plot_log_scaled_histogram.py
+-rw-r--r--   0        0        0      447 1970-01-01 00:00:00.000000 wujing-0.1.1/PKG-INFO
```

### Comparing `wujing-0.1.0/toolkit/plot/plot_log_scaled_histogram.py` & `wujing-0.1.1/toolkit/plot/plot_log_scaled_histogram.py`

 * *Files identical despite different names*

