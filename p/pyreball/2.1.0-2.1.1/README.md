# Comparing `tmp/pyreball-2.1.0.tar.gz` & `tmp/pyreball-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreball-2.1.0.tar", max compression
+gzip compressed data, was "pyreball-2.1.1.tar", max compression
```

## Comparing `pyreball-2.1.0.tar` & `pyreball-2.1.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    11344 2024-04-15 19:48:17.769266 pyreball-2.1.0/LICENSE
--rw-r--r--   0        0        0     4128 2024-04-15 19:48:17.769266 pyreball-2.1.0/README.md
--rw-r--r--   0        0        0     3254 2024-04-15 19:48:17.769266 pyreball-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      739 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/__init__.py
--rw-r--r--   0        0        0    25870 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/__main__.py
--rw-r--r--   0        0        0      597 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/_common.py
--rw-r--r--   0        0        0      573 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/cfg/config.ini
--rw-r--r--   0        0        0     1486 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/cfg/css.template
--rw-r--r--   0        0        0     1594 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/cfg/external_links.ini
--rw-r--r--   0        0        0      316 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/cfg/html.template
--rw-r--r--   0        0        0     1534 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/config_generator.py
--rw-r--r--   0        0        0      212 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/constants.py
--rw-r--r--   0        0        0    42545 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/html.py
--rw-r--r--   0        0        0        0 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/py.typed
--rw-r--r--   0        0        0    16707 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/text.py
--rw-r--r--   0        0        0        0 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/utils/__init__.py
--rw-r--r--   0        0        0      457 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/utils/logger.py
--rw-r--r--   0        0        0    13435 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/utils/param.py
--rw-r--r--   0        0        0     1059 2024-04-15 19:48:17.769266 pyreball-2.1.0/src/pyreball/utils/template.py
--rw-r--r--   0        0        0     6104 1970-01-01 00:00:00.000000 pyreball-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-06-01 09:36:18.582009 pyreball-2.1.1/LICENSE
+-rw-r--r--   0        0        0     4128 2024-06-01 09:36:18.582009 pyreball-2.1.1/README.md
+-rw-r--r--   0        0        0     3378 2024-06-01 09:36:18.586009 pyreball-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      739 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/__init__.py
+-rw-r--r--   0        0        0    25855 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/__main__.py
+-rw-r--r--   0        0        0      597 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/_common.py
+-rw-r--r--   0        0        0      573 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/cfg/config.ini
+-rw-r--r--   0        0        0     1486 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/cfg/css.template
+-rw-r--r--   0        0        0     1594 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/cfg/external_links.ini
+-rw-r--r--   0        0        0      316 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/cfg/html.template
+-rw-r--r--   0        0        0     1519 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/config_generator.py
+-rw-r--r--   0        0        0      212 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/constants.py
+-rw-r--r--   0        0        0    42545 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/html.py
+-rw-r--r--   0        0        0        0 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/py.typed
+-rw-r--r--   0        0        0    16707 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/text.py
+-rw-r--r--   0        0        0        0 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/utils/__init__.py
+-rw-r--r--   0        0        0    13419 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/utils/param.py
+-rw-r--r--   0        0        0     1043 2024-06-01 09:36:18.586009 pyreball-2.1.1/src/pyreball/utils/template.py
+-rw-r--r--   0        0        0     6228 1970-01-01 00:00:00.000000 pyreball-2.1.1/PKG-INFO
```

### Comparing `pyreball-2.1.0/LICENSE` & `pyreball-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/README.md` & `pyreball-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/pyproject.toml` & `pyreball-2.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyreball"
-version = "2.1.0"
+version = "2.1.1"
 description = "Python reporting tool."
 authors = ["Karel Vaculik <vaculik.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "pyreball", from = "src" }]
 keywords = ["python", "reporting", "html"]
 classifiers = [
@@ -15,14 +15,18 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
+[tool.poetry.urls]
+homepage = 'https://github.com/karelvaculik/pyreball'
+documentation = 'https://pyreball.readthedocs.io'
+
 [tool.poetry.dependencies]
 python = ">=3.8"
 altair = { version = "^5.0.1", optional = true }
 altair-viewer = { version = "^0.4.0", optional = true }
 bokeh = [
     { version = "^3.1.1", python = "<3.9", optional = true },
     { version = "^3.2.2", python = ">=3.9,<3.12", optional = true },
```

### Comparing `pyreball-2.1.0/src/pyreball/__init__.py` & `pyreball-2.1.1/src/pyreball/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/src/pyreball/__main__.py` & `pyreball-2.1.1/src/pyreball/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import json
+import logging
 import os
 import re
 import sys
 import textwrap
 import typing
 import xml
 from pathlib import Path
@@ -13,30 +14,29 @@
 from pyreball._common import get_default_path_to_config
 from pyreball.constants import (
     CONFIG_INI_FILENAME,
     HTML_TEMPLATE_FILENAME,
     LINKS_INI_FILENAME,
     STYLES_TEMPLATE_FILENAME,
 )
-from pyreball.utils.logger import get_logger
 from pyreball.utils.param import (
     ChoiceParameter,
     IntegerParameter,
     StringParameter,
     Substitutor,
     carefully_remove_directory_if_exists,
     check_and_fix_parameters,
     check_paging_sizes_string_parameter,
     get_external_links_from_config,
     get_file_config,
     merge_parameter_dictionaries,
 )
 from pyreball.utils.template import get_css, get_html
 
-logger = get_logger()
+logger = logging.getLogger(__name__)
 
 
 def _replace_ids(lines: List[str]) -> List[str]:
     """
     Replace IDs of HTML elements to create working anchors based on references.
 
     Args:
```

### Comparing `pyreball-2.1.0/src/pyreball/_common.py` & `pyreball-2.1.1/src/pyreball/_common.py`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/src/pyreball/cfg/config.ini` & `pyreball-2.1.1/src/pyreball/cfg/config.ini`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/src/pyreball/cfg/css.template` & `pyreball-2.1.1/src/pyreball/cfg/css.template`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/src/pyreball/cfg/external_links.ini` & `pyreball-2.1.1/src/pyreball/cfg/external_links.ini`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/src/pyreball/config_generator.py` & `pyreball-2.1.1/src/pyreball/config_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import argparse
+import logging
 import shutil
 from pathlib import Path
 
 from pyreball._common import get_default_path_to_config
 from pyreball.constants import (
     CONFIG_INI_FILENAME,
     HTML_TEMPLATE_FILENAME,
     LINKS_INI_FILENAME,
     STYLES_TEMPLATE_FILENAME,
 )
-from pyreball.utils.logger import get_logger
 
-logger = get_logger()
+logger = logging.getLogger(__name__)
 
 
 def copy_config_files(output_directory: Path) -> None:
     if output_directory.exists():
         logger.warning(
             f"Directory {output_directory} already exists, config will be over-written."
         )
```

### Comparing `pyreball-2.1.0/src/pyreball/html.py` & `pyreball-2.1.1/src/pyreball/html.py`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/src/pyreball/text.py` & `pyreball-2.1.1/src/pyreball/text.py`

 * *Files identical despite different names*

### Comparing `pyreball-2.1.0/src/pyreball/utils/param.py` & `pyreball-2.1.1/src/pyreball/utils/param.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import argparse
 import configparser
 import json
+import logging
 import os
 import re
 import shutil
 import sys
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
-from pyreball.utils.logger import get_logger
-
 ParametersType = Dict[str, Optional[Union[str, int]]]
 
-logger = get_logger()
+logger = logging.getLogger(__name__)
 
 _parameter_cache = {}
 
 
 class Parameter(ABC):
     def __init__(self, option_string: str, help: str):
         self.option_string = option_string
```

### Comparing `pyreball-2.1.0/src/pyreball/utils/template.py` & `pyreball-2.1.1/src/pyreball/utils/template.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+import logging
 import re
 import sys
 from pathlib import Path
 from typing import Tuple
 
-from pyreball.utils.logger import get_logger
-
-logger = get_logger()
+logger = logging.getLogger(__name__)
 
 
 def get_html(template_path: Path, title: str, css_definitions: str) -> Tuple[str, str]:
     with open(template_path) as f:
         html_text = f.read()
         html_start, html_end = html_text.split("<!--PYREBALL_REPORT_CONTENTS-->")
         html_start = re.sub("<!--PYREBALL_PAGE_TITLE-->", title, html_start)
```

### Comparing `pyreball-2.1.0/PKG-INFO` & `pyreball-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreball
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python reporting tool.
 License: Apache-2.0
 Keywords: python,reporting,html
 Author: Karel Vaculik
 Author-email: vaculik.dev@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,14 +27,16 @@
 Requires-Dist: numpy (>=1.25.2,<2.0.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "examples")
 Requires-Dist: numpy (>=1.26.4,<2.0.0) ; (python_version >= "3.12") and (extra == "examples")
 Requires-Dist: pandas (>=2.0.3,<3.0.0) ; (python_version < "3.9") and (extra == "examples")
 Requires-Dist: pandas (>=2.0.3,<3.0.0) ; (python_version >= "3.9" and python_version < "3.12") and (extra == "examples")
 Requires-Dist: pandas (>=2.2.2,<3.0.0) ; (python_version >= "3.12") and (extra == "examples")
 Requires-Dist: plotly (>=5.16.1,<6.0.0) ; extra == "examples"
 Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "examples"
+Project-URL: documentation, https://pyreball.readthedocs.io
+Project-URL: homepage, https://github.com/karelvaculik/pyreball
 Description-Content-Type: text/markdown
 
 # Pyreball
 
 <p style="text-align: center">
 
 ![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
```

