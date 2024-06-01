# Comparing `tmp/python3_commons-0.5.6.tar.gz` & `tmp/python3_commons-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_commons-0.5.6.tar", last modified: Wed May 29 23:20:41 2024, max compression
+gzip compressed data, was "python3_commons-0.5.7.tar", last modified: Sat Jun  1 06:29:35 2024, max compression
```

## Comparing `python3_commons-0.5.6.tar` & `python3_commons-0.5.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.148436 python3_commons-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 23:20:31.000000 python3_commons-0.5.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.140436 python3_commons-0.5.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.144436 python3_commons-0.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-29 23:20:31.000000 python3_commons-0.5.6/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 23:20:31.000000 python3_commons-0.5.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 23:20:31.000000 python3_commons-0.5.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-29 23:20:31.000000 python3_commons-0.5.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-05-29 23:20:31.000000 python3_commons-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 23:20:41.148436 python3_commons-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 23:20:31.000000 python3_commons-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 23:20:31.000000 python3_commons-0.5.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.144436 python3_commons-0.5.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 23:20:31.000000 python3_commons-0.5.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.144436 python3_commons-0.5.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 23:20:31.000000 python3_commons-0.5.6/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 23:20:31.000000 python3_commons-0.5.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 23:20:31.000000 python3_commons-0.5.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-05-29 23:20:31.000000 python3_commons-0.5.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-29 23:20:31.000000 python3_commons-0.5.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 23:20:31.000000 python3_commons-0.5.6/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 23:20:31.000000 python3_commons-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 23:20:31.000000 python3_commons-0.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 23:20:31.000000 python3_commons-0.5.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 23:20:31.000000 python3_commons-0.5.6/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-29 23:20:41.148436 python3_commons-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 23:20:31.000000 python3_commons-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.140436 python3_commons-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.144436 python3_commons-0.5.6/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.144436 python3_commons-0.5.6/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.148436 python3_commons-0.5.6/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 23:20:31.000000 python3_commons-0.5.6/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.148436 python3_commons-0.5.6/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 23:20:41.000000 python3_commons-0.5.6/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 23:20:41.000000 python3_commons-0.5.6/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 23:20:41.000000 python3_commons-0.5.6/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 23:20:41.000000 python3_commons-0.5.6/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 23:20:41.000000 python3_commons-0.5.6/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 23:20:41.000000 python3_commons-0.5.6/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:20:41.148436 python3_commons-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 23:20:31.000000 python3_commons-0.5.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-29 23:20:31.000000 python3_commons-0.5.6/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-29 23:20:31.000000 python3_commons-0.5.6/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.627537 python3_commons-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 06:29:28.000000 python3_commons-0.5.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.615537 python3_commons-0.5.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.619537 python3_commons-0.5.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-06-01 06:29:28.000000 python3_commons-0.5.7/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 06:29:28.000000 python3_commons-0.5.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 06:29:28.000000 python3_commons-0.5.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 06:29:28.000000 python3_commons-0.5.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-06-01 06:29:28.000000 python3_commons-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 06:29:35.627537 python3_commons-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 06:29:28.000000 python3_commons-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 06:29:28.000000 python3_commons-0.5.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 06:29:28.000000 python3_commons-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-01 06:29:28.000000 python3_commons-0.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 06:29:28.000000 python3_commons-0.5.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 06:29:28.000000 python3_commons-0.5.7/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-06-01 06:29:35.627537 python3_commons-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-01 06:29:28.000000 python3_commons-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.619537 python3_commons-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.627537 python3_commons-0.5.7/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.627537 python3_commons-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 06:29:28.000000 python3_commons-0.5.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-06-01 06:29:28.000000 python3_commons-0.5.7/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 06:29:28.000000 python3_commons-0.5.7/tests/test_msgspec.py
```

### Comparing `python3_commons-0.5.6/.coveragerc` & `python3_commons-0.5.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/.github/workflows/python-publish.yaml` & `python3_commons-0.5.7/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/.gitignore` & `python3_commons-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/LICENSE` & `python3_commons-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/PKG-INFO` & `python3_commons-0.5.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.6
+Version: 0.5.7
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.6/docs/Makefile` & `python3_commons-0.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/docs/conf.py` & `python3_commons-0.5.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/docs/index.rst` & `python3_commons-0.5.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/setup.cfg` & `python3_commons-0.5.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.5.6
+version = 0.5.7
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
```

### Comparing `python3_commons-0.5.6/src/python3_commons/audit.py` & `python3_commons-0.5.7/src/python3_commons/audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     now = datetime.now(tz=UTC) - timedelta(days=1)
     year = now.year
     month = now.month
     day = now.day
     bucket_name = s3_settings.s3_bucket
     fo = BytesIO()
     object_names = []
-    date_path = object_storage.get_absolute_path(f'{root_path}/{year}/{month:02}/{day:02}')
+    date_path = f'{root_path}/{year}/{month:02}/{day:02}'
 
     with tarfile.open(fileobj=fo, mode='w|bz2') as archive:
         if objects := object_storage.get_objects(bucket_name, date_path, recursive=True):
             logger.info(f'Compacting files in: {date_path}')
 
             for name, last_modified, content in objects:
                 info = tarfile.TarInfo(name)
```

### Comparing `python3_commons-0.5.6/src/python3_commons/conf.py` & `python3_commons-0.5.7/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/src/python3_commons/db.py` & `python3_commons-0.5.7/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/src/python3_commons/helpers.py` & `python3_commons-0.5.7/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/src/python3_commons/logging/formatter.py` & `python3_commons-0.5.7/src/python3_commons/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/src/python3_commons/object_storage.py` & `python3_commons-0.5.7/src/python3_commons/object_storage.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/src/python3_commons/serializers/json.py` & `python3_commons-0.5.7/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/src/python3_commons/serializers/msgpack.py` & `python3_commons-0.5.7/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/src/python3_commons/serializers/msgspec.py` & `python3_commons-0.5.7/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/src/python3_commons.egg-info/PKG-INFO` & `python3_commons-0.5.7/src/python3_commons.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.6
+Version: 0.5.7
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.6/src/python3_commons.egg-info/SOURCES.txt` & `python3_commons-0.5.7/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/tests/conftest.py` & `python3_commons-0.5.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/tests/test_msgpack.py` & `python3_commons-0.5.7/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.6/tests/test_msgspec.py` & `python3_commons-0.5.7/tests/test_msgspec.py`

 * *Files identical despite different names*

