# Comparing `tmp/moroccan_prayer_times-0.0.10-py3-none-any.whl.zip` & `tmp/moroccan_prayer_times-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7560 bytes, number of entries: 8
+Zip file size: 7514 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 24-Jun-01 15:11 src/__init__.py
--rw-r--r--  2.0 unx    14272 b- defN 24-Jun-01 17:52 src/main.py
--rw-r--r--  2.0 unx     1072 b- defN 24-Jun-01 17:59 moroccan_prayer_times-0.0.10.dist-info/LICENSE
--rw-r--r--  2.0 unx     3225 b- defN 24-Jun-01 17:59 moroccan_prayer_times-0.0.10.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 17:59 moroccan_prayer_times-0.0.10.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 24-Jun-01 17:59 moroccan_prayer_times-0.0.10.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Jun-01 17:59 moroccan_prayer_times-0.0.10.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      708 b- defN 24-Jun-01 17:59 moroccan_prayer_times-0.0.10.dist-info/RECORD
-8 files, 19418 bytes uncompressed, 6300 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx    14201 b- defN 24-Jun-01 16:01 src/main.py
+-rw-r--r--  2.0 unx     1072 b- defN 24-Jun-01 16:08 moroccan_prayer_times-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3224 b- defN 24-Jun-01 16:08 moroccan_prayer_times-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 16:08 moroccan_prayer_times-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 24-Jun-01 16:08 moroccan_prayer_times-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Jun-01 16:08 moroccan_prayer_times-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      702 b- defN 24-Jun-01 16:08 moroccan_prayer_times-0.0.9.dist-info/RECORD
+8 files, 19340 bytes uncompressed, 6266 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: src/__init__.py
 Comment: 
 
 Filename: src/main.py
 Comment: 
 
-Filename: moroccan_prayer_times-0.0.10.dist-info/LICENSE
+Filename: moroccan_prayer_times-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: moroccan_prayer_times-0.0.10.dist-info/METADATA
+Filename: moroccan_prayer_times-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: moroccan_prayer_times-0.0.10.dist-info/WHEEL
+Filename: moroccan_prayer_times-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: moroccan_prayer_times-0.0.10.dist-info/entry_points.txt
+Filename: moroccan_prayer_times-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: moroccan_prayer_times-0.0.10.dist-info/top_level.txt
+Filename: moroccan_prayer_times-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: moroccan_prayer_times-0.0.10.dist-info/RECORD
+Filename: moroccan_prayer_times-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/main.py

```diff
@@ -38,18 +38,15 @@
 
 
 def locale():
     """Get user locale from config file. Fallback is 'en'"""
     return config.get(SECTION_NAME, "locale", fallback=DEFAULT_LOCALE)
 
 
-# Needed for PyI18n
-os.chdir(Path(os.path.realpath(__file__)).parent)
-
-i18n = PyI18n(available_locales=("ar", "en", "fr"), load_path="translations/")
+i18n = PyI18n(available_locales=("ar", "en", "fr"), load_path="src/translations/")
 _: Callable = i18n.gettext
 
 app = typer.Typer(help=APP_NAME, add_help_option=False, add_completion=False)
 
 
 def _flush():
     """Save the current config in the dedicated file"""
@@ -333,15 +330,15 @@
         for index, prayer_time in enumerate(prayer_times.values()):
             prayer_hour, prayer_minute = map(int, prayer_time.split(":"))
             if prayer_hour == current_hour and prayer_minute == current_minute:
                 is_now = True
                 next_prayer_index = index
                 break
             elif prayer_hour > current_hour or (
-                    prayer_hour == current_hour and prayer_minute > current_minute
+                prayer_hour == current_hour and prayer_minute > current_minute
             ):
                 next_prayer_time_string = f"{prayer_hour:02}:{prayer_minute:02}"
                 next_prayer_index = index
                 break
 
         if is_now:
             prayer_name_in_locale = _(
```

## Comparing `moroccan_prayer_times-0.0.10.dist-info/LICENSE` & `moroccan_prayer_times-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `moroccan_prayer_times-0.0.10.dist-info/METADATA` & `moroccan_prayer_times-0.0.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moroccan_prayer_times
-Version: 0.0.10
+Version: 0.0.9
 Summary: Moroccan Prayer Times CLI
 Home-page: https://github.com/ismailbenhallam/prayer-times-cli/
 Author: Ismail BENHALLAM
 Author-email: ismailben44@gmail.com
 Keywords: prayer times,prayer_times,prayer,morocco
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

