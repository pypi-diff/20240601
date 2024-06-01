# Comparing `tmp/metalarchivist-0.5.4.tar.gz` & `tmp/metalarchivist-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.5.4.tar", last modified: Fri May 31 12:46:14 2024, max compression
+gzip compressed data, was "metalarchivist-0.5.5.tar", last modified: Fri May 31 13:41:53 2024, max compression
```

## Comparing `metalarchivist-0.5.4.tar` & `metalarchivist-0.5.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.707263 metalarchivist-0.5.4/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 12:46:14.707263 metalarchivist-0.5.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 12:46:14.707263 metalarchivist-0.5.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.700263 metalarchivist-0.5.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.701263 metalarchivist-0.5.4/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)     3601 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.703263 metalarchivist-0.5.4/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3585 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.703263 metalarchivist-0.5.4/src/metalarchivist/export/data/
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/data/user-agents.json
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/label.py
--rwxrwxrwx   0 root         (0) root         (0)     7272 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.705263 metalarchivist-0.5.4/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)     1437 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9478 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/album.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.705263 metalarchivist-0.5.4/src/metalarchivist/interface/api/
--rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/api/page.py
--rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/label.py
--rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/theme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.707263 metalarchivist-0.5.4/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1001 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.706263 metalarchivist-0.5.4/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10359 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     4073 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     6166 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_labels.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.747459 metalarchivist-0.5.5/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 13:41:53.746459 metalarchivist-0.5.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 13:41:53.747459 metalarchivist-0.5.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.739459 metalarchivist-0.5.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.740459 metalarchivist-0.5.5/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)     3601 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.742459 metalarchivist-0.5.5/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3585 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.743459 metalarchivist-0.5.5/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7272 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.744459 metalarchivist-0.5.5/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1437 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9489 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.745459 metalarchivist-0.5.5/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/metalarchivist/interface/theme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.746459 metalarchivist-0.5.5/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 13:41:53.000000 metalarchivist-0.5.5/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-31 13:41:53.000000 metalarchivist-0.5.5/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 13:41:53.000000 metalarchivist-0.5.5/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-31 13:41:53.000000 metalarchivist-0.5.5/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-31 13:41:53.000000 metalarchivist-0.5.5/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:41:53.746459 metalarchivist-0.5.5/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10793 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     4073 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     6166 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-31 13:41:40.000000 metalarchivist-0.5.5/src/test/test_themes.py
```

### Comparing `metalarchivist-0.5.4/LICENSE` & `metalarchivist-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/PKG-INFO` & `metalarchivist-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.5.4
+Version: 0.5.5
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.5.4/pyproject.toml` & `metalarchivist-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.5.4"
+version = "0.5.5"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.5.4/src/metalarchivist/__init__.py` & `metalarchivist-0.5.5/src/metalarchivist/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/export/album.py` & `metalarchivist-0.5.5/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/export/band.py` & `metalarchivist-0.5.5/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/export/data/user-agents.json` & `metalarchivist-0.5.5/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/export/genre.py` & `metalarchivist-0.5.5/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/export/label.py` & `metalarchivist-0.5.5/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/export/util.py` & `metalarchivist-0.5.5/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.5.5/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/interface/album.py` & `metalarchivist-0.5.5/src/metalarchivist/interface/album.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     return release_date_parsed
 
 
 class AlbumXPath:
     LABEL_LINK = '//div[@id="album_info"]/dl/dt[text()="Label:"]/following-sibling::dd[1]/a'
     NAME = './/h1[contains(@class, "album_name")]/a/text()'
-    BAND_LINK = './/h2[@class="band_name"]/a'
+    BAND_LINK = './/h2[contains(@class, "band_name")]/a'
     DESCRIPTION_TITLES = '//div[@id="album_info"]/dl/dt/text()'
     DESCRIPTION_DETAILS = '//div[@id="album_info"]/dl/dd/text()'
     TRACKLIST = '//div[@id="album_tabs_tracklist"]//tr[@class="even" or @class="odd"]'
 
 
 @dataclass
 class AlbumLink:
```

### Comparing `metalarchivist-0.5.4/src/metalarchivist/interface/api/base.py` & `metalarchivist-0.5.5/src/metalarchivist/interface/api/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/interface/api/page.py` & `metalarchivist-0.5.5/src/metalarchivist/interface/api/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/interface/band.py` & `metalarchivist-0.5.5/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/interface/genre.py` & `metalarchivist-0.5.5/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/interface/label.py` & `metalarchivist-0.5.5/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist/interface/theme.py` & `metalarchivist-0.5.5/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.5.5/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.5.4
+Version: 0.5.5
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.5.4/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.5.5/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/test/test_albums.py` & `metalarchivist-0.5.5/src/test/test_albums.py`

 * *Files 3% similar despite different names*

```diff
@@ -245,21 +245,27 @@
         self.assertIsNotNone(album)
 
         album_json = album.to_dict()
         album_band_link = album_json['band']
 
         self.assertIn('band_key', album_band_link)
 
+    def test_album_profile_name(self):
         album = self.export.Album.get_profile('https://www.metal-archives.com/albums/Kawir/%CE%9A%CF%85%CE%B4%CE%BF%CE%B9%CE%BC%CE%BF%CF%83/1216552')
         self.assertIsNotNone(album.name)
 
+    def test_album_profile_tracklist(self):
         album = self.export.Album.get_profile('https://www.metal-archives.com/albums/Aamonblut/Black_Candle_Majesty/1239703')
         self.assertIsNotNone(album.tracklist[0].number)
         self.assertEqual(album.tracklist[0].number, '1')
 
+    def test_album_profile_band_link(self):
+        album = self.export.Album.get_profile('https://www.metal-archives.com/albums/%CE%A3%CF%84%CE%B1%CE%BC%CE%AC%CF%84%CE%B7%CF%82_%CE%99%CF%89%CE%AC%CE%BD%CE%BD%CE%BF%CF%85/Avalon_%28Hercules_Cover%29/1225997')
+        self.assertIsNotNone(album.band.name)
+        self.assertIsNotNone(album.band.link)
 
     def test_track_lyrics(self):
         track_lyrics = self.export.Album.get_track_lyrics('7299894')
         self.assertIsNotNone(track_lyrics.text)
 
 
     # def test_album_themes(self):
```

### Comparing `metalarchivist-0.5.4/src/test/test_bands.py` & `metalarchivist-0.5.5/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/test/test_genres.py` & `metalarchivist-0.5.5/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/test/test_labels.py` & `metalarchivist-0.5.5/src/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.4/src/test/test_themes.py` & `metalarchivist-0.5.5/src/test/test_themes.py`

 * *Files identical despite different names*

