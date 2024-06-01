# Comparing `tmp/mds_cashbook-7.0.34.tar.gz` & `tmp/mds_cashbook-7.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook-7.0.34.tar", last modified: Thu May 30 10:58:25 2024, max compression
+gzip compressed data, was "mds_cashbook-7.0.35.tar", last modified: Sat Jun  1 09:19:47 2024, max compression
```

## Comparing `mds_cashbook-7.0.34.tar` & `mds_cashbook-7.0.35.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.583778 mds_cashbook-7.0.34/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7969 2024-05-30 10:58:25.583778 mds_cashbook-7.0.34/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5454 2024-05-30 10:58:02.000000 mds_cashbook-7.0.34/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1500 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    23181 2024-01-03 20:03:30.000000 mds_cashbook-7.0.34/book.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    25770 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/book.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5335 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/category.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6152 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/category.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2243 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/cbreport.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      689 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/cbreport.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6924 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/configuration.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3777 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/configuration.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      225 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/const.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      500 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/cron.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      501 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/cron.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1866 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/currency.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.563778 mds_cashbook-7.0.34/docs/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      495 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/docs/settings.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1013 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/group.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.563778 mds_cashbook-7.0.34/icon/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3638 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/icon/notebook1.svg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      431 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/icon.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1045 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/ir.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    43435 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    13058 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.567778 mds_cashbook-7.0.34/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    46721 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    43888 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.583778 mds_cashbook-7.0.34/mds_cashbook.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7969 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1681 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       67 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      110 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2024-05-30 10:58:25.000000 mds_cashbook-7.0.34/mds_cashbook.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5212 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/menu.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     8068 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/message.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7164 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/mixin.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     4392 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/model.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    18283 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/reconciliation.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     9672 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/reconciliation.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.567778 mds_cashbook-7.0.34/report/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20379 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/report/cashbook.fods
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    52038 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/report/reconciliation.fods
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2024-05-30 10:58:25.583778 mds_cashbook-7.0.34/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3830 2023-12-31 11:47:46.000000 mds_cashbook-7.0.34/setup.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11193 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/splitline.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6066 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/splitline.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.575778 mds_cashbook-7.0.34/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      203 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    25017 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/book.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7013 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/tests/bookingwiz.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     8328 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/category.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6679 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/tests/config.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    74665 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/line.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    32358 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/tests/reconciliation.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    16431 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/tests/splitline.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      970 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/tests/test_module.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1551 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/tests/type.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    33651 2024-05-30 10:58:02.000000 mds_cashbook-7.0.34/tests/valuestore.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      359 2024-05-30 10:58:02.000000 mds_cashbook-7.0.34/tryton.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2128 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/types.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3454 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/types.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7138 2024-05-30 10:52:27.000000 mds_cashbook-7.0.34/valuestore.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-05-30 10:58:25.579778 mds_cashbook-7.0.34/view/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2491 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/book_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      503 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/book_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      598 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/book_tree.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      450 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/cashbook_line_context_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      725 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/category_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      248 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/category_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      337 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/category_tree.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      999 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/configuration_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1170 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/view/enterbooking_start_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1867 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/line_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      639 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/line_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      650 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/line_recon_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1085 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/recon_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      538 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/recon_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      940 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/split_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      612 2023-12-31 11:47:47.000000 mds_cashbook-7.0.34/view/split_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      379 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/type_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      298 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/type_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      533 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/wizard_openline_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      923 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/view/wizard_runrepbook_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     7324 2024-05-30 10:52:37.000000 mds_cashbook-7.0.34/wizard_booking.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      745 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_booking.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5542 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_openline.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1614 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_openline.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     4613 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_runreport.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1221 2023-12-01 19:18:18.000000 mds_cashbook-7.0.34/wizard_runreport.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-01 09:19:47.592887 mds_cashbook-7.0.35/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     8076 2024-06-01 09:19:47.588887 mds_cashbook-7.0.35/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     5529 2024-06-01 09:18:04.000000 mds_cashbook-7.0.35/README.rst
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1500 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    23181 2024-01-03 20:03:30.000000 mds_cashbook-7.0.35/book.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    25770 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/book.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     5335 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/category.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6152 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/category.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2243 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/cbreport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      689 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/cbreport.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7343 2024-06-01 09:14:28.000000 mds_cashbook-7.0.35/configuration.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3777 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/configuration.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      225 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/const.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      500 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/cron.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      501 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/cron.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1866 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/currency.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-01 09:19:47.564887 mds_cashbook-7.0.35/docs/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      495 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/docs/settings.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1013 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/group.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-01 09:19:47.568887 mds_cashbook-7.0.35/icon/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3638 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/icon/notebook1.svg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      431 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/icon.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1045 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/ir.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    43435 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/line.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    13058 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/line.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-01 09:19:47.568887 mds_cashbook-7.0.35/locale/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    47197 2024-06-01 09:14:28.000000 mds_cashbook-7.0.35/locale/de.po
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    44336 2024-06-01 09:14:28.000000 mds_cashbook-7.0.35/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-01 09:19:47.588887 mds_cashbook-7.0.35/mds_cashbook.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     8076 2024-06-01 09:19:47.000000 mds_cashbook-7.0.35/mds_cashbook.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1681 2024-06-01 09:19:47.000000 mds_cashbook-7.0.35/mds_cashbook.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-06-01 09:19:47.000000 mds_cashbook-7.0.35/mds_cashbook.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       67 2024-06-01 09:19:47.000000 mds_cashbook-7.0.35/mds_cashbook.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-06-01 09:19:47.000000 mds_cashbook-7.0.35/mds_cashbook.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      110 2024-06-01 09:19:47.000000 mds_cashbook-7.0.35/mds_cashbook.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2024-06-01 09:19:47.000000 mds_cashbook-7.0.35/mds_cashbook.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5212 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/menu.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     8068 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/message.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7164 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/mixin.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     4392 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/model.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    18283 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/reconciliation.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     9672 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/reconciliation.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-01 09:19:47.568887 mds_cashbook-7.0.35/report/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20379 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/report/cashbook.fods
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    52038 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/report/reconciliation.fods
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2024-06-01 09:19:47.592887 mds_cashbook-7.0.35/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3830 2023-12-31 11:47:46.000000 mds_cashbook-7.0.35/setup.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11193 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/splitline.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6066 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/splitline.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-01 09:19:47.576887 mds_cashbook-7.0.35/tests/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      203 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    25017 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/tests/book.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7148 2024-06-01 09:14:28.000000 mds_cashbook-7.0.35/tests/bookingwiz.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     8328 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/tests/category.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6872 2024-06-01 09:14:28.000000 mds_cashbook-7.0.35/tests/config.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    74665 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/tests/line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    32358 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/tests/reconciliation.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    16431 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/tests/splitline.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      970 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/tests/test_module.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1551 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/tests/type.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    33876 2024-05-30 11:17:38.000000 mds_cashbook-7.0.35/tests/valuestore.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      359 2024-06-01 09:18:12.000000 mds_cashbook-7.0.35/tryton.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2128 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/types.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3454 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/types.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7138 2024-05-30 10:52:27.000000 mds_cashbook-7.0.35/valuestore.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-01 09:19:47.588887 mds_cashbook-7.0.35/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2491 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/book_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      503 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/view/book_list.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      598 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/view/book_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      450 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/cashbook_line_context_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      725 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/category_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      248 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/category_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      337 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/category_tree.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1069 2024-06-01 09:14:28.000000 mds_cashbook-7.0.35/view/configuration_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1170 2024-05-30 10:52:37.000000 mds_cashbook-7.0.35/view/enterbooking_start_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1867 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/line_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      639 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/view/line_list.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      650 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/view/line_recon_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1085 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/recon_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      538 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/view/recon_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      940 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/split_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      612 2023-12-31 11:47:47.000000 mds_cashbook-7.0.35/view/split_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      379 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/type_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      298 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/type_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      533 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/wizard_openline_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      923 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/view/wizard_runrepbook_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7389 2024-06-01 09:14:29.000000 mds_cashbook-7.0.35/wizard_booking.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      745 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/wizard_booking.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5542 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/wizard_openline.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1614 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/wizard_openline.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     4613 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/wizard_runreport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1221 2023-12-01 19:18:18.000000 mds_cashbook-7.0.35/wizard_runreport.xml
```

### Comparing `mds_cashbook-7.0.34/PKG-INFO` & `mds_cashbook-7.0.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mds_cashbook
-Version: 7.0.34
+Version: 7.0.35
 Summary: Tryton module to add a cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook
 Description: mds-cashbook
@@ -158,14 +158,18 @@
         If you have hierarchical cash books, the amounts of subordinate cash books with foreign
         currency are converted  into the display currency of the parent cash book.
         
         
         Changes
         =======
         
+        *7.0.35 - 01.06.2024*
+        
+        - add: config setting for fixate in booking-wizard
+        
         *7.0.34 - 30.05.2024*
         
         - add: fixate of booking from booking-wizard
         
         *7.0.33 - 31.12.2023*
         
         - remove caching
```

### Comparing `mds_cashbook-7.0.34/README.rst` & `mds_cashbook-7.0.35/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,18 @@
 If you have hierarchical cash books, the amounts of subordinate cash books with foreign
 currency are converted  into the display currency of the parent cash book.
 
 
 Changes
 =======
 
+*7.0.35 - 01.06.2024*
+
+- add: config setting for fixate in booking-wizard
+
 *7.0.34 - 30.05.2024*
 
 - add: fixate of booking from booking-wizard
 
 *7.0.33 - 31.12.2023*
 
 - remove caching
```

### Comparing `mds_cashbook-7.0.34/__init__.py` & `mds_cashbook-7.0.35/__init__.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/book.py` & `mds_cashbook-7.0.35/book.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/book.xml` & `mds_cashbook-7.0.35/book.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/category.py` & `mds_cashbook-7.0.35/category.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/category.xml` & `mds_cashbook-7.0.35/category.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/cbreport.py` & `mds_cashbook-7.0.35/cbreport.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/cbreport.xml` & `mds_cashbook-7.0.35/cbreport.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/configuration.py` & `mds_cashbook-7.0.35/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,25 +67,27 @@
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[('btype', '!=', None), ('state', '=', 'open')]))
     book5 = fields.MultiValue(fields.Many2One(
         string='Cashbook 5',
         help='Cash book available in selection dialog.',
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[('btype', '!=', None), ('state', '=', 'open')]))
+    fixate = fields.MultiValue(fields.Boolean(
+        string='Fixate', help='Fixating of the booking is activated.'))
 
     @classmethod
     def multivalue_model(cls, field):
         """ get model for value
         """
         pool = Pool()
 
         if field in [
                 'date_from', 'date_to', 'checked', 'done',
                 'catnamelong', 'defbook', 'book1', 'book2',
-                'book3', 'book4', 'book5']:
+                'book3', 'book4', 'book5', 'fixate']:
             return pool.get('cashbook.configuration_user')
         return super(Configuration, cls).multivalue_model(field)
 
     @classmethod
     def default_checked(cls, **pattern):
         return cls.multivalue_model('checked').default_checked()
 
@@ -93,14 +95,18 @@
     def default_done(cls, **pattern):
         return cls.multivalue_model('done').default_done()
 
     @classmethod
     def default_catnamelong(cls, **pattern):
         return cls.multivalue_model('catnamelong').default_catnamelong()
 
+    @classmethod
+    def default_fixate(cls, **pattern):
+        return cls.multivalue_model('fixate').default_fixate()
+
 # end Configuration
 
 
 class UserConfiguration(ModelSQL, UserValueMixin):
     'User Configuration'
     __name__ = 'cashbook.configuration_user'
 
@@ -171,20 +177,27 @@
         model_name='cashbook.book', ondelete='SET NULL',
         domain=[
             ('btype', '!=', None),
             ('state', '=', 'open'),
             ('owner.id', '=', Eval('iduser', -1))
         ], depends=['iduser'])
 
+    fixate = fields.Boolean(
+        string='Fixate', help='Fixating of the booking is activated.')
+
     @classmethod
     def default_checked(cls):
         return True
 
     @classmethod
     def default_catnamelong(cls):
         return True
 
     @classmethod
     def default_done(cls):
         return False
 
+    @classmethod
+    def default_fixate(cls):
+        return False
+
 # end UserConfiguration
```

### Comparing `mds_cashbook-7.0.34/configuration.xml` & `mds_cashbook-7.0.35/configuration.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/currency.py` & `mds_cashbook-7.0.35/currency.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/group.xml` & `mds_cashbook-7.0.35/group.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/icon/notebook1.svg` & `mds_cashbook-7.0.35/icon/notebook1.svg`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/ir.py` & `mds_cashbook-7.0.35/ir.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/line.py` & `mds_cashbook-7.0.35/line.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/line.xml` & `mds_cashbook-7.0.35/line.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/locale/de.po` & `mds_cashbook-7.0.35/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -1254,14 +1254,22 @@
 msgid "Cashbook 5"
 msgstr "Kassenbuch 5"
 
 msgctxt "help:cashbook.configuration,book5:"
 msgid "Cash book available in selection dialog."
 msgstr "in Auswahldialog verfügbares Kassenbuch."
 
+msgctxt "field:cashbook.configuration,fixate:"
+msgid "Fixate"
+msgstr "Festschreiben"
+
+msgctxt "help:cashbook.configuration,fixate:"
+msgid "Fixating of the booking is activated."
+msgstr "Die Festschreiben der Buchung ist aktiviert."
+
 msgctxt "field:cashbook.configuration,date_from:"
 msgid "Start Date"
 msgstr "Beginndatum"
 
 msgctxt "field:cashbook.configuration,date_to:"
 msgid "End Date"
 msgstr "Endedatum"
@@ -1374,14 +1382,22 @@
 msgid "Cashbook 5"
 msgstr "Kassenbuch 5"
 
 msgctxt "help:cashbook.configuration_user,book5:"
 msgid "Cash book available in selection dialog."
 msgstr "in Auswahldialog verfügbares Kassenbuch."
 
+msgctxt "field:cashbook.configuration_user,fixate:"
+msgid "Fixate"
+msgstr "Festschreiben"
+
+msgctxt "help:cashbook.configuration_user,fixate:"
+msgid "Fixating of the booking is activated."
+msgstr "Die Festschreiben der Buchung ist aktiviert."
+
 
 ##################
 # cashbook.recon #
 ##################
 msgctxt "model:cashbook.recon,name:"
 msgid "Cashbook Reconciliation"
 msgstr "Kassenbuchabstimmung"
```

### Comparing `mds_cashbook-7.0.34/locale/en.po` & `mds_cashbook-7.0.35/locale/en.po`

 * *Files 1% similar despite different names*

```diff
@@ -1182,14 +1182,22 @@
 msgid "Cashbook 5"
 msgstr "Cashbook 5"
 
 msgctxt "help:cashbook.configuration,book5:"
 msgid "Cash book available in selection dialog."
 msgstr "Cash book available in selection dialog."
 
+msgctxt "field:cashbook.configuration,fixate:"
+msgid "Fixate"
+msgstr "Fixate"
+
+msgctxt "help:cashbook.configuration,fixate:"
+msgid "Fixating of the booking is activated."
+msgstr "Fixating of the booking is activated."
+
 msgctxt "field:cashbook.configuration,date_from:"
 msgid "Start Date"
 msgstr "Start Date"
 
 msgctxt "field:cashbook.configuration,date_to:"
 msgid "End Date"
 msgstr "End Date"
@@ -1298,14 +1306,22 @@
 msgid "Cashbook 5"
 msgstr "Cashbook 5"
 
 msgctxt "help:cashbook.configuration_user,book5:"
 msgid "Cash book available in selection dialog."
 msgstr "Cash book available in selection dialog."
 
+msgctxt "field:cashbook.configuration_user,fixate:"
+msgid "Fixate"
+msgstr "Fixate"
+
+msgctxt "help:cashbook.configuration_user,fixate:"
+msgid "Fixating of the booking is activated."
+msgstr "Fixating of the booking is activated."
+
 msgctxt "model:cashbook.recon,name:"
 msgid "Cashbook Reconciliation"
 msgstr "Cashbook Reconciliation"
 
 msgctxt "view:cashbook.recon:"
 msgid "Reconciliation period"
 msgstr "Reconciliation period"
```

### Comparing `mds_cashbook-7.0.34/mds_cashbook.egg-info/PKG-INFO` & `mds_cashbook-7.0.35/mds_cashbook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mds-cashbook
-Version: 7.0.34
+Version: 7.0.35
 Summary: Tryton module to add a cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook
 Description: mds-cashbook
@@ -158,14 +158,18 @@
         If you have hierarchical cash books, the amounts of subordinate cash books with foreign
         currency are converted  into the display currency of the parent cash book.
         
         
         Changes
         =======
         
+        *7.0.35 - 01.06.2024*
+        
+        - add: config setting for fixate in booking-wizard
+        
         *7.0.34 - 30.05.2024*
         
         - add: fixate of booking from booking-wizard
         
         *7.0.33 - 31.12.2023*
         
         - remove caching
```

### Comparing `mds_cashbook-7.0.34/mds_cashbook.egg-info/SOURCES.txt` & `mds_cashbook-7.0.35/mds_cashbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/menu.xml` & `mds_cashbook-7.0.35/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/message.xml` & `mds_cashbook-7.0.35/message.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/mixin.py` & `mds_cashbook-7.0.35/mixin.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/model.py` & `mds_cashbook-7.0.35/model.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/reconciliation.py` & `mds_cashbook-7.0.35/reconciliation.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/reconciliation.xml` & `mds_cashbook-7.0.35/reconciliation.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/report/cashbook.fods` & `mds_cashbook-7.0.35/report/cashbook.fods`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/report/reconciliation.fods` & `mds_cashbook-7.0.35/report/reconciliation.fods`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/setup.py` & `mds_cashbook-7.0.35/setup.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/splitline.py` & `mds_cashbook-7.0.35/splitline.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/splitline.xml` & `mds_cashbook-7.0.35/splitline.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/tests/book.py` & `mds_cashbook-7.0.35/tests/book.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/tests/bookingwiz.py` & `mds_cashbook-7.0.35/tests/bookingwiz.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         """
         pool = Pool()
         BookingWiz = pool.get('cashbook.enterbooking', type='wizard')
         Book = pool.get('cashbook.book')
         Category = pool.get('cashbook.category')
         Party = pool.get('party.party')
         IrDate = pool.get('ir.date')
+        Config = pool.get('cashbook.configuration')
 
         company = self.prep_company()
         with Transaction().set_context({
                 'company': company.id}):
             types = self.prep_type()
             book, = Book.create([{
                 'name': 'Cash Book',
@@ -47,29 +48,33 @@
                     'name': 'Income',
                     'cattype': 'in',
                 }, {
                     'name': 'Food',
                     'cattype': 'out',
                 }])
 
+            cfg1 = Config()
+            cfg1.fixate = True
+            cfg1.save()
+
             (sess_id, start_state, end_state) = BookingWiz.create()
             w_obj = BookingWiz(sess_id)
             self.assertEqual(start_state, 'start')
             self.assertEqual(end_state, 'end')
 
             result = BookingWiz.execute(sess_id, {}, start_state)
             self.assertEqual(list(result.keys()), ['view'])
             self.assertEqual(result['view']['defaults']['bookingtype'], 'out')
             self.assertEqual(result['view']['defaults']['cashbook'], None)
             self.assertEqual(result['view']['defaults']['amount'], None)
             self.assertEqual(result['view']['defaults']['party'], None)
             self.assertEqual(result['view']['defaults']['booktransf'], None)
             self.assertEqual(result['view']['defaults']['description'], None)
             self.assertEqual(result['view']['defaults']['category'], None)
-            self.assertEqual(result['view']['defaults']['fixate'], False)
+            self.assertEqual(result['view']['defaults']['fixate'], True)
 
             self.assertEqual(len(book.lines), 0)
 
             r1 = {
                 'amount': Decimal('10.0'),
                 'cashbook': book.id,
                 'party': party.id,
```

### Comparing `mds_cashbook-7.0.34/tests/category.py` & `mds_cashbook-7.0.35/tests/category.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/tests/config.py` & `mds_cashbook-7.0.35/tests/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,30 +174,33 @@
                 cfg1.save()
 
                 cfg2 = Configuration.get_singleton()
                 self.assertEqual(cfg2.date_from, None)
                 self.assertEqual(cfg2.date_to, None)
                 self.assertEqual(cfg2.checked, True)
                 self.assertEqual(cfg2.done, False)
+                self.assertEqual(cfg2.fixate, False)
 
                 cfg2.date_from = date(2022, 4, 1)
                 cfg2.date_to = date(2022, 5, 30)
                 cfg2.checked = False
+                cfg2.fixate = True
                 cfg2.save()
 
             # change to user 'diego'
             with Transaction().set_user(usr_lst[1].id):
                 cfg1 = Configuration()
                 cfg1.save()
 
                 cfg2 = Configuration.get_singleton()
                 self.assertEqual(cfg2.date_from, None)
                 self.assertEqual(cfg2.date_to, None)
                 self.assertEqual(cfg2.checked, True)
                 self.assertEqual(cfg2.done, False)
+                self.assertEqual(cfg2.fixate, False)
 
                 cfg2.date_from = date(2022, 4, 15)
                 cfg2.date_to = date(2022, 5, 15)
                 cfg2.save()
 
             # change to user 'frida' - check
             with Transaction().set_user(usr_lst[0].id):
@@ -205,9 +208,10 @@
                 cfg1.save()
 
                 cfg2 = Configuration.get_singleton()
                 self.assertEqual(cfg2.date_from, date(2022, 4, 1))
                 self.assertEqual(cfg2.date_to, date(2022, 5, 30))
                 self.assertEqual(cfg2.checked, False)
                 self.assertEqual(cfg2.done, False)
+                self.assertEqual(cfg2.fixate, True)
 
 # end ConfigTestCase
```

### Comparing `mds_cashbook-7.0.34/tests/line.py` & `mds_cashbook-7.0.35/tests/line.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/tests/reconciliation.py` & `mds_cashbook-7.0.35/tests/reconciliation.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/tests/splitline.py` & `mds_cashbook-7.0.35/tests/splitline.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/tests/test_module.py` & `mds_cashbook-7.0.35/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/tests/type.py` & `mds_cashbook-7.0.35/tests/type.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/tests/valuestore.py` & `mds_cashbook-7.0.35/tests/valuestore.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,27 +441,28 @@
                 values[7].rec_name,
                 '[Lev 0/Lev 1b | 0.00 € | Open]|balance_all|0.00|2')
             self.assertEqual(
                 values[8].rec_name,
                 '[Lev 0/Lev 1b | 0.00 € | Open]|balance_ref|0.00|2')
 
             # add bookings
-            Line.create([{
+            Line.create(self.prep_valstore_line_create_data(
+                [{
                 'cashbook': values[0].cashbook.id,  # Lev 0
                 'amount': Decimal('2.0'),
                 'bookingtype': 'in',
                 'category': category.id,
                 'date': date(2022, 5, 10),
                 }, {
                 'cashbook': values[3].cashbook.id,  # Lev 1a
                 'amount': Decimal('3.0'),
                 'bookingtype': 'in',
                 'category': category.id,
                 'date': date(2022, 5, 10),
-                }])
+                }]))
 
             # add 'date' to context, will return computed
             # (not stored) values
             with Transaction().set_context({'date': date(2022, 5, 10)}):
                 values = ValueStore.search(
                     [('field_name', 'in', [
                         'balance', 'balance_all', 'balance_ref'])],
@@ -568,14 +569,19 @@
             self.assertEqual(
                 values[7].rec_name,
                 '[Lev 0/Lev 1b | 0.00 € | Open]|balance_all|0.00|2')
             self.assertEqual(
                 values[8].rec_name,
                 '[Lev 0/Lev 1b | 0.00 € | Open]|balance_ref|0.00|2')
 
+    def prep_valstore_line_create_data(self, query):
+        """ allow add of data
+        """
+        return query
+
     @with_transaction()
     def test_valstore_search_sort_books(self):
         """ create cashbooks add lines, search/sort
             with and w/o 'date' in context
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
@@ -619,29 +625,30 @@
                 'start_date': date(2022, 5, 1),
                 }])
             self.assertEqual(len(books), 3)
             self.assertEqual(books[0].rec_name, 'Cashbook 1 | 10.00 usd | Open')
             self.assertEqual(books[1].rec_name, 'Cashbook 2 | 0.00 € | Open')
             self.assertEqual(books[2].rec_name, 'Cashbook 3 | 0.00 € | Open')
 
-            Line.create([{
+            Line.create(self.prep_valstore_line_create_data(
+                [{
                 'cashbook': books[1].id,
                 'bookingtype': 'in',
                 'amount': Decimal('5.0'),
                 'date': date(2022, 5, 6),
                 'description': '5€ in',
                 'category': category.id,
                 }, {
                 'cashbook': books[2].id,
                 'bookingtype': 'in',
                 'amount': Decimal('6.0'),
                 'date': date(2022, 5, 7),
                 'description': '6€ in',
                 'category': category.id,
-                }])
+                }]))
 
             # no 'date' in context, using stored values
             # workers not yet processed
             books = Book.search([], order=[('name', 'ASC')])
             self.assertEqual(len(books), 3)
             self.assertEqual(books[0].rec_name, 'Cashbook 1 | 10.00 usd | Open')
             self.assertEqual(books[1].rec_name, 'Cashbook 2 | 0.00 € | Open')
```

### Comparing `mds_cashbook-7.0.34/types.py` & `mds_cashbook-7.0.35/types.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/types.xml` & `mds_cashbook-7.0.35/types.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/valuestore.py` & `mds_cashbook-7.0.35/valuestore.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/book_form.xml` & `mds_cashbook-7.0.35/view/book_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/book_tree.xml` & `mds_cashbook-7.0.35/view/book_tree.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/category_form.xml` & `mds_cashbook-7.0.35/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/configuration_form.xml` & `mds_cashbook-7.0.35/view/configuration_form.xml`

 * *Files 3% similar despite different names*

#### Comparing `mds_cashbook-7.0.34/view/configuration_form.xml` & `mds_cashbook-7.0.35/view/configuration_form.xml`

```diff
@@ -20,11 +20,14 @@
   <field name="book2"/>
   <label name="book3"/>
   <field name="book3"/>
   <label name="book4"/>
   <field name="book4"/>
   <label name="book5"/>
   <field name="book5"/>
+  <label name="fixate"/>
+  <field name="fixate"/>
+  <newline/>
   <separator id="sepcb" colspan="4" string="Cashbook"/>
   <label name="catnamelong"/>
   <field name="catnamelong"/>
 </form>
```

### Comparing `mds_cashbook-7.0.34/view/enterbooking_start_form.xml` & `mds_cashbook-7.0.35/view/enterbooking_start_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/line_form.xml` & `mds_cashbook-7.0.35/view/line_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/line_list.xml` & `mds_cashbook-7.0.35/view/line_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/line_recon_list.xml` & `mds_cashbook-7.0.35/view/line_recon_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/recon_form.xml` & `mds_cashbook-7.0.35/view/recon_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/recon_list.xml` & `mds_cashbook-7.0.35/view/recon_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/split_form.xml` & `mds_cashbook-7.0.35/view/split_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/split_list.xml` & `mds_cashbook-7.0.35/view/split_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/wizard_openline_form.xml` & `mds_cashbook-7.0.35/view/wizard_openline_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/view/wizard_runrepbook_form.xml` & `mds_cashbook-7.0.35/view/wizard_runrepbook_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/wizard_booking.py` & `mds_cashbook-7.0.35/wizard_booking.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,15 +153,16 @@
 
         book_ids = []
         for x in ['defbook', 'book1', 'book2', 'book3', 'book4', 'book5']:
             if getattr(cfg1, x, None) is not None:
                 book_ids.append(getattr(cfg1, x, None).id)
 
         result = {
-            'fixate': False,
+            'fixate': cfg1.fixate
+            if cfg1 and cfg1.fixate is not None else False,
             'cashbooks': [x.id for x in Cashbook.search([
                     ('state', '=', 'open'),
                     ('btype', '!=', None),
                     ('owner', '=', Transaction().user),
                     ('id', 'in', book_ids),
                 ])],
             'bookingtype': getattr(self.start, 'bookingtype', 'out'),
```

### Comparing `mds_cashbook-7.0.34/wizard_booking.xml` & `mds_cashbook-7.0.35/wizard_booking.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/wizard_openline.py` & `mds_cashbook-7.0.35/wizard_openline.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/wizard_openline.xml` & `mds_cashbook-7.0.35/wizard_openline.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/wizard_runreport.py` & `mds_cashbook-7.0.35/wizard_runreport.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-7.0.34/wizard_runreport.xml` & `mds_cashbook-7.0.35/wizard_runreport.xml`

 * *Files identical despite different names*

