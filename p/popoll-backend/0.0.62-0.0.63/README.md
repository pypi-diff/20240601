# Comparing `tmp/popoll_backend-0.0.62.tar.gz` & `tmp/popoll_backend-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.62.tar", last modified: Wed May 29 16:18:04 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.63.tar", last modified: Sat Jun  1 07:57:40 2024, max compression
```

## Comparing `popoll_backend-0.0.62.tar` & `popoll_backend-0.0.63.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:04.200381 popoll_backend-0.0.62/
--rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/LICENSE
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 16:18:04.200381 popoll_backend-0.0.62/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:04.183381 popoll_backend-0.0.62/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     8488 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:04.185381 popoll_backend-0.0.62/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:04.187381 popoll_backend-0.0.62/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      736 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:04.189381 popoll_backend-0.0.62/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/dates.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/empty.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/polls.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/users.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:04.195381 popoll_backend-0.0.62/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     3633 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/delete_old_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_all_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_all_sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1948 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:04.200381 popoll_backend-0.0.62/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 16:18:04.000000 popoll_backend-0.0.62/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2798 2024-05-29 16:18:04.000000 popoll_backend-0.0.62/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 16:18:04.000000 popoll_backend-0.0.62/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-29 16:18:04.000000 popoll_backend-0.0.62/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-29 16:18:04.000000 popoll_backend-0.0.62/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-29 16:17:58.000000 popoll_backend-0.0.62/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 16:18:04.200381 popoll_backend-0.0.62/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 16:18:04.199381 popoll_backend-0.0.62/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_01_get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_02_create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_03_update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_04_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_08_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_09_create_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1857 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_10_get_user.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_11_update_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_12_delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_13_get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_14_create_date.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_15_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_16_update_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_17_delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_18_create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_19_update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_20_delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_21_get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_22_get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_23_get_create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_24_get_all_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-29 16:17:44.000000 popoll_backend-0.0.62/tests/test_25_delete_old_dates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.273747 popoll_backend-0.0.63/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      654 2024-06-01 07:57:40.273747 popoll_backend-0.0.63/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.256747 popoll_backend-0.0.63/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     8488 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.257747 popoll_backend-0.0.63/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.259747 popoll_backend-0.0.63/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.261747 popoll_backend-0.0.63/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/polls.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.268746 popoll_backend-0.0.63/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     3633 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/delete_old_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_all_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_all_sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/popoll_backend/query/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.273747 popoll_backend-0.0.63/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2798 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-06-01 07:57:40.000000 popoll_backend-0.0.63/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-06-01 07:57:34.000000 popoll_backend-0.0.63/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 07:57:40.273747 popoll_backend-0.0.63/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 07:57:40.272746 popoll_backend-0.0.63/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_01_get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_02_create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_03_update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_04_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_08_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_09_create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1857 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_10_get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_11_update_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_12_delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_13_get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_14_create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_15_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_16_update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_17_delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_18_create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_19_update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_20_delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_21_get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_22_get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_23_get_create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_24_get_all_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-06-01 07:57:20.000000 popoll_backend-0.0.63/tests/test_25_delete_old_dates.py
```

### Comparing `popoll_backend-0.0.62/PKG-INFO` & `popoll_backend-0.0.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.62
+Version: 0.0.63
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 License: Free
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `popoll_backend-0.0.62/popoll_backend/__main__.py` & `popoll_backend-0.0.63/popoll_backend/__main__.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.63/popoll_backend/model/db/answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/db/date.py` & `popoll_backend-0.0.63/popoll_backend/model/db/date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/db/session.py` & `popoll_backend-0.0.63/popoll_backend/model/db/session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/db/user_instruments.py` & `popoll_backend-0.0.63/popoll_backend/model/db/user_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/payload/date_details.py` & `popoll_backend-0.0.63/popoll_backend/model/payload/date_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.63/popoll_backend/model/payload/history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/payload/polls.py` & `popoll_backend-0.0.63/popoll_backend/model/payload/polls.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/payload/user_details.py` & `popoll_backend-0.0.63/popoll_backend/model/payload/user_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/model/payload/user_with_instruments.py` & `popoll_backend-0.0.63/popoll_backend/model/payload/user_with_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/__init__.py` & `popoll_backend-0.0.63/popoll_backend/query/__init__.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.63/popoll_backend/query/create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/create_date.py` & `popoll_backend-0.0.63/popoll_backend/query/create_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.63/popoll_backend/query/create_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/create_session.py` & `popoll_backend-0.0.63/popoll_backend/query/create_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/create_user.py` & `popoll_backend-0.0.63/popoll_backend/query/create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.63/popoll_backend/query/delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.63/popoll_backend/query/delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/delete_old_dates.py` & `popoll_backend-0.0.63/popoll_backend/query/delete_old_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.63/popoll_backend/query/delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_all_instruments.py` & `popoll_backend-0.0.63/popoll_backend/query/get_all_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_all_sessions.py` & `popoll_backend-0.0.63/popoll_backend/query/get_all_sessions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sqlite3
-from typing import List
+from typing import List, Union
 
 from popoll_backend.model import Payload
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.polls import Poll, Polls
 from popoll_backend.query import Query
 
 
@@ -13,15 +13,15 @@
     
     def __init__(self, id: str):
         self.id = id
         
     def process(self, db: str, cursor: sqlite3.Cursor) -> None:
         pass
         
-    def buildResponse(self, db: str, cursor: sqlite3.Cursor) -> Poll | Empty:
+    def buildResponse(self, db: str, cursor: sqlite3.Cursor) -> Union[Poll, Empty]:
         if cursor.execute('SELECT COUNT(*) FROM sessions WHERE session_id=?', (self.id,)).fetchone()[0] > 0:
             return Poll(db, cursor.execute('SELECT name FROM options').fetchone()[0])
         else:
             return Empty()
         
     def mergeResponses(self, answers: List[Payload]) -> Payload:
         return Polls(polls=[a for a in answers if not a.isEmpty])
```

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_date.py` & `popoll_backend-0.0.63/popoll_backend/query/get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_date_details.py` & `popoll_backend-0.0.63/popoll_backend/query/get_date_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.63/popoll_backend/query/get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_instrument.py` & `popoll_backend-0.0.63/popoll_backend/query/get_instrument.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.63/popoll_backend/query/get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_search_answer.py` & `popoll_backend-0.0.63/popoll_backend/query/get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_session.py` & `popoll_backend-0.0.63/popoll_backend/query/get_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_user_details.py` & `popoll_backend-0.0.63/popoll_backend/query/get_user_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_user_with_instruments.py` & `popoll_backend-0.0.63/popoll_backend/query/get_user_with_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/get_users.py` & `popoll_backend-0.0.63/popoll_backend/query/get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/update_answer.py` & `popoll_backend-0.0.63/popoll_backend/query/update_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/update_date.py` & `popoll_backend-0.0.63/popoll_backend/query/update_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/update_poll.py` & `popoll_backend-0.0.63/popoll_backend/query/update_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend/query/update_user.py` & `popoll_backend-0.0.63/popoll_backend/query/update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.63/popoll_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.62
+Version: 0.0.63
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 License: Free
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `popoll_backend-0.0.62/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.63/popoll_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/pyproject.toml` & `popoll_backend-0.0.63/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", 'wheel', 'flask', 'flask_cors', 'flask-restful', 'jsonpickle', 'sqlalchemy', 'sqlalchemy-utils', 'psycopg2-binary', 'pyyaml', 'pyopenssl']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "popoll_backend"
-version = "0.0.62"
+version = "0.0.63"
 authors = [
   { name="vivi5421", email="pypi@villard.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `popoll_backend-0.0.62/tests/test_01_get_poll.py` & `popoll_backend-0.0.63/tests/test_01_get_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_02_create_poll.py` & `popoll_backend-0.0.63/tests/test_02_create_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_04_get_instruments.py` & `popoll_backend-0.0.63/tests/test_04_get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_08_get_users.py` & `popoll_backend-0.0.63/tests/test_08_get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_09_create_user.py` & `popoll_backend-0.0.63/tests/test_09_create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_10_get_user.py` & `popoll_backend-0.0.63/tests/test_10_get_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_11_update_user.py` & `popoll_backend-0.0.63/tests/test_11_update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_12_delete_user.py` & `popoll_backend-0.0.63/tests/test_12_delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_13_get_dates.py` & `popoll_backend-0.0.63/tests/test_13_get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_14_create_date.py` & `popoll_backend-0.0.63/tests/test_14_create_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_15_get_date.py` & `popoll_backend-0.0.63/tests/test_15_get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_16_update_date.py` & `popoll_backend-0.0.63/tests/test_16_update_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_17_delete_date.py` & `popoll_backend-0.0.63/tests/test_17_delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_18_create_answer.py` & `popoll_backend-0.0.63/tests/test_18_create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_19_update_answer.py` & `popoll_backend-0.0.63/tests/test_19_update_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_20_delete_answer.py` & `popoll_backend-0.0.63/tests/test_20_delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_21_get_answer.py` & `popoll_backend-0.0.63/tests/test_21_get_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_22_get_search_answer.py` & `popoll_backend-0.0.63/tests/test_22_get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_23_get_create_session.py` & `popoll_backend-0.0.63/tests/test_23_get_create_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_24_get_all_session.py` & `popoll_backend-0.0.63/tests/test_24_get_all_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.62/tests/test_25_delete_old_dates.py` & `popoll_backend-0.0.63/tests/test_25_delete_old_dates.py`

 * *Files identical despite different names*

