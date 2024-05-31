# Comparing `tmp/pyhamtools-0.9.0.tar.gz` & `tmp/pyhamtools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyhamtools-0.9.0.tar", last modified: Thu Dec 28 20:07:01 2023, max compression
+gzip compressed data, was "pyhamtools-0.9.1.tar", last modified: Sun Mar 17 22:12:53 2024, max compression
```

## Comparing `pyhamtools-0.9.0.tar` & `pyhamtools-0.9.1.tar`

### file list

```diff
@@ -1,36 +1,45 @@
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-12-28 20:07:01.000000 pyhamtools-0.9.0/
--rw-r--r--   0 tobias     (501) staff       (20)      275 2023-12-28 20:07:01.000000 pyhamtools-0.9.0/PKG-INFO
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-12-28 20:07:01.000000 pyhamtools-0.9.0/test/
--rw-r--r--   0 tobias     (501) staff       (20)    16013 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_callinfo.py
--rw-r--r--   0 tobias     (501) staff       (20)     1201 2018-01-27 18:01:52.000000 pyhamtools-0.9.0/test/test_locator_latlong_to_locator.py
--rw-r--r--   0 tobias     (501) staff       (20)     2926 2022-12-31 01:30:20.000000 pyhamtools-0.9.0/test/test_lookuplib_countryfile.py
--rw-r--r--   0 tobias     (501) staff       (20)      856 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_clublog.py
--rw-r--r--   0 tobias     (501) staff       (20)     3445 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_lookuplib_clublogapi.py
--rw-r--r--   0 tobias     (501) staff       (20)     2095 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_lookuplib_redis.py
--rw-r--r--   0 tobias     (501) staff       (20)     1585 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_lotw.py
--rw-r--r--   0 tobias     (501) staff       (20)     3027 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_locator_sunrise_sunset.py
--rw-r--r--   0 tobias     (501) staff       (20)     4438 2021-12-15 23:07:09.000000 pyhamtools-0.9.0/test/test_utils_freq_to_band.py
--rw-r--r--   0 tobias     (501) staff       (20)     1184 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_lookuplib.py
--rw-r--r--   0 tobias     (501) staff       (20)     1020 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_eqsl.py
--rw-r--r--   0 tobias     (501) staff       (20)     9285 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_lookuplib_clublogxml.py
--rw-r--r--   0 tobias     (501) staff       (20)     4134 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_lookuplib_qrz.py
--rw-r--r--   0 tobias     (501) staff       (20)     1993 2018-01-27 18:01:54.000000 pyhamtools-0.9.0/test/test_locator_locator_to_latlong.py
--rw-r--r--   0 tobias     (501) staff       (20)     3426 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_dxcluster.py
--rw-r--r--   0 tobias     (501) staff       (20)     7599 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/test/test_lookuplib_gettersetter_api.py
--rw-r--r--   0 tobias     (501) staff       (20)     2402 2018-01-27 18:01:56.000000 pyhamtools-0.9.0/test/test_locator_distances.py
-drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-12-28 20:07:01.000000 pyhamtools-0.9.0/pyhamtools/
--rw-r--r--   0 tobias     (501) staff       (20)     6921 2018-05-20 18:04:58.000000 pyhamtools-0.9.0/pyhamtools/frequency.py
--rw-r--r--   0 tobias     (501) staff       (20)     6524 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/pyhamtools/qsl.py
--rw-r--r--   0 tobias     (501) staff       (20)      153 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/pyhamtools/version.py
--rw-r--r--   0 tobias     (501) staff       (20)    60807 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/pyhamtools/lookuplib.py
--rw-r--r--   0 tobias     (501) staff       (20)     1134 2022-12-03 22:08:09.000000 pyhamtools-0.9.0/pyhamtools/logparser.py
--rw-r--r--   0 tobias     (501) staff       (20)     7886 2022-12-31 01:21:08.000000 pyhamtools-0.9.0/pyhamtools/countryfilemapping.json
--rw-r--r--   0 tobias     (501) staff       (20)    18027 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/pyhamtools/callinfo.py
--rw-r--r--   0 tobias     (501) staff       (20)     2387 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/pyhamtools/dxcluster.py
--rw-r--r--   0 tobias     (501) staff       (20)      163 2018-01-27 18:02:27.000000 pyhamtools-0.9.0/pyhamtools/callsign_exceptions.py
--rw-r--r--   0 tobias     (501) staff       (20)       85 2018-01-27 18:02:21.000000 pyhamtools-0.9.0/pyhamtools/__init__.py
--rw-r--r--   0 tobias     (501) staff       (20)    10899 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/pyhamtools/locator.py
--rw-r--r--   0 tobias     (501) staff       (20)     2368 2018-05-20 18:09:54.000000 pyhamtools-0.9.0/pyhamtools/consts.py
--rw-r--r--   0 tobias     (501) staff       (20)     5013 2018-05-20 16:40:49.000000 pyhamtools-0.9.0/pyhamtools/utils.py
--rw-r--r--   0 tobias     (501) staff       (20)      128 2018-01-27 18:02:34.000000 pyhamtools-0.9.0/pyhamtools/exceptions.py
--rwxr-xr-x   0 tobias     (501) staff       (20)      662 2023-12-28 20:02:12.000000 pyhamtools-0.9.0/setup.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2024-03-17 22:12:53.916597 pyhamtools-0.9.1/
+-rw-r--r--   0 tobias     (501) staff       (20)     1081 2014-04-24 12:12:35.000000 pyhamtools-0.9.1/LICENSE
+-rw-r--r--   0 tobias     (501) staff       (20)      275 2024-03-17 22:12:53.916481 pyhamtools-0.9.1/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     5167 2024-01-03 21:09:05.000000 pyhamtools-0.9.1/README.md
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2024-03-17 22:12:53.911659 pyhamtools-0.9.1/pyhamtools/
+-rw-r--r--   0 tobias     (501) staff       (20)       85 2018-01-27 18:02:21.000000 pyhamtools-0.9.1/pyhamtools/__init__.py
+-rw-r--r--   0 tobias     (501) staff       (20)    18027 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/pyhamtools/callinfo.py
+-rw-r--r--   0 tobias     (501) staff       (20)      163 2018-01-27 18:02:27.000000 pyhamtools-0.9.1/pyhamtools/callsign_exceptions.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2368 2018-05-20 18:09:54.000000 pyhamtools-0.9.1/pyhamtools/consts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7886 2022-12-31 01:21:08.000000 pyhamtools-0.9.1/pyhamtools/countryfilemapping.json
+-rw-r--r--   0 tobias     (501) staff       (20)     2387 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/pyhamtools/dxcluster.py
+-rw-r--r--   0 tobias     (501) staff       (20)      128 2018-01-27 18:02:34.000000 pyhamtools-0.9.1/pyhamtools/exceptions.py
+-rw-r--r--   0 tobias     (501) staff       (20)     6921 2018-05-20 18:04:58.000000 pyhamtools-0.9.1/pyhamtools/frequency.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10899 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/pyhamtools/locator.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1134 2022-12-03 22:08:09.000000 pyhamtools-0.9.1/pyhamtools/logparser.py
+-rw-r--r--   0 tobias     (501) staff       (20)    60807 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/pyhamtools/lookuplib.py
+-rw-r--r--   0 tobias     (501) staff       (20)     6524 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/pyhamtools/qsl.py
+-rw-r--r--   0 tobias     (501) staff       (20)     5013 2018-05-20 16:40:49.000000 pyhamtools-0.9.1/pyhamtools/utils.py
+-rw-r--r--   0 tobias     (501) staff       (20)      153 2024-03-17 22:05:21.000000 pyhamtools-0.9.1/pyhamtools/version.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2024-03-17 22:12:53.912225 pyhamtools-0.9.1/pyhamtools.egg-info/
+-rw-r--r--   0 tobias     (501) staff       (20)      275 2024-03-17 22:12:53.000000 pyhamtools-0.9.1/pyhamtools.egg-info/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     1037 2024-03-17 22:12:53.000000 pyhamtools-0.9.1/pyhamtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        1 2024-03-17 22:12:53.000000 pyhamtools-0.9.1/pyhamtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias     (501) staff       (20)       85 2024-03-17 22:12:53.000000 pyhamtools-0.9.1/pyhamtools.egg-info/requires.txt
+-rw-r--r--   0 tobias     (501) staff       (20)       11 2024-03-17 22:12:53.000000 pyhamtools-0.9.1/pyhamtools.egg-info/top_level.txt
+-rw-r--r--   0 tobias     (501) staff       (20)       38 2024-03-17 22:12:53.916640 pyhamtools-0.9.1/setup.cfg
+-rwxr-xr-x   0 tobias     (501) staff       (20)      665 2024-03-17 22:05:04.000000 pyhamtools-0.9.1/setup.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2024-03-17 22:12:53.916134 pyhamtools-0.9.1/test/
+-rw-r--r--   0 tobias     (501) staff       (20)    16013 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_callinfo.py
+-rw-r--r--   0 tobias     (501) staff       (20)      856 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_clublog.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3426 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_dxcluster.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1020 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_eqsl.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2402 2018-01-27 18:01:56.000000 pyhamtools-0.9.1/test/test_locator_distances.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1201 2018-01-27 18:01:52.000000 pyhamtools-0.9.1/test/test_locator_latlong_to_locator.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1993 2018-01-27 18:01:54.000000 pyhamtools-0.9.1/test/test_locator_locator_to_latlong.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3027 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_locator_sunrise_sunset.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1184 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_lookuplib.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3445 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_lookuplib_clublogapi.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9285 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_lookuplib_clublogxml.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2926 2022-12-31 01:30:20.000000 pyhamtools-0.9.1/test/test_lookuplib_countryfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7599 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_lookuplib_gettersetter_api.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4134 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_lookuplib_qrz.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2095 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_lookuplib_redis.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1585 2023-12-28 20:02:12.000000 pyhamtools-0.9.1/test/test_lotw.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4438 2021-12-15 23:07:09.000000 pyhamtools-0.9.1/test/test_utils_freq_to_band.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyhamtools-0.9.0/test/test_callinfo.py` & `pyhamtools-0.9.1/test/test_callinfo.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_locator_latlong_to_locator.py` & `pyhamtools-0.9.1/test/test_locator_latlong_to_locator.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_lookuplib_countryfile.py` & `pyhamtools-0.9.1/test/test_lookuplib_countryfile.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_clublog.py` & `pyhamtools-0.9.1/test/test_clublog.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_lookuplib_clublogapi.py` & `pyhamtools-0.9.1/test/test_lookuplib_clublogapi.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_lookuplib_redis.py` & `pyhamtools-0.9.1/test/test_lookuplib_redis.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_lotw.py` & `pyhamtools-0.9.1/test/test_lotw.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_locator_sunrise_sunset.py` & `pyhamtools-0.9.1/test/test_locator_sunrise_sunset.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_utils_freq_to_band.py` & `pyhamtools-0.9.1/test/test_utils_freq_to_band.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_lookuplib.py` & `pyhamtools-0.9.1/test/test_lookuplib.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_eqsl.py` & `pyhamtools-0.9.1/test/test_eqsl.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_lookuplib_clublogxml.py` & `pyhamtools-0.9.1/test/test_lookuplib_clublogxml.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_lookuplib_qrz.py` & `pyhamtools-0.9.1/test/test_lookuplib_qrz.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_locator_locator_to_latlong.py` & `pyhamtools-0.9.1/test/test_locator_locator_to_latlong.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_dxcluster.py` & `pyhamtools-0.9.1/test/test_dxcluster.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_lookuplib_gettersetter_api.py` & `pyhamtools-0.9.1/test/test_lookuplib_gettersetter_api.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/test/test_locator_distances.py` & `pyhamtools-0.9.1/test/test_locator_distances.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/frequency.py` & `pyhamtools-0.9.1/pyhamtools/frequency.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/qsl.py` & `pyhamtools-0.9.1/pyhamtools/qsl.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/lookuplib.py` & `pyhamtools-0.9.1/pyhamtools/lookuplib.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/logparser.py` & `pyhamtools-0.9.1/pyhamtools/logparser.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/countryfilemapping.json` & `pyhamtools-0.9.1/pyhamtools/countryfilemapping.json`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/callinfo.py` & `pyhamtools-0.9.1/pyhamtools/callinfo.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/dxcluster.py` & `pyhamtools-0.9.1/pyhamtools/dxcluster.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/locator.py` & `pyhamtools-0.9.1/pyhamtools/locator.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/consts.py` & `pyhamtools-0.9.1/pyhamtools/consts.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/pyhamtools/utils.py` & `pyhamtools-0.9.1/pyhamtools/utils.py`

 * *Files identical despite different names*

### Comparing `pyhamtools-0.9.0/setup.py` & `pyhamtools-0.9.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 import os
-from distutils.core import setup
+from setuptools import setup
 
 kw = {}
 
 exec(open(os.path.join("pyhamtools","version.py")).read())
 
 setup(name='pyhamtools',
       version=__release__,
@@ -14,12 +14,12 @@
       url='http://github.com/dh1tw/pyhamtools',
       package_data={'': ['countryfilemapping.json']},
       packages=['pyhamtools'],
       install_requires=[
           "requests>=2.21.0",
           "ephem>=4.1.3",
           "beautifulsoup4>=4.7.1",
-          "lxml>=4.8.0",
+          "lxml>=4.8.0,<5.0.0",
           "redis>=2.10.6",
       ],
       **kw
      )
```

