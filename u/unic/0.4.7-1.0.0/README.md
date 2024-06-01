# Comparing `tmp/unic-0.4.7.tar.gz` & `tmp/unic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unic-0.4.7.tar", max compression
+gzip compressed data, was "unic-1.0.0.tar", max compression
```

## Comparing `unic-0.4.7.tar` & `unic-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.7/LICENSE
--rw-r--r--   0        0        0      888 2024-05-23 15:12:17.186843 unic-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     2398 2024-05-03 12:41:18.395441 unic-0.4.7/README.md
--rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.7/unic/__init__.py
--rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.7/unic/configs/metirc_system/settings.toml
--rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.7/unic/configs/timeunit/settings.toml
--rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.7/unic/configs/timezone/settings.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.7/unic/length_unit/metric_system/__init__.py
--rw-r--r--   0        0        0      865 2024-05-23 14:56:09.193757 unic-0.4.7/unic/length_unit/metric_system/metric_system_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.7/unic/length_unit/validators/__init__.py
--rw-r--r--   0        0        0     1279 2024-05-10 14:36:03.640060 unic-0.4.7/unic/length_unit/validators/validators.py
--rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.7/unic/time_unit/datetime/__init__.py
--rw-r--r--   0        0        0     1377 2024-05-16 14:49:57.983327 unic-0.4.7/unic/time_unit/datetime/datetime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.7/unic/time_unit/time/__init__.py
--rw-r--r--   0        0        0      834 2024-05-23 14:53:33.455521 unic-0.4.7/unic/time_unit/time/time_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.7/unic/time_unit/unixtime/__init__.py
--rw-r--r--   0        0        0     1303 2024-05-23 14:11:24.862341 unic-0.4.7/unic/time_unit/unixtime/unixtime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.7/unic/time_unit/validators/__init__.py
--rw-r--r--   0        0        0     2795 2024-05-21 15:45:17.999751 unic-0.4.7/unic/time_unit/validators/validators.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.7/unic/utils/__init__.py
--rw-r--r--   0        0        0      399 2024-05-14 16:00:12.297440 unic-0.4.7/unic/utils/config_parser.py
--rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 unic-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-1.0.0/LICENSE
+-rw-r--r--   0        0        0      911 2024-06-01 15:21:17.095203 unic-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2398 2024-05-03 12:41:18.395441 unic-1.0.0/README.md
+-rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-1.0.0/unic/__init__.py
+-rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-1.0.0/unic/configs/metirc_system/settings.toml
+-rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-1.0.0/unic/configs/timeunit/settings.toml
+-rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-1.0.0/unic/configs/timezone/settings.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-1.0.0/unic/length_unit/metric_system/__init__.py
+-rw-r--r--   0        0        0      865 2024-05-23 14:56:09.193757 unic-1.0.0/unic/length_unit/metric_system/metric_system_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-1.0.0/unic/length_unit/validators/__init__.py
+-rw-r--r--   0        0        0     1279 2024-05-10 14:36:03.640060 unic-1.0.0/unic/length_unit/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-1.0.0/unic/time_unit/datetime/__init__.py
+-rw-r--r--   0        0        0     1377 2024-05-16 14:49:57.983327 unic-1.0.0/unic/time_unit/datetime/datetime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-1.0.0/unic/time_unit/time/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-23 14:53:33.455521 unic-1.0.0/unic/time_unit/time/time_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-1.0.0/unic/time_unit/unixtime/__init__.py
+-rw-r--r--   0        0        0     1303 2024-05-23 14:11:24.862341 unic-1.0.0/unic/time_unit/unixtime/unixtime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-1.0.0/unic/time_unit/validators/__init__.py
+-rw-r--r--   0        0        0     2795 2024-05-21 15:45:17.999751 unic-1.0.0/unic/time_unit/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-1.0.0/unic/utils/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-14 16:00:12.297440 unic-1.0.0/unic/utils/config_parser.py
+-rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 unic-1.0.0/PKG-INFO
```

### Comparing `unic-0.4.7/LICENSE` & `unic-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/pyproject.toml` & `unic-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unic"
-version = "0.4.7"
+version = "1.0.0"
 description = "Python package for converting various units."
 authors = ["Subretu"]
 maintainers = ["Subretu"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/subretu/unic'
 keywords = ['unit', 'convert', 'time', 'timestamp', 'length']
@@ -24,11 +24,12 @@
 pydantic = "^2.1"
 tomli = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.1"
 black = "^24.4.2"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `unic-0.4.7/README.md` & `unic-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/__init__.py` & `unic-1.0.0/unic/__init__.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/configs/metirc_system/settings.toml` & `unic-1.0.0/unic/configs/metirc_system/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/configs/timezone/settings.toml` & `unic-1.0.0/unic/configs/timezone/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/length_unit/metric_system/metric_system_model.py` & `unic-1.0.0/unic/length_unit/metric_system/metric_system_model.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/length_unit/validators/validators.py` & `unic-1.0.0/unic/length_unit/validators/validators.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/time_unit/datetime/datetime_model.py` & `unic-1.0.0/unic/time_unit/datetime/datetime_model.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/time_unit/time/time_model.py` & `unic-1.0.0/unic/time_unit/time/time_model.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/time_unit/unixtime/unixtime_model.py` & `unic-1.0.0/unic/time_unit/unixtime/unixtime_model.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/unic/time_unit/validators/validators.py` & `unic-1.0.0/unic/time_unit/validators/validators.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.7/PKG-INFO` & `unic-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unic
-Version: 0.4.7
+Version: 1.0.0
 Summary: Python package for converting various units.
 Home-page: https://github.com/subretu/unic
 License: MIT
 Keywords: unit,convert,time,timestamp,length
 Author: Subretu
 Maintainer: Subretu
 Requires-Python: >=3.8,<4.0
```

