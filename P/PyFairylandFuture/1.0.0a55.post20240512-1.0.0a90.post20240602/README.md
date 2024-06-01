# Comparing `tmp/pyfairylandfuture-1.0.0a55.post20240512.tar.gz` & `tmp/pyfairylandfuture-1.0.0a90.post20240602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfairylandfuture-1.0.0a55.post20240512.tar", last modified: Sun May 12 03:38:50 2024, max compression
+gzip compressed data, was "pyfairylandfuture-1.0.0a90.post20240602.tar", last modified: Sat Jun  1 16:37:30 2024, max compression
```

## Comparing `pyfairylandfuture-1.0.0a55.post20240512.tar` & `pyfairylandfuture-1.0.0a90.post20240602.tar`

### file list

```diff
@@ -1,48 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.576389 pyfairylandfuture-1.0.0a55.post20240512/
--rw-rw-rw-   0        0        0    34523 2024-05-09 08:14:38.000000 pyfairylandfuture-1.0.0a55.post20240512/LICENSE.txt
--rw-rw-rw-   0        0        0     7883 2024-05-12 03:38:50.574396 pyfairylandfuture-1.0.0a55.post20240512/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.573398 pyfairylandfuture-1.0.0a55.post20240512/PyFairylandFuture.egg-info/
--rw-rw-rw-   0        0        0     7883 2024-05-12 03:38:50.000000 pyfairylandfuture-1.0.0a55.post20240512/PyFairylandFuture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1087 2024-05-12 03:38:50.000000 pyfairylandfuture-1.0.0a55.post20240512/PyFairylandFuture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 03:38:50.000000 pyfairylandfuture-1.0.0a55.post20240512/PyFairylandFuture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-12 03:38:50.000000 pyfairylandfuture-1.0.0a55.post20240512/PyFairylandFuture.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-12 03:38:50.000000 pyfairylandfuture-1.0.0a55.post20240512/PyFairylandFuture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5860 2024-05-11 08:08:29.000000 pyfairylandfuture-1.0.0a55.post20240512/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.544474 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/
--rw-rw-rw-   0        0        0      180 2024-05-09 08:15:49.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.545471 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/api/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:43:16.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.547466 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/common/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:44:07.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.548463 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/conf/
--rw-rw-rw-   0        0        0      180 2024-05-11 10:55:48.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.551456 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/constants/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:44:31.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/constants/__init__.py
--rw-rw-rw-   0        0        0     1506 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/constants/enums.py
--rw-rw-rw-   0        0        0      314 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/constants/typed.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.552452 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/core/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:43:29.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.556442 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/core/abstracts/
--rw-rw-rw-   0        0        0      180 2024-05-10 02:45:56.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/core/abstracts/__init__.py
--rw-rw-rw-   0        0        0     3363 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/core/abstracts/enumerate.py
--rw-rw-rw-   0        0        0     1157 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/core/abstracts/metaclass.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.562426 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/modules/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:46:13.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/modules/__init__.py
--rw-rw-rw-   0        0        0     3940 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/modules/datetimes.py
--rw-rw-rw-   0        0        0     5715 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/modules/decorators.py
--rw-rw-rw-   0        0        0     1249 2024-05-10 03:40:57.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/modules/exceptions.py
--rw-rw-rw-   0        0        0     6486 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/modules/journal.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.563423 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/scripts/
--rw-rw-rw-   0        0        0      180 2024-05-11 09:20:11.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.565419 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/test/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:32:02.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.566417 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/
--rw-rw-rw-   0        0        0      180 2024-05-09 10:43:16.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.569407 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/general/
--rw-rw-rw-   0        0        0      180 2024-05-10 02:26:32.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/general/__init__.py
--rw-rw-rw-   0        0        0     6145 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/general/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-12 03:38:50.571402 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/verifies/
--rw-rw-rw-   0        0        0      180 2024-05-10 10:55:57.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/verifies/__init__.py
--rw-rw-rw-   0        0        0     1635 2024-05-12 03:11:08.000000 pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/verifies/validate.py
--rw-rw-rw-   0        0        0       42 2024-05-12 03:38:50.576389 pyfairylandfuture-1.0.0a55.post20240512/setup.cfg
--rw-rw-rw-   0        0        0     8662 2024-05-12 03:28:11.000000 pyfairylandfuture-1.0.0a55.post20240512/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:30.051241 pyfairylandfuture-1.0.0a90.post20240602/
+-rw-rw-rw-   0        0        0    34523 2024-05-11 18:24:45.000000 pyfairylandfuture-1.0.0a90.post20240602/LICENSE.txt
+-rw-rw-rw-   0        0        0     8035 2024-06-01 16:37:30.047242 pyfairylandfuture-1.0.0a90.post20240602/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:30.045239 pyfairylandfuture-1.0.0a90.post20240602/PyFairylandFuture.egg-info/
+-rw-rw-rw-   0        0        0     8035 2024-06-01 16:37:29.000000 pyfairylandfuture-1.0.0a90.post20240602/PyFairylandFuture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1506 2024-06-01 16:37:29.000000 pyfairylandfuture-1.0.0a90.post20240602/PyFairylandFuture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 16:37:29.000000 pyfairylandfuture-1.0.0a90.post20240602/PyFairylandFuture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-06-01 16:37:29.000000 pyfairylandfuture-1.0.0a90.post20240602/PyFairylandFuture.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-01 16:37:29.000000 pyfairylandfuture-1.0.0a90.post20240602/PyFairylandFuture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5860 2024-05-11 18:24:45.000000 pyfairylandfuture-1.0.0a90.post20240602/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.550786 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:47.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.568399 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/api/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:46.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.584566 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/common/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:46.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.589566 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/conf/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:46.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.615564 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/constants/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:47.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/constants/__init__.py
+-rw-rw-rw-   0        0        0     1508 2024-06-01 15:19:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/constants/enums.py
+-rw-rw-rw-   0        0        0      339 2024-06-01 16:31:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/constants/typed.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.625568 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:46.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.666567 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/abstracts/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:46.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/abstracts/__init__.py
+-rw-rw-rw-   0        0        0      951 2024-06-01 16:31:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/abstracts/datasource.py
+-rw-rw-rw-   0        0        0      529 2024-06-01 15:19:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/abstracts/metaclass.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.681566 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/superclass/
+-rw-rw-rw-   0        0        0      186 2024-06-01 15:19:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/superclass/__init__.py
+-rw-rw-rw-   0        0        0     2408 2024-06-01 16:31:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/superclass/decorators.py
+-rw-rw-rw-   0        0        0     3363 2024-06-01 15:19:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/superclass/enumerate.py
+-rw-rw-rw-   0        0        0      832 2024-06-01 15:19:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/superclass/metaclass.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.685564 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/helpers/
+-rw-rw-rw-   0        0        0      180 2024-05-12 14:17:49.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.687564 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/models/
+-rw-rw-rw-   0        0        0      185 2024-06-01 15:19:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.698567 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/models/dataclasses/
+-rw-rw-rw-   0        0        0      185 2024-06-01 15:19:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/models/dataclasses/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-06-01 16:31:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/models/dataclasses/datasource.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.788192 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/modules/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:47.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/modules/__init__.py
+-rw-rw-rw-   0        0        0     2164 2024-06-01 16:31:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/modules/datasource.py
+-rw-rw-rw-   0        0        0     5962 2024-06-01 15:19:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/modules/datetimes.py
+-rw-rw-rw-   0        0        0     5197 2024-06-01 16:31:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/modules/decorators.py
+-rw-rw-rw-   0        0        0     1249 2024-05-11 18:24:47.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/modules/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.821183 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/scripts/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:47.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.842185 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/test/
+-rw-rw-rw-   0        0        0      180 2024-05-11 18:24:46.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/test/__init__.py
+-rw-rw-rw-   0        0        0      382 2024-06-01 16:31:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/test/_test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.871180 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/
+-rw-rw-rw-   0        0        0      180 2024-05-12 14:17:49.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:29.907183 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/general/
+-rw-rw-rw-   0        0        0      180 2024-05-12 14:17:49.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/general/__init__.py
+-rw-rw-rw-   0        0        0     6145 2024-05-12 14:17:49.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/general/constants.py
+-rw-rw-rw-   0        0        0    10174 2024-06-01 16:31:57.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/journal.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:37:30.039228 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/verifies/
+-rw-rw-rw-   0        0        0      180 2024-05-12 14:17:49.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/verifies/__init__.py
+-rw-rw-rw-   0        0        0     1635 2024-05-12 14:17:49.000000 pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/verifies/validate.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 16:37:30.051241 pyfairylandfuture-1.0.0a90.post20240602/setup.cfg
+-rw-rw-rw-   0        0        0     8967 2024-06-01 16:37:20.000000 pyfairylandfuture-1.0.0a90.post20240602/setup.py
```

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/LICENSE.txt` & `pyfairylandfuture-1.0.0a90.post20240602/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/PKG-INFO` & `pyfairylandfuture-1.0.0a90.post20240602/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: PyFairylandFuture
-Version: 1.0.0a55.post20240512
+Version: 1.0.0a90.post20240602
 Summary: personally developed Python library.
 Home-page: https://github.com/PrettiestFairy/pypi-fairylandfuture
 Author: Lionel Johnson
 Author-email: fairylandfuture@outlook.com
-Keywords: fairyland,Fairyland,pyfairyland,PyFairyland,fairy,Fairy
+Keywords: fairyland,Fairyland,pyfairyland,PyFairyland,fairy,Fairy,fairylandfuture,PyFairylandFuture,FairylandFuture
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -31,18 +30,24 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: black
 Requires-Dist: loguru
+Requires-Dist: python-dateutil
+Requires-Dist: requests
+Requires-Dist: pymysql
+Requires-Dist: pyyaml
 
 # PyPI - FairylandFuture
 
 > @software: PyCharm  
 > @author: [Lionel Johnson](https://fairy.host)  
 > @contact: [Blog](https://blog.fairy.host/) | [Github](https://github.com/PrettiestFairy) | [Telegram](https://t.me/FairylandFuture)  
 > @organization: [Github·FairylandFuture](https://github.com/FairylandFuture)
```

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/PyFairylandFuture.egg-info/PKG-INFO` & `pyfairylandfuture-1.0.0a90.post20240602/PyFairylandFuture.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: PyFairylandFuture
-Version: 1.0.0a55.post20240512
+Version: 1.0.0a90.post20240602
 Summary: personally developed Python library.
 Home-page: https://github.com/PrettiestFairy/pypi-fairylandfuture
 Author: Lionel Johnson
 Author-email: fairylandfuture@outlook.com
-Keywords: fairyland,Fairyland,pyfairyland,PyFairyland,fairy,Fairy
+Keywords: fairyland,Fairyland,pyfairyland,PyFairyland,fairy,Fairy,fairylandfuture,PyFairylandFuture,FairylandFuture
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -31,18 +30,24 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System :: Operating System Kernels :: Linux
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: black
 Requires-Dist: loguru
+Requires-Dist: python-dateutil
+Requires-Dist: requests
+Requires-Dist: pymysql
+Requires-Dist: pyyaml
 
 # PyPI - FairylandFuture
 
 > @software: PyCharm  
 > @author: [Lionel Johnson](https://fairy.host)  
 > @contact: [Blog](https://blog.fairy.host/) | [Github](https://github.com/PrettiestFairy) | [Telegram](https://t.me/FairylandFuture)  
 > @organization: [Github·FairylandFuture](https://github.com/FairylandFuture)
```

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/PyFairylandFuture.egg-info/SOURCES.txt` & `pyfairylandfuture-1.0.0a90.post20240602/PyFairylandFuture.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -11,21 +11,31 @@
 fairylandfuture/common/__init__.py
 fairylandfuture/conf/__init__.py
 fairylandfuture/constants/__init__.py
 fairylandfuture/constants/enums.py
 fairylandfuture/constants/typed.py
 fairylandfuture/core/__init__.py
 fairylandfuture/core/abstracts/__init__.py
-fairylandfuture/core/abstracts/enumerate.py
+fairylandfuture/core/abstracts/datasource.py
 fairylandfuture/core/abstracts/metaclass.py
+fairylandfuture/core/superclass/__init__.py
+fairylandfuture/core/superclass/decorators.py
+fairylandfuture/core/superclass/enumerate.py
+fairylandfuture/core/superclass/metaclass.py
+fairylandfuture/helpers/__init__.py
+fairylandfuture/models/__init__.py
+fairylandfuture/models/dataclasses/__init__.py
+fairylandfuture/models/dataclasses/datasource.py
 fairylandfuture/modules/__init__.py
+fairylandfuture/modules/datasource.py
 fairylandfuture/modules/datetimes.py
 fairylandfuture/modules/decorators.py
 fairylandfuture/modules/exceptions.py
-fairylandfuture/modules/journal.py
 fairylandfuture/scripts/__init__.py
 fairylandfuture/test/__init__.py
-fairylandfuture/util/__init__.py
-fairylandfuture/util/general/__init__.py
-fairylandfuture/util/general/constants.py
-fairylandfuture/util/verifies/__init__.py
-fairylandfuture/util/verifies/validate.py
+fairylandfuture/test/_test.py
+fairylandfuture/utils/__init__.py
+fairylandfuture/utils/journal.py
+fairylandfuture/utils/general/__init__.py
+fairylandfuture/utils/general/constants.py
+fairylandfuture/utils/verifies/__init__.py
+fairylandfuture/utils/verifies/validate.py
```

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/README.md` & `pyfairylandfuture-1.0.0a90.post20240602/README.md`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/constants/enums.py` & `pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/constants/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 @software: PyCharm
 @author: Lionel Johnson
 @contact: https://fairy.host
 @organization: https://github.com/FairylandFuture
 @since: 2024-05-10 10:45:41 UTC+8
 """
 
-from fairylandfuture.core.abstracts.enumerate import EnumBase
-from fairylandfuture.core.abstracts.enumerate import StringEnum
+from fairylandfuture.core.superclass.enumerate import EnumBase
+from fairylandfuture.core.superclass.enumerate import StringEnum
 
 
 class DateTimeEnum(StringEnum):
     """
     Date time enum.
     """
 
     DATE = date = "%Y-%m-%d"
     TIME = time = "%H:%M:%S"
     DATETIME = datetime = "%Y-%m-%d %H:%M:%S"
 
     DATE_CN = date_cn = "%Y年%m月%d日"
-    TIME_CH = time_cn = "%H时%M分%S秒"
+    TIME_CN = time_cn = "%H时%M分%S秒"
     DATETIME_CN = datetime_cn = "%Y年%m月%d日 %H时%M分%S秒"
 
     @classmethod
     def default(cls) -> str:
         return cls.DATETIME.value
 
     @classmethod
```

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/core/abstracts/enumerate.py` & `pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/superclass/enumerate.py`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/core/abstracts/metaclass.py` & `pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/core/superclass/metaclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding: utf8
 """ 
 @software: PyCharm
 @author: Lionel Johnson
 @contact: https://fairy.host
 @organization: https://github.com/FairylandFuture
-@since: 2024-05-10 10:58:14 UTC+8
+@since: 2024-05-18 下午5:21:05 UTC+8
 """
 
-import abc
 import functools
-from typing import Any, Dict
+from typing import Any
 
 
 class SingletonMeta(type):
     """
     Singleton pattern metaclass
     """
 
@@ -30,20 +29,7 @@
         :rtype: object
         """
         if not hasattr(cls, "__instance"):
             setattr(cls, "__instance", super().__call__(*args, **kwargs))
             return getattr(cls, "__instance")
         else:
             return getattr(cls, "__instance")
-
-
-class SingletonABCMeta(abc.ABCMeta):
-    """
-    Singleton meta
-    """
-
-    _instances: Dict[type, object] = dict()
-
-    def __call__(cls, *args, **kwargs):
-        if cls not in cls._instances:
-            cls._instances.update({cls: super().__call__(*args, **kwargs)})
-        return cls._instances.get(cls)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/modules/datetimes.py` & `pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/modules/datetimes.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 @author: Lionel Johnson
 @contact: https://fairy.host
 @organization: https://github.com/FairylandFuture
 @since: 2024-05-10 12:34:34 UTC+8
 """
 
 import time
-from datetime import datetime
-from typing import Union, Optional
+from datetime import datetime, timedelta
+from typing import Union, Optional, Any
+from dateutil.relativedelta import relativedelta
 
 from fairylandfuture.constants.enums import DateTimeEnum
-from fairylandfuture.core.abstracts.metaclass import SingletonMeta
-from fairylandfuture.util.verifies.validate import ParamTypeValidator
+from fairylandfuture.core.superclass.metaclass import SingletonMeta
+from fairylandfuture.utils.verifies.validate import ParamTypeValidator
 
 
 class DateTimeModule(SingletonMeta):
     """
     Date time utils.
     """
 
@@ -125,7 +126,69 @@
 
         if millisecond:
             return int(timestamp * 1000)
         if n:
             return int(timestamp * (10 ** (n - 10)))
 
         return int(timestamp)
+
+    @classmethod
+    def yesterday(cls, _format: str = DateTimeEnum.DATE.value) -> str:
+        """
+        Get yesterday's date.
+
+        :param _format: Date format.
+        :type _format: str
+        :return: Yesterday's date.
+        :rtype: str
+        """
+        return (datetime.now() - relativedelta(days=1)).strftime(_format)
+
+    @classmethod
+    def tomorrow(cls, _format: str = DateTimeEnum.DATE.value) -> str:
+        """
+        Get tomorrow's date.
+
+        :param _format: Date format.
+        :type _format: str
+        :return: Tomorrow's date.
+        :rtype: str
+        """
+        return (datetime.now() + relativedelta(days=1)).strftime(_format)
+
+    @classmethod
+    def daysdelta(
+        cls,
+        dt1: Union[str, int, float],
+        dt2: Union[str, int, float],
+        timestamp: bool = False,
+        millisecond: bool = False,
+        _format: str = DateTimeEnum.DATE.value,
+    ) -> int:
+        """
+        Calculate the number of days between two dates.
+
+        :param dt1: Datetime_str or timestamp of the first date.
+        :type dt1: str or int or float
+        :param dt2: Datetime_str or timestamp of the second date.
+        :type dt2: str or int or float
+        :param timestamp: Is timestamp or datetime_str.
+        :type timestamp: bool
+        :param millisecond: Is millisecond or not.
+        :type millisecond: bool
+        :param _format: Datetime_str format.
+        :type _format: str
+        :return: Days delta.
+        :rtype: int
+        """
+        if timestamp:
+            if millisecond:
+                date1 = datetime.fromtimestamp(dt1 / 1000)
+                date2 = datetime.fromtimestamp(dt2 / 1000)
+            else:
+                date1 = datetime.fromtimestamp(dt1)
+                date2 = datetime.fromtimestamp(dt2)
+        else:
+            date1 = datetime.strptime(dt1, _format)
+            date2 = datetime.strptime(dt2, _format)
+
+        return abs((date2 - date1).days)
```

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/modules/exceptions.py` & `pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/general/constants.py` & `pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/general/constants.py`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/fairylandfuture/util/verifies/validate.py` & `pyfairylandfuture-1.0.0a90.post20240602/fairylandfuture/utils/verifies/validate.py`

 * *Files identical despite different names*

### Comparing `pyfairylandfuture-1.0.0a55.post20240512/setup.py` & `pyfairylandfuture-1.0.0a90.post20240602/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 _MARK_TYPE = Literal["release", "test", "alpha", "beta"]
 
 _ROOT_PATH = os.path.abspath(os.path.dirname(__file__))
 _MAJOR = 1
 _SUB = 0
 _STAGE = 0
-_MARK = "alpha"
+_MARK: _MARK_TYPE = "alpha"
 
 if sys.version_info < (3, 7):
     sys.exit("Python 3.7 or higher is required.")
 
 
 class InstallDependenciesCommand(setuptools.Command):
     user_options = []
@@ -123,16 +123,15 @@
 
     @property
     def long_description_content_type(self):
         return "text/markdown"
 
     @property
     def packages_include(self):
-        include = ("fairylandfuture",)
-        # include = ("fairylandfuture/conf/publish/gitcommitrc",)
+        include = ("fairylandfuture", "fairylandfuture.*")
 
         return include
 
     @property
     def packages_exclude(self):
         exclude = (
             "bin",
@@ -144,34 +143,49 @@
             "test",
             # "fairylandfuture/test",
         )
 
         return exclude
 
     @property
+    def packages_data(self):
+        data = {"": ["*.txt", "*.rst", "*.md"], "fairylandfuture": ["fairylandfuture/conf/*"]}
+
+        return data
+
+    @property
     def fullname(self):
         return self.name + self.version
 
     @property
     def python_requires(self):
-        return ">=3.7"
+        return ">=3.8"
 
     @property
     def keywords(self):
-        return ["fairyland", "Fairyland", "pyfairyland", "PyFairyland", "fairy", "Fairy"]
+        return [
+            "fairyland",
+            "Fairyland",
+            "pyfairyland",
+            "PyFairyland",
+            "fairy",
+            "Fairy",
+            "fairylandfuture",
+            "PyFairylandFuture",
+            "FairylandFuture",
+        ]
 
     @property
     def include_package_data(self):
         return True
 
     @property
     def classifiers(self):
         results = [
             "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Programming Language :: Python :: 3.12",
             "Programming Language :: Python :: Implementation :: CPython",
             "Programming Language :: Python :: Implementation :: PyPy",
@@ -198,23 +212,25 @@
         ]
 
         return results
 
     @property
     def install_requires(self):
         results = [
+            "setuptools",
+            "black",
             "loguru",
+            "python-dateutil",
+            "requests",
+            "pymysql",
+            "pyyaml",
             # "pip-review",
             # "pip-autoremove",
-            # "black",
             # "python-dotenv",
-            # "pymysql",
             # "psycopg2-binary",
-            # "pyyaml",
-            # "requests",
             # "fake-useragent",
             # "tornado",
             # "pandas",
             # "django",
             # "django-stubs",
             # "djangorestframework",
             # "django-cors-headers",
@@ -237,29 +253,28 @@
 
     @staticmethod
     def __get_github_commit_count():
         # Fixed, Package error
         # with open(os.path.join(_ROOT_PATH, "fairylandfuture", "conf", "publish", "gitcommitrc"), "r", encoding="UTF-8") as FileIO:
         #     commit_count = FileIO.read()
         # return int(commit_count)
-        url = (
-            "https://raw.githubusercontent.com/PrettiestFairy/pypi-fairylandfuture/Pre-release/conf/publish/gitcommitrc"
-        )
-        response = requests.get(url)
-        if response.status_code == 200:
-            commit_count = int(response.text)
-            return commit_count
-        else:
-            try:
-                with open(os.path.join(_ROOT_PATH, "conf", "publish", "gitcommitrc"), "r", encoding="UTF-8") as FileIO:
-                    commit_count = FileIO.read()
-                return int(commit_count)
-            except Exception as err:
-                print(f"Error: {err}")
-                return 0
+        # url = "https://raw.githubusercontent.com/PrettiestFairy/pypi-fairylandfuture/Pre-release/conf/publish/gitcommitrc"
+        # response = requests.get(url)
+        # if response.status_code == 200:
+        #     commit_count = int(response.text)
+        #     return commit_count
+        # else:
+        #     try:
+        #         with open(os.path.join(_ROOT_PATH, "conf", "publish", "gitcommitrc"), "r", encoding="UTF-8") as FileIO:
+        #             commit_count = FileIO.read()
+        #         return int(commit_count)
+        #     except Exception as err:
+        #         print(f"Error: {err}")
+        #         return 0
+        return 90
 
 
 package = PackageInfo(_MAJOR, _SUB, _STAGE, _MARK)
 
 setuptools.setup(
     name=package.name,
     fullname=package.fullname,
@@ -270,16 +285,14 @@
     description=package.description,
     long_description=package.long_description,
     long_description_content_type=package.long_description_content_type,
     url=package.url,
     # license="AGPLv3+",
     # packages=setuptools.find_packages(include=package.packages_include, exclude=package.packages_exclude),
     packages=setuptools.find_packages(exclude=package.packages_exclude),
+    package_data=package.packages_data,
     include_package_data=package.include_package_data,
     classifiers=package.classifiers,
     python_requires=package.python_requires,
     install_requires=package.install_requires,
     cmdclass=package.cmdclass,
 )
-
-if __name__ == "__main__":
-    print(package.version)
```

