# Comparing `tmp/lb_database-1.1.6.tar.gz` & `tmp/lb_database-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lb_database-1.1.6.tar", last modified: Fri May 31 18:10:32 2024, max compression
+gzip compressed data, was "lb_database-1.1.7.tar", last modified: Fri May 31 21:07:37 2024, max compression
```

## Comparing `lb_database-1.1.6.tar` & `lb_database-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:10:32.148536 lb_database-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 18:10:32.148536 lb_database-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-31 18:10:24.000000 lb_database-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:10:32.144536 lb_database-1.1.6/enumDatabase/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-31 18:10:24.000000 lb_database-1.1.6/enumDatabase/EnumCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 18:10:24.000000 lb_database-1.1.6/enumDatabase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:10:32.144536 lb_database-1.1.6/lbConnection/
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbConnection/LbConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbConnection/Projection.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbConnection/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbConnection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:10:32.148536 lb_database-1.1.6/lbUser/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbUser/AddressLbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbUser/ConfirmationCodeLbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbUser/EnumStatusLbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbUser/LbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 18:10:24.000000 lb_database-1.1.6/lbUser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:10:32.148536 lb_database-1.1.6/lb_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 18:10:32.000000 lb_database-1.1.6/lb_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-31 18:10:32.000000 lb_database-1.1.6/lb_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:10:32.000000 lb_database-1.1.6/lb_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 18:10:32.000000 lb_database-1.1.6/lb_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:10:32.148536 lb_database-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 18:10:24.000000 lb_database-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:07:37.192016 lb_database-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 21:07:37.192016 lb_database-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-31 21:07:29.000000 lb_database-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:07:37.188016 lb_database-1.1.7/enumDatabase/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-31 21:07:29.000000 lb_database-1.1.7/enumDatabase/EnumCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 21:07:29.000000 lb_database-1.1.7/enumDatabase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:07:37.192016 lb_database-1.1.7/lbConnection/
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbConnection/LbConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbConnection/Projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbConnection/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbConnection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:07:37.192016 lb_database-1.1.7/lbUser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbUser/AddressLbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbUser/ConfirmationCodeLbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbUser/EnumStatusLbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbUser/LbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 21:07:29.000000 lb_database-1.1.7/lbUser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:07:37.192016 lb_database-1.1.7/lb_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 21:07:37.000000 lb_database-1.1.7/lb_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-31 21:07:37.000000 lb_database-1.1.7/lb_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:07:37.000000 lb_database-1.1.7/lb_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 21:07:37.000000 lb_database-1.1.7/lb_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 21:07:37.192016 lb_database-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 21:07:29.000000 lb_database-1.1.7/setup.py
```

### Comparing `lb_database-1.1.6/PKG-INFO` & `lb_database-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-database
-Version: 1.1.6
+Version: 1.1.7
 Summary: Library with data models by lb services
 Author: Lucas Barros
 Author-email: lucasbarros2000@hotmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lb_database-1.1.6/README.md` & `lb_database-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.6/lbConnection/LbConnection.py` & `lb_database-1.1.7/lbConnection/LbConnection.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,14 +110,27 @@
         :return: None
         """
 
         self.__lb_logger.info(f"Starting update one by query {query.query()}")
 
         self.__my_database[collection].update_one(query.query(), {"$set": update.query()})
 
+    def update_one_unset(self, query: Query, update: Query, collection: str) -> None:
+        """
+        Function for update one unset document by query
+        :param query: Query for update one document
+        :param update: Fields and values for update
+        :param collection: Collection for get data
+        :return: None
+        """
+
+        self.__lb_logger.info(f"Starting update one by query {query.query()}")
+
+        self.__my_database[collection].update_one(query.query(), {"$unset": update.query()})
+
     def update_many(self, query: Query, update: Query, collection: str) -> None:
         """
         Function for update many document by query
         :param query: Query for update many document
         :param update: Fields and values for update
         :param collection: Collection for get data
         :return: None
```

### Comparing `lb_database-1.1.6/lbUser/AddressLbUser.py` & `lb_database-1.1.7/lbUser/AddressLbUser.py`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.6/lbUser/ConfirmationCodeLbUser.py` & `lb_database-1.1.7/lbUser/ConfirmationCodeLbUser.py`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.6/lbUser/LbUser.py` & `lb_database-1.1.7/lbUser/LbUser.py`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.6/lb_database.egg-info/PKG-INFO` & `lb_database-1.1.7/lb_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-database
-Version: 1.1.6
+Version: 1.1.7
 Summary: Library with data models by lb services
 Author: Lucas Barros
 Author-email: lucasbarros2000@hotmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lb_database-1.1.6/setup.py` & `lb_database-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="lb-database",
-    version="1.1.6",
+    version="1.1.7",
     author="Lucas Barros",
     author_email="lucasbarros2000@hotmail.com",
     description="Library with data models by lb services",
     packages=setuptools.find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
```

