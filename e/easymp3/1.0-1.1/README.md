# Comparing `tmp/easymp3-1.0.tar.gz` & `tmp/easymp3-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymp3-1.0.tar", last modified: Sat Jun  1 21:01:50 2024, max compression
+gzip compressed data, was "easymp3-1.1.tar", last modified: Sat Jun  1 21:14:53 2024, max compression
```

## Comparing `easymp3-1.0.tar` & `easymp3-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:01:50.983308 easymp3-1.0/
--rw-rw-rw-   0        0        0     1090 2024-06-01 20:31:31.000000 easymp3-1.0/LICENSE
--rw-rw-rw-   0        0        0     6892 2024-06-01 21:01:50.983308 easymp3-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6717 2024-06-01 20:31:31.000000 easymp3-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:01:50.959133 easymp3-1.0/easymp3/
--rw-rw-rw-   0        0        0       35 2024-06-01 20:36:23.000000 easymp3-1.0/easymp3/__init__.py
--rw-rw-rw-   0        0        0    13994 2024-05-31 04:54:33.000000 easymp3-1.0/easymp3/easymp3.py
--rw-rw-rw-   0        0        0      514 2024-06-01 20:30:47.000000 easymp3-1.0/easymp3/exception.py
--rw-rw-rw-   0        0        0     2603 2024-05-28 00:56:24.000000 easymp3-1.0/easymp3/tag.py
--rw-rw-rw-   0        0        0     9855 2024-05-28 00:56:24.000000 easymp3-1.0/easymp3/util.py
-drwxrwxrwx   0        0        0        0 2024-06-01 21:01:50.982300 easymp3-1.0/easymp3.egg-info/
--rw-rw-rw-   0        0        0     6892 2024-06-01 21:01:50.000000 easymp3-1.0/easymp3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-06-01 21:01:50.000000 easymp3-1.0/easymp3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:01:50.000000 easymp3-1.0/easymp3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-06-01 21:01:50.000000 easymp3-1.0/easymp3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-01 21:01:50.000000 easymp3-1.0/easymp3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 21:01:50.984313 easymp3-1.0/setup.cfg
--rw-rw-rw-   0        0        0      410 2024-06-01 21:01:18.000000 easymp3-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:14:53.749537 easymp3-1.1/
+-rw-rw-rw-   0        0        0     1090 2024-06-01 20:31:31.000000 easymp3-1.1/LICENSE
+-rw-rw-rw-   0        0        0     6961 2024-06-01 21:14:53.748471 easymp3-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6717 2024-06-01 20:31:31.000000 easymp3-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 21:14:53.737324 easymp3-1.1/easymp3/
+-rw-rw-rw-   0        0        0       35 2024-06-01 20:36:23.000000 easymp3-1.1/easymp3/__init__.py
+-rw-rw-rw-   0        0        0    13994 2024-05-31 04:54:33.000000 easymp3-1.1/easymp3/easymp3.py
+-rw-rw-rw-   0        0        0      514 2024-06-01 20:30:47.000000 easymp3-1.1/easymp3/exception.py
+-rw-rw-rw-   0        0        0     2603 2024-05-28 00:56:24.000000 easymp3-1.1/easymp3/tag.py
+-rw-rw-rw-   0        0        0     9855 2024-05-28 00:56:24.000000 easymp3-1.1/easymp3/util.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:14:53.747516 easymp3-1.1/easymp3.egg-info/
+-rw-rw-rw-   0        0        0     6961 2024-06-01 21:14:53.000000 easymp3-1.1/easymp3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-06-01 21:14:53.000000 easymp3-1.1/easymp3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:14:53.000000 easymp3-1.1/easymp3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-01 21:14:53.000000 easymp3-1.1/easymp3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 21:14:53.000000 easymp3-1.1/easymp3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 21:14:53.749537 easymp3-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      489 2024-06-01 21:14:49.000000 easymp3-1.1/setup.py
```

### Comparing `easymp3-1.0/LICENSE` & `easymp3-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easymp3-1.0/PKG-INFO` & `easymp3-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: easymp3
-Version: 1.0
+Version: 1.1
+Summary: Easily tag and manipulate MP3 files in a programmatic way.
 Author: Chase Minert
 Author-email: cminert58@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EasyMP3
```

### Comparing `easymp3-1.0/README.md` & `easymp3-1.1/README.md`

 * *Files identical despite different names*

### Comparing `easymp3-1.0/easymp3/easymp3.py` & `easymp3-1.1/easymp3/easymp3.py`

 * *Files identical despite different names*

### Comparing `easymp3-1.0/easymp3/exception.py` & `easymp3-1.1/easymp3/exception.py`

 * *Files identical despite different names*

### Comparing `easymp3-1.0/easymp3/tag.py` & `easymp3-1.1/easymp3/tag.py`

 * *Files identical despite different names*

### Comparing `easymp3-1.0/easymp3/util.py` & `easymp3-1.1/easymp3/util.py`

 * *Files identical despite different names*

### Comparing `easymp3-1.0/easymp3.egg-info/PKG-INFO` & `easymp3-1.1/easymp3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: easymp3
-Version: 1.0
+Version: 1.1
+Summary: Easily tag and manipulate MP3 files in a programmatic way.
 Author: Chase Minert
 Author-email: cminert58@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EasyMP3
```

