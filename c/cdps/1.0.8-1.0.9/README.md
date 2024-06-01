# Comparing `tmp/cdps-1.0.8.tar.gz` & `tmp/cdps-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdps-1.0.8.tar", last modified: Sat Jun  1 15:33:40 2024, max compression
+gzip compressed data, was "cdps-1.0.9.tar", last modified: Sat Jun  1 15:41:53 2024, max compression
```

## Comparing `cdps-1.0.8.tar` & `cdps-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.019934 cdps-1.0.8/
--rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:33:40.018934 cdps-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 15:33:39.989606 cdps-1.0.8/cdps/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/__init__.py
--rw-rw-rw-   0        0        0      116 2024-06-01 15:30:54.000000 cdps-1.0.8/cdps/__main__.py
--rw-rw-rw-   0        0        0      393 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/boostrap.py
--rw-rw-rw-   0        0        0     1688 2024-06-01 15:30:46.000000 cdps-1.0.8/cdps/cdps_server.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.011902 cdps-1.0.8/cdps/cli/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/cli/__init__.py
--rw-rw-rw-   0        0        0     2328 2024-06-01 15:31:23.000000 cdps-1.0.8/cdps/cli/cli_entry.py
--rw-rw-rw-   0        0        0      226 2024-06-01 15:31:26.000000 cdps-1.0.8/cdps/cli/cli_gendefault.py
--rw-rw-rw-   0        0        0      338 2024-06-01 15:31:31.000000 cdps-1.0.8/cdps/cli/cli_init.py
--rw-rw-rw-   0        0        0      316 2024-06-01 15:31:37.000000 cdps-1.0.8/cdps/cli/cli_run.py
--rw-rw-rw-   0        0        0      185 2024-06-01 15:31:40.000000 cdps-1.0.8/cdps/cli/cli_version.py
--rw-rw-rw-   0        0        0     1210 2024-06-01 15:30:38.000000 cdps-1.0.8/cdps/config.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.012902 cdps-1.0.8/cdps/constants/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/constants/__init__.py
--rw-rw-rw-   0        0        0      112 2024-06-01 15:33:33.000000 cdps-1.0.8/cdps/constants/core_constant.py
--rw-rw-rw-   0        0        0      583 2024-06-01 15:32:25.000000 cdps-1.0.8/cdps/entrypoint.py
--rw-rw-rw-   0        0        0      401 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/state.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.018934 cdps-1.0.8/cdps/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/__init__.py
--rw-rw-rw-   0        0        0     1233 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/file_util.py
--rw-rw-rw-   0        0        0      344 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/lazy_item.py
--rw-rw-rw-   0        0        0      265 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/level.py
--rw-rw-rw-   0        0        0      554 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/line.py
--rw-rw-rw-   0        0        0     4397 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/logger.py
--rw-rw-rw-   0        0        0      765 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/resources_util.py
--rw-rw-rw-   0        0        0     1653 2024-06-01 15:31:08.000000 cdps-1.0.8/cdps/utils/yaml_data_storage.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.006890 cdps-1.0.8/cdps.egg-info/
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:33:40.019934 cdps-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1745 2024-06-01 15:33:14.000000 cdps-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:53.112894 cdps-1.0.9/
+-rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       77 2024-06-01 15:39:18.000000 cdps-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:41:53.112894 cdps-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:53.066908 cdps-1.0.9/cdps/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/__init__.py
+-rw-rw-rw-   0        0        0      116 2024-06-01 15:40:28.000000 cdps-1.0.9/cdps/__main__.py
+-rw-rw-rw-   0        0        0      393 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/boostrap.py
+-rw-rw-rw-   0        0        0     1698 2024-06-01 15:39:51.000000 cdps-1.0.9/cdps/cdps_server.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:53.105197 cdps-1.0.9/cdps/cli/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/cli/__init__.py
+-rw-rw-rw-   0        0        0     2353 2024-06-01 15:41:15.000000 cdps-1.0.9/cdps/cli/cli_entry.py
+-rw-rw-rw-   0        0        0      231 2024-06-01 15:41:19.000000 cdps-1.0.9/cdps/cli/cli_gendefault.py
+-rw-rw-rw-   0        0        0      348 2024-06-01 15:41:24.000000 cdps-1.0.9/cdps/cli/cli_init.py
+-rw-rw-rw-   0        0        0      326 2024-06-01 15:41:29.000000 cdps-1.0.9/cdps/cli/cli_run.py
+-rw-rw-rw-   0        0        0      190 2024-06-01 15:41:34.000000 cdps-1.0.9/cdps/cli/cli_version.py
+-rw-rw-rw-   0        0        0     1215 2024-06-01 15:39:47.000000 cdps-1.0.9/cdps/config.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:53.106230 cdps-1.0.9/cdps/constants/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/constants/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-06-01 15:41:41.000000 cdps-1.0.9/cdps/constants/core_constant.py
+-rw-rw-rw-   0        0        0      593 2024-06-01 15:39:38.000000 cdps-1.0.9/cdps/entrypoint.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:53.107805 cdps-1.0.9/cdps/resources/
+-rw-rw-rw-   0        0        0       94 2024-06-01 14:27:54.000000 cdps-1.0.9/cdps/resources/default_config.yml
+-rw-rw-rw-   0        0        0      401 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/state.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:53.111879 cdps-1.0.9/cdps/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/utils/__init__.py
+-rw-rw-rw-   0        0        0     1233 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/utils/file_util.py
+-rw-rw-rw-   0        0        0      344 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/utils/lazy_item.py
+-rw-rw-rw-   0        0        0     4397 2024-05-21 07:25:40.000000 cdps-1.0.9/cdps/utils/logger.py
+-rw-rw-rw-   0        0        0      741 2024-06-01 15:40:45.000000 cdps-1.0.9/cdps/utils/resources_util.py
+-rw-rw-rw-   0        0        0     1663 2024-06-01 15:40:37.000000 cdps-1.0.9/cdps/utils/yaml_data_storage.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:53.101245 cdps-1.0.9/cdps.egg-info/
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:41:52.000000 cdps-1.0.9/cdps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2024-06-01 15:41:53.000000 cdps-1.0.9/cdps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:41:52.000000 cdps-1.0.9/cdps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-06-01 15:41:52.000000 cdps-1.0.9/cdps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      172 2024-06-01 15:41:52.000000 cdps-1.0.9/cdps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 15:41:52.000000 cdps-1.0.9/cdps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      181 2024-06-01 15:15:23.000000 cdps-1.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:41:53.112894 cdps-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1745 2024-06-01 15:33:14.000000 cdps-1.0.9/setup.py
```

### Comparing `cdps-1.0.8/LICENSE` & `cdps-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdps-1.0.8/PKG-INFO` & `cdps-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.8
+Version: 1.0.9
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.8/README.md` & `cdps-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdps-1.0.8/cdps/cdps_server.py` & `cdps-1.0.9/cdps/cdps_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 from config import Config
 from state import State
 
-from utils.logger import Log
-from constants import core_constant
+from cdps.utils.logger import Log
+from cdps.constants import core_constant
 
 class CDPS:
     def __init__(self, *, generate_default_only: bool = False, initialize_environment: bool = False, focus: bool = False):
         self.log = Log()
         self.log.logger.info("Start {} {}".format(
             core_constant.NAME, core_constant.VERSION))
```

### Comparing `cdps-1.0.8/cdps/cli/cli_entry.py` & `cdps-1.0.9/cdps/cli/cli_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from argparse import ArgumentParser
 
-from constants import core_constant
-from cli.cli_version import show_version
-from cli.cli_init import initialize_environment
-from cli.cli_gendefault import generate_default_stuffs
-from cli.cli_run import run
+from cdps.constants import core_constant
+from cdps.cli.cli_version import show_version
+from cdps.cli.cli_init import initialize_environment
+from cdps.cli.cli_gendefault import generate_default_stuffs
+from cdps.cli.cli_run import run
 
 
 def cli_dispatch():
     if len(sys.argv) == 1:
         run()
         return
```

### Comparing `cdps-1.0.8/cdps/config.py` & `cdps-1.0.9/cdps/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 MCDR config file stuffs
 """
 from typing import Any, Tuple, Dict, Union
 
-from utils.yaml_data_storage import YamlDataStorage
+from cdps.utils.yaml_data_storage import YamlDataStorage
 
 CONFIG_FILE = 'config.yml'
 DEFAULT_CONFIG_RESOURCE_PATH = '/resources/default_config.yml'
 
 
 class Config(YamlDataStorage):
     def __init__(self):
```

### Comparing `cdps-1.0.8/cdps/entrypoint.py` & `cdps-1.0.9/cdps/entrypoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import platform
 import sys
 
-from constants import core_constant
-from boostrap import boostrap
+from cdps.constants import core_constant
+from cdps.boostrap import boostrap
 
 
 def __environment_check():
     """
 
     """
     python_version = sys.version_info.major+sys.version_info.minor*0.1
```

### Comparing `cdps-1.0.8/cdps/utils/file_util.py` & `cdps-1.0.9/cdps/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.8/cdps/utils/logger.py` & `cdps-1.0.9/cdps/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.8/cdps/utils/resources_util.py` & `cdps-1.0.9/cdps/utils/resources_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,15 @@
     'ROOT_PACKAGE',
     'get_data', 'get_yaml'
 ]
 
 from ruamel.yaml import YAML
 from ruamel.yaml.comments import CommentedMap
 
-import pkg_resources
-
-from core.constants import core_constant
+from cdps.constants import core_constant
 
 ROOT_PACKAGE = core_constant.PACKAGE_NAME
 
 
 def __get_path(path: str) -> str:
     if path.startswith('/'):
         path = path[1:]
```

### Comparing `cdps-1.0.8/cdps/utils/yaml_data_storage.py` & `cdps-1.0.9/cdps/utils/yaml_data_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from threading import RLock
 
 from ruamel.yaml import YAML
 from ruamel.yaml.comments import CommentedMap
 
-from utils import resources_util, file_util
-from utils.lazy_item import LazyItem
+from cdps.utils import resources_util, file_util
+from cdps.utils.lazy_item import LazyItem
 
 
 class YamlDataStorage:
     def __init__(self, file_path: str, default_file_path: str):
         self.__file_path = file_path
         self.__default_file_path = default_file_path
         self.__default_data = LazyItem(
```

### Comparing `cdps-1.0.8/cdps.egg-info/PKG-INFO` & `cdps-1.0.9/cdps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.8
+Version: 1.0.9
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.8/cdps.egg-info/SOURCES.txt` & `cdps-1.0.9/cdps.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 cdps/__init__.py
 cdps/__main__.py
 cdps/boostrap.py
 cdps/cdps_server.py
 cdps/config.py
 cdps/entrypoint.py
@@ -18,15 +20,14 @@
 cdps/cli/cli_entry.py
 cdps/cli/cli_gendefault.py
 cdps/cli/cli_init.py
 cdps/cli/cli_run.py
 cdps/cli/cli_version.py
 cdps/constants/__init__.py
 cdps/constants/core_constant.py
+cdps/resources/default_config.yml
 cdps/utils/__init__.py
 cdps/utils/file_util.py
 cdps/utils/lazy_item.py
-cdps/utils/level.py
-cdps/utils/line.py
 cdps/utils/logger.py
 cdps/utils/resources_util.py
 cdps/utils/yaml_data_storage.py
```

### Comparing `cdps-1.0.8/setup.py` & `cdps-1.0.9/setup.py`

 * *Files identical despite different names*

