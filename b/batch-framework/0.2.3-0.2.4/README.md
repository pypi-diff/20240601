# Comparing `tmp/batch-framework-0.2.3.tar.gz` & `tmp/batch-framework-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch-framework-0.2.3.tar", last modified: Mon May 20 14:06:30 2024, max compression
+gzip compressed data, was "batch-framework-0.2.4.tar", last modified: Sat Jun  1 07:50:15 2024, max compression
```

## Comparing `batch-framework-0.2.3.tar` & `batch-framework-0.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:06:30.510883 batch-framework-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 14:05:42.000000 batch-framework-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-20 14:06:30.510883 batch-framework-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 14:05:42.000000 batch-framework-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:06:30.510883 batch-framework-0.2.3/batch_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:06:30.510883 batch-framework-0.2.3/batch_framework/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/filesystem/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:06:30.510883 batch-framework-0.2.3/batch_framework/filesystem/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/filesystem/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/filesystem/dropbox/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/filesystem/dropbox/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/filesystem/dropbox/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/filesystem/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/parallize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/rdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 14:05:42.000000 batch-framework-0.2.3/batch_framework/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:06:30.510883 batch-framework-0.2.3/batch_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-20 14:06:30.000000 batch-framework-0.2.3/batch_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-20 14:06:30.000000 batch-framework-0.2.3/batch_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:06:30.000000 batch-framework-0.2.3/batch_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-20 14:06:30.000000 batch-framework-0.2.3/batch_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 14:06:30.000000 batch-framework-0.2.3/batch_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:06:30.510883 batch-framework-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-20 14:05:42.000000 batch-framework-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-01 07:49:28.000000 batch-framework-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-01 07:50:15.642428 batch-framework-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 07:49:28.000000 batch-framework-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/batch_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/batch_framework/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/batch_framework/filesystem/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/dropbox/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/dropbox/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/dropbox/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/parallize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/rdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/batch_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 07:50:15.642428 batch-framework-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-01 07:49:28.000000 batch-framework-0.2.4/setup.py
```

### Comparing `batch-framework-0.2.3/LICENSE` & `batch-framework-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/PKG-INFO` & `batch-framework-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-framework
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generate Batch Framework
 Home-page: https://github.com/jeffrey82221/batch_framework
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `batch-framework-0.2.3/batch_framework/adaptor.py` & `batch-framework-0.2.4/batch_framework/adaptor.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/base.py` & `batch-framework-0.2.4/batch_framework/base.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/etl.py` & `batch-framework-0.2.4/batch_framework/etl.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/executor.py` & `batch-framework-0.2.4/batch_framework/executor.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/filesystem/base.py` & `batch-framework-0.2.4/batch_framework/filesystem/base.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/filesystem/dropbox/config.py` & `batch-framework-0.2.4/batch_framework/filesystem/dropbox/config.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/filesystem/dropbox/dropbox.py` & `batch-framework-0.2.4/batch_framework/filesystem/dropbox/dropbox.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,72 +3,51 @@
 from concurrent.futures import ThreadPoolExecutor
 from threading import Semaphore, Thread
 from split_file_reader.split_file_writer import SplitFileWriter
 from split_file_reader import SplitFileReader
 import base64
 import dropbox
 import requests
-from dropboxdrivefs import DropboxDriveFileSystem
+import dropboxdrivefs
 from fsspec.implementations.dirfs import DirFileSystem
 from ..base import FileSystem
 from .config import DropboxConfig
 from .util import Pipe
 
 __all__ = ['DropboxBackend']
 
 
-class MyDropboxFS(DropboxConfig, DropboxDriveFileSystem):
-    def connect(self):
+class MyDropboxFS(DropboxConfig, dropboxdrivefs.DropboxDriveFileSystem):
+    """
+    Dropbox FileSystem Object
+    """
+    def connect(self, **kwargs):
         """ connect to the dropbox account with the given token
         """
         self.dbx = dropbox.Dropbox(
             app_key=self.app_key,
             app_secret=self.app_secret,
             oauth2_refresh_token=self.refresh_token
         )
         self.token = self.refresh_token
         self.session = requests.Session()
         self.session.auth = ("Authorization", self.token)
 
-    def copy(self, path1, path2, recursive=True, **kwargs):
-        if isinstance(path1, list):
-            for file_path in path1:
-                assert not file_path.endswith(
-                    '/'), 'multiple file copy should takes files as input'
-                self.copy(file_path, path2)
-        else:
-            if path1.endswith('/') and path2.endswith('/'):
-                assert recursive, 'recursive should be True for folder copying'
-                if not self.exists(path2[:-1]):
-                    self.dbx.files_copy(path1[:-1], path2[:-1])
-                else:
-                    self.rm(path2[:-1], recursive=True)
-                    self.dbx.files_copy(path1[:-1], path2[:-1])
-            elif path2.endswith('/'):
-                self.dbx.files_copy(path1, path2 + path1.split('/')[-1])
-            else:
-                self.dbx.files_copy(path1, path2)
-
-    def cp_file(self, path1, path2, **kwargs):
-        assert not path1.endswith('/'), f'{path1} is not a file'
-        assert not path2.endswith('/'), f'{path2} is not a file'
-        self.dbx.files_copy(path1, path2)
-
 
 limit_pool = Semaphore(value=8)
 
 
 class DropboxBackend(FileSystem):
     """
     Storage object with IO interface left abstract
     """
 
     def __init__(self, directory='/', chunksize=2000000):
         assert directory.startswith('/')
-        root_fs = MyDropboxFS(token='')
+        root_fs = MyDropboxFS()
         super().__init__(DirFileSystem(directory, root_fs))
         self._chunksize = chunksize
 
     def upload_core(self, file_obj: io.BytesIO, remote_path: str):
         """Upload file object
 
         Args:
```

### Comparing `batch-framework-0.2.3/batch_framework/filesystem/dropbox/util.py` & `batch-framework-0.2.4/batch_framework/filesystem/dropbox/util.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/filesystem/local.py` & `batch-framework-0.2.4/batch_framework/filesystem/local.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/parallize.py` & `batch-framework-0.2.4/batch_framework/parallize.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/rdb.py` & `batch-framework-0.2.4/batch_framework/rdb.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework/storage.py` & `batch-framework-0.2.4/batch_framework/storage.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/batch_framework.egg-info/PKG-INFO` & `batch-framework-0.2.4/batch_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-framework
-Version: 0.2.3
+Version: 0.2.4
 Summary: Generate Batch Framework
 Home-page: https://github.com/jeffrey82221/batch_framework
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `batch-framework-0.2.3/batch_framework.egg-info/SOURCES.txt` & `batch-framework-0.2.4/batch_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.3/setup.py` & `batch-framework-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     install_requires=[
         'pandas',
         'dropbox',
         'pyarrow',
         'duckdb',
         'paradag',
         'dill',
-        'dropboxdrivefs',
+        'dropboxdrivefs==1.4.1',
         'typing_extensions',
         'vaex',
         'tqdm',
         'types-PyYAML',
         'PyYAML',
         'split-file-reader==0.1.4'
     ]
```

