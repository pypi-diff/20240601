# Comparing `tmp/terraform-backend-s3-bucket-1.0.4.tar.gz` & `tmp/terraform-backend-s3-bucket-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terraform-backend-s3-bucket-1.0.4.tar", last modified: Wed May  1 06:29:12 2024, max compression
+gzip compressed data, was "terraform-backend-s3-bucket-1.0.5.tar", last modified: Sat Jun  1 06:03:34 2024, max compression
```

## Comparing `terraform-backend-s3-bucket-1.0.4.tar` & `terraform-backend-s3-bucket-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24335 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@1.0.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:28:59.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:29:12.982744 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 06:29:12.000000 terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:03:34.113515 terraform-backend-s3-bucket-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-06-01 06:03:34.113515 terraform-backend-s3-bucket-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:03:34.113515 terraform-backend-s3-bucket-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:03:34.113515 terraform-backend-s3-bucket-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:03:34.113515 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:03:34.113515 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24365 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@1.0.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:03:21.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:03:34.113515 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-06-01 06:03:34.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-06-01 06:03:34.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:03:34.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 06:03:34.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 06:03:34.000000 terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket.egg-info/top_level.txt
```

### Comparing `terraform-backend-s3-bucket-1.0.4/LICENSE` & `terraform-backend-s3-bucket-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-1.0.4/PKG-INFO` & `terraform-backend-s3-bucket-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-backend-s3-bucket
-Version: 1.0.4
+Version: 1.0.5
 Summary: Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.
 Home-page: https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `terraform-backend-s3-bucket-1.0.4/setup.py` & `terraform-backend-s3-bucket-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "terraform-backend-s3-bucket",
-    "version": "1.0.4",
+    "version": "1.0.5",
     "description": "Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/terraform-backend-s3-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "terraform_backend_s3_bucket",
         "terraform_backend_s3_bucket._jsii"
     ],
     "package_data": {
         "terraform_backend_s3_bucket._jsii": [
-            "terraform-backend-s3-bucket@1.0.4.jsii.tgz"
+            "terraform-backend-s3-bucket@1.0.5.jsii.tgz"
         ],
         "terraform_backend_s3_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket/__init__.py` & `terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/PKG-INFO` & `terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraform-backend-s3-bucket
-Version: 1.0.4
+Version: 1.0.5
 Summary: Creates an S3 bucket and a DynamoDB table for Terraform state and lock management.
 Home-page: https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/terraform-backend-s3-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `terraform-backend-s3-bucket-1.0.4/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt` & `terraform-backend-s3-bucket-1.0.5/src/terraform_backend_s3_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/terraform_backend_s3_bucket/py.typed
 src/terraform_backend_s3_bucket.egg-info/PKG-INFO
 src/terraform_backend_s3_bucket.egg-info/SOURCES.txt
 src/terraform_backend_s3_bucket.egg-info/dependency_links.txt
 src/terraform_backend_s3_bucket.egg-info/requires.txt
 src/terraform_backend_s3_bucket.egg-info/top_level.txt
 src/terraform_backend_s3_bucket/_jsii/__init__.py
-src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@1.0.4.jsii.tgz
+src/terraform_backend_s3_bucket/_jsii/terraform-backend-s3-bucket@1.0.5.jsii.tgz
```

