# Comparing `tmp/pytest_topo-0.0.1.tar.gz` & `tmp/pytest_topo-0.0.4.tar.gz`

## Comparing `pytest_topo-0.0.1.tar` & `pytest_topo-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,16 @@
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pytest_topo-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_topo-0.0.1/src/pytest_topo/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pytest_topo-0.0.1/LICENSE
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pytest_topo-0.0.1/README.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pytest_topo-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pytest_topo-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/DEVNOTES.md
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/src/pytest_topo/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/src/pytest_topo/plugin.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/src/pytest_topo/topo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/test_extendable.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/test_ordering.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/test_skipping.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/README.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/PKG-INFO
```

### Comparing `pytest_topo-0.0.1/LICENSE` & `pytest_topo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_topo-0.0.1/pyproject.toml` & `pytest_topo-0.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,56 @@
 [project]
-name = "pytest_topo"
-version = "0.0.1"
+name = "pytest-topo"
+version = "0.0.4"
 authors = [
   { name="Nick Sullivan", email="nick.dave.sullivan@gmail.com" },
 ]
 description = "Topological sorting for pytest"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "pytest>=8.2.1",
+]
 
-[project.urls]
-Homepage = "https://github.com/pypa/sampleproject"
-Issues = "https://github.com/pypa/sampleproject/issues"
+[project.optional-dependencies]
+test = [
+    "ruff==0.4.6",
+]
 
+[project.urls]
+Homepage = "https://github.com/Nick-Sullivan/pytest-topo"
+Issues = "https://github.com/Nick-Sullivan/pytest-topo/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
+
+[tool.pytest.ini_options]
+pythonpath = "src"
+markers = [
+    "dependency",
+    "depends_on",
+]
+
+[project.entry-points.pytest11]
+pytest_topo = "pytest_topo.plugin"
+
+[tool.ruff.lint]
+select = [
+    # pycodestyle
+    "E",
+    # Pyflakes
+    "F",
+    # pyupgrade
+    "UP",
+    # flake8-bugbear
+    "B",
+    # flake8-simplify
+    "SIM",
+    # isort
+    "I",
+]
```

