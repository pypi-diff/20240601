# Comparing `tmp/pyaicodingcube-0.0.6.tar.gz` & `tmp/pyaicodingcube-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaicodingcube-0.0.6.tar", last modified: Sat Jun  1 14:30:49 2024, max compression
+gzip compressed data, was "pyaicodingcube-0.0.7.tar", last modified: Sat Jun  1 14:37:11 2024, max compression
```

## Comparing `pyaicodingcube-0.0.6.tar` & `pyaicodingcube-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 14:30:49.254058 pyaicodingcube-0.0.6/
--rw-rw-rw-   0        0        0      150 2024-06-01 14:30:49.251567 pyaicodingcube-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 14:30:49.185097 pyaicodingcube-0.0.6/aicodingcube/
--rw-rw-rw-   0        0        0        0 2024-06-01 14:25:02.000000 pyaicodingcube-0.0.6/aicodingcube/__init__.py
--rw-rw-rw-   0        0        0    13811 2024-05-31 13:43:20.000000 pyaicodingcube-0.0.6/aicodingcube/aicodingcube.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:30:49.246797 pyaicodingcube-0.0.6/pyaicodingcube.egg-info/
--rw-rw-rw-   0        0        0      150 2024-06-01 14:30:48.000000 pyaicodingcube-0.0.6/pyaicodingcube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-06-01 14:30:48.000000 pyaicodingcube-0.0.6/pyaicodingcube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 14:30:48.000000 pyaicodingcube-0.0.6/pyaicodingcube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 14:30:48.000000 pyaicodingcube-0.0.6/pyaicodingcube.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 14:30:49.255293 pyaicodingcube-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      383 2024-06-01 14:30:38.000000 pyaicodingcube-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:37:11.701859 pyaicodingcube-0.0.7/
+-rw-rw-rw-   0        0        0      150 2024-06-01 14:37:11.700345 pyaicodingcube-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 14:37:11.657337 pyaicodingcube-0.0.7/pyaicodingcube/
+-rw-rw-rw-   0        0        0        0 2024-06-01 14:25:02.000000 pyaicodingcube-0.0.7/pyaicodingcube/__init__.py
+-rw-rw-rw-   0        0        0    13811 2024-05-31 13:43:20.000000 pyaicodingcube-0.0.7/pyaicodingcube/aicodingcube.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:37:11.695582 pyaicodingcube-0.0.7/pyaicodingcube.egg-info/
+-rw-rw-rw-   0        0        0      150 2024-06-01 14:37:11.000000 pyaicodingcube-0.0.7/pyaicodingcube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-06-01 14:37:11.000000 pyaicodingcube-0.0.7/pyaicodingcube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 14:37:11.000000 pyaicodingcube-0.0.7/pyaicodingcube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 14:37:11.000000 pyaicodingcube-0.0.7/pyaicodingcube.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 14:37:11.703313 pyaicodingcube-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-06-01 14:37:05.000000 pyaicodingcube-0.0.7/setup.py
```

### Comparing `pyaicodingcube-0.0.6/aicodingcube/aicodingcube.py` & `pyaicodingcube-0.0.7/pyaicodingcube/aicodingcube.py`

 * *Files identical despite different names*

