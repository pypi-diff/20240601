# Comparing `tmp/anne-1.1.2.tar.gz` & `tmp/anne-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anne-1.1.2.tar", last modified: Sat Jun  1 10:57:07 2024, max compression
+gzip compressed data, was "anne-1.1.3.tar", last modified: Sat Jun  1 14:19:33 2024, max compression
```

## Comparing `anne-1.1.2.tar` & `anne-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.541379 anne-1.1.2/
--rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     2293 2024-06-01 10:57:07.540382 anne-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.536395 anne-1.1.2/app/
-drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.537392 anne-1.1.2/app/anne/
--rw-rw-rw-   0        0        0       90 2024-06-01 09:09:16.000000 anne-1.1.2/app/anne/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.539386 anne-1.1.2/app/anne/browser/
--rw-rw-rw-   0        0        0    18825 2024-05-31 00:58:51.000000 anne-1.1.2/app/anne/browser/AnneBrowser.py
--rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.1.2/app/anne/browser/__init__.py
--rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.1.2/app/anne/browser/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.539386 anne-1.1.2/app/anne/info/
--rw-rw-rw-   0        0        0     6678 2024-06-01 10:56:55.000000 anne-1.1.2/app/anne/info/AnneInfo.py
--rw-rw-rw-   0        0        0       32 2024-06-01 09:09:05.000000 anne-1.1.2/app/anne/info/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.540382 anne-1.1.2/app/anne/proxy/
--rw-rw-rw-   0        0        0     5495 2024-06-01 09:07:50.000000 anne-1.1.2/app/anne/proxy/AnneProxy.py
--rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.1.2/app/anne/proxy/__init__.py
--rw-rw-rw-   0        0        0        2 2024-06-01 09:07:41.000000 anne-1.1.2/app/anne/proxy/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:57:07.538389 anne-1.1.2/app/anne.egg-info/
--rw-rw-rw-   0        0        0     2293 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-06-01 10:57:07.000000 anne-1.1.2/app/anne.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 10:57:07.541379 anne-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-06-01 10:57:06.000000 anne-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:19:33.464606 anne-1.1.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2293 2024-06-01 14:19:33.464606 anne-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 14:19:33.459620 anne-1.1.3/app/
+drwxrwxrwx   0        0        0        0 2024-06-01 14:19:33.460622 anne-1.1.3/app/anne/
+-rw-rw-rw-   0        0        0      126 2024-06-01 13:21:49.000000 anne-1.1.3/app/anne/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:19:33.462613 anne-1.1.3/app/anne/browser/
+-rw-rw-rw-   0        0        0    18825 2024-05-31 00:58:51.000000 anne-1.1.3/app/anne/browser/AnneBrowser.py
+-rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.1.3/app/anne/browser/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.1.3/app/anne/browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:19:33.463609 anne-1.1.3/app/anne/captcha/
+-rw-rw-rw-   0        0        0     4461 2024-06-01 14:06:46.000000 anne-1.1.3/app/anne/captcha/AnneCaptcha.py
+-rw-rw-rw-   0        0        0       38 2024-06-01 13:21:40.000000 anne-1.1.3/app/anne/captcha/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:19:33.463609 anne-1.1.3/app/anne/info/
+-rw-rw-rw-   0        0        0     8182 2024-06-01 14:19:19.000000 anne-1.1.3/app/anne/info/AnneInfo.py
+-rw-rw-rw-   0        0        0       32 2024-06-01 09:09:05.000000 anne-1.1.3/app/anne/info/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:19:33.464606 anne-1.1.3/app/anne/proxy/
+-rw-rw-rw-   0        0        0     5687 2024-06-01 14:06:15.000000 anne-1.1.3/app/anne/proxy/AnneProxy.py
+-rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.1.3/app/anne/proxy/__init__.py
+-rw-rw-rw-   0        0        0        2 2024-06-01 09:07:41.000000 anne-1.1.3/app/anne/proxy/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:19:33.462613 anne-1.1.3/app/anne.egg-info/
+-rw-rw-rw-   0        0        0     2293 2024-06-01 14:19:33.000000 anne-1.1.3/app/anne.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-06-01 14:19:33.000000 anne-1.1.3/app/anne.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 14:19:33.000000 anne-1.1.3/app/anne.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-06-01 14:19:33.000000 anne-1.1.3/app/anne.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 14:19:33.000000 anne-1.1.3/app/anne.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 14:19:33.464606 anne-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-06-01 14:19:32.000000 anne-1.1.3/setup.py
```

### Comparing `anne-1.1.2/LICENSE` & `anne-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anne-1.1.2/PKG-INFO` & `anne-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.1.2
+Version: 1.1.3
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.1.2/app/anne/browser/AnneBrowser.py` & `anne-1.1.3/app/anne/browser/AnneBrowser.py`

 * *Files identical despite different names*

### Comparing `anne-1.1.2/app/anne/browser/utils.py` & `anne-1.1.3/app/anne/browser/utils.py`

 * *Files identical despite different names*

### Comparing `anne-1.1.2/app/anne/info/AnneInfo.py` & `anne-1.1.3/app/anne/info/AnneInfo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,196 @@
 import requests, random, string, os, unidecode
 from faker import Faker
 
 class AnneInfo:
-    def __init__(self, country='vn'):
+    def __init__(self, country='vn', debug=False):
         self.name_list = {
             "vn": ['fname_vn', 'lname_vn'],
             "us": ['fname_us', 'lname_us']
         }
-        if country not in self.name_list: raise ValueError(f"Không hỗ trợ quốc gia: {country}\nCác quốc gia được hỗ trợ: vn, us")
+        if country not in self.name_list: raise ValueError(f"Không hỗ trợ quốc gia: {country}")
         self.country = country
         self.current_dir = os.path.dirname(os.path.abspath(__file__))
         self.faker = Faker()
+        self.debug = debug
 
-    def get_name(self):
-        if self.country in self.name_list:
-            fname_path = os.path.join(self.current_dir, 'data', f'{self.name_list[self.country][0]}.txt')
-            lname_path = os.path.join(self.current_dir, 'data', f'{self.name_list[self.country][1]}.txt')
-            with open(fname_path, 'r', encoding='utf-8') as f: first_names = f.readlines()
-            with open(lname_path, 'r', encoding='utf-8') as l: last_names = l.readlines()
-            first_name = random.choice(first_names).strip()
-            last_name = random.choice(last_names).strip()
-            data = {
-                "first_name": first_name,
-                "last_name": last_name
-            }
-            return data
-        else:
-            raise ValueError(f"Unsupported country: {country}")
-
-    def get_birth(self, day_space=(1, 28), month_space=(1, 12), year_space=(1960, 2004)):
-        day = random.randint(day_space[0], day_space[1])
-        month = random.randint(month_space[0], month_space[1])
-        year = random.randint(year_space[0], year_space[1])
-        full = f"{day}/{month}/{year}"
-        data = {
-            "day": day,
-            "month": month,
-            "year": year,
-            "full": full
-        }
-        return data
+    def getName(self):
+        data = {"first_name": None, "last_name": None}
+        try:
+            if self.country in self.name_list:
+                fname_path = os.path.join(self.current_dir, 'data', f'{self.name_list[self.country][0]}.txt')
+                lname_path = os.path.join(self.current_dir, 'data', f'{self.name_list[self.country][1]}.txt')
+                with open(fname_path, 'r', encoding='utf-8') as f: first_names = f.readlines()
+                with open(lname_path, 'r', encoding='utf-8') as l: last_names = l.readlines()
+                first_name = random.choice(first_names).strip()
+                last_name = random.choice(last_names).strip()
+                data["first_name"] = first_name
+                data["last_name"] = last_name
+                return data
+            else: print(f"Không hỗ trợ quốc gia: {self.country}")
+        except Exception as e:
+            if self.debug: print(f'Lỗi [getName]: {e}')
+            return data
+
+    def getBirth(self, day_space=(1, 28), month_space=(1, 12), year_space=(1960, 2004)):
+        try:
+            data = {"day": None, "month": None, "year": None, "full": None}
+            day = random.randint(day_space[0], day_space[1])
+            month = random.randint(month_space[0], month_space[1])
+            year = random.randint(year_space[0], year_space[1])
+            data["day"] = day
+            data["month"] = month
+            data["year"] = year
+            data["full"] = f"{day}/{month}/{year}"
+            return data
+        except Exception as e:
+            if self.debug: print(f'Lỗi [getBirth]: {e}')
+            return data
 
-    def get_email(self, first_name=None, last_name=None, username_custom=None, domain=None):
-        if not first_name and not last_name: first_name, last_name = self.get_name()
-        if not domain: domain = random.choice(['gmail.com', 'yahoo.com', 'outlook.com', 'hotmail.com'])
-
-        first_name = unidecode.unidecode(first_name).replace(" ", "").lower()
-        last_name = unidecode.unidecode(last_name).replace(" ", "").lower()
-        fname, lname = first_name, last_name
-
-        if not username_custom:
-            random_string = random.choice(string.ascii_lowercase) + ''.join(random.choices(string.ascii_lowercase + string.digits + '_', k=random.randint(5, 11)))
-            if random.choice([True, False]): fname, lname = last_name, first_name
-            position = random.choice(['before', 'middle', 'after'])
-            if position == 'before':  email = f"{random_string}{fname}{lname}"
-            elif position == 'middle': email = f"{fname}{random_string}{lname}"
-            elif position == 'after': email = f"{fname}{lname}{random_string}"
-            return f"{email}@{domain}"
-
-        elif username_custom:
-            parts = username_custom.split('*')
-            email = ''
-            for part in parts:
-                if part == '':
-                    num_random_chars = 1
-                    random_string = random.choice(string.ascii_lowercase) + ''.join(
-                    random.choices(string.ascii_lowercase + string.digits + '_', k=num_random_chars - 1))
-                    email += random_string
-                else:
-                    email += part
-            return f"{email}@{domain}"
+    def getEmail(self, first_name=None, last_name=None, username_custom=None, domain=None):
+        data = {"email": None}
+        try:
+            if not first_name and not last_name: first_name, last_name = self.get_name()
+            if not domain: domain = random.choice(['gmail.com', 'yahoo.com', 'outlook.com', 'hotmail.com'])
+
+            first_name = unidecode.unidecode(first_name).replace(" ", "").lower()
+            last_name = unidecode.unidecode(last_name).replace(" ", "").lower()
+            fname, lname = first_name, last_name
+
+            if not username_custom:
+                random_string = random.choice(string.ascii_lowercase) + ''.join(random.choices(string.ascii_lowercase + string.digits + '_', k=random.randint(5, 11)))
+                if random.choice([True, False]): fname, lname = last_name, first_name
+                position = random.choice(['before', 'middle', 'after'])
+                if position == 'before':  email = f"{random_string}{fname}{lname}"
+                elif position == 'middle': email = f"{fname}{random_string}{lname}"
+                elif position == 'after': email = f"{fname}{lname}{random_string}"
+                data["email"] = f"{email}@{domain}"
+                return data
+
+            elif username_custom:
+                parts = username_custom.split('*')
+                email = ''
+                for part in parts:
+                    if part == '':
+                        num_random_chars = 1
+                        random_string = random.choice(string.ascii_lowercase) + ''.join(
+                        random.choices(string.ascii_lowercase + string.digits + '_', k=num_random_chars - 1))
+                        email += random_string
+                    else:
+                        email += part
+                data["email"] = f"{email}@{domain}"
+                return data
+        except Exception as e:
+            if self.debug: print(f'Lỗi [getEmail]: {e}')
+            return data
 
-    def get_password(self, password_space=(12, 18), password_custom=None):
+    def getPassword(self, password_space=(12, 18), password_custom=None):
+        data = {"password": None}
         min, max = password_space
-        if not password_custom:
-            all_chars = string.ascii_letters + string.digits
-            return ''.join(random.choice(all_chars) for _ in range(random.randint(min, max)))
-        elif password_custom:
-            psw = ''
-            parts = password_custom.split('*')
-            for part in parts:
-                if part == '':
-                    num_random_chars = 1
-                    random_string = ''.join(random.choices(string.ascii_letters + string.digits, k=num_random_chars))
-                    psw += random_string
-                else:
-                    psw += part
-            return psw
-        else:
-            return "annesayhi"
 
-    def get_ua(self, platform='auto'):
+        try:
+            if not password_custom:
+                all_chars = string.ascii_letters + string.digits
+                psw = ''.join(random.choice(all_chars) for _ in range(random.randint(min, max)))
+                data["password"] = psw
+                return data
+
+            elif password_custom:
+                psw = ''
+                parts = password_custom.split('*')
+                for part in parts:
+                    if part == '':
+                        num_random_chars = 1
+                        random_string = ''.join(random.choices(string.ascii_letters + string.digits, k=num_random_chars))
+                        psw += random_string
+                    else:
+                        psw += part
+                data["password"] = psw
+                return data
+            else:
+                data["password"] = 'Anne'
+        except Exception as e:
+            if self.debug: print(f'Lỗi [getPassword]: {e}')
+            return data
+
+    def getUserAgent(self, platform='auto'):
         _platform = ['auto', 'android', 'ios', 'win', 'mac', 'linux']
-        if platform not in _platform: raise ValueError(f"Không hỗ trợ platform: {platform}\nPlatforms được hỗ trợ: {_platform}")
-        if platform in _platform:
-            if platform == 'auto': return self.faker.user_agent()
-            uas = os.path.join(self.current_dir, 'data', f'ua_{platform}.txt')
-            with open(uas, 'r', encoding='utf-8') as f: user_agents = f.readlines()
-            return random.choice(user_agents).strip()
+        if platform not in _platform: raise ValueError(f"Không hỗ trợ platform: {platform}")
+        data = {"user_agent": None}
+        try:
+            if platform in _platform:
+                if platform == 'auto': return self.faker.user_agent()
+                uas = os.path.join(self.current_dir, 'data', f'ua_{platform}.txt')
+                with open(uas, 'r', encoding='utf-8') as f: user_agents = f.readlines()
+                ua = random.choice(user_agents).strip()
+                data["user_agent"] = ua
+                return data
+        except Exception as e:
+            if self.debug: print(f'Lỗi [getUserAgent]: {e}')
+            return data
 
-    def get_info(self,
+    def getInfo(self,
                 day_space=(1, 28),
                 month_space=(1, 12),
                 year_space=(1960, 2004),
                 username_custom=None,
                 password_custom=None,
                 password_space=(12, 18),
                 domain=None,
                 platform='auto'
-
-                      ):
+                ):
 
         data = {
             "name": {
-                "first": "",
-                "last": "",
-                "full": ""
+                "first": None,
+                "last": None,
+                "full": None
             },
             "birth": {
-                "day": "",
-                "month": "",
-                "year": "",
-                "full": ""
+                "day": None,
+                "month": None,
+                "year": None,
+                "full": None
             },
-            "email": "",
-            "password": "",
-            "user_agent": ""
+            "email": None,
+            "password": None,
+            "user_agent": None
         }
 
+        try:
+            name_data = self.getName()
+            birth_data = self.getBirth(day_space, month_space, year_space)
+
+            # Name
+            data["name"]["first"] = name_data["first_name"]
+            data["name"]["last"] = name_data["last_name"]
+
+            if self.country == 'vn': data["name"]["full"] = f"{name_data['last_name']} {name_data['first_name']}"
+            elif self.country == 'us': data["name"]["full"] = f"{name_data['first_name']} {name_data['last_name']}"
+
+            # Birth
+            data["birth"]["day"] = birth_data["day"]
+            data["birth"]["month"] = birth_data["month"]
+            data["birth"]["year"] = birth_data["year"]
+            data["birth"]["full"] = birth_data["full"]
 
-        name_data = self.get_name()
-        birth_data = self.get_birth(day_space, month_space, year_space)
-
-        # Name
-        data["name"]["first"] = name_data["first_name"]
-        data["name"]["last"] = name_data["last_name"]
-
-        if self.country == 'vn': data["name"]["full"] = f"{name_data['last_name']} {name_data['first_name']}"
-        elif self.country == 'us': data["name"]["full"] = f"{name_data['first_name']} {name_data['last_name']}"
-
-        # Birth
-        data["birth"]["day"] = birth_data["day"]
-        data["birth"]["month"] = birth_data["month"]
-        data["birth"]["year"] = birth_data["year"]
-        data["birth"]["full"] = birth_data["full"]
-
-        # Email
-        data["email"] = self.get_email(name_data["first_name"], name_data["last_name"], username_custom, domain)
-
-        # Password
-        data["password"] = self.get_password(password_space, password_custom)
-
-        # User Agent
-        data["user_agent"] = self.get_ua(platform)
-
-        return data
+            # Email
+            data["email"] = self.getEmail(name_data["first_name"], name_data["last_name"], username_custom, domain)
 
+            # Password
+            data["password"] = self.getPassword(password_space, password_custom)
 
+            # User Agent
+            data["user_agent"] = self.getUserAgent(platform)
 
+            return data
 
+        except Exception as e:
+            if self.debug: print(f'Lỗi [getInfo]: {e}')
+            return data
```

### Comparing `anne-1.1.2/app/anne/proxy/AnneProxy.py` & `anne-1.1.3/app/anne/proxy/AnneProxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,91 +2,83 @@
 from .utils import *
 
 class AnneProxy:
     def __init__(self, debug=False):
         self.debug = debug
 
     def format(self, proxy) -> tuple:
-        proxy = str(proxy).strip()
-        pattern = re.compile(
-            r'(?:(?P<user>[^:@|]+):(?P<pass>[^:@|]+)[:@|])?'
-            r'(?P<host>[^:@|/]+)'
-            r'[:@|](?P<port>\d+)'
-            r'(?:[:@|](?P<user2>[^:@|]+):(?P<pass2>[^:@|]+))?'
-            r'|'
-            r'(?:(?P<user3>[^:@|]+):(?P<pass3>[^:@|]+)@)?'
-            r'(?P<host2>[^:@|/]+)'
-            r'@(?P<port2>\d+)'
-            r'|'
-            r'(?P<host3>[^:@|/]+)@(?P<port3>\d+)'
-        )
-        match = pattern.match(proxy)
-        if match:
-            user = match.group('user') or match.group('user2') or match.group('user3')
-            passw = match.group('pass') or match.group('pass2') or match.group('pass3')
-            host = match.group('host') or match.group('host2') or match.group('host3')
-            port = match.group('port') or match.group('port2') or match.group('port3')
-            return host, port, user, passw
-        else:
+        try:
+            proxy = str(proxy).strip()
+            pattern = re.compile(
+                r'(?:(?P<user>[^:@|]+):(?P<pass>[^:@|]+)[:@|])?'
+                r'(?P<host>[^:@|/]+)'
+                r'[:@|](?P<port>\d+)'
+                r'(?:[:@|](?P<user2>[^:@|]+):(?P<pass2>[^:@|]+))?'
+                r'|'
+                r'(?:(?P<user3>[^:@|]+):(?P<pass3>[^:@|]+)@)?'
+                r'(?P<host2>[^:@|/]+)'
+                r'@(?P<port2>\d+)'
+                r'|'
+                r'(?P<host3>[^:@|/]+)@(?P<port3>\d+)'
+            )
+            match = pattern.match(proxy)
+            if match:
+                user = match.group('user') or match.group('user2') or match.group('user3')
+                passw = match.group('pass') or match.group('pass2') or match.group('pass3')
+                host = match.group('host') or match.group('host2') or match.group('host3')
+                port = match.group('port') or match.group('port2') or match.group('port3')
+                return host, port, user, passw
+            else:
+                return None, None, None, None
+        except Exception as e:
+            if self.debug: print(f"Lỗi [format]: {e}")
             return None, None, None, None
 
-    def tmproxy(self,
-                api_key=None,
-                mode='get_proxy',
-                timeout=60):
+    def tmproxy(self, api_key=None, mode='get_proxy', timeout=60):
+        try:
 
-        if not api_key: print('Vui lòng đặt api key'); return False
+            if not api_key: print('Vui lòng đặt api key'); return False
 
-        api_url = "https://tmproxy.com/api/proxy"
+            api_url = "https://tmproxy.com/api/proxy"
 
-        if mode == 'get_proxy':
-            try:
+            if mode == 'get_proxy':
                 url = f"{api_url}/get-new-proxy"
                 payload = {"api_key": api_key}
                 headers = {"Content-Type": "application/json"}
                 proxy_https = None
                 start_time = time.time()
                 while not proxy_https:
                     if time.time() - start_time > timeout: break
                     response = requests.post(url, json=payload, headers=headers)
                     if not response.status_code == 200: return None
                     data = response.json()
                     proxy_https = data['data'].get('https')
                     if not proxy_https: time.sleep(1); continue
                     return None
                 return proxy_https
-            except Exception as e:
-                if self.debug: print(f"Lỗi: {e}")
-                return False
 
-        elif mode == 'check-key':
-            try:
+            elif mode == 'check-key':
                 url = f"{api_url}/stats"
-
                 payload = {"api_key": api_key}
-
                 response = requests.post(url, json=payload)
                 if not response.status_code == 200: return False
                 if response.json()['message'] == 'API không tồn tại': return False
                 return True
-            except Exception as e:
-                if self.debug: print(f"Lỗi: {e}")
-                return False
-
-    def tinsoftproxy(self,
-                     api_key=None,
-                     mode='get_proxy',
-                     timeout=60):
 
-        if not api_key:
-            print('Vui lòng đặt api key')
+            else: print(f'Không hỗ trợ mode: {mode}'); return False
+
+        except Exception as e:
+            if self.debug: print(f"Lỗi [tmproxy]: {e}")
             return False
 
-        if mode == 'get_proxy':
-            try:
+    def tinsoftproxy(self, api_key=None, mode='get_proxy', timeout=60):
+        try:
+            if not api_key: print('Vui lòng đặt api key'); return False
+
+            if mode == 'get_proxy':
                 start_time = time.time()
                 while True:
                     if time.time() - start_time > timeout:
                         break
                     try:
                         response = requests.get(f"http://proxy.tinsoftsv.com/api/changeProxy.php?key={api_key}")
                         if not response.status_code == 200: return None
@@ -95,48 +87,51 @@
                         else:
                             if 'next_change' in data:
                                 wait_time = int(data['next_change']) + 1
                                 time.sleep(wait_time)
                             else: return None
                     except requests.exceptions.RequestException:
                         time.sleep(10)
-            except Exception as e:
-                if self.debug: print(f"Lỗi: {e}"); return False
 
-        elif mode == 'check-key':
-            try:
-                response = requests.get(f"http://proxy.tinsoftsv.com/api/getKeyInfo.php?key={api_key}")
-                if not response.status_code == 200: return False
-                if response.json()['success']: return True
-                else: return False
-            except Exception as e:
-                if self.debug: print(f"Lỗi: {e}"); return False
-
-    def wwproxy(self,
-                api_key=None,
-                mode='get_proxy',
-                timeout=60):
+            elif mode == 'check-key':
+                try:
+                    response = requests.get(f"http://proxy.tinsoftsv.com/api/getKeyInfo.php?key={api_key}")
+                    if not response.status_code == 200: return False
+                    if response.json()['success']: return True
+                    else: return False
+                except Exception as e:
+                    if self.debug: print(f"Lỗi: {e}"); return False
+
+            else: print(f'Không hỗ trợ mode: {mode}'); return False
+
+        except Exception as e:
+            if self.debug: print(f"Lỗi [tinsoftproxy]: {e}")
+
+    def wwproxy(self, api_key=None, mode='get_proxy', timeout=60):
+        try:
 
-        if not api_key: print('Vui lòng đặt api key'); return False
+            if not api_key: print('Vui lòng đặt api key'); return False
 
-        if mode == 'get_proxy':
-            try:
+            if mode == 'get_proxy':
                 start_time = time.time()
                 while True:
                     if time.time() - start_time > timeout: break
                     response = requests.get(f"https://wwproxy.com/api/client/proxy/available?key={api_key}&provinceId=-1")
                     if not response.status_code == 200: return None
                     if response.json()['status'] == 'OK': return response.json()['data']['proxy']
                     time.sleep(1)
                 return None
-            except Exception as e:
-                if self.debug: print(f"Lỗi: {e}"); return False
 
-        elif mode == 'check-key': print('Chưa hỗ trợ chức năng này'); return False
+            elif mode == 'check-key': print('Chưa hỗ trợ chức năng này'); return False
 
+            else: print(f'Không hỗ trợ mode: {mode}'); return False
+
+        except Exception as e:
+            if self.debug: print(f"Lỗi [wwproxy]: {e}")
+            return False
```

### Comparing `anne-1.1.2/app/anne.egg-info/PKG-INFO` & `anne-1.1.3/app/anne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.1.2
+Version: 1.1.3
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.1.2/setup.py` & `anne-1.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="anne",
-    version="1.1.2",
+    version="1.1.3",
     description="Lib for lazy dev",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrship666/anne-lib",
     author="AnneHouman",
```

