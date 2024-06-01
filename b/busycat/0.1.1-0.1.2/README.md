# Comparing `tmp/busycat-0.1.1.tar.gz` & `tmp/busycat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busycat-0.1.1.tar", last modified: Thu May 30 05:11:31 2024, max compression
+gzip compressed data, was "busycat-0.1.2.tar", last modified: Sat Jun  1 03:15:59 2024, max compression
```

## Comparing `busycat-0.1.1.tar` & `busycat-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:11:31.752568 busycat-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 05:11:24.000000 busycat-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 05:11:31.752568 busycat-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 05:11:24.000000 busycat-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:11:31.748568 busycat-0.1.1/busycat/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 05:11:24.000000 busycat-0.1.1/busycat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-30 05:11:24.000000 busycat-0.1.1/busycat/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:11:31.752568 busycat-0.1.1/busycat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 05:11:31.000000 busycat-0.1.1/busycat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-30 05:11:31.000000 busycat-0.1.1/busycat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:11:31.000000 busycat-0.1.1/busycat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 05:11:31.000000 busycat-0.1.1/busycat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 05:11:31.000000 busycat-0.1.1/busycat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:11:31.752568 busycat-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-30 05:11:24.000000 busycat-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:15:59.143273 busycat-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-06-01 03:15:49.000000 busycat-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-06-01 03:15:59.143273 busycat-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 03:15:49.000000 busycat-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:15:59.143273 busycat-0.1.2/busycat/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 03:15:49.000000 busycat-0.1.2/busycat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-06-01 03:15:49.000000 busycat-0.1.2/busycat/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:15:59.143273 busycat-0.1.2/busycat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-06-01 03:15:59.000000 busycat-0.1.2/busycat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-01 03:15:59.000000 busycat-0.1.2/busycat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:15:59.000000 busycat-0.1.2/busycat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-01 03:15:59.000000 busycat-0.1.2/busycat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-01 03:15:59.000000 busycat-0.1.2/busycat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:15:59.143273 busycat-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-06-01 03:15:49.000000 busycat-0.1.2/setup.py
```

### Comparing `busycat-0.1.1/LICENSE` & `busycat-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `busycat-0.1.1/busycat/mysql.py` & `busycat-0.1.2/busycat/mysql.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,35 +48,43 @@
         data = [dict(zip(fields, row)) for row in results]
         json_data = json.dumps(data, default=str)
         return json_data
 
     def execute(self, sql: str, params: Union[Tuple, List[Tuple]] = None) -> Union[
         List[Dict[str, Any]], Dict[str, Any], bool]:
         self.ensure_connection()
-        try:
-            with self.db.cursor() as cursor:
-                if params:
-                    if isinstance(params, list):
-                        cursor.executemany(sql, params)
+        retries = 0
+        while retries < self.max_retries:
+            try:
+                with self.db.cursor() as cursor:
+                    if params:
+                        if isinstance(params, list):
+                            cursor.executemany(sql, params)
+                        else:
+                            cursor.execute(sql, params)
                     else:
-                        cursor.execute(sql, params)
-                else:
-                    cursor.execute(sql)
+                        cursor.execute(sql)
 
-                if sql.strip().lower().startswith("select"):
-                    results = cursor.fetchall()
-                    description = cursor.description
-                    return json.loads(self.trans_to_json(description, results))
+                    if sql.strip().lower().startswith("select"):
+                        results = cursor.fetchall()
+                        description = cursor.description
+                        return json.loads(self.trans_to_json(description, results))
+                    else:
+                        self.db.commit()
+                        return True
+            except pymysql.MySQLError as e:
+                print(f"SQL execution error: {e}")
+                if e.args[0] in (2006, 2013, 2014, 2018, 2027):  # Lost connection or server gone away
+                    print("Attempting to reconnect...")
+                    self.connect()
+                    retries += 1
                 else:
-                    self.db.commit()
-                    return True
-        except pymysql.MySQLError as e:
-            print(f"SQL execution error: {e}")
-            self.db.rollback()
-            return False
+                    self.db.rollback()
+                    return False
+        raise Exception("Maximum retry limit reached, failed to execute the query")
 
     def quit(self) -> None:
         try:
             self.cursor.close()
             self.db.close()
         except pymysql.MySQLError as e:
             print(f"Error closing connection: {e}")
```

### Comparing `busycat-0.1.1/setup.py` & `busycat-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="busycat",
-    version="0.1.1",
+    version="0.1.2",
     author="busycat",
     author_email="",
     description="selfmade pkg",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

