# Comparing `tmp/bettermysql-0.0.1.tar.gz` & `tmp/bettermysql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettermysql-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bettermysql-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bettermysql-0.0.1.tar` & `bettermysql-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:45:03.695286 bettermysql-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1307 2024-05-20 20:29:14.048126 bettermysql-0.0.1/README.md
--rw-r--r--   0        0        0     3737 2024-06-01 12:33:26.302915 bettermysql-0.0.1/bettermysql/__init__.py
--rw-r--r--   0        0        0     1148 2024-06-01 12:09:10.800471 bettermysql-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2166 1970-01-01 00:00:00.000000 bettermysql-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:45:03.695286 bettermysql-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1307 2024-06-01 12:41:22.592932 bettermysql-0.0.2/README.md
+-rw-r--r--   0        0        0     3616 2024-06-01 12:44:51.554970 bettermysql-0.0.2/bettermysql/__init__.py
+-rw-r--r--   0        0        0     1138 2024-06-01 12:43:36.908376 bettermysql-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 bettermysql-0.0.2/PKG-INFO
```

### Comparing `bettermysql-0.0.1/LICENSE.txt` & `bettermysql-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bettermysql-0.0.1/README.md` & `bettermysql-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # **About**
 
-A simple and lightweight ORM that facilitate some operations on SQL Server using of pyodbc.
+A simple and lightweight ORM that facilitate some operations on MySQL using of pymysql.
 
 # How to use
 
 ## **Preparation**
 
 ```python
 # Single call it once to setup the inner settings
-BetterMSSQL.setup("name of the database", "db user", "db password", "host", 1234) #port
+BetterMYSQL.setup("name of the database", "db user", "db password", "host", 1234) #port
 
 # Creating a DB Model
 class Fruits():
   _table = "fruit_table_name"
 
 class People():
   _table = "people_table_name"
@@ -21,18 +21,18 @@
 ## **Select**
 
 ```python
 # Select the first fruit ordered by name and retrieve the first row
 Fruits().select("name").order("name").row()  # returns one row
 
 # Select all data from the top 15 fruits
-Fruits().select("*").top("15").run() # returns a row list
+Fruits().select("*").limit("15").run() # returns a row list
 
 # Select all data from the top 15 fruits
-Fruits().select("*").top("15").run() # returns a row list
+Fruits().select("*").limit("15").run() # returns a row list
 
 # Select the name of the first person with 34 years old
 People().select("name").where("age = ?").cell(34) # returns the first cell of the first row
 ```
 
 ## **Insert**
```

### Comparing `bettermysql-0.0.1/bettermysql/__init__.py` & `bettermysql-0.0.2/bettermysql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pymysql
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 class MYSQLSingleton(type):
   _instances = {}
 
   def __call__(cls, *args, **kwargs):
     if cls not in cls._instances:
       cls._instances[cls] = super(MYSQLSingleton, cls).__call__(*args, **kwargs)
@@ -116,19 +116,14 @@
 
   def where(self, s):
     if (s):
       self.__query += f"where {s} "
 
     return self
     
-  def top(self, count):
-    self.__query = self.__query.replace('select', f'select top({count})')
-
-    return self
-
   def order(self, s):
     self.__query += f"order by {s} "
 
     return self
 
   def group(self, s):
     self.__query += f"group by {s} "
```

### Comparing `bettermysql-0.0.1/pyproject.toml` & `bettermysql-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ['flit_core>=3.2,<4']
 build-backend = 'flit_core.buildapi'
 
 [project]
 name = "bettermysql"
 authors = [{name = "matgasp"}]
-description="A simple and lightweight ORM that facilitate some operations on SQL Server using of pyodbc."
-keywords = ["better", "s3", "better mysql", "bettermysql"]
+description="A simple and lightweight ORM that facilitate some operations on MySQL using of pymysql."
+keywords = ["better", "better mysql", "bettermysql"]
 dependencies = ["pymysql"]
 
 license = {file = "LICENSE.txt"}
 requires-python = ">= 3.9"
 dynamic = ['version']
 readme = "README.md"
 classifiers = [
```

### Comparing `bettermysql-0.0.1/PKG-INFO` & `bettermysql-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bettermysql
-Version: 0.0.1
-Summary: A simple and lightweight ORM that facilitate some operations on SQL Server using of pyodbc.
-Keywords: better,s3,better mysql,bettermysql
+Version: 0.0.2
+Summary: A simple and lightweight ORM that facilitate some operations on MySQL using of pymysql.
+Keywords: better,better mysql,bettermysql
 Author: matgasp
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,23 +18,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pymysql
 Project-URL: Issues, https://github.com/matgasp/bettermysql/issues
 Project-URL: Repository, https://github.com/matgasp/bettermysql
 
 # **About**
 
-A simple and lightweight ORM that facilitate some operations on SQL Server using of pyodbc.
+A simple and lightweight ORM that facilitate some operations on MySQL using of pymysql.
 
 # How to use
 
 ## **Preparation**
 
 ```python
 # Single call it once to setup the inner settings
-BetterMSSQL.setup("name of the database", "db user", "db password", "host", 1234) #port
+BetterMYSQL.setup("name of the database", "db user", "db password", "host", 1234) #port
 
 # Creating a DB Model
 class Fruits():
   _table = "fruit_table_name"
 
 class People():
   _table = "people_table_name"
@@ -43,18 +43,18 @@
 ## **Select**
 
 ```python
 # Select the first fruit ordered by name and retrieve the first row
 Fruits().select("name").order("name").row()  # returns one row
 
 # Select all data from the top 15 fruits
-Fruits().select("*").top("15").run() # returns a row list
+Fruits().select("*").limit("15").run() # returns a row list
 
 # Select all data from the top 15 fruits
-Fruits().select("*").top("15").run() # returns a row list
+Fruits().select("*").limit("15").run() # returns a row list
 
 # Select the name of the first person with 34 years old
 People().select("name").where("age = ?").cell(34) # returns the first cell of the first row
 ```
 
 ## **Insert**
```

