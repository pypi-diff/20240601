# Comparing `tmp/easyfileops-0.1.1.tar.gz` & `tmp/easyfileops-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfileops-0.1.1.tar", last modified: Sat Jun  1 20:00:57 2024, max compression
+gzip compressed data, was "easyfileops-0.1.2.tar", last modified: Sat Jun  1 20:09:06 2024, max compression
```

## Comparing `easyfileops-0.1.1.tar` & `easyfileops-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 20:00:57.029372 easyfileops-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-06-01 20:00:57.019911 easyfileops-0.1.1/EasyFileOps/
--rw-rw-rw-   0        0        0     8279 2024-06-01 20:00:01.000000 easyfileops-0.1.1/EasyFileOps/init.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:00:57.027089 easyfileops-0.1.1/EasyFileOps.egg-info/
--rw-rw-rw-   0        0        0      167 2024-06-01 20:00:56.000000 easyfileops-0.1.1/EasyFileOps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-06-01 20:00:56.000000 easyfileops-0.1.1/EasyFileOps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 20:00:56.000000 easyfileops-0.1.1/EasyFileOps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 20:00:56.000000 easyfileops-0.1.1/EasyFileOps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-06-01 20:00:57.027089 easyfileops-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1726 2024-06-01 20:00:01.000000 easyfileops-0.1.1/README.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 20:00:57.029372 easyfileops-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      265 2024-06-01 19:58:28.000000 easyfileops-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:09:06.084915 easyfileops-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-06-01 20:09:06.068225 easyfileops-0.1.2/EasyFileOps/
+-rw-rw-rw-   0        0        0     8279 2024-06-01 20:00:01.000000 easyfileops-0.1.2/EasyFileOps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:09:06.082444 easyfileops-0.1.2/EasyFileOps.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-06-01 20:09:05.000000 easyfileops-0.1.2/EasyFileOps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-06-01 20:09:06.000000 easyfileops-0.1.2/EasyFileOps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 20:09:05.000000 easyfileops-0.1.2/EasyFileOps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 20:09:06.000000 easyfileops-0.1.2/EasyFileOps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-06-01 20:09:06.083669 easyfileops-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1726 2024-06-01 20:00:01.000000 easyfileops-0.1.2/README.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 20:09:06.086026 easyfileops-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      265 2024-06-01 20:08:37.000000 easyfileops-0.1.2/setup.py
```

### Comparing `easyfileops-0.1.1/EasyFileOps/init.py` & `easyfileops-0.1.2/EasyFileOps/__init__.py`

 * *Files identical despite different names*

### Comparing `easyfileops-0.1.1/README.txt` & `easyfileops-0.1.2/README.txt`

 * *Files identical despite different names*

