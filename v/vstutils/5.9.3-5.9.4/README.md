# Comparing `tmp/vstutils-5.9.3.tar.gz` & `tmp/vstutils-5.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.9.3.tar", last modified: Thu Mar 14 16:07:06 2024, max compression
+gzip compressed data, was "vstutils-5.9.4.tar", last modified: Sat Jun  1 04:18:41 2024, max compression
```

## Comparing `vstutils-5.9.3.tar` & `vstutils-5.9.4.tar`

### file list

```diff
@@ -1,291 +1,291 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.168767 vstutils-5.9.3/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.9.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1171 2023-10-07 05:51:20.000000 vstutils-5.9.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2024-01-11 12:04:31.000000 vstutils-5.9.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8240 2024-03-14 16:07:06.168767 vstutils-5.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2276 2024-01-11 12:04:31.000000 vstutils-5.9.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     4398 2024-02-01 07:51:59.000000 vstutils-5.9.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-12-21 20:32:28.000000 vstutils-5.9.3/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.9.3/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-12-21 20:32:28.000000 vstutils-5.9.3/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-02-06 02:30:57.000000 vstutils-5.9.3/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-12-06 02:11:16.000000 vstutils-5.9.3/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-01-11 12:04:31.000000 vstutils-5.9.3/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-02-06 02:30:57.000000 vstutils-5.9.3/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-02-27 04:42:18.000000 vstutils-5.9.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-14 16:07:06.168767 vstutils-5.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2426 2024-02-27 04:42:18.000000 vstutils-5.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.104767 vstutils-5.9.3/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-03-13 08:11:31.000000 vstutils-5.9.3/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.116767 vstutils-5.9.3/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15917 2024-02-01 07:52:49.000000 vstutils-5.9.3/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     3822 2023-10-07 05:51:20.000000 vstutils-5.9.3/vstutils/api/actions.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.9.3/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-11-17 00:50:16.000000 vstutils-5.9.3/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13625 2024-02-27 04:43:02.000000 vstutils-5.9.3/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    37549 2024-03-14 09:13:47.000000 vstutils-5.9.3/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6331 2024-02-08 04:05:05.000000 vstutils-5.9.3/vstutils/api/base.pyi
--rw-rw-rw-   0 root         (0) root         (0)    24031 2023-08-01 02:26:22.000000 vstutils-5.9.3/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6690 2023-11-25 05:46:17.000000 vstutils-5.9.3/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    19240 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    71911 2024-01-16 07:23:05.000000 vstutils-5.9.3/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    15468 2023-09-19 05:49:20.000000 vstutils-5.9.3/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.9.3/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2023-11-17 00:50:16.000000 vstutils-5.9.3/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.116767 vstutils-5.9.3/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-09-12 05:09:55.000000 vstutils-5.9.3/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4893 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-09-05 23:43:43.000000 vstutils-5.9.3/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1493 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1597 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9519 2023-11-17 00:50:16.000000 vstutils-5.9.3/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.9.3/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.116767 vstutils-5.9.3/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6270 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    25711 2023-12-21 20:32:28.000000 vstutils-5.9.3/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-20 19:01:25.000000 vstutils-5.9.3/vstutils/api/schema/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)    12118 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-12-21 20:32:28.000000 vstutils-5.9.3/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     9639 2024-01-16 07:23:05.000000 vstutils-5.9.3/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    11052 2023-09-26 06:28:24.000000 vstutils-5.9.3/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5665 2023-11-17 00:50:16.000000 vstutils-5.9.3/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-10-07 05:51:20.000000 vstutils-5.9.3/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3583 2024-02-06 02:30:57.000000 vstutils-5.9.3/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-09-19 05:49:20.000000 vstutils-5.9.3/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-07-20 20:14:05.000000 vstutils-5.9.3/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.9.3/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.9.3/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.092767 vstutils-5.9.3/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.120767 vstutils-5.9.3/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.120767 vstutils-5.9.3/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/doc_themes/vst-sphinx-theme/theme.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.120767 vstutils-5.9.3/vstutils/drivers/
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-12-21 20:32:28.000000 vstutils-5.9.3/vstutils/drivers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7453 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/drivers/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    10119 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/drivers/kombu.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.120767 vstutils-5.9.3/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3541 2023-11-17 00:50:16.000000 vstutils-5.9.3/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7469 2023-09-12 05:09:55.000000 vstutils-5.9.3/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.9.3/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6531 2023-12-21 20:32:28.000000 vstutils-5.9.3/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.120767 vstutils-5.9.3/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.124767 vstutils-5.9.3/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:54.000000 vstutils-5.9.3/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4959 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-12-19 03:38:29.000000 vstutils-5.9.3/vstutils/management/commands/rpc_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-17 22:32:27.000000 vstutils-5.9.3/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.9.3/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.9.3/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)     9821 2023-10-07 05:51:20.000000 vstutils-5.9.3/vstutils/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     2479 2023-10-07 05:51:20.000000 vstutils-5.9.3/vstutils/middleware.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.128767 vstutils-5.9.3/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    12091 2023-11-25 05:46:17.000000 vstutils-5.9.3/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-11-25 05:46:17.000000 vstutils-5.9.3/vstutils/models/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)    27339 2023-11-25 05:46:17.000000 vstutils-5.9.3/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5947 2023-11-25 05:46:17.000000 vstutils-5.9.3/vstutils/models/base.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4608 2023-10-07 05:51:20.000000 vstutils-5.9.3/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-10-07 05:51:20.000000 vstutils-5.9.3/vstutils/models/cent_notify.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16047 2024-01-11 12:04:31.000000 vstutils-5.9.3/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.9.3/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3880 2024-01-11 12:04:31.000000 vstutils-5.9.3/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/models/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8549 2023-08-08 02:23:29.000000 vstutils-5.9.3/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1988 2023-10-07 05:51:20.000000 vstutils-5.9.3/vstutils/models/fields.pyi
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-02-06 06:25:26.000000 vstutils-5.9.3/vstutils/models/model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8390 2023-11-17 00:50:16.000000 vstutils-5.9.3/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/models/queryset.pyi
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    57065 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.9.3/vstutils/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.092767 vstutils-5.9.3/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.140767 vstutils-5.9.3/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      149 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   125639 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      166 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1547 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136074 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15719 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38108 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/408.js
--rw-r--r--   0 root         (0) root         (0)       93 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/408.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  1066383 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      300 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      345 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)     2229 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    72156 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   535978 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    87203 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      218 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355653 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177805 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1420006 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/865.js
--rw-r--r--   0 root         (0) root         (0)     2010 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/865.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    49266 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   283787 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3350 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   449356 2024-03-14 16:07:05.000000 vstutils-5.9.3/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.140767 vstutils-5.9.3/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.140767 vstutils-5.9.3/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2184 2023-09-21 04:30:46.000000 vstutils-5.9.3/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5730 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-10-07 05:51:20.000000 vstutils-5.9.3/vstutils/tasks.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.144767 vstutils-5.9.3/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.9.3/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.9.3/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.9.3/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.9.3/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.144767 vstutils-5.9.3/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2860 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.9.3/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.9.3/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.144767 vstutils-5.9.3/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.144767 vstutils-5.9.3/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.9.3/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.144767 vstutils-5.9.3/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1583 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.148767 vstutils-5.9.3/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.148767 vstutils-5.9.3/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.148767 vstutils-5.9.3/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.152767 vstutils-5.9.3/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.152767 vstutils-5.9.3/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/templates/newproject/pyproject.toml.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2523 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     1257 2023-12-27 07:21:33.000000 vstutils-5.9.3/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.152767 vstutils-5.9.3/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.9.3/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.156767 vstutils-5.9.3/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.156767 vstutils-5.9.3/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.156767 vstutils-5.9.3/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.156767 vstutils-5.9.3/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.9.3/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)      437 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/templatetags/sw.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2023-09-19 05:49:20.000000 vstutils-5.9.3/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-12-06 02:11:16.000000 vstutils-5.9.3/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.9.3/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-09-19 05:49:20.000000 vstutils-5.9.3/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    18521 2023-11-17 00:50:16.000000 vstutils-5.9.3/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-09-21 04:30:46.000000 vstutils-5.9.3/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.160767 vstutils-5.9.3/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17307 2024-03-13 08:11:31.000000 vstutils-5.9.3/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    25628 2024-03-13 08:40:07.000000 vstutils-5.9.3/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    20424 2024-03-13 08:11:31.000000 vstutils-5.9.3/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2023-09-19 05:49:20.000000 vstutils-5.9.3/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    45765 2024-01-15 08:10:37.000000 vstutils-5.9.3/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11297 2023-12-06 02:11:16.000000 vstutils-5.9.3/vstutils/utils.pyi
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.9.3/vstutils/web.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.160767 vstutils-5.9.3/vstutils/webpush/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5287 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/api.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2024-02-27 04:43:02.000000 vstutils-5.9.3/vstutils/webpush/autodiscovery.py
--rw-rw-rw-   0 root         (0) root         (0)     4262 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.160767 vstutils-5.9.3/vstutils/webpush/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1920 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/models.py
--rw-rw-rw-   0 root         (0) root         (0)      437 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.096767 vstutils-5.9.3/vstutils/webpush/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.160767 vstutils-5.9.3/vstutils/webpush/templates/webpush/
--rw-rw-rw-   0 root         (0) root         (0)     1962 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/templates/webpush/notification-handler.js
--rw-rw-rw-   0 root         (0) root         (0)     3423 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.160767 vstutils-5.9.3/vstutils/webpush/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-02-01 07:51:59.000000 vstutils-5.9.3/vstutils/webpush/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.9.3/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 16:07:06.164767 vstutils-5.9.3/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8240 2024-03-14 16:07:06.000000 vstutils-5.9.3/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8581 2024-03-14 16:07:06.000000 vstutils-5.9.3/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-03-14 16:07:06.000000 vstutils-5.9.3/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-14 16:07:06.000000 vstutils-5.9.3/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 16:07:06.000000 vstutils-5.9.3/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1886 2024-03-14 16:07:06.000000 vstutils-5.9.3/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-14 16:07:06.000000 vstutils-5.9.3/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.380264 vstutils-5.9.4/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:36:10.000000 vstutils-5.9.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1171 2023-10-07 05:51:20.000000 vstutils-5.9.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-01-11 12:04:30.000000 vstutils-5.9.4/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8240 2024-06-01 04:18:41.380264 vstutils-5.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2024-01-11 12:04:30.000000 vstutils-5.9.4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4398 2024-06-01 04:11:47.000000 vstutils-5.9.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-12-21 20:32:27.000000 vstutils-5.9.4/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:36:10.000000 vstutils-5.9.4/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-12-21 20:32:27.000000 vstutils-5.9.4/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-06-01 04:11:47.000000 vstutils-5.9.4/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-06-01 04:11:47.000000 vstutils-5.9.4/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-01-11 12:04:30.000000 vstutils-5.9.4/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-06-01 04:11:47.000000 vstutils-5.9.4/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-06-01 04:11:47.000000 vstutils-5.9.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 04:18:41.380264 vstutils-5.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2024-06-01 04:11:47.000000 vstutils-5.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.304264 vstutils-5.9.4/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.312264 vstutils-5.9.4/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15917 2024-05-27 05:18:21.000000 vstutils-5.9.4/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3822 2024-05-27 05:18:21.000000 vstutils-5.9.4/vstutils/api/actions.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-11-17 00:50:16.000000 vstutils-5.9.4/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13625 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    37549 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6331 2024-02-08 04:05:03.000000 vstutils-5.9.4/vstutils/api/base.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    24031 2023-08-01 02:26:22.000000 vstutils-5.9.4/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6690 2023-11-25 05:46:15.000000 vstutils-5.9.4/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    19240 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    71911 2024-01-16 07:23:05.000000 vstutils-5.9.4/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    15468 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:14:38.000000 vstutils-5.9.4/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.316264 vstutils-5.9.4/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-09-12 05:09:54.000000 vstutils-5.9.4/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4893 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-09-05 23:43:42.000000 vstutils-5.9.4/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9519 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.316264 vstutils-5.9.4/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6270 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    25711 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-20 19:01:25.000000 vstutils-5.9.4/vstutils/api/schema/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)    12118 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-12-21 20:32:27.000000 vstutils-5.9.4/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     9639 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    11052 2023-09-26 06:28:24.000000 vstutils-5.9.4/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5665 2023-11-17 00:50:16.000000 vstutils-5.9.4/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-10-07 05:51:20.000000 vstutils-5.9.4/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3583 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-09-19 05:49:21.000000 vstutils-5.9.4/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-07-20 20:14:05.000000 vstutils-5.9.4/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.288264 vstutils-5.9.4/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.316264 vstutils-5.9.4/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.320264 vstutils-5.9.4/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.320264 vstutils-5.9.4/vstutils/drivers/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-12-21 20:32:27.000000 vstutils-5.9.4/vstutils/drivers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7453 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/drivers/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    10119 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/drivers/kombu.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.320264 vstutils-5.9.4/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7469 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6531 2023-12-21 20:32:27.000000 vstutils-5.9.4/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.320264 vstutils-5.9.4/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.324264 vstutils-5.9.4/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:53.000000 vstutils-5.9.4/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4959 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/management/commands/rpc_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-07-17 22:32:27.000000 vstutils-5.9.4/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)     9907 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/middleware.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.328264 vstutils-5.9.4/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    12091 2023-11-25 05:46:15.000000 vstutils-5.9.4/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-11-25 05:46:15.000000 vstutils-5.9.4/vstutils/models/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    27339 2023-11-25 05:46:15.000000 vstutils-5.9.4/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5947 2023-11-25 05:46:15.000000 vstutils-5.9.4/vstutils/models/base.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4608 2024-04-17 10:55:19.000000 vstutils-5.9.4/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-10-07 05:51:20.000000 vstutils-5.9.4/vstutils/models/cent_notify.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16047 2024-01-11 12:04:30.000000 vstutils-5.9.4/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.9.4/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2024-01-11 12:04:30.000000 vstutils-5.9.4/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/models/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8549 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2023-10-07 05:51:20.000000 vstutils-5.9.4/vstutils/models/fields.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/models/model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8390 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/models/queryset.pyi
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    57065 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:30:58.000000 vstutils-5.9.4/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.288264 vstutils-5.9.4/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.340264 vstutils-5.9.4/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      149 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   125639 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      166 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136074 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15719 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38108 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/408.js
+-rw-r--r--   0 root         (0) root         (0)       93 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/408.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  1066383 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      300 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      345 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    72156 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   535978 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    87203 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      218 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355653 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177805 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1420006 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/865.js
+-rw-r--r--   0 root         (0) root         (0)     2010 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/865.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    49266 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   283787 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3350 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   449356 2024-06-01 04:18:40.000000 vstutils-5.9.4/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.340264 vstutils-5.9.4/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.340264 vstutils-5.9.4/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5730 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-10-07 05:51:20.000000 vstutils-5.9.4/vstutils/tasks.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.344264 vstutils-5.9.4/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.344264 vstutils-5.9.4/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2860 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 07:56:30.000000 vstutils-5.9.4/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.344264 vstutils-5.9.4/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.344264 vstutils-5.9.4/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.348264 vstutils-5.9.4/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.352264 vstutils-5.9.4/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.356264 vstutils-5.9.4/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.356264 vstutils-5.9.4/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.360264 vstutils-5.9.4/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.360264 vstutils-5.9.4/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/templates/newproject/pyproject.toml.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2523 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2023-12-27 07:22:20.000000 vstutils-5.9.4/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.360264 vstutils-5.9.4/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.364264 vstutils-5.9.4/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.364264 vstutils-5.9.4/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.364264 vstutils-5.9.4/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.368264 vstutils-5.9.4/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-24 07:40:21.000000 vstutils-5.9.4/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)      437 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/templatetags/sw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-12-06 02:11:16.000000 vstutils-5.9.4/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-09-19 05:49:21.000000 vstutils-5.9.4/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18521 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-09-22 09:36:17.000000 vstutils-5.9.4/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.368264 vstutils-5.9.4/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17307 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    25628 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    20424 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    45765 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11297 2024-06-01 04:11:47.000000 vstutils-5.9.4/vstutils/utils.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.9.4/vstutils/web.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.368264 vstutils-5.9.4/vstutils/webpush/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5287 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-02-27 04:49:55.000000 vstutils-5.9.4/vstutils/webpush/autodiscovery.py
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.372264 vstutils-5.9.4/vstutils/webpush/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      437 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.292264 vstutils-5.9.4/vstutils/webpush/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.372264 vstutils-5.9.4/vstutils/webpush/templates/webpush/
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/templates/webpush/notification-handler.js
+-rw-rw-rw-   0 root         (0) root         (0)     3423 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.372264 vstutils-5.9.4/vstutils/webpush/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-02-01 07:52:27.000000 vstutils-5.9.4/vstutils/webpush/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:36:10.000000 vstutils-5.9.4/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 04:18:41.372264 vstutils-5.9.4/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8240 2024-06-01 04:18:41.000000 vstutils-5.9.4/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8581 2024-06-01 04:18:41.000000 vstutils-5.9.4/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-06-01 04:18:41.000000 vstutils-5.9.4/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-06-01 04:18:41.000000 vstutils-5.9.4/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 04:18:41.000000 vstutils-5.9.4/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1886 2024-06-01 04:18:41.000000 vstutils-5.9.4/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-06-01 04:18:41.000000 vstutils-5.9.4/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.9.3/LICENSE` & `vstutils-5.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/MANIFEST.in` & `vstutils-5.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/NOTICE` & `vstutils-5.9.4/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/PKG-INFO` & `vstutils-5.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.9.3
+Version: 5.9.4
 Summary: VST Utils Framework for fast create web-application
 Author-email: Sergei Kliuikov <sergey.k@vstconsulting.net>, Dmitriy Ovcharenko  <ovcharenkodd@gmail.com>
 Maintainer-email: VST Consulting <sergey.k@vstconsulting.net>
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source, https://gitlab.com/vstconsulting/vstutils
 Project-URL: Releases, https://pypi.org/project/vstutils/#history
```

### Comparing `vstutils-5.9.3/README.rst` & `vstutils-5.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/pyproject.toml` & `vstutils-5.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/requirements.txt` & `vstutils-5.9.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/setup.py` & `vstutils-5.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/actions.py` & `vstutils-5.9.4/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/actions.pyi` & `vstutils-5.9.4/vstutils/api/actions.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/admin.py` & `vstutils-5.9.4/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/auth.py` & `vstutils-5.9.4/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/base.py` & `vstutils-5.9.4/vstutils/api/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/base.pyi` & `vstutils-5.9.4/vstutils/api/base.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/decorators.py` & `vstutils-5.9.4/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/decorators.pyi` & `vstutils-5.9.4/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/endpoint.py` & `vstutils-5.9.4/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/fields.py` & `vstutils-5.9.4/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/filter_backends.py` & `vstutils-5.9.4/vstutils/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/filters.py` & `vstutils-5.9.4/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/health.py` & `vstutils-5.9.4/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/meta.py` & `vstutils-5.9.4/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/metrics.py` & `vstutils-5.9.4/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/migrations/0001_initial.py` & `vstutils-5.9.4/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.9.4/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.9.4/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.9.4/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.9.4/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.9.4/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/models.py` & `vstutils-5.9.4/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/pagination.py` & `vstutils-5.9.4/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/parsers.py` & `vstutils-5.9.4/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/permissions.py` & `vstutils-5.9.4/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/renderers.py` & `vstutils-5.9.4/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/responses.py` & `vstutils-5.9.4/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/responses.pyi` & `vstutils-5.9.4/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/routers.py` & `vstutils-5.9.4/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/routers.pyi` & `vstutils-5.9.4/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/schema/generators.py` & `vstutils-5.9.4/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/schema/info.py` & `vstutils-5.9.4/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/schema/inspectors.py` & `vstutils-5.9.4/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/schema/schema.py` & `vstutils-5.9.4/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/schema/views.py` & `vstutils-5.9.4/vstutils/api/schema/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/serializers.py` & `vstutils-5.9.4/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/throttling.py` & `vstutils-5.9.4/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/validators.py` & `vstutils-5.9.4/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/api/views.py` & `vstutils-5.9.4/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/asgi.py` & `vstutils-5.9.4/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/asgi_worker.py` & `vstutils-5.9.4/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/auth.py` & `vstutils-5.9.4/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/auth.pyi` & `vstutils-5.9.4/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/celery_beat_scheduler.py` & `vstutils-5.9.4/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.9.4/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/drivers/cache.py` & `vstutils-5.9.4/vstutils/drivers/cache.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/drivers/kombu.py` & `vstutils-5.9.4/vstutils/drivers/kombu.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/environment.py` & `vstutils-5.9.4/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/exceptions.py` & `vstutils-5.9.4/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/gui/context.py` & `vstutils-5.9.4/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/gui/forms.py` & `vstutils-5.9.4/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/gui/pwa_manifest.py` & `vstutils-5.9.4/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/gui/views.py` & `vstutils-5.9.4/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/ldap_utils.py` & `vstutils-5.9.4/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/_base.py` & `vstutils-5.9.4/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/celery_inspect.py` & `vstutils-5.9.4/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/dockerrun.py` & `vstutils-5.9.4/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/newproject.py` & `vstutils-5.9.4/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/rpc_worker.py` & `vstutils-5.9.4/vstutils/management/commands/rpc_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/run_task.py` & `vstutils-5.9.4/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/runrpc.py` & `vstutils-5.9.4/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/runserver.py` & `vstutils-5.9.4/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/management/commands/web.py` & `vstutils-5.9.4/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/middleware.py` & `vstutils-5.9.4/vstutils/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 class LangMiddleware(BaseMiddleware):
     __slots__ = ()
 
     def get_lang_object(self, request):
         set_cookie = True
         if 'lang' in request.GET:
             code = request.GET['lang']
+            set_cookie = request.COOKIES.get('settings.LANGUAGE_COOKIE_NAME') != code
         elif settings.LANGUAGE_COOKIE_NAME in request.COOKIES:
             code = request.COOKIES[settings.LANGUAGE_COOKIE_NAME]
             set_cookie = False
         else:
             code = translation.get_language_from_request(request)
         obj = Language.objects.filter(code=code).first()
         if obj is not None:
```

### Comparing `vstutils-5.9.3/vstutils/middleware.pyi` & `vstutils-5.9.4/vstutils/middleware.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/__init__.py` & `vstutils-5.9.4/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/__init__.pyi` & `vstutils-5.9.4/vstutils/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/base.py` & `vstutils-5.9.4/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/base.pyi` & `vstutils-5.9.4/vstutils/models/base.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/cent_notify.py` & `vstutils-5.9.4/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/cent_notify.pyi` & `vstutils-5.9.4/vstutils/models/cent_notify.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/custom_model.py` & `vstutils-5.9.4/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/custom_model.pyi` & `vstutils-5.9.4/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/decorators.py` & `vstutils-5.9.4/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/decorators.pyi` & `vstutils-5.9.4/vstutils/models/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/fields.py` & `vstutils-5.9.4/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/fields.pyi` & `vstutils-5.9.4/vstutils/models/fields.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/model.pyi` & `vstutils-5.9.4/vstutils/models/model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/queryset.py` & `vstutils-5.9.4/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/models/queryset.pyi` & `vstutils-5.9.4/vstutils/models/queryset.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/settings.ini` & `vstutils-5.9.4/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/settings.py` & `vstutils-5.9.4/vstutils/settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/281.chunk.js` & `vstutils-5.9.4/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/296.chunk.js` & `vstutils-5.9.4/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/345.chunk.js` & `vstutils-5.9.4/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/368.chunk.js` & `vstutils-5.9.4/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/408.js` & `vstutils-5.9.4/vstutils/static/bundle/408.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/421.js` & `vstutils-5.9.4/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.9.4/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/683.chunk.js` & `vstutils-5.9.4/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/686.js` & `vstutils-5.9.4/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/742.chunk.js` & `vstutils-5.9.4/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.9.4/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/755.js` & `vstutils-5.9.4/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/826.chunk.js` & `vstutils-5.9.4/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.9.4/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/844.js` & `vstutils-5.9.4/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/865.js` & `vstutils-5.9.4/vstutils/static/bundle/865.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/865.js.LICENSE.txt` & `vstutils-5.9.4/vstutils/static/bundle/865.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/app_loader.js` & `vstutils-5.9.4/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/base.js` & `vstutils-5.9.4/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.9.4/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.9.4/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/output.json` & `vstutils-5.9.4/vstutils/static/bundle/output.json`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/spa.js` & `vstutils-5.9.4/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/bundle/vstutils.js` & `vstutils-5.9.4/vstutils/static/bundle/vstutils.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static/img/anonymous.png` & `vstutils-5.9.4/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/static_files.py` & `vstutils-5.9.4/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/tasks.py` & `vstutils-5.9.4/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/tasks.pyi` & `vstutils-5.9.4/vstutils/tasks.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/auth/base.html` & `vstutils-5.9.4/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/auth/language_selector.html` & `vstutils-5.9.4/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/auth/tfa.html` & `vstutils-5.9.4/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/base.html` & `vstutils-5.9.4/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/gui/base.html` & `vstutils-5.9.4/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/gui/offline.html` & `vstutils-5.9.4/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/gui/service-worker.js` & `vstutils-5.9.4/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.9.4/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.9.4/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/package.json.template` & `vstutils-5.9.4/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.9.4/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/pyproject.toml.template` & `vstutils-5.9.4/vstutils/templates/newproject/pyproject.toml.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/setup.py.template` & `vstutils-5.9.4/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/test.py.template` & `vstutils-5.9.4/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.9.4/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.9.4/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.9.4/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/registration/confirm_email.html` & `vstutils-5.9.4/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.9.4/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.9.4/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/registration/user_registration.html` & `vstutils-5.9.4/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/rest_framework/admin.html` & `vstutils-5.9.4/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.9.4/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.9.4/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templatetags/request_static.py` & `vstutils-5.9.4/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templatetags/translation.py` & `vstutils-5.9.4/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.9.4/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.9.4/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/templatetags/vstconfigs.py` & `vstutils-5.9.4/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/tests.py` & `vstutils-5.9.4/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/tools.py` & `vstutils-5.9.4/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/translations/cn.py` & `vstutils-5.9.4/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/translations/ru.py` & `vstutils-5.9.4/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/translations/vi.py` & `vstutils-5.9.4/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/urls.py` & `vstutils-5.9.4/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/utils.py` & `vstutils-5.9.4/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/utils.pyi` & `vstutils-5.9.4/vstutils/utils.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/web.ini` & `vstutils-5.9.4/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/api.py` & `vstutils-5.9.4/vstutils/webpush/api.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/apps.py` & `vstutils-5.9.4/vstutils/webpush/apps.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/autodiscovery.py` & `vstutils-5.9.4/vstutils/webpush/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/base.py` & `vstutils-5.9.4/vstutils/webpush/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/migrations/0001_initial.py` & `vstutils-5.9.4/vstutils/webpush/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/models.py` & `vstutils-5.9.4/vstutils/webpush/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/templates/webpush/notification-handler.js` & `vstutils-5.9.4/vstutils/webpush/templates/webpush/notification-handler.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/test_utils.py` & `vstutils-5.9.4/vstutils/webpush/test_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/translations/ru.py` & `vstutils-5.9.4/vstutils/webpush/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/webpush/utils.py` & `vstutils-5.9.4/vstutils/webpush/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils/wsgi.py` & `vstutils-5.9.4/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils.egg-info/PKG-INFO` & `vstutils-5.9.4/vstutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.9.3
+Version: 5.9.4
 Summary: VST Utils Framework for fast create web-application
 Author-email: Sergei Kliuikov <sergey.k@vstconsulting.net>, Dmitriy Ovcharenko  <ovcharenkodd@gmail.com>
 Maintainer-email: VST Consulting <sergey.k@vstconsulting.net>
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source, https://gitlab.com/vstconsulting/vstutils
 Project-URL: Releases, https://pypi.org/project/vstutils/#history
```

### Comparing `vstutils-5.9.3/vstutils.egg-info/SOURCES.txt` & `vstutils-5.9.4/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.9.3/vstutils.egg-info/requires.txt` & `vstutils-5.9.4/vstutils.egg-info/requires.txt`

 * *Files identical despite different names*

