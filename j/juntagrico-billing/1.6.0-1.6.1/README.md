# Comparing `tmp/juntagrico_billing-1.6.0.tar.gz` & `tmp/juntagrico_billing-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juntagrico_billing-1.6.0.tar", last modified: Tue May 14 08:38:34 2024, max compression
+gzip compressed data, was "juntagrico_billing-1.6.1.tar", last modified: Sat Jun  1 21:33:26 2024, max compression
```

## Comparing `juntagrico_billing-1.6.0.tar` & `juntagrico_billing-1.6.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.647737 juntagrico_billing-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-14 08:38:34.647737 juntagrico_billing-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.631737 juntagrico_billing-1.6.0/juntagrico_billing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.635737 juntagrico_billing-1.6.0/juntagrico_billing/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/billitem_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/businessyear.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/admin/payment_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.635737 juntagrico_billing-1.6.0/juntagrico_billing/lifecycle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/lifecycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/lifecycle/billitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/lifecycle/payment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.635737 juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    18853 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/mailer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.635737 juntagrico_billing-1.6.0/juntagrico_billing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/migrations/0002_bill_published.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/migrations/0003_vat.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/models/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/models/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/querysets/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/querysets/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/querysets/payment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/templates/admin/juntagrico_billing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/templates/admin/juntagrico_billing/bill/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/admin/juntagrico_billing/bill/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/bills_notify.html
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/bookings_export.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/mails/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/mails/bill_notification.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.639737 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/messages/no_businessyear.html
--rw-r--r--   0 runner    (1001) docker     (127)     6409 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/open_bills.html
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/payments_upload.html
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/pending_bills.html
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/subscription_bookings.html
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/unpublished_bills.html
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/user_bill.html
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/user_bills.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.627737 juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.643736 juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/menu/
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/menu/admin.html
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/menu/user.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.643736 juntagrico_billing-1.6.0/juntagrico_billing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/test_billbookings.py
--rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/test_bills.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/test_payment_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/tests/test_payment_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.643736 juntagrico_billing-1.6.0/juntagrico_billing/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/bookings.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/esr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/payment_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/payment_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/pdfbill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/util/qrbill.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/juntagrico_billing/views_payment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:34.643736 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 08:38:34.000000 juntagrico_billing-1.6.0/juntagrico_billing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 08:38:28.000000 juntagrico_billing-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 08:38:34.647737 juntagrico_billing-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.174456 juntagrico_billing-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-06-01 21:33:26.174456 juntagrico_billing-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.162456 juntagrico_billing-1.6.1/juntagrico_billing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.166456 juntagrico_billing-1.6.1/juntagrico_billing/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/admin/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/admin/billitem_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/admin/businessyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/admin/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/admin/payment_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.166456 juntagrico_billing-1.6.1/juntagrico_billing/lifecycle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/lifecycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/lifecycle/billitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/lifecycle/payment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.158456 juntagrico_billing-1.6.1/juntagrico_billing/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.158456 juntagrico_billing-1.6.1/juntagrico_billing/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.166456 juntagrico_billing-1.6.1/juntagrico_billing/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    18853 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/mailer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.166456 juntagrico_billing-1.6.1/juntagrico_billing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/migrations/0002_bill_published.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/migrations/0003_vat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.166456 juntagrico_billing-1.6.1/juntagrico_billing/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/models/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/models/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.166456 juntagrico_billing-1.6.1/juntagrico_billing/querysets/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/querysets/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/querysets/payment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.158456 juntagrico_billing-1.6.1/juntagrico_billing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.158456 juntagrico_billing-1.6.1/juntagrico_billing/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.158456 juntagrico_billing-1.6.1/juntagrico_billing/templates/admin/juntagrico_billing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.166456 juntagrico_billing-1.6.1/juntagrico_billing/templates/admin/juntagrico_billing/bill/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/admin/juntagrico_billing/bill/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.170456 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/bills_notify.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/bookings_export.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.170456 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/mails/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/mails/bill_notification.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.170456 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/messages/no_businessyear.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6409 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/open_bills.html
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/payments_upload.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/pending_bills.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/subscription_bookings.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/unpublished_bills.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/user_bill.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/user_bills.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.158456 juntagrico_billing-1.6.1/juntagrico_billing/templates/juntagrico/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.170456 juntagrico_billing-1.6.1/juntagrico_billing/templates/juntagrico/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/juntagrico/menu/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/templates/juntagrico/menu/user.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.170456 juntagrico_billing-1.6.1/juntagrico_billing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/tests/test_billbookings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/tests/test_bills.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/tests/test_payment_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/tests/test_payment_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.174456 juntagrico_billing-1.6.1/juntagrico_billing/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/util/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/util/bookings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/util/esr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/util/payment_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/util/payment_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/util/pdfbill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/util/qrbill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/juntagrico_billing/views_payment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:33:26.174456 juntagrico_billing-1.6.1/juntagrico_billing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-06-01 21:33:26.000000 juntagrico_billing-1.6.1/juntagrico_billing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-06-01 21:33:26.000000 juntagrico_billing-1.6.1/juntagrico_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:33:26.000000 juntagrico_billing-1.6.1/juntagrico_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 21:33:26.000000 juntagrico_billing-1.6.1/juntagrico_billing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 21:33:26.000000 juntagrico_billing-1.6.1/juntagrico_billing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-01 21:33:18.000000 juntagrico_billing-1.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-01 21:33:26.174456 juntagrico_billing-1.6.1/setup.cfg
```

### Comparing `juntagrico_billing-1.6.0/LICENSE` & `juntagrico_billing-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/PKG-INFO` & `juntagrico_billing-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juntagrico-billing
-Version: 1.6.0
+Version: 1.6.1
 Summary: Send and manage bills in juntagrico.
 Author-email: juntagrico <python@juntagrico.org>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `juntagrico_billing-1.6.0/README.md` & `juntagrico_billing-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/admin/__init__.py` & `juntagrico_billing-1.6.1/juntagrico_billing/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/admin/bill.py` & `juntagrico_billing-1.6.1/juntagrico_billing/admin/bill.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/admin/billitem_inline.py` & `juntagrico_billing-1.6.1/juntagrico_billing/admin/billitem_inline.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/django.mo` & `juntagrico_billing-1.6.1/juntagrico_billing/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/locale/de/LC_MESSAGES/django.po` & `juntagrico_billing-1.6.1/juntagrico_billing/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/mailer.py` & `juntagrico_billing-1.6.1/juntagrico_billing/mailer.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py` & `juntagrico_billing-1.6.1/juntagrico_billing/migrations/0001_squashed_0012_post_1_4.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/migrations/0003_vat.py` & `juntagrico_billing-1.6.1/juntagrico_billing/migrations/0003_vat.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/models/account.py` & `juntagrico_billing-1.6.1/juntagrico_billing/models/account.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/models/bill.py` & `juntagrico_billing-1.6.1/juntagrico_billing/models/bill.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/models/payment.py` & `juntagrico_billing-1.6.1/juntagrico_billing/models/payment.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/models/settings.py` & `juntagrico_billing-1.6.1/juntagrico_billing/models/settings.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/bills_notify.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/bills_notify.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/bookings_export.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/bookings_export.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/mails/bill_notification.txt` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/mails/bill_notification.txt`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/open_bills.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/open_bills.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/payments_upload.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/payments_upload.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/pending_bills.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/pending_bills.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/subscription_bookings.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/subscription_bookings.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/unpublished_bills.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/unpublished_bills.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/user_bill.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/user_bill.html`

 * *Files 3% similar despite different names*

```diff
@@ -66,46 +66,52 @@
          </p>
     </div>
     {% endif %}
 
     <div class="row mb-4"><p class="col">{{ bill.public_notes | default_if_none:"" }}</p></div>
     
     {% if payments %}
-    <h4>{% trans "Payments per" %} {{ today|date:"SHORT_DATE_FORMAT" }}:</h4>
-    {% for payment in payments %}
-    <div class="row">
-        <div class="col-sm-2">{{ payment.paid_date|date:"SHORT_DATE_FORMAT" }}</div>
-        <div class="col-sm-8">{{ payment.type }}</div>
-        <div class="col-sm-2 text-right">{{ payment.amount | floatformat:2 }}</div>
-    </div>    
-    {% endfor %}
-    <div class="row font-weight-bold mt-3">
-        {% if bill.paid %}
-        <div class="col">{% trans "Bill paid completely" %}</div>
-        {% else %}
-        <div class="col-sm-5">{% trans "Amount open yet" %}:</div>
-        <div class="col-sm-5"></div>
-        <div class="col-sm-2 text-right">{{ open_amount | floatformat:2 }}</div>
-        {% endif %}
-    </div>
+        <h4>{% trans "Payments per" %} {{ today|date:"SHORT_DATE_FORMAT" }}:</h4>
+        {% for payment in payments %}
+        <div class="row">
+            <div class="col-sm-2">{{ payment.paid_date|date:"SHORT_DATE_FORMAT" }}</div>
+            <div class="col-sm-8">{{ payment.type }}</div>
+            <div class="col-sm-2 text-right">{{ payment.amount | floatformat:2 }}</div>
+        </div>    
+        {% endfor %}
     {% endif %}
-    
+    {% if open_amount != 0 %}
+        <div class="row font-weight-bold mt-3">
+            <div class="col-sm-5">{% trans "Amount open yet" %}:</div>
+            <div class="col-sm-5"></div>
+            <div class="col-sm-2 text-right">{{ open_amount | floatformat:2 }}</div>
+        </div>
+    {% endif %}
+ 
+    {% if bill.paid %}
+        <div class="row">
+            <div class="col">{% trans "Bill paid completely" %}</div>
+        </div>
+    {% endif %}
+
     <div class="row my-3">
         <div class="col"><a href="{% url 'jb:user-bill-pdf' bill.pk  %}">{% trans "Download as PDF" %}</a></div>
     </div>
 
-    {% if qr_svg %}
+    {% if bill.amount_open > 0 %}
+        {% if qr_svg %}
 {{ qr_svg | safe }}
-    {% else %}
+        {% else %}
     <p class="mt-5">
         {% config "organisation_address" as addr %}
         {% trans "Please pay specifying bill number to:" %}<br>
         IBAN {{ paymenttype.iban }}<br>
         {{ paymenttype.name }}<br>
         {% trans "in favor of" %}<br> 
         {{ addr.name }}, {{ addr.zip }} {{ addr.city }}
     </p>
+        {% endif %}
     {% endif %}   
 </div>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -32,25 +32,23 @@
 {{ bill.public_notes | default_if_none:"" }}
 {% if payments %}
 ****** {{%% ttrraannss ""PPaayymmeennttss ppeerr"" %%}} {{{{ ttooddaayy||ddaattee::""SSHHOORRTT__DDAATTEE__FFOORRMMAATT"" }}}}:: ******
 {% for payment in payments %}
 {{ payment.paid_date|date:"SHORT_DATE_FORMAT" }}
 {{ payment.type }}
 {{ payment.amount | floatformat:2 }}
-{% endfor %}
-{% if bill.paid %}
-{% trans "Bill paid completely" %}
-{% else %}
+{% endfor %} {% endif %} {% if open_amount != 0 %}
 {% trans "Amount open yet" %}:
 {{ open_amount | floatformat:2 }}
-{% endif %}
+{% endif %} {% if bill.paid %}
+{% trans "Bill paid completely" %}
 {% endif %}
 _{_%_ _t_r_a_n_s_ _"_D_o_w_n_l_o_a_d_ _a_s_ _P_D_F_"_ _%_}
-{% if qr_svg %} {{ qr_svg | safe }} {% else %}
+{% if bill.amount_open > 0 %} {% if qr_svg %} {{ qr_svg | safe }} {% else %}
 {% config "organisation_address" as addr %} {% trans "Please pay specifying
 bill number to:" %}
 IBAN {{ paymenttype.iban }}
 {{ paymenttype.name }}
 {% trans "in favor of" %}
 {{ addr.name }}, {{ addr.zip }} {{ addr.city }}
-{% endif %}
+{% endif %} {% endif %}
 {% endblock %}
```

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/jb/user_bills.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/jb/user_bills.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/templates/juntagrico/menu/admin.html` & `juntagrico_billing-1.6.1/juntagrico_billing/templates/juntagrico/menu/admin.html`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/tests/__init__.py` & `juntagrico_billing-1.6.1/juntagrico_billing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/tests/test_billbookings.py` & `juntagrico_billing-1.6.1/juntagrico_billing/tests/test_billbookings.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/tests/test_bills.py` & `juntagrico_billing-1.6.1/juntagrico_billing/tests/test_bills.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/tests/test_payment_processor.py` & `juntagrico_billing-1.6.1/juntagrico_billing/tests/test_payment_processor.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/tests/test_payment_reader.py` & `juntagrico_billing-1.6.1/juntagrico_billing/tests/test_payment_reader.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/urls.py` & `juntagrico_billing-1.6.1/juntagrico_billing/urls.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/util/billing.py` & `juntagrico_billing-1.6.1/juntagrico_billing/util/billing.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/util/bookings.py` & `juntagrico_billing-1.6.1/juntagrico_billing/util/bookings.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/util/esr.py` & `juntagrico_billing-1.6.1/juntagrico_billing/util/esr.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/util/payment_processor.py` & `juntagrico_billing-1.6.1/juntagrico_billing/util/payment_processor.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/util/payment_reader.py` & `juntagrico_billing-1.6.1/juntagrico_billing/util/payment_reader.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/util/pdfbill.py` & `juntagrico_billing-1.6.1/juntagrico_billing/util/pdfbill.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,32 +65,37 @@
 
         # public notes
         if bill.public_notes:
             story.append(Paragraph(bill.public_notes, self.text))
 
         self.render_payments(bill, story)
 
-        # payment notice
-        url = BillingConfig.duedate_notice_url()
-        if url:
-            text = _('The billed amount is due for payment according to ' + 'the due date notice found here:')
-            story.append(Paragraph(
-                f'{text} <link href="{url}">{url}</link>.',
-                self.text))
-
-        self.render_payslip(bill, story)
+        if bill.amount_open > 0:
+            # payment notice
+            url = BillingConfig.duedate_notice_url()
+            if url:
+                text = _('The billed amount is due for payment according to ' + 'the due date notice found here:')
+                story.append(Paragraph(
+                    f'{text} <link href="{url}">{url}</link>.',
+                    self.text))
+
+            self.render_payslip(bill, story)
+        else:
+            self.qrpayslip_drawing = None
 
         # build the pdf document
         # setting title and author prevents "anonymous" display
         # in certain pdf viewers (eg firefox)
-        doc = SimpleDocTemplate(
-            outfile,
-            title='',
-            author='',
-            bottomMargin=self.bottom_margin)
+        kwargs = {
+            'title': '',
+            'author': ''}
+        if self.qrpayslip_drawing:
+            kwargs['bottomMargin'] = self.bottom_margin
+
+        doc = SimpleDocTemplate(outfile, **kwargs)
 
         doc.build(
             story,
             onFirstPage=self.draw_payslip,
             onLaterPages=self.draw_payslip)
 
     def render_addresses(self, bill, story):
@@ -176,49 +181,50 @@
             )
         )
 
     def render_payments(self, bill, story):
         """
         render list of payments.
         """
+        sum = 0.0
+        lines = []
         if bill.payments.all():
             story.append(Paragraph('<b>%s %s</b>' % (
                 _('Payments per'),
                 self.date_format(datetime.date.today())), self.heading2))
 
-            lines = []
-            sum = 0.0
             for payment in bill.payments.all():
                 lines.append((
                     self.date_format(payment.paid_date),
                     payment.type,
                     Paragraph('%10.2f' % payment.amount, self.normalright)))
                 sum += payment.amount
 
             lines.append((
                 Paragraph(_('Total payments'), self.normal),
                 '',
                 Paragraph('%10.2f' % sum, self.normalright)))
 
-            if sum < bill.amount:
-                lines.append((
-                    Paragraph(_('Amount open yet'), self.normal),
-                    '',
-                    Paragraph(
-                        '<b>%10.2f</b>' % (bill.amount - sum),
-                        self.normalright)))
-
-            payments_table = Table(
-                lines, (4 * cm, None, 2 * cm),
-                style=self.table_style)
+        # total line
+        if sum != bill.amount:
+            lines.append((
+                Paragraph(_('Amount open yet'), self.normal),
+                '',
+                Paragraph(
+                    '<b>%10.2f</b>' % (bill.amount - sum),
+                    self.normalright)))
+
+        payments_table = Table(
+            lines, (4 * cm, None, 2 * cm),
+            style=self.table_style)
 
-            story.append(payments_table)
+        story.append(payments_table)
 
-            if sum >= bill.amount:
-                story.append(Paragraph(_('Bill paid completely'), self.normal))
+        if bill.paid:
+            story.append(Paragraph(_('Bill paid completely'), self.normal))
 
     def render_payslip(self, bill, story):
         """
         render payslip part with QR-Code
         the payslip is produced into a reporlab
         drawing, which is actually rendered by
         the page render function draw_payslip.
```

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/util/qrbill.py` & `juntagrico_billing-1.6.1/juntagrico_billing/util/qrbill.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/views.py` & `juntagrico_billing-1.6.1/juntagrico_billing/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,18 @@
     # only allow for bookkepper or the bills member
     if not (request.user.has_perms(('juntagrico.is_book_keeper',)) or bill.member == member):
         raise PermissionDenied()
 
     settings = Settings.objects.first()
 
     # add QR-Bill part
-    qr_svg = get_qrbill_svg(bill, settings.default_paymenttype)
+    if bill.amount_open > 0:
+        qr_svg = get_qrbill_svg(bill, settings.default_paymenttype)
+    else:
+        qr_svg = None
 
     renderdict = {
         'member': bill.member,
         'bill': bill,
         'today': date.today(),
         'payments': bill.payments.all(),
         'open_amount': bill.amount - bill.amount_paid,
```

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing/views_payment.py` & `juntagrico_billing-1.6.1/juntagrico_billing/views_payment.py`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing.egg-info/PKG-INFO` & `juntagrico_billing-1.6.1/juntagrico_billing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juntagrico-billing
-Version: 1.6.0
+Version: 1.6.1
 Summary: Send and manage bills in juntagrico.
 Author-email: juntagrico <python@juntagrico.org>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `juntagrico_billing-1.6.0/juntagrico_billing.egg-info/SOURCES.txt` & `juntagrico_billing-1.6.1/juntagrico_billing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `juntagrico_billing-1.6.0/pyproject.toml` & `juntagrico_billing-1.6.1/pyproject.toml`

 * *Files identical despite different names*

