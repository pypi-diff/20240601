# Comparing `tmp/pyjpboatrace-0.3.0a4.tar.gz` & `tmp/pyjpboatrace-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjpboatrace-0.3.0a4.tar", last modified: Thu Apr  4 13:27:51 2024, max compression
+gzip compressed data, was "pyjpboatrace-0.3.1a0.tar", last modified: Sat Jun  1 16:17:57 2024, max compression
```

## Comparing `pyjpboatrace-0.3.0a4.tar` & `pyjpboatrace-0.3.1a0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49608 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47096 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:51.144098 pyjpboatrace-0.3.0a4/pyjpboatrace/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/certification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/pyjpboatrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/user_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyjpboatrace/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49608 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 13:27:51.000000 pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:27:51.148098 pyjpboatrace-0.3.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/tests/test_certification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/tests/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/tests/test_pyjpboatrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-04 13:27:31.000000 pyjpboatrace-0.3.0a4/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:17:57.164294 pyjpboatrace-0.3.1a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    50199 2024-06-01 16:17:57.160294 pyjpboatrace-0.3.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47649 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:17:57.160294 pyjpboatrace-0.3.1a0/pyjpboatrace/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyjpboatrace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyjpboatrace/certification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyjpboatrace/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyjpboatrace/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyjpboatrace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyjpboatrace/pyjpboatrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyjpboatrace/user_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyjpboatrace/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:17:57.160294 pyjpboatrace-0.3.1a0/pyjpboatrace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50199 2024-06-01 16:17:57.000000 pyjpboatrace-0.3.1a0/pyjpboatrace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-06-01 16:17:57.000000 pyjpboatrace-0.3.1a0/pyjpboatrace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:17:57.000000 pyjpboatrace-0.3.1a0/pyjpboatrace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-01 16:17:57.000000 pyjpboatrace-0.3.1a0/pyjpboatrace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 16:17:57.000000 pyjpboatrace-0.3.1a0/pyjpboatrace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:17:57.164294 pyjpboatrace-0.3.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:17:57.160294 pyjpboatrace-0.3.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/tests/test_certification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/tests/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/tests/test_pyjpboatrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-06-01 16:17:41.000000 pyjpboatrace-0.3.1a0/tests/test_validator.py
```

### Comparing `pyjpboatrace-0.3.0a4/LICENSE` & `pyjpboatrace-0.3.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/PKG-INFO` & `pyjpboatrace-0.3.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjpboatrace
-Version: 0.3.0a4
+Version: 0.3.1a0
 Summary: PyJPBoatrace: Python-based Japanese boatrace tools
 Author-email: hmasdev <hmasuidev1com@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 hmasdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,31 +41,31 @@
 Requires-Dist: requests>=2.28.1
 Requires-Dist: selenium>=4.6.0
 Requires-Dist: types-beautifulsoup4
 Requires-Dist: types-requests
 Provides-Extra: dev
 Requires-Dist: autopep8; extra == "dev"
 Requires-Dist: flake8>=3.8.4; extra == "dev"
+Requires-Dist: Jinja2; extra == "dev"
 Requires-Dist: mypy>=0.812; extra == "dev"
 Requires-Dist: pytest>=6.1.2; extra == "dev"
 Requires-Dist: pytest-cov>=2.10.1; extra == "dev"
 Requires-Dist: pytz; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: types-pytz; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 # PyJPBoatRace: Python-based Japanese boatrace tools :speedboat:
 
 ![GitHub top language](https://img.shields.io/github/languages/top/hmasdev/pyjpboatrace)
 ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/hmasdev/pyjpboatrace?sort=semver)
 ![GitHub](https://img.shields.io/github/license/hmasdev/pyjpboatrace)
 ![GitHub last commit](https://img.shields.io/github/last-commit/hmasdev/pyjpboatrace)
-![pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
-![flake8](https://github.com/hmasdev/pyjpboatrace/actions/workflows/code-style-check.yaml/badge.svg)
-![mypy](https://github.com/hmasdev/pyjpboatrace/actions/workflows/static-type-check.yaml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/pyjpboatrace.svg)](https://pypi.org/project/pyjpboatrace/)
+![Scheduled Test](https://github.com/hmasdev/pyjpboatrace/actions/workflows/tests_on_schedule.yaml/badge.svg)
 
 Japanese boat race is extremely exciting sports.
 It is also fun to predict the results of races.
 Prediction like machine learning method requires data.
 Thus, this package provides you with useful tools for data analysis and auto-betting for boatrace.
 
 ## Installation
@@ -132,107 +132,108 @@
 - Get a list of stadiums which hold races on the given day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_stadiums(d: datetime.date) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Stadiums.get(d: datetime.date) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
 
     ```python
     >>> from pyjpboatrace import PyJPBoatrace
     >>> from datetime import date
     >>> from pprint import pprint
     >>> pprint(PyJPBoatrace().get_stadiums(date(2021, 8, 12)))
     {'date': '2021-08-12',
-    'びわこ': {'day': '３日目',
-            'grade': ['ippan'],
-            'period': ['2021-08-10', '2021-08-15'],
-            'status': '-',
-            'timeframe': '',
-            'title': '滋賀県知事杯争奪第２６回びわこカップ'},
-    '三国': {'day': '２日目',
+     'びわこ': {'day': '３日目',
+             'grade': ['ippan'],
+             'period': ['2021-08-10', '2021-08-15'],
+             'status': '-',
+             'timeframe': '',
+             'title': '滋賀県知事杯争奪第２６回びわこカップ'},
+     '三国': {'day': '２日目',
             'grade': ['ippan'],
             'period': ['2021-08-11', '2021-08-16'],
             'status': '-',
             'timeframe': 'morning',
             'title': '第４９回しぶき賞'},
-    '下関': {'day': '最終日',
+     '下関': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-06', '2021-08-12'],
             'status': '-',
             'timeframe': 'nighter',
             'title': 'Ｈａｙａｓｈｉｋａｎｅ杯'},
-    '唐津': {'day': '最終日',
+     '唐津': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-07', '2021-08-12'],
             'status': '-',
             'timeframe': 'morning',
             'title': '唐津大賞がばい王者決定戦'},
-    '多摩川': {'day': '最終日',
-            'grade': ['ippan'],
-            'period': ['2021-08-08', '2021-08-12'],
-            'status': '-',
-            'timeframe': 'summer',
-            'title': '第５９回スポーツニッポン賞'},
-    '宮島': {'day': '最終日',
+     '多摩川': {'day': '最終日',
+             'grade': ['ippan'],
+             'period': ['2021-08-08', '2021-08-12'],
+             'status': '-',
+             'timeframe': 'summer',
+             'title': '第５９回スポーツニッポン賞'},
+     '宮島': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-07', '2021-08-12'],
             'status': '-',
             'timeframe': '',
             'title': '第５１回スポーツニッポン杯'},
-    '尼崎': {'day': '４日目',
+     '尼崎': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-09', '2021-08-14'],
             'status': '-',
             'timeframe': '',
             'title': '日本財団会長杯争奪第４９回オール兵庫王座決定戦'},
-    '常滑': {'day': '２日目',
+     '常滑': {'day': '２日目',
             'grade': ['ippan'],
             'period': ['2021-08-11', '2021-08-16'],
             'status': '-',
             'timeframe': '',
             'title': '名鉄杯争奪２０２１納涼お盆レース'},
-    '平和島': {'day': '３日目',
-            'grade': ['ippan'],
-            'period': ['2021-08-10', '2021-08-15'],
-            'status': '-',
-            'timeframe': 'summer',
-            'title': '第６１回デイリースポーツサマーカップ'},
-    '戸田': {'day': '初日',
+     '平和島': {'day': '３日目',
+             'grade': ['ippan'],
+             'period': ['2021-08-10', '2021-08-15'],
+             'status': '-',
+             'timeframe': 'summer',
+             'title': '第６１回デイリースポーツサマーカップ'},
+     '戸田': {'day': '初日',
             'grade': ['ippan'],
             'period': ['2021-08-12', '2021-08-17'],
             'status': '-',
             'timeframe': '',
             'title': '第４４回戸田ボート大賞・サンケイスポーツ杯'},
-    '桐生': {'day': '３日目',
+     '桐生': {'day': '３日目',
             'grade': ['ippan'],
             'period': ['2021-08-10', '2021-08-15'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '第５５回報知新聞社杯\u3000お盆レース'},
-    '若松': {'day': '４日目',
+     '若松': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-08', '2021-08-13'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '日刊スポーツ杯お盆特選競走'},
-    '蒲郡': {'day': '初日',
+     '蒲郡': {'day': '初日',
             'grade': ['ippan'],
             'period': ['2021-08-12', '2021-08-17'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '日刊スポーツ杯争奪\u3000納涼しぶきお盆特別選抜戦'},
-    '鳴門': {'day': '４日目',
+     '鳴門': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-09', '2021-08-14'],
             'status': '-',
             'timeframe': 'morning',
             'title': '第５４回渦王杯競走'}}
     ```
 
@@ -241,14 +242,15 @@
 - To get 12 races held in the given stadium on the given day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_12races(d: datetime.date, stadium: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Races.get(d: datetime.date, stadium: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -284,93 +286,94 @@
              'vote_limit': '2021-08-12 20:45:00'},
      '1R': {'racers': {'boat1': {'class': 'B1', 'name': '渡辺史之'},
                        'boat2': {'class': 'B1', 'name': '島倉都'},
                        'boat3': {'class': 'A2', 'name': '鳥居塚孝博'},
                        'boat4': {'class': 'B1', 'name': '松本純平'},
                        'boat5': {'class': 'A2', 'name': '橋本久和'},
                        'boat6': {'class': 'B2', 'name': '宮崎安奈'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 15:22:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 15:22:00'},
      '2R': {'racers': {'boat1': {'class': 'B1', 'name': '佐口達也'},
                        'boat2': {'class': 'A2', 'name': '本橋克洋'},
                        'boat3': {'class': 'B1', 'name': '寺本昇平'},
                        'boat4': {'class': 'B1', 'name': '津久井拓也'},
                        'boat5': {'class': 'B1', 'name': '久保原秀人'},
                        'boat6': {'class': 'A2', 'name': '中里英夫'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 15:49:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 15:49:00'},
      '3R': {'racers': {'boat1': {'class': 'B1', 'name': '小川時光'},
                        'boat2': {'class': 'A2', 'name': '野村誠'},
                        'boat3': {'class': 'B2', 'name': '黄金井裕子'},
                        'boat4': {'class': 'A2', 'name': '藤生雄人'},
                        'boat5': {'class': 'B1', 'name': '高山秀雄'},
                        'boat6': {'class': 'A1', 'name': '関浩哉'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 16:16:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 16:16:00'},
      '4R': {'racers': {'boat1': {'class': 'B1', 'name': '栗原謙治'},
                        'boat2': {'class': 'A2', 'name': '金子賢志'},
                        'boat3': {'class': 'B1', 'name': '関根彰人'},
                        'boat4': {'class': 'A1', 'name': '金子拓矢'},
                        'boat5': {'class': 'B2', 'name': '大久保佑香'},
                        'boat6': {'class': 'B1', 'name': '土屋太朗'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 16:45:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 16:45:00'},
      '5R': {'racers': {'boat1': {'class': 'B1', 'name': '原加央理'},
                        'boat2': {'class': 'B1', 'name': '佐藤航'},
                        'boat3': {'class': 'B1', 'name': '蜂須瑞生'},
                        'boat4': {'class': 'A2', 'name': '一柳和孝'},
                        'boat5': {'class': 'B1', 'name': '外崎悟'},
                        'boat6': {'class': 'A1', 'name': '毒島誠'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 17:13:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 17:13:00'},
      '6R': {'racers': {'boat1': {'class': 'A1', 'name': '椎名豊'},
                        'boat2': {'class': 'B1', 'name': '久保田美紀'},
                        'boat3': {'class': 'B1', 'name': '太田克哉'},
                        'boat4': {'class': 'B1', 'name': '島倉都'},
                        'boat5': {'class': 'B1', 'name': '金澤一洋'},
                        'boat6': {'class': 'B1', 'name': '寺本昇平'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 17:42:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 17:42:00'},
      '7R': {'racers': {'boat1': {'class': 'A2', 'name': '木村浩士'},
                        'boat2': {'class': 'B1', 'name': '久保原秀人'},
                        'boat3': {'class': 'A1', 'name': '上村純一'},
                        'boat4': {'class': 'B1', 'name': '鹿島敏弘'},
                        'boat5': {'class': 'B2', 'name': '宮崎安奈'},
                        'boat6': {'class': 'B2', 'name': '黄金井裕子'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 18:11:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 18:11:00'},
      '8R': {'racers': {'boat1': {'class': 'A2', 'name': '鳥居塚孝博'},
                        'boat2': {'class': 'B1', 'name': '高山秀雄'},
                        'boat3': {'class': 'B1', 'name': '吉田稔'},
                        'boat4': {'class': 'B1', 'name': '田中定雄'},
                        'boat5': {'class': 'A1', 'name': '久田敏之'},
                        'boat6': {'class': 'B2', 'name': '大久保佑香'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 18:41:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 18:41:00'},
      '9R': {'racers': {'boat1': {'class': 'B1', 'name': '崎利仁'},
                        'boat2': {'class': 'A2', 'name': '中里英夫'},
                        'boat3': {'class': 'B1', 'name': '塚原武之'},
                        'boat4': {'class': 'A1', 'name': '土屋智則'},
                        'boat5': {'class': 'B1', 'name': '関根彰人'},
                        'boat6': {'class': 'A1', 'name': '山崎智也'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 19:12:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 19:12:00'},
      'date': '2021-08-12',
      'stadium': 1}
     ```
 
     </details>
 
 - To get the basic information of the race in the stadium on a day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_race_info(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().RaceInfo.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -402,31 +405,31 @@
                'name': '武田光史',
                'racerid': 3654,
                'result': [{'ST': 0.19,
                            'boat': 5,
                            'course': 5,
                            'race': 6,
                            'rank': 4},
-                           {'ST': 0.14,
+                          {'ST': 0.14,
                            'boat': 3,
                            'course': 3,
                            'race': 12,
                            'rank': 5},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.6},
      'boat2': {'F': 0,
                'L': 0,
                'age': 25,
                'aveST': 0.21,
                'birthplace': '愛知',
                'boat': 64,
@@ -446,27 +449,27 @@
                'name': '大澤誠也',
                'racerid': 5074,
                'result': [{'ST': 0.19,
                            'boat': 3,
                            'course': 3,
                            'race': 6,
                            'rank': 3},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 53.1},
      'boat3': {'F': 0,
                'L': 0,
                'age': 45,
                'aveST': 0.17,
                'birthplace': '愛知',
                'boat': 41,
@@ -486,31 +489,31 @@
                'name': '堀本裕也',
                'racerid': 3895,
                'result': [{'ST': 0.06,
                            'boat': 5,
                            'course': 5,
                            'race': 4,
                            'rank': 5},
-                           {'ST': 0.2,
+                          {'ST': 0.2,
                            'boat': 2,
                            'course': 2,
                            'race': 11,
                            'rank': 4},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 50.0},
      'boat4': {'F': 0,
                'L': 0,
                'age': 47,
                'aveST': 0.18,
                'birthplace': '石川',
                'boat': 36,
@@ -530,27 +533,27 @@
                'name': '信濃由行',
                'racerid': 3620,
                'result': [{'ST': 0.26,
                            'boat': 5,
                            'course': 3,
                            'race': 3,
                            'rank': 5},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.3},
      'boat5': {'F': 0,
                'L': 0,
                'age': 30,
                'aveST': 0.19,
                'birthplace': '石川',
                'boat': 17,
@@ -570,31 +573,31 @@
                'name': '木田峰由季',
                'racerid': 4587,
                'result': [{'ST': 0.19,
                            'boat': 2,
                            'course': 2,
                            'race': 3,
                            'rank': 3},
-                           {'ST': 0.21,
+                          {'ST': 0.21,
                            'boat': 4,
                            'course': 5,
                            'race': 10,
                            'rank': 2},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.2},
      'boat6': {'F': 0,
                'L': 0,
                'age': 21,
                'aveST': '-',
                'birthplace': '福井',
                'boat': 15,
@@ -614,27 +617,27 @@
                'name': '加藤優弥',
                'racerid': 5185,
                'result': [{'ST': 0.01,
                            'boat': 6,
                            'course': 6,
                            'race': 4,
                            'rank': 6},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.6},
      'date': '2021-08-12',
      'race': 1,
      'race_title': ['みくにあさイチ', '1800m'],
      'stadium': 10}
     ```
 
@@ -643,14 +646,15 @@
 - To get the odds of win (単勝) and place-show (複勝) of the race in the stadium on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_win_placeshow(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().WinPlaceshowOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -678,14 +682,15 @@
 - To get the odds of quinella place (拡連複) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_quinellaplace(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().QuinellaplaceOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -721,14 +726,15 @@
 - To get the odds of exacta (二連単) and quinella (二連複) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_exacta_quinella(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().ExactaQuinellaOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -794,14 +800,15 @@
 - To get the odds of trifecta (三連単) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_trifecta(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBaotrace().TrifectaOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -942,14 +949,15 @@
 - To get the oods of trio （三連複） of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_trio(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Trio.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -990,14 +998,15 @@
 - To get the just-before information, e.g. weather and start-timing, of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_just_before_info(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().JustBeforeInfo.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -1079,14 +1088,15 @@
 - To get the race result of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_race_result(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Result.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -1100,15 +1110,17 @@
      'kimarite': '逃げ',
      'note': [],
      'payoff': {'exacta': {'payoff': 400, 'popularity': 2, 'result': '1-5'},
                 'exacta_all': [{'payoff': 400, 'popularity': 2, 'result': '1-5'}],
                 'place_show': [{'payoff': 100, 'popularity': '', 'result': '1'},
                                {'payoff': 150, 'popularity': '', 'result': '5'}],
                 'place_show_all': [{'payoff': 100, 'popularity': '', 'result': '1'},
-                                   {'payoff': 150, 'popularity': '', 'result': '5'}],
+                                   {'payoff': 150,
+                                    'popularity': '',
+                                    'result': '5'}],
                 'quinella': {'payoff': 440, 'popularity': 2, 'result': '1=5'},
                 'quinella_all': [{'payoff': 440, 'popularity': 2, 'result': '1=5'}],
                 'quinella_place': [{'payoff': 110,
                                     'popularity': 2,
                                     'result': '1=5'},
                                    {'payoff': 110,
                                     'popularity': 1,
@@ -1135,31 +1147,31 @@
                 'win_all': [{'payoff': 100, 'popularity': '', 'result': '1'}]},
      'race': 1,
      'result': [{'boat': 1,
                  'name': '武田光史',
                  'racerid': 3654,
                  'rank': 1,
                  'time': '1\'49"2'},
-                 {'boat': 5,
+                {'boat': 5,
                  'name': '木田峰由季',
                  'racerid': 4587,
                  'rank': 2,
                  'time': '1\'50"8'},
-                 {'boat': 3,
+                {'boat': 3,
                  'name': '堀本裕也',
                  'racerid': 3895,
                  'rank': 3,
                  'time': '1\'52"6'},
-                 {'boat': 2,
+                {'boat': 2,
                  'name': '大澤誠也',
                  'racerid': 5074,
                  'rank': 4,
                  'time': '1\'54"1'},
-                 {'boat': 6, 'name': '加藤優弥', 'racerid': 5185, 'rank': 5, 'time': ''},
-                 {'boat': 4,
+                {'boat': 6, 'name': '加藤優弥', 'racerid': 5185, 'rank': 5, 'time': ''},
+                {'boat': 4,
                  'name': '信濃由行',
                  'racerid': 3620,
                  'rank': 6,
                  'time': ''}],
      'return': [],
      'stadium': 10,
      'start_information': {'course1': {'ST': 0.26, 'boat': 1},
@@ -1239,14 +1251,15 @@
         exacta_betting_dict: Dict[str, int],
         quinela_betting_dict: Dict[str, int],
         quinellaplace_betting_dict: Dict[str, int],
         win_betting_dict: Dict[str, int],
         placeshow_betting_dict: Dict[str, int],
       ) -> bool
       ```
+
     - ```python
       PyJPBoatrace().Bet.do(
         stadium:int,
         race:int,
         trifecta_betting_dict: Dict[str, int],
         trio_betting_dict: Dict[str, int],
         exacta_betting_dict: Dict[str, int],
@@ -1366,56 +1379,56 @@
 6. Create new Pull Request
 
 ### Setup the develop environment
 
 First, fork this repository and clone it to your local machine.
 
 ```bash
-$ git clone https://github.com/hmasdev/pyjpboatrace/
-$ cd pyjpboatrace
+git clone https://github.com/hmasdev/pyjpboatrace/
+cd pyjpboatrace
 ```
 
 Then, create a virtual environment for your development,
 and install the required libraries.
 
 ```bash
-$ python -m venv venv
-$ source venv/bin/activate  # for Linux or MacOS
-$ # venv\Scripts\activate  # for Windows
-$ pip install -e .[dev]
+python -m venv venv
+source venv/bin/activate  # for Linux or MacOS
+# venv\Scripts\activate  # for Windows
+pip install -e .[dev]
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv sync --dev
+pipenv sync --dev
 ```
 
 </details>
 
 ### Test
 
 <div id="HowToTestAnchor"></div>
 
 You can do unit tests and integration tests as follows:
 
 ```bash
-$ ./download_html_for_test.sh  # Only 1 time
-$ pytest -m "not integrate and not spending_money" # unit tests
-$ pytest # unit tests and integration tests
+./download_html_for_test.sh  # Only 1 time
+pytest -m "not integrate and not spending_money" # unit tests
+pytest # unit tests and integration tests
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ ./download_html_for_test.sh  # Only 1 time
-$ pipenv run pytest -m "not integrate and not spending_money" # unit tests
-$ pipenv run pytest  # unit tests and integration tests
+./download_html_for_test.sh  # Only 1 time
+pipenv run pytest -m "not integrate and not spending_money" # unit tests
+pipenv run pytest  # unit tests and integration tests
 ```
 
 </details>
 
 `pytest` does not test depositing, withdrawing or betting.
 If you want to test them, make `.secrets.json` at first:
 
@@ -1427,49 +1440,64 @@
   "vote_pass": "YOUR_BETTING_PASSWORD"
 }
 ```
 
 Then, run
 
 ```bash
-$ pytest -m "spending_money"
+pytest -m "spending_money"
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv run pytest -m "spending_money"
+pipenv run pytest -m "spending_money"
 ```
 
 </details>
 
 WARNING: Tests with `spending_money` spend 700 yen.
 
 ### Check the format of code and static types
 
 You should execute the following codes to check the format of code and static types:
 
 ```bash
-$ flake8 pyjpboatrace tests
-$ mypy pyjpboatrace tests
+flake8 pyjpboatrace tests
+mypy pyjpboatrace tests
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv run flake8 pyjpboatrace
-$ pipenv run flake8 tests
-$ pipenv run mypy pyjpboatrace
-$ pipenv run mypy tests
+pipenv run flake8 pyjpboatrace
+pipenv run flake8 tests
+pipenv run mypy pyjpboatrace
+pipenv run mypy tests
 ```
 
 </details>
 
+### How to Update README.md
+
+To update the content of [README.md](./README.md), please do not edit the file directly.
+Instead, make your changes to [README.md.j2](./README.md.j2).
+
+After making updates to `README.md.j2`, execute the following command to regenerate `README.md`:
+
+```bash
+python update_readme.py > README.md
+```
+
+This process is necessary because README.md is dynamically generated from the README.md.j2 template.
+Direct modifications to README.md will be lost, as they are automatically overwritten by an automated process whenever the template is updated.
+
+Remember, to preserve your changes, always update README.md.j2 and not README.md directly.
 
 ## LICENSE
 
 [MIT](https://github.com/hmasdev/pyjpboatrace/tree/main/LICENSE)
 
 ## Authors
```

### Comparing `pyjpboatrace-0.3.0a4/README.md` & `pyjpboatrace-0.3.1a0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # PyJPBoatRace: Python-based Japanese boatrace tools :speedboat:
 
 ![GitHub top language](https://img.shields.io/github/languages/top/hmasdev/pyjpboatrace)
 ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/hmasdev/pyjpboatrace?sort=semver)
 ![GitHub](https://img.shields.io/github/license/hmasdev/pyjpboatrace)
 ![GitHub last commit](https://img.shields.io/github/last-commit/hmasdev/pyjpboatrace)
-![pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
-![flake8](https://github.com/hmasdev/pyjpboatrace/actions/workflows/code-style-check.yaml/badge.svg)
-![mypy](https://github.com/hmasdev/pyjpboatrace/actions/workflows/static-type-check.yaml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/pyjpboatrace.svg)](https://pypi.org/project/pyjpboatrace/)
+![Scheduled Test](https://github.com/hmasdev/pyjpboatrace/actions/workflows/tests_on_schedule.yaml/badge.svg)
 
 Japanese boat race is extremely exciting sports.
 It is also fun to predict the results of races.
 Prediction like machine learning method requires data.
 Thus, this package provides you with useful tools for data analysis and auto-betting for boatrace.
 
 ## Installation
@@ -77,107 +76,108 @@
 - Get a list of stadiums which hold races on the given day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_stadiums(d: datetime.date) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Stadiums.get(d: datetime.date) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
 
     ```python
     >>> from pyjpboatrace import PyJPBoatrace
     >>> from datetime import date
     >>> from pprint import pprint
     >>> pprint(PyJPBoatrace().get_stadiums(date(2021, 8, 12)))
     {'date': '2021-08-12',
-    'びわこ': {'day': '３日目',
-            'grade': ['ippan'],
-            'period': ['2021-08-10', '2021-08-15'],
-            'status': '-',
-            'timeframe': '',
-            'title': '滋賀県知事杯争奪第２６回びわこカップ'},
-    '三国': {'day': '２日目',
+     'びわこ': {'day': '３日目',
+             'grade': ['ippan'],
+             'period': ['2021-08-10', '2021-08-15'],
+             'status': '-',
+             'timeframe': '',
+             'title': '滋賀県知事杯争奪第２６回びわこカップ'},
+     '三国': {'day': '２日目',
             'grade': ['ippan'],
             'period': ['2021-08-11', '2021-08-16'],
             'status': '-',
             'timeframe': 'morning',
             'title': '第４９回しぶき賞'},
-    '下関': {'day': '最終日',
+     '下関': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-06', '2021-08-12'],
             'status': '-',
             'timeframe': 'nighter',
             'title': 'Ｈａｙａｓｈｉｋａｎｅ杯'},
-    '唐津': {'day': '最終日',
+     '唐津': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-07', '2021-08-12'],
             'status': '-',
             'timeframe': 'morning',
             'title': '唐津大賞がばい王者決定戦'},
-    '多摩川': {'day': '最終日',
-            'grade': ['ippan'],
-            'period': ['2021-08-08', '2021-08-12'],
-            'status': '-',
-            'timeframe': 'summer',
-            'title': '第５９回スポーツニッポン賞'},
-    '宮島': {'day': '最終日',
+     '多摩川': {'day': '最終日',
+             'grade': ['ippan'],
+             'period': ['2021-08-08', '2021-08-12'],
+             'status': '-',
+             'timeframe': 'summer',
+             'title': '第５９回スポーツニッポン賞'},
+     '宮島': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-07', '2021-08-12'],
             'status': '-',
             'timeframe': '',
             'title': '第５１回スポーツニッポン杯'},
-    '尼崎': {'day': '４日目',
+     '尼崎': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-09', '2021-08-14'],
             'status': '-',
             'timeframe': '',
             'title': '日本財団会長杯争奪第４９回オール兵庫王座決定戦'},
-    '常滑': {'day': '２日目',
+     '常滑': {'day': '２日目',
             'grade': ['ippan'],
             'period': ['2021-08-11', '2021-08-16'],
             'status': '-',
             'timeframe': '',
             'title': '名鉄杯争奪２０２１納涼お盆レース'},
-    '平和島': {'day': '３日目',
-            'grade': ['ippan'],
-            'period': ['2021-08-10', '2021-08-15'],
-            'status': '-',
-            'timeframe': 'summer',
-            'title': '第６１回デイリースポーツサマーカップ'},
-    '戸田': {'day': '初日',
+     '平和島': {'day': '３日目',
+             'grade': ['ippan'],
+             'period': ['2021-08-10', '2021-08-15'],
+             'status': '-',
+             'timeframe': 'summer',
+             'title': '第６１回デイリースポーツサマーカップ'},
+     '戸田': {'day': '初日',
             'grade': ['ippan'],
             'period': ['2021-08-12', '2021-08-17'],
             'status': '-',
             'timeframe': '',
             'title': '第４４回戸田ボート大賞・サンケイスポーツ杯'},
-    '桐生': {'day': '３日目',
+     '桐生': {'day': '３日目',
             'grade': ['ippan'],
             'period': ['2021-08-10', '2021-08-15'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '第５５回報知新聞社杯\u3000お盆レース'},
-    '若松': {'day': '４日目',
+     '若松': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-08', '2021-08-13'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '日刊スポーツ杯お盆特選競走'},
-    '蒲郡': {'day': '初日',
+     '蒲郡': {'day': '初日',
             'grade': ['ippan'],
             'period': ['2021-08-12', '2021-08-17'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '日刊スポーツ杯争奪\u3000納涼しぶきお盆特別選抜戦'},
-    '鳴門': {'day': '４日目',
+     '鳴門': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-09', '2021-08-14'],
             'status': '-',
             'timeframe': 'morning',
             'title': '第５４回渦王杯競走'}}
     ```
 
@@ -186,14 +186,15 @@
 - To get 12 races held in the given stadium on the given day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_12races(d: datetime.date, stadium: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Races.get(d: datetime.date, stadium: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -229,93 +230,94 @@
              'vote_limit': '2021-08-12 20:45:00'},
      '1R': {'racers': {'boat1': {'class': 'B1', 'name': '渡辺史之'},
                        'boat2': {'class': 'B1', 'name': '島倉都'},
                        'boat3': {'class': 'A2', 'name': '鳥居塚孝博'},
                        'boat4': {'class': 'B1', 'name': '松本純平'},
                        'boat5': {'class': 'A2', 'name': '橋本久和'},
                        'boat6': {'class': 'B2', 'name': '宮崎安奈'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 15:22:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 15:22:00'},
      '2R': {'racers': {'boat1': {'class': 'B1', 'name': '佐口達也'},
                        'boat2': {'class': 'A2', 'name': '本橋克洋'},
                        'boat3': {'class': 'B1', 'name': '寺本昇平'},
                        'boat4': {'class': 'B1', 'name': '津久井拓也'},
                        'boat5': {'class': 'B1', 'name': '久保原秀人'},
                        'boat6': {'class': 'A2', 'name': '中里英夫'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 15:49:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 15:49:00'},
      '3R': {'racers': {'boat1': {'class': 'B1', 'name': '小川時光'},
                        'boat2': {'class': 'A2', 'name': '野村誠'},
                        'boat3': {'class': 'B2', 'name': '黄金井裕子'},
                        'boat4': {'class': 'A2', 'name': '藤生雄人'},
                        'boat5': {'class': 'B1', 'name': '高山秀雄'},
                        'boat6': {'class': 'A1', 'name': '関浩哉'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 16:16:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 16:16:00'},
      '4R': {'racers': {'boat1': {'class': 'B1', 'name': '栗原謙治'},
                        'boat2': {'class': 'A2', 'name': '金子賢志'},
                        'boat3': {'class': 'B1', 'name': '関根彰人'},
                        'boat4': {'class': 'A1', 'name': '金子拓矢'},
                        'boat5': {'class': 'B2', 'name': '大久保佑香'},
                        'boat6': {'class': 'B1', 'name': '土屋太朗'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 16:45:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 16:45:00'},
      '5R': {'racers': {'boat1': {'class': 'B1', 'name': '原加央理'},
                        'boat2': {'class': 'B1', 'name': '佐藤航'},
                        'boat3': {'class': 'B1', 'name': '蜂須瑞生'},
                        'boat4': {'class': 'A2', 'name': '一柳和孝'},
                        'boat5': {'class': 'B1', 'name': '外崎悟'},
                        'boat6': {'class': 'A1', 'name': '毒島誠'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 17:13:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 17:13:00'},
      '6R': {'racers': {'boat1': {'class': 'A1', 'name': '椎名豊'},
                        'boat2': {'class': 'B1', 'name': '久保田美紀'},
                        'boat3': {'class': 'B1', 'name': '太田克哉'},
                        'boat4': {'class': 'B1', 'name': '島倉都'},
                        'boat5': {'class': 'B1', 'name': '金澤一洋'},
                        'boat6': {'class': 'B1', 'name': '寺本昇平'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 17:42:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 17:42:00'},
      '7R': {'racers': {'boat1': {'class': 'A2', 'name': '木村浩士'},
                        'boat2': {'class': 'B1', 'name': '久保原秀人'},
                        'boat3': {'class': 'A1', 'name': '上村純一'},
                        'boat4': {'class': 'B1', 'name': '鹿島敏弘'},
                        'boat5': {'class': 'B2', 'name': '宮崎安奈'},
                        'boat6': {'class': 'B2', 'name': '黄金井裕子'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 18:11:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 18:11:00'},
      '8R': {'racers': {'boat1': {'class': 'A2', 'name': '鳥居塚孝博'},
                        'boat2': {'class': 'B1', 'name': '高山秀雄'},
                        'boat3': {'class': 'B1', 'name': '吉田稔'},
                        'boat4': {'class': 'B1', 'name': '田中定雄'},
                        'boat5': {'class': 'A1', 'name': '久田敏之'},
                        'boat6': {'class': 'B2', 'name': '大久保佑香'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 18:41:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 18:41:00'},
      '9R': {'racers': {'boat1': {'class': 'B1', 'name': '崎利仁'},
                        'boat2': {'class': 'A2', 'name': '中里英夫'},
                        'boat3': {'class': 'B1', 'name': '塚原武之'},
                        'boat4': {'class': 'A1', 'name': '土屋智則'},
                        'boat5': {'class': 'B1', 'name': '関根彰人'},
                        'boat6': {'class': 'A1', 'name': '山崎智也'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 19:12:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 19:12:00'},
      'date': '2021-08-12',
      'stadium': 1}
     ```
 
     </details>
 
 - To get the basic information of the race in the stadium on a day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_race_info(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().RaceInfo.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -347,31 +349,31 @@
                'name': '武田光史',
                'racerid': 3654,
                'result': [{'ST': 0.19,
                            'boat': 5,
                            'course': 5,
                            'race': 6,
                            'rank': 4},
-                           {'ST': 0.14,
+                          {'ST': 0.14,
                            'boat': 3,
                            'course': 3,
                            'race': 12,
                            'rank': 5},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.6},
      'boat2': {'F': 0,
                'L': 0,
                'age': 25,
                'aveST': 0.21,
                'birthplace': '愛知',
                'boat': 64,
@@ -391,27 +393,27 @@
                'name': '大澤誠也',
                'racerid': 5074,
                'result': [{'ST': 0.19,
                            'boat': 3,
                            'course': 3,
                            'race': 6,
                            'rank': 3},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 53.1},
      'boat3': {'F': 0,
                'L': 0,
                'age': 45,
                'aveST': 0.17,
                'birthplace': '愛知',
                'boat': 41,
@@ -431,31 +433,31 @@
                'name': '堀本裕也',
                'racerid': 3895,
                'result': [{'ST': 0.06,
                            'boat': 5,
                            'course': 5,
                            'race': 4,
                            'rank': 5},
-                           {'ST': 0.2,
+                          {'ST': 0.2,
                            'boat': 2,
                            'course': 2,
                            'race': 11,
                            'rank': 4},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 50.0},
      'boat4': {'F': 0,
                'L': 0,
                'age': 47,
                'aveST': 0.18,
                'birthplace': '石川',
                'boat': 36,
@@ -475,27 +477,27 @@
                'name': '信濃由行',
                'racerid': 3620,
                'result': [{'ST': 0.26,
                            'boat': 5,
                            'course': 3,
                            'race': 3,
                            'rank': 5},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.3},
      'boat5': {'F': 0,
                'L': 0,
                'age': 30,
                'aveST': 0.19,
                'birthplace': '石川',
                'boat': 17,
@@ -515,31 +517,31 @@
                'name': '木田峰由季',
                'racerid': 4587,
                'result': [{'ST': 0.19,
                            'boat': 2,
                            'course': 2,
                            'race': 3,
                            'rank': 3},
-                           {'ST': 0.21,
+                          {'ST': 0.21,
                            'boat': 4,
                            'course': 5,
                            'race': 10,
                            'rank': 2},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.2},
      'boat6': {'F': 0,
                'L': 0,
                'age': 21,
                'aveST': '-',
                'birthplace': '福井',
                'boat': 15,
@@ -559,27 +561,27 @@
                'name': '加藤優弥',
                'racerid': 5185,
                'result': [{'ST': 0.01,
                            'boat': 6,
                            'course': 6,
                            'race': 4,
                            'rank': 6},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.6},
      'date': '2021-08-12',
      'race': 1,
      'race_title': ['みくにあさイチ', '1800m'],
      'stadium': 10}
     ```
 
@@ -588,14 +590,15 @@
 - To get the odds of win (単勝) and place-show (複勝) of the race in the stadium on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_win_placeshow(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().WinPlaceshowOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -623,14 +626,15 @@
 - To get the odds of quinella place (拡連複) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_quinellaplace(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().QuinellaplaceOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -666,14 +670,15 @@
 - To get the odds of exacta (二連単) and quinella (二連複) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_exacta_quinella(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().ExactaQuinellaOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -739,14 +744,15 @@
 - To get the odds of trifecta (三連単) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_trifecta(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBaotrace().TrifectaOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -887,14 +893,15 @@
 - To get the oods of trio （三連複） of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_trio(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Trio.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -935,14 +942,15 @@
 - To get the just-before information, e.g. weather and start-timing, of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_just_before_info(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().JustBeforeInfo.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -1024,14 +1032,15 @@
 - To get the race result of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_race_result(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Result.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -1045,15 +1054,17 @@
      'kimarite': '逃げ',
      'note': [],
      'payoff': {'exacta': {'payoff': 400, 'popularity': 2, 'result': '1-5'},
                 'exacta_all': [{'payoff': 400, 'popularity': 2, 'result': '1-5'}],
                 'place_show': [{'payoff': 100, 'popularity': '', 'result': '1'},
                                {'payoff': 150, 'popularity': '', 'result': '5'}],
                 'place_show_all': [{'payoff': 100, 'popularity': '', 'result': '1'},
-                                   {'payoff': 150, 'popularity': '', 'result': '5'}],
+                                   {'payoff': 150,
+                                    'popularity': '',
+                                    'result': '5'}],
                 'quinella': {'payoff': 440, 'popularity': 2, 'result': '1=5'},
                 'quinella_all': [{'payoff': 440, 'popularity': 2, 'result': '1=5'}],
                 'quinella_place': [{'payoff': 110,
                                     'popularity': 2,
                                     'result': '1=5'},
                                    {'payoff': 110,
                                     'popularity': 1,
@@ -1080,31 +1091,31 @@
                 'win_all': [{'payoff': 100, 'popularity': '', 'result': '1'}]},
      'race': 1,
      'result': [{'boat': 1,
                  'name': '武田光史',
                  'racerid': 3654,
                  'rank': 1,
                  'time': '1\'49"2'},
-                 {'boat': 5,
+                {'boat': 5,
                  'name': '木田峰由季',
                  'racerid': 4587,
                  'rank': 2,
                  'time': '1\'50"8'},
-                 {'boat': 3,
+                {'boat': 3,
                  'name': '堀本裕也',
                  'racerid': 3895,
                  'rank': 3,
                  'time': '1\'52"6'},
-                 {'boat': 2,
+                {'boat': 2,
                  'name': '大澤誠也',
                  'racerid': 5074,
                  'rank': 4,
                  'time': '1\'54"1'},
-                 {'boat': 6, 'name': '加藤優弥', 'racerid': 5185, 'rank': 5, 'time': ''},
-                 {'boat': 4,
+                {'boat': 6, 'name': '加藤優弥', 'racerid': 5185, 'rank': 5, 'time': ''},
+                {'boat': 4,
                  'name': '信濃由行',
                  'racerid': 3620,
                  'rank': 6,
                  'time': ''}],
      'return': [],
      'stadium': 10,
      'start_information': {'course1': {'ST': 0.26, 'boat': 1},
@@ -1184,14 +1195,15 @@
         exacta_betting_dict: Dict[str, int],
         quinela_betting_dict: Dict[str, int],
         quinellaplace_betting_dict: Dict[str, int],
         win_betting_dict: Dict[str, int],
         placeshow_betting_dict: Dict[str, int],
       ) -> bool
       ```
+
     - ```python
       PyJPBoatrace().Bet.do(
         stadium:int,
         race:int,
         trifecta_betting_dict: Dict[str, int],
         trio_betting_dict: Dict[str, int],
         exacta_betting_dict: Dict[str, int],
@@ -1311,56 +1323,56 @@
 6. Create new Pull Request
 
 ### Setup the develop environment
 
 First, fork this repository and clone it to your local machine.
 
 ```bash
-$ git clone https://github.com/hmasdev/pyjpboatrace/
-$ cd pyjpboatrace
+git clone https://github.com/hmasdev/pyjpboatrace/
+cd pyjpboatrace
 ```
 
 Then, create a virtual environment for your development,
 and install the required libraries.
 
 ```bash
-$ python -m venv venv
-$ source venv/bin/activate  # for Linux or MacOS
-$ # venv\Scripts\activate  # for Windows
-$ pip install -e .[dev]
+python -m venv venv
+source venv/bin/activate  # for Linux or MacOS
+# venv\Scripts\activate  # for Windows
+pip install -e .[dev]
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv sync --dev
+pipenv sync --dev
 ```
 
 </details>
 
 ### Test
 
 <div id="HowToTestAnchor"></div>
 
 You can do unit tests and integration tests as follows:
 
 ```bash
-$ ./download_html_for_test.sh  # Only 1 time
-$ pytest -m "not integrate and not spending_money" # unit tests
-$ pytest # unit tests and integration tests
+./download_html_for_test.sh  # Only 1 time
+pytest -m "not integrate and not spending_money" # unit tests
+pytest # unit tests and integration tests
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ ./download_html_for_test.sh  # Only 1 time
-$ pipenv run pytest -m "not integrate and not spending_money" # unit tests
-$ pipenv run pytest  # unit tests and integration tests
+./download_html_for_test.sh  # Only 1 time
+pipenv run pytest -m "not integrate and not spending_money" # unit tests
+pipenv run pytest  # unit tests and integration tests
 ```
 
 </details>
 
 `pytest` does not test depositing, withdrawing or betting.
 If you want to test them, make `.secrets.json` at first:
 
@@ -1372,49 +1384,64 @@
   "vote_pass": "YOUR_BETTING_PASSWORD"
 }
 ```
 
 Then, run
 
 ```bash
-$ pytest -m "spending_money"
+pytest -m "spending_money"
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv run pytest -m "spending_money"
+pipenv run pytest -m "spending_money"
 ```
 
 </details>
 
 WARNING: Tests with `spending_money` spend 700 yen.
 
 ### Check the format of code and static types
 
 You should execute the following codes to check the format of code and static types:
 
 ```bash
-$ flake8 pyjpboatrace tests
-$ mypy pyjpboatrace tests
+flake8 pyjpboatrace tests
+mypy pyjpboatrace tests
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv run flake8 pyjpboatrace
-$ pipenv run flake8 tests
-$ pipenv run mypy pyjpboatrace
-$ pipenv run mypy tests
+pipenv run flake8 pyjpboatrace
+pipenv run flake8 tests
+pipenv run mypy pyjpboatrace
+pipenv run mypy tests
 ```
 
 </details>
 
+### How to Update README.md
+
+To update the content of [README.md](./README.md), please do not edit the file directly.
+Instead, make your changes to [README.md.j2](./README.md.j2).
+
+After making updates to `README.md.j2`, execute the following command to regenerate `README.md`:
+
+```bash
+python update_readme.py > README.md
+```
+
+This process is necessary because README.md is dynamically generated from the README.md.j2 template.
+Direct modifications to README.md will be lost, as they are automatically overwritten by an automated process whenever the template is updated.
+
+Remember, to preserve your changes, always update README.md.j2 and not README.md directly.
 
 ## LICENSE
 
 [MIT](https://github.com/hmasdev/pyjpboatrace/tree/main/LICENSE)
 
 ## Authors
```

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace/__init__.py` & `pyjpboatrace-0.3.1a0/pyjpboatrace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import pyjpboatrace
 from . import scraper
 from . import user_information
 from . import utils
 from . import validator
 
 
-__version__ = 'v0.3.0a4'
+__version__ = 'v0.3.1a0'
 
 __all__ = [
     PyJPBoatrace.__name__,
     certification.__name__,
     const.__name__,
     drivers.__name__,
     exceptions.__name__,
```

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace/certification.py` & `pyjpboatrace-0.3.1a0/pyjpboatrace/certification.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace/const.py` & `pyjpboatrace-0.3.1a0/pyjpboatrace/const.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace/drivers.py` & `pyjpboatrace-0.3.1a0/pyjpboatrace/drivers.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace/exceptions.py` & `pyjpboatrace-0.3.1a0/pyjpboatrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace/pyjpboatrace.py` & `pyjpboatrace-0.3.1a0/pyjpboatrace/pyjpboatrace.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace/user_information.py` & `pyjpboatrace-0.3.1a0/pyjpboatrace/user_information.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace/validator.py` & `pyjpboatrace-0.3.1a0/pyjpboatrace/validator.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/PKG-INFO` & `pyjpboatrace-0.3.1a0/pyjpboatrace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjpboatrace
-Version: 0.3.0a4
+Version: 0.3.1a0
 Summary: PyJPBoatrace: Python-based Japanese boatrace tools
 Author-email: hmasdev <hmasuidev1com@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 hmasdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,31 +41,31 @@
 Requires-Dist: requests>=2.28.1
 Requires-Dist: selenium>=4.6.0
 Requires-Dist: types-beautifulsoup4
 Requires-Dist: types-requests
 Provides-Extra: dev
 Requires-Dist: autopep8; extra == "dev"
 Requires-Dist: flake8>=3.8.4; extra == "dev"
+Requires-Dist: Jinja2; extra == "dev"
 Requires-Dist: mypy>=0.812; extra == "dev"
 Requires-Dist: pytest>=6.1.2; extra == "dev"
 Requires-Dist: pytest-cov>=2.10.1; extra == "dev"
 Requires-Dist: pytz; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: types-pytz; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 # PyJPBoatRace: Python-based Japanese boatrace tools :speedboat:
 
 ![GitHub top language](https://img.shields.io/github/languages/top/hmasdev/pyjpboatrace)
 ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/hmasdev/pyjpboatrace?sort=semver)
 ![GitHub](https://img.shields.io/github/license/hmasdev/pyjpboatrace)
 ![GitHub last commit](https://img.shields.io/github/last-commit/hmasdev/pyjpboatrace)
-![pytest](https://github.com/hmasdev/pyjpboatrace/actions/workflows/pytest.yaml/badge.svg)
-![flake8](https://github.com/hmasdev/pyjpboatrace/actions/workflows/code-style-check.yaml/badge.svg)
-![mypy](https://github.com/hmasdev/pyjpboatrace/actions/workflows/static-type-check.yaml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/pyjpboatrace.svg)](https://pypi.org/project/pyjpboatrace/)
+![Scheduled Test](https://github.com/hmasdev/pyjpboatrace/actions/workflows/tests_on_schedule.yaml/badge.svg)
 
 Japanese boat race is extremely exciting sports.
 It is also fun to predict the results of races.
 Prediction like machine learning method requires data.
 Thus, this package provides you with useful tools for data analysis and auto-betting for boatrace.
 
 ## Installation
@@ -132,107 +132,108 @@
 - Get a list of stadiums which hold races on the given day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_stadiums(d: datetime.date) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Stadiums.get(d: datetime.date) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
 
     ```python
     >>> from pyjpboatrace import PyJPBoatrace
     >>> from datetime import date
     >>> from pprint import pprint
     >>> pprint(PyJPBoatrace().get_stadiums(date(2021, 8, 12)))
     {'date': '2021-08-12',
-    'びわこ': {'day': '３日目',
-            'grade': ['ippan'],
-            'period': ['2021-08-10', '2021-08-15'],
-            'status': '-',
-            'timeframe': '',
-            'title': '滋賀県知事杯争奪第２６回びわこカップ'},
-    '三国': {'day': '２日目',
+     'びわこ': {'day': '３日目',
+             'grade': ['ippan'],
+             'period': ['2021-08-10', '2021-08-15'],
+             'status': '-',
+             'timeframe': '',
+             'title': '滋賀県知事杯争奪第２６回びわこカップ'},
+     '三国': {'day': '２日目',
             'grade': ['ippan'],
             'period': ['2021-08-11', '2021-08-16'],
             'status': '-',
             'timeframe': 'morning',
             'title': '第４９回しぶき賞'},
-    '下関': {'day': '最終日',
+     '下関': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-06', '2021-08-12'],
             'status': '-',
             'timeframe': 'nighter',
             'title': 'Ｈａｙａｓｈｉｋａｎｅ杯'},
-    '唐津': {'day': '最終日',
+     '唐津': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-07', '2021-08-12'],
             'status': '-',
             'timeframe': 'morning',
             'title': '唐津大賞がばい王者決定戦'},
-    '多摩川': {'day': '最終日',
-            'grade': ['ippan'],
-            'period': ['2021-08-08', '2021-08-12'],
-            'status': '-',
-            'timeframe': 'summer',
-            'title': '第５９回スポーツニッポン賞'},
-    '宮島': {'day': '最終日',
+     '多摩川': {'day': '最終日',
+             'grade': ['ippan'],
+             'period': ['2021-08-08', '2021-08-12'],
+             'status': '-',
+             'timeframe': 'summer',
+             'title': '第５９回スポーツニッポン賞'},
+     '宮島': {'day': '最終日',
             'grade': ['ippan'],
             'period': ['2021-08-07', '2021-08-12'],
             'status': '-',
             'timeframe': '',
             'title': '第５１回スポーツニッポン杯'},
-    '尼崎': {'day': '４日目',
+     '尼崎': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-09', '2021-08-14'],
             'status': '-',
             'timeframe': '',
             'title': '日本財団会長杯争奪第４９回オール兵庫王座決定戦'},
-    '常滑': {'day': '２日目',
+     '常滑': {'day': '２日目',
             'grade': ['ippan'],
             'period': ['2021-08-11', '2021-08-16'],
             'status': '-',
             'timeframe': '',
             'title': '名鉄杯争奪２０２１納涼お盆レース'},
-    '平和島': {'day': '３日目',
-            'grade': ['ippan'],
-            'period': ['2021-08-10', '2021-08-15'],
-            'status': '-',
-            'timeframe': 'summer',
-            'title': '第６１回デイリースポーツサマーカップ'},
-    '戸田': {'day': '初日',
+     '平和島': {'day': '３日目',
+             'grade': ['ippan'],
+             'period': ['2021-08-10', '2021-08-15'],
+             'status': '-',
+             'timeframe': 'summer',
+             'title': '第６１回デイリースポーツサマーカップ'},
+     '戸田': {'day': '初日',
             'grade': ['ippan'],
             'period': ['2021-08-12', '2021-08-17'],
             'status': '-',
             'timeframe': '',
             'title': '第４４回戸田ボート大賞・サンケイスポーツ杯'},
-    '桐生': {'day': '３日目',
+     '桐生': {'day': '３日目',
             'grade': ['ippan'],
             'period': ['2021-08-10', '2021-08-15'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '第５５回報知新聞社杯\u3000お盆レース'},
-    '若松': {'day': '４日目',
+     '若松': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-08', '2021-08-13'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '日刊スポーツ杯お盆特選競走'},
-    '蒲郡': {'day': '初日',
+     '蒲郡': {'day': '初日',
             'grade': ['ippan'],
             'period': ['2021-08-12', '2021-08-17'],
             'status': '-',
             'timeframe': 'nighter',
             'title': '日刊スポーツ杯争奪\u3000納涼しぶきお盆特別選抜戦'},
-    '鳴門': {'day': '４日目',
+     '鳴門': {'day': '４日目',
             'grade': ['ippan'],
             'period': ['2021-08-09', '2021-08-14'],
             'status': '-',
             'timeframe': 'morning',
             'title': '第５４回渦王杯競走'}}
     ```
 
@@ -241,14 +242,15 @@
 - To get 12 races held in the given stadium on the given day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_12races(d: datetime.date, stadium: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Races.get(d: datetime.date, stadium: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -284,93 +286,94 @@
              'vote_limit': '2021-08-12 20:45:00'},
      '1R': {'racers': {'boat1': {'class': 'B1', 'name': '渡辺史之'},
                        'boat2': {'class': 'B1', 'name': '島倉都'},
                        'boat3': {'class': 'A2', 'name': '鳥居塚孝博'},
                        'boat4': {'class': 'B1', 'name': '松本純平'},
                        'boat5': {'class': 'A2', 'name': '橋本久和'},
                        'boat6': {'class': 'B2', 'name': '宮崎安奈'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 15:22:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 15:22:00'},
      '2R': {'racers': {'boat1': {'class': 'B1', 'name': '佐口達也'},
                        'boat2': {'class': 'A2', 'name': '本橋克洋'},
                        'boat3': {'class': 'B1', 'name': '寺本昇平'},
                        'boat4': {'class': 'B1', 'name': '津久井拓也'},
                        'boat5': {'class': 'B1', 'name': '久保原秀人'},
                        'boat6': {'class': 'A2', 'name': '中里英夫'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 15:49:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 15:49:00'},
      '3R': {'racers': {'boat1': {'class': 'B1', 'name': '小川時光'},
                        'boat2': {'class': 'A2', 'name': '野村誠'},
                        'boat3': {'class': 'B2', 'name': '黄金井裕子'},
                        'boat4': {'class': 'A2', 'name': '藤生雄人'},
                        'boat5': {'class': 'B1', 'name': '高山秀雄'},
                        'boat6': {'class': 'A1', 'name': '関浩哉'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 16:16:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 16:16:00'},
      '4R': {'racers': {'boat1': {'class': 'B1', 'name': '栗原謙治'},
                        'boat2': {'class': 'A2', 'name': '金子賢志'},
                        'boat3': {'class': 'B1', 'name': '関根彰人'},
                        'boat4': {'class': 'A1', 'name': '金子拓矢'},
                        'boat5': {'class': 'B2', 'name': '大久保佑香'},
                        'boat6': {'class': 'B1', 'name': '土屋太朗'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 16:45:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 16:45:00'},
      '5R': {'racers': {'boat1': {'class': 'B1', 'name': '原加央理'},
                        'boat2': {'class': 'B1', 'name': '佐藤航'},
                        'boat3': {'class': 'B1', 'name': '蜂須瑞生'},
                        'boat4': {'class': 'A2', 'name': '一柳和孝'},
                        'boat5': {'class': 'B1', 'name': '外崎悟'},
                        'boat6': {'class': 'A1', 'name': '毒島誠'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 17:13:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 17:13:00'},
      '6R': {'racers': {'boat1': {'class': 'A1', 'name': '椎名豊'},
                        'boat2': {'class': 'B1', 'name': '久保田美紀'},
                        'boat3': {'class': 'B1', 'name': '太田克哉'},
                        'boat4': {'class': 'B1', 'name': '島倉都'},
                        'boat5': {'class': 'B1', 'name': '金澤一洋'},
                        'boat6': {'class': 'B1', 'name': '寺本昇平'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 17:42:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 17:42:00'},
      '7R': {'racers': {'boat1': {'class': 'A2', 'name': '木村浩士'},
                        'boat2': {'class': 'B1', 'name': '久保原秀人'},
                        'boat3': {'class': 'A1', 'name': '上村純一'},
                        'boat4': {'class': 'B1', 'name': '鹿島敏弘'},
                        'boat5': {'class': 'B2', 'name': '宮崎安奈'},
                        'boat6': {'class': 'B2', 'name': '黄金井裕子'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 18:11:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 18:11:00'},
      '8R': {'racers': {'boat1': {'class': 'A2', 'name': '鳥居塚孝博'},
                        'boat2': {'class': 'B1', 'name': '高山秀雄'},
                        'boat3': {'class': 'B1', 'name': '吉田稔'},
                        'boat4': {'class': 'B1', 'name': '田中定雄'},
                        'boat5': {'class': 'A1', 'name': '久田敏之'},
                        'boat6': {'class': 'B2', 'name': '大久保佑香'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 18:41:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 18:41:00'},
      '9R': {'racers': {'boat1': {'class': 'B1', 'name': '崎利仁'},
                        'boat2': {'class': 'A2', 'name': '中里英夫'},
                        'boat3': {'class': 'B1', 'name': '塚原武之'},
                        'boat4': {'class': 'A1', 'name': '土屋智則'},
                        'boat5': {'class': 'B1', 'name': '関根彰人'},
                        'boat6': {'class': 'A1', 'name': '山崎智也'}},
-             'status': '発売終了',
-             'vote_limit': '2021-08-12 19:12:00'},
+            'status': '発売終了',
+            'vote_limit': '2021-08-12 19:12:00'},
      'date': '2021-08-12',
      'stadium': 1}
     ```
 
     </details>
 
 - To get the basic information of the race in the stadium on a day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_race_info(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().RaceInfo.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -402,31 +405,31 @@
                'name': '武田光史',
                'racerid': 3654,
                'result': [{'ST': 0.19,
                            'boat': 5,
                            'course': 5,
                            'race': 6,
                            'rank': 4},
-                           {'ST': 0.14,
+                          {'ST': 0.14,
                            'boat': 3,
                            'course': 3,
                            'race': 12,
                            'rank': 5},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.6},
      'boat2': {'F': 0,
                'L': 0,
                'age': 25,
                'aveST': 0.21,
                'birthplace': '愛知',
                'boat': 64,
@@ -446,27 +449,27 @@
                'name': '大澤誠也',
                'racerid': 5074,
                'result': [{'ST': 0.19,
                            'boat': 3,
                            'course': 3,
                            'race': 6,
                            'rank': 3},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 53.1},
      'boat3': {'F': 0,
                'L': 0,
                'age': 45,
                'aveST': 0.17,
                'birthplace': '愛知',
                'boat': 41,
@@ -486,31 +489,31 @@
                'name': '堀本裕也',
                'racerid': 3895,
                'result': [{'ST': 0.06,
                            'boat': 5,
                            'course': 5,
                            'race': 4,
                            'rank': 5},
-                           {'ST': 0.2,
+                          {'ST': 0.2,
                            'boat': 2,
                            'course': 2,
                            'race': 11,
                            'rank': 4},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 50.0},
      'boat4': {'F': 0,
                'L': 0,
                'age': 47,
                'aveST': 0.18,
                'birthplace': '石川',
                'boat': 36,
@@ -530,27 +533,27 @@
                'name': '信濃由行',
                'racerid': 3620,
                'result': [{'ST': 0.26,
                            'boat': 5,
                            'course': 3,
                            'race': 3,
                            'rank': 5},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.3},
      'boat5': {'F': 0,
                'L': 0,
                'age': 30,
                'aveST': 0.19,
                'birthplace': '石川',
                'boat': 17,
@@ -570,31 +573,31 @@
                'name': '木田峰由季',
                'racerid': 4587,
                'result': [{'ST': 0.19,
                            'boat': 2,
                            'course': 2,
                            'race': 3,
                            'rank': 3},
-                           {'ST': 0.21,
+                          {'ST': 0.21,
                            'boat': 4,
                            'course': 5,
                            'race': 10,
                            'rank': 2},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.2},
      'boat6': {'F': 0,
                'L': 0,
                'age': 21,
                'aveST': '-',
                'birthplace': '福井',
                'boat': 15,
@@ -614,27 +617,27 @@
                'name': '加藤優弥',
                'racerid': 5185,
                'result': [{'ST': 0.01,
                            'boat': 6,
                            'course': 6,
                            'race': 4,
                            'rank': 6},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {},
-                           {}],
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {},
+                          {}],
                'weight': 52.6},
      'date': '2021-08-12',
      'race': 1,
      'race_title': ['みくにあさイチ', '1800m'],
      'stadium': 10}
     ```
 
@@ -643,14 +646,15 @@
 - To get the odds of win (単勝) and place-show (複勝) of the race in the stadium on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_win_placeshow(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().WinPlaceshowOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -678,14 +682,15 @@
 - To get the odds of quinella place (拡連複) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_quinellaplace(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().QuinellaplaceOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -721,14 +726,15 @@
 - To get the odds of exacta (二連単) and quinella (二連複) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_exacta_quinella(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().ExactaQuinellaOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -794,14 +800,15 @@
 - To get the odds of trifecta (三連単) of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_trifecta(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBaotrace().TrifectaOdds.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -942,14 +949,15 @@
 - To get the oods of trio （三連複） of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_odds_trio(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Trio.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -990,14 +998,15 @@
 - To get the just-before information, e.g. weather and start-timing, of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_just_before_info(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().JustBeforeInfo.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -1079,14 +1088,15 @@
 - To get the race result of the race in the stadioum on the day:
 
   - API:
 
     - ```python
       PyJPBoatrace().get_race_result(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
+
     - ```python
       PyJPBoatrace().Result.get(d: datetime.date, stadium: int, race: int) -> Dict[str, Any]
       ```
 
   - Return:
     <details>
     <summary> Sample </summary>
@@ -1100,15 +1110,17 @@
      'kimarite': '逃げ',
      'note': [],
      'payoff': {'exacta': {'payoff': 400, 'popularity': 2, 'result': '1-5'},
                 'exacta_all': [{'payoff': 400, 'popularity': 2, 'result': '1-5'}],
                 'place_show': [{'payoff': 100, 'popularity': '', 'result': '1'},
                                {'payoff': 150, 'popularity': '', 'result': '5'}],
                 'place_show_all': [{'payoff': 100, 'popularity': '', 'result': '1'},
-                                   {'payoff': 150, 'popularity': '', 'result': '5'}],
+                                   {'payoff': 150,
+                                    'popularity': '',
+                                    'result': '5'}],
                 'quinella': {'payoff': 440, 'popularity': 2, 'result': '1=5'},
                 'quinella_all': [{'payoff': 440, 'popularity': 2, 'result': '1=5'}],
                 'quinella_place': [{'payoff': 110,
                                     'popularity': 2,
                                     'result': '1=5'},
                                    {'payoff': 110,
                                     'popularity': 1,
@@ -1135,31 +1147,31 @@
                 'win_all': [{'payoff': 100, 'popularity': '', 'result': '1'}]},
      'race': 1,
      'result': [{'boat': 1,
                  'name': '武田光史',
                  'racerid': 3654,
                  'rank': 1,
                  'time': '1\'49"2'},
-                 {'boat': 5,
+                {'boat': 5,
                  'name': '木田峰由季',
                  'racerid': 4587,
                  'rank': 2,
                  'time': '1\'50"8'},
-                 {'boat': 3,
+                {'boat': 3,
                  'name': '堀本裕也',
                  'racerid': 3895,
                  'rank': 3,
                  'time': '1\'52"6'},
-                 {'boat': 2,
+                {'boat': 2,
                  'name': '大澤誠也',
                  'racerid': 5074,
                  'rank': 4,
                  'time': '1\'54"1'},
-                 {'boat': 6, 'name': '加藤優弥', 'racerid': 5185, 'rank': 5, 'time': ''},
-                 {'boat': 4,
+                {'boat': 6, 'name': '加藤優弥', 'racerid': 5185, 'rank': 5, 'time': ''},
+                {'boat': 4,
                  'name': '信濃由行',
                  'racerid': 3620,
                  'rank': 6,
                  'time': ''}],
      'return': [],
      'stadium': 10,
      'start_information': {'course1': {'ST': 0.26, 'boat': 1},
@@ -1239,14 +1251,15 @@
         exacta_betting_dict: Dict[str, int],
         quinela_betting_dict: Dict[str, int],
         quinellaplace_betting_dict: Dict[str, int],
         win_betting_dict: Dict[str, int],
         placeshow_betting_dict: Dict[str, int],
       ) -> bool
       ```
+
     - ```python
       PyJPBoatrace().Bet.do(
         stadium:int,
         race:int,
         trifecta_betting_dict: Dict[str, int],
         trio_betting_dict: Dict[str, int],
         exacta_betting_dict: Dict[str, int],
@@ -1366,56 +1379,56 @@
 6. Create new Pull Request
 
 ### Setup the develop environment
 
 First, fork this repository and clone it to your local machine.
 
 ```bash
-$ git clone https://github.com/hmasdev/pyjpboatrace/
-$ cd pyjpboatrace
+git clone https://github.com/hmasdev/pyjpboatrace/
+cd pyjpboatrace
 ```
 
 Then, create a virtual environment for your development,
 and install the required libraries.
 
 ```bash
-$ python -m venv venv
-$ source venv/bin/activate  # for Linux or MacOS
-$ # venv\Scripts\activate  # for Windows
-$ pip install -e .[dev]
+python -m venv venv
+source venv/bin/activate  # for Linux or MacOS
+# venv\Scripts\activate  # for Windows
+pip install -e .[dev]
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv sync --dev
+pipenv sync --dev
 ```
 
 </details>
 
 ### Test
 
 <div id="HowToTestAnchor"></div>
 
 You can do unit tests and integration tests as follows:
 
 ```bash
-$ ./download_html_for_test.sh  # Only 1 time
-$ pytest -m "not integrate and not spending_money" # unit tests
-$ pytest # unit tests and integration tests
+./download_html_for_test.sh  # Only 1 time
+pytest -m "not integrate and not spending_money" # unit tests
+pytest # unit tests and integration tests
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ ./download_html_for_test.sh  # Only 1 time
-$ pipenv run pytest -m "not integrate and not spending_money" # unit tests
-$ pipenv run pytest  # unit tests and integration tests
+./download_html_for_test.sh  # Only 1 time
+pipenv run pytest -m "not integrate and not spending_money" # unit tests
+pipenv run pytest  # unit tests and integration tests
 ```
 
 </details>
 
 `pytest` does not test depositing, withdrawing or betting.
 If you want to test them, make `.secrets.json` at first:
 
@@ -1427,49 +1440,64 @@
   "vote_pass": "YOUR_BETTING_PASSWORD"
 }
 ```
 
 Then, run
 
 ```bash
-$ pytest -m "spending_money"
+pytest -m "spending_money"
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv run pytest -m "spending_money"
+pipenv run pytest -m "spending_money"
 ```
 
 </details>
 
 WARNING: Tests with `spending_money` spend 700 yen.
 
 ### Check the format of code and static types
 
 You should execute the following codes to check the format of code and static types:
 
 ```bash
-$ flake8 pyjpboatrace tests
-$ mypy pyjpboatrace tests
+flake8 pyjpboatrace tests
+mypy pyjpboatrace tests
 ```
 
 <details>
 <summary>[Deprecated] when using `pipenv`</summary>
 
 ```bash
-$ pipenv run flake8 pyjpboatrace
-$ pipenv run flake8 tests
-$ pipenv run mypy pyjpboatrace
-$ pipenv run mypy tests
+pipenv run flake8 pyjpboatrace
+pipenv run flake8 tests
+pipenv run mypy pyjpboatrace
+pipenv run mypy tests
 ```
 
 </details>
 
+### How to Update README.md
+
+To update the content of [README.md](./README.md), please do not edit the file directly.
+Instead, make your changes to [README.md.j2](./README.md.j2).
+
+After making updates to `README.md.j2`, execute the following command to regenerate `README.md`:
+
+```bash
+python update_readme.py > README.md
+```
+
+This process is necessary because README.md is dynamically generated from the README.md.j2 template.
+Direct modifications to README.md will be lost, as they are automatically overwritten by an automated process whenever the template is updated.
+
+Remember, to preserve your changes, always update README.md.j2 and not README.md directly.
 
 ## LICENSE
 
 [MIT](https://github.com/hmasdev/pyjpboatrace/tree/main/LICENSE)
 
 ## Authors
```

### Comparing `pyjpboatrace-0.3.0a4/pyjpboatrace.egg-info/SOURCES.txt` & `pyjpboatrace-0.3.1a0/pyjpboatrace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/pyproject.toml` & `pyjpboatrace-0.3.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 [project.urls]
 Repository = "http://github.com/hmasdev/pyjpboatrace"
 
 [project.optional-dependencies]
 dev = [
     "autopep8",
     "flake8>=3.8.4",
+    "Jinja2",
     "mypy>=0.812",
     "pytest>=6.1.2",
     "pytest-cov>=2.10.1",
     "pytz",
     "twine",
     "types-pytz",
     "wheel",
```

### Comparing `pyjpboatrace-0.3.0a4/tests/test_certification.py` & `pyjpboatrace-0.3.1a0/tests/test_certification.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/tests/test_drivers.py` & `pyjpboatrace-0.3.1a0/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/tests/test_pyjpboatrace.py` & `pyjpboatrace-0.3.1a0/tests/test_pyjpboatrace.py`

 * *Files identical despite different names*

### Comparing `pyjpboatrace-0.3.0a4/tests/test_validator.py` & `pyjpboatrace-0.3.1a0/tests/test_validator.py`

 * *Files identical despite different names*

