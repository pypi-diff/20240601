# Comparing `tmp/simplelogincmd-0.2.0.tar.gz` & `tmp/simplelogincmd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplelogincmd-0.2.0.tar", max compression
+gzip compressed data, was "simplelogincmd-0.2.1.tar", max compression
```

## Comparing `simplelogincmd-0.2.0.tar` & `simplelogincmd-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1072 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/LICENSE
--rw-r--r--   0        0        0      650 2024-05-25 08:26:46.389923 simplelogincmd-0.2.0/README.md
--rw-r--r--   0        0        0      630 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/__init__.py
--rw-r--r--   0        0        0       49 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/cli/__init__.py
--rw-r--r--   0        0        0     1012 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/cli/commands/__init__.py
--rw-r--r--   0        0        0     2630 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/cli/commands/account.py
--rw-r--r--   0        0        0    13896 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/commands/alias.py
--rw-r--r--   0        0        0     1424 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/commands/database.py
--rw-r--r--   0        0        0     4016 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/commands/mailbox.py
--rw-r--r--   0        0        0    12839 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/const.py
--rw-r--r--   0        0        0      825 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/cli/exceptions.py
--rw-r--r--   0        0        0     1378 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/main.py
--rw-r--r--   0        0        0     7787 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/cli/util.py
--rw-r--r--   0        0        0     2956 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/config.py
--rw-r--r--   0        0        0      322 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/const.py
--rw-r--r--   0        0        0      106 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/database/__init__.py
--rw-r--r--   0        0        0     4293 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/database/access_layer.py
--rw-r--r--   0        0        0     9488 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/database/models.py
--rw-r--r--   0        0        0     1087 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/database/session.py
--rw-r--r--   0        0        0      114 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/__init__.py
--rw-r--r--   0        0        0     3279 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/client.py
--rw-r--r--   0        0        0      784 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/const.py
--rw-r--r--   0        0        0      197 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/exceptions.py
--rw-r--r--   0        0        0    20896 2024-06-01 03:08:33.267320 simplelogincmd-0.2.0/simplelogincmd/rest/simplelogin.py
--rw-r--r--   0        0        0     2419 2024-05-25 07:38:18.074020 simplelogincmd-0.2.0/simplelogincmd/rest/util.py
--rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 simplelogincmd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/LICENSE
+-rw-r--r--   0        0        0      650 2024-05-25 08:26:46.389923 simplelogincmd-0.2.1/README.md
+-rw-r--r--   0        0        0      630 2024-06-01 04:29:49.494358 simplelogincmd-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/cli/__init__.py
+-rw-r--r--   0        0        0     1012 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2630 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/cli/commands/account.py
+-rw-r--r--   0        0        0    13896 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/cli/commands/alias.py
+-rw-r--r--   0        0        0     1424 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/cli/commands/database.py
+-rw-r--r--   0        0        0     4016 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/cli/commands/mailbox.py
+-rw-r--r--   0        0        0    12839 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/cli/const.py
+-rw-r--r--   0        0        0      825 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/cli/exceptions.py
+-rw-r--r--   0        0        0     1378 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/cli/main.py
+-rw-r--r--   0        0        0     7787 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/cli/util.py
+-rw-r--r--   0        0        0     2956 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/config.py
+-rw-r--r--   0        0        0      322 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/const.py
+-rw-r--r--   0        0        0      106 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/database/__init__.py
+-rw-r--r--   0        0        0     4293 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/database/access_layer.py
+-rw-r--r--   0        0        0     9488 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/database/models.py
+-rw-r--r--   0        0        0     1087 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/database/session.py
+-rw-r--r--   0        0        0      114 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/rest/__init__.py
+-rw-r--r--   0        0        0     3279 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/rest/client.py
+-rw-r--r--   0        0        0      784 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/rest/const.py
+-rw-r--r--   0        0        0      197 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/rest/exceptions.py
+-rw-r--r--   0        0        0    20896 2024-06-01 03:08:33.267320 simplelogincmd-0.2.1/simplelogincmd/rest/simplelogin.py
+-rw-r--r--   0        0        0     2419 2024-05-25 07:38:18.074020 simplelogincmd-0.2.1/simplelogincmd/rest/util.py
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 simplelogincmd-0.2.1/PKG-INFO
```

### Comparing `simplelogincmd-0.2.0/LICENSE` & `simplelogincmd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/README.md` & `simplelogincmd-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/pyproject.toml` & `simplelogincmd-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplelogincmd"
-version = "0.2.0"
+version = "0.2.1"
 description = "SimpleLogin command-line application"
 authors = ["truthless-dev <truthless.deviant248@simplelogin.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/commands/__init__.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/commands/account.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/commands/alias.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/commands/alias.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/commands/database.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/commands/database.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/commands/mailbox.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/commands/mailbox.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/const.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/const.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/exceptions.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/main.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/main.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/cli/util.py` & `simplelogincmd-0.2.1/simplelogincmd/cli/util.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/config.py` & `simplelogincmd-0.2.1/simplelogincmd/config.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/database/access_layer.py` & `simplelogincmd-0.2.1/simplelogincmd/database/access_layer.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/database/models.py` & `simplelogincmd-0.2.1/simplelogincmd/database/models.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/database/session.py` & `simplelogincmd-0.2.1/simplelogincmd/database/session.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/rest/client.py` & `simplelogincmd-0.2.1/simplelogincmd/rest/client.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/rest/const.py` & `simplelogincmd-0.2.1/simplelogincmd/rest/const.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/rest/simplelogin.py` & `simplelogincmd-0.2.1/simplelogincmd/rest/simplelogin.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/simplelogincmd/rest/util.py` & `simplelogincmd-0.2.1/simplelogincmd/rest/util.py`

 * *Files identical despite different names*

### Comparing `simplelogincmd-0.2.0/PKG-INFO` & `simplelogincmd-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplelogincmd
-Version: 0.2.0
+Version: 0.2.1
 Summary: SimpleLogin command-line application
 License: MIT
 Author: truthless-dev
 Author-email: truthless.deviant248@simplelogin.fr
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

