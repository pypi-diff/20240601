# Comparing `tmp/cicdpoetrytest1-0.0.2.tar.gz` & `tmp/cicdpoetrytest1-0.1.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicdpoetrytest1-0.0.2.tar", max compression
+gzip compressed data, was "cicdpoetrytest1-0.1.1.dev1.tar", max compression
```

## Comparing `cicdpoetrytest1-0.0.2.tar` & `cicdpoetrytest1-0.1.1.dev1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-05-31 15:49:42.028076 cicdpoetrytest1-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-31 15:49:42.028025 cicdpoetrytest1-0.0.2/cicdpoetrytest1/__init__.py
--rw-r--r--   0        0        0      778 2024-05-31 21:50:36.897575 cicdpoetrytest1-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      351 1970-01-01 00:00:00.000000 cicdpoetrytest1-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-31 15:49:42.028076 cicdpoetrytest1-0.1.1.dev1/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 15:49:42.028025 cicdpoetrytest1-0.1.1.dev1/cicdpoetrytest1/__init__.py
+-rw-r--r--   0        0        0      721 2024-05-31 22:06:43.192755 cicdpoetrytest1-0.1.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 cicdpoetrytest1-0.1.1.dev1/PKG-INFO
```

### Comparing `cicdpoetrytest1-0.0.2/pyproject.toml` & `cicdpoetrytest1-0.1.1.dev1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cicdpoetrytest1"
-version = "0.0.2"
+version = "0.1.1.dev1"
 description = ""
 authors = ["Steffen Albrecht <steffen.alb@posteo.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
@@ -15,14 +15,14 @@
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 strict = true
 format-jinja = """
     {%- if distance == 0 -%}
-        {{serialize_pep440(base, stage, revision) }}
-    {%- elif revision is not none -%}
-        {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
+        {{ serialize_pep440(base) }}
+    {%- elif branch == 'dev' -%}
+        {{ serialize_pep440(bump_version(base), dev = distance) }}
     {%- else -%}
-        {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
+        {{ serialize_pep440(bump_version(base), dev=distance, metadata=[commit]) }}
     {%- endif -%}
 """
```

