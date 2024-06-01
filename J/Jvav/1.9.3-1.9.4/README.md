# Comparing `tmp/Jvav-1.9.3.tar.gz` & `tmp/Jvav-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-zkxb_j_j/Jvav-1.9.3.tar", last modified: Fri May 31 16:50:52 2024, max compression
+gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-zai3ga1g/Jvav-1.9.4.tar", last modified: Sat Jun  1 03:02:18 2024, max compression
```

## Comparing `Jvav-1.9.3.tar` & `Jvav-1.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-31 16:50:52.000000 Jvav-1.9.3/
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)      295 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/SOURCES.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/dependency_links.txt
--rw-r--r--   0 zh         (501) staff       (20)       39 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/entry_points.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.3/Jvav.egg-info/not-zip-safe
--rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/requires.txt
--rw-r--r--   0 zh         (501) staff       (20)       11 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/top_level.txt
--rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.3/LICENSE
--rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.3/MANIFEST.in
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-05-31 16:50:52.000000 Jvav-1.9.3/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.3/README.md
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-31 16:50:52.000000 Jvav-1.9.3/jvav/
--rw-r--r--   0 zh         (501) staff       (20)      481 2024-05-31 16:50:21.000000 Jvav-1.9.3/jvav/__init__.py
--rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.3/jvav/cmd.py
--rw-r--r--   0 zh         (501) staff       (20)    76532 2024-05-31 16:49:02.000000 Jvav-1.9.3/jvav/utils.py
--rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:49:11.000000 Jvav-1.9.3/requirements.txt
--rw-r--r--   0 zh         (501) staff       (20)       38 2024-05-31 16:50:52.000000 Jvav-1.9.3/setup.cfg
--rw-r--r--   0 zh         (501) staff       (20)     1345 2024-05-31 16:50:22.000000 Jvav-1.9.3/setup.py
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-01 03:02:18.000000 Jvav-1.9.4/
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-01 03:02:18.000000 Jvav-1.9.4/Jvav.egg-info/
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-06-01 03:02:18.000000 Jvav-1.9.4/Jvav.egg-info/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)      295 2024-06-01 03:02:18.000000 Jvav-1.9.4/Jvav.egg-info/SOURCES.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2024-06-01 03:02:18.000000 Jvav-1.9.4/Jvav.egg-info/dependency_links.txt
+-rw-r--r--   0 zh         (501) staff       (20)       39 2024-06-01 03:02:18.000000 Jvav-1.9.4/Jvav.egg-info/entry_points.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.4/Jvav.egg-info/not-zip-safe
+-rw-r--r--   0 zh         (501) staff       (20)      579 2024-06-01 03:02:18.000000 Jvav-1.9.4/Jvav.egg-info/requires.txt
+-rw-r--r--   0 zh         (501) staff       (20)       11 2024-06-01 03:02:18.000000 Jvav-1.9.4/Jvav.egg-info/top_level.txt
+-rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.4/LICENSE
+-rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.4/MANIFEST.in
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-06-01 03:02:18.000000 Jvav-1.9.4/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.4/README.md
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-01 03:02:18.000000 Jvav-1.9.4/jvav/
+-rw-r--r--   0 zh         (501) staff       (20)      481 2024-06-01 03:01:21.000000 Jvav-1.9.4/jvav/__init__.py
+-rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.4/jvav/cmd.py
+-rw-r--r--   0 zh         (501) staff       (20)    76664 2024-06-01 02:59:52.000000 Jvav-1.9.4/jvav/utils.py
+-rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:49:11.000000 Jvav-1.9.4/requirements.txt
+-rw-r--r--   0 zh         (501) staff       (20)       38 2024-06-01 03:02:18.000000 Jvav-1.9.4/setup.cfg
+-rw-r--r--   0 zh         (501) staff       (20)     1345 2024-06-01 03:01:21.000000 Jvav-1.9.4/setup.py
```

### Comparing `Jvav-1.9.3/Jvav.egg-info/PKG-INFO` & `Jvav-1.9.4/Jvav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.3
+Version: 1.9.4
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.3 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.4 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.3/Jvav.egg-info/requires.txt` & `Jvav-1.9.4/Jvav.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.3/LICENSE` & `Jvav-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.3/PKG-INFO` & `Jvav-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.3
+Version: 1.9.4
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.3 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.4 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.3/README.md` & `Jvav-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.3/jvav/cmd.py` & `Jvav-1.9.4/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.3/jvav/utils.py` & `Jvav-1.9.4/jvav/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,29 +232,31 @@
             if not url:
                 return 404, None
             return 200, f"{self.BASE_URL}{url}"
         except Exception as e:
             self.log.error(f"JavDbUtil: 获取预览图片: {e}")
             return 404, None
 
-    def fuzzy_search_stars(self, text) -> typing.Tuple[int, list]:
+    def fuzzy_search_stars(self, text) -> typing.Tuple[int, any]:
         """模糊搜索演员
 
         :param str text: 演员名称
         :return typing.Tuple[int, list]: 状态码和演员列表
         """
         code, resp = self.send_req(url=JavDbUtil.BASE_URL_SEARCH_STAR + text)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             actor_boxs = soup.find_all(class_="actor-box")
             names = [box.find("a")["title"] for box in actor_boxs]
             if not names:
                 return 404, None
+            names = [name.split(',')[0] for name in names]
+            names = list(set(names))
             return 200, names
         except Exception as e:
             self.log.error(f"JavDbUtil: 模糊搜索演员: {e}")
             return 404, None
 
     def get_id_by_star_name(self, star_name: str, page=-1) -> typing.Tuple[int, str]:
         """根据演员名称获取一个番号
@@ -1434,14 +1436,15 @@
             return code, None
         try:
             soup = self.get_soup(resp)
             actor_boxs = soup.find_all(class_="avatar-box text-center")
             names = [box.find("img")["title"] for box in actor_boxs]
             if not names:
                 return 404, None
+            names = list(set(names))
             return 200, names
         except Exception as e:
             self.log.error(f"JavDbUtil: 模糊搜索演员: {e}")
             return 404, None
 
     def get_av_by_id(
             self,
```

### Comparing `Jvav-1.9.3/requirements.txt` & `Jvav-1.9.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.3/setup.py` & `Jvav-1.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="Jvav",
-    version="1.9.3",
+    version="1.9.4",
     description="Useful tools for Jav.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/akynazh/jvav",
     download_url="https://github.com/akynazh/jvav/releases/latest",
     author="akynazh",
     author_email="akynazh@gmail.com",
```

