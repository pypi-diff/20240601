# Comparing `tmp/entsoe-py-0.6.7.tar.gz` & `tmp/entsoe_py-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entsoe-py-0.6.7.tar", last modified: Wed Feb 21 15:39:32 2024, max compression
+gzip compressed data, was "entsoe_py-0.6.8.tar", last modified: Sat Jun  1 15:13:31 2024, max compression
```

## Comparing `entsoe-py-0.6.7.tar` & `entsoe_py-0.6.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:39:32.236983 entsoe-py-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-02-21 15:39:32.236983 entsoe-py-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:39:32.224983 entsoe-py-0.6.7/entsoe/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    75119 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/entsoe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:39:32.224983 entsoe-py-0.6.7/entsoe/geo/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:39:32.236983 entsoe-py-0.6.7/entsoe/geo/geojson/
--rw-r--r--   0 runner    (1001) docker     (127)    47525 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/AT.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    27680 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/BE.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    38425 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/BG.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/CH.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    40228 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/CZ.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   133011 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/DE_LU.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    65781 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/DK_1.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/DK_2.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    45888 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/EE.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   110461 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/ES.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   141232 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/FI.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   158622 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/FR.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   267088 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/GR.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   102548 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/HR.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    36985 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/HU.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_CALA.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    50809 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_CNOR.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    43645 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_CNOR_2020.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    52052 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_CSUD.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    44885 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_CSUD_2020.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    67852 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_NORD.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    30130 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_SARD.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_SICI.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    34209 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_SUD.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    37133 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/IT_SUD_2020.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/LT.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/LV.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    33960 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/NL.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   773550 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/NO_1.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   217427 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/NO_2.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   221446 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/NO_3.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   702723 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/NO_4.geojson
--rw-r--r--   0 runner    (1001) docker     (127)   440492 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/NO_5.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    58106 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/PL.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/PT.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    52241 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/RO.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    40937 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/RS.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    42877 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/SE_1.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    40138 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/SE_2.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    96287 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/SE_3.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    26450 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/SE_4.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    22802 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/SI.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/geojson/SK.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/geo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18928 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    28003 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/series_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/entsoe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:39:32.236983 entsoe-py-0.6.7/entsoe_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-02-21 15:39:32.000000 entsoe-py-0.6.7/entsoe_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-02-21 15:39:32.000000 entsoe-py-0.6.7/entsoe_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 15:39:32.000000 entsoe-py-0.6.7/entsoe_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 15:39:32.000000 entsoe-py-0.6.7/entsoe_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-21 15:39:32.000000 entsoe-py-0.6.7/entsoe_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-21 15:39:32.236983 entsoe-py-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-21 15:39:24.000000 entsoe-py-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:13:31.102150 entsoe_py-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-06-01 15:13:31.102150 entsoe_py-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:13:31.090149 entsoe_py-0.6.8/entsoe/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78134 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/entsoe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:13:31.090149 entsoe_py-0.6.8/entsoe/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:13:31.102150 entsoe_py-0.6.8/entsoe/geo/geojson/
+-rw-r--r--   0 runner    (1001) docker     (127)    47525 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/AT.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    27680 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/BE.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    38425 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/BG.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/CH.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    40228 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/CZ.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   133011 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/DE_LU.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    65781 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/DK_1.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/DK_2.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    45888 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/EE.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   110461 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/ES.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   141232 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/FI.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   158622 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/FR.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   267088 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/GR.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   102548 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/HR.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    36985 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/HU.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_CALA.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    50809 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_CNOR.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    43645 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_CNOR_2020.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    52052 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_CSUD.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    44885 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_CSUD_2020.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    67852 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_NORD.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    30130 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_SARD.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_SICI.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    34209 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_SUD.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    37133 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/IT_SUD_2020.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/LT.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/LV.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    33960 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/NL.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   773550 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/NO_1.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   217427 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/NO_2.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   221446 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/NO_3.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   702723 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/NO_4.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   440492 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/NO_5.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    58106 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/PL.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/PT.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    52241 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/RO.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    40937 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/RS.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    42877 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/SE_1.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    40138 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/SE_2.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    96287 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/SE_3.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    26450 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/SE_4.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    22802 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/SI.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/geojson/SK.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/geo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20959 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28003 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/series_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/entsoe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:13:31.102150 entsoe_py-0.6.8/entsoe_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-06-01 15:13:31.000000 entsoe_py-0.6.8/entsoe_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-06-01 15:13:31.000000 entsoe_py-0.6.8/entsoe_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 15:13:31.000000 entsoe_py-0.6.8/entsoe_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 15:13:31.000000 entsoe_py-0.6.8/entsoe_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 15:13:31.000000 entsoe_py-0.6.8/entsoe_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 15:13:31.102150 entsoe_py-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-06-01 15:13:27.000000 entsoe_py-0.6.8/setup.py
```

### Comparing `entsoe-py-0.6.7/LICENSE` & `entsoe_py-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/PKG-INFO` & `entsoe_py-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entsoe-py
-Version: 0.6.7
+Version: 0.6.8
 Summary: A python API wrapper for ENTSO-E
 Home-page: https://github.com/EnergieID/entsoe-py
 Author: EnergieID.be, Frank Boerman
 Author-email: jan@energieid.be, frank@fboerman.nl
 License: MIT
 Keywords: ENTSO-E data api energy
 Classifier: Development Status :: 5 - Production/Stable
@@ -66,14 +66,15 @@
 client.query_net_transfer_capacity_dayahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_weekahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_monthahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_yearahead(country_code_from, country_code_to, start, end)
 client.query_intraday_offered_capacity(country_code_from, country_code_to, start, end, implicit=True)
 client.query_offered_capacity(country_code_from, country_code_to, start, end, contract_marketagreement_type, implicit=True)
 client.query_contracted_reserve_prices(country_code, start, end, type_marketagreement_type, psr_type=None)
+client.query_contracted_reserve_prices_procured_capacity(country_code, start, end, process_type type_marketagreement_type, psr_type=None)
 client.query_contracted_reserve_amount(country_code, start, end, type_marketagreement_type, psr_type=None)
 client.query_procured_balancing_capacity(country_code, start, end, process_type, type_marketagreement_type=None)
 client.query_aggregate_water_reservoirs_and_hydro_storage(country_code, start, end)
 
 # methods that return ZIP (bytes)
 client.query_imbalance_prices(country_code, start, end, psr_type=None)
 client.query_unavailability_of_generation_units(country_code, start, end, docstatus=None, periodstartupdate=None, periodendupdate=None)
```

### Comparing `entsoe-py-0.6.7/README.md` & `entsoe_py-0.6.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 client.query_net_transfer_capacity_dayahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_weekahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_monthahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_yearahead(country_code_from, country_code_to, start, end)
 client.query_intraday_offered_capacity(country_code_from, country_code_to, start, end, implicit=True)
 client.query_offered_capacity(country_code_from, country_code_to, start, end, contract_marketagreement_type, implicit=True)
 client.query_contracted_reserve_prices(country_code, start, end, type_marketagreement_type, psr_type=None)
+client.query_contracted_reserve_prices_procured_capacity(country_code, start, end, process_type type_marketagreement_type, psr_type=None)
 client.query_contracted_reserve_amount(country_code, start, end, type_marketagreement_type, psr_type=None)
 client.query_procured_balancing_capacity(country_code, start, end, process_type, type_marketagreement_type=None)
 client.query_aggregate_water_reservoirs_and_hydro_storage(country_code, start, end)
 
 # methods that return ZIP (bytes)
 client.query_imbalance_prices(country_code, start, end, psr_type=None)
 client.query_unavailability_of_generation_units(country_code, start, end, docstatus=None, periodstartupdate=None, periodendupdate=None)
```

### Comparing `entsoe-py-0.6.7/entsoe/decorators.py` & `entsoe_py-0.6.8/entsoe/decorators.py`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/entsoe.py` & `entsoe_py-0.6.8/entsoe/entsoe.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .decorators import retry, paginated, year_limited, day_limited, documents_limited
 import warnings
 
 logger = logging.getLogger(__name__)
 warnings.filterwarnings('ignore', category=XMLParsedAsHTMLWarning)
 
 __title__ = "entsoe-py"
-__version__ = "0.6.7"
+__version__ = "0.6.8"
 __author__ = "EnergieID.be, Frank Boerman"
 __license__ = "MIT"
 
 URL = 'https://web-api.tp.entsoe.eu/api'
 
 
 class EntsoeRawClient:
@@ -902,14 +902,52 @@
             'offset': offset
         }
         if psr_type:
             params.update({'psrType': psr_type})
         response = self._base_request(params=params, start=start, end=end)
         return response.text
 
+    def query_contracted_reserve_prices_procured_capacity(
+            self, country_code: Union[Area, str], start: pd.Timestamp,
+            end: pd.Timestamp, process_type: str, 
+            type_marketagreement_type: str, psr_type: Optional[str] = None,
+            offset: int = 0) -> str:
+        """
+        Parameters
+        ----------
+        country_code : Area|str
+        start : pd.Timestamp
+        end : pd.Timestamp
+        process_type : str
+            type of process (see mappings.PROCESSTYPE)
+        type_marketagreement_type : str
+            type of contract (see mappings.MARKETAGREEMENTTYPE)
+        psr_type : str
+            filter query for a specific psr type
+        offset : int
+            offset for querying more than 100 documents
+
+        Returns
+        -------
+        str
+        """
+        area = lookup_area(country_code)
+        params = {
+            'documentType': 'A81', # [M] A81 = Contracted reserves
+            'businessType': 'B95', # [M] B95 = Procured capacity
+            'processType': process_type, # [M*] A51 = Automatic frequency restoration reserve; A52 =  Frequency containment reserve; A47 = Manual frequency restoration reserve; A46 = Replacement reserve
+            'controlArea_Domain': area.code,
+            'type_MarketAgreement.Type': type_marketagreement_type,
+            'offset': offset
+        }
+        if psr_type:
+            params.update({'psrType': psr_type})
+        response = self._base_request(params=params, start=start, end=end)
+        return response.text
+
     def query_contracted_reserve_amount(
             self, country_code: Union[Area, str], start: pd.Timestamp,
             end: pd.Timestamp, type_marketagreement_type: str,
             psr_type: Optional[str] = None,
             offset: int = 0) -> str:
         """
         Parameters
@@ -1155,15 +1193,15 @@
         return df
     
     @year_limited
     def query_day_ahead_prices(
             self, country_code: Union[Area, str],
             start: pd.Timestamp,
             end: pd.Timestamp,
-            resolution: List[Literal['60min', '30min', '15min']] = '60min') -> pd.Series:
+            resolution: Literal['60min', '30min', '15min'] = '60min') -> pd.Series:
         """
         Parameters
         ----------
         resolution: either 60min for hourly values,
             30min for half-hourly values or 15min for quarterly values, throws error if type is not available
         country_code : Area|str
         start : pd.Timestamp
@@ -1879,14 +1917,55 @@
             country_code=area, start=start, end=end,
             type_marketagreement_type=type_marketagreement_type,
             psr_type=psr_type, offset=offset)
         df = parse_contracted_reserve(text, area.tz, "procurement_price.amount")
         df = df.tz_convert(area.tz)
         df = df.truncate(before=start, after=end)
         return df
+    
+    @year_limited
+    @paginated
+    @documents_limited(100)
+    def query_contracted_reserve_prices_procured_capacity(
+            self,
+            country_code: Union[Area, str],
+            process_type: str,
+            type_marketagreement_type: str,
+            start: pd.Timestamp,
+            end: pd.Timestamp,
+            psr_type: Optional[str] = None,
+            offset: int = 0) -> pd.DataFrame:
+        """
+        Parameters
+        ----------
+        country_code : Area, str
+        process_type : str
+            type of process (see mappings.PROCESSTYPE)
+        type_marketagreement_type : str
+            type of contract (see mappings.MARKETAGREEMENTTYPE)
+        start : pd.Timestamp
+        end : pd.Timestamp
+        psr_type : str
+            filter query for a specific psr type
+        offset : int
+            offset for querying more than 100 documents
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        area = lookup_area(country_code)
+        text = super(EntsoePandasClient, self).query_contracted_reserve_prices_procured_capacity(
+            country_code=area, start=start, end=end,
+            process_type=process_type, type_marketagreement_type=type_marketagreement_type,
+            psr_type=psr_type, offset=offset)
+        df = parse_contracted_reserve(text, area.tz, "procurement_price.amount")
+        df = df.tz_convert(area.tz)
+        df = df.truncate(before=start, after=end)
+        return df    
 
     @year_limited
     @paginated
     @documents_limited(100)
     def query_contracted_reserve_amount(
             self,
             country_code: Union[Area, str],
```

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/AT.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/AT.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/BE.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/BE.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/BG.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/BG.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/CH.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/CH.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/CZ.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/CZ.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/DE_LU.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/DE_LU.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/DK_1.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/DK_1.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/DK_2.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/DK_2.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/EE.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/EE.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/ES.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/ES.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/FI.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/FI.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/FR.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/FR.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/GR.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/GR.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/HR.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/HR.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/HU.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/HU.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_CALA.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_CALA.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_CNOR.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_CNOR.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_CNOR_2020.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_CNOR_2020.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_CSUD.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_CSUD.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_CSUD_2020.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_CSUD_2020.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_NORD.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_NORD.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_SARD.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_SARD.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_SICI.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_SICI.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_SUD.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_SUD.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/IT_SUD_2020.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/IT_SUD_2020.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/LT.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/LT.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/LV.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/LV.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/NL.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/NL.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/NO_1.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/NO_1.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/NO_2.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/NO_2.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/NO_3.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/NO_3.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/NO_4.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/NO_4.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/NO_5.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/NO_5.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/PL.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/PL.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/PT.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/PT.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/RO.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/RO.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/RS.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/RS.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/SE_1.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/SE_1.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/SE_2.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/SE_2.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/SE_3.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/SE_3.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/SE_4.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/SE_4.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/SI.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/SI.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/geojson/SK.geojson` & `entsoe_py-0.6.8/entsoe/geo/geojson/SK.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/geo/utils.py` & `entsoe_py-0.6.8/entsoe/geo/utils.py`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/mappings.py` & `entsoe_py-0.6.8/entsoe/mappings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import enum
 from typing import Union
 
 
 def lookup_area(s: Union['Area', str]) -> 'Area':
     if isinstance(s, Area):
         # If it already is an Area object, we're happy
-        area = s
-    else:  # It is a string
-        try:
-            # If it is a "country code" string, we do a lookup
-            area = Area[s]
-        except KeyError:
-            # It is not, it may be a direct code
-            area = [area for area in Area if area.value == s][0]
-    return area
+        return s
+    if isinstance(s, str):
+        # If it is a "country code" string, we do a lookup
+        if Area.has_code(s.upper()):
+            return Area[s.upper()]
+
+        # If it is a "direct code", we do a lookup
+        for area in Area:
+            if area.value == s:
+                return area
 
+    raise ValueError('Invalid country code.')
 
 class Area(enum.Enum):
     """
     ENUM containing 3 things about an Area: CODE, Meaning, Timezone
     """
     def __new__(cls, *args, **kwds):
         obj = object.__new__(cls)
@@ -41,14 +43,18 @@
     def tz(self):
         return self._tz
 
     @property
     def code(self):
         return self.value
 
+    @classmethod
+    def has_code(cls, code:str)->bool:
+        return code in cls.__members__ 
+
     # List taken directly from the API Docs
     DE_50HZ =       '10YDE-VE-------2', '50Hertz CA, DE(50HzT) BZA',                    'Europe/Berlin',
     AL =            '10YAL-KESH-----5', 'Albania, OST BZ / CA / MBA',                   'Europe/Tirane',
     DE_AMPRION =    '10YDE-RWENET---I', 'Amprion CA',                                   'Europe/Berlin',
     AT =            '10YAT-APG------L', 'Austria, APG BZ / CA / MBA',                   'Europe/Vienna',
     BY =            '10Y1001A1001A51S', 'Belarus BZ / CA / MBA',                        'Europe/Minsk',
     BE =            '10YBE----------2', 'Belgium, Elia BZ / CA / MBA',                  'Europe/Brussels',
@@ -102,14 +108,15 @@
     LV =            '10YLV-1001A00074', 'Latvia, AST BZ / CA / MBA',                    'Europe/Riga',
     LT =            '10YLT-1001A0008Q', 'Lithuania, Litgrid BZ / CA / MBA',             'Europe/Vilnius',
     LU =            '10YLU-CEGEDEL-NQ', 'Luxembourg, CREOS CA',                         'Europe/Luxembourg',
     LU_BZN =        '10Y1001A1001A82H', 'Luxembourg',                                   'Europe/Luxembourg',
     MT =            '10Y1001A1001A93C', 'Malta, Malta BZ / CA / MBA',                   'Europe/Malta',
     ME =            '10YCS-CG-TSO---S', 'Montenegro, CGES BZ / CA / MBA',               'Europe/Podgorica',
     GB =            '10YGB----------A', 'National Grid BZ / CA/ MBA',                   'Europe/London',
+    GE =            '10Y1001A1001B012', 'Georgia',                                      'Asia/Tbilisi',
     GB_IFA =        '10Y1001C--00098F', 'GB(IFA) BZN',                                  'Europe/London',
     GB_IFA2 =       '17Y0000009369493', 'GB(IFA2) BZ',                                  'Europe/London',
     GB_ELECLINK =   '11Y0-0000-0265-K', 'GB(ElecLink) BZN',                             'Europe/London',
     UK =            '10Y1001A1001A92E', 'United Kingdom',                               'Europe/London',
     NL =            '10YNL----------L', 'Netherlands, TenneT NL BZ / CA/ MBA',          'Europe/Amsterdam',
     NO_1 =          '10YNO-1--------2', 'NO1 BZ / MBA',                                 'Europe/Oslo',
     NO_1A =         '10Y1001A1001A64J', 'NO1 A BZ',                                     'Europe/Oslo',
@@ -143,14 +150,15 @@
     UA =            '10Y1001C--00003F', 'Ukraine, Ukraine BZ, MBA',                     'Europe/Kiev',
     UA_DOBTPP =     '10Y1001A1001A869', 'Ukraine-DobTPP CTA',                           'Europe/Kiev',
     UA_BEI =        '10YUA-WEPS-----0', 'Ukraine BEI CTA',                              'Europe/Kiev',
     UA_IPS =        '10Y1001C--000182', 'Ukraine IPS CTA',                              'Europe/Kiev',
     XK =            '10Y1001C--00100H', 'Kosovo/ XK CA / XK BZN',                       'Europe/Rome',
     DE_AMP_LU =     '10Y1001C--00002H', 'Amprion LU CA',                                'Europe/Berlin'
 
+# https://transparency.entsoe.eu/content/static_content/Static%20content/web%20api/Guide.html#_psrtype
 PSRTYPE_MAPPINGS = {
     'A03': 'Mixed',
     'A04': 'Generation',
     'A05': 'Load',
     'B01': 'Biomass',
     'B02': 'Fossil Brown coal/Lignite',
     'B03': 'Fossil Coal-derived gas',
@@ -172,51 +180,73 @@
     'B19': 'Wind Onshore',
     'B20': 'Other',
     'B21': 'AC Link',
     'B22': 'DC Link',
     'B23': 'Substation',
     'B24': 'Transformer'}
 
+# https://transparency.entsoe.eu/content/static_content/Static%20content/web%20api/Guide.html#_docstatus
 DOCSTATUS = {'A01': 'Intermediate',
              'A02': 'Final',
              'A05': 'Active',
              'A09': 'Cancelled',
              'A13': 'Withdrawn',
              'X01': 'Estimated'}
 
-BSNTYPE = {'A29': 'Already allocated capacity (AAC)',
+# https://transparency.entsoe.eu/content/static_content/Static%20content/web%20api/Guide.html#_businesstype
+BSNTYPE = { 'A01': 'Production',
+           'A04': 'Consumption',
+           'A14': 'Aggregated energy data',
+           'A19': 'Balance energy deviation',
+           'A25': 'General Capacity Information',
+           'A29': 'Already allocated capacity (AAC)',
            'A43': 'Requested capacity (without price)',
            'A46': 'System Operator redispatching',
            'A53': 'Planned maintenance',
            'A54': 'Unplanned outage',
+           'A60': 'Minimum possible',
+           'A61': 'Maximum possible',
            'A85': 'Internal redispatch',
+           'A91': 'Positive forecast margin (if installed capacity > load forecast)',
+           'A92': 'Negative forecast margin (if load forecast > installed capacity)',
+           'A93': 'Wind generation',
+           'A94': 'Solar generation',
            'A95': 'Frequency containment reserve',
            'A96': 'Automatic frequency restoration reserve',
            'A97': 'Manual frequency restoration reserve',
            'A98': 'Replacement reserve',
            'B01': 'Interconnector network evolution',
            'B02': 'Interconnector network dismantling',
            'B03': 'Counter trade',
            'B04': 'Congestion costs',
            'B05': 'Capacity allocated (including price)',
            'B07': 'Auction revenue',
            'B08': 'Total nominated capacity',
            'B09': 'Net position',
            'B10': 'Congestion income',
-           'B11': 'Production unit'}
+           'B11': 'Production unit',
+           'B33': 'Area Control Error',
+           'B74': 'Offer',
+           'B75': 'Need', 
+           'B95': 'Procured capacity',
+           'C22': 'Shared Balancing Reserve Capacity', 
+           'C23': 'Share of reserve capacity',
+           'C24': 'Actual reserve capacity'}
 
+# https://transparency.entsoe.eu/content/static_content/Static%20content/web%20api/Guide.html#_contract_marketagreement_type_type_marketagreement_type
 MARKETAGREEMENTTYPE = {'A01': 'Daily',
                        'A02': 'Weekly',
                        'A03': 'Monthly',
                        'A04': 'Yearly',
                        'A05': 'Total',
                        'A06': 'Long term',
                        'A07': 'Intraday',
                        'A13': 'Hourly'}
 
+# https://transparency.entsoe.eu/content/static_content/Static%20content/web%20api/Guide.html#_documenttype
 DOCUMENTTYPE = {'A09': 'Finalised schedule',
                 'A11': 'Aggregated energy data report',
                 'A15': 'Acquiring system operator reserve schedule',
                 'A24': 'Bid document',
                 'A25': 'Allocation result document',
                 'A26': 'Capacity document',
                 'A31': 'Agreed capacity',
@@ -249,45 +279,52 @@
                 'A89': 'Contracted reserve prices',
                 'A90': 'Interconnection network expansion',
                 'A91': 'Counter trade notice',
                 'A92': 'Congestion costs',
                 'A93': 'DC link capacity',
                 'A94': 'Non EU allocations',
                 'A95': 'Configuration document',
-                'B11': 'Flow-based allocations'}
+                'B11': 'Flow-based allocations',
+                'B17': 'Aggregated netted external TSO schedule document',
+                'B45': 'Bid Availability Document'}
 
+# https://transparency.entsoe.eu/content/static_content/Static%20content/web%20api/Guide.html#_processtype
 PROCESSTYPE = {
     'A01': 'Day ahead',
     'A02': 'Intra day incremental',
     'A16': 'Realised',
     'A18': 'Intraday total',
     'A31': 'Week ahead',
     'A32': 'Month ahead',
     'A33': 'Year ahead',
     'A39': 'Synchronisation process',
     'A40': 'Intraday process',
     'A46': 'Replacement reserve',
     'A47': 'Manual frequency restoration reserve',
     'A51': 'Automatic frequency restoration reserve',
     'A52': 'Frequency containment reserve',
-    'A56': 'Frequency restoration reserve'
+    'A56': 'Frequency restoration reserve',
+    'A60': 'Scheduled activation mFRR',
+    'A61': 'Direct activation mFRR',
+    'A67': 'Central Selection aFRR',
+    'A68': 'Local Selection aFRR'
 }
 
 # neighbouring bidding zones that have cross_border flows
 NEIGHBOURS = {
     'BE': ['NL', 'DE_AT_LU', 'FR', 'GB', 'DE_LU'],
     'NL': ['BE', 'DE_AT_LU', 'DE_LU', 'GB', 'NO_2', 'DK_1'],
     'DE_AT_LU': ['BE', 'CH', 'CZ', 'DK_1', 'DK_2', 'FR', 'IT_NORD', 'IT_NORD_AT', 'NL', 'PL', 'SE_4', 'SI'],
     'FR': ['BE', 'CH', 'DE_AT_LU', 'DE_LU', 'ES', 'GB', 'IT_NORD', 'IT_NORD_FR'],
     'CH': ['AT', 'DE_AT_LU', 'DE_LU', 'FR', 'IT_NORD', 'IT_NORD_CH'],
     'AT': ['CH', 'CZ', 'DE_LU', 'HU', 'IT_NORD', 'SI'],
     'CZ': ['AT', 'DE_AT_LU', 'DE_LU', 'PL', 'SK'],
     'GB': ['BE', 'FR', 'IE_SEM', 'NL', 'NO_2', 'DK_1'],
     'NO_2': ['DE_LU', 'DK_1', 'NL', 'NO_1', 'NO_5', 'GB'],
-    'HU': ['AT', 'HR', 'RO', 'RS', 'SK', 'UA'],
+    'HU': ['AT', 'HR', 'RO', 'RS', 'SI', 'SK', 'UA'],
     'IT_NORD': ['CH', 'DE_AT_LU', 'FR', 'SI', 'AT', 'IT_CNOR'],
     'ES': ['FR', 'PT'],
     'SI': ['AT', 'DE_AT_LU', 'HR', 'IT_NORD'],
     'RS': ['AL', 'BA', 'BG', 'HR', 'HU', 'ME', 'MK', 'RO'],
     'PL': ['CZ', 'DE_AT_LU', 'DE_LU', 'LT', 'SE_4', 'SK', 'UA'],
     'ME': ['AL', 'BA', 'RS'],
     'DK_1': ['DE_AT_LU', 'DE_LU', 'DK_2', 'NO_2', 'SE_3', 'NL'],
```

### Comparing `entsoe-py-0.6.7/entsoe/misc.py` & `entsoe_py-0.6.8/entsoe/misc.py`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/parsers.py` & `entsoe_py-0.6.8/entsoe/parsers.py`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe/series_parsers.py` & `entsoe_py-0.6.8/entsoe/series_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 
 def _resolution_to_timedelta(res_text: str) -> str:
     """
     Convert an Entsoe resolution to something that pandas can understand
     """
     resolutions = {
         'PT60M': '60min',
-        'P1Y': '12M',
+        'P1Y': '12MS',
         'PT15M': '15min',
         'PT30M': '30min',
         'P1D': '1D',
         'P7D': '7D',
-        'P1M': '1M',
+        'P1M': '1MS',
     }
     delta = resolutions.get(res_text)
     if delta is None:
         raise NotImplementedError("Sorry, I don't know what to do with the "
                                   "resolution '{}', because there was no "
                                   "documentation to be found of this format. "
                                   "Everything is hard coded. Please open an "
```

### Comparing `entsoe-py-0.6.7/entsoe/utils.py` & `entsoe_py-0.6.8/entsoe/utils.py`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/entsoe_py.egg-info/PKG-INFO` & `entsoe_py-0.6.8/entsoe_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entsoe-py
-Version: 0.6.7
+Version: 0.6.8
 Summary: A python API wrapper for ENTSO-E
 Home-page: https://github.com/EnergieID/entsoe-py
 Author: EnergieID.be, Frank Boerman
 Author-email: jan@energieid.be, frank@fboerman.nl
 License: MIT
 Keywords: ENTSO-E data api energy
 Classifier: Development Status :: 5 - Production/Stable
@@ -66,14 +66,15 @@
 client.query_net_transfer_capacity_dayahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_weekahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_monthahead(country_code_from, country_code_to, start, end)
 client.query_net_transfer_capacity_yearahead(country_code_from, country_code_to, start, end)
 client.query_intraday_offered_capacity(country_code_from, country_code_to, start, end, implicit=True)
 client.query_offered_capacity(country_code_from, country_code_to, start, end, contract_marketagreement_type, implicit=True)
 client.query_contracted_reserve_prices(country_code, start, end, type_marketagreement_type, psr_type=None)
+client.query_contracted_reserve_prices_procured_capacity(country_code, start, end, process_type type_marketagreement_type, psr_type=None)
 client.query_contracted_reserve_amount(country_code, start, end, type_marketagreement_type, psr_type=None)
 client.query_procured_balancing_capacity(country_code, start, end, process_type, type_marketagreement_type=None)
 client.query_aggregate_water_reservoirs_and_hydro_storage(country_code, start, end)
 
 # methods that return ZIP (bytes)
 client.query_imbalance_prices(country_code, start, end, psr_type=None)
 client.query_unavailability_of_generation_units(country_code, start, end, docstatus=None, periodstartupdate=None, periodendupdate=None)
```

### Comparing `entsoe-py-0.6.7/entsoe_py.egg-info/SOURCES.txt` & `entsoe_py-0.6.8/entsoe_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.6.7/setup.py` & `entsoe_py-0.6.8/setup.py`

 * *Files identical despite different names*

