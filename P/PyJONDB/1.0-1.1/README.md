# Comparing `tmp/pyjondb-1.0.tar.gz` & `tmp/pyjondb-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjondb-1.0.tar", last modified: Sat Jun  1 00:26:44 2024, max compression
+gzip compressed data, was "pyjondb-1.1.tar", last modified: Sat Jun  1 00:32:19 2024, max compression
```

## Comparing `pyjondb-1.0.tar` & `pyjondb-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 00:26:44.097755 pyjondb-1.0/
--rw-rw-rw-   0        0        0     2996 2024-06-01 00:26:44.096432 pyjondb-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 00:26:44.095509 pyjondb-1.0/PyJONDB.egg-info/
--rw-rw-rw-   0        0        0     2996 2024-06-01 00:26:44.000000 pyjondb-1.0/PyJONDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-06-01 00:26:44.000000 pyjondb-1.0/PyJONDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 00:26:44.000000 pyjondb-1.0/PyJONDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 00:26:44.000000 pyjondb-1.0/PyJONDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-01 00:26:44.000000 pyjondb-1.0/PyJONDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 00:26:44.092915 pyjondb-1.0/pyjondb/
--rw-rw-rw-   0        0        0    15374 2024-06-01 00:07:16.000000 pyjondb-1.0/pyjondb/__init__.py
--rw-rw-rw-   0        0        0       42 2024-06-01 00:26:44.098755 pyjondb-1.0/setup.cfg
--rw-rw-rw-   0        0        0     3549 2024-06-01 00:26:40.000000 pyjondb-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:32:19.248740 pyjondb-1.1/
+-rw-rw-rw-   0        0        0     2732 2024-06-01 00:32:19.247740 pyjondb-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 00:32:19.245473 pyjondb-1.1/PyJONDB.egg-info/
+-rw-rw-rw-   0        0        0     2732 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 00:32:19.244471 pyjondb-1.1/pyjondb/
+-rw-rw-rw-   0        0        0    15374 2024-06-01 00:07:16.000000 pyjondb-1.1/pyjondb/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 00:32:19.248740 pyjondb-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1669 2024-06-01 00:32:16.000000 pyjondb-1.1/setup.py
```

### Comparing `pyjondb-1.0/PKG-INFO` & `pyjondb-1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.0
+Version: 1.1
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://github.com/t-a-g-o/PyJONDB
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
@@ -12,52 +12,50 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
 
+# Encrypted JSON Database
 
-        # Encrypted JSON Database
+## Overview
+This package provides a lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation. It uses the `cryptography` library for encryption and decryption of data, ensuring secure storage of your sensitive information.
 
-        ## Overview
-        This package provides a lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation. It uses the `cryptography` library for encryption and decryption of data, ensuring secure storage of your sensitive information.
+## Features
+- **Encryption and Decryption**: Uses Fernet symmetric encryption to protect your data.
+- **Collections**: Supports creating, reading, updating, and deleting collections.
+- **Documents**: Allows adding, finding, updating, and deleting documents within collections.
+- **Aggregation**: Provides basic aggregation functionality for querying documents.
+- **Linking Collections**: Supports linking between collections to create references.
+- **Tree Structure**: Allows creating tree structures by linking root documents to their child documents.
 
-        ## Features
-        - **Encryption and Decryption**: Uses Fernet symmetric encryption to protect your data.
-        - **Collections**: Supports creating, reading, updating, and deleting collections.
-        - **Documents**: Allows adding, finding, updating, and deleting documents within collections.
-        - **Aggregation**: Provides basic aggregation functionality for querying documents.
-        - **Linking Collections**: Supports linking between collections to create references.
-        - **Tree Structure**: Allows creating tree structures by linking root documents to their child documents.
-
-        ## Usage
-        ```python
-        import pyjondb
-
-        # Initialize the database
-        db = pyjondb.database('mydatabase', 'mysecretkey')
-
-        # Create the database
-        db.create()
-
-        # Create a new collection
-        db.create_collection('mycollection')
-
-        # Add a document to the collection
-        document = {'name': 'John Doe', 'age': 30}
-        db.add_document('mycollection', document)
-
-        # Find a document in the collection
-        query = {'name': 'John Doe'}
-        results = db.find_document('mycollection', query)
-        print(results)
-
-        # Update a document in the collection
-        document_id = results[0]['_id']
-        db.update_document('mycollection', document_id, {'age': 31})
+## Usage
+```python
+import pyjondb
 
-        # Delete a document from the collection
-        db.delete_document('mycollection', document_id)
+# Initialize the database
+db = pyjondb.database('mydatabase', 'mysecretkey')
 
-        ### Learn more about it at the docs: https://github.com/t-a-g-o/PyJONDB/wiki
-    
+# Create the database
+db.create()
+
+# Create a new collection
+db.create_collection('mycollection')
+
+# Add a document to the collection
+document = {'name': 'John Doe', 'age': 30}
+db.add_document('mycollection', document)
+
+# Find a document in the collection
+query = {'name': 'John Doe'}
+results = db.find_document('mycollection', query)
+print(results)
+
+# Update a document in the collection
+document_id = results[0]['_id']
+db.update_document('mycollection', document_id, {'age': 31})
+
+# Delete a document from the collection
+db.delete_document('mycollection', document_id)
+
+### Learn more about it at the docs: https://github.com/t-a-g-o/PyJONDB/wiki
```

### Comparing `pyjondb-1.0/PyJONDB.egg-info/PKG-INFO` & `pyjondb-1.1/PyJONDB.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.0
+Version: 1.1
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://github.com/t-a-g-o/PyJONDB
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
@@ -12,52 +12,50 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
 
+# Encrypted JSON Database
 
-        # Encrypted JSON Database
+## Overview
+This package provides a lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation. It uses the `cryptography` library for encryption and decryption of data, ensuring secure storage of your sensitive information.
 
-        ## Overview
-        This package provides a lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation. It uses the `cryptography` library for encryption and decryption of data, ensuring secure storage of your sensitive information.
+## Features
+- **Encryption and Decryption**: Uses Fernet symmetric encryption to protect your data.
+- **Collections**: Supports creating, reading, updating, and deleting collections.
+- **Documents**: Allows adding, finding, updating, and deleting documents within collections.
+- **Aggregation**: Provides basic aggregation functionality for querying documents.
+- **Linking Collections**: Supports linking between collections to create references.
+- **Tree Structure**: Allows creating tree structures by linking root documents to their child documents.
 
-        ## Features
-        - **Encryption and Decryption**: Uses Fernet symmetric encryption to protect your data.
-        - **Collections**: Supports creating, reading, updating, and deleting collections.
-        - **Documents**: Allows adding, finding, updating, and deleting documents within collections.
-        - **Aggregation**: Provides basic aggregation functionality for querying documents.
-        - **Linking Collections**: Supports linking between collections to create references.
-        - **Tree Structure**: Allows creating tree structures by linking root documents to their child documents.
-
-        ## Usage
-        ```python
-        import pyjondb
-
-        # Initialize the database
-        db = pyjondb.database('mydatabase', 'mysecretkey')
-
-        # Create the database
-        db.create()
-
-        # Create a new collection
-        db.create_collection('mycollection')
-
-        # Add a document to the collection
-        document = {'name': 'John Doe', 'age': 30}
-        db.add_document('mycollection', document)
-
-        # Find a document in the collection
-        query = {'name': 'John Doe'}
-        results = db.find_document('mycollection', query)
-        print(results)
-
-        # Update a document in the collection
-        document_id = results[0]['_id']
-        db.update_document('mycollection', document_id, {'age': 31})
+## Usage
+```python
+import pyjondb
 
-        # Delete a document from the collection
-        db.delete_document('mycollection', document_id)
+# Initialize the database
+db = pyjondb.database('mydatabase', 'mysecretkey')
 
-        ### Learn more about it at the docs: https://github.com/t-a-g-o/PyJONDB/wiki
-    
+# Create the database
+db.create()
+
+# Create a new collection
+db.create_collection('mycollection')
+
+# Add a document to the collection
+document = {'name': 'John Doe', 'age': 30}
+db.add_document('mycollection', document)
+
+# Find a document in the collection
+query = {'name': 'John Doe'}
+results = db.find_document('mycollection', query)
+print(results)
+
+# Update a document in the collection
+document_id = results[0]['_id']
+db.update_document('mycollection', document_id, {'age': 31})
+
+# Delete a document from the collection
+db.delete_document('mycollection', document_id)
+
+### Learn more about it at the docs: https://github.com/t-a-g-o/PyJONDB/wiki
```

### Comparing `pyjondb-1.0/pyjondb/__init__.py` & `pyjondb-1.1/pyjondb/__init__.py`

 * *Files identical despite different names*

