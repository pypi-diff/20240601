# Comparing `tmp/easyfileops-0.1.2.tar.gz` & `tmp/easyfileops-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfileops-0.1.2.tar", last modified: Sat Jun  1 20:09:06 2024, max compression
+gzip compressed data, was "easyfileops-0.1.3.tar", last modified: Sat Jun  1 20:12:53 2024, max compression
```

## Comparing `easyfileops-0.1.2.tar` & `easyfileops-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 20:09:06.084915 easyfileops-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-06-01 20:09:06.068225 easyfileops-0.1.2/EasyFileOps/
--rw-rw-rw-   0        0        0     8279 2024-06-01 20:00:01.000000 easyfileops-0.1.2/EasyFileOps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:09:06.082444 easyfileops-0.1.2/EasyFileOps.egg-info/
--rw-rw-rw-   0        0        0      167 2024-06-01 20:09:05.000000 easyfileops-0.1.2/EasyFileOps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-06-01 20:09:06.000000 easyfileops-0.1.2/EasyFileOps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 20:09:05.000000 easyfileops-0.1.2/EasyFileOps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 20:09:06.000000 easyfileops-0.1.2/EasyFileOps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-06-01 20:09:06.083669 easyfileops-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1726 2024-06-01 20:00:01.000000 easyfileops-0.1.2/README.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 20:09:06.086026 easyfileops-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      265 2024-06-01 20:08:37.000000 easyfileops-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:12:53.627228 easyfileops-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-06-01 20:12:53.604853 easyfileops-0.1.3/EasyFileOps/
+-rw-rw-rw-   0        0        0        0 2024-06-01 20:12:49.000000 easyfileops-0.1.3/EasyFileOps/__init__.py
+-rw-rw-rw-   0        0        0     8279 2024-06-01 20:12:49.000000 easyfileops-0.1.3/EasyFileOps/file.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:12:53.624816 easyfileops-0.1.3/EasyFileOps.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-06-01 20:12:53.000000 easyfileops-0.1.3/EasyFileOps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-06-01 20:12:53.000000 easyfileops-0.1.3/EasyFileOps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 20:12:53.000000 easyfileops-0.1.3/EasyFileOps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 20:12:53.000000 easyfileops-0.1.3/EasyFileOps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2024-06-01 20:12:53.626132 easyfileops-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1726 2024-06-01 20:00:01.000000 easyfileops-0.1.3/README.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 20:12:53.627228 easyfileops-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      265 2024-06-01 20:12:49.000000 easyfileops-0.1.3/setup.py
```

### Comparing `easyfileops-0.1.2/EasyFileOps/__init__.py` & `easyfileops-0.1.3/EasyFileOps/file.py`

 * *Files identical despite different names*

### Comparing `easyfileops-0.1.2/README.txt` & `easyfileops-0.1.3/README.txt`

 * *Files identical despite different names*

