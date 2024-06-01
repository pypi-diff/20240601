# Comparing `tmp/slumpy-0.0.1.tar.gz` & `tmp/slumpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slumpy-0.0.1.tar", last modified: Fri May 17 12:40:00 2024, max compression
+gzip compressed data, was "slumpy-0.1.0.tar", last modified: Sat Jun  1 19:28:30 2024, max compression
```

## Comparing `slumpy-0.0.1.tar` & `slumpy-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        0 2024-05-17 12:40:00.024443 slumpy-0.0.1/
--rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      187 2024-05-17 12:40:00.024443 slumpy-0.0.1/PKG-INFO
--rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)       38 2024-05-17 12:40:00.024443 slumpy-0.0.1/setup.cfg
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      208 2024-05-17 12:23:46.000000 slumpy-0.0.1/setup.py
-drwxrwxr-x   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        0 2024-05-17 12:40:00.020444 slumpy-0.0.1/slumpy/
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      817 2024-05-02 14:48:58.000000 slumpy-0.0.1/slumpy/Bool.py
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     1142 2024-05-02 14:48:56.000000 slumpy-0.0.1/slumpy/Dict.py
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     3264 2024-05-02 14:48:59.000000 slumpy-0.0.1/slumpy/Int.py
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     1515 2024-05-02 14:48:57.000000 slumpy-0.0.1/slumpy/List.py
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     3753 2024-05-02 14:48:58.000000 slumpy-0.0.1/slumpy/Real.py
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     1397 2024-05-02 14:49:00.000000 slumpy-0.0.1/slumpy/Str.py
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)       19 2024-04-27 15:14:50.000000 slumpy-0.0.1/slumpy/__init__.py
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)       29 2024-05-02 13:51:14.000000 slumpy-0.0.1/slumpy/general.py
--rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      117 2024-05-02 14:49:58.000000 slumpy-0.0.1/slumpy/main.py
-drwxrwxr-x   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        0 2024-05-17 12:40:00.024443 slumpy-0.0.1/slumpy.egg-info/
--rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      187 2024-05-17 12:40:00.000000 slumpy-0.0.1/slumpy.egg-info/PKG-INFO
--rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      268 2024-05-17 12:40:00.000000 slumpy-0.0.1/slumpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        1 2024-05-17 12:40:00.000000 slumpy-0.0.1/slumpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        7 2024-05-17 12:40:00.000000 slumpy-0.0.1/slumpy.egg-info/top_level.txt
+drwxrwxr-x   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        0 2024-06-01 19:28:30.674083 slumpy-0.1.0/
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     1066 2024-06-01 15:11:45.000000 slumpy-0.1.0/LICENSE
+-rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      316 2024-06-01 19:28:30.674083 slumpy-0.1.0/PKG-INFO
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      144 2024-06-01 16:20:41.000000 slumpy-0.1.0/README.md
+-rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)       38 2024-06-01 19:28:30.674083 slumpy-0.1.0/setup.cfg
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      376 2024-06-01 19:28:22.000000 slumpy-0.1.0/setup.py
+drwxrwxr-x   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        0 2024-06-01 19:28:30.674083 slumpy-0.1.0/slumpy.egg-info/
+-rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      316 2024-06-01 19:28:30.000000 slumpy-0.1.0/slumpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      274 2024-06-01 19:28:30.000000 slumpy-0.1.0/slumpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        1 2024-06-01 19:28:30.000000 slumpy-0.1.0/slumpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        4 2024-06-01 19:28:30.000000 slumpy-0.1.0/slumpy.egg-info/top_level.txt
+drwxrwxr-x   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)        0 2024-06-01 19:28:30.674083 slumpy-0.1.0/src/
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      105 2024-05-31 23:20:34.000000 slumpy-0.1.0/src/__init__.py
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)      872 2024-05-31 15:29:30.000000 slumpy-0.1.0/src/boolum_type.py
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     1177 2024-05-20 17:56:57.000000 slumpy-0.1.0/src/dictum_type.py
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     4028 2024-05-31 15:32:44.000000 slumpy-0.1.0/src/intum_type.py
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     1622 2024-05-31 22:59:15.000000 slumpy-0.1.0/src/listum_type.py
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     3753 2024-05-31 15:34:49.000000 slumpy-0.1.0/src/realum_type.py
+-rw-r--r--   0 gloack-zorin-pc  (1000) gloack-zorin-pc  (1000)     1164 2024-05-31 15:37:32.000000 slumpy-0.1.0/src/strum_type.py
```

