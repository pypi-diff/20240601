# Comparing `tmp/resemble-1.4.2.tar.gz` & `tmp/resemble-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resemble-1.4.2.tar", last modified: Sat Dec  9 00:59:38 2023, max compression
+gzip compressed data, was "resemble-1.4.3.tar", last modified: Sat Jun  1 01:37:43 2024, max compression
```

## Comparing `resemble-1.4.2.tar` & `resemble-1.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tedi       (501) staff       (20)        0 2023-12-09 00:59:38.960393 resemble-1.4.2/
--rw-r--r--   0 tedi       (501) staff       (20)     1077 2022-01-12 16:46:53.000000 resemble-1.4.2/LICENSE
--rw-r--r--   0 tedi       (501) staff       (20)     2648 2023-12-09 00:59:38.960142 resemble-1.4.2/PKG-INFO
--rw-r--r--   0 tedi       (501) staff       (20)     2098 2023-12-04 16:51:49.000000 resemble-1.4.2/README.md
--rw-r--r--   0 tedi       (501) staff       (20)       98 2022-01-12 16:46:53.000000 resemble-1.4.2/pyproject.toml
-drwxr-xr-x   0 tedi       (501) staff       (20)        0 2023-12-09 00:59:38.958456 resemble-1.4.2/resemble/
--rw-r--r--   0 tedi       (501) staff       (20)    22292 2023-12-09 00:59:08.000000 resemble-1.4.2/resemble/__init__.py
--rw-r--r--   0 tedi       (501) staff       (20)     1611 2022-02-02 03:22:01.000000 resemble-1.4.2/resemble/stream_decoder.py
-drwxr-xr-x   0 tedi       (501) staff       (20)        0 2023-12-09 00:59:38.959907 resemble-1.4.2/resemble.egg-info/
--rw-r--r--   0 tedi       (501) staff       (20)     2648 2023-12-09 00:59:38.000000 resemble-1.4.2/resemble.egg-info/PKG-INFO
--rw-r--r--   0 tedi       (501) staff       (20)      265 2023-12-09 00:59:38.000000 resemble-1.4.2/resemble.egg-info/SOURCES.txt
--rw-r--r--   0 tedi       (501) staff       (20)        1 2023-12-09 00:59:38.000000 resemble-1.4.2/resemble.egg-info/dependency_links.txt
--rw-r--r--   0 tedi       (501) staff       (20)       14 2023-12-09 00:59:38.000000 resemble-1.4.2/resemble.egg-info/requires.txt
--rw-r--r--   0 tedi       (501) staff       (20)        9 2023-12-09 00:59:38.000000 resemble-1.4.2/resemble.egg-info/top_level.txt
--rw-r--r--   0 tedi       (501) staff       (20)       38 2023-12-09 00:59:38.960437 resemble-1.4.2/setup.cfg
--rw-r--r--   0 tedi       (501) staff       (20)      772 2023-12-09 00:59:08.000000 resemble-1.4.2/setup.py
-drwxr-xr-x   0 tedi       (501) staff       (20)        0 2023-12-09 00:59:38.959484 resemble-1.4.2/tests/
--rw-r--r--   0 tedi       (501) staff       (20)     6522 2023-12-04 16:51:49.000000 resemble-1.4.2/tests/test_v2.py
+drwxr-xr-x   0 tedi       (501) staff       (20)        0 2024-06-01 01:37:43.412728 resemble-1.4.3/
+-rw-r--r--   0 tedi       (501) staff       (20)     1077 2022-01-12 16:46:53.000000 resemble-1.4.3/LICENSE
+-rw-r--r--   0 tedi       (501) staff       (20)     2648 2024-06-01 01:37:43.412541 resemble-1.4.3/PKG-INFO
+-rw-r--r--   0 tedi       (501) staff       (20)     2098 2023-12-04 16:51:49.000000 resemble-1.4.3/README.md
+-rw-r--r--   0 tedi       (501) staff       (20)       98 2022-01-12 16:46:53.000000 resemble-1.4.3/pyproject.toml
+drwxr-xr-x   0 tedi       (501) staff       (20)        0 2024-06-01 01:37:43.411284 resemble-1.4.3/resemble/
+-rw-r--r--   0 tedi       (501) staff       (20)    22432 2024-06-01 01:37:18.000000 resemble-1.4.3/resemble/__init__.py
+-rw-r--r--   0 tedi       (501) staff       (20)     1611 2022-02-02 03:22:01.000000 resemble-1.4.3/resemble/stream_decoder.py
+drwxr-xr-x   0 tedi       (501) staff       (20)        0 2024-06-01 01:37:43.412362 resemble-1.4.3/resemble.egg-info/
+-rw-r--r--   0 tedi       (501) staff       (20)     2648 2024-06-01 01:37:43.000000 resemble-1.4.3/resemble.egg-info/PKG-INFO
+-rw-r--r--   0 tedi       (501) staff       (20)      265 2024-06-01 01:37:43.000000 resemble-1.4.3/resemble.egg-info/SOURCES.txt
+-rw-r--r--   0 tedi       (501) staff       (20)        1 2024-06-01 01:37:43.000000 resemble-1.4.3/resemble.egg-info/dependency_links.txt
+-rw-r--r--   0 tedi       (501) staff       (20)       14 2024-06-01 01:37:43.000000 resemble-1.4.3/resemble.egg-info/requires.txt
+-rw-r--r--   0 tedi       (501) staff       (20)        9 2024-06-01 01:37:43.000000 resemble-1.4.3/resemble.egg-info/top_level.txt
+-rw-r--r--   0 tedi       (501) staff       (20)       38 2024-06-01 01:37:43.412760 resemble-1.4.3/setup.cfg
+-rw-r--r--   0 tedi       (501) staff       (20)      772 2024-06-01 01:37:18.000000 resemble-1.4.3/setup.py
+drwxr-xr-x   0 tedi       (501) staff       (20)        0 2024-06-01 01:37:43.412087 resemble-1.4.3/tests/
+-rw-r--r--   0 tedi       (501) staff       (20)     6522 2023-12-04 16:51:49.000000 resemble-1.4.3/tests/test_v2.py
```

### Comparing `resemble-1.4.2/LICENSE` & `resemble-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `resemble-1.4.2/PKG-INFO` & `resemble-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resemble
-Version: 1.4.2
+Version: 1.4.3
 Summary: Resemble API Client Library
 Home-page: https://github.com/resemble-ai/resemble-python
 Author: ResembleAI
 Author-email: team@resemble.ai
 Project-URL: Bug Tracker, https://github.com/resemble-ai/resemble-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resemble-1.4.2/README.md` & `resemble-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `resemble-1.4.2/resemble/__init__.py` & `resemble-1.4.3/resemble/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,23 +279,26 @@
             def all(self, page: int, page_size: int = None):
                 query = { 'page': page }
                 if page_size:
                     query['page_size'] = page_size
                 r = requests.get(Resemble.endpoint('v2', 'voices'), headers=Resemble._headers, params=query)
                 return r.json()
 
-            def create(self, name: str, consent: str, dataset_url: str = None, callback_uri: str = None):
+            def create(self, name: str, consent: str, dataset_url: str = None, callback_uri: str = None,
+                       voice_type: str = 'professional'):
                 json = {
                     'name': name,
                     'consent': consent
                 }
                 if dataset_url:
                     json['dataset_url'] = dataset_url
                 if callback_uri:
                     json['callback_uri'] = callback_uri
+                if voice_type:
+                    json['voice_type'] = voice_type
                 r = requests.post(Resemble.endpoint('v2', 'voices'), headers=Resemble._headers, json=json)
                 return r.json()
 
             def update(self, uuid: str, name: str, dataset_url: str = None):
                 json = {
                     'name': name
                 }
```

### Comparing `resemble-1.4.2/resemble/stream_decoder.py` & `resemble-1.4.3/resemble/stream_decoder.py`

 * *Files identical despite different names*

### Comparing `resemble-1.4.2/resemble.egg-info/PKG-INFO` & `resemble-1.4.3/resemble.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resemble
-Version: 1.4.2
+Version: 1.4.3
 Summary: Resemble API Client Library
 Home-page: https://github.com/resemble-ai/resemble-python
 Author: ResembleAI
 Author-email: team@resemble.ai
 Project-URL: Bug Tracker, https://github.com/resemble-ai/resemble-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resemble-1.4.2/setup.py` & `resemble-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="resemble",
-    version="1.4.2",
+    version="1.4.3",
     packages=["resemble"],
     install_requires=["requests>2,<3"],
     python_requires=">=3.6",
     author="ResembleAI",
     author_email="team@resemble.ai",
     description="Resemble API Client Library",
     long_description=long_description,
```

### Comparing `resemble-1.4.2/tests/test_v2.py` & `resemble-1.4.3/tests/test_v2.py`

 * *Files identical despite different names*

