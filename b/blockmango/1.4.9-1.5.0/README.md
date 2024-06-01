# Comparing `tmp/blockmango-1.4.9.tar.gz` & `tmp/blockmango-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.4.9.tar", last modified: Fri May 31 21:31:41 2024, max compression
+gzip compressed data, was "blockmango-1.5.0.tar", last modified: Sat Jun  1 07:53:12 2024, max compression
```

## Comparing `blockmango-1.4.9.tar` & `blockmango-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:31:41.630501 blockmango-1.4.9/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.9/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-31 21:31:41.626501 blockmango-1.4.9/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      571 2024-05-28 23:52:58.000000 blockmango-1.4.9/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:31:41.602501 blockmango-1.4.9/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.9/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     4610 2024-05-31 21:16:46.000000 blockmango-1.4.9/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)      690 2024-05-31 21:17:43.000000 blockmango-1.4.9/blockmango/config.py
--rw-------   0 userland  (2000) userland  (2000)     1325 2024-05-31 21:14:55.000000 blockmango-1.4.9/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     2486 2024-05-31 21:30:27.000000 blockmango-1.4.9/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-28 20:20:04.000000 blockmango-1.4.9/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.4.9/blockmango/http.py
--rw-------   0 userland  (2000) userland  (2000)     2036 2024-05-31 21:12:48.000000 blockmango-1.4.9/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:31:41.622501 blockmango-1.4.9/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      370 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-31 21:31:41.630501 blockmango-1.4.9/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)     1474 2024-05-31 21:31:34.000000 blockmango-1.4.9/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-06-01 07:53:12.971431 blockmango-1.5.0/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.5.0/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)     1703 2024-06-01 07:53:12.971431 blockmango-1.5.0/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      571 2024-05-28 23:52:58.000000 blockmango-1.5.0/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-06-01 07:53:12.955432 blockmango-1.5.0/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.5.0/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     4631 2024-06-01 07:43:34.000000 blockmango-1.5.0/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)      690 2024-05-31 21:17:43.000000 blockmango-1.5.0/blockmango/config.py
+-rw-------   0 userland  (2000) userland  (2000)     1346 2024-06-01 07:44:35.000000 blockmango-1.5.0/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     2507 2024-06-01 07:46:51.000000 blockmango-1.5.0/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     3541 2024-06-01 07:48:30.000000 blockmango-1.5.0/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.5.0/blockmango/http.py
+-rw-------   0 userland  (2000) userland  (2000)     2057 2024-06-01 07:49:27.000000 blockmango-1.5.0/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-06-01 07:53:12.967431 blockmango-1.5.0/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)     1703 2024-06-01 07:53:10.000000 blockmango-1.5.0/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      370 2024-06-01 07:53:10.000000 blockmango-1.5.0/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-06-01 07:53:10.000000 blockmango-1.5.0/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-06-01 07:53:10.000000 blockmango-1.5.0/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-06-01 07:53:10.000000 blockmango-1.5.0/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-06-01 07:53:12.971431 blockmango-1.5.0/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)     1474 2024-06-01 07:52:40.000000 blockmango-1.5.0/setup.py
```

### Comparing `blockmango-1.4.9/LICENSE.md` & `blockmango-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.9/PKG-INFO` & `blockmango-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockmango
-Version: 1.4.9
+Version: 1.5.0
 Summary: Blockman Go API package
 Home-page: https://github.com/darkkpy/blockmango
 Author: Dark
 Author-email: darkness0777@proton.me
 License: MIT
 Project-URL: Documentation, https://github.com/darkkpy/blockmango/tree/main/docs
 Project-URL: Source, https://github.com/darkkpy/blockmango
```

### Comparing `blockmango-1.4.9/README.md` & `blockmango-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.9/blockmango/clan.py` & `blockmango-1.5.0/blockmango/clan.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class Clan(HTTPMixin):
     __slots__ = ("headers",)
     base_url_clan = BASE_URL_CLAN
     base_url_clan_v2 = BASE_URL_CLAN_V2
     base_url_clan_v3 = BASE_URL_CLAN_V3
 
     def __init__(self, user_id, access_token):
-        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
+        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1", "language": "en_US"}
 
     def user_clan(self):
         return self._get(f"{self.base_url_clan}/tribe/base", headers=self.headers)
 
     def join(self, clan_id):
         return self._post(f"{self.base_url_clan}/tribe/member", headers=self.headers, json={"clanId": clan_id, "msg": ""})
```

### Comparing `blockmango-1.4.9/blockmango/config.py` & `blockmango-1.5.0/blockmango/config.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.9/blockmango/decoration.py` & `blockmango-1.5.0/blockmango/decoration.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .config import BASE_URL_DECORATION, BASE_URL_SHOP
 
 class Decoration(HTTPMixin):
     __slots__ = ("headers",)
     base_url = BASE_URL_DECORATION
 
     def __init__(self, user_id, access_token):
-        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
+        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1", "language": "en_US"}
 
     def skins(self, uid):
         params = {"engineVersion": "10105", "os": "android", "showVip": 1}
         return self._get(f"{self.base_url}/new/decorations/users/{uid}/classify/all", headers=self.headers, params=params)
 
     def current_price(self, skin_id, is_suit):
         payload = [{"id": skin_id, "isSuit": is_suit}]
```

### Comparing `blockmango-1.4.9/blockmango/friends.py` & `blockmango-1.5.0/blockmango/friends.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class Friends(HTTPMixin):
     __slots__ = ("headers",)
     base_url_friend = BASE_URL_FRIEND
     base_url_decoration = BASE_URL_DECORATION
 
     def __init__(self, user_id, access_token):
-        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
+        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1", "language": "en_US"}
 
     def delete_friend(self, friend_id):
         return self._delete(f"{self.base_url_friend}/friends", headers=self.headers, params={"friendId": friend_id})
 
     def request(self, friend_id, msg):
         payload = {"friendId": friend_id, "msg": msg, "type": 1}
         headers = {"Content-Type": "application/json", **self.headers}
```

### Comparing `blockmango-1.4.9/blockmango/groupchat.py` & `blockmango-1.5.0/blockmango/groupchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_URL_GROUP_V2 = "http://modsgs.sandboxol.com/msg/api/v2"
 
 
 class Group(HTTPMixin):
   __slots__ = ("headers",)
 
   def __init__(self, user_id, access_token):
-    self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
+    self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1", "language": "en_US" }
 
   def create(self, member_ids):
     endpoint = f"{BASE_URL_GROUP_V2}/msg/group/chat"
     json_data = { "cost": 0, "currency": 1, "memberIds": member_ids, "userId": self.headers["userId"] }
     return self._post(endpoint, headers=self.headers, json_data=json_data)
 
   def allow_invite(self, group_id, group_name, invite_status):
```

### Comparing `blockmango-1.4.9/blockmango/http.py` & `blockmango-1.5.0/blockmango/http.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.9/blockmango/user.py` & `blockmango-1.5.0/blockmango/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .config import BASE_URL_USER, BASE_URL_ROUTE, BASE_URL_USER_INFO
 
 class User(HTTPMixin):
     __slots__ = ("headers",)
     base_url = BASE_URL_USER
 
     def __init__(self, user_id, access_token):
-        self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
+        self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1", "language": "en_US" }
 
     def get_user_info(self):
         return self._get(f"{self.base_url}/v2/user/details/info", headers=self.headers)
 
     def set_birthday(self, birthday):
         return self._put(f"{BASE_URL_USER}/user/info", headers=self.headers, json_data={"birthday": birthday})
```

### Comparing `blockmango-1.4.9/blockmango.egg-info/PKG-INFO` & `blockmango-1.5.0/blockmango.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockmango
-Version: 1.4.9
+Version: 1.5.0
 Summary: Blockman Go API package
 Home-page: https://github.com/darkkpy/blockmango
 Author: Dark
 Author-email: darkness0777@proton.me
 License: MIT
 Project-URL: Documentation, https://github.com/darkkpy/blockmango/tree/main/docs
 Project-URL: Source, https://github.com/darkkpy/blockmango
```

### Comparing `blockmango-1.4.9/setup.py` & `blockmango-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open(filename, "r", encoding="utf-8") as file:
         return file.read() + "\n\n"
 
 long_description = read_md_file("README.md")
 
 setup(
     name='blockmango',
-    version='1.4.9',
+    version='1.5.0',
     author='Dark',
     author_email='darkness0777@proton.me',
     description='Blockman Go API package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/darkkpy/blockmango',
     packages=['blockmango'],
```

