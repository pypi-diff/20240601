# Comparing `tmp/pyaicodingcube-0.0.4.tar.gz` & `tmp/pyaicodingcube-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaicodingcube-0.0.4.tar", last modified: Sat Jun  1 14:03:35 2024, max compression
+gzip compressed data, was "pyaicodingcube-0.0.5.tar", last modified: Sat Jun  1 14:25:49 2024, max compression
```

## Comparing `pyaicodingcube-0.0.4.tar` & `pyaicodingcube-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 14:03:35.731721 pyaicodingcube-0.0.4/
--rw-rw-rw-   0        0        0       86 2024-06-01 14:03:35.729699 pyaicodingcube-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 14:03:35.702191 pyaicodingcube-0.0.4/pyaicodingcube/
--rw-rw-rw-   0        0        0      104 2024-06-01 14:03:17.000000 pyaicodingcube-0.0.4/pyaicodingcube/__init__.py
--rw-rw-rw-   0        0        0    13811 2024-05-31 13:43:20.000000 pyaicodingcube-0.0.4/pyaicodingcube/pyaicodingcube.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:03:35.726566 pyaicodingcube-0.0.4/pyaicodingcube.egg-info/
--rw-rw-rw-   0        0        0       86 2024-06-01 14:03:35.000000 pyaicodingcube-0.0.4/pyaicodingcube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-06-01 14:03:35.000000 pyaicodingcube-0.0.4/pyaicodingcube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 14:03:35.000000 pyaicodingcube-0.0.4/pyaicodingcube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-06-01 14:03:35.000000 pyaicodingcube-0.0.4/pyaicodingcube.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 14:03:35.731721 pyaicodingcube-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-06-01 14:02:51.000000 pyaicodingcube-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:49.134972 pyaicodingcube-0.0.5/
+-rw-rw-rw-   0        0        0      150 2024-06-01 14:25:49.132945 pyaicodingcube-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:49.091289 pyaicodingcube-0.0.5/pyaicodingcube/
+-rw-rw-rw-   0        0        0        0 2024-06-01 14:25:02.000000 pyaicodingcube-0.0.5/pyaicodingcube/__init__.py
+-rw-rw-rw-   0        0        0    13811 2024-05-31 13:43:20.000000 pyaicodingcube-0.0.5/pyaicodingcube/pyaicodingcube.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:25:49.128301 pyaicodingcube-0.0.5/pyaicodingcube.egg-info/
+-rw-rw-rw-   0        0        0      150 2024-06-01 14:25:48.000000 pyaicodingcube-0.0.5/pyaicodingcube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-06-01 14:25:48.000000 pyaicodingcube-0.0.5/pyaicodingcube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 14:25:48.000000 pyaicodingcube-0.0.5/pyaicodingcube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 14:25:48.000000 pyaicodingcube-0.0.5/pyaicodingcube.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 14:25:49.135576 pyaicodingcube-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-06-01 14:24:55.000000 pyaicodingcube-0.0.5/setup.py
```

### Comparing `pyaicodingcube-0.0.4/pyaicodingcube/pyaicodingcube.py` & `pyaicodingcube-0.0.5/pyaicodingcube/pyaicodingcube.py`

 * *Files identical despite different names*

