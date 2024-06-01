# Comparing `tmp/lama2923-1.1.6.tar.gz` & `tmp/lama2923-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-1.1.6.tar", last modified: Fri May 31 16:53:23 2024, max compression
+gzip compressed data, was "lama2923-1.1.7.tar", last modified: Sat Jun  1 19:12:21 2024, max compression
```

## Comparing `lama2923-1.1.6.tar` & `lama2923-1.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 16:53:23.242267 lama2923-1.1.6/
--rw-rw-rw-   0        0        0      962 2024-05-31 16:53:23.241293 lama2923-1.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 16:53:23.172918 lama2923-1.1.6/lama2923/
--rw-rw-rw-   0        0        0    24701 2024-05-31 16:53:13.000000 lama2923-1.1.6/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 16:53:23.193571 lama2923-1.1.6/lama2923.egg-info/
--rw-rw-rw-   0        0        0      962 2024-05-31 16:53:22.000000 lama2923-1.1.6/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-31 16:53:23.000000 lama2923-1.1.6/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 16:53:22.000000 lama2923-1.1.6/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 16:53:22.000000 lama2923-1.1.6/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 16:53:22.000000 lama2923-1.1.6/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 16:53:23.242267 lama2923-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1300 2024-05-31 16:53:09.000000 lama2923-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 19:12:21.234819 lama2923-1.1.7/
+-rw-rw-rw-   0        0        0      962 2024-06-01 19:12:21.225500 lama2923-1.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 19:12:21.155225 lama2923-1.1.7/lama2923/
+-rw-rw-rw-   0        0        0    24410 2024-06-01 19:11:36.000000 lama2923-1.1.7/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 19:12:21.221866 lama2923-1.1.7/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      962 2024-06-01 19:12:20.000000 lama2923-1.1.7/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-06-01 19:12:20.000000 lama2923-1.1.7/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 19:12:20.000000 lama2923-1.1.7/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-06-01 19:12:20.000000 lama2923-1.1.7/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 19:12:20.000000 lama2923-1.1.7/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 19:12:21.235332 lama2923-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2024-06-01 19:12:07.000000 lama2923-1.1.7/setup.py
```

### Comparing `lama2923-1.1.6/PKG-INFO` & `lama2923-1.1.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.1.6
+Version: 1.1.7
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.1.6/lama2923/__init__.py` & `lama2923-1.1.7/lama2923/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,20 +189,20 @@
 
 
 
 
 
 
 class Discord:
-    class User:
+    class Author:
         def __init__(self, token):
             self.token = str(token)
             response = requests.get('https://discord.com/api/v9/users/@me', headers={'Authorization': self.token})
             if response.status_code != 200:
-                raise TokenIsNotWork('Token is not working!')
+                raise TokenIsNotWork('Token : \'{}\' is not working!'.format(self.token))
             
         def send_message(self, Channel_id, Message, files=None):
             payload = {'content': str(Message)}
             headers = {'Authorization': self.token}
             if files is not None and isinstance(files, list):
                 files_data = {
                     os.path.basename(file_name): open(file_name, "rb").read()
@@ -238,19 +238,15 @@
             return response.status_code
         
         def get_channel_messages(self, Channel_id, limit=50):
             headers = {'Authorization': self.token}
             params = {'limit': limit}
             response = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}/messages', headers=headers, params=params)
             return response.status_code, response.json() if response.status_code == 200 else response.status_code
-        
-        def get_channel(self, Channel_id):
-            headers = {'Authorization': self.token}
-            response = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}', headers=headers)
-            return response.status_code, response.json() if response.status_code == 200 else response.status_code    
+          
     
         def get_channel_message(self, Channel_id, Message_id):
             headers = {'Authorization': self.token}
             response = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}', headers=headers)
             return response.status_code, response.json() if response.status_code == 200 else response.status_code
 
         def add_reaction(self, Channel_id, Message_id, emoji):
```

### Comparing `lama2923-1.1.6/lama2923.egg-info/PKG-INFO` & `lama2923-1.1.7/lama2923.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.1.6
+Version: 1.1.7
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.1.6/setup.py` & `lama2923-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='1.1.6',
+    version='1.1.7',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Api ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve Api işlemleri için kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

