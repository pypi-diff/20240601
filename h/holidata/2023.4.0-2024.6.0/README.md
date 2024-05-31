# Comparing `tmp/holidata-2023.4.0.tar.gz` & `tmp/holidata-2024.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/alatar/Projects/holidata/dist/.tmp-dyfu2p_o/holidata-2023.4.0.tar", last modified: Mon Apr 24 20:30:45 2023, max compression
+gzip compressed data, was "holidata-2024.6.0.tar", last modified: Fri May 31 22:18:31 2024, max compression
```

## Comparing `holidata-2023.4.0.tar` & `holidata-2024.6.0.tar`

### file list

```diff
@@ -1,95 +1,79 @@
-drwxr-xr-x   0 alatar     (501) staff       (20)        0 2023-04-24 20:30:45.610284 holidata-2023.4.0/
--rw-r--r--   0 alatar     (501) staff       (20)     1144 2022-07-10 20:34:28.000000 holidata-2023.4.0/LICENSE
--rw-r--r--   0 alatar     (501) staff       (20)       26 2022-07-10 20:34:28.000000 holidata-2023.4.0/MANIFEST.in
--rw-r--r--   0 alatar     (501) staff       (20)     3368 2023-04-24 20:30:45.610564 holidata-2023.4.0/PKG-INFO
--rw-r--r--   0 alatar     (501) staff       (20)     2332 2023-04-24 20:04:17.000000 holidata-2023.4.0/README.md
-drwxr-xr-x   0 alatar     (501) staff       (20)        0 2023-04-24 20:30:45.514322 holidata-2023.4.0/bin/
--rwxr-xr-x   0 alatar     (501) staff       (20)     2026 2023-04-24 20:18:17.000000 holidata-2023.4.0/bin/holidata
--rw-r--r--   0 alatar     (501) staff       (20)       87 2022-07-10 20:34:28.000000 holidata-2023.4.0/pyproject.toml
--rw-r--r--   0 alatar     (501) staff       (20)       74 2023-04-24 20:30:45.611546 holidata-2023.4.0/setup.cfg
--rw-r--r--   0 alatar     (501) staff       (20)     1695 2023-04-24 20:25:26.000000 holidata-2023.4.0/setup.py
-drwxr-xr-x   0 alatar     (501) staff       (20)        0 2023-04-24 20:30:45.510614 holidata-2023.4.0/src/
-drwxr-xr-x   0 alatar     (501) staff       (20)        0 2023-04-24 20:30:45.516145 holidata-2023.4.0/src/holidata/
--rw-r--r--   0 alatar     (501) staff       (20)     1911 2023-04-24 20:18:17.000000 holidata-2023.4.0/src/holidata/__init__.py
--rw-r--r--   0 alatar     (501) staff       (20)     2726 2023-04-24 20:08:14.000000 holidata-2023.4.0/src/holidata/emitters.py
-drwxr-xr-x   0 alatar     (501) staff       (20)        0 2023-04-24 20:30:45.607880 holidata-2023.4.0/src/holidata/holidays/
--rw-r--r--   0 alatar     (501) staff       (20)      172 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/AT.py
--rw-r--r--   0 alatar     (501) staff       (20)      100 2023-04-24 20:04:17.000000 holidata-2023.4.0/src/holidata/holidays/BE.py
--rw-r--r--   0 alatar     (501) staff       (20)      304 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/BR.py
--rw-r--r--   0 alatar     (501) staff       (20)      187 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/CA.py
--rw-r--r--   0 alatar     (501) staff       (20)      298 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/CH.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/CO.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/CZ.py
--rw-r--r--   0 alatar     (501) staff       (20)      223 2023-04-24 20:04:17.000000 holidata-2023.4.0/src/holidata/holidays/DE.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/DK.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/EE.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/ES.py
--rw-r--r--   0 alatar     (501) staff       (20)       94 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/FI.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/FR.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/GB.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/GR.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/HR.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/HU.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/IS.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/IT.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/NL.py
--rw-r--r--   0 alatar     (501) staff       (20)      110 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/NO.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/NZ.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/PL.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/PT.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/RU.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/SE.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/SI.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/SK.py
--rw-r--r--   0 alatar     (501) staff       (20)      112 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/TR.py
--rw-r--r--   0 alatar     (501) staff       (20)      520 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/US.py
--rw-r--r--   0 alatar     (501) staff       (20)       88 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/ZA.py
--rw-r--r--   0 alatar     (501) staff       (20)      880 2023-04-24 20:04:17.000000 holidata-2023.4.0/src/holidata/holidays/__init__.py
--rw-r--r--   0 alatar     (501) staff       (20)     2091 2022-09-04 17:40:17.000000 holidata-2023.4.0/src/holidata/holidays/cs-CZ.py
--rw-r--r--   0 alatar     (501) staff       (20)      644 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/da-DK.py
--rw-r--r--   0 alatar     (501) staff       (20)     1012 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/de-AT.py
--rw-r--r--   0 alatar     (501) staff       (20)      604 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/de-BE.py
--rw-r--r--   0 alatar     (501) staff       (20)     1310 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/de-CH.py
--rw-r--r--   0 alatar     (501) staff       (20)     3263 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/de-DE.py
--rw-r--r--   0 alatar     (501) staff       (20)     1581 2022-09-04 17:40:17.000000 holidata-2023.4.0/src/holidata/holidays/el-GR.py
--rw-r--r--   0 alatar     (501) staff       (20)     3250 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/en-CA.py
--rw-r--r--   0 alatar     (501) staff       (20)     5102 2023-04-24 20:08:14.000000 holidata-2023.4.0/src/holidata/holidays/en-GB.py
--rw-r--r--   0 alatar     (501) staff       (20)     4415 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/en-NZ.py
--rw-r--r--   0 alatar     (501) staff       (20)      746 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/en-US.py
--rw-r--r--   0 alatar     (501) staff       (20)     3209 2022-09-04 17:40:17.000000 holidata-2023.4.0/src/holidata/holidays/en-ZA.py
--rw-r--r--   0 alatar     (501) staff       (20)     2907 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/es-CO.py
--rw-r--r--   0 alatar     (501) staff       (20)    30343 2022-10-21 20:35:14.000000 holidata-2023.4.0/src/holidata/holidays/es-ES.py
--rw-r--r--   0 alatar     (501) staff       (20)      797 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/es-US.py
--rw-r--r--   0 alatar     (501) staff       (20)      748 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/et-EE.py
--rw-r--r--   0 alatar     (501) staff       (20)     1467 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/fi-FI.py
--rw-r--r--   0 alatar     (501) staff       (20)      597 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/fr-BE.py
--rw-r--r--   0 alatar     (501) staff       (20)     3699 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/fr-CA.py
--rw-r--r--   0 alatar     (501) staff       (20)      603 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/fr-FR.py
--rw-r--r--   0 alatar     (501) staff       (20)     5706 2023-04-24 20:08:14.000000 holidata-2023.4.0/src/holidata/holidays/holidays.py
--rw-r--r--   0 alatar     (501) staff       (20)     1158 2023-02-10 12:03:52.000000 holidata-2023.4.0/src/holidata/holidays/hr-HR.py
--rw-r--r--   0 alatar     (501) staff       (20)     9559 2022-09-04 17:40:17.000000 holidata-2023.4.0/src/holidata/holidays/hu-HU.py
--rw-r--r--   0 alatar     (501) staff       (20)     2266 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/is-IS.py
--rw-r--r--   0 alatar     (501) staff       (20)      573 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/it-IT.py
--rw-r--r--   0 alatar     (501) staff       (20)      801 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/nb-NO.py
--rw-r--r--   0 alatar     (501) staff       (20)      626 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/nl-BE.py
--rw-r--r--   0 alatar     (501) staff       (20)     1672 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/nl-NL.py
--rw-r--r--   0 alatar     (501) staff       (20)      845 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/pl-PL.py
--rw-r--r--   0 alatar     (501) staff       (20)     4273 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/pt-BR.py
--rw-r--r--   0 alatar     (501) staff       (20)      706 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/pt-PT.py
--rw-r--r--   0 alatar     (501) staff       (20)      625 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/ru-RU.py
--rw-r--r--   0 alatar     (501) staff       (20)      844 2022-07-10 20:34:28.000000 holidata-2023.4.0/src/holidata/holidays/sk-SK.py
--rw-r--r--   0 alatar     (501) staff       (20)     1408 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/sl-SI.py
--rw-r--r--   0 alatar     (501) staff       (20)     1439 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/sv-FI.py
--rw-r--r--   0 alatar     (501) staff       (20)     2085 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/sv-SE.py
--rw-r--r--   0 alatar     (501) staff       (20)     3696 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/holidays/tr-TR.py
--rw-r--r--   0 alatar     (501) staff       (20)      597 2023-04-24 20:08:14.000000 holidata-2023.4.0/src/holidata/plugin.py
--rw-r--r--   0 alatar     (501) staff       (20)     1918 2022-10-21 20:32:53.000000 holidata-2023.4.0/src/holidata/utils.py
-drwxr-xr-x   0 alatar     (501) staff       (20)        0 2023-04-24 20:30:45.518868 holidata-2023.4.0/src/holidata.egg-info/
--rw-r--r--   0 alatar     (501) staff       (20)     3368 2023-04-24 20:30:45.000000 holidata-2023.4.0/src/holidata.egg-info/PKG-INFO
--rw-r--r--   0 alatar     (501) staff       (20)     2448 2023-04-24 20:30:45.000000 holidata-2023.4.0/src/holidata.egg-info/SOURCES.txt
--rw-r--r--   0 alatar     (501) staff       (20)        1 2023-04-24 20:30:45.000000 holidata-2023.4.0/src/holidata.egg-info/dependency_links.txt
--rw-r--r--   0 alatar     (501) staff       (20)       92 2023-04-24 20:30:45.000000 holidata-2023.4.0/src/holidata.egg-info/requires.txt
--rw-r--r--   0 alatar     (501) staff       (20)        9 2023-04-24 20:30:45.000000 holidata-2023.4.0/src/holidata.egg-info/top_level.txt
-drwxr-xr-x   0 alatar     (501) staff       (20)        0 2023-04-24 20:30:45.609408 holidata-2023.4.0/tests/
--rw-r--r--   0 alatar     (501) staff       (20)     1262 2023-02-10 12:02:50.000000 holidata-2023.4.0/tests/test_holidata.py
--rw-r--r--   0 alatar     (501) staff       (20)     2208 2022-10-21 20:32:53.000000 holidata-2023.4.0/tests/test_holidays.py
+drwxr-xr-x   0 alatar     (501) staff       (20)        0 2024-05-31 22:18:31.272636 holidata-2024.6.0/
+-rw-r--r--   0 alatar     (501) staff       (20)     1144 2023-11-24 13:14:45.000000 holidata-2024.6.0/LICENSE
+-rw-r--r--   0 alatar     (501) staff       (20)       26 2023-11-24 13:14:45.000000 holidata-2024.6.0/MANIFEST.in
+-rw-r--r--   0 alatar     (501) staff       (20)     3524 2024-05-31 22:18:31.272315 holidata-2024.6.0/PKG-INFO
+-rw-r--r--   0 alatar     (501) staff       (20)     2332 2024-05-31 20:55:46.000000 holidata-2024.6.0/README.md
+drwxr-xr-x   0 alatar     (501) staff       (20)        0 2024-05-31 22:18:31.210517 holidata-2024.6.0/bin/
+-rwxr-xr-x   0 alatar     (501) staff       (20)     2003 2023-11-24 13:14:45.000000 holidata-2024.6.0/bin/holidata
+-rw-r--r--   0 alatar     (501) staff       (20)       87 2023-11-24 13:14:45.000000 holidata-2024.6.0/pyproject.toml
+-rw-r--r--   0 alatar     (501) staff       (20)       74 2024-05-31 22:18:31.273487 holidata-2024.6.0/setup.cfg
+-rw-r--r--   0 alatar     (501) staff       (20)     1659 2024-05-31 22:16:46.000000 holidata-2024.6.0/setup.py
+drwxr-xr-x   0 alatar     (501) staff       (20)        0 2024-05-31 22:18:31.205828 holidata-2024.6.0/src/
+drwxr-xr-x   0 alatar     (501) staff       (20)        0 2024-05-31 22:18:31.214178 holidata-2024.6.0/src/holidata/
+-rw-r--r--   0 alatar     (501) staff       (20)     1611 2024-05-31 20:55:46.000000 holidata-2024.6.0/src/holidata/__init__.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2796 2024-05-31 20:55:46.000000 holidata-2024.6.0/src/holidata/emitters.py
+drwxr-xr-x   0 alatar     (501) staff       (20)        0 2024-05-31 22:18:31.248667 holidata-2024.6.0/src/holidata/holidays/
+-rw-r--r--   0 alatar     (501) staff       (20)     3765 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/AT.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3296 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/BE.py
+-rw-r--r--   0 alatar     (501) staff       (20)    11608 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/BR.py
+-rw-r--r--   0 alatar     (501) staff       (20)     7348 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/CA.py
+-rw-r--r--   0 alatar     (501) staff       (20)     4361 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/CH.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3342 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/CO.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3086 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/CZ.py
+-rw-r--r--   0 alatar     (501) staff       (20)     5196 2024-05-31 22:16:46.000000 holidata-2024.6.0/src/holidata/holidays/DE.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1927 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/DK.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2031 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/EE.py
+drwxr-xr-x   0 alatar     (501) staff       (20)        0 2024-05-31 22:18:31.268186 holidata-2024.6.0/src/holidata/holidays/ES/
+-rw-r--r--   0 alatar     (501) staff       (20)     2670 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/AN.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2836 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/AR.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2591 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/AS.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2550 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/CB.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3167 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/CE.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3334 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/CL.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1839 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/CM.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1954 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/CN.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1107 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/CT.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2745 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/EX.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1383 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/GA.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1484 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/IB.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2467 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/MC.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3096 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/MD.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3528 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/ML.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1782 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/NC.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1630 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/PV.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2072 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/RI.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1851 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/VC.py
+-rw-r--r--   0 alatar     (501) staff       (20)     4705 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ES/__init__.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3671 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/FI.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1886 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/FR.py
+-rw-r--r--   0 alatar     (501) staff       (20)     5210 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/GB.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2938 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/GR.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2282 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/HR.py
+-rw-r--r--   0 alatar     (501) staff       (20)     5725 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/HU.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3074 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/IS.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1856 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/IT.py
+-rw-r--r--   0 alatar     (501) staff       (20)     3249 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/NL.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2594 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/NO.py
+-rw-r--r--   0 alatar     (501) staff       (20)     4709 2024-05-31 22:16:46.000000 holidata-2024.6.0/src/holidata/holidays/NZ.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2230 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/PL.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2193 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/PT.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1602 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/RU.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2960 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/SE.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2701 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/SI.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2433 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/SK.py
+-rw-r--r--   0 alatar     (501) staff       (20)     4469 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/TR.py
+-rw-r--r--   0 alatar     (501) staff       (20)     4009 2024-05-31 22:16:46.000000 holidata-2024.6.0/src/holidata/holidays/US.py
+-rw-r--r--   0 alatar     (501) staff       (20)     4492 2023-11-24 13:14:45.000000 holidata-2024.6.0/src/holidata/holidays/ZA.py
+-rw-r--r--   0 alatar     (501) staff       (20)      398 2024-05-31 20:55:46.000000 holidata-2024.6.0/src/holidata/holidays/__init__.py
+-rw-r--r--   0 alatar     (501) staff       (20)     7618 2024-05-31 20:55:46.000000 holidata-2024.6.0/src/holidata/holidays/holidays.py
+-rw-r--r--   0 alatar     (501) staff       (20)      597 2024-05-31 20:55:46.000000 holidata-2024.6.0/src/holidata/plugin.py
+-rw-r--r--   0 alatar     (501) staff       (20)     1918 2024-05-31 20:55:46.000000 holidata-2024.6.0/src/holidata/utils.py
+drwxr-xr-x   0 alatar     (501) staff       (20)        0 2024-05-31 22:18:31.270755 holidata-2024.6.0/src/holidata.egg-info/
+-rw-r--r--   0 alatar     (501) staff       (20)     3524 2024-05-31 22:18:31.000000 holidata-2024.6.0/src/holidata.egg-info/PKG-INFO
+-rw-r--r--   0 alatar     (501) staff       (20)     1930 2024-05-31 22:18:31.000000 holidata-2024.6.0/src/holidata.egg-info/SOURCES.txt
+-rw-r--r--   0 alatar     (501) staff       (20)        1 2024-05-31 22:18:31.000000 holidata-2024.6.0/src/holidata.egg-info/dependency_links.txt
+-rw-r--r--   0 alatar     (501) staff       (20)       69 2024-05-31 22:18:31.000000 holidata-2024.6.0/src/holidata.egg-info/requires.txt
+-rw-r--r--   0 alatar     (501) staff       (20)        9 2024-05-31 22:18:31.000000 holidata-2024.6.0/src/holidata.egg-info/top_level.txt
+drwxr-xr-x   0 alatar     (501) staff       (20)        0 2024-05-31 22:18:31.270025 holidata-2024.6.0/tests/
+-rw-r--r--   0 alatar     (501) staff       (20)     1527 2023-11-24 13:14:45.000000 holidata-2024.6.0/tests/test_holidata.py
+-rw-r--r--   0 alatar     (501) staff       (20)     2405 2024-05-31 20:55:46.000000 holidata-2024.6.0/tests/test_holidays.py
```

### Comparing `holidata-2023.4.0/LICENSE` & `holidata-2024.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `holidata-2023.4.0/PKG-INFO` & `holidata-2024.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: holidata
-Version: 2023.4.0
+Version: 2024.6.0
 Summary: Holidata is a utility for algorithmically producing holidays for a given locale and year
 Home-page: https://github.com/GothenburgBitFactory/holidata
 Author: Gothenburg Bit Factory
 Author-email: support@gothenburgbitfactory.org
 Project-URL: Bug Reports, https://github.com/GothenburgBitFactory/holidata/issues
 Project-URL: Source, https://github.com/GothenburgBitFactory/holidata
 Project-URL: Website, https://holidata.net
 Keywords: holiday,calendar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: arrow>=1.3.0
+Requires-Dist: docopt>=0.6.2
+Provides-Extra: test
+Requires-Dist: pytest>=7.4.2; extra == "test"
+Requires-Dist: snapshottest>=0.6.0; extra == "test"
 
 # Holidata
 
 `holidata` is a utility for algorithmically producing holiday data.
 Its purpose is mainly for [holidata.net](https://holidata.net).
 
 Holiday data can be produced for a given year in a supported locale and output format.
```

### Comparing `holidata-2023.4.0/README.md` & `holidata-2024.6.0/README.md`

 * *Files identical despite different names*

### Comparing `holidata-2023.4.0/setup.py` & `holidata-2024.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,44 +5,43 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="holidata",
-    version="2023.04.0",
+    version="2024.6.0",
     description="Holidata is a utility for algorithmically producing holidays for a given locale and year",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GothenburgBitFactory/holidata",
     author="Gothenburg Bit Factory",
     author_email="support@gothenburgbitfactory.org",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="holiday, calendar",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     include_package_data=True,
-    python_requires=">=3.7, <4",
+    python_requires=">=3.8, <4",
     install_requires=[
-        "arrow >= 1.2.2",
+        "arrow >= 1.3.0",
         "docopt >= 0.6.2",
-        "python-dateutil >= 2.8.2",
     ],
     extras_require={
         "test": [
-            "pytest >= 7.1.2",
+            "pytest >= 7.4.2",
             "snapshottest >= 0.6.0",
         ]
     },
     scripts=["bin/holidata"],
     project_urls={
         "Bug Reports": "https://github.com/GothenburgBitFactory/holidata/issues",
         "Source": "https://github.com/GothenburgBitFactory/holidata",
```

### Comparing `holidata-2023.4.0/src/holidata/__init__.py` & `holidata-2024.6.0/src/holidata/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,67 @@
-from .holidays import *
 from .emitters import Emitter
+from .holidays import *
+
 
 def get_country_for(identifier):
     country_class = Country.get(identifier)
 
     if not country_class:
-        raise ValueError("No plugin found for country id '{}'!".format(identifier))
+        raise ValueError(f"No country found for id '{identifier}'!")
 
     return country_class()
 
 
-def get_locale_class_for(identifier):
-    locale_class = Locale.get(identifier)
+def get_emitter_for(identifier):
+    emitter_class = Emitter.get(identifier)
 
-    if not locale_class:
-        raise ValueError("No plugin found for locale: {}!".format(identifier))
+    if not emitter_class:
+        raise ValueError(f"Unsupported output format '{identifier}'!")
 
-    return locale_class
+    return emitter_class()
 
 
-def create_locale_for(country_id=None, lang_id=None, year=None):
-    country_class = get_country_for(country_id)
+def for_locale(country_id, lang_id=None):
+    country = get_country_for(country_id)
+    lang_id = country.validate_language_or_get_default(lang_id)
 
-    if lang_id is not None and lang_id.lower() not in country_class.languages:
-        raise ValueError("Language '{}' is not defined for country '{}'!".format(lang_id, country_class.id))
-    elif lang_id is None and country_class.default_lang is not None:
-        lang_id = country_class.default_lang
-    elif lang_id is None:
-        raise ValueError("Country '{}' has no default language specified! Please choose one of [{}].".format(country_id, ", ".join(country_class.languages)))
+    return Locale(country, lang_id)
 
-    locale_class = get_locale_class_for("{}-{}".format(lang_id, country_id))
 
-    return locale_class(year)
+class Holidata:
+    emitter = None
+    holidays = None
 
+    def __init__(self, holidays, emitter=None):
+        self.holidays = holidays
+        self.emitter = emitter
 
-def create_emitter_for(identifier):
-    emitter_class = Emitter.get(identifier)
+    def __str__(self):
+        return self.emitter.output(self.holidays)
 
-    if not emitter_class:
-        raise ValueError("Unsupported output format: '{}'!".format(identifier))
+    def formatted_as(self, format_id):
+        self.emitter = get_emitter_for(format_id)
 
-    return emitter_class()
+        return self
 
 
-def parse_year(year):
-    try:
-        return int(year)
-    except:
-        raise ValueError(f"Invalid year '{year}'! Has to be an integer.")
+class Locale:
+    def __init__(self, country, lang):
+        self.country = country
+        self.lang = lang
 
+    def get_holidays_of(self, year):
+        return self.country.get_holidays_of(year, self.lang)
 
-class Holidata:
-    locale = None
-    emitter = None
+    def holidays_of(self, year):
+        return Holidata(self.country.get_holidays_of(self._parse_year(year), self.lang))
 
-    def __init__(self, country=None, language=None, year=None, output=None):
-        self.locale = create_locale_for(country_id=country, lang_id=language, year=parse_year(year))
-        self.emitter = create_emitter_for(output)
+    @staticmethod
+    def _parse_year(year):
+        try:
+            return int(year)
+        except ValueError:
+            raise ValueError(f"Invalid year '{year}'! Has to be an integer.")
 
-    def __str__(self):
-        return self.emitter.output(self.locale)
+    @property
+    def id(self):
+        return f"{self.lang}-{self.country.id}"
```

### Comparing `holidata-2023.4.0/src/holidata/emitters.py` & `holidata-2024.6.0/src/holidata/emitters.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import csv
 import io
 import json
 
 from holidata.plugin import PluginMount
 
-class Emitter(object, metaclass=PluginMount):
+
+class Emitter(metaclass=PluginMount):
     type = None
 
     def __init__(self):
         if self.type is None:
-            raise ValueError("Emitter {0} does not provide its type".format(self.__class__.__name__))
+            raise ValueError(f"Emitter {self.__class__.__name__} does not provide its type!")
 
     @staticmethod
     def get(identifier):
-         return Emitter.get_plugin(identifier, "type")
+        return Emitter.get_plugin(identifier, "type")
 
-    def output(self, locale):
+    def output(self, holidays):
         pass
 
 
 class JsonEmitter(Emitter):
     type = "json"
 
-    def output(self, locale):
-        export_data = [h.as_dict() for h in locale.holidays]
-        export_data.sort(key=lambda x: x["date"])
+    def output(self, holidays):
+        export_data = [h.as_dict() for h in holidays]
+        export_data.sort(key=lambda x: (x["date"], x["description"], x["region"]))
         return "\n".join([json.dumps(h, ensure_ascii=False, sort_keys=False, indent=None, separators=(",", ":")) for h in export_data]) + "\n"
 
 
 class CsvEmitter(Emitter):
     type = "csv"
 
-    def output(self, locale):
-        export_data = [h.as_dict() for h in locale.holidays]
-        export_data.sort(key=lambda x: x["date"])
+    def output(self, holidays):
+        export_data = [h.as_dict() for h in holidays]
+        export_data.sort(key=lambda x: (x["date"], x["description"], x["region"]))
         result = io.StringIO()
 
         writer = csv.DictWriter(result,
                                 ["locale", "region", "date", "description", "type", "notes"],
                                 quoting=csv.QUOTE_ALL,
                                 lineterminator="\n")
         writer.writeheader()
@@ -45,49 +46,49 @@
 
         return result.getvalue()
 
 
 class YamlEmitter(Emitter):
     type = "yaml"
 
-    def output(self, locale):
-        export_data = [h.as_dict() for h in locale.holidays]
-        export_data.sort(key=lambda x: x["date"])
+    def output(self, holidays):
+        export_data = [h.as_dict() for h in holidays]
+        export_data.sort(key=lambda x: (x["date"], x["description"], x["region"]))
 
         output = "%YAML 1.1\n"
         output += "---\n"
         for holiday in export_data:
             output += "  holiday:\n"
 
             for key in ["locale", "region", "date", "description", "type", "notes"]:
                 value = holiday[key]
 
                 if value is not None and value != "":
-                    output += "    {}: {}\n".format(key, value)
+                    output += f"    {key}: {value}\n"
                 else:
-                    output += "    {}:\n".format(key)
+                    output += f"    {key}:\n"
 
         output += "...\n"
         return output
 
 
 class XmlEmitter(Emitter):
     type = "xml"
 
-    def output(self, locale):
-        export_data = [h.as_dict() for h in locale.holidays]
-        export_data.sort(key=lambda x: x["date"])
+    def output(self, holidays):
+        export_data = [h.as_dict() for h in holidays]
+        export_data.sort(key=lambda x: (x["date"], x["description"], x["region"]))
 
         output = "<?xml version=\"1.0\" encoding=\"UTF-8\" ?>\n"
         output += "<holidays>\n"
 
         for holiday in export_data:
             output += "  <holiday>\n"
 
             for key in ["locale", "region", "date", "description", "type", "notes"]:
                 value = holiday[key] if key in holiday else ""
-                output += "    <{0}>{1}</{0}>\n".format(key, value if value is not None else "")
+                output += f"    <{key}>{value if value is not None else ''}</{key}>\n"
 
             output += "  </holiday>\n"
 
         output += "</holidays>\n"
         return output
```

### Comparing `holidata-2023.4.0/src/holidata/holidays/tr-TR.py` & `holidata-2024.6.0/src/holidata/holidays/TR.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,93 @@
-# coding=utf-8
+from dateutil.easter import EASTER_WESTERN
+
+from .holidays import Country
 from holidata.utils import SmartDayArrow
-from .holidays import Locale, Holiday
 
 """
 sources:
 law on national holidays and general holidays: https://www.mevzuat.gov.tr/mevzuat?MevzuatNo=2429&MevzuatTur=1&MevzuatTertip=5 
 dates for holidays 'Ramazan Bayramı' and 'Kurban Bayramı': https://vakithesaplama.diyanet.gov.tr/dini_gunler.php
 """
 
 
-class tr_TR(Locale):
-    """
-    01-01: [NF] Yılbaşı
-    04-23: [NF] Ulusal Egemenlik ve Çocuk Bayramı
-    05-01: [NF] Emek ve Dayanışma Günü
-    05-19: [NF] Atatürk'ü Anma, Gençlik ve Spor Bayramı
-    08-30: [NF] Zafer Bayramı
-    10-29: [NF] Cumhuriyet Bayramı
-    """
+class TR(Country):
+    id = "TR"
+    languages = ["tr"]
+    default_lang = "tr"
+    easter_type = EASTER_WESTERN
+
+    def __init__(self):
+        super().__init__()
+
+        self.define_holiday() \
+            .with_name("Yılbaşı") \
+            .on("01-01") \
+            .with_flags("NF")
+
+        self.define_holiday() \
+            .with_name("Ulusal Egemenlik ve Çocuk Bayramı") \
+            .on("04-23") \
+            .with_flags("NF")
+
+        self.define_holiday() \
+            .with_name("Emek ve Dayanışma Günü") \
+            .on("05-01") \
+            .with_flags("NF")
+
+        self.define_holiday() \
+            .with_name("Atatürk'ü Anma, Gençlik ve Spor Bayramı") \
+            .on("05-19") \
+            .with_flags("NF")
+
+        self.define_holiday() \
+            .with_name("Zafer Bayramı") \
+            .on("08-30") \
+            .with_flags("NF")
+
+        self.define_holiday() \
+            .with_name("Cumhuriyet Bayramı") \
+            .on("10-29") \
+            .with_flags("NF")
+
+        self.define_holiday() \
+            .with_name("Demokrasi ve Milli Birlik Günü") \
+            .on("07-15") \
+            .since(2017) \
+            .with_flags("NF")
 
-    locale = "tr-TR"
+        """
+        Ramazan Bayramı 1.-3. Gün
+        """
+        for i in [1, 2, 3]:
+            self.define_holiday() \
+                .with_name(f"Ramazan Bayramı ({i}. Gün)") \
+                .on(self.ramazan_bayrami_day(i)) \
+                .with_flags("NRV")
+
+        """
+        Kurban Bayramı 1.-4. Gün
+        """
+        for i in [1, 2, 3, 4]:
+            self.define_holiday() \
+                .with_name(f"Kurban Bayramı ({i}. Gün)") \
+                .on(self.kurban_bayrami_day(i)) \
+                .with_flags("NRV")
+
+    def ramazan_bayrami_day(self, ordinal):
+        def ramazan_bayrami_reference_shifted(year):
+            return self.__ramazan_bayrami_reference(year).shift(days=ordinal)
+
+        return ramazan_bayrami_reference_shifted
+
+    def kurban_bayrami_day(self, ordinal):
+        def kurban_bayrami_reference_shifted(year):
+            return self.__kurban_bayrami_reference(year).shift(days=ordinal)
+
+        return kurban_bayrami_reference_shifted
 
     @staticmethod
     def __ramazan_bayrami_reference(year):
         ramazan_bayrami_reference = {
             2011: SmartDayArrow(2011, 8, 29),
             2012: SmartDayArrow(2012, 8, 18),
             2013: SmartDayArrow(2013, 8,  7),
@@ -64,48 +128,7 @@
             2024: SmartDayArrow(2024,  6, 15),
             2025: SmartDayArrow(2025,  6,  5),
             2026: SmartDayArrow(2026,  5, 26),
             2027: SmartDayArrow(2027,  5, 15),
         }
 
         return kurban_bayrami_reference[year]
-
-    def holiday_demokrasi_ve_milli_birlik_gunu(self):
-        """
-        Democracy and National Unity Day (since 2017)
-        07-15 [NF] Demokrasi ve Milli Birlik Günü
-        """
-        return [Holiday(
-            self.locale,
-            "",
-            SmartDayArrow(self.year, 7, 15),
-            "Demokrasi ve Milli Birlik Günü",
-            "NF"
-        )] if self.year >= 2017 else []
-
-    def holiday_ramazan_bayrami(self):
-        """
-        Ramazan Bayramı 1.-3. Gün
-        """
-        reference = self.__ramazan_bayrami_reference(self.year)
-
-        return [Holiday(
-            self.locale,
-            "",
-            reference.shift(days=i),
-            "Ramazan Bayramı ({}. Gün)".format(i),
-            "NRV"
-        ) for i in [1, 2, 3]]
-
-    def holiday_kurban_bayrami(self):
-        """
-        Kurban Bayramı 1.-4. Gün
-        """
-        reference = self.__kurban_bayrami_reference(self.year)
-
-        return [Holiday(
-            self.locale,
-            "",
-            reference.shift(days=i),
-            "Kurban Bayramı ({}. Gün)".format(i),
-            "NRV"
-        ) for i in [1, 2, 3, 4]]
```

### Comparing `holidata-2023.4.0/src/holidata/plugin.py` & `holidata-2024.6.0/src/holidata/plugin.py`

 * *Files identical despite different names*

### Comparing `holidata-2023.4.0/src/holidata/utils.py` & `holidata-2024.6.0/src/holidata/utils.py`

 * *Files identical despite different names*

### Comparing `holidata-2023.4.0/src/holidata.egg-info/PKG-INFO` & `holidata-2024.6.0/src/holidata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: holidata
-Version: 2023.4.0
+Version: 2024.6.0
 Summary: Holidata is a utility for algorithmically producing holidays for a given locale and year
 Home-page: https://github.com/GothenburgBitFactory/holidata
 Author: Gothenburg Bit Factory
 Author-email: support@gothenburgbitfactory.org
 Project-URL: Bug Reports, https://github.com/GothenburgBitFactory/holidata/issues
 Project-URL: Source, https://github.com/GothenburgBitFactory/holidata
 Project-URL: Website, https://holidata.net
 Keywords: holiday,calendar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: arrow>=1.3.0
+Requires-Dist: docopt>=0.6.2
+Provides-Extra: test
+Requires-Dist: pytest>=7.4.2; extra == "test"
+Requires-Dist: snapshottest>=0.6.0; extra == "test"
 
 # Holidata
 
 `holidata` is a utility for algorithmically producing holiday data.
 Its purpose is mainly for [holidata.net](https://holidata.net).
 
 Holiday data can be produced for a given year in a supported locale and output format.
```

### Comparing `holidata-2023.4.0/src/holidata.egg-info/SOURCES.txt` & `holidata-2024.6.0/src/holidata.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 src/holidata/holidays/CA.py
 src/holidata/holidays/CH.py
 src/holidata/holidays/CO.py
 src/holidata/holidays/CZ.py
 src/holidata/holidays/DE.py
 src/holidata/holidays/DK.py
 src/holidata/holidays/EE.py
-src/holidata/holidays/ES.py
 src/holidata/holidays/FI.py
 src/holidata/holidays/FR.py
 src/holidata/holidays/GB.py
 src/holidata/holidays/GR.py
 src/holidata/holidays/HR.py
 src/holidata/holidays/HU.py
 src/holidata/holidays/IS.py
@@ -42,46 +41,30 @@
 src/holidata/holidays/SE.py
 src/holidata/holidays/SI.py
 src/holidata/holidays/SK.py
 src/holidata/holidays/TR.py
 src/holidata/holidays/US.py
 src/holidata/holidays/ZA.py
 src/holidata/holidays/__init__.py
-src/holidata/holidays/cs-CZ.py
-src/holidata/holidays/da-DK.py
-src/holidata/holidays/de-AT.py
-src/holidata/holidays/de-BE.py
-src/holidata/holidays/de-CH.py
-src/holidata/holidays/de-DE.py
-src/holidata/holidays/el-GR.py
-src/holidata/holidays/en-CA.py
-src/holidata/holidays/en-GB.py
-src/holidata/holidays/en-NZ.py
-src/holidata/holidays/en-US.py
-src/holidata/holidays/en-ZA.py
-src/holidata/holidays/es-CO.py
-src/holidata/holidays/es-ES.py
-src/holidata/holidays/es-US.py
-src/holidata/holidays/et-EE.py
-src/holidata/holidays/fi-FI.py
-src/holidata/holidays/fr-BE.py
-src/holidata/holidays/fr-CA.py
-src/holidata/holidays/fr-FR.py
 src/holidata/holidays/holidays.py
-src/holidata/holidays/hr-HR.py
-src/holidata/holidays/hu-HU.py
-src/holidata/holidays/is-IS.py
-src/holidata/holidays/it-IT.py
-src/holidata/holidays/nb-NO.py
-src/holidata/holidays/nl-BE.py
-src/holidata/holidays/nl-NL.py
-src/holidata/holidays/pl-PL.py
-src/holidata/holidays/pt-BR.py
-src/holidata/holidays/pt-PT.py
-src/holidata/holidays/ru-RU.py
-src/holidata/holidays/sk-SK.py
-src/holidata/holidays/sl-SI.py
-src/holidata/holidays/sv-FI.py
-src/holidata/holidays/sv-SE.py
-src/holidata/holidays/tr-TR.py
+src/holidata/holidays/ES/AN.py
+src/holidata/holidays/ES/AR.py
+src/holidata/holidays/ES/AS.py
+src/holidata/holidays/ES/CB.py
+src/holidata/holidays/ES/CE.py
+src/holidata/holidays/ES/CL.py
+src/holidata/holidays/ES/CM.py
+src/holidata/holidays/ES/CN.py
+src/holidata/holidays/ES/CT.py
+src/holidata/holidays/ES/EX.py
+src/holidata/holidays/ES/GA.py
+src/holidata/holidays/ES/IB.py
+src/holidata/holidays/ES/MC.py
+src/holidata/holidays/ES/MD.py
+src/holidata/holidays/ES/ML.py
+src/holidata/holidays/ES/NC.py
+src/holidata/holidays/ES/PV.py
+src/holidata/holidays/ES/RI.py
+src/holidata/holidays/ES/VC.py
+src/holidata/holidays/ES/__init__.py
 tests/test_holidata.py
 tests/test_holidays.py
```

### Comparing `holidata-2023.4.0/tests/test_holidata.py` & `holidata-2024.6.0/tests/test_holidata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 import pytest
 from snapshottest.file import FileSnapshot
 from snapshottest.formatter import Formatter
 
-from holidata import Locale
+from holidata import Locale, Country
 from tests import HOLIDATA_YEAR_MAX
 
 SNAPSHOT_FILE_PATH_PATTERN = "snapshots/snap_test_holidata/{}[{}-{}] 1.py"
 
 
+def create_locales():
+    response = []
+
+    for country_class in Country.plugins:
+        response.extend([Locale(country_class(), lang_id) for lang_id in country_class.languages])
+
+    return response
+
+
+locales = create_locales()
+
+
 @pytest.fixture(params=range(2011, HOLIDATA_YEAR_MAX))
 def year(request):
     return request.param
 
 
-@pytest.fixture(params=Locale.plugins)
-def locale(request, year):
-    return request.param(year)
+@pytest.fixture(params=locales, ids=[loc.id for loc in locales])
+def locale(request):
+    return request.param
 
 
-def test_holidata_produces_holidays_for_locale_and_year(snapshot, tmpdir, locale):
-    temp_file = tmpdir.join("{}.{}.py".format(locale.locale, locale.year))
+def test_holidata_produces_holidays_for_locale_and_year(snapshot, tmpdir, locale, year):
+    temp_file = tmpdir.join(f"{locale.id}.{year}.py")
 
-    export_data = [h.as_dict() for h in locale.holidays]
-    export_data.sort(key=lambda x: x["date"])
+    export_data = [h.as_dict() for h in locale.get_holidays_of(year)]
+    export_data.sort(key=lambda x: (x["date"], x["description"], x["region"]))
     temp_file.write(Formatter().format(export_data, 0))
 
     try:
         snapshot.assert_match(FileSnapshot(str(temp_file)))
     except AssertionError:
         with open(temp_file, "r") as tf:
             actual = "".join(tf.readlines())
 
         snapshot_file = SNAPSHOT_FILE_PATH_PATTERN.format(
             "test_holidata_produces_holidays_for_locale_and_year",
-            locale.__class__.__name__,
-            locale.year)
+            locale.id,
+            year)
 
         with open(snapshot_file) as sf:
             expected = "".join(sf.readlines())
 
         assert (actual == expected)
```

### Comparing `holidata-2023.4.0/tests/test_holidays.py` & `holidata-2024.6.0/tests/test_holidays.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,57 +2,69 @@
 
 import pytest
 
 from holidata import Locale, Country
 from tests import HOLIDATA_YEAR_MAX
 
 
+def create_locales():
+    response = []
+
+    for country_class in Country.plugins:
+        response.extend([Locale(country_class(), lang_id) for lang_id in country_class.languages])
+
+    return response
+
+
+locales = create_locales()
+
+
 @pytest.fixture(params=range(2011, HOLIDATA_YEAR_MAX))
 def year(request):
     return request.param
 
 
-@pytest.fixture(params=Locale.plugins)
-def locale(request, year):
-    return request.param(year)
+@pytest.fixture(params=locales, ids=[loc.id for loc in locales])
+def locale(request):
+    return request.param
 
 
 @pytest.fixture()
-def holidays(locale):
-    return locale.holidays
+def holidays(locale, year):
+    return locale.get_holidays_of(year)
 
 
 @pytest.fixture(params=Country.plugins)
 def country(request):
     return request.param()
 
 
 def test_country_should_be_constructable(country):
     pass
 
 
 def test_holiday_should_not_be_of_type_national_if_region_defined(holidays):
     for holiday in holidays:
-        if holiday.region == '':
-            assert "N" in holiday.flags, "Holiday '{}' ({}) in locale {} must have flag 'N': it has no regions defined".format(holiday.description, holiday.date.strftime("%Y-%m-%d"), holiday.locale)
+        if holiday.region == "":
+            assert "N" in holiday.flags, f"Holiday '{holiday.description}' ({holiday.date.strftime('%Y-%m-%d')}) in locale {holiday.locale} must have flag 'N': it has no regions defined"
 
 
 def test_holiday_should_be_of_type_national_if_no_region_defined(holidays):
     for holiday in holidays:
-        if holiday.region != '':
-            assert "N" not in holiday.flags, "Holiday '{}' ({}) in locale {} must not have flag 'N': it has regions defined".format(holiday.description, holiday.date.strftime("%Y-%m-%d"), holiday.locale)
+        if holiday.region != "":
+            assert "N" not in holiday.flags, f"Holiday '{holiday.description}' ({holiday.date.strftime('%Y-%m-%d')}) in locale {holiday.locale} must not have flag 'N': it has regions defined"
 
 
 def test_holiday_should_be_of_type_either_fixed_or_variable(holidays):
     for holiday in holidays:
         date_is_fixed = "F" in holiday.flags
         date_is_variable = "V" in holiday.flags
 
-        assert not (date_is_variable and date_is_fixed), "Holiday '{}' ({}) in locale {} must not have both flags 'F' and 'V'".format(holiday.description, holiday.date.strftime("%Y-%m-%d"), holiday.locale)
-        assert (date_is_variable or date_is_fixed), "Holiday '{}' ({}) in locale {} must have either flag 'F' or 'V'".format(holiday.description, holiday.date.strftime("%Y-%m-%d"), holiday.locale)
+        assert not (date_is_variable and date_is_fixed), f"Holiday '{holiday.description}' ({holiday.date.strftime('%Y-%m-%d')}) in locale {holiday.locale} must not have both flags 'F' and 'V'"
+        assert (date_is_variable or date_is_fixed), f"Holiday '{holiday.description}' ({holiday.date.strftime('%Y-%m-%d')}) in locale {holiday.locale} must have either flag 'F' or 'V'"
 
 
 def test_holiday_flags_should_be_in_the_correct_order(holidays):
     for holiday in holidays:
-        match = re.search(r"^N?R?[FV]?$", "{}".format(holiday.flags))
+        match = re.search(r"^N?R?[FV]?$", f"{holiday.flags}")
 
-        assert match is not None, "Flags for holiday '{}' ({}) in locale {} are not in the correct order. Flags '{}' should match 'N?R?[FV]?'".format(holiday.description, holiday.date.strftime("%Y-%m-%d"), holiday.locale, holiday.flags)
+        assert match is not None, f"Flags for holiday '{holiday.description}' ({holiday.date.strftime('%Y-%m-%d')}) in locale {holiday.locale} are not in the correct order. Flags '{holiday.flags}' should match 'N?R?[FV]?'"
```

