# Comparing `tmp/pyproject_pre_commit-0.1.8.tar.gz` & `tmp/pyproject_pre_commit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_pre_commit-0.1.8.tar", max compression
+gzip compressed data, was "pyproject_pre_commit-0.1.9.tar", max compression
```

## Comparing `pyproject_pre_commit-0.1.8.tar` & `pyproject_pre_commit-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11337 2023-02-06 14:22:52.605551 pyproject_pre_commit-0.1.8/LICENSE
--rw-r--r--   0        0        0     5374 2024-03-30 01:51:51.028365 pyproject_pre_commit-0.1.8/README.md
--rw-r--r--   0        0        0     3557 2024-03-30 01:55:45.258362 pyproject_pre_commit-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      111 2024-03-30 01:51:51.028365 pyproject_pre_commit-0.1.8/src/pyproject_pre_commit/__init__.py
--rw-r--r--   0        0        0       93 2024-03-30 01:51:51.028365 pyproject_pre_commit-0.1.8/src/pyproject_pre_commit/__version__.py
--rw-r--r--   0        0        0     1783 2024-03-30 01:51:51.028365 pyproject_pre_commit-0.1.8/src/pyproject_pre_commit/pyproject_pre_commit.py
--rw-r--r--   0        0        0     7765 1970-01-01 00:00:00.000000 pyproject_pre_commit-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-05-01 01:21:39.716387 pyproject_pre_commit-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5374 2024-05-01 01:21:39.716387 pyproject_pre_commit-0.1.9/README.md
+-rw-r--r--   0        0        0     3557 2024-05-01 01:21:40.568381 pyproject_pre_commit-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-05-01 01:21:39.716387 pyproject_pre_commit-0.1.9/src/pyproject_pre_commit/__init__.py
+-rw-r--r--   0        0        0       93 2024-05-01 01:21:39.716387 pyproject_pre_commit-0.1.9/src/pyproject_pre_commit/__version__.py
+-rw-r--r--   0        0        0     1783 2024-05-01 01:21:39.716387 pyproject_pre_commit-0.1.9/src/pyproject_pre_commit/pyproject_pre_commit.py
+-rw-r--r--   0        0        0     7765 1970-01-01 00:00:00.000000 pyproject_pre_commit-0.1.9/PKG-INFO
```

### Comparing `pyproject_pre_commit-0.1.8/LICENSE` & `pyproject_pre_commit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.1.8/README.md` & `pyproject_pre_commit-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.1.8/pyproject.toml` & `pyproject_pre_commit-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyproject-pre-commit"
-version = "0.1.8"
+version = "0.1.9"
 description = "pre-commit hooks for python projects using pyproject.toml."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/pyproject-pre-commit"
 homepage = "https://github.com/rcmdnk/pyproject-pre-commit"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["pre-commit", "pyproject.toml", "poetry"]
@@ -47,15 +47,15 @@
 mdformat = "^0.7.17"
 mdformat-gfm = "^0.3.5"
 mdformat-frontmatter = "^2.0.1"
 mdformat-footnote = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
-pytest-cov = "^4.1.0"
+pytest-cov = "^5.0.0"
 pytest-xdist = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `pyproject_pre_commit-0.1.8/src/pyproject_pre_commit/pyproject_pre_commit.py` & `pyproject_pre_commit-0.1.9/src/pyproject_pre_commit/pyproject_pre_commit.py`

 * *Files identical despite different names*

### Comparing `pyproject_pre_commit-0.1.8/PKG-INFO` & `pyproject_pre_commit-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-pre-commit
-Version: 0.1.8
+Version: 0.1.9
 Summary: pre-commit hooks for python projects using pyproject.toml.
 Home-page: https://github.com/rcmdnk/pyproject-pre-commit
 License: Apache-2.0
 Keywords: pre-commit,pyproject.toml,poetry
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

