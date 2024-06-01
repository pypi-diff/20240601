# Comparing `tmp/zoho_analytics_connector-1.4.4.tar.gz` & `tmp/zoho_analytics_connector-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho_analytics_connector-1.4.4.tar", last modified: Wed Oct 18 10:21:35 2023, max compression
+gzip compressed data, was "zoho_analytics_connector-1.4.5.tar", last modified: Sat Jun  1 02:12:06 2024, max compression
```

## Comparing `zoho_analytics_connector-1.4.4.tar` & `zoho_analytics_connector-1.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-10-18 10:21:35.678793 zoho_analytics_connector-1.4.4/
--rw-rw-r--   0 tim       (1000) tim       (1000)      217 2022-07-14 03:04:02.000000 zoho_analytics_connector-1.4.4/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)    14308 2023-10-18 10:21:35.678793 zoho_analytics_connector-1.4.4/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)    13584 2023-07-23 03:20:17.000000 zoho_analytics_connector-1.4.4/README.md
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-10-18 10:21:35.678793 zoho_analytics_connector-1.4.4/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)     1649 2023-10-18 10:21:26.000000 zoho_analytics_connector-1.4.4/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-10-18 10:21:35.678793 zoho_analytics_connector-1.4.4/zoho_analytics_connector/
--rw-rw-r--   0 tim       (1000) tim       (1000)   100603 2022-11-23 02:51:47.000000 zoho_analytics_connector-1.4.4/zoho_analytics_connector/analytics_client_upstream.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    10075 2023-07-23 03:06:02.000000 zoho_analytics_connector-1.4.4/zoho_analytics_connector/enhanced_report_client.py
--rw-rw-r--   0 tim       (1000) tim       (1000)   115524 2023-10-18 10:10:13.000000 zoho_analytics_connector-1.4.4/zoho_analytics_connector/report_client.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-10-18 10:21:35.678793 zoho_analytics_connector-1.4.4/zoho_analytics_connector.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)    14308 2023-10-18 10:21:35.000000 zoho_analytics_connector-1.4.4/zoho_analytics_connector.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      412 2023-10-18 10:21:35.000000 zoho_analytics_connector-1.4.4/zoho_analytics_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-10-18 10:21:35.000000 zoho_analytics_connector-1.4.4/zoho_analytics_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       15 2023-10-18 10:21:35.000000 zoho_analytics_connector-1.4.4/zoho_analytics_connector.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       25 2023-10-18 10:21:35.000000 zoho_analytics_connector-1.4.4/zoho_analytics_connector.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-06-01 02:12:06.813175 zoho_analytics_connector-1.4.5/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      217 2022-07-14 03:04:02.000000 zoho_analytics_connector-1.4.5/LICENSE
+-rw-r--r--   0 tim       (1000) tim       (1000)    14433 2024-06-01 02:12:06.813175 zoho_analytics_connector-1.4.5/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)    13584 2023-07-23 03:20:17.000000 zoho_analytics_connector-1.4.5/README.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-06-01 02:12:06.813175 zoho_analytics_connector-1.4.5/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1747 2024-06-01 02:11:49.000000 zoho_analytics_connector-1.4.5/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-06-01 02:12:06.812175 zoho_analytics_connector-1.4.5/zoho_analytics_connector/
+-rw-rw-r--   0 tim       (1000) tim       (1000)   100603 2022-11-23 02:51:47.000000 zoho_analytics_connector-1.4.5/zoho_analytics_connector/analytics_client_upstream.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10075 2023-07-23 03:06:02.000000 zoho_analytics_connector-1.4.5/zoho_analytics_connector/enhanced_report_client.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)   115402 2024-06-01 02:10:09.000000 zoho_analytics_connector-1.4.5/zoho_analytics_connector/report_client.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-06-01 02:12:06.813175 zoho_analytics_connector-1.4.5/zoho_analytics_connector.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)    14433 2024-06-01 02:12:06.000000 zoho_analytics_connector-1.4.5/zoho_analytics_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      412 2024-06-01 02:12:06.000000 zoho_analytics_connector-1.4.5/zoho_analytics_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-06-01 02:12:06.000000 zoho_analytics_connector-1.4.5/zoho_analytics_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       15 2024-06-01 02:12:06.000000 zoho_analytics_connector-1.4.5/zoho_analytics_connector.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       25 2024-06-01 02:12:06.000000 zoho_analytics_connector-1.4.5/zoho_analytics_connector.egg-info/top_level.txt
```

### Comparing `zoho_analytics_connector-1.4.4/PKG-INFO` & `zoho_analytics_connector-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: zoho_analytics_connector
-Version: 1.4.4
+Version: 1.4.5
 Summary: Zoho Analytics connector
 Home-page: https://github.com/timrichardson/zoho_analytics_connector
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MPL-2.0
 Keywords: zoho analytics
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: emoji
 
 Zoho Analytics Connector for Python
 ========================
 
 Zoho's Python SDK for Zoho Reports is old, however it is very complete.
 This is a version which is Python 3 ready, tested on Python 3.8 and 3.9 and in fairly substantial production use.
 
@@ -335,9 +338,7 @@
 1.1.0 Treat "another import is in progress" as a recoverable error (can be retried)
     Move home-made retry logic to low level: report_client.__sendRequest(), and make retry optionally available to the key functions in EnhancedZohoAnalyticsClient. 
     Functions can pass retry_countdown to use retry. The retry handling is coping well under some initial use in high volume production loads.
 
 1.0.4 Documentation improvements
 
 1.0.3 Some slightly better error handling if Zoho returns an empty response
-
-
```

### Comparing `zoho_analytics_connector-1.4.4/README.md` & `zoho_analytics_connector-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `zoho_analytics_connector-1.4.4/setup.py` & `zoho_analytics_connector-1.4.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 from os import path
 cmdclass = {'build_sphinx': BuildDoc}
 
 # https://pypi.org/classifiers/
 
 name = 'zoho_analytics_connector'
 keywords = 'zoho analytics'
-version = '1.4.4'
+version = '1.4.5'
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=name,
     keywords=keywords,
     version=version,
     packages=['zoho_analytics_connector'],
-    python_requires='>=3.8',
+    python_requires='>=3.6',
     install_requires=['requests','emoji'],
     setup_requires=['pytest-runner', 'wheel', 'sphinx'],
     tests_require=["pytest", ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Office/Business',
     ],
     url='https://github.com/timrichardson/zoho_analytics_connector',
```

### Comparing `zoho_analytics_connector-1.4.4/zoho_analytics_connector/analytics_client_upstream.py` & `zoho_analytics_connector-1.4.5/zoho_analytics_connector/analytics_client_upstream.py`

 * *Files identical despite different names*

### Comparing `zoho_analytics_connector-1.4.4/zoho_analytics_connector/enhanced_report_client.py` & `zoho_analytics_connector-1.4.5/zoho_analytics_connector/enhanced_report_client.py`

 * *Files identical despite different names*

### Comparing `zoho_analytics_connector-1.4.4/zoho_analytics_connector/report_client.py` & `zoho_analytics_connector-1.4.5/zoho_analytics_connector/report_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,16 +207,17 @@
                     if not code:
                         m = re.search(r'"code":(\d+)', respObj.response.text)
                         if m:
                             code = int(m.group(1))
                         else:
                             code = -1
                             logger.error(f"could not find error code in {respObj.response.text} ")
-                            time.sleep(min(10 - retry_countdown, 1) * 10)
-                            continue
+                            raise ServerError(urlResp=respObj, zoho_error_code=code)
+                            # time.sleep(min(10 - retry_countdown, 1) * 10)
+                            # continue
 
                     logger.debug(f"API returned a 400 result and an error code: {code} ")
                     if code in [6045, ]:
                         logger.error(
                             f"Zoho API Recoverable rate limit (rate limit exceeded); there are {retry_countdown + 1} retries left")
                         if retry_countdown < 0:
                             logger.error(
@@ -246,18 +247,15 @@
                             f"7232 error,an invalid value has been provided according to the column's data type) {respObj.response.text=} ")
                         raise ServerError(urlResp=respObj, zoho_error_code=code)
                     elif code in [7280, ]:
                         logger.error(
                             f"7280 error, relating to schema errors, return immediately {respObj.response.text}")
                         raise ServerError(urlResp=respObj, zoho_error_code=code)
                     elif code in [7389, ]:
-                        logger.error(f"7389 Error from zoho Organisation does not exist {respObj.response.text}")
-                        raise ServerError(urlResp=respObj, zoho_error_code=code)
-                    elif code in [7403, ]:
-                        logger.error(f"7403 SQL Parsing Error {respObj.response.text}")
+                        logger.error(f"7389 Error from zoho Organisation doest not exist {respObj.response.text}")
                         raise ServerError(urlResp=respObj, zoho_error_code=code)
                     elif code in [8540, ]:
                         logger.error(f"8540 Error, token has incorrect scope {respObj.response.text}")
                         raise ServerError(urlResp=respObj, zoho_error_code=code)
                     elif code in [8535, ]:  # invalid oauth token
                         try:
                             self.getOAuthToken()
```

### Comparing `zoho_analytics_connector-1.4.4/zoho_analytics_connector.egg-info/PKG-INFO` & `zoho_analytics_connector-1.4.5/zoho_analytics_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: zoho-analytics-connector
-Version: 1.4.4
+Version: 1.4.5
 Summary: Zoho Analytics connector
 Home-page: https://github.com/timrichardson/zoho_analytics_connector
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MPL-2.0
 Keywords: zoho analytics
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: emoji
 
 Zoho Analytics Connector for Python
 ========================
 
 Zoho's Python SDK for Zoho Reports is old, however it is very complete.
 This is a version which is Python 3 ready, tested on Python 3.8 and 3.9 and in fairly substantial production use.
 
@@ -335,9 +338,7 @@
 1.1.0 Treat "another import is in progress" as a recoverable error (can be retried)
     Move home-made retry logic to low level: report_client.__sendRequest(), and make retry optionally available to the key functions in EnhancedZohoAnalyticsClient. 
     Functions can pass retry_countdown to use retry. The retry handling is coping well under some initial use in high volume production loads.
 
 1.0.4 Documentation improvements
 
 1.0.3 Some slightly better error handling if Zoho returns an empty response
-
-
```

