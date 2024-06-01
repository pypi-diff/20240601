# Comparing `tmp/pyjondb-1.5.tar.gz` & `tmp/pyjondb-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjondb-1.5.tar", last modified: Sat Jun  1 00:54:41 2024, max compression
+gzip compressed data, was "pyjondb-1.6.tar", last modified: Sat Jun  1 06:03:14 2024, max compression
```

## Comparing `pyjondb-1.5.tar` & `pyjondb-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 00:54:41.750812 pyjondb-1.5/
--rw-rw-rw-   0        0        0     2720 2024-06-01 00:54:41.749811 pyjondb-1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 00:54:41.747811 pyjondb-1.5/PyJONDB.egg-info/
--rw-rw-rw-   0        0        0     2720 2024-06-01 00:54:41.000000 pyjondb-1.5/PyJONDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-06-01 00:54:41.000000 pyjondb-1.5/PyJONDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 00:54:41.000000 pyjondb-1.5/PyJONDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 00:54:41.000000 pyjondb-1.5/PyJONDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-01 00:54:41.000000 pyjondb-1.5/PyJONDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 00:54:41.746807 pyjondb-1.5/pyjondb/
--rw-rw-rw-   0        0        0    15374 2024-06-01 00:07:16.000000 pyjondb-1.5/pyjondb/__init__.py
--rw-rw-rw-   0        0        0     1664 2024-06-01 00:32:59.000000 pyjondb-1.5/pypi.readme
--rw-rw-rw-   0        0        0       42 2024-06-01 00:54:41.750812 pyjondb-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1754 2024-06-01 00:54:35.000000 pyjondb-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:03:14.102083 pyjondb-1.6/
+-rw-rw-rw-   0        0        0     1085 2024-06-01 01:14:36.000000 pyjondb-1.6/LICENSE
+-rw-rw-rw-   0        0        0     2707 2024-06-01 06:03:14.100081 pyjondb-1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 06:03:14.099081 pyjondb-1.6/PyJONDB.egg-info/
+-rw-rw-rw-   0        0        0     2707 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3008 2024-06-01 06:00:21.000000 pyjondb-1.6/README.md
+-rw-rw-rw-   0        0        0     1628 2024-06-01 06:02:25.000000 pyjondb-1.6/pypi.readme
+-rw-rw-rw-   0        0        0       42 2024-06-01 06:03:14.102083 pyjondb-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1754 2024-06-01 06:01:33.000000 pyjondb-1.6/setup.py
```

### Comparing `pyjondb-1.5/PKG-INFO` & `pyjondb-1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.5
+Version: 1.6
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: cryptography
 
 # Encrypted JSON Database
 
 ## Overview
 This package provides a lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation. It uses the `cryptography` library for encryption and decryption of data, ensuring secure storage of your sensitive information.
 
@@ -27,35 +28,32 @@
 - **Documents**: Allows adding, finding, updating, and deleting documents within collections.
 - **Aggregation**: Provides basic aggregation functionality for querying documents.
 - **Linking Collections**: Supports linking between collections to create references.
 - **Tree Structure**: Allows creating tree structures by linking root documents to their child documents.
 
 ## Usage
 ```python
-import pyjondb
+from pyjondb import database
+from pyjondb import session
 
-# Initialize the database
-db = pyjondb.database('mydatabase', 'mysecretkey')
+auth = session.start()
+auth.create_user('admin', 'adminpass', roles=['admin', 'user'])
 
-# Create the database
-db.create()
+# Authenticate and get a session ID
+session_id = auth.authenticate('admin', 'adminpass')
 
-# Create a new collection
-db.create_collection('mycollection')
+# Create a database instance with the session ID
+db = database.init('my_database', 'my_secret_key', auth, debug=True)
 
-# Add a document to the collection
-document = {'name': 'John Doe', 'age': 30}
-db.add_document('mycollection', document)
+# Create a database
+db.create(session_id)
 
-# Find a document in the collection
-query = {'name': 'John Doe'}
-results = db.find_document('mycollection', query)
-print(results)
+# Create a collection
+db.create_collection('my_collection', session_id)
 
-# Update a document in the collection
-document_id = results[0]['_id']
-db.update_document('mycollection', document_id, {'age': 31})
+# Add a document
+db.add_document('my_collection', {'name': 'example'}, session_id)
 
-# Delete a document from the collection
-db.delete_document('mycollection', document_id)
+# Read the collection
+print(db.read_collection('my_collection', session_id))
 ```
 ### Learn more about it at the docs: https://github.com/t-a-g-o/PyJONDB/wiki
```

### Comparing `pyjondb-1.5/PyJONDB.egg-info/PKG-INFO` & `pyjondb-1.6/PyJONDB.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.5
+Version: 1.6
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: cryptography
 
 # Encrypted JSON Database
 
 ## Overview
 This package provides a lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation. It uses the `cryptography` library for encryption and decryption of data, ensuring secure storage of your sensitive information.
 
@@ -27,35 +28,32 @@
 - **Documents**: Allows adding, finding, updating, and deleting documents within collections.
 - **Aggregation**: Provides basic aggregation functionality for querying documents.
 - **Linking Collections**: Supports linking between collections to create references.
 - **Tree Structure**: Allows creating tree structures by linking root documents to their child documents.
 
 ## Usage
 ```python
-import pyjondb
+from pyjondb import database
+from pyjondb import session
 
-# Initialize the database
-db = pyjondb.database('mydatabase', 'mysecretkey')
+auth = session.start()
+auth.create_user('admin', 'adminpass', roles=['admin', 'user'])
 
-# Create the database
-db.create()
+# Authenticate and get a session ID
+session_id = auth.authenticate('admin', 'adminpass')
 
-# Create a new collection
-db.create_collection('mycollection')
+# Create a database instance with the session ID
+db = database.init('my_database', 'my_secret_key', auth, debug=True)
 
-# Add a document to the collection
-document = {'name': 'John Doe', 'age': 30}
-db.add_document('mycollection', document)
+# Create a database
+db.create(session_id)
 
-# Find a document in the collection
-query = {'name': 'John Doe'}
-results = db.find_document('mycollection', query)
-print(results)
+# Create a collection
+db.create_collection('my_collection', session_id)
 
-# Update a document in the collection
-document_id = results[0]['_id']
-db.update_document('mycollection', document_id, {'age': 31})
+# Add a document
+db.add_document('my_collection', {'name': 'example'}, session_id)
 
-# Delete a document from the collection
-db.delete_document('mycollection', document_id)
+# Read the collection
+print(db.read_collection('my_collection', session_id))
 ```
 ### Learn more about it at the docs: https://github.com/t-a-g-o/PyJONDB/wiki
```

### Comparing `pyjondb-1.5/setup.py` & `pyjondb-1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), 'pypi.readme'), encoding='utf-8') as f:
     desc = f.read()
 
 setup(
     name='PyJONDB',
-    version='1.5',
+    version='1.6',
     description='A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.',
     long_description=desc,
     long_description_content_type='text/markdown',
     author='t-a-g-o',
     author_email='santiago@tago.works',
     url='https://tago.works/',
     packages=find_packages(),
```

