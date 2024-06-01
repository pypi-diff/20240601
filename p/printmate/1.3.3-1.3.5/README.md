# Comparing `tmp/printmate-1.3.3.tar.gz` & `tmp/printmate-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printmate-1.3.3.tar", last modified: Thu May 23 21:33:07 2024, max compression
+gzip compressed data, was "printmate-1.3.5.tar", last modified: Sat Jun  1 12:40:50 2024, max compression
```

## Comparing `printmate-1.3.3.tar` & `printmate-1.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 21:33:07.335690 printmate-1.3.3/
--rw-rw-rw-   0        0        0      819 2024-05-23 21:33:07.332197 printmate-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-23 21:30:50.000000 printmate-1.3.3/README.md
--rw-rw-rw-   0        0        0     1103 2024-05-15 21:05:01.000000 printmate-1.3.3/license
-drwxrwxrwx   0        0        0        0 2024-05-23 21:33:07.328184 printmate-1.3.3/printmate.egg-info/
--rw-rw-rw-   0        0        0      819 2024-05-23 21:33:06.000000 printmate-1.3.3/printmate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-23 21:33:07.000000 printmate-1.3.3/printmate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 21:33:06.000000 printmate-1.3.3/printmate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 21:33:06.000000 printmate-1.3.3/printmate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 21:33:06.000000 printmate-1.3.3/printmate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 21:33:07.335690 printmate-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      760 2024-05-23 21:32:52.000000 printmate-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:40:50.603105 printmate-1.3.5/
+-rw-rw-rw-   0        0        0      819 2024-06-01 12:40:50.587480 printmate-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-23 21:30:50.000000 printmate-1.3.5/README.md
+-rw-rw-rw-   0        0        0     1103 2024-05-15 21:05:01.000000 printmate-1.3.5/license
+drwxrwxrwx   0        0        0        0 2024-06-01 12:40:50.587480 printmate-1.3.5/printmate.egg-info/
+-rw-rw-rw-   0        0        0      819 2024-06-01 12:40:50.000000 printmate-1.3.5/printmate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-06-01 12:40:50.000000 printmate-1.3.5/printmate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:40:50.000000 printmate-1.3.5/printmate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 12:40:50.000000 printmate-1.3.5/printmate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:40:50.000000 printmate-1.3.5/printmate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 12:40:50.603105 printmate-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      760 2024-06-01 12:40:33.000000 printmate-1.3.5/setup.py
```

### Comparing `printmate-1.3.3/PKG-INFO` & `printmate-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: printmate
-Version: 1.3.3
+Version: 1.3.5
 Summary: A library used to print animated text
 Author: PyGaps CEO
 Author-email: soqratiakram33@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `printmate-1.3.3/license` & `printmate-1.3.5/license`

 * *Files identical despite different names*

### Comparing `printmate-1.3.3/printmate.egg-info/PKG-INFO` & `printmate-1.3.5/printmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: printmate
-Version: 1.3.3
+Version: 1.3.5
 Summary: A library used to print animated text
 Author: PyGaps CEO
 Author-email: soqratiakram33@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `printmate-1.3.3/setup.py` & `printmate-1.3.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="printmate",
-    version="1.3.3",
+    version="1.3.5",
     description="A library used to print animated text",
     long_description=README,
     long_description_content_type="text/markdown",
     author="PyGaps CEO",
     author_email="soqratiakram33@gmail.com",
     packages=find_packages(),
     classifiers=[
```

