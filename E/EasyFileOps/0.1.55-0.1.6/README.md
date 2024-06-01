# Comparing `tmp/easyfileops-0.1.55.tar.gz` & `tmp/easyfileops-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfileops-0.1.55.tar", last modified: Sat Jun  1 20:28:19 2024, max compression
+gzip compressed data, was "easyfileops-0.1.6.tar", last modified: Sat Jun  1 20:47:55 2024, max compression
```

## Comparing `easyfileops-0.1.55.tar` & `easyfileops-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 20:28:19.875213 easyfileops-0.1.55/
-drwxrwxrwx   0        0        0        0 2024-06-01 20:28:19.844730 easyfileops-0.1.55/EasyFileOps/
--rw-rw-rw-   0        0        0        0 2024-06-01 20:12:49.000000 easyfileops-0.1.55/EasyFileOps/__init__.py
--rw-rw-rw-   0        0        0     8301 2024-06-01 20:27:46.000000 easyfileops-0.1.55/EasyFileOps/file.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:28:19.875213 easyfileops-0.1.55/EasyFileOps.egg-info/
--rw-rw-rw-   0        0        0      168 2024-06-01 20:28:19.000000 easyfileops-0.1.55/EasyFileOps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-06-01 20:28:19.000000 easyfileops-0.1.55/EasyFileOps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 20:28:19.000000 easyfileops-0.1.55/EasyFileOps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 20:28:19.000000 easyfileops-0.1.55/EasyFileOps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      168 2024-06-01 20:28:19.875213 easyfileops-0.1.55/PKG-INFO
--rw-rw-rw-   0        0        0     1748 2024-06-01 20:27:46.000000 easyfileops-0.1.55/README.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 20:28:19.882690 easyfileops-0.1.55/setup.cfg
--rw-rw-rw-   0        0        0      266 2024-06-01 20:26:03.000000 easyfileops-0.1.55/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:47:55.449441 easyfileops-0.1.6/
+drwxrwxrwx   0        0        0        0 2024-06-01 20:47:55.433559 easyfileops-0.1.6/EasyFileOps/
+-rw-rw-rw-   0        0        0        0 2024-06-01 20:12:49.000000 easyfileops-0.1.6/EasyFileOps/__init__.py
+-rw-rw-rw-   0        0        0     8301 2024-06-01 20:27:46.000000 easyfileops-0.1.6/EasyFileOps/file.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:47:55.449441 easyfileops-0.1.6/EasyFileOps.egg-info/
+-rw-rw-rw-   0        0        0      156 2024-06-01 20:47:55.000000 easyfileops-0.1.6/EasyFileOps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-06-01 20:47:55.000000 easyfileops-0.1.6/EasyFileOps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 20:47:55.000000 easyfileops-0.1.6/EasyFileOps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 20:47:55.000000 easyfileops-0.1.6/EasyFileOps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      156 2024-06-01 20:47:55.449441 easyfileops-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1748 2024-06-01 20:27:46.000000 easyfileops-0.1.6/README.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 20:47:55.449441 easyfileops-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      254 2024-06-01 20:47:33.000000 easyfileops-0.1.6/setup.py
```

### Comparing `easyfileops-0.1.55/EasyFileOps/file.py` & `easyfileops-0.1.6/EasyFileOps/file.py`

 * *Files identical despite different names*

### Comparing `easyfileops-0.1.55/README.txt` & `easyfileops-0.1.6/README.txt`

 * *Files identical despite different names*

