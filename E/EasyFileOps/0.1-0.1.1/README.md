# Comparing `tmp/easyfileops-0.1.tar.gz` & `tmp/easyfileops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfileops-0.1.tar", last modified: Sat Jun  1 19:37:43 2024, max compression
+gzip compressed data, was "easyfileops-0.1.1.tar", last modified: Sat Jun  1 20:00:57 2024, max compression
```

## Comparing `easyfileops-0.1.tar` & `easyfileops-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 19:37:43.428494 easyfileops-0.1/
-drwxrwxrwx   0        0        0        0 2024-06-01 19:37:43.423636 easyfileops-0.1/EasyFileOps.egg-info/
--rw-rw-rw-   0        0        0      165 2024-06-01 19:37:43.000000 easyfileops-0.1/EasyFileOps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2024-06-01 19:37:43.000000 easyfileops-0.1/EasyFileOps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 19:37:43.000000 easyfileops-0.1/EasyFileOps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 19:37:43.000000 easyfileops-0.1/EasyFileOps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      165 2024-06-01 19:37:43.426566 easyfileops-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1721 2024-06-01 08:36:56.000000 easyfileops-0.1/README.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 19:37:43.428494 easyfileops-0.1/setup.cfg
--rw-rw-rw-   0        0        0      262 2024-06-01 19:37:26.000000 easyfileops-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:00:57.029372 easyfileops-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-06-01 20:00:57.019911 easyfileops-0.1.1/EasyFileOps/
+-rw-rw-rw-   0        0        0     8279 2024-06-01 20:00:01.000000 easyfileops-0.1.1/EasyFileOps/init.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:00:57.027089 easyfileops-0.1.1/EasyFileOps.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-06-01 20:00:56.000000 easyfileops-0.1.1/EasyFileOps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-06-01 20:00:56.000000 easyfileops-0.1.1/EasyFileOps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 20:00:56.000000 easyfileops-0.1.1/EasyFileOps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 20:00:56.000000 easyfileops-0.1.1/EasyFileOps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-06-01 20:00:57.027089 easyfileops-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1726 2024-06-01 20:00:01.000000 easyfileops-0.1.1/README.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 20:00:57.029372 easyfileops-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      265 2024-06-01 19:58:28.000000 easyfileops-0.1.1/setup.py
```

### Comparing `easyfileops-0.1/README.txt` & `easyfileops-0.1.1/README.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 ###
 DOCUMENTATION OF EasyFileOps
 ###
 ###
 You can install EasyFileOps via pip:
-pip install easyfileops
+pip install EasyFileOps
 ###
 ###
 Importing:
-from easyfileops import file
+from EasyFileOps import file
 or
-import easyfileops
+import EasyFileOps
+###
 ###
 EasyFileOps main method is file
 Parameters of file:
 filename (str) - Here write a file name to operate on
 option (str) - Available options: r, r+, rb, rb+, readline, readlines, readable, w, w+, wb, wb+, writelines, writable,
 a, a+, ab, ab+, seekable, flush, detach, fileno, truncate, isatty, split, splitlines
 towrite (str or bytes (optional)) - Content to write in operating file
```

