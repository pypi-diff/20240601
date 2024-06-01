# Comparing `tmp/ovos-skill-wikipedia-0.0.2a2.tar.gz` & `tmp/ovos-skill-wikipedia-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-skill-wikipedia-0.0.2a2.tar", last modified: Sat Jun  1 13:23:30 2024, max compression
+gzip compressed data, was "ovos-skill-wikipedia-0.0.2a3.tar", last modified: Sat Jun  1 13:24:27 2024, max compression
```

## Comparing `ovos-skill-wikipedia-0.0.2a2.tar` & `ovos-skill-wikipedia-0.0.2a3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.311136 ovos-skill-wikipedia-0.0.2a2/
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-06-01 13:23:30.311136 ovos-skill-wikipedia-0.0.2a2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      763 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    24758 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.295136 ovos-skill-wikipedia-0.0.2a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.299136 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/query.intent
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ca-es/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.299136 ovos-skill-wikipedia-0.0.2a2/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/de-de/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/de-de/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/de-de/query.intent
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/de-de/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/de-de/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/de-de/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/de-de/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/de-de/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.303136 ovos-skill-wikipedia-0.0.2a2/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/en-us/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/en-us/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/en-us/query.intent
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/en-us/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/en-us/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/en-us/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/en-us/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/en-us/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.303136 ovos-skill-wikipedia-0.0.2a2/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/es-es/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/es-es/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/es-es/query.intent
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/es-es/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/es-es/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/es-es/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/es-es/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/es-es/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.303136 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/query.intent
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/fr-fr/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.307136 ovos-skill-wikipedia-0.0.2a2/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/it-it/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/it-it/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/it-it/query.intent
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/it-it/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/it-it/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/it-it/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/it-it/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/it-it/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.307136 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/query.intent
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/pt-pt/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.307136 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/More.voc
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/no entry found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/query.intent
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/searching.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/thats all.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/wiki.intent
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/wikiroulette.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/wikiroulette.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.307136 ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-06-01 13:23:30.000000 ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-01 13:23:30.000000 ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:23:30.000000 ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-01 13:23:30.000000 ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 13:23:30.000000 ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 13:23:30.000000 ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/pic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.295136 ovos-skill-wikipedia-0.0.2a2/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.307136 ovos-skill-wikipedia-0.0.2a2/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/res/desktop/skill-wikipedia-for-humans.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/res/desktop/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.307136 ovos-skill-wikipedia-0.0.2a2/res/icon/
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/res/icon/wikipedia.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:23:30.311136 ovos-skill-wikipedia-0.0.2a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2771 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:23:30.311136 ovos-skill-wikipedia-0.0.2a2/ui/
--rw-r--r--   0 runner    (1001) docker     (127)   907480 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/ui/jumping.gif
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 13:23:26.000000 ovos-skill-wikipedia-0.0.2a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.709933 ovos-skill-wikipedia-0.0.2a3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-06-01 13:24:27.705933 ovos-skill-wikipedia-0.0.2a3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)      763 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24758 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.693933 ovos-skill-wikipedia-0.0.2a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.697933 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/query.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ca-es/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.697933 ovos-skill-wikipedia-0.0.2a3/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/de-de/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/de-de/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/de-de/query.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/de-de/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/de-de/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/de-de/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/de-de/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/de-de/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.697933 ovos-skill-wikipedia-0.0.2a3/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/en-us/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/en-us/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/en-us/query.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/en-us/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/en-us/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/en-us/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/en-us/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/en-us/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.697933 ovos-skill-wikipedia-0.0.2a3/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/es-es/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/es-es/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/es-es/query.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/es-es/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/es-es/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/es-es/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/es-es/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/es-es/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.701933 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/query.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/fr-fr/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.701933 ovos-skill-wikipedia-0.0.2a3/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/it-it/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/it-it/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/it-it/query.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/it-it/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/it-it/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/it-it/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/it-it/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/it-it/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.701933 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/query.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/pt-pt/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.705933 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/More.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/no entry found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/query.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/searching.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/thats all.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/wiki.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/wikiroulette.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/wikiroulette.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.705933 ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-06-01 13:24:27.000000 ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-01 13:24:27.000000 ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:24:27.000000 ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-01 13:24:27.000000 ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 13:24:27.000000 ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 13:24:27.000000 ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/pic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.693933 ovos-skill-wikipedia-0.0.2a3/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.705933 ovos-skill-wikipedia-0.0.2a3/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/res/desktop/skill-wikipedia-for-humans.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/res/desktop/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.705933 ovos-skill-wikipedia-0.0.2a3/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/res/icon/wikipedia.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:24:27.709933 ovos-skill-wikipedia-0.0.2a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2771 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:24:27.705933 ovos-skill-wikipedia-0.0.2a3/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)   907480 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/ui/jumping.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 13:24:24.000000 ovos-skill-wikipedia-0.0.2a3/version.py
```

### Comparing `ovos-skill-wikipedia-0.0.2a2/LICENSE` & `ovos-skill-wikipedia-0.0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/PKG-INFO` & `ovos-skill-wikipedia-0.0.2a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-skill-wikipedia
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: ovos wikipedia skill plugin
 Home-page: https://github.com/OpenVoiceOS/skill-ovos-wikipedia
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: ovos skill plugin
 License-File: LICENSE
```

### Comparing `ovos-skill-wikipedia-0.0.2a2/README.md` & `ovos-skill-wikipedia-0.0.2a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/__init__.py` & `ovos-skill-wikipedia-0.0.2a3/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/locale/ca-es/query.intent` & `ovos-skill-wikipedia-0.0.2a3/locale/ca-es/query.intent`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/locale/ca-es/wikiroulette.intent` & `ovos-skill-wikipedia-0.0.2a3/locale/ca-es/wikiroulette.intent`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/locale/ru-ru/query.intent` & `ovos-skill-wikipedia-0.0.2a3/locale/ru-ru/query.intent`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/PKG-INFO` & `ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-skill-wikipedia
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: ovos wikipedia skill plugin
 Home-page: https://github.com/OpenVoiceOS/skill-ovos-wikipedia
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: ovos skill plugin
 License-File: LICENSE
```

### Comparing `ovos-skill-wikipedia-0.0.2a2/ovos_skill_wikipedia.egg-info/SOURCES.txt` & `ovos-skill-wikipedia-0.0.2a3/ovos_skill_wikipedia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/res/desktop/skill.json` & `ovos-skill-wikipedia-0.0.2a3/res/desktop/skill.json`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/res/icon/wikipedia.png` & `ovos-skill-wikipedia-0.0.2a3/res/icon/wikipedia.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/setup.py` & `ovos-skill-wikipedia-0.0.2a3/setup.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-wikipedia-0.0.2a2/ui/jumping.gif` & `ovos-skill-wikipedia-0.0.2a3/ui/jumping.gif`

 * *Files identical despite different names*

