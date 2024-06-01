# Comparing `tmp/qwantz_metadata-2024.1.1.tar.gz` & `tmp/qwantz_metadata-2024.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwantz_metadata-2024.1.1.tar", last modified: Mon Jan  1 19:07:20 2024, max compression
+gzip compressed data, was "qwantz_metadata-2024.6.1.tar", last modified: Sat Jun  1 09:55:11 2024, max compression
```

## Comparing `qwantz_metadata-2024.1.1.tar` & `qwantz_metadata-2024.6.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-01-01 19:07:20.658341 qwantz_metadata-2024.1.1/
--rw-rw-r--   0 janek     (1000) janek     (1000)     1054 2023-09-21 15:57:17.000000 qwantz_metadata-2024.1.1/LICENSE
--rw-rw-r--   0 janek     (1000) janek     (1000)       31 2023-10-06 20:02:18.000000 qwantz_metadata-2024.1.1/MANIFEST.in
--rw-r--r--   0 janek     (1000) janek     (1000)     1971 2024-01-01 19:07:20.658341 qwantz_metadata-2024.1.1/PKG-INFO
--rw-rw-r--   0 janek     (1000) janek     (1000)     1063 2023-10-06 22:06:25.000000 qwantz_metadata-2024.1.1/README.md
--rw-rw-r--   0 janek     (1000) janek     (1000)      958 2024-01-01 19:05:50.000000 qwantz_metadata-2024.1.1/pyproject.toml
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-01-01 19:07:20.658341 qwantz_metadata-2024.1.1/qwantz_metadata/
--rw-rw-r--   0 janek     (1000) janek     (1000)       49 2023-10-06 20:02:31.000000 qwantz_metadata-2024.1.1/qwantz_metadata/__init__.py
--rw-rw-r--   0 janek     (1000) janek     (1000)     5678 2023-11-23 16:30:14.000000 qwantz_metadata-2024.1.1/qwantz_metadata/combine_metadata.py
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-01-01 19:07:20.658341 qwantz_metadata-2024.1.1/qwantz_metadata/data/
--rw-rw-r--   0 janek     (1000) janek     (1000)     1326 2023-10-06 22:06:24.000000 qwantz_metadata-2024.1.1/qwantz_metadata/data/extra_metadata.json
--rw-rw-r--   0 janek     (1000) janek     (1000)   150931 2023-10-28 10:06:49.000000 qwantz_metadata-2024.1.1/qwantz_metadata/data/guest_comics.json
--rw-rw-r--   0 janek     (1000) janek     (1000)    17696 2023-11-19 22:46:12.000000 qwantz_metadata-2024.1.1/qwantz_metadata/data/special_comics.json
--rw-rw-r--   0 janek     (1000) janek     (1000)     3453 2024-01-01 18:59:47.000000 qwantz_metadata-2024.1.1/qwantz_metadata/parse_qwantz_html.py
-drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-01-01 19:07:20.658341 qwantz_metadata-2024.1.1/qwantz_metadata.egg-info/
--rw-r--r--   0 janek     (1000) janek     (1000)     1971 2024-01-01 19:07:20.000000 qwantz_metadata-2024.1.1/qwantz_metadata.egg-info/PKG-INFO
--rw-rw-r--   0 janek     (1000) janek     (1000)      502 2024-01-01 19:07:20.000000 qwantz_metadata-2024.1.1/qwantz_metadata.egg-info/SOURCES.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)        1 2024-01-01 19:07:20.000000 qwantz_metadata-2024.1.1/qwantz_metadata.egg-info/dependency_links.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)       56 2024-01-01 19:07:20.000000 qwantz_metadata-2024.1.1/qwantz_metadata.egg-info/entry_points.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)       51 2024-01-01 19:07:20.000000 qwantz_metadata-2024.1.1/qwantz_metadata.egg-info/requires.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)       16 2024-01-01 19:07:20.000000 qwantz_metadata-2024.1.1/qwantz_metadata.egg-info/top_level.txt
--rw-rw-r--   0 janek     (1000) janek     (1000)       38 2024-01-01 19:07:20.658341 qwantz_metadata-2024.1.1/setup.cfg
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-06-01 09:55:11.545782 qwantz_metadata-2024.6.1/
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1054 2023-09-21 15:57:17.000000 qwantz_metadata-2024.6.1/LICENSE
+-rw-rw-r--   0 janek     (1000) janek     (1000)       31 2023-10-06 20:02:18.000000 qwantz_metadata-2024.6.1/MANIFEST.in
+-rw-r--r--   0 janek     (1000) janek     (1000)     1971 2024-06-01 09:55:11.545782 qwantz_metadata-2024.6.1/PKG-INFO
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1063 2023-10-06 22:06:25.000000 qwantz_metadata-2024.6.1/README.md
+-rw-rw-r--   0 janek     (1000) janek     (1000)      958 2024-06-01 09:54:24.000000 qwantz_metadata-2024.6.1/pyproject.toml
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-06-01 09:55:11.541782 qwantz_metadata-2024.6.1/qwantz_metadata/
+-rw-rw-r--   0 janek     (1000) janek     (1000)       49 2023-10-06 20:02:31.000000 qwantz_metadata-2024.6.1/qwantz_metadata/__init__.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     5678 2023-11-23 16:30:14.000000 qwantz_metadata-2024.6.1/qwantz_metadata/combine_metadata.py
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-06-01 09:55:11.541782 qwantz_metadata-2024.6.1/qwantz_metadata/data/
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1326 2023-10-06 22:06:24.000000 qwantz_metadata-2024.6.1/qwantz_metadata/data/extra_metadata.json
+-rw-rw-r--   0 janek     (1000) janek     (1000)   150472 2024-05-22 18:59:53.000000 qwantz_metadata-2024.6.1/qwantz_metadata/data/guest_comics.json
+-rw-rw-r--   0 janek     (1000) janek     (1000)    17696 2023-11-19 22:46:12.000000 qwantz_metadata-2024.6.1/qwantz_metadata/data/special_comics.json
+-rw-rw-r--   0 janek     (1000) janek     (1000)     1079 2024-05-23 19:17:16.000000 qwantz_metadata-2024.6.1/qwantz_metadata/hapax_legomena.py
+-rw-rw-r--   0 janek     (1000) janek     (1000)     3453 2024-05-22 20:46:49.000000 qwantz_metadata-2024.6.1/qwantz_metadata/parse_qwantz_html.py
+drwxrwxr-x   0 janek     (1000) janek     (1000)        0 2024-06-01 09:55:11.541782 qwantz_metadata-2024.6.1/qwantz_metadata.egg-info/
+-rw-r--r--   0 janek     (1000) janek     (1000)     1971 2024-06-01 09:55:11.000000 qwantz_metadata-2024.6.1/qwantz_metadata.egg-info/PKG-INFO
+-rw-rw-r--   0 janek     (1000) janek     (1000)      536 2024-06-01 09:55:11.000000 qwantz_metadata-2024.6.1/qwantz_metadata.egg-info/SOURCES.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)        1 2024-06-01 09:55:11.000000 qwantz_metadata-2024.6.1/qwantz_metadata.egg-info/dependency_links.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)       56 2024-06-01 09:55:11.000000 qwantz_metadata-2024.6.1/qwantz_metadata.egg-info/entry_points.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)       51 2024-06-01 09:55:11.000000 qwantz_metadata-2024.6.1/qwantz_metadata.egg-info/requires.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)       16 2024-06-01 09:55:11.000000 qwantz_metadata-2024.6.1/qwantz_metadata.egg-info/top_level.txt
+-rw-rw-r--   0 janek     (1000) janek     (1000)       38 2024-06-01 09:55:11.545782 qwantz_metadata-2024.6.1/setup.cfg
```

### Comparing `qwantz_metadata-2024.1.1/LICENSE` & `qwantz_metadata-2024.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qwantz_metadata-2024.1.1/PKG-INFO` & `qwantz_metadata-2024.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwantz_metadata
-Version: 2024.1.1
+Version: 2024.6.1
 Summary: Prepare metadata document for Dinosaur Comics
 Author-email: Jan Szejko <jan.szejko@gmail.com>
 Project-URL: homepage, https://github.com/janek37/qwantz_metadata
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `qwantz_metadata-2024.1.1/README.md` & `qwantz_metadata-2024.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qwantz_metadata-2024.1.1/pyproject.toml` & `qwantz_metadata-2024.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "qwantz_metadata"
 authors = [{name = "Jan Szejko", email = "jan.szejko@gmail.com"}]
-version = "2024.1.1"
+version = "2024.6.1"
 description = "Prepare metadata document for Dinosaur Comics"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
     "Environment :: Console",
```

### Comparing `qwantz_metadata-2024.1.1/qwantz_metadata/combine_metadata.py` & `qwantz_metadata-2024.6.1/qwantz_metadata/combine_metadata.py`

 * *Files identical despite different names*

### Comparing `qwantz_metadata-2024.1.1/qwantz_metadata/data/extra_metadata.json` & `qwantz_metadata-2024.6.1/qwantz_metadata/data/extra_metadata.json`

 * *Files identical despite different names*

### Comparing `qwantz_metadata-2024.1.1/qwantz_metadata/data/guest_comics.json` & `qwantz_metadata-2024.6.1/qwantz_metadata/data/guest_comics.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9901960784313726%*

 * *Differences: {'delete': "['comic2-joey.png']"}*

```diff
@@ -755,42 +755,14 @@
             [
                 "Narrator: 6.) FREE GRADUAL, IRREVERSIBLE DECLINE OF YOUR BODY AND ITS FACULTIES OVER TIME",
                 "T-Rex: Maaan! This sucks, but I mean, we DID get to go to a free comics convention that one time.",
                 "T-Rex and Utahraptor: NO REGRETS!!"
             ]
         ]
     },
-    "comic2-joey.png": {
-        "comic_id": 509,
-        "footer": [
-            "(C) 2005 Ryan North",
-            "www.qwantz.com"
-        ],
-        "guest_artist": "Joey Comeau",
-        "panels": [
-            [
-                "T-Rex: Everybody dies."
-            ],
-            [
-                "\u301ano text\u301b"
-            ],
-            [
-                "\u301ano text\u301b"
-            ],
-            [
-                "\u301ano text\u301b"
-            ],
-            [
-                "\u301ano text\u301b"
-            ],
-            [
-                "T-Rex: But we've still got some time!"
-            ]
-        ]
-    },
     "firmanproductions.gif": {
         "comic_id": 1776,
         "description": "The comic uses a close-to-standard template with dinosaurs replaced by hand-drawn humans in wedding outfits, presumably Ryan North (as T-Rex) and Jenn Klug (as both Dromiceiomimus and Utahraptor)",
         "footer": [
             "Absolute best wishes to Ryan and Jennifer! Congratulations!"
         ],
         "guest_artist": "Michael Firman",
```

### Comparing `qwantz_metadata-2024.1.1/qwantz_metadata/data/special_comics.json` & `qwantz_metadata-2024.6.1/qwantz_metadata/data/special_comics.json`

 * *Files identical despite different names*

### Comparing `qwantz_metadata-2024.1.1/qwantz_metadata/parse_qwantz_html.py` & `qwantz_metadata-2024.6.1/qwantz_metadata/parse_qwantz_html.py`

 * *Files identical despite different names*

### Comparing `qwantz_metadata-2024.1.1/qwantz_metadata.egg-info/PKG-INFO` & `qwantz_metadata-2024.6.1/qwantz_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwantz_metadata
-Version: 2024.1.1
+Version: 2024.6.1
 Summary: Prepare metadata document for Dinosaur Comics
 Author-email: Jan Szejko <jan.szejko@gmail.com>
 Project-URL: homepage, https://github.com/janek37/qwantz_metadata
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

