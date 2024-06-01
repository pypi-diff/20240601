# Comparing `tmp/graphmix-0.0.0.tar.gz` & `tmp/graphmix-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphmix-0.0.0.tar", last modified: Tue May 28 17:41:45 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `graphmix-0.0.0.tar` & `graphmix-0.0.1.tar`

### file list

```diff
@@ -1,96 +1,75 @@
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.264927 graphmix-0.0.0/
--rw-r--r--   0 jtaylor    (501) staff       (20)      733 2024-05-23 19:16:04.000000 graphmix-0.0.0/.bumpversion.cfg
--rw-r--r--   0 jtaylor    (501) staff       (20)     2035 2024-05-23 19:16:04.000000 graphmix-0.0.0/.cookiecutterrc
--rw-r--r--   0 jtaylor    (501) staff       (20)      176 2024-05-23 19:16:04.000000 graphmix-0.0.0/.coveragerc
--rw-r--r--   0 jtaylor    (501) staff       (20)      353 2024-05-23 19:16:04.000000 graphmix-0.0.0/.editorconfig
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.253379 graphmix-0.0.0/.github/
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.257125 graphmix-0.0.0/.github/workflows/
--rw-r--r--   0 jtaylor    (501) staff       (20)     4727 2024-05-28 17:33:31.000000 graphmix-0.0.0/.github/workflows/github-actions.yml
--rw-r--r--   0 jtaylor    (501) staff       (20)      686 2024-05-23 19:17:08.000000 graphmix-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 jtaylor    (501) staff       (20)      282 2024-05-23 19:16:04.000000 graphmix-0.0.0/.readthedocs.yml
--rw-r--r--   0 jtaylor    (501) staff       (20)       41 2024-05-23 20:26:49.000000 graphmix-0.0.0/AUTHORS.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)       86 2024-05-23 19:16:04.000000 graphmix-0.0.0/CHANGELOG.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)     2357 2024-05-23 21:39:44.000000 graphmix-0.0.0/CONTRIBUTING.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)     1109 2024-05-23 19:19:10.000000 graphmix-0.0.0/LICENSE
--rw-r--r--   0 jtaylor    (501) staff       (20)      427 2024-05-23 19:16:04.000000 graphmix-0.0.0/MANIFEST.in
--rw-r--r--   0 jtaylor    (501) staff       (20)     2267 2024-05-28 17:41:45.264694 graphmix-0.0.0/PKG-INFO
--rw-r--r--   0 jtaylor    (501) staff       (20)     2457 2024-05-23 19:16:04.000000 graphmix-0.0.0/README.rst
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.257381 graphmix-0.0.0/ci/
--rwxr-xr-x   0 jtaylor    (501) staff       (20)     2984 2024-05-28 17:35:45.000000 graphmix-0.0.0/ci/bootstrap.py
--rw-r--r--   0 jtaylor    (501) staff       (20)      239 2024-05-28 17:12:39.000000 graphmix-0.0.0/ci/requirements.txt
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.253575 graphmix-0.0.0/ci/templates/
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.253667 graphmix-0.0.0/ci/templates/.github/
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.257507 graphmix-0.0.0/ci/templates/.github/workflows/
--rw-r--r--   0 jtaylor    (501) staff       (20)     2205 2024-05-23 19:16:04.000000 graphmix-0.0.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.258877 graphmix-0.0.0/docs/
--rw-r--r--   0 jtaylor    (501) staff       (20)       28 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/authors.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)       30 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/changelog.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)      967 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/conf.py
--rw-r--r--   0 jtaylor    (501) staff       (20)       33 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/contributing.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)      244 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/index.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)       88 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/installation.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)       27 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/readme.rst
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.259343 graphmix-0.0.0/docs/reference/
--rw-r--r--   0 jtaylor    (501) staff       (20)      162 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/reference/graphmix.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)       60 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/reference/index.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)       17 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/requirements.txt
--rw-r--r--   0 jtaylor    (501) staff       (20)      109 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/spelling_wordlist.txt
--rw-r--r--   0 jtaylor    (501) staff       (20)      110 2024-05-23 19:16:04.000000 graphmix-0.0.0/docs/usage.rst
--rw-r--r--   0 jtaylor    (501) staff       (20)     1352 2024-05-28 17:32:36.000000 graphmix-0.0.0/pyproject.toml
--rw-r--r--   0 jtaylor    (501) staff       (20)      909 2024-05-23 19:16:04.000000 graphmix-0.0.0/pytest.ini
--rw-r--r--   0 jtaylor    (501) staff       (20)       38 2024-05-28 17:41:45.264969 graphmix-0.0.0/setup.cfg
--rwxr-xr-x   0 jtaylor    (501) staff       (20)     2946 2024-05-28 17:35:45.000000 graphmix-0.0.0/setup.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.254032 graphmix-0.0.0/src/
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.259898 graphmix-0.0.0/src/graphmix/
--rw-r--r--   0 jtaylor    (501) staff       (20)       22 2024-05-23 22:36:26.000000 graphmix-0.0.0/src/graphmix/__init__.py
--rw-r--r--   0 jtaylor    (501) staff       (20)      132 2024-05-23 20:24:15.000000 graphmix-0.0.0/src/graphmix/__main__.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.261284 graphmix-0.0.0/src/graphmix/chemistry/
--rw-r--r--   0 jtaylor    (501) staff       (20)        0 2024-05-23 20:25:58.000000 graphmix-0.0.0/src/graphmix/chemistry/__init__.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.261551 graphmix-0.0.0/src/graphmix/chemistry/adapters/
--rw-r--r--   0 jtaylor    (501) staff       (20)        0 2024-05-23 21:57:43.000000 graphmix-0.0.0/src/graphmix/chemistry/adapters/__init__.py
--rw-r--r--   0 jtaylor    (501) staff       (20)      312 2024-05-24 16:41:54.000000 graphmix-0.0.0/src/graphmix/chemistry/adapters/repository.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1622 2024-05-28 17:35:45.000000 graphmix-0.0.0/src/graphmix/chemistry/chemical.py
--rw-r--r--   0 jtaylor    (501) staff       (20)        0 2024-05-23 22:10:57.000000 graphmix-0.0.0/src/graphmix/chemistry/registry.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.262081 graphmix-0.0.0/src/graphmix/chemistry/service_layer/
--rw-r--r--   0 jtaylor    (501) staff       (20)        0 2024-05-24 16:18:16.000000 graphmix-0.0.0/src/graphmix/chemistry/service_layer/__init__.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1469 2024-05-28 00:34:19.000000 graphmix-0.0.0/src/graphmix/chemistry/service_layer/pubchem.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1766 2024-05-24 17:48:33.000000 graphmix-0.0.0/src/graphmix/chemistry/service_layer/registry.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1174 2024-05-28 06:42:42.000000 graphmix-0.0.0/src/graphmix/chemistry/service_layer/unit_of_work.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     4908 2024-05-28 06:41:31.000000 graphmix-0.0.0/src/graphmix/chemistry/units.py
--rw-r--r--   0 jtaylor    (501) staff       (20)      253 2024-05-23 22:36:26.000000 graphmix-0.0.0/src/graphmix/cli.py
--rw-r--r--   0 jtaylor    (501) staff       (20)       49 2024-05-24 17:45:43.000000 graphmix-0.0.0/src/graphmix/config.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.262524 graphmix-0.0.0/src/graphmix/core/
--rw-r--r--   0 jtaylor    (501) staff       (20)        0 2024-05-23 22:09:54.000000 graphmix-0.0.0/src/graphmix/core/__init__.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1339 2024-05-28 17:35:45.000000 graphmix-0.0.0/src/graphmix/core/repository.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.262961 graphmix-0.0.0/src/graphmix/core/sqlmodel/
--rw-r--r--   0 jtaylor    (501) staff       (20)        0 2024-05-23 22:16:10.000000 graphmix-0.0.0/src/graphmix/core/sqlmodel/__init__.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1217 2024-05-28 17:38:11.000000 graphmix-0.0.0/src/graphmix/core/sqlmodel/repository.py
--rw-r--r--   0 jtaylor    (501) staff       (20)      920 2024-05-28 17:39:28.000000 graphmix-0.0.0/src/graphmix/core/sqlmodel/unit_of_work.py
--rw-r--r--   0 jtaylor    (501) staff       (20)      524 2024-05-23 23:22:55.000000 graphmix-0.0.0/src/graphmix/core/unit_of_work.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     2255 2024-05-24 17:56:32.000000 graphmix-0.0.0/src/graphmix/core/util.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.263381 graphmix-0.0.0/src/graphmix/graph/
--rw-r--r--   0 jtaylor    (501) staff       (20)        0 2024-05-24 17:57:36.000000 graphmix-0.0.0/src/graphmix/graph/__init__.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1895 2024-05-28 17:35:45.000000 graphmix-0.0.0/src/graphmix/graph/graph.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     2838 2024-05-28 17:35:45.000000 graphmix-0.0.0/src/graphmix/graph/solution.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.264431 graphmix-0.0.0/src/graphmix.egg-info/
--rw-r--r--   0 jtaylor    (501) staff       (20)     2267 2024-05-28 17:41:45.000000 graphmix-0.0.0/src/graphmix.egg-info/PKG-INFO
--rw-r--r--   0 jtaylor    (501) staff       (20)     1893 2024-05-28 17:41:45.000000 graphmix-0.0.0/src/graphmix.egg-info/SOURCES.txt
--rw-r--r--   0 jtaylor    (501) staff       (20)        1 2024-05-28 17:41:45.000000 graphmix-0.0.0/src/graphmix.egg-info/dependency_links.txt
--rw-r--r--   0 jtaylor    (501) staff       (20)       46 2024-05-28 17:41:45.000000 graphmix-0.0.0/src/graphmix.egg-info/entry_points.txt
--rw-r--r--   0 jtaylor    (501) staff       (20)        1 2024-05-28 17:41:40.000000 graphmix-0.0.0/src/graphmix.egg-info/not-zip-safe
--rw-r--r--   0 jtaylor    (501) staff       (20)        9 2024-05-28 17:41:45.000000 graphmix-0.0.0/src/graphmix.egg-info/top_level.txt
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.263513 graphmix-0.0.0/tests/
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.254721 graphmix-0.0.0/tests/chemical/
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.263656 graphmix-0.0.0/tests/chemical/e2e/
--rw-r--r--   0 jtaylor    (501) staff       (20)      513 2024-05-24 17:17:46.000000 graphmix-0.0.0/tests/chemical/e2e/test_registry.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.263900 graphmix-0.0.0/tests/chemical/integration/
--rw-r--r--   0 jtaylor    (501) staff       (20)      693 2024-05-24 16:43:48.000000 graphmix-0.0.0/tests/chemical/integration/test_repository.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1055 2024-05-24 16:57:31.000000 graphmix-0.0.0/tests/chemical/integration/test_uow.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.264135 graphmix-0.0.0/tests/chemical/unit/
--rw-r--r--   0 jtaylor    (501) staff       (20)      522 2024-05-28 17:35:45.000000 graphmix-0.0.0/tests/chemical/unit/test_chemical.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     2157 2024-05-28 17:35:45.000000 graphmix-0.0.0/tests/chemical/unit/test_units.py
--rw-r--r--   0 jtaylor    (501) staff       (20)      642 2024-05-28 06:42:42.000000 graphmix-0.0.0/tests/conftest.py
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.254830 graphmix-0.0.0/tests/graph/
-drwxr-xr-x   0 jtaylor    (501) staff       (20)        0 2024-05-28 17:41:45.264259 graphmix-0.0.0/tests/graph/unit/
--rw-r--r--   0 jtaylor    (501) staff       (20)      856 2024-05-28 17:38:34.000000 graphmix-0.0.0/tests/graph/unit/test_graph.py
--rw-r--r--   0 jtaylor    (501) staff       (20)     1700 2024-05-23 19:16:04.000000 graphmix-0.0.0/tox.ini
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 graphmix-0.0.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 graphmix-0.0.1/.cookiecutterrc
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 graphmix-0.0.1/.coveragerc
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 graphmix-0.0.1/.editorconfig
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 graphmix-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 graphmix-0.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 graphmix-0.0.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 graphmix-0.0.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 graphmix-0.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 graphmix-0.0.1/pytest.ini
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 graphmix-0.0.1/tox.ini
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 graphmix-0.0.1/.github/workflows/github-actions.yml
+-rwxr-xr-x   0        0        0     2984 2020-02-02 00:00:00.000000 graphmix-0.0.1/ci/bootstrap.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 graphmix-0.0.1/ci/requirements.txt
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 graphmix-0.0.1/ci/templates/.github/workflows/github-actions.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/authors.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/changelog.rst
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/contributing.rst
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/index.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/installation.rst
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/readme.rst
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/usage.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/reference/graphmix.rst
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 graphmix-0.0.1/docs/reference/index.rst
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 graphmix-0.0.1/examples/graphmix_examples.ipynb
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/__main__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/cli.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/config.py
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/location.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/__init__.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/chemical.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/math.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/units.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/adapters/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/adapters/repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/service_layer/__init__.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/service_layer/pubchem.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/service_layer/registry.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/chemistry/service_layer/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/core/__init__.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/core/repository.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/core/unit_of_work.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/core/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/core/sqlmodel/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/core/sqlmodel/repository.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/core/sqlmodel/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/graph/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/graph/drawing.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/graph/model.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/graph/protocol.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/graph/solution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/graph/builder/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/graph/builder/builder.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 graphmix-0.0.1/src/graphmix/graph/builder/standards.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/conftest.py
+-rw-r--r--   0        0        0    19418 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/test.svg
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/e2e/chemical/test_registry.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/integration/chemical/test_repository.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/integration/chemical/test_uow.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/unit/test_location.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/unit/chemical/unit/test_chemical.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/unit/chemical/unit/test_units.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/unit/graph/test_protocol.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/unit/graph/test_solution.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 graphmix-0.0.1/tests/unit/graph/builder/test_standards.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 graphmix-0.0.1/.gitignore
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 graphmix-0.0.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 graphmix-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 graphmix-0.0.1/README.rst
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 graphmix-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 graphmix-0.0.1/PKG-INFO
```

### Comparing `graphmix-0.0.0/.bumpversion.cfg` & `graphmix-0.0.1/.bumpversion.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 [bumpversion]
-current_version = 0.0.0
+current_version = 0.0.1
 commit = True
 tag = True
 
-[bumpversion:file:setup.py]
-search = version="{current_version}"
-replace = version="{new_version}"
-
 [bumpversion:file (badge):README.rst]
 search = /v{current_version}.svg
 replace = /v{new_version}.svg
 
 [bumpversion:file (link):README.rst]
 search = /v{current_version}...main
 replace = /v{new_version}...main
@@ -22,7 +18,12 @@
 [bumpversion:file:src/graphmix/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [bumpversion:file:.cookiecutterrc]
 search = version: {current_version}
 replace = version: {new_version}
+
+[bumpversion:file:pyproject.toml]
+search = version = "{current_version}"
+replace = version = "{new_version}"
+
```

### Comparing `graphmix-0.0.0/.cookiecutterrc` & `graphmix-0.0.1/.cookiecutterrc`

 * *Files 1% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://python-graphmix.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
     test_matrix_separate_coverage: "no"
     tests_inside_package: "no"
-    version: "0.0.0"
+    version: 0.0.1
     version_manager: "bump2version"
     website: "https://blog.ionelmc.ro"
     year_from: "2024"
     year_to: "2024"
```

### Comparing `graphmix-0.0.0/.pre-commit-config.yaml` & `graphmix-0.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/CONTRIBUTING.rst` & `graphmix-0.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/LICENSE` & `graphmix-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/README.rst` & `graphmix-0.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/graphmix
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/graphmix.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/graphmix
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/jt05610/python-graphmix/v0.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/jt05610/python-graphmix/v0.0.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/jt05610/python-graphmix/compare/v0.0.0...main
+    :target: https://github.com/jt05610/python-graphmix/compare/v0.0.1...main
 
 
 
 .. end-badges
 
 Intelligent experiment planning and optimization powered by graph algorithms.
```

### Comparing `graphmix-0.0.0/ci/bootstrap.py` & `graphmix-0.0.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/ci/templates/.github/workflows/github-actions.yml` & `graphmix-0.0.1/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/docs/conf.py` & `graphmix-0.0.1/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,29 +11,31 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "GraphMix"
 year = "2024"
 author = "Jonathan Ross Taylor"
 copyright = f"{year}, {author}"
-version = release = "0.0.0"
+version = release = "0.0.1"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/jt05610/python-graphmix/issues/%s", "#%s"),
     "pr": ("https://github.com/jt05610/python-graphmix/pull/%s", "PR #%s"),
 }
 
 html_theme = "furo"
 html_theme_options = {
-    "githuburl": "https://github.com/jt05610/python-graphmix/",
+    "source_repository": "https://github.com/jt05610/python-graphmix/",
 }
 
 html_use_smartypants = True
 html_last_updated_fmt = "%b %d, %Y"
 html_split_index = False
 html_short_title = f"{project}-{version}"
 
 napoleon_use_ivar = True
 napoleon_use_rtype = False
 napoleon_use_param = False
+
+linkcheck_report_timeouts_as_broken = False
```

### Comparing `graphmix-0.0.0/pytest.ini` & `graphmix-0.0.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/src/graphmix/chemistry/chemical.py` & `graphmix-0.0.1/src/graphmix/chemistry/chemical.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import decimal
 from typing import Any
-from typing import Optional
 
 from sqlalchemy import String
 from sqlalchemy import TypeDecorator
 from sqlmodel import Field
 from sqlmodel import SQLModel
 
 from graphmix.chemistry.units import Q_
@@ -32,18 +31,18 @@
                 return Q_(value)
             return value
 
         return process
 
 
 class Chemical(SQLModel, table=True):
-    id: Optional[int] = Field(default=None, primary_key=True)
+    id: int | None = Field(default=None, primary_key=True, repr=False)
     name: str
     formula: str
-    smiles: Optional[str] = None
+    smiles: str | None = None
     molar_mass: MolarMass | str = Field(sa_type=Quantity)
 
     def count(self, element: str) -> int:
         if self.smiles is None:
             return 0
         return self.smiles.count(element)
```

### Comparing `graphmix-0.0.0/src/graphmix/chemistry/service_layer/pubchem.py` & `graphmix-0.0.1/src/graphmix/chemistry/service_layer/pubchem.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/src/graphmix/chemistry/service_layer/registry.py` & `graphmix-0.0.1/src/graphmix/chemistry/service_layer/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+from pathlib import Path
+
 from graphmix.chemistry.chemical import Chemical
 from graphmix.chemistry.service_layer.pubchem import PubChemService
-from graphmix.chemistry.service_layer.unit_of_work import DEFAULT_CHEMICAL_UOW
 from graphmix.chemistry.service_layer.unit_of_work import ChemicalUnitOfWork
+from graphmix.chemistry.service_layer.unit_of_work import session_factory
 
 
 class ChemicalRegistry:
     """
     A registry for storing and retrieving chemical information. Uses a local
     database to store chemicals, and queries PubChem if a chemical is not
     found.
     """
 
     uow: ChemicalUnitOfWork
     pubchem: PubChemService
 
-    def __init__(self, uow: ChemicalUnitOfWork = DEFAULT_CHEMICAL_UOW):
+    def __init__(
+        self,
+        uow: ChemicalUnitOfWork | None = None,
+        path: str | None = None,
+    ):
+        if uow is None:
+            uow = ChemicalUnitOfWork(session_factory=session_factory(path))
         self.uow = uow
         self.pubchem = PubChemService()
 
     def get_chemical(self, name: str) -> Chemical:
         """
         Get a chemical by name. If the chemical is not found in the local
         database, query PubChem for the chemical information.
         """
         with self.uow:
-            chemical = self.uow.repo.get_by("name", name)
+            chemical = self.uow.repo.get_by("name", name.lower())
             if chemical is not None:
                 return chemical
             chemical = self.pubchem.lookup(name)
             if chemical is None:
                 raise ValueError(f"Chemical {name} not found")
             self.uow.repo.add(chemical)
             self.uow.session.expunge(chemical)
@@ -38,12 +46,17 @@
     def add_chemical(self, chemical: Chemical):
         """
         Add a chemical to the local database.
         """
         with self.uow:
             if self.uow.repo.get_by("name", chemical.name) is not None:
                 raise ValueError(f"Chemical {chemical.name} already exists")
+            chemical.name = chemical.name.lower()
             self.uow.repo.add(chemical)
             self.uow.commit()
 
-    def chem(self, name: str) -> Chemical:
+    def Chemical(self, name: str) -> Chemical:
         return self.get_chemical(name)
+
+    @property
+    def path(self) -> Path:
+        return self.uow.path
```

### Comparing `graphmix-0.0.0/src/graphmix/chemistry/service_layer/unit_of_work.py` & `graphmix-0.0.1/src/graphmix/chemistry/service_layer/unit_of_work.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,34 +12,33 @@
 
 
 def db_path(db_name: str) -> Path:
     db_dir = get_app_dir(config.APP_NAME)
     return Path(db_dir) / db_name
 
 
-def session_factory(db_name: str = config.DB_NAME) -> SessionFactory:
-    path = db_path(db_name)
+def session_factory(db_name: str | Path | None = None) -> SessionFactory:
+    if db_name is None:
+        path = db_path(config.DB_NAME)
+    else:
+        path = Path(db_name)
+
     sqlite_path = f"sqlite:///{path}"
     needs_metadata = False
     if not Path.exists(path):
         needs_metadata = True
-        path.mkdir(parents=True)
+        path.parent.mkdir(parents=True, exist_ok=True)
+        path.touch()
 
     engine = create_engine(sqlite_path, echo=False)
     # if the file does not exist, create the metadata
     if needs_metadata:
         SQLModel.metadata.create_all(engine)
 
     def _factory():
         return Session(engine)
 
-    return _factory
-
-
-DEFAULT_SESSION_FACTORY = session_factory()
+    return SessionFactory(f=_factory, path=path)
 
 
 class ChemicalUnitOfWork(SqlModelUnitOfWork):
     model = Chemical
-
-
-DEFAULT_CHEMICAL_UOW = ChemicalUnitOfWork(DEFAULT_SESSION_FACTORY)
```

### Comparing `graphmix-0.0.0/src/graphmix/chemistry/units.py` & `graphmix-0.0.1/src/graphmix/chemistry/units.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from decimal import Decimal
-from enum import StrEnum
 from typing import Annotated
 from typing import Any
 
 import pint
 from pydantic import GetCoreSchemaHandler
 from pydantic import GetJsonSchemaHandler
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import CoreSchema
 from pydantic_core import core_schema
 
+from graphmix.core.util import StrEnum
+
 ureg = pint.UnitRegistry()
-ureg.setup_matplotlib()
 ureg.default_format = "P~"
 
 
 def dimensionality_validator(
     dimensionality: str | None = None, default_unit: str | None = None
 ):
 
@@ -23,29 +23,35 @@
 
         def validator_func(value: ureg.Quantity) -> ureg.Quantity:
             return value
 
     else:
 
         def validator_func(value: ureg.Quantity) -> ureg.Quantity:
-            if value.dimensionality != dimensionality:
+            if (
+                value.units.dimensionality != dimensionality
+                and value.units != "percent"
+            ):
                 raise ValueError(
                     f"Expected a quantity with dimensionality {dimensionality}, but got {value.dimensionality}."
                 )
             return value
 
     if default_unit is None:
 
         def convert_func(value: int | float | str | Decimal) -> ureg.Quantity:
             return ureg.Quantity(value)
 
     else:
 
         def convert_func(value: int | float | str | Decimal) -> ureg.Quantity:
-            return ureg.Quantity(value, default_unit)
+            q = ureg.Quantity(value)
+            if q.units == "":
+                q = Quantity(q.magnitude, default_unit)
+            return q
 
     class _QuantityPydanticAnnotation:
 
         @classmethod
         def __get_pydantic_core_schema__(
             cls, _source_type: Any, _handler: GetCoreSchemaHandler
         ) -> CoreSchema:
@@ -125,32 +131,50 @@
 mM = ureg.mM
 percent = ureg.percent
 g = ureg.g
 
 
 class Dimensionality(StrEnum):
     Mass = "[mass]"
-    Substance = "[substance]"
+    Mole = "[substance]"
     MolarMass = "[mass] / [substance]"
     MolarConcentration = "[substance] / [length] ** 3"
     MassConcentration = "[mass] / [length] ** 3"
     Volume = "[length] ** 3"
     Percent = "dimensionless"
 
 
-class DimQuantity:
-
+class DimQuantity(Quantity):
     def __class_getitem__(
-        cls, item: str | Dimensionality, default_unit: str | None = None
+        cls, item: str | Dimensionality | tuple[Dimensionality, str]
     ):
-        return Annotated[
-            ureg.Quantity, dimensionality_validator(item, default_unit)
-        ]
+        if isinstance(item, tuple):
+            validator = dimensionality_validator(item[0], item[1])
+        else:
+            validator = dimensionality_validator(item)
+
+        return Annotated[ureg.Quantity, validator]
+
+
+Mass = DimQuantity[Dimensionality.Mass, "g"]
+"""A Quantity that must have a mass unit."""
+
+Mole = DimQuantity[Dimensionality.Mole, "mol"]
+"""A Quantity that must have a mole unit."""
+
+MolarMass = DimQuantity[Dimensionality.MolarMass, "g/mol"]
+"""A Quantity that must have a molar mass unit."""
+
+MolarConcentration = DimQuantity[Dimensionality.MolarConcentration, "mol/mL"]
+"""A Quantity that must have a molar concentration unit."""
+
+MassConcentration = DimQuantity[Dimensionality.MassConcentration, "mg/mL"]
+"""A Quantity that must have a mass concentration unit."""
+
+Volume = DimQuantity[Dimensionality.Volume, "mL"]
+"""A Quantity that must have a volume unit."""
 
+Percent = DimQuantity[Dimensionality.Percent, "%"]
+"""A Quantity that must be dimensionless."""
 
-Mass = DimQuantity[Dimensionality.Mass]
-Substance = DimQuantity[Dimensionality.Substance]
-MolarMass = DimQuantity[Dimensionality.MolarMass]
-MolarConcentration = DimQuantity[Dimensionality.MolarConcentration]
-MassConcentration = DimQuantity[Dimensionality.MassConcentration]
-Volume = DimQuantity[Dimensionality.Volume]
-Percent = DimQuantity[Dimensionality.Percent]
+Concentration = MolarConcentration | MassConcentration
+"""A Quantity that must have a concentration unit, either molar or MassConcentration."""
```

### Comparing `graphmix-0.0.0/src/graphmix/core/repository.py` & `graphmix-0.0.1/src/graphmix/core/repository.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/src/graphmix/core/sqlmodel/repository.py` & `graphmix-0.0.1/src/graphmix/core/sqlmodel/repository.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/src/graphmix/core/sqlmodel/unit_of_work.py` & `graphmix-0.0.1/src/graphmix/core/sqlmodel/unit_of_work.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,32 @@
-from typing import Callable
+from collections.abc import Callable
+from pathlib import Path
 from typing import Generic
 
 from sqlmodel import Session
 
 from graphmix.core.repository import T
 from graphmix.core.sqlmodel.repository import SqlModelRepository
 from graphmix.core.unit_of_work import AbstractUnitOfWork
 
-SessionFactory = Callable[[], Session]
+
+class SessionFactory:
+    f: Callable[[], Session]
+    path: Path | None = None
+
+    def __init__(
+        self, f: Callable[[], Session], path: str | Path | None = None
+    ):
+        if path is not None and not isinstance(path, Path):
+            path = Path(path)
+        self.f = f
+        self.path = path
+
+    def __call__(self) -> Session:
+        return self.f()
 
 
 class SqlModelUnitOfWork(Generic[T], AbstractUnitOfWork):
     session_factory: SessionFactory
     session: Session
     model: type[T]
 
@@ -28,7 +43,11 @@
         self.session.close()
 
     def _commit(self):
         self.session.commit()
 
     def rollback(self):
         self.session.rollback()
+
+    @property
+    def path(self) -> Path:
+        return self.session_factory.path
```

### Comparing `graphmix-0.0.0/src/graphmix/core/unit_of_work.py` & `graphmix-0.0.1/src/graphmix/core/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/src/graphmix/core/util.py` & `graphmix-0.0.1/src/graphmix/core/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Everything here was copied directly from the `click` library, which is
 licensed under the BSD 3-Clause "New" or "Revised" License. The original source
 code can be found at https://github.com/pallets/click."""
 
 import os
 import sys
+from enum import Enum
 from pathlib import Path
 
 CYGWIN = sys.platform.startswith("cygwin")
 WIN = sys.platform.startswith("win")
 
 
 def _posixify(name: str) -> str:
@@ -60,7 +61,17 @@
             Path(Path("~/Library/Application Support")).expanduser() / app_name
         )
 
     return (
         Path(os.environ.get("XDG_CONFIG_HOME", Path("~/.config").expanduser()))
         / _posixify(app_name),
     )
+
+
+class StrEnum(str, Enum):
+    """
+    A string-based Enum copied from
+    https://www.cosmicpython.com/blog/2020-10-27-i-hate-enums.html
+    """
+
+    def __str__(self) -> str:
+        return str.__str__(self)
```

### Comparing `graphmix-0.0.0/src/graphmix/graph/graph.py` & `graphmix-0.0.1/src/graphmix/graph/model.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/tests/chemical/e2e/test_registry.py` & `graphmix-0.0.1/tests/e2e/chemical/test_registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,12 +6,20 @@
 def test_chemical_registry_adds_chemical_when_not_known(
     sqlite_session_factory,
 ):
     uow = ChemicalUnitOfWork(sqlite_session_factory)
 
     reg = ChemicalRegistry(uow)
 
-    water = reg.chem("water")
-
+    water = reg.Chemical("water")
     assert water.name == "water"
     assert water.formula == "H2O"
     assert water.molar_mass == Q_("18.015 g/mol")
+
+
+def test_registry_path(sqlite_session_factory, tmp_path):
+    tmp_db = tmp_path / "test.db"
+
+    assert not tmp_db.exists()
+    reg = ChemicalRegistry(path=tmp_db)
+    assert reg.path.exists()
+    assert tmp_db.exists()
```

### Comparing `graphmix-0.0.0/tests/chemical/integration/test_repository.py` & `graphmix-0.0.1/tests/integration/chemical/test_repository.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/tests/chemical/integration/test_uow.py` & `graphmix-0.0.1/tests/integration/chemical/test_uow.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/tests/chemical/unit/test_chemical.py` & `graphmix-0.0.1/tests/unit/chemical/unit/test_chemical.py`

 * *Files identical despite different names*

### Comparing `graphmix-0.0.0/tests/chemical/unit/test_units.py` & `graphmix-0.0.1/tests/unit/chemical/unit/test_units.py`

 * *Files 17% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             return
         instance = FakeModel(volume=passed_value)
         assertions(instance)
 
     checks_to_run = (
         (Q_("100 uL"), Q_("100 uL")),
         (Q_(100, "uL"), Q_("100 uL")),
-        (100, Q_("100 uL"), ValidationError),
+        (100, Q_("100 mL")),
         ("100 uL", Q_("100 uL")),
         ("100 s", Q_("100 uL"), ValidationError),
         (Q_(100, "s"), Q_("100 uL"), ValidationError),
     )
 
     for m, v, e in iter_tuple_with_arguments(checks_to_run, 3):
         assert_model(m, v, e)
```

