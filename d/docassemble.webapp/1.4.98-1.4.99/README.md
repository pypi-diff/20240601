# Comparing `tmp/docassemble.webapp-1.4.98.tar.gz` & `tmp/docassemble.webapp-1.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.webapp-1.4.98.tar", last modified: Thu Feb 29 18:39:32 2024, max compression
+gzip compressed data, was "docassemble.webapp-1.4.99.tar", last modified: Sat Mar  2 13:09:55 2024, max compression
```

## Comparing `docassemble.webapp-1.4.98.tar` & `docassemble.webapp-1.4.99.tar`

### file list

```diff
@@ -1,1296 +1,1296 @@
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1085 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/LICENSE.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:58.000000 docassemble.webapp-1.4.98/MANIFEST.in
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      615 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.433990 docassemble.webapp-1.4.98/docassemble/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       56 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       23 2024-02-29 18:38:53.000000 docassemble.webapp-1.4.98/docassemble/webapp/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/alembic/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       38 2017-08-13 12:29:02.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/README
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2280 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/env.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      548 2018-05-13 01:00:37.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/script.py.mako
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      538 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/025e06b85efc_package_github_branch.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4550 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/4328f2c08f05_add_indexes.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      557 2018-05-13 01:02:46.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/66f71cf543a4_temp_user_id_to_userdictkeys.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      606 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      511 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/77e8971ffcbf_first_alembic_revision.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3897 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4158 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      527 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/c2ef4831ef76_user_last_login.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1226 2018-05-16 02:31:37.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      729 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      548 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/fd1547c94c46_add_a_column_for_the_voicerss_voice.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1647 2017-08-13 12:29:02.000000 docassemble.webapp-1.4.98/docassemble/webapp/alembic.ini
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1098 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/api_key.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2172 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/app_object.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2558 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/app_socket.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    65126 2024-01-19 19:19:27.000000 docassemble.webapp-1.4.98/docassemble/webapp/backend.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      714 2023-12-11 01:54:38.000000 docassemble.webapp-1.4.98/docassemble/webapp/cleanup_sessions.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2883 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/clicksend.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      719 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/cloud.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      958 2024-02-29 17:36:07.000000 docassemble.webapp-1.4.98/docassemble/webapp/cloud_deregister.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1111 2024-02-29 17:37:00.000000 docassemble.webapp-1.4.98/docassemble/webapp/cloud_register.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      518 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/config_worker.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/core/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      167 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/core/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6445 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/core/models.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15993 2023-12-11 01:53:26.000000 docassemble.webapp-1.4.98/docassemble/webapp/create_tables.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      386 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/createminio.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17573 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/cron.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1931 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/da_flask_mail.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      603 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/daredis.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/data/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        7 2024-02-29 18:38:53.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/VERSION.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6913 2024-02-29 18:31:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/db-schema.txt
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/data/questions/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18794 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/questions/wizard-template.yml
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/data/static/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    10351 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/android-chrome-192x192.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    29787 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/android-chrome-512x512.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3030 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/apple-touch-icon.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      246 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/browserconfig.xml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      632 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/favicon-16x16.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1400 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/favicon-32x32.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    15086 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/favicon.ico
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3752 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/mstile-150x150.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3485 2017-04-02 22:18:46.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/safari-pinned-tab.svg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      426 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/site.webmanifest
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       26 2017-04-02 20:26:52.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/robots.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4638 2017-05-16 01:19:25.000000 docassemble.webapp-1.4.98/docassemble/webapp/data/static/test-document.docx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2568 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/database.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2018 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/db_object.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      811 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/deregister.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10218 2024-02-29 11:46:16.000000 docassemble.webapp-1.4.98/docassemble/webapp/develop.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14301 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/file_access.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      335 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/file_number.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    36419 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/files.py
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     4863 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/fix_postgresql_tables.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2492 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/fixpickle.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1954 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/google_api.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5234 2023-12-22 03:35:08.000000 docassemble.webapp-1.4.98/docassemble/webapp/info.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3985 2024-02-14 13:48:04.000000 docassemble.webapp-1.4.98/docassemble/webapp/install_certs.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3470 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/jsonstore.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1829 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/list-cloud.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2107 2023-12-21 01:20:57.000000 docassemble.webapp-1.4.98/docassemble/webapp/listlog.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      273 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/logserver.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    35526 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/machinelearning.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4537 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/mailgun_mail.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/packages/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-04-15 09:56:46.000000 docassemble.webapp-1.4.98/docassemble/webapp/packages/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2008 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/packages/models.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26073 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/playground.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7721 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/process_email.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1000 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/register.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2328 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/restart.py
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     1917 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/retrieve_js_and_css.sh
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      120 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/run.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2952 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/screenreader.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5398 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/sendgrid_mail.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1603119 2024-02-29 17:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/server.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8076 2024-02-29 18:38:53.000000 docassemble.webapp-1.4.98/docassemble/webapp/setup.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    52786 2024-01-19 19:38:36.000000 docassemble.webapp-1.4.98/docassemble/webapp/socketserver.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       97 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/socketstop.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      217 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/sockettest.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      309 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/sqlalchemy_url.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      139 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/starthook.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.437990 docassemble.webapp-1.4.98/docassemble/webapp/static/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/app/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   143452 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.eot
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60774 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.json
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   347588 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.ttf
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   160576 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.woff
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   125116 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.woff2
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22174 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/additional-methods.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   170612 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/adminbundle.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31831 2023-12-06 11:50:37.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/app.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22291 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/app.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24213 2023-12-06 13:04:03.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/app.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12058 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/app.min.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      482 2018-06-05 11:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/auth0-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1229 2017-03-18 01:24:28.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/azure-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      147 2018-09-13 21:10:37.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/blank.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    45509 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/bundle.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   500762 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/bundle.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   410814 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/bundlenojquery.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   412188 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/bundlewrapjquery.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1150 2017-04-02 21:01:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/chat.ico
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1257 2015-04-04 15:28:40.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/facebook-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1387 2015-10-05 03:38:54.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/google-logo.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    89947 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/jquery.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24601 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/jquery.validate.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3407 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/jquery.visible.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2058 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/jquery.visible.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1681 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/js.cookie.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1264 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/keycloak-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      351 2016-07-05 02:35:15.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/option-vertical.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2685 2016-07-05 02:35:15.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/option-vertical.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      430 2017-06-15 10:37:03.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/phone-logo.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21977 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/playgroundbundle.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   669455 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/playgroundbundle.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4036 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/pygments.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1930 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/pygments.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    44191 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/socket.io.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   163765 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/socket.io.min.js.map
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1539 2015-04-04 16:31:24.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/twitter-logo.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2717 2018-09-18 02:49:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/upload.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2109 2016-09-25 16:03:42.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/webrtc.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2365 2016-10-18 04:15:55.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/webrtc.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3020 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/wrap.svg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1561 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/app/zitadel-logo.png
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/areyousure/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11061 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/areyousure/README.md
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5559 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/areyousure/jquery.are-you-sure.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.429990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   232948 2023-12-02 01:47:15.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   589161 2023-12-02 01:47:22.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    80663 2023-12-02 01:47:47.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   331886 2023-12-02 01:47:59.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60577 2023-12-02 01:47:54.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   220350 2023-12-02 01:48:04.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2927 2017-09-24 22:47:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      881 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      765 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.min.css
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/js/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    23056 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12055 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3215 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/CODE_OF_CONDUCT.md
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     6399 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/CONTRIBUTING.md
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      105 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/FUNDING.yml
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     1443 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/ISSUE_TEMPLATE.md
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)      245 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      448 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/config.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      707 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/stale.yml
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)       67 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.gitignore
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       68 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.npmignore
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     1555 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/LICENSE.md
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    11990 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2042 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1728 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.min.css
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    12262 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.css
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     9020 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.min.css
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/img/
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     2670 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/img/loading-sm.gif
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)      847 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/img/loading.gif
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   251909 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   125022 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5592 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/LANG.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6812 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ar.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6175 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/az.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6582 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/bg.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5996 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ca.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5884 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/cr.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6129 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/cs.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5836 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/da.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6071 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/de.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     8175 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/el.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6111 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/es.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5483 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/et.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7063 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/fa.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5227 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/fi.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6253 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/fr.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6087 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/gl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6093 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/he.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6241 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/hu.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5819 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/id.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6024 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/it.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7319 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ja.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     8967 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ka.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6230 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/kr.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6110 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/kz.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5887 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/lt.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5916 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/nl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5526 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/no.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5835 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/pl.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6137 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt-BR.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6118 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5971 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ro.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7694 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ru.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6126 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/sk.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5574 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/sl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5801 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/sr-latn.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5676 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/sv.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7300 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/th.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6129 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/tr.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7360 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/uk.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6413 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/uz.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6012 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/vi.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5562 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh-TW.js
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5587 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    75990 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    29919 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   120577 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    42997 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.429990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     4052 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.css
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     1607 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3116 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1164 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.441990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4042 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3070 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3257 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2554 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4075 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3116 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3289 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2600 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fa/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     2024 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1782 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fas/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2074 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1834 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/gly/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     2127 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/gly/theme.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1871 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/gly/theme.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      221 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/.codeclimate.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      103 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/.npmignore
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        6 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/.nvmrc
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      774 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/.sass-lint.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      107 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/.travis.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1207 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/LICENSE.md
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15714 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    84330 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    51588 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11286 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9935 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.min.css
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       87 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/.editorconfig
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      160 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/.gitattributes
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      169 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/.npmignore
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12802 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/AUTHORS
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   114675 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/CHANGELOG.md
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1107 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/LICENSE
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1944 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.429990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/comment/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9230 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/comment/comment.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4849 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/comment/continuecomment.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/dialog/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      507 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/dialog/dialog.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5252 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/dialog/dialog.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1546 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/autorefresh.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      116 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/fullscreen.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1497 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/fullscreen.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4661 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/panel.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2831 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/placeholder.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1918 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/rulers.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7123 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/closebrackets.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8544 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/closetag.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3989 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/continuelist.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6818 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/matchbrackets.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2358 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/matchtags.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1006 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/trailingspace.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4475 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/brace-fold.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2164 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/comment-fold.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4985 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/foldcode.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      435 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/foldgutter.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5539 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/foldgutter.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1676 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/indent-fold.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1608 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/markdown-fold.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6702 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/xml-fold.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1683 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/anyword-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2580 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/css-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11458 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/html-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6855 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/javascript-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      649 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/show-hint.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19792 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/show-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9595 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/sql-hint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5705 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/xml-hint.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1468 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/coffeescript-lint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1312 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/css-lint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1991 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/html-lint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2161 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/javascript-lint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1335 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/json-lint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3035 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/lint.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9987 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/lint.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1257 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/yaml-lint.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/merge/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3423 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/merge/merge.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38660 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/merge/merge.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2543 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/loadmode.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5191 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/multiplex.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1367 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/multiplex_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3243 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/overlay.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8076 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/simple.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1308 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/colorize.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12053 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/runmode-standalone.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2777 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/runmode.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11498 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/runmode.node.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4630 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/annotatescrollbar.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1584 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/scrollpastend.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1347 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5465 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2143 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/jump-to-line.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6216 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/match-highlighter.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      188 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3858 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11863 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/search.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12234 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/searchcursor.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.445990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/selection/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2509 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/selection/active-line.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3849 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/selection/mark-selection.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3295 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/selection/selection-pointer.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/tern/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1872 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/tern/tern.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26448 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/tern/tern.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1211 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/tern/worker.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/wrap/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6109 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/wrap/hardwrap.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/keymap/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16336 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/keymap/emacs.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26694 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/keymap/sublime.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   232203 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/keymap/vim.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/lib/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8720 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/lib/codemirror.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   401787 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/lib/codemirror.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/apl/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4739 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/apl/apl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2190 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/apl/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asciiarmor/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2449 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asciiarmor/asciiarmor.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1340 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asciiarmor/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asn.1/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7738 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asn.1/asn.1.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2275 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asn.1/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asterisk/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8142 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asterisk/asterisk.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4661 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asterisk/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/brainfuck/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2177 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/brainfuck/brainfuck.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3349 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/brainfuck/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    37259 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/clike.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10561 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28529 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/scala.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5465 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clojure/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15391 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clojure/clojure.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2738 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clojure/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18973 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clojure/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cmake/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2603 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cmake/cmake.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4163 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cmake/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cobol/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10325 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cobol/cobol.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8095 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cobol/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/coffeescript/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10038 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/coffeescript/coffeescript.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22488 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/coffeescript/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/commonlisp/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4597 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/commonlisp/commonlisp.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6702 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/commonlisp/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/crystal/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12865 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/crystal/crystal.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2616 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/crystal/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    40492 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/css.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2840 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/gss.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      463 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/gss_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2222 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4075 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/less.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1910 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/less_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2811 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/scss.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3182 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/scss_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7523 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cypher/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7130 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cypher/cypher.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1976 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cypher/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1346 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cypher/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/d/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7706 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/d/d.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6343 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/d/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      416 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/d/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dart/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5490 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dart/dart.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1638 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dart/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/diff/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1141 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/diff/diff.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4420 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/diff/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/django/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11794 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/django/django.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2072 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/django/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dockerfile/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4741 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dockerfile/dockerfile.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2262 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dockerfile/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5232 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dockerfile/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dtd/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4815 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dtd/dtd.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3332 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dtd/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dylan/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10115 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dylan/dylan.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13027 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dylan/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2741 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dylan/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ebnf/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6072 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ebnf/ebnf.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2445 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ebnf/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ecl/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8846 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ecl/ecl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1420 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ecl/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/eiffel/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3747 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/eiffel/eiffel.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13209 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/eiffel/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/elm/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5657 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/elm/elm.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1635 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/elm/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/erlang/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18876 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/erlang/erlang.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2163 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/erlang/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/factor/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3559 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/factor/factor.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2035 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/factor/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fcl/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4706 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fcl/fcl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3107 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fcl/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/forth/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5233 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/forth/forth.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1794 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/forth/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fortran/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8634 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fortran/fortran.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2487 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fortran/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gas/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9147 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gas/gas.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1851 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gas/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gfm/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5106 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gfm/gfm.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3655 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gfm/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6872 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gfm/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gherkin/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13260 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gherkin/gherkin.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1577 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gherkin/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/go/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6064 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/go/go.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2185 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/go/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/groovy/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8411 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/groovy/groovy.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2188 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/groovy/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haml/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5357 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haml/haml.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2082 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haml/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3013 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haml/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/handlebars/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2408 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/handlebars/handlebars.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2298 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/handlebars/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8167 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell/haskell.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2189 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell-literate/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1393 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell-literate/haskell-literate.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9385 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell-literate/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haxe/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17566 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haxe/haxe.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2572 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haxe/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlembedded/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1723 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlembedded/htmlembedded.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2081 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlembedded/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.449990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlmixed/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5688 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlmixed/htmlmixed.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3430 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlmixed/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/http/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2798 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/http/http.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1388 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/http/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/idl/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14893 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/idl/idl.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1686 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/idl/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8367 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4668 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38894 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/javascript.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2138 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/json-ld.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20328 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1610 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/typescript.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jinja2/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2061 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jinja2/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5907 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jinja2/jinja2.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jsx/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2405 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jsx/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5233 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jsx/jsx.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4277 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jsx/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/julia/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2428 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/julia/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11358 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/julia/julia.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/livescript/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9854 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/livescript/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7671 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/livescript/livescript.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/lua/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2087 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/lua/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6005 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/lua/lua.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28731 2022-03-06 21:30:57.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/damarkdown.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12782 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31325 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/markdown.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38880 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mathematica/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2265 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mathematica/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5641 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mathematica/mathematica.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mbox/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1304 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mbox/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3652 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mbox/mbox.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15926 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/meta.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mirc/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5867 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mirc/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10080 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mirc/mirc.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mllike/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4679 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mllike/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8725 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mllike/mllike.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/modelica/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2018 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/modelica/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6936 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/modelica/modelica.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4321 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6917 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/mscgen.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3829 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/mscgen_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3292 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/msgenny_test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4206 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/xu_test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mumps/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2603 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mumps/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5356 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mumps/mumps.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nginx/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5256 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nginx/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10167 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nginx/nginx.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nsis/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1775 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nsis/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8107 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nsis/nsis.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ntriples/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2443 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ntriples/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7044 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ntriples/ntriples.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/octave/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1858 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/octave/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4528 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/octave/octave.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/oz/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1354 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/oz/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6663 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/oz/oz.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pascal/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1435 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pascal/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4207 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pascal/pascal.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pegjs/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1885 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pegjs/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3532 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pegjs/pegjs.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/perl/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1537 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/perl/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56084 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/perl/perl.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/php/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1995 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/php/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18339 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/php/php.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6640 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/php/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pig/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1486 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pig/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5813 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pig/pig.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/powershell/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7481 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/powershell/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12921 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/powershell/powershell.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2968 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/powershell/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/properties/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1566 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/properties/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2174 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/properties/properties.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/protobuf/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2637 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/protobuf/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2192 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/protobuf/protobuf.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pug/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2484 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pug/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15991 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pug/pug.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/puppet/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3271 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/puppet/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7575 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/puppet/puppet.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/python/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6270 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/python/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14952 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/python/python.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2850 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/python/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/q/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8956 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/q/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6596 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/q/q.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/r/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2529 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/r/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6740 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/r/r.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rpm/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rpm/changes/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2168 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rpm/changes/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4618 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rpm/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3774 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rpm/rpm.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rst/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17764 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rst/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17550 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rst/rst.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ruby/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5762 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ruby/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10703 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ruby/ruby.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      855 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ruby/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rust/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1525 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rust/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3100 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rust/rust.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      995 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rust/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sas/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1849 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sas/index.html
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    15458 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sas/sas.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sass/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1642 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sass/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11619 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sass/sass.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5141 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sass/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/scheme/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2565 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/scheme/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15266 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/scheme/scheme.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/shell/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1787 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/shell/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5383 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/shell/shell.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2377 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/shell/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sieve/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2346 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sieve/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4288 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sieve/sieve.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/slim/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2931 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/slim/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18029 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/slim/slim.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3133 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/slim/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smalltalk/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1915 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smalltalk/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4546 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smalltalk/smalltalk.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smarty/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3968 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smarty/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6843 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smarty/smarty.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.453990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/solr/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1360 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/solr/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2675 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/solr/solr.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/soy/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1934 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/soy/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23022 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/soy/soy.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12338 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/soy/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sparql/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1784 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sparql/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6901 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sparql/sparql.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/spreadsheet/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1387 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/spreadsheet/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3142 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/spreadsheet/spreadsheet.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sql/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3403 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sql/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    59293 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sql/sql.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stex/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4338 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stex/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7798 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stex/stex.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3704 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stex/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stylus/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2483 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stylus/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    42246 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stylus/stylus.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/swift/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1773 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/swift/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7527 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/swift/swift.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9428 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/swift/test.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tcl/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6308 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tcl/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4947 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tcl/tcl.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/textile/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4357 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/textile/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9442 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/textile/test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13838 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/textile/textile.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiddlywiki/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4574 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiddlywiki/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      220 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiddlywiki/tiddlywiki.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8512 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiddlywiki/tiddlywiki.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiki/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1717 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiki/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      439 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiki/tiki.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8465 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiki/tiki.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/toml/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1835 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/toml/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2900 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/toml/toml.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tornado/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1797 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tornado/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2499 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tornado/tornado.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/troff/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4476 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/troff/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2395 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/troff/troff.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3543 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10158 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn/ttcn.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn-cfg/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3658 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn-cfg/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7860 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn-cfg/ttcn-cfg.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/turtle/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1539 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/turtle/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4852 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/turtle/turtle.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/twig/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1460 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/twig/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4568 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/twig/twig.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vb/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1472 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vb/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9839 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vb/vb.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vbscript/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1512 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vbscript/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13798 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vbscript/vbscript.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/velocity/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3311 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/velocity/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7131 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/velocity/velocity.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/verilog/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2614 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/verilog/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12323 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/verilog/test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29786 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/verilog/verilog.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vhdl/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2481 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vhdl/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6707 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vhdl/vhdl.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vue/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2073 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vue/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2887 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vue/vue.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/wast/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1784 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/wast/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21987 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/wast/test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4807 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/wast/wast.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/webidl/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2159 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/webidl/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5787 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/webidl/webidl.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xml/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2166 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xml/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1761 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xml/test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13353 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xml/xml.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xquery/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8662 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xquery/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5114 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xquery/test.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15755 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xquery/xquery.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yacas/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2187 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yacas/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5429 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yacas/yacas.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2109 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3735 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml/yaml.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3083 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2509 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.457991 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/z80/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1401 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/z80/index.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3580 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/z80/z80.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.461990 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1987 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/3024-day.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2076 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/3024-night.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7702 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/abbott.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1969 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/abcdef.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      103 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ambiance-mobile.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26493 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ambiance.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2421 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ayu-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2538 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ayu-mirage.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2292 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/base16-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2124 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/base16-light.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1413 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/bespin.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1931 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/blackboard.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1726 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/cobalt.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1677 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/colorforth.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2686 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/darcula.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2042 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/dracula.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2614 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/duotone-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2719 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/duotone-light.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1187 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/eclipse.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      781 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/elegant.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2286 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/erlang-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1918 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/gruvbox-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1469 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/hopscotch.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2515 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/icecoder.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1672 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/idea.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1442 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/isotope.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      517 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/juejin.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2637 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/lesser-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3991 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/liquibyte.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1914 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/lucario.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2607 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/material-darker.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2767 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/material-ocean.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2923 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/material-palenight.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2533 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/material.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2112 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/mbo.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5196 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/mdn-like.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1856 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/midnight.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2179 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/monokai.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2369 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/moxer.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      688 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/neat.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      947 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/neo.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1746 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/night.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2088 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/nord.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2440 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/oceanic-next.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1804 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/panda-syntax.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2078 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/paraiso-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2078 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/paraiso-light.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2485 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/pastel-on-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1514 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/railscasts.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1801 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/rubyblue.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2009 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/seti.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2440 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/shadowfox.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5337 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/solarized.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      751 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ssms.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1940 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/the-matrix.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1769 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/tomorrow-night-bright.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2439 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/tomorrow-night-eighties.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2440 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ttcn.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2164 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/twilight.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2142 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/vibrant-ink.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3033 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/xq-dark.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2255 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/xq-light.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1884 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/yeti.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3075 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/yonce.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2001 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/zenburn.css
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.469991 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17268 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/actions-parameters.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12998 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/actions.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11717 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/age_in_years.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56854 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/alignment.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21522 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/all-true.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    50677 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/allow-emailing-false.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4389 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/as-datetime.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   135261 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/attachment-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13634 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/audio.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19808 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/auto-terms.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11382 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action_flash.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11382 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action_javascript.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action_refresh.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action_with_response_action.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11359 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_response_action_flash.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10740 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/buttons-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21691 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/buttons-icons.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12060 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/buttons-labels.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13126 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/buttons.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6047 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/capitalize.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4394 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/chat-partners-available.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12769 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/check-in.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11099 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices-combobox.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13705 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices-dropdown.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22972 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices-icons.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19684 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices-with-default.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19893 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10569 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7383 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/comment.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10803 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/continue-button-label.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14401 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/continue.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11638 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/country.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26548 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/cron.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    43642 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/css.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5623 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/currency.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5285 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/current-datetime.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16116 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/dadict.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3988 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/dafile.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11814 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/database_storage.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11803 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/date-difference.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12966 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/date-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4232 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/date-interval.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9474 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/date-parts.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5541 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/dead-end.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13778 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/decoration.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9069 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/def.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11281 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/defined.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8039 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/del.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4006 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/device.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11725 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/dialog-box.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    55811 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document-docx.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58370 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document-file.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60880 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document-language.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    67827 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document-variable-name.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56752 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34388 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/docx-template-table.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34757 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/docx-template.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14541 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/doors.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10627 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/email-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18631 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/email-to-case-simple.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18631 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/email-to-case.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18838 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/emoji-inline.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11709 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exists.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7103 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exit-buttons.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10180 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exit-choices.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12116 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exit-url.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9401 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exit.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8708 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/external_files.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25112 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-checkboxes.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12060 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-choices-combobox.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11548 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-choices.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16234 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-mc-exclude.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16234 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-mc.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23154 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-noyesmaybe.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24536 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-yesno.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21736 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-yesnomaybe.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24516 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-yesnoradio.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19513 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-yesnowide.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21231 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fix-punctuation.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4717 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/for_fruit.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8039 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/force-ask.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8259 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/force-gather.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32606 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/formatting.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9089 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-dict-object.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17024 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-dict-value.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13811 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-dict.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9218 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-fruit-at-least-two.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11776 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-fruit-gather.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11099 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-fruit-number.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14113 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-fruit.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14906 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-set-object.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10364 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-set.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8716 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/generic-object.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4433 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/get-default-timezone.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16575 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/help-damages-audio.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23318 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/help.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20326 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/hideif-boolean.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29068 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/html.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15386 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/image-sets.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14948 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/images.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9555 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/imports.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/include.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15384 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/indefinite-article.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14115 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/initial.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3633 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/interface.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17183 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/interview-help.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20436 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/interview-url.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21938 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/interview_url_action.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3505 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/js_action_call.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11157 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/js_url_action.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2337 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/js_variables.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15459 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/label.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14870 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/language.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8437 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/language_from_browser.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4335 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/language_from_browser_restricted.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3704 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/lists.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25876 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/loading-legal.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23906 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/loading-util.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7878 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/madlibs.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3546 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-01.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3118 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-02.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6352 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-03.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6352 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-04.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3292 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-05.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9163 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-06.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2462 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-07.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6832 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-09.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10569 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mandatory.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    67776 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/markdown.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10310 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/menu-item.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10655 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/message.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15962 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/metadata.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16028 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/min.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11344 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/minlength.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9444 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-classify.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9181 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-datatype.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18348 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-export-yaml.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      354 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-export.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6828 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-predict.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6828 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-save-and-predict.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9658 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mlarea-datatype.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11104 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/modules.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11685 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/money-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9787 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/need.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14471 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/nested-loop.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12230 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/nice-number.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10407 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/no-label-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    27436 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/note.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12595 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/noun-plural.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11084 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/noyes.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14737 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/number-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16214 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object-checkboxes.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14699 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object-disable-others.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13219 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object-radio.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10235 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object-selections.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10453 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17062 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/objects.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22843 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ocr-chord.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20326 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ocr.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23012 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/optional-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8274 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ordinal-number.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12679 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/other.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58333 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/page-numbers.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16253 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/password-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9496 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/past-tense.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    51015 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pdf-a.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19862 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pdf-fill-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12171 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pdf-fill-signature.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24929 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pdf-fill.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12918 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/periodic-amount.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11325 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/periodic-value.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19272 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/prevent-back.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19272 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/prevent-going-back.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9509 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/progress-features.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9795 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/progress.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18786 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pull-down-with-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15669 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pull-down.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20531 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/qr-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2952 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/quantity-noun.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13474 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/quote_paragraphs.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    27426 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/radio-list.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21419 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/range.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11560 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/reconsider.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22042 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/redis.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8298 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/refresh.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10247 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/reload.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7496 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/required-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11560 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/reset.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10798 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/response-json.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7484 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/response-svg.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      825 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/response.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22273 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/resume-button-label.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    45696 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/review.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23999 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/salutation.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24041 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/save-url-to-file.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9746 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/script.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20961 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords-code.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28927 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords-get-sections.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22015 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords-review.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22106 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords-set-sections.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22800 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28276 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9226 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/send-email.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14870 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/set-language.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15954 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/showif-boolean.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16875 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/showif.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34936 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/shuffle.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22291 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/signature.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5202 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/signin.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58915 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/single-spacing.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5901 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/space-underscore.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10375 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/state.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18965 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/static_image.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10109 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/subdivision-type.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7290 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/table-mako.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6771 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/table-markdown.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7124 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/table.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12382 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/target-template.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32422 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/template-file.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    37584 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/template-subject.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32422 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/template.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19527 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/terms.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10820 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-box-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20969 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-default.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18283 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-field.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25945 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-help.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23948 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-hint.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13398 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/timezone-list.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5432 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/title-case.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4107 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/today.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26745 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/under.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25496 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/upload-multiple.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24708 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/upload.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17380 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/url-of.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    41705 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/valid-formats.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11304 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/value.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/variables_as_json.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   245391 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/video.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8585 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/yesno-custom.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11084 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/yesno.png
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11702 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/examples/yesnomaybe.png
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.433990 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.473991 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1627443 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/all.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1597188 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/all.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   477868 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/brands.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   477004 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/brands.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    39338 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/conflict-detection.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24798 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/conflict-detection.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   121752 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/fontawesome.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    88423 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/fontawesome.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   152666 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/regular.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   150749 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/regular.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   875814 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/solid.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   881669 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/solid.min.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    33609 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/v4-shims.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32952 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/v4-shims.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.473991 docassemble.webapp-1.4.98/docassemble/webapp/static/img/
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     2670 2023-10-25 10:19:40.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/img/loading-sm.gif
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)      847 2023-10-25 10:19:40.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/img/loading.gif
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3431 2021-02-15 17:42:19.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/index.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.473991 docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1082 2017-07-24 02:34:45.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/LICENSE
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4910 2017-07-24 02:34:45.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.473991 docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2192 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/jquery-labelauty.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13174 2023-12-03 21:43:22.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/jquery-labelauty.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1571 2023-12-01 23:08:09.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4639 2023-12-03 21:46:08.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.473991 docassemble.webapp-1.4.98/docassemble/webapp/static/office/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       23 2018-09-15 03:10:29.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/office/.babelrc
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1464 2018-09-14 00:24:57.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/office/cat-in-circle-32.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2799 2018-09-14 00:24:53.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/office/cat-in-circle-80.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      100 2018-09-15 12:39:38.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/office/office.css
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4280 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/office/officeinner.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   248871 2018-09-15 03:21:53.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/office/polyfill.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20178 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/office/word.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.473991 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1753 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/README.md
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13080 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click-off.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8341 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click-off.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13392 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click-on.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8322 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click-on.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     7572 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8049 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    16801 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-snap.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9961 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-snap.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13231 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-stapler.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9920 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-stapler.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2018-09-17 11:27:42.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/word.js
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.473991 docassemble.webapp-1.4.98/docassemble/webapp/static/yamlmixed/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6478 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/static/yamlmixed/yamlmixed.js
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1478 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/telnyx.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.473991 docassemble.webapp-1.4.98/docassemble/webapp/templates/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:13.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:25.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14257 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/base.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-12-23 00:30:43.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/blank.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      406 2018-06-28 11:35:30.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/flask_extra_wide_base.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      602 2020-01-03 14:53:32.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/flask_two_col_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      460 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/flask_user_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      431 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/flask_wide_base.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      487 2017-06-07 12:01:03.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/flask_wide_twocol_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6016 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/form_macros.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       41 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/page_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      230 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/page_base_half.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      283 2018-06-07 11:37:54.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/page_base_half_pgfiles.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      110 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/page_base_half_wider.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:30.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1814 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/_macros.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1674 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/change_password.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       63 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/base_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       54 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/base_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       50 2015-03-30 03:22:41.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/base_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      468 2018-05-16 10:28:37.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/confirm_email_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      369 2018-05-16 10:29:16.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/confirm_email_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      118 2018-05-16 10:29:27.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/confirm_email_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      442 2018-05-16 10:30:11.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/forgot_password_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      350 2018-05-16 10:30:33.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/forgot_password_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      114 2018-05-16 10:30:45.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/forgot_password_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      260 2016-12-05 04:58:43.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/invite_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      249 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/invite_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      110 2018-05-16 10:31:29.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/invite_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      371 2018-05-16 10:33:07.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/password_changed_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      347 2018-05-16 10:33:28.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/password_changed_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      130 2018-05-16 10:33:41.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/password_changed_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      568 2018-05-16 10:34:39.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/registered_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      464 2018-05-16 10:35:16.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/registered_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      220 2018-05-16 10:35:57.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/registered_subject.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      511 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/reregistered_message.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      424 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/reregistered_message.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      120 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/reregistered_subject.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      362 2018-05-16 10:37:44.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/username_changed_message.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      312 2018-05-16 10:38:00.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/username_changed_message.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      130 2018-05-16 10:38:13.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/username_changed_subject.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1163 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/forgot_password.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      547 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/google_login.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1000 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/invite.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10831 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/login.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1898 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/login_or_register.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1285 2020-07-28 01:34:57.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/manage_emails.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       53 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/member_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      742 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_choose.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      465 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_login.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      743 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_reconfigure.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      672 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_setup.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      440 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_sms_setup.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      445 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_verify_sms_setup.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      434 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/phone_login.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      523 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/phone_login_verify.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       53 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/public_base.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9919 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/register.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      432 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/resend_confirm_email.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1283 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/reset_password.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1039 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/user_profile.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      834 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/404.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      783 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/501.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:34.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      877 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/admin_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1670 2023-12-22 03:35:08.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/config.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      371 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/create_package.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1023 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/create_playground_package.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      642 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/gd_sync_wait.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1284 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/github.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      404 2020-07-28 01:29:18.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/google_sync.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      966 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/googledrive.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      163 2016-11-26 18:11:31.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/health_check.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1050 2020-07-28 01:28:13.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/home_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4694 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/interviews.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3112 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/logs.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      667 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/manage_account.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4396 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/manage_api.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2217 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/manage_playgrounds.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4951 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/manage_projects.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      882 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/member_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1737 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/monitor.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      640 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/od_sync_wait.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      678 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/officeaddin.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      545 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/officefunctionfile.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5637 2019-05-21 21:50:45.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/officemanifest.xml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4932 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/officeouter.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      967 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/onedrive.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      726 2018-02-25 11:28:04.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/packages.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9957 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/playground.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      198 2018-11-23 20:30:43.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/playground_poll.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9605 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/playgroundfiles.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11843 2023-12-03 19:58:23.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/playgroundpackages.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      900 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/pull_playground_package.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1428 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/rename_project.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      294 2017-10-05 03:05:06.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/restart.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      457 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/socketserver.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      425 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/start-embedded.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1191 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/start.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      579 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/test_embed.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      244 2017-05-30 00:47:01.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/testgoogledrive.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      354 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/testpost.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14703 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/train.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2567 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/update_package.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      743 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/update_package_wait.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3231 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/utilities.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      125 2017-01-19 12:40:42.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/view_source.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      939 2019-05-21 21:49:14.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/webrtc.html
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:37.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/__init__.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      669 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/add_user_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2689 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/edit_user_profile_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      474 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/new_role_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      703 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/request_developer.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      587 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/rolelist.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5712 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/user_profile_page.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4071 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/templates/users/userlist.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      182 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/testrun.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      946 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/translations.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    41744 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/update.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      486 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/update_config.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2609 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/user_database.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/docassemble/webapp/users/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2016-12-05 04:58:43.000000 docassemble.webapp-1.4.98/docassemble/webapp/users/__init__.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1079 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.98/docassemble/webapp/users/_readme.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21134 2024-02-29 11:50:31.000000 docassemble.webapp-1.4.98/docassemble/webapp/users/forms.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8053 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/users/models.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23889 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/users/views.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      429 2024-02-29 18:31:46.000000 docassemble.webapp-1.4.98/docassemble/webapp/validators.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1154 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/watchdog.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      893 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/worker.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7934 2024-01-06 21:05:56.000000 docassemble.webapp-1.4.98/docassemble/webapp/worker_common.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    84270 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/worker_tasks.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      581 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.98/docassemble/webapp/wsgi_restart.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:39:32.433990 docassemble.webapp-1.4.98/docassemble.webapp.egg-info/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      615 2024-02-29 18:39:32.000000 docassemble.webapp-1.4.98/docassemble.webapp.egg-info/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60732 2024-02-29 18:39:32.000000 docassemble.webapp-1.4.98/docassemble.webapp.egg-info/SOURCES.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2024-02-29 18:39:32.000000 docassemble.webapp-1.4.98/docassemble.webapp.egg-info/dependency_links.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2024-02-29 18:39:32.000000 docassemble.webapp-1.4.98/docassemble.webapp.egg-info/namespace_packages.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2024-02-29 18:39:32.000000 docassemble.webapp-1.4.98/docassemble.webapp.egg-info/not-zip-safe
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5219 2024-02-29 18:39:32.000000 docassemble.webapp-1.4.98/docassemble.webapp.egg-info/requires.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2024-02-29 18:39:32.000000 docassemble.webapp-1.4.98/docassemble.webapp.egg-info/top_level.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       57 2017-04-27 11:36:34.000000 docassemble.webapp-1.4.98/docassemble.wsgi
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       79 2024-02-29 18:39:32.477991 docassemble.webapp-1.4.98/setup.cfg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11104 2024-02-29 18:38:53.000000 docassemble.webapp-1.4.98/setup.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1085 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/LICENSE.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:58.000000 docassemble.webapp-1.4.99/MANIFEST.in
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      615 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.846841 docassemble.webapp-1.4.99/docassemble/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       56 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.850841 docassemble.webapp-1.4.99/docassemble/webapp/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       23 2024-03-02 13:09:31.000000 docassemble.webapp-1.4.99/docassemble/webapp/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.850841 docassemble.webapp-1.4.99/docassemble/webapp/alembic/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       38 2017-08-13 12:29:02.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/README
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2280 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/env.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      548 2018-05-13 01:00:37.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/script.py.mako
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.850841 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      538 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/025e06b85efc_package_github_branch.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4550 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/4328f2c08f05_add_indexes.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      557 2018-05-13 01:02:46.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/66f71cf543a4_temp_user_id_to_userdictkeys.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      606 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      511 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/77e8971ffcbf_first_alembic_revision.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3897 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4158 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      527 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/c2ef4831ef76_user_last_login.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1226 2018-05-16 02:31:37.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      729 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      548 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/fd1547c94c46_add_a_column_for_the_voicerss_voice.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1647 2017-08-13 12:29:02.000000 docassemble.webapp-1.4.99/docassemble/webapp/alembic.ini
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1098 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/api_key.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2172 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/app_object.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2558 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/app_socket.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    65126 2024-01-19 19:19:27.000000 docassemble.webapp-1.4.99/docassemble/webapp/backend.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      714 2023-12-11 01:54:38.000000 docassemble.webapp-1.4.99/docassemble/webapp/cleanup_sessions.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2883 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/clicksend.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      719 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/cloud.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      958 2024-02-29 17:36:07.000000 docassemble.webapp-1.4.99/docassemble/webapp/cloud_deregister.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1111 2024-02-29 17:37:00.000000 docassemble.webapp-1.4.99/docassemble/webapp/cloud_register.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      518 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/config_worker.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.850841 docassemble.webapp-1.4.99/docassemble/webapp/core/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      167 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/core/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6445 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/core/models.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15993 2023-12-11 01:53:26.000000 docassemble.webapp-1.4.99/docassemble/webapp/create_tables.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      386 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/createminio.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17573 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/cron.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1931 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/da_flask_mail.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      603 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/daredis.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.850841 docassemble.webapp-1.4.99/docassemble/webapp/data/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        7 2024-03-02 13:09:31.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/VERSION.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6913 2024-03-02 13:08:26.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/db-schema.txt
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/data/questions/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18794 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/questions/wizard-template.yml
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/data/static/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    10351 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/android-chrome-192x192.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    29787 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/android-chrome-512x512.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3030 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/apple-touch-icon.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      246 2017-04-03 03:30:52.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/browserconfig.xml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      632 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/favicon-16x16.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1400 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/favicon-32x32.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    15086 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/favicon.ico
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3752 2017-04-03 03:30:54.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/mstile-150x150.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3485 2017-04-02 22:18:46.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/safari-pinned-tab.svg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      426 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/site.webmanifest
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       26 2017-04-02 20:26:52.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/robots.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4638 2017-05-16 01:19:25.000000 docassemble.webapp-1.4.99/docassemble/webapp/data/static/test-document.docx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2568 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/database.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2018 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/db_object.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      811 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/deregister.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10218 2024-02-29 11:46:16.000000 docassemble.webapp-1.4.99/docassemble/webapp/develop.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14301 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/file_access.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      335 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/file_number.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    36419 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/files.py
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     4863 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/fix_postgresql_tables.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2492 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/fixpickle.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1954 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/google_api.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5234 2023-12-22 03:35:08.000000 docassemble.webapp-1.4.99/docassemble/webapp/info.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3985 2024-02-14 13:48:04.000000 docassemble.webapp-1.4.99/docassemble/webapp/install_certs.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3470 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/jsonstore.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1829 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/list-cloud.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2107 2023-12-21 01:20:57.000000 docassemble.webapp-1.4.99/docassemble/webapp/listlog.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      273 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/logserver.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    35526 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/machinelearning.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4537 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/mailgun_mail.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/packages/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-04-15 09:56:46.000000 docassemble.webapp-1.4.99/docassemble/webapp/packages/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2008 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/packages/models.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26073 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/playground.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7721 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/process_email.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1000 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/register.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2328 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/restart.py
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     1917 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/retrieve_js_and_css.sh
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      120 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/run.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2952 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/screenreader.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5398 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/sendgrid_mail.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1603119 2024-02-29 17:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/server.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8076 2024-03-02 13:09:31.000000 docassemble.webapp-1.4.99/docassemble/webapp/setup.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    52786 2024-01-19 19:38:36.000000 docassemble.webapp-1.4.99/docassemble/webapp/socketserver.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       97 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/socketstop.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      217 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/sockettest.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      309 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/sqlalchemy_url.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      139 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/starthook.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/static/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/static/app/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   143452 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.eot
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60774 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.json
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   347588 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.ttf
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   160576 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.woff
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   125116 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.woff2
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22174 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/additional-methods.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   170612 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/adminbundle.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31831 2023-12-06 11:50:37.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/app.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22291 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/app.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24213 2023-12-06 13:04:03.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/app.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12058 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/app.min.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      482 2018-06-05 11:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/auth0-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1229 2017-03-18 01:24:28.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/azure-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      147 2018-09-13 21:10:37.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/blank.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    45509 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/bundle.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   500762 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/bundle.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   410814 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/bundlenojquery.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   412188 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/bundlewrapjquery.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1150 2017-04-02 21:01:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/chat.ico
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1257 2015-04-04 15:28:40.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/facebook-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1387 2015-10-05 03:38:54.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/google-logo.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    89947 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/jquery.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24601 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/jquery.validate.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3407 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/jquery.visible.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2058 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/jquery.visible.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1681 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/js.cookie.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1264 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/keycloak-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      351 2016-07-05 02:35:15.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/option-vertical.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2685 2016-07-05 02:35:15.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/option-vertical.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      430 2017-06-15 10:37:03.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/phone-logo.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21977 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/playgroundbundle.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   669455 2023-12-08 16:24:50.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/playgroundbundle.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4036 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/pygments.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1930 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/pygments.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    44191 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/socket.io.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   163765 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/socket.io.min.js.map
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1539 2015-04-04 16:31:24.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/twitter-logo.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2717 2018-09-18 02:49:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/upload.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2109 2016-09-25 16:03:42.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/webrtc.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2365 2016-10-18 04:15:55.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/webrtc.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3020 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/wrap.svg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1561 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/app/zitadel-logo.png
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/static/areyousure/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11061 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/areyousure/README.md
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5559 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/areyousure/jquery.are-you-sure.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.842841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   232948 2023-12-02 01:47:15.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   589161 2023-12-02 01:47:22.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    80663 2023-12-02 01:47:47.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   331886 2023-12-02 01:47:59.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60577 2023-12-02 01:47:54.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   220350 2023-12-02 01:48:04.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2927 2017-09-24 22:47:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      881 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      765 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.min.css
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.854841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/js/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    23056 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12055 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3215 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/CODE_OF_CONDUCT.md
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     6399 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/CONTRIBUTING.md
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      105 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/FUNDING.yml
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     1443 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/ISSUE_TEMPLATE.md
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)      245 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      448 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/config.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      707 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/stale.yml
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)       67 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.gitignore
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       68 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.npmignore
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     1555 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/LICENSE.md
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    11990 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2042 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1728 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.min.css
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    12262 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.css
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     9020 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.min.css
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/img/
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)     2670 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/img/loading-sm.gif
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)      847 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/img/loading.gif
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   251909 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   125022 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5592 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/LANG.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6812 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ar.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6175 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/az.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6582 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/bg.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5996 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ca.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5884 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/cr.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6129 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/cs.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5836 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/da.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6071 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/de.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     8175 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/el.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6111 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/es.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5483 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/et.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7063 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/fa.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5227 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/fi.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6253 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/fr.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6087 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/gl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6093 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/he.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6241 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/hu.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5819 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/id.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6024 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/it.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7319 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ja.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     8967 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ka.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6230 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/kr.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6110 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/kz.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5887 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/lt.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5916 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/nl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5526 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/no.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5835 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/pl.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6137 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt-BR.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6118 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5971 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ro.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7694 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ru.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6126 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/sk.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5574 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/sl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5801 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/sr-latn.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5676 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/sv.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7300 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/th.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6129 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/tr.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     7360 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/uk.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6413 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/uz.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     6012 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/vi.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5562 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh-TW.js
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5587 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    75990 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    29919 2020-10-23 19:33:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   120577 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    42997 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.842841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     4052 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.css
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     1607 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3116 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1164 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.858841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4042 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3070 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3257 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2554 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4075 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3116 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3289 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2600 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fa/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     2024 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1782 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fas/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2074 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1834 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/gly/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     2127 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/gly/theme.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1871 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/gly/theme.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      221 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/.codeclimate.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      103 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/.npmignore
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        6 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/.nvmrc
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      774 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/.sass-lint.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      107 2017-07-06 20:05:12.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/.travis.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1207 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/LICENSE.md
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15714 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    84330 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    51588 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11286 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9935 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.min.css
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       87 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/.editorconfig
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      160 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/.gitattributes
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      169 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/.npmignore
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12802 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/AUTHORS
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   114675 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/CHANGELOG.md
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1107 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/LICENSE
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1944 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.842841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/comment/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9230 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/comment/comment.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4849 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/comment/continuecomment.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/dialog/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      507 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/dialog/dialog.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5252 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/dialog/dialog.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1546 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/autorefresh.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      116 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/fullscreen.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1497 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/fullscreen.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4661 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/panel.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2831 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/placeholder.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1918 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/rulers.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.862841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7123 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/closebrackets.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8544 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/closetag.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3989 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/continuelist.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6818 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/matchbrackets.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2358 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/matchtags.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1006 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/trailingspace.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4475 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/brace-fold.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2164 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/comment-fold.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4985 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/foldcode.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      435 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/foldgutter.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5539 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/foldgutter.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1676 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/indent-fold.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1608 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/markdown-fold.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6702 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/xml-fold.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1683 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/anyword-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2580 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/css-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11458 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/html-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6855 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/javascript-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      649 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/show-hint.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19792 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/show-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9595 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/sql-hint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5705 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/xml-hint.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1468 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/coffeescript-lint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1312 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/css-lint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1991 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/html-lint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2161 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/javascript-lint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1335 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/json-lint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3035 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/lint.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9987 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/lint.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1257 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/yaml-lint.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/merge/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3423 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/merge/merge.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38660 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/merge/merge.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2543 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/loadmode.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5191 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/multiplex.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1367 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/multiplex_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3243 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/overlay.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8076 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/simple.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1308 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/colorize.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12053 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/runmode-standalone.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2777 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/runmode.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11498 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/runmode.node.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4630 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/annotatescrollbar.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1584 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/scrollpastend.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1347 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5465 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2143 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/jump-to-line.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6216 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/match-highlighter.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      188 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3858 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11863 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/search.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12234 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/searchcursor.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/selection/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2509 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/selection/active-line.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3849 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/selection/mark-selection.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3295 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/selection/selection-pointer.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/tern/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1872 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/tern/tern.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26448 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/tern/tern.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1211 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/tern/worker.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/wrap/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6109 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/wrap/hardwrap.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/keymap/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16336 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/keymap/emacs.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26694 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/keymap/sublime.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   232203 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/keymap/vim.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/lib/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8720 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/lib/codemirror.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   401787 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/lib/codemirror.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/apl/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4739 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/apl/apl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2190 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/apl/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asciiarmor/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2449 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asciiarmor/asciiarmor.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1340 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asciiarmor/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asn.1/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7738 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asn.1/asn.1.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2275 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asn.1/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asterisk/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8142 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asterisk/asterisk.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4661 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asterisk/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/brainfuck/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2177 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/brainfuck/brainfuck.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3349 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/brainfuck/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.866841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    37259 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/clike.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10561 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28529 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/scala.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5465 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clojure/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15391 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clojure/clojure.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2738 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clojure/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18973 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clojure/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cmake/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2603 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cmake/cmake.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4163 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cmake/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cobol/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10325 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cobol/cobol.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8095 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cobol/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/coffeescript/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10038 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/coffeescript/coffeescript.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22488 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/coffeescript/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/commonlisp/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4597 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/commonlisp/commonlisp.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6702 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/commonlisp/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/crystal/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12865 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/crystal/crystal.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2616 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/crystal/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    40492 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/css.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2840 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/gss.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      463 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/gss_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2222 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4075 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/less.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1910 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/less_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2811 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/scss.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3182 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/scss_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7523 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cypher/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7130 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cypher/cypher.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1976 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cypher/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1346 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cypher/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/d/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7706 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/d/d.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6343 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/d/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      416 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/d/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dart/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5490 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dart/dart.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1638 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dart/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/diff/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1141 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/diff/diff.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4420 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/diff/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/django/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11794 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/django/django.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2072 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/django/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dockerfile/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4741 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dockerfile/dockerfile.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2262 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dockerfile/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5232 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dockerfile/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dtd/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4815 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dtd/dtd.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3332 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dtd/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dylan/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10115 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dylan/dylan.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13027 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dylan/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2741 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dylan/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ebnf/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6072 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ebnf/ebnf.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2445 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ebnf/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ecl/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8846 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ecl/ecl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1420 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ecl/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/eiffel/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3747 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/eiffel/eiffel.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13209 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/eiffel/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/elm/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5657 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/elm/elm.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1635 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/elm/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/erlang/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18876 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/erlang/erlang.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2163 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/erlang/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/factor/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3559 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/factor/factor.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2035 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/factor/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fcl/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4706 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fcl/fcl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3107 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fcl/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/forth/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5233 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/forth/forth.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1794 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/forth/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fortran/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8634 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fortran/fortran.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2487 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fortran/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gas/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9147 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gas/gas.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1851 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gas/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gfm/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5106 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gfm/gfm.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3655 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gfm/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6872 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gfm/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gherkin/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13260 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gherkin/gherkin.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1577 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gherkin/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/go/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6064 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/go/go.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2185 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/go/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/groovy/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8411 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/groovy/groovy.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2188 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/groovy/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haml/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5357 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haml/haml.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2082 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haml/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3013 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haml/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/handlebars/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2408 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/handlebars/handlebars.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2298 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/handlebars/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8167 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell/haskell.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2189 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell-literate/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1393 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell-literate/haskell-literate.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9385 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell-literate/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haxe/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17566 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haxe/haxe.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2572 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haxe/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlembedded/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1723 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlembedded/htmlembedded.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2081 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlembedded/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlmixed/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5688 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlmixed/htmlmixed.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3430 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlmixed/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/http/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2798 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/http/http.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1388 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/http/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/idl/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14893 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/idl/idl.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1686 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/idl/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8367 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4668 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38894 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/javascript.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2138 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/json-ld.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20328 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1610 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/typescript.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jinja2/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2061 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jinja2/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5907 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jinja2/jinja2.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jsx/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2405 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jsx/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5233 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jsx/jsx.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4277 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jsx/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.870841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/julia/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2428 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/julia/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11358 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/julia/julia.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/livescript/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9854 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/livescript/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7671 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/livescript/livescript.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/lua/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2087 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/lua/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6005 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/lua/lua.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28731 2022-03-06 21:30:57.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/damarkdown.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12782 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31325 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/markdown.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    38880 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mathematica/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2265 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mathematica/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5641 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mathematica/mathematica.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mbox/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1304 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mbox/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3652 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mbox/mbox.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15926 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/meta.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mirc/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5867 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mirc/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10080 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mirc/mirc.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mllike/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4679 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mllike/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8725 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mllike/mllike.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/modelica/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2018 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/modelica/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6936 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/modelica/modelica.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4321 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6917 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/mscgen.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3829 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/mscgen_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3292 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/msgenny_test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4206 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/xu_test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mumps/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2603 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mumps/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5356 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mumps/mumps.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nginx/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5256 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nginx/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10167 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nginx/nginx.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nsis/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1775 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nsis/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8107 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nsis/nsis.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ntriples/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2443 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ntriples/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7044 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ntriples/ntriples.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/octave/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1858 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/octave/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4528 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/octave/octave.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/oz/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1354 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/oz/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6663 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/oz/oz.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pascal/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1435 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pascal/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4207 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pascal/pascal.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pegjs/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1885 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pegjs/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3532 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pegjs/pegjs.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/perl/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1537 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/perl/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56084 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/perl/perl.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/php/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1995 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/php/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18339 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/php/php.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6640 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/php/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pig/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1486 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pig/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5813 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pig/pig.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/powershell/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7481 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/powershell/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12921 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/powershell/powershell.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2968 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/powershell/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/properties/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1566 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/properties/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2174 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/properties/properties.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/protobuf/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2637 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/protobuf/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2192 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/protobuf/protobuf.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pug/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2484 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pug/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15991 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pug/pug.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/puppet/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3271 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/puppet/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7575 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/puppet/puppet.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/python/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6270 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/python/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14952 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/python/python.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2850 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/python/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/q/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8956 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/q/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6596 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/q/q.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/r/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2529 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/r/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6740 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/r/r.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rpm/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rpm/changes/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2168 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rpm/changes/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4618 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rpm/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3774 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rpm/rpm.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rst/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17764 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rst/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17550 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rst/rst.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ruby/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5762 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ruby/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10703 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ruby/ruby.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      855 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ruby/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rust/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1525 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rust/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3100 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rust/rust.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      995 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rust/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sas/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1849 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sas/index.html
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    15458 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sas/sas.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sass/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1642 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sass/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11619 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sass/sass.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5141 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sass/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/scheme/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2565 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/scheme/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15266 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/scheme/scheme.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/shell/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1787 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/shell/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5383 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/shell/shell.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2377 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/shell/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sieve/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2346 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sieve/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4288 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sieve/sieve.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/slim/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2931 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/slim/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18029 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/slim/slim.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3133 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/slim/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smalltalk/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1915 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smalltalk/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4546 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smalltalk/smalltalk.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smarty/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3968 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smarty/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6843 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smarty/smarty.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.874841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/solr/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1360 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/solr/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2675 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/solr/solr.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/soy/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1934 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/soy/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23022 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/soy/soy.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12338 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/soy/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sparql/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1784 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sparql/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6901 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sparql/sparql.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/spreadsheet/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1387 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/spreadsheet/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3142 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/spreadsheet/spreadsheet.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sql/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3403 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sql/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    59293 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sql/sql.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stex/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4338 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stex/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7798 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stex/stex.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3704 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stex/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stylus/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2483 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stylus/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    42246 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stylus/stylus.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/swift/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1773 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/swift/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7527 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/swift/swift.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9428 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/swift/test.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tcl/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6308 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tcl/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4947 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tcl/tcl.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/textile/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4357 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/textile/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9442 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/textile/test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13838 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/textile/textile.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiddlywiki/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4574 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiddlywiki/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      220 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiddlywiki/tiddlywiki.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8512 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiddlywiki/tiddlywiki.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiki/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1717 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiki/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      439 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiki/tiki.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8465 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiki/tiki.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/toml/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1835 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/toml/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2900 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/toml/toml.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tornado/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1797 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tornado/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2499 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tornado/tornado.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/troff/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4476 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/troff/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2395 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/troff/troff.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3543 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10158 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn/ttcn.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn-cfg/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3658 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn-cfg/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7860 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn-cfg/ttcn-cfg.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/turtle/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1539 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/turtle/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4852 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/turtle/turtle.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/twig/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1460 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/twig/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4568 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/twig/twig.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vb/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1472 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vb/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9839 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vb/vb.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vbscript/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1512 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vbscript/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13798 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vbscript/vbscript.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/velocity/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3311 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/velocity/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7131 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/velocity/velocity.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/verilog/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2614 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/verilog/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12323 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/verilog/test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29786 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/verilog/verilog.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vhdl/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2481 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vhdl/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6707 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vhdl/vhdl.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vue/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2073 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vue/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2887 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vue/vue.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/wast/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1784 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/wast/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21987 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/wast/test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4807 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/wast/wast.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/webidl/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2159 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/webidl/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5787 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/webidl/webidl.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xml/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2166 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xml/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1761 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xml/test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13353 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xml/xml.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xquery/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8662 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xquery/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5114 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xquery/test.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15755 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xquery/xquery.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yacas/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2187 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yacas/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5429 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yacas/yacas.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2109 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3735 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml/yaml.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.878841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3083 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2509 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.882841 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/z80/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1401 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/z80/index.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3580 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/z80/z80.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.886842 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1987 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/3024-day.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2076 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/3024-night.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7702 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/abbott.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1969 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/abcdef.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      103 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ambiance-mobile.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26493 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ambiance.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2421 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ayu-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2538 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ayu-mirage.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2292 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/base16-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2124 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/base16-light.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1413 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/bespin.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1931 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/blackboard.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1726 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/cobalt.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1677 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/colorforth.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2686 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/darcula.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2042 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/dracula.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2614 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/duotone-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2719 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/duotone-light.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1187 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/eclipse.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      781 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/elegant.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2286 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/erlang-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1918 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/gruvbox-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1469 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/hopscotch.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2515 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/icecoder.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1672 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/idea.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1442 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/isotope.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      517 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/juejin.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2637 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/lesser-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3991 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/liquibyte.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1914 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/lucario.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2607 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/material-darker.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2767 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/material-ocean.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2923 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/material-palenight.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2533 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/material.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2112 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/mbo.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5196 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/mdn-like.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1856 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/midnight.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2179 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/monokai.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2369 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/moxer.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      688 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/neat.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      947 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/neo.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1746 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/night.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2088 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/nord.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2440 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/oceanic-next.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1804 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/panda-syntax.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2078 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/paraiso-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2078 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/paraiso-light.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2485 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/pastel-on-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1514 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/railscasts.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1801 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/rubyblue.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2009 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/seti.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2440 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/shadowfox.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5337 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/solarized.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      751 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ssms.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1940 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/the-matrix.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1769 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/tomorrow-night-bright.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2439 2023-02-04 19:25:58.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/tomorrow-night-eighties.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2440 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ttcn.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2164 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/twilight.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2142 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/vibrant-ink.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3033 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/xq-dark.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2255 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/xq-light.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1884 2023-10-25 10:19:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/yeti.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3075 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/yonce.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2001 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/zenburn.css
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.894842 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17268 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/actions-parameters.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12998 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/actions.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11717 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/age_in_years.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56854 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/alignment.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21522 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/all-true.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    50677 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/allow-emailing-false.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4389 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/as-datetime.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   135261 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/attachment-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13634 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/audio.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19808 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/auto-terms.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11382 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action_flash.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11382 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action_javascript.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action_refresh.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action_with_response_action.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11359 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_response_action_flash.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10740 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/buttons-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21691 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/buttons-icons.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12060 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/buttons-labels.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13126 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/buttons.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6047 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/capitalize.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4394 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/chat-partners-available.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12769 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/check-in.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11099 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices-combobox.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13705 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices-dropdown.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22972 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices-icons.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19684 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices-with-default.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19893 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10569 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7383 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/comment.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10803 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/continue-button-label.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14401 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/continue.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11638 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/country.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26548 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/cron.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    43642 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/css.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5623 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/currency.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5285 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/current-datetime.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16116 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/dadict.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3988 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/dafile.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11814 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/database_storage.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11803 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/date-difference.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12966 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/date-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4232 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/date-interval.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9474 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/date-parts.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5541 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/dead-end.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13778 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/decoration.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9069 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/def.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11281 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/defined.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8039 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/del.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4006 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/device.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11725 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/dialog-box.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    55811 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document-docx.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58370 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document-file.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60880 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document-language.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    67827 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document-variable-name.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    56752 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34388 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/docx-template-table.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34757 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/docx-template.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14541 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/doors.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10627 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/email-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18631 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/email-to-case-simple.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18631 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/email-to-case.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18838 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/emoji-inline.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11709 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exists.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7103 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exit-buttons.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10180 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exit-choices.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12116 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exit-url.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9401 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exit.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8708 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/external_files.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25112 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-checkboxes.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12060 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-choices-combobox.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11548 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-choices.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16234 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-mc-exclude.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16234 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-mc.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23154 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-noyesmaybe.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24536 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-yesno.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21736 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-yesnomaybe.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24516 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-yesnoradio.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19513 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-yesnowide.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21231 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fix-punctuation.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4717 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/for_fruit.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8039 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/force-ask.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8259 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/force-gather.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32606 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/formatting.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9089 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-dict-object.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17024 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-dict-value.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13811 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-dict.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9218 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-fruit-at-least-two.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11776 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-fruit-gather.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11099 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-fruit-number.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14113 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-fruit.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14906 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-set-object.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10364 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-set.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8716 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/generic-object.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4433 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/get-default-timezone.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16575 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/help-damages-audio.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23318 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/help.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20326 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/hideif-boolean.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    29068 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/html.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15386 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/image-sets.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14948 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/images.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9555 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/imports.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/include.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15384 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/indefinite-article.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14115 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/initial.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3633 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/interface.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17183 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/interview-help.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20436 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/interview-url.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21938 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/interview_url_action.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3505 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/js_action_call.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11157 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/js_url_action.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2337 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/js_variables.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15459 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/label.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14870 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/language.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8437 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/language_from_browser.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4335 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/language_from_browser_restricted.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3704 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/lists.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25876 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/loading-legal.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23906 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/loading-util.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7878 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/madlibs.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3546 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-01.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3118 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-02.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6352 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-03.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6352 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-04.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3292 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-05.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9163 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-06.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2462 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-07.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6832 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-09.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10569 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mandatory.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    67776 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/markdown.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10310 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/menu-item.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10655 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/message.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15962 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/metadata.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16028 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/min.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11344 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/minlength.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9444 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-classify.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9181 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-datatype.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18348 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-export-yaml.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      354 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-export.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6828 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-predict.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6828 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-save-and-predict.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9658 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mlarea-datatype.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11104 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/modules.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11685 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/money-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9787 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/need.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14471 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/nested-loop.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12230 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/nice-number.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10407 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/no-label-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    27436 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/note.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12595 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/noun-plural.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11084 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/noyes.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14737 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/number-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16214 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object-checkboxes.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14699 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object-disable-others.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13219 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object-radio.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10235 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object-selections.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10453 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17062 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/objects.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22843 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ocr-chord.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20326 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ocr.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23012 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/optional-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8274 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ordinal-number.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12679 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/other.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58333 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/page-numbers.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16253 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/password-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9496 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/past-tense.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    51015 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pdf-a.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19862 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pdf-fill-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12171 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pdf-fill-signature.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24929 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pdf-fill.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12918 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/periodic-amount.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11325 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/periodic-value.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19272 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/prevent-back.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19272 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/prevent-going-back.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9509 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/progress-features.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9795 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/progress.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18786 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pull-down-with-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15669 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pull-down.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20531 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/qr-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2952 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/quantity-noun.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13474 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/quote_paragraphs.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    27426 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/radio-list.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21419 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/range.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11560 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/reconsider.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22042 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/redis.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8298 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/refresh.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10247 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/reload.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7496 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/required-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11560 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/reset.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10798 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/response-json.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7484 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/response-svg.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      825 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/response.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22273 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/resume-button-label.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    45696 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/review.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23999 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/salutation.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24041 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/save-url-to-file.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9746 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/script.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20961 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords-code.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28927 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords-get-sections.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22015 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords-review.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22106 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords-set-sections.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22800 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    28276 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9226 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/send-email.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14870 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/set-language.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    15954 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/showif-boolean.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    16875 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/showif.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    34936 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/shuffle.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    22291 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/signature.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5202 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/signin.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    58915 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/single-spacing.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5901 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/space-underscore.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10375 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/state.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18965 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/static_image.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10109 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/subdivision-type.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7290 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/table-mako.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6771 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/table-markdown.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7124 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/table.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    12382 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/target-template.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32422 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/template-file.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    37584 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/template-subject.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32422 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/template.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    19527 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/terms.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10820 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-box-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20969 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-default.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18283 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-field.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25945 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-help.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23948 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-hint.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13398 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/timezone-list.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5432 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/title-case.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4107 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/today.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    26745 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/under.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25496 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/upload-multiple.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24708 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/upload.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    17380 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/url-of.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    41705 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/valid-formats.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11304 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/value.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10271 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/variables_as_json.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   245391 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/video.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8585 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/yesno-custom.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11084 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/yesno.png
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11702 2023-12-06 11:43:48.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/examples/yesnomaybe.png
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.846841 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.898842 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1627443 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/all.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)  1597188 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/all.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   477868 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/brands.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   477004 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/brands.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    39338 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/conflict-detection.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    24798 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/conflict-detection.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   121752 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/fontawesome.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    88423 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/fontawesome.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   152666 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/regular.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   150749 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/regular.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   875814 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/solid.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   881669 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/solid.min.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    33609 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/v4-shims.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    32952 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/v4-shims.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.898842 docassemble.webapp-1.4.99/docassemble/webapp/static/img/
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     2670 2023-10-25 10:19:40.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/img/loading-sm.gif
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)      847 2023-10-25 10:19:40.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/img/loading.gif
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3431 2021-02-15 17:42:19.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/index.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.898842 docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1082 2017-07-24 02:34:45.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/LICENSE
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4910 2017-07-24 02:34:45.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.898842 docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2192 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/jquery-labelauty.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    13174 2023-12-03 21:43:22.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/jquery-labelauty.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1571 2023-12-01 23:08:09.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4639 2023-12-03 21:46:08.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.898842 docassemble.webapp-1.4.99/docassemble/webapp/static/office/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       23 2018-09-15 03:10:29.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/office/.babelrc
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1464 2018-09-14 00:24:57.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/office/cat-in-circle-32.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2799 2018-09-14 00:24:53.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/office/cat-in-circle-80.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      100 2018-09-15 12:39:38.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/office/office.css
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4280 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/office/officeinner.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   248871 2018-09-15 03:21:53.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/office/polyfill.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    20178 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/office/word.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.898842 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1753 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/README.md
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13080 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click-off.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8341 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click-off.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13392 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click-on.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8322 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click-on.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     7572 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8049 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    16801 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-snap.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9961 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-snap.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13231 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-stapler.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9920 2016-10-29 17:44:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-stapler.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2018-09-17 11:27:42.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/word.js
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/docassemble/webapp/static/yamlmixed/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6478 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/static/yamlmixed/yamlmixed.js
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1478 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/telnyx.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/docassemble/webapp/templates/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:13.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:25.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14257 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/base.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-12-23 00:30:43.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/blank.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      406 2018-06-28 11:35:30.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/flask_extra_wide_base.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      602 2020-01-03 14:53:32.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/flask_two_col_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      460 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/flask_user_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      431 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/flask_wide_base.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      487 2017-06-07 12:01:03.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/flask_wide_twocol_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6016 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/form_macros.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       41 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/page_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      230 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/page_base_half.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      283 2018-06-07 11:37:54.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/page_base_half_pgfiles.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      110 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/page_base_half_wider.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:30.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1814 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/_macros.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1674 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/change_password.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       63 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/base_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       54 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/base_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       50 2015-03-30 03:22:41.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/base_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      468 2018-05-16 10:28:37.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/confirm_email_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      369 2018-05-16 10:29:16.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/confirm_email_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      118 2018-05-16 10:29:27.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/confirm_email_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      442 2018-05-16 10:30:11.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/forgot_password_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      350 2018-05-16 10:30:33.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/forgot_password_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      114 2018-05-16 10:30:45.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/forgot_password_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      260 2016-12-05 04:58:43.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/invite_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      249 2016-12-01 22:24:19.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/invite_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      110 2018-05-16 10:31:29.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/invite_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      371 2018-05-16 10:33:07.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/password_changed_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      347 2018-05-16 10:33:28.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/password_changed_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      130 2018-05-16 10:33:41.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/password_changed_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      568 2018-05-16 10:34:39.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/registered_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      464 2018-05-16 10:35:16.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/registered_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      220 2018-05-16 10:35:57.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/registered_subject.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      511 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/reregistered_message.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      424 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/reregistered_message.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      120 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/reregistered_subject.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      362 2018-05-16 10:37:44.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/username_changed_message.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      312 2018-05-16 10:38:00.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/username_changed_message.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      130 2018-05-16 10:38:13.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/username_changed_subject.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1163 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/forgot_password.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      547 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/google_login.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1000 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/invite.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    10831 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/login.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1898 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/login_or_register.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1285 2020-07-28 01:34:57.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/manage_emails.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       53 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/member_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      742 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_choose.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      465 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_login.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      743 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_reconfigure.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      672 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_setup.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      440 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_sms_setup.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      445 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_verify_sms_setup.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      434 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/phone_login.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      523 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/phone_login_verify.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       53 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/public_base.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9919 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/register.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      432 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/resend_confirm_email.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1283 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/reset_password.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1039 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/user_profile.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      834 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/404.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      783 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/501.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:34.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      877 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/admin_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1670 2023-12-22 03:35:08.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/config.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      371 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/create_package.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1023 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/create_playground_package.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      642 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/gd_sync_wait.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1284 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/github.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      404 2020-07-28 01:29:18.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/google_sync.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      966 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/googledrive.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      163 2016-11-26 18:11:31.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/health_check.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1050 2020-07-28 01:28:13.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/home_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4694 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/interviews.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3112 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/logs.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      667 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/manage_account.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4396 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/manage_api.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2217 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/manage_playgrounds.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4951 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/manage_projects.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      882 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/member_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1737 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/monitor.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      640 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/od_sync_wait.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      678 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/officeaddin.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      545 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/officefunctionfile.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5637 2019-05-21 21:50:45.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/officemanifest.xml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4932 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/officeouter.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      967 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/onedrive.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      726 2018-02-25 11:28:04.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/packages.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9957 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/playground.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      198 2018-11-23 20:30:43.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/playground_poll.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9605 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/playgroundfiles.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11843 2023-12-03 19:58:23.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/playgroundpackages.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      900 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/pull_playground_package.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1428 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/rename_project.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      294 2017-10-05 03:05:06.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/restart.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      457 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/socketserver.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      425 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/start-embedded.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1191 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/start.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      579 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/test_embed.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      244 2017-05-30 00:47:01.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/testgoogledrive.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      354 2018-04-28 22:15:04.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/testpost.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14703 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/train.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2567 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/update_package.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      743 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/update_package_wait.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3231 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/utilities.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      125 2017-01-19 12:40:42.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/view_source.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      939 2019-05-21 21:49:14.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/webrtc.html
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2015-03-29 18:58:37.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/__init__.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      669 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/add_user_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2689 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/edit_user_profile_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      474 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/new_role_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      703 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/request_developer.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      587 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/rolelist.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5712 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/user_profile_page.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4071 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/templates/users/userlist.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      182 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/testrun.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      946 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/translations.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    41744 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/update.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      486 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/update_config.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2609 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/user_database.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.902842 docassemble.webapp-1.4.99/docassemble/webapp/users/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)        0 2016-12-05 04:58:43.000000 docassemble.webapp-1.4.99/docassemble/webapp/users/__init__.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1079 2015-03-29 18:16:59.000000 docassemble.webapp-1.4.99/docassemble/webapp/users/_readme.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    21134 2024-02-29 11:50:31.000000 docassemble.webapp-1.4.99/docassemble/webapp/users/forms.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     8053 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/users/models.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23889 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/users/views.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      429 2024-02-29 18:31:46.000000 docassemble.webapp-1.4.99/docassemble/webapp/validators.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1154 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/watchdog.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      893 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/worker.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7934 2024-01-06 21:05:56.000000 docassemble.webapp-1.4.99/docassemble/webapp/worker_common.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    84270 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/worker_tasks.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      581 2023-11-27 02:50:05.000000 docassemble.webapp-1.4.99/docassemble/webapp/wsgi_restart.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:55.846841 docassemble.webapp-1.4.99/docassemble.webapp.egg-info/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      615 2024-03-02 13:09:55.000000 docassemble.webapp-1.4.99/docassemble.webapp.egg-info/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    60732 2024-03-02 13:09:55.000000 docassemble.webapp-1.4.99/docassemble.webapp.egg-info/SOURCES.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2024-03-02 13:09:55.000000 docassemble.webapp-1.4.99/docassemble.webapp.egg-info/dependency_links.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2024-03-02 13:09:55.000000 docassemble.webapp-1.4.99/docassemble.webapp.egg-info/namespace_packages.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2024-03-02 13:09:55.000000 docassemble.webapp-1.4.99/docassemble.webapp.egg-info/not-zip-safe
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5222 2024-03-02 13:09:55.000000 docassemble.webapp-1.4.99/docassemble.webapp.egg-info/requires.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2024-03-02 13:09:55.000000 docassemble.webapp-1.4.99/docassemble.webapp.egg-info/top_level.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       57 2017-04-27 11:36:34.000000 docassemble.webapp-1.4.99/docassemble.wsgi
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       79 2024-03-02 13:09:55.906842 docassemble.webapp-1.4.99/setup.cfg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    11107 2024-03-02 13:09:31.000000 docassemble.webapp-1.4.99/setup.py
```

### Comparing `docassemble.webapp-1.4.98/LICENSE.txt` & `docassemble.webapp-1.4.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/PKG-INFO` & `docassemble.webapp-1.4.99/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.webapp
-Version: 1.4.98
+Version: 1.4.99
 Summary: The web application components of the docassemble system.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/env.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/env.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/script.py.mako` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/025e06b85efc_package_github_branch.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/025e06b85efc_package_github_branch.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/4328f2c08f05_add_indexes.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/4328f2c08f05_add_indexes.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/66f71cf543a4_temp_user_id_to_userdictkeys.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/66f71cf543a4_temp_user_id_to_userdictkeys.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/693d02299f38_fix_indexes.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/9be372ec38bc_alter_database_for_mysql_compatibility.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/a8746ddab8cb_add_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/c2ef4831ef76_user_last_login.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/c2ef4831ef76_user_last_login.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/eb61567ea005_length_of_subdivisionfirst.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/f0b00081fda9_uploads_persistent_global.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic/versions/fd1547c94c46_add_a_column_for_the_voicerss_voice.py` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic/versions/fd1547c94c46_add_a_column_for_the_voicerss_voice.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/alembic.ini` & `docassemble.webapp-1.4.99/docassemble/webapp/alembic.ini`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/api_key.py` & `docassemble.webapp-1.4.99/docassemble/webapp/api_key.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/app_object.py` & `docassemble.webapp-1.4.99/docassemble/webapp/app_object.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/app_socket.py` & `docassemble.webapp-1.4.99/docassemble/webapp/app_socket.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/backend.py` & `docassemble.webapp-1.4.99/docassemble/webapp/backend.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/cleanup_sessions.py` & `docassemble.webapp-1.4.99/docassemble/webapp/cleanup_sessions.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/clicksend.py` & `docassemble.webapp-1.4.99/docassemble/webapp/clicksend.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/cloud.py` & `docassemble.webapp-1.4.99/docassemble/webapp/cloud.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/cloud_deregister.py` & `docassemble.webapp-1.4.99/docassemble/webapp/cloud_deregister.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/cloud_register.py` & `docassemble.webapp-1.4.99/docassemble/webapp/cloud_register.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/config_worker.py` & `docassemble.webapp-1.4.99/docassemble/webapp/config_worker.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/core/models.py` & `docassemble.webapp-1.4.99/docassemble/webapp/core/models.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/create_tables.py` & `docassemble.webapp-1.4.99/docassemble/webapp/create_tables.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/cron.py` & `docassemble.webapp-1.4.99/docassemble/webapp/cron.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/da_flask_mail.py` & `docassemble.webapp-1.4.99/docassemble/webapp/da_flask_mail.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/daredis.py` & `docassemble.webapp-1.4.99/docassemble/webapp/daredis.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/db-schema.txt` & `docassemble.webapp-1.4.99/docassemble/webapp/data/db-schema.txt`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/questions/wizard-template.yml` & `docassemble.webapp-1.4.99/docassemble/webapp/data/questions/wizard-template.yml`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/android-chrome-192x192.png` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/android-chrome-512x512.png` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/apple-touch-icon.png` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/favicon-16x16.png` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/favicon-32x32.png` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/favicon.ico` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/mstile-150x150.png` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/favicon/safari-pinned-tab.svg` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/data/static/test-document.docx` & `docassemble.webapp-1.4.99/docassemble/webapp/data/static/test-document.docx`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/database.py` & `docassemble.webapp-1.4.99/docassemble/webapp/database.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/db_object.py` & `docassemble.webapp-1.4.99/docassemble/webapp/db_object.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/deregister.py` & `docassemble.webapp-1.4.99/docassemble/webapp/deregister.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/develop.py` & `docassemble.webapp-1.4.99/docassemble/webapp/develop.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/file_access.py` & `docassemble.webapp-1.4.99/docassemble/webapp/file_access.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/files.py` & `docassemble.webapp-1.4.99/docassemble/webapp/files.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/fix_postgresql_tables.py` & `docassemble.webapp-1.4.99/docassemble/webapp/fix_postgresql_tables.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/fixpickle.py` & `docassemble.webapp-1.4.99/docassemble/webapp/fixpickle.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/google_api.py` & `docassemble.webapp-1.4.99/docassemble/webapp/google_api.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/info.py` & `docassemble.webapp-1.4.99/docassemble/webapp/info.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/install_certs.py` & `docassemble.webapp-1.4.99/docassemble/webapp/install_certs.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/jsonstore.py` & `docassemble.webapp-1.4.99/docassemble/webapp/jsonstore.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/list-cloud.py` & `docassemble.webapp-1.4.99/docassemble/webapp/list-cloud.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/listlog.py` & `docassemble.webapp-1.4.99/docassemble/webapp/listlog.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/machinelearning.py` & `docassemble.webapp-1.4.99/docassemble/webapp/machinelearning.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/mailgun_mail.py` & `docassemble.webapp-1.4.99/docassemble/webapp/mailgun_mail.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/packages/models.py` & `docassemble.webapp-1.4.99/docassemble/webapp/packages/models.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/playground.py` & `docassemble.webapp-1.4.99/docassemble/webapp/playground.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/process_email.py` & `docassemble.webapp-1.4.99/docassemble/webapp/process_email.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/register.py` & `docassemble.webapp-1.4.99/docassemble/webapp/register.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/restart.py` & `docassemble.webapp-1.4.99/docassemble/webapp/restart.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/retrieve_js_and_css.sh` & `docassemble.webapp-1.4.99/docassemble/webapp/retrieve_js_and_css.sh`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/screenreader.py` & `docassemble.webapp-1.4.99/docassemble/webapp/screenreader.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/sendgrid_mail.py` & `docassemble.webapp-1.4.99/docassemble/webapp/sendgrid_mail.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/server.py` & `docassemble.webapp-1.4.99/docassemble/webapp/server.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/setup.py` & `docassemble.webapp-1.4.99/docassemble/webapp/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import timedelta
 import re
 import importlib
 from docassemble.webapp.app_object import app
 from docassemble.base.config import daconfig
 import docassemble.webapp.database
-da_version = '1.4.98'
+da_version = '1.4.99'
 app.config['DA_VERSION'] = da_version
 app.config['APP_NAME'] = daconfig.get('appname', 'docassemble')
 app.config['BRAND_NAME'] = daconfig.get('brandname', daconfig.get('appname', 'docassemble'))
 app.config['SHOW_PROFILE'] = bool(daconfig.get('show profile link', True))
 app.config['SHOW_MY_INTERVIEWS'] = bool(daconfig.get('show interviews link', True))
 app.config['SHOW_DISPATCH'] = bool(len(daconfig['dispatch']) and daconfig.get('show dispatch link', False) > 0)
 # app.config['ADMINS'] = [daconfig.get('admin address', None)]
```

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/socketserver.py` & `docassemble.webapp-1.4.99/docassemble/webapp/socketserver.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.eot` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.eot`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.json` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.json`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.ttf` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.woff` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/MaterialIcons-Regular.woff2` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/additional-methods.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/additional-methods.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/adminbundle.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/adminbundle.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/app.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/app.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/app.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/app.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/app.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/app.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/app.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/app.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/azure-logo.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/azure-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/bundle.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/bundle.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/bundle.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/bundle.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/bundlenojquery.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/bundlenojquery.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/bundlewrapjquery.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/bundlewrapjquery.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/chat.ico` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/chat.ico`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/facebook-logo.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/facebook-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/google-logo.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/google-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/jquery.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/jquery.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/jquery.validate.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/jquery.validate.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/jquery.visible.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/jquery.visible.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/jquery.visible.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/jquery.visible.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/js.cookie.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/keycloak-logo.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/keycloak-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/option-vertical.svg` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/option-vertical.svg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/playgroundbundle.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/playgroundbundle.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/playgroundbundle.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/playgroundbundle.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/pygments.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/pygments.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/pygments.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/pygments.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/socket.io.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/socket.io.min.js.map` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/socket.io.min.js.map`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/twitter-logo.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/twitter-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/upload.svg` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/upload.svg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/webrtc.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/webrtc.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/webrtc.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/webrtc.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/wrap.svg` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/wrap.svg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/app/zitadel-logo.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/app/zitadel-logo.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/areyousure/README.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/areyousure/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/areyousure/jquery.are-you-sure.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/areyousure/jquery.are-you-sure.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/css/bootstrap.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/css/bootstrap.min.css.map` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js.map` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/bootstrap.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap/js/bootstrap.min.js.map` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/README.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/css/bootstrap-combobox.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-combobox/js/bootstrap-combobox.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/CODE_OF_CONDUCT.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/CONTRIBUTING.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/ISSUE_TEMPLATE.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/.github/stale.yml` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/LICENSE.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/README.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/fileinput-rtl.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/css/fileinput.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/img/loading-sm.gif` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/img/loading-sm.gif`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/img/loading.gif` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/img/loading.gif`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/fileinput.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/LANG.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/LANG.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ar.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ar.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/az.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/az.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/bg.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/bg.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ca.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ca.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/cr.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/cr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/cs.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/cs.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/da.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/da.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/de.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/de.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/el.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/el.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/es.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/es.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/et.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/et.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/fa.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/fa.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/fi.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/fi.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/fr.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/fr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/gl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/gl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/he.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/he.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/hu.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/hu.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/id.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/id.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/it.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/it.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ja.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ja.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ka.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ka.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/kr.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/kr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/kz.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/kz.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/lt.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/lt.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/nl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/nl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/no.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/no.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/pl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/pl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt-BR.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt-BR.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/pt.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ro.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ro.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/ru.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/ru.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/sk.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/sk.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/sl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/sl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/sr-latn.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/sr-latn.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/sv.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/sv.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/th.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/th.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/tr.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/tr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/uk.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/uk.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/uz.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/uz.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/vi.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/vi.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh-TW.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh-TW.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/locales/zh.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/piexif.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/js/plugins/sortable.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer/theme.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fa/theme.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/explorer-fas/theme.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fa/theme.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/fas/theme.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/gly/theme.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/gly/theme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-fileinput/themes/gly/theme.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-fileinput/themes/gly/theme.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/.sass-lint.yml` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/.sass-lint.yml`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/LICENSE.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/README.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/bootstrap-slider.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/bootstrap-slider/dist/css/bootstrap-slider.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/AUTHORS` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/AUTHORS`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/CHANGELOG.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/LICENSE` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/README.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/comment/comment.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/comment/comment.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/comment/continuecomment.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/comment/continuecomment.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/dialog/dialog.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/dialog/dialog.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/autorefresh.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/autorefresh.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/fullscreen.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/fullscreen.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/panel.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/panel.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/placeholder.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/placeholder.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/display/rulers.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/display/rulers.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/closebrackets.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/closebrackets.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/closetag.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/closetag.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/continuelist.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/continuelist.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/matchbrackets.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/matchtags.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/matchtags.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/edit/trailingspace.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/edit/trailingspace.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/brace-fold.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/brace-fold.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/comment-fold.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/comment-fold.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/foldcode.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/foldcode.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/foldgutter.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/foldgutter.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/indent-fold.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/indent-fold.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/markdown-fold.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/markdown-fold.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/fold/xml-fold.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/fold/xml-fold.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/anyword-hint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/anyword-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/css-hint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/css-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/html-hint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/html-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/javascript-hint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/javascript-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/show-hint.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/show-hint.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/show-hint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/show-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/sql-hint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/sql-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/hint/xml-hint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/hint/xml-hint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/coffeescript-lint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/coffeescript-lint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/css-lint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/css-lint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/html-lint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/html-lint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/javascript-lint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/javascript-lint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/json-lint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/json-lint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/lint.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/lint.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/lint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/lint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/lint/yaml-lint.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/lint/yaml-lint.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/merge/merge.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/merge/merge.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/merge/merge.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/merge/merge.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/loadmode.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/loadmode.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/multiplex.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/multiplex.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/multiplex_test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/multiplex_test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/overlay.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/overlay.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/mode/simple.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/mode/simple.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/colorize.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/colorize.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/runmode-standalone.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/runmode-standalone.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/runmode.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/runmode.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/runmode/runmode.node.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/runmode/runmode.node.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/annotatescrollbar.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/annotatescrollbar.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/scrollpastend.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/scrollpastend.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/scroll/simplescrollbars.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/jump-to-line.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/jump-to-line.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/match-highlighter.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/match-highlighter.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/matchesonscrollbar.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/search.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/search.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/search/searchcursor.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/search/searchcursor.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/selection/active-line.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/selection/active-line.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/selection/mark-selection.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/selection/mark-selection.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/selection/selection-pointer.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/selection/selection-pointer.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/tern/tern.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/tern/tern.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/tern/tern.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/tern/tern.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/tern/worker.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/tern/worker.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/addon/wrap/hardwrap.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/addon/wrap/hardwrap.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/keymap/emacs.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/keymap/emacs.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/keymap/sublime.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/keymap/sublime.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/keymap/vim.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/keymap/vim.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/lib/codemirror.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/lib/codemirror.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/lib/codemirror.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/lib/codemirror.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/apl/apl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/apl/apl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/apl/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/apl/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asciiarmor/asciiarmor.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asciiarmor/asciiarmor.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asciiarmor/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asciiarmor/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asn.1/asn.1.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asn.1/asn.1.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asn.1/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asn.1/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asterisk/asterisk.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asterisk/asterisk.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/asterisk/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/asterisk/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/brainfuck/brainfuck.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/brainfuck/brainfuck.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/brainfuck/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/brainfuck/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/clike.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/clike.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/scala.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/scala.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clike/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clike/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clojure/clojure.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clojure/clojure.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clojure/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clojure/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/clojure/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/clojure/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cmake/cmake.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cmake/cmake.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cmake/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cmake/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cobol/cobol.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cobol/cobol.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cobol/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cobol/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/coffeescript/coffeescript.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/coffeescript/coffeescript.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/coffeescript/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/coffeescript/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/commonlisp/commonlisp.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/commonlisp/commonlisp.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/commonlisp/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/commonlisp/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/crystal/crystal.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/crystal/crystal.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/crystal/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/crystal/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/css.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/css.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/gss.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/gss.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/less.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/less.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/less_test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/less_test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/scss.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/scss.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/scss_test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/scss_test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/css/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/css/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cypher/cypher.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cypher/cypher.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cypher/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cypher/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/cypher/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/cypher/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/d/d.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/d/d.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/d/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/d/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dart/dart.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dart/dart.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dart/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dart/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/diff/diff.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/diff/diff.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/diff/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/diff/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/django/django.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/django/django.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/django/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/django/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dockerfile/dockerfile.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dockerfile/dockerfile.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dockerfile/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dockerfile/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dockerfile/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dockerfile/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dtd/dtd.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dtd/dtd.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dtd/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dtd/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dylan/dylan.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dylan/dylan.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dylan/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dylan/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/dylan/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/dylan/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ebnf/ebnf.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ebnf/ebnf.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ebnf/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ebnf/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ecl/ecl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ecl/ecl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ecl/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ecl/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/eiffel/eiffel.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/eiffel/eiffel.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/eiffel/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/eiffel/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/elm/elm.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/elm/elm.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/elm/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/elm/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/erlang/erlang.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/erlang/erlang.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/erlang/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/erlang/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/factor/factor.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/factor/factor.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/factor/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/factor/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fcl/fcl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fcl/fcl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fcl/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fcl/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/forth/forth.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/forth/forth.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/forth/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/forth/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fortran/fortran.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fortran/fortran.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/fortran/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/fortran/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gas/gas.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gas/gas.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gas/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gas/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gfm/gfm.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gfm/gfm.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gfm/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gfm/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gfm/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gfm/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gherkin/gherkin.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gherkin/gherkin.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/gherkin/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/gherkin/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/go/go.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/go/go.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/go/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/go/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/groovy/groovy.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/groovy/groovy.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/groovy/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/groovy/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haml/haml.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haml/haml.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haml/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haml/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haml/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haml/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/handlebars/handlebars.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/handlebars/handlebars.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/handlebars/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/handlebars/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell/haskell.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell/haskell.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell-literate/haskell-literate.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell-literate/haskell-literate.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haskell-literate/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haskell-literate/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haxe/haxe.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haxe/haxe.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/haxe/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/haxe/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlembedded/htmlembedded.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlembedded/htmlembedded.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlembedded/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlembedded/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlmixed/htmlmixed.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlmixed/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/htmlmixed/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/htmlmixed/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/http/http.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/http/http.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/http/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/http/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/idl/idl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/idl/idl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/idl/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/idl/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/javascript.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/javascript.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/json-ld.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/json-ld.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/javascript/typescript.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/javascript/typescript.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jinja2/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jinja2/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jinja2/jinja2.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jinja2/jinja2.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jsx/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jsx/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jsx/jsx.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jsx/jsx.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/jsx/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/jsx/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/julia/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/julia/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/julia/julia.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/julia/julia.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/livescript/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/livescript/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/livescript/livescript.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/livescript/livescript.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/lua/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/lua/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/lua/lua.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/lua/lua.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/damarkdown.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/damarkdown.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/markdown.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/markdown.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/markdown/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/markdown/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mathematica/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mathematica/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mathematica/mathematica.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mathematica/mathematica.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mbox/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mbox/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mbox/mbox.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mbox/mbox.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/meta.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/meta.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mirc/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mirc/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mirc/mirc.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mirc/mirc.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mllike/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mllike/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mllike/mllike.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mllike/mllike.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/modelica/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/modelica/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/modelica/modelica.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/modelica/modelica.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/mscgen.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/mscgen.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/mscgen_test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/mscgen_test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/msgenny_test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/msgenny_test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mscgen/xu_test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mscgen/xu_test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mumps/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mumps/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/mumps/mumps.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/mumps/mumps.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nginx/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nginx/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nginx/nginx.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nginx/nginx.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nsis/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nsis/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/nsis/nsis.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/nsis/nsis.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ntriples/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ntriples/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ntriples/ntriples.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ntriples/ntriples.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/octave/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/octave/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/octave/octave.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/octave/octave.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/oz/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/oz/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/oz/oz.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/oz/oz.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pascal/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pascal/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pascal/pascal.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pascal/pascal.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pegjs/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pegjs/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pegjs/pegjs.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pegjs/pegjs.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/perl/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/perl/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/perl/perl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/perl/perl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/php/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/php/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/php/php.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/php/php.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/php/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/php/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pig/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pig/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pig/pig.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pig/pig.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/powershell/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/powershell/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/powershell/powershell.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/powershell/powershell.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/powershell/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/powershell/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/properties/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/properties/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/properties/properties.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/properties/properties.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/protobuf/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/protobuf/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/protobuf/protobuf.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/protobuf/protobuf.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pug/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pug/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/pug/pug.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/pug/pug.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/puppet/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/puppet/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/puppet/puppet.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/puppet/puppet.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/python/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/python/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/python/python.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/python/python.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/python/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/python/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/q/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/q/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/q/q.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/q/q.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/r/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/r/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/r/r.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/r/r.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rpm/changes/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rpm/changes/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rpm/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rpm/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rpm/rpm.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rpm/rpm.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rst/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rst/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rst/rst.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rst/rst.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ruby/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ruby/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ruby/ruby.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ruby/ruby.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ruby/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ruby/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rust/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rust/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rust/rust.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rust/rust.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/rust/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/rust/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sas/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sas/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sas/sas.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sas/sas.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sass/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sass/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sass/sass.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sass/sass.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sass/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sass/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/scheme/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/scheme/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/scheme/scheme.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/scheme/scheme.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/shell/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/shell/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/shell/shell.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/shell/shell.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/shell/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/shell/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sieve/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sieve/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sieve/sieve.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sieve/sieve.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/slim/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/slim/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/slim/slim.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/slim/slim.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/slim/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/slim/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smalltalk/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smalltalk/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smalltalk/smalltalk.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smalltalk/smalltalk.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smarty/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smarty/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/smarty/smarty.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/smarty/smarty.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/solr/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/solr/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/solr/solr.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/solr/solr.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/soy/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/soy/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/soy/soy.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/soy/soy.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/soy/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/soy/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sparql/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sparql/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sparql/sparql.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sparql/sparql.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/spreadsheet/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/spreadsheet/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/spreadsheet/spreadsheet.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/spreadsheet/spreadsheet.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sql/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sql/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/sql/sql.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/sql/sql.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stex/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stex/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stex/stex.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stex/stex.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stex/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stex/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stylus/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stylus/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/stylus/stylus.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/stylus/stylus.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/swift/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/swift/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/swift/swift.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/swift/swift.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/swift/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/swift/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tcl/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tcl/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tcl/tcl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tcl/tcl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/textile/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/textile/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/textile/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/textile/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/textile/textile.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/textile/textile.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiddlywiki/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiddlywiki/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiddlywiki/tiddlywiki.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiddlywiki/tiddlywiki.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiki/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiki/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tiki/tiki.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tiki/tiki.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/toml/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/toml/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/toml/toml.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/toml/toml.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tornado/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tornado/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/tornado/tornado.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/tornado/tornado.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/troff/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/troff/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/troff/troff.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/troff/troff.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn/ttcn.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn/ttcn.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn-cfg/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn-cfg/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/ttcn-cfg/ttcn-cfg.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/ttcn-cfg/ttcn-cfg.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/turtle/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/turtle/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/turtle/turtle.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/turtle/turtle.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/twig/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/twig/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/twig/twig.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/twig/twig.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vb/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vb/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vb/vb.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vb/vb.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vbscript/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vbscript/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vbscript/vbscript.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vbscript/vbscript.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/velocity/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/velocity/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/velocity/velocity.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/velocity/velocity.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/verilog/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/verilog/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/verilog/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/verilog/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/verilog/verilog.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/verilog/verilog.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vhdl/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vhdl/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vhdl/vhdl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vhdl/vhdl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vue/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vue/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/vue/vue.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/vue/vue.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/wast/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/wast/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/wast/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/wast/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/wast/wast.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/wast/wast.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/webidl/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/webidl/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/webidl/webidl.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/webidl/webidl.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xml/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xml/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xml/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xml/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xml/xml.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xml/xml.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xquery/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xquery/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xquery/test.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xquery/test.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/xquery/xquery.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/xquery/xquery.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yacas/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yacas/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yacas/yacas.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yacas/yacas.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml/yaml.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml/yaml.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/z80/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/z80/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/mode/z80/z80.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/mode/z80/z80.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/3024-day.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/3024-day.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/3024-night.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/3024-night.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/abbott.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/abbott.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/abcdef.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/abcdef.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ambiance.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ambiance.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ayu-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ayu-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ayu-mirage.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ayu-mirage.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/base16-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/base16-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/base16-light.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/base16-light.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/bespin.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/bespin.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/blackboard.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/blackboard.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/cobalt.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/cobalt.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/colorforth.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/colorforth.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/darcula.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/darcula.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/dracula.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/dracula.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/duotone-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/duotone-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/duotone-light.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/duotone-light.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/eclipse.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/eclipse.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/elegant.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/elegant.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/erlang-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/erlang-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/gruvbox-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/gruvbox-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/hopscotch.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/hopscotch.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/icecoder.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/icecoder.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/idea.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/idea.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/isotope.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/isotope.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/juejin.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/juejin.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/lesser-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/lesser-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/liquibyte.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/liquibyte.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/lucario.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/lucario.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/material-darker.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/material-darker.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/material-ocean.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/material-ocean.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/material-palenight.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/material-palenight.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/material.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/material.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/mbo.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/mbo.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/mdn-like.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/mdn-like.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/midnight.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/midnight.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/monokai.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/monokai.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/moxer.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/moxer.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/neat.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/neat.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/neo.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/neo.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/night.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/night.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/nord.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/nord.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/oceanic-next.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/oceanic-next.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/panda-syntax.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/panda-syntax.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/paraiso-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/paraiso-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/paraiso-light.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/paraiso-light.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/pastel-on-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/pastel-on-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/railscasts.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/railscasts.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/rubyblue.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/rubyblue.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/seti.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/seti.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/shadowfox.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/shadowfox.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/solarized.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/solarized.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ssms.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ssms.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/the-matrix.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/the-matrix.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/tomorrow-night-bright.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/tomorrow-night-bright.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/tomorrow-night-eighties.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/tomorrow-night-eighties.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/ttcn.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/ttcn.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/twilight.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/twilight.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/vibrant-ink.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/vibrant-ink.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/xq-dark.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/xq-dark.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/xq-light.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/xq-light.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/yeti.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/yeti.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/yonce.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/yonce.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/codemirror/theme/zenburn.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/codemirror/theme/zenburn.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/actions-parameters.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/actions-parameters.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/actions.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/actions.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/age_in_years.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/age_in_years.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/alignment.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/alignment.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/all-true.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/all-true.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/allow-emailing-false.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/allow-emailing-false.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/as-datetime.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/as-datetime.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/attachment-code.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/attachment-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/audio.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/audio.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/auto-terms.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/auto-terms.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action_flash.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action_flash.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action_javascript.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action_javascript.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action_refresh.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action_refresh.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_action_with_response_action.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_action_with_response_action.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/background_response_action_flash.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/background_response_action_flash.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/buttons-code.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/buttons-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/buttons-icons.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/buttons-icons.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/buttons-labels.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/buttons-labels.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/buttons.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/buttons.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/capitalize.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/capitalize.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/chat-partners-available.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/chat-partners-available.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/check-in.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/check-in.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices-combobox.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices-combobox.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices-dropdown.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices-dropdown.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices-icons.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices-icons.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices-with-default.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices-with-default.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/choices.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/choices.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/code.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/comment.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/comment.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/continue-button-label.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/continue-button-label.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/continue.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/continue.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/country.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/country.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/cron.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/cron.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/css.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/css.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/currency.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/currency.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/current-datetime.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/current-datetime.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/dadict.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/dadict.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/dafile.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/dafile.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/database_storage.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/database_storage.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/date-difference.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/date-difference.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/date-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/date-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/date-interval.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/date-interval.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/date-parts.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/date-parts.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/dead-end.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/dead-end.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/decoration.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/decoration.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/def.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/def.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/defined.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/defined.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/del.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/del.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/device.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/device.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/dialog-box.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/dialog-box.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document-docx.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document-docx.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document-file.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document-file.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document-language.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document-language.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document-variable-name.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document-variable-name.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/document.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/document.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/docx-template-table.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/docx-template-table.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/docx-template.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/docx-template.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/doors.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/doors.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/email-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/email-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/email-to-case-simple.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/email-to-case-simple.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/email-to-case.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/email-to-case.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/emoji-inline.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/emoji-inline.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exists.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exists.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exit-buttons.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exit-buttons.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exit-choices.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exit-choices.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exit-url.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exit-url.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/exit.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/exit.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/external_files.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/external_files.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-checkboxes.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-checkboxes.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-choices-combobox.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-choices-combobox.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-choices.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-choices.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-mc-exclude.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-mc-exclude.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-mc.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-mc.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-noyesmaybe.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-noyesmaybe.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-yesno.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-yesno.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-yesnomaybe.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-yesnomaybe.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-yesnoradio.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-yesnoradio.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fields-yesnowide.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fields-yesnowide.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/fix-punctuation.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/fix-punctuation.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/for_fruit.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/for_fruit.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/force-ask.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/force-ask.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/force-gather.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/force-gather.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/formatting.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/formatting.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-dict-object.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-dict-object.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-dict-value.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-dict-value.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-dict.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-dict.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-fruit-at-least-two.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-fruit-at-least-two.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-fruit-gather.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-fruit-gather.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-fruit-number.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-fruit-number.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-fruit.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-fruit.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-set-object.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-set-object.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/gather-set.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/gather-set.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/generic-object.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/generic-object.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/get-default-timezone.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/get-default-timezone.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/help-damages-audio.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/help-damages-audio.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/help.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/help.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/hideif-boolean.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/hideif-boolean.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/html.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/html.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/image-sets.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/image-sets.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/images.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/images.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/imports.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/imports.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/include.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/include.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/indefinite-article.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/indefinite-article.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/initial.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/initial.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/interface.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/interface.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/interview-help.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/interview-help.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/interview-url.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/interview-url.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/interview_url_action.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/interview_url_action.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/js_action_call.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/js_action_call.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/js_url_action.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/js_url_action.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/js_variables.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/js_variables.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/label.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/label.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/language.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/language.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/language_from_browser.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/language_from_browser.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/language_from_browser_restricted.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/language_from_browser_restricted.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/lists.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/lists.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/loading-legal.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/loading-legal.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/loading-util.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/loading-util.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/madlibs.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/madlibs.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-01.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-01.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-02.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-02.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-03.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-03.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-04.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-04.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-05.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-05.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-06.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-06.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-07.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-07.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mako-09.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mako-09.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mandatory.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mandatory.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/markdown.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/markdown.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/menu-item.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/menu-item.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/message.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/message.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/metadata.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/metadata.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/min.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/min.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/minlength.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/minlength.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-classify.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-classify.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-datatype.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-datatype.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-export-yaml.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-export-yaml.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-predict.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-predict.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ml-save-and-predict.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ml-save-and-predict.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/mlarea-datatype.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/mlarea-datatype.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/modules.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/modules.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/money-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/money-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/need.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/need.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/nested-loop.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/nested-loop.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/nice-number.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/nice-number.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/no-label-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/no-label-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/note.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/note.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/noun-plural.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/noun-plural.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/noyes.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/noyes.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/number-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/number-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object-checkboxes.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object-checkboxes.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object-disable-others.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object-disable-others.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object-radio.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object-radio.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object-selections.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object-selections.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/object.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/object.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/objects.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/objects.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ocr-chord.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ocr-chord.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ocr.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ocr.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/optional-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/optional-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/ordinal-number.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/ordinal-number.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/other.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/other.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/page-numbers.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/page-numbers.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/password-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/password-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/past-tense.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/past-tense.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pdf-a.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pdf-a.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pdf-fill-code.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pdf-fill-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pdf-fill-signature.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pdf-fill-signature.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pdf-fill.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pdf-fill.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/periodic-amount.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/periodic-amount.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/periodic-value.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/periodic-value.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/prevent-back.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/prevent-back.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/prevent-going-back.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/prevent-going-back.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/progress-features.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/progress-features.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/progress.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/progress.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pull-down-with-code.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pull-down-with-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/pull-down.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/pull-down.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/qr-code.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/qr-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/quantity-noun.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/quantity-noun.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/quote_paragraphs.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/quote_paragraphs.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/radio-list.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/radio-list.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/range.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/range.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/reconsider.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/reconsider.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/redis.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/redis.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/refresh.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/refresh.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/reload.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/reload.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/required-code.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/required-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/reset.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/reset.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/response-json.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/response-json.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/response-svg.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/response-svg.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/response.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/response.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/resume-button-label.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/resume-button-label.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/review.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/review.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/salutation.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/salutation.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/save-url-to-file.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/save-url-to-file.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/script.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/script.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords-code.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords-code.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords-get-sections.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords-get-sections.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords-review.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords-review.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords-set-sections.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords-set-sections.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections-keywords.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections-keywords.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/sections.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/sections.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/send-email.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/send-email.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/set-language.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/set-language.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/showif-boolean.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/showif-boolean.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/showif.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/showif.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/shuffle.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/shuffle.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/signature.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/signature.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/signin.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/signin.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/single-spacing.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/single-spacing.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/space-underscore.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/space-underscore.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/state.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/state.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/static_image.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/static_image.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/subdivision-type.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/subdivision-type.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/table-mako.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/table-mako.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/table-markdown.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/table-markdown.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/table.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/table.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/target-template.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/target-template.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/template-file.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/template-file.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/template-subject.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/template-subject.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/template.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/template.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/terms.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/terms.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-box-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-box-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-default.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-default.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-field.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-field.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-help.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-help.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/text-hint.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/text-hint.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/timezone-list.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/timezone-list.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/title-case.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/title-case.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/today.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/today.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/under.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/under.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/upload-multiple.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/upload-multiple.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/upload.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/upload.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/url-of.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/url-of.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/valid-formats.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/valid-formats.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/value.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/value.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/variables_as_json.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/variables_as_json.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/video.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/video.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/yesno-custom.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/yesno-custom.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/yesno.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/yesno.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/examples/yesnomaybe.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/examples/yesnomaybe.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/all.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/all.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/all.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/all.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/brands.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/brands.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/brands.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/brands.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/conflict-detection.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/conflict-detection.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/conflict-detection.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/conflict-detection.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/fontawesome.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/fontawesome.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/regular.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/regular.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/regular.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/regular.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/solid.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/solid.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/solid.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/v4-shims.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/v4-shims.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/fontawesome/js/v4-shims.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/fontawesome/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/img/loading-sm.gif` & `docassemble.webapp-1.4.99/docassemble/webapp/static/img/loading-sm.gif`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/img/loading.gif` & `docassemble.webapp-1.4.99/docassemble/webapp/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/index.html` & `docassemble.webapp-1.4.99/docassemble/webapp/static/index.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/LICENSE` & `docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/README.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/jquery-labelauty.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/jquery-labelauty.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/jquery-labelauty.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/jquery-labelauty.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.css` & `docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/labelauty/source/jquery-labelauty.min.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/office/cat-in-circle-32.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/office/cat-in-circle-32.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/office/cat-in-circle-80.png` & `docassemble.webapp-1.4.99/docassemble/webapp/static/office/cat-in-circle-80.png`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/office/officeinner.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/office/officeinner.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/office/polyfill.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/office/polyfill.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/office/word.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/office/word.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/README.md` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click-off.mp3` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click-off.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click-off.ogg` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click-off.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click-on.mp3` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click-on.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click-on.ogg` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click-on.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click.mp3` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-click.ogg` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-click.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-snap.mp3` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-snap.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-snap.ogg` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-snap.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-stapler.mp3` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-stapler.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/sounds/notification-stapler.ogg` & `docassemble.webapp-1.4.99/docassemble/webapp/static/sounds/notification-stapler.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/static/yamlmixed/yamlmixed.js` & `docassemble.webapp-1.4.99/docassemble/webapp/static/yamlmixed/yamlmixed.js`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/telnyx.py` & `docassemble.webapp-1.4.99/docassemble/webapp/telnyx.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/base.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/flask_two_col_base.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/flask_two_col_base.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/base_templates/form_macros.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/base_templates/form_macros.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/_macros.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/_macros.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/change_password.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/change_password.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/emails/registered_message.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/emails/registered_message.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/forgot_password.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/forgot_password.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/google_login.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/google_login.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/invite.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/invite.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/login.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/login.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/login_or_register.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/login_or_register.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/manage_emails.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/manage_emails.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_choose.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_choose.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_reconfigure.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_reconfigure.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/mfa_setup.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/mfa_setup.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/phone_login_verify.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/phone_login_verify.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/register.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/register.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/reset_password.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/reset_password.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/flask_user/user_profile.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/flask_user/user_profile.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/404.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/404.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/501.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/501.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/admin_page.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/admin_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/config.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/config.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/create_playground_package.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/create_playground_package.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/gd_sync_wait.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/gd_sync_wait.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/github.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/github.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/googledrive.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/googledrive.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/home_page.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/home_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/interviews.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/interviews.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/logs.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/logs.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/manage_account.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/manage_account.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/manage_api.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/manage_api.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/manage_playgrounds.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/manage_playgrounds.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/manage_projects.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/manage_projects.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/member_page.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/member_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/monitor.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/monitor.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/od_sync_wait.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/od_sync_wait.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/officeaddin.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/officeaddin.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/officefunctionfile.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/officefunctionfile.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/officemanifest.xml` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/officemanifest.xml`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/officeouter.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/officeouter.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/onedrive.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/onedrive.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/packages.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/packages.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/playground.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/playground.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/playgroundfiles.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/playgroundfiles.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/playgroundpackages.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/playgroundpackages.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/pull_playground_package.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/pull_playground_package.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/rename_project.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/rename_project.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/start.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/start.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/test_embed.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/test_embed.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/train.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/train.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/update_package.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/update_package.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/update_package_wait.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/update_package_wait.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/utilities.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/utilities.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/pages/webrtc.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/pages/webrtc.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/users/add_user_page.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/users/add_user_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/users/edit_user_profile_page.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/users/edit_user_profile_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/users/request_developer.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/users/request_developer.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/users/rolelist.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/users/rolelist.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/users/user_profile_page.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/users/user_profile_page.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/templates/users/userlist.html` & `docassemble.webapp-1.4.99/docassemble/webapp/templates/users/userlist.html`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/translations.py` & `docassemble.webapp-1.4.99/docassemble/webapp/translations.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/update.py` & `docassemble.webapp-1.4.99/docassemble/webapp/update.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/user_database.py` & `docassemble.webapp-1.4.99/docassemble/webapp/user_database.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/users/_readme.txt` & `docassemble.webapp-1.4.99/docassemble/webapp/users/_readme.txt`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/users/forms.py` & `docassemble.webapp-1.4.99/docassemble/webapp/users/forms.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/users/models.py` & `docassemble.webapp-1.4.99/docassemble/webapp/users/models.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/users/views.py` & `docassemble.webapp-1.4.99/docassemble/webapp/users/views.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/watchdog.py` & `docassemble.webapp-1.4.99/docassemble/webapp/watchdog.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/worker.py` & `docassemble.webapp-1.4.99/docassemble/webapp/worker.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/worker_common.py` & `docassemble.webapp-1.4.99/docassemble/webapp/worker_common.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/worker_tasks.py` & `docassemble.webapp-1.4.99/docassemble/webapp/worker_tasks.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble/webapp/wsgi_restart.py` & `docassemble.webapp-1.4.99/docassemble/webapp/wsgi_restart.py`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble.webapp.egg-info/PKG-INFO` & `docassemble.webapp-1.4.99/docassemble.webapp.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.webapp
-Version: 1.4.98
+Version: 1.4.99
 Summary: The web application components of the docassemble system.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `docassemble.webapp-1.4.98/docassemble.webapp.egg-info/SOURCES.txt` & `docassemble.webapp-1.4.99/docassemble.webapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docassemble.webapp-1.4.98/docassemble.webapp.egg-info/requires.txt` & `docassemble.webapp-1.4.99/docassemble.webapp.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 Flask-WTF==1.2.1
 Flask==3.0.0
 Hyphenate==1.1.0
 Jinja2==3.1.3
 Mako==1.3.0
 Markdown==3.5.1
 MarkupSafe==2.1.3
-Pillow==10.1.0
+Pillow==10.2.0
 PyJWT==2.8.0
 PyLaTeX==1.4.2
 PyNaCl==1.5.0
 PySocks==1.7.1
 PyYAML==6.0.1
 Pygments==2.17.2
 SQLAlchemy==2.0.23
 SecretStorage==3.3.3
 SocksiPy-branch==1.1
 WTForms==3.1.1
 Werkzeug==3.0.1
 XlsxWriter==3.1.9
 acme==2.8.0
 aiohttp-retry==2.8.3
-aiohttp==3.9.1
+aiohttp==3.9.2
 aiosignal==1.3.1
 airtable-python-wrapper==0.15.3
 alembic==1.13.1
 amqp==5.2.0
 anyio==4.2.0
 argon2-cffi-bindings==21.2.0
 argon2-cffi==23.1.0
@@ -60,15 +60,15 @@
 bleach==6.1.0
 blinker==1.7.0
 boto3==1.34.5
 boto==2.49.0
 botocore==1.34.5
 cachetools==5.3.2
 cairocffi==1.6.1
-celery==5.3.6
+celery==5.4.0rc1
 certbot-apache==2.8.0
 certbot-nginx==2.8.0
 certbot==2.8.0
 certifi==2023.11.17
 cffi==1.16.0
 chardet==5.2.0
 charset-normalizer==3.3.2
@@ -87,17 +87,17 @@
 cssselect2==0.7.0
 defusedxml==0.7.1
 deprecation==2.1.0
 distro==1.8.0
 dnspython==2.4.2
 docassemble-backports==1.0
 docassemble-textstat==0.7.2
-docassemble.base==1.4.98
-docassemble.demo==1.4.98
-docassemble==1.4.98
+docassemble.base==1.4.99
+docassemble.demo==1.4.99
+docassemble==1.4.99
 docassemblekvsession==0.8
 docopt==0.6.2
 docutils==0.20.1
 docxcompose==1.4.0
 docxtpl==0.16.7
 email-validator==2.1.0.post1
 et-xmlfile==1.1.0
@@ -216,15 +216,15 @@
 pytz-deprecation-shim==0.1.0.post0
 pytz==2023.3.post1
 pyu2f==0.1.5
 pyzbar==0.1.9
 qrcode==7.4.2
 rauth==0.7.3
 readme-renderer==42.0
-redis==5.0.1
+redis==5.0.2
 regex==2023.10.3
 reportlab==4.0.8
 repoze.lru==0.7
 requests-oauthlib==1.3.1
 requests-toolbelt==1.0.0
 requests==2.31.0
 retry-decorator==1.1.1
```

### Comparing `docassemble.webapp-1.4.98/setup.py` & `docassemble.webapp-1.4.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding='utf-8').read()
 
 setup_requires = [
     'enum34==1.1.10'
     ]
 install_requires = [
-    'docassemble==1.4.98',
-    'docassemble.base==1.4.98',
-    'docassemble.demo==1.4.98',
+    'docassemble==1.4.99',
+    'docassemble.base==1.4.99',
+    'docassemble.demo==1.4.99',
     "3to2==1.1.1",
     "acme==2.8.0",
-    "aiohttp==3.9.1",
+    "aiohttp==3.9.2",
     "aiohttp-retry==2.8.3",
     "aiosignal==1.3.1",
     "airtable-python-wrapper==0.15.3",
     "alembic==1.13.1",
     "amqp==5.2.0",
     "anyio==4.2.0",
     "argon2-cffi==23.1.0",
@@ -46,15 +46,15 @@
     "blinker==1.7.0",
     "boto==2.49.0",
     "boto3==1.34.5",
     "botocore==1.34.5",
     "cachetools==5.3.2",
     "cairocffi==1.6.1",
     "CairoSVG==2.7.1",
-    "celery==5.3.6",
+    "celery==5.4.0rc1",
     "certbot==2.8.0",
     "certbot-apache==2.8.0",
     "certbot-nginx==2.8.0",
     "certifi==2023.11.17",
     "cffi==1.16.0",
     "chardet==5.2.0",
     "charset-normalizer==3.3.2",
@@ -177,15 +177,15 @@
     "parse==1.20.0",
     "parse-type==0.6.2",
     "parsedatetime==2.6",
     "passlib==1.7.4",
     "pdfminer.six==20221105",
     "phonenumbers==8.13.27",
     "pikepdf==8.10.1",
-    "Pillow==10.1.0",
+    "Pillow==10.2.0",
     "pkginfo==1.9.6",
     "pluggy==1.3.0",
     "ply==3.11",
     "portalocker==2.8.2",
     "prompt-toolkit==3.0.43",
     "proto-plus==1.23.0",
     "protobuf==4.25.1",
@@ -222,15 +222,15 @@
     "pytz-deprecation-shim==0.1.0.post0",
     "pyu2f==0.1.5",
     "PyYAML==6.0.1",
     "pyzbar==0.1.9",
     "qrcode==7.4.2",
     "rauth==0.7.3",
     "readme-renderer==42.0",
-    "redis==5.0.1",
+    "redis==5.0.2",
     "regex==2023.10.3",
     "reportlab==4.0.8",
     "repoze.lru==0.7",
     "requests==2.31.0",
     "requests-oauthlib==1.3.1",
     "requests-toolbelt==1.0.0",
     "retry-decorator==1.1.1",
@@ -293,15 +293,15 @@
     "XlsxWriter==3.1.9",
     "xlwt==1.3.0",
     "yarl==1.9.4",
     "zipp==3.17.0"
 ]
 
 setup(name='docassemble.webapp',
-      version='1.4.98',
+      version='1.4.99',
       python_requires='>=3.9',
       description=('The web application components of the docassemble system.'),
       long_description=read("README.md"),
       long_description_content_type='text/markdown',
       author='Jonathan Pyle',
       author_email='jhpyle@gmail.com',
       license='MIT',
```

