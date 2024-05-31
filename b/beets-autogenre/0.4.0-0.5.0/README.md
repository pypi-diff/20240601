# Comparing `tmp/beets_autogenre-0.4.0-py3-none-any.whl.zip` & `tmp/beets_autogenre-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12576 bytes, number of entries: 9
--rw-r--r--  2.0 unx       75 b- defN 24-May-07 02:10 beetsplug/__init__.py
--rw-r--r--  2.0 unx    15630 b- defN 24-May-07 02:10 beetsplug/autogenre/__init__.py
--rw-r--r--  2.0 unx      225 b- defN 24-May-07 02:10 beetsplug/autogenre/config_default.yaml
--rw-r--r--  2.0 unx     2077 b- defN 24-May-07 02:10 beetsplug/autogenre/genretree.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5509 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      776 b- defN 24-May-07 02:11 beets_autogenre-0.4.0.dist-info/RECORD
-9 files, 35751 bytes uncompressed, 11226 bytes compressed:  68.6%
+Zip file size: 12660 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       75 b- defN 24-May-31 23:39 beetsplug/__init__.py
+-rw-r--r--  2.0 unx    15839 b- defN 24-May-31 23:39 beetsplug/autogenre/__init__.py
+-rw-r--r--  2.0 unx      237 b- defN 24-May-31 23:39 beetsplug/autogenre/config_default.yaml
+-rw-r--r--  2.0 unx     2077 b- defN 24-May-31 23:39 beetsplug/autogenre/genretree.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-31 23:43 beets_autogenre-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-31 23:43 beets_autogenre-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 23:43 beets_autogenre-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-31 23:43 beets_autogenre-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      776 b- defN 24-May-31 23:43 beets_autogenre-0.5.0.dist-info/RECORD
+9 files, 35972 bytes uncompressed, 11310 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: beetsplug/autogenre/config_default.yaml
 Comment: 
 
 Filename: beetsplug/autogenre/genretree.py
 Comment: 
 
-Filename: beets_autogenre-0.4.0.dist-info/LICENSE
+Filename: beets_autogenre-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: beets_autogenre-0.4.0.dist-info/METADATA
+Filename: beets_autogenre-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: beets_autogenre-0.4.0.dist-info/WHEEL
+Filename: beets_autogenre-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: beets_autogenre-0.4.0.dist-info/top_level.txt
+Filename: beets_autogenre-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: beets_autogenre-0.4.0.dist-info/RECORD
+Filename: beets_autogenre-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beetsplug/autogenre/__init__.py

```diff
@@ -55,15 +55,17 @@
         assert _is_plugin_enabled('xtractor'), "The 'xtractor' plugin is not enabled!"
         self._lastgenre = LastGenrePlugin()
         self._xtractor = XtractorCommand(config['xtractor'])
         self._lastgenre_conf = config['lastgenre'].get() or {}
         self._separator = self._lastgenre_conf.get('separator') or ', '
         self._remix_regex = re.compile(r'.+[^\w](remix|bootleg|remake)', re.IGNORECASE)
         self._genre_tree = None
-        # TODO: add auto-detect support
+        # TODO: fix auto support - fix genres field mapping, see https://github.com/beetbox/mediafile/blob/master/mediafile.py#L1814
+        if self.config['auto'].get(bool):
+            self.import_stages = [self.imported]
 
     def imported(self, session, task):
         """Event hook called when an import task finishes."""
         if task.is_album:
             for item in task.album.items():
                 self._update_item_genre(item)
 
@@ -76,15 +78,16 @@
         self._log.info("Set track genre '{}' ({}): {}", genre, source, item)
         item.genre = genre
         item.genres = genres
         item.genre_source = source
         if not self.config['pretend'].get():
             if config['import']['write'].get():
                 item.try_write()
-            item.store(['genre', 'genres', 'genre_source'])
+            item.store(['genre'])
+            item.store(['genres', 'genre_source'])
 
     def _update_album_genre(self, album):
         genre = _most_common([item.genre for item in album.items()])
         if album.genre != genre and genre:
             album.genre = genre
             self._log.info("Set genre '{}' for album {}", album.genre, album)
             if not self.config['pretend'].get():
```

## beetsplug/autogenre/config_default.yaml

```diff
@@ -1,7 +1,8 @@
+auto: false
 pretend: false
 all: false
 force: false
 lastgenre: true
 xtractor: true
 from_title: true
 parent_genres: true
```

## Comparing `beets_autogenre-0.4.0.dist-info/LICENSE` & `beets_autogenre-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beets_autogenre-0.4.0.dist-info/METADATA` & `beets_autogenre-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-autogenre
-Version: 0.4.0
+Version: 0.5.0
 Summary: Detect the genres for each song within your beets library
 Home-page: https://github.com/mgoltzsche/beets-autogenre
 Author: Max Goltzsche
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `beets_autogenre-0.4.0.dist-info/RECORD` & `beets_autogenre-0.5.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 beetsplug/__init__.py,sha256=QDJyS5jtJnGFsSuOx43ZvLBCOrHImm8NrZk5f9URWdk,75
-beetsplug/autogenre/__init__.py,sha256=i4TSzSxK8QwijnaQJI_vRaZ5sakjqcj6Vj-iHHa_puo,15630
-beetsplug/autogenre/config_default.yaml,sha256=HSQ1D1PIyFtGNOi6DEVT5tFQlmtTvvB9RnnQffQBToA,225
+beetsplug/autogenre/__init__.py,sha256=Hh7-PXypQk1JbVeWHSspZVvHguyAmlWmjXBom1liVZQ,15839
+beetsplug/autogenre/config_default.yaml,sha256=jnuAIfFEqTY6zjvNxAwj1he_BYO85bGPi2SKyHPulkI,237
 beetsplug/autogenre/genretree.py,sha256=a4ghZNDaPuV7qMAK_shwrQAqTNfsbdL4GwMFd3GTtLc,2077
-beets_autogenre-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-beets_autogenre-0.4.0.dist-info/METADATA,sha256=ai_1R5rAfo4NuPGIO_YUsLcaJ8mgMQYTmayjJVtTYic,5509
-beets_autogenre-0.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-beets_autogenre-0.4.0.dist-info/top_level.txt,sha256=za8u6CXAGbgac8cUyn9NlsgXqqq-_4HHZcNmJnfmyWc,10
-beets_autogenre-0.4.0.dist-info/RECORD,,
+beets_autogenre-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+beets_autogenre-0.5.0.dist-info/METADATA,sha256=DG-DhloMcPFYfXsarD8PsE8qDdsbnVT8Q2WcCC_8KM8,5509
+beets_autogenre-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+beets_autogenre-0.5.0.dist-info/top_level.txt,sha256=za8u6CXAGbgac8cUyn9NlsgXqqq-_4HHZcNmJnfmyWc,10
+beets_autogenre-0.5.0.dist-info/RECORD,,
```

