# Comparing `tmp/jinjyaml-0.4.tar.gz` & `tmp/jinjyaml-0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjyaml-0.4.tar", last modified: Sat Jun  1 10:20:21 2024, max compression
+gzip compressed data, was "jinjyaml-0.4rc1.tar", last modified: Fri Mar 15 09:45:15 2024, max compression
```

## Comparing `jinjyaml-0.4.tar` & `jinjyaml-0.4rc1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 10:20:21.264975 jinjyaml-0.4/
--rw-rw-rw-   0        0        0      188 2023-06-13 10:06:00.000000 jinjyaml-0.4/AUTHORS.md
--rw-rw-rw-   0        0        0      733 2024-06-01 10:16:33.000000 jinjyaml-0.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1548 2023-06-13 10:06:00.000000 jinjyaml-0.4/LICENSE
--rw-rw-rw-   0        0        0      127 2024-03-15 09:06:58.000000 jinjyaml-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4855 2024-06-01 10:20:21.262909 jinjyaml-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3181 2024-03-15 09:06:58.000000 jinjyaml-0.4/README.md
--rw-rw-rw-   0        0        0     2145 2024-06-01 10:20:06.000000 jinjyaml-0.4/pyproject.toml
--rw-rw-rw-   0        0        0      194 2024-06-01 10:16:23.000000 jinjyaml-0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 10:20:21.264975 jinjyaml-0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 10:20:21.211531 jinjyaml-0.4/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 10:20:21.254154 jinjyaml-0.4/src/jinjyaml/
--rw-rw-rw-   0        0        0      492 2024-06-01 10:16:23.000000 jinjyaml-0.4/src/jinjyaml/__init__.py
--rw-rw-rw-   0        0        0      422 2024-06-01 10:20:20.000000 jinjyaml-0.4/src/jinjyaml/_version.py
--rw-rw-rw-   0        0        0     1725 2024-06-01 10:16:23.000000 jinjyaml-0.4/src/jinjyaml/constructor.py
--rw-rw-rw-   0        0        0      286 2024-06-01 10:16:23.000000 jinjyaml-0.4/src/jinjyaml/data.py
--rw-rw-rw-   0        0        0     4174 2024-06-01 10:16:23.000000 jinjyaml-0.4/src/jinjyaml/functions.py
--rw-rw-rw-   0        0        0        0 2024-06-01 10:16:23.000000 jinjyaml-0.4/src/jinjyaml/py.typed
--rw-rw-rw-   0        0        0     1108 2024-06-01 10:16:23.000000 jinjyaml-0.4/src/jinjyaml/representer.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:20:21.260909 jinjyaml-0.4/src/jinjyaml.egg-info/
--rw-rw-rw-   0        0        0      260 2024-06-01 10:20:21.000000 jinjyaml-0.4/src/jinjyaml.egg-info/SOURCES.txt
+drwxrwxrwx   0        0        0        0 2024-03-15 09:45:15.604319 jinjyaml-0.4rc1/
+-rw-rw-rw-   0        0        0      188 2023-06-13 10:06:00.000000 jinjyaml-0.4rc1/AUTHORS.md
+-rw-rw-rw-   0        0        0      565 2024-03-15 09:09:00.000000 jinjyaml-0.4rc1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1548 2023-06-13 10:06:00.000000 jinjyaml-0.4rc1/LICENSE
+-rw-rw-rw-   0        0        0      127 2024-03-15 09:06:58.000000 jinjyaml-0.4rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4858 2024-03-15 09:45:15.601318 jinjyaml-0.4rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     3181 2024-03-15 09:06:58.000000 jinjyaml-0.4rc1/README.md
+-rw-rw-rw-   0        0        0     2138 2024-03-15 09:09:00.000000 jinjyaml-0.4rc1/pyproject.toml
+-rw-rw-rw-   0        0        0      189 2024-03-15 09:09:00.000000 jinjyaml-0.4rc1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-03-15 09:45:15.605322 jinjyaml-0.4rc1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-15 09:45:15.532319 jinjyaml-0.4rc1/src/
+drwxrwxrwx   0        0        0        0 2024-03-15 09:45:15.588343 jinjyaml-0.4rc1/src/jinjyaml/
+-rw-rw-rw-   0        0        0      410 2024-03-15 09:08:49.000000 jinjyaml-0.4rc1/src/jinjyaml/__init__.py
+-rw-rw-rw-   0        0        0      425 2024-03-15 09:45:14.000000 jinjyaml-0.4rc1/src/jinjyaml/_version.py
+-rw-rw-rw-   0        0        0     1691 2024-03-15 09:08:49.000000 jinjyaml-0.4rc1/src/jinjyaml/_yaml_types.py
+-rw-rw-rw-   0        0        0     1953 2024-03-15 09:08:49.000000 jinjyaml-0.4rc1/src/jinjyaml/_yaml_types_backward.py
+-rw-rw-rw-   0        0        0     1444 2024-03-15 09:08:49.000000 jinjyaml-0.4rc1/src/jinjyaml/constructor.py
+-rw-rw-rw-   0        0        0      250 2024-03-15 09:08:49.000000 jinjyaml-0.4rc1/src/jinjyaml/data.py
+-rw-rw-rw-   0        0        0     4175 2024-03-15 09:09:00.000000 jinjyaml-0.4rc1/src/jinjyaml/functions.py
+-rw-rw-rw-   0        0        0      804 2024-03-15 09:08:49.000000 jinjyaml-0.4rc1/src/jinjyaml/representer.py
+drwxrwxrwx   0        0        0        0 2024-03-15 09:45:15.599319 jinjyaml-0.4rc1/src/jinjyaml.egg-info/
+-rw-rw-rw-   0        0        0      303 2024-03-15 09:45:15.000000 jinjyaml-0.4rc1/src/jinjyaml.egg-info/SOURCES.txt
```

### Comparing `jinjyaml-0.4/LICENSE` & `jinjyaml-0.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjyaml-0.4/PKG-INFO` & `jinjyaml-0.4rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjyaml
-Version: 0.4
+Version: 0.4rc1
 Summary: Application specific YAML tag of Jinja2 template
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://pypi.org/project/jinjyaml/
 Project-URL: documentation, https://jinjyaml.readthedocs.io/
 Project-URL: repository, https://github.com/tanbro/jinjyaml
 Project-URL: changelog, https://github.com/tanbro/jinjyaml/blob/master/CHANGELOG.md
```

### Comparing `jinjyaml-0.4/README.md` & `jinjyaml-0.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `jinjyaml-0.4/pyproject.toml` & `jinjyaml-0.4rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -54,13 +54,16 @@
 documentation = "https://jinjyaml.readthedocs.io/"
 repository = "https://github.com/tanbro/jinjyaml"
 changelog = "https://github.com/tanbro/jinjyaml/blob/master/CHANGELOG.md"
 
 [tool.setuptools.packages.find]
 where = ["src"] # list of folders that contain the packages (["."] by default)
 
-[tool.setuptools.package-data]
-pyyaml_include = ["jinjyaml/py.typed"]
-
 [tool.setuptools_scm]
 # version_scheme = "guess-next-dev"    # guess-next-dev or post-release
 write_to = "src/jinjyaml/_version.py"
+
+[tool.black]
+line-length = 128
+
+[tool.isort]
+profile = "black"
```

### Comparing `jinjyaml-0.4/src/jinjyaml/functions.py` & `jinjyaml-0.4rc1/src/jinjyaml/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, Any, Mapping, MutableMapping, MutableSequence, Optional, Sequence, Type, Union
+import sys
+from typing import Any, Mapping, MutableMapping, MutableSequence, Optional, Sequence
 
 import jinja2
 import yaml
 
 from .data import Data
 
-if TYPE_CHECKING:  # pragma: no cover
-    from yaml.cyaml import _CLoader
-    from yaml.loader import _Loader
+if sys.version_info < (3, 12):  # pragma: no cover
+    from ._yaml_types_backward import TYamlLoaderTypes
+else:  # pragma: no cover
+    from ._yaml_types import TYamlLoaderTypes
 
 
 __all__ = ["extract"]
 
 
 def extract(
     obj: Any,
-    loader_type: Type[Union[_Loader, _CLoader]],
+    loader_type: TYamlLoaderTypes,
     env: Optional[jinja2.Environment] = None,
     context: Optional[Mapping[str, Any]] = None,
     inplace: bool = False,
 ) -> Any:
     """Recursively render and parse template tag objects in a YAML doc-tree.
 
     Args:
```

