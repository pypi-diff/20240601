# Comparing `tmp/easyfileops-0.1.5.tar.gz` & `tmp/easyfileops-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfileops-0.1.5.tar", last modified: Sat Jun  1 20:22:55 2024, max compression
+gzip compressed data, was "easyfileops-0.1.55.tar", last modified: Sat Jun  1 20:28:19 2024, max compression
```

## Comparing `easyfileops-0.1.5.tar` & `easyfileops-0.1.55.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 20:22:55.930440 easyfileops-0.1.5/
-drwxrwxrwx   0        0        0        0 2024-06-01 20:22:55.904761 easyfileops-0.1.5/EasyFileOps/
--rw-rw-rw-   0        0        0        0 2024-06-01 20:12:49.000000 easyfileops-0.1.5/EasyFileOps/__init__.py
--rw-rw-rw-   0        0        0     8255 2024-06-01 20:22:45.000000 easyfileops-0.1.5/EasyFileOps/file.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:22:55.924761 easyfileops-0.1.5/EasyFileOps.egg-info/
--rw-rw-rw-   0        0        0      167 2024-06-01 20:22:55.000000 easyfileops-0.1.5/EasyFileOps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-06-01 20:22:55.000000 easyfileops-0.1.5/EasyFileOps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 20:22:55.000000 easyfileops-0.1.5/EasyFileOps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 20:22:55.000000 easyfileops-0.1.5/EasyFileOps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      167 2024-06-01 20:22:55.929879 easyfileops-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1702 2024-06-01 20:22:45.000000 easyfileops-0.1.5/README.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 20:22:55.930440 easyfileops-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      265 2024-06-01 20:22:45.000000 easyfileops-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:28:19.875213 easyfileops-0.1.55/
+drwxrwxrwx   0        0        0        0 2024-06-01 20:28:19.844730 easyfileops-0.1.55/EasyFileOps/
+-rw-rw-rw-   0        0        0        0 2024-06-01 20:12:49.000000 easyfileops-0.1.55/EasyFileOps/__init__.py
+-rw-rw-rw-   0        0        0     8301 2024-06-01 20:27:46.000000 easyfileops-0.1.55/EasyFileOps/file.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:28:19.875213 easyfileops-0.1.55/EasyFileOps.egg-info/
+-rw-rw-rw-   0        0        0      168 2024-06-01 20:28:19.000000 easyfileops-0.1.55/EasyFileOps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-06-01 20:28:19.000000 easyfileops-0.1.55/EasyFileOps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 20:28:19.000000 easyfileops-0.1.55/EasyFileOps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 20:28:19.000000 easyfileops-0.1.55/EasyFileOps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      168 2024-06-01 20:28:19.875213 easyfileops-0.1.55/PKG-INFO
+-rw-rw-rw-   0        0        0     1748 2024-06-01 20:27:46.000000 easyfileops-0.1.55/README.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 20:28:19.882690 easyfileops-0.1.55/setup.cfg
+-rw-rw-rw-   0        0        0      266 2024-06-01 20:26:03.000000 easyfileops-0.1.55/setup.py
```

### Comparing `easyfileops-0.1.5/EasyFileOps/file.py` & `easyfileops-0.1.55/EasyFileOps/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ###
 ###
 You can install EasyFileOps via pip:
 pip install EasyFileOps
 ###
 ###
 Importing:
-from EasyFileOps import file
+from EasyFileOps import file as efo (or any name you want)
 ###
 ###
 EasyFileOps main method is file
 Parameters of file:
 filename (str) - Here write a file name to operate on
 option (str) - Available options: r, r+, rb, rb+, readline, readlines, readable, w, w+, wb, wb+, writelines, writable,
 a, a+, ab, ab+, seekable, flush, detach, fileno, truncate, isatty, split, splitlines
@@ -39,24 +39,24 @@
 option split:
 -words: return words in file
 ###
 ###
 Example usages
 
 #Reading entire content of file
-content, lines = file("example.txt", "r")
+content, lines = efo.file("example.txt", "r")
 
 #Wrinting content to a file
-file("example.txt", "w", "Hi EasyFileOps!")
+efo.file("example.txt", "w", "Hi EasyFileOps!")
 
 #or writing with seek
-file("example.txt", "w", "Hi EasyFileOps!", 8)
+efo.file("example.txt", "w", "Hi EasyFileOps!", 8)
 
 #Truncate
-file("example.txt", "truncate", 40)
+efo.file("example.txt", "truncate", 40)
 ###
 ###
 IMPORTANT!!!
 if you use these options: seekable, writable, readable, truncate or detach constructions changes:
 -for seekable, writable, readable: file("example.txt", "seekable, writable or readable option", "option any with r, w or a")
 -for truncate: file("example.txt", "truncate", "(bytes in int)")
 -for detach: file("example.txt", "detach", "option any with r, w or a")
```

### Comparing `easyfileops-0.1.5/README.txt` & `easyfileops-0.1.55/README.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ###
 ###
 You can install EasyFileOps via pip:
 pip install EasyFileOps
 ###
 ###
 Importing:
-from EasyFileOps import file
+from EasyFileOps import file as efo (or any name you want)
 ###
 ###
 EasyFileOps main method is file
 Parameters of file:
 filename (str) - Here write a file name to operate on
 option (str) - Available options: r, r+, rb, rb+, readline, readlines, readable, w, w+, wb, wb+, writelines, writable,
 a, a+, ab, ab+, seekable, flush, detach, fileno, truncate, isatty, split, splitlines
@@ -35,24 +35,24 @@
 option split:
 -words: return words in file
 ###
 ###
 Example usages
 
 #Reading entire content of file
-content, lines = file("example.txt", "r")
+content, lines = efo.file("example.txt", "r")
 
 #Wrinting content to a file
-file("example.txt", "w", "Hi EasyFileOps!")
+efo.file("example.txt", "w", "Hi EasyFileOps!")
 
 #or writing with seek
-file("example.txt", "w", "Hi EasyFileOps!", 8)
+efo.file("example.txt", "w", "Hi EasyFileOps!", 8)
 
 #Truncate
-file("example.txt", "truncate", 40)
+efo.file("example.txt", "truncate", 40)
 ###
 ###
 IMPORTANT!!!
 if you use these options: seekable, writable, readable, truncate or detach constructions changes:
 -for seekable, writable, readable: file("example.txt", "seekable, writable or readable option", "option any with r, w or a")
 -for truncate: file("example.txt", "truncate", "(bytes in int)")
 -for detach: file("example.txt", "detach", "option any with r, w or a")
```

