# Comparing `tmp/airtable_scraper-0.0.2.tar.gz` & `tmp/airtable_scraper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtable_scraper-0.0.2.tar", last modified: Sat Jun  1 01:11:05 2024, max compression
+gzip compressed data, was "airtable_scraper-0.0.3.tar", last modified: Sat Jun  1 01:20:12 2024, max compression
```

## Comparing `airtable_scraper-0.0.2.tar` & `airtable_scraper-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kangchen   (502) staff       (20)        0 2024-06-01 01:11:05.544356 airtable_scraper-0.0.2/
--rw-r--r--   0 kangchen   (502) staff       (20)     1065 2024-03-26 01:56:57.000000 airtable_scraper-0.0.2/LICENSE
--rw-r--r--   0 kangchen   (502) staff       (20)     4232 2024-06-01 01:11:05.544129 airtable_scraper-0.0.2/PKG-INFO
--rw-r--r--   0 kangchen   (502) staff       (20)     2334 2024-05-31 22:39:25.000000 airtable_scraper-0.0.2/README.md
--rw-r--r--   0 kangchen   (502) staff       (20)      762 2024-06-01 01:10:54.000000 airtable_scraper-0.0.2/pyproject.toml
--rw-r--r--   0 kangchen   (502) staff       (20)       38 2024-06-01 01:11:05.544398 airtable_scraper-0.0.2/setup.cfg
-drwxr-xr-x   0 kangchen   (502) staff       (20)        0 2024-06-01 01:11:05.539848 airtable_scraper-0.0.2/src/
-drwxr-xr-x   0 kangchen   (502) staff       (20)        0 2024-06-01 01:11:05.542443 airtable_scraper-0.0.2/src/airtable_scraper/
--rw-r--r--   0 kangchen   (502) staff       (20)       46 2024-03-13 09:43:11.000000 airtable_scraper-0.0.2/src/airtable_scraper/__init__.py
--rw-r--r--   0 kangchen   (502) staff       (20)      273 2024-03-13 09:46:08.000000 airtable_scraper-0.0.2/src/airtable_scraper/_logger_config.py
--rw-r--r--   0 kangchen   (502) staff       (20)     1928 2024-03-23 06:52:59.000000 airtable_scraper-0.0.2/src/airtable_scraper/_models.py
--rw-r--r--   0 kangchen   (502) staff       (20)    26436 2024-06-01 01:03:07.000000 airtable_scraper-0.0.2/src/airtable_scraper/airtable_scraper.py
--rw-r--r--   0 kangchen   (502) staff       (20)     5699 2024-03-23 08:23:42.000000 airtable_scraper-0.0.2/src/airtable_scraper/table_utils.py
--rw-r--r--   0 kangchen   (502) staff       (20)     2544 2024-03-23 12:27:14.000000 airtable_scraper-0.0.2/src/airtable_scraper/typing.py
-drwxr-xr-x   0 kangchen   (502) staff       (20)        0 2024-06-01 01:11:05.543823 airtable_scraper-0.0.2/src/airtable_scraper.egg-info/
--rw-r--r--   0 kangchen   (502) staff       (20)     4232 2024-06-01 01:11:05.000000 airtable_scraper-0.0.2/src/airtable_scraper.egg-info/PKG-INFO
--rw-r--r--   0 kangchen   (502) staff       (20)      463 2024-06-01 01:11:05.000000 airtable_scraper-0.0.2/src/airtable_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 kangchen   (502) staff       (20)        1 2024-06-01 01:11:05.000000 airtable_scraper-0.0.2/src/airtable_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 kangchen   (502) staff       (20)       30 2024-06-01 01:11:05.000000 airtable_scraper-0.0.2/src/airtable_scraper.egg-info/requires.txt
--rw-r--r--   0 kangchen   (502) staff       (20)       17 2024-06-01 01:11:05.000000 airtable_scraper-0.0.2/src/airtable_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 kangchen   (502) staff       (20)        0 2024-06-01 01:20:12.975076 airtable_scraper-0.0.3/
+-rw-r--r--   0 kangchen   (502) staff       (20)     1065 2024-03-26 01:56:57.000000 airtable_scraper-0.0.3/LICENSE
+-rw-r--r--   0 kangchen   (502) staff       (20)     4232 2024-06-01 01:20:12.974808 airtable_scraper-0.0.3/PKG-INFO
+-rw-r--r--   0 kangchen   (502) staff       (20)     2334 2024-05-31 22:39:25.000000 airtable_scraper-0.0.3/README.md
+-rw-r--r--   0 kangchen   (502) staff       (20)      762 2024-06-01 01:19:19.000000 airtable_scraper-0.0.3/pyproject.toml
+-rw-r--r--   0 kangchen   (502) staff       (20)       38 2024-06-01 01:20:12.975126 airtable_scraper-0.0.3/setup.cfg
+drwxr-xr-x   0 kangchen   (502) staff       (20)        0 2024-06-01 01:20:12.971208 airtable_scraper-0.0.3/src/
+drwxr-xr-x   0 kangchen   (502) staff       (20)        0 2024-06-01 01:20:12.972879 airtable_scraper-0.0.3/src/airtable_scraper/
+-rw-r--r--   0 kangchen   (502) staff       (20)       46 2024-03-13 09:43:11.000000 airtable_scraper-0.0.3/src/airtable_scraper/__init__.py
+-rw-r--r--   0 kangchen   (502) staff       (20)      273 2024-03-13 09:46:08.000000 airtable_scraper-0.0.3/src/airtable_scraper/_logger_config.py
+-rw-r--r--   0 kangchen   (502) staff       (20)     1928 2024-03-23 06:52:59.000000 airtable_scraper-0.0.3/src/airtable_scraper/_models.py
+-rw-r--r--   0 kangchen   (502) staff       (20)    26409 2024-06-01 01:15:24.000000 airtable_scraper-0.0.3/src/airtable_scraper/airtable_scraper.py
+-rw-r--r--   0 kangchen   (502) staff       (20)     5699 2024-03-23 08:23:42.000000 airtable_scraper-0.0.3/src/airtable_scraper/table_utils.py
+-rw-r--r--   0 kangchen   (502) staff       (20)     2544 2024-03-23 12:27:14.000000 airtable_scraper-0.0.3/src/airtable_scraper/typing.py
+drwxr-xr-x   0 kangchen   (502) staff       (20)        0 2024-06-01 01:20:12.974490 airtable_scraper-0.0.3/src/airtable_scraper.egg-info/
+-rw-r--r--   0 kangchen   (502) staff       (20)     4232 2024-06-01 01:20:12.000000 airtable_scraper-0.0.3/src/airtable_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 kangchen   (502) staff       (20)      463 2024-06-01 01:20:12.000000 airtable_scraper-0.0.3/src/airtable_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 kangchen   (502) staff       (20)        1 2024-06-01 01:20:12.000000 airtable_scraper-0.0.3/src/airtable_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 kangchen   (502) staff       (20)       30 2024-06-01 01:20:12.000000 airtable_scraper-0.0.3/src/airtable_scraper.egg-info/requires.txt
+-rw-r--r--   0 kangchen   (502) staff       (20)       17 2024-06-01 01:20:12.000000 airtable_scraper-0.0.3/src/airtable_scraper.egg-info/top_level.txt
```

### Comparing `airtable_scraper-0.0.2/LICENSE` & `airtable_scraper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airtable_scraper-0.0.2/PKG-INFO` & `airtable_scraper-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtable_scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Public airtable web scraper tool
 Author-email: Kang Chen <kangchen.work@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Kang Chen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtable_scraper-0.0.2/README.md` & `airtable_scraper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `airtable_scraper-0.0.2/pyproject.toml` & `airtable_scraper-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtable_scraper"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Kang Chen", email="kangchen.work@gmail.com" },
 ]
 description = "Public airtable web scraper tool"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

### Comparing `airtable_scraper-0.0.2/src/airtable_scraper/_models.py` & `airtable_scraper-0.0.3/src/airtable_scraper/_models.py`

 * *Files identical despite different names*

### Comparing `airtable_scraper-0.0.2/src/airtable_scraper/airtable_scraper.py` & `airtable_scraper-0.0.3/src/airtable_scraper/airtable_scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,14 @@
 
     def _get_new_url(self) -> str | Any:
         """Get the hidden api endpoint to actual airtable data.
 
         Returns:
             str | Any: Api endpoint. None if table not found in http response
         """
-        print(self.__page)
         url_with_params = re.search(r"urlWithParams:\s*\"(.*?)\"", self.__page).group(1)
         if not url_with_params:
             logger.error(f"Could not parse urlWithParams. Failed to scrape table: {self._url}")
             raise
         url_with_params = url_with_params.replace("u002F", "").replace("\\", "/")
         return "https://airtable.com" + url_with_params
```

### Comparing `airtable_scraper-0.0.2/src/airtable_scraper/table_utils.py` & `airtable_scraper-0.0.3/src/airtable_scraper/table_utils.py`

 * *Files identical despite different names*

### Comparing `airtable_scraper-0.0.2/src/airtable_scraper/typing.py` & `airtable_scraper-0.0.3/src/airtable_scraper/typing.py`

 * *Files identical despite different names*

### Comparing `airtable_scraper-0.0.2/src/airtable_scraper.egg-info/PKG-INFO` & `airtable_scraper-0.0.3/src/airtable_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtable_scraper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Public airtable web scraper tool
 Author-email: Kang Chen <kangchen.work@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Kang Chen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

