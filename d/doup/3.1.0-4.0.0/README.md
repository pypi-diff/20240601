# Comparing `tmp/doup-3.1.0.tar.gz` & `tmp/doup-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doup-3.1.0.tar", last modified: Sat Feb 25 20:36:16 2023, max compression
+gzip compressed data, was "doup-4.0.0.tar", last modified: Sat Oct 14 20:08:08 2023, max compression
```

## Comparing `doup-3.1.0.tar` & `doup-4.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 20:36:16.981395 doup-3.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-02-25 20:35:23.000000 doup-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2992 2023-02-25 20:36:16.981395 doup-3.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-02-25 20:35:23.000000 doup-3.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-02-25 20:35:23.000000 doup-3.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-02-25 20:36:16.982395 doup-3.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-02-25 20:35:23.000000 doup-3.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 20:36:16.972394 doup-3.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 20:36:16.976394 doup-3.1.0/src/doup/
--rw-rw-rw-   0 root         (0) root         (0)     2307 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/EntryPoint.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 20:36:16.979395 doup-3.1.0/src/doup/analyzer/
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/analyzer/ImageNameAnalyzer.py
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/analyzer/StringAnalyzer.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/analyzer/TagAnalyzer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 20:36:16.980394 doup-3.1.0/src/doup/crawler/
--rw-rw-rw-   0 root         (0) root         (0)     2323 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/crawler/DirectoryCrawler.py
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/crawler/DockerhubCrawler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 20:36:16.980394 doup-3.1.0/src/doup/dto/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/dto/DirectorySummary.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/dto/DockerImage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 20:36:16.981395 doup-3.1.0/src/doup/services/
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/services/FileService.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-02-25 20:35:23.000000 doup-3.1.0/src/doup/services/OutputService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 20:36:16.978394 doup-3.1.0/src/doup.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2992 2023-02-25 20:36:16.000000 doup-3.1.0/src/doup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-25 20:36:16.000000 doup-3.1.0/src/doup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-25 20:36:16.000000 doup-3.1.0/src/doup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-02-25 20:36:16.000000 doup-3.1.0/src/doup.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-02-25 20:36:16.000000 doup-3.1.0/src/doup.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-25 20:36:16.000000 doup-3.1.0/src/doup.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-14 20:08:08.049195 doup-4.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-10-14 20:07:42.000000 doup-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3095 2023-10-14 20:08:08.049195 doup-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2023-10-14 20:07:42.000000 doup-4.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-10-14 20:07:42.000000 doup-4.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-10-14 20:08:08.049195 doup-4.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-10-14 20:07:42.000000 doup-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-14 20:08:08.045195 doup-4.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-14 20:08:08.045195 doup-4.0.0/src/doup/
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/EntryPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-14 20:08:08.049195 doup-4.0.0/src/doup/analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/analyzer/ImageNameAnalyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/analyzer/StringAnalyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/analyzer/TagAnalyzer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-14 20:08:08.049195 doup-4.0.0/src/doup/crawler/
+-rw-rw-rw-   0 root         (0) root         (0)     2323 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/crawler/DirectoryCrawler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/crawler/DockerhubCrawler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-14 20:08:08.049195 doup-4.0.0/src/doup/dto/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/dto/DirectorySummary.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/dto/DockerImage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-14 20:08:08.049195 doup-4.0.0/src/doup/services/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/services/FileService.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-10-14 20:07:42.000000 doup-4.0.0/src/doup/services/OutputService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-14 20:08:08.049195 doup-4.0.0/src/doup.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3095 2023-10-14 20:08:08.000000 doup-4.0.0/src/doup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-10-14 20:08:08.000000 doup-4.0.0/src/doup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-14 20:08:08.000000 doup-4.0.0/src/doup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-10-14 20:08:08.000000 doup-4.0.0/src/doup.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-10-14 20:08:08.000000 doup-4.0.0/src/doup.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-10-14 20:08:08.000000 doup-4.0.0/src/doup.egg-info/top_level.txt
```

### Comparing `doup-3.1.0/LICENSE` & `doup-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/PKG-INFO` & `doup-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: doup
-Version: 3.1.0
+Version: 4.0.0
 Summary: doup is a command line tool to find and update Docker-Image-Strings in project files.
 Author-email: Kay Gerlitzki <developed@kygr.org>
 Project-URL: Homepage, https://gitlab.com/doup1/doup
 Project-URL: Bug Tracker, https://gitlab.com/doup1/doup/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: termcolor
+Requires-Dist: requests
+Requires-Dist: tabulate
+Requires-Dist: types-tabulate
 
 # 🚀 doup
 
 A command line tool to find and update dockertags in project files.
 
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 [![pipeline main](https://gitlab.com/doup1/doup/badges/main/pipeline.svg)](https://gitlab.com/doup1/doup/blob/feature/update_readme/README.md)
```

### Comparing `doup-3.1.0/README.md` & `doup-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/pyproject.toml` & `doup-4.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/src/doup/EntryPoint.py` & `doup-4.0.0/src/doup/EntryPoint.py`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/src/doup/analyzer/StringAnalyzer.py` & `doup-4.0.0/src/doup/analyzer/StringAnalyzer.py`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/src/doup/analyzer/TagAnalyzer.py` & `doup-4.0.0/src/doup/analyzer/TagAnalyzer.py`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/src/doup/crawler/DirectoryCrawler.py` & `doup-4.0.0/src/doup/crawler/DirectoryCrawler.py`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/src/doup/crawler/DockerhubCrawler.py` & `doup-4.0.0/src/doup/crawler/DockerhubCrawler.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,10 +33,11 @@
         "https://hub.docker.com/v2/repositories/" + repository + "/tags/?page_size=1000"
     )
 
     response = json.loads(requests.get(url).text)
     tags = []
     for result in response["results"]:
         for image in result["images"]:
-            if image["digest"] == digest:
+            tag_digest = image.get("digest")
+            if tag_digest and tag_digest == digest:
                 tags.append(result["name"])
     return tags
```

### Comparing `doup-3.1.0/src/doup/dto/DirectorySummary.py` & `doup-4.0.0/src/doup/dto/DirectorySummary.py`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/src/doup/dto/DockerImage.py` & `doup-4.0.0/src/doup/dto/DockerImage.py`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/src/doup/services/OutputService.py` & `doup-4.0.0/src/doup/services/OutputService.py`

 * *Files identical despite different names*

### Comparing `doup-3.1.0/src/doup.egg-info/PKG-INFO` & `doup-4.0.0/src/doup.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: doup
-Version: 3.1.0
+Version: 4.0.0
 Summary: doup is a command line tool to find and update Docker-Image-Strings in project files.
 Author-email: Kay Gerlitzki <developed@kygr.org>
 Project-URL: Homepage, https://gitlab.com/doup1/doup
 Project-URL: Bug Tracker, https://gitlab.com/doup1/doup/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: termcolor
+Requires-Dist: requests
+Requires-Dist: tabulate
+Requires-Dist: types-tabulate
 
 # 🚀 doup
 
 A command line tool to find and update dockertags in project files.
 
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 [![pipeline main](https://gitlab.com/doup1/doup/badges/main/pipeline.svg)](https://gitlab.com/doup1/doup/blob/feature/update_readme/README.md)
```

### Comparing `doup-3.1.0/src/doup.egg-info/SOURCES.txt` & `doup-4.0.0/src/doup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

