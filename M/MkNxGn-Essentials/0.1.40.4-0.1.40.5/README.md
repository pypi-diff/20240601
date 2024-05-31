# Comparing `tmp/MkNxGn_Essentials-0.1.40.4.tar.gz` & `tmp/MkNxGn_Essentials-0.1.40.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MkNxGn_Essentials-0.1.40.4.tar", last modified: Tue Jan 30 21:04:24 2024, max compression
+gzip compressed data, was "MkNxGn_Essentials-0.1.40.5.tar", last modified: Fri May 31 23:43:48 2024, max compression
```

## Comparing `MkNxGn_Essentials-0.1.40.4.tar` & `MkNxGn_Essentials-0.1.40.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/cdn/
--rw-rw-rw-   0        0        0     2966 2021-08-17 20:54:39.000000 MkNxGn_Essentials-0.1.40.4/essentials/cdn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/conversation/
--rw-rw-rw-   0        0        0    17109 2023-10-03 20:30:09.000000 MkNxGn_Essentials-0.1.40.4/essentials/conversation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/file_ops/
--rw-rw-rw-   0        0        0     8405 2023-09-13 17:18:29.000000 MkNxGn_Essentials-0.1.40.4/essentials/file_ops/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/html/
--rw-rw-rw-   0        0        0      480 2022-12-19 19:31:34.000000 MkNxGn_Essentials-0.1.40.4/essentials/html/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/image_ops/
--rw-rw-rw-   0        0        0     2061 2024-01-30 21:04:09.000000 MkNxGn_Essentials-0.1.40.4/essentials/image_ops/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/logger_ops/
--rw-rw-rw-   0        0        0     1387 2020-04-26 12:02:05.000000 MkNxGn_Essentials-0.1.40.4/essentials/logger_ops/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/network_ops/
--rw-rw-rw-   0        0        0     4911 2023-08-30 22:40:51.000000 MkNxGn_Essentials-0.1.40.4/essentials/network_ops/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/objects/
--rw-rw-rw-   0        0        0     4799 2024-01-13 18:48:53.000000 MkNxGn_Essentials-0.1.40.4/essentials/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/run_data/
--rw-rw-rw-   0        0        0     4489 2020-04-20 23:16:23.000000 MkNxGn_Essentials-0.1.40.4/essentials/run_data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/search/
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/search/text/
--rw-rw-rw-   0        0        0    14279 2023-10-03 20:27:14.000000 MkNxGn_Essentials-0.1.40.4/essentials/search/text/__init__.py
--rw-rw-rw-   0        0        0        0 2020-08-09 21:10:07.000000 MkNxGn_Essentials-0.1.40.4/essentials/search/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/socket_ops/
--rw-rw-rw-   0        0        0    20856 2021-08-17 20:54:51.000000 MkNxGn_Essentials-0.1.40.4/essentials/socket_ops/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/socket_ops_v2/
--rw-rw-rw-   0        0        0    37165 2023-08-22 19:56:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/socket_ops_v2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/time_events/
--rw-rw-rw-   0        0        0     5803 2020-07-26 16:30:28.000000 MkNxGn_Essentials-0.1.40.4/essentials/time_events/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/tokening/
--rw-rw-rw-   0        0        0     1444 2020-01-20 16:31:26.000000 MkNxGn_Essentials-0.1.40.4/essentials/tokening/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/essentials/typing/
--rw-rw-rw-   0        0        0     5465 2023-05-15 18:56:11.000000 MkNxGn_Essentials-0.1.40.4/essentials/typing/__init__.py
--rw-rw-rw-   0        0        0    18886 2021-08-17 20:56:06.000000 MkNxGn_Essentials-0.1.40.4/essentials/__init__.py
--rw-rw-rw-   0        0        0     1091 2020-05-08 05:10:41.000000 MkNxGn_Essentials-0.1.40.4/LICENSE
-drwxrwxrwx   0        0        0        0 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/MkNxGn_Essentials.egg-info/
--rw-rw-rw-   0        0        0        1 2024-01-30 21:04:23.000000 MkNxGn_Essentials-0.1.40.4/MkNxGn_Essentials.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3492 2024-01-30 21:04:23.000000 MkNxGn_Essentials-0.1.40.4/MkNxGn_Essentials.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      734 2024-01-30 21:04:23.000000 MkNxGn_Essentials-0.1.40.4/MkNxGn_Essentials.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2024-01-30 21:04:23.000000 MkNxGn_Essentials-0.1.40.4/MkNxGn_Essentials.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3492 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/PKG-INFO
--rw-rw-rw-   0        0        0     3010 2020-08-09 21:19:20.000000 MkNxGn_Essentials-0.1.40.4/README.md
--rw-rw-rw-   0        0        0       42 2024-01-30 21:04:24.000000 MkNxGn_Essentials-0.1.40.4/setup.cfg
--rw-rw-rw-   0        0        0      685 2024-01-30 21:04:18.000000 MkNxGn_Essentials-0.1.40.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.865682 MkNxGn_Essentials-0.1.40.5/
+-rw-rw-rw-   0        0        0     1091 2020-05-08 05:10:41.000000 MkNxGn_Essentials-0.1.40.5/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.861683 MkNxGn_Essentials-0.1.40.5/MkNxGn_Essentials.egg-info/
+-rw-rw-rw-   0        0        0     3451 2024-05-31 23:43:48.000000 MkNxGn_Essentials-0.1.40.5/MkNxGn_Essentials.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2024-05-31 23:43:48.000000 MkNxGn_Essentials-0.1.40.5/MkNxGn_Essentials.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 23:43:48.000000 MkNxGn_Essentials-0.1.40.5/MkNxGn_Essentials.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 23:43:48.000000 MkNxGn_Essentials-0.1.40.5/MkNxGn_Essentials.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3451 2024-05-31 23:43:48.863682 MkNxGn_Essentials-0.1.40.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3010 2020-08-09 21:19:20.000000 MkNxGn_Essentials-0.1.40.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.754691 MkNxGn_Essentials-0.1.40.5/essentials/
+-rw-rw-rw-   0        0        0    18886 2021-08-17 20:56:06.000000 MkNxGn_Essentials-0.1.40.5/essentials/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.756691 MkNxGn_Essentials-0.1.40.5/essentials/cdn/
+-rw-rw-rw-   0        0        0     2966 2021-08-17 20:54:39.000000 MkNxGn_Essentials-0.1.40.5/essentials/cdn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.769729 MkNxGn_Essentials-0.1.40.5/essentials/conversation/
+-rw-rw-rw-   0        0        0    17109 2023-10-03 20:30:09.000000 MkNxGn_Essentials-0.1.40.5/essentials/conversation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.784690 MkNxGn_Essentials-0.1.40.5/essentials/file_ops/
+-rw-rw-rw-   0        0        0     8442 2024-05-31 23:31:45.000000 MkNxGn_Essentials-0.1.40.5/essentials/file_ops/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.788687 MkNxGn_Essentials-0.1.40.5/essentials/html/
+-rw-rw-rw-   0        0        0      480 2022-12-19 19:31:34.000000 MkNxGn_Essentials-0.1.40.5/essentials/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.792686 MkNxGn_Essentials-0.1.40.5/essentials/image_ops/
+-rw-rw-rw-   0        0        0     2061 2024-01-30 21:04:09.000000 MkNxGn_Essentials-0.1.40.5/essentials/image_ops/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.796687 MkNxGn_Essentials-0.1.40.5/essentials/logger_ops/
+-rw-rw-rw-   0        0        0     1387 2020-04-26 12:02:05.000000 MkNxGn_Essentials-0.1.40.5/essentials/logger_ops/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.800691 MkNxGn_Essentials-0.1.40.5/essentials/network_ops/
+-rw-rw-rw-   0        0        0     4911 2023-08-30 22:40:51.000000 MkNxGn_Essentials-0.1.40.5/essentials/network_ops/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.805688 MkNxGn_Essentials-0.1.40.5/essentials/objects/
+-rw-rw-rw-   0        0        0     4799 2024-01-13 18:48:53.000000 MkNxGn_Essentials-0.1.40.5/essentials/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.808683 MkNxGn_Essentials-0.1.40.5/essentials/run_data/
+-rw-rw-rw-   0        0        0     4489 2020-04-20 23:16:23.000000 MkNxGn_Essentials-0.1.40.5/essentials/run_data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.810684 MkNxGn_Essentials-0.1.40.5/essentials/search/
+-rw-rw-rw-   0        0        0        0 2020-08-09 21:10:07.000000 MkNxGn_Essentials-0.1.40.5/essentials/search/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.823683 MkNxGn_Essentials-0.1.40.5/essentials/search/text/
+-rw-rw-rw-   0        0        0    14279 2023-10-03 20:27:14.000000 MkNxGn_Essentials-0.1.40.5/essentials/search/text/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.838684 MkNxGn_Essentials-0.1.40.5/essentials/socket_ops/
+-rw-rw-rw-   0        0        0    20856 2021-08-17 20:54:51.000000 MkNxGn_Essentials-0.1.40.5/essentials/socket_ops/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.850685 MkNxGn_Essentials-0.1.40.5/essentials/socket_ops_v2/
+-rw-rw-rw-   0        0        0    37165 2023-08-22 19:56:24.000000 MkNxGn_Essentials-0.1.40.5/essentials/socket_ops_v2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.853682 MkNxGn_Essentials-0.1.40.5/essentials/time_events/
+-rw-rw-rw-   0        0        0     5803 2020-07-26 16:30:28.000000 MkNxGn_Essentials-0.1.40.5/essentials/time_events/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.856680 MkNxGn_Essentials-0.1.40.5/essentials/tokening/
+-rw-rw-rw-   0        0        0     1444 2020-01-20 16:31:26.000000 MkNxGn_Essentials-0.1.40.5/essentials/tokening/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 23:43:48.859683 MkNxGn_Essentials-0.1.40.5/essentials/typing/
+-rw-rw-rw-   0        0        0     5465 2023-05-15 18:56:11.000000 MkNxGn_Essentials-0.1.40.5/essentials/typing/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 23:43:48.866684 MkNxGn_Essentials-0.1.40.5/setup.cfg
+-rw-rw-rw-   0        0        0      685 2024-05-31 23:32:10.000000 MkNxGn_Essentials-0.1.40.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/cdn/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/cdn/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/conversation/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/file_ops/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/file_ops/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,29 +125,29 @@
         path = os.path.join(workingDir, path)
 
     if encrypt:
         return json.loads(DecodeWithKey(encrypt, read_file(path)))
 
     return json.loads(read_file(path))
 
-def read_file(path, byte=False, encrypt=False):
+def read_file(path, byte=False, encrypt=False, encoding="utf-8"):
     """
     Read File
     
     Read and returns data From a file optionally gives bytes to read in bytes format
 
     path - String: Dir of the json file
     byte - Bool, False: Read as bytes, defaults to false."""
     if workingDir != False:
         path = os.path.join(workingDir, path)
 
     if byte:
         file = open(path, "rb")
     else:
-        file = open(path, "r")
+        file = open(path, "r", encoding=encoding)
     data = file.read()
     file.close()
     if encrypt:
         return DecodeWithKey(encrypt, data)
     return data
 
 def write_file(path, data, append=False, byte=False, encrypt=False, encoding="utf-8"):
```

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/image_ops/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/image_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/logger_ops/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/logger_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/network_ops/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/network_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/objects/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/run_data/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/run_data/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/search/text/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/search/text/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/socket_ops/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/socket_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/socket_ops_v2/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/socket_ops_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/time_events/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/time_events/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/tokening/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/tokening/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/typing/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/essentials/__init__.py` & `MkNxGn_Essentials-0.1.40.5/essentials/__init__.py`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/LICENSE` & `MkNxGn_Essentials-0.1.40.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/MkNxGn_Essentials.egg-info/PKG-INFO` & `MkNxGn_Essentials-0.1.40.5/MkNxGn_Essentials.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
-Name: MkNxGn-Essentials
-Version: 0.1.40.4
+Name: MkNxGn_Essentials
+Version: 0.1.40.5
 Summary: MkNxGn File Writing, Network Essentials and More - A lot more
 Home-page: https://mknxgn.com/
 Author: Mark Cartagena
 Author-email: mark@mknxgn.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mknxgn_essentials
@@ -106,9 +104,7 @@
 Includes:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Text search - reason; Matches a query to multiple phrases and words and finds the best solution<br>
 <br>
 
 ``` python
 from essentials.search import text
 ```
-
-
```

### Comparing `MkNxGn_Essentials-0.1.40.4/MkNxGn_Essentials.egg-info/SOURCES.txt` & `MkNxGn_Essentials-0.1.40.5/MkNxGn_Essentials.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/PKG-INFO` & `MkNxGn_Essentials-0.1.40.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: MkNxGn_Essentials
-Version: 0.1.40.4
+Version: 0.1.40.5
 Summary: MkNxGn File Writing, Network Essentials and More - A lot more
 Home-page: https://mknxgn.com/
 Author: Mark Cartagena
 Author-email: mark@mknxgn.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mknxgn_essentials
@@ -106,9 +104,7 @@
 Includes:<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Text search - reason; Matches a query to multiple phrases and words and finds the best solution<br>
 <br>
 
 ``` python
 from essentials.search import text
 ```
-
-
```

### Comparing `MkNxGn_Essentials-0.1.40.4/README.md` & `MkNxGn_Essentials-0.1.40.5/README.md`

 * *Files identical despite different names*

### Comparing `MkNxGn_Essentials-0.1.40.4/setup.py` & `MkNxGn_Essentials-0.1.40.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MkNxGn_Essentials",
-    version="0.1.40.4",
+    version="0.1.40.5",
     author="Mark Cartagena",
     author_email="mark@mknxgn.com",
     description="MkNxGn File Writing, Network Essentials and More - A lot more",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mknxgn.com/",
     install_requires=[],
```

