# Comparing `tmp/codejudge-common-utils-0.0.3.tar.gz` & `tmp/codejudge-common-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codejudge-common-utils-0.0.3.tar", last modified: Sat Jun  1 19:27:51 2024, max compression
+gzip compressed data, was "codejudge-common-utils-0.0.4.tar", last modified: Sat Jun  1 19:51:28 2024, max compression
```

## Comparing `codejudge-common-utils-0.0.3.tar` & `codejudge-common-utils-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:27:51.621431 codejudge-common-utils-0.0.3/
--rw-r--r--   0 yash       (501) staff       (20)     2250 2024-06-01 19:27:51.621190 codejudge-common-utils-0.0.3/PKG-INFO
--rw-r--r--   0 yash       (501) staff       (20)     1496 2024-05-09 12:19:46.000000 codejudge-common-utils-0.0.3/README.md
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:27:51.617474 codejudge-common-utils-0.0.3/codejudge_common_utils.egg-info/
--rw-r--r--   0 yash       (501) staff       (20)     2250 2024-06-01 19:27:51.000000 codejudge-common-utils-0.0.3/codejudge_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 yash       (501) staff       (20)      527 2024-06-01 19:27:51.000000 codejudge-common-utils-0.0.3/codejudge_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 yash       (501) staff       (20)        1 2024-06-01 19:27:51.000000 codejudge-common-utils-0.0.3/codejudge_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 yash       (501) staff       (20)        7 2024-06-01 19:27:51.000000 codejudge-common-utils-0.0.3/codejudge_common_utils.egg-info/top_level.txt
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:27:51.620773 codejudge-common-utils-0.0.3/common/
--rw-r--r--   0 yash       (501) staff       (20)        0 2024-05-08 13:47:56.000000 codejudge-common-utils-0.0.3/common/__init__.py
--rw-r--r--   0 yash       (501) staff       (20)      179 2024-05-13 20:27:30.000000 codejudge-common-utils-0.0.3/common/common_util.py
--rw-r--r--   0 yash       (501) staff       (20)       72 2024-05-14 11:27:25.000000 codejudge-common-utils-0.0.3/common/constants.py
--rw-r--r--   0 yash       (501) staff       (20)      395 2024-06-01 14:19:58.000000 codejudge-common-utils-0.0.3/common/data_purging_interface.py
--rw-r--r--   0 yash       (501) staff       (20)     6198 2024-06-01 19:22:04.000000 codejudge-common-utils-0.0.3/common/data_purging_util.py
--rw-r--r--   0 yash       (501) staff       (20)     7957 2024-05-09 19:18:11.000000 codejudge-common-utils-0.0.3/common/date_time_util.py
--rw-r--r--   0 yash       (501) staff       (20)     2167 2024-06-01 14:08:40.000000 codejudge-common-utils-0.0.3/common/enum_util.py
--rw-r--r--   0 yash       (501) staff       (20)     4908 2024-06-01 14:09:00.000000 codejudge-common-utils-0.0.3/common/enums.py
--rw-r--r--   0 yash       (501) staff       (20)     2763 2024-05-13 22:11:10.000000 codejudge-common-utils-0.0.3/common/interval_dates_and_archive_table_name.py
--rw-r--r--   0 yash       (501) staff       (20)      429 2024-05-13 08:22:33.000000 codejudge-common-utils-0.0.3/common/interval_type_to_process_function_mapping.py
--rw-r--r--   0 yash       (501) staff       (20)     1144 2024-05-14 09:38:43.000000 codejudge-common-utils-0.0.3/common/model_util.py
--rw-r--r--   0 yash       (501) staff       (20)     4906 2024-06-01 19:22:04.000000 codejudge-common-utils-0.0.3/common/table_util.py
--rw-r--r--   0 yash       (501) staff       (20)       38 2024-06-01 19:27:51.621492 codejudge-common-utils-0.0.3/setup.cfg
--rw-r--r--   0 yash       (501) staff       (20)      986 2024-06-01 19:27:43.000000 codejudge-common-utils-0.0.3/setup.py
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:51:28.104319 codejudge-common-utils-0.0.4/
+-rw-r--r--   0 yash       (501) staff       (20)     2250 2024-06-01 19:51:28.104090 codejudge-common-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 yash       (501) staff       (20)     1496 2024-05-09 12:19:46.000000 codejudge-common-utils-0.0.4/README.md
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:51:28.100986 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/
+-rw-r--r--   0 yash       (501) staff       (20)     2250 2024-06-01 19:51:28.000000 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 yash       (501) staff       (20)      527 2024-06-01 19:51:28.000000 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 yash       (501) staff       (20)        1 2024-06-01 19:51:28.000000 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 yash       (501) staff       (20)        7 2024-06-01 19:51:28.000000 codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/top_level.txt
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-06-01 19:51:28.103713 codejudge-common-utils-0.0.4/common/
+-rw-r--r--   0 yash       (501) staff       (20)        0 2024-05-08 13:47:56.000000 codejudge-common-utils-0.0.4/common/__init__.py
+-rw-r--r--   0 yash       (501) staff       (20)      179 2024-05-13 20:27:30.000000 codejudge-common-utils-0.0.4/common/common_util.py
+-rw-r--r--   0 yash       (501) staff       (20)      102 2024-06-01 19:49:23.000000 codejudge-common-utils-0.0.4/common/constants.py
+-rw-r--r--   0 yash       (501) staff       (20)      395 2024-06-01 14:19:58.000000 codejudge-common-utils-0.0.4/common/data_purging_interface.py
+-rw-r--r--   0 yash       (501) staff       (20)     6271 2024-06-01 19:49:23.000000 codejudge-common-utils-0.0.4/common/data_purging_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     7957 2024-05-09 19:18:11.000000 codejudge-common-utils-0.0.4/common/date_time_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     2167 2024-06-01 14:08:40.000000 codejudge-common-utils-0.0.4/common/enum_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     4908 2024-06-01 14:09:00.000000 codejudge-common-utils-0.0.4/common/enums.py
+-rw-r--r--   0 yash       (501) staff       (20)     2763 2024-05-13 22:11:10.000000 codejudge-common-utils-0.0.4/common/interval_dates_and_archive_table_name.py
+-rw-r--r--   0 yash       (501) staff       (20)      429 2024-05-13 08:22:33.000000 codejudge-common-utils-0.0.4/common/interval_type_to_process_function_mapping.py
+-rw-r--r--   0 yash       (501) staff       (20)     1144 2024-05-14 09:38:43.000000 codejudge-common-utils-0.0.4/common/model_util.py
+-rw-r--r--   0 yash       (501) staff       (20)     4906 2024-06-01 19:22:04.000000 codejudge-common-utils-0.0.4/common/table_util.py
+-rw-r--r--   0 yash       (501) staff       (20)       38 2024-06-01 19:51:28.104369 codejudge-common-utils-0.0.4/setup.cfg
+-rw-r--r--   0 yash       (501) staff       (20)      986 2024-06-01 19:51:23.000000 codejudge-common-utils-0.0.4/setup.py
```

### Comparing `codejudge-common-utils-0.0.3/PKG-INFO` & `codejudge-common-utils-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codejudge-common-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A codejudge common util library for python to perform certain tasks.
 Author: Yash Mittal
 Author-email: akhil@codejudge.io
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `codejudge-common-utils-0.0.3/README.md` & `codejudge-common-utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.3/codejudge_common_utils.egg-info/PKG-INFO` & `codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codejudge-common-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A codejudge common util library for python to perform certain tasks.
 Author: Yash Mittal
 Author-email: akhil@codejudge.io
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `codejudge-common-utils-0.0.3/codejudge_common_utils.egg-info/SOURCES.txt` & `codejudge-common-utils-0.0.4/codejudge_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.3/common/data_purging_util.py` & `codejudge-common-utils-0.0.4/common/data_purging_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import math
 import os.path
 
 from django.db import transaction, connection
 from rest_framework import status
 
+from common.constants import DATA_PURGING_MAX_RETRY
 from common.table_util import TableUtil
 from restapi.common.list_util import ListUtil
 from restapi.common.file_util import FileUtil
 from restapi.test.worker.data_purging_framework.data_purging_process import get_unique_ids_to_s3_file_paths_map, \
     upload_json_file_in_s3_and_get_uuid_to_file_urls_map
 from restapi.exception.exception import RecruitException
 
@@ -65,15 +66,15 @@
                         logger.info("Records are successfully inserted in archive table {}".format(archive_table_name))
                         TableUtil.delete_records(table_name_str, records_to_delete, table_name_prefix, cursor, is_fb,
                                                  app1)
                         logger.info("Records are successfully deleted from the main table {}".format(main_table_name))
                         is_completed = True
         except Exception as e:
             if is_completed is False:
-                retry_count = 3
+                retry_count = DATA_PURGING_MAX_RETRY
                 while retry_count > 0:
                     cursor = connection.cursor()
                     with transaction.atomic():
                         if is_archive_table_present is False:
                             TableUtil.drop_archive_table_if_exist(archive_table_name)
                             TableUtil.create_archive_table(archive_table_name, table_name_str, table_name_prefix, cursor, is_fb)
                             TableUtil.make_migrations_to_create_table()
```

### Comparing `codejudge-common-utils-0.0.3/common/date_time_util.py` & `codejudge-common-utils-0.0.4/common/date_time_util.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.3/common/enum_util.py` & `codejudge-common-utils-0.0.4/common/enum_util.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.3/common/enums.py` & `codejudge-common-utils-0.0.4/common/enums.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.3/common/interval_dates_and_archive_table_name.py` & `codejudge-common-utils-0.0.4/common/interval_dates_and_archive_table_name.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.3/common/model_util.py` & `codejudge-common-utils-0.0.4/common/model_util.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.3/common/table_util.py` & `codejudge-common-utils-0.0.4/common/table_util.py`

 * *Files identical despite different names*

### Comparing `codejudge-common-utils-0.0.3/setup.py` & `codejudge-common-utils-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="codejudge-common-utils",
-    version="0.0.3",
+    version="0.0.4",
     description="A codejudge common util library for python to perform certain tasks.",
     long_description=long_description,
     author="Yash Mittal",
     author_email="akhil@codejudge.io",
     classifiers=
     [
         "Environment :: Web Environment",
```

