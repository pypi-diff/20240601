# Comparing `tmp/extrautilities-1.7.tar.gz` & `tmp/extrautilities-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-1.7.tar", last modified: Thu May 30 09:48:25 2024, max compression
+gzip compressed data, was "extrautilities-1.8.tar", last modified: Sat Jun  1 15:25:15 2024, max compression
```

## Comparing `extrautilities-1.7.tar` & `extrautilities-1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 09:48:25.279210 extrautilities-1.7/
-drwxrwxrwx   0        0        0        0 2024-05-30 09:48:25.264580 extrautilities-1.7/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.7/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.7/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0      729 2024-05-30 09:48:07.000000 extrautilities-1.7/ExtraUtils/asyncThreads.py
--rw-rw-rw-   0        0        0     2909 2024-05-29 19:13:25.000000 extrautilities-1.7/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.7/ExtraUtils/callbackVoid.py
--rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.7/ExtraUtils/getFileContent.py
--rw-rw-rw-   0        0        0     3181 2024-05-28 18:10:03.000000 extrautilities-1.7/ExtraUtils/timeBasedToken.py
--rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-1.7/ExtraUtils/validate_dict.py
--rw-rw-rw-   0        0        0     3349 2024-05-30 09:48:25.278206 extrautilities-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 09:48:25.277710 extrautilities-1.7/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     3349 2024-05-30 09:48:25.000000 extrautilities-1.7/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-05-30 09:48:25.000000 extrautilities-1.7/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 09:48:25.000000 extrautilities-1.7/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 09:48:25.000000 extrautilities-1.7/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-30 09:48:25.000000 extrautilities-1.7/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 09:48:25.279210 extrautilities-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1132 2024-05-30 09:48:24.000000 extrautilities-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:25:15.907260 extrautilities-1.8/
+drwxrwxrwx   0        0        0        0 2024-06-01 15:25:15.889437 extrautilities-1.8/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.8/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.8/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0      729 2024-05-30 09:48:07.000000 extrautilities-1.8/ExtraUtils/asyncThreads.py
+-rw-rw-rw-   0        0        0     3183 2024-06-01 15:25:03.000000 extrautilities-1.8/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.8/ExtraUtils/callbackVoid.py
+-rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.8/ExtraUtils/getFileContent.py
+-rw-rw-rw-   0        0        0     3181 2024-05-28 18:10:03.000000 extrautilities-1.8/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-1.8/ExtraUtils/validate_dict.py
+-rw-rw-rw-   0        0        0     3349 2024-06-01 15:25:15.906754 extrautilities-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:25:15.905732 extrautilities-1.8/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     3349 2024-06-01 15:25:15.000000 extrautilities-1.8/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-06-01 15:25:15.000000 extrautilities-1.8/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:25:15.000000 extrautilities-1.8/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:25:15.000000 extrautilities-1.8/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 15:25:15.000000 extrautilities-1.8/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:25:15.907260 extrautilities-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2024-06-01 15:25:14.000000 extrautilities-1.8/setup.py
```

### Comparing `extrautilities-1.7/ExtraUtils/RateLimit.py` & `extrautilities-1.8/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.7/ExtraUtils/asyncThreads.py` & `extrautilities-1.8/ExtraUtils/asyncThreads.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.7/ExtraUtils/asyncTokens.py` & `extrautilities-1.8/ExtraUtils/asyncTokens.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,40 +51,48 @@
     pub_key = load_pem_public_key(
         key.encode('utf-8'),
         backend=default_backend()
     )
     return pub_key
 
 def sign(message, priv_key):
+    if isinstance(nachricht, str):
+        nachricht = nachricht.encode()
     signature = priv_key.sign(
-        message.encode(),
+        message,
         padding.PSS(
             mgf=padding.MGF1(hashes.SHA256()),
             salt_length=padding.PSS.MAX_LENGTH
         ),
         hashes.SHA256()
     )
     return signature
 
 def verify(message, signature, pub_key):
+    if isinstance(signature, str):
+        signature = signature.encode()
+    if isinstance(message, str):
+        message = message.encode()
     try:
         pub_key.verify(
             signature,
-            message.encode(),
+            message,
             padding.PSS(
                 mgf=padding.MGF1(hashes.SHA256()),
                 salt_length=padding.PSS.MAX_LENGTH
             ),
             hashes.SHA256()
         )
         return True
     except:
         return False
 
 def decrypt(message, priv_key):
+    if isinstance(message, str):
+        message = message.encode()
     decrypted_message = priv_key.decrypt(
         message,
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA256()),
             algorithm=hashes.SHA256(),
             label=None
         )
```

### Comparing `extrautilities-1.7/ExtraUtils/getFileContent.py` & `extrautilities-1.8/ExtraUtils/getFileContent.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.7/ExtraUtils/timeBasedToken.py` & `extrautilities-1.8/ExtraUtils/timeBasedToken.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.7/ExtraUtils/validate_dict.py` & `extrautilities-1.8/ExtraUtils/validate_dict.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.7/PKG-INFO` & `extrautilities-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.7
+Version: 1.8
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.7/README.md` & `extrautilities-1.8/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-1.7/extrautilities.egg-info/PKG-INFO` & `extrautilities-1.8/extrautilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.7
+Version: 1.8
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.7/setup.py` & `extrautilities-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='1.7',
+    version='1.8',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
```

