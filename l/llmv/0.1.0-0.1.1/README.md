# Comparing `tmp/llmv-0.1.0.tar.gz` & `tmp/llmv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmv-0.1.0.tar", last modified: Fri May 31 20:24:52 2024, max compression
+gzip compressed data, was "llmv-0.1.1.tar", last modified: Fri May 31 20:57:30 2024, max compression
```

## Comparing `llmv-0.1.0.tar` & `llmv-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 adam       (505) staff       (20)        0 2024-05-31 20:24:52.435898 llmv-0.1.0/
--rw-r--r--   0 adam       (505) staff       (20)      308 2024-05-31 20:24:52.435583 llmv-0.1.0/PKG-INFO
--rw-r--r--   0 adam       (505) staff       (20)       18 2024-05-31 20:23:00.000000 llmv-0.1.0/README.md
-drwxr-xr-x   0 adam       (505) staff       (20)        0 2024-05-31 20:24:52.433872 llmv-0.1.0/llmv/
--rw-r--r--   0 adam       (505) staff       (20)        0 2024-05-31 19:30:01.000000 llmv-0.1.0/llmv/__init__.py
--rw-r--r--   0 adam       (505) staff       (20)       67 2024-05-31 19:41:24.000000 llmv-0.1.0/llmv/__main__.py
--rw-r--r--   0 adam       (505) staff       (20)     7957 2024-05-31 20:10:40.000000 llmv-0.1.0/llmv/chat.py
--rwxr-xr-x   0 adam       (505) staff       (20)     5569 2024-05-31 19:26:37.000000 llmv-0.1.0/llmv/llm_template.py
--rw-r--r--   0 adam       (505) staff       (20)     4948 2024-05-31 20:14:34.000000 llmv-0.1.0/llmv/llmv.py
--rw-r--r--   0 adam       (505) staff       (20)     7095 2024-05-31 20:09:20.000000 llmv-0.1.0/llmv/prompt.py
-drwxr-xr-x   0 adam       (505) staff       (20)        0 2024-05-31 20:24:52.435244 llmv-0.1.0/llmv.egg-info/
--rw-r--r--   0 adam       (505) staff       (20)      308 2024-05-31 20:24:52.000000 llmv-0.1.0/llmv.egg-info/PKG-INFO
--rw-r--r--   0 adam       (505) staff       (20)      253 2024-05-31 20:24:52.000000 llmv-0.1.0/llmv.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (505) staff       (20)        1 2024-05-31 20:24:52.000000 llmv-0.1.0/llmv.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (505) staff       (20)       66 2024-05-31 20:24:52.000000 llmv-0.1.0/llmv.egg-info/requires.txt
--rw-r--r--   0 adam       (505) staff       (20)        5 2024-05-31 20:24:52.000000 llmv-0.1.0/llmv.egg-info/top_level.txt
--rw-r--r--   0 adam       (505) staff       (20)       38 2024-05-31 20:24:52.435981 llmv-0.1.0/setup.cfg
--rw-r--r--   0 adam       (505) staff       (20)      587 2024-05-31 20:24:47.000000 llmv-0.1.0/setup.py
+drwxr-xr-x   0 adam       (505) staff       (20)        0 2024-05-31 20:57:30.772801 llmv-0.1.1/
+-rw-r--r--   0 adam       (505) staff       (20)      308 2024-05-31 20:57:30.772533 llmv-0.1.1/PKG-INFO
+-rw-r--r--   0 adam       (505) staff       (20)       18 2024-05-31 20:23:00.000000 llmv-0.1.1/README.md
+drwxr-xr-x   0 adam       (505) staff       (20)        0 2024-05-31 20:57:30.770629 llmv-0.1.1/llmv/
+-rw-r--r--   0 adam       (505) staff       (20)        0 2024-05-31 19:30:01.000000 llmv-0.1.1/llmv/__init__.py
+-rw-r--r--   0 adam       (505) staff       (20)       67 2024-05-31 19:41:24.000000 llmv-0.1.1/llmv/__main__.py
+-rw-r--r--   0 adam       (505) staff       (20)     7957 2024-05-31 20:10:40.000000 llmv-0.1.1/llmv/chat.py
+-rwxr-xr-x   0 adam       (505) staff       (20)     5569 2024-05-31 19:26:37.000000 llmv-0.1.1/llmv/llm_template.py
+-rw-r--r--   0 adam       (505) staff       (20)     4948 2024-05-31 20:14:34.000000 llmv-0.1.1/llmv/llmv.py
+-rw-r--r--   0 adam       (505) staff       (20)     7095 2024-05-31 20:09:20.000000 llmv-0.1.1/llmv/prompt.py
+drwxr-xr-x   0 adam       (505) staff       (20)        0 2024-05-31 20:57:30.772227 llmv-0.1.1/llmv.egg-info/
+-rw-r--r--   0 adam       (505) staff       (20)      308 2024-05-31 20:57:30.000000 llmv-0.1.1/llmv.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (505) staff       (20)      284 2024-05-31 20:57:30.000000 llmv-0.1.1/llmv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (505) staff       (20)        1 2024-05-31 20:57:30.000000 llmv-0.1.1/llmv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (505) staff       (20)       40 2024-05-31 20:57:30.000000 llmv-0.1.1/llmv.egg-info/entry_points.txt
+-rw-r--r--   0 adam       (505) staff       (20)       66 2024-05-31 20:57:30.000000 llmv-0.1.1/llmv.egg-info/requires.txt
+-rw-r--r--   0 adam       (505) staff       (20)        5 2024-05-31 20:57:30.000000 llmv-0.1.1/llmv.egg-info/top_level.txt
+-rw-r--r--   0 adam       (505) staff       (20)       38 2024-05-31 20:57:30.772861 llmv-0.1.1/setup.cfg
+-rw-r--r--   0 adam       (505) staff       (20)      689 2024-05-31 20:57:24.000000 llmv-0.1.1/setup.py
```

### Comparing `llmv-0.1.0/llmv/chat.py` & `llmv-0.1.1/llmv/chat.py`

 * *Files identical despite different names*

### Comparing `llmv-0.1.0/llmv/llm_template.py` & `llmv-0.1.1/llmv/llm_template.py`

 * *Files identical despite different names*

### Comparing `llmv-0.1.0/llmv/llmv.py` & `llmv-0.1.1/llmv/llmv.py`

 * *Files identical despite different names*

### Comparing `llmv-0.1.0/llmv/prompt.py` & `llmv-0.1.1/llmv/prompt.py`

 * *Files identical despite different names*

