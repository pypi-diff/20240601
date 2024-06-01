# Comparing `tmp/genshin-1.7.0.tar.gz` & `tmp/genshin-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genshin-1.7.0.tar", last modified: Thu May 30 13:06:04 2024, max compression
+gzip compressed data, was "genshin-1.7.1.tar", last modified: Sat Jun  1 12:58:15 2024, max compression
```

## Comparing `genshin-1.7.0.tar` & `genshin-1.7.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.928471 genshin-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-30 13:06:00.000000 genshin-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-30 13:06:04.928471 genshin-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-30 13:06:00.000000 genshin-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.908470 genshin-1.7.0/genshin/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.912471 genshin-1.7.0/genshin/client/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.912471 genshin-1.7.0/genshin/client/components/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.912471 genshin-1.7.0/genshin/client/components/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/client/components/auth/subclients/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/subclients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/subclients/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/subclients/game.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/auth/subclients/web.py
--rw-r--r--   0 runner    (1001) docker     (127)    21107 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/client/components/calculator/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/calculator/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/calculator/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/client/components/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/genshin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/honkai.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/chronicle/starrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/diary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/hoyolab.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/lineup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/teapot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/components/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/client/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/manager/cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)    17675 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/manager/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/client/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.916471 genshin-1.7.0/genshin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.920471 genshin-1.7.0/genshin/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/geetest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/qrcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/auth/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.920471 genshin-1.7.0/genshin/models/genshin/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/character.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.920471 genshin-1.7.0/genshin/models/genshin/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/abyss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/chronicle/tcg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/diary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/lineup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/teapot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/genshin/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.920471 genshin-1.7.0/genshin/models/honkai/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/battlesuit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/models/honkai/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/chronicle/battlesuits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/chronicle/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/chronicle/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/honkai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/models/hoyolab/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/hoyolab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/hoyolab/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/hoyolab/private.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/hoyolab/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/models/starrail/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/character.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/models/starrail/chronicle/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/rogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/models/starrail/chronicle/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.924471 genshin-1.7.0/genshin/paginators/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/paginators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/paginators/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/paginators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.928471 genshin-1.7.0/genshin/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/ds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/extdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/logfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-30 13:06:00.000000 genshin-1.7.0/genshin/utility/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.928471 genshin-1.7.0/genshin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 13:06:04.000000 genshin-1.7.0/genshin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-30 13:06:00.000000 genshin-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:06:04.928471 genshin-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 13:06:00.000000 genshin-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:04.928471 genshin-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:06:00.000000 genshin-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-30 13:06:00.000000 genshin-1.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-30 13:06:00.000000 genshin-1.7.0/tests/test_paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.841907 genshin-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-01 12:58:12.000000 genshin-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-06-01 12:58:15.837907 genshin-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-06-01 12:58:12.000000 genshin-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.821907 genshin-1.7.1/genshin/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.821907 genshin-1.7.1/genshin/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.825907 genshin-1.7.1/genshin/client/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.825907 genshin-1.7.1/genshin/client/components/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13514 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/auth/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.825907 genshin-1.7.1/genshin/client/components/auth/subclients/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/auth/subclients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/auth/subclients/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/auth/subclients/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/auth/subclients/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21107 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.825907 genshin-1.7.1/genshin/client/components/calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14697 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/calculator/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/calculator/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.825907 genshin-1.7.1/genshin/client/components/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/chronicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/chronicle/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/chronicle/genshin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/chronicle/honkai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/chronicle/starrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/hoyolab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/teapot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/components/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.829907 genshin-1.7.1/genshin/client/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/manager/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17452 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/manager/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/client/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.829907 genshin-1.7.1/genshin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.829907 genshin-1.7.1/genshin/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/auth/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/auth/geetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/auth/qrcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/auth/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/auth/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.829907 genshin-1.7.1/genshin/models/genshin/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.833907 genshin-1.7.1/genshin/models/genshin/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/chronicle/abyss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/chronicle/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/chronicle/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/chronicle/notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/chronicle/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/chronicle/tcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/diary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/lineup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/teapot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/genshin/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.833907 genshin-1.7.1/genshin/models/honkai/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/honkai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/honkai/battlesuit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.833907 genshin-1.7.1/genshin/models/honkai/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/honkai/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/honkai/chronicle/battlesuits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/honkai/chronicle/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/honkai/chronicle/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/honkai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.833907 genshin-1.7.1/genshin/models/hoyolab/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/hoyolab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/hoyolab/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/hoyolab/private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/hoyolab/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.833907 genshin-1.7.1/genshin/models/starrail/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.837907 genshin-1.7.1/genshin/models/starrail/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/chronicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/chronicle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/chronicle/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/chronicle/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/chronicle/notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/chronicle/rogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/models/starrail/chronicle/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.837907 genshin-1.7.1/genshin/paginators/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/paginators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/paginators/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/paginators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.837907 genshin-1.7.1/genshin/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/extdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/logfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-06-01 12:58:12.000000 genshin-1.7.1/genshin/utility/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.837907 genshin-1.7.1/genshin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-06-01 12:58:15.000000 genshin-1.7.1/genshin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-06-01 12:58:15.000000 genshin-1.7.1/genshin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 12:58:15.000000 genshin-1.7.1/genshin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 12:58:15.000000 genshin-1.7.1/genshin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 12:58:15.000000 genshin-1.7.1/genshin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-06-01 12:58:12.000000 genshin-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 12:58:15.841907 genshin-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-06-01 12:58:12.000000 genshin-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:15.837907 genshin-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 12:58:12.000000 genshin-1.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-06-01 12:58:12.000000 genshin-1.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-06-01 12:58:12.000000 genshin-1.7.1/tests/test_paginators.py
```

### Comparing `genshin-1.7.0/LICENSE` & `genshin-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/PKG-INFO` & `genshin-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin
-Version: 1.7.0
+Version: 1.7.1
 Summary: An API wrapper for Genshin Impact.
 Home-page: https://github.com/thesadru/genshin.py
 Author: thesadru
 Author-email: thesadru@gmail.com
 License: MIT
 Project-URL: Documentation, https://thesadru.github.io/genshin.py
 Project-URL: Issue tracker, https://github.com/thesadru/genshin.py/issues
```

### Comparing `genshin-1.7.0/README.md` & `genshin-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/__main__.py` & `genshin-1.7.1/genshin/__main__.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/cache.py` & `genshin-1.7.1/genshin/client/cache.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/clients.py` & `genshin-1.7.1/genshin/client/clients.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/compatibility.py` & `genshin-1.7.1/genshin/client/compatibility.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/auth/client.py` & `genshin-1.7.1/genshin/client/components/auth/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 
 import asyncio
 import logging
 import typing
 
 import aiohttp
 
-from genshin import errors, types
+from genshin import constants, errors, types
 from genshin.client import routes
 from genshin.client.components import base
 from genshin.client.manager import managers
 from genshin.client.manager.cookie import fetch_cookie_token_with_game_token, fetch_stoken_with_game_token
 from genshin.models.auth.cookie import (
     AppLoginResult,
     CNWebLoginResult,
     GameLoginResult,
     MobileLoginResult,
     QRLoginResult,
     WebLoginResult,
 )
-from genshin.models.auth.geetest import MMT, RiskyCheckMMT, RiskyCheckMMTResult, SessionMMT, SessionMMTResult
+from genshin.models.auth.geetest import MMT, MMTResult, RiskyCheckMMT, RiskyCheckMMTResult, SessionMMT, SessionMMTResult
 from genshin.models.auth.qrcode import QRCodeStatus
 from genshin.models.auth.verification import ActionTicket
-from genshin.types import Game
 from genshin.utility import auth as auth_utility
 from genshin.utility import ds as ds_utility
 
 from . import server, subclients
 
 __all__ = ["AuthClient"]
 
@@ -269,40 +268,65 @@
             "account_id": stoken.aid,
             "ltmid": stoken.mid,
             "cookie_token": cookie_token,
         }
         self.set_cookies(cookies)
         return QRLoginResult(**cookies)
 
-    @base.region_specific(types.Region.CHINESE)
     @managers.no_multi
     async def create_mmt(self) -> MMT:
         """Create a geetest challenge."""
-        is_genshin = self.game is Game.GENSHIN
+        if self.default_game is None:
+            raise ValueError("No default game set.")
+
         headers = {
-            "DS": ds_utility.generate_create_geetest_ds(),
-            "x-rpc-challenge_game": "2" if is_genshin else "6",
-            "x-rpc-page": "v4.1.5-ys_#ys" if is_genshin else "v1.4.1-rpg_#/rpg",
-            "x-rpc-tool-verison": "v4.1.5-ys" if is_genshin else "v1.4.1-rpg",
-            **auth_utility.CREATE_MMT_HEADERS,
+            "DS": ds_utility.generate_geetest_ds(self.region),
+            **auth_utility.CREATE_MMT_HEADERS[self.region],
         }
 
+        url = routes.CREATE_MMT_URL.get_url(self.region)
+        if self.region is types.Region.OVERSEAS:
+            url = url.update_query(app_key=constants.GEETEST_RECORD_KEYS[self.default_game])
+
         assert isinstance(self.cookie_manager, managers.CookieManager)
         async with self.cookie_manager.create_session() as session:
-            async with session.get(
-                routes.CREATE_MMT_URL.get_url(), headers=headers, cookies=self.cookie_manager.cookies
-            ) as r:
+            async with session.get(url, headers=headers, cookies=self.cookie_manager.cookies) as r:
                 data = await r.json()
 
         if not data["data"]:
             errors.raise_for_retcode(data)
 
         return MMT(**data["data"])
 
     @base.region_specific(types.Region.OVERSEAS)
+    @managers.no_multi
+    async def verify_mmt(self, mmt_result: MMTResult) -> None:
+        """Verify a geetest challenge."""
+        if self.default_game is None:
+            raise ValueError("No default game set.")
+
+        headers = {
+            "DS": ds_utility.generate_geetest_ds(self.region),
+            **auth_utility.CREATE_MMT_HEADERS[self.region],
+        }
+
+        body = mmt_result.dict()
+        body["app_key"] = constants.GEETEST_RECORD_KEYS[self.default_game]
+
+        assert isinstance(self.cookie_manager, managers.CookieManager)
+        async with self.cookie_manager.create_session() as session:
+            async with session.post(
+                routes.VERIFY_MMT_URL.get_url(), json=body, headers=headers, cookies=self.cookie_manager.cookies
+            ) as r:
+                data = await r.json()
+
+        if not data["data"]:
+            errors.raise_for_retcode(data)
+
+    @base.region_specific(types.Region.OVERSEAS)
     async def os_game_login(
         self,
         account: str,
         password: str,
         *,
         encrypted: bool = False,
         port: int = 5000,
```

### Comparing `genshin-1.7.0/genshin/client/components/auth/server.py` & `genshin-1.7.1/genshin/client/components/auth/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     SessionMMTv4,
     SessionMMTv4Result,
 )
 from genshin.utility import auth as auth_utility
 
 __all__ = ["PAGES", "enter_code", "launch_webapp", "solve_geetest"]
 
-PAGES: typing.Final[typing.Dict[typing.Literal["captcha", "captcha-v4", "enter-code"], str]] = {
+PAGES: typing.Final[typing.Dict[typing.Literal["captcha", "enter-code"], str]] = {
     "captcha": """
     <!DOCTYPE html>
     <head>
       <meta name="referrer" content="no-referrer"/>
     </head>
     <html>
       <body></body>
@@ -40,33 +40,33 @@
         fetch("/mmt")
           .then((response) => response.json())
           .then((mmt) => {
             const initParams = geetestVersion === 3 ? {
               gt: mmt.gt,
               challenge: mmt.challenge,
               new_captcha: mmt.new_captcha,
-              api_server: '{api_server}',
+              api_server: "{api_server}",
               https: /^https/i.test(window.location.protocol),
               product: "bind",
-              lang: '{lang}',
+              lang: "{lang}",
             } : {
               captchaId: mmt.gt,
               riskType: mmt.risk_type,
               userInfo: mmt.session_id ? JSON.stringify({
                 mmt_key: mmt.session_id
               }) : undefined,
-              api_server: '{api_server}',
+              api_server: "{api_server}",
               product: "bind",
-              language: '{lang}',
+              language: "{lang}",
             };
             initGeetest(
               initParams,
               (captcha) => {
                 captcha.onReady(() => {
-                  captcha.verify();
+                  geetestVersion == 3 ? captcha.verify() : captcha.showCaptcha();
                 });
                 captcha.onSuccess(() => {
                   fetch("/send-data", {
                     method: "POST",
                     body: JSON.stringify({
                       ...(mmt.session_id && {session_id: mmt.session_id}),
                       ...(mmt.check_id && {check_id: mmt.check_id}),
```

### Comparing `genshin-1.7.0/genshin/client/components/auth/subclients/app.py` & `genshin-1.7.1/genshin/client/components/auth/subclients/app.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/auth/subclients/game.py` & `genshin-1.7.1/genshin/client/components/auth/subclients/game.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/auth/subclients/web.py` & `genshin-1.7.1/genshin/client/components/auth/subclients/web.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/base.py` & `genshin-1.7.1/genshin/client/components/base.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/calculator/calculator.py` & `genshin-1.7.1/genshin/client/components/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/calculator/client.py` & `genshin-1.7.1/genshin/client/components/calculator/client.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/chronicle/base.py` & `genshin-1.7.1/genshin/client/components/chronicle/base.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/chronicle/genshin.py` & `genshin-1.7.1/genshin/client/components/chronicle/genshin.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/chronicle/honkai.py` & `genshin-1.7.1/genshin/client/components/chronicle/honkai.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/chronicle/starrail.py` & `genshin-1.7.1/genshin/client/components/chronicle/starrail.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/daily.py` & `genshin-1.7.1/genshin/client/components/daily.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/diary.py` & `genshin-1.7.1/genshin/client/components/diary.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/gacha.py` & `genshin-1.7.1/genshin/client/components/gacha.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/hoyolab.py` & `genshin-1.7.1/genshin/client/components/hoyolab.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/lineup.py` & `genshin-1.7.1/genshin/client/components/lineup.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/teapot.py` & `genshin-1.7.1/genshin/client/components/teapot.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/transaction.py` & `genshin-1.7.1/genshin/client/components/transaction.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/components/wiki.py` & `genshin-1.7.1/genshin/client/components/wiki.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/manager/cookie.py` & `genshin-1.7.1/genshin/client/manager/cookie.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/manager/managers.py` & `genshin-1.7.1/genshin/client/manager/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 import aiohttp.typedefs
 import yarl
 
 from genshin import errors, types
 from genshin.client import ratelimit
 from genshin.utility import fs as fs_utility
 
-from ...constants import MIYOUSHE_GEETEST_RETCODES
-
 _LOGGER = logging.getLogger(__name__)
 
 __all__ = [
     "BaseCookieManager",
     "CookieManager",
     "InternationalCookieManager",
     "RotatingCookieManager",
@@ -151,17 +149,14 @@
                     new_keys = new_cookies.keys() - cookies.keys()
                     if new_keys:
                         cookies.update(new_cookies)
                         _LOGGER.debug("Updating cookies for %s: %s", get_cookie_identifier(cookies), new_keys)
 
         errors.check_for_geetest(data)
 
-        if data["retcode"] in MIYOUSHE_GEETEST_RETCODES:
-            raise errors.MiyousheGeetestError(data, {k: morsel.value for k, morsel in response.cookies.items()})
-
         if data["retcode"] == 0:
             return data["data"]
 
         errors.raise_for_retcode(data)
 
     @abc.abstractmethod
     async def request(
```

### Comparing `genshin-1.7.0/genshin/client/ratelimit.py` & `genshin-1.7.1/genshin/client/ratelimit.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/client/routes.py` & `genshin-1.7.1/genshin/client/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "LINEUP_URL",
     "MI18N",
     "RECORD_URL",
     "REWARD_URL",
     "TAKUMI_URL",
     "TEAPOT_URL",
     "VERIFY_EMAIL_URL",
+    "VERIFY_MMT_URL",
     "WEBAPI_URL",
     "WEBSTATIC_URL",
     "WEB_LOGIN_URL",
     "YSULOG_URL",
     "Route",
 ]
 
@@ -197,15 +198,15 @@
         hkrpg="https://sg-hkrpg-api.hoyoverse.com/common/apicdkey/api/webExchangeCdkey",
     ),
     chinese=dict(),
 )
 
 GACHA_URL = GameRoute(
     overseas=dict(
-        genshin="https://hk4e-api-os.hoyoverse.com/event/gacha_info/api/",
+        genshin="https://hk4e-api-os.hoyoverse.com/gacha_info/api/",
         hkrpg="https://api-os-takumi.mihoyo.com/common/gacha_record/api/",
     ),
     chinese=dict(
         genshin="https://hk4e-api.mihoyo.com/event/gacha_info/api/",
         hkrpg="https://api-takumi.mihoyo.com/common/gacha_record/api/",
     ),
 )
@@ -235,18 +236,21 @@
 CHECK_MOBILE_VALIDITY_URL = Route("https://webapi.account.mihoyo.com/Api/is_mobile_registrable")
 MOBILE_OTP_URL = Route("https://passport-api.miyoushe.com/account/ma-cn-verifier/verifier/createLoginCaptcha")
 MOBILE_LOGIN_URL = Route("https://passport-api.miyoushe.com/account/ma-cn-passport/web/loginByMobileCaptcha")
 
 CREATE_QRCODE_URL = Route("https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/panda/qrcode/fetch")
 CHECK_QRCODE_URL = Route("https://hk4e-sdk.mihoyo.com/hk4e_cn/combo/panda/qrcode/query")
 
-CREATE_MMT_URL = Route(
-    "https://api-takumi-record.mihoyo.com/game_record/app/card/wapi/createVerification?is_high=false"
+CREATE_MMT_URL = InternationalRoute(
+    overseas="https://sg-public-api.hoyolab.com/event/toolcomsrv/risk/createGeetest?is_high=true",
+    chinese="https://api-takumi-record.mihoyo.com/game_record/app/card/wapi/createVerification?is_high=false",
 )
 
+VERIFY_MMT_URL = Route("https://sg-public-api.hoyolab.com/event/toolcomsrv/risk/verifyGeetest")
+
 GAME_RISKY_CHECK_URL = InternationalRoute(
     overseas="https://api-account-os.hoyoverse.com/account/risky/api/check",
     chinese="https://gameapi-account.mihoyo.com/account/risky/api/check",
 )
 
 SHIELD_LOGIN_URL = GameRoute(
     overseas=dict(
```

### Comparing `genshin-1.7.0/genshin/constants.py` & `genshin-1.7.1/genshin/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Constants hardcoded for optimizations."""
 
 from . import types
 
-__all__ = ["LANGS"]
+__all__ = ["APP_IDS", "APP_KEYS", "DS_SALT", "GEETEST_RETCODES", "LANGS"]
 
 
 LANGS = {
     "zh-cn": "简体中文",
     "zh-tw": "繁體中文",
     "de-de": "Deutsch",
     "en-us": "English",
@@ -29,16 +29,16 @@
     types.Region.CHINESE: "xV8v4Qu54lUKrEYFZkJhB8cuOh9Asafs",
     "app_login": "IZPgfb0dRPtBeLuFkdDznSZ6f4wWt6y2",
     "cn_signin": "LyD1rXqMv2GJhnwdvCBjFOKGiKuLY3aO",
     "cn_passport": "JwYDpKvLj6MrMqqYU6jTKF17KNO2PXoS",
 }
 """Dynamic Secret Salts."""
 
-MIYOUSHE_GEETEST_RETCODES = {10035, 5003, 10041, 1034}
-"""API error codes that indicate a Geetest was triggered during this Miyoushe API request."""
+GEETEST_RETCODES = {10035, 5003, 10041, 1034}
+"""API error codes that indicate a Geetest was triggered during the API request."""
 
 APP_KEYS = {
     types.Game.GENSHIN: {
         types.Region.OVERSEAS: "6a4c78fe0356ba4673b8071127b28123",
         types.Region.CHINESE: "d0d3a7342df2026a70f650b907800111",
     },
     types.Game.STARRAIL: {
@@ -71,7 +71,15 @@
     },
     types.Game.ZZZ: {
         types.Region.OVERSEAS: "15",
         types.Region.CHINESE: "12",
     },
 }
 """App IDs used for game login."""
+
+GEETEST_RECORD_KEYS = {
+    types.Game.GENSHIN: "hk4e_game_record",
+    types.Game.STARRAIL: "hkrpg_game_record",
+    types.Game.HONKAI: "bh3_game_record",
+    types.Game.ZZZ: "nap_game_record",
+}
+"""Keys used to submit geetest result."""
```

### Comparing `genshin-1.7.0/genshin/errors.py` & `genshin-1.7.1/genshin/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Errors received from the API."""
 
 import typing
 
+from genshin.constants import GEETEST_RETCODES
+
 __all__ = [
     "ERRORS",
     "AccountNotFound",
     "AlreadyClaimed",
     "AuthkeyException",
     "AuthkeyTimeout",
     "CookieException",
+    "DailyGeetestTriggered",
     "DataNotPublic",
-    "GeetestTriggered",
+    "GeetestError",
     "GenshinException",
     "InvalidAuthkey",
     "InvalidCookies",
-    "MiyousheGeetestError",
     "RedemptionClaimed",
     "RedemptionCooldown",
     "RedemptionException",
     "RedemptionInvalid",
     "TooManyRequests",
     "check_for_geetest",
     "raise_for_retcode",
@@ -110,16 +112,16 @@
 class AlreadyClaimed(GenshinException):
     """Already claimed the daily reward today."""
 
     retcode = -5003
     msg = "Already claimed the daily reward today."
 
 
-class GeetestTriggered(GenshinException):
-    """Geetest triggered."""
+class DailyGeetestTriggered(GenshinException):
+    """Geetest triggered during daily reward claim."""
 
     msg = "Geetest triggered during daily reward claim."
 
     gt: str
     challenge: str
 
     def __init__(self, response: typing.Mapping[str, typing.Any], *, gt: str, challenge: str) -> None:
@@ -183,26 +185,21 @@
 
 class WrongOTP(GenshinException):
     """Wrong OTP code."""
 
     msg = "The provided OTP code is wrong."
 
 
-class MiyousheGeetestError(GenshinException):
-    """Geetest triggered during Miyoushe API request."""
+class GeetestError(GenshinException):
+    """Geetest triggered during the battle chronicle API request."""
 
-    def __init__(
-        self,
-        response: typing.Dict[str, typing.Any],
-        cookies: typing.Mapping[str, str],
-    ) -> None:
-        self.cookies = cookies
+    def __init__(self, response: typing.Dict[str, typing.Any]) -> None:
         super().__init__(response)
 
-    msg = "Geetest triggered during Miyoushe API request."
+    msg = "Geetest triggered during the battle chronicle API request."
 
 
 class OTPRateLimited(GenshinException):
     """Too many OTP messages sent for the number.
 
     The limit is 40 messages/day/number.
     """
@@ -336,21 +333,24 @@
 
     if "redemption" in m:
         raise RedemptionException(data)
 
     raise GenshinException(data)
 
 
-def check_for_geetest(response: typing.Dict[str, typing.Any]) -> None:
-    """Check if geetest was triggered and raise an error."""
-    if not response.get("data"):  # if is an error
+def check_for_geetest(data: typing.Dict[str, typing.Any]) -> None:
+    """Check if geetest was triggered during the request and raise an error if so."""
+    if data["retcode"] in GEETEST_RETCODES:
+        raise GeetestError(data)
+
+    if not data.get("data"):  # if is an error
         return
 
-    gt_result = response["data"].get("gt_result", response["data"])
+    gt_result = data["data"].get("gt_result", data["data"])
 
     if (
         gt_result.get("risk_code") != 0
         and gt_result.get("gt")
         and gt_result.get("challenge")
         and gt_result.get("success") != 0
     ):
-        raise GeetestTriggered(response, gt=gt_result.get("gt"), challenge=gt_result.get("challenge"))
+        raise DailyGeetestTriggered(data, gt=gt_result.get("gt"), challenge=gt_result.get("challenge"))
```

### Comparing `genshin-1.7.0/genshin/models/auth/cookie.py` & `genshin-1.7.1/genshin/models/auth/cookie.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/auth/geetest.py` & `genshin-1.7.1/genshin/models/auth/geetest.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/auth/qrcode.py` & `genshin-1.7.1/genshin/models/auth/qrcode.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/auth/responses.py` & `genshin-1.7.1/genshin/models/auth/responses.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/auth/verification.py` & `genshin-1.7.1/genshin/models/auth/verification.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/calculator.py` & `genshin-1.7.1/genshin/models/genshin/calculator.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/character.py` & `genshin-1.7.1/genshin/models/genshin/character.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/chronicle/abyss.py` & `genshin-1.7.1/genshin/models/genshin/chronicle/abyss.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/chronicle/activities.py` & `genshin-1.7.1/genshin/models/genshin/chronicle/activities.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/chronicle/characters.py` & `genshin-1.7.1/genshin/models/genshin/chronicle/characters.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/chronicle/notes.py` & `genshin-1.7.1/genshin/models/genshin/chronicle/notes.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/chronicle/stats.py` & `genshin-1.7.1/genshin/models/genshin/chronicle/stats.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/chronicle/tcg.py` & `genshin-1.7.1/genshin/models/genshin/chronicle/tcg.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/constants.py` & `genshin-1.7.1/genshin/models/genshin/constants.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/daily.py` & `genshin-1.7.1/genshin/models/genshin/daily.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/diary.py` & `genshin-1.7.1/genshin/models/genshin/diary.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/gacha.py` & `genshin-1.7.1/genshin/models/genshin/gacha.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/lineup.py` & `genshin-1.7.1/genshin/models/genshin/lineup.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/teapot.py` & `genshin-1.7.1/genshin/models/genshin/teapot.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/transaction.py` & `genshin-1.7.1/genshin/models/genshin/transaction.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/genshin/wiki.py` & `genshin-1.7.1/genshin/models/genshin/wiki.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/honkai/battlesuit.py` & `genshin-1.7.1/genshin/models/honkai/battlesuit.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/honkai/chronicle/battlesuits.py` & `genshin-1.7.1/genshin/models/honkai/chronicle/battlesuits.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/honkai/chronicle/modes.py` & `genshin-1.7.1/genshin/models/honkai/chronicle/modes.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/honkai/chronicle/stats.py` & `genshin-1.7.1/genshin/models/honkai/chronicle/stats.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/honkai/constants.py` & `genshin-1.7.1/genshin/models/honkai/constants.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/hoyolab/announcements.py` & `genshin-1.7.1/genshin/models/hoyolab/announcements.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/hoyolab/record.py` & `genshin-1.7.1/genshin/models/hoyolab/record.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/model.py` & `genshin-1.7.1/genshin/models/model.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/starrail/character.py` & `genshin-1.7.1/genshin/models/starrail/character.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/starrail/chronicle/challenge.py` & `genshin-1.7.1/genshin/models/starrail/chronicle/challenge.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/starrail/chronicle/characters.py` & `genshin-1.7.1/genshin/models/starrail/chronicle/characters.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/starrail/chronicle/notes.py` & `genshin-1.7.1/genshin/models/starrail/chronicle/notes.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/starrail/chronicle/rogue.py` & `genshin-1.7.1/genshin/models/starrail/chronicle/rogue.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/models/starrail/chronicle/stats.py` & `genshin-1.7.1/genshin/models/starrail/chronicle/stats.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/paginators/api.py` & `genshin-1.7.1/genshin/paginators/api.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/paginators/base.py` & `genshin-1.7.1/genshin/paginators/base.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/types.py` & `genshin-1.7.1/genshin/types.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/utility/auth.py` & `genshin-1.7.1/genshin/utility/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import base64
 import hmac
 import json
 import typing
 from hashlib import sha256
 
-from genshin import constants
+from genshin import constants, types
 
 __all__ = ["encrypt_credentials", "generate_sign"]
 
 
 # RSA key used for OS app/web login
 LOGIN_KEY_TYPE_1 = b"""
 -----BEGIN PUBLIC KEY-----
@@ -66,16 +66,27 @@
 
 EMAIL_VERIFY_HEADERS = {
     "x-rpc-app_id": "c9oqaq3s3gu8",
     "x-rpc-client_type": "2",
 }
 
 CREATE_MMT_HEADERS = {
-    "x-rpc-app_version": "2.60.1",
-    "x-rpc-client_type": "5",
+    types.Region.OVERSEAS: {
+        "x-rpc-challenge_path": "https://bbs-api-os.hoyolab.com/game_record/app/hkrpg/api/challenge",
+        "x-rpc-app_version": "2.55.0",
+        "x-rpc-challenge_game": "6",
+        "x-rpc-client_type": "5",
+    },
+    types.Region.CHINESE: {
+        "x-rpc-app_version": "2.60.1",
+        "x-rpc-client_type": "5",
+        "x-rpc-challenge_game": "6",
+        "x-rpc-page": "v1.4.1-rpg_#/rpg",
+        "x-rpc-tool-version": "v1.4.1-rpg",
+    },
 }
 
 DEVICE_ID = "D6AF5103-D297-4A01-B86A-87F87DS5723E"
 
 RISKY_CHECK_HEADERS = {
     "x-rpc-client_type": "1",
     "x-rpc-channel_id": "1",
```

### Comparing `genshin-1.7.0/genshin/utility/concurrency.py` & `genshin-1.7.1/genshin/utility/concurrency.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/utility/deprecation.py` & `genshin-1.7.1/genshin/utility/deprecation.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/utility/ds.py` & `genshin-1.7.1/genshin/utility/ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import time
 import typing
 
 from genshin import constants, types
 
 __all__ = [
     "generate_cn_dynamic_secret",
-    "generate_create_geetest_ds",
     "generate_dynamic_secret",
+    "generate_geetest_ds",
     "generate_passport_ds",
     "get_ds_headers",
 ]
 
 
 def generate_dynamic_secret(salt: str = constants.DS_SALT[types.Region.OVERSEAS]) -> str:
     """Create a new overseas dynamic secret."""
@@ -74,14 +74,13 @@
     r = "".join(random.sample(string.ascii_letters, 6))
     b = json.dumps(body)
     h = hashlib.md5(f"salt={salt}&t={t}&r={r}&b={b}&q=".encode()).hexdigest()
     result = f"{t},{r},{h}"
     return result
 
 
-def generate_create_geetest_ds() -> str:
-    """Create a dynamic secret for Miyoushe createVerification API endpoint."""
-    salt = constants.DS_SALT[types.Region.CHINESE]
+def generate_geetest_ds(region: types.Region) -> str:
+    """Create a dynamic secret for geetest API endpoint."""
     t = int(time.time())
     r = random.randint(100000, 200000)
-    h = hashlib.md5(f"salt={salt}&t={t}&r={r}&b=&q=is_high=false".encode()).hexdigest()
+    h = hashlib.md5(f"salt={constants.DS_SALT[region]}&t={t}&r={r}&b=&q=is_high=false".encode()).hexdigest()
     return f"{t},{r},{h}"
```

### Comparing `genshin-1.7.0/genshin/utility/extdb.py` & `genshin-1.7.1/genshin/utility/extdb.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/utility/fs.py` & `genshin-1.7.1/genshin/utility/fs.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/utility/logfile.py` & `genshin-1.7.1/genshin/utility/logfile.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin/utility/uid.py` & `genshin-1.7.1/genshin/utility/uid.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/genshin.egg-info/PKG-INFO` & `genshin-1.7.1/genshin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin
-Version: 1.7.0
+Version: 1.7.1
 Summary: An API wrapper for Genshin Impact.
 Home-page: https://github.com/thesadru/genshin.py
 Author: thesadru
 Author-email: thesadru@gmail.com
 License: MIT
 Project-URL: Documentation, https://thesadru.github.io/genshin.py
 Project-URL: Issue tracker, https://github.com/thesadru/genshin.py/issues
```

### Comparing `genshin-1.7.0/genshin.egg-info/SOURCES.txt` & `genshin-1.7.1/genshin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/pyproject.toml` & `genshin-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/setup.py` & `genshin-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Run setuptools."""
 
 from setuptools import find_packages, setup
 
 setup(
     name="genshin",
-    version="1.7.0",
+    version="1.7.1",
     author="thesadru",
     author_email="thesadru@gmail.com",
     description="An API wrapper for Genshin Impact.",
     keywords="hoyoverse mihoyo genshin genshin-impact honkai".split(),
     url="https://github.com/thesadru/genshin.py",
     project_urls={
         "Documentation": "https://thesadru.github.io/genshin.py",
```

### Comparing `genshin-1.7.0/tests/conftest.py` & `genshin-1.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `genshin-1.7.0/tests/test_paginators.py` & `genshin-1.7.1/tests/test_paginators.py`

 * *Files identical despite different names*

