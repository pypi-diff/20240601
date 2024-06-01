# Comparing `tmp/chalkpy-2.9.8.tar.gz` & `tmp/chalkpy-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalkpy-2.9.8.tar", last modified: Wed Jun 21 22:13:40 2023, max compression
+gzip compressed data, was "chalkpy-2.9.9.tar", last modified: Thu Jun 22 18:40:58 2023, max compression
```

## Comparing `chalkpy-2.9.8.tar` & `chalkpy-2.9.9.tar`

### file list

```diff
@@ -1,944 +1,944 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.507605 chalkpy-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-21 22:13:21.000000 chalkpy-2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-06-21 22:13:40.507605 chalkpy-2.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-21 22:13:21.000000 chalkpy-2.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.395606 chalkpy-2.9.8/chalk/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.395606 chalkpy-2.9.8/chalk/_autosql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_autosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_autosql/autosql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.395606 chalkpy-2.9.8/chalk/_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)    17401 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_monitoring/Chart.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_monitoring/charts_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_monitoring/charts_enums_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_monitoring/charts_series_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_monitoring/gql_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.395606 chalkpy-2.9.8/chalk/_reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_reporting/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_reporting/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/_reporting/rich/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_reporting/rich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_reporting/rich/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_reporting/rich/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_reporting/rich/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_validation/feature_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/client/
--rw-r--r--   0 runner    (1001) docker     (123)    48783 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61821 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/client/client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/client/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27925 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/client/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/client/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/client/serialization/query_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/clogging/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/clogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/clogging/chalk_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/config/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/config/project_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/df/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/df/ChalkDataFrameImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/df/ast_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/feature_n/
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/feature_n/feature_1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_1/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/feature_n/feature_10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_10/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/feature_n/feature_100/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_100/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_100/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/feature_n/feature_101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_101/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/feature_n/feature_102/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_102/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_102/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/feature_n/feature_103/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_103/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_103/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.399606 chalkpy-2.9.8/chalk/feature_n/feature_104/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_104/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_104/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_105/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_105/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_105/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_106/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_106/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_106/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_107/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_107/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_107/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_108/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_108/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_108/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_109/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_109/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_109/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_11/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_110/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_110/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_110/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_111/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_111/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_111/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_112/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_112/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_112/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_113/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_113/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_113/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_114/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_115/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_115/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_115/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_116/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_116/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_116/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_117/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_117/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_117/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_118/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_118/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_118/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_119/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_119/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_119/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.403606 chalkpy-2.9.8/chalk/feature_n/feature_12/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_12/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_120/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_120/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_120/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_121/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_121/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_121/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_122/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_123/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_123/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_123/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_124/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_124/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_124/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_125/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_125/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_125/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_126/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_126/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_126/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_127/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_127/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_127/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_128/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_128/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_128/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_129/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_129/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_129/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_13/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_13/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_130/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_130/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_130/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_131/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_131/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_132/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_132/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_132/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_133/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_133/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_133/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_134/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_134/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_134/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_135/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_135/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_135/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.407606 chalkpy-2.9.8/chalk/feature_n/feature_136/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_136/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_136/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_137/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_137/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_137/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_138/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_138/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_138/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_139/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_139/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_139/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_14/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_14/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_14/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_140/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_140/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_140/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_141/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_141/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_141/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_142/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_142/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_142/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_143/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_143/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_143/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_144/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_144/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_144/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_145/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_145/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_145/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_146/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_146/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_146/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_147/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_147/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_147/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_148/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_148/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_148/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_149/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_149/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_149/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_15/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_15/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.411606 chalkpy-2.9.8/chalk/feature_n/feature_150/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_150/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_150/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.415606 chalkpy-2.9.8/chalk/feature_n/feature_151/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_151/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_151/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.415606 chalkpy-2.9.8/chalk/feature_n/feature_152/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_152/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_152/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.415606 chalkpy-2.9.8/chalk/feature_n/feature_153/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_153/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_153/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.415606 chalkpy-2.9.8/chalk/feature_n/feature_154/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_154/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_154/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.415606 chalkpy-2.9.8/chalk/feature_n/feature_155/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_155/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_155/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.419606 chalkpy-2.9.8/chalk/feature_n/feature_156/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_156/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_156/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.419606 chalkpy-2.9.8/chalk/feature_n/feature_157/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_157/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_157/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.419606 chalkpy-2.9.8/chalk/feature_n/feature_158/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_158/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_158/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.419606 chalkpy-2.9.8/chalk/feature_n/feature_159/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_159/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_159/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.419606 chalkpy-2.9.8/chalk/feature_n/feature_16/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_16/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.423606 chalkpy-2.9.8/chalk/feature_n/feature_160/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_160/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_160/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.423606 chalkpy-2.9.8/chalk/feature_n/feature_161/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_161/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_161/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.423606 chalkpy-2.9.8/chalk/feature_n/feature_162/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_162/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_162/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.423606 chalkpy-2.9.8/chalk/feature_n/feature_163/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_163/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_163/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.423606 chalkpy-2.9.8/chalk/feature_n/feature_164/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_164/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_164/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.427606 chalkpy-2.9.8/chalk/feature_n/feature_165/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_165/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_165/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.427606 chalkpy-2.9.8/chalk/feature_n/feature_166/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_166/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_166/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.427606 chalkpy-2.9.8/chalk/feature_n/feature_167/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_167/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_167/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.427606 chalkpy-2.9.8/chalk/feature_n/feature_168/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_168/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_168/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.431606 chalkpy-2.9.8/chalk/feature_n/feature_169/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_169/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_169/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.431606 chalkpy-2.9.8/chalk/feature_n/feature_17/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_17/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_17/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.431606 chalkpy-2.9.8/chalk/feature_n/feature_170/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_170/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_170/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.431606 chalkpy-2.9.8/chalk/feature_n/feature_171/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_171/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_171/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.431606 chalkpy-2.9.8/chalk/feature_n/feature_172/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_172/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_172/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.435606 chalkpy-2.9.8/chalk/feature_n/feature_173/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_173/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_173/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.435606 chalkpy-2.9.8/chalk/feature_n/feature_174/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_174/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_174/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.435606 chalkpy-2.9.8/chalk/feature_n/feature_175/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_175/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_175/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.435606 chalkpy-2.9.8/chalk/feature_n/feature_176/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_176/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_176/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.435606 chalkpy-2.9.8/chalk/feature_n/feature_177/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_177/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_177/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.439606 chalkpy-2.9.8/chalk/feature_n/feature_178/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_178/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_178/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.439606 chalkpy-2.9.8/chalk/feature_n/feature_179/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_179/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_179/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.439606 chalkpy-2.9.8/chalk/feature_n/feature_18/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_18/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_18/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.439606 chalkpy-2.9.8/chalk/feature_n/feature_180/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_180/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_180/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_181/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_181/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_181/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_182/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_182/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_182/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_183/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_183/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_183/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_184/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_184/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_184/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_185/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_185/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_185/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_186/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_186/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_186/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_187/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_187/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_187/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_188/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_188/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_188/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_189/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_189/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_189/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_19/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_19/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_19/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_190/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_190/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_190/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_191/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_191/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_191/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_192/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_192/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_192/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.443606 chalkpy-2.9.8/chalk/feature_n/feature_193/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_193/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_193/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_194/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_194/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_194/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_195/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_195/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_195/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_196/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_196/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_196/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_197/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_197/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_197/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_198/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_198/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_198/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_199/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_199/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_199/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_2/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_20/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_200/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_200/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_201/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_201/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_201/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_202/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_202/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_202/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_203/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_203/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_203/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_204/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_204/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_204/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_205/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_205/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_206/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_206/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_206/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_207/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_207/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_207/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.447605 chalkpy-2.9.8/chalk/feature_n/feature_208/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_208/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_208/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_209/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_21/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_21/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_210/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_211/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_211/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_211/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_212/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_212/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_212/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_213/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_213/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_213/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_214/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_214/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_214/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_215/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_215/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_215/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_216/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_216/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_216/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_217/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_217/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_217/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_218/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_218/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_218/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_219/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_219/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_219/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_22/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_220/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_220/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_221/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_221/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_221/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_222/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_222/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_222/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_223/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_223/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_223/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.451605 chalkpy-2.9.8/chalk/feature_n/feature_224/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_224/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_224/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_225/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_225/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_225/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_226/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_226/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_226/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_227/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_227/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_227/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_228/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_228/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_228/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_229/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_229/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_229/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_23/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_230/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_230/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_230/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_231/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_231/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_231/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_232/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_232/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_232/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_233/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_233/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_233/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_234/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_234/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_234/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_235/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_235/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_235/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_236/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_236/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_236/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_237/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_237/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_237/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_238/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_238/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_238/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_239/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_239/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_239/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.455606 chalkpy-2.9.8/chalk/feature_n/feature_24/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_24/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_240/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_240/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_241/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_241/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_241/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_242/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_242/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_242/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_243/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_243/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_243/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_244/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_244/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_244/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_245/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_245/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_245/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_246/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_246/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_246/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_247/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_247/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_247/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_248/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_248/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_248/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_249/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_249/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_249/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_25/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_25/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_250/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_250/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_250/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_251/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_251/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_251/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_252/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_252/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_252/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_253/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_253/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_253/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.459606 chalkpy-2.9.8/chalk/feature_n/feature_254/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_254/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_254/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_255/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_255/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_255/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_256/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_256/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_256/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_26/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_26/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_27/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_27/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_27/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_28/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_28/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_28/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_29/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_29/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_29/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_3/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_30/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_30/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_30/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_31/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_31/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_31/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_32/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_32/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_33/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_34/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_34/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_34/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_35/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_35/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_35/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_36/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_36/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_36/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_37/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_37/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_37/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_38/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_38/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_38/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_39/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_39/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_39/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.463605 chalkpy-2.9.8/chalk/feature_n/feature_4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_4/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_40/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_40/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_41/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_41/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_41/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_42/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_42/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_42/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_43/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_43/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_43/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_44/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_44/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_44/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_45/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_45/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_45/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_46/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_46/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_46/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_47/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_47/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_47/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_48/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_48/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_48/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_49/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_49/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_49/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_5/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_50/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_50/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_50/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_51/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_51/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_51/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_52/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_52/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_52/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_53/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_53/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_54/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_54/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_54/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.467605 chalkpy-2.9.8/chalk/feature_n/feature_55/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_55/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_55/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_56/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_56/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_57/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_57/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_57/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_58/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_58/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_58/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_59/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_59/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_59/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_6/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_60/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_60/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_60/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_61/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_61/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_61/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_62/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_62/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_62/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_63/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_63/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_63/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_64/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_64/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_64/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_65/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_65/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_65/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_66/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_66/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_66/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_67/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_67/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_67/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_68/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_68/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_68/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_69/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_69/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_69/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_7/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.471605 chalkpy-2.9.8/chalk/feature_n/feature_70/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_70/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_70/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_71/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_71/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_71/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_72/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_72/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_72/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_73/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_73/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_73/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_74/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_74/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_74/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_75/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_75/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_75/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_76/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_76/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_76/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_77/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_77/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_77/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_78/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_78/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_78/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_79/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_79/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_79/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_8/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_80/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_80/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_80/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_81/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_81/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_81/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_82/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_82/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_82/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_83/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_83/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_83/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_84/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_84/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_84/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_85/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_85/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_85/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.475605 chalkpy-2.9.8/chalk/feature_n/feature_86/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_86/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_86/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_87/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_87/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_87/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_88/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_88/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_88/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_89/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_89/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_89/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_9/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_90/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_90/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_90/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_91/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_91/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_91/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_92/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_92/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_92/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_93/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_93/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_93/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_94/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_94/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_94/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_95/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_95/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_95/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_96/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_96/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_96/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_97/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_97/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_97/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_98/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_98/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_98/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.479606 chalkpy-2.9.8/chalk/feature_n/feature_99/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_99/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/feature_n/feature_99/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.483605 chalkpy-2.9.8/chalk/features/
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_chalkop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_class_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.483605 chalkpy-2.9.8/chalk/features/_encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/missing_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/_encoding/serialized_dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.483605 chalkpy-2.9.8/chalk/features/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22208 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/dataframe/_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    66535 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/dataframe/_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/dataframe/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    33411 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/feature_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/feature_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/feature_set_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/feature_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/feature_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/live_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/primary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/pseudofeatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    73224 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/features/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.491605 chalkpy-2.9.8/chalk/gitignore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/gitignore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/gitignore/gitignore_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/gitignore/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.491605 chalkpy-2.9.8/chalk/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/integrations/named.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.491605 chalkpy-2.9.8/chalk/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.491605 chalkpy-2.9.8/chalk/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/mypy_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.495605 chalkpy-2.9.8/chalk/parsed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/parsed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/parsed/_graph_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/parsed/branch_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/parsed/branch_state_rich.py
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/parsed/duplicate_input_gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    13647 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/parsed/json_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/parsed/user_types_to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.495605 chalkpy-2.9.8/chalk/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/serialization/parsed_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.495605 chalkpy-2.9.8/chalk/sink/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sink/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.495605 chalkpy-2.9.8/chalk/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    30317 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.495605 chalkpy-2.9.8/chalk/sql/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/incremental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.499605 chalkpy-2.9.8/chalk/sql/_internal/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/cloudsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.499605 chalkpy-2.9.8/chalk/sql/_internal/integrations/psycopg3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/psycopg3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/integrations/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    24588 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/sql_file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21054 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/sql_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/_internal/string_chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/finalized_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    22108 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/sql/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.499605 chalkpy-2.9.8/chalk/streams/
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/streams/_file_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/streams/_kafka_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/streams/_kinesis_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/streams/_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/streams/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/streams/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.503605 chalkpy-2.9.8/chalk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.507605 chalkpy-2.9.8/chalk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/annotation_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/async_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/cached_type_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/collection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/environment_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/log_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/metaprogramming.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/missing_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-06-21 22:13:21.000000 chalkpy-2.9.8/chalk/utils/stubgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:40.507605 chalkpy-2.9.8/chalkpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-21 22:13:40.000000 chalkpy-2.9.8/chalkpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-06-21 22:13:21.000000 chalkpy-2.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:13:40.507605 chalkpy-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 22:13:21.000000 chalkpy-2.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.268378 chalkpy-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-22 18:40:37.000000 chalkpy-2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-06-22 18:40:58.268378 chalkpy-2.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-22 18:40:37.000000 chalkpy-2.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.156377 chalkpy-2.9.9/chalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.156377 chalkpy-2.9.9/chalk/_autosql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_autosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_autosql/autosql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.160378 chalkpy-2.9.9/chalk/_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)    17401 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_monitoring/Chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_monitoring/charts_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_monitoring/charts_enums_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_monitoring/charts_series_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_monitoring/gql_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.160378 chalkpy-2.9.9/chalk/_reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_reporting/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_reporting/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.160378 chalkpy-2.9.9/chalk/_reporting/rich/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_reporting/rich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_reporting/rich/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_reporting/rich/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_reporting/rich/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.160378 chalkpy-2.9.9/chalk/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_validation/feature_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    48917 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62843 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/client/client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/client/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28344 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/client/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/client/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/client/serialization/query_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/clogging/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/clogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/clogging/chalk_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/config/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/config/project_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/df/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/df/ChalkDataFrameImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/df/ast_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/feature_n/
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/feature_n/feature_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_1/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/feature_n/feature_10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_10/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/feature_n/feature_100/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_100/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_100/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/feature_n/feature_101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_101/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.164378 chalkpy-2.9.9/chalk/feature_n/feature_102/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_102/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_102/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_103/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_103/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_103/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_104/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_104/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_104/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_105/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_105/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_105/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_106/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_106/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_106/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_107/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_107/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_107/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_108/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_108/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_108/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_109/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_109/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_109/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_11/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_110/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_110/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_110/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_111/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_111/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_111/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_112/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_112/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_112/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.168377 chalkpy-2.9.9/chalk/feature_n/feature_113/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_113/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_113/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_114/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_115/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_115/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_115/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_116/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_116/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_116/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_117/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_117/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_117/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_118/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_118/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_118/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_119/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_119/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_119/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_12/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_120/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_120/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_120/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_121/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_121/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_121/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_122/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_123/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_123/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_123/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_124/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_124/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_124/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.172378 chalkpy-2.9.9/chalk/feature_n/feature_125/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_125/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_125/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_126/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_126/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_126/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_127/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_127/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_127/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_128/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_128/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_128/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_129/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_129/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_129/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_13/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_13/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_130/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_130/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_130/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_131/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_131/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_132/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_132/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_132/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_133/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_133/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_133/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_134/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_134/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_134/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_135/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_135/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_135/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.176378 chalkpy-2.9.9/chalk/feature_n/feature_136/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_136/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_136/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_137/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_137/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_137/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_138/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_138/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_138/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_139/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_139/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_139/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_14/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_14/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_14/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_140/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_140/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_140/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_141/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_141/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_141/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_142/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_142/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_142/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_143/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_143/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_143/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_144/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_144/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_144/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_145/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_145/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_145/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_146/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_146/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_146/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_147/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_147/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_147/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.180378 chalkpy-2.9.9/chalk/feature_n/feature_148/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_148/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_148/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_149/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_149/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_149/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_15/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_15/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_150/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_150/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_150/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_151/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_151/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_151/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_152/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_152/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_152/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_153/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_153/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_153/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_154/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_154/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_154/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_155/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_155/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_155/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_156/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_156/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_156/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_157/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_157/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_157/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_158/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_158/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_158/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.184378 chalkpy-2.9.9/chalk/feature_n/feature_159/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_159/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_159/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_16/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_16/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_160/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_161/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_161/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_161/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_162/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_162/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_162/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_163/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_163/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_163/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_164/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_164/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_164/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_165/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_165/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_165/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_166/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_166/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_166/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_167/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_167/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_167/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_168/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_168/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_168/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.188378 chalkpy-2.9.9/chalk/feature_n/feature_169/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_169/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_169/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_17/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_17/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_17/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_170/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_170/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_170/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_171/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_171/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_171/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_172/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_172/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_172/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_173/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_173/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_173/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_174/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_174/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_174/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_175/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_175/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_175/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_176/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_176/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_176/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_177/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_177/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_177/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.192378 chalkpy-2.9.9/chalk/feature_n/feature_178/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_178/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_178/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_179/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_179/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_179/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_18/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_18/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_18/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_180/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_180/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_180/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_181/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_181/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_181/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_182/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_182/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_182/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_183/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_183/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_183/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_184/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_184/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_184/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_185/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_185/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_185/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_186/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_186/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_186/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_187/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_187/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_187/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.196378 chalkpy-2.9.9/chalk/feature_n/feature_188/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_188/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_188/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_189/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_189/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_189/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_19/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_19/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_19/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_190/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_190/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_190/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_191/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_191/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_191/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_192/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_192/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_192/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_193/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_193/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_193/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_194/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_194/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_194/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_195/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_195/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_195/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_196/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_196/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_196/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_197/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_197/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_197/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_198/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_198/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_198/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.200378 chalkpy-2.9.9/chalk/feature_n/feature_199/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_199/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_199/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_2/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_20/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_200/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_200/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_201/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_201/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_201/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_202/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_202/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_202/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_203/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_203/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_203/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_204/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_204/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_204/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_205/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_205/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_206/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_206/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_206/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_207/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_207/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_207/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.204378 chalkpy-2.9.9/chalk/feature_n/feature_208/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_208/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_208/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_209/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_21/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_210/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_211/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_211/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_211/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_212/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_212/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_212/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_213/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_213/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_213/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_214/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_214/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_214/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_215/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_215/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_215/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_216/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_216/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_216/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_217/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_217/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_217/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_218/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_218/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_218/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.208378 chalkpy-2.9.9/chalk/feature_n/feature_219/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_219/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_219/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_22/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_220/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_221/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_221/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_221/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_222/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_222/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_222/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_223/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_223/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_223/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_224/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_224/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_224/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_225/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_225/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_225/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_226/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_226/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_226/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_227/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_227/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_227/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_228/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_228/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_228/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_229/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_229/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_229/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_23/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.212378 chalkpy-2.9.9/chalk/feature_n/feature_230/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_230/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_230/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_231/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_231/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_231/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_232/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_232/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_232/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_233/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_233/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_233/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_234/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_234/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_234/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_235/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_235/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_235/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_236/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_236/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_236/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_237/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_237/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_237/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_238/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_238/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_238/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_239/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_239/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_239/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_24/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_24/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_240/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_240/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.216378 chalkpy-2.9.9/chalk/feature_n/feature_241/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_241/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_241/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_242/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_242/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_242/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_243/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_243/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_243/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_244/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_244/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_244/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_245/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_245/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_245/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_246/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_246/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_246/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_247/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_247/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_247/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_248/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_248/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_248/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_249/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_249/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_249/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_25/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_25/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.220378 chalkpy-2.9.9/chalk/feature_n/feature_250/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_250/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_250/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_251/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_251/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_251/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_252/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_252/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_252/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_253/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_253/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_253/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_254/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_254/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_254/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_255/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_255/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_255/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_256/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_256/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_256/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_26/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_26/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_27/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_27/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_27/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_28/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_28/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_28/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_29/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_29/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_29/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_3/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.224378 chalkpy-2.9.9/chalk/feature_n/feature_30/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_30/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_30/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_31/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_31/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_31/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_32/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_32/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_33/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_34/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_34/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_34/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_35/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_35/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_35/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_36/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_36/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_36/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_37/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_37/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_38/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_38/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_38/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_39/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_39/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_39/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_4/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_40/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_40/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_41/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_41/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_41/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.228378 chalkpy-2.9.9/chalk/feature_n/feature_42/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_42/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_42/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_43/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_43/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_43/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_44/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_44/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_44/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_45/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_45/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_45/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_46/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_46/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_46/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_47/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_47/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_47/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_48/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_48/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_48/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_49/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_49/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_49/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_5/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_50/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_50/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_51/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_51/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_51/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_52/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_52/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_52/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.232378 chalkpy-2.9.9/chalk/feature_n/feature_53/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_53/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_54/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_54/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_54/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_55/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_55/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_55/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_56/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_56/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_57/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_57/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_57/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_58/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_58/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_58/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_59/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_59/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_59/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_6/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_60/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_60/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_60/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_61/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_61/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_61/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_62/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_62/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_62/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_63/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_63/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_63/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_64/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_64/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.236378 chalkpy-2.9.9/chalk/feature_n/feature_65/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_65/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_65/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_66/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_66/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_66/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_67/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_67/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_67/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_68/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_68/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_68/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_69/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_69/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_69/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_7/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_70/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_70/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_70/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_71/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_71/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_71/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_72/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_72/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_72/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_73/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_73/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_73/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_74/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_74/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_74/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_75/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_75/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_75/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.240378 chalkpy-2.9.9/chalk/feature_n/feature_76/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_76/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_76/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_77/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_77/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_77/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_78/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_78/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_78/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_79/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_79/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_79/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_8/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_80/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_80/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_80/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_81/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_81/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_81/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_82/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_82/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_82/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_83/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_83/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_83/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_84/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_84/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_84/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_85/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_85/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_85/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_86/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_86/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_86/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_87/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_87/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_87/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.244378 chalkpy-2.9.9/chalk/feature_n/feature_88/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_88/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_88/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_89/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_89/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_89/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_9/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_90/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_90/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_90/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_91/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_91/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_91/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_92/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_92/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_92/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_93/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_93/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_93/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_94/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_94/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_94/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_95/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_95/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_95/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_96/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_96/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_96/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_97/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_97/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_97/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_98/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_98/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_98/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.248378 chalkpy-2.9.9/chalk/feature_n/feature_99/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_99/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/feature_n/feature_99/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.252378 chalkpy-2.9.9/chalk/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_chalkop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_class_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.256378 chalkpy-2.9.9/chalk/features/_encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/missing_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/_encoding/serialized_dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.256378 chalkpy-2.9.9/chalk/features/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22208 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/dataframe/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66535 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/dataframe/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/dataframe/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33411 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/feature_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/feature_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/feature_set_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/feature_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/feature_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/live_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/pseudofeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73224 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/features/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.256378 chalkpy-2.9.9/chalk/gitignore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/gitignore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/gitignore/gitignore_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/gitignore/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.256378 chalkpy-2.9.9/chalk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/integrations/named.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.256378 chalkpy-2.9.9/chalk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.256378 chalkpy-2.9.9/chalk/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/mypy_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.260378 chalkpy-2.9.9/chalk/parsed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/parsed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/parsed/_graph_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/parsed/branch_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/parsed/branch_state_rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/parsed/duplicate_input_gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13647 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/parsed/json_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/parsed/user_types_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.260378 chalkpy-2.9.9/chalk/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/serialization/parsed_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.260378 chalkpy-2.9.9/chalk/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sink/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.260378 chalkpy-2.9.9/chalk/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    30317 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.260378 chalkpy-2.9.9/chalk/sql/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.260378 chalkpy-2.9.9/chalk/sql/_internal/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/cloudsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.264378 chalkpy-2.9.9/chalk/sql/_internal/integrations/psycopg3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/psycopg3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/integrations/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24588 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/sql_file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21054 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/sql_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/_internal/string_chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/finalized_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22108 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/sql/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.264378 chalkpy-2.9.9/chalk/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/streams/_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/streams/_kafka_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/streams/_kinesis_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/streams/_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/streams/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/streams/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.264378 chalkpy-2.9.9/chalk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.268378 chalkpy-2.9.9/chalk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/annotation_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/cached_type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/environment_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/log_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/metaprogramming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/missing_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-06-22 18:40:37.000000 chalkpy-2.9.9/chalk/utils/stubgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:40:58.268378 chalkpy-2.9.9/chalkpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-22 18:40:58.000000 chalkpy-2.9.9/chalkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-06-22 18:40:37.000000 chalkpy-2.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:40:58.268378 chalkpy-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 18:40:37.000000 chalkpy-2.9.9/setup.py
```

### Comparing `chalkpy-2.9.8/PKG-INFO` & `chalkpy-2.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalkpy
-Version: 2.9.8
+Version: 2.9.9
 Summary: Python SDK for Chalk
 Author: Chalk AI, Inc.
 Project-URL: homepage, https://chalk.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `chalkpy-2.9.8/README.md` & `chalkpy-2.9.9/README.md`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/__init__.py` & `chalkpy-2.9.9/chalk/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_autosql/autosql.py` & `chalkpy-2.9.9/chalk/_autosql/autosql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_monitoring/Chart.py` & `chalkpy-2.9.9/chalk/_monitoring/Chart.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_monitoring/charts_codegen.py` & `chalkpy-2.9.9/chalk/_monitoring/charts_codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_monitoring/charts_enums_codegen.py` & `chalkpy-2.9.9/chalk/_monitoring/charts_enums_codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_monitoring/charts_series_base.py` & `chalkpy-2.9.9/chalk/_monitoring/charts_series_base.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_monitoring/gql_conversion.py` & `chalkpy-2.9.9/chalk/_monitoring/gql_conversion.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_reporting/models.py` & `chalkpy-2.9.9/chalk/_reporting/models.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_reporting/progress.py` & `chalkpy-2.9.9/chalk/_reporting/progress.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import collections
 import time
 import uuid
 from datetime import datetime, timedelta
 from functools import cached_property
-from typing import Dict, Iterable, Mapping, Optional, cast
+from typing import Dict, Iterable, List, Mapping, Optional, Tuple, cast
 
 from rich import box, get_console
 from rich.console import Group
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.progress import BarColumn, MofNCompleteColumn, Progress, SpinnerColumn, TaskID, TextColumn, TimeElapsedColumn
 from rich.style import Style
@@ -24,14 +25,15 @@
 
 _kind_to_display_type = {
     BatchOpKind.RECOMPUTE: "Dataset Recompute",
     BatchOpKind.OFFLINE_QUERY: "Offline Query",
 }
 
 _MAX_ERRORS_TO_DISPLAY = 10
+_TTableRow = Tuple[str, str]
 
 
 class ProgressService:
     def __init__(self, operation_id: uuid.UUID, client: "ChalkAPIClientImpl", caller_method: Optional[str] = None):
         """
         :param operation_id: The ID of the operation that the ProgressService
             is polling for. This is commonly a `DatasetRevision` ID.
@@ -108,28 +110,81 @@
             rows_done_new = resolver_report.progress.computed + resolver_report.progress.failed
             self.resolver_progress.update(resolver_task_id, completed=rows_done_new)
 
     def handle_success(self, main_task_id: TaskID, operation_display_type: str) -> None:
         self.enclosure_panel.title = "chalk ■"
         self.main_progress.update(main_task_id, description=f"{operation_display_type} completed", completed=1)
 
-    def get_failing_resolver(self, batch_report: BatchReport) -> Optional[str]:
+    def _get_failing_resolver(self, batch_report: BatchReport) -> Optional[str]:
         """
         :return: The name of the resolver that failed, or None if no resolver failed.
         """
         for resolver in batch_report.resolvers:
             if resolver.status == BatchOpStatus.FAILED:
                 return resolver.resolver_fqn
 
+    @staticmethod
+    def _get_pkey_display_value(error: ChalkError) -> Optional[str]:
+        if error.display_primary_key is None:
+            return None
+
+        value = ""
+        if error.display_primary_key_fqn:
+            value += error.display_primary_key_fqn + ": "
+
+        value += error.display_primary_key
+
+        return value
+
+    def _get_error_details(self, errors: List[ChalkError]) -> List[_TTableRow]:
+        if not errors:
+            return [
+                (
+                    "Error Message",
+                    "Unfortunately the cause of this error is unknown. Please contact Chalk for support and provide the Revision ID or the Trace ID above.",
+                )
+            ]
+
+        truncated_from = None
+        if len(errors) > _MAX_ERRORS_TO_DISPLAY:
+            truncated_from = len(errors)
+            errors = errors[:_MAX_ERRORS_TO_DISPLAY]
+
+        t_details_for_one_error = List[_TTableRow]
+        grouped_details: Dict[int, t_details_for_one_error] = collections.defaultdict(list)
+        for i, e in enumerate(errors):
+            grouped_details[i].append((f"Error {i + 1}", e.message) if len(errors) > 1 else ("Error", e.message))
+            if e.exception and e.exception.message:
+                grouped_details[i].append((f"Exception", e.exception.message))
+            if e.exception and e.exception.stacktrace:
+                grouped_details[i].append((f"Stacktrace", e.exception.stacktrace))
+            if val := self._get_pkey_display_value(e):
+                grouped_details[i].append((f"Pkey", val))
+
+        flattened_details = sum(list(grouped_details.values()), [])
+        if truncated_from:
+            flattened_details.append(
+                ("Errors Truncated", f"Displaying only {_MAX_ERRORS_TO_DISPLAY} out of {truncated_from}")
+            )
+
+        return flattened_details
+
     def handle_and_raise_error(
         self,
         batch_report: BatchReport,
         main_task_id: TaskID,
         operation_display_type: str,
     ) -> None:
+        all_errors = batch_report.all_errors or []
+        if not all_errors and batch_report.error:
+            # `all_errors` is added long after `error`.
+            # We might be hitting old server code here,
+            # make sure we can still talk to old server.
+            all_errors.append(batch_report.error)
+
         panel = self.enclosure_panel
         main_progress = self.main_progress
         progress_table = cast(Table, self.enclosure_panel.renderable)
 
         self.handle_explainer_text_if_erring()
         panel.border_style = Style(color="red")
         main_progress.update(
@@ -142,87 +197,21 @@
         }
 
         metadata = batch_report.operation_metadata or {}
         if not isinstance(metadata, Mapping):
             metadata = {}
 
         metadata_tuples = [(key_to_display_key.get(k, k), v) for k, v in metadata.items()]
+        failing_resolver = self._get_failing_resolver(batch_report)
 
-        stacktrace_tuples = []
-        pkey_tuples = []
-
-        def _get_pkey_display_value(error: ChalkError) -> str | None:
-            if error.display_primary_key is None:
-                return None
-
-            value = ""
-            if error.display_primary_key_fqn:
-                value += error.display_primary_key_fqn + ": "
-
-            value += error.display_primary_key
-
-            return value
-
-        truncated_from = None
-        all_errors = batch_report.all_errors or []
-        if not all_errors and batch_report.error:
-            # `all_errors` is added long after `error`.
-            # We might be hitting old server code here,
-            # make sure we can still talk to old server.
-            all_errors.append(batch_report.error)
-
-        if not all_errors:
-            error_tuples = [
-                (
-                    "Error Message",
-                    "Unfortunately the cause of this error is unknown. Please contact Chalk for support and provide the Revision ID or the Trace ID above.",
-                )
-            ]
-        elif len(all_errors) == 1:
-
-            single_error = all_errors[0]
-            error_tuples = [("Error Message", single_error.message)]
-            stacktrace = single_error.exception and single_error.exception.stacktrace
-            stacktrace_tuples = [("Stacktrace", stacktrace)] if stacktrace else [None]
-            pkey_value = _get_pkey_display_value(single_error)
-            pkey_tuples = [("Pkey", pkey_value)] if pkey_value else [None]
-
-        else:
-            if len(all_errors) > _MAX_ERRORS_TO_DISPLAY:
-                truncated_from = len(all_errors)
-            all_errors = all_errors[:_MAX_ERRORS_TO_DISPLAY]
-            error_tuples = [(f"Error {i + 1}", e.message) for i, e in enumerate(all_errors)]
-            stacktrace_tuples = [
-                (f"Stacktrace {i + 1}", e.exception.stacktrace) if (e.exception and e.exception.stacktrace) else None
-                for i, e in enumerate(all_errors)
-            ]
-            pkey_tuples = [
-                (f"Error {i + 1} Pkey", val) if (val := _get_pkey_display_value(e)) else None
-                for i, e in enumerate(all_errors)
-            ]
-
-        grouped_error_pkey_stacktrace_tuples = []
-        for i in range(len(all_errors)):
-            grouped_error_pkey_stacktrace_tuples.append(error_tuples[i])
-            if pkey_tuples[i] is not None:
-                grouped_error_pkey_stacktrace_tuples.append(pkey_tuples[i])
-            if stacktrace_tuples[i] is not None:
-                grouped_error_pkey_stacktrace_tuples.append(stacktrace_tuples[i])
-
-        failing_resolver = self.get_failing_resolver(batch_report)
-        table_contents = [
+        table_contents: List[_TTableRow] = [
             ("Revision ID", str(self.operation_id)),
             *metadata_tuples,
             *([("Failing Resolver", failing_resolver)] if failing_resolver else []),
-            *grouped_error_pkey_stacktrace_tuples,
-            *(
-                [("Errors Truncated", f"Displaying only {_MAX_ERRORS_TO_DISPLAY} out of {truncated_from}")]
-                if truncated_from
-                else []
-            ),
+            *self._get_error_details(all_errors),
         ]
         error_box = Table(
             box=box.SQUARE,
             show_lines=True,
             show_header=False,
             style=Style(color="red"),
             row_styles=[Style(color="red")] * len(table_contents),
```

### Comparing `chalkpy-2.9.8/chalk/_reporting/rich/live.py` & `chalkpy-2.9.9/chalk/_reporting/rich/live.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/_validation/validation.py` & `chalkpy-2.9.9/chalk/_validation/validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/cli.py` & `chalkpy-2.9.9/chalk/cli.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/client/__init__.py` & `chalkpy-2.9.9/chalk/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pandas as pd
 import requests
 from typing_extensions import TypeAlias
 
 from chalk.client.exc import ChalkAuthException, ChalkBaseException
 from chalk.client.models import (
     BranchDeployResponse,
+    BranchIdParam,
     ChalkError,
     ChalkException,
     DatasetFilter,
     ErrorCode,
     ErrorCodeCategory,
     FeatureDropResponse,
     FeatureObservationDeletionResponse,
@@ -1343,14 +1344,17 @@
         >>> from chalk.client import ChalkClient
         >>> client = ChalkClient()
         >>> client.create_branch("my-new-branch")
         >>> client.set_branch("my-new-branch")
         """
         ...
 
+    def reset_branch(self, branch: BranchIdParam = ..., environment: Optional[EnvironmentId] = None):
+        ...
+
     def branch_state(
         self,
         branch: Union[BranchId, Ellipsis] = ...,
         environment: Optional[EnvironmentId] = None,
     ) -> BranchGraphSummary:
         """
         Returns a `chalk.parsed.branch_state.BranchGraphSummary` object that contains the state of the branch server:
```

### Comparing `chalkpy-2.9.8/chalk/client/client_impl.py` & `chalkpy-2.9.9/chalk/client/client_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from chalk._version import __version__ as chalkpy_version
 from chalk.client import ChalkClient, FeatureReference, OnlineQueryResult
 from chalk.client.dataset import DatasetImpl, DatasetVersion, dataset_from_response, load_dataset
 from chalk.client.exc import _CHALK_TRACE_ID_KEY, ChalkAuthException, ChalkBaseException, ChalkCustomException
 from chalk.client.models import (
     BranchDeployRequest,
     BranchDeployResponse,
+    BranchIdParam,
     ChalkError,
     ComputeResolverOutputRequest,
     ComputeResolverOutputResponse,
     CreateOfflineQueryJobRequest,
     CreateOfflineQueryJobResponse,
     DatasetRecomputeRequest,
     DatasetRecomputeResponse,
@@ -1618,14 +1619,37 @@
             api_server_override=self._get_local_server_override(branch),
             response=None,  # get the JSON
             preview_deployment_id=None,
             json=None,
         )
         return result.json()
 
+    def reset_branch(self, branch: BranchIdParam = ..., environment: Optional[EnvironmentId] = None):
+        if branch is Ellipsis:
+            branch = self._config.branch
+        if branch is None:
+            raise RuntimeError("No branch specified or set in client. This method only works for branch deployments.")
+        available_branches = self.get_branches()
+        if branch not in available_branches:
+            raise RuntimeError(
+                f"The branch `{branch}` does not exist. "
+                f"Available branches are: {available_branches}. "
+                f"To create a branch, use `ChalkClient.create_branch(...)`"
+            )
+        self._request(
+            method="POST",
+            uri=f"/v1/branch/{branch}/reset",
+            environment_override=environment,
+            branch=branch,
+            api_server_override=self._get_local_server_override(branch),
+            response=None,
+            preview_deployment_id=None,
+            json=None,
+        )
+
     def branch_state(
         self,
         branch: Union[BranchId, Ellipsis] = ...,
         environment: Optional[EnvironmentId] = None,
     ):
         if branch is Ellipsis:
             branch = self._config.branch
```

### Comparing `chalkpy-2.9.8/chalk/client/dataset.py` & `chalkpy-2.9.9/chalk/client/dataset.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/client/exc.py` & `chalkpy-2.9.9/chalk/client/exc.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/client/models.py` & `chalkpy-2.9.9/chalk/client/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,7 +844,18 @@
 
 class BranchDeployResponse(BaseModel):
     branch_name: str
     new_branch_created: bool
 
     source_deployment_id: str
     branch_deployment_id: str
+
+
+BranchIdParam: TypeAlias = Union[None, str, type(Ellipsis)]
+"""
+Type used for the 'branch' paremeter in calls to the Chalk Client.
+The branch can either be:
+ 1. A string that is used as the branch name for the request
+ 2. None, in which case the request is _not_ sent to a branch server,
+ 3. Ellipsis (...), indicating that the branch name (or lack thereof) is
+    inferred from the ChalkClient's current branch.
+"""
```

### Comparing `chalkpy-2.9.8/chalk/client/serialization/query_serialization.py` & `chalkpy-2.9.9/chalk/client/serialization/query_serialization.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/config/auth_config.py` & `chalkpy-2.9.9/chalk/config/auth_config.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/config/project_config.py` & `chalkpy-2.9.9/chalk/config/project_config.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/df/ast_parser.py` & `chalkpy-2.9.9/chalk/df/ast_parser.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/__init__.py` & `chalkpy-2.9.9/chalk/feature_n/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/codegen.py` & `chalkpy-2.9.9/chalk/feature_n/codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_10/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_10/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_100/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_100/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_101/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_101/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_102/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_102/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_103/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_103/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_104/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_104/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_105/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_105/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_106/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_106/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_107/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_107/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_108/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_108/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_109/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_109/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_11/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_11/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_110/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_110/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_111/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_111/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_112/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_112/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_113/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_113/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_114/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_114/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_115/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_115/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_116/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_116/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_117/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_117/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_118/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_118/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_119/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_119/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_12/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_12/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_120/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_120/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_121/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_121/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_122/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_122/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_123/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_123/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_124/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_124/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_125/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_125/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_126/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_126/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_127/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_127/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_128/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_128/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_129/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_129/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_13/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_13/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_130/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_130/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_131/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_131/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_132/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_132/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_133/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_133/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_134/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_134/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_135/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_135/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_136/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_136/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_137/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_137/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_138/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_138/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_139/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_139/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_14/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_14/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_140/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_140/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_141/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_141/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_142/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_142/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_143/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_143/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_144/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_144/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_145/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_145/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_146/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_146/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_147/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_147/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_148/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_148/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_149/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_149/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_15/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_15/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_150/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_150/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_151/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_151/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_152/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_152/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_153/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_153/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_154/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_154/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_155/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_155/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_156/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_156/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_157/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_157/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_158/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_158/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_159/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_159/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_16/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_16/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_160/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_160/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_161/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_161/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_162/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_162/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_163/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_163/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_164/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_164/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_165/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_165/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_166/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_166/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_167/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_167/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_168/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_168/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_169/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_169/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_17/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_17/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_170/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_170/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_171/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_171/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_172/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_172/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_173/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_173/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_174/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_174/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_175/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_175/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_176/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_176/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_177/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_177/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_178/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_178/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_179/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_179/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_18/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_18/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_180/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_180/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_181/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_181/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_182/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_182/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_183/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_183/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_184/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_184/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_185/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_185/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_186/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_186/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_187/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_187/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_188/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_188/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_189/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_189/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_19/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_19/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_190/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_190/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_191/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_191/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_192/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_192/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_193/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_193/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_194/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_194/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_195/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_195/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_196/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_196/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_197/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_197/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_198/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_198/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_199/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_199/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_20/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_20/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_200/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_200/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_201/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_201/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_202/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_202/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_203/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_203/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_204/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_204/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_205/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_205/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_206/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_206/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_207/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_207/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_208/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_208/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_209/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_209/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_21/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_21/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_210/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_210/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_211/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_211/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_212/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_212/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_213/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_213/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_214/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_214/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_215/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_215/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_216/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_216/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_217/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_217/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_218/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_218/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_219/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_219/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_22/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_22/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_220/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_220/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_221/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_221/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_222/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_222/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_223/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_223/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_224/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_224/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_225/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_225/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_226/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_226/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_227/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_227/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_228/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_228/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_229/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_229/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_23/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_23/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_230/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_230/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_231/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_231/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_232/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_232/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_233/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_233/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_234/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_234/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_235/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_235/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_236/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_236/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_237/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_237/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_238/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_238/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_239/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_239/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_24/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_24/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_240/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_240/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_241/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_241/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_242/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_242/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_243/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_243/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_244/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_244/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_245/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_245/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_246/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_246/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_247/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_247/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_248/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_248/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_249/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_249/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_25/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_25/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_250/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_250/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_251/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_251/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_252/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_252/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_253/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_253/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_254/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_254/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_255/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_255/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_256/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_256/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_26/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_26/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_27/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_27/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_28/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_28/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_29/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_29/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_30/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_30/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_31/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_31/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_32/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_32/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_33/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_33/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_34/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_34/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_35/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_35/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_36/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_36/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_37/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_37/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_38/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_38/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_39/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_39/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_40/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_40/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_41/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_41/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_42/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_42/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_43/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_43/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_44/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_44/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_45/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_45/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_46/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_46/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_47/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_47/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_48/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_48/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_49/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_49/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_50/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_50/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_51/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_51/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_52/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_52/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_53/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_53/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_54/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_54/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_55/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_55/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_56/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_56/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_57/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_57/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_58/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_58/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_59/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_59/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_60/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_60/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_61/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_61/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_62/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_62/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_63/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_63/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_64/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_64/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_65/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_65/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_66/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_66/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_67/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_67/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_68/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_68/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_69/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_69/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_7/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_7/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_70/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_70/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_71/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_71/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_72/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_72/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_73/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_73/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_74/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_74/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_75/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_75/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_76/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_76/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_77/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_77/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_78/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_78/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_79/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_79/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_8/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_8/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_80/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_80/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_81/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_81/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_82/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_82/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_83/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_83/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_84/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_84/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_85/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_85/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_86/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_86/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_87/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_87/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_88/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_88/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_89/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_89/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_9/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_9/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_90/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_90/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_91/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_91/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_92/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_92/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_93/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_93/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_94/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_94/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_95/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_95/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_96/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_96/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_97/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_97/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_98/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_98/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/feature_n/feature_99/feature.py` & `chalkpy-2.9.9/chalk/feature_n/feature_99/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/__init__.py` & `chalkpy-2.9.9/chalk/features/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_chalkop.py` & `chalkpy-2.9.9/chalk/features/_chalkop.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_class_property.py` & `chalkpy-2.9.9/chalk/features/_class_property.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_encoding/converter.py` & `chalkpy-2.9.9/chalk/features/_encoding/converter.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_encoding/inputs.py` & `chalkpy-2.9.9/chalk/features/_encoding/inputs.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_encoding/json.py` & `chalkpy-2.9.9/chalk/features/_encoding/json.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_encoding/outputs.py` & `chalkpy-2.9.9/chalk/features/_encoding/outputs.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_encoding/pyarrow.py` & `chalkpy-2.9.9/chalk/features/_encoding/pyarrow.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_encoding/rich.py` & `chalkpy-2.9.9/chalk/features/_encoding/rich.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/_encoding/serialized_dtype.py` & `chalkpy-2.9.9/chalk/features/_encoding/serialized_dtype.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/dataframe/_filters.py` & `chalkpy-2.9.9/chalk/features/dataframe/_filters.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/dataframe/_impl.py` & `chalkpy-2.9.9/chalk/features/dataframe/_impl.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/dataframe/_validation.py` & `chalkpy-2.9.9/chalk/features/dataframe/_validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/feature_field.py` & `chalkpy-2.9.9/chalk/features/feature_field.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/feature_set.py` & `chalkpy-2.9.9/chalk/features/feature_set.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/feature_set_decorator.py` & `chalkpy-2.9.9/chalk/features/feature_set_decorator.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/feature_time.py` & `chalkpy-2.9.9/chalk/features/feature_time.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/feature_wrapper.py` & `chalkpy-2.9.9/chalk/features/feature_wrapper.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/filter.py` & `chalkpy-2.9.9/chalk/features/filter.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/hooks.py` & `chalkpy-2.9.9/chalk/features/hooks.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/live_updates.py` & `chalkpy-2.9.9/chalk/features/live_updates.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/primary.py` & `chalkpy-2.9.9/chalk/features/primary.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/pseudofeatures.py` & `chalkpy-2.9.9/chalk/features/pseudofeatures.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/resolver.py` & `chalkpy-2.9.9/chalk/features/resolver.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/features/tag.py` & `chalkpy-2.9.9/chalk/features/tag.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/gitignore/gitignore_parser.py` & `chalkpy-2.9.9/chalk/gitignore/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/gitignore/helper.py` & `chalkpy-2.9.9/chalk/gitignore/helper.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/importer.py` & `chalkpy-2.9.9/chalk/importer.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/integrations/named.py` & `chalkpy-2.9.9/chalk/integrations/named.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/logging/__init__.py` & `chalkpy-2.9.9/chalk/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/mypy_plugin.py` & `chalkpy-2.9.9/chalk/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/parsed/_graph_validation.py` & `chalkpy-2.9.9/chalk/parsed/_graph_validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/parsed/branch_state.py` & `chalkpy-2.9.9/chalk/parsed/branch_state.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/parsed/branch_state_rich.py` & `chalkpy-2.9.9/chalk/parsed/branch_state_rich.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/parsed/duplicate_input_gql.py` & `chalkpy-2.9.9/chalk/parsed/duplicate_input_gql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/parsed/json_conversions.py` & `chalkpy-2.9.9/chalk/parsed/json_conversions.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/parsed/user_types_to_json.py` & `chalkpy-2.9.9/chalk/parsed/user_types_to_json.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/serialization/parsed_annotation.py` & `chalkpy-2.9.9/chalk/serialization/parsed_annotation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/__init__.py` & `chalkpy-2.9.9/chalk/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/chalk_query.py` & `chalkpy-2.9.9/chalk/sql/_internal/chalk_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/incremental.py` & `chalkpy-2.9.9/chalk/sql/_internal/incremental.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/bigquery.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/bigquery.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/cloudsql.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/cloudsql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/databricks.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/databricks.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/mysql.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/mysql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/postgres.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/postgres.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/redshift.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/redshift.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/snowflake.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/snowflake.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/integrations/sqlite.py` & `chalkpy-2.9.9/chalk/sql/_internal/integrations/sqlite.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/sql_file_resolver.py` & `chalkpy-2.9.9/chalk/sql/_internal/sql_file_resolver.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/sql_source.py` & `chalkpy-2.9.9/chalk/sql/_internal/sql_source.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/_internal/string_chalk_query.py` & `chalkpy-2.9.9/chalk/sql/_internal/string_chalk_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/finalized_query.py` & `chalkpy-2.9.9/chalk/sql/finalized_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/sql/protocols.py` & `chalkpy-2.9.9/chalk/sql/protocols.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/state.py` & `chalkpy-2.9.9/chalk/state.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/streams/__init__.py` & `chalkpy-2.9.9/chalk/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/streams/_kafka_source.py` & `chalkpy-2.9.9/chalk/streams/_kafka_source.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/streams/_kinesis_source.py` & `chalkpy-2.9.9/chalk/streams/_kinesis_source.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/streams/_windows.py` & `chalkpy-2.9.9/chalk/streams/_windows.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/streams/types.py` & `chalkpy-2.9.9/chalk/streams/types.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/testing/__init__.py` & `chalkpy-2.9.9/chalk/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/annotation_parsing.py` & `chalkpy-2.9.9/chalk/utils/annotation_parsing.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/collections.py` & `chalkpy-2.9.9/chalk/utils/collections.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/duration.py` & `chalkpy-2.9.9/chalk/utils/duration.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/enum.py` & `chalkpy-2.9.9/chalk/utils/enum.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/environment_parsing.py` & `chalkpy-2.9.9/chalk/utils/environment_parsing.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/inspect.py` & `chalkpy-2.9.9/chalk/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/log_with_context.py` & `chalkpy-2.9.9/chalk/utils/log_with_context.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/metaprogramming.py` & `chalkpy-2.9.9/chalk/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/notebook.py` & `chalkpy-2.9.9/chalk/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/paths.py` & `chalkpy-2.9.9/chalk/utils/paths.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/string.py` & `chalkpy-2.9.9/chalk/utils/string.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalk/utils/stubgen.py` & `chalkpy-2.9.9/chalk/utils/stubgen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/chalkpy.egg-info/SOURCES.txt` & `chalkpy-2.9.9/chalkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chalkpy-2.9.8/pyproject.toml` & `chalkpy-2.9.9/pyproject.toml`

 * *Files identical despite different names*

