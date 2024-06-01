# Comparing `tmp/popoll_backend-0.0.63.tar.gz` & `tmp/popoll_backend-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.63.tar", last modified: Sat Jun  1 07:57:40 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.64.tar", last modified: Sat Jun  1 08:04:35 2024, max compression
```

## Comparing `popoll_backend-0.0.63.tar` & `popoll_backend-0.0.64.tar`

### file list

```diff
@@ -1,90 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.273747 popoll_backend-0.0.63/
--rw-rw-rw-   0 root         (0) root         (0)        4 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/LICENSE
--rw-r--r--   0 root         (0) root         (0)      654 2024-06-01 07:57:40.273747 popoll_backend-0.0.63/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.256747 popoll_backend-0.0.63/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     8488 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.257747 popoll_backend-0.0.63/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.259747 popoll_backend-0.0.63/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      736 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.261747 popoll_backend-0.0.63/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/dates.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/empty.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/polls.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/users.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.268746 popoll_backend-0.0.63/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     3633 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/delete_old_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_all_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_all_sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1948 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.273747 popoll_backend-0.0.63/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2798 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-06-01 07:57:34.000000 popoll_backend-0.0.63/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 07:57:40.273747 popoll_backend-0.0.63/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.272746 popoll_backend-0.0.63/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_01_get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_02_create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_03_update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_04_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_08_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_09_create_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1857 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_10_get_user.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_11_update_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_12_delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_13_get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_14_create_date.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_15_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_16_update_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_17_delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_18_create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_19_update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_20_delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_21_get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_22_get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_23_get_create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_24_get_all_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_25_delete_old_dates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.916393 popoll_backend-0.0.64/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      654 2024-06-01 08:04:35.916393 popoll_backend-0.0.64/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.899393 popoll_backend-0.0.64/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     8554 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.900393 popoll_backend-0.0.64/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.902393 popoll_backend-0.0.64/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.904393 popoll_backend-0.0.64/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/polls.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.905393 popoll_backend-0.0.64/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.905393 popoll_backend-0.0.64/popoll_backend/query/all/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/all/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/all/delete_old_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/all/get_all_sessions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.911393 popoll_backend-0.0.64/popoll_backend/query/poll/
+-rw-rw-rw-   0 root         (0) root         (0)     1929 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_all_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1985 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/popoll_backend/query/poll/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.915393 popoll_backend-0.0.64/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-06-01 08:04:35.000000 popoll_backend-0.0.64/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3006 2024-06-01 08:04:35.000000 popoll_backend-0.0.64/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 08:04:35.000000 popoll_backend-0.0.64/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-06-01 08:04:35.000000 popoll_backend-0.0.64/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-06-01 08:04:35.000000 popoll_backend-0.0.64/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-06-01 08:04:30.000000 popoll_backend-0.0.64/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 08:04:35.916393 popoll_backend-0.0.64/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 08:04:35.915393 popoll_backend-0.0.64/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_01_get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_02_create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_03_update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_04_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_08_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_09_create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1857 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_10_get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_11_update_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_12_delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_13_get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_14_create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_15_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_16_update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_17_delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_18_create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_19_update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_20_delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_21_get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_22_get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_23_get_create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_24_get_all_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-06-01 08:04:17.000000 popoll_backend-0.0.64/tests/test_25_delete_old_dates.py
```

### Comparing `popoll_backend-0.0.63/PKG-INFO` & `popoll_backend-0.0.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.63
+Version: 0.0.64
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 License: Free
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `popoll_backend-0.0.63/popoll_backend/__main__.py` & `popoll_backend-0.0.64/popoll_backend/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,41 +9,40 @@
 
 from flask_cors import CORS
 from flask_restful import Api, Resource
 from functools import wraps
 from typing import Any, Dict
 
 from popoll_backend.model.payload.history import History
-from popoll_backend.query.create_answer import CreateAnswer
-from popoll_backend.query.create_date import CreateDate
-from popoll_backend.query.create_poll import CreatePoll
-from popoll_backend.query.create_user import CreateUser
-from popoll_backend.query.delete_answer import DeleteAnswer
-from popoll_backend.query.delete_date import DeleteDate
-from popoll_backend.query.delete_old_dates import DeleteOldDates
-from popoll_backend.query.delete_user import DeleteUser
-from popoll_backend.query.get_all_instruments import GetAllInstruments
-from popoll_backend.query.get_all_sessions import GetAllSession
-from popoll_backend.query.get_answer import GetAnswer
-from popoll_backend.query.get_date import GetDate
-from popoll_backend.query.get_date_details import GetDateDetails
-from popoll_backend.query.get_dates import GetDates
-from popoll_backend.query.get_instrument import GetInstrument
-from popoll_backend.query.get_instruments import GetInstruments
-from popoll_backend.query.get_poll import GetPoll
-from popoll_backend.query.get_search_answer import GetSearchAnswer
-from popoll_backend.query.get_session import GetSession
-from popoll_backend.query.get_user_details import GetUserDetails
-from popoll_backend.query.get_user_with_instruments import GetUserWithInstruments
-from popoll_backend.query.get_users import GetUsers
-from popoll_backend.query.update_answer import UpdateAnswer
-from popoll_backend.query.update_date import UpdateDate
-from popoll_backend.query.update_poll import UpdatePoll
-from popoll_backend.query.create_session import CreateSession
-from popoll_backend.query.update_user import UpdateUser
+from popoll_backend.query.poll.create_answer import CreateAnswer
+from popoll_backend.query.poll.create_date import CreateDate
+from popoll_backend.query.poll.create_poll import CreatePoll
+from popoll_backend.query.poll.create_user import CreateUser
+from popoll_backend.query.poll.delete_answer import DeleteAnswer
+from popoll_backend.query.poll.delete_date import DeleteDate
+from popoll_backend.query.all.delete_old_dates import DeleteOldDates
+from popoll_backend.query.poll.delete_user import DeleteUser
+from popoll_backend.query.poll.get_all_instruments import GetAllInstruments
+from popoll_backend.query.all.get_all_sessions import GetAllSession
+from popoll_backend.query.poll.get_answer import GetAnswer
+from popoll_backend.query.poll.get_date import GetDate
+from popoll_backend.query.poll.get_date_details import GetDateDetails
+from popoll_backend.query.poll.get_dates import GetDates
+from popoll_backend.query.poll.get_instruments import GetInstruments
+from popoll_backend.query.poll.get_poll import GetPoll
+from popoll_backend.query.poll.get_search_answer import GetSearchAnswer
+from popoll_backend.query.poll.get_session import GetSession
+from popoll_backend.query.poll.get_user_details import GetUserDetails
+from popoll_backend.query.poll.get_user_with_instruments import GetUserWithInstruments
+from popoll_backend.query.poll.get_users import GetUsers
+from popoll_backend.query.poll.update_answer import UpdateAnswer
+from popoll_backend.query.poll.update_date import UpdateDate
+from popoll_backend.query.poll.update_poll import UpdatePoll
+from popoll_backend.query.poll.create_session import CreateSession
+from popoll_backend.query.poll.update_user import UpdateUser
 
 
 app = flask.Flask(__name__)
 CORS(app)
 api = Api(app)
```

### Comparing `popoll_backend-0.0.63/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.64/popoll_backend/model/db/answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/popoll_backend/model/db/date.py` & `popoll_backend-0.0.64/popoll_backend/model/db/date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/popoll_backend/model/db/session.py` & `popoll_backend-0.0.64/popoll_backend/model/db/session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/popoll_backend/model/db/user_instruments.py` & `popoll_backend-0.0.64/popoll_backend/model/db/user_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/popoll_backend/model/payload/date_details.py` & `popoll_backend-0.0.64/popoll_backend/model/payload/date_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.64/popoll_backend/model/payload/history.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 class History(Payload):
     
     def __init__(self, request: flask.Request, response, kwargs):
         self.date = datetime.datetime.now().isoformat(sep='T', timespec='auto')
         self.method = request.method
         self.path = request.path
-        self.matching_path = request.url_rule.rule
         self.ip = request.headers.get('Host', None)
         self.sessionId = request.headers.get('SessionId', None)
         self.queryParams = kwargs
         self.body = request.data
         with contextlib.suppress(Exception):
             self.body_json = json.loads(request.data)
         self.response = response
```

### Comparing `popoll_backend-0.0.63/popoll_backend/model/payload/user_details.py` & `popoll_backend-0.0.64/popoll_backend/model/payload/user_details.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
 from popoll_backend.model import Payload
-from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
+from popoll_backend.model.db.user import User
 
 class UserDetailsDate():
     
-    def __init__(self, user: UserWithInstruments, date: Date, answers: List[Answer]):
+    def __init__(self, user: User, date: Date, answers: List[Answer]):
         self.date: Date = date
         _ans = [a for a in answers if a.user_id == user.id and a.date_id == date.id]
         self.answer: Optional[Answer] = _ans[0] if len(_ans) > 0 else None
         
 
 class UserDetails(Payload):
     
-    def __init__(self, user: UserWithInstruments, answers: List[Answer], dates: List[Date]):
-        self.user: UserWithInstruments = user
+    def __init__(self, user: User, answers: List[Answer], dates: List[Date]):
+        self.user: User = user
         self.dates: List[UserDetailsDate] = [UserDetailsDate(user, date, answers) for date in dates]
```

### Comparing `popoll_backend-0.0.63/popoll_backend/model/payload/user_with_instruments.py` & `popoll_backend-0.0.64/popoll_backend/model/payload/user_with_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/create_answer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sqlite3
 
 import flask
 
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import PollQuery, fetchlast, is_date_frozen
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast, is_date_frozen
 
 
 class CreateAnswer(PollQuery):
     
     user_id: int
     date_id: int
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/create_date.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/update_date.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import datetime
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import PollQuery, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast
 
 
-class CreateDate(PollQuery):
+class UpdateDate(PollQuery):
     
+    id: int
     title: str
     date: datetime.date
     time: Optional[datetime.time]
     end_time: Optional[datetime.time]
     is_frozen: bool
     
-    id: int
-    
-    def __init__(self, poll: str, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time], is_frozen: bool):
+    def __init__(self, poll: str, id: int, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time], is_frozen: bool):
         super().__init__(poll)
+        self.id = id
         self.title = title
         self.date = date
         self.time = time
         self.end_time = end_time
         self.is_frozen = is_frozen
-    
-    def process(self, cursor: sqlite3.Cursor) -> None:
-        self.id = cursor.execute('INSERT INTO dates(title, date, time, end_time, is_frozen) VALUES (?, ?, ?, ?, ?)', (self.title, self.date, self.time, self.end_time, self.is_frozen)).lastrowid
         
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        cursor.execute('UPDATE dates SET title=?, date=?, time=?, end_time=?, is_frozen=? WHERE id=?', (self.title, self.date, self.time, self.end_time, self.is_frozen, self.id))
+    
     def buildResponse(self, cursor: sqlite3.Cursor) -> Date:
         return fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/create_poll.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.option import Option
 from popoll_backend.model.db.session import Session
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import PollQuery
+from popoll_backend.query.poll import PollQuery
 
 
 class CreatePoll(PollQuery):
     
     fail_if_db_exists: bool = True
     fail_if_db_not_exists: bool = False
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/create_session.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/create_session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import datetime
 import sqlite3
 
 from popoll_backend.model.db.session import Session
-from popoll_backend.query import PollQuery, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast
 
 
 class CreateSession(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: str, user_id: int):
         super().__init__(poll)
         self.id = id
         self.user_id = user_id
 
     def process(self, cursor: sqlite3.Cursor) -> None:
         cursor.execute('DELETE FROM sessions WHERE session_id=?', (self.id,))
-        return cursor.execute('INSERT INTO sessions(session_id, user_id, datetime) VALUES(?, ?, ?)', (self.id, self.user_id, self.getNow())).lastrowid
+        cursor.execute('INSERT INTO sessions(session_id, user_id, datetime) VALUES(?, ?, ?)', (self.id, self.user_id, self.getNow())).lastrowid
 
     def buildResponse(self, cursor: sqlite3.Cursor) -> Session:
         return fetchlast(cursor.execute('SELECT * FROM sessions WHERE session_id=?', (self.id,)), Session)
     
     def getNow(self) -> str:
         return datetime.datetime.now().isoformat(sep='T', timespec='auto')
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/create_user.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/update_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-import flask
 import sqlite3
 from typing import List
 
+import flask
+
 from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import PollQuery, fetchall, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall, fetchlast
 
 
-class CreateUser(PollQuery):
+class UpdateUser(PollQuery):
     
+    id: int
     name: str
     main_instrument: int
     instruments: List[int]
     
-    id: int
-    
-    def __init__(self, poll: str, name: str, main_instrument: int, instruments: List[int]):
+    def __init__(self, poll, id, name, main_instrument, instruments):
         super().__init__(poll)
+        self.id = id
         self.name = name
         self.main_instrument = main_instrument
         self.instruments = instruments
     
-    def process(self, cursor: sqlite3.Cursor) -> None:
-        self.id = cursor.execute('INSERT INTO users(name) VALUES(?)', (self.name,)).lastrowid
+    def process(self, cursor: sqlite3.Cursor):
+        cursor.execute('UPDATE users SET name=? WHERE id=?', (self.name, self.id))
+        cursor.execute('DELETE FROM user_instruments WHERE user_id=?', (self.id,))
         rows = [(self.id, self.main_instrument, True)] + [(self.id, instru, False) for instru in self.instruments if not instru == self.main_instrument]
         cursor.executemany('INSERT INTO user_instruments(user_id, instrument_id, is_main) VALUES(?, ?, ?)', rows)
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
         return UserWithInstruments(
             user=fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
             instruments=fetchall(cursor.execute('SELECT * FROM instruments'), Instrument), 
             user_instruments=fetchall(cursor.execute('SELECT * from user_instruments where user_id=?', (self.id,)), UserInstruments)
         )
     
     def error(self, e: sqlite3.Error):
         if isinstance(e, sqlite3.IntegrityError):
             if e.sqlite_errorcode == sqlite3.SQLITE_CONSTRAINT_UNIQUE:
-                flask.abort(409, f'User with name {self.name} already exists.')
+                flask.abort(409, f'User with name {self.name} already exists, cannot update.')
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/delete_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import sqlite3
 from popoll_backend.model import Payload
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import PollQuery
+from popoll_backend.query.poll import PollQuery
 
 
-class DeleteAnswer(PollQuery):
+class DeleteUser(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
     
     def process(self, cursor: sqlite3.Cursor) -> None:
-        cursor.execute('DELETE FROM answers WHERE id=?', (self.id,))
+        cursor.execute('DELETE FROM users WHERE id=?', (self.id,))
     
     def buildResponse(self, _: sqlite3.Cursor) -> IdPayload:
         return Empty()
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/delete_date.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sqlite3
 from popoll_backend.model import Payload
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import PollQuery
+from popoll_backend.query.poll import PollQuery
 
 
 class DeleteDate(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/delete_old_dates.py` & `popoll_backend-0.0.64/popoll_backend/query/all/delete_old_dates.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
 import sqlite3
 from typing import List, Tuple
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.payload.empty import Empty
-from popoll_backend.query import Query, fetchall
+from popoll_backend.query.all import Query
+from popoll_backend.query import fetchall
 
 def dateBefore(day=datetime.date.today(), years: int=0, days: int=0):
     today = day.isoformat()
     beforeYears = today[0:3] + str(int(today[3])-years) + today[4:] # big hack to replace year in string to get rid of bissectil years
     return (datetime.date.fromisoformat(beforeYears) - datetime.timedelta(days=days))
 
 class DeleteOldDates(Query):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/delete_answer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import sqlite3
 from popoll_backend.model import Payload
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import PollQuery
+from popoll_backend.query.poll import PollQuery
 
 
-class DeleteUser(PollQuery):
+class DeleteAnswer(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
     
     def process(self, cursor: sqlite3.Cursor) -> None:
-        cursor.execute('DELETE FROM users WHERE id=?', (self.id,))
+        cursor.execute('DELETE FROM answers WHERE id=?', (self.id,))
     
     def buildResponse(self, _: sqlite3.Cursor) -> IdPayload:
         return Empty()
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_all_instruments.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_all_instruments.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.instruments import Instruments
-from popoll_backend.query import PollQuery, fetchall
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall
 
 
 class GetAllInstruments(PollQuery):
     
     instruments: List[Instrument]
     
     def __init__(self, poll: str):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_all_sessions.py` & `popoll_backend-0.0.64/popoll_backend/query/all/get_all_sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import sqlite3
 from typing import List, Union
 
 from popoll_backend.model import Payload
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.polls import Poll, Polls
-from popoll_backend.query import Query
+from popoll_backend.query.all import Query
 
 
 class GetAllSession(Query):
     
-    id: int
+    id: str
     
     def __init__(self, id: str):
         self.id = id
         
     def process(self, db: str, cursor: sqlite3.Cursor) -> None:
         pass
         
     def buildResponse(self, db: str, cursor: sqlite3.Cursor) -> Union[Poll, Empty]:
         if cursor.execute('SELECT COUNT(*) FROM sessions WHERE session_id=?', (self.id,)).fetchone()[0] > 0:
             return Poll(db, cursor.execute('SELECT name FROM options').fetchone()[0])
         else:
             return Empty()
         
     def mergeResponses(self, answers: List[Payload]) -> Payload:
-        return Polls(polls=[a for a in answers if not a.isEmpty])
+        return Polls([a for a in answers if not a.isEmpty])
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_date.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_date.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sqlite3
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import PollQuery, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast
 
 
 class GetDate(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_date_details.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_date_details.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.date_details import DateDetails
-from popoll_backend.query import PollQuery, fetchall, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall, fetchlast
 
 
 class GetDateDetails(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_dates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.payload.dates import Dates
-from popoll_backend.query import PollQuery, fetchall
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall
 
 
 class GetDates(PollQuery):
     
     dates: List[Date]
     
     def __init__(self, poll: str):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_instrument.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_instrument.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sqlite3
 
 from popoll_backend.model.db.instrument import Instrument
-from popoll_backend.query import PollQuery, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast
 
 
 class GetInstrument(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_instruments.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.instruments import Instruments
-from popoll_backend.query import PollQuery, fetchall
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall
 
 
 class GetInstruments(PollQuery):
     
     instruments: List[Instrument]
     
     def __init__(self, poll: str):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_search_answer.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_search_answer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sqlite3
 
 import flask
 
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import PollQuery, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast
 
 
 class GetSearchAnswer(PollQuery):
     
     userId: int
     dateId: int
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_session.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sqlite3
 
 from popoll_backend.model.db.session import Session
-from popoll_backend.query import PollQuery, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast
 
 
 class GetSession(PollQuery):
     
     id: int
     session: Session
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_user_details.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_user_details.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sqlite3
 
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.user import User
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
 from popoll_backend.model.payload.user_details import UserDetails
-from popoll_backend.query import PollQuery, fetchall, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall, fetchlast
 
 
 class GetUserDetails(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_user_with_instruments.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_user_with_instruments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sqlite3
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import PollQuery, fetchall, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall, fetchlast
 
 
 class GetUserWithInstruments(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/get_users.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/get_users.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.users import Users
-from popoll_backend.query import PollQuery, fetchall
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall
 
 
 class GetUsers(PollQuery):
     
     def __init__(self, poll: str):
         super().__init__(poll)
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/update_answer.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/update_answer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sqlite3
 from typing import Optional
 
 import flask
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import PollQuery, fetchlast, get_date_id, is_date_frozen
-from popoll_backend.query.get_answer import GetAnswer
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast, get_date_id, is_date_frozen
 
 
 class UpdateAnswer(PollQuery):
     
     id: int
     response: Optional[bool]
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/update_date.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/create_date.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import datetime
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import PollQuery, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchlast
 
 
-class UpdateDate(PollQuery):
+class CreateDate(PollQuery):
     
-    id: int
     title: str
     date: datetime.date
     time: Optional[datetime.time]
     end_time: Optional[datetime.time]
     is_frozen: bool
     
-    def __init__(self, poll: str, id: int, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time], is_frozen: bool):
+    id: int
+    
+    def __init__(self, poll: str, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time], is_frozen: bool):
         super().__init__(poll)
-        self.id = id
         self.title = title
         self.date = date
         self.time = time
         self.end_time = end_time
         self.is_frozen = is_frozen
-        
-    def process(self, cursor: sqlite3.Cursor) -> None:
-        cursor.execute('UPDATE dates SET title=?, date=?, time=?, end_time=?, is_frozen=? WHERE id=?', (self.title, self.date, self.time, self.end_time, self.is_frozen, self.id))
     
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        self.id = cursor.execute('INSERT INTO dates(title, date, time, end_time, is_frozen) VALUES (?, ?, ?, ?, ?)', (self.title, self.date, self.time, self.end_time, self.is_frozen)).lastrowid
+        
     def buildResponse(self, cursor: sqlite3.Cursor) -> Date:
         return fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/update_poll.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/update_poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sqlite3
 
 from popoll_backend.model.db.option import Option
-from popoll_backend.query import PollQuery
+from popoll_backend.query.poll import PollQuery
 
 
 class UpdatePoll(PollQuery):
     
     name: str
     color: str
```

### Comparing `popoll_backend-0.0.63/popoll_backend/query/update_user.py` & `popoll_backend-0.0.64/popoll_backend/query/poll/create_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,43 @@
+import flask
 import sqlite3
 from typing import List
 
-import flask
-
 from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import PollQuery, fetchall, fetchlast
+from popoll_backend.query.poll import PollQuery
+from popoll_backend.query import fetchall, fetchlast
 
 
-class UpdateUser(PollQuery):
+class CreateUser(PollQuery):
     
-    id: int
     name: str
     main_instrument: int
     instruments: List[int]
     
-    def __init__(self, poll, id, name, main_instrument, instruments):
+    id: int
+    
+    def __init__(self, poll: str, name: str, main_instrument: int, instruments: List[int]):
         super().__init__(poll)
-        self.id = id
         self.name = name
         self.main_instrument = main_instrument
         self.instruments = instruments
     
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('UPDATE users SET name=? WHERE id=?', (self.name, self.id))
-        cursor.execute('DELETE FROM user_instruments WHERE user_id=?', (self.id,))
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        self.id = cursor.execute('INSERT INTO users(name) VALUES(?)', (self.name,)).lastrowid
         rows = [(self.id, self.main_instrument, True)] + [(self.id, instru, False) for instru in self.instruments if not instru == self.main_instrument]
         cursor.executemany('INSERT INTO user_instruments(user_id, instrument_id, is_main) VALUES(?, ?, ?)', rows)
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
         return UserWithInstruments(
             user=fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
             instruments=fetchall(cursor.execute('SELECT * FROM instruments'), Instrument), 
             user_instruments=fetchall(cursor.execute('SELECT * from user_instruments where user_id=?', (self.id,)), UserInstruments)
         )
     
     def error(self, e: sqlite3.Error):
         if isinstance(e, sqlite3.IntegrityError):
             if e.sqlite_errorcode == sqlite3.SQLITE_CONSTRAINT_UNIQUE:
-                flask.abort(409, f'User with name {self.name} already exists, cannot update.')
+                flask.abort(409, f'User with name {self.name} already exists.')
```

### Comparing `popoll_backend-0.0.63/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.64/popoll_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.63
+Version: 0.0.64
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 License: Free
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `popoll_backend-0.0.63/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.64/popoll_backend.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,41 +25,43 @@
 popoll_backend/model/payload/instruments.py
 popoll_backend/model/payload/polls.py
 popoll_backend/model/payload/user_details.py
 popoll_backend/model/payload/user_with_instruments.py
 popoll_backend/model/payload/users.py
 popoll_backend/model/payload/users_payload_details.py
 popoll_backend/query/__init__.py
-popoll_backend/query/create_answer.py
-popoll_backend/query/create_date.py
-popoll_backend/query/create_poll.py
-popoll_backend/query/create_session.py
-popoll_backend/query/create_user.py
-popoll_backend/query/delete_answer.py
-popoll_backend/query/delete_date.py
-popoll_backend/query/delete_old_dates.py
-popoll_backend/query/delete_user.py
-popoll_backend/query/get_all_instruments.py
-popoll_backend/query/get_all_sessions.py
-popoll_backend/query/get_answer.py
-popoll_backend/query/get_date.py
-popoll_backend/query/get_date_details.py
-popoll_backend/query/get_dates.py
-popoll_backend/query/get_instrument.py
-popoll_backend/query/get_instruments.py
-popoll_backend/query/get_poll.py
-popoll_backend/query/get_search_answer.py
-popoll_backend/query/get_session.py
-popoll_backend/query/get_user_details.py
-popoll_backend/query/get_user_with_instruments.py
-popoll_backend/query/get_users.py
-popoll_backend/query/update_answer.py
-popoll_backend/query/update_date.py
-popoll_backend/query/update_poll.py
-popoll_backend/query/update_user.py
+popoll_backend/query/all/__init__.py
+popoll_backend/query/all/delete_old_dates.py
+popoll_backend/query/all/get_all_sessions.py
+popoll_backend/query/poll/__init__.py
+popoll_backend/query/poll/create_answer.py
+popoll_backend/query/poll/create_date.py
+popoll_backend/query/poll/create_poll.py
+popoll_backend/query/poll/create_session.py
+popoll_backend/query/poll/create_user.py
+popoll_backend/query/poll/delete_answer.py
+popoll_backend/query/poll/delete_date.py
+popoll_backend/query/poll/delete_user.py
+popoll_backend/query/poll/get_all_instruments.py
+popoll_backend/query/poll/get_answer.py
+popoll_backend/query/poll/get_date.py
+popoll_backend/query/poll/get_date_details.py
+popoll_backend/query/poll/get_dates.py
+popoll_backend/query/poll/get_instrument.py
+popoll_backend/query/poll/get_instruments.py
+popoll_backend/query/poll/get_poll.py
+popoll_backend/query/poll/get_search_answer.py
+popoll_backend/query/poll/get_session.py
+popoll_backend/query/poll/get_user_details.py
+popoll_backend/query/poll/get_user_with_instruments.py
+popoll_backend/query/poll/get_users.py
+popoll_backend/query/poll/update_answer.py
+popoll_backend/query/poll/update_date.py
+popoll_backend/query/poll/update_poll.py
+popoll_backend/query/poll/update_user.py
 tests/test_01_get_poll.py
 tests/test_02_create_poll.py
 tests/test_03_update_poll.py
 tests/test_04_get_instruments.py
 tests/test_08_get_users.py
 tests/test_09_create_user.py
 tests/test_10_get_user.py
```

### Comparing `popoll_backend-0.0.63/pyproject.toml` & `popoll_backend-0.0.64/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", 'wheel', 'flask', 'flask_cors', 'flask-restful', 'jsonpickle', 'sqlalchemy', 'sqlalchemy-utils', 'psycopg2-binary', 'pyyaml', 'pyopenssl']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "popoll_backend"
-version = "0.0.63"
+version = "0.0.64"
 authors = [
   { name="vivi5421", email="pypi@villard.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `popoll_backend-0.0.63/tests/test_01_get_poll.py` & `popoll_backend-0.0.64/tests/test_01_get_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_02_create_poll.py` & `popoll_backend-0.0.64/tests/test_02_create_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_04_get_instruments.py` & `popoll_backend-0.0.64/tests/test_04_get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_08_get_users.py` & `popoll_backend-0.0.64/tests/test_08_get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_09_create_user.py` & `popoll_backend-0.0.64/tests/test_09_create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_10_get_user.py` & `popoll_backend-0.0.64/tests/test_10_get_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_11_update_user.py` & `popoll_backend-0.0.64/tests/test_11_update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_12_delete_user.py` & `popoll_backend-0.0.64/tests/test_12_delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_13_get_dates.py` & `popoll_backend-0.0.64/tests/test_13_get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_14_create_date.py` & `popoll_backend-0.0.64/tests/test_14_create_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_15_get_date.py` & `popoll_backend-0.0.64/tests/test_15_get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_16_update_date.py` & `popoll_backend-0.0.64/tests/test_16_update_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_17_delete_date.py` & `popoll_backend-0.0.64/tests/test_17_delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_18_create_answer.py` & `popoll_backend-0.0.64/tests/test_18_create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_19_update_answer.py` & `popoll_backend-0.0.64/tests/test_19_update_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_20_delete_answer.py` & `popoll_backend-0.0.64/tests/test_20_delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_21_get_answer.py` & `popoll_backend-0.0.64/tests/test_21_get_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_22_get_search_answer.py` & `popoll_backend-0.0.64/tests/test_22_get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_23_get_create_session.py` & `popoll_backend-0.0.64/tests/test_23_get_create_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_24_get_all_session.py` & `popoll_backend-0.0.64/tests/test_24_get_all_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.63/tests/test_25_delete_old_dates.py` & `popoll_backend-0.0.64/tests/test_25_delete_old_dates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 
-from popoll_backend.query.delete_old_dates import dateBefore
+from popoll_backend.query.all.delete_old_dates import dateBefore
 from tests import IntegrationTest
 
 class TestDeleteOldDates(IntegrationTest):
     
     today = datetime.date.today()
 
     def setUp(self):
```

