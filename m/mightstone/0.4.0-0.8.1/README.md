# Comparing `tmp/mightstone-0.4.0.tar.gz` & `tmp/mightstone-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mightstone-0.4.0.tar", max compression
+gzip compressed data, was "mightstone-0.8.1.tar", max compression
```

## Comparing `mightstone-0.4.0.tar` & `mightstone-0.8.1.tar`

### file list

```diff
@@ -1,40 +1,51 @@
--rw-r--r--   0        0        0     1078 2023-02-26 22:30:20.902617 mightstone-0.4.0/LICENSE
--rw-r--r--   0        0        0     1341 2023-02-26 22:30:20.902617 mightstone-0.4.0/README.md
--rw-r--r--   0        0        0     2902 2023-02-26 22:30:22.094681 mightstone-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      146 2023-02-26 22:30:22.066680 mightstone-0.4.0/src/mightstone/__init__.py
--rw-r--r--   0        0        0      266 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/app.py
--rw-r--r--   0        0        0     1196 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/__init__.py
--rw-r--r--   0        0        0     2017 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/__init__.py
--rw-r--r--   0        0        0     5983 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/async_file_obj.py
--rw-r--r--   0        0        0      907 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/async_reader.py
--rw-r--r--   0        0        0     1054 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/async_writer.py
--rw-r--r--   0        0        0      189 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/codecs/__init__.py
--rw-r--r--   0        0        0      129 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/codecs/bzip2_codec.py
--rw-r--r--   0        0        0      656 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/codecs/gzip_codec.py
--rw-r--r--   0        0        0      132 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/codecs/lzma_codec.py
--rw-r--r--   0        0        0      298 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/ass/compressor/codecs/none_codec.py
--rw-r--r--   0        0        0   108168 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/assets/LiberationMono-Regular.ttf
--rw-r--r--   0        0        0        0 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/assets/__init__.py
--rw-r--r--   0        0        0     1490 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/cli/__init__.py
--rw-r--r--   0        0        0       38 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/cli/__main__.py
--rw-r--r--   0        0        0     1129 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/cli/utils.py
--rw-r--r--   0        0        0     1068 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/containers.py
--rw-r--r--   0        0        0      158 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/core.py
--rw-r--r--   0        0        0       75 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/py.typed
--rw-r--r--   0        0        0        0 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/rule/__init__.py
--rw-r--r--   0        0        0     6917 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/rule/color.py
--rw-r--r--   0        0        0    14720 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/rule/cr.py
--rw-r--r--   0        0        0     1256 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/__init__.py
--rw-r--r--   0        0        0    17507 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/cardconjurer/__init__.py
--rw-r--r--   0        0        0     1379 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/cardconjurer/commands.py
--rw-r--r--   0        0        0     8903 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/cardconjurer/models.py
--rw-r--r--   0        0        0    19641 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/edhrec/__init__.py
--rw-r--r--   0        0        0     3954 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/edhrec/commands.py
--rw-r--r--   0        0        0    15784 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/mtgjson/__init__.py
--rw-r--r--   0        0        0     1681 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/mtgjson/commands.py
--rw-r--r--   0        0        0    67243 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/mtgjson/models.py
--rw-r--r--   0        0        0    17934 2023-02-26 22:30:20.918618 mightstone-0.4.0/src/mightstone/services/scryfall/__init__.py
--rw-r--r--   0        0        0     4589 2023-02-26 22:30:20.922618 mightstone-0.4.0/src/mightstone/services/scryfall/commands.py
--rw-r--r--   0        0        0    32702 2023-02-26 22:30:20.922618 mightstone-0.4.0/src/mightstone/services/scryfall/models.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 mightstone-0.4.0/setup.py
--rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 mightstone-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-02-02 11:49:59.972255 mightstone-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3455 2024-05-31 11:18:53.904196 mightstone-0.8.1/README.md
+-rw-r--r--   0        0        0     3849 2024-06-01 09:04:06.492341 mightstone-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-08-07 15:16:20.206866 mightstone-0.8.1/src/mightstone/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-31 20:29:47.097147 mightstone-0.8.1/src/mightstone/app.py
+-rw-r--r--   0        0        0     2067 2024-05-31 20:29:47.097814 mightstone-0.8.1/src/mightstone/ass/__init__.py
+-rw-r--r--   0        0        0     2074 2024-05-31 20:29:47.100839 mightstone-0.8.1/src/mightstone/ass/compressor/__init__.py
+-rw-r--r--   0        0        0     6269 2023-04-01 22:58:25.830003 mightstone-0.8.1/src/mightstone/ass/compressor/async_file_obj.py
+-rw-r--r--   0        0        0      907 2023-02-16 12:35:10.586599 mightstone-0.8.1/src/mightstone/ass/compressor/async_reader.py
+-rw-r--r--   0        0        0     1054 2023-02-16 12:35:10.578896 mightstone-0.8.1/src/mightstone/ass/compressor/async_writer.py
+-rw-r--r--   0        0        0      189 2023-02-12 07:22:10.775623 mightstone-0.8.1/src/mightstone/ass/compressor/codecs/__init__.py
+-rw-r--r--   0        0        0      129 2023-02-12 07:22:10.777341 mightstone-0.8.1/src/mightstone/ass/compressor/codecs/bzip2_codec.py
+-rw-r--r--   0        0        0      657 2024-05-31 11:18:53.926981 mightstone-0.8.1/src/mightstone/ass/compressor/codecs/gzip_codec.py
+-rw-r--r--   0        0        0      132 2023-02-12 07:39:45.049398 mightstone-0.8.1/src/mightstone/ass/compressor/codecs/lzma_codec.py
+-rw-r--r--   0        0        0      298 2023-02-12 07:22:10.781095 mightstone-0.8.1/src/mightstone/ass/compressor/codecs/none_codec.py
+-rw-r--r--   0        0        0   108168 2023-02-20 06:22:43.915164 mightstone-0.8.1/src/mightstone/assets/LiberationMono-Regular.ttf
+-rw-r--r--   0        0        0        0 2023-02-20 06:22:43.915368 mightstone-0.8.1/src/mightstone/assets/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-01 22:58:25.830444 mightstone-0.8.1/src/mightstone/cli/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-01 22:58:25.831025 mightstone-0.8.1/src/mightstone/cli/__main__.py
+-rw-r--r--   0        0        0     2470 2024-05-31 20:29:47.102923 mightstone-0.8.1/src/mightstone/cli/commands.py
+-rw-r--r--   0        0        0      500 2024-05-31 20:29:47.104553 mightstone-0.8.1/src/mightstone/cli/models.py
+-rw-r--r--   0        0        0     1129 2023-02-16 19:49:47.726501 mightstone-0.8.1/src/mightstone/cli/utils.py
+-rw-r--r--   0        0        0      142 2024-05-31 20:29:47.105058 mightstone-0.8.1/src/mightstone/common.py
+-rw-r--r--   0        0        0     4193 2024-05-31 20:29:47.105646 mightstone-0.8.1/src/mightstone/config.py
+-rw-r--r--   0        0        0     5830 2024-05-31 20:29:47.108563 mightstone-0.8.1/src/mightstone/containers.py
+-rw-r--r--   0        0        0     2674 2024-05-31 20:29:47.109506 mightstone-0.8.1/src/mightstone/core.py
+-rw-r--r--   0        0        0       75 2023-02-02 11:50:00.054239 mightstone-0.8.1/src/mightstone/py.typed
+-rw-r--r--   0        0        0        0 2023-02-02 12:00:25.869231 mightstone-0.8.1/src/mightstone/rule/__init__.py
+-rw-r--r--   0        0        0     7276 2024-05-31 20:29:47.110084 mightstone-0.8.1/src/mightstone/rule/color.py
+-rw-r--r--   0        0        0     1440 2024-05-31 20:29:47.110680 mightstone-0.8.1/src/mightstone/services/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-01 22:58:25.838207 mightstone-0.8.1/src/mightstone/services/cardconjurer/__init__.py
+-rw-r--r--   0        0        0    18909 2024-05-31 20:29:47.111488 mightstone-0.8.1/src/mightstone/services/cardconjurer/api.py
+-rw-r--r--   0        0        0      989 2024-05-31 11:18:53.927635 mightstone-0.8.1/src/mightstone/services/cardconjurer/commands.py
+-rw-r--r--   0        0        0     9312 2024-05-31 20:29:47.112303 mightstone-0.8.1/src/mightstone/services/cardconjurer/models.py
+-rw-r--r--   0        0        0       89 2023-04-01 22:58:25.839626 mightstone-0.8.1/src/mightstone/services/edhrec/__init__.py
+-rw-r--r--   0        0        0    15203 2024-05-31 20:29:47.113046 mightstone-0.8.1/src/mightstone/services/edhrec/api.py
+-rw-r--r--   0        0        0     3963 2024-05-31 11:18:53.928349 mightstone-0.8.1/src/mightstone/services/edhrec/commands.py
+-rw-r--r--   0        0        0     6166 2024-05-31 20:29:47.113718 mightstone-0.8.1/src/mightstone/services/edhrec/models.py
+-rw-r--r--   0        0        0       82 2023-04-01 22:58:25.842801 mightstone-0.8.1/src/mightstone/services/mtgjson/__init__.py
+-rw-r--r--   0        0        0    20810 2024-05-31 20:29:47.114643 mightstone-0.8.1/src/mightstone/services/mtgjson/api.py
+-rw-r--r--   0        0        0     1723 2023-04-01 22:58:25.843398 mightstone-0.8.1/src/mightstone/services/mtgjson/commands.py
+-rw-r--r--   0        0        0    91075 2024-05-31 20:29:47.115706 mightstone-0.8.1/src/mightstone/services/mtgjson/models.py
+-rw-r--r--   0        0        0      158 2023-04-01 22:58:25.844335 mightstone-0.8.1/src/mightstone/services/scryfall/__init__.py
+-rw-r--r--   0        0        0    20566 2024-05-31 20:29:47.116477 mightstone-0.8.1/src/mightstone/services/scryfall/api.py
+-rw-r--r--   0        0        0     4454 2023-04-01 22:58:25.844967 mightstone-0.8.1/src/mightstone/services/scryfall/commands.py
+-rw-r--r--   0        0        0    34863 2024-05-31 20:29:47.117491 mightstone-0.8.1/src/mightstone/services/scryfall/models.py
+-rw-r--r--   0        0        0       69 2023-04-01 22:58:25.845855 mightstone-0.8.1/src/mightstone/services/wotc/__init__.py
+-rw-r--r--   0        0        0     3665 2024-05-31 20:29:47.118236 mightstone-0.8.1/src/mightstone/services/wotc/api.py
+-rw-r--r--   0        0        0    13510 2024-05-31 20:29:47.118926 mightstone-0.8.1/src/mightstone/services/wotc/models.py
+-rw-r--r--   0        0        0     3027 2024-05-31 20:29:47.119529 mightstone-0.8.1/src/mightstone/storage.py
+-rw-r--r--   0        0        0     5505 1970-01-01 00:00:00.000000 mightstone-0.8.1/PKG-INFO
```

### Comparing `mightstone-0.4.0/LICENSE` & `mightstone-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mightstone-0.4.0/pyproject.toml` & `mightstone-0.8.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "mightstone"
-version = "0.4.0"
+version = "0.8.1"
 description = "A library manage all things Magic The Gathering related in python"
 authors = ["Guillaume Boddaert"]
 # Use identifier from https://spdx.org/licenses/
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/guibod/mightstone"
 repository = "https://github.com/guibod/mightstone"
 documentation = "https://github.com/guibod/mightstone/blob/master/README.md"
 classifiers = [
     # https://pypi.org/classifiers/
     "Environment :: Console",
-    "Development Status :: 1 - Planning",
+    "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.9",
     "Topic :: Games/Entertainment :: Board Games",
     "Topic :: Software Development :: Libraries",
     "Typing :: Typed",
     "Framework :: AsyncIO"
 ]
 
@@ -24,34 +24,51 @@
 # If you publish you package on PyPI, these will appear in the Project Links section.
 "Bug Tracker" = "https://github.com/guibod/mightstone/issues"
 
 [tool.poetry.scripts]
 mightstone = "mightstone.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.9.0"
+python = ">=3.9.0,<3.12"
 click = "^8.0.1"
-beanie = "^1.17.0"
+beanie = "1.26.0"
+pydantic = "2.7.2"
 ordered-set = "^4.1.0"
-pytest = "^7.2.1"
 python-slugify = "^8.0.0"
-aiofiles = "^22.1.0"
-nest-asyncio = "^1.5.6"
+aiofiles = "^23.2.1"
 asyncstdlib = "^3.10.5"
 ijson = "^3.2.0.post0"
-aiostream = "^0.4.5"
-aiosqlite = "^0.18.0"
 appdirs = "^1.4.4"
 requests = "^2.28.2"
-pillow = "^9.4.0"
+pillow = ">=9.4,<11.0"
 cairosvg = "^2.6.0"
 dependency-injector = "^4.41.0"
 logging = "^0.4.9.6"
-httpx = "^0.23.3"
-httpx-cache = "^0.7.0"
+httpx = "^0.27.0"
+httpx-cache = "^0.13.0"
+asgiref = "^3.6.0"
+orjson-pydantic = "^3.6.7"
+motor = "^3.1.1"
+pymongo-inmemory = "^0.4.2"
+pylint-pydantic = "0.3.2"
+pydantic-settings = "^2.2.1"
+pydantic-extra-types = "^2.7.0"
+
+[tool.poetry.group.types]
+optional = true
+
+[tool.poetry.group.types.dependencies]
+types-aiofiles = "^23.2.0.0"
+types-pillow = "^9.4.0.17"
+types-pyyaml = "^6.0.12.8"
+types-pygments = "^2.14.0.5"
+types-python-slugify = "^8.0.0.1"
+types-setuptools = "^67.6.0.5"
+types-orjson = "^3.6.2"
+types-toml = "^0.10.8.5"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.0.0"
 autodoc-pydantic = "^1.8.0"
@@ -61,31 +78,32 @@
 [tool.poetry.group.release]
 optional = true
 
 [tool.poetry.group.release.dependencies]
 python-semantic-release = "^7.33.1"
 
 [tool.poetry.group.dev.dependencies]
+pytest = "^8.2.1"
 bandit = "^1.6.2"
-black = "^23.0"
+black = ">=23,<25"
 isort= "^5.0.8"
 flake8 = "^5.0.4"
 jedi-language-server = "^0.22.0"
 pylint = "^2.6.0"
-pytest = "^7.0.1"
 pytest-cov = "^4.0"
 pytest-xdist = "^2.5.0"
 vulture = "^2.3"
-mypy = "^0.982"
-pyinstaller = "^4.1"
-pylint-pydantic = "^0.1.6"
+mypy = "^1.10"
+pyinstaller = ">=4.1,<6.0"
 toml = "^0.10.2"
 pytest-asyncio = "^0.20.3"
 pixelmatch = "^0.3.0"
 
+
+
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
@@ -104,16 +122,40 @@
 [tool.bandit]
 
 [tool.pytest.ini_options]
 # Example
 filterwarnings = [
     "ignore::DeprecationWarning:moto.*:",
     "ignore::DeprecationWarning:boto.*:",
+    "ignore::pytest.PytestUnraisableExceptionWarning"
 ]
+#markers = [
+#    'skip_remote_api:Skips remote api calls on CI',
+#    'skip_remote_api_2:Skips remote api calls on CI (same thing but i don’t know how to relative import)'
+#]
 
 [tool.semantic_release]
 version_variable = ["src/mightstone/__init__.py:__version_", "docs/source/conf.py:version"]
-version_toml = "pyproject.toml:tool.poetry.version"
+version_toml = ["pyproject.toml:tool.poetry.version"]
 branch = "main"
 build_command = "pip install poetry && make build"
 upload_to_pypi = true
-upload_to_release = true
+upload_to_vcs_release = true
+
+[tool.mypy]
+python_version = "3.9"
+
+[[tool.mypy.overrides]]
+module = [
+    "httpx_cache",
+    "ijson",
+    "appdirs",
+    "cairosvg",
+    "beanita",
+    "beanita.db",
+    "motor",
+    "motor.motor_asyncio",
+    "pymongo_inmemory",
+    "pymongo_inmemory.context"
+]
+ignore_missing_imports = true
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mightstone-0.4.0/src/mightstone/ass/compressor/__init__.py` & `mightstone-0.8.1/src/mightstone/ass/compressor/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 This code was extracted from the asyncstream library that is licenseless and
 seems an abandoned project
 
 see: https://github.com/chimpler/async-stream
 """
-from typing import Iterable, Optional
+
+from typing import Any, AsyncIterable, Iterable, Optional, Union
 
 from mightstone.ass.compressor.async_file_obj import AsyncFileObj
 from mightstone.ass.compressor.async_reader import AsyncReader
 from mightstone.ass.compressor.async_writer import AsyncWriter
 
 
 def open(
-    afd: str,
+    afd: Union[AsyncIterable[bytes], Any],
     mode=None,
     encoding=None,
     compression=None,
     *args,
     **kwargs,
 ):
     if encoding is None and compression is None:
```

### Comparing `mightstone-0.4.0/src/mightstone/ass/compressor/async_file_obj.py` & `mightstone-0.8.1/src/mightstone/ass/compressor/async_file_obj.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from typing import AsyncIterable, Optional
+from typing import AsyncIterable, List, Optional, Union
+
+import aiofiles.threadpool.binary
 
 from mightstone.ass.compressor.codecs import error_import_usage
 
 
 class AsyncFileObj(object):
     MODE_DEFAULT = 0
     MODE_BINARY = 1
     MODE_TEXT = 2
 
     def __init__(
         self,
-        afd,
+        afd: Union[
+            AsyncIterable[bytes], aiofiles.threadpool.binary.AsyncBufferedReader
+        ],
         mode,
         compressor,
         decompressor,
         ignore_header=False,
         buffer_size=1024 * 1024,
     ):
         self._afd = afd
@@ -22,15 +26,15 @@
         self._compressor = compressor
         self._decompressor = decompressor
         self._ignore_header = ignore_header
         self._header = None
         self._buffer = b""
         self._buffer_size = buffer_size
         self._eof = False
-        self._lines = []
+        self._lines: List[bytes] = []
         self._index = 0
         self._filename = None
         self._has_flushed = True
         self._is_closed = False
 
         if mode is None:
             self._file_type = self.MODE_BINARY
@@ -52,19 +56,22 @@
         if n == 0:
             # Do not read from parent iterator
             return b""
 
         buffer_size = n if n else 1024 * 1024
         if isinstance(self._afd, AsyncIterable):
             async for data in self._afd:
-                self._buffer += self._decompressor.decompress(data)
-                if len(self._buffer) >= buffer_size and n is not None:
-                    result = self._buffer[:buffer_size]
-                    self._buffer = self._buffer[buffer_size:]
-                    return result
+                try:
+                    self._buffer += self._decompressor.decompress(data)
+                    if len(self._buffer) >= buffer_size and n is not None:
+                        result = self._buffer[:buffer_size]
+                        self._buffer = self._buffer[buffer_size:]
+                        return result
+                except GeneratorExit:
+                    return b""
 
             if hasattr(self._decompressor, "flush"):
                 data = self._decompressor.flush()
                 if data:
                     self._buffer += data
             result = self._buffer
             self._buffer = b""
@@ -91,15 +98,15 @@
                         self._buffer += data
                 self._eof = True
 
     async def _write(self, buffer: bytes):
         self._has_flushed = False
         compressed_data = self._compressor.compress(buffer)
         if compressed_data:
-            return await self._afd.write(compressed_data)
+            return await self._afd.write(compressed_data)  # type: ignore
         else:
             return 0
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
```

### Comparing `mightstone-0.4.0/src/mightstone/ass/compressor/async_reader.py` & `mightstone-0.8.1/src/mightstone/ass/compressor/async_reader.py`

 * *Files identical despite different names*

### Comparing `mightstone-0.4.0/src/mightstone/ass/compressor/async_writer.py` & `mightstone-0.8.1/src/mightstone/ass/compressor/async_writer.py`

 * *Files identical despite different names*

### Comparing `mightstone-0.4.0/src/mightstone/ass/compressor/codecs/gzip_codec.py` & `mightstone-0.8.1/src/mightstone/ass/compressor/codecs/gzip_codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         compress_level,  # level: 0-9
         zlib.DEFLATED,  # method: must be DEFLATED
         16 + zlib.MAX_WBITS,  # window size in bits:
         #   -15..-8: negate, suppress header
         #   8..15: normal
         #   16..30: subtract 16, gzip header
         zlib.DEF_MEM_LEVEL,  # mem level: 1..8/9
-        0  # strategy:
+        0,  # strategy:
         #   0 = Z_DEFAULT_STRATEGY
         #   1 = Z_FILTERED
         #   2 = Z_HUFFMAN_ONLY
         #   3 = Z_RLE
         #   4 = Z_FIXED
     )
```

### Comparing `mightstone-0.4.0/src/mightstone/assets/LiberationMono-Regular.ttf` & `mightstone-0.8.1/src/mightstone/assets/LiberationMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `mightstone-0.4.0/src/mightstone/cli/utils.py` & `mightstone-0.8.1/src/mightstone/cli/utils.py`

 * *Files identical despite different names*

### Comparing `mightstone-0.4.0/src/mightstone/rule/color.py` & `mightstone-0.8.1/src/mightstone/rule/color.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,89 @@
 import itertools
 import logging
 from collections import Counter
-from typing import Iterable, Iterator, List, Mapping, Sequence, Union
+from typing import (
+    Annotated,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Union,
+    overload,
+)
 
 from ordered_set import OrderedSet
-from pydantic import constr, validator
+from pydantic import StringConstraints
 
 from mightstone.core import MightstoneModel
 
 logger = logging.getLogger(__name__)
 
+ColorGlyph = Annotated[
+    str, StringConstraints(min_length=1, max_length=1, to_lower=True)
+]
+
 
 class Color(MightstoneModel):
-    symbol: constr(to_lower=True, min_length=1, max_length=1)
+    symbol: ColorGlyph
 
     def __str__(self):
         return f"{{{self.symbol.upper()}}}"
 
     def __repr__(self):
         return f"Color({self.symbol})"
 
 
-class ColorPie(MightstoneModel, Sequence[Color]):
-    colors: List[Color]
-
-    @validator("colors")
-    def sanitize(cls, colors: Iterable[Color]) -> [Color]:
+class ColorPie(Sequence[Color]):
+    def __init__(self, colors: Iterable[Color]):
         if not all(isinstance(x, Color) for x in colors):
             raise ValueError("Please provide a Color object iterable")
 
         duplicates = [k for k, v in Counter(list(colors)).items() if v > 1]
         if len(duplicates):
             duplicates_as_string = ",".join(map(str, duplicates))
             raise ValueError(
                 f"A color pie cannot hold the same color twice. {duplicates_as_string}"
             )
 
         # TODO: search duplicates color values
-        return list(colors)
+        self.colors = list(colors)
 
-    def __getitem__(self, i: Union[int, str]):
+    def __getitem__(self, i: Union[int, slice, Union[int, str]]):
         if isinstance(i, int):
             return self.colors[i]
 
         try:
             return next(color for color in self.colors if color.symbol == i)
         except StopIteration:
             raise KeyError(f"{i} not found in {self}")
 
     def __len__(self) -> int:
         return len(self.colors)
 
     def __iter__(self) -> Iterator[Color]:
-        return iter(self.colors)
+        for color in self.colors:
+            yield color
 
     def shift(self, color: Color, step: int = 1) -> Color:
         return self.colors[(step + self.index(color)) % len(self.colors)]
 
     def __hash__(self):
         return hash(tuple(self))
 
     def parse(self, identity_as_string: str) -> "Identity":
         colors = []
         for letter in identity_as_string:
             colors.append(self[letter])
         return Identity(self, colors)
 
-    def combinations(self) -> ["Identity"]:
+    def combinations(self) -> List["Identity"]:
         """
         A mathematical computation of all possible combinations of colors
         This will not provide a proper color pie centric combination though
         and cannot be used to provide a complete identity map that would
         build the red enemy guild (Boros) as rw, instead of wr in this case
         """
         return [
@@ -116,18 +129,18 @@
         return f"ColorPie({self.colors})"
 
 
 class Identity(Sequence[Color]):
     def __init__(self, pie: ColorPie, colors: Iterable[Color]):
         self.pie = pie
         self.colors = OrderedSet(colors)
-        self._name = None
-        self.aliases = []
+        self._name = ""
+        self.aliases: List[str] = []
 
-    def describe(self, name: str = None, aliases: [str] = None):
+    def describe(self, name: Optional[str] = None, aliases: Optional[List[str]] = None):
         if name:
             self._name = name
         if aliases:
             self.aliases.extend(aliases)
 
     @property
     def name(self):
@@ -155,30 +168,36 @@
 
     def __str__(self):
         return f"{self.name}"
 
     def __repr__(self):
         return f"Identity({self.canonical})"
 
-    def __getitem__(self, i: int) -> Color:
+    @overload
+    def __getitem__(self, i: int) -> Color: ...
+
+    @overload
+    def __getitem__(self, i: slice) -> OrderedSet[Color]: ...
+
+    def __getitem__(self, i: Union[int, slice]) -> Union[Color, OrderedSet[Color]]:
         return self.colors.__getitem__(i)
 
     def __len__(self):
         return len(self.colors)
 
-    def __eq__(self, other: "Identity"):
-        try:
-            return other.checksum() == self.checksum()
-        except TypeError:
-            return False
+    def __eq__(self, other: object):
+        if not isinstance(other, Identity):
+            return NotImplemented
+
+        return other.checksum() == self.checksum()
 
 
 class IdentityMap(Mapping[int, Identity]):
     def __init__(self, pie: ColorPie):
-        self.map = {}
+        self.map: Dict[int, Identity] = {}
         self.pie = pie
 
     def add(self, ident: Identity):
         """
         Appends an identity to the map
         No addition if the identity already exists
         """
@@ -204,15 +223,15 @@
                     return identity
 
         raise KeyError
 
     def __len__(self) -> int:
         return self.map.__len__()
 
-    def __iter__(self) -> Iterator[str]:
+    def __iter__(self) -> Iterator[int]:
         return self.map.__iter__()
 
 
 class ColorAffinity(MightstoneModel):
     """
     When talking about which colors get which evergreen creature keywords,
     R&D tends to talk about a system called "primary/secondary/tertiary".
```

### Comparing `mightstone-0.4.0/src/mightstone/rule/cr.py` & `mightstone-0.8.1/src/mightstone/services/wotc/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-import asyncio
-import logging
 import re
 from collections import defaultdict
-from datetime import date, datetime, timedelta
+from datetime import datetime
 from io import StringIO
 from itertools import takewhile
-from typing import Dict, List, Mapping, TextIO
+from typing import Any, DefaultDict, Dict, List, Mapping, Optional, TextIO
 
-import httpx
-import requests
+from pydantic import ConfigDict, GetCoreSchemaHandler
+from pydantic_core import CoreSchema, core_schema
 
-from mightstone.core import MightstoneModel
-
-# TODO: get rid of requests dependency, use async client
-
-
-logger = logging.getLogger(__name__)
+from mightstone.core import MightstoneDocument, MightstoneModel
 
 
 class RuleRef(str):
     """
     Rules reference use the same pattern with a rule number
 
     <rule>[.<sub_rule>[<letter>]][<trailing_dot>]
@@ -38,14 +31,20 @@
         r"(?P<reference>"
         r"(?P<rule>\d{3})"
         r"(\.((?P<sub_rule>\d+)(?P<letter>[a-z])?))?"
         r"(?P<trailing_dot>\.)?"
         r")"
     )
 
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        return core_schema.no_info_after_validator_function(cls, handler(str))
+
     def __new__(cls, value, *args, **kwargs):
         return super(RuleRef, cls).__new__(cls, value)
 
     def __init__(self, value):
         res = self.regex.match(value)
         if not res:
             raise ValueError(f"{self} is not a valid reference")
@@ -59,15 +58,17 @@
         if res.group("sub_rule"):
             self.sub_rule = int(res.group("sub_rule"))
         self.letter = res.group("letter")
         self.canonical = self.build(self.rule, self.sub_rule, self.letter)
         self.section = int(res.group("rule")[0])
 
     @classmethod
-    def build(cls, rule: int, sub_rule: int = None, letter: str = None):
+    def build(
+        cls, rule: int, sub_rule: Optional[int] = None, letter: Optional[str] = None
+    ):
         out = str(rule)
         if sub_rule:
             out += f".{sub_rule}"
             if letter:
                 out += f"{letter}"
         return out
 
@@ -131,41 +132,53 @@
     """
     A string than can contain reference to rule
     """
 
     see_rule = re.compile(r"rule " + RuleRef.regex.pattern)
     see_section = re.compile(r"section " + SectionRef.regex.pattern)
 
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        return core_schema.no_info_after_validator_function(cls, handler(str))
+
     def __new__(cls, value, *args, **kwargs):
         return super(RuleText, cls).__new__(cls, value)
 
     def __init__(self, value):
         self.refs = []
         for item in self.see_rule.findall(value):
             self.refs.append(RuleRef(item[0]))
         for item in self.see_section.findall(value):
             self.refs.append(SectionRef(item[0]))
 
 
 class Example(str):
     pattern = re.compile(r"(?P<example>Example: (?P<text>.+))")
 
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        return core_schema.no_info_after_validator_function(cls, handler(str))
+
     def __new__(cls, value, *args, **kwargs):
         return super(Example, cls).__new__(cls, value)
 
     def __init__(self, value):
         res = self.pattern.match(value)
         if not res:
             raise ValueError("String is not an example")
         self.text = RuleText(res.group("text"))
 
 
 class Rule(MightstoneModel):
-    ref: RuleRef = None
-    text: RuleText = None
+    ref: RuleRef
+    text: RuleText
     examples: List[Example] = []
 
     @classmethod
     def parse_text(cls, value):
         pattern = re.compile(RuleRef.regex.pattern + r"\s+(?P<text>\w+.*)")
 
         res = pattern.match(value)
@@ -179,27 +192,37 @@
 
 class Effectiveness(str):
     pattern = re.compile(
         r"(?P<effective>These rules are effective as of"
         r" (?P<date>(?P<month>\w+) (?P<day>\d+), (?P<year>\d{4})).)"
     )
 
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        return core_schema.no_info_after_validator_function(cls, handler(str))
+
     def __new__(cls, value, *args, **kwargs):
         return super(Effectiveness, cls).__new__(cls, value)
 
     def __init__(self, value):
         res = self.pattern.match(value)
         if not res:
-            raise ValueError("String is not an example")
+            raise ValueError("String is not a valid effectiveness string")
         self.date = datetime.strptime(res.group("date"), "%B %d, %Y").date()
 
 
-class Ruleset(MightstoneModel, Mapping):
+class Ruleset(MightstoneModel):
     rules: Dict[str, Rule] = dict()
-    last_rule: Rule = None
+    last_rule: Optional[Rule] = None
+
+    # def __iter__(self) -> Iterator[Rule]:  # type: ignore
+    #     for rule in self.rules.values():
+    #         yield rule
 
     def __getitem__(self, k: str) -> Rule:
         return self.rules[k]
 
     def __len__(self) -> int:
         return len(self.rules)
 
@@ -210,32 +233,38 @@
                 self.rules[rule.ref.canonical] = rule
                 self.last_rule = rule
                 continue
             except ValueError:
                 pass
 
             try:
-                self.rules[self.last_rule.ref.canonical].examples.append(Example(line))
+                if self.last_rule:
+                    self.rules[self.last_rule.ref.canonical].examples.append(
+                        Example(line)
+                    )
                 continue
             except (ValueError, AttributeError):
                 pass
 
     def search(self, string: str):
         return [
             item for item in self.rules.values() if string.lower() in item.text.lower()
         ]
 
-    def range(self, low: str, up: str = None):
+    def range(self, low: str, up: Optional[str] = None):
         low = RuleRef(low)
         if not up:
             up = RuleRef(low).next()
         else:
             up = RuleRef(up)
 
-        return [item for item in self.rules.values() if up > item.ref >= low]
+        if up:
+            return [item for item in self.rules.values() if up > item.ref >= low]
+
+        return [item for item in self.rules.values() if item.ref >= low]
 
     def index(self):
         self.rules = dict(sorted(self.rules.items()))
 
 
 class Term(MightstoneModel):
     term: str
@@ -262,27 +291,28 @@
             or string.lower() in item.description.lower()
         ]
 
     def index(self):
         self.terms = dict(sorted(self.terms.items()))
 
 
-class ComprehensiveRules(MightstoneModel):
-    effective: date = None
+class ComprehensiveRules(MightstoneDocument):
+    effective: Optional[Effectiveness] = None
     ruleset: Ruleset = Ruleset()
     glossary: Glossary = Glossary()
+    model_config = ConfigDict(arbitrary_types_allowed=True)  # type: ignore
 
     def search(self, string):
         found = []
         found.extend(self.ruleset.search(string))
         found.extend(self.glossary.search(string))
         return found
 
     @classmethod
-    def from_text(cls, buffer: TextIO):
+    def parse(cls, buffer: TextIO):
         cr = ComprehensiveRules()
         in_glossary = False
         in_credits = False
         buffer2 = StringIO("\n".join(buffer.read().splitlines()))
 
         for line in buffer2:
             line = line.strip()
@@ -318,107 +348,36 @@
                 continue
 
         cr.ruleset.index()
         cr.glossary.index()
 
         return cr
 
-    @classmethod
-    def from_file(cls, path):
-        with open(path, "r") as f:
-            return cls.from_text(f)
-
-    @classmethod
-    def from_url(cls, url: str):
-        with requests.get(url) as f:
-            f.raise_for_status()
-            try:
-                content = StringIO(f.content.decode("UTF-8"))
-            except UnicodeDecodeError:
-                content = StringIO(f.content.decode("iso-8859-1"))
-
-            return cls.from_text(content)
-
-    @classmethod
-    def from_latest(cls):
-        latest = cls.latest()
-        return cls.from_url(latest)
-
-    @classmethod
-    def latest(cls):
-        pattern = re.compile(r"https://media.wizards.com/.*/MagicComp.+\.txt")
-        with requests.get("https://magic.wizards.com/en/rules") as f:
-            f.raise_for_status()
-            res = pattern.search(f.text)
-            if res:
-                return res.group(0).replace(" ", "%20")
-            raise RuntimeError("Unable to find URL of the last comprehensive rules")
-
-    @classmethod
-    async def explore(cls, f: date, t: date = None, concurrency=3):
-        """
-        AFAIK Wizards don’t support an historic index of previous rules.
-        This method will force try every possible rule using the current format:
-
-        https://media.wizards.com/YYYY/downloads/MagicComp%20Rules%20{YYYY}{MM}{DD}.txt
-        :param f: The min date to scan
-        :param t: The max date to scan (defaults to today)
-        :param concurrency: The max number of concurrent HTTP requests
-        :return: A list of existing rules url
-        """
-        if not t:
-            t = date.today()
-
-        urls = []
-        for n in range(int((t - f).days)):
-            d = f + timedelta(n)
-            urls.append(d.strftime("/%Y/downloads/MagicComp%%20Rules%%20%Y%m%d.txt"))
-            urls.append(d.strftime("/%Y/downloads/MagicCompRules%%20%Y%m%d.txt"))
-        map(lambda x: f"https://media.wizards.com{x}", urls)
-
-        found = []
-        sem = asyncio.Semaphore(concurrency)
-
-        async def test_url(session, url):
-            async with sem:
-                logger.debug("GET %s", url)
-                resp = session.get(url)
-                if resp.status == 200:
-                    logger.info("Found %s", url)
-                    found.append(url)
-
-        async with httpx.Client() as session:
-            tasks = []
-            for url in urls:
-                task = asyncio.ensure_future(test_url(session, url))
-                tasks.append(task)
-            await asyncio.gather(*tasks, return_exceptions=True)
-
-        return found
-
     def diff(self, cr: "ComprehensiveRules"):
         """
         Compare two comprehensive rule set for change in rules and terms
 
         For both, terms and rules, provide a dict for:
          - `added` a dict of added object
          - `changed` a dict of dict (before/after) object
          - `removed` a dict of removed object
 
         :param cr: An other comprehensive rule set to compare
         :return: a dict of changes
         """
-        if cr.effective > self.effective:
+        if cr.effective and self.effective and cr.effective > self.effective:
             older = self
             newer = cr
         else:
             older = cr
             newer = self
 
-        diff = defaultdict(lambda: {"added": {}, "removed": {}, "changed": {}})
+        diff: DefaultDict = defaultdict(
+            lambda: {"added": {}, "removed": {}, "changed": {}}
+        )
 
         new_rules = set(newer.ruleset.rules)
         old_rules = set(older.ruleset.rules)
         moved_from = {}
 
         # Check for inclusion, search for same text, but new index
         for ref in new_rules - old_rules:
```

### Comparing `mightstone-0.4.0/src/mightstone/services/__init__.py` & `mightstone-0.8.1/src/mightstone/services/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import asyncio
+from typing import Optional
 
 import ijson as ijson_module
 from httpx import AsyncClient, BaseTransport
 
-try:
-    ijson = ijson_module.get_backend("yajl2")
-except ImportError:
-    ijson = ijson_module.get_backend("python")
+# try:
+#     ijson = ijson_module.get_backend("yajl2")
+# except ImportError:
+ijson = ijson_module.get_backend("python")
 
 
 class ServiceError(Exception):
     def __init__(self, message, url=None, status=None, data=None, method=None):
         self.message = message
         self.url = url
         self.status = status
@@ -18,31 +19,37 @@
         self.method = method
 
     def __str__(self):
         return "{message} (HTTP:{status} {method} {url})".format(**self.__dict__)
 
 
 class MightstoneHttpClient:
-    base_url = None
+    base_url: str
     """
     Base url of the service (must be a root path such as https://example.com)
     """
     delay = 0
     """
     Induced delay in second between each API call
     """
 
-    def __init__(self, transport: BaseTransport = None):
+    def __init__(self, transport: Optional[BaseTransport] = None):
+        self.transport = transport
+        self.ijson = ijson
+
+    @property
+    def client(self):
+        # See: https://github.com/encode/httpx/issues/2473
         options = {
-            "transport": transport,
-            "headers": {"cache-control": f"max-age={60*60*24}"},
+            "transport": self.transport,
+            "headers": {"cache-control": f"max-age={60 * 60 * 24}"},
         }
-        if self.base_url:
+        if hasattr(self, "base_url"):
             options["base_url"] = self.base_url
-        self.client = AsyncClient(**options)
-        self.ijson = ijson
+
+        return AsyncClient(**options)
 
     async def close(self):
         await self.client.aclose()
 
     async def _sleep(self):
         await asyncio.sleep(self.delay)
```

### Comparing `mightstone-0.4.0/src/mightstone/services/cardconjurer/__init__.py` & `mightstone-0.8.1/src/mightstone/services/cardconjurer/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import asyncio
 import base64
 import datetime
+import logging
 import os.path
 import re
 import textwrap
 from collections import defaultdict
 from io import BytesIO
-from typing import Dict, Generic, TypeVar, Union
+from typing import Dict, Optional, Tuple, Type, TypeVar, Union, cast, overload
 from urllib.parse import urlparse
 
 import aiofiles
+import httpx
 import PIL.Image
 from httpx import HTTPStatusError
 from PIL import Image, ImageDraw, ImageFont, UnidentifiedImageError
-from pydantic.color import Color
-from pydantic.error_wrappers import ValidationError
+from PIL.ImageFont import FreeTypeFont
+from pydantic import ValidationError
+from pydantic_extra_types.color import Color
 
-from mightstone import logger
+from mightstone.ass import synchronize
 from mightstone.services import MightstoneHttpClient, ServiceError
 from mightstone.services.cardconjurer.models import (
     Card,
     FilterOverlay,
     FilterShadow,
     HorizontalAlign,
 )
@@ -37,24 +40,26 @@
 T = TypeVar("T")
 
 
 base64_prefix = re.compile("^data:image/(?P<mime>.+);base64,")
 inline_icon = re.compile(r"(?P<icon>{(?P<name>\w+)})")
 inline_icon_sep = re.compile(r"({\w+})")
 
+logger = logging.getLogger("mightstone")
+
 
 class CardConjurer(MightstoneHttpClient):
     """
     Card Conjurer client
     """
 
-    base_url = None
+    base_url: str
     default_font = "LiberationMono-Regular.ttf"
 
-    def __init__(self, default_font=None, **kwargs):
+    def __init__(self, default_font: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
 
         self.assets_images: Dict[str, Image.Image] = {}
         self.assets_fonts: Dict[str, BytesIO] = {}
         if not default_font:
             default_font = os.path.join(
                 os.path.dirname(__file__), "../../assets/LiberationMono-Regular.ttf"
@@ -64,53 +69,57 @@
 
     def clear(self):
         with open(self.default_font, "rb") as f:
             default_font = BytesIO(f.read())
         self.assets_fonts = defaultdict(lambda: default_font)
         self.assets_images = {}
 
-    async def template(self, url_or_path) -> Template:
+    async def template_async(self, url_or_path) -> Template:
         """
         Open a ``Template``, local or through HTTP
 
         :param url_or_path: A path or an url
         :return: ``Template`` instance
         """
         if urlparse(url_or_path).scheme != "":
             return await self._url(Template, url_or_path)
         return await self._file(Template, url_or_path)
 
-    async def card(self, url_or_path) -> Card:
+    template = synchronize(template_async)
+
+    async def card_async(self, url_or_path) -> Card:
         """
         Open a ``Card``, local or through HTTP
 
         :param url_or_path: A path or an url
         :return: ``Card`` instance
         """
         if urlparse(url_or_path).scheme != "":
             return await self._url(Card, url_or_path)
         return await self._file(Card, url_or_path)
 
-    async def render(self, card: Card, output=None) -> PIL.Image.Image:
+    card = synchronize(card_async)
+
+    async def render_async(self, card: Card, output=None) -> PIL.Image.Image:
         """
         Render a card object into a PIL Image
 
         :param card: Card model from Card Conjurer
         :param output: A path or a file like object for writing
         :return: A PIL Image object
         """
         # TODO: Use async to download assets first, then build the image
         image = Image.new("RGBA", (card.width, card.height), (255, 255, 255, 0))
 
         coros = []
         template = Template.dummy()
-        if card.dependencies.template.url:
-            template_path = card.asset_root_url + "/" + card.dependencies.template.url
+        if card.dependencies.template and card.dependencies.template.url:
+            template_path = f"{card.asset_root_url}/{card.dependencies.template.url}"
             try:
-                template = await self.template(template_path)
+                template = await self.template_async(template_path)
             except FileNotFoundError:
                 raise ServiceError(
                     f"Unable to find parent template for {card.name},"
                     f" {template_path} was composed from the card path. Please try to"
                     " define a custom asset_root_url for this card."
                 )
             for font in template.context.fonts:
@@ -171,40 +180,58 @@
             image = self._add_corners(image, 60)
 
         if output:
             image.save(output)
 
         return image
 
-    async def _file(self, model: Generic[T], path: str) -> T:
+    render = synchronize(render_async)
+
+    @overload
+    async def _file(self, model: Type[Card], path: str) -> Card: ...
+
+    @overload
+    async def _file(self, model: Type[Template], path: str) -> Template: ...
+
+    async def _file(
+        self, model: Union[Type[Card], Type[Template]], path: str
+    ) -> Union[Card, Template]:
         """
         Reads a Card Conjurer model from a local file using asyncio
 
         :param model: The model (either ``Card`` or ``Template``)
         :param path: The local path to read from
         :return: Model validated instance
         """
         try:
             async with aiofiles.open(path, encoding="utf-8") as f:
-                x = model.parse_raw(await f.read())
+                x = model.model_validate_json(await f.read())
                 x.asset_root_url = os.path.dirname(path)
                 return x
         except ValidationError as e:
             raise ServiceError(
                 message=f"Failed to validate {Template} data, {e.errors()}",
                 url=path,
                 status=None,
                 data=e,
             )
 
-    async def _url(self, model: Generic[T], url: str) -> T:
+    @overload
+    async def _url(self, model: Type[Card], url: str) -> Card: ...
+
+    @overload
+    async def _url(self, model: Type[Template], url: str) -> Template: ...
+
+    async def _url(
+        self, model: Union[Type[Card], Type[Template]], url: str
+    ) -> Union[Card, Template]:
         try:
             f = await self.client.get(url)
             f.raise_for_status()
-            x = model.parse_raw(f.content)
+            x = model.model_validate_json(f.content)
             x.asset_root_url = "{uri.scheme}://{uri.netloc}".format(uri=urlparse(url))
             return x
         except ValidationError as e:
             raise ServiceError(
                 message=f"Failed to validate {Template} data, {e.errors()}",
                 url=url,
                 method="GET",
@@ -216,57 +243,59 @@
                 message="Failed to fetch CardConjurer template",
                 url=e.request.url,
                 method=e.request.method,
                 status=e.response.status_code,
                 data=None,
             )
 
-    async def _fetch_font(self, font: TemplateFont, base_uri: str = None):
+    async def _fetch_font(self, font: TemplateFont, base_uri: Optional[str] = None):
         uri = font.src
         if base_uri:
             uri = base_uri + "/" + font.src
 
         parsed_uri = urlparse(uri, "file")
         logger.info("Fetching font %s", font)
         if parsed_uri.scheme == "file":
-            async with aiofiles.open(uri) as f:
+            async with aiofiles.open(uri, "rb") as f:
                 buffer = BytesIO(await f.read())
         elif parsed_uri.scheme in ("http", "https"):
-            f = await self.client.get(uri)
-            buffer = BytesIO(f.content)
+            response: httpx.Response = await self.client.get(uri)
+            buffer = BytesIO(response.content)
         else:
             raise RuntimeError(f"Unknown scheme {parsed_uri.scheme}")
 
         logger.info("%s successfully fetched", font)
         self.assets_fonts[font.name] = buffer
 
-    async def _fetch_image(self, img: Union[CCImage, Symbol], base_uri: str = None):
+    async def _fetch_image(
+        self, img: Union[CCImage, Symbol], base_uri: Optional[str] = None
+    ):
         if base64_prefix.match(img.src):
             logger.info("Using BASE64 image")
             fo = BytesIO(base64.b64decode(base64_prefix.sub("", img.src)))
             self.assets_images[img.src] = self._image_potentially_from_svg(fo)
             return
 
         uri = img.src
         if base_uri:
             uri = base_uri + "/" + img.src
 
         parsed_uri = urlparse(uri, "file")
         logger.info("Fetching image %s", uri)
         if parsed_uri.scheme == "file":
-            async with aiofiles.open(uri) as f:
+            async with aiofiles.open(uri, "rb") as f:
                 self.assets_images[img.src] = self._image_potentially_from_svg(
                     BytesIO(await f.read())
                 )
                 return
 
         if parsed_uri.scheme in ("http", "https"):
-            f = await self.client.get(uri)
+            response: httpx.Response = await self.client.get(uri)
             self.assets_images[img.src] = self._image_potentially_from_svg(
-                BytesIO(f.content)
+                BytesIO(response.content)
             )
             return
 
         raise ValueError(f"URI: {uri} scheme is not supported")
 
     @staticmethod
     def _image_potentially_from_svg(file: BytesIO) -> Image.Image:
@@ -284,30 +313,33 @@
 
             svg2png_buffer = BytesIO()
             cairosvg.svg2png(file_obj=file, write_to=svg2png_buffer)
             return Image.open(svg2png_buffer)
 
     async def _add_text2(self, layer: Text, symbols: Dict[str, Symbol], **kwargs):
         im = PIL.Image.new("RGBA", (layer.width, layer.height), (0, 0, 0, 0))
-        font_file = self.assets_fonts[layer.font]
+        if layer.font:
+            font_file = self.assets_fonts[layer.font]
+        else:
+            font_file = self.assets_fonts["default"]
         font_file.seek(0)
-        font = ImageFont.truetype(font_file, layer.size)
+        font: FreeTypeFont = ImageFont.truetype(font_file, layer.size)
         draw = ImageDraw.Draw(im, "RGBA")
 
         if layer.align == HorizontalAlign.LEFT:
             anchor = "la"
             origin = 0
         elif layer.align == HorizontalAlign.RIGHT:
             anchor = "ra"
             origin = layer.width
         else:
             if inline_icon_sep.match(layer.text):
                 raise ValueError("Centered text with inline icon is not supported")
             anchor = "ma"
-            origin = layer.width / 2
+            origin = round(layer.width / 2)
 
         text = coreTextCode(layer.text)
         xy = (origin, 0)
         line_height = round(layer.size * layer.lineHeightScale)
         max_y = 0
 
         for line in get_wrapped_text(text, font, layer.width).splitlines():
@@ -322,15 +354,15 @@
                 if not icon:
                     bb = draw.textbbox(xy, part, font=font, anchor=anchor)
                     draw.text(
                         xy,
                         part,
                         font=font,
                         anchor=anchor,
-                        fill=layer.color.as_rgb_tuple(),
+                        fill=pycolor_to_pilcolor(layer.color),
                     )
 
                     xy = (xy[0] + bb[2] - bb[0], xy[1])
                 else:
                     if icon.group("name").lower() not in symbols:
                         raise ValueError(
                             f"Could not resolve symbol {icon.group('name')} in"
@@ -350,16 +382,16 @@
                     if layer.align == HorizontalAlign.RIGHT:
                         icon_position = (xy[0] - icon_size[0] - icon_padding, icon_y)
                         xy = (icon_position[0] - icon_padding, xy[1])
                     else:
                         icon_position = (xy[0] + icon_padding, icon_y)
                         xy = (xy[0] + icon_size[0] + icon_padding + icon_padding, xy[1])
 
-                    icon = self.assets_images[symbol.src].resize(icon_size)
-                    im.alpha_composite(icon, icon_position)
+                    icon_image = self.assets_images[symbol.src].resize(icon_size)
+                    im.alpha_composite(icon_image, icon_position)
 
             max_y = xy[1] + line_height
             xy = (origin, max_y)
 
         if max_y > layer.height:
             # TODO: if too high, retry with smaller font
             pass
@@ -434,15 +466,15 @@
         alpha.paste(circle.crop((rad, rad, rad * 2, rad * 2)), (w - rad, h - rad))
 
         im.putalpha(alpha)
 
         return im
 
 
-def get_wrapped_text(text: str, font: ImageFont.ImageFont, max_width: int):
+def get_wrapped_text(text: str, font: ImageFont.FreeTypeFont, max_width: int):
     """
     A text wrapper that will wraps a string over a maximum text width for a given font
     and given width in an image
 
     :param text: The text to wrap
     :param font: A pillow ``ImageFont`` instance
     :param max_width: The maximum width your text should fit in
@@ -471,23 +503,37 @@
         .replace("{/i}", "")
         .replace("{line}", "\n")
     )
 
 
 def apply_overlay(im: Image.Image, color: Color):
     clean_layer = Image.new("RGBA", im.size, (255, 255, 255, 0))
-    overlay = Image.new("RGBA", im.size, color.as_rgb_tuple())
+    overlay = Image.new("RGBA", im.size, pycolor_to_pilcolor(color))
     return Image.composite(overlay, clean_layer, im)
 
 
 def apply_shadow(im: Image.Image, color, offset_x=0, offset_y=0):
     clean_layer = Image.new("RGBA", im.size, (255, 255, 255, 0))
-    shadow = Image.new("RGBA", im.size, color=color.as_rgb_tuple())
+    shadow = Image.new("RGBA", im.size, pycolor_to_pilcolor(color))
     clean_layer.paste(shadow, (offset_x, offset_y), mask=im)
     clean_layer.paste(im, (0, 0), mask=im)
 
     return clean_layer
 
 
 def apply_opacity(im: Image.Image, opacity):
     alpha = im.getchannel("A")
     im.putalpha(alpha.point(lambda i: (opacity * 256) if i > 0 else 0))
+
+
+def pycolor_to_pilcolor(
+    color: Color,
+) -> Union[Tuple[int, int, int], Tuple[int, int, int, int]]:
+    t = color.as_rgb_tuple()
+    if not t:
+        return 0, 0, 0, 0
+
+    if len(t) == 4:
+        t = cast(Tuple[int, int, int, float], t)
+        return t[0], t[1], t[2], round(t[3] * 255)
+
+    return cast(Tuple[int, int, int], t)
```

### Comparing `mightstone-0.4.0/src/mightstone/services/edhrec/__init__.py` & `mightstone-0.8.1/src/mightstone/services/mtgjson/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,649 +1,685 @@
+"""
+MTGJSON support core
+"""
+
+import json
 import logging
-import re
 from enum import Enum
-from pathlib import Path
-from typing import AsyncGenerator, Dict, List, Optional, Tuple, Union
+from typing import (
+    Any,
+    AsyncGenerator,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+)
 
 import asyncstdlib
 from httpx import HTTPStatusError
-from pydantic.error_wrappers import ValidationError
-from pydantic.fields import Field
+from pydantic import ValidationError
 
+from mightstone.ass import compressor, sync_generator, synchronize
 from mightstone.core import MightstoneModel
 from mightstone.services import MightstoneHttpClient, ServiceError
+from mightstone.services.mtgjson.models import (
+    Card,
+    CardAtomic,
+    CardFace,
+    CardPrices,
+    CardTypes,
+    Deck,
+    DeckList,
+    Keywords,
+    Meta,
+    Set,
+    SetList,
+    TcgPlayerSKU,
+    TcgPlayerSKUs,
+)
+
+DictOfListOfKey = Tuple[str, int]
+DictOfListOfModel = Tuple[DictOfListOfKey, Any]
+ListOfKey = int
+ListOfModel = Tuple[ListOfKey, Any]
+DictOfKey = str
+DictOfModel = Tuple[DictOfKey, Any]
+GeneratorModel = Union[DictOfListOfModel, ListOfModel, DictOfModel]
+GeneratorKey = Union[DictOfListOfKey, ListOfKey, DictOfKey]
 
-salt_parser = re.compile(r"Salt Score: (?P<salt>[\d.]+)\n")
-synergy_parser = re.compile(r"(?P<synergy>[\d.]+)% synergy")
+logger = logging.getLogger("mightstone")
 
-logger = logging.getLogger(__name__)
 
+class MtgJsonMode(Enum):
+    """
+    Available data parse mode
 
-class EdhRecIdentity(Enum):
-    COLORLESS = "colorless"
-    W = "w"
-    U = "u"
-    B = "b"
-    R = "r"
-    G = "g"
-    WU = "wu"
-    UB = "ub"
-    BR = "br"
-    RG = "rg"
-    GW = "gw"
-    WB = "wb"
-    UR = "ur"
-    BG = "bg"
-    RW = "rw"
-    GU = "gu"
-    WUB = "wub"
-    UBR = "ubr"
-    BRG = "brg"
-    RGW = "rgw"
-    GWU = "gwu"
-    WBG = "wbg"
-    URW = "urw"
-    BGU = "bgu"
-    RWB = "rwb"
-    GUR = "gur"
-    WUBR = "wubr"
-    UBRG = "ubrg"
-    BRGW = "brgw"
-    RGWU = "rgwu"
-    GWUB = "gwub"
-    WUBRG = "wubrg"
-
-
-class EdhRecTag(Enum):
-    TRIBES = "tribes"
-    SET = "sets"
-    NONE = ""
-    THEME_POPULARITY = "themesbypopularitysort"
-    THEME = "themes"
-    COMMANDER = "topcommanders"
-    COMPANION = "companions"
-
-
-class EdhRecType(Enum):
-    CREATURE = "creatures"
-    INSTANT = "instants"
-    SORCERY = "sorceries"
-    ARTIFACT = "artifacts"
-    ARTIFACT_EQUIPMENT = "equipment"
-    ARTIFACT_UTILITY = "utility-artifacts"
-    ARTIFACT_MANA = "mana-artifacts"
-    ENCHANTMENT = "enchantments"
-    ENCHANTMENT_AURA = "auras"
-    PLANESWALKER = "planeswalker"
-    LAND = "lands"
-    LAND_UTILITY = "utility-lands"
-    LAND_FIXING = "color-fixing-lands"
-
-
-class EdhRecCategory(Enum):
-    TOP_COMMANDER = "topcommanders"
-    COMMANDER = "commanders"
-    NEW = "newcards"
-    HIGH_SYNERGY = "highsynergycards"
-    TOP_CARD = "topcards"
-    CREATURE = "creatures"
-    INSTANT = "instants"
-    SORCERY = "sorceries"
-    ARTEFACT_UTIL = "utilityartifacts"
-    ENCHANTMENT = "enchantments"
-    PLANEWALKER = "planeswalkers"
-    LAND_UTIL = "utilitylands"
-    ARTEFACT_MANA = "manaartifacts"
-    LAND = "lands"
-
-
-class EdhRecPeriod(Enum):
-    PAST_WEEK = "pastweek"
-    PAST_MONTH = "pastmonth"
-    PAST_2YEAR = "past2years"
-
-
-class EdhRecCardRef(MightstoneModel):
-    name: str
-    url: str
-
-
-class EdhRecCard(MightstoneModel):
-    cmc: int
-    color_identity: List[str]
-
-    combos: bool = None
-    label: str = None
-    legal_commander: bool = None
-
-    image_uris: List[dict]
-    is_commander: bool = None
-    layout: str
-    name: str
-    names: List[str]
-    inclusion: int = None
-    num_decks: int = None
-    potential_decks: int = None
-    precon: str = None
-    prices: dict
-    primary_type: str
-    rarity: str
-    salt: float
-    sanitized: str
-    sanitized_wo: str
-    type: str
-    url: str = None
-    aetherhub_uri: str = None
-    archidekt_uri: str = None
-    deckstats_uri: str = None
-    moxfield_uri: str = None
-    mtggoldfish_uri: str = None
-    scryfall_uri: str = None
-    spellbook_uri: str = None
-
-
-class EdhRecCommanderSub(MightstoneModel):
-    count: int
-    suffix: str = Field(alias="href-suffix")
-    value: str
-
-
-class EdhRecCommanderDistribution(MightstoneModel):
-    artifact: int = 0
-    creature: int = 0
-    enchantment: int = 0
-    instant: int = 0
-    land: int = 0
-    planeswalker: int = 0
-    sorcery: int = 0
-
-
-class EdhRecCardItem(MightstoneModel):
-    tag: str
-    name: str
-    slug: str
-    url: Path
-    label: str = None
-    inclusion: int = None
-    cards: List[EdhRecCardRef] = None
-    count: int = None
-    num_decks: int = None
-    potential_decks: int = None
-    synergy: float = None
-    salt: float = None
-
-    @classmethod
-    def parse_payload(cls, data: dict, tag: str = None):
-        salt = salt_parser.search(data.get("label", "unspecified"))
-        if salt:
-            data["salt"] = float(salt.group("salt"))
-
-        synergy = synergy_parser.search(data.get("label", ""))
-        if synergy:
-            data["synergy"] = float(synergy.group("synergy"))
-
-        return EdhRecCardItem.parse_obj(
-            {
-                **data,
-                "tag": tag,
-                "url": str("/pages" + data.get("url") + ".json"),
-                "slug": slugify(data.get("name", "")),
-            }
-        )
-
-
-class EdhRecCardList(MightstoneModel):
-    tag: str
-    items: List[EdhRecCardItem] = []
-
-    @classmethod
-    def parse_payload(cls, data: dict):
-        tag = data.get("tag")
-        return EdhRecCardList.parse_obj(
-            {
-                "tag": tag,
-                "items": list(
-                    EdhRecCardItem.parse_payload(item, tag).dict()
-                    for item in data["cardviews"]
-                ),
-            }
-        )
-
-
-class EdhRecCommander(MightstoneModel):
-    card: EdhRecCard
-    articles: List[dict] = []
-    cards: List[EdhRecCardList] = []
-    mana_curve: Dict[int, int] = {i: 0 for i in range(0, 11)}
-    themes: List[EdhRecCommanderSub] = []
-    budget: List[EdhRecCommanderSub] = []
-    distribution: EdhRecCommanderDistribution
-    links: List[dict] = []
-
-    @classmethod
-    def parse_payload(cls, data: dict):
-        return EdhRecCommander(
-            card=EdhRecCard.parse_obj(
-                data.get("container", {}).get("json_dict", {}).get("card")
-            ),
-            cards=[
-                EdhRecCardList.parse_payload(payload)
-                for payload in data.get("container", {})
-                .get("json_dict", {})
-                .get("cardlists")
-            ],
-            articles=data.get("panels", {}).get("articles", []),
-            links=data.get("panels", {}).get("links", []),
-            mana_curve=data.get("panels", {}).get("mana_curve", {}),
-            themes=data.get("panels", {}).get("tribelinks", {}).get("themes", {}),
-            budget=data.get("panels", {}).get("tribelinks", {}).get("budget", {}),
-            distribution=data,
-        )
-
-
-class EdhRecFilterOperator(Enum):
-    GREATER_THAN = "gt"
-    LESS_THAN = "lt"
-    EQUAL = "eq"
-    NOT_EQUAL = "ne"
-
-
-class EdhRecFilterType(Enum):
-    CREATURE = "c"
-    INSTANT = "i"
-    SORCERY = "s"
-    ARTIFACT = "a"
-    ENCHANTMENT = "e"
-    PLANESWALKER = "p"
-    LANDS = "l"
-    PRICE = "d"
-
-
-class EdhRecFilterComparator(MightstoneModel):
-    value: int = 0
-    operator: EdhRecFilterOperator = EdhRecFilterOperator.EQUAL
-
-    def __str__(self):
-        return f"{self.operator.value}={self.value}"
-
-
-class EdhRecFilterQuery(MightstoneModel):
-    card_in: List[str] = []
-    card_out: List[str] = []
-    count: Dict[EdhRecFilterType, EdhRecFilterComparator] = {}
-
-    def __str__(self):
-        filters = []
-        filters.extend([f"Out={card}" for card in self.card_out])
-        filters.extend([f"In={card}" for card in self.card_in])
-        filters.extend(
-            [f"{field.value}:{comparator}" for field, comparator in self.count.items()]
-        )
-        return ";".join(filters)
-
-
-class EdhRecRecs(MightstoneModel):
-    commanders: List[EdhRecCard] = []
-    inRecs: List[EdhRecCard] = []
-    outRecs: List[EdhRecCard] = []
-
-
-class EdhRecApi(MightstoneHttpClient):
-    """
-    HTTP client for dynamic data hosted at https://edhrec.com/api/
-    """
-
-    base_url = "https://edhrec.com"
-
-    async def recs(self, commanders: List[str], cards: List[str]):
-        """
-        Obtain EDHREC recommendations for a given commander (or partners duo)
-        for a given set of cards in the deck.
-
-        Returns a list of 99 suggested cards not contained in the list
-        :param commanders: A list of one or two commander card name
-        :param cards: A list of card name
-        :exception ClientResponseError
-        :returns An EdhRecRecs object
-        """
-        try:
-            session = await self._build_session()
-            async with session.post(
-                "/api/recs/",
-                json={"cards": cards, "commanders": commanders},
-            ) as f:
-                f.raise_for_status()
-                data = await f.json()
+    MTGJSON model is not consistent, this enum describe the expected data structure
+    of a MTGJSON response
+    """
 
-                if data.get("errors"):
-                    raise ServiceError(
-                        message=data.get("errors")[0],
-                        data=data,
-                        url=f.request_info.real_url,
-                        status=f.status,
-                    )
+    LIST_OF_MODEL = 0
+    """
+    In this mode, we expect a structure similar to
+     .. code-block:: json
+     {"data": [{"prop": 1}, "b": {"prop": 2}]}
+    """
+    DICT_OF_MODEL = 1
+    """
+    In this mode, we expect a structure similar to
+     .. code-block:: json
+     {"data": {"a": {"prop": 1}, "b": {"prop": 2}}}
+    """
+    DICT_OF_LIST_OF_MODEL = 2
+    """
+    In this mode, we expect a structure similar to
+     .. code-block:: json
+     {"data": {"a": [{"prop": 1}], "b": [{"prop": 2}]}}
+    """
 
-                return EdhRecRecs.parse_obj(data)
 
-        except HTTPStatusError as e:
-            raise ServiceError(
-                message="Failed to fetch data from EDHREC",
-                url=e.request.url,
-                status=e.response.status,
-            )
+class MtgJsonCompression(str, Enum):
+    """
+    Available compression mode enumerator
+
+    MTGJSON provide 5 compression formats, Mightstone support 4 of them.
+    """
 
-    async def filter(self, commander: str, query: EdhRecFilterQuery) -> EdhRecCommander:
+    NONE = ""
+    """ No compression, use raw JSON """
+    XZ = "xz"
+    """ LZMA compression, use .xz files """
+    ZIP = "zip"
+    """ ZIP compression, use .zip files (not supported)"""
+    GZIP = "gz"
+    """ GZIP compression, use .gz files"""
+    BZ2 = "bz2"
+    """ BZIP2 compression, use .bz2 files"""
+
+    def to_stream_compression(self):
         """
-        Read Commander related information, and return an EdhRecCommander object
+        Compute the compression type to a python module
 
-        :param commander: Commander name or slug
-        :param query: An EdhRecFilterQuery object describing the request
-        :return: An EdhRecCommander representing answer
+        :return: the name of the python module
         """
-        try:
-            session = await self._build_session()
-            async with session.get(
-                "/api/filters/",
-                params={
-                    "f": str(query),
-                    "dir": "commanders",
-                    "cmdr": slugify(commander),
-                },
-            ) as f:
-                f.raise_for_status()
-                return EdhRecCommander.parse_payload(await f.json())
+        if self.value == "":
+            return None
+        elif self.value == "xz":
+            return "lzma"
+        elif self.value == "gz":
+            return "gzip"
+        elif self.value == "bz2":
+            return "bzip2"
+        raise ValueError(f"{self.name} compression protocol cannot be read as a stream")
 
-        except HTTPStatusError as e:
-            raise ServiceError(
-                message="Failed to fetch data from EDHREC",
-                url=e.request.url,
-                status=e.response.status_code,
-            )
 
+_T = TypeVar("_T", bound=MightstoneModel)
 
-class EdhRecStatic(MightstoneHttpClient):
+
+class MtgJson(MightstoneHttpClient):
     """
-    HTTP client for static JSON data hosted at https://json.edhrec.com
+    MTGJSON client
+
+    Supports compression and will get gzip versions by default.
     """
 
-    base_url = "https://json.edhrec.com"
+    base_url = "https://mtgjson.com"
+
+    def __init__(
+        self,
+        compression: Optional[MtgJsonCompression] = None,
+        version: int = 5,
+        *args,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.version = int(version)
+        if compression is None:
+            compression = MtgJsonCompression.GZIP
+        self.compression = MtgJsonCompression(compression)
+
+    def set_compression(self, compression=MtgJsonCompression):
+        self.compression = MtgJsonCompression(compression)
 
-    async def commander(self, name: str, sub: str = None) -> EdhRecCommander:
+    async def all_printings_async(self) -> AsyncGenerator[Set, None]:
         """
+        all Card (Set) cards, including all printings and variations, categorized by
+        set.
 
-        :param name: Commander
-        :param sub:
-        :return:
-        """
-        path = f"commanders/{slugify(name)}.json"
-        if sub:
-            path = f"commanders/{slugify(name)}/{slugify(sub)}.json"
-
-        data = await self._get_static_page(path)
-
-        return EdhRecCommander.parse_payload(data)
-
-    async def tribes(
-        self, identity: Union[EdhRecIdentity, str] = None, limit: int = None
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        if identity:
-            identity = EdhRecIdentity(identity)
-            async for item in self._page_item_generator(
-                f"commanders/{identity.value}.json",
-                EdhRecTag.TRIBES,
-                related=True,
-                limit=limit,
-            ):
-                yield item
-        else:
-            async for item in self._page_item_generator(
-                "tribes.json", EdhRecTag.TRIBES, limit=limit
-            ):
-                yield item
-
-    async def themes(
-        self, identity: Union[EdhRecIdentity, str] = None, limit: int = None
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        if identity:
-            identity = EdhRecIdentity(identity)
-            async for item in self._page_item_generator(
-                f"commanders/{identity.value}.json",
-                EdhRecTag.THEME,
-                related=True,
-                limit=limit,
-            ):
-                yield item
-        else:
-            async for item in self._page_item_generator(
-                "themes.json", EdhRecTag.THEME_POPULARITY, limit=limit
-            ):
-                yield item
-
-    async def sets(self, limit: int = None) -> AsyncGenerator[dict, None]:
-        async for item in self._page_item_generator(
-            "sets.json", EdhRecTag.SET, limit=limit
+        :return: An async iterator of CardSet
+        """
+        async for k, item in self._iterate_model(
+            kind="AllPrintings", model=Set, mode=MtgJsonMode.DICT_OF_MODEL
         ):
             yield item
 
-    async def salt(
-        self, year: int = None, limit: int = None
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        path = "top/salt.json"
-        if year:
-            path = f"top/salt-{year}.json"
-        async for item in self._page_item_generator(path, limit=limit):
+    all_printings = sync_generator(all_printings_async)
+
+    async def all_identifiers_async(self) -> AsyncGenerator[Card, None]:
+        """
+        all Card (Set) cards organized by card UUID.
+
+        :return: An async iterator of Card object (either CardToken, or CardSet)
+        """
+        async for k, item in self._iterate_model(  # type: ignore # no-qa
+            kind="AllIdentifiers", model=Card
+        ):
             yield item
 
-    async def top_cards(
-        self,
-        type: EdhRecType = None,
-        period: EdhRecPeriod = EdhRecPeriod.PAST_WEEK,
-        limit: int = None,
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        period = EdhRecPeriod(period)
-        if type:
-            type = EdhRecType(type)
-            async for item in self._page_item_generator(
-                f"top/{type.value}.json", period, limit=limit
-            ):
-                yield item
-            return
-
-        if period == EdhRecPeriod.PAST_WEEK:
-            path = "top/week.json"
-        elif period == EdhRecPeriod.PAST_MONTH:
-            path = "top/month.json"
-        else:
-            path = "top/year.json"
-        async for item in self._page_item_generator(path, limit=limit):
+    all_identifiers = sync_generator(all_identifiers_async)
+
+    async def all_prices_async(self) -> AsyncGenerator[CardPrices, None]:
+        """
+        all prices of cards in various formats.
+
+        :return: An async iterator of CardPrices
+        """
+        async for k, item in self._iterate_model(kind="AllPrices"):
+            yield CardPrices(uuid=k, **item)  # type: ignore
+
+    all_prices = sync_generator(all_prices_async)
+
+    async def atomic_cards_async(self) -> AsyncGenerator[CardAtomic, None]:
+        """
+        every Card (Atomic) card.
+
+        :return: An async iterator of ``CardAtomic``
+        """
+        async for item in self._atomic(kind="AtomicCards"):
             yield item
 
-    async def cards(
-        self,
-        theme: str = None,
-        commander: str = None,
-        identity: Union[EdhRecIdentity, str] = None,
-        set: str = None,
-        category: EdhRecCategory = None,
-        limit: int = None,
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        if category:
-            category = EdhRecCategory(category)
-
-        if not theme and not commander and not set:
-            raise ValueError("You must either provide a theme, commander or set")
-
-        if commander:
-            if theme:
-                raise ValueError("commander and theme options are mutually exclusive")
-            if identity:
-                raise ValueError(
-                    "commander and identity options are mutually exclusive"
-                )
-            if set:
-                raise ValueError("commander and set options are mutually exclusive")
+    atomic_cards = sync_generator(atomic_cards_async)
+
+    async def card_types_async(self) -> CardTypes:
+        """
+        every card type of any type of card.
+
+        :return: A ``CardTypes`` object
+        """
+        return await self._get_item("CardTypes", model=CardTypes)
+
+    card_types = synchronize(card_types_async)
+
+    async def compiled_list_async(self) -> List[str]:
+        """
+        all individual outputs from MTGJSON, such as AllPrintings, CardTypes, etc.
 
-            slug = slugify(commander)
-            path = f"commanders/{slug}.json"
-            if theme:
-                path = f"commanders/{slug}/{slugify(theme)}.json"
-            async for item in self._page_item_generator(path, category, limit=limit):
-                yield item
-
-            return
-
-        if set:
-            if theme:
-                raise ValueError("set and theme options are mutually exclusive")
-            if identity:
-                raise ValueError("set and identity options are mutually exclusive")
-            async for item in self._page_item_generator(
-                f"sets/{slugify(set)}.json", category, limit=limit
-            ):
-                yield item
-            return
-
-        if identity and not theme:
-            raise ValueError("you must specify a theme to search by color identity")
-
-        path = f"themes/{slugify(theme)}.json"
-        if identity:
-            identity = EdhRecIdentity(identity)
-            path = f"themes/{slugify(theme)}/{identity.value}.json"
-        async for item in self._page_item_generator(path, category, limit=limit):
-            yield item
-
-    async def companions(
-        self, limit: int = None
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        async for item in self._page_item_generator(
-            "companions.json", EdhRecTag.COMPANION, limit=limit
+        :return: A list of string
+        """
+        return await self._get_item("CompiledList", model=list)
+
+    compiled_list = synchronize(compiled_list_async)
+
+    async def deck_list_async(self) -> AsyncGenerator[DeckList, None]:
+        """
+        all individual Deck data.
+
+        :return: An async iterator of DeckList
+        """
+        async for i, item in self._iterate_model(
+            kind="DeckList", model=DeckList, mode=MtgJsonMode.LIST_OF_MODEL
         ):
             yield item
 
-    async def partners(
-        self, identity: Union[EdhRecIdentity, str] = None, limit: int = None
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        path = "partners.json"
-        if identity:
-            identity = EdhRecIdentity(identity)
-            path = f"partners/{identity.value}.json"
-        async for item in self._page_item_generator(path, limit=limit):
-            yield item
-
-    async def commanders(
-        self, identity: Union[EdhRecIdentity, str] = None, limit: int = None
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        path = "commanders.json"
-        if identity:
-            identity = EdhRecIdentity(identity)
-            path = f"commanders/{identity.value}.json"
-        async for item in self._page_item_generator(path, limit=limit):
-            yield item
-
-    async def combos(
-        self, identity: Union[EdhRecIdentity, str], limit: int = None
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        identity = EdhRecIdentity(identity)
-        async for item in self._page_item_generator(
-            f"combos/{identity.value}.json", limit=limit
+    deck_list = sync_generator(deck_list_async)
+
+    async def deck_async(self, file_name: str) -> Deck:
+        """
+        Recovers a deck data
+
+        :param file_name: the deck file_name
+        :return: A ``Deck`` object
+        """
+        return await self._get_item(f"decks/{file_name}", model=Deck)
+
+    deck = synchronize(deck_async)
+
+    async def enum_values_async(self) -> dict:
+        """
+        All known property values for various Data Models.
+
+        :return: a ``dict`` object
+        """
+        return await self._get_item("EnumValues", model=dict)
+
+    enum_values = synchronize(enum_values_async)
+
+    async def keywords_async(self) -> Keywords:
+        """
+        a list of possible all keywords used on all cards.
+
+        :return: A ``Keywords`` object
+        """
+        return await self._get_item("Keywords", model=Keywords)
+
+    keywords = synchronize(keywords_async)
+
+    async def legacy_async(self) -> AsyncGenerator[Set, None]:
+        """
+        all Card (Set) cards organized by Set, restricted to sets legal in the
+        Legacy format.
+
+        :return: An async iterator of ``Set``
+        """
+        async for k, item in self._iterate_model(kind="Legacy", model=Set):
+            yield item
+
+    legacy = sync_generator(legacy_async)
+
+    async def legacy_atomic_async(self) -> AsyncGenerator[CardAtomic, None]:
+        """
+        all Card (Set) cards organized by Set, restricted to sets legal in the
+        Legacy format.
+
+        :return: An async iterator of ``CardAtomic``
+        """
+        async for item in self._atomic(kind="LegacyAtomic"):
+            yield item
+
+    legacy_atomic = sync_generator(legacy_atomic_async)
+
+    async def meta_async(self) -> Meta:
+        """
+        the metadata object with ISO 8601 dates for latest build and SemVer
+        specifications of the MTGJSON release.
+
+        :return: A Meta object
+        """
+        return await self._get_item("Meta", model=Meta)
+
+    meta = synchronize(meta_async)
+
+    async def modern_async(self) -> AsyncGenerator[Set, None]:
+        """
+        all Card (Set) cards organized by Set, restricted to sets legal in the
+        Modern format.
+
+        :return: An async iterator of ``Set``
+        """
+        async for k, item in self._iterate_model(kind="Modern", model=Set):
+            yield item
+
+    modern = sync_generator(modern_async)
+
+    async def modern_atomic_async(self) -> AsyncGenerator[CardAtomic, None]:
+        """
+        all Card (Atomic) cards, restricted to cards legal in the Modern format.
+
+        :return: An async iterator of ``CardAtomic``
+        """
+        async for item in self._atomic(kind="ModernAtomic"):
+            yield item
+
+    modern_atomic = sync_generator(modern_atomic_async)
+
+    async def pauper_atomic_async(self) -> AsyncGenerator[CardAtomic, None]:
+        """
+        all Card (Atomic) cards, restricted to cards legal in the Pauper format.
+
+        :return: An async iterator of ``CardAtomic``
+        """
+        async for item in self._atomic(kind="PauperAtomic"):
+            yield item
+
+    pauper_atomic = sync_generator(pauper_atomic_async)
+
+    async def pioneer_async(self) -> AsyncGenerator[Set, None]:
+        """
+        all Card (Set) cards organized by Set, restricted to cards legal in the
+        Pioneer format.
+
+        :return: An async iterator of ``Set``
+        """
+        async for k, item in self._iterate_model(kind="Pioneer", model=Set):
+            yield item
+
+    pioneer = sync_generator(pioneer_async)
+
+    async def pioneer_atomic_async(self) -> AsyncGenerator[CardAtomic, None]:
+        """
+        all Card (Atomic) cards, restricted to cards legal in the Pioneer format.
+
+        :return: An async iterator of ``CardAtomic``
+        """
+        async for item in self._atomic(kind="PioneerAtomic"):
+            yield item
+
+    pioneer_atomic = sync_generator(pioneer_atomic_async)
+
+    async def set_list_async(self) -> AsyncGenerator[SetList, None]:
+        """
+        a list of meta data for all Set data.
+
+        :return: An async iterator of ``SetList``
+        """
+        async for k, item in self._iterate_model(
+            kind="SetList", model=SetList, mode=MtgJsonMode.LIST_OF_MODEL
         ):
             yield item
 
-    async def combo(
-        self, identity: str, identifier: Union[EdhRecIdentity, str], limit: int = None
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        identity = EdhRecIdentity(identity)
-        async for item in self._page_item_generator(
-            f"combos/{identity.value}/{int(identifier)}.json", limit=limit
+    set_list = sync_generator(set_list_async)
+
+    async def set_async(self, code: str) -> SetList:
+        """
+        Get a Set data
+
+        :param code: The set identifier, such as "IKO" for "Ikoria, lair of the
+                     monsters"
+
+        :return: The set representation
+        """
+        return await self._get_item(code, SetList)
+
+    set = synchronize(set_async)
+
+    async def standard_async(self) -> AsyncGenerator[Set, None]:
+        """
+        all Card (Set) cards organized by Set, restricted to cards legal in the
+        Standard format.
+
+        :return: An async iterator of ``Set``
+        """
+        async for k, item in self._iterate_model(kind="Standard", model=Set):
+            yield item
+
+    standard = sync_generator(standard_async)
+
+    async def standard_atomic_async(self) -> AsyncGenerator[CardAtomic, None]:
+        """
+        all Card (Atomic) cards, restricted to cards legal in the Standard format.
+
+        :return: An async iterator of ``CardAtomic``
+        """
+        async for item in self._atomic(kind="StandardAtomic"):
+            yield item
+
+    standard_atomic = sync_generator(standard_atomic_async)
+
+    async def tcg_player_skus_async(self) -> AsyncGenerator[TcgPlayerSKUs, None]:
+        """
+        TCGplayer SKU information based on card UUIDs.
+
+        :return: an async iterator of ``TcgPlayerSKUs``
+        """
+        group: Optional[TcgPlayerSKUs] = None
+        async for (k, i), item in self._iterate_model(
+            kind="TcgplayerSkus",
+            model=TcgPlayerSKU,
+            mode=MtgJsonMode.DICT_OF_LIST_OF_MODEL,
         ):
+            if not group or k != group.uuid:
+                if group:
+                    yield group
+                group = TcgPlayerSKUs(uuid=k, skus=[])  # type: ignore
+            group.skus.append(item)
+
+            yield group
+
+    tcg_player_skus = sync_generator(tcg_player_skus_async)
+
+    async def vintage_async(self) -> AsyncGenerator[Set, None]:
+        """
+        all Card (Set) cards organized by Set, restricted to sets legal in the
+        Vintage format.
+
+        :return: An async iterator of ``Set``
+        """
+        async for k, item in self._iterate_model(kind="Vintage", model=Set):
+            yield item
+
+    vintage = sync_generator(vintage_async)
+
+    async def vintage_atomic_async(self) -> AsyncGenerator[CardAtomic, None]:
+        """
+        all Card (Atomic) cards, restricted to sets legal in the Vintage format.
+
+        :return: An async iterator of ``CardAtomic``
+        """
+        async for item in self._atomic(kind="VintageAtomic"):
             yield item
 
-    async def _page_item_generator(
+    vintage_atomic = sync_generator(vintage_atomic_async)
+
+    async def _atomic(self, kind: str) -> AsyncGenerator[CardAtomic, None]:
+        card: Optional[CardAtomic] = None
+        async for (k, i), item in self._iterate_model(
+            kind=kind, model=CardFace, mode=MtgJsonMode.DICT_OF_LIST_OF_MODEL
+        ):
+            if not card or k != card.ascii_name:
+                if card:
+                    yield card
+                card = CardAtomic(ascii_name=k, faces=[])  # type: ignore
+            card.faces.append(item)
+
+        if card:
+            yield card
+
+    async def _get_item(
         self,
-        path,
-        tag: Union[EdhRecTag, EdhRecType, EdhRecPeriod, EdhRecCategory] = None,
-        related=False,
-        limit: int = None,
-    ) -> AsyncGenerator[EdhRecCardItem, None]:
-        """
-        Async generator that will wrap Pydantic validation
-        and ensure that no validation error are raised
-        """
-        if tag:
-            tag = tag.value
-
-        enumerator = asyncstdlib.enumerate(self._get_page(path, tag, related))
-        async with asyncstdlib.scoped_iter(enumerator) as protected_enumerator:
-            async for i, (tag, page, index, item) in protected_enumerator:
-                if limit and i == limit:
-                    logging.debug(f"Reached limit of {limit}, stopping iteration")
-                    return
-
-                try:
-                    yield EdhRecCardItem.parse_payload(item, tag)
-                except ValidationError as e:
-                    logging.warning(
-                        "Failed to parse an EDHREC item from %s at page %d, index %d",
-                        path,
-                        page,
-                        index,
-                    )
-                    logging.debug(e.json())
+        kind: str,
+        model: Union[Type[_T], Type[Dict], Type[List]] = dict,
+        **kwargs,
+    ) -> _T:
+        path = f"/api/v{self.version}/{kind}.json"
+        if self.compression != MtgJsonCompression.NONE:
+            path += "." + self.compression.value
 
-    async def _get_static_page(self, path) -> dict:
         try:
-            f = await self.client.get(f"/pages/{path}")
-            f.raise_for_status()
-            return f.json()
+            async with self.client.stream("GET", path, **kwargs) as f:
+                async with compressor.open(
+                    f.aiter_bytes(),
+                    compression=self.compression.to_stream_compression(),
+                ) as f2:
+                    data = json.loads(await f2.read())
+                    data = data.get("data")
+
+                    if issubclass(model, MightstoneModel):
+                        return model.model_validate(data)  # type: ignore
+
+                    return model(data)  # type: ignore
+        except ValidationError as e:
+            raise ServiceError(
+                message=f"Failed to validate {model} data, {e.errors()}",
+                url=path,
+                method="GET",
+                status=None,
+                data=e,
+            )
         except HTTPStatusError as e:
             raise ServiceError(
-                message="Failed to fetch data from EDHREC",
+                message="Failed to fetch data from MTG Json",
                 url=e.request.url,
+                method=e.request.method,
                 status=e.response.status_code,
+                data=None,
             )
 
-    async def _get_page(
-        self, path, tag: str = None, related=False
-    ) -> AsyncGenerator[Tuple[str, int, int, dict], None]:
-        """
-        Read a EDHREC page data, and return it as a tuple:
-        - tag as string
-        - page
-        - index
-        - the payload itself
-        """
-        data = await self._get_static_page(path)
-        page = 1
-
-        if related:
-            iterator = [
-                {"tag": tag, "cardviews": data.get("relatedinfo", {}).get(tag, [])}
-            ]
-        else:
-            iterator = (
-                data.get("container", {}).get("json_dict", {}).get("cardlists", [])
-            )
+    @overload
+    def _iterate_model(
+        self, kind: str
+    ) -> AsyncGenerator[Tuple[DictOfKey, Dict], None]: ...
+
+    @overload
+    def _iterate_model(
+        self, kind: str, model: None
+    ) -> AsyncGenerator[Tuple[DictOfKey, Dict], None]: ...
+
+    @overload
+    def _iterate_model(
+        self, kind: str, model: Type[_T]
+    ) -> AsyncGenerator[Tuple[DictOfKey, _T], None]: ...
+
+    @overload
+    def _iterate_model(
+        self, kind: str, model: None, mode: Literal[MtgJsonMode.DICT_OF_MODEL]
+    ) -> AsyncGenerator[Tuple[DictOfKey, Dict], None]: ...
+
+    @overload
+    def _iterate_model(
+        self, kind: str, model: Type[_T], mode: Literal[MtgJsonMode.DICT_OF_MODEL]
+    ) -> AsyncGenerator[Tuple[DictOfKey, _T], None]: ...
+
+    @overload
+    def _iterate_model(
+        self, kind: str, model: None, mode: Literal[MtgJsonMode.LIST_OF_MODEL]
+    ) -> AsyncGenerator[Tuple[ListOfKey, Dict], None]: ...
+
+    @overload
+    def _iterate_model(
+        self, kind: str, model: Type[_T], mode: Literal[MtgJsonMode.LIST_OF_MODEL]
+    ) -> AsyncGenerator[Tuple[ListOfKey, _T], None]: ...
+
+    @overload
+    def _iterate_model(
+        self, kind: str, model: None, mode: Literal[MtgJsonMode.DICT_OF_LIST_OF_MODEL]
+    ) -> AsyncGenerator[Tuple[DictOfListOfKey, Dict], None]: ...
+
+    @overload
+    def _iterate_model(
+        self,
+        kind: str,
+        model: Type[_T],
+        mode: Literal[MtgJsonMode.DICT_OF_LIST_OF_MODEL],
+    ) -> AsyncGenerator[Tuple[DictOfListOfKey, _T], None]: ...
+
+    async def _iterate_model(
+        self,
+        kind: str,
+        model: Optional[Type[_T]] = None,
+        mode: MtgJsonMode = MtgJsonMode.DICT_OF_MODEL,
+        error_threshold: int = 10,
+        **kwargs,
+    ) -> AsyncGenerator[Tuple[GeneratorKey, Union[_T, Dict]], None]:
+        error = 0
+        async for k, v in self._iterate_raw(kind, mode, **kwargs):
+            try:
+                if model:
+                    yield k, model.model_validate(v)
+                else:
+                    yield k, dict(v)
+            except ValidationError as e:
+                error += 1
+                logger.warning(
+                    "Failed to validate %s data, for item %s, %s", model, k, e.errors
+                )
+
+                if error > error_threshold:
+                    raise RuntimeError(
+                        "Too many model validation error, something is wrong"
+                    )
+
+    # @overload
+    # def _iterate_raw(
+    #     self,
+    #     kind: str,
+    #     mode: Literal[MtgJsonMode.DICT_OF_MODEL],
+    # ) -> AsyncGenerator[DictOfModel, None]: ...
+    #
+    # @overload
+    # def _iterate_raw(
+    #     self,
+    #     kind: str,
+    #     mode: Literal[MtgJsonMode.DICT_OF_MODEL],
+    #     ijson_path: str
+    # ) -> AsyncGenerator[DictOfModel, None]: ...
+    #
+    # @overload
+    # def _iterate_raw(
+    #     self,
+    #     kind: str,
+    #     mode: Literal[MtgJsonMode.DICT_OF_LIST_OF_MODEL],
+    # ) -> AsyncGenerator[DictOfListOfModel, None]: ...
+    #
+    # @overload
+    # def _iterate_raw(
+    #     self,
+    #     kind: str,
+    #     mode: Literal[MtgJsonMode.DICT_OF_LIST_OF_MODEL],
+    #     ijson_path: str
+    # ) -> AsyncGenerator[DictOfListOfModel, None]: ...
+    #
+    # @overload
+    # def _iterate_raw(
+    #     self,
+    #     kind: str,
+    #     mode: Literal[MtgJsonMode.LIST_OF_MODEL],
+    # ) -> AsyncGenerator[ListOfModel, None]: ...
+    #
+    # @overload
+    # def _iterate_raw(
+    #     self,
+    #     kind: str,
+    #     mode: Literal[MtgJsonMode.LIST_OF_MODEL],
+    #     ijson_path: str
+    # ) -> AsyncGenerator[ListOfModel, None]: ...
+
+    async def _iterate_raw(
+        self,
+        kind: str,
+        mode: MtgJsonMode,
+        ijson_path: Optional[str] = None,
+    ) -> AsyncGenerator[GeneratorModel, None]:
+        path = f"/api/v{self.version}/{kind}.json"
+        if self.compression != MtgJsonCompression.NONE:
+            path += "." + self.compression.value
+
+        compression = self.compression.to_stream_compression()
+
+        generator: Callable[
+            [Any, Any, Optional[str]], AsyncGenerator[GeneratorModel, None]
+        ] = dict_of_model_generator
+        if mode == MtgJsonMode.LIST_OF_MODEL:
+            generator = list_of_model_generator
+        elif mode == MtgJsonMode.DICT_OF_LIST_OF_MODEL:
+            generator = dict_of_list_of_model_generator
+
+        async with self.client.stream("GET", path) as f:
+            try:
+                f.raise_for_status()
+            except HTTPStatusError as e:
+                raise ServiceError(
+                    message="Failed to fetch data from Mtg JSON",
+                    url=e.request.url,
+                    method=e.request.method,
+                    status=e.response.status_code,
+                    data=e.response.content,
+                )
 
-        for item_list in iterator:
-            current_tag = item_list.get("tag", "")
-            if tag is not None and str(tag) != current_tag:
-                continue
-
-            for index, item in enumerate(item_list.get("cardviews", [])):
-                yield current_tag, page, index, item,
-
-            while item_list.get("more"):
-                item_list = await self._get_static_page(f"{item_list.get('more')}")
-                page += 1
-                for index, item in enumerate(item_list.get("cardviews", [])):
-                    yield current_tag, page, index, item
-
-
-def slugify(string: Optional[str]):
-    import slugify
-
-    if string is None:
-        return None
-    return slugify.slugify(
-        string, separator="-", replacements=[("'", ""), ("+", "plus-")]
-    )
+            async with compressor.open(f.aiter_bytes(), compression=compression) as bit:
+                async for item in generator(self.ijson, bit, ijson_path):
+                    yield item
+
+
+async def dict_of_list_of_model_generator(
+    ijson, bytes_iterator, ijson_path=None
+) -> AsyncGenerator[DictOfListOfModel, None]:
+    if not ijson_path:
+        ijson_path = "data"
+    async for k, l in ijson.kvitems_async(bytes_iterator, ijson_path):
+        for i, v in enumerate(l, start=1):
+            yield (k, i), v
+
+
+async def list_of_model_generator(
+    ijson, bytes_iterator, ijson_path=None
+) -> AsyncGenerator[ListOfModel, None]:
+    if not ijson_path:
+        ijson_path = "data.item"
+    async for i, v in asyncstdlib.enumerate(
+        ijson.items_async(bytes_iterator, ijson_path)
+    ):
+        yield i, v
+
+
+async def dict_of_model_generator(
+    ijson, bytes_iterator, ijson_path=None
+) -> AsyncGenerator[DictOfModel, None]:
+    if not ijson_path:
+        ijson_path = "data"
+    async for k, v in ijson.kvitems_async(bytes_iterator, ijson_path):
+        yield k, v
```

### Comparing `mightstone-0.4.0/src/mightstone/services/mtgjson/__init__.py` & `mightstone-0.8.1/src/mightstone/services/edhrec/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,489 +1,482 @@
-"""
-MTGJSON support core
-"""
-
-import json
+import logging
 from enum import Enum
-from typing import Any, AsyncGenerator, List, Optional, Tuple, Type, TypeVar, Union
+from typing import AsyncGenerator, List, Optional, Tuple, Union
 
-from aiostream.stream import enumerate as aenumerate
+import asyncstdlib
 from httpx import HTTPStatusError
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 
-from mightstone import logger
-from mightstone.ass import compressor
+from mightstone.ass import sync_generator, synchronize
 from mightstone.services import MightstoneHttpClient, ServiceError
-from mightstone.services.mtgjson.models import (
-    Card,
-    CardAtomic,
-    CardAtomicGroup,
-    CardPrices,
-    CardSet,
-    CardTypes,
-    Deck,
-    DeckList,
-    Keywords,
-    Meta,
-    Set,
-    SetList,
-    TcgPlayerSKU,
-    TcgPlayerSKUs,
+from mightstone.services.edhrec.models import (
+    EdhRecCardItem,
+    EdhRecCategory,
+    EdhRecCommander,
+    EdhRecFilterQuery,
+    EdhRecPeriod,
+    EdhRecRecs,
+    slugify,
 )
 
+logger = logging.getLogger("mightstone")
 
-class MtgJsonMode(Enum):
-    """
-    Available data parse mode
-
-    MTGJSON model is not consistent, this enum describe the expected data structure
-    of a MTGJSON response
-    """
-
-    LIST_OF_MODEL = 0
-    """
-    In this mode, we expect a structure similar to
-     .. code-block:: json
-     {"data": [{"prop": 1}, "b": {"prop": 2}]}
-    """
-    DICT_OF_MODEL = 1
-    """
-    In this mode, we expect a structure similar to
-     .. code-block:: json
-     {"data": {"a": {"prop": 1}, "b": {"prop": 2}}}
-    """
-    DICT_OF_LIST_OF_MODEL = 2
-    """
-    In this mode, we expect a structure similar to
-     .. code-block:: json
-     {"data": {"a": [{"prop": 1}], "b": [{"prop": 2}]}}
-    """
-
-
-class MtgJsonCompression(str, Enum):
-    """
-    Available compression mode enumerator
-
-    MTGJSON provide 5 compression formats, Mightstone support 4 of them.
-    """
 
+class EdhRecIdentity(str, Enum):
+    COLORLESS = "colorless"
+    W = "w"
+    U = "u"
+    B = "b"
+    R = "r"
+    G = "g"
+    WU = "wu"
+    UB = "ub"
+    BR = "br"
+    RG = "rg"
+    GW = "gw"
+    WB = "wb"
+    UR = "ur"
+    BG = "bg"
+    RW = "rw"
+    GU = "gu"
+    WUB = "wub"
+    UBR = "ubr"
+    BRG = "brg"
+    RGW = "rgw"
+    GWU = "gwu"
+    WBG = "wbg"
+    URW = "urw"
+    BGU = "bgu"
+    RWB = "rwb"
+    GUR = "gur"
+    WUBR = "wubr"
+    UBRG = "ubrg"
+    BRGW = "brgw"
+    RGWU = "rgwu"
+    GWUB = "gwub"
+    WUBRG = "wubrg"
+
+
+class EdhRecTag(str, Enum):
+    TRIBES = "tribes"
+    SET = "sets"
     NONE = ""
-    """ No compression, use raw JSON """
-    XZ = "xz"
-    """ LZMA compression, use .xz files """
-    ZIP = "zip"
-    """ ZIP compression, use .zip files (not supported)"""
-    GZIP = "gz"
-    """ GZIP compression, use .gz files"""
-    BZ2 = "bz2"
-    """ BZIP2 compression, use .bz2 files"""
+    THEME_POPULARITY = "themesbypopularitysort"
+    THEME = "themes"
+    COMMANDER = "topcommanders"
+    COMPANION = "companions"
 
-    def to_stream_compression(self):
-        """
-        Compute the compression type to a python module
 
-        :return: the name of the python module
-        """
-        if self.value == "":
-            return None
-        elif self.value == "xz":
-            return "lzma"
-        elif self.value == "gz":
-            return "gzip"
-        elif self.value == "bz2":
-            return "bzip2"
-        raise ValueError(f"{self.name} compression protocol cannot be read as a stream")
+class EdhRecType(str, Enum):
+    CREATURE = "creatures"
+    INSTANT = "instants"
+    SORCERY = "sorceries"
+    ARTIFACT = "artifacts"
+    ARTIFACT_EQUIPMENT = "equipment"
+    ARTIFACT_UTILITY = "utility-artifacts"
+    ARTIFACT_MANA = "mana-artifacts"
+    ENCHANTMENT = "enchantments"
+    ENCHANTMENT_AURA = "auras"
+    PLANESWALKER = "planeswalker"
+    LAND = "lands"
+    LAND_UTILITY = "utility-lands"
+    LAND_FIXING = "color-fixing-lands"
 
 
-T = TypeVar("T")
-
-
-class MtgJson(MightstoneHttpClient):
+class EdhRecApi(MightstoneHttpClient):
     """
-    MTGJSON client
-
-    Supports compression and will get gzip versions by default.
+    HTTP client for dynamic data hosted at https://edhrec.com/api/
     """
 
-    base_url = "https://mtgjson.com"
-
-    def __init__(
-        self,
-        compression: MtgJsonCompression = None,
-        version: int = 5,
-        *args,
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
-        self.version = int(version)
-        if compression is None:
-            compression = MtgJsonCompression.GZIP
-        self.compression = MtgJsonCompression(compression)
+    base_url = "https://edhrec.com"
 
-    async def all_printings(self) -> AsyncGenerator[CardSet, None]:
+    async def recommendations_async(self, commanders: List[str], cards: List[str]):
         """
-        all Card (Set) cards, including all printings and variations, categorized by
-        set.
-
-        :return: An async iterator of CardSet
-        """
-        async for k, item in self._iterate_model(
-            kind="AllPrintings", model=Set, mode=MtgJsonMode.DICT_OF_MODEL
-        ):
-            yield item
+        Obtain EDHREC recommendations for a given commander (or partners duo)
+        for a given set of cards in the deck.
 
-    async def all_identifiers(self) -> AsyncGenerator[Card, None]:
+        Returns a list of 99 suggested cards not contained in the list
+        :param commanders: A list of one or two commander card name
+        :param cards: A list of card name
+        :exception ClientResponseError
+        :returns An EdhRecRecs object
         """
-        all Card (Set) cards organized by card UUID.
-
-        :return: An async iterator of Card object (either CardToken, or CardSet)
-        """
-        async for k, item in self._iterate_model(kind="AllIdentifiers", model=Card):
-            yield item
-
-    async def all_prices(self) -> AsyncGenerator[CardPrices, None]:
-        """
-        all prices of cards in various formats.
-
-        :return: An async iterator of CardPrices
-        """
-        async for k, item in self._iterate_model(kind="AllPrices"):
-            yield CardPrices(uuid=k, **item)
-
-    async def atomic_cards(self) -> AsyncGenerator[CardAtomic, None]:
-        """
-        every Card (Atomic) card.
-
-        :return: An async iterator of ``CardAtomicGroup``
-        """
-        async for item in self._atomic(kind="AtomicCards"):
-            yield item
-
-    async def card_types(self) -> CardTypes:
-        """
-        every card type of any type of card.
-
-        :return: A ``CardTypes`` object
-        """
-        return await self._get_item("CardTypes", model=CardTypes)
-
-    async def compiled_list(self) -> List[str]:
-        """
-        all individual outputs from MTGJSON, such as AllPrintings, CardTypes, etc.
+        try:
+            session = self.client
+            async with session.post(
+                "/api/recs/",
+                json={"cards": cards, "commanders": commanders},
+            ) as f:
+                f.raise_for_status()
+                data = await f.json()
 
-        :return: A list of string
-        """
-        return await self._get_item("CompiledList", model=list)
+                if data.get("errors"):
+                    raise ServiceError(
+                        message=data.get("errors")[0],
+                        data=data,
+                        url=f.request_info.real_url,
+                        status=f.status,
+                    )
 
-    async def deck_list(self) -> AsyncGenerator[DeckList, None]:
-        """
-        all individual Deck data.
+                return EdhRecRecs.model_validate(data)
 
-        :return: An async iterator of DeckList
-        """
-        async for i, item in self._iterate_model(
-            kind="DeckList", model=DeckList, mode=MtgJsonMode.LIST_OF_MODEL
-        ):
-            yield item
+        except HTTPStatusError as e:
+            raise ServiceError(
+                message="Failed to fetch data from EDHREC",
+                url=e.request.url,
+                status=e.response.status_code,
+            )
 
-    async def deck(self, file_name: str) -> Deck:
-        """
-        Recovers a deck data
+    recommendations = synchronize(recommendations_async)
 
-        :param file_name: the deck file_name
-        :return: A ``Deck`` object
+    async def filter_async(
+        self, commander: str, query: EdhRecFilterQuery
+    ) -> EdhRecCommander:
         """
-        return await self._get_item(f"decks/{file_name}", model=Deck)
+        Read Commander related information, and return an EdhRecCommander object
 
-    async def enum_values(self) -> dict:
+        :param commander: Commander name or slug
+        :param query: An EdhRecFilterQuery object describing the request
+        :return: An EdhRecCommander representing answer
         """
-        All known property values for various Data Models.
+        try:
+            session = await self.client
+            async with session.get(
+                "/api/filters/",
+                params={
+                    "f": str(query),
+                    "dir": "commanders",
+                    "cmdr": slugify(commander),
+                },
+            ) as f:
+                f.raise_for_status()
+                return EdhRecCommander.parse_payload(await f.json())
 
-        :return: a ``dict`` object
-        """
-        return await self._get_item("EnumValues", model=dict)
+        except HTTPStatusError as e:
+            raise ServiceError(
+                message="Failed to fetch data from EDHREC",
+                url=e.request.url,
+                status=e.response.status_code,
+            )
 
-    async def keywords(self) -> Keywords:
-        """
-        a list of possible all keywords used on all cards.
+    filter = synchronize(filter_async)
 
-        :return: A ``Keywords`` object
-        """
-        return await self._get_item("Keywords", model=Keywords)
 
-    async def legacy(self) -> AsyncGenerator[Set, None]:
-        """
-        all Card (Set) cards organized by Set, restricted to sets legal in the
-        Legacy format.
+class EdhRecStatic(MightstoneHttpClient):
+    """
+    HTTP client for static JSON data hosted at https://json.edhrec.com
+    """
 
-        :return: An async iterator of ``Set``
-        """
-        async for k, item in self._iterate_model(kind="Legacy", model=Set):
-            yield item
+    base_url = "https://json.edhrec.com"
 
-    async def legacy_atomic(self) -> AsyncGenerator[CardAtomicGroup, None]:
+    async def commander_async(
+        self, name: str, sub: Optional[str] = None
+    ) -> EdhRecCommander:
         """
-        all Card (Set) cards organized by Set, restricted to sets legal in the
-        Legacy format.
 
-        :return: An async iterator of ``CardAtomicGroup``
+        :param name: Commander
+        :param sub:
+        :return:
         """
-        async for item in self._atomic(kind="LegacyAtomic"):
-            yield item
+        path = f"commanders/{slugify(name)}.json"
+        if sub:
+            path = f"commanders/{slugify(name)}/{slugify(sub)}.json"
 
-    async def meta(self) -> Meta:
-        """
-        the metadata object with ISO 8601 dates for latest build and SemVer
-        specifications of the MTGJSON release.
+        data = await self._get_static_page(path)
 
-        :return: A Meta object
-        """
-        return await self._get_item("Meta", model=Meta)
+        return EdhRecCommander.parse_payload(data)
 
-    async def modern(self) -> AsyncGenerator[Set, None]:
-        """
-        all Card (Set) cards organized by Set, restricted to sets legal in the
-        Modern format.
+    commander = synchronize(commander_async)
 
-        :return: An async iterator of ``Set``
-        """
-        async for k, item in self._iterate_model(kind="Modern", model=Set):
-            yield item
+    async def tribes_async(
+        self,
+        identity: Optional[Union[EdhRecIdentity, str]] = None,
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        if identity:
+            identity = EdhRecIdentity(identity)
+            async for item in self._page_item_generator(
+                f"commanders/{identity.value}.json",
+                EdhRecTag.TRIBES,
+                related=True,
+                limit=limit,
+            ):
+                yield item
+        else:
+            async for item in self._page_item_generator(
+                "tribes.json", EdhRecTag.TRIBES, limit=limit
+            ):
+                yield item
 
-    async def modern_atomic(self) -> AsyncGenerator[CardAtomicGroup, None]:
-        """
-        all Card (Atomic) cards, restricted to cards legal in the Modern format.
+    tribes = sync_generator(tribes_async)
 
-        :return: An async iterator of ``CardAtomicGroup``
-        """
-        async for item in self._atomic(kind="ModernAtomic"):
+    async def themes_async(
+        self,
+        identity: Optional[Union[EdhRecIdentity, str]] = None,
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        if identity:
+            identity = EdhRecIdentity(identity)
+            async for item in self._page_item_generator(
+                f"commanders/{identity.value}.json",
+                EdhRecTag.THEME,
+                related=True,
+                limit=limit,
+            ):
+                yield item
+        else:
+            async for item in self._page_item_generator(
+                "themes.json", EdhRecTag.THEME_POPULARITY, limit=limit
+            ):
+                yield item
+
+    themes = sync_generator(themes_async)
+
+    async def sets_async(
+        self, limit: Optional[int] = None
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        async for item in self._page_item_generator(
+            "sets.json", EdhRecTag.SET, limit=limit
+        ):
             yield item
 
-    async def pauper_atomic(self) -> AsyncGenerator[CardAtomicGroup, None]:
-        """
-        all Card (Atomic) cards, restricted to cards legal in the Pauper format.
+    sets = sync_generator(sets_async)
 
-        :return: An async iterator of ``CardAtomicGroup``
-        """
-        async for item in self._atomic(kind="PauperAtomic"):
+    async def salt_async(
+        self, year: Optional[int] = None, limit: Optional[int] = None
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        path = "top/salt.json"
+        if year:
+            path = f"top/salt-{year}.json"
+        async for item in self._page_item_generator(path, limit=limit):
             yield item
 
-    async def pioneer(self) -> AsyncGenerator[Set, None]:
-        """
-        all Card (Set) cards organized by Set, restricted to cards legal in the
-        Pioneer format.
+    salt = sync_generator(salt_async)
 
-        :return: An async iterator of ``Set``
-        """
-        async for k, item in self._iterate_model(kind="Pioneer", model=Set):
+    async def top_cards_async(
+        self,
+        type: Optional[EdhRecType] = None,
+        period: EdhRecPeriod = EdhRecPeriod.PAST_WEEK,
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        period = EdhRecPeriod(period)
+        if type:
+            type = EdhRecType(type)
+            async for item in self._page_item_generator(
+                f"top/{type.value}.json", period, limit=limit
+            ):
+                yield item
+            return
+
+        if period == EdhRecPeriod.PAST_WEEK:
+            path = "top/week.json"
+        elif period == EdhRecPeriod.PAST_MONTH:
+            path = "top/month.json"
+        else:
+            path = "top/year.json"
+        async for item in self._page_item_generator(path, limit=limit):
             yield item
 
-    async def pioneer_atomic(self) -> AsyncGenerator[CardAtomicGroup, None]:
-        """
-        all Card (Atomic) cards, restricted to cards legal in the Pioneer format.
+    top_cards = sync_generator(top_cards_async)
 
-        :return: An async iterator of ``CardAtomicGroup``
-        """
-        async for item in self._atomic(kind="PioneerAtomic"):
-            yield item
-
-    async def set_list(self) -> AsyncGenerator[SetList, None]:
-        """
-        a list of meta data for all Set data.
+    async def cards_async(
+        self,
+        theme: Optional[str] = None,
+        commander: Optional[str] = None,
+        identity: Optional[Union[EdhRecIdentity, str]] = None,
+        set: Optional[str] = None,
+        category: Optional[EdhRecCategory] = None,
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        if category:
+            category = EdhRecCategory(category)
+
+        if not theme and not commander and not set:
+            raise ValueError("You must either provide a theme, commander or set")
+
+        if commander:
+            if theme:
+                raise ValueError("commander and theme options are mutually exclusive")
+            if identity:
+                raise ValueError(
+                    "commander and identity options are mutually exclusive"
+                )
+            if set:
+                raise ValueError("commander and set options are mutually exclusive")
 
-        :return: An async iterator of ``SetList``
-        """
-        async for k, item in self._iterate_model(
-            kind="SetList", model=SetList, mode=MtgJsonMode.LIST_OF_MODEL
+            slug = slugify(commander)
+            path = f"commanders/{slug}.json"
+            if theme:
+                path = f"commanders/{slug}/{slugify(theme)}.json"
+            async for item in self._page_item_generator(path, category, limit=limit):
+                yield item
+
+            return
+
+        if set:
+            if theme:
+                raise ValueError("set and theme options are mutually exclusive")
+            if identity:
+                raise ValueError("set and identity options are mutually exclusive")
+            async for item in self._page_item_generator(
+                f"sets/{slugify(set)}.json", category, limit=limit
+            ):
+                yield item
+            return
+
+        if identity and not theme:
+            raise ValueError("you must specify a theme to search by color identity")
+
+        path = f"themes/{slugify(theme)}.json"
+        if identity:
+            identity = EdhRecIdentity(identity)
+            path = f"themes/{slugify(theme)}/{identity.value}.json"
+        async for item in self._page_item_generator(path, category, limit=limit):
+            yield item
+
+    cards = sync_generator(cards_async)
+
+    async def companions_async(
+        self, limit: Optional[int] = None
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        async for item in self._page_item_generator(
+            "companions.json", EdhRecTag.COMPANION, limit=limit
         ):
             yield item
 
-    async def set(self, code: str) -> SetList:
-        """
-        Get a Set data
-
-        :param code: The set identifier, such as "IKO" for "Ikoria, lair of the
-                     monsters"
-
-        :return: The set representation
-        """
-        return await self._get_item(code, SetList)
-
-    async def standard(self) -> AsyncGenerator[Set, None]:
-        """
-        all Card (Set) cards organized by Set, restricted to cards legal in the
-        Standard format.
+    companions = sync_generator(companions_async)
 
-        :return: An async iterator of ``Set``
-        """
-        async for k, item in self._iterate_model(kind="Standard", model=Set):
-            yield item
-
-    async def standard_atomic(self) -> AsyncGenerator[CardAtomicGroup, None]:
-        """
-        all Card (Atomic) cards, restricted to cards legal in the Standard format.
-
-        :return: An async iterator of ``CardAtomicGroup``
-        """
-        async for item in self._atomic(kind="StandardAtomic"):
+    async def partners_async(
+        self,
+        identity: Optional[Union[EdhRecIdentity, str]] = None,
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        path = "partners.json"
+        if identity:
+            identity = EdhRecIdentity(identity)
+            path = f"partners/{identity.value}.json"
+        async for item in self._page_item_generator(path, limit=limit):
             yield item
 
-    async def tcg_player_skus(self) -> AsyncGenerator[TcgPlayerSKUs, None]:
-        """
-        TCGplayer SKU information based on card UUIDs.
+    partners = sync_generator(partners_async)
 
-        :return: an async iterator of ``TcgPlayerSKUs``
-        """
-        group: Optional[TcgPlayerSKUs] = None
-        async for (k, i), item in self._iterate_model(
-            kind="TcgplayerSkus",
-            model=TcgPlayerSKU,
-            mode=MtgJsonMode.DICT_OF_LIST_OF_MODEL,
+    async def commanders_async(
+        self,
+        identity: Optional[Union[EdhRecIdentity, str]] = None,
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        path = "commanders.json"
+        if identity:
+            identity = EdhRecIdentity(identity)
+            path = f"commanders/{identity.value}.json"
+        async for item in self._page_item_generator(path, limit=limit):
+            yield item
+
+    commanders = sync_generator(commanders_async)
+
+    async def combos_async(
+        self, identity: Union[EdhRecIdentity, str], limit: Optional[int] = None
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        identity = EdhRecIdentity(identity)
+        async for item in self._page_item_generator(
+            f"combos/{identity.value}.json", limit=limit
         ):
-            if not group or k != group.uuid:
-                if group:
-                    yield group
-                group = TcgPlayerSKUs(uuid=k, skus=[])
-            group.skus.append(item)
-
-        yield group
-
-    async def vintage(self) -> AsyncGenerator[Set, None]:
-        """
-        all Card (Set) cards organized by Set, restricted to sets legal in the
-        Vintage format.
-
-        :return: An async iterator of ``Set``
-        """
-        async for k, item in self._iterate_model(kind="Vintage", model=Set):
             yield item
 
-    async def vintage_atomic(self) -> AsyncGenerator[CardAtomicGroup, None]:
-        """
-        all Card (Atomic) cards, restricted to sets legal in the Vintage format.
-
-        :return: An async iterator of ``CardAtomicGroup``
-        """
-        async for item in self._atomic(kind="VintageAtomic"):
-            yield item
+    combos = sync_generator(combos_async)
 
-    async def _atomic(self, kind: str) -> AsyncGenerator[CardAtomicGroup, None]:
-        group: Optional[CardAtomicGroup] = None
-        async for (k, i), item in self._iterate_model(
-            kind=kind, model=CardAtomic, mode=MtgJsonMode.DICT_OF_LIST_OF_MODEL
+    async def combo_async(
+        self,
+        identity: str,
+        identifier: Union[EdhRecIdentity, str],
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        identity = EdhRecIdentity(identity)
+        async for item in self._page_item_generator(
+            f"combos/{identity.value}/{int(identifier)}.json", limit=limit
         ):
-            if not group or k != group.name:
-                if group:
-                    yield group
-                group = CardAtomicGroup(name=k, prints=[])
-            group.prints.append(item)
+            yield item
 
-        yield group
+    combo = sync_generator(combo_async)
 
-    async def _get_item(
+    async def _page_item_generator(
         self,
-        kind: str,
-        model: Type[T] = dict,
-        **kwargs,
-    ) -> T:
-        path = f"/api/v{self.version}/{kind}.json"
-        if self.compression != MtgJsonCompression.NONE:
-            path += "." + self.compression.value
+        path,
+        tag: Optional[
+            Union[EdhRecTag, EdhRecType, EdhRecPeriod, EdhRecCategory]
+        ] = None,
+        related=False,
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[EdhRecCardItem, None]:
+        """
+        Async generator that will wrap Pydantic validation
+        and ensure that no validation error are raised
+        """
+        ttag: Optional[str] = None
+        if tag:
+            ttag = tag.value
+
+        enumerator = asyncstdlib.enumerate(self._get_page(path, ttag, related))
+        async with asyncstdlib.scoped_iter(enumerator) as protected_enumerator:
+            async for i, (ttag, page, index, item) in protected_enumerator:
+                if limit and i == limit:
+                    logger.debug(f"Reached limit of {limit}, stopping iteration")
+                    return
 
+                try:
+                    yield EdhRecCardItem.parse_payload(item, ttag)
+                except ValidationError as e:
+                    logger.warning(
+                        "Failed to parse an EDHREC item from %s at page %d, index %d",
+                        path,
+                        page,
+                        index,
+                    )
+                    logger.debug(e.json())
+
+    async def _get_static_page(self, path) -> dict:
         try:
-            async with self.client.stream("GET", path, **kwargs) as f:
-                async with compressor.open(
-                    f.aiter_bytes(),
-                    compression=self.compression.to_stream_compression(),
-                ) as f2:
-                    data = json.loads(await f2.read())
-                    data = data.get("data")
-
-                    try:
-                        return model.parse_obj(data)
-                    except AttributeError:
-                        return model(data)
-        except ValidationError as e:
-            raise ServiceError(
-                message=f"Failed to validate {model} data, {e.errors()}",
-                url=path,
-                method="GET",
-                status=None,
-                data=e,
-            )
+            f = await self.client.get(f"/pages/{path}")
+            f.raise_for_status()
+            return f.json()
         except HTTPStatusError as e:
             raise ServiceError(
-                message="Failed to fetch data from MTG Json",
+                message="Failed to fetch data from EDHREC",
                 url=e.request.url,
-                method=e.request.method,
                 status=e.response.status_code,
-                data=None,
             )
 
-    async def _iterate_model(
-        self, model: Type[T] = dict, error_threshold: int = 10, **kwargs
-    ) -> AsyncGenerator[Tuple[Union[str, int, Tuple[str, int]], T], None]:
-        error = 0
-        async for k, v in self._iterate_raw(**kwargs):
-            try:
-                try:
-                    yield k, model.parse_obj(v)
-                except AttributeError:
-                    yield k, model(v)
-            except ValidationError as e:
-                error += 1
-                logger.warning(
-                    "Failed to validate %s data, for item %s, %s", model, k, e.errors
-                )
-
-                if error > error_threshold:
-                    raise RuntimeError(
-                        "Too many model validation error, something is wrong"
-                    )
+    async def _get_page(
+        self, path, tag: Optional[str] = None, related=False
+    ) -> AsyncGenerator[Tuple[str, int, int, dict], None]:
+        """
+        Read a EDHREC page data, and return it as a tuple:
+        - tag as string
+        - page
+        - index
+        - the payload itself
+        """
+        data = await self._get_static_page(path)
+        page = 1
+
+        if related:
+            iterator = [
+                {"tag": tag, "cardviews": data.get("relatedinfo", {}).get(tag, [])}
+            ]
+        else:
+            iterator = (
+                data.get("container", {}).get("json_dict", {}).get("cardlists", [])
+            )
 
-    async def _iterate_raw(
-        self,
-        kind: str,
-        ijson_path: str = None,
-        mode: MtgJsonMode = MtgJsonMode.DICT_OF_MODEL,
-    ) -> AsyncGenerator[Tuple[Union[str, int, Tuple[str, int]], Any], None]:
-        path = f"/api/v{self.version}/{kind}.json"
-        if self.compression != MtgJsonCompression.NONE:
-            path += "." + self.compression.value
-
-        logger.debug("Fetching %s", path)
-        async with self.client.stream("GET", path) as f:
-            try:
-                f.raise_for_status()
-                logger.debug("Reading %s", path)
-                # TODO: also grab meta.version and meta.date
-                async with compressor.open(
-                    f.aiter_bytes(),
-                    compression=self.compression.to_stream_compression(),
-                ) as f2:
-                    if mode == MtgJsonMode.DICT_OF_MODEL:
-                        if not ijson_path:
-                            ijson_path = "data"
-                        async for k, v in self.ijson.kvitems_async(f2, ijson_path):
-                            yield k, v
-                    elif mode == MtgJsonMode.LIST_OF_MODEL:
-                        if not ijson_path:
-                            ijson_path = "data.item"
-                        async for i, v in aenumerate(
-                            self.ijson.items_async(f2, ijson_path)
-                        ):
-                            yield i, v
-                    elif mode == MtgJsonMode.DICT_OF_LIST_OF_MODEL:
-                        if not ijson_path:
-                            ijson_path = "data"
-                        async for k, l in self.ijson.kvitems_async(f2, ijson_path):
-                            for i, v in enumerate(l, start=1):
-                                yield (k, i), v
-                logger.debug("Done %s", path)
-            except HTTPStatusError as e:
-                raise ServiceError(
-                    message="Failed to fetch data from Mtg JSON",
-                    url=e.request.url,
-                    method=e.request.method,
-                    status=e.response.status_code,
-                    data=e.response.content,
-                )
+        for item_list in iterator:
+            current_tag = item_list.get("tag", "")
+            if tag is not None and str(tag) != current_tag:
+                continue
+
+            for index, item in enumerate(item_list.get("cardviews", [])):
+                yield current_tag, page, index, item,
+
+            while item_list.get("more"):
+                item_list = await self._get_static_page(f"{item_list.get('more')}")
+                page += 1
+                for index, item in enumerate(item_list.get("cardviews", [])):
+                    yield current_tag, page, index, item
```

### Comparing `mightstone-0.4.0/src/mightstone/services/scryfall/__init__.py` & `mightstone-0.8.1/src/mightstone/services/scryfall/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Scryfall.com support classes
 """
 
-from typing import Any, List, Union
+from typing import Dict, List, Optional, TypeVar, Union, cast
 
 import ijson
 from httpx import HTTPStatusError
-from pydantic.error_wrappers import ValidationError
-from typing_extensions import AsyncGenerator, TypeVar
+from pydantic import ValidationError
+from pydantic.networks import AnyUrl
+from typing_extensions import AsyncGenerator, Type, overload
 
+from mightstone.ass import compressor, sync_generator, synchronize
 from mightstone.services import MightstoneHttpClient, ServiceError
 from mightstone.services.scryfall.models import (
     BulkTagType,
     Card,
     CardIdentifierPath,
     Catalog,
     CatalogType,
@@ -27,72 +29,87 @@
     IdentifierNameSet,
     IdentifierOracleId,
     ManaCost,
     Migration,
     Ruling,
     RulingIdentifierPath,
     ScryfallList,
+    ScryfallModel,
     Set,
     SortStrategy,
     Symbol,
     Tag,
     UniqueStrategy,
 )
 
-T = TypeVar("T")
+_T = TypeVar("_T", bound=ScryfallModel)
 
 
 class Scryfall(MightstoneHttpClient):
     """
     Scryfall API client
     """
 
     base_url = "https://api.scryfall.com"
 
-    async def get_bulk_tags(self, tag_type: BulkTagType) -> AsyncGenerator[Tag, None]:
+    async def get_bulk_tags_async(
+        self, tag_type: BulkTagType
+    ) -> AsyncGenerator[Tag, None]:
         """
         Access the private tag repository
 
         This is an alpha feature, and could be removed later.
+
         :param tag_type: The tag type either oracle or illustration
         :return: A scryfall `Tag` instance async generator
         """
-        tag_type = BulkTagType(tag_type)
-        async with self.client.get(f"/private/tags/{tag_type}") as f:
+        async with self.client.stream("GET", f"/private/tags/{tag_type.value}") as f:
             f.raise_for_status()
-            async for current_tag in ijson.items_async(f.content, "data.item"):
-                yield Tag.parse_obj(current_tag)
+            async for current_tag in ijson.items_async(
+                compressor.open(f.aiter_bytes()), "data.item"
+            ):
+                yield Tag.model_validate(current_tag)
+
+    get_bulk_tags = sync_generator(get_bulk_tags_async)
 
-    async def get_bulk_data(self, bulk_type: str) -> AsyncGenerator[Card, None]:
+    async def get_bulk_data_async(self, bulk_type: str) -> AsyncGenerator[Card, None]:
         """
         Access the bulk cards
         This script uses ijson and should stream data on the fly
 
         See https://scryfall.com/docs/api/bulk-data for more informations
+
         :param bulk_type: A string describing the bulk export name
-        :return:
+        :return: An async iterator of ``Card``
         """
         bulk_types = []
         bulk = None
-        async with self.client.get("/bulk-data") as f:
+        async with self.client.stream("GET", "/bulk-data") as f:
             f.raise_for_status()
-            async for current_bulk in ijson.items_async(f.content, "data.item"):
+
+            async for current_bulk in ijson.items_async(
+                compressor.open(f.aiter_bytes()), "data.item"
+            ):
                 bulk_types.append(current_bulk.get("type"))
                 if current_bulk.get("type") == bulk_type:
                     bulk = current_bulk
 
         if not bulk:
             raise IndexError(f"{bulk_type} bulk type not found in {bulk_types}")
 
-        async with self.client.get(bulk.get("download_uri")) as f:
+        async with self.client.stream("GET", bulk.get("download_uri")) as f:
             f.raise_for_status()
-            async for current_card in ijson.items_async(f.content, "item"):
-                yield Card.parse_obj(current_card)
+            async for current_card in ijson.items_async(
+                compressor.open(f.aiter_bytes()), "item"
+            ):
+                yield Card.model_validate(current_card)
 
-    async def card(
+    get_bulk_data = sync_generator(get_bulk_data_async)
+
+    async def card_async(
         self, id: str, type: CardIdentifierPath = CardIdentifierPath.SCRYFALL
     ) -> Card:
         """
         Returns a single card with a given ID, or by its code set / collector number
 
         Depending on the `type` value, one of the following endpoint will be reached:
          * /cards/:id
@@ -100,41 +117,49 @@
          * /cards/multiverse/:id
          * /cards/mtgo/:id
          * /cards/arena/:id
          * /cards/cardmarket/:id
          * /cards/:code/:number
 
         :param id: The requested `Card` identifier string, for code-number, please
-        use / as separator (dmu/123) :param type: The card identifier, please refer
-        to `CardIdentifierPath` enum :return A scryfall `Card` instance
+                   use / as separator (dmu/123)
+        :param type: The card identifier, please refer to `CardIdentifierPath` enum
         :param type: Type of id researched
+        :return: A scryfall `Card` instance
         """
         type = CardIdentifierPath(type)
         path = f"/cards/{id}"
         if type.value and type != CardIdentifierPath.CODE_NUMBER:
             path = f"/cards/{type.value}/{id}"
         return await self._get_item(path, Card)
 
-    async def random(self, q: str = None) -> Card:
+    card = synchronize(card_async)
+
+    async def random_async(self, q: Optional[str] = None) -> Card:
         """
         Returns a single random Card object.
 
         This method will use:
         - /cards/random
 
         :param q: The optional parameter q supports the same fulltext search system
-        that the main site uses. Providing q will filter the pool of cards before
-        returning a random entry. :return A scryfall `Card` instance
+                  that the main site uses. Providing q will filter the pool of cards
+                  before returning a random entry.
+        :return: A scryfall `Card` instance
         """
         params = {}
         if q:
             params["q"] = q
-        return await self._get_item("/cards/random", Card, params=params)
+        return await self._get_item(
+            "/cards/random", Card, params=params, headers={"cache-control": "no-cache"}
+        )
 
-    async def search(
+    random = synchronize(random_async)
+
+    async def search_async(
         self,
         q: str,
         unique: UniqueStrategy = UniqueStrategy.CARDS,
         order: SortStrategy = SortStrategy.NAME,
         dir: DirectionStrategy = DirectionStrategy.AUTO,
         include_extras=False,
         include_multilingual=False,
@@ -145,23 +170,24 @@
         Returns a List object containing Cards found using a fulltext search string.
         This string supports the same fulltext search system that the main site uses.
 
         :param unique: The strategy for omitting similar cards.
         :param order: The method to sort returned cards.
         :param dir: The direction to sort cards.
         :param include_extras: If true, extra cards (tokens, planes, etc) will be
-               included. Equivalent to adding include:extras to the fulltext search.
+                               included. Equivalent to adding include:extras to the
+                               fulltext search.
         :param include_multilingual: If true, cards in every language supported by
-               Scryfall will be included.
+                                     Scryfall will be included.
         :param include_variations: If true, rare care variants will be included,
-        like the Hairy Runesword.
+                                   like the Hairy Runesword.
         :param q: A fulltext search query.
         :param limit: The number of item to return, please note that Mightstone
-        wraps Scryfall pagination and streams the results
-        :return A scryfall `Card` instance async generator
+                      wraps Scryfall pagination and streams the results
+        :return: A scryfall `Card` instance async generator
         """
         params = {
             "unique": UniqueStrategy(unique).value,
             "order": SortStrategy(order).value,
             "dir": DirectionStrategy(dir).value,
             "include_extras": str(include_extras),
             "include_multilingual": str(include_multilingual),
@@ -169,18 +195,20 @@
             "q": q,
         }
         async for item in self._list(
             "/cards/search", params=params, model=Card, limit=limit
         ):
             yield item
 
-    async def named(self, q: str, set: str = None, exact=True):
+    search = sync_generator(search_async)
+
+    async def named_async(self, q: str, set: Optional[str] = None, exact=True) -> Card:
         """
         Returns a Card based on a name search string. This method is designed for
-        building chat bots, forum bots, and other services that need card details
+        building chatbots, forum bots, and other services that need card details
         quickly.
 
         If exact mode is on, a card with that exact name is returned. Otherwise,
         an Exception is raised because no card matches. If exact mode is off and a
         card name matches that string, then that card is returned. If not, a fuzzy
         search is executed for your card name. The server allows misspellings and
         partial words to be provided. For example: jac bele will match Jace Beleren.
@@ -189,29 +217,33 @@
         an exception will be raised describing the problem: either more than 1 one
         card matched your search, or zero cards matched.
 
         Card names are case-insensitive and punctuation is optional (you can drop
         apostrophes and periods etc). For example: fIReBALL is the same as Fireball
         and smugglers copter is the same as Smuggler's Copter.
 
-        :param q: The searched card name :param exact: Run a strict text research
-        instead of a fuzzy search :param set: You may also provide a set code in the
-        set parameter, in which case the name search and the returned card print will
-        be limited to the specified set. :return A scryfall `Card` instance
+        :param q: The searched card name
+        :param exact: Run a strict text research instead of a fuzzy search
+        :param set: You may also provide a set code in the
+                    set parameter, in which case the name search and the returned card
+                    print will be limited to the specified set.
+        :return: A scryfall `Card` instance
         """
         params = {}
         if exact:
             params["exact"] = q
         else:
             params["fuzzy"] = q
         if set:
             params["set"] = set
         return await self._get_item("/cards/named", Card, params=params)
 
-    async def autocomplete(self, q: str, include_extras=False):
+    named = synchronize(named_async)
+
+    async def autocomplete_async(self, q: str, include_extras=False) -> Catalog:
         """
         Returns a Catalog object containing up to 20 full English card names that
         could be autocompletions of the given string parameter.
 
         This method is designed for creating assistive UI elements that allow users
         to free-type card names.
         The names are sorted with the nearest match first, highly favoring results
@@ -220,121 +252,138 @@
         Spaces, punctuation, and capitalization are ignored.
 
         If q is less than 2 characters long, or if no names match, the Catalog will
         contain 0 items (instead of returning any errors).
 
         :param q: The string to autocomplete.
         :param include_extras: If true, extra cards (tokens, planes, vanguards, etc)
-               will be included.
+                               will be included.
         :return: A scryfall `Card` instance async generator
         """
         params = {"q": q}
         if include_extras:
             params["include_extras"] = include_extras
         return await self._get_item("/cards/autocomplete", Catalog, params=params)
 
-    async def collection(
+    autocomplete = synchronize(autocomplete_async)
+
+    async def collection_async(
         self,
         identifiers: List[
             Union[
                 IdentifierId,
                 IdentifierName,
                 IdentifierNameSet,
                 IdentifierMtgId,
                 IdentifierOracleId,
                 IdentifierMultiverseId,
                 IdentifierCollectorNumberSet,
                 IdentifierIllustrationId,
             ]
         ],
-    ):
+    ) -> AsyncGenerator[Card, None]:
         """
         Accepts a JSON array of card identifiers, and returns a List object with the
         collection of requested cards. A maximum of 75 card references may be
         submitted per request.
 
         :param identifiers: Each submitted card identifier must be a JSON object with
-        one or more of the keys id, mtgo_id, multiverse_id, oracle_id,
-        illustration_id, name, set, and collector_number :return: A scryfall `Card`
-        instance async generator
+                            one or more of the keys id, mtgo_id, multiverse_id,
+                            oracle_id, illustration_id, name, set, and collector_number
+        :return: A scryfall `Card` instance async generator
         """
         async for item in self._list(
             "/cards/collection", Card, verb="POST", json={"identifiers": identifiers}
         ):
             yield item
 
-    async def rulings(
+    collection = sync_generator(collection_async)
+
+    async def rulings_async(
         self,
         id: str,
         type: RulingIdentifierPath = RulingIdentifierPath.SCRYFALL,
-        limit: int = None,
-    ):
+        limit: Optional[int] = None,
+    ) -> AsyncGenerator[Ruling, None]:
         """
         Returns a single card with the given ID.
 
         Depending on the `type` value, one of the following endpoint will be reached:
          * /cards/:id/rulings
          * /cards/multiverse/:id/rulings
          * /cards/mtgo/:id/rulings
          * /cards/arena/:id/rulings
 
         :param id: The requested `Card` identifier string. In the case of card-number,
-        use set/number (separated by a slash, for instance dmu/123)
+                   use set/number (separated by a slash, for instance dmu/123)
         :param type: The card identifier, please refer to `RulingIdentifierPath` enum
-        :return A scryfall `Ruling` instance async generator
+        :return: A scryfall `Ruling` instance async generator
         """
         type = RulingIdentifierPath(type)
         path = f"/cards/{id}/rulings"
         if type.value and type != RulingIdentifierPath.CODE_NUMBER:
             path = f"/cards/{type.value}/{id}/rulings"
 
         async for item in self._list(path, Ruling, limit=limit):
             yield item
 
-    async def symbols(self, limit: int = None):
+    rulings = sync_generator(rulings_async)
+
+    async def symbols_async(
+        self, limit: Optional[int] = None
+    ) -> AsyncGenerator[Symbol, None]:
         """
         Returns a List of all Card Symbols.
 
         :param limit: The number of item to return, please note that Mightstone
-        wraps Scryfall pagination and streams the results
+                      wraps Scryfall pagination and streams the results
         :return: A scryfall `Symbol` instance async generator
         """
         async for item in self._list("/symbology", Symbol, limit=limit):
             yield item
 
-    async def parse_mana(self, cost: str):
+    symbols = sync_generator(symbols_async)
+
+    async def parse_mana_async(self, cost: str) -> ManaCost:
         """
         Parses the given mana cost parameter and returns Scryfall’s interpretation.
 
         The server understands most community shorthand for mana costs (such as 2WW
         for {2}{W}{W}). Symbols can also be out of order, lowercase, or have multiple
         colorless costs (such as 2{g}2 for {4}{G}).
 
         If part of the string could not be understood, the server will raise an Error
         object describing the problem.
 
+        :param cost: A mana cost string
         :return: A `ManaCost` instance
         """
         return await self._get_item(
             "/symbology/parse-mana", ManaCost, params={"cost": cost}
         )
 
-    async def catalog(self, type: CatalogType):
+    parse_mana = synchronize(parse_mana_async)
+
+    async def catalog_async(self, type: CatalogType) -> Catalog:
         """
         A Catalog object contains an array of Magic datapoints (words, card values,
         etc). Catalog objects are provided by the API as aids for building other
         Magic software and understanding possible values for a field on Card objects.
 
         :param type: See `CatalogType` for more informations
         :return: A `Catalog` instance
         """
         type = CatalogType(type)
         return await self._get_item(f"/catalog/{type.value}", Catalog)
 
-    async def migrations(self, limit: int = None):
+    catalog = synchronize(catalog_async)
+
+    async def migrations_async(
+        self, limit: Optional[int] = None
+    ) -> AsyncGenerator[Migration, None]:
         """
         For the vast majority of Scryfall’s database, Magic card entries are additive.
         We add new and upcoming cards as we learn about them and obtain images.
 
         In rare instances, Scryfall may discover that a card in our database does not
         really exist, or it has been deleted from a digital game permanently. In
         these situations, we provide endpoints to help you reconcile downstream data
@@ -349,120 +398,150 @@
 
         delete
         The given UUID is being discarded, and no replacement data is being provided.
         This likely means the old records are fully invalid. This migration exists to
         provide evidence that cards were removed from Scryfall’s database.
 
         :param limit: The number of item to return, please note that Mightstone wraps
-        Scryfall pagination and streams the results
+                      Scryfall pagination and streams the results
         :return: A `Migration` instance async generator
         """
         async for item in self._list("/migrations", Migration, limit=limit):
             yield item
 
-    async def migration(self, id: str):
+    migrations = sync_generator(migrations_async)
+
+    async def migration_async(self, id: str) -> Migration:
         """
         Returns a single Card Migration with the given :id
 
         :return: A `Migration` instance
         """
         return await self._get_item(f"/migrations/{id}", Migration)
 
-    async def sets(self, limit: int = None):
+    migration = synchronize(migration_async)
+
+    async def sets_async(
+        self, limit: Optional[int] = None
+    ) -> AsyncGenerator[Set, None]:
         """
         Returns a List object of all Sets on Scryfall.
 
         :param limit: The number of item to return, please note that Mightstone
-        wraps Scryfall pagination and streams the results
+                      wraps Scryfall pagination and streams the results
         :return: A `Set` instance async generator
         """
         async for item in self._list("/sets", Set, limit=limit):
             yield item
 
-    async def set(self, id_or_code: str = None) -> Set:
+    sets = sync_generator(sets_async)
+
+    async def set_async(self, id_or_code: Optional[str] = None) -> Set:
         """
         Returns a Set with the given set code.
 
         :param id_or_code: The code can be either the code or the mtgo_code or the
-        scryfall UUID for the set.
+                           scryfall UUID for the set.
         :return: A `Set` instance
         """
         return await self._get_item(f"/sets/{id_or_code}", Set)
 
-    async def _get_item(self, path, model: T = None, **kwargs) -> Union[T, Any]:
+    set = sync_generator(sets_async)
+
+    @overload
+    async def _get_item(self, path: str, model: None, **kwargs) -> Dict: ...
+
+    @overload
+    async def _get_item(self, path: str, model: Type[_T], **kwargs) -> _T: ...
+
+    async def _get_item(
+        self, path: str, model: Optional[Type[_T]] = None, **kwargs
+    ) -> Union[_T, Dict]:
         try:
-            async with self.client.get(path, **kwargs) as f:
-                if not f.ok:
-                    error = Error.parse_obj(await f.json())
-                    raise ServiceError(
-                        message=error.details,
-                        method=f.method,
-                        url=f.real_url,
-                        status=f.status,
-                        data=error,
-                    )
-                data = await f.json()
-                if model:
-                    data = model.parse_obj(data)
-                return data
+            response = await self.client.get(path, **kwargs)
+            if not response.is_success:
+                error = Error.model_validate(response.json())
+                raise ServiceError(
+                    message=error.details,
+                    method=response.request.method,
+                    url=response.request.url,
+                    status=response.status_code,
+                    data=error,
+                )
+            data = response.json()
+            if model:
+                data = model.model_validate(data)
+            return data
         except ValidationError as e:
             raise ServiceError(
                 message=f"Failed to validate {model} data, {e.errors()}",
                 url=path,
                 method="GET",
                 status=None,
                 data=e,
             )
         except HTTPStatusError as e:
             raise ServiceError(
                 message="Failed to fetch data from Scryfall",
                 url=e.request.url,
                 method=e.request.method,
                 status=e.response.status_code,
-                data=Error.parse_raw(e.response.content),
+                data=Error.model_validate_json(e.response.content),
             )
 
+    @overload
+    def _list(self, path: str, model: None, **kwargs) -> AsyncGenerator[Dict, None]: ...
+
+    @overload
+    def _list(
+        self, path: str, model: Type[_T], **kwargs
+    ) -> AsyncGenerator[_T, None]: ...
+
     async def _list(
-        self, path, model: T = None, verb="GET", limit=None, **kwargs
-    ) -> AsyncGenerator[T, None]:
+        self, path, model: Optional[Type[_T]] = None, verb="GET", limit=None, **kwargs
+    ) -> AsyncGenerator[Union[_T, Dict], None]:
         i = 0
         try:
             while True:
-                f = await self.client.request(verb, path, **kwargs)
-                if f.is_error:
+                response = await self.client.request(verb, path, **kwargs)
+                if response.is_error:
                     raise ServiceError(
                         message="Failed to fetch data from Scryfall",
-                        url=f.real_url,
-                        status=f.status,
-                        data=Error.parse_obj(f.json()),
+                        url=response.request.url,
+                        status=response.status_code,
+                        data=Error.model_validate(response.json()),
                     )
 
-                my_list = ScryfallList.parse_obj(f.json())
+                my_list = ScryfallList.model_validate(response.json())
+                if my_list is None:
+                    return
+
                 for item in my_list.data:
                     if limit and i >= limit:
                         return
                     i += 1
 
                     if model:
-                        yield model.parse_obj(item)
+                        yield model.model_validate(item)
                     else:
                         yield item
 
                 if not my_list.has_more:
                     return
 
-                path = my_list.next_page.path + "?" + my_list.next_page.query
+                next_page = cast(AnyUrl, my_list.next_page)
+                path = f"{next_page.path}?{next_page.query}"
                 await self._sleep()
         except ValidationError as e:
             raise ServiceError(
                 message=f"Failed to validate {model} data for item #{i}, {e.errors()}",
                 url=path,
                 status=None,
                 data=e,
             )
         except HTTPStatusError as e:
             raise ServiceError(
                 message="Failed to fetch data from Scryfall",
                 url=e.request.url,
                 status=e.response.status_code,
-                data=Error.parse_obj(e),
+                data=Error.model_validate(e),
             )
```

### Comparing `mightstone-0.4.0/src/mightstone/services/scryfall/models.py` & `mightstone-0.8.1/src/mightstone/services/scryfall/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,105 @@
 import datetime
-from decimal import Decimal
 from enum import Enum
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 from uuid import UUID, uuid4
 
-from pydantic import AnyUrl, Field
-from typing_extensions import TypedDict
+from beanie import DecimalAnnotation, Indexed
+from pydantic import (
+    AnyUrl,
+    Field,
+    GetCoreSchemaHandler,
+    GetJsonSchemaHandler,
+    model_validator,
+)
+from pydantic.json_schema import JsonSchemaValue
+from pydantic_core import CoreSchema
+from pydantic_core import core_schema
+from pydantic_core import core_schema as cs
+from typing_extensions import Literal, TypedDict
 
-from mightstone.core import MightstoneModel
+from mightstone.common import generate_uuid_from_string
+from mightstone.core import MightstoneDocument, MightstoneModel
 
 
 class Color(str):
     WHITE = "W"
     BLUE = "U"
     BLACK = "B"
     RED = "R"
     GREEN = "G"
     COLORLESS = "C"
 
     @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
+    def __get_pydantic_core_schema__(
+        cls, source_type: Any, handler: GetCoreSchemaHandler
+    ) -> CoreSchema:
+        return core_schema.no_info_after_validator_function(cls, handler(str))
 
     @classmethod
-    def __modify_schema__(cls, field_schema):
-        # __modify_schema__ should mutate the dict it receives in place,
-        # the returned value will be ignored
-        field_schema.update(
-            # simplified regex here for brevity, see the wikipedia link above
-            pattern="^[WUBRG]$",
-            # some example postcodes
-            examples=["U", "W"],
-        )
+    def __get_pydantic_json_schema__(
+        cls, core_schema: cs.CoreSchema, handler: GetJsonSchemaHandler
+    ) -> JsonSchemaValue:
+        json_schema = handler(core_schema)
+        json_schema = handler.resolve_ref_schema(json_schema)
+        json_schema["pattern"] = ("^[WUBRG]$",)
+        json_schema["title"] = "Color"
+        json_schema["examples"] = ["U", "W"]
+        return json_schema
 
     @classmethod
     def validate(cls, v):
         if not isinstance(v, str):
             raise TypeError("string required")
         if v not in [cls.WHITE, cls.BLUE, cls.BLACK, cls.RED, cls.GREEN, cls.COLORLESS]:
             raise TypeError("string is not a legal color code")
 
         return v
 
     def __repr__(self):
         return f"Color({super().__repr__()})"
 
 
-class ScryfallList(MightstoneModel):
+class ScryfallModel(MightstoneModel):
+    pass
+
+
+class ScryfallDocument(ScryfallModel, MightstoneDocument):  # type: ignore
+    pass
+
+
+class ScryfallList(ScryfallModel):
+    object: Literal["list"]
     data: List
     """An array of the requested objects, in a specific order."""
     has_more: bool = False
     """if this List is paginated and there is a page beyond the current page."""
-    next_page: AnyUrl = None
+    next_page: Optional[AnyUrl] = None
     """If there is a page beyond the current page, this field will contain a full API
     URI to that page. You may submit a HTTP GET request to that URI to continue
     paginating forward on this List."""
-    total_cards: int = None
+    total_cards: Optional[int] = None
     """If this is a list of Card objects, this field will contain the total number
     of cards found across all pages."""
     warnings: List[str] = []
     """An array of human-readable warnings issued when generating this list, as
     strings. Warnings are non-fatal issues that the API discovered with your input.
     In general, they indicate that the List will not contain the all of the information
     you requested. You should fix the warnings and re-submit your request."""
 
 
-class Error(MightstoneModel):
+class Error(ScryfallModel):
+    object: Literal["error"]
     status: int
     """An integer HTTP status code for this error."""
     code: str
     """A computer-friendly string representing the appropriate HTTP status code."""
     details: str
     """A human-readable string explaining the error."""
-    type: str = None
+    type: Optional[str] = None
     """A computer-friendly string that provides additional context for the main error.
     For example, an endpoint many generate HTTP 404 errors for different kinds of
     input. This field will provide a label for the specific kind of 404 failure,
     such as ambiguous."""
     warnings: List[str] = []
     """If your input also generated non-failure warnings, they will be provided as
      human-readable strings in this array."""
@@ -94,37 +117,37 @@
     type_line: str
     """The type line of this card."""
     uri: AnyUrl
     """A URI where you can retrieve a full object describing this card on Scryfall’s
     API. """
 
 
-class CardImagery(TypedDict, total=False):
-    png: Optional[AnyUrl]
+class CardImagery(MightstoneModel):
+    png: Optional[AnyUrl] = None
     """A transparent, rounded full card PNG. This is the best image to use for videos
     or other high-quality content. """
-    border_crop: Optional[AnyUrl]
+    border_crop: Optional[AnyUrl] = None
     """A full card image with the rounded corners and the majority of the border
     cropped off. Designed for dated contexts where rounded images can’t be used. """
-    art_crop: Optional[AnyUrl]
+    art_crop: Optional[AnyUrl] = None
     """A rectangular crop of the card’s art only. Not guaranteed to be perfect for cards
     with outlier designs or strange frame arrangements"""
-    large: Optional[AnyUrl]
+    large: Optional[AnyUrl] = None
     """A large full card image"""
-    normal: Optional[AnyUrl]
+    normal: Optional[AnyUrl] = None
     """A medium-sized full card image"""
-    small: Optional[AnyUrl]
+    small: Optional[AnyUrl] = None
     """A small full card image. Designed for use as thumbnail or list icon."""
 
 
 class CardFace(TypedDict, total=False):
     artist: Optional[str]
     """The name of the illustrator of this card face. Newly spoiled cards may not
     have this field yet. """
-    cmc: Optional[Decimal]
+    cmc: Optional[DecimalAnnotation]
     """The mana value of this particular face, if the card is reversible."""
     color_indicator: Optional[List[Color]]
     """The colors in this face’s color indicator, if any."""
     colors: Optional[List[Color]]
     """This face’s colors, if the game defines colors for the individual face of this
     card. """
     flavor_text: Optional[str]
@@ -164,66 +187,63 @@
     """This face’s toughness, if any."""
     type_line: Optional[str]
     """The type line of this particular face, if the card is reversible."""
     watermark: Optional[str]
     """The watermark on this particulary card face, if any."""
 
 
-class Preview(TypedDict, total=False):
-    previewed_at: Optional[datetime.date]
+class Preview(MightstoneModel):
+    previewed_at: Optional[datetime.date] = None
     """The date this card was previewed"""
-    source_uri: Optional[str]
+    source_uri: Optional[str] = None
     """A link to the preview for this card."""
-    source: Optional[str]
+    source: Optional[str] = None
     """The name of the source that previewed this card."""
 
 
 class BulkTagType(str, Enum):
     ORACLE = "oracle"
     ILLUSTRATION = "illustration"
 
 
-class Tag(MightstoneModel):
+class Tag(MightstoneDocument):
     object: str
-    id: UUID = Field(default_factory=uuid4)
+    id: UUID = Field(default_factory=uuid4)  # type: ignore
     label: str
     type: str
     description: Optional[str]
     oracle_ids: List[UUID]
 
-    class Settings:
-        name = "tags"
-
 
-class Card(MightstoneModel):
+class Card(MightstoneDocument):
     arena_id: Optional[int] = None
     """This card’s Arena ID, if any. A large percentage of cards are not available on
     Arena and do not have this ID. """
 
-    id: UUID = Field(default_factory=uuid4)
+    id: UUID = Field(default_factory=uuid4)  # type: ignore
     """A unique ID for this card in Scryfall’s database."""
     lang: str
     """A language code for this printing."""
-    mtgo_id: Optional[int]
+    mtgo_id: Optional[int] = None
     """This card’s Magic Online ID (also known as the Catalog ID), if any. A large
     percentage of cards are not available on Magic Online and do not have this ID."""
-    mtgo_foil_id: Optional[int]
+    mtgo_foil_id: Optional[int] = None
     """This card’s foil Magic Online ID (also known as the Catalog ID), if any. A
     large percentage of cards are not available on Magic Online and do not have this
     ID."""
-    multiverse_ids: Optional[List[int]]
+    multiverse_ids: Optional[List[int]] = None
     """This card’s multiverse IDs on Gatherer, if any, as an array of integers.
     Note that Scryfall includes many promo cards, tokens, and other esoteric objects
     that do not have these identifiers."""
-    tcgplayer_id: Optional[int]
+    tcgplayer_id: Optional[int] = None
     """This card’s ID on TCGplayer’s API, also known as the productId."""
-    tcgplayer_etched_id: Optional[int]
+    tcgplayer_etched_id: Optional[int] = None
     """This card’s ID on TCGplayer’s API, for its etched version if that version is a
      separate product."""
-    cardmarket_id: Optional[int]
+    cardmarket_id: Optional[int] = None
     """This card’s ID on Cardmarket’s API, also known as the idProduct."""
     object: str
     """A content type for this object, always card."""
     oracle_id: UUID
     """A unique ID for this card’s oracle identity.
     This value is consistent across reprinted card editions, and unique among
     different cards with the same name (tokens, Unstable variants, etc)."""
@@ -233,136 +253,136 @@
     rulings_uri: AnyUrl
     """A link to this card’s rulings list on Scryfall’s API."""
     scryfall_uri: AnyUrl
     """A link to this card’s permapage on Scryfall’s website."""
     uri: AnyUrl
     """A link to this card object on Scryfall’s API."""
 
-    all_parts: Optional[List[dict]]
+    all_parts: Optional[List[dict]] = None
     """If this card is closely related to other cards, this property will be an array
     with Related Card Objects. """
-    card_faces: Optional[List[dict]]
+    card_faces: Optional[List[dict]] = None
     """An array of Card Face objects, if this card is multifaced."""
-    cmc: Decimal
+    cmc: DecimalAnnotation
     """The card’s converted mana cost. Note that some funny cards have fractional
     mana costs. """
     color_identity: List[Color]
     """This card’s color identity."""
-    color_indicator: Optional[List[Color]]
+    color_indicator: Optional[List[Color]] = None
     """The colors in this card’s color indicator, if any.
     A null value for this field indicates the card does not have one."""
-    colors: Optional[List[Color]]
+    colors: Optional[List[Color]] = None
     """This card’s colors, if the overall card has colors defined by the rules.
     Otherwise the colors will be on the card_faces objects, see below."""
-    edhrec_rank: Optional[int]
+    edhrec_rank: Optional[int] = None
     """This card’s overall rank/popularity on EDHREC. Not all cards are ranked."""
-    hand_modifier: Optional[str]
+    hand_modifier: Optional[str] = None
     """This card’s hand modifier, if it is Vanguard card. This value will contain a
     delta, such as -1. """
     keywords: List[str]
     """An array of keywords that this card uses, such as 'Flying' and 'Cumulative
     upkeep'. """
     layout: str
     """A code for this card’s layout."""
     legalities: dict
     """An object describing the legality of this card across play formats.
     Possible legalities are legal, not_legal, restricted, and banned."""
-    life_modifier: Optional[str]
+    life_modifier: Optional[str] = None
     """This card’s life modifier, if it is Vanguard card. This value will contain a
     delta, such as +2. """
-    loyalty: Optional[str]
+    loyalty: Optional[str] = None
     """This loyalty if any. Note that some cards have loyalties that are not numeric,
     such as X. """
-    mana_cost: Optional[str]
+    mana_cost: Optional[str] = None
     """The mana cost for this card. This value will be any empty string "" if the
     cost is absent. Remember that per the game rules, a missing mana cost and a mana
     cost of {0} are different values. Multi-faced cards will report this value in
     card faces. """
     name: str
     """The name of this card. If this card has multiple faces, this field will
     contain both names separated by ␣//␣. """
-    oracle_text: Optional[str]
+    oracle_text: Optional[str] = None
     """The Oracle text for this card, if any."""
     oversized: bool
     """True if this card is oversized."""
-    penny_rank: Optional[int]
+    penny_rank: Optional[int] = None
     """This card’s rank/popularity on Penny Dreadful. Not all cards are ranked."""
-    power: Optional[str]
+    power: Optional[str] = None
     """This card’s power, if any. Note that some cards have powers that are not
     numeric, such as *. """
-    produced_mana: Optional[List[str]]
+    produced_mana: Optional[List[str]] = None
     """Colors of mana that this card could produce."""
     reserved: bool
     """True if this card is on the Reserved List."""
-    toughness: Optional[str]
+    toughness: Optional[str] = None
     """This card’s toughness, if any. Note that some cards have toughnesses that are
     not numeric, such as *. """
     type_line: str
     """The type line of this card."""
 
-    artist: Optional[str]
+    artist: Optional[str] = None
     """The name of the illustrator of this card. Newly spoiled cards may not have
     this field yet. """
-    attraction_lights: Optional[List[str]]
+    attraction_lights: Optional[List[str]] = None
     """The lit Unfinity attractions lights on this card, if any."""
     booster: bool
     """Whether this card is found in boosters."""
     border_color: str
     """This card’s border color: black, white, borderless, silver, or gold."""
-    card_back_id: Optional[UUID]
+    card_back_id: Optional[UUID] = None
     """The Scryfall ID for the card back design present on this card."""
     collector_number: str
     """This card’s collector number. Note that collector numbers can contain
     non-numeric characters, such as letters or ★. """
-    content_warning: Optional[bool]
+    content_warning: Optional[bool] = None
     """True if you should consider avoiding use of this print downstream."""
     digital: bool
     """	True if this card was only released in a video game."""
     finishes: List[str]
     """An array of computer-readable flags that indicate if this card can come in
     foil, nonfoil, or etched finishes. """
-    flavor_name: Optional[str]
+    flavor_name: Optional[str] = None
     """The just-for-fun name printed on the card (such as for Godzilla series cards)."""
-    flavor_text: Optional[str]
+    flavor_text: Optional[str] = None
     """The flavor text, if any."""
-    frame_effects: Optional[List[str]]
+    frame_effects: Optional[List[str]] = None
     """This card’s frame effects, if any."""
     frame: str
     """This card’s frame layout."""
     full_art: bool
     """True if this card’s artwork is larger than normal."""
     games: List[str]
     """A list of games that this card print is available in, paper, arena,
     and/or mtgo. """
     highres_image: bool
     """True if this card’s imagery is high resolution."""
-    illustration_id: Optional[UUID]
+    illustration_id: Optional[UUID] = None
     """A unique identifier for the card artwork that remains consistent across reprints.
     Newly spoiled cards may not have this field yet."""
     image_status: str
     """A computer-readable indicator for the state of this card’s image, one of :
     missing, placeholder, lowres, or highres_scan."""
-    image_uris: Optional[CardImagery]
+    image_uris: Optional[CardImagery] = None
     """An object listing available imagery for this card. See the Card Imagery
     article for more information. """
-    prices: Dict[str, Optional[str]]
+    prices: Dict[str, Optional[str]] = {}
     """An object containing daily price information for this card, including:
      usd, usd_foil, usd_etched, eur, and tix prices, as strings."""
-    printed_name: Optional[str]
+    printed_name: Optional[str] = None
     """The localized name printed on this card, if any."""
-    printed_text: Optional[str]
+    printed_text: Optional[str] = None
     """The localized text printed on this card, if any."""
-    printed_type_line: Optional[str]
+    printed_type_line: Optional[str] = None
     """The localized type line printed on this card, if any."""
     promo: bool
     """True if this card is a promotional print."""
-    promo_types: Optional[List[str]]
+    promo_types: Optional[List[str]] = None
     """An array of strings describing what categories of promo cards this card falls
     into. """
-    purchase_uris: Optional[Dict[str, str]]
+    purchase_uris: Optional[Dict[str, str]] = None
     """An object providing URIs to this card’s listing on major marketplaces."""
     rarity: str
     """This card’s rarity. One of common, uncommon, rare, special, mythic, or bonus."""
     related_uris: Dict[str, AnyUrl]
     """An object providing URIs to this card’s listing on other Magic: The Gathering
     online resources. """
     released_at: datetime.date
@@ -385,30 +405,22 @@
     """This card’s Set object UUID."""
     story_spotlight: bool
     """True if this card is a Story Spotlight."""
     textless: bool
     """True if the card is printed without text."""
     variation: bool
     """Whether this card is a variation of another printing."""
-    variation_of: Optional[UUID]
+    variation_of: Optional[UUID] = None
     """The printing ID of the printing this card is a variation of."""
-    security_stamp: Optional[str]
+    security_stamp: Optional[str] = None
     """The security stamp on this card, if any. One of oval, triangle, acorn, circle,
     arena, or heart. """
-    watermark: Optional[str]
+    watermark: Optional[str] = None
     """This card’s watermark, if any."""
-    preview: Optional[Preview]
-
-    class Settings:
-        name = "cards"
-        bson_encoders = {
-            datetime.date: lambda dt: datetime.datetime(
-                year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, second=0
-            )
-        }
+    preview: Optional[Preview] = None
 
 
 class SetType(str, Enum):
     CORE = "core"
     """A yearly Magic core set (Tenth Edition, etc)"""
     EXPANSION = "expansion"
     """A rotational expansion set in a block (Zendikar, etc)"""
@@ -450,51 +462,52 @@
     """A set that contains purely promotional cards"""
     TOKEN = "token"  # nosec, damnit bandit, that’s not a security issue
     """A set made up of tokens and emblems."""
     MEMO = "memorabilia"
     """A set made up of gold-bordered, oversize, or trophy cards that are not legal"""
 
 
-class Set(MightstoneModel):
+class Set(ScryfallDocument):
     """
     A Set object represents a group of related Magic cards. All Card objects on Scryfall
      belong to exactly one set.
 
     Due to Magic’s long and complicated history, Scryfall includes many un-official sets
      as a way to group promotional or outlier cards together. Such sets will likely have
       a code that begins with p or t, such as pcel or tori.
 
     Official sets always have a three-letter set code, such as zen.
     """
 
-    id: UUID
+    object: Literal["set"]
+    id: UUID = Field(default_factory=uuid4)  # type: ignore
     """A unique ID for this set on Scryfall that will not change."""
-    code: str
+    code: Indexed(str, unique=True)  # type: ignore
     "The unique three to five-letter code for this set."
-    mtgo_code: str = None
+    mtgo_code: Optional[str] = None
     """The unique code for this set on MTGO, which may differ from the regular code."""
-    tcgplayer_id: int = None
+    tcgplayer_id: Optional[int] = None
     """This set’s ID on TCGplayer’s API, also known as the groupId."""
     name: str
     """The English name of the set."""
     set_type: SetType
     """A computer-readable classification for this set. See below."""
-    released_at: datetime.date = None
+    released_at: Optional[datetime.date] = None
     """The date the set was released or the first card was printed in the set (in
     GMT-8 Pacific time). """
-    block_code: str = None
+    block_code: Optional[str] = None
     """The block code for this set, if any."""
-    block: str = None
+    block: Optional[str] = None
     """The block or group name code for this set, if any."""
-    parent_set_code: str = None
+    parent_set_code: Optional[str] = None
     """The set code for the parent set, if any. promo and token sets often have a
     parent set. """
     card_count: int
     """The number of cards in this set."""
-    printed_size: int = None
+    printed_size: Optional[int] = None
     """The denominator for the set’s printed collector numbers."""
     digital: bool
     """True if this set was only released in a video game."""
     foil_only: bool
     """True if this set contains only foil cards."""
     nonfoil_only: bool
     """True if this set contains only nonfoil cards."""
@@ -508,89 +521,106 @@
     You should download it and use it locally for your particular user interface
     needs."""
     search_uri: AnyUrl
     """A Scryfall API URI that you can request to begin paginating over the cards
     in this set."""
 
 
-class Symbol(MightstoneModel):
+class Symbol(ScryfallDocument):
     """
     A Card Symbol object represents an illustrated symbol that may appear in card’s
     mana cost or Oracle text. Symbols are based on the notation used in the
     Comprehensive Rules.
     For more information about how the Scryfall API represents mana and costs, see the
     colors and costs overview.
     """
 
+    object: Literal["card_symbol"]
+    id: Optional[UUID] = None  # type: ignore
     symbol: str
     """The plaintext symbol. Often surrounded with curly braces {}. Note that not all
      symbols are ASCII text (for example, {∞})."""
-    loose_variant: str = None
+    loose_variant: Optional[str] = None
     """An alternate version of this symbol, if it is possible to write it without
     curly braces."""
     english: str
     """An English snippet that describes this symbol. Appropriate for use in alt text
     or other accessible communication formats."""
     transposable: bool
     """True if it is possible to write this symbol “backwards”.
     For example, the official symbol {U/P} is sometimes written as {P/U} or {P\\U} in
     informal settings.
     Note that the Scryfall API never writes symbols backwards in other responses. This
     field is provided for informational purposes."""
     represents_mana: bool
-    """True if this is a mana symbol."""
-    cmc: Decimal = None
+    """if this is a mana symbol."""
+    cmc: Optional[DecimalAnnotation] = None
     """A decimal number representing this symbol’s converted mana cost. Note that mana
     symbols from funny sets can have fractional converted mana costs."""
     appears_in_mana_costs: bool
     """True if this symbol appears in a mana cost on any Magic card. For example {20}
     has this field set to false because {20} only appears in Oracle text, not mana
     costs."""
     funny: bool
     """True if this symbol is only used on funny cards or Un-cards."""
     colors: List[Color] = []
     """An array of colors that this symbol represents."""
-    gatherer_alternates: List[str] = None
+    gatherer_alternates: Optional[List[str]] = None
     """An array of plaintext versions of this symbol that Gatherer uses on old cards
     to describe original printed text. For example: {W} has ["oW", "ooW"] as
     alternates."""
-    svg_uri: AnyUrl = None
+    svg_uri: Optional[AnyUrl] = None
     """A URI to an SVG image of this symbol on Scryfall’s CDNs."""
 
+    @model_validator(mode="wrap")
+    @classmethod
+    def enforce_id(cls, value: Any, handler) -> "ScryfallDocument":
+        doc = handler(value)
+
+        if not isinstance(value, Dict):
+            return doc
+
+        if "id" not in value:
+            if "symbol" in value:
+                doc.id = generate_uuid_from_string(value["symbol"])
+
+        return doc
 
-class ManaCost(MightstoneModel):
+
+class ManaCost(ScryfallModel):
     cost: str
     """The normalized cost, with correctly-ordered and wrapped mana symbols."""
-    cmc: Decimal
+    cmc: DecimalAnnotation
     """The converted mana cost. If you submit Un-set mana symbols, this decimal
      could include fractional parts."""
     colors: List[Color]
     """The colors of the given cost."""
     colorless: bool
     """True if the cost is colorless."""
     monocolored: bool
     """True if the cost is monocolored."""
     multicolored: bool
     """True if the cost is multicolored."""
 
 
-class Migration(MightstoneModel):
+class Migration(ScryfallDocument):
+    object: Literal["migration"]
     uri: AnyUrl
     """A link to the current object on Scryfall’s API."""
-    id: UUID
+    id: UUID = Field(default_factory=uuid4)  # type: ignore
     """This migration’s unique UUID."""
-    created_at: datetime.date = None
+    created_at: Optional[datetime.date] = None
     """The date this migration was performed."""
     migration_strategy: str
     """A computer-readable indicator of the migration strategy."""
     old_scryfall_id: UUID
     """The id of the affected API Card object."""
-    new_scryfall_id: UUID = None
+    new_scryfall_id: Optional[UUID] = None
     """The replacement id of the API Card object if this is a merge."""
-    note: str = None
+    note: Optional[str] = None
     """A note left by the Scryfall team about this migration."""
 
 
 class UniqueStrategy(str, Enum):
     CARDS = "cards"
     """
     Removes duplicate gameplay objects (cards that share a name and have the same
@@ -725,22 +755,39 @@
     """Returns a Catalog of all keyword actions in Scryfall’s database. Values are
     updated as soon as a new card is entered for spoiler seasons. """
     ABILITY_WORDS = "ability-words"
     """Returns a Catalog of all ability words in Scryfall’s database. Values are
     updated as soon as a new card is entered for spoiler seasons. """
 
 
-class Catalog(MightstoneModel):
-    uri: AnyUrl = None
+class Catalog(ScryfallDocument):
+    object: Literal["catalog"]
+    id: Optional[UUID] = None  # type: ignore
+    """Object type, always catalog"""
+    uri: Optional[AnyUrl] = None
     """A link to the current catalog on Scryfall’s API."""
     total_values: int
     """The number of items in the data array."""
     data: List[str]
     """An array of datapoints, as strings."""
 
+    @model_validator(mode="wrap")
+    @classmethod
+    def enforce_id(cls, value: Any, handler) -> "ScryfallDocument":
+        doc = handler(value)
+
+        if not isinstance(value, Dict):
+            return doc
+
+        if "id" not in value:
+            if "uri" in value:
+                doc.id = generate_uuid_from_string(value["uri"])
+
+        return doc
+
 
 class IdentifierId(TypedDict):
     """Finds a card with the specified Scryfall id."""
 
     id: UUID
 
 
@@ -782,28 +829,29 @@
 class IdentifierCollectorNumberSet(TypedDict):
     """Finds a card matching the specified name and set."""
 
     collector_number: int
     set: str
 
 
-class Ruling(MightstoneModel):
+class Ruling(ScryfallDocument):
     """
     Rulings represent Oracle rulings, Wizards of the Coast set release notes,
     or Scryfall notes for a particular card.
 
     If two cards have the same name, they will have the same set of rulings objects.
     If a card has rulings, it usually has more than one.
 
     Rulings with a scryfall source have been added by the Scryfall team, either to
     provide additional context for the card, or explain how the card works in an
     unofficial format (such as Duel Commander).
     """
 
-    oracle_id: UUID
+    object: Literal["ruling"]
+    oracle_id: UUID  # type: ignore
     """
     Oracle unique identifier
     """
     source: str
     """A computer-readable string indicating which company produced this ruling,
     either wotc or scryfall. """
     published_at: datetime.date
```

