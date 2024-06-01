# Comparing `tmp/python3_commons-0.5.7.tar.gz` & `tmp/python3_commons-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_commons-0.5.7.tar", last modified: Sat Jun  1 06:29:35 2024, max compression
+gzip compressed data, was "python3_commons-0.5.8.tar", last modified: Sat Jun  1 08:05:18 2024, max compression
```

## Comparing `python3_commons-0.5.7.tar` & `python3_commons-0.5.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.627537 python3_commons-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 06:29:28.000000 python3_commons-0.5.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.615537 python3_commons-0.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.619537 python3_commons-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-06-01 06:29:28.000000 python3_commons-0.5.7/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 06:29:28.000000 python3_commons-0.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 06:29:28.000000 python3_commons-0.5.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 06:29:28.000000 python3_commons-0.5.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-06-01 06:29:28.000000 python3_commons-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 06:29:35.627537 python3_commons-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 06:29:28.000000 python3_commons-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 06:29:28.000000 python3_commons-0.5.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 06:29:28.000000 python3_commons-0.5.7/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 06:29:28.000000 python3_commons-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-01 06:29:28.000000 python3_commons-0.5.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 06:29:28.000000 python3_commons-0.5.7/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 06:29:28.000000 python3_commons-0.5.7/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-06-01 06:29:35.627537 python3_commons-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-01 06:29:28.000000 python3_commons-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.619537 python3_commons-0.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.623537 python3_commons-0.5.7/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-06-01 06:29:28.000000 python3_commons-0.5.7/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.627537 python3_commons-0.5.7/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 06:29:35.000000 python3_commons-0.5.7/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:29:35.627537 python3_commons-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 06:29:28.000000 python3_commons-0.5.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-06-01 06:29:28.000000 python3_commons-0.5.7/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 06:29:28.000000 python3_commons-0.5.7/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 08:05:06.000000 python3_commons-0.5.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.253991 python3_commons-0.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.257991 python3_commons-0.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-06-01 08:05:06.000000 python3_commons-0.5.8/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 08:05:06.000000 python3_commons-0.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 08:05:06.000000 python3_commons-0.5.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 08:05:06.000000 python3_commons-0.5.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-06-01 08:05:06.000000 python3_commons-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 08:05:18.261991 python3_commons-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 08:05:06.000000 python3_commons-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 08:05:06.000000 python3_commons-0.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.257991 python3_commons-0.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.257991 python3_commons-0.5.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 08:05:06.000000 python3_commons-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-01 08:05:06.000000 python3_commons-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 08:05:06.000000 python3_commons-0.5.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 08:05:06.000000 python3_commons-0.5.8/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-06-01 08:05:18.261991 python3_commons-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-01 08:05:06.000000 python3_commons-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.253991 python3_commons-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.257991 python3_commons-0.5.8/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 08:05:06.000000 python3_commons-0.5.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-06-01 08:05:06.000000 python3_commons-0.5.8/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 08:05:06.000000 python3_commons-0.5.8/tests/test_msgspec.py
```

### Comparing `python3_commons-0.5.7/.coveragerc` & `python3_commons-0.5.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/.github/workflows/python-publish.yaml` & `python3_commons-0.5.8/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/.gitignore` & `python3_commons-0.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/LICENSE` & `python3_commons-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/PKG-INFO` & `python3_commons-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.7
+Version: 0.5.8
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.7/docs/Makefile` & `python3_commons-0.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/docs/conf.py` & `python3_commons-0.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/docs/index.rst` & `python3_commons-0.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/setup.cfg` & `python3_commons-0.5.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.5.7
+version = 0.5.8
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
```

### Comparing `python3_commons-0.5.7/src/python3_commons/audit.py` & `python3_commons-0.5.8/src/python3_commons/audit.py`

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
-    date_path = f'{root_path}/{year}/{month:02}/{day:02}'
+    date_path = object_storage.get_absolute_path(f'{root_path}/{year}/{month:02}/{day:02}')
 
     with tarfile.open(fileobj=fo, mode='w|bz2') as archive:
         if objects := object_storage.get_objects(bucket_name, date_path, recursive=True):
             logger.info(f'Compacting files in: {date_path}')
 
             for name, last_modified, content in objects:
                 info = tarfile.TarInfo(name)
```

### Comparing `python3_commons-0.5.7/src/python3_commons/conf.py` & `python3_commons-0.5.8/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/src/python3_commons/db.py` & `python3_commons-0.5.8/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/src/python3_commons/helpers.py` & `python3_commons-0.5.8/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/src/python3_commons/logging/formatter.py` & `python3_commons-0.5.8/src/python3_commons/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/src/python3_commons/object_storage.py` & `python3_commons-0.5.8/src/python3_commons/object_storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,29 +39,27 @@
     return path
 
 
 def put_object(bucket_name: str, path: str, data: io.BytesIO, length: int) -> str:
     s3_client = get_s3_client(s3_settings)
 
     if s3_client:
-        path = get_absolute_path(path)
         result = s3_client.put_object(bucket_name, path, data, length)
 
         logger.debug(f'Stored object into object storage: {bucket_name}:{path}')
 
         return result.location
     else:
         logger.warning(f'No S3 client available, skipping object put')
 
 
 def get_object_stream(bucket_name: str, path: str):
     s3_client = get_s3_client(s3_settings)
 
     if s3_client:
-        path = get_absolute_path(path)
         logger.debug(f'Getting object from object storage: {bucket_name}:{path}')
 
         try:
             response = s3_client.get_object(bucket_name, path)
         except Exception as e:
             logger.debug(f'Failed getting object from object storage: {bucket_name}:{path}', exc_info=e)
 
@@ -90,16 +88,14 @@
     s3_client = get_s3_client(s3_settings)
 
     yield from s3_client.list_objects(bucket_name, prefix=prefix, recursive=recursive)
 
 
 def get_objects(bucket_name: str, path: str,
                 recursive: bool = True) -> Generator[tuple[str, datetime, bytes], None, None]:
-    path = get_absolute_path(path)
-
     for obj in list_objects(bucket_name, path, recursive):
         object_name = obj.object_name
 
         if obj.size:
             data = get_object(bucket_name, object_name)
         else:
             data = b''
@@ -113,15 +109,14 @@
 
 
 def remove_objects(bucket_name: str, prefix: str = None,
                    object_names: Iterable[str] = None) -> Iterable[DeleteError] | None:
     s3_client = get_s3_client(s3_settings)
 
     if prefix:
-        prefix = get_absolute_path(prefix)
         delete_object_list = map(
             lambda obj: DeleteObject(obj.object_name), s3_client.list_objects(bucket_name, prefix=prefix,
                                                                               recursive=True)
         )
     elif object_names:
         delete_object_list = map(DeleteObject, object_names)
     else:
```

### Comparing `python3_commons-0.5.7/src/python3_commons/serializers/json.py` & `python3_commons-0.5.8/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/src/python3_commons/serializers/msgpack.py` & `python3_commons-0.5.8/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/src/python3_commons/serializers/msgspec.py` & `python3_commons-0.5.8/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/src/python3_commons.egg-info/PKG-INFO` & `python3_commons-0.5.8/src/python3_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.7
+Version: 0.5.8
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.7/src/python3_commons.egg-info/SOURCES.txt` & `python3_commons-0.5.8/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/tests/conftest.py` & `python3_commons-0.5.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/tests/test_msgpack.py` & `python3_commons-0.5.8/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.7/tests/test_msgspec.py` & `python3_commons-0.5.8/tests/test_msgspec.py`

 * *Files identical despite different names*

