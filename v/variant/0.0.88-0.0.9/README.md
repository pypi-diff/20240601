# Comparing `tmp/variant-0.0.88.tar.gz` & `tmp/variant-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variant-0.0.88.tar", max compression
+gzip compressed data, was "variant-0.0.9.tar", max compression
```

## Comparing `variant-0.0.88.tar` & `variant-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0     9602 2024-06-01 09:17:31.604842 variant-0.0.88/README.md
--rw-r--r--   0        0        0      663 2024-06-01 09:17:31.604842 variant-0.0.88/pyproject.toml
--rw-r--r--   0        0        0       22 2024-06-01 09:17:31.612842 variant-0.0.88/variant/__init__.py
--rw-r--r--   0        0        0     6356 2024-06-01 09:17:31.612842 variant-0.0.88/variant/cli.py
--rwxr-xr-x   0        0        0     6704 2024-06-01 09:17:31.612842 variant-0.0.88/variant/coordinate.py
--rwxr-xr-x   0        0        0    16871 2024-06-01 09:17:31.612842 variant-0.0.88/variant/effect.py
--rw-r--r--   0        0        0     1612 2024-06-01 09:17:31.612842 variant-0.0.88/variant/effect_ordering.py
--rwxr-xr-x   0        0        0     3945 2024-06-01 09:17:31.612842 variant-0.0.88/variant/motif.py
--rw-r--r--   0        0        0     1112 2024-06-01 09:17:31.612842 variant-0.0.88/variant/utils.py
--rw-r--r--   0        0        0    10457 1970-01-01 00:00:00.000000 variant-0.0.88/PKG-INFO
+-rw-r--r--   0        0        0     3286 2021-11-25 02:34:02.880549 variant-0.0.9/README.md
+-rw-r--r--   0        0        0      575 2021-11-25 02:40:09.737917 variant-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2021-11-24 05:00:56.582691 variant-0.0.9/variant/__init__.py
+-rwxr-xr-x   0        0        0     6644 2021-11-25 02:33:29.101142 variant-0.0.9/variant/effect.py
+-rw-r--r--   0        0        0     4077 2021-11-25 02:41:38.497736 variant-0.0.9/setup.py
+-rw-r--r--   0        0        0     4011 2021-11-25 02:41:38.498001 variant-0.0.9/PKG-INFO
```

### Comparing `variant-0.0.88/pyproject.toml` & `variant-0.0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [tool.poetry]
 name = "variant"
-version = "0.0.88"
+version = "0.0.9"
 description = ""
 authors = ["Chang Ye <yech1990@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["bioinformatics", "variant", "mutation", "RNA modification"]
 repository = "https://github.com/yech1990/variant"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-numpy = "^1.26.4"
-pyfaidx = "^0.8.1.1"
-pyensembl = "^2.2.4"
+python = "^3.6"
+pyensembl = "^1.9.4"
 varcode = "*"
-rich-click = "^1.8.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 setuptools = "57.4.0"
 
 [tool.poetry.scripts]
-variant-effect = 'variant.cli:effect'
-variant = 'variant.cli:cli'
+variant-effect = 'variant.effect:run'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+
```

