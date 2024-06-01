# Comparing `tmp/blockmango-1.4.8.tar.gz` & `tmp/blockmango-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.4.8.tar", last modified: Fri May 31 21:20:42 2024, max compression
+gzip compressed data, was "blockmango-1.4.9.tar", last modified: Fri May 31 21:31:41 2024, max compression
```

## Comparing `blockmango-1.4.8.tar` & `blockmango-1.4.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:20:42.706502 blockmango-1.4.8/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.8/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-31 21:20:42.706502 blockmango-1.4.8/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      571 2024-05-28 23:52:58.000000 blockmango-1.4.8/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:20:42.682502 blockmango-1.4.8/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.8/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     4610 2024-05-31 21:16:46.000000 blockmango-1.4.8/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)      690 2024-05-31 21:17:43.000000 blockmango-1.4.8/blockmango/config.py
--rw-------   0 userland  (2000) userland  (2000)     1325 2024-05-31 21:14:55.000000 blockmango-1.4.8/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     2443 2024-05-31 21:15:54.000000 blockmango-1.4.8/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-28 20:20:04.000000 blockmango-1.4.8/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.4.8/blockmango/http.py
--rw-------   0 userland  (2000) userland  (2000)     2036 2024-05-31 21:12:48.000000 blockmango-1.4.8/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:20:42.698502 blockmango-1.4.8/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      370 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-31 21:20:42.706502 blockmango-1.4.8/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)     1474 2024-05-31 21:20:14.000000 blockmango-1.4.8/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:31:41.630501 blockmango-1.4.9/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.9/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-31 21:31:41.626501 blockmango-1.4.9/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      571 2024-05-28 23:52:58.000000 blockmango-1.4.9/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:31:41.602501 blockmango-1.4.9/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.9/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     4610 2024-05-31 21:16:46.000000 blockmango-1.4.9/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)      690 2024-05-31 21:17:43.000000 blockmango-1.4.9/blockmango/config.py
+-rw-------   0 userland  (2000) userland  (2000)     1325 2024-05-31 21:14:55.000000 blockmango-1.4.9/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     2486 2024-05-31 21:30:27.000000 blockmango-1.4.9/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-28 20:20:04.000000 blockmango-1.4.9/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.4.9/blockmango/http.py
+-rw-------   0 userland  (2000) userland  (2000)     2036 2024-05-31 21:12:48.000000 blockmango-1.4.9/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:31:41.622501 blockmango-1.4.9/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      370 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-31 21:31:41.000000 blockmango-1.4.9/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-31 21:31:41.630501 blockmango-1.4.9/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)     1474 2024-05-31 21:31:34.000000 blockmango-1.4.9/setup.py
```

### Comparing `blockmango-1.4.8/LICENSE.md` & `blockmango-1.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.8/PKG-INFO` & `blockmango-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockmango
-Version: 1.4.8
+Version: 1.4.9
 Summary: Blockman Go API package
 Home-page: https://github.com/darkkpy/blockmango
 Author: Dark
 Author-email: darkness0777@proton.me
 License: MIT
 Project-URL: Documentation, https://github.com/darkkpy/blockmango/tree/main/docs
 Project-URL: Source, https://github.com/darkkpy/blockmango
```

### Comparing `blockmango-1.4.8/README.md` & `blockmango-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.8/blockmango/clan.py` & `blockmango-1.4.9/blockmango/clan.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.8/blockmango/config.py` & `blockmango-1.4.9/blockmango/config.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.8/blockmango/decoration.py` & `blockmango-1.4.9/blockmango/decoration.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.8/blockmango/friends.py` & `blockmango-1.4.9/blockmango/friends.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     def delete_friend(self, friend_id):
         return self._delete(f"{self.base_url_friend}/friends", headers=self.headers, params={"friendId": friend_id})
 
     def request(self, friend_id, msg):
         payload = {"friendId": friend_id, "msg": msg, "type": 1}
         headers = {"Content-Type": "application/json", **self.headers}
-        return self._post(f"{self.base_url_friend}/friends", headers=headers, json=payload)
+        return self._post(f"{self.base_url_friend}/friends", headers=headers, json_data=payload)  # Pass 'json_data' instead of 'json'
 
     def popularity(self, friend_id):
         return self._get(f"{self.base_url_friend}/popularity/{friend_id}", headers=self.headers)
 
     def info(self, friend_id):
         return self._get(f"{self.base_url_friend}/friends/{friend_id}", headers=self.headers)
```

### Comparing `blockmango-1.4.8/blockmango/groupchat.py` & `blockmango-1.4.9/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.8/blockmango/http.py` & `blockmango-1.4.9/blockmango/http.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.8/blockmango/user.py` & `blockmango-1.4.9/blockmango/user.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.8/blockmango.egg-info/PKG-INFO` & `blockmango-1.4.9/blockmango.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockmango
-Version: 1.4.8
+Version: 1.4.9
 Summary: Blockman Go API package
 Home-page: https://github.com/darkkpy/blockmango
 Author: Dark
 Author-email: darkness0777@proton.me
 License: MIT
 Project-URL: Documentation, https://github.com/darkkpy/blockmango/tree/main/docs
 Project-URL: Source, https://github.com/darkkpy/blockmango
```

### Comparing `blockmango-1.4.8/setup.py` & `blockmango-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open(filename, "r", encoding="utf-8") as file:
         return file.read() + "\n\n"
 
 long_description = read_md_file("README.md")
 
 setup(
     name='blockmango',
-    version='1.4.8',
+    version='1.4.9',
     author='Dark',
     author_email='darkness0777@proton.me',
     description='Blockman Go API package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/darkkpy/blockmango',
     packages=['blockmango'],
```

