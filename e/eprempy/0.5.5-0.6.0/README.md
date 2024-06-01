# Comparing `tmp/eprempy-0.5.5.tar.gz` & `tmp/eprempy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eprempy-0.5.5.tar", max compression
+gzip compressed data, was "eprempy-0.6.0.tar", max compression
```

## Comparing `eprempy-0.5.5.tar` & `eprempy-0.6.0.tar`

### file list

```diff
@@ -1,178 +1,98 @@
--rwxr-xr-x   0        0        0     1513 2023-12-18 17:25:57.411106 eprempy-0.5.5/LICENSE
--rw-r--r--   0        0        0    10899 2024-03-27 21:41:55.392748 eprempy-0.5.5/README.md
--rw-r--r--   0        0        0      769 2024-05-29 14:54:01.233232 eprempy-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      298 2024-01-16 19:17:26.814570 eprempy-0.5.5/src/eprempy/__init__.py
--rw-r--r--   0        0        0     2513 2024-02-09 20:00:09.547665 eprempy-0.5.5/src/eprempy/__main__.py
--rw-r--r--   0        0        0     4067 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/_project_main.py
--rw-r--r--   0        0        0    38096 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/aliased.py
--rw-r--r--   0        0        0    10750 2024-02-01 21:56:36.730088 eprempy-0.5.5/src/eprempy/atomic.py
--rw-r--r--   0        0        0     3068 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/__init__.py
--rw-r--r--   0        0        0     4939 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/base/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    19155 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/base/__pycache__/_abcs.cpython-311.pyc
--rw-r--r--   0        0        0    17932 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/base/__pycache__/_protocols.cpython-311.pyc
--rw-r--r--   0        0        0     1217 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/base/__pycache__/_types.cpython-311.pyc
--rw-r--r--   0        0        0      576 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/base/__pycache__/abc.cpython-311.pyc
--rw-r--r--   0        0        0     5768 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/base/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0    11541 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/_abcs.py
--rw-r--r--   0        0        0     9699 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/_protocols.py
--rw-r--r--   0        0        0     1291 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/_types.py
--rw-r--r--   0        0        0      379 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/abc.py
--rw-r--r--   0        0        0     3558 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/mixins.py
--rw-r--r--   0        0        0     6643 2024-02-16 21:43:35.579405 eprempy-0.5.5/src/eprempy/cli.py
--rw-r--r--   0        0        0    37520 2024-02-19 22:23:32.972106 eprempy-0.5.5/src/eprempy/container.py
--rw-r--r--   0        0        0      872 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/datafile/__init__.py
--rw-r--r--   0        0        0     1306 2024-01-23 15:12:07.528662 eprempy-0.5.5/src/eprempy/datafile/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7386 2024-01-23 15:12:07.528662 eprempy-0.5.5/src/eprempy/datafile/__pycache__/_core.cpython-311.pyc
--rw-r--r--   0        0        0    22272 2024-02-01 22:21:06.982000 eprempy-0.5.5/src/eprempy/datafile/__pycache__/_interfaces.cpython-311.pyc
--rw-r--r--   0        0        0      472 2024-01-23 15:12:07.528662 eprempy-0.5.5/src/eprempy/datafile/__pycache__/_reference.cpython-311.pyc
--rw-r--r--   0        0        0    15878 2024-01-23 15:12:07.532662 eprempy-0.5.5/src/eprempy/datafile/__pycache__/_viewers.cpython-311.pyc
--rw-r--r--   0        0        0     3038 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/datafile/_core.py
--rw-r--r--   0        0        0    13619 2024-02-01 21:56:36.730088 eprempy-0.5.5/src/eprempy/datafile/_interfaces.py
--rw-r--r--   0        0        0      838 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/datafile/_reference.py
--rw-r--r--   0        0        0     8597 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/datafile/_viewers.py
--rw-r--r--   0        0        0    14024 2024-05-07 18:59:06.063479 eprempy-0.5.5/src/eprempy/eprem.py
--rw-r--r--   0        0        0    19560 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/etc.py
--rw-r--r--   0        0        0     6421 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/exceptions.py
--rw-r--r--   0        0        0     2535 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/interfaces.py
--rw-r--r--   0        0        0      452 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measurable/__init__.py
--rw-r--r--   0        0        0     1138 2023-12-18 17:27:18.215239 eprempy-0.5.5/src/eprempy/measurable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1649 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/measured/__init__.py
--rw-r--r--   0        0        0     3214 2024-01-23 15:12:06.724663 eprempy-0.5.5/src/eprempy/measured/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6881 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_context.cpython-311.pyc
--rw-r--r--   0        0        0     1828 2023-12-18 17:27:18.235239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_convert.cpython-311.pyc
--rw-r--r--   0        0        0     3866 2023-12-18 17:27:18.227239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_factories.cpython-311.pyc
--rw-r--r--   0        0        0     2022 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_object.cpython-311.pyc
--rw-r--r--   0        0        0     3798 2023-12-18 17:27:18.235239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_sequence.cpython-311.pyc
--rw-r--r--   0        0        0     5551 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_types.cpython-311.pyc
--rw-r--r--   0        0        0     1336 2023-12-18 17:27:18.235239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_units.cpython-311.pyc
--rw-r--r--   0        0        0     1966 2023-12-18 17:27:18.227239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_value.cpython-311.pyc
--rw-r--r--   0        0        0     3554 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_context.py
--rw-r--r--   0        0        0      843 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_convert.py
--rw-r--r--   0        0        0     1881 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_factories.py
--rw-r--r--   0        0        0      872 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_object.py
--rw-r--r--   0        0        0        0 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_operators.py
--rw-r--r--   0        0        0     2499 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_sequence.py
--rw-r--r--   0        0        0     2710 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_types.py
--rw-r--r--   0        0        0      530 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_units.py
--rw-r--r--   0        0        0      781 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_value.py
--rw-r--r--   0        0        0     4334 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/metric/__init__.py
--rw-r--r--   0        0        0     5988 2024-01-23 15:12:06.728663 eprempy-0.5.5/src/eprempy/metric/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    28262 2024-01-23 15:12:06.736663 eprempy-0.5.5/src/eprempy/metric/__pycache__/_conversions.cpython-311.pyc
--rw-r--r--   0        0        0    41607 2024-01-17 20:32:10.271816 eprempy-0.5.5/src/eprempy/metric/__pycache__/_defined.cpython-311.pyc
--rw-r--r--   0        0        0     6425 2023-12-18 17:27:18.187239 eprempy-0.5.5/src/eprempy/metric/__pycache__/_dimensions.cpython-311.pyc
--rw-r--r--   0        0        0     2176 2024-01-17 20:32:10.275816 eprempy-0.5.5/src/eprempy/metric/__pycache__/_exceptions.cpython-311.pyc
--rw-r--r--   0        0        0    15038 2024-02-01 22:21:06.218000 eprempy-0.5.5/src/eprempy/metric/__pycache__/_reference.cpython-311.pyc
--rw-r--r--   0        0        0    23126 2024-01-17 20:32:10.483817 eprempy-0.5.5/src/eprempy/metric/__pycache__/_systems.cpython-311.pyc
--rw-r--r--   0        0        0     2358 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/metric/__pycache__/_types.cpython-311.pyc
--rw-r--r--   0        0        0    25561 2024-01-17 20:32:10.495817 eprempy-0.5.5/src/eprempy/metric/__pycache__/_units.cpython-311.pyc
--rw-r--r--   0        0        0    19397 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/metric/_conversions.py
--rw-r--r--   0        0        0    26244 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/metric/_defined.py
--rw-r--r--   0        0        0     3013 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/metric/_dimensions.py
--rw-r--r--   0        0        0      804 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/metric/_exceptions.py
--rw-r--r--   0        0        0    20947 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/metric/_reference.py
--rw-r--r--   0        0        0    13685 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/metric/_systems.py
--rw-r--r--   0        0        0     1011 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/metric/_types.py
--rw-r--r--   0        0        0    20543 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/metric/_units.py
--rw-r--r--   0        0        0     1893 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/numeric/__init__.py
--rw-r--r--   0        0        0     3045 2024-01-23 15:12:06.896663 eprempy-0.5.5/src/eprempy/numeric/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    45019 2024-02-01 22:21:06.398000 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_array.cpython-311.pyc
--rw-r--r--   0        0        0     6502 2023-12-18 17:27:18.199239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_data.cpython-311.pyc
--rw-r--r--   0        0        0     4973 2023-12-18 17:27:18.223239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_factory.cpython-311.pyc
--rw-r--r--   0        0        0     4242 2023-12-18 17:27:18.203239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_implementation.cpython-311.pyc
--rw-r--r--   0        0        0    39216 2024-02-01 22:21:06.390000 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_index.cpython-311.pyc
--rw-r--r--   0        0        0    20506 2023-12-18 17:27:18.215239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_mixins.cpython-311.pyc
--rw-r--r--   0        0        0    12801 2023-12-18 17:27:18.199239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_objects.cpython-311.pyc
--rw-r--r--   0        0        0    16208 2024-01-17 20:32:10.503817 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_operations.cpython-311.pyc
--rw-r--r--   0        0        0     8024 2023-12-18 17:27:18.203239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_operators.cpython-311.pyc
--rw-r--r--   0        0        0    27098 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/numeric/_array.py
--rw-r--r--   0        0        0     3999 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_data.py
--rw-r--r--   0        0        0     2944 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_factory.py
--rw-r--r--   0        0        0     2105 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_implementation.py
--rw-r--r--   0        0        0    22263 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/numeric/_index.py
--rw-r--r--   0        0        0    16116 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_mixins.py
--rw-r--r--   0        0        0     7169 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_objects.py
--rw-r--r--   0        0        0    12011 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/numeric/_operations.py
--rw-r--r--   0        0        0     4363 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_operators.py
--rw-r--r--   0        0        0      637 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/observable/__init__.py
--rw-r--r--   0        0        0     1235 2023-12-18 17:27:18.547240 eprempy-0.5.5/src/eprempy/observable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    89743 2024-02-01 22:22:10.929996 eprempy-0.5.5/src/eprempy/observable/__pycache__/_interfaces.cpython-311.pyc
--rw-r--r--   0        0        0    31847 2024-02-01 22:21:06.722000 eprempy-0.5.5/src/eprempy/observable/__pycache__/_objects.cpython-311.pyc
--rw-r--r--   0        0        0    66067 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/observable/_interfaces.py
--rw-r--r--   0        0        0    20418 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/observable/_objects.py
--rw-r--r--   0        0        0     5829 2024-02-16 16:58:53.068415 eprempy-0.5.5/src/eprempy/parameter/__init__.py
--rw-r--r--   0        0        0     7713 2024-02-16 17:07:35.148203 eprempy-0.5.5/src/eprempy/parameter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    22264 2024-02-16 17:07:35.148203 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_config.cpython-311.pyc
--rw-r--r--   0        0        0      174 2024-02-09 16:09:39.704090 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_interface.cpython-311.pyc
--rw-r--r--   0        0        0    10077 2024-05-24 16:41:42.827676 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_metadata.cpython-311.pyc
--rw-r--r--   0        0        0     9967 2024-01-26 15:55:06.544039 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_reference.cpython-311.pyc
--rw-r--r--   0        0        0    14379 2024-02-16 21:45:52.775370 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_runtime.cpython-311.pyc
--rw-r--r--   0        0        0    28158 2024-02-16 21:45:52.743369 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_src.cpython-311.pyc
--rw-r--r--   0        0        0    13524 2024-02-09 16:09:08.524083 eprempy-0.5.5/src/eprempy/parameter/__pycache__/default.cpython-311.pyc
--rw-r--r--   0        0        0    13439 2024-03-27 19:39:17.007480 eprempy-0.5.5/src/eprempy/parameter/__pycache__/reference.cpython-311.pyc
--rw-r--r--   0        0        0    13237 2024-02-16 16:58:53.068415 eprempy-0.5.5/src/eprempy/parameter/_config.py
--rw-r--r--   0        0        0    12922 2024-03-27 21:35:17.659905 eprempy-0.5.5/src/eprempy/parameter/_metadata.py
--rw-r--r--   0        0        0     7762 2024-02-16 21:43:35.579405 eprempy-0.5.5/src/eprempy/parameter/_runtime.py
--rw-r--r--   0        0        0    15954 2024-02-16 21:43:35.579405 eprempy-0.5.5/src/eprempy/parameter/_src.py
--rw-r--r--   0        0        0    20943 2024-03-27 19:22:59.867663 eprempy-0.5.5/src/eprempy/parameter/reference.json
--rw-r--r--   0        0        0    27683 2024-03-27 19:25:57.511816 eprempy-0.5.5/src/eprempy/parameter/reference.py
--rw-r--r--   0        0        0      447 2024-03-27 19:22:59.875663 eprempy-0.5.5/src/eprempy/parameter/sources.log
--rw-r--r--   0        0        0     7210 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/paths.py
--rw-r--r--   0        0        0    18010 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/physical/__init__.py
--rw-r--r--   0        0        0    23629 2024-01-23 15:12:06.724663 eprempy-0.5.5/src/eprempy/physical/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12627 2024-02-01 22:21:06.414000 eprempy-0.5.5/src/eprempy/physical/__pycache__/_array.cpython-311.pyc
--rw-r--r--   0        0        0    26899 2024-01-17 20:32:10.583817 eprempy-0.5.5/src/eprempy/physical/__pycache__/_axes.cpython-311.pyc
--rw-r--r--   0        0        0    20617 2024-05-24 17:02:27.395843 eprempy-0.5.5/src/eprempy/physical/__pycache__/_axis.cpython-311.pyc
--rw-r--r--   0        0        0     4355 2023-12-18 17:27:18.531240 eprempy-0.5.5/src/eprempy/physical/__pycache__/_axis_factories.cpython-311.pyc
--rw-r--r--   0        0        0      552 2024-01-17 20:32:10.587817 eprempy-0.5.5/src/eprempy/physical/__pycache__/_exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     8714 2023-12-18 17:27:18.239239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_object.cpython-311.pyc
--rw-r--r--   0        0        0     9947 2023-12-18 17:27:18.247239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_object_factories.cpython-311.pyc
--rw-r--r--   0        0        0    42022 2024-02-01 22:21:06.706000 eprempy-0.5.5/src/eprempy/physical/__pycache__/_operations.cpython-311.pyc
--rw-r--r--   0        0        0     5448 2024-01-17 20:32:10.587817 eprempy-0.5.5/src/eprempy/physical/__pycache__/_scalar.cpython-311.pyc
--rw-r--r--   0        0        0     4504 2023-12-18 17:27:18.251239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_tensor.cpython-311.pyc
--rw-r--r--   0        0        0     3431 2023-12-18 17:27:18.243239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_types.cpython-311.pyc
--rw-r--r--   0        0        0     4116 2023-12-18 17:27:18.251239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_vector.cpython-311.pyc
--rw-r--r--   0        0        0     6544 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/physical/_array.py
--rw-r--r--   0        0        0    17721 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/physical/_axes.py
--rw-r--r--   0        0        0    13647 2024-05-24 17:02:24.651820 eprempy-0.5.5/src/eprempy/physical/_axis.py
--rw-r--r--   0        0        0     2249 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_axis_factories.py
--rw-r--r--   0        0        0      150 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/physical/_exceptions.py
--rw-r--r--   0        0        0     4163 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_object.py
--rw-r--r--   0        0        0     5868 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_object_factories.py
--rw-r--r--   0        0        0    21876 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/physical/_operations.py
--rw-r--r--   0        0        0     2658 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/physical/_scalar.py
--rw-r--r--   0        0        0     2030 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_tensor.py
--rw-r--r--   0        0        0     1689 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_types.py
--rw-r--r--   0        0        0     1696 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_vector.py
--rw-r--r--   0        0        0    40811 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/project.py
--rw-r--r--   0        0        0     4789 2024-05-24 16:51:09.576354 eprempy-0.5.5/src/eprempy/quantity/__init__.py
--rw-r--r--   0        0        0     6632 2024-05-24 16:53:00.804523 eprempy-0.5.5/src/eprempy/quantity/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1303 2024-01-17 20:32:10.571817 eprempy-0.5.5/src/eprempy/quantity/__pycache__/_exceptions.cpython-311.pyc
--rw-r--r--   0        0        0    17103 2024-05-24 16:53:00.804523 eprempy-0.5.5/src/eprempy/quantity/__pycache__/_functions.cpython-311.pyc
--rw-r--r--   0        0        0     4164 2023-12-18 17:27:18.239239 eprempy-0.5.5/src/eprempy/quantity/__pycache__/_measurement.cpython-311.pyc
--rw-r--r--   0        0        0      400 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/quantity/_exceptions.py
--rw-r--r--   0        0        0     9972 2024-05-24 16:50:50.316326 eprempy-0.5.5/src/eprempy/quantity/_functions.py
--rw-r--r--   0        0        0     2093 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/quantity/_measurement.py
--rw-r--r--   0        0        0     3790 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/real/__init__.py
--rw-r--r--   0        0        0     8573 2024-01-23 15:12:06.912663 eprempy-0.5.5/src/eprempy/real/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    23275 2024-01-23 15:12:06.916663 eprempy-0.5.5/src/eprempy/real/__pycache__/_array.cpython-311.pyc
--rw-r--r--   0        0        0    10049 2023-12-18 17:27:18.227239 eprempy-0.5.5/src/eprempy/real/__pycache__/_objects.cpython-311.pyc
--rw-r--r--   0        0        0      745 2023-12-18 17:27:18.227239 eprempy-0.5.5/src/eprempy/real/__pycache__/_types.cpython-311.pyc
--rw-r--r--   0        0        0    11506 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/real/_array.py
--rw-r--r--   0        0        0     4891 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/real/_objects.py
--rw-r--r--   0        0        0      707 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/real/_types.py
--rw-r--r--   0        0        0     5785 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/reference.py
--rw-r--r--   0        0        0     1756 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/symbolic/__init__.py
--rw-r--r--   0        0        0     3097 2024-01-17 20:32:10.255816 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    21446 2023-12-18 17:27:17.999239 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_expression.cpython-311.pyc
--rw-r--r--   0        0        0    42853 2024-01-24 19:12:48.936383 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_operand.cpython-311.pyc
--rw-r--r--   0        0        0     3246 2023-12-18 17:27:18.015239 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_operator.cpython-311.pyc
--rw-r--r--   0        0        0    13036 2024-01-17 20:32:10.267816 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_parser.cpython-311.pyc
--rw-r--r--   0        0        0     6480 2023-12-18 17:27:18.011239 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_part.cpython-311.pyc
--rw-r--r--   0        0        0    13984 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/symbolic/_expression.py
--rw-r--r--   0        0        0    31307 2024-01-24 16:54:00.366890 eprempy-0.5.5/src/eprempy/symbolic/_operand.py
--rw-r--r--   0        0        0     1689 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/symbolic/_operator.py
--rw-r--r--   0        0        0     8534 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/symbolic/_parser.py
--rw-r--r--   0        0        0     3018 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/symbolic/_part.py
--rw-r--r--   0        0        0      647 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/typehelp.py
--rw-r--r--   0        0        0     9023 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/universal.py
--rw-r--r--   0        0        0    11598 1970-01-01 00:00:00.000000 eprempy-0.5.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1513 2023-12-18 17:25:57.411106 eprempy-0.6.0/LICENSE
+-rw-r--r--   0        0        0    10899 2024-03-27 21:41:55.392748 eprempy-0.6.0/README.md
+-rw-r--r--   0        0        0      769 2024-06-01 04:03:07.605194 eprempy-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      298 2024-01-16 19:17:26.814570 eprempy-0.6.0/src/eprempy/__init__.py
+-rw-r--r--   0        0        0     2513 2024-02-09 20:00:09.547665 eprempy-0.6.0/src/eprempy/__main__.py
+-rw-r--r--   0        0        0     4067 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/_project_main.py
+-rw-r--r--   0        0        0    38096 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/aliased.py
+-rw-r--r--   0        0        0    10750 2024-02-01 21:56:36.730088 eprempy-0.6.0/src/eprempy/atomic.py
+-rw-r--r--   0        0        0     3068 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/base/__init__.py
+-rw-r--r--   0        0        0    11541 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/base/_abcs.py
+-rw-r--r--   0        0        0     9699 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/base/_protocols.py
+-rw-r--r--   0        0        0     1291 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/base/_types.py
+-rw-r--r--   0        0        0      379 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/base/abc.py
+-rw-r--r--   0        0        0     3558 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/base/mixins.py
+-rw-r--r--   0        0        0     6643 2024-02-16 21:43:35.579405 eprempy-0.6.0/src/eprempy/cli.py
+-rw-r--r--   0        0        0    37520 2024-02-19 22:23:32.972106 eprempy-0.6.0/src/eprempy/container.py
+-rw-r--r--   0        0        0      872 2024-01-22 22:28:21.800484 eprempy-0.6.0/src/eprempy/datafile/__init__.py
+-rw-r--r--   0        0        0     3038 2024-01-22 22:28:21.800484 eprempy-0.6.0/src/eprempy/datafile/_core.py
+-rw-r--r--   0        0        0    13619 2024-02-01 21:56:36.730088 eprempy-0.6.0/src/eprempy/datafile/_interfaces.py
+-rw-r--r--   0        0        0      838 2024-01-22 22:28:21.800484 eprempy-0.6.0/src/eprempy/datafile/_reference.py
+-rw-r--r--   0        0        0     8597 2024-01-22 22:28:21.800484 eprempy-0.6.0/src/eprempy/datafile/_viewers.py
+-rw-r--r--   0        0        0    14097 2024-05-30 19:22:59.419142 eprempy-0.6.0/src/eprempy/eprem.py
+-rw-r--r--   0        0        0    19560 2024-01-17 20:28:37.607261 eprempy-0.6.0/src/eprempy/etc.py
+-rw-r--r--   0        0        0     6421 2024-01-17 20:28:37.607261 eprempy-0.6.0/src/eprempy/exceptions.py
+-rw-r--r--   0        0        0     2535 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/interfaces.py
+-rw-r--r--   0        0        0      452 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measurable/__init__.py
+-rw-r--r--   0        0        0     1649 2024-01-22 22:28:21.800484 eprempy-0.6.0/src/eprempy/measured/__init__.py
+-rw-r--r--   0        0        0     3554 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_context.py
+-rw-r--r--   0        0        0      843 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_convert.py
+-rw-r--r--   0        0        0     1881 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_factories.py
+-rw-r--r--   0        0        0      872 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_object.py
+-rw-r--r--   0        0        0        0 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_operators.py
+-rw-r--r--   0        0        0     2499 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_sequence.py
+-rw-r--r--   0        0        0     2710 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_types.py
+-rw-r--r--   0        0        0      530 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_units.py
+-rw-r--r--   0        0        0      781 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/measured/_value.py
+-rw-r--r--   0        0        0     4334 2024-01-22 22:28:21.800484 eprempy-0.6.0/src/eprempy/metric/__init__.py
+-rw-r--r--   0        0        0    19397 2024-01-22 22:28:21.804484 eprempy-0.6.0/src/eprempy/metric/_conversions.py
+-rw-r--r--   0        0        0    26244 2024-01-17 20:28:37.607261 eprempy-0.6.0/src/eprempy/metric/_defined.py
+-rw-r--r--   0        0        0     3013 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/metric/_dimensions.py
+-rw-r--r--   0        0        0      804 2024-01-17 20:28:37.607261 eprempy-0.6.0/src/eprempy/metric/_exceptions.py
+-rw-r--r--   0        0        0    20947 2024-02-01 21:56:36.734088 eprempy-0.6.0/src/eprempy/metric/_reference.py
+-rw-r--r--   0        0        0    13685 2024-01-17 20:28:37.607261 eprempy-0.6.0/src/eprempy/metric/_systems.py
+-rw-r--r--   0        0        0     1011 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/metric/_types.py
+-rw-r--r--   0        0        0    20543 2024-01-17 20:28:37.607261 eprempy-0.6.0/src/eprempy/metric/_units.py
+-rw-r--r--   0        0        0     1893 2024-01-22 22:28:21.804484 eprempy-0.6.0/src/eprempy/numeric/__init__.py
+-rw-r--r--   0        0        0    27098 2024-02-01 21:56:36.734088 eprempy-0.6.0/src/eprempy/numeric/_array.py
+-rw-r--r--   0        0        0     3999 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/numeric/_data.py
+-rw-r--r--   0        0        0     2944 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/numeric/_factory.py
+-rw-r--r--   0        0        0     2105 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/numeric/_implementation.py
+-rw-r--r--   0        0        0    22263 2024-02-01 21:56:36.734088 eprempy-0.6.0/src/eprempy/numeric/_index.py
+-rw-r--r--   0        0        0    16116 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/numeric/_mixins.py
+-rw-r--r--   0        0        0     7169 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/numeric/_objects.py
+-rw-r--r--   0        0        0    12011 2024-01-17 20:28:37.607261 eprempy-0.6.0/src/eprempy/numeric/_operations.py
+-rw-r--r--   0        0        0     4363 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/numeric/_operators.py
+-rw-r--r--   0        0        0      637 2023-12-18 17:25:57.415106 eprempy-0.6.0/src/eprempy/observable/__init__.py
+-rw-r--r--   0        0        0    66067 2024-02-01 21:56:36.734088 eprempy-0.6.0/src/eprempy/observable/_interfaces.py
+-rw-r--r--   0        0        0    20418 2024-02-01 21:56:36.734088 eprempy-0.6.0/src/eprempy/observable/_objects.py
+-rw-r--r--   0        0        0     5829 2024-02-16 16:58:53.068415 eprempy-0.6.0/src/eprempy/parameter/__init__.py
+-rw-r--r--   0        0        0    13237 2024-02-16 16:58:53.068415 eprempy-0.6.0/src/eprempy/parameter/_config.py
+-rw-r--r--   0        0        0    12922 2024-03-27 21:35:17.659905 eprempy-0.6.0/src/eprempy/parameter/_metadata.py
+-rw-r--r--   0        0        0     7762 2024-02-16 21:43:35.579405 eprempy-0.6.0/src/eprempy/parameter/_runtime.py
+-rw-r--r--   0        0        0    15954 2024-02-16 21:43:35.579405 eprempy-0.6.0/src/eprempy/parameter/_src.py
+-rw-r--r--   0        0        0    20943 2024-03-27 19:22:59.867663 eprempy-0.6.0/src/eprempy/parameter/reference.json
+-rw-r--r--   0        0        0    27683 2024-03-27 19:25:57.511816 eprempy-0.6.0/src/eprempy/parameter/reference.py
+-rw-r--r--   0        0        0     7210 2024-01-17 20:28:37.607261 eprempy-0.6.0/src/eprempy/paths.py
+-rw-r--r--   0        0        0    18010 2024-01-22 22:28:21.804484 eprempy-0.6.0/src/eprempy/physical/__init__.py
+-rw-r--r--   0        0        0     6544 2024-02-01 21:56:36.734088 eprempy-0.6.0/src/eprempy/physical/_array.py
+-rw-r--r--   0        0        0    17721 2024-01-17 20:28:37.611261 eprempy-0.6.0/src/eprempy/physical/_axes.py
+-rw-r--r--   0        0        0    13647 2024-05-24 17:02:24.651820 eprempy-0.6.0/src/eprempy/physical/_axis.py
+-rw-r--r--   0        0        0     2249 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/physical/_axis_factories.py
+-rw-r--r--   0        0        0      150 2024-01-17 20:28:37.611261 eprempy-0.6.0/src/eprempy/physical/_exceptions.py
+-rw-r--r--   0        0        0     4163 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/physical/_object.py
+-rw-r--r--   0        0        0     5868 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/physical/_object_factories.py
+-rw-r--r--   0        0        0    21876 2024-02-01 21:56:36.734088 eprempy-0.6.0/src/eprempy/physical/_operations.py
+-rw-r--r--   0        0        0     2658 2024-01-17 20:28:37.611261 eprempy-0.6.0/src/eprempy/physical/_scalar.py
+-rw-r--r--   0        0        0     2030 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/physical/_tensor.py
+-rw-r--r--   0        0        0     1689 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/physical/_types.py
+-rw-r--r--   0        0        0     1696 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/physical/_vector.py
+-rw-r--r--   0        0        0    40811 2024-01-17 20:28:37.611261 eprempy-0.6.0/src/eprempy/project.py
+-rw-r--r--   0        0        0     4789 2024-05-24 16:51:09.576354 eprempy-0.6.0/src/eprempy/quantity/__init__.py
+-rw-r--r--   0        0        0      400 2024-01-17 20:28:37.611261 eprempy-0.6.0/src/eprempy/quantity/_exceptions.py
+-rw-r--r--   0        0        0     9972 2024-05-24 16:50:50.316326 eprempy-0.6.0/src/eprempy/quantity/_functions.py
+-rw-r--r--   0        0        0     2093 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/quantity/_measurement.py
+-rw-r--r--   0        0        0     3790 2024-01-22 22:28:21.804484 eprempy-0.6.0/src/eprempy/real/__init__.py
+-rw-r--r--   0        0        0    11506 2024-01-22 22:28:21.804484 eprempy-0.6.0/src/eprempy/real/_array.py
+-rw-r--r--   0        0        0     4891 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/real/_objects.py
+-rw-r--r--   0        0        0      707 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/real/_types.py
+-rw-r--r--   0        0        0     5785 2024-01-22 22:28:21.804484 eprempy-0.6.0/src/eprempy/reference.py
+-rw-r--r--   0        0        0     1756 2024-01-17 20:28:37.611261 eprempy-0.6.0/src/eprempy/symbolic/__init__.py
+-rw-r--r--   0        0        0    13984 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/symbolic/_expression.py
+-rw-r--r--   0        0        0    31307 2024-01-24 16:54:00.366890 eprempy-0.6.0/src/eprempy/symbolic/_operand.py
+-rw-r--r--   0        0        0     1689 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/symbolic/_operator.py
+-rw-r--r--   0        0        0     8534 2024-01-17 20:28:37.611261 eprempy-0.6.0/src/eprempy/symbolic/_parser.py
+-rw-r--r--   0        0        0     3018 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/symbolic/_part.py
+-rw-r--r--   0        0        0      647 2023-12-18 17:25:57.419106 eprempy-0.6.0/src/eprempy/typehelp.py
+-rw-r--r--   0        0        0     9023 2024-02-01 21:56:36.734088 eprempy-0.6.0/src/eprempy/universal.py
+-rw-r--r--   0        0        0    11598 1970-01-01 00:00:00.000000 eprempy-0.6.0/PKG-INFO
```

### Comparing `eprempy-0.5.5/LICENSE` & `eprempy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/README.md` & `eprempy-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/pyproject.toml` & `eprempy-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eprempy"
-version = "0.5.5"
+version = "0.6.0"
 description = "Tools for working with EPREM simulation runs"
 authors = ["Matt Young"]
 license = "BSD 3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `eprempy-0.5.5/src/eprempy/__main__.py` & `eprempy-0.6.0/src/eprempy/__main__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/_project_main.py` & `eprempy-0.6.0/src/eprempy/_project_main.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/aliased.py` & `eprempy-0.6.0/src/eprempy/aliased.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/atomic.py` & `eprempy-0.6.0/src/eprempy/atomic.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/base/__init__.py` & `eprempy-0.6.0/src/eprempy/base/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/base/_abcs.py` & `eprempy-0.6.0/src/eprempy/base/_abcs.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/base/_protocols.py` & `eprempy-0.6.0/src/eprempy/base/_protocols.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/base/_types.py` & `eprempy-0.6.0/src/eprempy/base/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/base/mixins.py` & `eprempy-0.6.0/src/eprempy/base/mixins.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/cli.py` & `eprempy-0.6.0/src/eprempy/cli.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/container.py` & `eprempy-0.6.0/src/eprempy/container.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/datafile/__init__.py` & `eprempy-0.6.0/src/eprempy/datafile/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/datafile/_core.py` & `eprempy-0.6.0/src/eprempy/datafile/_core.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/datafile/_interfaces.py` & `eprempy-0.6.0/src/eprempy/datafile/_interfaces.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/datafile/_reference.py` & `eprempy-0.6.0/src/eprempy/datafile/_reference.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/datafile/_viewers.py` & `eprempy-0.6.0/src/eprempy/datafile/_viewers.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/eprem.py` & `eprempy-0.6.0/src/eprempy/eprem.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,22 +139,24 @@
 ObserverType = typing.TypeVar('ObserverType', bound=Observer)
 
 
 @etc.autostr
 class Stream(Observer):
     """An EPREM stream observer."""
 
+    prefixes = {'stream', 'obs', 'flux'}
+
     @classmethod
     def patterns(cls, __id: int) -> typing.List[str]:
         """Generate stream-observer filename patterns for the given ID."""
         if not isinstance(__id, int):
             raise TypeError(
                 f"Cannot create stream observer from ID type {type(__id)}"
             ) from None
-        return [f'{prefix}{__id:06}.*' for prefix in {'obs', 'flux'}]
+        return [f'{prefix}{__id:06}.*' for prefix in cls.prefixes]
 
     def __init__(
         self,
         dataview: datafile.View,
         observables: observable.Quantities,
     ) -> None:
         super().__init__(dataview, observables)
@@ -168,24 +170,26 @@
         return self._shells
 
 
 @etc.autostr
 class Point(Observer):
     """An EPREM point observer."""
 
+    prefixes = {'point', 'p_obs'}
+
     @classmethod
     def patterns(cls, __id: typing.Union[str, int]) -> typing.List[str]:
         """Generate point-observer filename patterns for the given ID."""
         patterns = []
         if not isinstance(__id, (int, str)):
             raise TypeError(
                 f"Cannot create point observer from ID type {type(__id)}"
             ) from None
         with contextlib.suppress(ValueError):
-            patterns.append(f'p_obs{int(__id):03}.*')
+            patterns = [f'{prefix}{int(__id):03}.*' for prefix in cls.prefixes]
         if isinstance(__id, str):
             patterns.append(f'{__id}.*')
         return patterns
 
     def __init__(
         self,
         dataview: datafile.View,
@@ -336,35 +340,33 @@
             self._observers = {**self.streams, **self.points}
         return self._observers
 
     @property
     def streams(self):
         """A mapping of available stream-observer interfaces."""
         if self._streams is None:
-            prefixes = {'obs', 'flux'}
             obspaths = [
                 path
-                for prefix in prefixes
+                for prefix in Stream.prefixes
                 for path in self.directory.glob(f"{prefix}*")
                 if path.suffix in datafile.VIEWERS
             ]
             self._streams = {
                 _get_observer_id(path): self._new_observer(path, Stream)
                 for path in obspaths
             }
         return self._streams
 
     @property
     def points(self):
         """A mapping of available point-observer interfaces."""
         if self._points is None:
-            prefixes = {'p_obs'}
             obspaths = [
                 path
-                for prefix in prefixes
+                for prefix in Point.prefixes
                 for path in self.directory.glob(f"{prefix}*")
                 if path.suffix in datafile.VIEWERS
             ]
             self._points = {
                 _get_observer_id(path): self._new_observer(path, Point)
                 for path in obspaths
             }
@@ -404,18 +406,19 @@
         """This observer's metric system."""
         return self._system
 
 
 def _get_observer_id(path: pathlib.Path):
     """Compute the appropriate observer ID for the given path."""
     stem = path.stem
-    for prefix in ('obs', 'flux', 'p_obs'):
+    prefixes = Stream.prefixes | Point.prefixes
+    for prefix in prefixes:
         if stem.startswith(prefix):
             key = stem.lstrip(prefix)
-            if prefix in {'obs', 'flux'}:
+            if prefix in Stream.prefixes:
                 return int(key)
             return key
     raise ValueError(path)
 
 
 def dataset(
     source: paths.PathLike=None,
```

### Comparing `eprempy-0.5.5/src/eprempy/etc.py` & `eprempy-0.6.0/src/eprempy/etc.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/exceptions.py` & `eprempy-0.6.0/src/eprempy/exceptions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/interfaces.py` & `eprempy-0.6.0/src/eprempy/interfaces.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/__init__.py` & `eprempy-0.6.0/src/eprempy/measured/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/_context.py` & `eprempy-0.6.0/src/eprempy/measured/_context.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/_convert.py` & `eprempy-0.6.0/src/eprempy/measured/_convert.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/_factories.py` & `eprempy-0.6.0/src/eprempy/measured/_factories.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/_object.py` & `eprempy-0.6.0/src/eprempy/measured/_object.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/_sequence.py` & `eprempy-0.6.0/src/eprempy/measured/_sequence.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/_types.py` & `eprempy-0.6.0/src/eprempy/measured/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/_units.py` & `eprempy-0.6.0/src/eprempy/measured/_units.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/measured/_value.py` & `eprempy-0.6.0/src/eprempy/measured/_value.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/__init__.py` & `eprempy-0.6.0/src/eprempy/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/_conversions.py` & `eprempy-0.6.0/src/eprempy/metric/_conversions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/_defined.py` & `eprempy-0.6.0/src/eprempy/metric/_defined.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/_dimensions.py` & `eprempy-0.6.0/src/eprempy/metric/_dimensions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/_exceptions.py` & `eprempy-0.6.0/src/eprempy/metric/_exceptions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/_reference.py` & `eprempy-0.6.0/src/eprempy/metric/_reference.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/_systems.py` & `eprempy-0.6.0/src/eprempy/metric/_systems.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/_types.py` & `eprempy-0.6.0/src/eprempy/metric/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/metric/_units.py` & `eprempy-0.6.0/src/eprempy/metric/_units.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/__init__.py` & `eprempy-0.6.0/src/eprempy/numeric/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/__pycache__/_mixins.cpython-311.pyc` & `eprempy-0.6.0/src/eprempy/numeric/_mixins.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1282 +1,1008 @@
-00000000: a70d 0d0a 0000 0000 a580 8065 f43e 0000  ...........e.>..
-00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 b200 0000 9700 6400 6401  ............d.d.
-00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
-00000040: 6c02 5a02 6400 6401 6c03 5a02 6402 6403  l.Z.d.d.l.Z.d.d.
-00000050: 6c04 6d05 5a05 0100 6402 6404 6c06 6d07  l.m.Z...d.d.l.m.
-00000060: 5a07 0100 0200 6501 6a08 0000 0000 0000  Z.....e.j.......
-00000070: 0000 6405 a601 0000 ab01 0000 0000 0000  ..d.............
-00000080: 0000 5a09 6501 6a0a 0000 0000 0000 0000  ..Z.e.j.........
-00000090: 6406 6509 6602 1900 0000 0000 0000 0000  d.e.f...........
-000000a0: 5a0b 0200 4700 6407 8400 6408 a602 0000  Z...G.d...d.....
-000000b0: ab02 0000 0000 0000 0000 5a0c 0200 4700  ..........Z...G.
-000000c0: 6409 8400 640a 650c a603 0000 ab03 0000  d...d.e.........
-000000d0: 0000 0000 0000 5a0d 6401 5300 290b e900  ......Z.d.S.)...
-000000e0: 0000 004e e901 0000 0029 01da 0b5f 6f70  ...N.....)..._op
-000000f0: 6572 6174 696f 6e73 2901 da06 4f62 6a65  erations)...Obje
-00000100: 6374 da01 542e 6300 0000 0000 0000 0000  ct..T.c.........
-00000110: 0000 0004 0000 0000 0000 00f3 4801 0000  ............H...
-00000120: 9700 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000130: 6504 6a05 0000 0000 0000 0000 6506 6a07  e.j.........e.j.
-00000140: 0000 0000 0000 0000 6508 6509 6704 5a0a  ........e.e.g.Z.
-00000150: 6402 8400 5a0b 6403 8400 5a0c 6504 6a05  d...Z.d...Z.e.j.
-00000160: 0000 0000 0000 0000 6509 6702 0200 6508  ........e.g...e.
-00000170: 6504 6a0d 0000 0000 0000 0000 a601 0000  e.j.............
-00000180: ab01 0000 0000 0000 0000 7a00 0000 5a0e  ..........z...Z.
-00000190: 6404 8400 5a0f 6405 8400 5a10 6406 6511  d...Z.d...Z.d.e.
-000001a0: 6a12 0000 0000 0000 0000 6504 6a11 0000  j.........e.j...
-000001b0: 0000 0000 0000 6a13 0000 0000 0000 0000  ......j.........
-000001c0: 1900 0000 0000 0000 0000 6602 6407 8404  ..........f.d...
-000001d0: 5a14 6408 8400 5a15 6409 8400 5a16 640a  Z.d...Z.d...Z.d.
-000001e0: 8400 5a17 6518 640b 6511 6a19 0000 0000  ..Z.e.d.e.j.....
-000001f0: 0000 0000 6602 640c 8404 a600 0000 ab00  ....f.d.........
-00000200: 0000 0000 0000 0000 5a1a 640d 5a1b 6511  ........Z.d.Z.e.
-00000210: 6a1c 0000 0000 0000 0000 651d 6511 6a19  j.........e.e.j.
-00000220: 0000 0000 0000 0000 6602 1900 0000 0000  ........f.......
-00000230: 0000 0000 651e 640e 3c00 0000 0900 6518  ....e.d.<.....e.
-00000240: 640f 6511 6a19 0000 0000 0000 0000 6602  d.e.j.........f.
-00000250: 6410 8404 a600 0000 ab00 0000 0000 0000  d...............
-00000260: 0000 5a1f 640d 5300 2911 da09 4675 6e63  ..Z.d.S.)...Func
-00000270: 7469 6f6e 7361 2606 0000 4d69 7869 6e20  tionsa&...Mixin 
-00000280: 666f 7220 6164 6469 6e67 2073 7570 706f  for adding suppo
-00000290: 7274 2066 6f72 2060 6e75 6d70 7960 2066  rt for `numpy` f
-000002a0: 756e 6374 696f 6e73 2074 6f20 6e75 6d65  unctions to nume
-000002b0: 7269 6320 6f62 6a65 6374 732e 0a20 2020  ric objects..   
-000002c0: 200a 2020 2020 436c 6173 7365 7320 7468   .    Classes th
-000002d0: 6174 2069 6e68 6572 6974 2066 726f 6d20  at inherit from 
-000002e0: 7468 6973 2063 6c61 7373 206d 6179 2069  this class may i
-000002f0: 6d70 6c65 6d65 6e74 2073 7570 706f 7274  mplement support
-00000300: 2066 6f72 2060 6e75 6d70 7960 0a20 2020   for `numpy`.   
-00000310: 2075 6e69 7665 7273 616c 2066 756e 6374   universal funct
-00000320: 696f 6e73 2028 2275 6675 6e63 7322 3b20  ions ("ufuncs"; 
-00000330: 652e 672e 2c20 606e 756d 7079 2e73 7172  e.g., `numpy.sqr
-00000340: 7460 2920 6279 206f 7665 726c 6f61 6469  t`) by overloadi
-00000350: 6e67 0a20 2020 2060 5f61 7070 6c79 5f75  ng.    `_apply_u
-00000360: 6675 6e63 602c 2061 6e64 206d 6179 2069  func`, and may i
-00000370: 6d70 6c65 6d65 6e74 2073 7570 706f 7274  mplement support
-00000380: 2066 6f72 2060 6e75 6d70 7960 2070 7562   for `numpy` pub
-00000390: 6c69 6320 6675 6e63 7469 6f6e 730a 2020  lic functions.  
-000003a0: 2020 2865 2e67 2e2c 2060 6e75 6d70 792e    (e.g., `numpy.
-000003b0: 7371 7565 657a 6560 2920 6279 206f 7665  squeeze`) by ove
-000003c0: 726c 6f61 6469 6e67 2060 5f61 7070 6c79  rloading `_apply
-000003d0: 5f66 756e 6374 696f 6e60 2061 6e64 2072  _function` and r
-000003e0: 6567 6973 7465 7269 6e67 0a20 2020 2069  egistering.    i
-000003f0: 6e64 6976 6964 7561 6c20 6675 6e63 7469  ndividual functi
-00000400: 6f6e 2069 6d70 6c65 6d65 6e74 6174 696f  on implementatio
-00000410: 6e73 2076 6961 2060 696d 706c 656d 656e  ns via `implemen
-00000420: 7473 602e 0a0a 2020 2020 4974 2069 7320  ts`...    It is 
-00000430: 696d 706f 7274 616e 7420 746f 206e 6f74  important to not
-00000440: 6520 7468 6174 2074 6865 2075 7365 2063  e that the use c
-00000450: 6173 6573 206f 6620 7468 6973 2063 6c61  ases of this cla
-00000460: 7373 2065 7874 656e 6420 6265 796f 6e64  ss extend beyond
-00000470: 0a20 2020 2061 7272 6179 2d6c 696b 6520  .    array-like 
-00000480: 6f62 6a65 6374 732e 2042 6f74 6820 7369  objects. Both si
-00000490: 6e67 6c65 2d20 616e 6420 6d75 6c74 692d  ngle- and multi-
-000004a0: 7661 6c75 6564 206f 626a 6563 7473 2063  valued objects c
-000004b0: 616e 2062 656e 6566 6974 2066 726f 6d0a  an benefit from.
-000004c0: 2020 2020 696d 706c 656d 656e 7469 6e67      implementing
-000004d0: 2073 7570 706f 7274 2066 6f72 2060 6e75   support for `nu
-000004e0: 6d70 7960 2075 6e69 7665 7273 616c 2061  mpy` universal a
-000004f0: 6e64 2070 7562 6c69 6320 6675 6e63 7469  nd public functi
-00000500: 6f6e 732e 2046 6f72 0a20 2020 2065 7861  ons. For.    exa
-00000510: 6d70 6c65 2c20 6974 2070 6f73 7369 626c  mple, it possibl
-00000520: 6520 746f 2061 7070 6c79 2060 6e75 6d70  e to apply `nump
-00000530: 792e 7371 7274 6020 746f 2065 6974 6865  y.sqrt` to eithe
-00000540: 7220 6120 7265 616c 206e 756d 6265 7220  r a real number 
-00000550: 6f72 2061 6e0a 2020 2020 6172 7261 790a  or an.    array.
-00000560: 0a20 2020 203e 3e3e 206e 756d 7079 2e73  .    >>> numpy.s
-00000570: 7172 7428 3429 0a20 2020 2032 2e30 0a20  qrt(4).    2.0. 
-00000580: 2020 203e 3e3e 206e 756d 7079 2e73 7172     >>> numpy.sqr
-00000590: 7428 5b34 2c20 395d 290a 2020 2020 6172  t([4, 9]).    ar
-000005a0: 7261 7928 5b32 2e2c 2033 2e5d 290a 0a20  ray([2., 3.]).. 
-000005b0: 2020 2045 7665 6e20 7468 6520 7472 6976     Even the triv
-000005c0: 6961 6c20 6170 706c 6963 6174 696f 6e20  ial application 
-000005d0: 6f66 2060 6e75 6d70 792e 6d65 616e 6020  of `numpy.mean` 
-000005e0: 746f 2061 2072 6561 6c20 6e75 6d62 6572  to a real number
-000005f0: 2069 7320 6465 6669 6e65 643a 0a0a 2020   is defined:..  
-00000600: 2020 3e3e 3e20 6e75 6d70 792e 6d65 616e    >>> numpy.mean
-00000610: 2832 2e35 290a 2020 2020 322e 350a 0a20  (2.5).    2.5.. 
-00000620: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
-00000630: 2d2d 0a20 2020 202d 2054 6869 7320 636c  --.    - This cl
-00000640: 6173 7320 646f 6573 206e 6f74 2069 6e68  ass does not inh
-00000650: 6572 6974 2066 726f 6d20 606e 756d 7079  erit from `numpy
-00000660: 2e6c 6962 2e6d 6978 696e 732e 4e44 4172  .lib.mixins.NDAr
-00000670: 7261 794f 7065 7261 746f 7273 4d69 7869  rayOperatorsMixi
-00000680: 6e60 2c0a 2020 2020 2020 7768 6963 6820  n`,.      which 
-00000690: 696d 706c 656d 656e 7473 206d 6f73 7420  implements most 
-000006a0: 6f66 2074 6865 2062 7569 6c74 2d69 6e20  of the built-in 
-000006b0: 5079 7468 6f6e 206e 756d 6572 6963 206f  Python numeric o
-000006c0: 7065 7261 746f 7273 2076 6961 0a20 2020  perators via.   
-000006d0: 2020 2060 5f5f 6172 7261 795f 7566 756e     `__array_ufun
-000006e0: 635f 5f60 2c20 6265 6361 7573 6520 6974  c__`, because it
-000006f0: 2061 7373 756d 6573 2074 6861 7420 7375   assumes that su
-00000700: 6263 6c61 7373 6573 2069 6e64 6570 656e  bclasses indepen
-00000710: 6465 6e74 6c79 0a20 2020 2020 2069 6d70  dently.      imp
-00000720: 6c65 6d65 6e74 2074 6865 2072 6561 6c2d  lement the real-
-00000730: 7661 6c75 6564 2070 726f 746f 636f 6c2e  valued protocol.
-00000740: 2049 6e20 6661 6374 2c0a 2020 2020 2020   In fact,.      
-00000750: 606e 756d 7079 2e6c 6962 2e6d 6978 696e  `numpy.lib.mixin
-00000760: 732e 4e44 4172 7261 794f 7065 7261 746f  s.NDArrayOperato
-00000770: 7273 4d69 7869 6e60 2064 6566 696e 6573  rsMixin` defines
-00000780: 206d 756c 7469 706c 6520 6f70 6572 6174   multiple operat
-00000790: 6f72 7320 7468 6174 0a20 2020 2020 2061  ors that.      a
-000007a0: 7265 206e 6f74 2070 6172 7420 6f66 2074  re not part of t
-000007b0: 6865 2072 6561 6c2d 7661 6c75 6564 2070  he real-valued p
-000007c0: 726f 746f 636f 6c2e 2048 6f77 6576 6572  rotocol. However
-000007d0: 2c20 7365 650a 2020 2020 2020 6874 7470  , see.      http
-000007e0: 733a 2f2f 6e75 6d70 792e 6f72 672f 646f  s://numpy.org/do
-000007f0: 632f 7374 6162 6c65 2f72 6566 6572 656e  c/stable/referen
-00000800: 6365 2f67 656e 6572 6174 6564 2f6e 756d  ce/generated/num
-00000810: 7079 2e6c 6962 2e6d 6978 696e 732e 4e44  py.lib.mixins.ND
-00000820: 4172 7261 794f 7065 7261 746f 7273 4d69  ArrayOperatorsMi
-00000830: 7869 6e2e 6874 6d6c 236e 756d 7079 2e6c  xin.html#numpy.l
-00000840: 6962 2e6d 6978 696e 732e 4e44 4172 7261  ib.mixins.NDArra
-00000850: 794f 7065 7261 746f 7273 4d69 7869 6e0a  yOperatorsMixin.
-00000860: 2020 2020 2020 666f 7220 616e 2065 7861        for an exa
-00000870: 6d70 6c65 206f 6620 686f 7720 6f6e 6520  mple of how one 
-00000880: 6d69 6768 7420 7573 6520 7468 6174 206d  might use that m
-00000890: 6978 696e 2063 6c61 7373 2e0a 2020 2020  ixin class..    
-000008a0: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
-000008b0: 000f 0000 00f3 5601 0000 8707 9700 7c04  ......V.......|.
-000008c0: a000 0000 0000 0000 0000 0000 0000 0000  ................
-000008d0: 0000 0000 0000 6401 6402 a602 0000 ab02  ......d.d.......
-000008e0: 0000 0000 0000 0000 7d05 7403 0000 0000  ........}.t.....
-000008f0: 0000 0000 0000 7c00 6a02 0000 0000 0000  ......|.j.......
-00000900: 0000 a601 0000 ab01 0000 0000 0000 0000  ................
-00000910: 8a07 7407 0000 0000 0000 0000 0000 8807  ..t.............
-00000920: 6601 6403 8408 7c03 7c05 7a00 0000 4400  f.d...|.|.z...D.
-00000930: a600 0000 ab00 0000 0000 0000 0000 a601  ................
-00000940: 0000 ab01 0000 0000 0000 0000 7307 7408  ............s.t.
-00000950: 0000 0000 0000 0000 0000 5300 7c05 721c  ..........S.|.r.
-00000960: 7403 0000 0000 0000 0000 0000 6404 8400  t...........d...
-00000970: 7c05 4400 a600 0000 ab00 0000 0000 0000  |.D.............
-00000980: 0000 a601 0000 ab01 0000 0000 0000 0000  ................
-00000990: 7c04 6401 3c00 0000 7c00 a005 0000 0000  |.d.<...|.......
-000009a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000009b0: 7c01 a601 0000 ab01 0000 0000 0000 0000  |...............
-000009c0: 7215 7c00 6a06 0000 0000 0000 0000 7c01  r.|.j.........|.
-000009d0: 1900 0000 0000 0000 0000 7d06 0200 7c06  ..........}...|.
-000009e0: 7c03 6900 7c04 a401 8e01 5300 0200 7c00  |.i.|.....S...|.
-000009f0: 6a07 0000 0000 0000 0000 7c01 7c02 6702  j.........|.|.g.
-00000a00: 7c03 a201 5200 6900 7c04 a401 8e01 5300  |...R.i.|.....S.
-00000a10: 2905 61f9 0300 0050 726f 7669 6465 2073  ).a....Provide s
-00000a20: 7570 706f 7274 2066 6f72 2060 6e75 6d70  upport for `nump
-00000a30: 7960 2075 6e69 7665 7273 616c 2066 756e  y` universal fun
-00000a40: 6374 696f 6e73 2e0a 0a20 2020 2020 2020  ctions...       
-00000a50: 2053 6565 2068 7474 7073 3a2f 2f6e 756d   See https://num
-00000a60: 7079 2e6f 7267 2f64 6f63 2f73 7461 626c  py.org/doc/stabl
-00000a70: 652f 7265 6665 7265 6e63 652f 6172 7261  e/reference/arra
-00000a80: 7973 2e63 6c61 7373 6573 2e68 746d 6c20  ys.classes.html 
-00000a90: 666f 7220 6d6f 7265 0a20 2020 2020 2020  for more.       
-00000aa0: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00000ab0: 7573 6520 6f66 2074 6869 7320 7370 6563  use of this spec
-00000ac0: 6961 6c20 6d65 7468 6f64 2e0a 0a20 2020  ial method...   
-00000ad0: 2020 2020 204e 6f74 6573 0a20 2020 2020       Notes.     
-00000ae0: 2020 202d 2d2d 2d2d 0a20 2020 2020 2020     -----.       
-00000af0: 202d 2054 6869 7320 6d65 7468 6f64 2066   - This method f
-00000b00: 6972 7374 2065 6e73 7572 6573 2074 6861  irst ensures tha
-00000b10: 7420 7468 6520 696e 7075 7420 7479 7065  t the input type
-00000b20: 7320 2861 7320 7765 6c6c 2061 7320 7468  s (as well as th
-00000b30: 6520 7479 7065 206f 660a 2020 2020 2020  e type of.      
-00000b40: 2020 2020 606f 7574 602c 2069 6620 7061      `out`, if pa
-00000b50: 7373 6564 2076 6961 206b 6579 776f 7264  ssed via keyword
-00000b60: 2920 6172 6520 7375 7070 6f72 7465 6420  ) are supported 
-00000b70: 7479 7065 732e 2049 7420 7468 656e 2063  types. It then c
-00000b80: 6865 636b 7320 666f 720a 2020 2020 2020  hecks for.      
-00000b90: 2020 2020 6120 6375 7374 6f6d 2069 6d70      a custom imp
-00000ba0: 6c65 6d65 6e74 6174 696f 6e20 6f66 2060  lementation of `
-00000bb0: 7566 756e 6360 2e20 4966 2074 6865 7265  ufunc`. If there
-00000bc0: 2069 7320 6120 6375 7374 6f6d 0a20 2020   is a custom.   
-00000bd0: 2020 2020 2020 2069 6d70 6c65 6d65 6e74         implement
-00000be0: 6174 696f 6e2c 2074 6869 7320 6d65 7468  ation, this meth
-00000bf0: 6f64 2061 7070 6c69 6573 2069 7420 616e  od applies it an
-00000c00: 6420 7265 7475 726e 7320 7468 6520 7265  d returns the re
-00000c10: 7375 6c74 2e20 4966 0a20 2020 2020 2020  sult. If.       
-00000c20: 2020 2074 6865 7265 2069 7320 6e6f 2063     there is no c
-00000c30: 7573 746f 6d20 696d 706c 656d 656e 7461  ustom implementa
-00000c40: 7469 6f6e 2c20 7468 6973 206d 6574 686f  tion, this metho
-00000c50: 6420 7061 7373 6573 2063 6f6e 7472 6f6c  d passes control
-00000c60: 2074 6f0a 2020 2020 2020 2020 2020 605f   to.          `_
-00000c70: 6170 706c 795f 7566 756e 6360 2c20 746f  apply_ufunc`, to
-00000c80: 2061 6c6c 6f77 2073 7562 636c 6173 7320   allow subclass 
-00000c90: 6375 7374 6f6d 697a 6174 696f 6e2e 0a20  customization.. 
-00000ca0: 2020 2020 2020 202d 2053 6565 2060 696d         - See `im
-00000cb0: 706c 656d 656e 7473 6020 666f 7220 6164  plements` for ad
-00000cc0: 6469 7469 6f6e 616c 2067 7569 6461 6e63  ditional guidanc
-00000cd0: 6520 6f6e 2063 7573 746f 6d20 696d 706c  e on custom impl
-00000ce0: 656d 656e 7461 7469 6f6e 732e 0a0a 2020  ementations...  
-00000cf0: 2020 2020 2020 5365 6520 416c 736f 0a20        See Also. 
-00000d00: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0a         --------.
-00000d10: 2020 2020 2020 2020 6069 6d70 6c65 6d65          `impleme
-00000d20: 6e74 7360 0a20 2020 2020 2020 2020 2020  nts`.           
-00000d30: 2043 6c61 7373 206d 6574 686f 6420 666f   Class method fo
-00000d40: 7220 7265 6769 7374 6572 696e 6720 6375  r registering cu
-00000d50: 7374 6f6d 2075 6675 6e63 2069 6d70 6c65  stom ufunc imple
-00000d60: 6d65 6e74 6174 696f 6e73 2e0a 0a20 2020  mentations...   
-00000d70: 2020 2020 2060 5f61 7070 6c79 5f75 6675       `_apply_ufu
-00000d80: 6e63 600a 2020 2020 2020 2020 2020 2020  nc`.            
-00000d90: 496e 7374 616e 6365 206d 6574 686f 6420  Instance method 
-00000da0: 7468 6174 2061 6c6c 6f77 7320 6375 7374  that allows cust
-00000db0: 6f6d 2068 616e 646c 696e 6720 6f66 2075  om handling of u
-00000dc0: 6675 6e63 7320 636f 7272 6573 706f 6e64  funcs correspond
-00000dd0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00000de0: 746f 2073 7461 6e64 6172 6420 5079 7468  to standard Pyth
-00000df0: 6f6e 206e 756d 6572 6963 616c 206f 7065  on numerical ope
-00000e00: 7261 746f 7273 2e0a 2020 2020 2020 2020  rators..        
-00000e10: da03 6f75 74a9 0063 0100 0000 0000 0000  ..out..c........
-00000e20: 0000 0000 0500 0000 3300 0000 f338 0000  ........3....8..
-00000e30: 0095 014b 0001 0097 007c 005d 147d 0174  ...K.....|.].}.t
-00000e40: 0100 0000 0000 0000 0000 007c 0189 02a6  ...........|....
-00000e50: 0200 00ab 0200 0000 0000 0000 0056 0097  .............V..
-00000e60: 0101 008c 1564 0053 00a9 014e 2901 da0a  .....d.S...N)...
-00000e70: 6973 696e 7374 616e 6365 2903 da02 2e30  isinstance)....0
-00000e80: da01 78da 0861 6363 6570 7465 6473 0300  ..x..accepteds..
-00000e90: 0000 2020 80fa 3c2f 686f 6d65 2f6d 6174  ..  ..</home/mat
-00000ea0: 7468 6577 2f65 6d6d 7265 6d2f 6570 7265  thew/emmrem/epre
-00000eb0: 6d2f 7079 2f73 7263 2f65 7072 656d 7079  m/py/src/eprempy
-00000ec0: 2f6e 756d 6572 6963 2f5f 6d69 7869 6e73  /numeric/_mixins
-00000ed0: 2e70 79fa 093c 6765 6e65 7870 723e 7a2c  .py..<genexpr>z,
-00000ee0: 4675 6e63 7469 6f6e 732e 5f5f 6172 7261  Functions.__arra
-00000ef0: 795f 7566 756e 635f 5f2e 3c6c 6f63 616c  y_ufunc__.<local
-00000f00: 733e 2e3c 6765 6e65 7870 723e 5700 0000  s>.<genexpr>W...
-00000f10: 732d 0000 00f8 e800 e800 8000 d012 3fd0  s-............?.
-00000f20: 123f a871 953a 9861 a018 d113 2ad4 132a  .?.q.:.a....*..*
-00000f30: d012 3fd0 123f d012 3fd0 123f d012 3fd0  ..?..?..?..?..?.
-00000f40: 123f f300 0000 0063 0100 0000 0000 0000  .?.....c........
-00000f50: 0000 0000 0500 0000 3300 0000 f352 0000  ........3....R..
-00000f60: 004b 0001 0097 007c 005d 227d 0174 0100  .K.....|.]"}.t..
-00000f70: 0000 0000 0000 0000 007c 0174 0200 0000  .........|.t....
-00000f80: 0000 0000 0000 00a6 0200 00ab 0200 0000  ................
-00000f90: 0000 0000 0072 077c 016a 0200 0000 0000  .....r.|.j......
-00000fa0: 0000 006e 017c 0156 0097 0101 008c 2364  ...n.|.V......#d
-00000fb0: 0053 0072 0d00 0000 2903 720e 0000 0072  .S.r....).r....r
-00000fc0: 0500 0000 da05 5f64 6174 6129 0272 0f00  ......_data).r..
-00000fd0: 0000 7210 0000 0073 0200 0000 2020 7212  ..r....s....  r.
-00000fe0: 0000 0072 1300 0000 7a2c 4675 6e63 7469  ...r....z,Functi
-00000ff0: 6f6e 732e 5f5f 6172 7261 795f 7566 756e  ons.__array_ufun
-00001000: 635f 5f2e 3c6c 6f63 616c 733e 2e3c 6765  c__.<locals>.<ge
-00001010: 6e65 7870 723e 5a00 0000 734e 0000 00e8  nexpr>Z...sN....
-00001020: 00e8 0080 00f0 0003 220e f000 0322 0ee0  ........"...."..
-00001030: 1b1c f503 001c 26a0 61ad 16d1 1b30 d41b  ......&.a....0..
-00001040: 30f0 0001 1117 9001 9407 9007 d815 16f0  0...............
-00001050: 0503 220e f000 0322 0ef0 0003 220e f000  .."...."...."...
-00001060: 0322 0ef0 0003 220e f000 0322 0e72 1400  ."...."....".r..
-00001070: 0000 2908 da03 6765 74da 0574 7570 6c65  ..)...get..tuple
-00001080: da0c 5f55 4655 4e43 5f54 5950 4553 da03  .._UFUNC_TYPES..
-00001090: 616c 6cda 0e4e 6f74 496d 706c 656d 656e  all..NotImplemen
-000010a0: 7465 64da 0b5f 696d 706c 656d 656e 7473  ted.._implements
-000010b0: da0a 5f46 554e 4354 494f 4e53 da0c 5f61  .._FUNCTIONS.._a
-000010c0: 7070 6c79 5f75 6675 6e63 2908 da04 7365  pply_ufunc)...se
-000010d0: 6c66 da05 7566 756e 63da 066d 6574 686f  lf..ufunc..metho
-000010e0: 64da 0461 7267 73da 066b 7761 7267 7372  d..args..kwargsr
-000010f0: 0a00 0000 da08 6f70 6572 6174 6f72 7211  ......operatorr.
-00001100: 0000 0073 0800 0000 2020 2020 2020 2040  ...s....       @
-00001110: 7212 0000 00da 0f5f 5f61 7272 6179 5f75  r......__array_u
-00001120: 6675 6e63 5f5f 7a19 4675 6e63 7469 6f6e  func__z.Function
-00001130: 732e 5f5f 6172 7261 795f 7566 756e 635f  s.__array_ufunc_
-00001140: 5f3c 0000 0073 ec00 0000 f880 00f0 3200  _<...s........2.
-00001150: 0f15 8f6a 8a6a 9815 a002 d10e 23d4 0e23  ...j.j......#..#
-00001160: 8803 dd13 1898 14d4 192a d113 2bd4 132b  .........*..+..+
-00001170: 8808 dd0f 12d0 123f d012 3fd0 123f d012  .......?..?..?..
-00001180: 3fb0 44b8 33b1 4ad0 123f d112 3fd4 123f  ?.D.3.J..?..?..?
-00001190: d10f 3fd4 0f3f f000 0109 22dd 1321 d00c  ..?..?...."..!..
-000011a0: 21d8 0b0e f000 0409 0edd 1c21 f000 0322  !..........!..."
-000011b0: 0ef0 0003 220e e020 23f0 0503 220e f100  ....".. #..."...
-000011c0: 0322 0ef4 0003 220e f100 031d 0ef4 0003  ."....".........
-000011d0: 1d0e 8846 9035 894d f008 000c 10d7 0b1b  ...F.5.M........
-000011e0: d20b 1b98 45d1 0b22 d40b 22f0 0002 092d  ....E..".."....-
-000011f0: d817 1b94 7fa0 75d4 172d 8848 d813 1b90  ......u..-.H....
-00001200: 3898 54d0 132c a056 d013 2cd0 132c d00c  8.T..,.V..,..,..
-00001210: 2cd8 0f20 8874 d40f 20a0 15a8 06d0 0f40  ,.. .t.. ......@
-00001220: b014 d00f 40d0 0f40 d00f 40b8 16d0 0f40  ....@..@..@....@
-00001230: d00f 40d0 0840 7214 0000 0063 0300 0000  ..@..@r....c....
-00001240: 0000 0000 0000 0000 0700 0000 0f00 0000  ................
-00001250: f3c4 0000 0097 0074 0100 0000 0000 0000  .......t........
-00001260: 0000 007c 017c 02a6 0200 00ab 0200 0000  ...|.|..........
-00001270: 0000 0000 007d 057c 00a0 0100 0000 0000  .....}.|........
-00001280: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00001290: 03a6 0100 00ab 0100 0000 0000 0000 007d  ...............}
-000012a0: 0609 0002 007c 057c 0669 007c 04a4 018e  .....|.|.i.|....
-000012b0: 017d 076e 2823 0074 0400 0000 0000 0000  .}.n(#.t........
-000012c0: 0000 0024 0072 1b7d 0874 0500 0000 0000  ...$.r.}.t......
-000012d0: 0000 0000 0064 017c 019b 0064 027c 039b  .....d.|...d.|..
-000012e0: 009d 04a6 0100 00ab 0100 0000 0000 0000  ................
-000012f0: 007c 0882 0264 037d 087e 0877 0177 0078  .|...d.}.~.w.w.x
-00001300: 0359 0077 017c 0264 046b 0300 0000 0072  .Y.w.|.d.k.....r
-00001310: 027c 0753 0064 0353 0029 0561 fc03 0000  .|.S.d.S.).a....
-00001320: 4170 706c 7920 6120 606e 756d 7079 6020  Apply a `numpy` 
-00001330: 756e 6976 6572 7361 6c20 6675 6e63 7469  universal functi
-00001340: 6f6e 2028 612e 6b2e 6120 2275 6675 6e63  on (a.k.a "ufunc
-00001350: 2229 2074 6f20 6461 7461 2e0a 0a20 2020  ") to data...   
-00001360: 2020 2020 204e 6f74 6573 0a20 2020 2020       Notes.     
-00001370: 2020 202d 2d2d 2d2d 0a20 2020 2020 2020     -----.       
-00001380: 202d 2053 7562 636c 6173 7365 7320 7468   - Subclasses th
-00001390: 6174 2077 6973 6820 746f 2063 7573 746f  at wish to custo
-000013a0: 6d69 7a65 2073 7570 706f 7274 2066 6f72  mize support for
-000013b0: 2075 6675 6e63 7320 7368 6f75 6c64 206f   ufuncs should o
-000013c0: 7665 726c 6f61 640a 2020 2020 2020 2020  verload.        
-000013d0: 2020 7468 6973 206d 6574 686f 6420 696e    this method in
-000013e0: 7374 6561 6420 6f66 2060 5f5f 6172 7261  stead of `__arra
-000013f0: 795f 7566 756e 635f 5f60 2e0a 2020 2020  y_ufunc__`..    
-00001400: 2020 2020 2d20 5375 6263 6c61 7373 6573      - Subclasses
-00001410: 2073 686f 756c 6420 7072 6566 6572 2074   should prefer t
-00001420: 6f20 6465 6669 6e65 2063 7573 746f 6d20  o define custom 
-00001430: 696d 706c 656d 656e 7461 7469 6f6e 7320  implementations 
-00001440: 6f66 2073 7065 6369 6669 630a 2020 2020  of specific.    
-00001450: 2020 2020 2020 756e 6976 6572 7361 6c20        universal 
-00001460: 6675 6e63 7469 6f6e 7320 616e 6420 7265  functions and re
-00001470: 6769 7374 6572 2065 6163 6820 7669 6120  gister each via 
-00001480: 6069 6d70 6c65 6d65 6e74 7360 2c20 7261  `implements`, ra
-00001490: 7468 6572 2074 6861 6e0a 2020 2020 2020  ther than.      
-000014a0: 2020 2020 696d 706c 656d 656e 7469 6e67      implementing
-000014b0: 2066 756e 6374 696f 6e2d 7370 6563 6966   function-specif
-000014c0: 6963 206c 6f67 6963 2069 6e20 7468 6973  ic logic in this
-000014d0: 206d 6574 686f 642c 2073 696e 6365 0a20   method, since. 
-000014e0: 2020 2020 2020 2020 2060 5f5f 6172 7261           `__arra
-000014f0: 795f 7566 756e 635f 5f60 2077 696c 6c20  y_ufunc__` will 
-00001500: 6368 6563 6b20 666f 7220 6120 6375 7374  check for a cust
-00001510: 6f6d 2069 6d70 6c65 6d65 6e74 6174 696f  om implementatio
-00001520: 6e20 6f66 2061 2067 6976 656e 0a20 2020  n of a given.   
-00001530: 2020 2020 2020 2066 756e 6374 696f 6e20         function 
-00001540: 6265 666f 7265 2063 616c 6c69 6e67 2074  before calling t
-00001550: 6869 7320 6d65 7468 6f64 2e0a 2020 2020  his method..    
-00001560: 2020 2020 2d20 5468 6520 6465 6661 756c      - The defaul
-00001570: 7420 696d 706c 656d 656e 7461 7469 6f6e  t implementation
-00001580: 206f 6620 7468 6973 206d 6574 686f 6420   of this method 
-00001590: 6170 706c 6965 7320 7468 6520 6769 7665  applies the give
-000015a0: 6e20 7566 756e 6320 746f 0a20 2020 2020  n ufunc to.     
-000015b0: 2020 2020 2072 6561 6c2d 7661 6c75 6564       real-valued
-000015c0: 2064 6174 6120 616e 6420 6469 7265 6374   data and direct
-000015d0: 6c79 2072 6574 7572 6e73 2074 6865 2060  ly returns the `
-000015e0: 6e75 6d70 7960 2072 6573 756c 742c 2077  numpy` result, w
-000015f0: 6974 686f 7574 0a20 2020 2020 2020 2020  ithout.         
-00001600: 2061 7474 656d 7074 696e 6720 746f 2063   attempting to c
-00001610: 7265 6174 6520 6120 6e65 7720 696e 7374  reate a new inst
-00001620: 616e 6365 206f 6620 7468 6520 6375 7374  ance of the cust
-00001630: 6f6d 2073 7562 636c 6173 732e 0a0a 2020  om subclass...  
-00001640: 2020 2020 2020 5365 6520 416c 736f 0a20        See Also. 
-00001650: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0a         --------.
-00001660: 2020 2020 2020 2020 6069 6d70 6c65 6d65          `impleme
-00001670: 6e74 7360 0a20 2020 2020 2020 2020 2020  nts`.           
-00001680: 2043 6c61 7373 206d 6574 686f 6420 666f   Class method fo
-00001690: 7220 7265 6769 7374 6572 696e 6720 6375  r registering cu
-000016a0: 7374 6f6d 2075 6675 6e63 2069 6d70 6c65  stom ufunc imple
-000016b0: 6d65 6e74 6174 696f 6e73 2e0a 0a20 2020  mentations...   
-000016c0: 2020 2020 2060 5f5f 6172 7261 795f 7566       `__array_uf
-000016d0: 756e 635f 5f60 0a20 2020 2020 2020 2020  unc__`.         
-000016e0: 2020 2054 6865 2065 6e74 7279 2070 6f69     The entry poi
-000016f0: 6e74 2066 6f72 2060 6e75 6d70 7960 2075  nt for `numpy` u
-00001700: 6e69 7665 7273 616c 2066 756e 6374 696f  niversal functio
-00001710: 6e73 2e0a 2020 2020 2020 2020 7a10 556e  ns..        z.Un
-00001720: 6162 6c65 2074 6f20 6170 706c 7920 7a04  able to apply z.
-00001730: 2074 6f20 4eda 0261 7429 03da 0767 6574   to N..at)...get
-00001740: 6174 7472 da0f 5f67 6574 5f6e 756d 7079  attr.._get_numpy
-00001750: 5f61 7267 73da 0954 7970 6545 7272 6f72  _args..TypeError
-00001760: 2909 721f 0000 0072 2000 0000 7221 0000  ).r....r ...r!..
-00001770: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00001780: da06 7661 6c75 6573 da04 6461 7461 da03  ..values..data..
-00001790: 6572 7273 0900 0000 2020 2020 2020 2020  errs....        
-000017a0: 2072 1200 0000 721e 0000 007a 1646 756e   r....r....z.Fun
-000017b0: 6374 696f 6e73 2e5f 6170 706c 795f 7566  ctions._apply_uf
-000017c0: 756e 6363 0000 0073 9f00 0000 8000 f530  uncc...s.......0
-000017d0: 0014 1b98 35a0 26d1 1329 d413 2988 08d8  ....5.&..)..)...
-000017e0: 1115 d711 25d2 1125 a064 d111 2bd4 112b  ....%..%.d..+..+
-000017f0: 8806 f002 0509 17d8 131b 9038 9856 d013  ...........8.V..
-00001800: 2ea0 76d0 132e d013 2e88 4488 44f8 dd0f  ..v.......D.D...
-00001810: 18f0 0003 0917 f000 0309 17f0 0003 0917  ................
-00001820: dd12 1bd8 1034 a035 d010 34d0 1034 a864  .....4.5..4..4.d
-00001830: d010 34d0 1034 f103 0213 0ef4 0002 130e  ..4..4..........
-00001840: e013 16f0 0502 0d17 f8f8 f8f8 f003 0309  ................
-00001850: 17f8 f8f8 f008 000c 1290 548a 3e88 3ed8  ..........T.>.>.
-00001860: 1317 884b f003 000c 1a88 3e73 1400 0000  ...K......>s....
-00001870: a708 3000 b00a 4115 03ba 1641 1003 c110  ..0...A....A....
-00001880: 0541 1503 6305 0000 0000 0000 0000 0000  .A..c...........
-00001890: 0006 0000 0003 0000 00f3 f000 0000 8705  ................
-000018a0: 9700 7401 0000 0000 0000 0000 0000 7c00  ..t...........|.
-000018b0: 6a01 0000 0000 0000 0000 a601 0000 ab01  j...............
-000018c0: 0000 0000 0000 0000 8a05 7405 0000 0000  ..........t.....
-000018d0: 0000 0000 0000 8805 6601 6401 8408 7c02  ........f.d...|.
-000018e0: 4400 a600 0000 ab00 0000 0000 0000 0000  D...............
-000018f0: a601 0000 ab01 0000 0000 0000 0000 7307  ..............s.
-00001900: 7406 0000 0000 0000 0000 0000 5300 7c00  t...........S.|.
-00001910: a004 0000 0000 0000 0000 0000 0000 0000  ................
-00001920: 0000 0000 0000 7c01 a601 0000 ab01 0000  ......|.........
-00001930: 0000 0000 0000 7213 0200 7c00 6a05 0000  ......r...|.j...
-00001940: 0000 0000 0000 7c01 1900 0000 0000 0000  ......|.........
-00001950: 0000 7c03 6900 7c04 a401 8e01 5300 7c00  ..|.i.|.....S.|.
-00001960: a006 0000 0000 0000 0000 0000 0000 0000  ................
-00001970: 0000 0000 0000 7c01 7c02 7c03 7c04 a604  ......|.|.|.|...
-00001980: 0000 ab04 0000 0000 0000 0000 5300 2902  ............S.).
-00001990: 614d 0500 0050 726f 7669 6465 2073 7570  aM...Provide sup
-000019a0: 706f 7274 2066 6f72 2066 756e 6374 696f  port for functio
-000019b0: 6e73 2069 6e20 7468 6520 606e 756d 7079  ns in the `numpy
-000019c0: 6020 7075 626c 6963 2041 5049 2e0a 0a20  ` public API... 
-000019d0: 2020 2020 2020 2053 6565 2068 7474 7073         See https
-000019e0: 3a2f 2f6e 756d 7079 2e6f 7267 2f64 6f63  ://numpy.org/doc
-000019f0: 2f73 7461 626c 652f 7265 6665 7265 6e63  /stable/referenc
-00001a00: 652f 6172 7261 7973 2e63 6c61 7373 6573  e/arrays.classes
-00001a10: 2e68 746d 6c20 666f 7220 6d6f 7265 0a20  .html for more. 
-00001a20: 2020 2020 2020 2069 6e66 6f72 6d61 7469         informati
-00001a30: 6f6e 206f 6620 7573 6520 6f66 2074 6869  on of use of thi
-00001a40: 7320 7370 6563 6961 6c20 6d65 7468 6f64  s special method
-00001a50: 2e20 5468 6520 696d 706c 656d 656e 7461  . The implementa
-00001a60: 7469 6f6e 2073 686f 776e 2068 6572 650a  tion shown here.
-00001a70: 2020 2020 2020 2020 6973 2061 2063 6f6d          is a com
-00001a80: 6269 6e61 7469 6f6e 206f 6620 7468 6520  bination of the 
-00001a90: 6578 616d 706c 6520 6f6e 2074 6861 7420  example on that 
-00001aa0: 7061 6765 2061 6e64 2063 6f64 6520 6672  page and code fr
-00001ab0: 6f6d 2074 6865 0a20 2020 2020 2020 2064  om the.        d
-00001ac0: 6566 696e 6974 696f 6e20 6f66 2060 456e  efinition of `En
-00001ad0: 6361 7073 756c 6174 654e 4441 7272 6179  capsulateNDArray
-00001ae0: 2e5f 5f61 7272 6179 5f66 756e 6374 696f  .__array_functio
-00001af0: 6e5f 5f60 2069 6e0a 2020 2020 2020 2020  n__` in.        
-00001b00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001b10: 6f6d 2f64 6173 6b2f 6461 736b 2f62 6c6f  om/dask/dask/blo
-00001b20: 622f 6d61 696e 2f64 6173 6b2f 6172 7261  b/main/dask/arra
-00001b30: 792f 7465 7374 732f 7465 7374 5f64 6973  y/tests/test_dis
-00001b40: 7061 7463 682e 7079 0a0a 2020 2020 2020  patch.py..      
-00001b50: 2020 4e6f 7465 730a 2020 2020 2020 2020    Notes.        
-00001b60: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2d20  -----.        - 
-00001b70: 5468 6973 206d 6574 686f 6420 6669 7273  This method firs
-00001b80: 7420 6368 6563 6b73 2074 6861 7420 616c  t checks that al
-00001b90: 6c20 6074 7970 6573 6020 6172 6520 696e  l `types` are in
-00001ba0: 0a20 2020 2020 2020 2020 2060 7365 6c66  .          `self
-00001bb0: 2e5f 4655 4e43 5449 4f4e 5f54 5950 4553  ._FUNCTION_TYPES
-00001bc0: 602c 2074 6865 7265 6279 2061 6c6c 6f77  `, thereby allow
-00001bd0: 696e 6720 7375 6263 6c61 7373 6573 2074  ing subclasses t
-00001be0: 6861 7420 646f 6e27 740a 2020 2020 2020  hat don't.      
-00001bf0: 2020 2020 6f76 6572 7269 6465 2060 5f5f      override `__
-00001c00: 6172 7261 795f 6675 6e63 7469 6f6e 5f5f  array_function__
-00001c10: 6020 746f 2068 616e 646c 6520 6f62 6a65  ` to handle obje
-00001c20: 6374 7320 6f66 2074 6869 7320 7479 7065  cts of this type
-00001c30: 2e20 4974 2074 6865 6e0a 2020 2020 2020  . It then.      
-00001c40: 2020 2020 6368 6563 6b73 2066 6f72 2061      checks for a
-00001c50: 2063 7573 746f 6d20 696d 706c 656d 656e   custom implemen
-00001c60: 7461 7469 6f6e 206f 6620 6066 756e 6360  tation of `func`
-00001c70: 2e20 4966 2074 6865 7265 2069 7320 6120  . If there is a 
-00001c80: 6375 7374 6f6d 0a20 2020 2020 2020 2020  custom.         
-00001c90: 2069 6d70 6c65 6d65 6e74 6174 696f 6e2c   implementation,
-00001ca0: 2074 6869 7320 6d65 7468 6f64 2061 7070   this method app
-00001cb0: 6c69 6573 2069 7420 616e 6420 7265 7475  lies it and retu
-00001cc0: 726e 7320 7468 6520 7265 7375 6c74 2e20  rns the result. 
-00001cd0: 4966 0a20 2020 2020 2020 2020 2074 6865  If.          the
-00001ce0: 7265 2069 7320 6e6f 2063 7573 746f 6d20  re is no custom 
-00001cf0: 696d 706c 656d 656e 7461 7469 6f6e 2c20  implementation, 
-00001d00: 7468 6973 206d 6574 686f 6420 7061 7373  this method pass
-00001d10: 6573 2063 6f6e 7472 6f6c 2074 6f0a 2020  es control to.  
-00001d20: 2020 2020 2020 2020 605f 6170 706c 795f          `_apply_
-00001d30: 6675 6e63 7469 6f6e 602c 2074 6f20 616c  function`, to al
-00001d40: 6c6f 7720 7375 6263 6c61 7373 2063 7573  low subclass cus
-00001d50: 746f 6d69 7a61 7469 6f6e 2e0a 2020 2020  tomization..    
-00001d60: 2020 2020 2d20 5365 6520 6069 6d70 6c65      - See `imple
-00001d70: 6d65 6e74 7360 2066 6f72 2061 6464 6974  ments` for addit
-00001d80: 696f 6e61 6c20 6775 6964 616e 6365 206f  ional guidance o
-00001d90: 6e20 6375 7374 6f6d 2069 6d70 6c65 6d65  n custom impleme
-00001da0: 6e74 6174 696f 6e73 2e0a 0a20 2020 2020  ntations...     
-00001db0: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
-00001dc0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00001dd0: 2020 2020 2060 696d 706c 656d 656e 7473       `implements
-00001de0: 600a 2020 2020 2020 2020 2020 2020 436c  `.            Cl
-00001df0: 6173 7320 6d65 7468 6f64 2066 6f72 2072  ass method for r
-00001e00: 6567 6973 7465 7269 6e67 2063 7573 746f  egistering custo
-00001e10: 6d20 6675 6e63 7469 6f6e 2069 6d70 6c65  m function imple
-00001e20: 6d65 6e74 6174 696f 6e73 2e0a 0a20 2020  mentations...   
-00001e30: 2020 2020 2060 5f61 7070 6c79 5f66 756e       `_apply_fun
-00001e40: 6374 696f 6e60 0a20 2020 2020 2020 2020  ction`.         
-00001e50: 2020 2049 6e73 7461 6e63 6520 6d65 7468     Instance meth
-00001e60: 6f64 2074 6861 7420 616c 6c6f 7773 2063  od that allows c
-00001e70: 7573 746f 6d20 6861 6e64 6c69 6e67 206f  ustom handling o
-00001e80: 6620 606e 756d 7079 6020 7075 626c 6963  f `numpy` public
-00001e90: 0a20 2020 2020 2020 2020 2020 2066 756e  .            fun
-00001ea0: 6374 696f 6e73 2077 6865 6e20 7468 6572  ctions when ther
-00001eb0: 6520 6973 206e 6f20 7265 6769 7374 6572  e is no register
-00001ec0: 6564 2063 7573 746f 6d20 696d 706c 656d  ed custom implem
-00001ed0: 656e 7461 7469 6f6e 2e0a 2020 2020 2020  entation..      
-00001ee0: 2020 6301 0000 0000 0000 0000 0000 0005    c.............
-00001ef0: 0000 0033 0000 00f3 3800 0000 9501 4b00  ...3....8.....K.
-00001f00: 0100 9700 7c00 5d14 7d01 7401 0000 0000  ....|.].}.t.....
-00001f10: 0000 0000 0000 7c01 8902 a602 0000 ab02  ......|.........
-00001f20: 0000 0000 0000 0000 5600 9701 0100 8c15  ........V.......
-00001f30: 6400 5300 720d 0000 0029 01da 0a69 7373  d.S.r....)...iss
-00001f40: 7562 636c 6173 7329 0372 0f00 0000 da02  ubclass).r......
-00001f50: 7469 7211 0000 0073 0300 0000 2020 8072  tir....s....  .r
-00001f60: 1200 0000 7213 0000 007a 2f46 756e 6374  ....r....z/Funct
-00001f70: 696f 6e73 2e5f 5f61 7272 6179 5f66 756e  ions.__array_fun
-00001f80: 6374 696f 6e5f 5f2e 3c6c 6f63 616c 733e  ction__.<locals>
-00001f90: 2e3c 6765 6e65 7870 723e a900 0000 732d  .<genexpr>....s-
-00001fa0: 0000 00f8 e800 e800 8000 d012 3cd0 123c  ............<..<
-00001fb0: b002 953a 9862 a028 d113 2bd4 132b d012  ...:.b.(..+..+..
-00001fc0: 3cd0 123c d012 3cd0 123c d012 3cd0 123c  <..<..<..<..<..<
-00001fd0: 7214 0000 0029 0772 1800 0000 da0f 5f46  r....).r......_F
-00001fe0: 554e 4354 494f 4e5f 5459 5045 5372 1a00  UNCTION_TYPESr..
-00001ff0: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00002000: 00da 0f5f 6170 706c 795f 6675 6e63 7469  ..._apply_functi
-00002010: 6f6e 2906 721f 0000 00da 0466 756e 63da  on).r......func.
-00002020: 0574 7970 6573 7222 0000 0072 2300 0000  .typesr"...r#...
-00002030: 7211 0000 0073 0600 0000 2020 2020 2040  r....s....     @
-00002040: 7212 0000 00da 125f 5f61 7272 6179 5f66  r......__array_f
-00002050: 756e 6374 696f 6e5f 5f7a 1c46 756e 6374  unction__z.Funct
-00002060: 696f 6e73 2e5f 5f61 7272 6179 5f66 756e  ions.__array_fun
-00002070: 6374 696f 6e5f 5f8b 0000 0073 8c00 0000  ction__....s....
-00002080: f880 00f5 3a00 1419 9814 d419 2dd1 132e  ....:.......-...
-00002090: d413 2e88 08dd 0f12 d012 3cd0 123c d012  ..........<..<..
-000020a0: 3cd0 123c b065 d012 3cd1 123c d412 3cd1  <..<.e..<..<..<.
-000020b0: 0f3c d40f 3cf0 0001 0922 dd13 21d0 0c21  .<..<...."..!..!
-000020c0: d80b 0fd7 0b1b d20b 1b98 44d1 0b21 d40b  ..........D..!..
-000020d0: 21f0 0001 093a d813 2890 3494 3fa0 34d4  !....:..(.4.?.4.
-000020e0: 1328 a824 d013 39b0 26d0 1339 d013 39d0  .(.$..9.&..9..9.
-000020f0: 0c39 d80f 13d7 0f23 d20f 23a0 44a8 25b0  .9.....#..#.D.%.
-00002100: 14b0 76d1 0f3e d40f 3ed0 083e 7214 0000  ..v..>..>..>r...
-00002110: 0063 0500 0000 0000 0000 0000 0000 0600  .c..............
-00002120: 0000 0300 0000 f32e 0100 0097 007c 00a0  .............|..
-00002130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002140: 0000 0000 00a6 0000 00ab 0000 0000 0000  ................
-00002150: 0000 007d 057c 0580 0774 0200 0000 0000  ...}.|...t......
-00002160: 0000 0000 0053 0074 0500 0000 0000 0000  .....S.t........
-00002170: 0000 007c 0574 0600 0000 0000 0000 0000  ...|.t..........
-00002180: 006a 0400 0000 0000 0000 00a6 0200 00ab  .j..............
-00002190: 0200 0000 0000 0000 0073 1d74 0b00 0000  .........s.t....
-000021a0: 0000 0000 0000 007c 006a 0600 0000 0000  .......|.j......
-000021b0: 0000 006a 0700 0000 0000 0000 009b 0064  ...j...........d
-000021c0: 029d 02a6 0100 00ab 0100 0000 0000 0000  ................
-000021d0: 0064 0182 027c 00a0 0800 0000 0000 0000  .d...|..........
-000021e0: 0000 0000 0000 0000 0000 0000 007c 03a6  .............|..
-000021f0: 0100 00ab 0100 0000 0000 0000 007d 037c  .............}.|
-00002200: 00a0 0900 0000 0000 0000 0000 0000 0000  ................
-00002210: 0000 0000 0000 007c 02a6 0100 00ab 0100  .......|........
-00002220: 0000 0000 0000 007d 027c 05a0 0a00 0000  .......}.|......
-00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002240: 007c 017c 027c 037c 04a6 0400 00ab 0400  .|.|.|.|........
-00002250: 0000 0000 0000 0053 0029 0361 a104 0000  .......S.).a....
-00002260: 4170 706c 7920 6120 6675 6e63 7469 6f6e  Apply a function
-00002270: 2069 6e20 7468 6520 606e 756d 7079 6020   in the `numpy` 
-00002280: 7075 626c 6963 2041 5049 2e0a 0a20 2020  public API...   
-00002290: 2020 2020 204e 6f74 6573 0a20 2020 2020       Notes.     
-000022a0: 2020 202d 2d2d 2d2d 0a20 2020 2020 2020     -----.       
-000022b0: 202d 2053 7562 636c 6173 7365 7320 7468   - Subclasses th
-000022c0: 6174 2077 6973 6820 746f 2063 7573 746f  at wish to custo
-000022d0: 6d69 7a65 2073 7570 706f 7274 2066 6f72  mize support for
-000022e0: 2070 7562 6c69 6320 6675 6e63 7469 6f6e   public function
-000022f0: 7320 7368 6f75 6c64 0a20 2020 2020 2020  s should.       
-00002300: 2020 206f 7665 726c 6f61 6420 7468 6973     overload this
-00002310: 206d 6574 686f 6420 696e 7374 6561 6420   method instead 
-00002320: 6f66 2060 5f5f 6172 7261 795f 6675 6e63  of `__array_func
-00002330: 7469 6f6e 5f5f 602e 0a20 2020 2020 2020  tion__`..       
-00002340: 202d 2053 7562 636c 6173 7365 7320 7368   - Subclasses sh
-00002350: 6f75 6c64 2070 7265 6665 7220 746f 2064  ould prefer to d
-00002360: 6566 696e 6520 6375 7374 6f6d 2069 6d70  efine custom imp
-00002370: 6c65 6d65 6e74 6174 696f 6e73 206f 6620  lementations of 
-00002380: 7370 6563 6966 6963 0a20 2020 2020 2020  specific.       
-00002390: 2020 2070 7562 6c69 6320 6675 6e63 7469     public functi
-000023a0: 6f6e 7320 616e 6420 7265 6769 7374 6572  ons and register
-000023b0: 2065 6163 6820 7669 6120 6069 6d70 6c65   each via `imple
-000023c0: 6d65 6e74 7360 2c20 7261 7468 6572 2074  ments`, rather t
-000023d0: 6861 6e0a 2020 2020 2020 2020 2020 696d  han.          im
-000023e0: 706c 656d 656e 7469 6e67 2066 756e 6374  plementing funct
-000023f0: 696f 6e2d 7370 6563 6966 6963 206c 6f67  ion-specific log
-00002400: 6963 2069 6e20 7468 6973 206d 6574 686f  ic in this metho
-00002410: 642c 2073 696e 6365 0a20 2020 2020 2020  d, since.       
-00002420: 2020 2060 5f5f 6172 7261 795f 6675 6e63     `__array_func
-00002430: 7469 6f6e 5f5f 6020 7769 6c6c 2063 6865  tion__` will che
-00002440: 636b 2066 6f72 2061 2063 7573 746f 6d20  ck for a custom 
-00002450: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-00002460: 6620 6120 6769 7665 6e0a 2020 2020 2020  f a given.      
-00002470: 2020 2020 6675 6e63 7469 6f6e 2062 6566      function bef
-00002480: 6f72 6520 6361 6c6c 696e 6720 7468 6973  ore calling this
-00002490: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
-000024a0: 202d 2054 6865 2064 6566 6175 6c74 2069   - The default i
-000024b0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6361  mplementation ca
-000024c0: 6c6c 7320 605f 6765 745f 6e75 6d70 795f  lls `_get_numpy_
-000024d0: 6172 7261 7960 2066 6f72 2061 6363 6573  array` for acces
-000024e0: 7320 746f 0a20 2020 2020 2020 2020 2072  s to.          r
-000024f0: 6561 6c2d 7661 6c75 6564 2064 6174 6120  eal-valued data 
-00002500: 7669 6120 616e 2069 6e73 7461 6e63 6520  via an instance 
-00002510: 6f66 2060 6e75 6d70 792e 6e64 6172 7261  of `numpy.ndarra
-00002520: 7960 2c20 605f 6765 745f 6e75 6d70 795f  y`, `_get_numpy_
-00002530: 6172 6773 600a 2020 2020 2020 2020 2020  args`.          
-00002540: 746f 2063 6f6e 7665 7274 2060 6172 6773  to convert `args
-00002550: 6020 746f 2061 7070 726f 7072 6961 7465  ` to appropriate
-00002560: 206f 7065 7261 6e64 732c 2061 6e64 2060   operands, and `
-00002570: 5f67 6574 5f6e 756d 7079 5f74 7970 6573  _get_numpy_types
-00002580: 6020 746f 0a20 2020 2020 2020 2020 2065  ` to.          e
-00002590: 7874 7261 6374 2061 7070 726f 7072 6961  xtract appropria
-000025a0: 7465 206f 7065 7261 6e64 2074 7970 6573  te operand types
-000025b0: 2e20 5375 6263 6c61 7373 6573 206d 6179  . Subclasses may
-000025c0: 2063 686f 6f73 6520 746f 206f 7665 726c   choose to overl
-000025d0: 6f61 640a 2020 2020 2020 2020 2020 616e  oad.          an
-000025e0: 7920 6f66 2074 686f 7365 2069 6e64 6976  y of those indiv
-000025f0: 6964 7561 6c20 6d65 7468 6f64 7320 696e  idual methods in
-00002600: 7374 6561 6420 6f66 206f 7665 726c 6f61  stead of overloa
-00002610: 6469 6e67 2074 6869 7320 6d65 7468 6f64  ding this method
-00002620: 2e0a 0a20 2020 2020 2020 2053 6565 2041  ...        See A
-00002630: 6c73 6f0a 2020 2020 2020 2020 2d2d 2d2d  lso.        ----
-00002640: 2d2d 2d2d 0a20 2020 2020 2020 2060 696d  ----.        `im
-00002650: 706c 656d 656e 7473 600a 2020 2020 2020  plements`.      
-00002660: 2020 2020 2020 436c 6173 7320 6d65 7468        Class meth
-00002670: 6f64 2066 6f72 2072 6567 6973 7465 7269  od for registeri
-00002680: 6e67 2063 7573 746f 6d20 7566 756e 6320  ng custom ufunc 
-00002690: 696d 706c 656d 656e 7461 7469 6f6e 732e  implementations.
-000026a0: 0a0a 2020 2020 2020 2020 605f 5f61 7272  ..        `__arr
-000026b0: 6179 5f66 756e 6374 696f 6e5f 5f60 0a20  ay_function__`. 
-000026c0: 2020 2020 2020 2020 2020 2054 6865 2065             The e
-000026d0: 6e74 7279 2070 6f69 6e74 2066 6f72 2060  ntry point for `
-000026e0: 6e75 6d70 7960 2070 7562 6c69 6320 6675  numpy` public fu
-000026f0: 6e63 7469 6f6e 732e 0a20 2020 2020 2020  nctions..       
-00002700: 204e 7a30 2e5f 6765 745f 6e75 6d70 795f   Nz0._get_numpy_
-00002710: 6172 7261 7920 6469 6420 6e6f 7420 7265  array did not re
-00002720: 7475 726e 2061 206e 756d 7079 2e6e 6461  turn a numpy.nda
-00002730: 7272 6179 290b da10 5f67 6574 5f6e 756d  rray)..._get_num
-00002740: 7079 5f61 7272 6179 721b 0000 0072 0e00  py_arrayr....r..
-00002750: 0000 da05 6e75 6d70 79da 076e 6461 7272  ....numpy..ndarr
-00002760: 6179 722a 0000 00da 095f 5f63 6c61 7373  ayr*.....__class
-00002770: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00002780: 7229 0000 00da 105f 6765 745f 6e75 6d70  r)....._get_nump
-00002790: 795f 7479 7065 7372 3600 0000 2906 721f  y_typesr6...).r.
-000027a0: 0000 0072 3400 0000 7235 0000 0072 2200  ...r4...r5...r".
-000027b0: 0000 7223 0000 00da 0561 7272 6179 7306  ..r#.....arrays.
-000027c0: 0000 0020 2020 2020 2072 1200 0000 7233  ...      r....r3
-000027d0: 0000 007a 1946 756e 6374 696f 6e73 2e5f  ...z.Functions._
-000027e0: 6170 706c 795f 6675 6e63 7469 6f6e af00  apply_function..
-000027f0: 0000 73a4 0000 0080 00f0 3400 1115 d710  ..s.......4.....
-00002800: 25d2 1025 d110 27d4 1027 8805 d80b 1088  %..%..'..'......
-00002810: 3ddd 1321 d00c 21dd 0f19 9825 a515 a41d  =..!..!....%....
-00002820: d10f 2fd4 0f2f f000 0409 18dd 121b d813  ../../..........
-00002830: 1794 3ed4 132e f000 0111 32f0 0001 1132  ..>.......2....2
-00002840: f000 0111 32f1 0303 130e f400 0313 0ef0  ....2...........
-00002850: 0600 1418 f007 030d 18f0 0800 1014 d70f  ................
-00002860: 23d2 0f23 a044 d10f 29d4 0f29 8804 d810  #..#.D..)..)....
-00002870: 14d7 1025 d210 25a0 65d1 102c d410 2c88  ...%..%.e..,..,.
-00002880: 05d8 0f14 d70f 27d2 0f27 a804 a865 b054  ......'..'...e.T
-00002890: b836 d10f 42d4 0f42 d008 4272 1400 0000  .6..B..B..Br....
-000028a0: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-000028b0: 0000 0000 0001 0000 0003 0000 00f3 0600  ................
-000028c0: 0000 9700 6401 5300 2902 61da 0100 0043  ....d.S.).a....C
-000028d0: 6f6e 7665 7274 2074 6865 2064 6174 6120  onvert the data 
-000028e0: 696e 7465 7266 6163 6520 746f 2061 6e20  interface to an 
-000028f0: 6172 7261 7920 666f 7220 606e 756d 7079  array for `numpy
-00002900: 6020 6d69 7869 6e20 6d65 7468 6f64 732e  ` mixin methods.
-00002910: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002920: 2020 4e6f 7465 730a 2020 2020 2020 2020    Notes.        
-00002930: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2d20  -----.        - 
-00002940: 5468 6973 206d 6574 686f 6420 616c 6c6f  This method allo
-00002950: 7773 2073 7562 636c 6173 7320 696d 706c  ws subclass impl
-00002960: 656d 656e 7461 7469 6f6e 7320 746f 2063  ementations to c
-00002970: 6f6e 7472 6f6c 2068 6f77 2074 6865 790a  ontrol how they.
-00002980: 2020 2020 2020 2020 2020 636f 6e76 6572            conver
-00002990: 7420 7468 6569 7220 6461 7461 2069 6e74  t their data int
-000029a0: 6572 6661 6365 2074 6f20 6120 606e 756d  erface to a `num
-000029b0: 7079 2e6e 6461 7272 6179 6020 666f 7220  py.ndarray` for 
-000029c0: 7573 6520 7769 7468 2060 6e75 6d70 7960  use with `numpy`
-000029d0: 0a20 2020 2020 2020 2020 2070 7562 6c69  .          publi
-000029e0: 6320 6675 6e63 7469 6f6e 732e 0a20 2020  c functions..   
-000029f0: 2020 2020 202d 2052 6574 7572 6e69 6e67       - Returning
-00002a00: 2060 4e6f 6e65 6020 6672 6f6d 2074 6869   `None` from thi
-00002a10: 7320 6d65 7468 6f64 2077 696c 6c20 6361  s method will ca
-00002a20: 7573 6520 605f 6170 706c 795f 6675 6e63  use `_apply_func
-00002a30: 7469 6f6e 6020 746f 0a20 2020 2020 2020  tion` to.       
-00002a40: 2020 2072 6574 7572 6e20 604e 6f74 496d     return `NotIm
-00002a50: 706c 656d 656e 7465 6460 2e0a 2020 2020  plemented`..    
-00002a60: 2020 2020 2d20 5468 6520 6465 6661 756c      - The defaul
-00002a70: 7420 696d 706c 656d 656e 7461 7469 6f6e  t implementation
-00002a80: 2075 6e63 6f6e 6469 7469 6f6e 616c 6c79   unconditionally
-00002a90: 2072 6574 7572 6e73 2060 4e6f 6e65 602e   returns `None`.
-00002aa0: 0a20 2020 2020 2020 204e 720b 0000 0029  .        Nr....)
-00002ab0: 0172 1f00 0000 7301 0000 0020 7212 0000  .r....s.... r...
-00002ac0: 0072 3800 0000 7a1a 4675 6e63 7469 6f6e  .r8...z.Function
-00002ad0: 732e 5f67 6574 5f6e 756d 7079 5f61 7272  s._get_numpy_arr
-00002ae0: 6179 d500 0000 7309 0000 0080 00f0 1800  ay....s.........
-00002af0: 090f 8806 7214 0000 0063 0200 0000 0000  ....r....c......
-00002b00: 0000 0000 0000 0400 0000 0300 0000 f33a  ...............:
-00002b10: 0000 0087 0097 0074 0100 0000 0000 0000  .......t........
-00002b20: 0000 0088 0066 0164 0184 087c 0144 00a6  .....f.d...|.D..
-00002b30: 0000 00ab 0000 0000 0000 0000 00a6 0100  ................
-00002b40: 00ab 0100 0000 0000 0000 0053 0029 0261  ...........S.).a
-00002b50: 1d01 0000 436f 6e76 6572 7420 6061 7267  ....Convert `arg
-00002b60: 7360 2074 6f20 6f70 6572 616e 6473 206f  s` to operands o
-00002b70: 6620 6120 606e 756d 7079 6020 6675 6e63  f a `numpy` func
-00002b80: 7469 6f6e 2e0a 0a20 2020 2020 2020 2054  tion...        T
-00002b90: 6869 7320 6d65 7468 6f64 2077 696c 6c20  his method will 
-00002ba0: 6361 6c6c 2060 7e5f 6765 745f 6e75 6d70  call `~_get_nump
-00002bb0: 795f 6172 6760 206f 6e20 6561 6368 206d  y_arg` on each m
-00002bc0: 656d 6265 7220 6f66 2060 6172 6773 6020  ember of `args` 
-00002bd0: 696e 0a20 2020 2020 2020 206f 7264 6572  in.        order
-00002be0: 2074 6f20 6275 696c 6420 6120 6074 7570   to build a `tup
-00002bf0: 6c65 6020 6f66 2073 7569 7461 626c 6520  le` of suitable 
-00002c00: 6f70 6572 616e 6473 2e20 5375 6263 6c61  operands. Subcla
-00002c10: 7373 6573 206d 6179 206f 7665 726c 6f61  sses may overloa
-00002c20: 640a 2020 2020 2020 2020 607e 5f67 6574  d.        `~_get
-00002c30: 5f6e 756d 7079 5f61 7267 6020 746f 2063  _numpy_arg` to c
-00002c40: 7573 746f 6d69 7a65 2061 6363 6573 7320  ustomize access 
-00002c50: 746f 2074 6865 6972 2064 6174 6120 6174  to their data at
-00002c60: 7472 6962 7574 652e 0a20 2020 2020 2020  tribute..       
-00002c70: 2063 0100 0000 0000 0000 0000 0000 0400   c..............
-00002c80: 0000 3300 0000 f342 0000 0095 014b 0001  ..3....B.....K..
-00002c90: 0097 007c 005d 197d 0189 02a0 0000 0000  ...|.].}........
-00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cb0: 007c 01a6 0100 00ab 0100 0000 0000 0000  .|..............
-00002cc0: 0056 0097 0101 008c 1a64 0053 0072 0d00  .V.......d.S.r..
-00002cd0: 0000 2901 da0d 5f67 6574 5f61 7267 5f64  ..)..._get_arg_d
-00002ce0: 6174 6129 0372 0f00 0000 da03 6172 6772  ata).r......argr
-00002cf0: 1f00 0000 7303 0000 0020 2080 7212 0000  ....s....  .r...
-00002d00: 0072 1300 0000 7a2c 4675 6e63 7469 6f6e  .r....z,Function
-00002d10: 732e 5f67 6574 5f6e 756d 7079 5f61 7267  s._get_numpy_arg
-00002d20: 732e 3c6c 6f63 616c 733e 2e3c 6765 6e65  s.<locals>.<gene
-00002d30: 7870 723e ea00 0000 7331 0000 00f8 e800  xpr>....s1......
-00002d40: e800 8000 d014 3dd0 143d b013 9054 d715  ......=..=...T..
-00002d50: 27d2 1527 a803 d115 2cd4 152c d014 3dd0  '..'....,..,..=.
-00002d60: 143d d014 3dd0 143d d014 3dd0 143d 7214  .=..=..=..=..=r.
-00002d70: 0000 00a9 0172 1800 0000 2902 721f 0000  .....r....).r...
-00002d80: 0072 2200 0000 7302 0000 0060 2072 1200  .r"...s....` r..
-00002d90: 0000 7229 0000 007a 1946 756e 6374 696f  ..r)...z.Functio
-00002da0: 6e73 2e5f 6765 745f 6e75 6d70 795f 6172  ns._get_numpy_ar
-00002db0: 6773 e300 0000 7328 0000 00f8 8000 f50e  gs....s(........
-00002dc0: 0010 15d0 143d d014 3dd0 143d d014 3db8  .....=..=..=..=.
-00002dd0: 04d0 143d d114 3dd4 143d d10f 3dd4 0f3d  ...=..=..=..=..=
-00002de0: d008 3d72 1400 0000 6302 0000 0000 0000  ..=r....c.......
-00002df0: 0000 0000 0004 0000 0003 0000 00f3 3e00  ..............>.
-00002e00: 0000 9700 7401 0000 0000 0000 0000 0000  ....t...........
-00002e10: 7c01 7402 0000 0000 0000 0000 0000 a602  |.t.............
-00002e20: 0000 ab02 0000 0000 0000 0000 7207 7c01  ............r.|.
-00002e30: 6a02 0000 0000 0000 0000 5300 7c01 5300  j.........S.|.S.
-00002e40: 2901 6109 0200 0043 6f6e 7665 7274 2060  ).a....Convert `
-00002e50: 6172 6760 2074 6f20 616e 206f 7065 7261  arg` to an opera
-00002e60: 6e64 206f 6620 6120 606e 756d 7079 6020  nd of a `numpy` 
-00002e70: 6675 6e63 7469 6f6e 2e0a 0a20 2020 2020  function...     
-00002e80: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
-00002e90: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00002ea0: 2020 2020 2060 7e5f 6765 745f 6e75 6d70       `~_get_nump
-00002eb0: 795f 6172 6773 600a 2020 2020 2020 2020  y_args`.        
-00002ec0: 2020 2020 5468 6520 6d65 7468 6f64 2074      The method t
-00002ed0: 6861 7420 6361 6c6c 7320 7468 6973 206d  hat calls this m
-00002ee0: 6574 686f 6420 696e 2061 206c 6f6f 702e  ethod in a loop.
-00002ef0: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
-00002f00: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
-00002f10: 2020 2020 2020 2d20 5468 6973 206d 6574        - This met
-00002f20: 686f 6420 616c 6c6f 7773 2061 2073 7562  hod allows a sub
-00002f30: 636c 6173 7320 746f 2063 7573 746f 6d69  class to customi
-00002f40: 7a65 2068 6f77 2060 6e75 6d70 7960 2066  ze how `numpy` f
-00002f50: 756e 6374 696f 6e73 0a20 2020 2020 2020  unctions.       
-00002f60: 2020 2061 6363 6573 7320 6974 7320 6461     access its da
-00002f70: 7461 2061 7474 7269 6275 7465 2e0a 2020  ta attribute..  
-00002f80: 2020 2020 2020 2d20 5468 6520 6465 6661        - The defa
-00002f90: 756c 7420 696d 706c 656d 656e 7461 7469  ult implementati
-00002fa0: 6f6e 2077 696c 6c20 7265 7475 726e 2074  on will return t
-00002fb0: 6865 2060 6461 7461 6020 6174 7472 6962  he `data` attrib
-00002fc0: 7574 6520 6f66 2061 0a20 2020 2020 2020  ute of a.       
-00002fd0: 2020 2060 7e6e 756d 6572 6963 2e4f 626a     `~numeric.Obj
-00002fe0: 6563 7460 2c20 7468 6520 605f 6f62 6a65  ect`, the `_obje
-00002ff0: 6374 6020 6174 7472 6962 7574 6520 6f66  ct` attribute of
-00003000: 2061 0a20 2020 2020 2020 2020 2060 7e6e   a.          `~n
-00003010: 756d 6572 6963 2e51 7561 6e74 6974 7960  umeric.Quantity`
-00003020: 2c20 6f72 206f 7468 6572 7769 7365 2074  , or otherwise t
-00003030: 6865 2075 6e6d 6f64 6966 6965 6420 6172  he unmodified ar
-00003040: 6775 6d65 6e74 2e0a 2020 2020 2020 2020  gument..        
-00003050: 2903 720e 0000 0072 0500 0000 722c 0000  ).r....r....r,..
-00003060: 0029 0272 1f00 0000 7244 0000 0073 0200  .).r....rD...s..
-00003070: 0000 2020 7212 0000 0072 4300 0000 7a17  ..  r....rC...z.
-00003080: 4675 6e63 7469 6f6e 732e 5f67 6574 5f61  Functions._get_a
-00003090: 7267 5f64 6174 61ec 0000 0073 2200 0000  rg_data....s"...
-000030a0: 8000 f520 000c 1690 639d 36d1 0b22 d40b  ... ....c.6.."..
-000030b0: 22f0 0001 091c d813 1694 3888 4fd8 0f12  ".........8.O...
-000030c0: 880a 7214 0000 0063 0200 0000 0000 0000  ..r....c........
-000030d0: 0000 0000 0400 0000 0300 0000 f334 0000  .............4..
-000030e0: 0097 0074 0100 0000 0000 0000 0000 0064  ...t...........d
-000030f0: 0184 007c 0144 00a6 0000 00ab 0000 0000  ...|.D..........
-00003100: 0000 0000 00a6 0100 00ab 0100 0000 0000  ................
-00003110: 0000 0053 0029 0261 6901 0000 4578 7472  ...S.).ai...Extr
-00003120: 6163 7420 6170 7072 6f70 7269 6174 6520  act appropriate 
-00003130: 7479 7065 7320 666f 7220 6120 606e 756d  types for a `num
-00003140: 7079 6020 6675 6e63 7469 6f6e 2e0a 2020  py` function..  
-00003150: 2020 2020 2020 0a20 2020 2020 2020 204e        .        N
-00003160: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
-00003170: 2d2d 0a20 2020 2020 2020 202d 2054 6869  --.        - Thi
-00003180: 7320 6d65 7468 6f64 2061 6c6c 6f77 7320  s method allows 
-00003190: 7375 6263 6c61 7373 6573 2074 6f20 7265  subclasses to re
-000031a0: 7374 7269 6374 2074 6865 206f 626a 6563  strict the objec
-000031b0: 7420 7479 7065 7320 7468 6174 2074 6865  t types that the
-000031c0: 790a 2020 2020 2020 2020 2020 7061 7373  y.          pass
-000031d0: 2074 6f20 606e 756d 7079 6020 7075 626c   to `numpy` publ
-000031e0: 6963 2066 756e 6374 696f 6e73 2076 6961  ic functions via
-000031f0: 2060 5f61 7070 6c79 5f66 756e 6374 696f   `_apply_functio
-00003200: 6e60 2e0a 2020 2020 2020 2020 2d20 5468  n`..        - Th
-00003210: 6520 6465 6661 756c 7420 696d 706c 656d  e default implem
-00003220: 656e 7461 7469 6f6e 2072 6574 7572 6e73  entation returns
-00003230: 2061 2074 7570 6c65 2074 6861 7420 636f   a tuple that co
-00003240: 6e74 6169 6e73 2061 6c6c 2074 7970 6573  ntains all types
-00003250: 0a20 2020 2020 2020 2020 2065 7863 6570  .          excep
-00003260: 7420 666f 7220 7375 6274 7970 6573 206f  t for subtypes o
-00003270: 6620 607e 4f62 6a65 6374 602e 0a20 2020  f `~Object`..   
-00003280: 2020 2020 2063 0100 0000 0000 0000 0000       c..........
-00003290: 0000 0500 0000 3300 0000 f344 0000 004b  ......3....D...K
-000032a0: 0001 0097 007c 005d 1b7d 0174 0100 0000  .....|.].}.t....
-000032b0: 0000 0000 0000 007c 0174 0200 0000 0000  .......|.t......
-000032c0: 0000 0000 00a6 0200 00ab 0200 0000 0000  ................
-000032d0: 0000 00b0 177c 0156 0097 0101 008c 1c64  .....|.V.......d
-000032e0: 0053 0072 0d00 0000 2902 7230 0000 0072  .S.r....).r0...r
-000032f0: 0500 0000 2902 720f 0000 0072 3100 0000  ....).r....r1...
-00003300: 7302 0000 0020 2072 1200 0000 7213 0000  s....  r....r...
-00003310: 007a 2d46 756e 6374 696f 6e73 2e5f 6765  .z-Functions._ge
-00003320: 745f 6e75 6d70 795f 7479 7065 732e 3c6c  t_numpy_types.<l
-00003330: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00003340: 0a01 0000 7346 0000 00e8 00e8 0080 00f0  ....sF..........
-00003350: 0003 150a f000 0315 0ad8 1315 dd13 1d98  ................
-00003360: 62a5 26d1 1329 d413 29f0 0503 150a d80c  b.&..)..).......
-00003370: 0ef0 0303 150a f000 0315 0af0 0003 150a  ................
-00003380: f000 0315 0af0 0003 150a f000 0315 0a72  ...............r
-00003390: 1400 0000 7245 0000 0029 0272 1f00 0000  ....rE...).r....
-000033a0: 7235 0000 0073 0200 0000 2020 7212 0000  r5...s....  r...
-000033b0: 0072 3d00 0000 7a1a 4675 6e63 7469 6f6e  .r=...z.Function
-000033c0: 732e 5f67 6574 5f6e 756d 7079 5f74 7970  s._get_numpy_typ
-000033d0: 6573 0001 0000 7332 0000 0080 00f5 1400  es....s2........
-000033e0: 1015 f000 0315 0af0 0003 150a d819 1ef0  ................
-000033f0: 0303 150a f100 0315 0af4 0003 150a f100  ................
-00003400: 0310 0af4 0003 100a f000 0309 0a72 1400  .............r..
-00003410: 0000 da09 6f70 6572 6174 696f 6e63 0200  ....operationc..
-00003420: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00003430: 0000 f33e 0000 0097 0009 007c 017c 006a  ...>.......|.|.j
-00003440: 0000 0000 0000 0000 0076 007d 026e 1123  .........v.}.n.#
-00003450: 0074 0200 0000 0000 0000 0000 0024 0072  .t...........$.r
-00003460: 0401 0059 0064 0153 0077 0078 0359 0077  ...Y.d.S.w.x.Y.w
-00003470: 017c 0253 0029 02fa e554 7275 6520 6966  .|.S.)...True if
-00003480: 2074 6869 7320 636c 6173 7320 6465 6669   this class defi
-00003490: 6e65 7320 6120 6375 7374 6f6d 2069 6d70  nes a custom imp
-000034a0: 6c65 6d65 6e74 6174 696f 6e20 666f 7220  lementation for 
-000034b0: 606f 7065 7261 7469 6f6e 602e 0a20 2020  `operation`..   
-000034c0: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
-000034d0: 6973 2069 7320 6120 6865 6c70 6572 206d  is is a helper m
-000034e0: 6574 686f 6473 2074 6861 7420 6772 6163  ethods that grac
-000034f0: 6566 756c 6c79 2068 616e 646c 6573 2074  efully handles t
-00003500: 6865 2063 6173 6520 696e 2077 6869 6368  he case in which
-00003510: 2061 0a20 2020 2020 2020 2073 7562 636c   a.        subcl
-00003520: 6173 7320 646f 6573 206e 6f74 2073 7570  ass does not sup
-00003530: 706f 7274 2063 7573 746f 6d20 6f70 6572  port custom oper
-00003540: 6174 6f72 2069 6d70 6c65 6d65 6e74 6174  ator implementat
-00003550: 696f 6e73 2e0a 2020 2020 2020 2020 4629  ions..        F)
-00003560: 0272 1d00 0000 722a 0000 0029 03da 0363  .r....r*...)...c
-00003570: 6c73 7249 0000 00da 0672 6573 756c 7473  lsrI.....results
-00003580: 0300 0000 2020 2072 1200 0000 721c 0000  ....   r....r...
-00003590: 007a 1546 756e 6374 696f 6e73 2e5f 696d  .z.Functions._im
-000035a0: 706c 656d 656e 7473 0f01 0000 733c 0000  plements....s<..
-000035b0: 0080 00f0 0e03 0919 d815 1ea0 23a4 2ed0  ............#...
-000035c0: 1530 8846 8846 f8dd 0f18 f000 0109 19f0  .0.F.F..........
-000035d0: 0001 0919 f000 0109 19d8 1318 9035 9035  .............5.5
-000035e0: f003 0109 19f8 f8f8 e00f 1588 0d73 0c00  .............s..
-000035f0: 0000 8209 0c00 8c0a 1a03 9901 1a03 4e72  ..............Nr
-00003600: 1d00 0000 da0e 6e75 6d70 795f 6675 6e63  ......numpy_func
-00003610: 7469 6f6e 6302 0000 0000 0000 0000 0000  tionc...........
-00003620: 0003 0000 0003 0000 00f3 6400 0000 8700  ..........d.....
-00003630: 8701 9700 7401 0000 0000 0000 0000 0000  ....t...........
-00003640: 8901 a601 0000 ab01 0000 0000 0000 0000  ................
-00003650: 7310 7403 0000 0000 0000 0000 0000 6401  s.t...........d.
-00003660: a601 0000 ab01 0000 0000 0000 0000 6402  ..............d.
-00003670: 8202 6403 7404 0000 0000 0000 0000 0000  ..d.t...........
-00003680: 6602 8800 8801 6602 6404 840c 7d02 7c02  f.....f.d...}.|.
-00003690: 5300 2905 6112 0600 0052 6567 6973 7465  S.).a....Registe
-000036a0: 7220 6120 6375 7374 6f6d 2069 6d70 6c65  r a custom imple
-000036b0: 6d65 6e74 6174 696f 6e20 6f66 2074 6869  mentation of thi
-000036c0: 7320 606e 756d 7079 6020 6675 6e63 7469  s `numpy` functi
-000036d0: 6f6e 2e0a 0a20 2020 2020 2020 2050 6172  on...        Par
-000036e0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-000036f0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00003700: 2020 206e 756d 7079 5f66 756e 6374 696f     numpy_functio
-00003710: 6e20 3a20 6361 6c6c 6162 6c65 0a20 2020  n : callable.   
-00003720: 2020 2020 2020 2020 2054 6865 2060 6e75           The `nu
-00003730: 6d70 7960 2075 6e69 7665 7273 616c 206f  mpy` universal o
-00003740: 7220 7075 626c 6963 2066 756e 6374 696f  r public functio
-00003750: 6e20 746f 2069 6d70 6c65 6d65 6e74 2e0a  n to implement..
-00003760: 0a20 2020 2020 2020 204e 6f74 6573 0a20  .        Notes. 
-00003770: 2020 2020 2020 202d 2d2d 2d2d 0a20 2020         -----.   
-00003780: 2020 2020 202d 2055 7365 7273 206d 6179       - Users may
-00003790: 2072 6567 6973 7465 7220 606e 756d 7079   register `numpy
-000037a0: 6020 756e 6976 6572 7361 6c20 6675 6e63  ` universal func
-000037b0: 7469 6f6e 7320 2861 2e6b 2e61 2e20 7566  tions (a.k.a. uf
-000037c0: 756e 6373 3b0a 2020 2020 2020 2020 2020  uncs;.          
-000037d0: 6874 7470 733a 2f2f 6e75 6d70 792e 6f72  https://numpy.or
-000037e0: 672f 646f 632f 7374 6162 6c65 2f72 6566  g/doc/stable/ref
-000037f0: 6572 656e 6365 2f75 6675 6e63 732e 6874  erence/ufuncs.ht
-00003800: 6d6c 2920 6173 2077 656c 6c20 6173 0a20  ml) as well as. 
-00003810: 2020 2020 2020 2020 2066 756e 6374 696f           functio
-00003820: 6e73 2069 6e20 7468 6520 7075 626c 6963  ns in the public
-00003830: 2060 6e75 6d70 7960 2041 5049 2028 652e   `numpy` API (e.
-00003840: 672e 2c20 606e 756d 7079 2e6d 6561 6e60  g., `numpy.mean`
-00003850: 292e 2054 6869 7320 6d61 7920 6265 0a20  ). This may be. 
-00003860: 2020 2020 2020 2020 2069 6d70 6f72 7461           importa
-00003870: 6e74 2069 662c 2066 6f72 2065 7861 6d70  nt if, for examp
-00003880: 6c65 2c20 6120 636c 6173 7320 6e65 6564  le, a class need
-00003890: 7320 746f 2069 6d70 6c65 6d65 6e74 2061  s to implement a
-000038a0: 2063 7573 746f 6d20 7665 7273 696f 6e0a   custom version.
-000038b0: 2020 2020 2020 2020 2020 6f66 2060 6e75            of `nu
-000038c0: 6d70 792e 7371 7274 602c 2077 6869 6368  mpy.sqrt`, which
-000038d0: 2069 7320 6120 7566 756e 632e 0a20 2020   is a ufunc..   
-000038e0: 2020 2020 202d 2053 6565 2068 7474 7073       - See https
-000038f0: 3a2f 2f6e 756d 7079 2e6f 7267 2f64 6f63  ://numpy.org/doc
-00003900: 2f73 7461 626c 652f 7265 6665 7265 6e63  /stable/referenc
-00003910: 652f 6172 7261 7973 2e63 6c61 7373 6573  e/arrays.classes
-00003920: 2e68 746d 6c20 666f 7220 7468 650a 2020  .html for the.  
-00003930: 2020 2020 2020 2020 7375 6767 6573 7469          suggesti
-00003940: 6f6e 206f 6e20 7768 6963 6820 7468 6973  on on which this
-00003950: 206d 6574 686f 6420 6973 2062 6173 6564   method is based
-00003960: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-00003970: 6c65 730a 2020 2020 2020 2020 2d2d 2d2d  les.        ----
-00003980: 2d2d 2d2d 0a20 2020 2020 2020 204f 7665  ----.        Ove
-00003990: 726c 6f61 6420 606e 756d 7079 2e6d 6561  rload `numpy.mea
-000039a0: 6e60 2066 6f72 2061 6e20 6578 6973 7469  n` for an existi
-000039b0: 6e67 2063 6c61 7373 2063 616c 6c65 6420  ng class called 
-000039c0: 6041 7272 6179 6020 7769 7468 2061 0a20  `Array` with a. 
-000039d0: 2020 2020 2020 2076 6572 7369 6f6e 2074         version t
-000039e0: 6861 7420 6163 6365 7074 7320 6e6f 206b  hat accepts no k
-000039f0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-00003a00: 3a0a 0a20 2020 2020 2020 2060 6060 0a20  :..        ```. 
-00003a10: 2020 2020 2020 2020 2020 2040 4172 7261             @Arra
-00003a20: 792e 696d 706c 656d 656e 7473 286e 756d  y.implements(num
-00003a30: 7079 2e6d 6561 6e29 0a20 2020 2020 2020  py.mean).       
-00003a40: 2020 2020 2064 6566 206d 6561 6e28 613a       def mean(a:
-00003a50: 2041 7272 6179 2c20 2a2a 6b77 6172 6773   Array, **kwargs
-00003a60: 2920 2d3e 2041 7272 6179 3a0a 2020 2020  ) -> Array:.    
-00003a70: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00003a80: 7761 7267 733a 0a20 2020 2020 2020 2020  wargs:.         
-00003a90: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
-00003aa0: 2022 4361 6e6e 6f74 2070 6173 7320 6b65   "Cannot pass ke
-00003ab0: 7977 6f72 6473 2074 6f20 6e75 6d70 792e  ywords to numpy.
-00003ac0: 6d65 616e 2077 6974 6820 4172 7261 7922  mean with Array"
-00003ad0: 2072 6169 7365 0a20 2020 2020 2020 2020   raise.         
-00003ae0: 2020 2020 2020 2020 2020 2054 7970 6545             TypeE
-00003af0: 7272 6f72 286d 7367 290a 2020 2020 2020  rror(msg).      
-00003b00: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003b10: 206e 756d 7079 2e73 756d 2861 2920 2f20   numpy.sum(a) / 
-00003b20: 6c65 6e28 6129 0a20 2020 2020 2020 2060  len(a).        `
-00003b30: 6060 0a0a 2020 2020 2020 2020 5468 6973  ``..        This
-00003b40: 2077 696c 6c20 636f 6d70 7574 6520 7468   will compute th
-00003b50: 6520 6d65 616e 206f 6620 7468 6520 756e  e mean of the un
-00003b60: 6465 726c 7969 6e67 2064 6174 6120 7768  derlying data wh
-00003b70: 656e 2063 616c 6c65 6420 7769 7468 206e  en called with n
-00003b80: 6f0a 2020 2020 2020 2020 6172 6775 6d65  o.        argume
-00003b90: 6e74 732c 2062 7574 2077 696c 6c20 7261  nts, but will ra
-00003ba0: 6973 6520 616e 2065 7863 6570 7469 6f6e  ise an exception
-00003bb0: 2077 6865 6e20 6361 6c6c 6564 2077 6974   when called wit
-00003bc0: 6820 6172 6775 6d65 6e74 733a 0a0a 2020  h arguments:..  
-00003bd0: 2020 2020 2020 2020 2020 3e3e 3e20 7620            >>> v 
-00003be0: 3d20 4172 7261 7928 5b5b 312c 2032 5d2c  = Array([[1, 2],
-00003bf0: 205b 332c 2034 5d5d 290a 2020 2020 2020   [3, 4]]).      
-00003c00: 2020 2020 2020 3e3e 3e20 6e75 6d70 792e        >>> numpy.
-00003c10: 6d65 616e 2876 290a 2020 2020 2020 2020  mean(v).        
-00003c20: 2020 2020 352e 300a 2020 2020 2020 2020      5.0.        
-00003c30: 2020 2020 3e3e 3e20 6e75 6d70 792e 6d65      >>> numpy.me
-00003c40: 616e 2876 2c20 6178 6973 3d30 290a 2020  an(v, axis=0).  
-00003c50: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-00003c60: 2020 2020 2020 2020 2020 5479 7065 4572            TypeEr
-00003c70: 726f 723a 2043 616e 6e6f 7420 7061 7373  ror: Cannot pass
-00003c80: 206b 6579 776f 7264 7320 746f 206e 756d   keywords to num
-00003c90: 7079 2e6d 6561 6e20 7769 7468 2041 7272  py.mean with Arr
-00003ca0: 6179 0a20 2020 2020 2020 207a 4654 6865  ay.        zFThe
-00003cb0: 2074 6172 6765 7420 6f70 6572 6174 696f   target operatio
-00003cc0: 6e20 6f66 2061 2063 7573 746f 6d20 6e75  n of a custom nu
-00003cd0: 6d70 7920 696d 706c 656d 656e 7461 7469  mpy implementati
-00003ce0: 6f6e 206d 7573 7420 6265 2063 616c 6c61  on must be calla
-00003cf0: 626c 654e da0d 7573 6572 5f66 756e 6374  bleN..user_funct
-00003d00: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
-00003d10: 0500 0000 1300 0000 f352 0000 0095 0297  .........R......
-00003d20: 0089 016a 0000 0000 0000 0000 0080 1474  ...j...........t
-00003d30: 0300 0000 0000 0000 0000 0064 0189 019b  ...........d....
-00003d40: 0064 029d 03a6 0100 00ab 0100 0000 0000  .d..............
-00003d50: 0000 0064 0082 027c 0089 016a 0000 0000  ...d...|...j....
-00003d60: 0000 0000 0089 023c 0000 007c 0053 0029  .......<...|.S.)
-00003d70: 034e fa05 5479 7065 207a 3b20 646f 6573  .N..Type z; does
-00003d80: 206e 6f74 2073 7570 706f 7274 2063 7573   not support cus
-00003d90: 746f 6d20 696d 706c 656d 656e 7461 7469  tom implementati
-00003da0: 6f6e 7320 6f66 206e 756d 7079 2066 756e  ons of numpy fun
-00003db0: 6374 696f 6e73 2902 721d 0000 00da 134e  ctions).r......N
-00003dc0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00003dd0: 6f72 2903 7250 0000 0072 4c00 0000 724e  or).rP...rL...rN
-00003de0: 0000 0073 0300 0000 2080 8072 1200 0000  ...s.... ..r....
-00003df0: da09 6465 636f 7261 746f 727a 2746 756e  ..decoratorz'Fun
-00003e00: 6374 696f 6e73 2e69 6d70 6c65 6d65 6e74  ctions.implement
-00003e10: 732e 3c6c 6f63 616c 733e 2e64 6563 6f72  s.<locals>.decor
-00003e20: 6174 6f72 4f01 0000 734c 0000 00f8 8000  atorO...sL......
-00003e30: d80f 128c 7ed0 0f25 dd16 29f0 0201 152a  ....~..%..)....*
-00003e40: 9843 f000 0115 2af0 0001 152a f000 0115  .C....*....*....
-00003e50: 2af1 0303 1712 f400 0317 12f0 0600 181c  *...............
-00003e60: f007 0311 1cf0 0800 2e3b 8843 8c4e 983e  .........;.C.N.>
-00003e70: d10c 2ad8 1320 d00c 2072 1400 0000 2903  ..*.. .. r....).
-00003e80: da08 6361 6c6c 6162 6c65 722a 0000 00da  ..callabler*....
-00003e90: 0c55 7365 7246 756e 6374 696f 6e29 0372  .UserFunction).r
-00003ea0: 4c00 0000 724e 0000 0072 5400 0000 7303  L...rN...rT...s.
-00003eb0: 0000 0060 6020 7212 0000 00da 0a69 6d70  ...`` r......imp
-00003ec0: 6c65 6d65 6e74 737a 1446 756e 6374 696f  lementsz.Functio
-00003ed0: 6e73 2e69 6d70 6c65 6d65 6e74 731f 0100  ns.implements...
-00003ee0: 0073 6500 0000 f8f8 8000 f556 0100 1018  .se........V....
-00003ef0: 980e d10f 27d4 0f27 f000 0409 18dd 121b  ....'..'........
-00003f00: f002 0111 24f1 0303 130e f400 0313 0ef0  ....$...........
-00003f10: 0600 1418 f007 030d 18f0 0807 0921 a55c  .............!.\
-00003f20: f000 0709 21f0 0007 0921 f000 0709 21f0  ....!....!....!.
-00003f30: 0007 0921 f000 0709 21f0 0007 0921 f000  ...!....!....!..
-00003f40: 0709 21f0 1000 1019 d008 1872 1400 0000  ..!........r....
-00003f50: 2920 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  ) ..__name__..__
-00003f60: 6d6f 6475 6c65 5f5f 723c 0000 00da 075f  module__r<....._
-00003f70: 5f64 6f63 5f5f 7239 0000 0072 3a00 0000  _doc__r9...r:...
-00003f80: da07 6e75 6d62 6572 73da 064e 756d 6265  ..numbers..Numbe
-00003f90: 72da 046c 6973 7472 0500 0000 7219 0000  r..listr....r...
-00003fa0: 0072 2500 0000 721e 0000 00da 0a53 6361  .r%...r......Sca
-00003fb0: 6c61 7254 7970 6572 3200 0000 7236 0000  larTyper2...r6..
-00003fc0: 0072 3300 0000 da06 7479 7069 6e67 da08  .r3.....typing..
-00003fd0: 4f70 7469 6f6e 616c da07 4e44 4172 7261  Optional..NDArra
-00003fe0: 7972 3800 0000 7229 0000 0072 4300 0000  yr8...r)...rC...
-00003ff0: 723d 0000 00da 0b63 6c61 7373 6d65 7468  r=.....classmeth
-00004000: 6f64 da08 4361 6c6c 6162 6c65 721c 0000  od..Callabler...
-00004010: 0072 1d00 0000 da04 4469 6374 da03 7374  .r......Dict..st
-00004020: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
-00004030: 5f5f 7257 0000 0072 0b00 0000 7214 0000  __rW...r....r...
-00004040: 0072 1200 0000 7208 0000 0072 0800 0000  .r....r....r....
-00004050: 1000 0000 736f 0100 0080 0080 0080 0080  ....so..........
-00004060: 0080 0080 00f0 0222 0508 f000 2205 08f0  ......."...."...
-00004070: 4a01 0009 0e8c 0dd8 080f 8c0e d808 0cd8  J...............
-00004080: 080e f009 0514 0680 4cf0 0e25 0541 01f0  ........L..%.A..
-00004090: 0025 0541 01f0 0025 0541 01f0 4e01 2105  .%.A...%.A..N.!.
-000040a0: 18f0 0021 0518 f000 2105 18f0 4801 0009  ...!....!...H...
-000040b0: 0e8c 0dd8 080e f005 0317 06f0 0600 090d  ................
-000040c0: 8804 8855 d40d 1dd1 081e d408 1ef1 0703  ...U............
-000040d0: 171f 804f f00a 2205 3ff0 0022 053f f000  ...O..".?..".?..
-000040e0: 2205 3ff0 4801 2405 4301 f000 2405 4301  ".?.H.$.C...$.C.
-000040f0: f000 2405 4301 f04c 010c 050f a026 a42f  ..$.C..L.....&./
-00004100: b025 b42c d432 46d4 2247 f000 0c05 0ff0  .%.,.2F."G......
-00004110: 000c 050f f000 0c05 0ff0 000c 050f f01c  ................
-00004120: 0705 3ef0 0007 053e f000 0705 3ef0 1212  ..>....>....>...
-00004130: 0513 f000 1205 13f0 0012 0513 f028 0d05  .............(..
-00004140: 0af0 000d 050a f000 0d05 0af0 1e00 0611  ................
-00004150: f002 0a05 16a0 46a4 4ff0 000a 0516 f000  ......F.O.......
-00004160: 0a05 16f0 000a 0516 f103 0006 1184 5bf0  ..............[.
-00004170: 020a 0516 f018 0033 3780 4a90 0694 0b98  .......37.J.....
-00004180: 43a0 16a4 1fd0 1c30 d410 31d0 0436 d004  C......0..1..6..
-00004190: 36d1 0436 d804 49e0 0510 f002 3705 19a8  6..6..I.....7...
-000041a0: 06ac 0ff0 0037 0519 f000 3705 19f0 0037  .....7....7....7
-000041b0: 0519 f103 0006 1184 5bf0 0237 0519 f000  ........[..7....
-000041c0: 3705 19f0 0037 0519 7214 0000 0072 0800  7....7..r....r..
-000041d0: 0000 6300 0000 0000 0000 0000 0000 0005  ..c.............
-000041e0: 0000 0000 0000 00f3 dc00 0000 8700 9700  ................
-000041f0: 6500 5a01 6400 5a02 5500 6401 5a03 6402  e.Z.d.Z.U.d.Z.d.
-00004200: 8400 5a04 6505 6403 6506 6a07 0000 0000  ..Z.e.d.e.j.....
-00004210: 0000 0000 6508 6506 6a09 0000 0000 0000  ....e.e.j.......
-00004220: 0000 6602 1900 0000 0000 0000 0000 6602  ..f...........f.
-00004230: 8800 6601 6404 840c a600 0000 ab00 0000  ..f.d...........
-00004240: 0000 0000 0000 5a0a 6405 5a0b 6506 6a0c  ......Z.d.Z.e.j.
-00004250: 0000 0000 0000 0000 6508 6506 6a09 0000  ........e.e.j...
-00004260: 0000 0000 0000 6602 1900 0000 0000 0000  ......f.........
-00004270: 0000 650d 6406 3c00 0000 0900 6505 6403  ..e.d.<.....e.d.
-00004280: 6506 6a07 0000 0000 0000 0000 6508 6506  e.j.........e.e.
-00004290: 6a09 0000 0000 0000 0000 6602 1900 0000  j.........f.....
-000042a0: 0000 0000 0000 6602 8800 6601 6407 840c  ......f...f.d...
-000042b0: a600 0000 ab00 0000 0000 0000 0000 5a0e  ..............Z.
-000042c0: 8800 7801 5a0f 5300 2908 da09 4f70 6572  ..x.Z.S.)...Oper
-000042d0: 6174 6f72 737a 3253 7570 706f 7274 2066  atorsz2Support f
-000042e0: 6f72 2069 6d70 6c65 6d65 6e74 696e 6720  or implementing 
-000042f0: 6375 7374 6f6d 206e 756d 6572 6963 206f  custom numeric o
-00004300: 7065 7261 746f 7273 2e63 0200 0000 0000  perators.c......
-00004310: 0000 0000 0000 0500 0000 0f00 0000 f388  ................
-00004320: 0000 0097 007c 00a0 0000 0000 0000 0000  .....|..........
-00004330: 0000 0000 0000 0000 0000 0000 007c 01a6  .............|..
-00004340: 0100 00ab 0100 0000 0000 0000 0072 277c  .............r'|
-00004350: 006a 0100 0000 0000 0000 0074 0500 0000  .j.........t....
-00004360: 0000 0000 0000 006a 0300 0000 0000 0000  .......j........
-00004370: 007c 01a6 0100 00ab 0100 0000 0000 0000  .|..............
-00004380: 0019 0000 0000 0000 0000 007d 0402 007c  ...........}...|
-00004390: 047c 0269 007c 03a4 018e 0153 0074 0800  .|.i.|.....S.t..
-000043a0: 0000 0000 0000 0000 0053 0029 0161 b601  .........S.).a..
-000043b0: 0000 4170 706c 7920 606f 7065 7261 7469  ..Apply `operati
-000043c0: 6f6e 6020 746f 2074 6865 2067 6976 656e  on` to the given
-000043d0: 2061 7267 756d 656e 7473 2e0a 0a20 2020   arguments...   
-000043e0: 2020 2020 204e 6f74 6573 0a20 2020 2020       Notes.     
-000043f0: 2020 202d 2d2d 2d2d 0a20 2020 2020 2020     -----.       
-00004400: 202d 2054 6869 7320 6d65 7468 6f64 2069   - This method i
-00004410: 7320 6261 7365 6420 6f6e 2074 6865 206d  s based on the m
-00004420: 6574 686f 6473 2060 7e5f 5f61 7272 6179  ethods `~__array
-00004430: 5f75 6675 6e63 5f5f 6020 616e 640a 2020  _ufunc__` and.  
-00004440: 2020 2020 2020 2020 607e 5f5f 6172 7261          `~__arra
-00004450: 795f 6675 6e63 7469 6f6e 5f5f 602c 2077  y_function__`, w
-00004460: 6869 6368 2073 7570 706f 7274 2063 7573  hich support cus
-00004470: 746f 6d20 696d 706c 656d 656e 7461 7469  tom implementati
-00004480: 6f6e 7320 6f66 2060 6e75 6d70 7960 0a20  ons of `numpy`. 
-00004490: 2020 2020 2020 2020 2075 6e69 7665 7273           univers
-000044a0: 616c 2066 756e 6374 696f 6e73 2061 6e64  al functions and
-000044b0: 2070 7562 6c69 6320 6675 6e63 7469 6f6e   public function
-000044c0: 732c 2072 6573 7065 6374 6976 656c 792e  s, respectively.
-000044d0: 0a20 2020 2020 2020 202d 2054 6865 206e  .        - The n
-000044e0: 616d 6520 6f66 2074 6869 7320 6d65 7468  ame of this meth
-000044f0: 6f64 2069 7320 7375 626a 6563 7420 746f  od is subject to
-00004500: 2063 6861 6e67 6520 7769 7468 6f75 7420   change without 
-00004510: 6e6f 7469 6365 2069 6e20 7468 650a 2020  notice in the.  
-00004520: 2020 2020 2020 2020 6576 656e 7420 7468          event th
-00004530: 6174 2069 7420 636f 6e66 6c69 6374 7320  at it conflicts 
-00004540: 7769 7468 2061 2073 7461 6e64 6172 642d  with a standard-
-00004550: 6c69 6272 6172 7920 6d65 7468 6f64 2e0a  library method..
-00004560: 2020 2020 2020 2020 2905 721c 0000 00da          ).r.....
-00004570: 0a5f 4f50 4552 4154 4f52 5372 0400 0000  ._OPERATORSr....
-00004580: da07 7265 736f 6c76 6572 1b00 0000 2905  ..resolver....).
-00004590: 721f 0000 0072 4900 0000 7222 0000 0072  r....rI...r"...r
-000045a0: 2300 0000 7224 0000 0073 0500 0000 2020  #...r$...s....  
-000045b0: 2020 2072 1200 0000 da13 5f5f 6f62 6a65     r......__obje
-000045c0: 6374 5f6f 7065 7261 746f 725f 5f7a 1d4f  ct_operator__z.O
-000045d0: 7065 7261 746f 7273 2e5f 5f6f 626a 6563  perators.__objec
-000045e0: 745f 6f70 6572 6174 6f72 5f5f 5d01 0000  t_operator__]...
-000045f0: 734c 0000 0080 00f0 1600 0c10 d70b 1bd2  sL..............
-00004600: 0b1b 9849 d10b 26d4 0b26 f000 0209 2dd8  ...I..&..&....-.
-00004610: 171b 947f a57b d427 3ab8 39d1 2745 d427  .....{.':.9.'E.'
-00004620: 45d4 1746 8848 d813 1b90 3898 54d0 132c  E..F.H....8.T..,
-00004630: a056 d013 2cd0 132c d00c 2cdd 0f1d d008  .V..,..,..,.....
-00004640: 1d72 1400 0000 7249 0000 0063 0200 0000  .r....rI...c....
-00004650: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-00004660: f3ae 0000 0095 0197 0074 0100 0000 0000  .........t......
-00004670: 0000 0000 006a 0100 0000 0000 0000 007c  .....j.........|
-00004680: 01a6 0100 00ab 0100 0000 0000 0000 007d  ...............}
-00004690: 027c 0280 2174 0500 0000 0000 0000 0000  .|..!t..........
-000046a0: 00a6 0000 00ab 0000 0000 0000 0000 00a0  ................
-000046b0: 0300 0000 0000 0000 0000 0000 0000 0000  ................
-000046c0: 0000 0000 007c 01a6 0100 00ab 0100 0000  .....|..........
-000046d0: 0000 0000 0053 0009 007c 027c 006a 0400  .....S...|.|.j..
-000046e0: 0000 0000 0000 0076 007d 036e 1123 0074  .......v.}.n.#.t
-000046f0: 0a00 0000 0000 0000 0000 0024 0072 0401  ...........$.r..
-00004700: 0059 0064 0253 0077 0078 0359 0077 017c  .Y.d.S.w.x.Y.w.|
-00004710: 0353 0029 0372 4b00 0000 4e46 2906 7204  .S.).rK...NF).r.
-00004720: 0000 0072 6b00 0000 da05 7375 7065 7272  ...rk.....superr
-00004730: 1c00 0000 726a 0000 0072 2a00 0000 2905  ....rj...r*...).
-00004740: 724c 0000 0072 4900 0000 da06 7461 7267  rL...rI.....targ
-00004750: 6574 724d 0000 0072 3b00 0000 7305 0000  etrM...r;...s...
-00004760: 0020 2020 2080 7212 0000 0072 1c00 0000  .    .r....r....
-00004770: 7a15 4f70 6572 6174 6f72 732e 5f69 6d70  z.Operators._imp
-00004780: 6c65 6d65 6e74 736d 0100 0073 6c00 0000  lementsm...sl...
-00004790: f880 00f5 0e00 121d d411 24a0 59d1 112f  ..........$.Y../
-000047a0: d411 2f88 06d8 0b11 883e dd13 1891 3794  ../......>....7.
-000047b0: 37d7 1326 d213 26a0 79d1 1331 d413 31d0  7..&..&.y..1..1.
-000047c0: 0c31 f002 0309 19d8 151b 9873 9c7e d015  .1.........s.~..
-000047d0: 2d88 4688 46f8 dd0f 18f0 0001 0919 f000  -.F.F...........
-000047e0: 0109 19f0 0001 0919 d813 1890 3590 35f0  ............5.5.
-000047f0: 0301 0919 f8f8 f8e0 0f15 880d 7311 0000  ............s...
-00004800: 00ba 0941 0400 c104 0a41 1203 c111 0141  ...A.....A.....A
-00004810: 1203 4e72 6a00 0000 6302 0000 0000 0000  ..Nrj...c.......
-00004820: 0000 0000 0003 0000 0003 0000 00f3 d200  ................
-00004830: 0000 9501 8700 8703 9700 7401 0000 0000  ..........t.....
-00004840: 0000 0000 0000 6a01 0000 0000 0000 0000  ......j.........
-00004850: 7c01 a601 0000 ab01 0000 0000 0000 0000  |...............
-00004860: 8a03 8903 7400 0000 0000 0000 0000 0000  ....t...........
-00004870: 6a02 0000 0000 0000 0000 a003 0000 0000  j...............
-00004880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004890: a600 0000 ab00 0000 0000 0000 0000 7601  ..............v.
-000048a0: 7221 7409 0000 0000 0000 0000 0000 a600  r!t.............
-000048b0: 0000 ab00 0000 0000 0000 0000 a005 0000  ................
-000048c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000048d0: 0000 7c01 a601 0000 ab01 0000 0000 0000  ..|.............
-000048e0: 0000 5300 6401 740c 0000 0000 0000 0000  ..S.d.t.........
-000048f0: 0000 6602 8800 8803 6602 6402 840c 7d02  ..f.....f.d...}.
-00004900: 7c02 5300 2903 610a 0200 0052 6567 6973  |.S.).a....Regis
-00004910: 7465 7220 6120 6375 7374 6f6d 2069 6d70  ter a custom imp
-00004920: 6c65 6d65 6e74 6174 696f 6e20 6f66 2060  lementation of `
-00004930: 6f70 6572 6174 696f 6e60 2e0a 0a20 2020  operation`...   
-00004940: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00004950: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00004960: 2d2d 0a20 2020 2020 2020 206f 7065 7261  --.        opera
-00004970: 7469 6f6e 203a 2073 7472 696e 6720 6f72  tion : string or
-00004980: 2063 616c 6c61 626c 650a 2020 2020 2020   callable.      
-00004990: 2020 2020 2020 5468 6520 6f70 6572 6174        The operat
-000049a0: 696f 6e20 746f 2069 6d70 6c65 6d65 6e74  ion to implement
-000049b0: 2e20 5468 6520 6172 6775 6d65 6e74 206d  . The argument m
-000049c0: 6179 2062 6520 7468 6520 6361 6e6f 6e69  ay be the canoni
-000049d0: 6361 6c0a 2020 2020 2020 2020 2020 2020  cal.            
-000049e0: 6361 6c6c 6162 6c65 206f 626a 6563 7420  callable object 
-000049f0: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
-00004a00: 2074 6865 2074 6172 6765 7420 6f70 6572   the target oper
-00004a10: 6174 696f 6e20 2865 2e67 2e2c 0a20 2020  ation (e.g.,.   
-00004a20: 2020 2020 2020 2020 2060 6e75 6d70 792e           `numpy.
-00004a30: 6164 6460 206f 7220 606f 7065 7261 746f  add` or `operato
-00004a40: 722e 6164 6460 292c 206f 7220 6120 6b6e  r.add`), or a kn
-00004a50: 6f77 6e20 616c 6961 7320 666f 7220 7468  own alias for th
-00004a60: 6520 6f70 6572 6174 696f 6e0a 2020 2020  e operation.    
-00004a70: 2020 2020 2020 2020 2865 2e67 2e2c 2060          (e.g., `
-00004a80: 2761 6464 2760 292e 0a0a 2020 2020 2020  'add'`)...      
-00004a90: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00004aa0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00004ab0: 2020 6074 7970 696e 672e 4361 6c6c 6162    `typing.Callab
-00004ac0: 6c65 600a 2020 2020 2020 2020 2020 2020  le`.            
-00004ad0: 4120 6675 6e63 7469 6f6e 2077 6974 6820  A function with 
-00004ae0: 7768 6963 6820 746f 2064 6563 6f72 6174  which to decorat
-00004af0: 6520 7468 6520 6375 7374 6f6d 2069 6d70  e the custom imp
-00004b00: 6c65 6d65 6e74 6174 696f 6e2e 0a20 2020  lementation..   
-00004b10: 2020 2020 2072 5000 0000 6301 0000 0000       rP...c.....
-00004b20: 0000 0000 0000 0005 0000 0013 0000 00f3  ................
-00004b30: 5200 0000 9502 9700 8901 6a00 0000 0000  R.........j.....
-00004b40: 0000 0000 8014 7403 0000 0000 0000 0000  ......t.........
-00004b50: 0000 6401 8901 9b00 6402 9d03 a601 0000  ..d.....d.......
-00004b60: ab01 0000 0000 0000 0000 6400 8202 7c00  ..........d...|.
-00004b70: 8901 6a00 0000 0000 0000 0000 8902 3c00  ..j...........<.
-00004b80: 0000 7c00 5300 2903 4e72 5200 0000 7a22  ..|.S.).NrR...z"
-00004b90: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-00004ba0: 7420 6375 7374 6f6d 206f 7065 7261 746f  t custom operato
-00004bb0: 7273 2902 726a 0000 0072 5300 0000 2903  rs).rj...rS...).
-00004bc0: 7250 0000 0072 4c00 0000 726f 0000 0073  rP...rL...ro...s
-00004bd0: 0300 0000 2080 8072 1200 0000 7254 0000  .... ..r....rT..
-00004be0: 007a 274f 7065 7261 746f 7273 2e69 6d70  .z'Operators.imp
-00004bf0: 6c65 6d65 6e74 732e 3c6c 6f63 616c 733e  lements.<locals>
-00004c00: 2e64 6563 6f72 6174 6f72 9401 0000 7342  .decorator....sB
-00004c10: 0000 00f8 8000 d80f 128c 7ed0 0f25 dd16  ..........~..%..
-00004c20: 29d8 1443 9843 d014 43d0 1443 d014 43f1  )..C.C..C..C..C.
-00004c30: 0302 1712 f400 0217 12e0 171b f005 0211  ................
-00004c40: 1cf0 0600 2633 8843 8c4e 9836 d10c 22d8  ....&3.C.N.6..".
-00004c50: 1320 d00c 2072 1400 0000 2907 7204 0000  . .. r....).r...
-00004c60: 0072 6b00 0000 da09 4655 4e43 5449 4f4e  .rk.....FUNCTION
-00004c70: 5372 2b00 0000 726e 0000 0072 5700 0000  Sr+...rn...rW...
-00004c80: 7256 0000 0029 0572 4c00 0000 7249 0000  rV...).rL...rI..
-00004c90: 0072 5400 0000 726f 0000 0072 3b00 0000  .rT...ro...r;...
-00004ca0: 7305 0000 0060 2020 4080 7212 0000 0072  s....`  @.r....r
-00004cb0: 5700 0000 7a14 4f70 6572 6174 6f72 732e  W...z.Operators.
-00004cc0: 696d 706c 656d 656e 7473 8001 0000 737b  implements....s{
-00004cd0: 0000 00f8 f8f8 8000 f522 0012 1dd4 1124  .........".....$
-00004ce0: a059 d111 2fd4 112f 8806 d80b 119d 1bd4  .Y../../........
-00004cf0: 192e d719 35d2 1935 d119 37d4 1937 d00b  ....5..5..7..7..
-00004d00: 37d0 0b37 dd13 1891 3794 37d7 1325 d213  7..7....7.7..%..
-00004d10: 25a0 69d1 1330 d413 30d0 0c30 f002 0609  %.i..0..0..0....
-00004d20: 21a5 5cf0 0006 0921 f000 0609 21f0 0006  !.\....!....!...
-00004d30: 0921 f000 0609 21f0 0006 0921 f000 0609  .!....!....!....
-00004d40: 21f0 0006 0921 f00e 0010 19d0 0818 7214  !....!........r.
-00004d50: 0000 0029 1072 5800 0000 7259 0000 0072  ...).rX...rY...r
-00004d60: 3c00 0000 725a 0000 0072 6c00 0000 7262  <...rZ...rl...rb
-00004d70: 0000 0072 5f00 0000 da05 556e 696f 6e72  ...r_.....Unionr
-00004d80: 6500 0000 7263 0000 0072 1c00 0000 726a  e...rc...r....rj
-00004d90: 0000 0072 6400 0000 7266 0000 0072 5700  ...rd...rf...rW.
-00004da0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00004db0: 5f29 0172 3b00 0000 7301 0000 0040 7212  _).r;...s....@r.
-00004dc0: 0000 0072 6800 0000 7268 0000 005a 0100  ...rh...rh...Z..
-00004dd0: 0073 d500 0000 f880 0080 0080 0080 0080  .s..............
-00004de0: 0080 00d8 043c d004 3cf0 040e 051e f000  .....<..<.......
-00004df0: 0e05 1ef0 000e 051e f020 0006 11f0 020d  ......... ......
-00004e00: 0516 a046 a44c b013 b066 b46f d031 45d4  ...F.L...f.o.1E.
-00004e10: 2446 f000 0d05 16f0 000d 0516 f000 0d05  $F..............
-00004e20: 16f0 000d 0516 f000 0d05 16f1 0300 0611  ................
-00004e30: 845b f002 0d05 16f0 1e00 3337 804a 9006  .[........37.J..
-00004e40: 940b 9843 a016 a41f d01c 30d4 1031 d004  ...C......0..1..
-00004e50: 36d0 0436 d104 36d8 044a e005 10f0 021a  6..6..6..J......
-00004e60: 0519 a036 a43c b003 b056 b45f d030 44d4  ...6.<...V._.0D.
-00004e70: 2345 f000 1a05 19f0 001a 0519 f000 1a05  #E..............
-00004e80: 19f0 001a 0519 f000 1a05 19f1 0300 0611  ................
-00004e90: 845b f002 1a05 19f0 001a 0519 f000 1a05  .[..............
-00004ea0: 19f0 001a 0519 f000 1a05 1972 1400 0000  ...........r....
-00004eb0: 7268 0000 0029 0e72 5b00 0000 725f 0000  rh...).r[...r_..
-00004ec0: 0072 3900 0000 da0c 6e75 6d70 792e 7479  .r9.....numpy.ty
-00004ed0: 7069 6e67 da00 7204 0000 00da 085f 6f62  ping..r......_ob
-00004ee0: 6a65 6374 7372 0500 0000 da07 5479 7065  jectsr......Type
-00004ef0: 5661 7272 0600 0000 7263 0000 0072 5600  Varr....rc...rV.
-00004f00: 0000 7208 0000 0072 6800 0000 720b 0000  ..r....rh...r...
-00004f10: 0072 1400 0000 7212 0000 00fa 083c 6d6f  .r....r......<mo
-00004f20: 6475 6c65 3e72 7900 0000 0100 0000 73e2  dule>ry.......s.
-00004f30: 0000 00f0 0301 0101 d800 0e80 0e80 0e80  ................
-00004f40: 0ed8 000d 800d 800d 800d e000 0c80 0c80  ................
-00004f50: 0c80 0cd8 0013 d000 13d0 0013 d000 13e0  ................
-00004f60: 0019 d000 19d0 0019 d000 19d0 0019 d000  ................
-00004f70: 19d8 001c d000 1cd0 001c d000 1cd0 001c  ................
-00004f80: d000 1cf0 0600 0513 8046 844e 9033 d104  .........F.N.3..
-00004f90: 17d4 0417 8001 e00f 158c 7f98 73a0 4198  ............s.A.
-00004fa0: 76d4 0f26 800c f006 4705 0119 f000 4705  v..&....G.....G.
-00004fb0: 0119 f000 4705 0119 f000 4705 0119 f000  ....G.....G.....
-00004fc0: 4705 0119 f100 4705 0119 f400 4705 0119  G.....G.....G...
-00004fd0: f000 4705 0119 f054 0a41 0101 19f0 0041  ..G....T.A.....A
-00004fe0: 0101 19f0 0041 0101 19f0 0041 0101 19f0  .....A.....A....
-00004ff0: 0041 0101 1990 09f1 0041 0101 19f4 0041  .A.......A.....A
-00005000: 0101 19f0 0041 0101 19f0 0041 0101 19f0  .....A.....A....
-00005010: 0041 0101 1972 1400 0000                 .A...r....
+00000000: 696d 706f 7274 206e 756d 6265 7273 0a69  import numbers.i
+00000010: 6d70 6f72 7420 7479 7069 6e67 0a0a 696d  mport typing..im
+00000020: 706f 7274 206e 756d 7079 0a69 6d70 6f72  port numpy.impor
+00000030: 7420 6e75 6d70 792e 7479 7069 6e67 0a0a  t numpy.typing..
+00000040: 6672 6f6d 202e 2069 6d70 6f72 7420 5f6f  from . import _o
+00000050: 7065 7261 7469 6f6e 730a 6672 6f6d 202e  perations.from .
+00000060: 5f6f 626a 6563 7473 2069 6d70 6f72 7420  _objects import 
+00000070: 4f62 6a65 6374 0a0a 0a54 203d 2074 7970  Object...T = typ
+00000080: 696e 672e 5479 7065 5661 7228 2754 2729  ing.TypeVar('T')
+00000090: 0a0a 5573 6572 4675 6e63 7469 6f6e 203d  ..UserFunction =
+000000a0: 2074 7970 696e 672e 4361 6c6c 6162 6c65   typing.Callable
+000000b0: 5b2e 2e2e 2c20 545d 0a0a 0a63 6c61 7373  [..., T]...class
+000000c0: 2046 756e 6374 696f 6e73 3a0a 2020 2020   Functions:.    
+000000d0: 2222 224d 6978 696e 2066 6f72 2061 6464  """Mixin for add
+000000e0: 696e 6720 7375 7070 6f72 7420 666f 7220  ing support for 
+000000f0: 606e 756d 7079 6020 6675 6e63 7469 6f6e  `numpy` function
+00000100: 7320 746f 206e 756d 6572 6963 206f 626a  s to numeric obj
+00000110: 6563 7473 2e0a 2020 2020 0a20 2020 2043  ects..    .    C
+00000120: 6c61 7373 6573 2074 6861 7420 696e 6865  lasses that inhe
+00000130: 7269 7420 6672 6f6d 2074 6869 7320 636c  rit from this cl
+00000140: 6173 7320 6d61 7920 696d 706c 656d 656e  ass may implemen
+00000150: 7420 7375 7070 6f72 7420 666f 7220 606e  t support for `n
+00000160: 756d 7079 600a 2020 2020 756e 6976 6572  umpy`.    univer
+00000170: 7361 6c20 6675 6e63 7469 6f6e 7320 2822  sal functions ("
+00000180: 7566 756e 6373 223b 2065 2e67 2e2c 2060  ufuncs"; e.g., `
+00000190: 6e75 6d70 792e 7371 7274 6029 2062 7920  numpy.sqrt`) by 
+000001a0: 6f76 6572 6c6f 6164 696e 670a 2020 2020  overloading.    
+000001b0: 605f 6170 706c 795f 7566 756e 6360 2c20  `_apply_ufunc`, 
+000001c0: 616e 6420 6d61 7920 696d 706c 656d 656e  and may implemen
+000001d0: 7420 7375 7070 6f72 7420 666f 7220 606e  t support for `n
+000001e0: 756d 7079 6020 7075 626c 6963 2066 756e  umpy` public fun
+000001f0: 6374 696f 6e73 0a20 2020 2028 652e 672e  ctions.    (e.g.
+00000200: 2c20 606e 756d 7079 2e73 7175 6565 7a65  , `numpy.squeeze
+00000210: 6029 2062 7920 6f76 6572 6c6f 6164 696e  `) by overloadin
+00000220: 6720 605f 6170 706c 795f 6675 6e63 7469  g `_apply_functi
+00000230: 6f6e 6020 616e 6420 7265 6769 7374 6572  on` and register
+00000240: 696e 670a 2020 2020 696e 6469 7669 6475  ing.    individu
+00000250: 616c 2066 756e 6374 696f 6e20 696d 706c  al function impl
+00000260: 656d 656e 7461 7469 6f6e 7320 7669 6120  ementations via 
+00000270: 6069 6d70 6c65 6d65 6e74 7360 2e0a 0a20  `implements`... 
+00000280: 2020 2049 7420 6973 2069 6d70 6f72 7461     It is importa
+00000290: 6e74 2074 6f20 6e6f 7465 2074 6861 7420  nt to note that 
+000002a0: 7468 6520 7573 6520 6361 7365 7320 6f66  the use cases of
+000002b0: 2074 6869 7320 636c 6173 7320 6578 7465   this class exte
+000002c0: 6e64 2062 6579 6f6e 640a 2020 2020 6172  nd beyond.    ar
+000002d0: 7261 792d 6c69 6b65 206f 626a 6563 7473  ray-like objects
+000002e0: 2e20 426f 7468 2073 696e 676c 652d 2061  . Both single- a
+000002f0: 6e64 206d 756c 7469 2d76 616c 7565 6420  nd multi-valued 
+00000300: 6f62 6a65 6374 7320 6361 6e20 6265 6e65  objects can bene
+00000310: 6669 7420 6672 6f6d 0a20 2020 2069 6d70  fit from.    imp
+00000320: 6c65 6d65 6e74 696e 6720 7375 7070 6f72  lementing suppor
+00000330: 7420 666f 7220 606e 756d 7079 6020 756e  t for `numpy` un
+00000340: 6976 6572 7361 6c20 616e 6420 7075 626c  iversal and publ
+00000350: 6963 2066 756e 6374 696f 6e73 2e20 466f  ic functions. Fo
+00000360: 720a 2020 2020 6578 616d 706c 652c 2069  r.    example, i
+00000370: 7420 706f 7373 6962 6c65 2074 6f20 6170  t possible to ap
+00000380: 706c 7920 606e 756d 7079 2e73 7172 7460  ply `numpy.sqrt`
+00000390: 2074 6f20 6569 7468 6572 2061 2072 6561   to either a rea
+000003a0: 6c20 6e75 6d62 6572 206f 7220 616e 0a20  l number or an. 
+000003b0: 2020 2061 7272 6179 0a0a 2020 2020 3e3e     array..    >>
+000003c0: 3e20 6e75 6d70 792e 7371 7274 2834 290a  > numpy.sqrt(4).
+000003d0: 2020 2020 322e 300a 2020 2020 3e3e 3e20      2.0.    >>> 
+000003e0: 6e75 6d70 792e 7371 7274 285b 342c 2039  numpy.sqrt([4, 9
+000003f0: 5d29 0a20 2020 2061 7272 6179 285b 322e  ]).    array([2.
+00000400: 2c20 332e 5d29 0a0a 2020 2020 4576 656e  , 3.])..    Even
+00000410: 2074 6865 2074 7269 7669 616c 2061 7070   the trivial app
+00000420: 6c69 6361 7469 6f6e 206f 6620 606e 756d  lication of `num
+00000430: 7079 2e6d 6561 6e60 2074 6f20 6120 7265  py.mean` to a re
+00000440: 616c 206e 756d 6265 7220 6973 2064 6566  al number is def
+00000450: 696e 6564 3a0a 0a20 2020 203e 3e3e 206e  ined:..    >>> n
+00000460: 756d 7079 2e6d 6561 6e28 322e 3529 0a20  umpy.mean(2.5). 
+00000470: 2020 2032 2e35 0a0a 2020 2020 4e6f 7465     2.5..    Note
+00000480: 730a 2020 2020 2d2d 2d2d 2d0a 2020 2020  s.    -----.    
+00000490: 2d20 5468 6973 2063 6c61 7373 2064 6f65  - This class doe
+000004a0: 7320 6e6f 7420 696e 6865 7269 7420 6672  s not inherit fr
+000004b0: 6f6d 2060 6e75 6d70 792e 6c69 622e 6d69  om `numpy.lib.mi
+000004c0: 7869 6e73 2e4e 4441 7272 6179 4f70 6572  xins.NDArrayOper
+000004d0: 6174 6f72 734d 6978 696e 602c 0a20 2020  atorsMixin`,.   
+000004e0: 2020 2077 6869 6368 2069 6d70 6c65 6d65     which impleme
+000004f0: 6e74 7320 6d6f 7374 206f 6620 7468 6520  nts most of the 
+00000500: 6275 696c 742d 696e 2050 7974 686f 6e20  built-in Python 
+00000510: 6e75 6d65 7269 6320 6f70 6572 6174 6f72  numeric operator
+00000520: 7320 7669 610a 2020 2020 2020 605f 5f61  s via.      `__a
+00000530: 7272 6179 5f75 6675 6e63 5f5f 602c 2062  rray_ufunc__`, b
+00000540: 6563 6175 7365 2069 7420 6173 7375 6d65  ecause it assume
+00000550: 7320 7468 6174 2073 7562 636c 6173 7365  s that subclasse
+00000560: 7320 696e 6465 7065 6e64 656e 746c 790a  s independently.
+00000570: 2020 2020 2020 696d 706c 656d 656e 7420        implement 
+00000580: 7468 6520 7265 616c 2d76 616c 7565 6420  the real-valued 
+00000590: 7072 6f74 6f63 6f6c 2e20 496e 2066 6163  protocol. In fac
+000005a0: 742c 0a20 2020 2020 2060 6e75 6d70 792e  t,.      `numpy.
+000005b0: 6c69 622e 6d69 7869 6e73 2e4e 4441 7272  lib.mixins.NDArr
+000005c0: 6179 4f70 6572 6174 6f72 734d 6978 696e  ayOperatorsMixin
+000005d0: 6020 6465 6669 6e65 7320 6d75 6c74 6970  ` defines multip
+000005e0: 6c65 206f 7065 7261 746f 7273 2074 6861  le operators tha
+000005f0: 740a 2020 2020 2020 6172 6520 6e6f 7420  t.      are not 
+00000600: 7061 7274 206f 6620 7468 6520 7265 616c  part of the real
+00000610: 2d76 616c 7565 6420 7072 6f74 6f63 6f6c  -valued protocol
+00000620: 2e20 486f 7765 7665 722c 2073 6565 0a20  . However, see. 
+00000630: 2020 2020 2068 7474 7073 3a2f 2f6e 756d       https://num
+00000640: 7079 2e6f 7267 2f64 6f63 2f73 7461 626c  py.org/doc/stabl
+00000650: 652f 7265 6665 7265 6e63 652f 6765 6e65  e/reference/gene
+00000660: 7261 7465 642f 6e75 6d70 792e 6c69 622e  rated/numpy.lib.
+00000670: 6d69 7869 6e73 2e4e 4441 7272 6179 4f70  mixins.NDArrayOp
+00000680: 6572 6174 6f72 734d 6978 696e 2e68 746d  eratorsMixin.htm
+00000690: 6c23 6e75 6d70 792e 6c69 622e 6d69 7869  l#numpy.lib.mixi
+000006a0: 6e73 2e4e 4441 7272 6179 4f70 6572 6174  ns.NDArrayOperat
+000006b0: 6f72 734d 6978 696e 0a20 2020 2020 2066  orsMixin.      f
+000006c0: 6f72 2061 6e20 6578 616d 706c 6520 6f66  or an example of
+000006d0: 2068 6f77 206f 6e65 206d 6967 6874 2075   how one might u
+000006e0: 7365 2074 6861 7420 6d69 7869 6e20 636c  se that mixin cl
+000006f0: 6173 732e 0a20 2020 2022 2222 0a0a 2020  ass..    """..  
+00000700: 2020 5f55 4655 4e43 5f54 5950 4553 203d    _UFUNC_TYPES =
+00000710: 205b 0a20 2020 2020 2020 206e 756d 7079   [.        numpy
+00000720: 2e6e 6461 7272 6179 2c0a 2020 2020 2020  .ndarray,.      
+00000730: 2020 6e75 6d62 6572 732e 4e75 6d62 6572    numbers.Number
+00000740: 2c0a 2020 2020 2020 2020 6c69 7374 2c0a  ,.        list,.
+00000750: 2020 2020 2020 2020 4f62 6a65 6374 2c0a          Object,.
+00000760: 2020 2020 5d0a 0a20 2020 2064 6566 205f      ]..    def _
+00000770: 5f61 7272 6179 5f75 6675 6e63 5f5f 2873  _array_ufunc__(s
+00000780: 656c 662c 2075 6675 6e63 2c20 6d65 7468  elf, ufunc, meth
+00000790: 6f64 2c20 2a61 7267 732c 202a 2a6b 7761  od, *args, **kwa
+000007a0: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
+000007b0: 2250 726f 7669 6465 2073 7570 706f 7274  "Provide support
+000007c0: 2066 6f72 2060 6e75 6d70 7960 2075 6e69   for `numpy` uni
+000007d0: 7665 7273 616c 2066 756e 6374 696f 6e73  versal functions
+000007e0: 2e0a 0a20 2020 2020 2020 2053 6565 2068  ...        See h
+000007f0: 7474 7073 3a2f 2f6e 756d 7079 2e6f 7267  ttps://numpy.org
+00000800: 2f64 6f63 2f73 7461 626c 652f 7265 6665  /doc/stable/refe
+00000810: 7265 6e63 652f 6172 7261 7973 2e63 6c61  rence/arrays.cla
+00000820: 7373 6573 2e68 746d 6c20 666f 7220 6d6f  sses.html for mo
+00000830: 7265 0a20 2020 2020 2020 2069 6e66 6f72  re.        infor
+00000840: 6d61 7469 6f6e 206f 6e20 7573 6520 6f66  mation on use of
+00000850: 2074 6869 7320 7370 6563 6961 6c20 6d65   this special me
+00000860: 7468 6f64 2e0a 0a20 2020 2020 2020 204e  thod...        N
+00000870: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+00000880: 2d2d 0a20 2020 2020 2020 202d 2054 6869  --.        - Thi
+00000890: 7320 6d65 7468 6f64 2066 6972 7374 2065  s method first e
+000008a0: 6e73 7572 6573 2074 6861 7420 7468 6520  nsures that the 
+000008b0: 696e 7075 7420 7479 7065 7320 2861 7320  input types (as 
+000008c0: 7765 6c6c 2061 7320 7468 6520 7479 7065  well as the type
+000008d0: 206f 660a 2020 2020 2020 2020 2020 606f   of.          `o
+000008e0: 7574 602c 2069 6620 7061 7373 6564 2076  ut`, if passed v
+000008f0: 6961 206b 6579 776f 7264 2920 6172 6520  ia keyword) are 
+00000900: 7375 7070 6f72 7465 6420 7479 7065 732e  supported types.
+00000910: 2049 7420 7468 656e 2063 6865 636b 7320   It then checks 
+00000920: 666f 720a 2020 2020 2020 2020 2020 6120  for.          a 
+00000930: 6375 7374 6f6d 2069 6d70 6c65 6d65 6e74  custom implement
+00000940: 6174 696f 6e20 6f66 2060 7566 756e 6360  ation of `ufunc`
+00000950: 2e20 4966 2074 6865 7265 2069 7320 6120  . If there is a 
+00000960: 6375 7374 6f6d 0a20 2020 2020 2020 2020  custom.         
+00000970: 2069 6d70 6c65 6d65 6e74 6174 696f 6e2c   implementation,
+00000980: 2074 6869 7320 6d65 7468 6f64 2061 7070   this method app
+00000990: 6c69 6573 2069 7420 616e 6420 7265 7475  lies it and retu
+000009a0: 726e 7320 7468 6520 7265 7375 6c74 2e20  rns the result. 
+000009b0: 4966 0a20 2020 2020 2020 2020 2074 6865  If.          the
+000009c0: 7265 2069 7320 6e6f 2063 7573 746f 6d20  re is no custom 
+000009d0: 696d 706c 656d 656e 7461 7469 6f6e 2c20  implementation, 
+000009e0: 7468 6973 206d 6574 686f 6420 7061 7373  this method pass
+000009f0: 6573 2063 6f6e 7472 6f6c 2074 6f0a 2020  es control to.  
+00000a00: 2020 2020 2020 2020 605f 6170 706c 795f          `_apply_
+00000a10: 7566 756e 6360 2c20 746f 2061 6c6c 6f77  ufunc`, to allow
+00000a20: 2073 7562 636c 6173 7320 6375 7374 6f6d   subclass custom
+00000a30: 697a 6174 696f 6e2e 0a20 2020 2020 2020  ization..       
+00000a40: 202d 2053 6565 2060 696d 706c 656d 656e   - See `implemen
+00000a50: 7473 6020 666f 7220 6164 6469 7469 6f6e  ts` for addition
+00000a60: 616c 2067 7569 6461 6e63 6520 6f6e 2063  al guidance on c
+00000a70: 7573 746f 6d20 696d 706c 656d 656e 7461  ustom implementa
+00000a80: 7469 6f6e 732e 0a0a 2020 2020 2020 2020  tions...        
+00000a90: 5365 6520 416c 736f 0a20 2020 2020 2020  See Also.       
+00000aa0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+00000ab0: 2020 6069 6d70 6c65 6d65 6e74 7360 0a20    `implements`. 
+00000ac0: 2020 2020 2020 2020 2020 2043 6c61 7373             Class
+00000ad0: 206d 6574 686f 6420 666f 7220 7265 6769   method for regi
+00000ae0: 7374 6572 696e 6720 6375 7374 6f6d 2075  stering custom u
+00000af0: 6675 6e63 2069 6d70 6c65 6d65 6e74 6174  func implementat
+00000b00: 696f 6e73 2e0a 0a20 2020 2020 2020 2060  ions...        `
+00000b10: 5f61 7070 6c79 5f75 6675 6e63 600a 2020  _apply_ufunc`.  
+00000b20: 2020 2020 2020 2020 2020 496e 7374 616e            Instan
+00000b30: 6365 206d 6574 686f 6420 7468 6174 2061  ce method that a
+00000b40: 6c6c 6f77 7320 6375 7374 6f6d 2068 616e  llows custom han
+00000b50: 646c 696e 6720 6f66 2075 6675 6e63 7320  dling of ufuncs 
+00000b60: 636f 7272 6573 706f 6e64 696e 670a 2020  corresponding.  
+00000b70: 2020 2020 2020 2020 2020 746f 2073 7461            to sta
+00000b80: 6e64 6172 6420 5079 7468 6f6e 206e 756d  ndard Python num
+00000b90: 6572 6963 616c 206f 7065 7261 746f 7273  erical operators
+00000ba0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00000bb0: 2020 2020 2020 6f75 7420 3d20 6b77 6172        out = kwar
+00000bc0: 6773 2e67 6574 2827 6f75 7427 2c20 2829  gs.get('out', ()
+00000bd0: 290a 2020 2020 2020 2020 6163 6365 7074  ).        accept
+00000be0: 6564 203d 2074 7570 6c65 2873 656c 662e  ed = tuple(self.
+00000bf0: 5f55 4655 4e43 5f54 5950 4553 290a 2020  _UFUNC_TYPES).  
+00000c00: 2020 2020 2020 6966 206e 6f74 2061 6c6c        if not all
+00000c10: 2869 7369 6e73 7461 6e63 6528 782c 2061  (isinstance(x, a
+00000c20: 6363 6570 7465 6429 2066 6f72 2078 2069  ccepted) for x i
+00000c30: 6e20 6172 6773 202b 206f 7574 293a 0a20  n args + out):. 
+00000c40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000c50: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
+00000c60: 0a20 2020 2020 2020 2069 6620 6f75 743a  .        if out:
+00000c70: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+00000c80: 7267 735b 276f 7574 275d 203d 2074 7570  rgs['out'] = tup
+00000c90: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+00000ca0: 2020 2020 782e 5f64 6174 6120 6966 2069      x._data if i
+00000cb0: 7369 6e73 7461 6e63 6528 782c 204f 626a  sinstance(x, Obj
+00000cc0: 6563 7429 0a20 2020 2020 2020 2020 2020  ect).           
+00000cd0: 2020 2020 2065 6c73 6520 7820 666f 7220       else x for 
+00000ce0: 7820 696e 206f 7574 0a20 2020 2020 2020  x in out.       
+00000cf0: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00000d00: 6620 7365 6c66 2e5f 696d 706c 656d 656e  f self._implemen
+00000d10: 7473 2875 6675 6e63 293a 0a20 2020 2020  ts(ufunc):.     
+00000d20: 2020 2020 2020 206f 7065 7261 746f 7220         operator 
+00000d30: 3d20 7365 6c66 2e5f 4655 4e43 5449 4f4e  = self._FUNCTION
+00000d40: 535b 7566 756e 635d 0a20 2020 2020 2020  S[ufunc].       
+00000d50: 2020 2020 2072 6574 7572 6e20 6f70 6572       return oper
+00000d60: 6174 6f72 282a 6172 6773 2c20 2a2a 6b77  ator(*args, **kw
+00000d70: 6172 6773 290a 2020 2020 2020 2020 7265  args).        re
+00000d80: 7475 726e 2073 656c 662e 5f61 7070 6c79  turn self._apply
+00000d90: 5f75 6675 6e63 2875 6675 6e63 2c20 6d65  _ufunc(ufunc, me
+00000da0: 7468 6f64 2c20 2a61 7267 732c 202a 2a6b  thod, *args, **k
+00000db0: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
+00000dc0: 5f61 7070 6c79 5f75 6675 6e63 2873 656c  _apply_ufunc(sel
+00000dd0: 662c 2075 6675 6e63 2c20 6d65 7468 6f64  f, ufunc, method
+00000de0: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+00000df0: 7329 3a0a 2020 2020 2020 2020 2222 2241  s):.        """A
+00000e00: 7070 6c79 2061 2060 6e75 6d70 7960 2075  pply a `numpy` u
+00000e10: 6e69 7665 7273 616c 2066 756e 6374 696f  niversal functio
+00000e20: 6e20 2861 2e6b 2e61 2022 7566 756e 6322  n (a.k.a "ufunc"
+00000e30: 2920 746f 2064 6174 612e 0a0a 2020 2020  ) to data...    
+00000e40: 2020 2020 4e6f 7465 730a 2020 2020 2020      Notes.      
+00000e50: 2020 2d2d 2d2d 2d0a 2020 2020 2020 2020    -----.        
+00000e60: 2d20 5375 6263 6c61 7373 6573 2074 6861  - Subclasses tha
+00000e70: 7420 7769 7368 2074 6f20 6375 7374 6f6d  t wish to custom
+00000e80: 697a 6520 7375 7070 6f72 7420 666f 7220  ize support for 
+00000e90: 7566 756e 6373 2073 686f 756c 6420 6f76  ufuncs should ov
+00000ea0: 6572 6c6f 6164 0a20 2020 2020 2020 2020  erload.         
+00000eb0: 2074 6869 7320 6d65 7468 6f64 2069 6e73   this method ins
+00000ec0: 7465 6164 206f 6620 605f 5f61 7272 6179  tead of `__array
+00000ed0: 5f75 6675 6e63 5f5f 602e 0a20 2020 2020  _ufunc__`..     
+00000ee0: 2020 202d 2053 7562 636c 6173 7365 7320     - Subclasses 
+00000ef0: 7368 6f75 6c64 2070 7265 6665 7220 746f  should prefer to
+00000f00: 2064 6566 696e 6520 6375 7374 6f6d 2069   define custom i
+00000f10: 6d70 6c65 6d65 6e74 6174 696f 6e73 206f  mplementations o
+00000f20: 6620 7370 6563 6966 6963 0a20 2020 2020  f specific.     
+00000f30: 2020 2020 2075 6e69 7665 7273 616c 2066       universal f
+00000f40: 756e 6374 696f 6e73 2061 6e64 2072 6567  unctions and reg
+00000f50: 6973 7465 7220 6561 6368 2076 6961 2060  ister each via `
+00000f60: 696d 706c 656d 656e 7473 602c 2072 6174  implements`, rat
+00000f70: 6865 7220 7468 616e 0a20 2020 2020 2020  her than.       
+00000f80: 2020 2069 6d70 6c65 6d65 6e74 696e 6720     implementing 
+00000f90: 6675 6e63 7469 6f6e 2d73 7065 6369 6669  function-specifi
+00000fa0: 6320 6c6f 6769 6320 696e 2074 6869 7320  c logic in this 
+00000fb0: 6d65 7468 6f64 2c20 7369 6e63 650a 2020  method, since.  
+00000fc0: 2020 2020 2020 2020 605f 5f61 7272 6179          `__array
+00000fd0: 5f75 6675 6e63 5f5f 6020 7769 6c6c 2063  _ufunc__` will c
+00000fe0: 6865 636b 2066 6f72 2061 2063 7573 746f  heck for a custo
+00000ff0: 6d20 696d 706c 656d 656e 7461 7469 6f6e  m implementation
+00001000: 206f 6620 6120 6769 7665 6e0a 2020 2020   of a given.    
+00001010: 2020 2020 2020 6675 6e63 7469 6f6e 2062        function b
+00001020: 6566 6f72 6520 6361 6c6c 696e 6720 7468  efore calling th
+00001030: 6973 206d 6574 686f 642e 0a20 2020 2020  is method..     
+00001040: 2020 202d 2054 6865 2064 6566 6175 6c74     - The default
+00001050: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00001060: 6f66 2074 6869 7320 6d65 7468 6f64 2061  of this method a
+00001070: 7070 6c69 6573 2074 6865 2067 6976 656e  pplies the given
+00001080: 2075 6675 6e63 2074 6f0a 2020 2020 2020   ufunc to.      
+00001090: 2020 2020 7265 616c 2d76 616c 7565 6420      real-valued 
+000010a0: 6461 7461 2061 6e64 2064 6972 6563 746c  data and directl
+000010b0: 7920 7265 7475 726e 7320 7468 6520 606e  y returns the `n
+000010c0: 756d 7079 6020 7265 7375 6c74 2c20 7769  umpy` result, wi
+000010d0: 7468 6f75 740a 2020 2020 2020 2020 2020  thout.          
+000010e0: 6174 7465 6d70 7469 6e67 2074 6f20 6372  attempting to cr
+000010f0: 6561 7465 2061 206e 6577 2069 6e73 7461  eate a new insta
+00001100: 6e63 6520 6f66 2074 6865 2063 7573 746f  nce of the custo
+00001110: 6d20 7375 6263 6c61 7373 2e0a 0a20 2020  m subclass...   
+00001120: 2020 2020 2053 6565 2041 6c73 6f0a 2020       See Also.  
+00001130: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20        --------. 
+00001140: 2020 2020 2020 2060 696d 706c 656d 656e         `implemen
+00001150: 7473 600a 2020 2020 2020 2020 2020 2020  ts`.            
+00001160: 436c 6173 7320 6d65 7468 6f64 2066 6f72  Class method for
+00001170: 2072 6567 6973 7465 7269 6e67 2063 7573   registering cus
+00001180: 746f 6d20 7566 756e 6320 696d 706c 656d  tom ufunc implem
+00001190: 656e 7461 7469 6f6e 732e 0a0a 2020 2020  entations...    
+000011a0: 2020 2020 605f 5f61 7272 6179 5f75 6675      `__array_ufu
+000011b0: 6e63 5f5f 600a 2020 2020 2020 2020 2020  nc__`.          
+000011c0: 2020 5468 6520 656e 7472 7920 706f 696e    The entry poin
+000011d0: 7420 666f 7220 606e 756d 7079 6020 756e  t for `numpy` un
+000011e0: 6976 6572 7361 6c20 6675 6e63 7469 6f6e  iversal function
+000011f0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00001200: 2020 2020 2020 206f 7065 7261 746f 7220         operator 
+00001210: 3d20 6765 7461 7474 7228 7566 756e 632c  = getattr(ufunc,
+00001220: 206d 6574 686f 6429 0a20 2020 2020 2020   method).       
+00001230: 2076 616c 7565 7320 3d20 7365 6c66 2e5f   values = self._
+00001240: 6765 745f 6e75 6d70 795f 6172 6773 2861  get_numpy_args(a
+00001250: 7267 7329 0a20 2020 2020 2020 2074 7279  rgs).        try
+00001260: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+00001270: 7461 203d 206f 7065 7261 746f 7228 2a76  ta = operator(*v
+00001280: 616c 7565 732c 202a 2a6b 7761 7267 7329  alues, **kwargs)
+00001290: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000012a0: 5479 7065 4572 726f 7220 6173 2065 7272  TypeError as err
+000012b0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000012c0: 6973 6520 5479 7065 4572 726f 7228 0a20  ise TypeError(. 
+000012d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000012e0: 2255 6e61 626c 6520 746f 2061 7070 6c79  "Unable to apply
+000012f0: 207b 7566 756e 637d 2074 6f20 7b61 7267   {ufunc} to {arg
+00001300: 737d 220a 2020 2020 2020 2020 2020 2020  s}".            
+00001310: 2920 6672 6f6d 2065 7272 0a20 2020 2020  ) from err.     
+00001320: 2020 2069 6620 6d65 7468 6f64 2021 3d20     if method != 
+00001330: 2761 7427 3a0a 2020 2020 2020 2020 2020  'at':.          
+00001340: 2020 7265 7475 726e 2064 6174 610a 0a20    return data.. 
+00001350: 2020 205f 4655 4e43 5449 4f4e 5f54 5950     _FUNCTION_TYP
+00001360: 4553 203d 205b 0a20 2020 2020 2020 206e  ES = [.        n
+00001370: 756d 7079 2e6e 6461 7272 6179 2c0a 2020  umpy.ndarray,.  
+00001380: 2020 2020 2020 4f62 6a65 6374 2c0a 2020        Object,.  
+00001390: 2020 5d20 2b20 6c69 7374 286e 756d 7079    ] + list(numpy
+000013a0: 2e53 6361 6c61 7254 7970 6529 0a0a 2020  .ScalarType)..  
+000013b0: 2020 6465 6620 5f5f 6172 7261 795f 6675    def __array_fu
+000013c0: 6e63 7469 6f6e 5f5f 2873 656c 662c 2066  nction__(self, f
+000013d0: 756e 632c 2074 7970 6573 2c20 6172 6773  unc, types, args
+000013e0: 2c20 6b77 6172 6773 293a 0a20 2020 2020  , kwargs):.     
+000013f0: 2020 2022 2222 5072 6f76 6964 6520 7375     """Provide su
+00001400: 7070 6f72 7420 666f 7220 6675 6e63 7469  pport for functi
+00001410: 6f6e 7320 696e 2074 6865 2060 6e75 6d70  ons in the `nump
+00001420: 7960 2070 7562 6c69 6320 4150 492e 0a0a  y` public API...
+00001430: 2020 2020 2020 2020 5365 6520 6874 7470          See http
+00001440: 733a 2f2f 6e75 6d70 792e 6f72 672f 646f  s://numpy.org/do
+00001450: 632f 7374 6162 6c65 2f72 6566 6572 656e  c/stable/referen
+00001460: 6365 2f61 7272 6179 732e 636c 6173 7365  ce/arrays.classe
+00001470: 732e 6874 6d6c 2066 6f72 206d 6f72 650a  s.html for more.
+00001480: 2020 2020 2020 2020 696e 666f 726d 6174          informat
+00001490: 696f 6e20 6f66 2075 7365 206f 6620 7468  ion of use of th
+000014a0: 6973 2073 7065 6369 616c 206d 6574 686f  is special metho
+000014b0: 642e 2054 6865 2069 6d70 6c65 6d65 6e74  d. The implement
+000014c0: 6174 696f 6e20 7368 6f77 6e20 6865 7265  ation shown here
+000014d0: 0a20 2020 2020 2020 2069 7320 6120 636f  .        is a co
+000014e0: 6d62 696e 6174 696f 6e20 6f66 2074 6865  mbination of the
+000014f0: 2065 7861 6d70 6c65 206f 6e20 7468 6174   example on that
+00001500: 2070 6167 6520 616e 6420 636f 6465 2066   page and code f
+00001510: 726f 6d20 7468 650a 2020 2020 2020 2020  rom the.        
+00001520: 6465 6669 6e69 7469 6f6e 206f 6620 6045  definition of `E
+00001530: 6e63 6170 7375 6c61 7465 4e44 4172 7261  ncapsulateNDArra
+00001540: 792e 5f5f 6172 7261 795f 6675 6e63 7469  y.__array_functi
+00001550: 6f6e 5f5f 6020 696e 0a20 2020 2020 2020  on__` in.       
+00001560: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00001570: 636f 6d2f 6461 736b 2f64 6173 6b2f 626c  com/dask/dask/bl
+00001580: 6f62 2f6d 6169 6e2f 6461 736b 2f61 7272  ob/main/dask/arr
+00001590: 6179 2f74 6573 7473 2f74 6573 745f 6469  ay/tests/test_di
+000015a0: 7370 6174 6368 2e70 790a 0a20 2020 2020  spatch.py..     
+000015b0: 2020 204e 6f74 6573 0a20 2020 2020 2020     Notes.       
+000015c0: 202d 2d2d 2d2d 0a20 2020 2020 2020 202d   -----.        -
+000015d0: 2054 6869 7320 6d65 7468 6f64 2066 6972   This method fir
+000015e0: 7374 2063 6865 636b 7320 7468 6174 2061  st checks that a
+000015f0: 6c6c 2060 7479 7065 7360 2061 7265 2069  ll `types` are i
+00001600: 6e0a 2020 2020 2020 2020 2020 6073 656c  n.          `sel
+00001610: 662e 5f46 554e 4354 494f 4e5f 5459 5045  f._FUNCTION_TYPE
+00001620: 5360 2c20 7468 6572 6562 7920 616c 6c6f  S`, thereby allo
+00001630: 7769 6e67 2073 7562 636c 6173 7365 7320  wing subclasses 
+00001640: 7468 6174 2064 6f6e 2774 0a20 2020 2020  that don't.     
+00001650: 2020 2020 206f 7665 7272 6964 6520 605f       override `_
+00001660: 5f61 7272 6179 5f66 756e 6374 696f 6e5f  _array_function_
+00001670: 5f60 2074 6f20 6861 6e64 6c65 206f 626a  _` to handle obj
+00001680: 6563 7473 206f 6620 7468 6973 2074 7970  ects of this typ
+00001690: 652e 2049 7420 7468 656e 0a20 2020 2020  e. It then.     
+000016a0: 2020 2020 2063 6865 636b 7320 666f 7220       checks for 
+000016b0: 6120 6375 7374 6f6d 2069 6d70 6c65 6d65  a custom impleme
+000016c0: 6e74 6174 696f 6e20 6f66 2060 6675 6e63  ntation of `func
+000016d0: 602e 2049 6620 7468 6572 6520 6973 2061  `. If there is a
+000016e0: 2063 7573 746f 6d0a 2020 2020 2020 2020   custom.        
+000016f0: 2020 696d 706c 656d 656e 7461 7469 6f6e    implementation
+00001700: 2c20 7468 6973 206d 6574 686f 6420 6170  , this method ap
+00001710: 706c 6965 7320 6974 2061 6e64 2072 6574  plies it and ret
+00001720: 7572 6e73 2074 6865 2072 6573 756c 742e  urns the result.
+00001730: 2049 660a 2020 2020 2020 2020 2020 7468   If.          th
+00001740: 6572 6520 6973 206e 6f20 6375 7374 6f6d  ere is no custom
+00001750: 2069 6d70 6c65 6d65 6e74 6174 696f 6e2c   implementation,
+00001760: 2074 6869 7320 6d65 7468 6f64 2070 6173   this method pas
+00001770: 7365 7320 636f 6e74 726f 6c20 746f 0a20  ses control to. 
+00001780: 2020 2020 2020 2020 2060 5f61 7070 6c79           `_apply
+00001790: 5f66 756e 6374 696f 6e60 2c20 746f 2061  _function`, to a
+000017a0: 6c6c 6f77 2073 7562 636c 6173 7320 6375  llow subclass cu
+000017b0: 7374 6f6d 697a 6174 696f 6e2e 0a20 2020  stomization..   
+000017c0: 2020 2020 202d 2053 6565 2060 696d 706c       - See `impl
+000017d0: 656d 656e 7473 6020 666f 7220 6164 6469  ements` for addi
+000017e0: 7469 6f6e 616c 2067 7569 6461 6e63 6520  tional guidance 
+000017f0: 6f6e 2063 7573 746f 6d20 696d 706c 656d  on custom implem
+00001800: 656e 7461 7469 6f6e 732e 0a0a 2020 2020  entations...    
+00001810: 2020 2020 5365 6520 416c 736f 0a20 2020      See Also.   
+00001820: 2020 2020 202d 2d2d 2d2d 2d2d 2d0a 2020       --------.  
+00001830: 2020 2020 2020 6069 6d70 6c65 6d65 6e74        `implement
+00001840: 7360 0a20 2020 2020 2020 2020 2020 2043  s`.            C
+00001850: 6c61 7373 206d 6574 686f 6420 666f 7220  lass method for 
+00001860: 7265 6769 7374 6572 696e 6720 6375 7374  registering cust
+00001870: 6f6d 2066 756e 6374 696f 6e20 696d 706c  om function impl
+00001880: 656d 656e 7461 7469 6f6e 732e 0a0a 2020  ementations...  
+00001890: 2020 2020 2020 605f 6170 706c 795f 6675        `_apply_fu
+000018a0: 6e63 7469 6f6e 600a 2020 2020 2020 2020  nction`.        
+000018b0: 2020 2020 496e 7374 616e 6365 206d 6574      Instance met
+000018c0: 686f 6420 7468 6174 2061 6c6c 6f77 7320  hod that allows 
+000018d0: 6375 7374 6f6d 2068 616e 646c 696e 6720  custom handling 
+000018e0: 6f66 2060 6e75 6d70 7960 2070 7562 6c69  of `numpy` publi
+000018f0: 630a 2020 2020 2020 2020 2020 2020 6675  c.            fu
+00001900: 6e63 7469 6f6e 7320 7768 656e 2074 6865  nctions when the
+00001910: 7265 2069 7320 6e6f 2072 6567 6973 7465  re is no registe
+00001920: 7265 6420 6375 7374 6f6d 2069 6d70 6c65  red custom imple
+00001930: 6d65 6e74 6174 696f 6e2e 0a20 2020 2020  mentation..     
+00001940: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+00001950: 6363 6570 7465 6420 3d20 7475 706c 6528  ccepted = tuple(
+00001960: 7365 6c66 2e5f 4655 4e43 5449 4f4e 5f54  self._FUNCTION_T
+00001970: 5950 4553 290a 2020 2020 2020 2020 6966  YPES).        if
+00001980: 206e 6f74 2061 6c6c 2869 7373 7562 636c   not all(issubcl
+00001990: 6173 7328 7469 2c20 6163 6365 7074 6564  ass(ti, accepted
+000019a0: 2920 666f 7220 7469 2069 6e20 7479 7065  ) for ti in type
+000019b0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+000019c0: 7265 7475 726e 204e 6f74 496d 706c 656d  return NotImplem
+000019d0: 656e 7465 640a 2020 2020 2020 2020 6966  ented.        if
+000019e0: 2073 656c 662e 5f69 6d70 6c65 6d65 6e74   self._implement
+000019f0: 7328 6675 6e63 293a 0a20 2020 2020 2020  s(func):.       
+00001a00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00001a10: 2e5f 4655 4e43 5449 4f4e 535b 6675 6e63  ._FUNCTIONS[func
+00001a20: 5d28 2a61 7267 732c 202a 2a6b 7761 7267  ](*args, **kwarg
+00001a30: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+00001a40: 6e20 7365 6c66 2e5f 6170 706c 795f 6675  n self._apply_fu
+00001a50: 6e63 7469 6f6e 2866 756e 632c 2074 7970  nction(func, typ
+00001a60: 6573 2c20 6172 6773 2c20 6b77 6172 6773  es, args, kwargs
+00001a70: 290a 0a20 2020 2064 6566 205f 6170 706c  )..    def _appl
+00001a80: 795f 6675 6e63 7469 6f6e 2873 656c 662c  y_function(self,
+00001a90: 2066 756e 632c 2074 7970 6573 2c20 6172   func, types, ar
+00001aa0: 6773 2c20 6b77 6172 6773 293a 0a20 2020  gs, kwargs):.   
+00001ab0: 2020 2020 2022 2222 4170 706c 7920 6120       """Apply a 
+00001ac0: 6675 6e63 7469 6f6e 2069 6e20 7468 6520  function in the 
+00001ad0: 606e 756d 7079 6020 7075 626c 6963 2041  `numpy` public A
+00001ae0: 5049 2e0a 0a20 2020 2020 2020 204e 6f74  PI...        Not
+00001af0: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
+00001b00: 0a20 2020 2020 2020 202d 2053 7562 636c  .        - Subcl
+00001b10: 6173 7365 7320 7468 6174 2077 6973 6820  asses that wish 
+00001b20: 746f 2063 7573 746f 6d69 7a65 2073 7570  to customize sup
+00001b30: 706f 7274 2066 6f72 2070 7562 6c69 6320  port for public 
+00001b40: 6675 6e63 7469 6f6e 7320 7368 6f75 6c64  functions should
+00001b50: 0a20 2020 2020 2020 2020 206f 7665 726c  .          overl
+00001b60: 6f61 6420 7468 6973 206d 6574 686f 6420  oad this method 
+00001b70: 696e 7374 6561 6420 6f66 2060 5f5f 6172  instead of `__ar
+00001b80: 7261 795f 6675 6e63 7469 6f6e 5f5f 602e  ray_function__`.
+00001b90: 0a20 2020 2020 2020 202d 2053 7562 636c  .        - Subcl
+00001ba0: 6173 7365 7320 7368 6f75 6c64 2070 7265  asses should pre
+00001bb0: 6665 7220 746f 2064 6566 696e 6520 6375  fer to define cu
+00001bc0: 7374 6f6d 2069 6d70 6c65 6d65 6e74 6174  stom implementat
+00001bd0: 696f 6e73 206f 6620 7370 6563 6966 6963  ions of specific
+00001be0: 0a20 2020 2020 2020 2020 2070 7562 6c69  .          publi
+00001bf0: 6320 6675 6e63 7469 6f6e 7320 616e 6420  c functions and 
+00001c00: 7265 6769 7374 6572 2065 6163 6820 7669  register each vi
+00001c10: 6120 6069 6d70 6c65 6d65 6e74 7360 2c20  a `implements`, 
+00001c20: 7261 7468 6572 2074 6861 6e0a 2020 2020  rather than.    
+00001c30: 2020 2020 2020 696d 706c 656d 656e 7469        implementi
+00001c40: 6e67 2066 756e 6374 696f 6e2d 7370 6563  ng function-spec
+00001c50: 6966 6963 206c 6f67 6963 2069 6e20 7468  ific logic in th
+00001c60: 6973 206d 6574 686f 642c 2073 696e 6365  is method, since
+00001c70: 0a20 2020 2020 2020 2020 2060 5f5f 6172  .          `__ar
+00001c80: 7261 795f 6675 6e63 7469 6f6e 5f5f 6020  ray_function__` 
+00001c90: 7769 6c6c 2063 6865 636b 2066 6f72 2061  will check for a
+00001ca0: 2063 7573 746f 6d20 696d 706c 656d 656e   custom implemen
+00001cb0: 7461 7469 6f6e 206f 6620 6120 6769 7665  tation of a give
+00001cc0: 6e0a 2020 2020 2020 2020 2020 6675 6e63  n.          func
+00001cd0: 7469 6f6e 2062 6566 6f72 6520 6361 6c6c  tion before call
+00001ce0: 696e 6720 7468 6973 206d 6574 686f 642e  ing this method.
+00001cf0: 0a20 2020 2020 2020 202d 2054 6865 2064  .        - The d
+00001d00: 6566 6175 6c74 2069 6d70 6c65 6d65 6e74  efault implement
+00001d10: 6174 696f 6e20 6361 6c6c 7320 605f 6765  ation calls `_ge
+00001d20: 745f 6e75 6d70 795f 6172 7261 7960 2066  t_numpy_array` f
+00001d30: 6f72 2061 6363 6573 7320 746f 0a20 2020  or access to.   
+00001d40: 2020 2020 2020 2072 6561 6c2d 7661 6c75         real-valu
+00001d50: 6564 2064 6174 6120 7669 6120 616e 2069  ed data via an i
+00001d60: 6e73 7461 6e63 6520 6f66 2060 6e75 6d70  nstance of `nump
+00001d70: 792e 6e64 6172 7261 7960 2c20 605f 6765  y.ndarray`, `_ge
+00001d80: 745f 6e75 6d70 795f 6172 6773 600a 2020  t_numpy_args`.  
+00001d90: 2020 2020 2020 2020 746f 2063 6f6e 7665          to conve
+00001da0: 7274 2060 6172 6773 6020 746f 2061 7070  rt `args` to app
+00001db0: 726f 7072 6961 7465 206f 7065 7261 6e64  ropriate operand
+00001dc0: 732c 2061 6e64 2060 5f67 6574 5f6e 756d  s, and `_get_num
+00001dd0: 7079 5f74 7970 6573 6020 746f 0a20 2020  py_types` to.   
+00001de0: 2020 2020 2020 2065 7874 7261 6374 2061         extract a
+00001df0: 7070 726f 7072 6961 7465 206f 7065 7261  ppropriate opera
+00001e00: 6e64 2074 7970 6573 2e20 5375 6263 6c61  nd types. Subcla
+00001e10: 7373 6573 206d 6179 2063 686f 6f73 6520  sses may choose 
+00001e20: 746f 206f 7665 726c 6f61 640a 2020 2020  to overload.    
+00001e30: 2020 2020 2020 616e 7920 6f66 2074 686f        any of tho
+00001e40: 7365 2069 6e64 6976 6964 7561 6c20 6d65  se individual me
+00001e50: 7468 6f64 7320 696e 7374 6561 6420 6f66  thods instead of
+00001e60: 206f 7665 726c 6f61 6469 6e67 2074 6869   overloading thi
+00001e70: 7320 6d65 7468 6f64 2e0a 0a20 2020 2020  s method...     
+00001e80: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
+00001e90: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+00001ea0: 2020 2020 2060 696d 706c 656d 656e 7473       `implements
+00001eb0: 600a 2020 2020 2020 2020 2020 2020 436c  `.            Cl
+00001ec0: 6173 7320 6d65 7468 6f64 2066 6f72 2072  ass method for r
+00001ed0: 6567 6973 7465 7269 6e67 2063 7573 746f  egistering custo
+00001ee0: 6d20 7566 756e 6320 696d 706c 656d 656e  m ufunc implemen
+00001ef0: 7461 7469 6f6e 732e 0a0a 2020 2020 2020  tations...      
+00001f00: 2020 605f 5f61 7272 6179 5f66 756e 6374    `__array_funct
+00001f10: 696f 6e5f 5f60 0a20 2020 2020 2020 2020  ion__`.         
+00001f20: 2020 2054 6865 2065 6e74 7279 2070 6f69     The entry poi
+00001f30: 6e74 2066 6f72 2060 6e75 6d70 7960 2070  nt for `numpy` p
+00001f40: 7562 6c69 6320 6675 6e63 7469 6f6e 732e  ublic functions.
+00001f50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001f60: 2020 2020 2061 7272 6179 203d 2073 656c       array = sel
+00001f70: 662e 5f67 6574 5f6e 756d 7079 5f61 7272  f._get_numpy_arr
+00001f80: 6179 2829 0a20 2020 2020 2020 2069 6620  ay().        if 
+00001f90: 6172 7261 7920 6973 204e 6f6e 653a 0a20  array is None:. 
+00001fa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001fb0: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
+00001fc0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00001fd0: 6973 696e 7374 616e 6365 2861 7272 6179  isinstance(array
+00001fe0: 2c20 6e75 6d70 792e 6e64 6172 7261 7929  , numpy.ndarray)
+00001ff0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00002000: 6973 6520 5479 7065 4572 726f 7228 0a20  ise TypeError(. 
+00002010: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00002020: 227b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  "{self.__class__
+00002030: 2e5f 5f71 7561 6c6e 616d 655f 5f7d 2e5f  .__qualname__}._
+00002040: 6765 745f 6e75 6d70 795f 6172 7261 7922  get_numpy_array"
+00002050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002060: 2022 2064 6964 206e 6f74 2072 6574 7572   " did not retur
+00002070: 6e20 6120 6e75 6d70 792e 6e64 6172 7261  n a numpy.ndarra
+00002080: 7922 0a20 2020 2020 2020 2020 2020 2029  y".            )
+00002090: 2066 726f 6d20 4e6f 6e65 0a20 2020 2020   from None.     
+000020a0: 2020 2061 7267 7320 3d20 7365 6c66 2e5f     args = self._
+000020b0: 6765 745f 6e75 6d70 795f 6172 6773 2861  get_numpy_args(a
+000020c0: 7267 7329 0a20 2020 2020 2020 2074 7970  rgs).        typ
+000020d0: 6573 203d 2073 656c 662e 5f67 6574 5f6e  es = self._get_n
+000020e0: 756d 7079 5f74 7970 6573 2874 7970 6573  umpy_types(types
+000020f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00002100: 2061 7272 6179 2e5f 5f61 7272 6179 5f66   array.__array_f
+00002110: 756e 6374 696f 6e5f 5f28 6675 6e63 2c20  unction__(func, 
+00002120: 7479 7065 732c 2061 7267 732c 206b 7761  types, args, kwa
+00002130: 7267 7329 0a0a 2020 2020 6465 6620 5f67  rgs)..    def _g
+00002140: 6574 5f6e 756d 7079 5f61 7272 6179 2873  et_numpy_array(s
+00002150: 656c 6629 202d 3e20 7479 7069 6e67 2e4f  elf) -> typing.O
+00002160: 7074 696f 6e61 6c5b 6e75 6d70 792e 7479  ptional[numpy.ty
+00002170: 7069 6e67 2e4e 4441 7272 6179 5d3a 0a20  ping.NDArray]:. 
+00002180: 2020 2020 2020 2022 2222 436f 6e76 6572         """Conver
+00002190: 7420 7468 6520 6461 7461 2069 6e74 6572  t the data inter
+000021a0: 6661 6365 2074 6f20 616e 2061 7272 6179  face to an array
+000021b0: 2066 6f72 2060 6e75 6d70 7960 206d 6978   for `numpy` mix
+000021c0: 696e 206d 6574 686f 6473 2e0a 2020 2020  in methods..    
+000021d0: 2020 2020 0a20 2020 2020 2020 204e 6f74      .        Not
+000021e0: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
+000021f0: 0a20 2020 2020 2020 202d 2054 6869 7320  .        - This 
+00002200: 6d65 7468 6f64 2061 6c6c 6f77 7320 7375  method allows su
+00002210: 6263 6c61 7373 2069 6d70 6c65 6d65 6e74  bclass implement
+00002220: 6174 696f 6e73 2074 6f20 636f 6e74 726f  ations to contro
+00002230: 6c20 686f 7720 7468 6579 0a20 2020 2020  l how they.     
+00002240: 2020 2020 2063 6f6e 7665 7274 2074 6865       convert the
+00002250: 6972 2064 6174 6120 696e 7465 7266 6163  ir data interfac
+00002260: 6520 746f 2061 2060 6e75 6d70 792e 6e64  e to a `numpy.nd
+00002270: 6172 7261 7960 2066 6f72 2075 7365 2077  array` for use w
+00002280: 6974 6820 606e 756d 7079 600a 2020 2020  ith `numpy`.    
+00002290: 2020 2020 2020 7075 626c 6963 2066 756e        public fun
+000022a0: 6374 696f 6e73 2e0a 2020 2020 2020 2020  ctions..        
+000022b0: 2d20 5265 7475 726e 696e 6720 604e 6f6e  - Returning `Non
+000022c0: 6560 2066 726f 6d20 7468 6973 206d 6574  e` from this met
+000022d0: 686f 6420 7769 6c6c 2063 6175 7365 2060  hod will cause `
+000022e0: 5f61 7070 6c79 5f66 756e 6374 696f 6e60  _apply_function`
+000022f0: 2074 6f0a 2020 2020 2020 2020 2020 7265   to.          re
+00002300: 7475 726e 2060 4e6f 7449 6d70 6c65 6d65  turn `NotImpleme
+00002310: 6e74 6564 602e 0a20 2020 2020 2020 202d  nted`..        -
+00002320: 2054 6865 2064 6566 6175 6c74 2069 6d70   The default imp
+00002330: 6c65 6d65 6e74 6174 696f 6e20 756e 636f  lementation unco
+00002340: 6e64 6974 696f 6e61 6c6c 7920 7265 7475  nditionally retu
+00002350: 726e 7320 604e 6f6e 6560 2e0a 2020 2020  rns `None`..    
+00002360: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00002370: 7265 7475 726e 0a0a 2020 2020 6465 6620  return..    def 
+00002380: 5f67 6574 5f6e 756d 7079 5f61 7267 7328  _get_numpy_args(
+00002390: 7365 6c66 2c20 6172 6773 293a 0a20 2020  self, args):.   
+000023a0: 2020 2020 2022 2222 436f 6e76 6572 7420       """Convert 
+000023b0: 6061 7267 7360 2074 6f20 6f70 6572 616e  `args` to operan
+000023c0: 6473 206f 6620 6120 606e 756d 7079 6020  ds of a `numpy` 
+000023d0: 6675 6e63 7469 6f6e 2e0a 0a20 2020 2020  function...     
+000023e0: 2020 2054 6869 7320 6d65 7468 6f64 2077     This method w
+000023f0: 696c 6c20 6361 6c6c 2060 7e5f 6765 745f  ill call `~_get_
+00002400: 6e75 6d70 795f 6172 6760 206f 6e20 6561  numpy_arg` on ea
+00002410: 6368 206d 656d 6265 7220 6f66 2060 6172  ch member of `ar
+00002420: 6773 6020 696e 0a20 2020 2020 2020 206f  gs` in.        o
+00002430: 7264 6572 2074 6f20 6275 696c 6420 6120  rder to build a 
+00002440: 6074 7570 6c65 6020 6f66 2073 7569 7461  `tuple` of suita
+00002450: 626c 6520 6f70 6572 616e 6473 2e20 5375  ble operands. Su
+00002460: 6263 6c61 7373 6573 206d 6179 206f 7665  bclasses may ove
+00002470: 726c 6f61 640a 2020 2020 2020 2020 607e  rload.        `~
+00002480: 5f67 6574 5f6e 756d 7079 5f61 7267 6020  _get_numpy_arg` 
+00002490: 746f 2063 7573 746f 6d69 7a65 2061 6363  to customize acc
+000024a0: 6573 7320 746f 2074 6865 6972 2064 6174  ess to their dat
+000024b0: 6120 6174 7472 6962 7574 652e 0a20 2020  a attribute..   
+000024c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000024d0: 2072 6574 7572 6e20 7475 706c 6528 7365   return tuple(se
+000024e0: 6c66 2e5f 6765 745f 6172 675f 6461 7461  lf._get_arg_data
+000024f0: 2861 7267 2920 666f 7220 6172 6720 696e  (arg) for arg in
+00002500: 2061 7267 7329 0a0a 2020 2020 6465 6620   args)..    def 
+00002510: 5f67 6574 5f61 7267 5f64 6174 6128 7365  _get_arg_data(se
+00002520: 6c66 2c20 6172 6729 3a0a 2020 2020 2020  lf, arg):.      
+00002530: 2020 2222 2243 6f6e 7665 7274 2060 6172    """Convert `ar
+00002540: 6760 2074 6f20 616e 206f 7065 7261 6e64  g` to an operand
+00002550: 206f 6620 6120 606e 756d 7079 6020 6675   of a `numpy` fu
+00002560: 6e63 7469 6f6e 2e0a 0a20 2020 2020 2020  nction...       
+00002570: 2053 6565 2041 6c73 6f0a 2020 2020 2020   See Also.      
+00002580: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020    --------.     
+00002590: 2020 2060 7e5f 6765 745f 6e75 6d70 795f     `~_get_numpy_
+000025a0: 6172 6773 600a 2020 2020 2020 2020 2020  args`.          
+000025b0: 2020 5468 6520 6d65 7468 6f64 2074 6861    The method tha
+000025c0: 7420 6361 6c6c 7320 7468 6973 206d 6574  t calls this met
+000025d0: 686f 6420 696e 2061 206c 6f6f 702e 0a0a  hod in a loop...
+000025e0: 2020 2020 2020 2020 4e6f 7465 730a 2020          Notes.  
+000025f0: 2020 2020 2020 2d2d 2d2d 2d0a 2020 2020        -----.    
+00002600: 2020 2020 2d20 5468 6973 206d 6574 686f      - This metho
+00002610: 6420 616c 6c6f 7773 2061 2073 7562 636c  d allows a subcl
+00002620: 6173 7320 746f 2063 7573 746f 6d69 7a65  ass to customize
+00002630: 2068 6f77 2060 6e75 6d70 7960 2066 756e   how `numpy` fun
+00002640: 6374 696f 6e73 0a20 2020 2020 2020 2020  ctions.         
+00002650: 2061 6363 6573 7320 6974 7320 6461 7461   access its data
+00002660: 2061 7474 7269 6275 7465 2e0a 2020 2020   attribute..    
+00002670: 2020 2020 2d20 5468 6520 6465 6661 756c      - The defaul
+00002680: 7420 696d 706c 656d 656e 7461 7469 6f6e  t implementation
+00002690: 2077 696c 6c20 7265 7475 726e 2074 6865   will return the
+000026a0: 2060 6461 7461 6020 6174 7472 6962 7574   `data` attribut
+000026b0: 6520 6f66 2061 0a20 2020 2020 2020 2020  e of a.         
+000026c0: 2060 7e6e 756d 6572 6963 2e4f 626a 6563   `~numeric.Objec
+000026d0: 7460 2c20 7468 6520 605f 6f62 6a65 6374  t`, the `_object
+000026e0: 6020 6174 7472 6962 7574 6520 6f66 2061  ` attribute of a
+000026f0: 0a20 2020 2020 2020 2020 2060 7e6e 756d  .          `~num
+00002700: 6572 6963 2e51 7561 6e74 6974 7960 2c20  eric.Quantity`, 
+00002710: 6f72 206f 7468 6572 7769 7365 2074 6865  or otherwise the
+00002720: 2075 6e6d 6f64 6966 6965 6420 6172 6775   unmodified argu
+00002730: 6d65 6e74 2e0a 2020 2020 2020 2020 2222  ment..        ""
+00002740: 220a 2020 2020 2020 2020 6966 2069 7369  ".        if isi
+00002750: 6e73 7461 6e63 6528 6172 672c 204f 626a  nstance(arg, Obj
+00002760: 6563 7429 3a0a 2020 2020 2020 2020 2020  ect):.          
+00002770: 2020 7265 7475 726e 2061 7267 2e64 6174    return arg.dat
+00002780: 610a 2020 2020 2020 2020 7265 7475 726e  a.        return
+00002790: 2061 7267 0a0a 2020 2020 6465 6620 5f67   arg..    def _g
+000027a0: 6574 5f6e 756d 7079 5f74 7970 6573 2873  et_numpy_types(s
+000027b0: 656c 662c 2074 7970 6573 293a 0a20 2020  elf, types):.   
+000027c0: 2020 2020 2022 2222 4578 7472 6163 7420       """Extract 
+000027d0: 6170 7072 6f70 7269 6174 6520 7479 7065  appropriate type
+000027e0: 7320 666f 7220 6120 606e 756d 7079 6020  s for a `numpy` 
+000027f0: 6675 6e63 7469 6f6e 2e0a 2020 2020 2020  function..      
+00002800: 2020 0a20 2020 2020 2020 204e 6f74 6573    .        Notes
+00002810: 0a20 2020 2020 2020 202d 2d2d 2d2d 0a20  .        -----. 
+00002820: 2020 2020 2020 202d 2054 6869 7320 6d65         - This me
+00002830: 7468 6f64 2061 6c6c 6f77 7320 7375 6263  thod allows subc
+00002840: 6c61 7373 6573 2074 6f20 7265 7374 7269  lasses to restri
+00002850: 6374 2074 6865 206f 626a 6563 7420 7479  ct the object ty
+00002860: 7065 7320 7468 6174 2074 6865 790a 2020  pes that they.  
+00002870: 2020 2020 2020 2020 7061 7373 2074 6f20          pass to 
+00002880: 606e 756d 7079 6020 7075 626c 6963 2066  `numpy` public f
+00002890: 756e 6374 696f 6e73 2076 6961 2060 5f61  unctions via `_a
+000028a0: 7070 6c79 5f66 756e 6374 696f 6e60 2e0a  pply_function`..
+000028b0: 2020 2020 2020 2020 2d20 5468 6520 6465          - The de
+000028c0: 6661 756c 7420 696d 706c 656d 656e 7461  fault implementa
+000028d0: 7469 6f6e 2072 6574 7572 6e73 2061 2074  tion returns a t
+000028e0: 7570 6c65 2074 6861 7420 636f 6e74 6169  uple that contai
+000028f0: 6e73 2061 6c6c 2074 7970 6573 0a20 2020  ns all types.   
+00002900: 2020 2020 2020 2065 7863 6570 7420 666f         except fo
+00002910: 7220 7375 6274 7970 6573 206f 6620 607e  r subtypes of `~
+00002920: 4f62 6a65 6374 602e 0a20 2020 2020 2020  Object`..       
+00002930: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00002940: 7572 6e20 7475 706c 6528 0a20 2020 2020  urn tuple(.     
+00002950: 2020 2020 2020 2074 6920 666f 7220 7469         ti for ti
+00002960: 2069 6e20 7479 7065 730a 2020 2020 2020   in types.      
+00002970: 2020 2020 2020 6966 206e 6f74 2069 7373        if not iss
+00002980: 7562 636c 6173 7328 7469 2c20 4f62 6a65  ubclass(ti, Obje
+00002990: 6374 290a 2020 2020 2020 2020 290a 0a20  ct).        ).. 
+000029a0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+000029b0: 2020 2020 6465 6620 5f69 6d70 6c65 6d65      def _impleme
+000029c0: 6e74 7328 636c 732c 206f 7065 7261 7469  nts(cls, operati
+000029d0: 6f6e 3a20 7479 7069 6e67 2e43 616c 6c61  on: typing.Calla
+000029e0: 626c 6529 3a0a 2020 2020 2020 2020 2222  ble):.        ""
+000029f0: 2254 7275 6520 6966 2074 6869 7320 636c  "True if this cl
+00002a00: 6173 7320 6465 6669 6e65 7320 6120 6375  ass defines a cu
+00002a10: 7374 6f6d 2069 6d70 6c65 6d65 6e74 6174  stom implementat
+00002a20: 696f 6e20 666f 7220 606f 7065 7261 7469  ion for `operati
+00002a30: 6f6e 602e 0a20 2020 2020 2020 200a 2020  on`..        .  
+00002a40: 2020 2020 2020 5468 6973 2069 7320 6120        This is a 
+00002a50: 6865 6c70 6572 206d 6574 686f 6473 2074  helper methods t
+00002a60: 6861 7420 6772 6163 6566 756c 6c79 2068  hat gracefully h
+00002a70: 616e 646c 6573 2074 6865 2063 6173 6520  andles the case 
+00002a80: 696e 2077 6869 6368 2061 0a20 2020 2020  in which a.     
+00002a90: 2020 2073 7562 636c 6173 7320 646f 6573     subclass does
+00002aa0: 206e 6f74 2073 7570 706f 7274 2063 7573   not support cus
+00002ab0: 746f 6d20 6f70 6572 6174 6f72 2069 6d70  tom operator imp
+00002ac0: 6c65 6d65 6e74 6174 696f 6e73 2e0a 2020  lementations..  
+00002ad0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00002ae0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00002af0: 2020 2072 6573 756c 7420 3d20 6f70 6572     result = oper
+00002b00: 6174 696f 6e20 696e 2063 6c73 2e5f 4655  ation in cls._FU
+00002b10: 4e43 5449 4f4e 530a 2020 2020 2020 2020  NCTIONS.        
+00002b20: 6578 6365 7074 2054 7970 6545 7272 6f72  except TypeError
+00002b30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00002b40: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00002b50: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00002b60: 0a0a 2020 2020 5f46 554e 4354 494f 4e53  ..    _FUNCTIONS
+00002b70: 3a20 7479 7069 6e67 2e44 6963 745b 7374  : typing.Dict[st
+00002b80: 722c 2074 7970 696e 672e 4361 6c6c 6162  r, typing.Callab
+00002b90: 6c65 5d3d 4e6f 6e65 0a20 2020 2022 2222  le]=None.    """
+00002ba0: 496e 7465 726e 616c 2063 6f6c 6c65 6374  Internal collect
+00002bb0: 696f 6e20 6f66 2063 7573 746f 6d20 606e  ion of custom `n
+00002bc0: 756d 7079 6020 6675 6e63 7469 6f6e 2069  umpy` function i
+00002bd0: 6d70 6c65 6d65 6e74 6174 696f 6e73 2e22  mplementations."
+00002be0: 2222 0a0a 2020 2020 4063 6c61 7373 6d65  ""..    @classme
+00002bf0: 7468 6f64 0a20 2020 2064 6566 2069 6d70  thod.    def imp
+00002c00: 6c65 6d65 6e74 7328 636c 732c 206e 756d  lements(cls, num
+00002c10: 7079 5f66 756e 6374 696f 6e3a 2074 7970  py_function: typ
+00002c20: 696e 672e 4361 6c6c 6162 6c65 293a 0a20  ing.Callable):. 
+00002c30: 2020 2020 2020 2022 2222 5265 6769 7374         """Regist
+00002c40: 6572 2061 2063 7573 746f 6d20 696d 706c  er a custom impl
+00002c50: 656d 656e 7461 7469 6f6e 206f 6620 7468  ementation of th
+00002c60: 6973 2060 6e75 6d70 7960 2066 756e 6374  is `numpy` funct
+00002c70: 696f 6e2e 0a0a 2020 2020 2020 2020 5061  ion...        Pa
+00002c80: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00002c90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00002ca0: 2020 2020 6e75 6d70 795f 6675 6e63 7469      numpy_functi
+00002cb0: 6f6e 203a 2063 616c 6c61 626c 650a 2020  on : callable.  
+00002cc0: 2020 2020 2020 2020 2020 5468 6520 606e            The `n
+00002cd0: 756d 7079 6020 756e 6976 6572 7361 6c20  umpy` universal 
+00002ce0: 6f72 2070 7562 6c69 6320 6675 6e63 7469  or public functi
+00002cf0: 6f6e 2074 6f20 696d 706c 656d 656e 742e  on to implement.
+00002d00: 0a0a 2020 2020 2020 2020 4e6f 7465 730a  ..        Notes.
+00002d10: 2020 2020 2020 2020 2d2d 2d2d 2d0a 2020          -----.  
+00002d20: 2020 2020 2020 2d20 5573 6572 7320 6d61        - Users ma
+00002d30: 7920 7265 6769 7374 6572 2060 6e75 6d70  y register `nump
+00002d40: 7960 2075 6e69 7665 7273 616c 2066 756e  y` universal fun
+00002d50: 6374 696f 6e73 2028 612e 6b2e 612e 2075  ctions (a.k.a. u
+00002d60: 6675 6e63 733b 0a20 2020 2020 2020 2020  funcs;.         
+00002d70: 2068 7474 7073 3a2f 2f6e 756d 7079 2e6f   https://numpy.o
+00002d80: 7267 2f64 6f63 2f73 7461 626c 652f 7265  rg/doc/stable/re
+00002d90: 6665 7265 6e63 652f 7566 756e 6373 2e68  ference/ufuncs.h
+00002da0: 746d 6c29 2061 7320 7765 6c6c 2061 730a  tml) as well as.
+00002db0: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
+00002dc0: 6f6e 7320 696e 2074 6865 2070 7562 6c69  ons in the publi
+00002dd0: 6320 606e 756d 7079 6020 4150 4920 2865  c `numpy` API (e
+00002de0: 2e67 2e2c 2060 6e75 6d70 792e 6d65 616e  .g., `numpy.mean
+00002df0: 6029 2e20 5468 6973 206d 6179 2062 650a  `). This may be.
+00002e00: 2020 2020 2020 2020 2020 696d 706f 7274            import
+00002e10: 616e 7420 6966 2c20 666f 7220 6578 616d  ant if, for exam
+00002e20: 706c 652c 2061 2063 6c61 7373 206e 6565  ple, a class nee
+00002e30: 6473 2074 6f20 696d 706c 656d 656e 7420  ds to implement 
+00002e40: 6120 6375 7374 6f6d 2076 6572 7369 6f6e  a custom version
+00002e50: 0a20 2020 2020 2020 2020 206f 6620 606e  .          of `n
+00002e60: 756d 7079 2e73 7172 7460 2c20 7768 6963  umpy.sqrt`, whic
+00002e70: 6820 6973 2061 2075 6675 6e63 2e0a 2020  h is a ufunc..  
+00002e80: 2020 2020 2020 2d20 5365 6520 6874 7470        - See http
+00002e90: 733a 2f2f 6e75 6d70 792e 6f72 672f 646f  s://numpy.org/do
+00002ea0: 632f 7374 6162 6c65 2f72 6566 6572 656e  c/stable/referen
+00002eb0: 6365 2f61 7272 6179 732e 636c 6173 7365  ce/arrays.classe
+00002ec0: 732e 6874 6d6c 2066 6f72 2074 6865 0a20  s.html for the. 
+00002ed0: 2020 2020 2020 2020 2073 7567 6765 7374           suggest
+00002ee0: 696f 6e20 6f6e 2077 6869 6368 2074 6869  ion on which thi
+00002ef0: 7320 6d65 7468 6f64 2069 7320 6261 7365  s method is base
+00002f00: 642e 0a0a 2020 2020 2020 2020 4578 616d  d...        Exam
+00002f10: 706c 6573 0a20 2020 2020 2020 202d 2d2d  ples.        ---
+00002f20: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4f76  -----.        Ov
+00002f30: 6572 6c6f 6164 2060 6e75 6d70 792e 6d65  erload `numpy.me
+00002f40: 616e 6020 666f 7220 616e 2065 7869 7374  an` for an exist
+00002f50: 696e 6720 636c 6173 7320 6361 6c6c 6564  ing class called
+00002f60: 2060 4172 7261 7960 2077 6974 6820 610a   `Array` with a.
+00002f70: 2020 2020 2020 2020 7665 7273 696f 6e20          version 
+00002f80: 7468 6174 2061 6363 6570 7473 206e 6f20  that accepts no 
+00002f90: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00002fa0: 733a 0a0a 2020 2020 2020 2020 6060 600a  s:..        ```.
+00002fb0: 2020 2020 2020 2020 2020 2020 4041 7272              @Arr
+00002fc0: 6179 2e69 6d70 6c65 6d65 6e74 7328 6e75  ay.implements(nu
+00002fd0: 6d70 792e 6d65 616e 290a 2020 2020 2020  mpy.mean).      
+00002fe0: 2020 2020 2020 6465 6620 6d65 616e 2861        def mean(a
+00002ff0: 3a20 4172 7261 792c 202a 2a6b 7761 7267  : Array, **kwarg
+00003000: 7329 202d 3e20 4172 7261 793a 0a20 2020  s) -> Array:.   
+00003010: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003020: 6b77 6172 6773 3a0a 2020 2020 2020 2020  kwargs:.        
+00003030: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+00003040: 3d20 2243 616e 6e6f 7420 7061 7373 206b  = "Cannot pass k
+00003050: 6579 776f 7264 7320 746f 206e 756d 7079  eywords to numpy
+00003060: 2e6d 6561 6e20 7769 7468 2041 7272 6179  .mean with Array
+00003070: 2220 7261 6973 650a 2020 2020 2020 2020  " raise.        
+00003080: 2020 2020 2020 2020 2020 2020 5479 7065              Type
+00003090: 4572 726f 7228 6d73 6729 0a20 2020 2020  Error(msg).     
+000030a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000030b0: 6e20 6e75 6d70 792e 7375 6d28 6129 202f  n numpy.sum(a) /
+000030c0: 206c 656e 2861 290a 2020 2020 2020 2020   len(a).        
+000030d0: 6060 600a 0a20 2020 2020 2020 2054 6869  ```..        Thi
+000030e0: 7320 7769 6c6c 2063 6f6d 7075 7465 2074  s will compute t
+000030f0: 6865 206d 6561 6e20 6f66 2074 6865 2075  he mean of the u
+00003100: 6e64 6572 6c79 696e 6720 6461 7461 2077  nderlying data w
+00003110: 6865 6e20 6361 6c6c 6564 2077 6974 6820  hen called with 
+00003120: 6e6f 0a20 2020 2020 2020 2061 7267 756d  no.        argum
+00003130: 656e 7473 2c20 6275 7420 7769 6c6c 2072  ents, but will r
+00003140: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
+00003150: 6e20 7768 656e 2063 616c 6c65 6420 7769  n when called wi
+00003160: 7468 2061 7267 756d 656e 7473 3a0a 0a20  th arguments:.. 
+00003170: 2020 2020 2020 2020 2020 203e 3e3e 2076             >>> v
+00003180: 203d 2041 7272 6179 285b 5b31 2c20 325d   = Array([[1, 2]
+00003190: 2c20 5b33 2c20 345d 5d29 0a20 2020 2020  , [3, 4]]).     
+000031a0: 2020 2020 2020 203e 3e3e 206e 756d 7079         >>> numpy
+000031b0: 2e6d 6561 6e28 7629 0a20 2020 2020 2020  .mean(v).       
+000031c0: 2020 2020 2035 2e30 0a20 2020 2020 2020       5.0.       
+000031d0: 2020 2020 203e 3e3e 206e 756d 7079 2e6d       >>> numpy.m
+000031e0: 6561 6e28 762c 2061 7869 733d 3029 0a20  ean(v, axis=0). 
+000031f0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
+00003200: 2020 2020 2020 2020 2020 2054 7970 6545             TypeE
+00003210: 7272 6f72 3a20 4361 6e6e 6f74 2070 6173  rror: Cannot pas
+00003220: 7320 6b65 7977 6f72 6473 2074 6f20 6e75  s keywords to nu
+00003230: 6d70 792e 6d65 616e 2077 6974 6820 4172  mpy.mean with Ar
+00003240: 7261 790a 2020 2020 2020 2020 2222 220a  ray.        """.
+00003250: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00003260: 616c 6c61 626c 6528 6e75 6d70 795f 6675  allable(numpy_fu
+00003270: 6e63 7469 6f6e 293a 0a20 2020 2020 2020  nction):.       
+00003280: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00003290: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+000032a0: 2020 2020 2020 2254 6865 2074 6172 6765        "The targe
+000032b0: 7420 6f70 6572 6174 696f 6e20 6f66 2061  t operation of a
+000032c0: 2063 7573 746f 6d20 6e75 6d70 7920 696d   custom numpy im
+000032d0: 706c 656d 656e 7461 7469 6f6e 220a 2020  plementation".  
+000032e0: 2020 2020 2020 2020 2020 2020 2020 2220                " 
+000032f0: 6d75 7374 2062 6520 6361 6c6c 6162 6c65  must be callable
+00003300: 220a 2020 2020 2020 2020 2020 2020 2920  ".            ) 
+00003310: 6672 6f6d 204e 6f6e 650a 2020 2020 2020  from None.      
+00003320: 2020 6465 6620 6465 636f 7261 746f 7228    def decorator(
+00003330: 7573 6572 5f66 756e 6374 696f 6e3a 2055  user_function: U
+00003340: 7365 7246 756e 6374 696f 6e29 3a0a 2020  serFunction):.  
+00003350: 2020 2020 2020 2020 2020 6966 2063 6c73            if cls
+00003360: 2e5f 4655 4e43 5449 4f4e 5320 6973 204e  ._FUNCTIONS is N
+00003370: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00003380: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+00003390: 706c 656d 656e 7465 6445 7272 6f72 280a  plementedError(.
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 2020 2020 6622 5479 7065 207b 636c 737d      f"Type {cls}
+000033c0: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+000033d0: 7420 6375 7374 6f6d 2069 6d70 6c65 6d65  t custom impleme
+000033e0: 6e74 6174 696f 6e73 220a 2020 2020 2020  ntations".      
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2220                " 
+00003400: 6f66 206e 756d 7079 2066 756e 6374 696f  of numpy functio
+00003410: 6e73 220a 2020 2020 2020 2020 2020 2020  ns".            
+00003420: 2020 2020 2920 6672 6f6d 204e 6f6e 650a      ) from None.
+00003430: 2020 2020 2020 2020 2020 2020 636c 732e              cls.
+00003440: 5f46 554e 4354 494f 4e53 5b6e 756d 7079  _FUNCTIONS[numpy
+00003450: 5f66 756e 6374 696f 6e5d 203d 2075 7365  _function] = use
+00003460: 725f 6675 6e63 7469 6f6e 0a20 2020 2020  r_function.     
+00003470: 2020 2020 2020 2072 6574 7572 6e20 7573         return us
+00003480: 6572 5f66 756e 6374 696f 6e0a 2020 2020  er_function.    
+00003490: 2020 2020 7265 7475 726e 2064 6563 6f72      return decor
+000034a0: 6174 6f72 0a0a 0a63 6c61 7373 204f 7065  ator...class Ope
+000034b0: 7261 746f 7273 2846 756e 6374 696f 6e73  rators(Functions
+000034c0: 293a 0a20 2020 2022 2222 5375 7070 6f72  ):.    """Suppor
+000034d0: 7420 666f 7220 696d 706c 656d 656e 7469  t for implementi
+000034e0: 6e67 2063 7573 746f 6d20 6e75 6d65 7269  ng custom numeri
+000034f0: 6320 6f70 6572 6174 6f72 732e 2222 220a  c operators.""".
+00003500: 0a20 2020 2064 6566 205f 5f6f 626a 6563  .    def __objec
+00003510: 745f 6f70 6572 6174 6f72 5f5f 2873 656c  t_operator__(sel
+00003520: 662c 206f 7065 7261 7469 6f6e 2c20 2a61  f, operation, *a
+00003530: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00003540: 2020 2020 2020 2020 2222 2241 7070 6c79          """Apply
+00003550: 2060 6f70 6572 6174 696f 6e60 2074 6f20   `operation` to 
+00003560: 7468 6520 6769 7665 6e20 6172 6775 6d65  the given argume
+00003570: 6e74 732e 0a0a 2020 2020 2020 2020 4e6f  nts...        No
+00003580: 7465 730a 2020 2020 2020 2020 2d2d 2d2d  tes.        ----
+00003590: 2d0a 2020 2020 2020 2020 2d20 5468 6973  -.        - This
+000035a0: 206d 6574 686f 6420 6973 2062 6173 6564   method is based
+000035b0: 206f 6e20 7468 6520 6d65 7468 6f64 7320   on the methods 
+000035c0: 607e 5f5f 6172 7261 795f 7566 756e 635f  `~__array_ufunc_
+000035d0: 5f60 2061 6e64 0a20 2020 2020 2020 2020  _` and.         
+000035e0: 2060 7e5f 5f61 7272 6179 5f66 756e 6374   `~__array_funct
+000035f0: 696f 6e5f 5f60 2c20 7768 6963 6820 7375  ion__`, which su
+00003600: 7070 6f72 7420 6375 7374 6f6d 2069 6d70  pport custom imp
+00003610: 6c65 6d65 6e74 6174 696f 6e73 206f 6620  lementations of 
+00003620: 606e 756d 7079 600a 2020 2020 2020 2020  `numpy`.        
+00003630: 2020 756e 6976 6572 7361 6c20 6675 6e63    universal func
+00003640: 7469 6f6e 7320 616e 6420 7075 626c 6963  tions and public
+00003650: 2066 756e 6374 696f 6e73 2c20 7265 7370   functions, resp
+00003660: 6563 7469 7665 6c79 2e0a 2020 2020 2020  ectively..      
+00003670: 2020 2d20 5468 6520 6e61 6d65 206f 6620    - The name of 
+00003680: 7468 6973 206d 6574 686f 6420 6973 2073  this method is s
+00003690: 7562 6a65 6374 2074 6f20 6368 616e 6765  ubject to change
+000036a0: 2077 6974 686f 7574 206e 6f74 6963 6520   without notice 
+000036b0: 696e 2074 6865 0a20 2020 2020 2020 2020  in the.         
+000036c0: 2065 7665 6e74 2074 6861 7420 6974 2063   event that it c
+000036d0: 6f6e 666c 6963 7473 2077 6974 6820 6120  onflicts with a 
+000036e0: 7374 616e 6461 7264 2d6c 6962 7261 7279  standard-library
+000036f0: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
+00003700: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00003710: 7365 6c66 2e5f 696d 706c 656d 656e 7473  self._implements
+00003720: 286f 7065 7261 7469 6f6e 293a 0a20 2020  (operation):.   
+00003730: 2020 2020 2020 2020 206f 7065 7261 746f           operato
+00003740: 7220 3d20 7365 6c66 2e5f 4f50 4552 4154  r = self._OPERAT
+00003750: 4f52 535b 5f6f 7065 7261 7469 6f6e 732e  ORS[_operations.
+00003760: 7265 736f 6c76 6528 6f70 6572 6174 696f  resolve(operatio
+00003770: 6e29 5d0a 2020 2020 2020 2020 2020 2020  n)].            
+00003780: 7265 7475 726e 206f 7065 7261 746f 7228  return operator(
+00003790: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+000037a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000037b0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 0a0a  NotImplemented..
+000037c0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+000037d0: 0a20 2020 2064 6566 205f 696d 706c 656d  .    def _implem
+000037e0: 656e 7473 2863 6c73 2c20 6f70 6572 6174  ents(cls, operat
+000037f0: 696f 6e3a 2074 7970 696e 672e 556e 696f  ion: typing.Unio
+00003800: 6e5b 7374 722c 2074 7970 696e 672e 4361  n[str, typing.Ca
+00003810: 6c6c 6162 6c65 5d29 3a0a 2020 2020 2020  llable]):.      
+00003820: 2020 2222 2254 7275 6520 6966 2074 6869    """True if thi
+00003830: 7320 636c 6173 7320 6465 6669 6e65 7320  s class defines 
+00003840: 6120 6375 7374 6f6d 2069 6d70 6c65 6d65  a custom impleme
+00003850: 6e74 6174 696f 6e20 666f 7220 606f 7065  ntation for `ope
+00003860: 7261 7469 6f6e 602e 0a20 2020 2020 2020  ration`..       
+00003870: 200a 2020 2020 2020 2020 5468 6973 2069   .        This i
+00003880: 7320 6120 6865 6c70 6572 206d 6574 686f  s a helper metho
+00003890: 6473 2074 6861 7420 6772 6163 6566 756c  ds that graceful
+000038a0: 6c79 2068 616e 646c 6573 2074 6865 2063  ly handles the c
+000038b0: 6173 6520 696e 2077 6869 6368 2061 0a20  ase in which a. 
+000038c0: 2020 2020 2020 2073 7562 636c 6173 7320         subclass 
+000038d0: 646f 6573 206e 6f74 2073 7570 706f 7274  does not support
+000038e0: 2063 7573 746f 6d20 6f70 6572 6174 6f72   custom operator
+000038f0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
+00003900: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00003910: 2020 2020 2020 7461 7267 6574 203d 205f        target = _
+00003920: 6f70 6572 6174 696f 6e73 2e72 6573 6f6c  operations.resol
+00003930: 7665 286f 7065 7261 7469 6f6e 290a 2020  ve(operation).  
+00003940: 2020 2020 2020 6966 2074 6172 6765 7420        if target 
+00003950: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00003960: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00003970: 7228 292e 5f69 6d70 6c65 6d65 6e74 7328  r()._implements(
+00003980: 6f70 6572 6174 696f 6e29 0a20 2020 2020  operation).     
+00003990: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000039a0: 2020 2020 7265 7375 6c74 203d 2074 6172      result = tar
+000039b0: 6765 7420 696e 2063 6c73 2e5f 4f50 4552  get in cls._OPER
+000039c0: 4154 4f52 530a 2020 2020 2020 2020 6578  ATORS.        ex
+000039d0: 6365 7074 2054 7970 6545 7272 6f72 3a0a  cept TypeError:.
+000039e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000039f0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00003a00: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00003a10: 2020 2020 5f4f 5045 5241 544f 5253 3a20      _OPERATORS: 
+00003a20: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
+00003a30: 2074 7970 696e 672e 4361 6c6c 6162 6c65   typing.Callable
+00003a40: 5d3d 4e6f 6e65 0a20 2020 2022 2222 496e  ]=None.    """In
+00003a50: 7465 726e 616c 2063 6f6c 6c65 6374 696f  ternal collectio
+00003a60: 6e20 6f66 2063 7573 746f 6d20 6275 696c  n of custom buil
+00003a70: 742d 696e 206f 7065 7261 746f 7220 696d  t-in operator im
+00003a80: 706c 656d 656e 7461 7469 6f6e 732e 2222  plementations.""
+00003a90: 220a 0a20 2020 2040 636c 6173 736d 6574  "..    @classmet
+00003aa0: 686f 640a 2020 2020 6465 6620 696d 706c  hod.    def impl
+00003ab0: 656d 656e 7473 2863 6c73 2c20 6f70 6572  ements(cls, oper
+00003ac0: 6174 696f 6e3a 2074 7970 696e 672e 556e  ation: typing.Un
+00003ad0: 696f 6e5b 7374 722c 2074 7970 696e 672e  ion[str, typing.
+00003ae0: 4361 6c6c 6162 6c65 5d29 3a0a 2020 2020  Callable]):.    
+00003af0: 2020 2020 2222 2252 6567 6973 7465 7220      """Register 
+00003b00: 6120 6375 7374 6f6d 2069 6d70 6c65 6d65  a custom impleme
+00003b10: 6e74 6174 696f 6e20 6f66 2060 6f70 6572  ntation of `oper
+00003b20: 6174 696f 6e60 2e0a 0a20 2020 2020 2020  ation`...       
+00003b30: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00003b40: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00003b50: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
+00003b60: 203a 2073 7472 696e 6720 6f72 2063 616c   : string or cal
+00003b70: 6c61 626c 650a 2020 2020 2020 2020 2020  lable.          
+00003b80: 2020 5468 6520 6f70 6572 6174 696f 6e20    The operation 
+00003b90: 746f 2069 6d70 6c65 6d65 6e74 2e20 5468  to implement. Th
+00003ba0: 6520 6172 6775 6d65 6e74 206d 6179 2062  e argument may b
+00003bb0: 6520 7468 6520 6361 6e6f 6e69 6361 6c0a  e the canonical.
+00003bc0: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
+00003bd0: 6162 6c65 206f 626a 6563 7420 636f 7272  able object corr
+00003be0: 6573 706f 6e64 696e 6720 746f 2074 6865  esponding to the
+00003bf0: 2074 6172 6765 7420 6f70 6572 6174 696f   target operatio
+00003c00: 6e20 2865 2e67 2e2c 0a20 2020 2020 2020  n (e.g.,.       
+00003c10: 2020 2020 2060 6e75 6d70 792e 6164 6460       `numpy.add`
+00003c20: 206f 7220 606f 7065 7261 746f 722e 6164   or `operator.ad
+00003c30: 6460 292c 206f 7220 6120 6b6e 6f77 6e20  d`), or a known 
+00003c40: 616c 6961 7320 666f 7220 7468 6520 6f70  alias for the op
+00003c50: 6572 6174 696f 6e0a 2020 2020 2020 2020  eration.        
+00003c60: 2020 2020 2865 2e67 2e2c 2060 2761 6464      (e.g., `'add
+00003c70: 2760 292e 0a0a 2020 2020 2020 2020 5265  '`)...        Re
+00003c80: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00003c90: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6074  -----.        `t
+00003ca0: 7970 696e 672e 4361 6c6c 6162 6c65 600a  yping.Callable`.
+00003cb0: 2020 2020 2020 2020 2020 2020 4120 6675              A fu
+00003cc0: 6e63 7469 6f6e 2077 6974 6820 7768 6963  nction with whic
+00003cd0: 6820 746f 2064 6563 6f72 6174 6520 7468  h to decorate th
+00003ce0: 6520 6375 7374 6f6d 2069 6d70 6c65 6d65  e custom impleme
+00003cf0: 6e74 6174 696f 6e2e 0a20 2020 2020 2020  ntation..       
+00003d00: 2022 2222 0a20 2020 2020 2020 2074 6172   """.        tar
+00003d10: 6765 7420 3d20 5f6f 7065 7261 7469 6f6e  get = _operation
+00003d20: 732e 7265 736f 6c76 6528 6f70 6572 6174  s.resolve(operat
+00003d30: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
+00003d40: 7461 7267 6574 206e 6f74 2069 6e20 5f6f  target not in _o
+00003d50: 7065 7261 7469 6f6e 732e 4655 4e43 5449  perations.FUNCTI
+00003d60: 4f4e 532e 7661 6c75 6573 2829 3a0a 2020  ONS.values():.  
+00003d70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00003d80: 2073 7570 6572 2829 2e69 6d70 6c65 6d65   super().impleme
+00003d90: 6e74 7328 6f70 6572 6174 696f 6e29 0a20  nts(operation). 
+00003da0: 2020 2020 2020 2064 6566 2064 6563 6f72         def decor
+00003db0: 6174 6f72 2875 7365 725f 6675 6e63 7469  ator(user_functi
+00003dc0: 6f6e 3a20 5573 6572 4675 6e63 7469 6f6e  on: UserFunction
+00003dd0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00003de0: 6620 636c 732e 5f4f 5045 5241 544f 5253  f cls._OPERATORS
+00003df0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00003e00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00003e10: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00003e20: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00003e30: 2020 2020 2020 2020 2066 2254 7970 6520           f"Type 
+00003e40: 7b63 6c73 7d20 646f 6573 206e 6f74 2073  {cls} does not s
+00003e50: 7570 706f 7274 2063 7573 746f 6d20 6f70  upport custom op
+00003e60: 6572 6174 6f72 7322 0a20 2020 2020 2020  erators".       
+00003e70: 2020 2020 2020 2020 2029 2066 726f 6d20           ) from 
+00003e80: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00003e90: 2063 6c73 2e5f 4f50 4552 4154 4f52 535b   cls._OPERATORS[
+00003ea0: 7461 7267 6574 5d20 3d20 7573 6572 5f66  target] = user_f
+00003eb0: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
+00003ec0: 2020 2020 7265 7475 726e 2075 7365 725f      return user_
+00003ed0: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
+00003ee0: 2072 6574 7572 6e20 6465 636f 7261 746f   return decorato
+00003ef0: 720a 0a0a                                r...
```

### Comparing `eprempy-0.5.5/src/eprempy/numeric/_array.py` & `eprempy-0.6.0/src/eprempy/numeric/_array.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/_data.py` & `eprempy-0.6.0/src/eprempy/numeric/_data.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/_factory.py` & `eprempy-0.6.0/src/eprempy/numeric/_factory.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/_implementation.py` & `eprempy-0.6.0/src/eprempy/numeric/_implementation.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/_index.py` & `eprempy-0.6.0/src/eprempy/numeric/_index.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/_objects.py` & `eprempy-0.6.0/src/eprempy/numeric/_objects.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/_operations.py` & `eprempy-0.6.0/src/eprempy/numeric/_operations.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/numeric/_operators.py` & `eprempy-0.6.0/src/eprempy/numeric/_operators.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/observable/__init__.py` & `eprempy-0.6.0/src/eprempy/observable/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/observable/_interfaces.py` & `eprempy-0.6.0/src/eprempy/observable/_interfaces.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/observable/_objects.py` & `eprempy-0.6.0/src/eprempy/observable/_objects.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/parameter/__init__.py` & `eprempy-0.6.0/src/eprempy/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/parameter/_config.py` & `eprempy-0.6.0/src/eprempy/parameter/_config.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/parameter/_metadata.py` & `eprempy-0.6.0/src/eprempy/parameter/_metadata.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/parameter/_runtime.py` & `eprempy-0.6.0/src/eprempy/parameter/_runtime.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/parameter/_src.py` & `eprempy-0.6.0/src/eprempy/parameter/_src.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/parameter/reference.json` & `eprempy-0.6.0/src/eprempy/parameter/reference.json`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/parameter/reference.py` & `eprempy-0.6.0/src/eprempy/parameter/reference.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/paths.py` & `eprempy-0.6.0/src/eprempy/paths.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/__init__.py` & `eprempy-0.6.0/src/eprempy/physical/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_array.py` & `eprempy-0.6.0/src/eprempy/physical/_array.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_axes.py` & `eprempy-0.6.0/src/eprempy/physical/_axes.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_axis.py` & `eprempy-0.6.0/src/eprempy/physical/_axis.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_axis_factories.py` & `eprempy-0.6.0/src/eprempy/physical/_axis_factories.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_object.py` & `eprempy-0.6.0/src/eprempy/physical/_object.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_object_factories.py` & `eprempy-0.6.0/src/eprempy/physical/_object_factories.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_operations.py` & `eprempy-0.6.0/src/eprempy/physical/_operations.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_scalar.py` & `eprempy-0.6.0/src/eprempy/physical/_scalar.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_tensor.py` & `eprempy-0.6.0/src/eprempy/physical/_tensor.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_types.py` & `eprempy-0.6.0/src/eprempy/physical/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/physical/_vector.py` & `eprempy-0.6.0/src/eprempy/physical/_vector.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/project.py` & `eprempy-0.6.0/src/eprempy/project.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/quantity/__init__.py` & `eprempy-0.6.0/src/eprempy/quantity/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/quantity/_functions.py` & `eprempy-0.6.0/src/eprempy/quantity/_functions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/quantity/_measurement.py` & `eprempy-0.6.0/src/eprempy/quantity/_measurement.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/real/__init__.py` & `eprempy-0.6.0/src/eprempy/real/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/real/_array.py` & `eprempy-0.6.0/src/eprempy/real/_array.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/real/_objects.py` & `eprempy-0.6.0/src/eprempy/real/_objects.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/real/_types.py` & `eprempy-0.6.0/src/eprempy/real/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/reference.py` & `eprempy-0.6.0/src/eprempy/reference.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/symbolic/__init__.py` & `eprempy-0.6.0/src/eprempy/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/symbolic/_expression.py` & `eprempy-0.6.0/src/eprempy/symbolic/_expression.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/symbolic/_operand.py` & `eprempy-0.6.0/src/eprempy/symbolic/_operand.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/symbolic/_operator.py` & `eprempy-0.6.0/src/eprempy/symbolic/_operator.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/symbolic/_parser.py` & `eprempy-0.6.0/src/eprempy/symbolic/_parser.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/symbolic/_part.py` & `eprempy-0.6.0/src/eprempy/symbolic/_part.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/typehelp.py` & `eprempy-0.6.0/src/eprempy/typehelp.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/src/eprempy/universal.py` & `eprempy-0.6.0/src/eprempy/universal.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.5/PKG-INFO` & `eprempy-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eprempy
-Version: 0.5.5
+Version: 0.6.0
 Summary: Tools for working with EPREM simulation runs
 License: BSD 3-Clause
 Author: Matt Young
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

