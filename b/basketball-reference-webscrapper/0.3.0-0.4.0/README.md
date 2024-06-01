# Comparing `tmp/basketball_reference_webscrapper-0.3.0.tar.gz` & `tmp/basketball_reference_webscrapper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basketball_reference_webscrapper-0.3.0.tar", max compression
+gzip compressed data, was "basketball_reference_webscrapper-0.4.0.tar", max compression
```

## Comparing `basketball_reference_webscrapper-0.3.0.tar` & `basketball_reference_webscrapper-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      120 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/constants/__init__.py
--rw-r--r--   0        0        0     1223 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/constants/team_city_refdata.csv
--rw-r--r--   0        0        0        0 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/data_models/__init_.py
--rw-r--r--   0        0        0      213 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/data_models/feature_model.py
--rw-r--r--   0        0        0     2153 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/params.yaml
--rw-r--r--   0        0        0        0 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/utils/__init__.py
--rw-r--r--   0        0        0     1075 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/utils/logs.py
--rw-r--r--   0        0        0     8575 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/webscrapping_basketball_reference.py
--rw-r--r--   0        0        0      958 2024-05-29 16:30:47.553898 basketball_reference_webscrapper-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2967 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/constants/__init__.py
+-rw-r--r--   0        0        0     1223 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/constants/team_city_refdata.csv
+-rw-r--r--   0        0        0        0 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/data_models/__init_.py
+-rw-r--r--   0        0        0      213 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/data_models/feature_model.py
+-rw-r--r--   0        0        0     2153 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/params.yaml
+-rw-r--r--   0        0        0        0 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/utils/__init__.py
+-rw-r--r--   0        0        0     1075 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/utils/logs.py
+-rw-r--r--   0        0        0     8575 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/webscrapping_basketball_reference.py
+-rw-r--r--   0        0        0      958 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.4.0/PKG-INFO
```

### Comparing `basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/constants/team_city_refdata.csv` & `basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/constants/team_city_refdata.csv`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/params.yaml` & `basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/params.yaml`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/utils/logs.py` & `basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/utils/logs.py`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.3.0/basketball_reference_webscrapper/webscrapping_basketball_reference.py` & `basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/webscrapping_basketball_reference.py`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.3.0/pyproject.toml` & `basketball_reference_webscrapper-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basketball-reference-webscrapper"
-version = "0.3.0"
+version = "0.4.0"
 description = "Python package for Basketball Reference that gathers data by scraping the website"
 authors = ["Yannick Flores <yannick.flores1992@gmail.com>"]
 readme = "README.md"
 exclude = ["tests", "docs"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

