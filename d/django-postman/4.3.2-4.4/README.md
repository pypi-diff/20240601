# Comparing `tmp/django-postman-4.3.2.tar.gz` & `tmp/django_postman-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-postman-4.3.2.tar", last modified: Wed Jul 19 20:38:20 2023, max compression
+gzip compressed data, was "django_postman-4.4.tar", last modified: Sat Jun  1 16:30:57 2024, max compression
```

## Comparing `django-postman-4.3.2.tar` & `django_postman-4.4.tar`

### file list

```diff
@@ -1,193 +1,195 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.586575 django-postman-4.3.2/
--rw-rw-rw-   0        0        0     8914 2023-07-19 19:55:51.000000 django-postman-4.3.2/CHANGELOG
--rw-rw-rw-   0        0        0     1533 2020-06-29 17:45:15.000000 django-postman-4.3.2/LICENSE
--rw-rw-rw-   0        0        0      181 2020-06-29 17:45:15.000000 django-postman-4.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4223 2023-07-19 20:38:20.586575 django-postman-4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2020-06-29 17:45:15.000000 django-postman-4.3.2/README
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.367537 django-postman-4.3.2/django_postman.egg-info/
--rw-rw-rw-   0        0        0     4223 2023-07-19 20:38:20.000000 django-postman-4.3.2/django_postman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4533 2023-07-19 20:38:20.000000 django-postman-4.3.2/django_postman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 20:38:20.000000 django-postman-4.3.2/django_postman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 20:38:20.000000 django-postman-4.3.2/django_postman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-19 20:38:20.000000 django-postman-4.3.2/django_postman.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.398787 django-postman-4.3.2/docs/
--rw-rw-rw-   0        0        0     3142 2020-06-29 17:45:15.000000 django-postman-4.3.2/docs/Makefile
--rw-rw-rw-   0        0        0     2674 2021-03-01 17:41:11.000000 django-postman-4.3.2/docs/api.rst
--rw-rw-rw-   0        0        0     6528 2023-07-17 18:20:47.000000 django-postman-4.3.2/docs/conf.py
--rw-rw-rw-   0        0        0      612 2020-06-29 17:45:15.000000 django-postman-4.3.2/docs/faq.rst
--rw-rw-rw-   0        0        0    10494 2021-03-07 17:39:01.000000 django-postman-4.3.2/docs/features.rst
--rw-rw-rw-   0        0        0     4453 2023-07-05 12:13:55.000000 django-postman-4.3.2/docs/index.rst
--rwxrwxrwx   0        0        0     3200 2020-06-29 17:45:15.000000 django-postman-4.3.2/docs/make.bat
--rw-rw-rw-   0        0        0     1614 2020-06-29 17:45:15.000000 django-postman-4.3.2/docs/management.rst
--rw-rw-rw-   0        0        0     2973 2020-06-29 17:45:15.000000 django-postman-4.3.2/docs/moderation.rst
--rw-rw-rw-   0        0        0     2320 2020-06-29 17:45:15.000000 django-postman-4.3.2/docs/notification.rst
--rw-rw-rw-   0        0        0    14750 2022-08-01 18:15:41.000000 django-postman-4.3.2/docs/quickstart.rst
--rw-rw-rw-   0        0        0     3106 2020-06-29 17:45:15.000000 django-postman-4.3.2/docs/tags-filters.rst
--rw-rw-rw-   0        0        0     3872 2020-06-29 17:45:15.000000 django-postman-4.3.2/docs/views.rst
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.429923 django-postman-4.3.2/postman/
--rw-rw-rw-   0        0        0      514 2023-07-17 18:20:51.000000 django-postman-4.3.2/postman/__init__.py
--rw-rw-rw-   0        0        0     7409 2020-07-16 19:42:04.000000 django-postman-4.3.2/postman/admin.py
--rw-rw-rw-   0        0        0     3486 2023-07-12 15:02:50.000000 django-postman-4.3.2/postman/api.py
--rw-rw-rw-   0        0        0      515 2021-03-01 16:41:06.000000 django-postman-4.3.2/postman/api_urls.py
--rw-rw-rw-   0        0        0     1175 2021-03-03 17:07:11.000000 django-postman-4.3.2/postman/api_views.py
--rw-rw-rw-   0        0        0     1291 2023-07-17 16:54:56.000000 django-postman-4.3.2/postman/apps.py
--rw-rw-rw-   0        0        0      360 2022-10-18 16:34:08.000000 django-postman-4.3.2/postman/context_processors.py
--rw-rw-rw-   0        0        0     5539 2020-07-16 19:43:29.000000 django-postman-4.3.2/postman/fields.py
--rw-rw-rw-   0        0        0     8874 2020-07-16 19:45:03.000000 django-postman-4.3.2/postman/forms.py
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.329773 django-postman-4.3.2/postman/locale/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/ar/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.429923 django-postman-4.3.2/postman/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0        0        0     5182 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/ar/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    15300 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/ar/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/cs/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.429923 django-postman-4.3.2/postman/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2233 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/cs/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    13646 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/cs/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/da/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.429923 django-postman-4.3.2/postman/locale/da/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2232 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/da/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    13466 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/da/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/de/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.445559 django-postman-4.3.2/postman/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9857 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16776 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/el/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.445559 django-postman-4.3.2/postman/locale/el/LC_MESSAGES/
--rw-rw-rw-   0        0        0    12781 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/el/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    19740 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/el/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/en/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.445559 django-postman-4.3.2/postman/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      367 2016-11-01 10:23:16.000000 django-postman-4.3.2/postman/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12890 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/eo/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.445559 django-postman-4.3.2/postman/locale/eo/LC_MESSAGES/
--rw-rw-rw-   0        0        0    10997 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/eo/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16827 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/eo/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/es/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.445559 django-postman-4.3.2/postman/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9676 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16629 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/fa_IR/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.461179 django-postman-4.3.2/postman/locale/fa_IR/LC_MESSAGES/
--rw-rw-rw-   0        0        0    11104 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/fa_IR/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    17998 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/fa_IR/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.461179 django-postman-4.3.2/postman/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    11266 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    17123 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/fr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.304641 django-postman-4.3.2/postman/locale/hu/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.461179 django-postman-4.3.2/postman/locale/hu/LC_MESSAGES/
--rw-rw-rw-   0        0        0    11314 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/hu/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16472 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/hu/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/it/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.461179 django-postman-4.3.2/postman/locale/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0     8918 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/it/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16272 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/it/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/ka/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.476806 django-postman-4.3.2/postman/locale/ka/LC_MESSAGES/
--rw-rw-rw-   0        0        0    11562 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/ka/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    19119 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/ka/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/lv/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.476806 django-postman-4.3.2/postman/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9539 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/lv/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16413 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/lv/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/nl/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.476806 django-postman-4.3.2/postman/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     4943 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    14626 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/pl/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.476806 django-postman-4.3.2/postman/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0        0        0    10026 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/pl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    17081 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/pl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/pt_BR/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.476806 django-postman-4.3.2/postman/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9642 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16551 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/ru/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.492430 django-postman-4.3.2/postman/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0        0        0    12201 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    19127 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/ru/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/sl_SI/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.492430 django-postman-4.3.2/postman/locale/sl_SI/LC_MESSAGES/
--rw-rw-rw-   0        0        0     4269 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/sl_SI/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    13779 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/sl_SI/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/th_TH/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.492430 django-postman-4.3.2/postman/locale/th_TH/LC_MESSAGES/
--rw-rw-rw-   0        0        0    13518 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/th_TH/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    20335 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/th_TH/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.320267 django-postman-4.3.2/postman/locale/tr/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.492430 django-postman-4.3.2/postman/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9587 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/tr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16575 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/tr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.329773 django-postman-4.3.2/postman/locale/zh_CN/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.508057 django-postman-4.3.2/postman/locale/zh_CN/LC_MESSAGES/
--rw-rw-rw-   0        0        0     8919 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/zh_CN/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    15718 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/zh_CN/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.329773 django-postman-4.3.2/postman/locale/zh_TW/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.508057 django-postman-4.3.2/postman/locale/zh_TW/LC_MESSAGES/
--rw-rw-rw-   0        0        0     8869 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/zh_TW/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    15705 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/locale/zh_TW/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.508057 django-postman-4.3.2/postman/management/
--rw-rw-rw-   0        0        0        0 2020-07-10 19:46:56.000000 django-postman-4.3.2/postman/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.508057 django-postman-4.3.2/postman/management/commands/
--rw-rw-rw-   0        0        0        0 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/management/commands/__init__.py
--rw-rw-rw-   0        0        0     3675 2020-07-16 11:50:15.000000 django-postman-4.3.2/postman/management/commands/postman_checkup.py
--rw-rw-rw-   0        0        0     1887 2020-07-14 20:47:20.000000 django-postman-4.3.2/postman/management/commands/postman_cleanup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.508057 django-postman-4.3.2/postman/migrations/
--rw-rw-rw-   0        0        0     3524 2020-07-14 20:47:20.000000 django-postman-4.3.2/postman/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/migrations/__init__.py
--rw-rw-rw-   0        0        0    22894 2023-07-17 16:55:00.000000 django-postman-4.3.2/postman/models.py
--rw-rw-rw-   0        0        0     1478 2022-08-01 17:05:11.000000 django-postman-4.3.2/postman/module_for_tests.py
--rw-rw-rw-   0        0        0     4441 2023-07-17 16:15:33.000000 django-postman-4.3.2/postman/query.py
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.329773 django-postman-4.3.2/postman/static/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.329773 django-postman-4.3.2/postman/static/postman/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.523682 django-postman-4.3.2/postman/static/postman/css/
--rw-rw-rw-   0        0        0      126 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/static/postman/css/admin.css
--rw-rw-rw-   0        0        0      544 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/static/postman/css/postman.css
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.530187 django-postman-4.3.2/postman/templates/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.329773 django-postman-4.3.2/postman/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.329773 django-postman-4.3.2/postman/templates/admin/postman/
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.539694 django-postman-4.3.2/postman/templates/admin/postman/pendingmessage/
--rw-rw-rw-   0        0        0     1698 2020-07-17 09:23:27.000000 django-postman-4.3.2/postman/templates/admin/postman/pendingmessage/change_form.html
--rw-rw-rw-   0        0        0      331 2020-07-17 09:21:34.000000 django-postman-4.3.2/postman/templates/admin/postman/pendingmessage/submit_line.html
--rw-rw-rw-   0        0        0      962 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/autocomplete_postman_multiple_as1-1.html
--rw-rw-rw-   0        0        0     1602 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/autocomplete_postman_multiple_as1-2.html
--rw-rw-rw-   0        0        0     2886 2020-07-17 09:18:35.000000 django-postman-4.3.2/postman/templates/autocomplete_postman_multiple_as1-3.html
--rw-rw-rw-   0        0        0      812 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/autocomplete_postman_single_as1-1.html
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.555325 django-postman-4.3.2/postman/templates/postman/
--rw-rw-rw-   0        0        0      375 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/archives.html
--rw-rw-rw-   0        0        0      942 2020-07-17 09:30:45.000000 django-postman-4.3.2/postman/templates/postman/base.html
--rw-rw-rw-   0        0        0     4084 2020-07-17 09:27:57.000000 django-postman-4.3.2/postman/templates/postman/base_folder.html
--rw-rw-rw-   0        0        0      811 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/base_write.html
--rw-rw-rw-   0        0        0     1464 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/email_user.txt
--rw-rw-rw-   0        0        0      196 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/email_user_subject.txt
--rw-rw-rw-   0        0        0     1324 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/email_visitor.txt
--rw-rw-rw-   0        0        0      196 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/email_visitor_subject.txt
--rw-rw-rw-   0        0        0      321 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/inbox.html
--rw-rw-rw-   0        0        0     1185 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/inc_subject_ex.html
--rw-rw-rw-   0        0        0      240 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/reply.html
--rw-rw-rw-   0        0        0      391 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/sent.html
--rw-rw-rw-   0        0        0      491 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/trash.html
--rw-rw-rw-   0        0        0     2589 2020-07-17 09:34:13.000000 django-postman-4.3.2/postman/templates/postman/view.html
--rw-rw-rw-   0        0        0      114 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman/write.html
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.570960 django-postman-4.3.2/postman/templates/postman_for_tests/
--rw-rw-rw-   0        0        0       26 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman_for_tests/context_processors.html
--rw-rw-rw-   0        0        0       60 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman_for_tests/email_html_and_empty_txt.html
--rw-rw-rw-   0        0        0        0 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman_for_tests/email_html_and_empty_txt.txt
--rw-rw-rw-   0        0        0       54 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman_for_tests/email_html_and_txt.html
--rw-rw-rw-   0        0        0       83 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman_for_tests/email_html_and_txt.txt
--rw-rw-rw-   0        0        0       50 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman_for_tests/email_html_only.html
--rw-rw-rw-   0        0        0       78 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templates/postman_for_tests/email_txt_only.txt
-drwxrwxrwx   0        0        0        0 2023-07-19 20:38:20.586575 django-postman-4.3.2/postman/templatetags/
--rw-rw-rw-   0        0        0        0 2020-06-29 17:45:15.000000 django-postman-4.3.2/postman/templatetags/__init__.py
--rw-rw-rw-   0        0        0      928 2020-07-14 20:47:20.000000 django-postman-4.3.2/postman/templatetags/pagination_tags.py
--rw-rw-rw-   0        0        0      391 2020-07-14 20:47:20.000000 django-postman-4.3.2/postman/templatetags/postman_admin_modify.py
--rw-rw-rw-   0        0        0     4846 2023-07-12 16:46:14.000000 django-postman-4.3.2/postman/templatetags/postman_tags.py
--rw-rw-rw-   0        0        0   121942 2023-07-17 18:22:28.000000 django-postman-4.3.2/postman/tests.py
--rw-rw-rw-   0        0        0     5544 2021-03-01 17:00:27.000000 django-postman-4.3.2/postman/urls.py
--rw-rw-rw-   0        0        0    10321 2021-03-01 16:57:51.000000 django-postman-4.3.2/postman/urls_for_tests.py
--rw-rw-rw-   0        0        0     8918 2022-08-01 18:15:54.000000 django-postman-4.3.2/postman/utils.py
--rw-rw-rw-   0        0        0    18327 2021-03-07 17:55:16.000000 django-postman-4.3.2/postman/views.py
--rw-rw-rw-   0        0        0     1286 2023-07-19 20:36:57.000000 django-postman-4.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-19 20:38:20.586575 django-postman-4.3.2/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-07-19 19:47:32.000000 django-postman-4.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:57.221836 django_postman-4.4/
+-rw-rw-rw-   0        0        0     9022 2024-05-30 17:36:19.000000 django_postman-4.4/CHANGELOG
+-rw-rw-rw-   0        0        0     1533 2020-06-29 17:45:15.000000 django_postman-4.4/LICENSE
+-rw-rw-rw-   0        0        0      181 2020-06-29 17:45:15.000000 django_postman-4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4244 2024-06-01 16:30:57.218838 django_postman-4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2020-06-29 17:45:15.000000 django_postman-4.4/README
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:57.217835 django_postman-4.4/django_postman.egg-info/
+-rw-rw-rw-   0        0        0     4244 2024-06-01 16:30:55.000000 django_postman-4.4/django_postman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4609 2024-06-01 16:30:56.000000 django_postman-4.4/django_postman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 16:30:55.000000 django_postman-4.4/django_postman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 16:30:55.000000 django_postman-4.4/django_postman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 16:30:55.000000 django_postman-4.4/django_postman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.367578 django_postman-4.4/docs/
+-rw-rw-rw-   0        0        0     3142 2020-06-29 17:45:15.000000 django_postman-4.4/docs/Makefile
+-rw-rw-rw-   0        0        0     2674 2021-03-01 17:41:11.000000 django_postman-4.4/docs/api.rst
+-rw-rw-rw-   0        0        0     6632 2024-05-31 19:41:33.000000 django_postman-4.4/docs/conf.py
+-rw-rw-rw-   0        0        0      612 2020-06-29 17:45:15.000000 django_postman-4.4/docs/faq.rst
+-rw-rw-rw-   0        0        0    10494 2021-03-07 17:39:01.000000 django_postman-4.4/docs/features.rst
+-rw-rw-rw-   0        0        0     4453 2023-07-05 12:13:55.000000 django_postman-4.4/docs/index.rst
+-rwxrwxrwx   0        0        0     3200 2020-06-29 17:45:15.000000 django_postman-4.4/docs/make.bat
+-rw-rw-rw-   0        0        0     1614 2020-06-29 17:45:15.000000 django_postman-4.4/docs/management.rst
+-rw-rw-rw-   0        0        0     2973 2020-06-29 17:45:15.000000 django_postman-4.4/docs/moderation.rst
+-rw-rw-rw-   0        0        0     2320 2020-06-29 17:45:15.000000 django_postman-4.4/docs/notification.rst
+-rw-rw-rw-   0        0        0    15899 2024-05-31 18:26:27.000000 django_postman-4.4/docs/quickstart.rst
+-rw-rw-rw-   0        0        0       30 2024-04-24 20:04:57.000000 django_postman-4.4/docs/requirements.txt
+-rw-rw-rw-   0        0        0     3106 2020-06-29 17:45:15.000000 django_postman-4.4/docs/tags-filters.rst
+-rw-rw-rw-   0        0        0     3872 2020-06-29 17:45:15.000000 django_postman-4.4/docs/views.rst
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.502585 django_postman-4.4/postman/
+-rw-rw-rw-   0        0        0      511 2024-05-31 19:41:35.000000 django_postman-4.4/postman/__init__.py
+-rw-rw-rw-   0        0        0     7409 2020-07-16 19:42:04.000000 django_postman-4.4/postman/admin.py
+-rw-rw-rw-   0        0        0     3486 2023-07-12 15:02:50.000000 django_postman-4.4/postman/api.py
+-rw-rw-rw-   0        0        0      515 2021-03-01 16:41:06.000000 django_postman-4.4/postman/api_urls.py
+-rw-rw-rw-   0        0        0     1175 2021-03-03 17:07:11.000000 django_postman-4.4/postman/api_views.py
+-rw-rw-rw-   0        0        0     1291 2023-07-17 16:54:56.000000 django_postman-4.4/postman/apps.py
+-rw-rw-rw-   0        0        0      360 2022-10-18 16:34:08.000000 django_postman-4.4/postman/context_processors.py
+-rw-rw-rw-   0        0        0     5539 2020-07-16 19:43:29.000000 django_postman-4.4/postman/fields.py
+-rw-rw-rw-   0        0        0     8874 2020-07-16 19:45:03.000000 django_postman-4.4/postman/forms.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.149858 django_postman-4.4/postman/locale/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.110015 django_postman-4.4/postman/locale/ar/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.519838 django_postman-4.4/postman/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5182 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    15300 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/ar/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.111017 django_postman-4.4/postman/locale/cs/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.534857 django_postman-4.4/postman/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2233 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    13646 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/cs/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.112015 django_postman-4.4/postman/locale/da/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.552887 django_postman-4.4/postman/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2232 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/da/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    13466 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/da/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.115451 django_postman-4.4/postman/locale/de/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.569409 django_postman-4.4/postman/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9857 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16776 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.116456 django_postman-4.4/postman/locale/el/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.585462 django_postman-4.4/postman/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    12781 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/el/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    19740 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/el/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.117450 django_postman-4.4/postman/locale/en/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.602974 django_postman-4.4/postman/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      367 2016-11-01 10:23:16.000000 django_postman-4.4/postman/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12890 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.118479 django_postman-4.4/postman/locale/eo/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.621007 django_postman-4.4/postman/locale/eo/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    10997 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/eo/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16827 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/eo/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.125023 django_postman-4.4/postman/locale/es/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.637672 django_postman-4.4/postman/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9676 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16629 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.127027 django_postman-4.4/postman/locale/fa_IR/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.654719 django_postman-4.4/postman/locale/fa_IR/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    11104 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    17998 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/fa_IR/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.128027 django_postman-4.4/postman/locale/fr/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.671237 django_postman-4.4/postman/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    11266 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    17123 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.131024 django_postman-4.4/postman/locale/hu/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.687763 django_postman-4.4/postman/locale/hu/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    11314 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16472 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/hu/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.132535 django_postman-4.4/postman/locale/it/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.703579 django_postman-4.4/postman/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     8918 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/it/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16272 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/it/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.134549 django_postman-4.4/postman/locale/ka/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.720099 django_postman-4.4/postman/locale/ka/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    11562 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/ka/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    19119 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/ka/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.136571 django_postman-4.4/postman/locale/lv/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.735129 django_postman-4.4/postman/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9539 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/lv/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16413 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/lv/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.138557 django_postman-4.4/postman/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.753174 django_postman-4.4/postman/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     4943 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    14626 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.139564 django_postman-4.4/postman/locale/pl/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.768691 django_postman-4.4/postman/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    10026 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    17081 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/pl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.141558 django_postman-4.4/postman/locale/pt_BR/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.785996 django_postman-4.4/postman/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9642 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16551 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.142560 django_postman-4.4/postman/locale/ru/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.801472 django_postman-4.4/postman/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    12201 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    19127 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/ru/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.143864 django_postman-4.4/postman/locale/sl_SI/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.819520 django_postman-4.4/postman/locale/sl_SI/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     4269 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    13779 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/sl_SI/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.145857 django_postman-4.4/postman/locale/th_TH/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.836558 django_postman-4.4/postman/locale/th_TH/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    13518 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/th_TH/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    20335 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/th_TH/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.147867 django_postman-4.4/postman/locale/tr/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.853074 django_postman-4.4/postman/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9587 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16575 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/tr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.148860 django_postman-4.4/postman/locale/zh_CN/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.870818 django_postman-4.4/postman/locale/zh_CN/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     8919 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    15718 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/zh_CN/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.150857 django_postman-4.4/postman/locale/zh_TW/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.888275 django_postman-4.4/postman/locale/zh_TW/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     8869 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    15705 2020-06-29 17:45:15.000000 django_postman-4.4/postman/locale/zh_TW/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.890264 django_postman-4.4/postman/management/
+-rw-rw-rw-   0        0        0        0 2020-07-10 19:46:56.000000 django_postman-4.4/postman/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.912032 django_postman-4.4/postman/management/commands/
+-rw-rw-rw-   0        0        0        0 2020-06-29 17:45:15.000000 django_postman-4.4/postman/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     3675 2020-07-16 11:50:15.000000 django_postman-4.4/postman/management/commands/postman_checkup.py
+-rw-rw-rw-   0        0        0     1887 2020-07-14 20:47:20.000000 django_postman-4.4/postman/management/commands/postman_cleanup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.925055 django_postman-4.4/postman/migrations/
+-rw-rw-rw-   0        0        0     3524 2020-07-14 20:47:20.000000 django_postman-4.4/postman/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2020-06-29 17:45:15.000000 django_postman-4.4/postman/migrations/__init__.py
+-rw-rw-rw-   0        0        0    22894 2023-07-17 16:55:00.000000 django_postman-4.4/postman/models.py
+-rw-rw-rw-   0        0        0     1764 2024-05-30 20:56:53.000000 django_postman-4.4/postman/module_for_tests.py
+-rw-rw-rw-   0        0        0     4441 2023-07-17 16:15:33.000000 django_postman-4.4/postman/query.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.155889 django_postman-4.4/postman/static/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.155889 django_postman-4.4/postman/static/postman/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.937595 django_postman-4.4/postman/static/postman/css/
+-rw-rw-rw-   0        0        0      126 2020-06-29 17:45:15.000000 django_postman-4.4/postman/static/postman/css/admin.css
+-rw-rw-rw-   0        0        0      544 2020-06-29 17:45:15.000000 django_postman-4.4/postman/static/postman/css/postman.css
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.992808 django_postman-4.4/postman/templates/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.157887 django_postman-4.4/postman/templates/admin/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:56.158890 django_postman-4.4/postman/templates/admin/postman/
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:57.015850 django_postman-4.4/postman/templates/admin/postman/pendingmessage/
+-rw-rw-rw-   0        0        0     1698 2020-07-17 09:23:27.000000 django_postman-4.4/postman/templates/admin/postman/pendingmessage/change_form.html
+-rw-rw-rw-   0        0        0      331 2020-07-17 09:21:34.000000 django_postman-4.4/postman/templates/admin/postman/pendingmessage/submit_line.html
+-rw-rw-rw-   0        0        0      962 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/autocomplete_postman_multiple_as1-1.html
+-rw-rw-rw-   0        0        0     1602 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/autocomplete_postman_multiple_as1-2.html
+-rw-rw-rw-   0        0        0     2886 2020-07-17 09:18:35.000000 django_postman-4.4/postman/templates/autocomplete_postman_multiple_as1-3.html
+-rw-rw-rw-   0        0        0      812 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/autocomplete_postman_single_as1-1.html
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:57.126978 django_postman-4.4/postman/templates/postman/
+-rw-rw-rw-   0        0        0      375 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/archives.html
+-rw-rw-rw-   0        0        0      942 2020-07-17 09:30:45.000000 django_postman-4.4/postman/templates/postman/base.html
+-rw-rw-rw-   0        0        0     4084 2020-07-17 09:27:57.000000 django_postman-4.4/postman/templates/postman/base_folder.html
+-rw-rw-rw-   0        0        0      811 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/base_write.html
+-rw-rw-rw-   0        0        0     1464 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/email_user.txt
+-rw-rw-rw-   0        0        0      196 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/email_user_subject.txt
+-rw-rw-rw-   0        0        0     1324 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/email_visitor.txt
+-rw-rw-rw-   0        0        0      196 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/email_visitor_subject.txt
+-rw-rw-rw-   0        0        0      321 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/inbox.html
+-rw-rw-rw-   0        0        0     1185 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/inc_subject_ex.html
+-rw-rw-rw-   0        0        0      240 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/reply.html
+-rw-rw-rw-   0        0        0      391 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/sent.html
+-rw-rw-rw-   0        0        0      491 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/trash.html
+-rw-rw-rw-   0        0        0     2589 2020-07-17 09:34:13.000000 django_postman-4.4/postman/templates/postman/view.html
+-rw-rw-rw-   0        0        0      114 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman/write.html
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:57.183093 django_postman-4.4/postman/templates/postman_for_tests/
+-rw-rw-rw-   0        0        0       26 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman_for_tests/context_processors.html
+-rw-rw-rw-   0        0        0       60 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman_for_tests/email_html_and_empty_txt.html
+-rw-rw-rw-   0        0        0        0 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman_for_tests/email_html_and_empty_txt.txt
+-rw-rw-rw-   0        0        0       54 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman_for_tests/email_html_and_txt.html
+-rw-rw-rw-   0        0        0       83 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman_for_tests/email_html_and_txt.txt
+-rw-rw-rw-   0        0        0       50 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman_for_tests/email_html_only.html
+-rw-rw-rw-   0        0        0       15 2024-05-30 20:55:43.000000 django_postman-4.4/postman/templates/postman_for_tests/email_subject.txt
+-rw-rw-rw-   0        0        0       78 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templates/postman_for_tests/email_txt_only.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 16:30:57.214835 django_postman-4.4/postman/templatetags/
+-rw-rw-rw-   0        0        0        0 2020-06-29 17:45:15.000000 django_postman-4.4/postman/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      928 2020-07-14 20:47:20.000000 django_postman-4.4/postman/templatetags/pagination_tags.py
+-rw-rw-rw-   0        0        0      391 2020-07-14 20:47:20.000000 django_postman-4.4/postman/templatetags/postman_admin_modify.py
+-rw-rw-rw-   0        0        0     4846 2023-07-12 16:46:14.000000 django_postman-4.4/postman/templatetags/postman_tags.py
+-rw-rw-rw-   0        0        0   122812 2024-05-31 19:41:20.000000 django_postman-4.4/postman/tests.py
+-rw-rw-rw-   0        0        0     5544 2021-03-01 17:00:27.000000 django_postman-4.4/postman/urls.py
+-rw-rw-rw-   0        0        0    10321 2021-03-01 16:57:51.000000 django_postman-4.4/postman/urls_for_tests.py
+-rw-rw-rw-   0        0        0     9275 2024-05-30 17:08:23.000000 django_postman-4.4/postman/utils.py
+-rw-rw-rw-   0        0        0    18327 2021-03-07 17:55:16.000000 django_postman-4.4/postman/views.py
+-rw-rw-rw-   0        0        0     1286 2023-07-19 20:36:57.000000 django_postman-4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 16:30:57.221836 django_postman-4.4/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-07-19 19:47:32.000000 django_postman-4.4/setup.py
```

### Comparing `django-postman-4.3.2/CHANGELOG` & `django_postman-4.4/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ========================
 Django Postman changelog
 ========================
 
+Version 4.4, June 2024
+----------------------
+* Added a setting: POSTMAN_CONTEXT_EMAIL (enhancement #131).
+
 Version 4.3.2, July 2023
 ------------------------
 * Fixed issue #128, (doc only) Transifex web application's domain change.
 * Fixed issue #129, a django.contrib.sites detection adjustment, for Django 4.
 * Forced postman_unread tag to return a string in all cases, required for Django 4.
 * Fixed the sql compiler for getting by-conversation messages, for Django 4.
 * Set explicitly default_auto_field to AutoField, introduced in Django 3.2.
```

### Comparing `django-postman-4.3.2/LICENSE` & `django_postman-4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/PKG-INFO` & `django_postman-4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postman
-Version: 4.3.2
+Version: 4.4
 Summary: User-to-User messaging system for Django, with gateway to AnonymousUser, moderation and thread management, user & exchange filters, inbox/sent/archives/trash folders, support for apps: auto-complete, notification, mailer.
 Author-email: Patrick Samson <maxcom@laposte.net>
 License: Copyright (c) 2010, Patrick Samson.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -41,14 +41,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Communications :: Email
 Description-Content-Type: text/plain
 License-File: LICENSE
+Requires-Dist: Django
 
 ==============
 Django Postman
 ==============
 
 This is an application for the Django web framework.
```

### Comparing `django-postman-4.3.2/README` & `django_postman-4.4/README`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/django_postman.egg-info/PKG-INFO` & `django_postman-4.4/django_postman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-postman
-Version: 4.3.2
+Version: 4.4
 Summary: User-to-User messaging system for Django, with gateway to AnonymousUser, moderation and thread management, user & exchange filters, inbox/sent/archives/trash folders, support for apps: auto-complete, notification, mailer.
 Author-email: Patrick Samson <maxcom@laposte.net>
 License: Copyright (c) 2010, Patrick Samson.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -41,14 +41,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Communications :: Email
 Description-Content-Type: text/plain
 License-File: LICENSE
+Requires-Dist: Django
 
 ==============
 Django Postman
 ==============
 
 This is an application for the Django web framework.
```

### Comparing `django-postman-4.3.2/django_postman.egg-info/SOURCES.txt` & `django_postman-4.4/django_postman.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/features.rst
 docs/index.rst
 docs/make.bat
 docs/management.rst
 docs/moderation.rst
 docs/notification.rst
 docs/quickstart.rst
+docs/requirements.txt
 docs/tags-filters.rst
 docs/views.rst
 postman/__init__.py
 postman/admin.py
 postman/api.py
 postman/api_urls.py
 postman/api_views.py
@@ -116,12 +117,13 @@
 postman/templates/postman/write.html
 postman/templates/postman_for_tests/context_processors.html
 postman/templates/postman_for_tests/email_html_and_empty_txt.html
 postman/templates/postman_for_tests/email_html_and_empty_txt.txt
 postman/templates/postman_for_tests/email_html_and_txt.html
 postman/templates/postman_for_tests/email_html_and_txt.txt
 postman/templates/postman_for_tests/email_html_only.html
+postman/templates/postman_for_tests/email_subject.txt
 postman/templates/postman_for_tests/email_txt_only.txt
 postman/templatetags/__init__.py
 postman/templatetags/pagination_tags.py
 postman/templatetags/postman_admin_modify.py
 postman/templatetags/postman_tags.py
```

### Comparing `django-postman-4.3.2/docs/Makefile` & `django_postman-4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/api.rst` & `django_postman-4.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/conf.py` & `django_postman-4.4/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,68 +7,69 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys, os
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
+# import sys, os
 #sys.path.append(os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = []
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+# templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
 #source_encoding = 'utf-8'
 
 # The master toctree document.
-master_doc = 'index'
+# root_doc = 'index'
 
 # General information about the project.
-project = u'django-postman'
-copyright = u'2010, Patrick Samson'
+project = 'django-postman'
+copyright = '2010, Patrick Samson'
+author = 'Patrick Samson'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '4.3'
+version = '4.4'
 # The full version, including alpha/beta/rc tags.
-release = '4.3.2'
+release = '4.4'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
 
 # List of documents that shouldn't be included in the build.
 #unused_docs = []
 
-# List of directories, relative to source directory, that shouldn't be searched
-# for source files.
-exclude_trees = ['_build']
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# These patterns also affect html_static_path and html_extra_path
+exclude_patterns = ['_build']
 
 # The reST default role (used for this markup: `text`) to use for all documents.
 #default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 #add_function_parentheses = True
 
@@ -77,25 +78,25 @@
 #add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 #show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+# pygments_style = 'sphinx'
 
 # A list of ignored prefixes for module index sorting.
 #modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
-# The theme to use for HTML and HTML Help pages.  Major themes that come with
-# Sphinx are currently 'default' and 'sphinxdoc'.
-html_theme = 'alabaster'
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+html_theme = 'furo'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
@@ -116,15 +117,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 #html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 #html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
@@ -167,18 +168,18 @@
 #latex_paper_size = 'letter'
 
 # The font size ('10pt', '11pt' or '12pt').
 #latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
-latex_documents = [
-  ('index', 'django-postman.tex', u'django-postman Documentation',
-   u'Patrick Samson', 'manual'),
-]
+# latex_documents = [
+  # ('index', 'django-postman.tex', u'django-postman Documentation',
+   # u'Patrick Samson', 'manual'),
+# ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
```

### Comparing `django-postman-4.3.2/docs/faq.rst` & `django_postman-4.4/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/features.rst` & `django_postman-4.4/docs/features.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/index.rst` & `django_postman-4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/make.bat` & `django_postman-4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/management.rst` & `django_postman-4.4/docs/management.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/moderation.rst` & `django_postman-4.4/docs/moderation.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/notification.rst` & `django_postman-4.4/docs/notification.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/quickstart.rst` & `django_postman-4.4/docs/quickstart.rst`

 * *Files 6% similar despite different names*

```diff
@@ -129,26 +129,49 @@
             #...
             def notification_approval(self, action, site):
                 return True if self.is_active else 'support@mydom.com'
 
     Note: The ``POSTMAN_DISABLE_USER_EMAILING`` setting is kept for backward compatibility, but the same effect can be obtained
     with ``POSTMAN_NOTIFICATION_APPROVAL = False``.
 
+``POSTMAN_CONTEXT_EMAIL``
+    *New in version 4.4.*
+
+    You can extend the context used to build the parts of emails (template renderings, from, sending params).
+    The value can be specified as:
+
+    * A function.
+    * The full path to a function, as a string, whose import will be deferred. For example: 'myapp.mymodule.myfunc'.
+
+    In both cases, the function receives one parameter: a dictionary with the default context variables
+    as stated in section :ref:`for_visitors`, that is: {'site': ..., 'object': ..., 'action': ...}.
+    The return must be a dictionary. It can be the given parameter or a new copy, with existing entries left and yours added.
+
+    *Defaults to*: None ; meaning the context will stay with the default entries.
+
+    Example::
+
+        def get_context_email(context):
+            context['my_key'] = 'my-value'
+            return context
+        POSTMAN_CONTEXT_EMAIL = get_context_email  # default is None
+
 ``POSTMAN_FROM_EMAIL``
     *New in version 3.6.0.*
 
     Set it if you want to override the default 'from' field value.
     The value can be specified as:
 
     * An explicit string.
     * (*New in version 4.3*) A function.
     * (*New in version 4.3*) The full path to a function, as a string, whose import will be deferred. For example: 'myapp.mymodule.myfunc'.
 
-    In both cases, the function receives one parameter: a dictionary with the same context variables
+    The function receives one parameter: a dictionary with the same context variables
     as for the subject and body template rendering: {'site': ..., 'object': ..., 'action': ...}.
+    (*New in version 4.4*) This dictionary may be extended by the ``POSTMAN_CONTEXT_EMAIL`` hook.
     The return must be a string.
 
     *Defaults to*: DEFAULT_FROM_EMAIL.
 
     Example::
 
         def get_from_email(context):
@@ -162,14 +185,15 @@
     The value can be specified as:
 
     * A function.
     * (*New in version 4.3*) The full path to a function, as a string, whose import will be deferred. For example: 'myapp.mymodule.myfunc'.
 
     In both cases, the function receives one parameter: a dictionary with the same context variables
     as for the subject and body template rendering: {'site': ..., 'object': ..., 'action': ...}.
+    (*New in version 4.4*) This dictionary may be extended by the ``POSTMAN_CONTEXT_EMAIL`` hook.
     The return must be a dictionary, possibly empty, with django.core.mail.EmailMessage parameters as keys.
 
     *Defaults to*: None.
 
     Example::
 
         def get_params_email(context):
```

### Comparing `django-postman-4.3.2/docs/tags-filters.rst` & `django_postman-4.4/docs/tags-filters.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/docs/views.rst` & `django_postman-4.4/docs/views.rst`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/admin.py` & `django_postman-4.4/postman/admin.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/api.py` & `django_postman-4.4/postman/api.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/api_urls.py` & `django_postman-4.4/postman/api_urls.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/api_views.py` & `django_postman-4.4/postman/api_views.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/apps.py` & `django_postman-4.4/postman/apps.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/fields.py` & `django_postman-4.4/postman/fields.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/forms.py` & `django_postman-4.4/postman/forms.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/ar/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/ar/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/cs/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/cs/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/da/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/da/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/de/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/de/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/el/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/el/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/en/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/eo/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/eo/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/es/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/es/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/fa_IR/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/fa_IR/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/fr/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/fr/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/hu/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/hu/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/it/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/it/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/ka/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/ka/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/ka/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/lv/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/lv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/lv/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/nl/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/nl/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/pl/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/pl/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/pt_BR/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/pt_BR/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/ru/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/ru/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/sl_SI/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/sl_SI/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/th_TH/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/th_TH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/th_TH/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/tr/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/tr/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/zh_CN/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/zh_CN/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/zh_TW/LC_MESSAGES/django.mo` & `django_postman-4.4/postman/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/locale/zh_TW/LC_MESSAGES/django.po` & `django_postman-4.4/postman/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/management/commands/postman_checkup.py` & `django_postman-4.4/postman/management/commands/postman_checkup.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/management/commands/postman_cleanup.py` & `django_postman-4.4/postman/management/commands/postman_cleanup.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/migrations/0001_initial.py` & `django_postman-4.4/postman/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/models.py` & `django_postman-4.4/postman/models.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/module_for_tests.py` & `django_postman-4.4/postman/module_for_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,22 @@
         return user_representation(self.user)
 
 
 def user_representation(user):
     "for POSTMAN_SHOW_USER_AS, in test_get_user_representation()"
     return 'nick_' + user.get_username()  # some user representation
 
+def context_email(context):
+    "for POSTMAN_CONTEXT_EMAIL, in test_context_email()"
+    context['extra_key'] = '{}_{}'.format(
+        context['object'].sender.username,
+        context['action']
+    )  # a way to prove at the same time the parameters transmission
+    return context
+
 def from_email(context):
     "for POSTMAN_FROM_EMAIL, in test_from_email()"
     return '{}_{}@domain.tld'.format(
         context['object'].sender.username,
         context['action']
     )  # a way to prove at the same time the parameters transmission
```

### Comparing `django-postman-4.3.2/postman/query.py` & `django_postman-4.4/postman/query.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/static/postman/css/postman.css` & `django_postman-4.4/postman/static/postman/css/postman.css`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/admin/postman/pendingmessage/change_form.html` & `django_postman-4.4/postman/templates/admin/postman/pendingmessage/change_form.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/autocomplete_postman_multiple_as1-1.html` & `django_postman-4.4/postman/templates/autocomplete_postman_multiple_as1-1.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/autocomplete_postman_multiple_as1-2.html` & `django_postman-4.4/postman/templates/autocomplete_postman_multiple_as1-2.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/autocomplete_postman_multiple_as1-3.html` & `django_postman-4.4/postman/templates/autocomplete_postman_multiple_as1-3.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/autocomplete_postman_single_as1-1.html` & `django_postman-4.4/postman/templates/autocomplete_postman_single_as1-1.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/postman/base.html` & `django_postman-4.4/postman/templates/postman/base.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/postman/base_folder.html` & `django_postman-4.4/postman/templates/postman/base_folder.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/postman/base_write.html` & `django_postman-4.4/postman/templates/postman/base_write.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/postman/email_user.txt` & `django_postman-4.4/postman/templates/postman/email_user.txt`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/postman/email_visitor.txt` & `django_postman-4.4/postman/templates/postman/email_visitor.txt`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/postman/inc_subject_ex.html` & `django_postman-4.4/postman/templates/postman/inc_subject_ex.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templates/postman/view.html` & `django_postman-4.4/postman/templates/postman/view.html`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templatetags/pagination_tags.py` & `django_postman-4.4/postman/templatetags/pagination_tags.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/templatetags/postman_tags.py` & `django_postman-4.4/postman/templatetags/postman_tags.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/tests.py` & `django_postman-4.4/postman/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
 class GenericTest(TestCase):
     """
     Usual generic tests.
     """
     def test_version(self):
-        self.assertEqual(sys.modules['postman'].__version__, "4.3.2")
+        self.assertEqual(sys.modules['postman'].__version__, "4.4")
 
 
 class TransactionViewTest(TransactionTestCase):
     """
     Test some transactional behavior.
     Can't use Django TestCase class, because it has a special treament for commit/rollback to speed up the database resetting.
     """
@@ -2024,14 +2024,39 @@
         site = self.get_site()
         self.check_email('nonexistent_template', recipient_list, m, action, site)
         self.check_email('email_txt_only', recipient_list, m, action, site, 'Text only\n')
         self.check_email('email_html_only', recipient_list, m, action, site, ('Html only\n', '<div>Html only</div>\n'))
         self.check_email('email_html_and_empty_txt', recipient_list, m, action, site, ('Html and empty Text\n', '<div>Html and empty Text</div>\n'))
         self.check_email('email_html_and_txt', recipient_list, m, action, site, ('Alternate Text\n', '<div>Html and Text</div>\n'))
 
+    def check_context_email(self, m, action, setting):
+        mail.outbox = []
+        settings.POSTMAN_CONTEXT_EMAIL = setting
+        self.reload_modules()
+        email(
+            'postman_for_tests/email_subject.txt',
+            'postman_for_tests/email_txt_only',  # any
+            ['recipient@domain.tld'],
+            m,
+            action,
+            None
+        )
+        self.assertEqual(mail.outbox[0].subject, '{}_{}'.format(m.sender.username, action))
+
+    def test_context_email(self):
+        "Test the POSTMAN_CONTEXT_EMAIL setting."
+        m = self.c12()
+        action = 'some_action'
+
+        # a function
+        self.check_context_email(m, action, lambda context: dict(context, extra_key='{}_{}'.format(m.sender.username, action)))
+
+        # a path to a function
+        self.check_context_email(m, action, 'postman.module_for_tests.context_email')
+
     def check_from_email(self, subject_template, message_template_name, recipient_list, object, action, site, from_email):
         mail.outbox = []
         email(subject_template, message_template_name, recipient_list, object, action, site)
         self.assertEqual(mail.outbox[0].from_email, from_email)
 
     def test_from_email(self):
         "Test the POSTMAN_FROM_EMAIL setting."
@@ -2316,15 +2341,15 @@
         c2_m1 = self.c12(sender_deleted_at=good_date, recipient_deleted_at=good_date)
         c2_m1.thread = c2_m1; c2_m1.save()
         c2_m2 = self.c21(parent=c2_m1, thread=c2_m1.thread, sender_deleted_at=now(), recipient_deleted_at=good_date)
 
         c3_m1 = self.c12(sender_deleted_at=good_date, recipient_deleted_at=good_date)
         c3_m1.thread = c3_m1; c3_m1.save()
         c3_m2 = self.c21(parent=c3_m1, thread=c3_m1.thread, sender_deleted_at=good_date)  # missing recipient_deleted_at
-        
+
         out = StringIO()
         call_command('postman_cleanup', verbosity=0, stdout=out)
         self.assertEqual(out.getvalue(), '')
         self.assertListEqual(list(Message.objects.all()), [c3_m2, c3_m1, c2_m2, c2_m1])
 
     def test_cleanup_days(self):
         "Test the 'days' option."
```

### Comparing `django-postman-4.3.2/postman/urls.py` & `django_postman-4.4/postman/urls.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/urls_for_tests.py` & `django_postman-4.4/postman/urls_for_tests.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/postman/utils.py` & `django_postman-4.4/postman/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from importlib import import_module
 from textwrap import TextWrapper
 
-from django import VERSION
 from django.apps import apps
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.template import TemplateDoesNotExist
 from django.template.loader import render_to_string
 from django.utils.encoding import force_str
 from django.utils.html import strip_tags
@@ -58,14 +57,16 @@
         msg = EmailMultiAlternatives(subject, message, from_email, recipient_list, **kwargs)
         if html_message:
             msg.attach_alternative(html_message, 'text/html')
         return msg.send(**send_kwargs)
 
 # to disable email notification to users
 DISABLE_USER_EMAILING = getattr(settings, 'POSTMAN_DISABLE_USER_EMAILING', False)
+# custom context for email
+CONTEXT_EMAIL = getattr(settings, 'POSTMAN_CONTEXT_EMAIL', None)
 # custom default 'from'
 FROM_EMAIL = getattr(settings, 'POSTMAN_FROM_EMAIL', settings.DEFAULT_FROM_EMAIL)
 # custom parameters for emailing
 PARAMS_EMAIL = getattr(settings, 'POSTMAN_PARAMS_EMAIL', None)
 # support for custom user models that use a custom email field name
 EMAIL_FIELD = get_user_model().get_email_field_name()
 
@@ -106,14 +107,19 @@
     return subject if re.match(pattern, subject, re.IGNORECASE) else str.format(subject=subject)
 
 
 @sensitive_variables('subject', 'html_message', 'message')
 def email(subject_template, message_template_name, recipient_list, object, action, site):
     """Compose and send an email."""
     context = {'site': site, 'object': object, 'action': action}
+    if callable(CONTEXT_EMAIL):
+        context = CONTEXT_EMAIL(context)
+    elif isinstance(CONTEXT_EMAIL, str):  # expected syntax: 'myapp.mymodule.myfunc'
+        mod_path, _, attr_name = CONTEXT_EMAIL.rpartition('.')
+        context = getattr(import_module(mod_path), attr_name)(context)
     subject = render_to_string(subject_template, context)
     # Email subject *must not* contain newlines
     subject = ''.join(subject.splitlines())
 
     # look for html and/or txt versions
     try:
         html_message = render_to_string(message_template_name + '.html', context)
```

### Comparing `django-postman-4.3.2/postman/views.py` & `django_postman-4.4/postman/views.py`

 * *Files identical despite different names*

### Comparing `django-postman-4.3.2/pyproject.toml` & `django_postman-4.4/pyproject.toml`

 * *Files identical despite different names*

