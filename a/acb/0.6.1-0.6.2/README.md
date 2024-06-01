# Comparing `tmp/acb-0.6.1.tar.gz` & `tmp/acb-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.6.1.tar", last modified: Sun May 19 20:00:46 2024, max compression
+gzip compressed data, was "acb-0.6.2.tar", last modified: Mon May 20 11:03:19 2024, max compression
```

## Comparing `acb-0.6.1.tar` & `acb-0.6.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 acb-0.6.1/LICENSE
--rw-r--r--   0        0        0      772 2024-05-19 19:52:53.054302 acb-0.6.1/README.md
--rw-r--r--   0        0        0      880 2024-02-09 10:50:18.605994 acb-0.6.1/acb/__init__.py
--rw-r--r--   0        0        0      819 2024-01-16 17:26:09.434218 acb-0.6.1/acb/actions/__init__.py
--rw-r--r--   0        0        0     1180 2023-10-09 11:44:35.662080 acb-0.6.1/acb/actions/compress.py
--rw-r--r--   0        0        0     4784 2024-03-18 08:07:46.797620 acb-0.6.1/acb/actions/encode.py
--rw-r--r--   0        0        0      897 2023-10-11 15:39:52.116219 acb-0.6.1/acb/actions/hash.py
--rw-r--r--   0        0        0     5526 2024-03-18 07:52:52.122921 acb-0.6.1/acb/adapters/__init__.py
--rw-r--r--   0        0        0       60 2023-11-04 13:17:17.290924 acb-0.6.1/acb/adapters/app/__init__.py
--rw-r--r--   0        0        0      242 2024-02-09 17:35:46.026715 acb-0.6.1/acb/adapters/app/_base.py
--rw-r--r--   0        0        0     1286 2024-02-09 17:35:46.099339 acb-0.6.1/acb/adapters/app/main.py
--rw-r--r--   0        0        0       62 2023-11-04 13:17:17.342044 acb-0.6.1/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0     1610 2024-03-02 10:09:36.352462 acb-0.6.1/acb/adapters/cache/_base.py
--rw-r--r--   0        0        0      828 2024-02-04 19:59:42.029846 acb-0.6.1/acb/adapters/cache/memory.py
--rw-r--r--   0        0        0     1635 2024-02-09 18:00:21.800300 acb-0.6.1/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0       60 2023-11-04 13:17:17.324879 acb-0.6.1/acb/adapters/dns/__init__.py
--rw-r--r--   0        0        0     1044 2024-02-08 21:13:44.164932 acb-0.6.1/acb/adapters/dns/_base.py
--rw-r--r--   0        0        0     4880 2024-02-04 19:48:52.688550 acb-0.6.1/acb/adapters/dns/cloud_dns.py
--rw-r--r--   0        0        0       61 2023-11-04 13:17:17.317246 acb-0.6.1/acb/adapters/ftpd/__init__.py
--rw-r--r--   0        0        0      192 2024-02-08 21:13:44.096140 acb-0.6.1/acb/adapters/ftpd/_base.py
--rw-r--r--   0        0        0      927 2024-02-09 17:35:46.084380 acb-0.6.1/acb/adapters/ftpd/ftp.py
--rw-r--r--   0        0        0     1186 2024-02-09 11:37:04.876043 acb-0.6.1/acb/adapters/ftpd/sftp.py
--rw-r--r--   0        0        0       63 2023-11-04 13:17:17.311082 acb-0.6.1/acb/adapters/logger/__init__.py
--rw-r--r--   0        0        0      154 2024-02-08 21:13:44.117416 acb-0.6.1/acb/adapters/logger/_base.py
--rw-r--r--   0        0        0     3512 2024-04-12 00:33:56.007870 acb-0.6.1/acb/adapters/logger/loguru.py
--rw-r--r--   0        0        0       36 2023-11-06 07:39:19.522148 acb-0.6.1/acb/adapters/logger/structlog.py
--rw-r--r--   0        0        0       63 2024-02-07 20:56:24.207919 acb-0.6.1/acb/adapters/models/__init__.py
--rw-r--r--   0        0        0      247 2024-05-19 15:42:40.075662 acb-0.6.1/acb/adapters/models/_base.py
--rw-r--r--   0        0        0     2361 2024-05-19 15:48:46.214106 acb-0.6.1/acb/adapters/models/default.py
--rw-r--r--   0        0        0       67 2023-11-04 13:17:17.331356 acb-0.6.1/acb/adapters/monitoring/__init__.py
--rw-r--r--   0        0        0      223 2024-02-09 11:37:04.889721 acb-0.6.1/acb/adapters/monitoring/_base.py
--rw-r--r--   0        0        0      720 2024-02-04 19:48:52.574105 acb-0.6.1/acb/adapters/monitoring/sentry.py
--rw-r--r--   0        0        0       62 2023-11-04 13:17:17.303819 acb-0.6.1/acb/adapters/nosql/__init__.py
--rw-r--r--   0        0        0      210 2024-02-08 14:44:50.391598 acb-0.6.1/acb/adapters/nosql/_base.py
--rw-r--r--   0        0        0       36 2023-11-06 07:39:19.537543 acb-0.6.1/acb/adapters/nosql/firestore.py
--rw-r--r--   0        0        0       32 2023-11-06 07:39:19.533503 acb-0.6.1/acb/adapters/nosql/mongodb.py
--rw-r--r--   0        0        0      531 2023-09-27 19:36:20.695500 acb-0.6.1/acb/adapters/nosql/redis.py
--rw-r--r--   0        0        0       65 2023-11-04 13:17:17.335837 acb-0.6.1/acb/adapters/requests/__init__.py
--rw-r--r--   0        0        0     1028 2024-02-09 09:59:55.837594 acb-0.6.1/acb/adapters/requests/_base.py
--rw-r--r--   0        0        0     1673 2024-02-09 17:35:46.206206 acb-0.6.1/acb/adapters/requests/httpx.py
--rw-r--r--   0        0        0       63 2024-03-01 14:14:36.276395 acb-0.6.1/acb/adapters/secret/__init__.py
--rw-r--r--   0        0        0      776 2024-03-01 14:28:02.408356 acb-0.6.1/acb/adapters/secret/_base.py
--rw-r--r--   0        0        0       44 2023-11-06 07:39:19.541900 acb-0.6.1/acb/adapters/secret/infisical.py
--rw-r--r--   0        0        0     4617 2024-03-01 14:28:02.414547 acb-0.6.1/acb/adapters/secret/secret_manager.py
--rw-r--r--   0        0        0       61 2023-11-04 13:17:17.297294 acb-0.6.1/acb/adapters/smtp/__init__.py
--rw-r--r--   0        0        0     1264 2024-02-08 21:13:44.252071 acb-0.6.1/acb/adapters/smtp/_base.py
--rw-r--r--   0        0        0      513 2024-02-04 19:48:52.578362 acb-0.6.1/acb/adapters/smtp/gmail.py
--rw-r--r--   0        0        0     8886 2024-02-09 13:11:23.103262 acb-0.6.1/acb/adapters/smtp/mailgun.py
--rw-r--r--   0        0        0       60 2024-01-24 11:37:13.631301 acb-0.6.1/acb/adapters/sql/__init__.py
--rw-r--r--   0        0        0    12235 2024-02-09 13:11:23.094473 acb-0.6.1/acb/adapters/sql/_backup.py
--rw-r--r--   0        0        0     6668 2024-04-02 07:53:33.461560 acb-0.6.1/acb/adapters/sql/_base.py
--rw-r--r--   0        0        0       26 2024-02-08 14:45:26.613293 acb-0.6.1/acb/adapters/sql/_migrate.py
--rw-r--r--   0        0        0      253 2024-03-09 15:10:21.640219 acb-0.6.1/acb/adapters/sql/mysql.py
--rw-r--r--   0        0        0       32 2023-11-06 07:39:19.528015 acb-0.6.1/acb/adapters/sql/pgsql.py
--rw-r--r--   0        0        0       64 2023-11-04 13:17:17.284637 acb-0.6.1/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     5464 2024-03-02 09:47:43.464852 acb-0.6.1/acb/adapters/storage/_base.py
--rw-r--r--   0        0        0      368 2023-10-16 10:33:57.704006 acb-0.6.1/acb/adapters/storage/azure.py
--rw-r--r--   0        0        0     1456 2023-12-29 09:18:35.395587 acb-0.6.1/acb/adapters/storage/cloud_storage.py
--rw-r--r--   0        0        0      548 2024-02-04 19:48:52.633037 acb-0.6.1/acb/adapters/storage/file.py
--rw-r--r--   0        0        0      326 2024-02-04 19:48:52.631331 acb-0.6.1/acb/adapters/storage/memory.py
--rw-r--r--   0        0        0      381 2023-10-16 10:33:57.717425 acb-0.6.1/acb/adapters/storage/s3.py
--rw-r--r--   0        0        0    10433 2024-04-02 07:37:38.490567 acb-0.6.1/acb/config.py
--rw-r--r--   0        0        0     2212 2024-04-02 07:49:59.744042 acb-0.6.1/acb/debug.py
--rw-r--r--   0        0        0      587 2024-01-13 20:57:32.759244 acb-0.6.1/acb/depends.py
--rw-r--r--   0        0        0     3444 2024-05-19 20:00:46.441353 acb-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 acb-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 acb-0.6.2/LICENSE
+-rw-r--r--   0        0        0      772 2024-05-19 19:52:53.054302 acb-0.6.2/README.md
+-rw-r--r--   0        0        0      880 2024-02-09 10:50:18.605994 acb-0.6.2/acb/__init__.py
+-rw-r--r--   0        0        0      819 2024-01-16 17:26:09.434218 acb-0.6.2/acb/actions/__init__.py
+-rw-r--r--   0        0        0     1180 2023-10-09 11:44:35.662080 acb-0.6.2/acb/actions/compress.py
+-rw-r--r--   0        0        0     4784 2024-03-18 08:07:46.797620 acb-0.6.2/acb/actions/encode.py
+-rw-r--r--   0        0        0      897 2023-10-11 15:39:52.116219 acb-0.6.2/acb/actions/hash.py
+-rw-r--r--   0        0        0     5526 2024-03-18 07:52:52.122921 acb-0.6.2/acb/adapters/__init__.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:17:17.290924 acb-0.6.2/acb/adapters/app/__init__.py
+-rw-r--r--   0        0        0      242 2024-02-09 17:35:46.026715 acb-0.6.2/acb/adapters/app/_base.py
+-rw-r--r--   0        0        0     1286 2024-02-09 17:35:46.099339 acb-0.6.2/acb/adapters/app/main.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:17:17.342044 acb-0.6.2/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0     1610 2024-03-02 10:09:36.352462 acb-0.6.2/acb/adapters/cache/_base.py
+-rw-r--r--   0        0        0      828 2024-02-04 19:59:42.029846 acb-0.6.2/acb/adapters/cache/memory.py
+-rw-r--r--   0        0        0     1635 2024-02-09 18:00:21.800300 acb-0.6.2/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:17:17.324879 acb-0.6.2/acb/adapters/dns/__init__.py
+-rw-r--r--   0        0        0     1044 2024-02-08 21:13:44.164932 acb-0.6.2/acb/adapters/dns/_base.py
+-rw-r--r--   0        0        0     4880 2024-02-04 19:48:52.688550 acb-0.6.2/acb/adapters/dns/cloud_dns.py
+-rw-r--r--   0        0        0       61 2023-11-04 13:17:17.317246 acb-0.6.2/acb/adapters/ftpd/__init__.py
+-rw-r--r--   0        0        0      192 2024-02-08 21:13:44.096140 acb-0.6.2/acb/adapters/ftpd/_base.py
+-rw-r--r--   0        0        0      927 2024-02-09 17:35:46.084380 acb-0.6.2/acb/adapters/ftpd/ftp.py
+-rw-r--r--   0        0        0     1186 2024-02-09 11:37:04.876043 acb-0.6.2/acb/adapters/ftpd/sftp.py
+-rw-r--r--   0        0        0       63 2023-11-04 13:17:17.311082 acb-0.6.2/acb/adapters/logger/__init__.py
+-rw-r--r--   0        0        0      154 2024-02-08 21:13:44.117416 acb-0.6.2/acb/adapters/logger/_base.py
+-rw-r--r--   0        0        0     3512 2024-04-12 00:33:56.007870 acb-0.6.2/acb/adapters/logger/loguru.py
+-rw-r--r--   0        0        0       36 2023-11-06 07:39:19.522148 acb-0.6.2/acb/adapters/logger/structlog.py
+-rw-r--r--   0        0        0       63 2024-02-07 20:56:24.207919 acb-0.6.2/acb/adapters/models/__init__.py
+-rw-r--r--   0        0        0      247 2024-05-19 15:42:40.075662 acb-0.6.2/acb/adapters/models/_base.py
+-rw-r--r--   0        0        0     2361 2024-05-19 15:48:46.214106 acb-0.6.2/acb/adapters/models/default.py
+-rw-r--r--   0        0        0       67 2023-11-04 13:17:17.331356 acb-0.6.2/acb/adapters/monitoring/__init__.py
+-rw-r--r--   0        0        0      223 2024-02-09 11:37:04.889721 acb-0.6.2/acb/adapters/monitoring/_base.py
+-rw-r--r--   0        0        0      720 2024-02-04 19:48:52.574105 acb-0.6.2/acb/adapters/monitoring/sentry.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:17:17.303819 acb-0.6.2/acb/adapters/nosql/__init__.py
+-rw-r--r--   0        0        0      210 2024-02-08 14:44:50.391598 acb-0.6.2/acb/adapters/nosql/_base.py
+-rw-r--r--   0        0        0       36 2023-11-06 07:39:19.537543 acb-0.6.2/acb/adapters/nosql/firestore.py
+-rw-r--r--   0        0        0       32 2023-11-06 07:39:19.533503 acb-0.6.2/acb/adapters/nosql/mongodb.py
+-rw-r--r--   0        0        0      531 2023-09-27 19:36:20.695500 acb-0.6.2/acb/adapters/nosql/redis.py
+-rw-r--r--   0        0        0       65 2023-11-04 13:17:17.335837 acb-0.6.2/acb/adapters/requests/__init__.py
+-rw-r--r--   0        0        0     1028 2024-02-09 09:59:55.837594 acb-0.6.2/acb/adapters/requests/_base.py
+-rw-r--r--   0        0        0     1673 2024-02-09 17:35:46.206206 acb-0.6.2/acb/adapters/requests/httpx.py
+-rw-r--r--   0        0        0       63 2024-03-01 14:14:36.276395 acb-0.6.2/acb/adapters/secret/__init__.py
+-rw-r--r--   0        0        0      776 2024-03-01 14:28:02.408356 acb-0.6.2/acb/adapters/secret/_base.py
+-rw-r--r--   0        0        0       44 2023-11-06 07:39:19.541900 acb-0.6.2/acb/adapters/secret/infisical.py
+-rw-r--r--   0        0        0     4617 2024-03-01 14:28:02.414547 acb-0.6.2/acb/adapters/secret/secret_manager.py
+-rw-r--r--   0        0        0       61 2023-11-04 13:17:17.297294 acb-0.6.2/acb/adapters/smtp/__init__.py
+-rw-r--r--   0        0        0     1264 2024-02-08 21:13:44.252071 acb-0.6.2/acb/adapters/smtp/_base.py
+-rw-r--r--   0        0        0      513 2024-02-04 19:48:52.578362 acb-0.6.2/acb/adapters/smtp/gmail.py
+-rw-r--r--   0        0        0     8886 2024-02-09 13:11:23.103262 acb-0.6.2/acb/adapters/smtp/mailgun.py
+-rw-r--r--   0        0        0       60 2024-01-24 11:37:13.631301 acb-0.6.2/acb/adapters/sql/__init__.py
+-rw-r--r--   0        0        0    12235 2024-02-09 13:11:23.094473 acb-0.6.2/acb/adapters/sql/_backup.py
+-rw-r--r--   0        0        0     6668 2024-04-02 07:53:33.461560 acb-0.6.2/acb/adapters/sql/_base.py
+-rw-r--r--   0        0        0       26 2024-02-08 14:45:26.613293 acb-0.6.2/acb/adapters/sql/_migrate.py
+-rw-r--r--   0        0        0      253 2024-03-09 15:10:21.640219 acb-0.6.2/acb/adapters/sql/mysql.py
+-rw-r--r--   0        0        0       32 2023-11-06 07:39:19.528015 acb-0.6.2/acb/adapters/sql/pgsql.py
+-rw-r--r--   0        0        0       64 2023-11-04 13:17:17.284637 acb-0.6.2/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     5464 2024-03-02 09:47:43.464852 acb-0.6.2/acb/adapters/storage/_base.py
+-rw-r--r--   0        0        0      368 2023-10-16 10:33:57.704006 acb-0.6.2/acb/adapters/storage/azure.py
+-rw-r--r--   0        0        0     1456 2023-12-29 09:18:35.395587 acb-0.6.2/acb/adapters/storage/cloud_storage.py
+-rw-r--r--   0        0        0      548 2024-02-04 19:48:52.633037 acb-0.6.2/acb/adapters/storage/file.py
+-rw-r--r--   0        0        0      326 2024-02-04 19:48:52.631331 acb-0.6.2/acb/adapters/storage/memory.py
+-rw-r--r--   0        0        0      381 2023-10-16 10:33:57.717425 acb-0.6.2/acb/adapters/storage/s3.py
+-rw-r--r--   0        0        0    10433 2024-04-02 07:37:38.490567 acb-0.6.2/acb/config.py
+-rw-r--r--   0        0        0     2212 2024-04-02 07:49:59.744042 acb-0.6.2/acb/debug.py
+-rw-r--r--   0        0        0      587 2024-01-13 20:57:32.759244 acb-0.6.2/acb/depends.py
+-rw-r--r--   0        0        0     3444 2024-05-20 11:03:19.446234 acb-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 acb-0.6.2/PKG-INFO
```

### Comparing `acb-0.6.1/LICENSE` & `acb-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/README.md` & `acb-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/__init__.py` & `acb-0.6.2/acb/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/actions/__init__.py` & `acb-0.6.2/acb/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/actions/compress.py` & `acb-0.6.2/acb/actions/compress.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/actions/encode.py` & `acb-0.6.2/acb/actions/encode.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/actions/hash.py` & `acb-0.6.2/acb/actions/hash.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/__init__.py` & `acb-0.6.2/acb/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/app/main.py` & `acb-0.6.2/acb/adapters/app/main.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/cache/_base.py` & `acb-0.6.2/acb/adapters/cache/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/cache/memory.py` & `acb-0.6.2/acb/adapters/cache/memory.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/cache/redis.py` & `acb-0.6.2/acb/adapters/cache/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/dns/_base.py` & `acb-0.6.2/acb/adapters/dns/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/dns/cloud_dns.py` & `acb-0.6.2/acb/adapters/dns/cloud_dns.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/ftpd/ftp.py` & `acb-0.6.2/acb/adapters/ftpd/ftp.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/ftpd/sftp.py` & `acb-0.6.2/acb/adapters/ftpd/sftp.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/logger/loguru.py` & `acb-0.6.2/acb/adapters/logger/loguru.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/models/default.py` & `acb-0.6.2/acb/adapters/models/default.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/monitoring/sentry.py` & `acb-0.6.2/acb/adapters/monitoring/sentry.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/nosql/redis.py` & `acb-0.6.2/acb/adapters/nosql/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/requests/_base.py` & `acb-0.6.2/acb/adapters/requests/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/requests/httpx.py` & `acb-0.6.2/acb/adapters/requests/httpx.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/secret/_base.py` & `acb-0.6.2/acb/adapters/secret/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/secret/secret_manager.py` & `acb-0.6.2/acb/adapters/secret/secret_manager.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/smtp/_base.py` & `acb-0.6.2/acb/adapters/smtp/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/smtp/gmail.py` & `acb-0.6.2/acb/adapters/smtp/gmail.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/smtp/mailgun.py` & `acb-0.6.2/acb/adapters/smtp/mailgun.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/sql/_backup.py` & `acb-0.6.2/acb/adapters/sql/_backup.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/sql/_base.py` & `acb-0.6.2/acb/adapters/sql/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/storage/_base.py` & `acb-0.6.2/acb/adapters/storage/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/storage/cloud_storage.py` & `acb-0.6.2/acb/adapters/storage/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/adapters/storage/file.py` & `acb-0.6.2/acb/adapters/storage/file.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/config.py` & `acb-0.6.2/acb/config.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/debug.py` & `acb-0.6.2/acb/debug.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/acb/depends.py` & `acb-0.6.2/acb/depends.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.1/pyproject.toml` & `acb-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,37 +38,37 @@
 [tool.creosote]
 paths = [
     "acb",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
     "pytest",
-    "pdm-bump",
     "pdm",
-    "pyfiglet",
     "pre-commit",
-    "autotyping",
     "ulid-py",
+    "pdm-bump",
     "phonenumbers",
-    "alive-progress",
     "pyyaml",
+    "pyfiglet",
+    "autotyping",
+    "alive-progress",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "acb",
 ]
 skips = [
     "B603",
-    "B403",
-    "B404",
     "B113",
+    "B404",
+    "B403",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "acb",
 ]
@@ -89,15 +89,15 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "acb"
-version = "0.6.1"
+version = "0.6.2"
 description = "Asynchronous Component Base"
 dependencies = [
     "itsdangerous>=2.2.0",
     "arrow>=1.3.0",
     "dill>=0.3.8",
     "blake3>=0.4.1",
     "loguru>=0.7.2",
```

### Comparing `acb-0.6.1/PKG-INFO` & `acb-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acb
-Version: 0.6.1
+Version: 0.6.2
 Summary: Asynchronous Component Base
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Pydantic
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acb Version: 0.6.1 Summary: Asynchronous Component
+Metadata-Version: 2.1 Name: acb Version: 0.6.2 Summary: Asynchronous Component
 Base Author-Email: lesleslie
 wedgwoodwebworks.com> License: BSD-3-Clause Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.12 Classifier: Framework :: Pydantic Classifier:
 Framework :: Pydantic :: 2 Classifier: Framework :: AsyncIO Classifier: Typing
 :: Typed Classifier: License :: OSI Approved :: BSD License Classifier:
 Development Status :: 3 - Alpha Classifier: Topic :: Software Development ::
```

