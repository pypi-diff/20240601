# Comparing `tmp/export_to_telegraph-0.0.98.tar.gz` & `tmp/export_to_telegraph-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/export_to_telegraph-0.0.98.tar", last modified: Sat Dec 26 20:18:55 2020, max compression
+gzip compressed data, was "dist/export_to_telegraph-0.0.99.tar", last modified: Sat Dec 26 20:19:30 2020, max compression
```

## Comparing `export_to_telegraph-0.0.98.tar` & `export_to_telegraph-0.0.99.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-12-26 20:18:55.897316 export_to_telegraph-0.0.98/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      931 2020-12-26 20:18:55.896893 export_to_telegraph-0.0.98/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      318 2019-10-22 13:59:01.000000 export_to_telegraph-0.0.98/README.md
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-12-26 20:18:55.893909 export_to_telegraph-0.0.98/export_to_telegraph/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     4375 2020-08-13 16:51:40.000000 export_to_telegraph-0.0.98/export_to_telegraph/__init__.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     2645 2020-12-26 20:18:49.000000 export_to_telegraph-0.0.98/export_to_telegraph/article.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     2325 2020-08-07 01:08:31.000000 export_to_telegraph-0.0.98/export_to_telegraph/author.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      337 2020-12-18 12:26:27.000000 export_to_telegraph-0.0.98/export_to_telegraph/common.py
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1657 2020-12-26 18:09:10.000000 export_to_telegraph-0.0.98/export_to_telegraph/title.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-12-26 20:18:55.896324 export_to_telegraph-0.0.98/export_to_telegraph.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      931 2020-12-26 20:18:55.000000 export_to_telegraph-0.0.98/export_to_telegraph.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      384 2020-12-26 20:18:55.000000 export_to_telegraph-0.0.98/export_to_telegraph.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-12-26 20:18:55.000000 export_to_telegraph-0.0.98/export_to_telegraph.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      117 2020-12-26 20:18:55.000000 export_to_telegraph-0.0.98/export_to_telegraph.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       20 2020-12-26 20:18:55.000000 export_to_telegraph-0.0.98/export_to_telegraph.egg-info/top_level.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-12-26 20:18:55.897442 export_to_telegraph-0.0.98/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      909 2020-12-26 20:18:53.000000 export_to_telegraph-0.0.98/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-12-26 20:19:30.984436 export_to_telegraph-0.0.99/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      931 2020-12-26 20:19:30.984095 export_to_telegraph-0.0.99/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      318 2019-10-22 13:59:01.000000 export_to_telegraph-0.0.99/README.md
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-12-26 20:19:30.981519 export_to_telegraph-0.0.99/export_to_telegraph/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     4375 2020-08-13 16:51:40.000000 export_to_telegraph-0.0.99/export_to_telegraph/__init__.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     2644 2020-12-26 20:19:26.000000 export_to_telegraph-0.0.99/export_to_telegraph/article.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     2325 2020-08-07 01:08:31.000000 export_to_telegraph-0.0.99/export_to_telegraph/author.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      337 2020-12-18 12:26:27.000000 export_to_telegraph-0.0.99/export_to_telegraph/common.py
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1657 2020-12-26 18:09:10.000000 export_to_telegraph-0.0.99/export_to_telegraph/title.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-12-26 20:19:30.983610 export_to_telegraph-0.0.99/export_to_telegraph.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      931 2020-12-26 20:19:30.000000 export_to_telegraph-0.0.99/export_to_telegraph.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      384 2020-12-26 20:19:30.000000 export_to_telegraph-0.0.99/export_to_telegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-12-26 20:19:30.000000 export_to_telegraph-0.0.99/export_to_telegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      117 2020-12-26 20:19:30.000000 export_to_telegraph-0.0.99/export_to_telegraph.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       20 2020-12-26 20:19:30.000000 export_to_telegraph-0.0.99/export_to_telegraph.egg-info/top_level.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-12-26 20:19:30.984547 export_to_telegraph-0.0.99/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      909 2020-12-26 20:19:28.000000 export_to_telegraph-0.0.99/setup.py
```

### Comparing `export_to_telegraph-0.0.98/PKG-INFO` & `export_to_telegraph-0.0.99/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export_to_telegraph
-Version: 0.0.98
+Version: 0.0.99
 Summary: Library for export webpage to Telegraph.
 Home-page: https://github.com/gaoyunzhi/export_to_telegraph
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # export_to_telegraph
```

### Comparing `export_to_telegraph-0.0.98/export_to_telegraph/__init__.py` & `export_to_telegraph-0.0.99/export_to_telegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `export_to_telegraph-0.0.98/export_to_telegraph/article.py` & `export_to_telegraph-0.0.99/export_to_telegraph/article.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 			new_url = 'https://card.weibo.com/article/m/aj/detail?id=' + wid + '&_t=' + str(int(time.time()))
 			json = yaml.load(cached_url.get(new_url, 
 				headers={'referer': url}, force_cache = force_cache), Loader=yaml.FullLoader)
 			return '<div><title>%s</title>%s</div>' % (json['data']['title'], json['data']['content'])
 		return getContentFromAlbum(weibo_2_album.get(url))
 	return cached_url.get(url, force_cache=force_cache)
 
-def getTitle(url, force_cache=True, toSimplified = Falses):
+def getTitle(url, force_cache=True, toSimplified = False):
 	try:
 		content = getContent(url, force_cache=force_cache)
 		soup = BeautifulSoup(_trimWebpage(content), 'html.parser')
 		doc = Document(content)
 		title =  _findTitle(soup, doc)
 		if toSimplified:
 			return cc.convert(title)
```

### Comparing `export_to_telegraph-0.0.98/export_to_telegraph/author.py` & `export_to_telegraph-0.0.99/export_to_telegraph/author.py`

 * *Files identical despite different names*

### Comparing `export_to_telegraph-0.0.98/export_to_telegraph/title.py` & `export_to_telegraph-0.0.99/export_to_telegraph/title.py`

 * *Files identical despite different names*

### Comparing `export_to_telegraph-0.0.98/export_to_telegraph.egg-info/PKG-INFO` & `export_to_telegraph-0.0.99/export_to_telegraph.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export-to-telegraph
-Version: 0.0.98
+Version: 0.0.99
 Summary: Library for export webpage to Telegraph.
 Home-page: https://github.com/gaoyunzhi/export_to_telegraph
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # export_to_telegraph
```

### Comparing `export_to_telegraph-0.0.98/setup.py` & `export_to_telegraph-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="export_to_telegraph",
-    version="0.0.98",
+    version="0.0.99",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Library for export webpage to Telegraph.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/export_to_telegraph",
     packages=setuptools.find_packages(),
```

