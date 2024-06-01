# Comparing `tmp/heaserver_keychain-1.3.0.tar.gz` & `tmp/heaserver_keychain-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_keychain-1.3.0.tar", last modified: Wed May 22 00:05:37 2024, max compression
+gzip compressed data, was "heaserver_keychain-1.3.1.tar", last modified: Sat Jun  1 14:16:18 2024, max compression
```

## Comparing `heaserver_keychain-1.3.0.tar` & `heaserver_keychain-1.3.1.tar`

### file list

```diff
@@ -1,54 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.707608 heaserver_keychain-1.3.0/
--rw-rw-rw-   0        0        0      325 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/.gitignore
--rw-rw-rw-   0        0        0     1579 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5416 2024-05-22 00:05:37.706608 heaserver_keychain-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4090 2024-05-22 00:04:34.000000 heaserver_keychain-1.3.0/README.md
--rw-rw-rw-   0        0        0     2654 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/RELEASING.md
--rw-rw-rw-   0        0        0      588 2024-03-21 23:50:19.000000 heaserver_keychain-1.3.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.427909 heaserver_keychain-1.3.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.427909 heaserver_keychain-1.3.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.559549 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.578360 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752
--rw-rw-rw-   0        0        0     4195 2024-05-17 22:48:39.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     6736 2024-05-17 23:10:18.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      109 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/requirements_dev.txt
--rw-rw-rw-   0        0        0     1048 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-22 00:05:37.707608 heaserver_keychain-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1830 2024-05-22 00:04:56.000000 heaserver_keychain-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.431077 heaserver_keychain-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.430029 heaserver_keychain-1.3.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.592906 heaserver_keychain-1.3.0/src/heaserver/keychain/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/src/heaserver/keychain/__init__.py
--rw-rw-rw-   0        0        0    17020 2024-03-21 23:50:19.000000 heaserver_keychain-1.3.0/src/heaserver/keychain/service.py
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.604575 heaserver_keychain-1.3.0/src/heaserver/keychain/wstl/
--rw-rw-rw-   0        0        0    18063 2024-05-21 23:29:36.000000 heaserver_keychain-1.3.0/src/heaserver/keychain/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.703225 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/
--rw-rw-rw-   0        0        0     5416 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.432131 heaserver_keychain-1.3.0/tests/
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.432729 heaserver_keychain-1.3.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.677196 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.703199 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848
--rw-rw-rw-   0        0        0     2205 2024-01-04 18:07:50.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296
--rw-rw-rw-   0        0        0     3828 2024-05-17 22:49:36.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/test_all.py
--rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     6604 2024-05-17 22:49:23.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.347507 heaserver_keychain-1.3.1/
+-rw-rw-rw-   0        0        0      325 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/.gitignore
+-rw-rw-rw-   0        0        0     1579 2024-06-01 14:02:42.000000 heaserver_keychain-1.3.1/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5525 2024-06-01 14:16:18.346506 heaserver_keychain-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4199 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/README.md
+-rw-rw-rw-   0        0        0     2654 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/RELEASING.md
+-rw-rw-rw-   0        0        0      588 2024-06-01 14:02:42.000000 heaserver_keychain-1.3.1/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.219910 heaserver_keychain-1.3.1/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.219910 heaserver_keychain-1.3.1/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.289512 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4195 2024-05-22 20:33:47.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     7770 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      109 2024-06-01 13:52:52.000000 heaserver_keychain-1.3.1/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0     1167 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 14:16:18.347507 heaserver_keychain-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-06-01 14:14:19.000000 heaserver_keychain-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.220925 heaserver_keychain-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.220925 heaserver_keychain-1.3.1/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.297512 heaserver_keychain-1.3.1/src/heaserver/keychain/
+-rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/src/heaserver/keychain/__init__.py
+-rw-rw-rw-   0        0        0    40816 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/src/heaserver/keychain/service.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.303512 heaserver_keychain-1.3.1/src/heaserver/keychain/wstl/
+-rw-rw-rw-   0        0        0    19645 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/src/heaserver/keychain/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.344506 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/
+-rw-rw-rw-   0        0        0     5525 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1111 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.221918 heaserver_keychain-1.3.1/tests/
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.221918 heaserver_keychain-1.3.1/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.342522 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/
+-rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/__init__.py
+-rw-rw-rw-   0        0        0     3828 2024-05-22 20:33:47.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     7582 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/testcase.py
```

### Comparing `heaserver_keychain-1.3.0/Dockerfile` & `heaserver_keychain-1.3.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.0/LICENSE` & `heaserver_keychain-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.0/PKG-INFO` & `heaserver_keychain-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.3.0
+Version: 1.3.1
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,21 +21,23 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.6.0
+Requires-Dist: heaserver~=1.6.2
 
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
+## Version 1.3.1
+* Introduces Managed Credentials with ability create and specify life span of credential 
 
 ## Version 1.3.0
 * Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
 
 ## Version 1.2.0
 * Display type display name in properties card.
```

### Comparing `heaserver_keychain-1.3.0/README.md` & `heaserver_keychain-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
+## Version 1.3.1
+* Introduces Managed Credentials with ability create and specify life span of credential 
 
 ## Version 1.3.0
 * Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
 
 ## Version 1.2.0
 * Display type display name in properties card.
```

### Comparing `heaserver_keychain-1.3.0/RELEASING.md` & `heaserver_keychain-1.3.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.0/docker-entrypoint.sh` & `heaserver_keychain-1.3.1/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py` & `heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py` & `heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/testcase.py` & `heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/testcase.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,19 @@
                                                   #        rel=['hea-context-menu', 'hea-dynamic-standard', 'hea-icon-duplicator']),
                                                   Action(name='heaserver-keychain-credentials-get-self',
                                                              url='http://localhost:8080/credentials/{id}',
                                                              rel=['self']),
                                                   Action(name='heaserver-keychain-awscredentials-get-cli-credentials-file',
                                                              url='http://localhost:8080/credentials/{id}/awsclicredentialsfile',
                                                              rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
-                                                             itemif='type=="heaobject.keychain.AWSCredentials"')
+                                                             itemif='type=="heaobject.keychain.AWSCredentials"'),
+                                                  Action(name='heaserver-keychain-get-create-awscredential',
+                                                         url='http://localhost:8080/credentials/{id}/managedawscredential',
+                                                         rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
+                                                         itemif='type=="heaobject.keychain.AWSCredentials"')
                                                   ],
                                      get_all_actions=[Action(name='heaserver-keychain-credentials-get-properties',
                                                              rel=['hea-context-menu', 'hea-properties'],
                                                              itemif='type=="heaobject.keychain.Credentials"'),
                                                       Action(name='heaserver-keychain-awscredentials-get-properties',
                                                              rel=['hea-context-menu', 'hea-properties'],
                                                              itemif='type=="heaobject.keychain.AWSCredentials"'),
@@ -91,10 +95,15 @@
                                                       #        rel=['hea-context-menu', 'hea-dynamic-standard', 'hea-icon-duplicator']),
                                                       Action(name='heaserver-keychain-credentials-get-self',
                                                              url='http://localhost:8080/credentials/{id}',
                                                              rel=['self']),
                                                       Action(name='heaserver-keychain-awscredentials-get-cli-credentials-file',
                                                              url='http://localhost:8080/credentials/{id}/awsclicredentialsfile',
                                                              rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
-                                                             itemif='type=="heaobject.keychain.AWSCredentials"')],
+                                                             itemif='type=="heaobject.keychain.AWSCredentials"'),
+                                                      Action(name='heaserver-keychain-get-create-awscredential',
+                                                             url='http://localhost:8080/credentials/{id}/managedawscredential',
+                                                             rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
+                                                             itemif='type=="heaobject.keychain.AWSCredentials"')
+                                                      ],
                                      #duplicate_action_name='heaserver-keychain-credentials-duplicate-form'
                                      )
```

### Comparing `heaserver_keychain-1.3.0/run-swaggerui.py` & `heaserver_keychain-1.3.1/run-swaggerui.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 if __name__ == '__main__':
     swaggerui.run(project_slug='heaserver-keychain', desktop_objects=db_store,
                   wstl_builder_factory=builder_factory(service.__package__),
                   routes=[(get, '/credentials/{id}', service.get_credentials),
                           (get, '/credentials/byname/{name}', service.get_credentials_by_name),
                           (get, '/credentials/', service.get_all_credentials),
                           (post, '/credentials/', service.post_credentials),
+                          (post, '/credentials/{id}/managedawscredential', service.post_create_aws_credentials_form),
                           (put, '/credentials/{id}', service.put_credentials),
                           (delete, '/credentials/{id}', service.delete_credentials)])
```

### Comparing `heaserver_keychain-1.3.0/setup.py` & `heaserver_keychain-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-keychain',
-    version='1.3.0',
+    version='1.3.1',
     description="a service for managing laboratory credentials",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.keychain'],
     package_data={'heaserver.keychain': ['wstl/*.json']},
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

### Comparing `heaserver_keychain-1.3.0/src/heaserver/keychain/wstl/all.json` & `heaserver_keychain-1.3.1/src/heaserver/keychain/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9651785714285714%*

 * *Differences: {"'wstl'": '{\'actions\': {4: {\'description\': "Retrieve credentials file to copy and paste into '*

 * *           'your home directory\'s .aws directory", \'type\': \'unsafe\', \'action\': \'update\', '*

 * *           '\'prompt\': \'Retrieve\'}, 5: {\'description\': "Retrieve credentials file to copy and '*

 * *           'paste into your home directory\'s .aws directory", \'prompt\': \'Retrieve\'}, 7: '*

 * *           "{'type': 'safe', 'action': 'read'}, 9: {'type': 'unsafe', 'action': 'update'}, insert: "*

 * *           "[(2 […]*

```diff
@@ -13,27 +13,76 @@
                 "description": "Open this credential",
                 "name": "heaserver-keychain-credentials-open-choices",
                 "prompt": "Open",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
+                "action": "update",
+                "description": "Create a new aws credential",
+                "name": "heaserver-keychain-get-create-awscredential",
+                "prompt": "New",
+                "target": "item read cj",
+                "type": "unsafe"
+            },
+            {
                 "action": "read",
-                "description": "Generate credentials file to copy and paste into your home directory's .aws directory",
+                "description": "Create a new aws credential",
+                "inputs": [
+                    {
+                        "name": "key_lifespan",
+                        "prompt": "Key Duration",
+                        "required": true,
+                        "suggest": [
+                            {
+                                "text": "24 hours",
+                                "value": "24"
+                            },
+                            {
+                                "text": "48 hours",
+                                "value": "48"
+                            },
+                            {
+                                "text": "72 hours",
+                                "value": "72"
+                            }
+                        ],
+                        "type": "select",
+                        "value": "24"
+                    },
+                    {
+                        "hea": {
+                            "display": false
+                        },
+                        "name": "type",
+                        "prompt": "Type",
+                        "readOnly": true,
+                        "required": true,
+                        "value": "heaobject.keychain.AWSCredentials"
+                    }
+                ],
+                "name": "heaserver-keychain-get-create-awscredential-form",
+                "prompt": "New",
+                "target": "item cj-template",
+                "type": "safe"
+            },
+            {
+                "action": "update",
+                "description": "Retrieve credentials file to copy and paste into your home directory's .aws directory",
                 "name": "heaserver-keychain-awscredentials-get-cli-credentials-file",
-                "prompt": "Generate credentials file",
+                "prompt": "Retrieve",
                 "target": "item read cj",
-                "type": "safe"
+                "type": "unsafe"
             },
             {
                 "action": "read",
-                "description": "Generate credentials file to copy and paste into your home directory's .aws directory",
+                "description": "Retrieve credentials file to copy and paste into your home directory's .aws directory",
                 "inputs": [],
                 "name": "heaserver-keychain-awscredentials-get-cli-credentials-file-form",
-                "prompt": "Generate credentials file",
+                "prompt": "Retrieve",
                 "target": "item cj-template",
                 "type": "safe"
             },
             {
                 "action": "update",
                 "description": "View and edit these credentials' properties",
                 "inputs": [
@@ -178,15 +227,15 @@
                 ],
                 "name": "heaserver-keychain-credentials-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
             {
-                "action": "update",
+                "action": "read",
                 "description": "View and edit these AWS credentials' properties",
                 "inputs": [
                     {
                         "hea": {
                             "display": false
                         },
                         "name": "id",
@@ -451,15 +500,15 @@
                         ],
                         "type": "select"
                     }
                 ],
                 "name": "heaserver-keychain-awscredentials-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
-                "type": "unsafe"
+                "type": "safe"
             },
             {
                 "action": "update",
                 "description": "Duplicate these credentials",
                 "inputs": [
                     {
                         "name": "display_name",
@@ -537,18 +586,18 @@
                 ],
                 "name": "heaserver-keychain-credentials-duplicate-form",
                 "prompt": "Duplicate",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
             {
-                "action": "read",
+                "action": "update",
                 "description": "View these credentials",
                 "name": "heaserver-keychain-credentials-get-self",
                 "prompt": "View",
                 "target": "item read cj",
-                "type": "safe"
+                "type": "unsafe"
             }
         ],
         "title": "HEA Keychain"
     }
 }
```

### Comparing `heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/PKG-INFO` & `heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.3.0
+Version: 1.3.1
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,21 +21,23 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.6.0
+Requires-Dist: heaserver~=1.6.2
 
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
+## Version 1.3.1
+* Introduces Managed Credentials with ability create and specify life span of credential 
 
 ## Version 1.3.0
 * Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
 
 ## Version 1.2.0
 * Display type display name in properties card.
```

### Comparing `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/permissionstestcase.py` & `heaserver_keychain-1.3.1/tests/heaserver/keychaintest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/test_all_with_bad_permissions.py` & `heaserver_keychain-1.3.1/tests/heaserver/keychaintest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/testcase.py` & `heaserver_keychain-1.3.1/tests/heaserver/keychaintest/testcase.py`

 * *Files 15% similar despite different names*

```diff
@@ -71,15 +71,19 @@
                                                   #            rel=['hea-context-menu', 'hea-dynamic-standard', 'hea-icon-duplicator']),
                                                   Action(name='heaserver-keychain-credentials-get-self',
                                                              url='http://localhost:8080/credentials/{id}',
                                                              rel=['self']),
                                                   Action(name='heaserver-keychain-awscredentials-get-cli-credentials-file',
                                                              url='http://localhost:8080/credentials/{id}/awsclicredentialsfile',
                                                              rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
-                                                             itemif='type=="heaobject.keychain.AWSCredentials"')
+                                                             itemif='type=="heaobject.keychain.AWSCredentials"'),
+                                                  Action(name='heaserver-keychain-get-create-awscredential',
+                                                         url='http://localhost:8080/credentials/{id}/managedawscredential',
+                                                         rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
+                                                         itemif='type=="heaobject.keychain.AWSCredentials"')
                                                   ],
                                      get_all_actions=[Action(name='heaserver-keychain-credentials-get-properties',
                                                              rel=['hea-context-menu', 'hea-properties'],
                                                              itemif='type=="heaobject.keychain.Credentials"'),
                                                       Action(name='heaserver-keychain-awscredentials-get-properties',
                                                              rel=['hea-context-menu', 'hea-properties'],
                                                              itemif='type=="heaobject.keychain.AWSCredentials"'),
@@ -91,10 +95,14 @@
                                                       #            rel=['hea-context-menu', 'hea-dynamic-standard', 'hea-icon-duplicator']),
                                                       Action(name='heaserver-keychain-credentials-get-self',
                                                                  url='http://localhost:8080/credentials/{id}',
                                                                  rel=['self']),
                                                       Action(name='heaserver-keychain-awscredentials-get-cli-credentials-file',
                                                              url='http://localhost:8080/credentials/{id}/awsclicredentialsfile',
                                                              rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
+                                                             itemif='type=="heaobject.keychain.AWSCredentials"'),
+                                                      Action(name='heaserver-keychain-get-create-awscredential',
+                                                             url='http://localhost:8080/credentials/{id}/managedawscredential',
+                                                             rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
                                                              itemif='type=="heaobject.keychain.AWSCredentials"')],
                                      #duplicate_action_name='heaserver-keychain-credentials-duplicate-form'
                                      )
```

