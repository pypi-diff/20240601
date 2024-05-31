# Comparing `tmp/rcpchgrowth-4.0.0.tar.gz` & `tmp/rcpchgrowth-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcpchgrowth-4.0.0.tar", last modified: Tue Mar 19 11:53:39 2024, max compression
+gzip compressed data, was "rcpchgrowth-4.0.1.tar", last modified: Fri May 31 23:45:54 2024, max compression
```

## Comparing `rcpchgrowth-4.0.0.tar` & `rcpchgrowth-4.0.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.951671 rcpchgrowth-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-19 11:53:39.951671 rcpchgrowth-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.943670 rcpchgrowth-4.0.0/rcpchgrowth/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/age_advice_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/bmi_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/bone_age.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/centile_bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/chart_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.943670 rcpchgrowth-4.0.0/rcpchgrowth/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/constants/age_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/constants/bone_age_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/constants/height_predictions_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/constants/reference_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/constants/validation_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.947670 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.947670 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-19 11:52:20.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 runner    (1001) docker     (127)  1058807 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/bayley-pineau.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/data_tables.txt
--rw-r--r--   0 runner    (1001) docker     (127)   156863 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/trisomy_21.json
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/turner.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.951671 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/
--rw-r--r--   0 runner    (1001) docker     (127)  1199717 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/GrowthCharts.xls
--rw-r--r--   0 runner    (1001) docker     (127)   165925 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/huiqi_cole_methods.bas
--rw-r--r--   0 runner    (1001) docker     (127)   110063 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/uk_who_0_20_preterm.json
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/uk_who_0_20_term.json
--rw-r--r--   0 runner    (1001) docker     (127)   179902 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk90_child.json
--rw-r--r--   0 runner    (1001) docker     (127)    19892 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk90_preterm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk90_term.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.951671 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/RCPCH weight correlation matrix by month.csv
--rw-r--r--   0 runner    (1001) docker     (127)    52900 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/RCPCH weight correlation matrix by week.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_month.json
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_month.py
--rw-r--r--   0 runner    (1001) docker     (127)    78513 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_week.json
--rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/who_children.json
--rw-r--r--   0 runner    (1001) docker     (127)    37436 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/data_tables/who_infants.json
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/date_calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    29651 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/dynamic_growth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/fictional_child.py
--rw-r--r--   0 runner    (1001) docker     (127)    18679 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/global_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    33614 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.951671 rcpchgrowth-4.0.0/rcpchgrowth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/tests/test_global_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/tests/test_measurement_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/trisomy_21.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/turner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/rcpchgrowth/uk_who.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:53:39.951671 rcpchgrowth-4.0.0/rcpchgrowth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-19 11:53:39.000000 rcpchgrowth-4.0.0/rcpchgrowth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-19 11:53:39.000000 rcpchgrowth-4.0.0/rcpchgrowth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:53:39.000000 rcpchgrowth-4.0.0/rcpchgrowth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-19 11:53:39.000000 rcpchgrowth-4.0.0/rcpchgrowth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-19 11:53:39.000000 rcpchgrowth-4.0.0/rcpchgrowth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:53:39.951671 rcpchgrowth-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-19 11:51:57.000000 rcpchgrowth-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.615090 rcpchgrowth-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-31 23:45:54.615090 rcpchgrowth-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.607091 rcpchgrowth-4.0.1/rcpchgrowth/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/age_advice_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/bmi_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/bone_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/centile_bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/chart_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.607091 rcpchgrowth-4.0.1/rcpchgrowth/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/constants/age_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/constants/bone_age_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/constants/height_predictions_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/constants/reference_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/constants/validation_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.611091 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.611091 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-31 23:44:34.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)  1058807 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/bayley-pineau.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/data_tables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   156863 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/trisomy_21.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/turner.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.615090 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  1199717 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/GrowthCharts.xls
+-rw-r--r--   0 runner    (1001) docker     (127)   165925 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/huiqi_cole_methods.bas
+-rw-r--r--   0 runner    (1001) docker     (127)   110063 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/uk_who_0_20_preterm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/uk_who_0_20_term.json
+-rw-r--r--   0 runner    (1001) docker     (127)   179902 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk90_child.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19892 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk90_preterm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk90_term.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.615090 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/RCPCH weight correlation matrix by month.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    52900 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/RCPCH weight correlation matrix by week.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_month.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78513 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_week.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/who_children.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37436 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/data_tables/who_infants.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/date_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29651 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/dynamic_growth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/fictional_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18679 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/global_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33614 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.615090 rcpchgrowth-4.0.1/rcpchgrowth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/tests/test_global_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/tests/test_measurement_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/trisomy_21.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/turner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/rcpchgrowth/uk_who.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:54.615090 rcpchgrowth-4.0.1/rcpchgrowth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-31 23:45:54.000000 rcpchgrowth-4.0.1/rcpchgrowth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-31 23:45:54.000000 rcpchgrowth-4.0.1/rcpchgrowth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:45:54.000000 rcpchgrowth-4.0.1/rcpchgrowth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 23:45:54.000000 rcpchgrowth-4.0.1/rcpchgrowth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 23:45:54.000000 rcpchgrowth-4.0.1/rcpchgrowth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 23:45:54.615090 rcpchgrowth-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-31 23:44:08.000000 rcpchgrowth-4.0.1/setup.py
```

### Comparing `rcpchgrowth-4.0.0/LICENSE` & `rcpchgrowth-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/PKG-INFO` & `rcpchgrowth-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcpchgrowth
-Version: 4.0.0
+Version: 4.0.1
 Summary: SDS and Centile calculations for UK Growth Data
 Home-page: https://github.com/rcpch/digital-growth-charts/blob/master/README.md
 Author: @eatyourpeas, @marcusbaw, @statist7, RCPCH Incubator
 Author-email: incubator@rcpch.ac.uk
 Project-URL: Bug Reports, https://github.com/rcpch/rcpchgrowth-python/issues
 Project-URL: API management, https://dev.rcpch.ac.uk
 Project-URL: Source, https://github.com/rcpch/rcpchgrowth-python
```

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/__init__.py` & `rcpchgrowth-4.0.1/rcpchgrowth/__init__.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/age_advice_strings.py` & `rcpchgrowth-4.0.1/rcpchgrowth/age_advice_strings.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/bmi_functions.py` & `rcpchgrowth-4.0.1/rcpchgrowth/bmi_functions.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/bone_age.py` & `rcpchgrowth-4.0.1/rcpchgrowth/bone_age.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/centile_bands.py` & `rcpchgrowth-4.0.1/rcpchgrowth/centile_bands.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/chart_functions.py` & `rcpchgrowth-4.0.1/rcpchgrowth/chart_functions.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/constants/age_constants.py` & `rcpchgrowth-4.0.1/rcpchgrowth/constants/age_constants.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/constants/reference_constants.py` & `rcpchgrowth-4.0.1/rcpchgrowth/constants/reference_constants.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/constants/validation_constants.py` & `rcpchgrowth-4.0.1/rcpchgrowth/constants/validation_constants.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/bayley-pineau.pdf` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/bayley-pineau.pdf`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/trisomy_21.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/trisomy_21.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/turner.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/turner.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/GrowthCharts.xls` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/GrowthCharts.xls`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/huiqi_cole_methods.bas` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/huiqi_cole_methods.bas`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/uk_who_0_20_preterm.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/uk_who_0_20_preterm.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk-who_resources/uk_who_0_20_term.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk-who_resources/uk_who_0_20_term.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk90_child.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk90_child.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk90_preterm.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk90_preterm.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk90_term.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk90_term.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/RCPCH weight correlation matrix by month.csv` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/RCPCH weight correlation matrix by month.csv`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/RCPCH weight correlation matrix by week.csv` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/RCPCH weight correlation matrix by week.csv`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_month.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_month.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_month.py` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_month.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_week.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/uk_who_weight_correlation_matrices/weight_correlation_by_week.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/who_children.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/who_children.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/data_tables/who_infants.json` & `rcpchgrowth-4.0.1/rcpchgrowth/data_tables/who_infants.json`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/date_calculations.py` & `rcpchgrowth-4.0.1/rcpchgrowth/date_calculations.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,61 +8,62 @@
 5 functions to calculate age related parameters
  - chronological_decimal_age: returns a decimal age from 2 dates (takes birth_date and observation_date)
  - corrected_decimal_age: returns a corrected decimal age accounting for prematurity (takes birth_date: date, observation_date: date, gestation_weeks: int, gestation_days: int, pregnancy_length_day [optional])
  - chronological_calendar_age: returns a calendar age as a string (takes birth_date or estimated_date_delivery and observation_date)
  - estimated_date_delivery: returns estimated date of delivery in a known premature infant (takes birth_date, gestation_weeks, gestation_days, pregnancy_length_days[optional])
 """
 
-def chronological_decimal_age(birth_date: date, observation_date: date) -> float:
 
+def chronological_decimal_age(birth_date: date, observation_date: date) -> float:
     """
     Calculates a decimal age from two dates supplied as raw dates without times.
     Returns value floating point
     :param birth_date: date of birth
     :param observation_date: date observation made
     """
 
     days_between = observation_date - birth_date
     chronological_decimal_age = days_between.days / 365.25
     return chronological_decimal_age
-    
 
-def corrected_decimal_age(birth_date: date, observation_date: date, gestation_weeks: int, gestation_days: int)->float: 
+
+def corrected_decimal_age(
+    birth_date: date, observation_date: date, gestation_weeks: int, gestation_days: int
+) -> float:
     """
     Corrects for gestational age across the life course, including term.
     Any baby 37-42 weeks returns decimal age of 0.0
     Depends on chronological_decimal_age
     :param birth_date: date of birth
     :param observation_date: date observation made
     :param gestation_weeks: weeks of gestation up to 40
     :param gestation_days: days in excess of weeks
     """
 
     if birth_date > observation_date:
         raise Exception("Birth date cannot be after the date of observation.")
-    
+
     correction_days = 0
     pregnancy_length_days = TERM_PREGNANCY_LENGTH_DAYS
 
     if gestation_weeks == 0:
         gestation_weeks = 40
         gestation_days = 0
-        
+
     pregnancy_length_days = (gestation_weeks * 7) + gestation_days
 
     ## age correction
     correction_days = TERM_PREGNANCY_LENGTH_DAYS - pregnancy_length_days
     edd = birth_date + timedelta(days=correction_days)
-    corrected_age =  chronological_decimal_age(edd, observation_date)
+    corrected_age = chronological_decimal_age(edd, observation_date)
 
     return corrected_age
 
 
 def chronological_calendar_age(birth_date: date, observation_date: date) -> str:
-    
     """
     returns age in years, months, weeks and days: to return a corrected calendar age use passes EDD instead of birth date
     """
 
     if birth_date > observation_date:
         raise Exception("Birth date cannot be after the date of observation.")
 
@@ -82,77 +83,80 @@
         date_string.append(str(months) + " months")
     if months == 1:
         date_string.append(str(months) + " month")
     if days == 1:
         date_string.append(str(days) + " day")
     if days > 1:
         if weeks > 0:
-            remainingdays = days - (weeks*7)
+            remainingdays = days - (weeks * 7)
             if weeks == 1:
                 date_string.append(str(weeks) + " week")
             elif weeks > 1:
                 date_string.append(str(weeks) + " weeks")
             if remainingdays == 1:
                 date_string.append(str(remainingdays) + " day")
             if remainingdays > 1:
                 date_string.append(str(remainingdays) + " days")
         else:
             date_string.append(str(days) + " days")
     if len(date_string) > 1:
-        return (', '.join(date_string[:-1])) + ' and ' + date_string[-1]
+        return (", ".join(date_string[:-1])) + " and " + date_string[-1]
     elif len(date_string) == 1:
         return date_string[0]
     elif birth_date == observation_date:
-        return 'Happy Birthday'
+        return "Birth date is today."
     else:
-        return ''
+        return ""
 
 
-def estimated_date_delivery(birth_date: date, gestation_weeks: int, gestation_days: int) -> date:
+def estimated_date_delivery(
+    birth_date: date, gestation_weeks: int, gestation_days: int
+) -> date:
     """
     Returns estimated date of delivery from gestational age and birthdate
     Will still calculate an estimated date of delivery if already term (>37 weeks)
     """
 
     pregnancy_length_days = TERM_PREGNANCY_LENGTH_DAYS
 
     if gestation_weeks > 0:
         pregnancy_length_days = (gestation_weeks * 7) + gestation_days
-    
+
     prematurity = TERM_PREGNANCY_LENGTH_DAYS - pregnancy_length_days
 
     edd = birth_date + timedelta(days=prematurity)
     return edd
 
 
-def corrected_gestational_age(birth_date: date, observation_date: date, gestation_weeks: int, gestation_days: int)->str:
+def corrected_gestational_age(
+    birth_date: date, observation_date: date, gestation_weeks: int, gestation_days: int
+) -> str:
     """
     Returns a corrected gestational age
     """
     edd = estimated_date_delivery(birth_date, gestation_weeks, gestation_days)
     forty_two_weeks_gestation_date = edd + timedelta(days=14)
 
     if observation_date >= forty_two_weeks_gestation_date:
-        #beyond 2 weeks post term - chronological age measured in days / weeks / months years
-        #no correction
-        return {
-            "corrected_gestation_weeks": None,
-            "corrected_gestation_days": None
-        }
-    
+        # beyond 2 weeks post term - chronological age measured in days / weeks / months years
+        # no correction
+        return {"corrected_gestation_weeks": None, "corrected_gestation_days": None}
+
     pregnancy_length_days = (gestation_weeks * 7) + gestation_days
     time_alive = observation_date - birth_date
     days_of_life = time_alive.days
     days_since_conception = days_of_life + pregnancy_length_days
 
     corrected_weeks = math.floor(days_since_conception / 7)
     corrected_supplementary_days = days_since_conception - (corrected_weeks * 7)
 
-    if (corrected_weeks == 42 and corrected_supplementary_days > 0) or corrected_weeks > 42:
-        # corrected gestational age will not be returned beyond 42 weeks
+    if (
+        corrected_weeks == 42 and corrected_supplementary_days > 0
+    ) or corrected_weeks > 42:
+        # corrected gestational age will not be returned beyond 42 weeks
         corrected_weeks = None
         corrected_supplementary_days = None
 
     return {
-        'corrected_gestation_weeks': corrected_weeks,
-        'corrected_gestation_days': corrected_supplementary_days
+        "corrected_gestation_weeks": corrected_weeks,
+        "corrected_gestation_days": corrected_supplementary_days,
     }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/dynamic_growth.py` & `rcpchgrowth-4.0.1/rcpchgrowth/dynamic_growth.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/fictional_child.py` & `rcpchgrowth-4.0.1/rcpchgrowth/fictional_child.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/global_functions.py` & `rcpchgrowth-4.0.1/rcpchgrowth/global_functions.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/measurement.py` & `rcpchgrowth-4.0.1/rcpchgrowth/measurement.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/tests/test_dates.py` & `rcpchgrowth-4.0.1/rcpchgrowth/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/tests/test_global_functions.py` & `rcpchgrowth-4.0.1/rcpchgrowth/tests/test_global_functions.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/tests/test_measurement_class.py` & `rcpchgrowth-4.0.1/rcpchgrowth/tests/test_measurement_class.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/trisomy_21.py` & `rcpchgrowth-4.0.1/rcpchgrowth/trisomy_21.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/turner.py` & `rcpchgrowth-4.0.1/rcpchgrowth/turner.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth/uk_who.py` & `rcpchgrowth-4.0.1/rcpchgrowth/uk_who.py`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth.egg-info/PKG-INFO` & `rcpchgrowth-4.0.1/rcpchgrowth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcpchgrowth
-Version: 4.0.0
+Version: 4.0.1
 Summary: SDS and Centile calculations for UK Growth Data
 Home-page: https://github.com/rcpch/digital-growth-charts/blob/master/README.md
 Author: @eatyourpeas, @marcusbaw, @statist7, RCPCH Incubator
 Author-email: incubator@rcpch.ac.uk
 Project-URL: Bug Reports, https://github.com/rcpch/rcpchgrowth-python/issues
 Project-URL: API management, https://dev.rcpch.ac.uk
 Project-URL: Source, https://github.com/rcpch/rcpchgrowth-python
```

### Comparing `rcpchgrowth-4.0.0/rcpchgrowth.egg-info/SOURCES.txt` & `rcpchgrowth-4.0.1/rcpchgrowth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcpchgrowth-4.0.0/setup.py` & `rcpchgrowth-4.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="rcpchgrowth",
-    version="4.0.0",
+    version="4.0.1",
     description="SDS and Centile calculations for UK Growth Data",
     long_description=long_description,
     url="https://github.com/rcpch/digital-growth-charts/blob/master/README.md",
     author="@eatyourpeas, @marcusbaw, @statist7, RCPCH Incubator",
     author_email="incubator@rcpch.ac.uk",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

