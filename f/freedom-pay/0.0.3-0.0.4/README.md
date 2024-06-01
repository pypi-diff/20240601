# Comparing `tmp/freedom_pay-0.0.3.tar.gz` & `tmp/freedom_pay-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freedom_pay-0.0.3.tar", last modified: Fri May 24 05:30:39 2024, max compression
+gzip compressed data, was "freedom_pay-0.0.4.tar", last modified: Sat Jun  1 08:02:44 2024, max compression
```

## Comparing `freedom_pay-0.0.3.tar` & `freedom_pay-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 05:30:39.280578 freedom_pay-0.0.3/
--rw-rw-rw-   0        0        0     1057 2024-05-23 06:09:01.000000 freedom_pay-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      600 2024-05-24 05:30:39.280578 freedom_pay-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 11:40:11.000000 freedom_pay-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 05:30:39.273578 freedom_pay-0.0.3/freedom_pay/
--rw-rw-rw-   0        0        0        0 2024-05-23 05:30:35.000000 freedom_pay-0.0.3/freedom_pay/__init__.py
--rw-rw-rw-   0        0        0     8148 2024-05-23 06:09:01.000000 freedom_pay-0.0.3/freedom_pay/main.py
--rw-rw-rw-   0        0        0     1422 2024-05-23 06:14:42.000000 freedom_pay-0.0.3/freedom_pay/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 05:30:39.279578 freedom_pay-0.0.3/freedom_pay.egg-info/
--rw-rw-rw-   0        0        0      600 2024-05-24 05:30:39.000000 freedom_pay-0.0.3/freedom_pay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-05-24 05:30:39.000000 freedom_pay-0.0.3/freedom_pay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 05:30:39.000000 freedom_pay-0.0.3/freedom_pay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-24 05:30:39.000000 freedom_pay-0.0.3/freedom_pay.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-24 05:30:39.000000 freedom_pay-0.0.3/freedom_pay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 05:30:39.281582 freedom_pay-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-24 05:28:30.000000 freedom_pay-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:02:44.499033 freedom_pay-0.0.4/
+-rw-rw-rw-   0        0        0     1057 2024-05-23 06:09:01.000000 freedom_pay-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      600 2024-06-01 08:02:44.499033 freedom_pay-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-23 11:40:11.000000 freedom_pay-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 08:02:44.488998 freedom_pay-0.0.4/freedom_pay/
+-rw-rw-rw-   0        0        0        0 2024-05-23 05:30:35.000000 freedom_pay-0.0.4/freedom_pay/__init__.py
+-rw-rw-rw-   0        0        0     8149 2024-05-24 05:51:51.000000 freedom_pay-0.0.4/freedom_pay/service.py
+-rw-rw-rw-   0        0        0     1422 2024-05-23 06:14:42.000000 freedom_pay-0.0.4/freedom_pay/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:02:44.497999 freedom_pay-0.0.4/freedom_pay.egg-info/
+-rw-rw-rw-   0        0        0      600 2024-06-01 08:02:44.000000 freedom_pay-0.0.4/freedom_pay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-06-01 08:02:44.000000 freedom_pay-0.0.4/freedom_pay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 08:02:44.000000 freedom_pay-0.0.4/freedom_pay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-06-01 08:02:44.000000 freedom_pay-0.0.4/freedom_pay.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 08:02:44.000000 freedom_pay-0.0.4/freedom_pay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 08:02:44.501034 freedom_pay-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-06-01 08:01:10.000000 freedom_pay-0.0.4/setup.py
```

### Comparing `freedom_pay-0.0.3/LICENSE` & `freedom_pay-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `freedom_pay-0.0.3/PKG-INFO` & `freedom_pay-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedom_pay
-Version: 0.0.3
+Version: 0.0.4
 Summary: wqewqewqewq
 Home-page: https://gitlab.com/erlan.kubanychbekov.000/freedompay_lib
 Author: erllan.000
 Author-email: erlan.kubanychbekov.000@gmail.com
 Project-URL: GitLab, https://gitlab.com/erlan.kubanychbekov.000/freedompay_lib
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `freedom_pay-0.0.3/freedom_pay/main.py` & `freedom_pay-0.0.4/freedom_pay/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import hashlib
 import xml.etree.ElementTree as ET
-from utils import generate_random_string
+from .utils import generate_random_string
 from datetime import timedelta, timezone
 
 
 class FreedomPay:
     DOMAIN = 'api.paybox.money'
 
     def __init__(self, merchant_id, secret_key, pg_success_url, pg_failure_url, pg_back_link):
```

### Comparing `freedom_pay-0.0.3/freedom_pay/utils.py` & `freedom_pay-0.0.4/freedom_pay/utils.py`

 * *Files identical despite different names*

### Comparing `freedom_pay-0.0.3/freedom_pay.egg-info/PKG-INFO` & `freedom_pay-0.0.4/freedom_pay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedom_pay
-Version: 0.0.3
+Version: 0.0.4
 Summary: wqewqewqewq
 Home-page: https://gitlab.com/erlan.kubanychbekov.000/freedompay_lib
 Author: erllan.000
 Author-email: erlan.kubanychbekov.000@gmail.com
 Project-URL: GitLab, https://gitlab.com/erlan.kubanychbekov.000/freedompay_lib
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `freedom_pay-0.0.3/setup.py` & `freedom_pay-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='freedom_pay',
-    version='0.0.3',
+    version='0.0.4',
     author='erllan.000',
     author_email='erlan.kubanychbekov.000@gmail.com',
     description='wqewqewqewq',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/erlan.kubanychbekov.000/freedompay_lib',
     packages=find_packages(),
```

