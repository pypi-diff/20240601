# Comparing `tmp/anne-1.1.1.tar.gz` & `tmp/anne-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anne-1.1.1.tar", last modified: Sat Jun  1 10:32:02 2024, max compression
+gzip compressed data, was "anne-1.1.2.tar", last modified: Sat Jun  1 10:57:07 2024, max compression
```

## Comparing `anne-1.1.1.tar` & `anne-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 10:32:02.724558 anne-1.1.1/
--rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2295 2024-06-01 10:32:02.724558 anne-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 10:32:02.720571 anne-1.1.1/app/
-drwxrwxrwx   0        0        0        0 2024-06-01 10:32:02.721567 anne-1.1.1/app/anne/
--rw-rw-rw-   0        0        0       90 2024-06-01 09:09:16.000000 anne-1.1.1/app/anne/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:32:02.723561 anne-1.1.1/app/anne/browser/
--rw-rw-rw-   0        0        0    18825 2024-05-31 00:58:51.000000 anne-1.1.1/app/anne/browser/AnneBrowser.py
--rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.1.1/app/anne/browser/__init__.py
--rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.1.1/app/anne/browser/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:32:02.723561 anne-1.1.1/app/anne/info/
--rw-rw-rw-   0        0        0     5935 2024-06-01 10:22:47.000000 anne-1.1.1/app/anne/info/AnneInfo.py
--rw-rw-rw-   0        0        0       32 2024-06-01 09:09:05.000000 anne-1.1.1/app/anne/info/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:32:02.724558 anne-1.1.1/app/anne/proxy/
--rw-rw-rw-   0        0        0     5495 2024-06-01 09:07:50.000000 anne-1.1.1/app/anne/proxy/AnneProxy.py
--rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.1.1/app/anne/proxy/__init__.py
--rw-rw-rw-   0        0        0        2 2024-06-01 09:07:41.000000 anne-1.1.1/app/anne/proxy/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:32:02.722564 anne-1.1.1/app/anne.egg-info/
--rw-rw-rw-   0        0        0     2295 2024-06-01 10:32:02.000000 anne-1.1.1/app/anne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-06-01 10:32:02.000000 anne-1.1.1/app/anne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 10:32:02.000000 anne-1.1.1/app/anne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-06-01 10:32:02.000000 anne-1.1.1/app/anne.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-06-01 10:32:02.000000 anne-1.1.1/app/anne.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 10:32:02.724558 anne-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-06-01 10:32:02.000000 anne-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.541379 anne-1.1.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2293 2024-06-01 10:57:07.540382 anne-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.536395 anne-1.1.2/app/
+drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.537392 anne-1.1.2/app/anne/
+-rw-rw-rw-   0        0        0       90 2024-06-01 09:09:16.000000 anne-1.1.2/app/anne/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.539386 anne-1.1.2/app/anne/browser/
+-rw-rw-rw-   0        0        0    18825 2024-05-31 00:58:51.000000 anne-1.1.2/app/anne/browser/AnneBrowser.py
+-rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.1.2/app/anne/browser/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.1.2/app/anne/browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.539386 anne-1.1.2/app/anne/info/
+-rw-rw-rw-   0        0        0     6678 2024-06-01 10:56:55.000000 anne-1.1.2/app/anne/info/AnneInfo.py
+-rw-rw-rw-   0        0        0       32 2024-06-01 09:09:05.000000 anne-1.1.2/app/anne/info/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.540382 anne-1.1.2/app/anne/proxy/
+-rw-rw-rw-   0        0        0     5495 2024-06-01 09:07:50.000000 anne-1.1.2/app/anne/proxy/AnneProxy.py
+-rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.1.2/app/anne/proxy/__init__.py
+-rw-rw-rw-   0        0        0        2 2024-06-01 09:07:41.000000 anne-1.1.2/app/anne/proxy/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.538389 anne-1.1.2/app/anne.egg-info/
+-rw-rw-rw-   0        0        0     2293 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 10:57:07.541379 anne-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-06-01 10:57:06.000000 anne-1.1.2/setup.py
```

### Comparing `anne-1.1.1/LICENSE` & `anne-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anne-1.1.1/PKG-INFO` & `anne-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.1.1
+Version: 1.1.2
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Anne
-
 Anne - Fast and easy
 
 ## Mục lục
 
 - [Giới thiệu](#giới-thiệu)
 - [Cài đặt](#cài-đặt)
 - [Cập nhật](#cập-nhật)
```

### Comparing `anne-1.1.1/app/anne/browser/AnneBrowser.py` & `anne-1.1.2/app/anne/browser/AnneBrowser.py`

 * *Files identical despite different names*

### Comparing `anne-1.1.1/app/anne/browser/utils.py` & `anne-1.1.2/app/anne/browser/utils.py`

 * *Files identical despite different names*

### Comparing `anne-1.1.1/app/anne/info/AnneInfo.py` & `anne-1.1.2/app/anne/info/AnneInfo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import requests, random, string, os, unidecode
-
+from faker import Faker
 
 class AnneInfo:
     def __init__(self, country='vn'):
         self.name_list = {
             "vn": ['fname_vn', 'lname_vn'],
             "us": ['fname_us', 'lname_us']
         }
-        if country not in self.name_list: raise ValueError(f"Không hỗ trợ quốc gia: {country}")
+        if country not in self.name_list: raise ValueError(f"Không hỗ trợ quốc gia: {country}\nCác quốc gia được hỗ trợ: vn, us")
         self.country = country
         self.current_dir = os.path.dirname(os.path.abspath(__file__))
-
+        self.faker = Faker()
 
     def get_name(self):
         if self.country in self.name_list:
             fname_path = os.path.join(self.current_dir, 'data', f'{self.name_list[self.country][0]}.txt')
             lname_path = os.path.join(self.current_dir, 'data', f'{self.name_list[self.country][1]}.txt')
             with open(fname_path, 'r', encoding='utf-8') as f: first_names = f.readlines()
             with open(lname_path, 'r', encoding='utf-8') as l: last_names = l.readlines()
@@ -86,22 +86,32 @@
                     psw += random_string
                 else:
                     psw += part
             return psw
         else:
             return "annesayhi"
 
+    def get_ua(self, platform='auto'):
+        _platform = ['auto', 'android', 'ios', 'win', 'mac', 'linux']
+        if platform not in _platform: raise ValueError(f"Không hỗ trợ platform: {platform}\nPlatforms được hỗ trợ: {_platform}")
+        if platform in _platform:
+            if platform == 'auto': return self.faker.user_agent()
+            uas = os.path.join(self.current_dir, 'data', f'ua_{platform}.txt')
+            with open(uas, 'r', encoding='utf-8') as f: user_agents = f.readlines()
+            return random.choice(user_agents).strip()
+
     def get_info(self,
                 day_space=(1, 28),
                 month_space=(1, 12),
                 year_space=(1960, 2004),
                 username_custom=None,
                 password_custom=None,
                 password_space=(12, 18),
-                domain=None
+                domain=None,
+                platform='auto'
 
                       ):
 
         data = {
             "name": {
                 "first": "",
                 "last": "",
@@ -110,23 +120,21 @@
             "birth": {
                 "day": "",
                 "month": "",
                 "year": "",
                 "full": ""
             },
             "email": "",
-            "password": ""
+            "password": "",
+            "user_agent": ""
         }
 
 
         name_data = self.get_name()
         birth_data = self.get_birth(day_space, month_space, year_space)
-        password_data = self.get_password(password_space, password_custom)
-        email_data = self.get_email(name_data["first_name"], name_data["last_name"], username_custom, domain)
-
 
         # Name
         data["name"]["first"] = name_data["first_name"]
         data["name"]["last"] = name_data["last_name"]
 
         if self.country == 'vn': data["name"]["full"] = f"{name_data['last_name']} {name_data['first_name']}"
         elif self.country == 'us': data["name"]["full"] = f"{name_data['first_name']} {name_data['last_name']}"
@@ -134,18 +142,22 @@
         # Birth
         data["birth"]["day"] = birth_data["day"]
         data["birth"]["month"] = birth_data["month"]
         data["birth"]["year"] = birth_data["year"]
         data["birth"]["full"] = birth_data["full"]
 
         # Email
-        data["email"] = email_data
+        data["email"] = self.get_email(name_data["first_name"], name_data["last_name"], username_custom, domain)
 
         # Password
-        data["password"] = password_data
+        data["password"] = self.get_password(password_space, password_custom)
+
+        # User Agent
+        data["user_agent"] = self.get_ua(platform)
+
         return data
```

### Comparing `anne-1.1.1/app/anne/proxy/AnneProxy.py` & `anne-1.1.2/app/anne/proxy/AnneProxy.py`

 * *Files identical despite different names*

### Comparing `anne-1.1.1/app/anne.egg-info/PKG-INFO` & `anne-1.1.2/app/anne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.1.1
+Version: 1.1.2
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Anne
-
 Anne - Fast and easy
 
 ## Mục lục
 
 - [Giới thiệu](#giới-thiệu)
 - [Cài đặt](#cài-đặt)
 - [Cập nhật](#cập-nhật)
```

### Comparing `anne-1.1.1/setup.py` & `anne-1.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="anne",
-    version="1.1.1",
+    version="1.1.2",
     description="Lib for lazy dev",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrship666/anne-lib",
     author="AnneHouman",
```

