# Comparing `tmp/cdps-1.0.6.tar.gz` & `tmp/cdps-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdps-1.0.6.tar", last modified: Sat Jun  1 15:27:07 2024, max compression
+gzip compressed data, was "cdps-1.0.7.tar", last modified: Sat Jun  1 15:31:54 2024, max compression
```

## Comparing `cdps-1.0.6.tar` & `cdps-1.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.406601 cdps-1.0.6/
--rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:27:07.405611 cdps-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.363858 cdps-1.0.6/cdps/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/__main__.py
--rw-rw-rw-   0        0        0      393 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/boostrap.py
--rw-rw-rw-   0        0        0     1708 2024-06-01 15:18:23.000000 cdps-1.0.6/cdps/cdps_server.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.398595 cdps-1.0.6/cdps/cli/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/cli/__init__.py
--rw-rw-rw-   0        0        0     2353 2024-05-23 16:49:32.000000 cdps-1.0.6/cdps/cli/cli_entry.py
--rw-rw-rw-   0        0        0      231 2024-06-01 15:19:05.000000 cdps-1.0.6/cdps/cli/cli_gendefault.py
--rw-rw-rw-   0        0        0      348 2024-06-01 15:19:01.000000 cdps-1.0.6/cdps/cli/cli_init.py
--rw-rw-rw-   0        0        0      326 2024-06-01 15:18:55.000000 cdps-1.0.6/cdps/cli/cli_run.py
--rw-rw-rw-   0        0        0      190 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/cli/cli_version.py
--rw-rw-rw-   0        0        0     1215 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/config.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.399637 cdps-1.0.6/cdps/constants/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/constants/__init__.py
--rw-rw-rw-   0        0        0      112 2024-06-01 15:26:51.000000 cdps-1.0.6/cdps/constants/core_constant.py
--rw-rw-rw-   0        0        0      598 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/entrypoint.py
--rw-rw-rw-   0        0        0      401 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/state.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.405611 cdps-1.0.6/cdps/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/__init__.py
--rw-rw-rw-   0        0        0     1233 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/file_util.py
--rw-rw-rw-   0        0        0      344 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/lazy_item.py
--rw-rw-rw-   0        0        0      265 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/level.py
--rw-rw-rw-   0        0        0      554 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/line.py
--rw-rw-rw-   0        0        0     4397 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/logger.py
--rw-rw-rw-   0        0        0      765 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/resources_util.py
--rw-rw-rw-   0        0        0     1663 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/yaml_data_storage.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.393890 cdps-1.0.6/cdps.egg-info/
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:27:07.406601 cdps-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1710 2024-06-01 15:27:04.000000 cdps-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.530191 cdps-1.0.7/
+-rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:31:54.529167 cdps-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.495981 cdps-1.0.7/cdps/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/__init__.py
+-rw-rw-rw-   0        0        0      116 2024-06-01 15:30:54.000000 cdps-1.0.7/cdps/__main__.py
+-rw-rw-rw-   0        0        0      393 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/boostrap.py
+-rw-rw-rw-   0        0        0     1688 2024-06-01 15:30:46.000000 cdps-1.0.7/cdps/cdps_server.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.521497 cdps-1.0.7/cdps/cli/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/cli/__init__.py
+-rw-rw-rw-   0        0        0     2328 2024-06-01 15:31:23.000000 cdps-1.0.7/cdps/cli/cli_entry.py
+-rw-rw-rw-   0        0        0      226 2024-06-01 15:31:26.000000 cdps-1.0.7/cdps/cli/cli_gendefault.py
+-rw-rw-rw-   0        0        0      338 2024-06-01 15:31:31.000000 cdps-1.0.7/cdps/cli/cli_init.py
+-rw-rw-rw-   0        0        0      316 2024-06-01 15:31:37.000000 cdps-1.0.7/cdps/cli/cli_run.py
+-rw-rw-rw-   0        0        0      185 2024-06-01 15:31:40.000000 cdps-1.0.7/cdps/cli/cli_version.py
+-rw-rw-rw-   0        0        0     1210 2024-06-01 15:30:38.000000 cdps-1.0.7/cdps/config.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.522517 cdps-1.0.7/cdps/constants/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/constants/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-06-01 15:31:49.000000 cdps-1.0.7/cdps/constants/core_constant.py
+-rw-rw-rw-   0        0        0      588 2024-06-01 15:30:33.000000 cdps-1.0.7/cdps/entrypoint.py
+-rw-rw-rw-   0        0        0      401 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/state.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.529167 cdps-1.0.7/cdps/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/__init__.py
+-rw-rw-rw-   0        0        0     1233 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/file_util.py
+-rw-rw-rw-   0        0        0      344 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/lazy_item.py
+-rw-rw-rw-   0        0        0      265 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/level.py
+-rw-rw-rw-   0        0        0      554 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/line.py
+-rw-rw-rw-   0        0        0     4397 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/logger.py
+-rw-rw-rw-   0        0        0      765 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/resources_util.py
+-rw-rw-rw-   0        0        0     1653 2024-06-01 15:31:08.000000 cdps-1.0.7/cdps/utils/yaml_data_storage.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.517801 cdps-1.0.7/cdps.egg-info/
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      172 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:31:54.530191 cdps-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1710 2024-06-01 15:27:04.000000 cdps-1.0.7/setup.py
```

### Comparing `cdps-1.0.6/LICENSE` & `cdps-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdps-1.0.6/PKG-INFO` & `cdps-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.6
+Version: 1.0.7
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.6/README.md` & `cdps-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cdps-1.0.6/cdps/cdps_server.py` & `cdps-1.0.7/cdps/cdps_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
-from core.config import Config
-from core.state import State
+from config import Config
+from state import State
 
-from core.utils.logger import Log
-from core.constants import core_constant
+from utils.logger import Log
+from constants import core_constant
 
 class CDPS:
     def __init__(self, *, generate_default_only: bool = False, initialize_environment: bool = False, focus: bool = False):
         self.log = Log()
         self.log.logger.info("Start {} {}".format(
             core_constant.NAME, core_constant.VERSION))
```

### Comparing `cdps-1.0.6/cdps/cli/cli_entry.py` & `cdps-1.0.7/cdps/cli/cli_entry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from argparse import ArgumentParser
 
-from core.constants import core_constant
-from core.cli.cli_version import show_version
-from core.cli.cli_init import initialize_environment
-from core.cli.cli_gendefault import generate_default_stuffs
-from core.cli.cli_run import run
+from constants import core_constant
+from cli.cli_version import show_version
+from cli.cli_init import initialize_environment
+from cli.cli_gendefault import generate_default_stuffs
+from cli.cli_run import run
 
 
 def cli_dispatch():
     if len(sys.argv) == 1:
         run()
         return
```

### Comparing `cdps-1.0.6/cdps/config.py` & `cdps-1.0.7/cdps/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 MCDR config file stuffs
 """
 from typing import Any, Tuple, Dict, Union
 
-from core.utils.yaml_data_storage import YamlDataStorage
+from utils.yaml_data_storage import YamlDataStorage
 
 CONFIG_FILE = 'config.yml'
 DEFAULT_CONFIG_RESOURCE_PATH = '/resources/default_config.yml'
 
 
 class Config(YamlDataStorage):
     def __init__(self):
```

### Comparing `cdps-1.0.6/cdps/entrypoint.py` & `cdps-1.0.7/cdps/entrypoint.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import platform
 import sys
 
-from core.constants import core_constant
-from core.boostrap import boostrap
+from constants import core_constant
+from boostrap import boostrap
 
 
 def __environment_check():
     """
 
     """
     python_version = sys.version_info.major+sys.version_info.minor*0.1
```

### Comparing `cdps-1.0.6/cdps/utils/file_util.py` & `cdps-1.0.7/cdps/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.6/cdps/utils/line.py` & `cdps-1.0.7/cdps/utils/line.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.6/cdps/utils/logger.py` & `cdps-1.0.7/cdps/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.6/cdps/utils/resources_util.py` & `cdps-1.0.7/cdps/utils/resources_util.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.6/cdps/utils/yaml_data_storage.py` & `cdps-1.0.7/cdps/utils/yaml_data_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from threading import RLock
 
 from ruamel.yaml import YAML
 from ruamel.yaml.comments import CommentedMap
 
-from core.utils import resources_util, file_util
-from core.utils.lazy_item import LazyItem
+from utils import resources_util, file_util
+from utils.lazy_item import LazyItem
 
 
 class YamlDataStorage:
     def __init__(self, file_path: str, default_file_path: str):
         self.__file_path = file_path
         self.__default_file_path = default_file_path
         self.__default_data = LazyItem(
```

### Comparing `cdps-1.0.6/cdps.egg-info/PKG-INFO` & `cdps-1.0.7/cdps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.6
+Version: 1.0.7
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.6/cdps.egg-info/SOURCES.txt` & `cdps-1.0.7/cdps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdps-1.0.6/setup.py` & `cdps-1.0.7/setup.py`

 * *Files identical despite different names*

