# Comparing `tmp/twelvelabs-0.1.24.tar.gz` & `tmp/twelvelabs-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twelvelabs-0.1.24.tar", last modified: Fri May 17 03:30:16 2024, max compression
+gzip compressed data, was "twelvelabs-0.1.25.tar", last modified: Sat Jun  1 06:08:02 2024, max compression
```

## Comparing `twelvelabs-0.1.24.tar` & `twelvelabs-0.1.25.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.406175 twelvelabs-0.1.24/twelvelabs/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.406175 twelvelabs-0.1.24/twelvelabs/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/models/video.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/twelvelabs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/resources/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.410175 twelvelabs-0.1.24/twelvelabs/types/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/types/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-17 03:30:07.000000 twelvelabs-0.1.24/twelvelabs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:30:16.406175 twelvelabs-0.1.24/twelvelabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 03:30:16.000000 twelvelabs-0.1.24/twelvelabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:08:02.440201 twelvelabs-0.1.25/
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-06-01 06:08:02.440201 twelvelabs-0.1.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:08:02.440201 twelvelabs-0.1.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:08:02.436201 twelvelabs-0.1.25/twelvelabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:08:02.436201 twelvelabs-0.1.25/twelvelabs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/models/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:08:02.440201 twelvelabs-0.1.25/twelvelabs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/resources/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:08:02.440201 twelvelabs-0.1.25/twelvelabs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/types/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-06-01 06:07:52.000000 twelvelabs-0.1.25/twelvelabs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:08:02.436201 twelvelabs-0.1.25/twelvelabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-06-01 06:08:02.000000 twelvelabs-0.1.25/twelvelabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-06-01 06:08:02.000000 twelvelabs-0.1.25/twelvelabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:08:02.000000 twelvelabs-0.1.25/twelvelabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 06:08:02.000000 twelvelabs-0.1.25/twelvelabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 06:08:02.000000 twelvelabs-0.1.25/twelvelabs.egg-info/top_level.txt
```

### Comparing `twelvelabs-0.1.24/LICENSE` & `twelvelabs-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/PKG-INFO` & `twelvelabs-0.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.24
+Version: 0.1.25
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
 License: UNKNOWN
 Description: # TwelveLabs Python SDK
         [![PyPI version](https://img.shields.io/pypi/v/twelvelabs.svg)](https://pypi.org/project/twelvelabs/)
```

### Comparing `twelvelabs-0.1.24/README.md` & `twelvelabs-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/setup.py` & `twelvelabs-0.1.25/setup.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/__init__.py` & `twelvelabs-0.1.25/twelvelabs/__init__.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/base_client.py` & `twelvelabs-0.1.25/twelvelabs/base_client.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/client.py` & `twelvelabs-0.1.25/twelvelabs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 class TwelveLabs(APIClient):
     engine: resources.Engine
     index: resources.Index
     task: resources.Task
     search: resources.Search
     generate: resources.Generate
     classify: resources.Classify
+    embed: resources.Embed
 
     base_url: str
     api_key: str
 
     def __init__(
         self,
         api_key: str,
@@ -40,13 +41,14 @@
 
         self.engine = resources.Engine(self)
         self.index = resources.Index(self)
         self.task = resources.Task(self)
         self.search = resources.Search(self)
         self.generate = resources.Generate(self)
         self.classify = resources.Classify(self)
+        self.embed = resources.Embed(self)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc, tb):
         pass
```

### Comparing `twelvelabs-0.1.24/twelvelabs/exceptions.py` & `twelvelabs-0.1.25/twelvelabs/exceptions.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/models/_base.py` & `twelvelabs-0.1.25/twelvelabs/models/_base.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/models/classify.py` & `twelvelabs-0.1.25/twelvelabs/models/classify.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 class ClassifyDetailedScore(BaseModel):
     max_score: float
     avg_score: float
     normalized_score: float
 
 
 class ClassifyClip(BaseModel):
-    start: int
-    end: int
+    start: float
+    end: float
     score: float
     option: str
     prompt: str
     thumbnail_url: Optional[str] = None
     detailed_scores: Optional[ClassifyDetailedScore] = None
```

### Comparing `twelvelabs-0.1.24/twelvelabs/models/generate.py` & `twelvelabs-0.1.25/twelvelabs/models/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/models/index.py` & `twelvelabs-0.1.25/twelvelabs/models/index.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/models/search.py` & `twelvelabs-0.1.25/twelvelabs/models/search.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/models/task.py` & `twelvelabs-0.1.25/twelvelabs/models/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def delete(self, **kwargs) -> None:
         return self._resource.delete(self.id, **kwargs)
 
     def wait_for_done(
         self,
         *,
         sleep_interval: float = 5.0,
-        callback: Optional[Callable[[Task], None]],
+        callback: Optional[Callable[[Task], None]] = None,
         **kwargs,
     ) -> Task:
         if sleep_interval <= 0:
             raise ValueError("sleep_interval must be greater than 0")
         while not self.done:
             self._resource._sleep(sleep_interval)
             task = self.retrieve(**kwargs)
```

### Comparing `twelvelabs-0.1.24/twelvelabs/models/video.py` & `twelvelabs-0.1.25/twelvelabs/models/video.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/resources/classify.py` & `twelvelabs-0.1.25/twelvelabs/resources/classify.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/resources/generate.py` & `twelvelabs-0.1.25/twelvelabs/resources/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/resources/index.py` & `twelvelabs-0.1.25/twelvelabs/resources/index.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/resources/search.py` & `twelvelabs-0.1.25/twelvelabs/resources/search.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/resources/task.py` & `twelvelabs-0.1.25/twelvelabs/resources/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,19 +122,23 @@
         opened_files: List[BinaryIO] = []
         # TODO validate video supported (ffmpeg)
         if file is not None:
             if isinstance(file, str):
                 file = open(file, "rb")
                 opened_files.append(file)
             files["video_file"] = file
+        else:
+            # Request should be sent as multipart-form even file not exists
+            files["dummy"] = ("", "")
+
         if transcription_file is not None:
             if isinstance(transcription_file, str):
                 transcription_file = open(transcription_file, "rb")
                 opened_files.append(transcription_file)
-            data["transcription_file"] = transcription_file
+            files["transcription_file"] = transcription_file
             data["provide_transcription"] = True
         if transcription_url is not None:
             data["provide_transcription"] = True
 
         try:
             res = self._post(
                 "tasks", data=remove_none_values(data), files=files, **kwargs
```

### Comparing `twelvelabs-0.1.24/twelvelabs/resources/video.py` & `twelvelabs-0.1.25/twelvelabs/resources/video.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs/util.py` & `twelvelabs-0.1.25/twelvelabs/util.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.24/twelvelabs.egg-info/PKG-INFO` & `twelvelabs-0.1.25/twelvelabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.24
+Version: 0.1.25
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
 License: UNKNOWN
 Description: # TwelveLabs Python SDK
         [![PyPI version](https://img.shields.io/pypi/v/twelvelabs.svg)](https://pypi.org/project/twelvelabs/)
```

### Comparing `twelvelabs-0.1.24/twelvelabs.egg-info/SOURCES.txt` & `twelvelabs-0.1.25/twelvelabs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 twelvelabs.egg-info/SOURCES.txt
 twelvelabs.egg-info/dependency_links.txt
 twelvelabs.egg-info/requires.txt
 twelvelabs.egg-info/top_level.txt
 twelvelabs/models/__init__.py
 twelvelabs/models/_base.py
 twelvelabs/models/classify.py
+twelvelabs/models/embed.py
 twelvelabs/models/engine.py
 twelvelabs/models/generate.py
 twelvelabs/models/index.py
 twelvelabs/models/search.py
 twelvelabs/models/task.py
 twelvelabs/models/video.py
 twelvelabs/resources/__init__.py
 twelvelabs/resources/classify.py
+twelvelabs/resources/embed.py
 twelvelabs/resources/engine.py
 twelvelabs/resources/generate.py
 twelvelabs/resources/index.py
 twelvelabs/resources/search.py
 twelvelabs/resources/task.py
 twelvelabs/resources/video.py
 twelvelabs/types/__init__.py
```

