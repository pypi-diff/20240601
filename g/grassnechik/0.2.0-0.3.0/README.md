# Comparing `tmp/grassnechik-0.2.0.tar.gz` & `tmp/grassnechik-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassnechik-0.2.0.tar", max compression
+gzip compressed data, was "grassnechik-0.3.0.tar", max compression
```

## Comparing `grassnechik-0.2.0.tar` & `grassnechik-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      118 2024-05-25 13:26:08.000239 grassnechik-0.2.0/grassnechik/__init__.py
--rw-r--r--   0        0        0     7843 2024-04-07 13:02:28.369417 grassnechik-0.2.0/grassnechik/constants.py
--rw-r--r--   0        0        0     4504 2024-05-25 13:26:08.009228 grassnechik-0.2.0/grassnechik/grassnechik.py
--rw-r--r--   0        0        0      936 2024-05-25 11:59:51.878110 grassnechik-0.2.0/grassnechik/key.py
--rw-r--r--   0        0        0      112 2024-04-07 12:17:39.483649 grassnechik-0.2.0/grassnechik/types.py
--rw-r--r--   0        0        0      768 2024-05-25 13:26:36.235450 grassnechik-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      274 1970-01-01 00:00:00.000000 grassnechik-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      118 2024-05-30 18:44:52.497701 grassnechik-0.3.0/grassnechik/__init__.py
+-rw-r--r--   0        0        0     7843 2024-04-07 13:02:28.369417 grassnechik-0.3.0/grassnechik/constants.py
+-rw-r--r--   0        0        0     4504 2024-06-01 09:53:08.325677 grassnechik-0.3.0/grassnechik/grassnechik.py
+-rw-r--r--   0        0        0      936 2024-05-30 20:22:47.349212 grassnechik-0.3.0/grassnechik/key.py
+-rw-r--r--   0        0        0      112 2024-04-07 12:17:39.483649 grassnechik-0.3.0/grassnechik/types.py
+-rw-r--r--   0        0        0     1097 2024-06-01 10:22:36.361596 grassnechik-0.3.0/LICENSE
+-rw-r--r--   0        0        0      790 2024-06-01 10:20:47.152265 grassnechik-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1993 2024-06-01 10:18:45.406730 grassnechik-0.3.0/README.md
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 grassnechik-0.3.0/PKG-INFO
```

### Comparing `grassnechik-0.2.0/grassnechik/constants.py` & `grassnechik-0.3.0/grassnechik/constants.py`

 * *Files identical despite different names*

### Comparing `grassnechik-0.2.0/grassnechik/grassnechik.py` & `grassnechik-0.3.0/grassnechik/grassnechik.py`

 * *Files identical despite different names*

### Comparing `grassnechik-0.2.0/grassnechik/key.py` & `grassnechik-0.3.0/grassnechik/key.py`

 * *Files identical despite different names*

### Comparing `grassnechik-0.2.0/pyproject.toml` & `grassnechik-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "grassnechik"
-version = "0.2.0"
+version = "0.3.0"
 description = "Cryptography Library"
+readme = "README.md"
 authors = ["Sviatoslav Bobryshev <wstswsb@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 
 
 [tool.poetry.group.dev.dependencies]
```

