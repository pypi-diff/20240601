# Comparing `tmp/omnijp-2.4.0.tar.gz` & `tmp/omnijp-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnijp-2.4.0.tar", last modified: Sun May 26 04:19:00 2024, max compression
+gzip compressed data, was "omnijp-2.5.0.tar", last modified: Sat Jun  1 06:19:48 2024, max compression
```

## Comparing `omnijp-2.4.0.tar` & `omnijp-2.5.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.562815 omnijp-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-26 04:18:47.000000 omnijp-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-26 04:19:00.562815 omnijp-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-26 04:18:47.000000 omnijp-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.558815 omnijp-2.4.0/calc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:18:47.000000 omnijp-2.4.0/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-26 04:18:47.000000 omnijp-2.4.0/calc/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.558815 omnijp-2.4.0/dbdisk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.558815 omnijp-2.4.0/dbdisk/caches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/caches/db_disk_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/caches/db_disk_cache_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.558815 omnijp-2.4.0/dbdisk/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/database/database_pg_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/database/database_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/database/database_sybase_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/db_disk_cache_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/db_disk_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/db_disk_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 04:18:47.000000 omnijp-2.4.0/dbdisk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.558815 omnijp-2.4.0/omnijp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-26 04:19:00.000000 omnijp-2.4.0/omnijp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 04:19:00.000000 omnijp-2.4.0/omnijp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 04:19:00.000000 omnijp-2.4.0/omnijp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 04:19:00.000000 omnijp-2.4.0/omnijp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 04:19:00.000000 omnijp-2.4.0/omnijp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-26 04:19:00.000000 omnijp-2.4.0/omnijp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.562815 omnijp-2.4.0/restq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:18:47.000000 omnijp-2.4.0/restq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-26 04:18:47.000000 omnijp-2.4.0/restq/disk_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-26 04:18:47.000000 omnijp-2.4.0/restq/http_cached_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-26 04:18:47.000000 omnijp-2.4.0/restq/http_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 04:19:00.562815 omnijp-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-26 04:18:47.000000 omnijp-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.562815 omnijp-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:18:47.000000 omnijp-2.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-26 04:18:47.000000 omnijp-2.4.0/tests/test_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:00.562815 omnijp-2.4.0/xmlcreator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:18:47.000000 omnijp-2.4.0/xmlcreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-26 04:18:47.000000 omnijp-2.4.0/xmlcreator/xml_creator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.226325 omnijp-2.5.0/
+-rw-rw-rw-   0        0        0     1085 2024-02-10 04:50:11.000000 omnijp-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0      164 2024-06-01 06:19:48.225324 omnijp-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4484 2024-06-01 06:08:26.000000 omnijp-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.190325 omnijp-2.5.0/omnijp.egg-info/
+-rw-rw-rw-   0        0        0      164 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      922 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 06:19:48.226325 omnijp-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      416 2024-06-01 06:18:55.000000 omnijp-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.191348 omnijp-2.5.0/src/
+-rw-rw-rw-   0        0        0        0 2024-05-26 06:34:17.000000 omnijp-2.5.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.194353 omnijp-2.5.0/src/calc/
+-rw-rw-rw-   0        0        0        0 2024-02-10 04:33:16.000000 omnijp-2.5.0/src/calc/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-02-10 04:34:06.000000 omnijp-2.5.0/src/calc/calculator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.196325 omnijp-2.5.0/src/common/
+-rw-rw-rw-   0        0        0        0 2024-05-26 06:36:25.000000 omnijp-2.5.0/src/common/__init__.py
+-rw-rw-rw-   0        0        0      556 2024-05-26 06:49:00.000000 omnijp-2.5.0/src/common/helper.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.203349 omnijp-2.5.0/src/dbdisk/
+-rw-rw-rw-   0        0        0        0 2024-02-12 05:18:51.000000 omnijp-2.5.0/src/dbdisk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.207353 omnijp-2.5.0/src/dbdisk/caches/
+-rw-rw-rw-   0        0        0        0 2024-05-26 02:12:09.000000 omnijp-2.5.0/src/dbdisk/caches/__init__.py
+-rw-rw-rw-   0        0        0      369 2024-05-26 02:11:42.000000 omnijp-2.5.0/src/dbdisk/caches/db_disk_cache.py
+-rw-rw-rw-   0        0        0     1667 2024-05-26 06:37:55.000000 omnijp-2.5.0/src/dbdisk/caches/db_disk_cache_csv.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.212323 omnijp-2.5.0/src/dbdisk/database/
+-rw-rw-rw-   0        0        0        0 2024-05-25 16:32:55.000000 omnijp-2.5.0/src/dbdisk/database/__init__.py
+-rw-rw-rw-   0        0        0      381 2024-06-01 05:56:51.000000 omnijp-2.5.0/src/dbdisk/database/database_pg_service.py
+-rw-rw-rw-   0        0        0     1173 2024-06-01 05:55:24.000000 omnijp-2.5.0/src/dbdisk/database/database_service.py
+-rw-rw-rw-   0        0        0      383 2024-06-01 05:56:51.000000 omnijp-2.5.0/src/dbdisk/database/database_sybase_service.py
+-rw-rw-rw-   0        0        0     1817 2024-05-26 06:34:50.000000 omnijp-2.5.0/src/dbdisk/db_disk_cache_builder.py
+-rw-rw-rw-   0        0        0      617 2024-05-26 06:34:50.000000 omnijp-2.5.0/src/dbdisk/db_disk_factory.py
+-rw-rw-rw-   0        0        0      960 2024-05-26 06:34:50.000000 omnijp-2.5.0/src/dbdisk/db_disk_request.py
+-rw-rw-rw-   0        0        0      163 2024-05-26 03:14:27.000000 omnijp-2.5.0/src/dbdisk/types.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.218354 omnijp-2.5.0/src/restq/
+-rw-rw-rw-   0        0        0        0 2024-02-10 16:45:36.000000 omnijp-2.5.0/src/restq/__init__.py
+-rw-rw-rw-   0        0        0     2257 2024-02-12 03:37:07.000000 omnijp-2.5.0/src/restq/disk_cache.py
+-rw-rw-rw-   0        0        0      628 2024-05-26 06:34:50.000000 omnijp-2.5.0/src/restq/http_cached_request.py
+-rw-rw-rw-   0        0        0      850 2024-02-12 16:53:43.000000 omnijp-2.5.0/src/restq/http_request.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.221324 omnijp-2.5.0/src/xmlcreator/
+-rw-rw-rw-   0        0        0        0 2024-02-13 11:26:40.000000 omnijp-2.5.0/src/xmlcreator/__init__.py
+-rw-rw-rw-   0        0        0      704 2024-02-13 11:33:31.000000 omnijp-2.5.0/src/xmlcreator/xml_creator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.224325 omnijp-2.5.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-10 04:34:25.000000 omnijp-2.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      595 2024-05-26 06:34:50.000000 omnijp-2.5.0/tests/test_calculator.py
```

### Comparing `omnijp-2.4.0/dbdisk/caches/db_disk_cache_csv.py` & `omnijp-2.5.0/src/dbdisk/caches/db_disk_cache_csv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import os
-import csv
-from dbdisk.caches.db_disk_cache import DbDiskCache
-from dbdisk.helper import split_into_subsets, zip_directory
-
-
-class DbDiskCacheCsv(DbDiskCache):
-    def save(self, header, data):
-        try:
-            local_cache_dir = self.get_local_cache_path()
-            os.makedirs(local_cache_dir, exist_ok=True)
-            subsets = split_into_subsets(data, self.rows_per_file)
-            count = 1
-            total = 0
-            for subset in subsets:
-                file_path = os.path.join(local_cache_dir, f"{self.cache_name}_{count}.csv")
-                self.save_file(header, subset, file_path)
-                count += 1
-                total += len(subset)
-            print(f"Total records saved: {total}")
-            if self.can_zip:
-                zip_directory(local_cache_dir,local_cache_dir)
-        except Exception as e:
-            print(f"Error saving cache: {e}")
-            return False
-        print(f"Cache saved to {file_path}")
-        return True
-    def get_local_cache_path(self):
-        return os.path.join(self.cache_dir, self.cache_name) if self.can_zip else self.cache_dir
-    @staticmethod
-    def save_file(header, data, file_path):
-        try:
-            with open(file_path, 'w', newline='') as csv_file:
-                csv_writer = csv.writer(csv_file)
-                csv_writer.writerow(header)
-                for row in data:
-                    csv_writer.writerow(row)
-        except Exception as e:
-            print(f"Error saving cache: {e}")
-            return False
-        print(f"Cache saved to {file_path}")
-        return True
-
-
-
+import os
+import csv
+from src.dbdisk.caches.db_disk_cache import DbDiskCache
+from src.common.helper import split_into_subsets, zip_directory
+
+
+class DbDiskCacheCsv(DbDiskCache):
+    def save(self, header, data):
+        try:
+            local_cache_dir = self.get_local_cache_path()
+            os.makedirs(local_cache_dir, exist_ok=True)
+            subsets = split_into_subsets(data, self.rows_per_file)
+            count = 1
+            total = 0
+            for subset in subsets:
+                file_path = os.path.join(local_cache_dir, f"{self.cache_name}_{count}.csv")
+                self.save_file(header, subset, file_path)
+                count += 1
+                total += len(subset)
+            print(f"Total records saved: {total}")
+            if self.can_zip:
+                zip_directory(local_cache_dir,local_cache_dir)
+        except Exception as e:
+            print(f"Error saving cache: {e}")
+            return False
+        print(f"Cache saved to {file_path}")
+        return True
+    def get_local_cache_path(self):
+        return os.path.join(self.cache_dir, self.cache_name) if self.can_zip else self.cache_dir
+    @staticmethod
+    def save_file(header, data, file_path):
+        try:
+            with open(file_path, 'w', newline='') as csv_file:
+                csv_writer = csv.writer(csv_file)
+                csv_writer.writerow(header)
+                for row in data:
+                    csv_writer.writerow(row)
+        except Exception as e:
+            print(f"Error saving cache: {e}")
+            return False
+        print(f"Cache saved to {file_path}")
+        return True
+
+
+
```

### Comparing `omnijp-2.4.0/dbdisk/db_disk_cache_builder.py` & `omnijp-2.5.0/src/dbdisk/db_disk_cache_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from dbdisk.db_disk_request import DbDiskRequest
-from dbdisk.types import DbType, DiskFileType
-
-MAX_ROWS = 1000000
-class DbDiskCacheBuilder:
-    def __init__(self):
-        self.db_type = DbType.NONE
-        self.disk_file_type = DiskFileType.CSV
-        self.cache_path = None
-        self.cache_name = None
-        self.connection_string = None
-        self.can_zip = False
-        self.rows_per_file = MAX_ROWS
-
-
-    @classmethod
-    def create(cls, setup):
-        builder = cls()
-        setup(builder)
-        return builder
-
-    def set_db_type(self, db_type: DbType):
-        self.db_type = db_type
-        return self
-    def set_disk_file_type(self, disk_file_type: DiskFileType):
-        self.disk_file_type = disk_file_type
-        return self
-    def set_cache_path(self, path):
-        self.cache_path = path
-        return self
-
-    def set_cache_name(self, name):
-        self.cache_name = name
-        return self
-
-    def set_connection_string(self, connection_string):
-        self.connection_string = connection_string
-        return self
-
-    def set_can_zip(self, can_zip):
-        self.can_zip = can_zip
-        return self
-
-    def set_rows_per_file(self, rows_per_file):
-        self.rows_per_file = rows_per_file
-        return self
-
-    def execute(self, query):
-        print(f"Executing query: {query}")
-        print(f"Using cache path: {self.cache_path}")
-        print(f"Cache name: {self.cache_name}")
-        print(f"Connection string: {self.connection_string}")
-        print(f"Database type: {self.db_type}")
-        return DbDiskRequest(self.connection_string, self.cache_path, self.cache_name,self.disk_file_type, self.can_zip, self.rows_per_file).execute(query)
-        # Add actual database execution logic here
-
+from src.dbdisk.db_disk_request import DbDiskRequest
+from src.dbdisk.types import DbType, DiskFileType
+
+MAX_ROWS = 1000000
+class DbDiskCacheBuilder:
+    def __init__(self):
+        self.db_type = DbType.NONE
+        self.disk_file_type = DiskFileType.CSV
+        self.cache_path = None
+        self.cache_name = None
+        self.connection_string = None
+        self.can_zip = False
+        self.rows_per_file = MAX_ROWS
+
+
+    @classmethod
+    def create(cls, setup):
+        builder = cls()
+        setup(builder)
+        return builder
+
+    def set_db_type(self, db_type: DbType):
+        self.db_type = db_type
+        return self
+    def set_disk_file_type(self, disk_file_type: DiskFileType):
+        self.disk_file_type = disk_file_type
+        return self
+    def set_cache_path(self, path):
+        self.cache_path = path
+        return self
+
+    def set_cache_name(self, name):
+        self.cache_name = name
+        return self
+
+    def set_connection_string(self, connection_string):
+        self.connection_string = connection_string
+        return self
+
+    def set_can_zip(self, can_zip):
+        self.can_zip = can_zip
+        return self
+
+    def set_rows_per_file(self, rows_per_file):
+        self.rows_per_file = rows_per_file
+        return self
+
+    def execute(self, query):
+        print(f"Executing query: {query}")
+        print(f"Using cache path: {self.cache_path}")
+        print(f"Cache name: {self.cache_name}")
+        print(f"Connection string: {self.connection_string}")
+        print(f"Database type: {self.db_type}")
+        return DbDiskRequest(self.connection_string, self.cache_path, self.cache_name,self.disk_file_type, self.can_zip, self.rows_per_file).execute(query)
+        # Add actual database execution logic here
+
```

### Comparing `omnijp-2.4.0/dbdisk/db_disk_factory.py` & `omnijp-2.5.0/src/dbdisk/db_disk_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from dbdisk.caches.db_disk_cache_csv import DbDiskCacheCsv
-from dbdisk.types import DiskFileType
-
-
-class DbDiskFactory:
-    @staticmethod
-    def create_db_disk(disk_file_type, cache_dir, cache_name, can_zip=False, rows_per_file=1000000):
-        match disk_file_type:
-            case DiskFileType.CSV:
-                return DbDiskCacheCsv(cache_dir, cache_name,can_zip, rows_per_file)
-            case DiskFileType.JSON:
-                raise NotImplementedError
-            case DiskFileType.XML:
-                raise NotImplementedError
-            case _:
-                return None
-
+from src.dbdisk.caches.db_disk_cache_csv import DbDiskCacheCsv
+from src.dbdisk.types import DiskFileType
+
+
+class DbDiskFactory:
+    @staticmethod
+    def create_db_disk(disk_file_type, cache_dir, cache_name, can_zip=False, rows_per_file=1000000):
+        match disk_file_type:
+            case DiskFileType.CSV:
+                return DbDiskCacheCsv(cache_dir, cache_name,can_zip, rows_per_file)
+            case DiskFileType.JSON:
+                raise NotImplementedError
+            case DiskFileType.XML:
+                raise NotImplementedError
+            case _:
+                return None
+
```

### Comparing `omnijp-2.4.0/restq/disk_cache.py` & `omnijp-2.5.0/src/restq/disk_cache.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import os
-import pickle
-from datetime import timedelta, datetime
-
-
-class DiskCache:
-    FILE_PREFIX = "restq_"
-
-    def __init__(self, cache_dir, expires=timedelta(days=5)):
-        self.cache_dir = cache_dir
-        self.expires = expires
-
-    def save(self, result, cache_name):
-        """Saves the result to a file in the cache directory.
-        The file name is prefixed with 'restq_' and the cache
-        name. """
-        try:
-            self.clear(cache_name)
-            path = self.cache_path(cache_name)
-            folder = os.path.dirname(path)
-            if not os.path.exists(folder):
-                os.makedirs(folder)
-            with open(path, 'wb') as fp:
-                pickle.dump(result, fp)
-        except Exception as e:
-            print(f"Error saving cache: {e}")
-
-    def load(self, cache_name):
-        """ Loads the result from a file in the cache directory."""
-        try:
-            path = self.cache_path(cache_name)
-            with open(path, 'rb') as fp:
-                return pickle.load(fp)
-        except Exception as e:
-            print(f"Error loading cache: {e}")
-            return None
-
-    def clear(self, cache_name):
-        """Clears the cache for the given cache name."""
-        try:
-            for file in os.listdir(self.cache_dir):
-                if file.startswith(f"{self.FILE_PREFIX}{cache_name}"):
-                    file_path = os.path.join(self.cache_dir, file)
-                    creation_time = datetime.fromtimestamp(os.path.getmtime(file_path))
-                    if self.has_expired(creation_time):
-                        os.remove(file_path)
-        except Exception as e:
-            print(f"Error clearing cache: {e}")
-
-    def has_expired(self, timestamp):
-        """Returns True if the cache has expired."""
-        result_datetime = timestamp + self.expires
-        return datetime.utcnow() > result_datetime
-
-    def cache_path(self, cache_name, date=datetime.now()):
-        """Returns the cache path for the given cache name."""
-        formatted_date = date.strftime("%d-%m-%Y")
-        filename = f"{self.FILE_PREFIX}{cache_name}_{formatted_date}.json"
+import os
+import pickle
+from datetime import timedelta, datetime
+
+
+class DiskCache:
+    FILE_PREFIX = "restq_"
+
+    def __init__(self, cache_dir, expires=timedelta(days=5)):
+        self.cache_dir = cache_dir
+        self.expires = expires
+
+    def save(self, result, cache_name):
+        """Saves the result to a file in the cache directory.
+        The file name is prefixed with 'restq_' and the cache
+        name. """
+        try:
+            self.clear(cache_name)
+            path = self.cache_path(cache_name)
+            folder = os.path.dirname(path)
+            if not os.path.exists(folder):
+                os.makedirs(folder)
+            with open(path, 'wb') as fp:
+                pickle.dump(result, fp)
+        except Exception as e:
+            print(f"Error saving cache: {e}")
+
+    def load(self, cache_name):
+        """ Loads the result from a file in the cache directory."""
+        try:
+            path = self.cache_path(cache_name)
+            with open(path, 'rb') as fp:
+                return pickle.load(fp)
+        except Exception as e:
+            print(f"Error loading cache: {e}")
+            return None
+
+    def clear(self, cache_name):
+        """Clears the cache for the given cache name."""
+        try:
+            for file in os.listdir(self.cache_dir):
+                if file.startswith(f"{self.FILE_PREFIX}{cache_name}"):
+                    file_path = os.path.join(self.cache_dir, file)
+                    creation_time = datetime.fromtimestamp(os.path.getmtime(file_path))
+                    if self.has_expired(creation_time):
+                        os.remove(file_path)
+        except Exception as e:
+            print(f"Error clearing cache: {e}")
+
+    def has_expired(self, timestamp):
+        """Returns True if the cache has expired."""
+        result_datetime = timestamp + self.expires
+        return datetime.utcnow() > result_datetime
+
+    def cache_path(self, cache_name, date=datetime.now()):
+        """Returns the cache path for the given cache name."""
+        formatted_date = date.strftime("%d-%m-%Y")
+        filename = f"{self.FILE_PREFIX}{cache_name}_{formatted_date}.json"
         return os.path.join(self.cache_dir, filename)
```

### Comparing `omnijp-2.4.0/restq/http_cached_request.py` & `omnijp-2.5.0/src/restq/http_cached_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from restq.http_request import HttpRequest
-from restq.disk_cache import DiskCache
-
-
-class HttpCachedRequest(HttpRequest):
-    def __init__(self):
-        self.cache = None
-        super().__init__()
-
-    def set_cache(self, cache_dir):
-        self.cache = DiskCache(cache_dir)
-        return self
-
-    def build(self):
-        return self
-
-    def request_get(self, url, cache_name):
-        result = super().request_get(url)
-        if result.status_code == 200:
-            self.cache.save(result.content, cache_name)
-            return result.content
-        return self.cache.load(cache_name)
+from src.restq.http_request import HttpRequest
+from src.restq.disk_cache import DiskCache
+
+
+class HttpCachedRequest(HttpRequest):
+    def __init__(self):
+        self.cache = None
+        super().__init__()
+
+    def set_cache(self, cache_dir):
+        self.cache = DiskCache(cache_dir)
+        return self
+
+    def build(self):
+        return self
+
+    def request_get(self, url, cache_name):
+        result = super().request_get(url)
+        if result.status_code == 200:
+            self.cache.save(result.content, cache_name)
+            return result.content
+        return self.cache.load(cache_name)
```

