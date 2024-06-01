# Comparing `tmp/pyaicodingcube-0.0.2.tar.gz` & `tmp/pyaicodingcube-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaicodingcube-0.0.2.tar", last modified: Fri May 31 14:42:08 2024, max compression
+gzip compressed data, was "pyaicodingcube-0.0.3.tar", last modified: Sat Jun  1 13:39:01 2024, max compression
```

## Comparing `pyaicodingcube-0.0.2.tar` & `pyaicodingcube-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 14:42:08.729468 pyaicodingcube-0.0.2/
--rw-rw-rw-   0        0        0       86 2024-05-31 14:42:08.729468 pyaicodingcube-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 14:42:08.703575 pyaicodingcube-0.0.2/pyaicodingcube/
--rw-rw-rw-   0        0        0      247 2024-05-29 11:28:34.000000 pyaicodingcube-0.0.2/pyaicodingcube/__init__.py
--rw-rw-rw-   0        0        0    13811 2024-05-31 13:43:20.000000 pyaicodingcube-0.0.2/pyaicodingcube/pyaicodingcube.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:42:08.727210 pyaicodingcube-0.0.2/pyaicodingcube.egg-info/
--rw-rw-rw-   0        0        0       86 2024-05-31 14:42:08.000000 pyaicodingcube-0.0.2/pyaicodingcube.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-31 14:42:08.000000 pyaicodingcube-0.0.2/pyaicodingcube.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 14:42:08.000000 pyaicodingcube-0.0.2/pyaicodingcube.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-31 14:42:08.000000 pyaicodingcube-0.0.2/pyaicodingcube.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 14:42:08.729468 pyaicodingcube-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-05-29 11:28:18.000000 pyaicodingcube-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:39:01.408492 pyaicodingcube-0.0.3/
+-rw-rw-rw-   0        0        0       86 2024-06-01 13:39:01.406979 pyaicodingcube-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 13:39:01.355402 pyaicodingcube-0.0.3/pyaicodingcube/
+-rw-rw-rw-   0        0        0      249 2024-06-01 13:35:20.000000 pyaicodingcube-0.0.3/pyaicodingcube/__init__.py
+-rw-rw-rw-   0        0        0    13811 2024-05-31 13:43:20.000000 pyaicodingcube-0.0.3/pyaicodingcube/pyaicodingcube.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:39:01.402045 pyaicodingcube-0.0.3/pyaicodingcube.egg-info/
+-rw-rw-rw-   0        0        0       86 2024-06-01 13:39:01.000000 pyaicodingcube-0.0.3/pyaicodingcube.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-06-01 13:39:01.000000 pyaicodingcube-0.0.3/pyaicodingcube.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:39:01.000000 pyaicodingcube-0.0.3/pyaicodingcube.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 13:39:01.000000 pyaicodingcube-0.0.3/pyaicodingcube.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 13:39:01.408492 pyaicodingcube-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-06-01 13:35:49.000000 pyaicodingcube-0.0.3/setup.py
```

### Comparing `pyaicodingcube-0.0.2/pyaicodingcube/pyaicodingcube.py` & `pyaicodingcube-0.0.3/pyaicodingcube/pyaicodingcube.py`

 * *Files identical despite different names*

