# Comparing `tmp/easyfileops-0.1.4.tar.gz` & `tmp/easyfileops-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfileops-0.1.4.tar", last modified: Sat Jun  1 20:14:59 2024, max compression
+gzip compressed data, was "easyfileops-0.1.5.tar", last modified: Sat Jun  1 20:22:55 2024, max compression
```

## Comparing `easyfileops-0.1.4.tar` & `easyfileops-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 20:14:59.987882 easyfileops-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-06-01 20:14:59.971936 easyfileops-0.1.4/EasyFileOps/
--rw-rw-rw-   0        0        0        0 2024-06-01 20:12:49.000000 easyfileops-0.1.4/EasyFileOps/__init__.py
--rw-rw-rw-   0        0        0     8279 2024-06-01 20:12:49.000000 easyfileops-0.1.4/EasyFileOps/file.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:14:59.987882 easyfileops-0.1.4/EasyFileOps.egg-info/
--rw-rw-rw-   0        0        0      167 2024-06-01 20:14:59.000000 easyfileops-0.1.4/EasyFileOps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-06-01 20:14:59.000000 easyfileops-0.1.4/EasyFileOps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 20:14:59.000000 easyfileops-0.1.4/EasyFileOps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 20:14:59.000000 easyfileops-0.1.4/EasyFileOps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-06-01 20:14:59.987882 easyfileops-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1726 2024-06-01 20:00:01.000000 easyfileops-0.1.4/README.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 20:14:59.987882 easyfileops-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      265 2024-06-01 20:14:44.000000 easyfileops-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:22:55.930440 easyfileops-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-06-01 20:22:55.904761 easyfileops-0.1.5/EasyFileOps/
+-rw-rw-rw-   0        0        0        0 2024-06-01 20:12:49.000000 easyfileops-0.1.5/EasyFileOps/__init__.py
+-rw-rw-rw-   0        0        0     8255 2024-06-01 20:22:45.000000 easyfileops-0.1.5/EasyFileOps/file.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:22:55.924761 easyfileops-0.1.5/EasyFileOps.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-06-01 20:22:55.000000 easyfileops-0.1.5/EasyFileOps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-06-01 20:22:55.000000 easyfileops-0.1.5/EasyFileOps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 20:22:55.000000 easyfileops-0.1.5/EasyFileOps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 20:22:55.000000 easyfileops-0.1.5/EasyFileOps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-06-01 20:22:55.929879 easyfileops-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1702 2024-06-01 20:22:45.000000 easyfileops-0.1.5/README.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 20:22:55.930440 easyfileops-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      265 2024-06-01 20:22:45.000000 easyfileops-0.1.5/setup.py
```

### Comparing `easyfileops-0.1.4/EasyFileOps/file.py` & `easyfileops-0.1.5/EasyFileOps/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 ###
 You can install EasyFileOps via pip:
 pip install EasyFileOps
 ###
 ###
 Importing:
 from EasyFileOps import file
-or
-import EasyFileOps
 ###
 ###
 EasyFileOps main method is file
 Parameters of file:
 filename (str) - Here write a file name to operate on
 option (str) - Available options: r, r+, rb, rb+, readline, readlines, readable, w, w+, wb, wb+, writelines, writable,
 a, a+, ab, ab+, seekable, flush, detach, fileno, truncate, isatty, split, splitlines
```

### Comparing `easyfileops-0.1.4/README.txt` & `easyfileops-0.1.5/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 ###
 You can install EasyFileOps via pip:
 pip install EasyFileOps
 ###
 ###
 Importing:
 from EasyFileOps import file
-or
-import EasyFileOps
 ###
 ###
 EasyFileOps main method is file
 Parameters of file:
 filename (str) - Here write a file name to operate on
 option (str) - Available options: r, r+, rb, rb+, readline, readlines, readable, w, w+, wb, wb+, writelines, writable,
 a, a+, ab, ab+, seekable, flush, detach, fileno, truncate, isatty, split, splitlines
```

