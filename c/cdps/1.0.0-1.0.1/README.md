# Comparing `tmp/CDPS-1.0.0.tar.gz` & `tmp/cdps-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CDPS-1.0.0.tar", last modified: Sat Jun  1 14:36:11 2024, max compression
+gzip compressed data, was "cdps-1.0.1.tar", last modified: Sat Jun  1 15:05:13 2024, max compression
```

## Comparing `CDPS-1.0.0.tar` & `cdps-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 14:36:11.870940 CDPS-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-06-01 14:36:11.869940 CDPS-1.0.0/CDPS.egg-info/
--rw-rw-rw-   0        0        0      234 2024-06-01 14:36:11.000000 CDPS-1.0.0/CDPS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-06-01 14:36:11.000000 CDPS-1.0.0/CDPS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 14:36:11.000000 CDPS-1.0.0/CDPS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 14:36:11.000000 CDPS-1.0.0/CDPS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 CDPS-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      234 2024-06-01 14:36:11.869940 CDPS-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 CDPS-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 14:36:11.870940 CDPS-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      363 2024-06-01 14:35:28.000000 CDPS-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:05:13.474017 cdps-1.0.1/
+-rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      755 2024-06-01 15:05:13.474017 cdps-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:05:13.473018 cdps-1.0.1/cdps.egg-info/
+-rw-rw-rw-   0        0        0      755 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      218 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:05:13.474017 cdps-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1489 2024-06-01 15:04:37.000000 cdps-1.0.1/setup.py
```

### Comparing `CDPS-1.0.0/LICENSE` & `cdps-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CDPS-1.0.0/README.md` & `cdps-1.0.1/README.md`

 * *Files identical despite different names*

