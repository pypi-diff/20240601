# Comparing `tmp/extrautilities-1.9.tar.gz` & `tmp/extrautilities-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-1.9.tar", last modified: Sat Jun  1 15:27:13 2024, max compression
+gzip compressed data, was "extrautilities-2.0.tar", last modified: Sat Jun  1 15:39:14 2024, max compression
```

## Comparing `extrautilities-1.9.tar` & `extrautilities-2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:13.661392 extrautilities-1.9/
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:13.646695 extrautilities-1.9/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.9/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.9/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0      729 2024-05-30 09:48:07.000000 extrautilities-1.9/ExtraUtils/asyncThreads.py
--rw-rw-rw-   0        0        0     3177 2024-06-01 15:26:58.000000 extrautilities-1.9/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.9/ExtraUtils/callbackVoid.py
--rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.9/ExtraUtils/getFileContent.py
--rw-rw-rw-   0        0        0     3181 2024-05-28 18:10:03.000000 extrautilities-1.9/ExtraUtils/timeBasedToken.py
--rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-1.9/ExtraUtils/validate_dict.py
--rw-rw-rw-   0        0        0     3349 2024-06-01 15:27:13.660888 extrautilities-1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:13.659255 extrautilities-1.9/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     3349 2024-06-01 15:27:13.000000 extrautilities-1.9/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-06-01 15:27:13.000000 extrautilities-1.9/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:27:13.000000 extrautilities-1.9/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:27:13.000000 extrautilities-1.9/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-06-01 15:27:13.000000 extrautilities-1.9/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:27:13.661392 extrautilities-1.9/setup.cfg
--rw-rw-rw-   0        0        0     1132 2024-06-01 15:27:12.000000 extrautilities-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:39:14.625389 extrautilities-2.0/
+drwxrwxrwx   0        0        0        0 2024-06-01 15:39:14.610794 extrautilities-2.0/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-2.0/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-2.0/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0      729 2024-05-30 09:48:07.000000 extrautilities-2.0/ExtraUtils/asyncThreads.py
+-rw-rw-rw-   0        0        0     3168 2024-06-01 15:37:59.000000 extrautilities-2.0/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-2.0/ExtraUtils/callbackVoid.py
+-rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-2.0/ExtraUtils/getFileContent.py
+-rw-rw-rw-   0        0        0     3181 2024-05-28 18:10:03.000000 extrautilities-2.0/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-2.0/ExtraUtils/validate_dict.py
+-rw-rw-rw-   0        0        0     3349 2024-06-01 15:39:14.624884 extrautilities-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:39:14.623375 extrautilities-2.0/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     3349 2024-06-01 15:39:14.000000 extrautilities-2.0/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-06-01 15:39:14.000000 extrautilities-2.0/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:39:14.000000 extrautilities-2.0/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:39:14.000000 extrautilities-2.0/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 15:39:14.000000 extrautilities-2.0/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:39:14.625389 extrautilities-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2024-06-01 15:38:35.000000 extrautilities-2.0/setup.py
```

### Comparing `extrautilities-1.9/ExtraUtils/RateLimit.py` & `extrautilities-2.0/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.9/ExtraUtils/asyncThreads.py` & `extrautilities-2.0/ExtraUtils/asyncThreads.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.9/ExtraUtils/asyncTokens.py` & `extrautilities-2.0/ExtraUtils/asyncTokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         message,
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA256()),
             algorithm=hashes.SHA256(),
             label=None
         )
     )
-    return decrypted_message.decode()
+    return decrypted_message
 
 # Example:
 # priv_key, pub_key = generiere_rsa_schluesselpaar()
 # message = encrypt("Geheime Nachricht", pub_key)
 # print(f"Verschlüsselt: {message}")
 # 
 # decrypted_message = decrypt(message, priv_key)
```

### Comparing `extrautilities-1.9/ExtraUtils/getFileContent.py` & `extrautilities-2.0/ExtraUtils/getFileContent.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.9/ExtraUtils/timeBasedToken.py` & `extrautilities-2.0/ExtraUtils/timeBasedToken.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.9/ExtraUtils/validate_dict.py` & `extrautilities-2.0/ExtraUtils/validate_dict.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.9/PKG-INFO` & `extrautilities-2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.9
+Version: 2.0
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.9/README.md` & `extrautilities-2.0/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-1.9/extrautilities.egg-info/PKG-INFO` & `extrautilities-2.0/extrautilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.9
+Version: 2.0
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.9/setup.py` & `extrautilities-2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='1.9',
+    version='2.0',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
```

