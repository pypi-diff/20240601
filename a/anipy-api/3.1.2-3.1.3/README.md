# Comparing `tmp/anipy_api-3.1.2.tar.gz` & `tmp/anipy_api-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_api-3.1.2.tar", max compression
+gzip compressed data, was "anipy_api-3.1.3.tar", max compression
```

## Comparing `anipy_api-3.1.2.tar` & `anipy_api-3.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      227 2024-05-30 12:07:29.289708 anipy_api-3.1.2/README.md
--rw-r--r--   0        0        0      825 2024-05-30 12:07:29.289708 anipy_api-3.1.2/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/__init__.py
--rw-r--r--   0        0        0     5493 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/anime.py
--rw-r--r--   0        0        0    11550 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/download.py
--rw-r--r--   0        0        0     2765 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/error.py
--rw-r--r--   0        0        0     8130 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/locallist.py
--rw-r--r--   0        0        0    20790 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/mal.py
--rw-r--r--   0        0        0      132 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/__init__.py
--rw-r--r--   0        0        0     5499 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/base.py
--rw-r--r--   0        0        0     1692 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/player.py
--rw-r--r--   0        0        0      267 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/__init__.py
--rw-r--r--   0        0        0     1147 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/mpv.py
--rw-r--r--   0        0        0     2651 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/mpv_control.py
--rw-r--r--   0        0        0      941 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/syncplay.py
--rw-r--r--   0        0        0      918 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/vlc.py
--rw-r--r--   0        0        0      628 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/__init__.py
--rw-r--r--   0        0        0     5321 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/base.py
--rw-r--r--   0        0        0     3397 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/filter.py
--rw-r--r--   0        0        0     1543 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/provider.py
--rw-r--r--   0        0        0      183 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/providers/__init__.py
--rw-r--r--   0        0        0    12198 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/providers/gogo_provider.py
--rw-r--r--   0        0        0     8596 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/providers/yugen_provider.py
--rw-r--r--   0        0        0      896 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/utils.py
--rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 anipy_api-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-06-01 13:03:33.405826 anipy_api-3.1.3/README.md
+-rw-r--r--   0        0        0      825 2024-06-01 13:03:33.405826 anipy_api-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/__init__.py
+-rw-r--r--   0        0        0     5493 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/anime.py
+-rw-r--r--   0        0        0    11550 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/download.py
+-rw-r--r--   0        0        0     2765 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/error.py
+-rw-r--r--   0        0        0     8130 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/locallist.py
+-rw-r--r--   0        0        0    20790 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/mal.py
+-rw-r--r--   0        0        0      132 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/player/__init__.py
+-rw-r--r--   0        0        0     5499 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/player/base.py
+-rw-r--r--   0        0        0     1692 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/player/player.py
+-rw-r--r--   0        0        0      267 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/player/players/__init__.py
+-rw-r--r--   0        0        0     1147 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/player/players/mpv.py
+-rw-r--r--   0        0        0     2649 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/player/players/mpv_control.py
+-rw-r--r--   0        0        0      941 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/player/players/syncplay.py
+-rw-r--r--   0        0        0      918 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/player/players/vlc.py
+-rw-r--r--   0        0        0      628 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/provider/__init__.py
+-rw-r--r--   0        0        0     5321 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/provider/base.py
+-rw-r--r--   0        0        0     3397 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/provider/filter.py
+-rw-r--r--   0        0        0     1543 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/provider/provider.py
+-rw-r--r--   0        0        0      183 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/provider/providers/__init__.py
+-rw-r--r--   0        0        0    12198 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/provider/providers/gogo_provider.py
+-rw-r--r--   0        0        0     8596 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/provider/providers/yugen_provider.py
+-rw-r--r--   0        0        0      896 2024-06-01 13:03:33.405826 anipy_api-3.1.3/src/anipy_api/provider/utils.py
+-rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 anipy_api-3.1.3/PKG-INFO
```

### Comparing `anipy_api-3.1.2/pyproject.toml` & `anipy_api-3.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-api"
-version = "3.1.2"
+version = "3.1.3"
 description = "api for anipy-cli"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-api"
 keywords = ["anime", "api"]
```

### Comparing `anipy_api-3.1.2/src/anipy_api/anime.py` & `anipy_api-3.1.3/src/anipy_api/anime.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/download.py` & `anipy_api-3.1.3/src/anipy_api/download.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/error.py` & `anipy_api-3.1.3/src/anipy_api/error.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/locallist.py` & `anipy_api-3.1.3/src/anipy_api/locallist.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/mal.py` & `anipy_api-3.1.3/src/anipy_api/mal.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/player/base.py` & `anipy_api-3.1.3/src/anipy_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/player/player.py` & `anipy_api-3.1.3/src/anipy_api/player/player.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/player/players/mpv.py` & `anipy_api-3.1.3/src/anipy_api/player/players/mpv.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/player/players/mpv_control.py` & `anipy_api-3.1.3/src/anipy_api/player/players/mpv_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         if len(mpv_args) <= 1:
             mpv_args = {
                 "input_default_bindings": True,
                 "input_vo_keyboard": True,
                 "force_window": "immediate",
                 "title": "MPV - Receiving Links from anipy-cli",
-                "osc": "True",
+                "osc": True,
             }
 
         self.mpv = MPV(**mpv_args)
 
     def play_title(self, anime: "Anime", stream: "ProviderStream"):
         self.mpv.force_media_title = self._get_media_title(anime, stream)
```

### Comparing `anipy_api-3.1.2/src/anipy_api/player/players/syncplay.py` & `anipy_api-3.1.3/src/anipy_api/player/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/player/players/vlc.py` & `anipy_api-3.1.3/src/anipy_api/player/players/vlc.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/provider/__init__.py` & `anipy_api-3.1.3/src/anipy_api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/provider/base.py` & `anipy_api-3.1.3/src/anipy_api/provider/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/provider/filter.py` & `anipy_api-3.1.3/src/anipy_api/provider/filter.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/provider/provider.py` & `anipy_api-3.1.3/src/anipy_api/provider/provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/provider/providers/gogo_provider.py` & `anipy_api-3.1.3/src/anipy_api/provider/providers/gogo_provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/provider/providers/yugen_provider.py` & `anipy_api-3.1.3/src/anipy_api/provider/providers/yugen_provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/src/anipy_api/provider/utils.py` & `anipy_api-3.1.3/src/anipy_api/provider/utils.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.2/PKG-INFO` & `anipy_api-3.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-api
-Version: 3.1.2
+Version: 3.1.3
 Summary: api for anipy-cli
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,api
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
```

