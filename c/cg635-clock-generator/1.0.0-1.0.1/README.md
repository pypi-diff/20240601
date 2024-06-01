# Comparing `tmp/cg635_clock_generator-1.0.0.tar.gz` & `tmp/cg635_clock_generator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg635_clock_generator-1.0.0.tar", last modified: Sat Jun  1 21:14:00 2024, max compression
+gzip compressed data, was "cg635_clock_generator-1.0.1.tar", last modified: Sat Jun  1 21:14:00 2024, max compression
```

## Comparing `cg635_clock_generator-1.0.0.tar` & `cg635_clock_generator-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.729048 cg635_clock_generator-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      573 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2867 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1670 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     8080 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2661 2024-06-01 21:14:00.729048 cg635_clock_generator-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.718048 cg635_clock_generator-1.0.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.718048 cg635_clock_generator-1.0.0/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/_static/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)   362028 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/_static/cg635.png
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/authors.md
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/changelog.md
--rw-rw-rw-   0 root         (0) root         (0)    10125 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/contributing.md
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/index.md
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/license.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/readme.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-06-01 21:14:00.729048 cg635_clock_generator-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.712048 cg635_clock_generator-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.722048 cg635_clock_generator-1.0.0/src/cg635_clock_generator/
--rw-rw-rw-   0 root         (0) root         (0)     1099 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14351 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator/cg635_clock_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.724048 cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2661 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       66 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.724048 cg635_clock_generator-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7590 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/tests/cg635_clock_generator_mocker.py
--rw-rw-rw-   0 root         (0) root         (0)     1685 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     7361 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/tests/test_cg635_clock_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2024-06-01 21:13:32.000000 cg635_clock_generator-1.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.524047 cg635_clock_generator-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     8080 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-06-01 21:14:00.524047 cg635_clock_generator-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.519046 cg635_clock_generator-1.0.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.520046 cg635_clock_generator-1.0.1/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/_static/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)   362028 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/_static/cg635.png
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/authors.md
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/changelog.md
+-rw-rw-rw-   0 root         (0) root         (0)    10125 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/contributing.md
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/license.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/readme.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2024-06-01 21:14:00.525046 cg635_clock_generator-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.516046 cg635_clock_generator-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.521046 cg635_clock_generator-1.0.1/src/cg635_clock_generator/
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14351 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator/cg635_clock_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.523046 cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       66 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-06-01 21:14:00.000000 cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:14:00.523046 cg635_clock_generator-1.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7590 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/tests/cg635_clock_generator_mocker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     7361 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/tests/test_cg635_clock_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2024-06-01 21:13:30.000000 cg635_clock_generator-1.0.1/tox.ini
```

### Comparing `cg635_clock_generator-1.0.0/.coveragerc` & `cg635_clock_generator-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/.gitignore` & `cg635_clock_generator-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/.gitlab-ci.yml` & `cg635_clock_generator-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/.pre-commit-config.yaml` & `cg635_clock_generator-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/CONTRIBUTING.md` & `cg635_clock_generator-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/LICENSE.txt` & `cg635_clock_generator-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/PKG-INFO` & `cg635_clock_generator-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: cg635-clock-generator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interface with a Stanford Research Systems CG635 Synthesized Clock Generator
 Home-page: https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator
 Author: Leandro Lanzieri
 Author-email: leandro.lanzieri@desy.de
 License: LGPL-3.0-or-later
 Project-URL: Source, https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator
+Project-URL: Documentation, http://cg635-clock-generator-leandro-lanzieri-c9d5fa14e6af42e02aa27f45.pages.desy.de
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: pyvisa
 Requires-Dist: pyvisa-py
 Requires-Dist: pyserial
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
-# cg635-clock-generator - Stanford Research Systems CG635 Synthesized Clock Generator Interface
+# SRS-CG635 Synthesized Clock Generator Interface
 
 Interface with a Stanford Research Systems CG635 Synthesized Clock Generator.
 
 ## Installation
 
 ```bash
-$ pip install git+https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator.git
+$ pip install cg635-clock-generator
 ```
 
 ## Supported Features
 
 - Frequency control
 - Phase control
 - CMOS output levels and standards control
```

### Comparing `cg635_clock_generator-1.0.0/README.md` & `cg635_clock_generator-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# cg635-clock-generator - Stanford Research Systems CG635 Synthesized Clock Generator Interface
+# SRS-CG635 Synthesized Clock Generator Interface
 
 Interface with a Stanford Research Systems CG635 Synthesized Clock Generator.
 
 ## Installation
 
 ```bash
-$ pip install git+https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator.git
+$ pip install cg635-clock-generator
 ```
 
 ## Supported Features
 
 - Frequency control
 - Phase control
 - CMOS output levels and standards control
```

### Comparing `cg635_clock_generator-1.0.0/docs/Makefile` & `cg635_clock_generator-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/docs/_static/cg635.png` & `cg635_clock_generator-1.0.1/docs/_static/cg635.png`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/docs/conf.py` & `cg635_clock_generator-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/docs/index.md` & `cg635_clock_generator-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/setup.cfg` & `cg635_clock_generator-1.0.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 license = LGPL-3.0-or-later
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator
 project_urls = 
 	Source = https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator
+	Documentation = http://cg635-clock-generator-leandro-lanzieri-c9d5fa14e6af42e02aa27f45.pages.desy.de
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
```

### Comparing `cg635_clock_generator-1.0.0/setup.py` & `cg635_clock_generator-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/src/cg635_clock_generator/__init__.py` & `cg635_clock_generator-1.0.1/src/cg635_clock_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/src/cg635_clock_generator/cg635_clock_generator.py` & `cg635_clock_generator-1.0.1/src/cg635_clock_generator/cg635_clock_generator.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/src/cg635_clock_generator/constants.py` & `cg635_clock_generator-1.0.1/src/cg635_clock_generator/constants.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/src/cg635_clock_generator/exceptions.py` & `cg635_clock_generator-1.0.1/src/cg635_clock_generator/exceptions.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/PKG-INFO` & `cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: cg635-clock-generator
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interface with a Stanford Research Systems CG635 Synthesized Clock Generator
 Home-page: https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator
 Author: Leandro Lanzieri
 Author-email: leandro.lanzieri@desy.de
 License: LGPL-3.0-or-later
 Project-URL: Source, https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator
+Project-URL: Documentation, http://cg635-clock-generator-leandro-lanzieri-c9d5fa14e6af42e02aa27f45.pages.desy.de
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: pyvisa
 Requires-Dist: pyvisa-py
 Requires-Dist: pyserial
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
-# cg635-clock-generator - Stanford Research Systems CG635 Synthesized Clock Generator Interface
+# SRS-CG635 Synthesized Clock Generator Interface
 
 Interface with a Stanford Research Systems CG635 Synthesized Clock Generator.
 
 ## Installation
 
 ```bash
-$ pip install git+https://gitlab.desy.de/leandro.lanzieri/cg635-clock-generator.git
+$ pip install cg635-clock-generator
 ```
 
 ## Supported Features
 
 - Frequency control
 - Phase control
 - CMOS output levels and standards control
```

### Comparing `cg635_clock_generator-1.0.0/src/cg635_clock_generator.egg-info/SOURCES.txt` & `cg635_clock_generator-1.0.1/src/cg635_clock_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/tests/cg635_clock_generator_mocker.py` & `cg635_clock_generator-1.0.1/tests/cg635_clock_generator_mocker.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/tests/conftest.py` & `cg635_clock_generator-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/tests/test_cg635_clock_generator.py` & `cg635_clock_generator-1.0.1/tests/test_cg635_clock_generator.py`

 * *Files identical despite different names*

### Comparing `cg635_clock_generator-1.0.0/tox.ini` & `cg635_clock_generator-1.0.1/tox.ini`

 * *Files identical despite different names*

