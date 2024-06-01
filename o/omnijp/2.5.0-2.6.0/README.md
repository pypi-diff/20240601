# Comparing `tmp/omnijp-2.5.0.tar.gz` & `tmp/omnijp-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnijp-2.5.0.tar", last modified: Sat Jun  1 06:19:48 2024, max compression
+gzip compressed data, was "omnijp-2.6.0.tar", last modified: Sat Jun  1 06:29:38 2024, max compression
```

## Comparing `omnijp-2.5.0.tar` & `omnijp-2.6.0.tar`

### file list

```diff
@@ -1,47 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.226325 omnijp-2.5.0/
--rw-rw-rw-   0        0        0     1085 2024-02-10 04:50:11.000000 omnijp-2.5.0/LICENSE
--rw-rw-rw-   0        0        0      164 2024-06-01 06:19:48.225324 omnijp-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4484 2024-06-01 06:08:26.000000 omnijp-2.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.190325 omnijp-2.5.0/omnijp.egg-info/
--rw-rw-rw-   0        0        0      164 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      922 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 06:19:48.000000 omnijp-2.5.0/omnijp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 06:19:48.226325 omnijp-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0      416 2024-06-01 06:18:55.000000 omnijp-2.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.191348 omnijp-2.5.0/src/
--rw-rw-rw-   0        0        0        0 2024-05-26 06:34:17.000000 omnijp-2.5.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.194353 omnijp-2.5.0/src/calc/
--rw-rw-rw-   0        0        0        0 2024-02-10 04:33:16.000000 omnijp-2.5.0/src/calc/__init__.py
--rw-rw-rw-   0        0        0      324 2024-02-10 04:34:06.000000 omnijp-2.5.0/src/calc/calculator.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.196325 omnijp-2.5.0/src/common/
--rw-rw-rw-   0        0        0        0 2024-05-26 06:36:25.000000 omnijp-2.5.0/src/common/__init__.py
--rw-rw-rw-   0        0        0      556 2024-05-26 06:49:00.000000 omnijp-2.5.0/src/common/helper.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.203349 omnijp-2.5.0/src/dbdisk/
--rw-rw-rw-   0        0        0        0 2024-02-12 05:18:51.000000 omnijp-2.5.0/src/dbdisk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.207353 omnijp-2.5.0/src/dbdisk/caches/
--rw-rw-rw-   0        0        0        0 2024-05-26 02:12:09.000000 omnijp-2.5.0/src/dbdisk/caches/__init__.py
--rw-rw-rw-   0        0        0      369 2024-05-26 02:11:42.000000 omnijp-2.5.0/src/dbdisk/caches/db_disk_cache.py
--rw-rw-rw-   0        0        0     1667 2024-05-26 06:37:55.000000 omnijp-2.5.0/src/dbdisk/caches/db_disk_cache_csv.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.212323 omnijp-2.5.0/src/dbdisk/database/
--rw-rw-rw-   0        0        0        0 2024-05-25 16:32:55.000000 omnijp-2.5.0/src/dbdisk/database/__init__.py
--rw-rw-rw-   0        0        0      381 2024-06-01 05:56:51.000000 omnijp-2.5.0/src/dbdisk/database/database_pg_service.py
--rw-rw-rw-   0        0        0     1173 2024-06-01 05:55:24.000000 omnijp-2.5.0/src/dbdisk/database/database_service.py
--rw-rw-rw-   0        0        0      383 2024-06-01 05:56:51.000000 omnijp-2.5.0/src/dbdisk/database/database_sybase_service.py
--rw-rw-rw-   0        0        0     1817 2024-05-26 06:34:50.000000 omnijp-2.5.0/src/dbdisk/db_disk_cache_builder.py
--rw-rw-rw-   0        0        0      617 2024-05-26 06:34:50.000000 omnijp-2.5.0/src/dbdisk/db_disk_factory.py
--rw-rw-rw-   0        0        0      960 2024-05-26 06:34:50.000000 omnijp-2.5.0/src/dbdisk/db_disk_request.py
--rw-rw-rw-   0        0        0      163 2024-05-26 03:14:27.000000 omnijp-2.5.0/src/dbdisk/types.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.218354 omnijp-2.5.0/src/restq/
--rw-rw-rw-   0        0        0        0 2024-02-10 16:45:36.000000 omnijp-2.5.0/src/restq/__init__.py
--rw-rw-rw-   0        0        0     2257 2024-02-12 03:37:07.000000 omnijp-2.5.0/src/restq/disk_cache.py
--rw-rw-rw-   0        0        0      628 2024-05-26 06:34:50.000000 omnijp-2.5.0/src/restq/http_cached_request.py
--rw-rw-rw-   0        0        0      850 2024-02-12 16:53:43.000000 omnijp-2.5.0/src/restq/http_request.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.221324 omnijp-2.5.0/src/xmlcreator/
--rw-rw-rw-   0        0        0        0 2024-02-13 11:26:40.000000 omnijp-2.5.0/src/xmlcreator/__init__.py
--rw-rw-rw-   0        0        0      704 2024-02-13 11:33:31.000000 omnijp-2.5.0/src/xmlcreator/xml_creator.py
-drwxrwxrwx   0        0        0        0 2024-06-01 06:19:48.224325 omnijp-2.5.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-10 04:34:25.000000 omnijp-2.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0      595 2024-05-26 06:34:50.000000 omnijp-2.5.0/tests/test_calculator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.413047 omnijp-2.6.0/
+-rw-rw-rw-   0        0        0     1085 2024-02-10 04:50:11.000000 omnijp-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0     5425 2024-06-01 06:29:38.412070 omnijp-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4485 2024-06-01 06:24:15.000000 omnijp-2.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.370128 omnijp-2.6.0/omnijp.egg-info/
+-rw-rw-rw-   0        0        0     5425 2024-06-01 06:29:38.000000 omnijp-2.6.0/omnijp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2024-06-01 06:29:38.000000 omnijp-2.6.0/omnijp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 06:29:38.000000 omnijp-2.6.0/omnijp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-06-01 06:29:38.000000 omnijp-2.6.0/omnijp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2024-06-01 06:29:38.000000 omnijp-2.6.0/omnijp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 06:29:38.000000 omnijp-2.6.0/omnijp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 06:29:38.413047 omnijp-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1263 2024-06-01 06:29:29.000000 omnijp-2.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.371046 omnijp-2.6.0/src/
+-rw-rw-rw-   0        0        0        0 2024-05-26 06:34:17.000000 omnijp-2.6.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.374072 omnijp-2.6.0/src/calc/
+-rw-rw-rw-   0        0        0        0 2024-02-10 04:33:16.000000 omnijp-2.6.0/src/calc/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-02-10 04:34:06.000000 omnijp-2.6.0/src/calc/calculator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.377045 omnijp-2.6.0/src/common/
+-rw-rw-rw-   0        0        0        0 2024-05-26 06:36:25.000000 omnijp-2.6.0/src/common/__init__.py
+-rw-rw-rw-   0        0        0      556 2024-05-26 06:49:00.000000 omnijp-2.6.0/src/common/helper.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.384046 omnijp-2.6.0/src/dbdisk/
+-rw-rw-rw-   0        0        0        0 2024-02-12 05:18:51.000000 omnijp-2.6.0/src/dbdisk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.388072 omnijp-2.6.0/src/dbdisk/caches/
+-rw-rw-rw-   0        0        0        0 2024-05-26 02:12:09.000000 omnijp-2.6.0/src/dbdisk/caches/__init__.py
+-rw-rw-rw-   0        0        0      369 2024-05-26 02:11:42.000000 omnijp-2.6.0/src/dbdisk/caches/db_disk_cache.py
+-rw-rw-rw-   0        0        0     1666 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/dbdisk/caches/db_disk_cache_csv.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.394046 omnijp-2.6.0/src/dbdisk/database/
+-rw-rw-rw-   0        0        0        0 2024-05-25 16:32:55.000000 omnijp-2.6.0/src/dbdisk/database/__init__.py
+-rw-rw-rw-   0        0        0      385 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/dbdisk/database/database_pg_service.py
+-rw-rw-rw-   0        0        0     1173 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/dbdisk/database/database_service.py
+-rw-rw-rw-   0        0        0      387 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/dbdisk/database/database_sybase_service.py
+-rw-rw-rw-   0        0        0     1852 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/dbdisk/db_disk_cache_builder.py
+-rw-rw-rw-   0        0        0      616 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/dbdisk/db_disk_factory.py
+-rw-rw-rw-   0        0        0     1005 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/dbdisk/db_disk_request.py
+-rw-rw-rw-   0        0        0      165 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/dbdisk/types.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.400069 omnijp-2.6.0/src/openai/
+-rw-rw-rw-   0        0        0        0 2024-06-01 06:23:45.000000 omnijp-2.6.0/src/openai/__init__.py
+-rw-rw-rw-   0        0        0      765 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/openai/async_openai_bot.py
+-rw-rw-rw-   0        0        0      685 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/openai/openai_bot.py
+-rw-rw-rw-   0        0        0     1010 2024-06-01 06:26:24.000000 omnijp-2.6.0/src/openai/openai_bot_base.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.405047 omnijp-2.6.0/src/restq/
+-rw-rw-rw-   0        0        0        0 2024-02-10 16:45:36.000000 omnijp-2.6.0/src/restq/__init__.py
+-rw-rw-rw-   0        0        0     2257 2024-02-12 03:37:07.000000 omnijp-2.6.0/src/restq/disk_cache.py
+-rw-rw-rw-   0        0        0      628 2024-05-26 06:34:50.000000 omnijp-2.6.0/src/restq/http_cached_request.py
+-rw-rw-rw-   0        0        0      850 2024-02-12 16:53:43.000000 omnijp-2.6.0/src/restq/http_request.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.408046 omnijp-2.6.0/src/xmlcreator/
+-rw-rw-rw-   0        0        0        0 2024-02-13 11:26:40.000000 omnijp-2.6.0/src/xmlcreator/__init__.py
+-rw-rw-rw-   0        0        0      704 2024-02-13 11:33:31.000000 omnijp-2.6.0/src/xmlcreator/xml_creator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:29:38.411047 omnijp-2.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-10 04:34:25.000000 omnijp-2.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      595 2024-05-26 06:34:50.000000 omnijp-2.6.0/tests/test_calculator.py
```

### Comparing `omnijp-2.5.0/LICENSE` & `omnijp-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omnijp-2.5.0/README.md` & `omnijp-2.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,20 +51,24 @@
 ```
 ### AsyncOpenAIBot
 And here's an example of how to use the `AsyncOpenAIBot` 
 To use the AsyncOpenAIBot class, you need to provide a valid OpenAI API key when creating an instance of the class. 
 This key is used to authenticate your requests to the OpenAI API.  
 
 Here's a basic example of how to use the AsyncOpenAIBot class:
+
 ```python
 import os
-from src.openaibot.openai_bot import OpenAIBot
+from src.openai.openai_bot import OpenAIBot
+
+
 def my_callback(response):
     print("Received response:", response)
 
+
 def run_bot_async():
     import asyncio
     openai_key = os.getenv("OPENAI_API_KEY")
     if openai_key is None:
         print("Please set OPENAI_API_KEY environment variable")
         exit(1)
```

### Comparing `omnijp-2.5.0/omnijp.egg-info/SOURCES.txt` & `omnijp-2.6.0/omnijp.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 src/dbdisk/caches/__init__.py
 src/dbdisk/caches/db_disk_cache.py
 src/dbdisk/caches/db_disk_cache_csv.py
 src/dbdisk/database/__init__.py
 src/dbdisk/database/database_pg_service.py
 src/dbdisk/database/database_service.py
 src/dbdisk/database/database_sybase_service.py
+src/openai/__init__.py
+src/openai/async_openai_bot.py
+src/openai/openai_bot.py
+src/openai/openai_bot_base.py
 src/restq/__init__.py
 src/restq/disk_cache.py
 src/restq/http_cached_request.py
 src/restq/http_request.py
 src/xmlcreator/__init__.py
 src/xmlcreator/xml_creator.py
 tests/__init__.py
```

### Comparing `omnijp-2.5.0/src/common/helper.py` & `omnijp-2.6.0/src/common/helper.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.5.0/src/dbdisk/caches/db_disk_cache_csv.py` & `omnijp-2.6.0/src/dbdisk/caches/db_disk_cache_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,31 +15,30 @@
             for subset in subsets:
                 file_path = os.path.join(local_cache_dir, f"{self.cache_name}_{count}.csv")
                 self.save_file(header, subset, file_path)
                 count += 1
                 total += len(subset)
             print(f"Total records saved: {total}")
             if self.can_zip:
-                zip_directory(local_cache_dir,local_cache_dir)
+                zip_directory(local_cache_dir, local_cache_dir)
         except Exception as e:
             print(f"Error saving cache: {e}")
             return False
         print(f"Cache saved to {file_path}")
         return True
+
     def get_local_cache_path(self):
         return os.path.join(self.cache_dir, self.cache_name) if self.can_zip else self.cache_dir
+
     @staticmethod
     def save_file(header, data, file_path):
         try:
             with open(file_path, 'w', newline='') as csv_file:
                 csv_writer = csv.writer(csv_file)
                 csv_writer.writerow(header)
                 for row in data:
                     csv_writer.writerow(row)
         except Exception as e:
             print(f"Error saving cache: {e}")
             return False
         print(f"Cache saved to {file_path}")
         return True
-
-
-
```

### Comparing `omnijp-2.5.0/src/dbdisk/database/database_service.py` & `omnijp-2.6.0/src/dbdisk/database/database_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import psycopg2
 import pymssql
 
 
 class DatabaseService:
 
     def __init__(self, connection_string):
-       self.connection_string = connection_string
+        self.connection_string = connection_string
 
     def execute(self, query):
         try:
             connection = self.connect()
             cursor = connection.cursor()
             cursor.execute(query)
             header = [desc[0] for desc in cursor.description]
@@ -30,13 +30,13 @@
     @abstractmethod
     def connect(self):
         pass
 
     @abstractmethod
     def handle_error(self, error):
         error_messages = {
-             psycopg2.Error: "Error connecting to PostgreSQL:",
-             pymssql.Error : "Error connecting to Sybase:"
+            psycopg2.Error: "Error connecting to PostgreSQL:",
+            pymssql.Error: "Error connecting to Sybase:"
         }
         error_type = type(error)
         message = error_messages.get(error_type, "Unknown error")
-        raise Exception(message, error)
+        raise Exception(message, error)
```

### Comparing `omnijp-2.5.0/src/dbdisk/db_disk_cache_builder.py` & `omnijp-2.6.0/src/dbdisk/db_disk_cache_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from src.dbdisk.db_disk_request import DbDiskRequest
 from src.dbdisk.types import DbType, DiskFileType
 
 MAX_ROWS = 1000000
+
+
 class DbDiskCacheBuilder:
     def __init__(self):
         self.db_type = DbType.NONE
         self.disk_file_type = DiskFileType.CSV
         self.cache_path = None
         self.cache_name = None
         self.connection_string = None
         self.can_zip = False
         self.rows_per_file = MAX_ROWS
 
-
     @classmethod
     def create(cls, setup):
         builder = cls()
         setup(builder)
         return builder
 
     def set_db_type(self, db_type: DbType):
         self.db_type = db_type
         return self
+
     def set_disk_file_type(self, disk_file_type: DiskFileType):
         self.disk_file_type = disk_file_type
         return self
+
     def set_cache_path(self, path):
         self.cache_path = path
         return self
 
     def set_cache_name(self, name):
         self.cache_name = name
         return self
@@ -47,10 +50,10 @@
 
     def execute(self, query):
         print(f"Executing query: {query}")
         print(f"Using cache path: {self.cache_path}")
         print(f"Cache name: {self.cache_name}")
         print(f"Connection string: {self.connection_string}")
         print(f"Database type: {self.db_type}")
-        return DbDiskRequest(self.connection_string, self.cache_path, self.cache_name,self.disk_file_type, self.can_zip, self.rows_per_file).execute(query)
+        return DbDiskRequest(self.connection_string, self.cache_path, self.cache_name, self.disk_file_type,
+                             self.can_zip, self.rows_per_file).execute(query)
         # Add actual database execution logic here
-
```

### Comparing `omnijp-2.5.0/src/dbdisk/db_disk_factory.py` & `omnijp-2.6.0/src/dbdisk/db_disk_factory.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 
 class DbDiskFactory:
     @staticmethod
     def create_db_disk(disk_file_type, cache_dir, cache_name, can_zip=False, rows_per_file=1000000):
         match disk_file_type:
             case DiskFileType.CSV:
-                return DbDiskCacheCsv(cache_dir, cache_name,can_zip, rows_per_file)
+                return DbDiskCacheCsv(cache_dir, cache_name, can_zip, rows_per_file)
             case DiskFileType.JSON:
                 raise NotImplementedError
             case DiskFileType.XML:
                 raise NotImplementedError
             case _:
                 return None
-
```

### Comparing `omnijp-2.5.0/src/dbdisk/db_disk_request.py` & `omnijp-2.6.0/src/dbdisk/db_disk_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,9 @@
         self.can_zip = can_zip
         self.rows_per_file = rows_per_file
 
     def execute(self, query):
         db_pg_service = DatabasePgService(self.connection_string)
         header, data = db_pg_service.execute(query)
         print(data)
-        return DbDiskFactory.create_db_disk(self.disk_file_type, self.cache_dir, self.cache_name, self.can_zip, self.rows_per_file).save(header, data)
+        return DbDiskFactory.create_db_disk(self.disk_file_type, self.cache_dir, self.cache_name, self.can_zip,
+                                            self.rows_per_file).save(header, data)
```

### Comparing `omnijp-2.5.0/src/restq/disk_cache.py` & `omnijp-2.6.0/src/restq/disk_cache.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.5.0/src/restq/http_cached_request.py` & `omnijp-2.6.0/src/restq/http_cached_request.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.5.0/src/restq/http_request.py` & `omnijp-2.6.0/src/restq/http_request.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.5.0/src/xmlcreator/xml_creator.py` & `omnijp-2.6.0/src/xmlcreator/xml_creator.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.5.0/tests/test_calculator.py` & `omnijp-2.6.0/tests/test_calculator.py`

 * *Files identical despite different names*

