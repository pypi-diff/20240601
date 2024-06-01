# Comparing `tmp/heaserver_people-1.3.1.tar.gz` & `tmp/heaserver_people-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_people-1.3.1.tar", last modified: Tue May 21 23:39:31 2024, max compression
+gzip compressed data, was "heaserver_people-1.3.2.tar", last modified: Sat Jun  1 13:31:33 2024, max compression
```

## Comparing `heaserver_people-1.3.1.tar` & `heaserver_people-1.3.2.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.389366 heaserver_people-1.3.1/
--rw-rw-rw-   0        0        0      261 2023-12-18 20:25:25.000000 heaserver_people-1.3.1/.editorconfig
--rw-rw-rw-   0        0        0      353 2023-12-18 20:25:25.000000 heaserver_people-1.3.1/.gitignore
--rw-rw-rw-   0        0        0    11625 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6031 2024-05-21 23:39:31.388581 heaserver_people-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4673 2024-05-21 23:38:09.000000 heaserver_people-1.3.1/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.323184 heaserver_people-1.3.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.350643 heaserver_people-1.3.1/integrationtests/.pytest_cache/
--rw-rw-rw-   0        0        0       39 2023-02-23 16:41:17.000000 heaserver_people-1.3.1/integrationtests/.pytest_cache/.gitignore
--rw-rw-rw-   0        0        0      194 2023-02-23 16:41:17.000000 heaserver_people-1.3.1/integrationtests/.pytest_cache/CACHEDIR.TAG
--rw-rw-rw-   0        0        0      303 2023-02-23 16:41:17.000000 heaserver_people-1.3.1/integrationtests/.pytest_cache/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.323184 heaserver_people-1.3.1/integrationtests/.pytest_cache/v/
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.353645 heaserver_people-1.3.1/integrationtests/.pytest_cache/v/cache/
--rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver_people-1.3.1/integrationtests/.pytest_cache/v/cache/nodeids
--rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver_people-1.3.1/integrationtests/.pytest_cache/v/cache/stepwise
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.323184 heaserver_people-1.3.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.360899 heaserver_people-1.3.1/integrationtests/heaserver/personintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/integrationtests/heaserver/personintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4674 2024-04-18 03:47:11.000000 heaserver_people-1.3.1/integrationtests/heaserver/personintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      547 2024-02-25 02:42:01.000000 heaserver_people-1.3.1/integrationtests/heaserver/personintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     9151 2024-05-21 23:33:02.000000 heaserver_people-1.3.1/integrationtests/heaserver/personintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 23:39:31.390217 heaserver_people-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1854 2024-05-21 23:38:55.000000 heaserver_people-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.323184 heaserver_people-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.323184 heaserver_people-1.3.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.369717 heaserver_people-1.3.1/src/heaserver/person/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/src/heaserver/person/__init__.py
--rw-rw-rw-   0        0        0     4121 2024-02-25 02:42:01.000000 heaserver_people-1.3.1/src/heaserver/person/keycloakmockmongotestcase.py
--rw-rw-rw-   0        0        0    40214 2024-05-21 23:18:19.000000 heaserver_people-1.3.1/src/heaserver/person/keycloakmongo.py
--rw-rw-rw-   0        0        0    10027 2024-03-26 23:05:06.000000 heaserver_people-1.3.1/src/heaserver/person/keycloakmongotestcase.py
--rw-rw-rw-   0        0        0    19537 2024-05-21 23:31:38.000000 heaserver_people-1.3.1/src/heaserver/person/service.py
--rw-rw-rw-   0        0        0     2114 2024-05-21 23:18:19.000000 heaserver_people-1.3.1/src/heaserver/person/testcasedata.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.370717 heaserver_people-1.3.1/src/heaserver/person/wstl/
--rw-rw-rw-   0        0        0    16523 2024-05-21 23:18:19.000000 heaserver_people-1.3.1/src/heaserver/person/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.386584 heaserver_people-1.3.1/src/heaserver_people.egg-info/
--rw-rw-rw-   0        0        0     6031 2024-05-21 23:39:31.000000 heaserver_people-1.3.1/src/heaserver_people.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2024-05-21 23:39:31.000000 heaserver_people-1.3.1/src/heaserver_people.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 23:39:31.000000 heaserver_people-1.3.1/src/heaserver_people.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-21 23:39:31.000000 heaserver_people-1.3.1/src/heaserver_people.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-21 23:39:31.000000 heaserver_people-1.3.1/src/heaserver_people.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 23:39:31.000000 heaserver_people-1.3.1/src/heaserver_people.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.330884 heaserver_people-1.3.1/tests/
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.330884 heaserver_people-1.3.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-21 23:39:31.385583 heaserver_people-1.3.1/tests/heaserver/persontest/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/tests/heaserver/persontest/__init__.py
--rw-rw-rw-   0        0        0     4010 2024-04-18 03:47:11.000000 heaserver_people-1.3.1/tests/heaserver/persontest/permissionstestcase.py
--rw-rw-rw-   0        0        0     1343 2023-12-18 20:25:26.000000 heaserver_people-1.3.1/tests/heaserver/persontest/test_all.py
--rw-rw-rw-   0        0        0     8473 2024-05-21 23:32:46.000000 heaserver_people-1.3.1/tests/heaserver/persontest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.237797 heaserver_people-1.3.2/
+-rw-rw-rw-   0        0        0      261 2023-07-17 19:11:22.000000 heaserver_people-1.3.2/.editorconfig
+-rw-rw-rw-   0        0        0      353 2023-07-17 19:11:22.000000 heaserver_people-1.3.2/.gitignore
+-rw-rw-rw-   0        0        0    11625 2023-07-17 19:11:22.000000 heaserver_people-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-07-17 19:11:22.000000 heaserver_people-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6119 2024-06-01 13:31:33.237797 heaserver_people-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4761 2024-06-01 13:29:39.000000 heaserver_people-1.3.2/README.md
+-rw-rw-rw-   0        0        0     1878 2023-07-17 19:11:22.000000 heaserver_people-1.3.2/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.077891 heaserver_people-1.3.2/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.078894 heaserver_people-1.3.2/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.131953 heaserver_people-1.3.2/integrationtests/heaserver/personintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-07-17 19:11:22.000000 heaserver_people-1.3.2/integrationtests/heaserver/personintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4674 2024-05-13 15:30:02.000000 heaserver_people-1.3.2/integrationtests/heaserver/personintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      547 2023-12-12 20:18:22.000000 heaserver_people-1.3.2/integrationtests/heaserver/personintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     9151 2024-05-26 20:18:55.000000 heaserver_people-1.3.2/integrationtests/heaserver/personintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2024-05-21 21:01:59.000000 heaserver_people-1.3.2/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-08-29 13:24:09.000000 heaserver_people-1.3.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 13:31:33.238797 heaserver_people-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1854 2024-06-01 13:29:39.000000 heaserver_people-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.079890 heaserver_people-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.078894 heaserver_people-1.3.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.169945 heaserver_people-1.3.2/src/heaserver/person/
+-rw-rw-rw-   0        0        0        0 2023-07-17 19:11:22.000000 heaserver_people-1.3.2/src/heaserver/person/__init__.py
+-rw-rw-rw-   0        0        0     4416 2024-05-26 21:04:37.000000 heaserver_people-1.3.2/src/heaserver/person/keycloakmockmongotestcase.py
+-rw-rw-rw-   0        0        0    44225 2024-05-30 15:48:03.000000 heaserver_people-1.3.2/src/heaserver/person/keycloakmongo.py
+-rw-rw-rw-   0        0        0    11008 2024-05-26 21:04:37.000000 heaserver_people-1.3.2/src/heaserver/person/keycloakmongotestcase.py
+-rw-rw-rw-   0        0        0    20433 2024-05-30 15:48:03.000000 heaserver_people-1.3.2/src/heaserver/person/service.py
+-rw-rw-rw-   0        0        0     2114 2024-05-26 20:18:55.000000 heaserver_people-1.3.2/src/heaserver/person/testcasedata.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.175945 heaserver_people-1.3.2/src/heaserver/person/wstl/
+-rw-rw-rw-   0        0        0    16523 2024-05-26 20:18:55.000000 heaserver_people-1.3.2/src/heaserver/person/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.236797 heaserver_people-1.3.2/src/heaserver_people.egg-info/
+-rw-rw-rw-   0        0        0     6119 2024-06-01 13:31:33.000000 heaserver_people-1.3.2/src/heaserver_people.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1811 2024-06-01 13:31:33.000000 heaserver_people-1.3.2/src/heaserver_people.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:31:33.000000 heaserver_people-1.3.2/src/heaserver_people.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-06-01 13:31:33.000000 heaserver_people-1.3.2/src/heaserver_people.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-06-01 13:31:33.000000 heaserver_people-1.3.2/src/heaserver_people.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 13:31:33.000000 heaserver_people-1.3.2/src/heaserver_people.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.080915 heaserver_people-1.3.2/tests/
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.080915 heaserver_people-1.3.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.218661 heaserver_people-1.3.2/tests/heaserver/persontest/
+-rw-rw-rw-   0        0        0        0 2023-07-17 19:11:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:31:33.235808 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.15768
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.16124
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.28000
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.29900
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.32012
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.3816
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.38400
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.4680
+-rw-rw-rw-   0        0        0     2160 2023-11-27 18:30:22.000000 heaserver_people-1.3.2/tests/heaserver/persontest/__pycache__/test_all.cpython-310-pytest-7.3.2.pyc.7808
+-rw-rw-rw-   0        0        0     4010 2024-05-13 15:30:02.000000 heaserver_people-1.3.2/tests/heaserver/persontest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     1343 2023-11-16 16:03:00.000000 heaserver_people-1.3.2/tests/heaserver/persontest/test_all.py
+-rw-rw-rw-   0        0        0     8473 2024-05-26 20:18:55.000000 heaserver_people-1.3.2/tests/heaserver/persontest/testcase.py
```

### Comparing `heaserver_people-1.3.1/LICENSE` & `heaserver_people-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/PKG-INFO` & `heaserver_people-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-people
-Version: 1.3.1
+Version: 1.3.2
 Summary: A microservice designed to provide CRUD operations for the Person HEA object type
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-people,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.6.0
+Requires-Dist: heaserver~=1.6.2
 
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.3.2
+* Adds ability got get access tokens internally for microservices.
+
 ## Version 1.3.1
 * Prevent Volumes collection from appearing in the system menu.
 
 ## Version 1.3.0
 * Display type display name in properties card, and return it from GET calls.
 * Changed /groups and /roles to get all groups and roles.
 * New API for modifying a person's groups.
```

### Comparing `heaserver_people-1.3.1/README.md` & `heaserver_people-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.3.2
+* Adds ability got get access tokens internally for microservices.
+
 ## Version 1.3.1
 * Prevent Volumes collection from appearing in the system menu.
 
 ## Version 1.3.0
 * Display type display name in properties card, and return it from GET calls.
 * Changed /groups and /roles to get all groups and roles.
 * New API for modifying a person's groups.
```

### Comparing `heaserver_people-1.3.1/RELEASING.md` & `heaserver_people-1.3.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/integrationtests/heaserver/personintegrationtest/permissionstestcase.py` & `heaserver_people-1.3.2/integrationtests/heaserver/personintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/integrationtests/heaserver/personintegrationtest/test_all.py` & `heaserver_people-1.3.2/integrationtests/heaserver/personintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/integrationtests/heaserver/personintegrationtest/testcase.py` & `heaserver_people-1.3.2/integrationtests/heaserver/personintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/setup.py` & `heaserver_people-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-people',
-    version='1.3.1',
+    version='1.3.2',
     description="A microservice designed to provide CRUD operations for the Person HEA object type",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.person'],
     package_data={'heaserver.person': ['wstl/*.json']},
-    install_requires=['heaserver~=1.6.0'],
+    install_requires=['heaserver~=1.6.2'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver_people-1.3.1/src/heaserver/person/keycloakmockmongotestcase.py` & `heaserver_people-1.3.2/src/heaserver/person/keycloakmockmongotestcase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import configparser
 from aiohttp.web import Request
 
 from aiohttp.web_request import Request
-from heaobject.person import Person
+from heaobject.person import Person, AccessToken
 from heaobject.user import ALL_USERS
 from heaserver.service.oidcclaimhdrs import SUB
 from heaserver.service.testcase.mockmongo import MockMongo, MockMongoManager
 
 from heaserver.person.keycloakmongo import DEFAULT_CLIENT_ID, DEFAULT_REALM, DEFAULT_HOST, DEFAULT_SECRET_FILE, \
     CONFIG_SECTION, DEFAULT_VERIFY_SSL
 from heaserver.person.testcasedata import person1, person2
 
 
 class KeycloakMockMongo(MockMongo):
     def __init__(self, config: configparser.ConfigParser | None = None,
                  client_id: str | None = DEFAULT_CLIENT_ID,
                  realm: str | None = DEFAULT_REALM,
                  host: str | None = DEFAULT_HOST,
+                 alt_host: str | None = None,
                  secret: str | None = None,
                  secret_file: str | None = DEFAULT_SECRET_FILE,
                  verify_ssl: bool = False):
         super().__init__(config)
         if config and CONFIG_SECTION in config:
             _section = config[CONFIG_SECTION]
             self.__realm = str(_section.get('Realm', realm) or DEFAULT_REALM)
             self.__verify_ssl = _section.getboolean('VerifySSL', verify_ssl if verify_ssl is not None else DEFAULT_VERIFY_SSL)
             self.__host = str(_section.get('Host', host) or DEFAULT_HOST)
+            self.__alt_host = str(_section.get('AltHost', alt_host))
             _secret = _section.get('Secret', secret)
             self.__secret = str(_secret) if _secret else None
             _secret_file = _section.get('SecretFile', secret_file)
             self.__secret_file = str(_secret_file) if _secret_file else None
         else:
             self.__realm = str(realm) if realm else DEFAULT_REALM
             self.__verify_ssl = bool(verify_ssl) if verify_ssl is not None else DEFAULT_VERIFY_SSL
             self.__host = str(host) if host else DEFAULT_HOST
+            self.__alt_host = str(alt_host) if alt_host else None
             self.__secret = str(secret) if secret else None
             self.__secret_file = str(secret_file) if secret_file else None
 
 
         self.__client_id = str(client_id) if client_id else DEFAULT_CLIENT_ID
 
     @property
@@ -60,16 +63,18 @@
     def secret_file(self) -> str | None:
         return self.__secret_file
 
     @property
     def verify_ssl(self) -> bool:
         return self.__verify_ssl
 
-    async def get_keycloak_access_token(self, request: Request) -> str:
-        return '12345678'
+    async def get_keycloak_access_token(self, request: Request) -> AccessToken:
+        access_token_obj = AccessToken()
+        access_token_obj.id = '12345678'
+        return access_token_obj
 
     async def get_users(self, request: Request, params: dict[str, str] | None = None) -> list[Person]:
         persons = []
         for r in (person1, person2):
             if params is None or all(hasattr(r, k) and v == getattr(r, k) for k, v in params.items()):
                 persons.append(r)
         return persons
```

### Comparing `heaserver_people-1.3.1/src/heaserver/person/keycloakmongo.py` & `heaserver_people-1.3.2/src/heaserver/person/keycloakmongo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import configparser
 from typing import Any
 from heaserver.service.db.mongo import MongoManager, Mongo
 from heaserver.service import appproperty
 from heaserver.service.client import get_property
 from heaserver.service.oidcclaimhdrs import SUB
 from heaserver.service.util import queued_processing
-from heaobject.person import Person, Role, get_system_person, get_system_people, Group, GroupType
+from heaobject.person import Person, Role, get_system_person, get_system_people, Group, GroupType, AccessToken
 from heaobject.user import NONE_USER, ALL_USERS, is_system_user, CREDENTIALS_MANAGER_USER
 from heaobject.root import ShareImpl, Permission
 from heaobject.util import parse_bool
 from aiohttp import ClientResponseError
 from aiohttp.web import Request
 from yarl import URL
 import logging
@@ -50,33 +50,36 @@
 DEFAULT_KEYCLOAK_COMPATIBILITY = KeycloakCompatibility.FIFTEEN
 
 class KeycloakMongo(Mongo):
     """
     Database object for accessing a keycloak server. It subclasses Mongo so that some user data that Keycloak does not
     support might be stored in Mongo.
     """
+
     def __init__(self, config: configparser.ConfigParser | None = None,
                  client_id: str | None = DEFAULT_CLIENT_ID,
                  admin_client_id: str | None = DEFAULT_ADMIN_CLIENT_ID,
                  realm: str | None = DEFAULT_REALM,
                  host: str | None = DEFAULT_HOST,
+                 alt_host: str | None = None,
                  secret: str | None = None,
                  secret_file: str | None = DEFAULT_SECRET_FILE,
                  verify_ssl: bool = DEFAULT_VERIFY_SSL,
                  keycloak_compatibility: KeycloakCompatibility | None = KeycloakCompatibility.FIFTEEN):
         """
         Initializes Keycloak access with a configparser object or manually set configuration parameters. For all
         manually set configuration parameters, the empty string is treated the same as None.
 
         :param config: a configparser.ConfigParser object, which should have a Keycloak section with the following
         properties:
 
             Realm = the Keycloak realm.
             VerifySSL = whether to verify SSL certificates (defaults to yes).
             Host = the keycloak hostname.
+            AltHost = the keycloak alternate hostname.
             Secret = the secret for accessing keycloak.
             SecretFile = alternatively, a file with one line containing the secret.
             Compatibility = 15 or 19 denoting Keycloak 15-18 versus >= 19. The default is 15.
             ClientId = the client id to use. The default is hea.
             AdminClientId = the admin client id to use. The default is admin-cli.
 
         :param client_id: the client id to use. The default is hea.
@@ -94,49 +97,55 @@
         """
         super().__init__(config)
         self.__ttl_cache = TTLCache(maxsize=128, ttl=30)
         if config and CONFIG_SECTION in config:
             _section = config[CONFIG_SECTION]
             _realm = _section.get('Realm', realm)
             self.__realm = str(_realm) if _realm is not None else DEFAULT_REALM
-            self.__verify_ssl = _section.getboolean('VerifySSL', verify_ssl if verify_ssl is not None else DEFAULT_VERIFY_SSL)
+            self.__verify_ssl = _section.getboolean('VerifySSL',
+                                                    verify_ssl if verify_ssl is not None else DEFAULT_VERIFY_SSL)
             self.__host = str(_section.get('Host', host) or DEFAULT_HOST)
+            self.__alt_host = str(_section.get('AltHost', alt_host))
             _secret = _section.get('Secret', secret)
             self.__secret = str(_secret) if _secret else None
             _secret_file = _section.get('SecretFile', secret_file)
             self.__secret_file = str(_secret_file) if _secret_file else None
-            compat = _section.get('Compatibility', None) or keycloak_compatibility or DEFAULT_KEYCLOAK_COMPATIBILITY.value
+            compat = _section.get('Compatibility',
+                                  None) or keycloak_compatibility or DEFAULT_KEYCLOAK_COMPATIBILITY.value
             self.__keycloak_compatibility = KeycloakCompatibility(compat)
             _client_id = _section.get('ClientId', client_id)
             self.__client_id = str(_client_id) if _client_id is not None else DEFAULT_CLIENT_ID
             _admin_client_id = _section.get('AdminClientId', admin_client_id)
             self.__admin_client_id = str(_admin_client_id) if _admin_client_id is not None else DEFAULT_ADMIN_CLIENT_ID
         else:
             self.__realm = str(realm) if realm is not None else DEFAULT_REALM
             self.__verify_ssl = bool(verify_ssl) if verify_ssl is not None else DEFAULT_VERIFY_SSL
             self.__host = str(host) if host is not None else DEFAULT_HOST
+            self.__alt_host = str(alt_host) if alt_host else None
             self.__secret = str(secret) if secret is not None else None
             self.__secret_file = str(secret_file) if secret_file is not None else None
             if keycloak_compatibility is not None and not isinstance(keycloak_compatibility, KeycloakCompatibility):
-                raise ValueError(f'Keycloak_compatibility must be a KeycloakCompatibility enum value or None but was {keycloak_compatibility}')
+                raise ValueError(
+                    f'Keycloak_compatibility must be a KeycloakCompatibility enum value or None but was {keycloak_compatibility}')
             self.__keycloak_compatibility = keycloak_compatibility or DEFAULT_KEYCLOAK_COMPATIBILITY
             self.__client_id = str(client_id) if client_id is not None else DEFAULT_CLIENT_ID
             self.__admin_client_id = str(admin_client_id) if admin_client_id is not None else DEFAULT_ADMIN_CLIENT_ID
         if self.keycloak_compatibility == KeycloakCompatibility.FIFTEEN:
             self.__base_url = URL(self.host) / 'auth'
+            self.__alt_base_url = URL(self.alt_host) / 'auth' if self.__alt_host else None
         else:
             self.__base_url = URL(self.host)
+            self.__alt_base_url = URL(self.alt_host) if self.__alt_host else None
         logger = logging.getLogger(__name__)
         logger.info('Using Keycloak %s mode', self.__keycloak_compatibility.value)
         if self.__host is None:
             raise ValueError
         logger.debug('host is %s', self.__host)
         self.__expiry: datetime | None = None
-        self.__access_token: str | None = None
-
+        self.__access_token: AccessToken | None = None
 
     @property
     def client_id(self) -> str:
         """The Keycloak client id. The default is hea."""
         return self.__client_id
 
     @property
@@ -149,14 +158,18 @@
         return self.__realm
 
     @property
     def host(self) -> str:
         return self.__host
 
     @property
+    def alt_host(self) -> str:
+        return self.__alt_host
+
+    @property
     def secret(self) -> str | None:
         return self.__secret
 
     @property
     def secret_file(self) -> str | None:
         return self.__secret_file
 
@@ -170,23 +183,24 @@
 
     @property
     def _base_url(self) -> URL:
         """A URL composed of the hostname and /auth or not depending on whether keycloak compatibility is set to 15 or
         19."""
         return self.__base_url
 
-    async def get_keycloak_access_token(self, request: Request) -> str:
+    async def get_keycloak_access_token(self, request: Request) -> AccessToken:
         """
         Request an access token from Keycloak. It tries obtaining a secret from the following places, in order:
         1) The secret parameter of this class' constructor, or the Secret property of the Keycloak section of the HEA
         config file.
         2) A file whose name is passed into the constructor, or provided in the SecretFile property of the Keycloak
         section of the HEA config file. The file must contain one line with the secret.
         3) The KEYCLOAK_QUERY_ADMIN_SECRET registry property.
 
+        :param use_alt_base_url:
         :param request: the HTTP request (request).
         :return: the access token or None if not found.
         """
         async with _ACCESS_TOKEN_LOCK:
             if self.__expiry and self.__expiry >= datetime.now() + timedelta(minutes=1):
                 return self.__access_token
             else:
@@ -213,16 +227,62 @@
                 }
                 logger.debug('Going to verify ssl? %r', self.verify_ssl)
                 async with session.post(token_url, data=token_body, verify_ssl=self.verify_ssl) as response_:
                     content = await response_.json()
                     logger.debug('content %s', content)
                     access_token = content['access_token']
                     self.__expiry = datetime.now() + timedelta(seconds=int(content['expires_in']))
-                    self.__access_token = access_token
-                return access_token
+                    access_token_obj = AccessToken()
+                    access_token_obj.id = access_token
+                    self.__access_token = access_token_obj
+                return access_token_obj
+
+    async def get_keycloak_alt_access_token(self, request: Request) -> AccessToken:
+        """
+        Request an access token from Keycloak with alternate path. It tries obtaining a secret from the following places, in order:
+        1) The secret parameter of this class' constructor, or the Secret property of the Keycloak section of the HEA
+        config file.
+        2) A file whose name is passed into the constructor, or provided in the SecretFile property of the Keycloak
+        section of the HEA config file. The file must contain one line with the secret.
+        3) The KEYCLOAK_QUERY_ADMIN_SECRET registry property.
+
+        :param use_alt_base_url:
+        :param request: the HTTP request (request).
+        :return: the access token or None if not found.
+        """
+        async with _ACCESS_TOKEN_LOCK:
+                session = request.app[appproperty.HEA_CLIENT_SESSION]
+                logger = logging.getLogger(__name__)
+
+                token_url = self.__alt_base_url / 'realms' / self.realm / 'protocol' / 'openid-connect' / 'token'
+                logger.debug('Requesting new access token using credentials')
+                if self.secret:
+                    secret = self.secret
+                    logger.debug('Read secret from config or constructor')
+                elif self.secret_file and (secret_file_path := Path(self.secret_file)).exists():
+                    secret = secret_file_path.read_text(encoding='utf-8')
+                    logger.debug('Read secret from file')
+                elif secret_property := await get_property(request.app, KEYCLOAK_QUERY_ADMIN_SECRET):
+                    secret = secret_property.value
+                    logger.debug('Read secret from registry service')
+                else:
+                    raise ValueError('No secret defined')
+                token_body = {
+                    'client_secret': secret,
+                    'client_id': self.admin_client_id,
+                    'grant_type': 'client_credentials'
+                }
+                logger.debug('Going to verify ssl? %r', self.verify_ssl)
+                async with session.post(token_url, data=token_body, verify_ssl=self.verify_ssl) as response_:
+                    content = await response_.json()
+                    logger.debug('content %s', content)
+                    access_token = content['access_token']
+                    access_token_obj = AccessToken()
+                    access_token_obj.id = access_token
+                return access_token_obj
 
     async def get_users(self, request: Request, params: dict[str, str] | None = None) -> list[Person]:
         """
         Gets a list of users from Keycloak using the '/auth/admin/realms/{realm}/users' REST API call.
 
         :param request: the HTTP request (required).
         :param params: any query parameters to add to the users request.
@@ -230,15 +290,16 @@
         """
         logger = logging.getLogger(__name__)
         exclude_system_users = parse_bool(request.query.get('excludesystem', 'no'))
         cached_val = self.__ttl_cache.get(('all_users', exclude_system_users, None))
         if cached_val is not None:
             return list(cached_val)
         else:
-            access_token = await self.get_keycloak_access_token(request)
+            access_token_obj = await self.get_keycloak_access_token(request)
+            access_token = access_token_obj.id
             session = request.app[appproperty.HEA_CLIENT_SESSION]
             users_url = self.__base_url / 'admin' / 'realms' / self.realm / 'users'
             if params:
                 params_ = {}
                 for k, v in params.items():
                     match k:
                         case 'name':
@@ -297,15 +358,16 @@
             return cached_val
         else:
             if is_system_user(id_):
                 person = get_system_person(id_)
                 self.__ttl_cache[('one_user', id_)] = person
                 return person
             else:
-                access_token = await self.get_keycloak_access_token(request)
+                access_token_obj = await self.get_keycloak_access_token(request)
+                access_token = access_token_obj.id
                 session = request.app[appproperty.HEA_CLIENT_SESSION]
                 user_url = self.__base_url / 'admin' / 'realms' / self.realm / 'users' / id_
                 async with session.get(user_url,
                                     headers={'Authorization': f'Bearer {access_token}'},
                                     verify_ssl=self.verify_ssl) as response_:
                     user_json = await response_.json()
                     logger.debug('Response was %s', user_json)
@@ -317,15 +379,14 @@
                 group_dicts: list[dict[str, Any]] = []
                 async for group_dict in self.__get_user_groups_json(request, id_):
                     group_dicts.append(group_dict)
                 person = self.__keycloak_user_to_person(user_json, group_dicts)
                 self.__ttl_cache[('one_user', id_)] = person
                 return deepcopy(person)
 
-
     async def get_current_user_roles(self, request: Request) -> list[Role]:
         """
         Gets the current user's roles.
 
         :param request: the HTTP request (required).
         :returns: a list of Role objects.
         :raises ClientResponseError: if something went wrong getting role information.
@@ -348,16 +409,16 @@
 
         :param request: the HTTP request (required).
         :param role_name: the role to check (required).
         :returns: True or False.
         :raises ClientResponseError: if something went wrong getting role information.
         :raises ValueError: if something went wrong getting role information due to an internal server error.
         """
-        async for role_json in self.__get_my_roles_json(request):
-            if role_json['name'] == role_name:
+        for role in await self.get_current_user_roles(request):
+            if role.role == role_name:
                 return True
         else:
             return False
 
     async def get_user_groups(self, request: Request, sub: str) -> list[Group]:
         """
         Gets the current user's groups.
@@ -370,15 +431,16 @@
         """
         logger = logging.getLogger(__name__)
         cached_val = self.__ttl_cache.get(('my_groups', sub))
         if cached_val is not None:
             return cached_val
         else:
             groups = [self.__new_group(sub, group_json) async for group_json in self.__get_user_groups_json(request, sub)]
-            access_token = await self.get_keycloak_access_token(request)
+            access_token_obj = await self.get_keycloak_access_token(request)
+            access_token = access_token_obj.id
             session = request.app[appproperty.HEA_CLIENT_SESSION]
             role_base_url = self._base_url / 'admin' / 'realms' / self.realm
             session_get = partial(session.get,
                                     headers={'Authorization': f'Bearer {access_token}'},
                                     verify_ssl=self.verify_ssl)
             for group in groups:
                 try:
@@ -404,15 +466,16 @@
         logger = logging.getLogger(__name__)
         sub = request.headers.get(SUB, NONE_USER)
         cached_val = self.__ttl_cache.get(('my_groups', sub))
         if cached_val is not None:
             return cached_val
         else:
             groups = [self.__new_group(sub, group_json) async for group_json in self.__get_my_groups_json(request)]
-            access_token = await self.get_keycloak_access_token(request)
+            access_token_obj = await self.get_keycloak_access_token(request)
+            access_token = access_token_obj.id
             session = request.app[appproperty.HEA_CLIENT_SESSION]
             role_base_url = self._base_url / 'admin' / 'realms' / self.realm
             session_get = partial(session.get,
                                     headers={'Authorization': f'Bearer {access_token}'},
                                     verify_ssl=self.verify_ssl)
             for group in groups:
                 try:
@@ -490,40 +553,43 @@
         return await self.add_user_to_group(request, sub, id_)
 
     async def add_user_to_group(self, request: Request, sub: str, id_: str) -> bool:
         logger = logging.getLogger(__name__)
         actual_sub = request.headers.get(SUB, NONE_USER)
         if actual_sub not in (sub, CREDENTIALS_MANAGER_USER):
             return False
-        access_token = await self.get_keycloak_access_token(request)
+        access_token_obj = await self.get_keycloak_access_token(request)
+        access_token = access_token_obj.id
         session = request.app[appproperty.HEA_CLIENT_SESSION]
         role_base_url = self._base_url / 'admin' / 'realms' / self.realm / 'users' / sub / 'groups'
         session_put = partial(session.put,
                             headers={'Authorization': f'Bearer {access_token}'},
                             verify_ssl=self.verify_ssl)
         async with session_put(role_base_url / id_) as response_:
             if response_.status == 404:
                 return False
             if response_.status != 204:
                 raise ValueError('Adding user to group failed')
             self.__ttl_cache.pop(('my_groups', sub), None)
             self.__ttl_cache.pop(('all_users', True, None), None)
             self.__ttl_cache.pop(('all_users', False, None), None)
             self.__ttl_cache.pop(('one_user', sub), None)
+            self.__ttl_cache.pop(('my_roles', sub), None)
             return True
 
     async def remove_current_user_group(self, request: Request, id_: str) -> bool:
         sub = request.headers.get(SUB, NONE_USER)
         return await self.remove_user_group(request, sub, id_)
 
     async def remove_user_group(self, request: Request, sub: str, id_: str) -> bool:
         actual_sub = request.headers.get(SUB, NONE_USER)
         if actual_sub not in (sub, CREDENTIALS_MANAGER_USER):
             return False
-        access_token = await self.get_keycloak_access_token(request)
+        access_token_obj = await self.get_keycloak_access_token(request)
+        access_token = access_token_obj.id
         session = request.app[appproperty.HEA_CLIENT_SESSION]
 
         role_base_url = self._base_url / 'admin' / 'realms' / self.realm / 'users' / sub / 'groups'
         session_delete = partial(session.delete,
                             headers={'Authorization': f'Bearer {access_token}'},
                             verify_ssl=self.verify_ssl, raise_for_status=False)
         async with session_delete(role_base_url / id_) as response_:
@@ -531,14 +597,15 @@
                 return False
             if response_.status != 204:
                 raise ValueError('Adding user to group failed')
             self.__ttl_cache.pop(('my_groups', sub), None)
             self.__ttl_cache.pop(('all_users', True, None), None)
             self.__ttl_cache.pop(('all_users', False, None), None)
             self.__ttl_cache.pop(('one_user', sub), None)
+            self.__ttl_cache.pop(('my_roles', sub), None)
             return True
 
     async def remove_current_user_group_by_group(self, request: Request, group: str) -> bool:
         if (group_obj := await self.get_current_user_group_by_group(request, group)) is None:
             return False
         return await self.remove_current_user_group(request, group_obj.id)
 
@@ -564,16 +631,16 @@
         share1.permissions = [Permission.VIEWER]
         role.shares = [share1]
         return role
 
     async def __get_my_roles_json(self, request: Request) -> AsyncGenerator[dict[str, Any], None]:
         logger = logging.getLogger(__name__)
         sub = request.headers.get(SUB, NONE_USER)
-        access_token = await self.get_keycloak_access_token(request)
-
+        access_token_obj = await self.get_keycloak_access_token(request)
+        access_token = access_token_obj.id
         session = request.app[appproperty.HEA_CLIENT_SESSION]
 
         role_base_url = self._base_url / 'admin' / 'realms' / self.realm
         session_get = partial(session.get,
                             headers={'Authorization': f'Bearer {access_token}'},
                             verify_ssl=self.verify_ssl)
         roles = {}
@@ -596,15 +663,16 @@
         logger.debug('roles are %s', roles)
         for role_ in roles.values():
             yield role_
 
     async def __get_all_roles_json(self, request: Request) -> AsyncGenerator[dict[str, Any], None]:
         logger = logging.getLogger(__name__)
         sub = request.headers.get(SUB, NONE_USER)
-        access_token = await self.get_keycloak_access_token(request)
+        access_token_obj = await self.get_keycloak_access_token(request)
+        access_token = access_token_obj.id
 
         session = request.app[appproperty.HEA_CLIENT_SESSION]
 
         role_base_url = self._base_url / 'admin' / 'realms' / self.realm
         session_get = partial(session.get,
                             headers={'Authorization': f'Bearer {access_token}'},
                             verify_ssl=self.verify_ssl)
@@ -647,30 +715,32 @@
     async def __get_my_groups_json(self, request: Request) -> AsyncGenerator[dict[str, Any], None]:
         sub = request.headers.get(SUB, NONE_USER)
         async for group_dict in self.__get_user_groups_json(request, sub):
             yield group_dict
 
     async def __get_user_groups_json(self, request: Request, sub: str) -> AsyncGenerator[dict[str, Any], None]:
         logger = logging.getLogger(__name__)
-        access_token = await self.get_keycloak_access_token(request)
+        access_token_obj = await self.get_keycloak_access_token(request)
+        access_token = access_token_obj.id
 
         session = request.app[appproperty.HEA_CLIENT_SESSION]
 
         group_base_url = self._base_url / 'admin' / 'realms' / self.realm
         session_get = partial(session.get,
                             headers={'Authorization': f'Bearer {access_token}'},
                             verify_ssl=self.verify_ssl)
         async with session_get(group_base_url / 'users' / sub / 'groups') as response_:
             for group_dict in await response_.json():
                 logger.debug('Returning group %s', group_dict)
                 yield group_dict
 
     async def __get_all_groups_json(self, request: Request) -> AsyncGenerator[dict[str, Any], None]:
         logger = logging.getLogger(__name__)
-        access_token = await self.get_keycloak_access_token(request)
+        access_token_obj = await self.get_keycloak_access_token(request)
+        access_token = access_token_obj.id
 
         session = request.app[appproperty.HEA_CLIENT_SESSION]
 
         group_base_url = self._base_url / 'admin' / 'realms' / self.realm
         session_get = partial(session.get,
                             headers={'Authorization': f'Bearer {access_token}'},
                             verify_ssl=self.verify_ssl)
@@ -691,15 +761,17 @@
 
         :param request: the HTTP request (required).
         :param sub: the username (required).
         :param groups: the groups (required).
         :raises ValueError if an error occurred adding the roles due an internal server error.
         """
         logger = logging.getLogger(__name__)
-        access_token = await self.get_keycloak_access_token(request)
+        access_token_obj = await self.get_keycloak_access_token(request)
+        access_token = access_token_obj.id
+
         session = request.app[appproperty.HEA_CLIENT_SESSION]
 
         session_get = partial(session.get,
                                 headers={'Authorization': f'Bearer {access_token}'},
                                 verify_ssl=self.verify_ssl)
         role_base_url = self._base_url / 'admin' / 'realms' / self.realm
         for group in groups:
```

### Comparing `heaserver_people-1.3.1/src/heaserver/person/keycloakmongotestcase.py` & `heaserver_people-1.3.2/src/heaserver/person/keycloakmongotestcase.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from contextlib import ExitStack
 from typing import Generator
 
 import requests
 from aiohttp.web_request import Request
 from docker.errors import APIError
-from heaobject.person import Person
+from heaobject.person import Person, AccessToken
 from heaserver.service import appproperty
 from heaserver.service.db.database import MicroserviceDatabaseManager
 from heaserver.service.testcase.docker import start_other_container
 from heaserver.service.testcase.dockermongo import DockerMongoManager
 from heaserver.service.testcase.testenv import DockerContainerConfig, DockerVolumeMapping
 from heaserver.service.util import retry
 from yarl import URL
@@ -210,31 +210,51 @@
         return {
             'username': 'admin',
             'password': 'admin',
             'client_id': 'admin-cli',
             'grant_type': 'password'
         }
 
-    async def get_keycloak_access_token(self, request: Request) -> str:
+    async def get_keycloak_access_token(self, request: Request) -> AccessToken:
         """
         Request an access token from Keycloak.
 
         :param request: the HTTP request (required).
         :return: the access token or None if not found.
         """
         session = request.app[appproperty.HEA_CLIENT_SESSION]
         logger = logging.getLogger(__name__)
         logger.debug('Requesting new access token using credentials')
 
         async with session.post(self.token_url, data=self.token_body, verify_ssl=self.verify_ssl) as response_:
             content = await response_.json()
             logging.getLogger(__name__).debug(f'content {content}')
             access_token = content['access_token']
-        return access_token
+            access_token_obj = AccessToken()
+            access_token_obj.id = access_token
+        return access_token_obj
 
+    async def get_keycloak_alt_access_token(self,  request: Request) -> AccessToken:
+        """
+        Request an access token from Keycloak.
+
+        :param request: the HTTP request (required).
+        :return: the access token or None if not found.
+        """
+        session = request.app[appproperty.HEA_CLIENT_SESSION]
+        logger = logging.getLogger(__name__)
+        logger.debug('Requesting new access token using credentials')
+
+        async with session.post(self.token_url, data=self.token_body, verify_ssl=self.verify_ssl) as response_:
+            content = await response_.json()
+            logging.getLogger(__name__).debug(f'content {content}')
+            access_token = content['access_token']
+            access_token_obj = AccessToken()
+            access_token_obj.id = access_token
+        return access_token_obj
 
 class KeycloakMongoForPyTest(KeycloakMongoForTesting):
     async def get_users(self, request: Request, params: dict[str, str] | None = None) -> \
             list[Person]:
         users = await super().get_users(request, params)
         for user in users:
             match user.name:
```

### Comparing `heaserver_people-1.3.1/src/heaserver/person/service.py` & `heaserver_people-1.3.2/src/heaserver/person/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 from heaobject.person import Group
 from .keycloakmongo import KeycloakMongoManager
 from heaobject.user import NONE_USER
 from aiohttp import ClientResponseError
 from base64 import urlsafe_b64decode
 from binascii import Error as B64DecodeError
 
-
 MONGODB_PERSON_COLLECTION = 'people'
 
+
 @routes.get('/ping')
 async def ping(request: web.Request) -> web.Response:
     """
     For testing whether the service is up.
 
     :param request: the HTTP request.
     :return: Always returns status code 200.
@@ -212,22 +212,24 @@
                                       permissions=[role.get_permissions(sub) for role in roles])
     except ClientResponseError as e:
         if e.status == 404:
             return await response.get_all(request, [])
         else:
             return response.status_generic(e.status, body=e.message)
 
+
 @routes.get('/roles/{id}')
 @action(name='heaserver-people-role-get-properties', rel='hea-properties')
 @action(name='heaserver-people-role-get-self', rel='self', path='roles/{id}')
 async def get_role(request: web.Request) -> web.Response:
     """
-    Gets the requested role for the current user.
+    Gets the requested role.
 
-    :param request: the HTTP request.
+    :param request: the HTTP request. Requires an Authorization header with a valid Bearer token, in
+    addition to the usual OIDC_CLAIM_sub header.
     :return: all roles.
     ---
     summary: All roles.
     tags:
         - heaserver-people
     responses:
       '200':
@@ -248,15 +250,15 @@
         else:
             return response.status_generic(e.status, body=e.message)
 
 
 @routes.get('/roles/byname/{name}')
 async def get_role_by_name(request: web.Request) -> web.Response:
     """
-    Gets the requested role for the current user. Requires an Authorization header with a valid Bearer token, in
+    Gets the requested role. Requires an Authorization header with a valid Bearer token, in
     addition to the usual OIDC_CLAIM_sub header.
 
     :param request: the HTTP request.
     :return: all roles.
     ---
     summary: All roles.
     tags:
@@ -306,20 +308,22 @@
                                       permissions=[group.get_permissions(sub) for group in groups])
     except ClientResponseError as e:
         if e.status == 404:
             return await response.get_all(request, [])
         else:
             return response.status_generic(e.status, body=e.message)
 
+
 @routes.get('/groups/{id}')
 @action(name='heaserver-people-group-get-properties', rel='hea-properties')
 @action(name='heaserver-people-group-get-self', rel='self', path='groups/{id}')
 async def get_group(request: web.Request) -> web.Response:
     """
-    Gets the requested group for the current user.
+    Gets the requested group. Requires an Authorization header with a valid Bearer token, in
+    addition to the usual OIDC_CLAIM_sub header.
 
     :param request: the HTTP request.
     :return: all groups.
     ---
     summary: All groups.
     tags:
         - heaserver-people
@@ -341,15 +345,15 @@
             return response.status_not_found()
         else:
             return response.status_generic(e.status, body=e.message)
 
 @routes.get('/groups/byname/{name}')
 async def get_group_by_name(request: web.Request) -> web.Response:
     """
-    Gets the requested group for the current user. Requires an Authorization header with a valid Bearer token, in
+    Gets the requested group. Requires an Authorization header with a valid Bearer token, in
     addition to the usual OIDC_CLAIM_sub header.
 
     :param request: the HTTP request.
     :return: all groups.
     ---
     summary: All groups.
     tags:
@@ -437,13 +441,30 @@
     person_id = request.match_info['person_id']
     if person_id == 'me':
         result = await request.app[appproperty.HEA_DB].remove_current_user_group_by_group(request, group)
     else:
         result = await request.app[appproperty.HEA_DB].remove_user_group_by_group(request, person_id, group)
     return await response.delete(result)
 
+@routes.get('/people/internal/token')
+async def get_token(request: web.Request) -> web.Response:
+    logger = logging.getLogger(__name__)
+    try:
+        if logger.getEffectiveLevel() == logging.DEBUG:
+            logger.debug('headers %s', request.headers)
+        token = await request.app[appproperty.HEA_DB].get_keycloak_alt_access_token(request)
+    except ClientResponseError as e:
+        logger.exception('Got client response error')
+        if e.status == 404:
+            return response.status_not_found()
+        else:
+            return response.status_generic(e.status, body=e.message)
+    except B64DecodeError as e:
+        return response.status_not_found()
+    return await response.get(request, token.to_dict())
+
 def main() -> None:
     config = init_cmd_line(description='Read-only wrapper around Keycloak for accessing user information.',
                            default_port=8080)
     start(package_name='heaserver-people', db=KeycloakMongoManager, config=config, wstl_builder_factory=builder_factory(__package__))
```

### Comparing `heaserver_people-1.3.1/src/heaserver/person/testcasedata.py` & `heaserver_people-1.3.2/src/heaserver/person/testcasedata.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/src/heaserver/person/wstl/all.json` & `heaserver_people-1.3.2/src/heaserver/person/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/src/heaserver_people.egg-info/PKG-INFO` & `heaserver_people-1.3.2/src/heaserver_people.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-people
-Version: 1.3.1
+Version: 1.3.2
 Summary: A microservice designed to provide CRUD operations for the Person HEA object type
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-people,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.6.0
+Requires-Dist: heaserver~=1.6.2
 
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.3.2
+* Adds ability got get access tokens internally for microservices.
+
 ## Version 1.3.1
 * Prevent Volumes collection from appearing in the system menu.
 
 ## Version 1.3.0
 * Display type display name in properties card, and return it from GET calls.
 * Changed /groups and /roles to get all groups and roles.
 * New API for modifying a person's groups.
```

### Comparing `heaserver_people-1.3.1/tests/heaserver/persontest/permissionstestcase.py` & `heaserver_people-1.3.2/tests/heaserver/persontest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/tests/heaserver/persontest/test_all.py` & `heaserver_people-1.3.2/tests/heaserver/persontest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.3.1/tests/heaserver/persontest/testcase.py` & `heaserver_people-1.3.2/tests/heaserver/persontest/testcase.py`

 * *Files identical despite different names*

