# Comparing `tmp/rest_solace-0.2.3.tar.gz` & `tmp/rest_solace-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_solace-0.2.3.tar", last modified: Wed May 29 19:23:33 2024, max compression
+gzip compressed data, was "rest_solace-0.2.4.tar", last modified: Sat Jun  1 12:34:40 2024, max compression
```

## Comparing `rest_solace-0.2.3.tar` & `rest_solace-0.2.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.905680 rest_solace-0.2.3/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.2.3/.gitignore
--rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.2.3/LICENSE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1837 2024-05-29 19:20:47.000000 rest_solace-0.2.3/NOTICE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)    13505 2024-05-29 19:23:33.905680 rest_solace-0.2.3/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)    12568 2024-05-29 19:22:53.000000 rest_solace-0.2.3/README.rst
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.893680 rest_solace-0.2.3/docs/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      581 2024-05-22 06:25:58.000000 rest_solace-0.2.3/docs/development_refrences.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     3067 2024-05-29 16:57:51.000000 rest_solace-0.2.3/docs/getting_started_with_solace.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)      276 2024-05-10 17:58:06.000000 rest_solace-0.2.3/docs/index.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)    23870 2024-05-29 19:15:20.000000 rest_solace-0.2.3/docs/messaging_publisher.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4053 2024-05-29 18:08:44.000000 rest_solace-0.2.3/docs/semp_v2_endpoint_support.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2372 2024-05-29 19:20:12.000000 rest_solace-0.2.3/pyproject.toml
--rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-29 19:23:33.905680 rest_solace-0.2.3/setup.cfg
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.889680 rest_solace-0.2.3/src/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.893680 rest_solace-0.2.3/src/rest_solace/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.2.3/src/rest_solace/__init__.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.901680 rest_solace-0.2.3/src/rest_solace/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/action.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/consumer.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/http_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/manage.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/manager.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/publish.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/publisher.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5927 2024-05-19 16:38:53.000000 rest_solace-0.2.3/src/rest_solace/consumer.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.2.3/src/rest_solace/exceptions.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5439 2024-05-29 16:33:53.000000 rest_solace-0.2.3/src/rest_solace/http_client.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    31160 2024-05-19 19:46:54.000000 rest_solace-0.2.3/src/rest_solace/manager.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    36989 2024-05-29 18:54:46.000000 rest_solace-0.2.3/src/rest_solace/publisher.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.905680 rest_solace-0.2.3/src/rest_solace.egg-info/
--rw-r--r--   0 skyler    (1000) skyler    (1000)    13505 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1463 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/SOURCES.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/dependency_links.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       32 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/requires.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/top_level.txt
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.905680 rest_solace-0.2.3/tests/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.905680 rest_solace-0.2.3/tests/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.2.3/tests/__pycache__/manager_unittest.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.2.3/tests/consumer_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.2.3/tests/empty_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.2.3/tests/manager_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2835 2024-05-19 15:56:09.000000 rest_solace-0.2.3/tests/pub_sub_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7776 2024-05-26 20:05:55.000000 rest_solace-0.2.3/tests/publisher_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      422 2024-05-26 20:03:38.000000 rest_solace-0.2.3/tests/test_data.json
--rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.2.3/tests/util.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-06-01 12:34:40.432939 rest_solace-0.2.4/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.2.4/.gitignore
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.2.4/LICENSE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1837 2024-05-29 19:20:47.000000 rest_solace-0.2.4/NOTICE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    13505 2024-06-01 12:34:40.428939 rest_solace-0.2.4/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    12568 2024-05-29 19:22:53.000000 rest_solace-0.2.4/README.rst
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-06-01 12:34:40.408939 rest_solace-0.2.4/docs/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      581 2024-05-22 06:25:58.000000 rest_solace-0.2.4/docs/development_refrences.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     3067 2024-05-29 16:57:51.000000 rest_solace-0.2.4/docs/getting_started_with_solace.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      366 2024-05-29 19:28:03.000000 rest_solace-0.2.4/docs/index.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    23870 2024-05-29 19:15:20.000000 rest_solace-0.2.4/docs/messaging_publisher.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4053 2024-06-01 12:02:34.000000 rest_solace-0.2.4/docs/semp_v2_endpoint_support.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2372 2024-06-01 12:19:06.000000 rest_solace-0.2.4/pyproject.toml
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-06-01 12:34:40.432939 rest_solace-0.2.4/setup.cfg
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-06-01 12:34:40.404939 rest_solace-0.2.4/src/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-06-01 12:34:40.416939 rest_solace-0.2.4/src/rest_solace/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.2.4/src/rest_solace/__init__.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-06-01 12:34:40.424939 rest_solace-0.2.4/src/rest_solace/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/action.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/consumer.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/http_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/manage.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/publish.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/publisher.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.2.4/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5927 2024-05-19 16:38:53.000000 rest_solace-0.2.4/src/rest_solace/consumer.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.2.4/src/rest_solace/exceptions.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5439 2024-05-29 16:33:53.000000 rest_solace-0.2.4/src/rest_solace/http_client.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    31630 2024-06-01 12:30:21.000000 rest_solace-0.2.4/src/rest_solace/manager.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    36989 2024-06-01 12:02:34.000000 rest_solace-0.2.4/src/rest_solace/publisher.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-06-01 12:34:40.428939 rest_solace-0.2.4/src/rest_solace.egg-info/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    13505 2024-06-01 12:34:40.000000 rest_solace-0.2.4/src/rest_solace.egg-info/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1463 2024-06-01 12:34:40.000000 rest_solace-0.2.4/src/rest_solace.egg-info/SOURCES.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-06-01 12:34:40.000000 rest_solace-0.2.4/src/rest_solace.egg-info/dependency_links.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       32 2024-06-01 12:34:40.000000 rest_solace-0.2.4/src/rest_solace.egg-info/requires.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-06-01 12:34:40.000000 rest_solace-0.2.4/src/rest_solace.egg-info/top_level.txt
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-06-01 12:34:40.428939 rest_solace-0.2.4/tests/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-06-01 12:34:40.428939 rest_solace-0.2.4/tests/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.2.4/tests/__pycache__/manager_unittest.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.2.4/tests/consumer_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.2.4/tests/empty_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.2.4/tests/manager_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2835 2024-05-19 15:56:09.000000 rest_solace-0.2.4/tests/pub_sub_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7776 2024-05-26 20:05:55.000000 rest_solace-0.2.4/tests/publisher_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      422 2024-05-26 20:03:38.000000 rest_solace-0.2.4/tests/test_data.json
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.2.4/tests/util.py
```

### Comparing `rest_solace-0.2.3/LICENSE.txt` & `rest_solace-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/NOTICE.txt` & `rest_solace-0.2.4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/PKG-INFO` & `rest_solace-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-solace
-Version: 0.2.3
+Version: 0.2.4
 Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
 Author-email: Skyler Guha <skylerguha@gmail.com>
 Maintainer-email: Skyler Guha <skylerguha@gmail.com>
 License: apache 2.0
 Project-URL: pypi, https://pypi.org/project/rest-solace/
 Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
 Project-URL: repository, https://github.com/skyler-guha/rest-solace
```

### Comparing `rest_solace-0.2.3/README.rst` & `rest_solace-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/docs/development_refrences.rst` & `rest_solace-0.2.4/docs/development_refrences.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/docs/getting_started_with_solace.rst` & `rest_solace-0.2.4/docs/getting_started_with_solace.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/docs/messaging_publisher.rst` & `rest_solace-0.2.4/docs/messaging_publisher.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/docs/semp_v2_endpoint_support.rst` & `rest_solace-0.2.4/docs/semp_v2_endpoint_support.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/pyproject.toml` & `rest_solace-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     #"time"             #part of the standard library
     #"json",            #part of the standard library
     #"urllib"           #part of the standard library
     #"asyncio"          #part of the standard library
     #"logging"          #part of the standard library
     #"warnings"         #part of the standard library
 ]
-version = "0.2.3"
+version = "0.2.4"
 
 [project.urls]
 pypi = "https://pypi.org/project/rest-solace/"
 documentation = "https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst"
 repository = "https://github.com/skyler-guha/rest-solace"
 
 #Doing an editable install: pip install --editable .
```

### Comparing `rest_solace-0.2.3/src/rest_solace/__init__.py` & `rest_solace-0.2.4/src/rest_solace/__init__.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/action.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/action.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/config.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/consumer.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/consumer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/http_client.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/http_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/manage.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/manage.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/manager.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/publish.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/publish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/publisher.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/publisher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/semp_client.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/semp_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/__pycache__/subscriber.cpython-311.pyc` & `rest_solace-0.2.4/src/rest_solace/__pycache__/subscriber.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/consumer.py` & `rest_solace-0.2.4/src/rest_solace/consumer.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/http_client.py` & `rest_solace-0.2.4/src/rest_solace/http_client.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace/manager.py` & `rest_solace-0.2.4/src/rest_solace/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .http_client import HttpClient
 from urllib.parse import urlsplit, urlunsplit
+import warnings
+from warnings import *
 
 class Manager():
     
     def __init__(self, user_name:str, password:str,
                  host:str, semp_port:str= "8080", verify_ssl=False) -> None:
         """Class for creating a Manage object for communicating with a broker regarding management stuff.
 
@@ -594,14 +596,20 @@
             remoteHost (str): IPv4 address at which your consumer is running at.
             remotePort (int): The port that your consumer uses to listen for incoming messages.
             postRequestTarget (str): The rest endpoint on the consumer side that will be targeted when sending the message.
             clientProfileName (str, optional): Client Profiles are used to assign common configuration properties to clients that have been successfully authorized. Defaults to 'default'.
             clientUsername (str, optional): A client is only authorized to connect to a Message VPN that is associated with a Client Username that the client has been assigned.
         """
 
+        message = "This function is in development phase and will be fully working in rest-solace version 0.3."+ \
+        " The current version of this function will be incompatible with the one in the future release."+ \
+        "The clientProfileName parameter will likely be removed and will be taken from the client details from solace."
+        warnings.warn(message= message,
+                      category= FutureWarning)
+
         #step0
         self.update_client_profile(msgVpnName= msgVpnName, clientProfileName= clientProfileName)
         self.update_client_username(msgVpnName= msgVpnName, clientUsername= clientUsername)
 
         #step1
         self.create_queue_endpoint(queueName=queueName, msgVpnName=msgVpnName, throw_exception= False)
```

### Comparing `rest_solace-0.2.3/src/rest_solace/publisher.py` & `rest_solace-0.2.4/src/rest_solace/publisher.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/src/rest_solace.egg-info/PKG-INFO` & `rest_solace-0.2.4/src/rest_solace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-solace
-Version: 0.2.3
+Version: 0.2.4
 Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
 Author-email: Skyler Guha <skylerguha@gmail.com>
 Maintainer-email: Skyler Guha <skylerguha@gmail.com>
 License: apache 2.0
 Project-URL: pypi, https://pypi.org/project/rest-solace/
 Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
 Project-URL: repository, https://github.com/skyler-guha/rest-solace
```

### Comparing `rest_solace-0.2.3/src/rest_solace.egg-info/SOURCES.txt` & `rest_solace-0.2.4/src/rest_solace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/tests/__pycache__/manager_unittest.cpython-311.pyc` & `rest_solace-0.2.4/tests/__pycache__/manager_unittest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/tests/consumer_test.py` & `rest_solace-0.2.4/tests/consumer_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/tests/empty_test.py` & `rest_solace-0.2.4/tests/empty_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/tests/manager_test.py` & `rest_solace-0.2.4/tests/manager_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/tests/pub_sub_test.py` & `rest_solace-0.2.4/tests/pub_sub_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/tests/publisher_test.py` & `rest_solace-0.2.4/tests/publisher_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.3/tests/util.py` & `rest_solace-0.2.4/tests/util.py`

 * *Files identical despite different names*

