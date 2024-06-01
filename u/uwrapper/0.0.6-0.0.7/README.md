# Comparing `tmp/uwrapper-0.0.6.tar.gz` & `tmp/uwrapper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwrapper-0.0.6.tar", last modified: Sat Jun  1 15:36:44 2024, max compression
+gzip compressed data, was "uwrapper-0.0.7.tar", last modified: Sat Jun  1 15:41:08 2024, max compression
```

## Comparing `uwrapper-0.0.6.tar` & `uwrapper-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:36:44.411438 uwrapper-0.0.6/
--rw-rw-rw-   0        0        0      787 2024-06-01 15:36:44.407463 uwrapper-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-06-01 15:36:44.411438 uwrapper-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1039 2024-06-01 15:36:40.000000 uwrapper-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:36:44.343437 uwrapper-0.0.6/uwrapper/
--rw-rw-rw-   0        0        0       45 2024-06-01 15:20:04.000000 uwrapper-0.0.6/uwrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:36:44.383434 uwrapper-0.0.6/uwrapper/config/
--rw-rw-rw-   0        0        0       60 2024-06-01 13:44:37.000000 uwrapper-0.0.6/uwrapper/config/__init__.py
--rw-rw-rw-   0        0        0      527 2024-06-01 15:36:14.000000 uwrapper-0.0.6/uwrapper/config/config.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:36:44.387436 uwrapper-0.0.6/uwrapper/scripts/
--rw-rw-rw-   0        0        0       85 2024-06-01 13:45:05.000000 uwrapper-0.0.6/uwrapper/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:36:44.395436 uwrapper-0.0.6/uwrapper/scripts/services/
--rw-rw-rw-   0        0        0       20 2024-06-01 13:45:23.000000 uwrapper-0.0.6/uwrapper/scripts/services/__init__.py
--rw-rw-rw-   0        0        0      921 2024-06-01 12:10:08.000000 uwrapper-0.0.6/uwrapper/scripts/services/login.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:36:44.399461 uwrapper-0.0.6/uwrapper/scripts/src/
--rw-rw-rw-   0        0        0        0 2024-06-01 13:45:51.000000 uwrapper-0.0.6/uwrapper/scripts/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:36:44.403437 uwrapper-0.0.6/uwrapper.egg-info/
--rw-rw-rw-   0        0        0      787 2024-06-01 15:36:44.000000 uwrapper-0.0.6/uwrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-06-01 15:36:44.000000 uwrapper-0.0.6/uwrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:36:44.000000 uwrapper-0.0.6/uwrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-06-01 15:36:44.000000 uwrapper-0.0.6/uwrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 15:36:44.000000 uwrapper-0.0.6/uwrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:08.734840 uwrapper-0.0.7/
+-rw-rw-rw-   0        0        0      787 2024-06-01 15:41:08.730838 uwrapper-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:41:08.734840 uwrapper-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2024-06-01 15:40:12.000000 uwrapper-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:08.639498 uwrapper-0.0.7/uwrapper/
+-rw-rw-rw-   0        0        0       22 2024-06-01 15:40:30.000000 uwrapper-0.0.7/uwrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:08.710852 uwrapper-0.0.7/uwrapper/scripts/
+-rw-rw-rw-   0        0        0       85 2024-06-01 13:45:05.000000 uwrapper-0.0.7/uwrapper/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:08.718840 uwrapper-0.0.7/uwrapper/scripts/services/
+-rw-rw-rw-   0        0        0       20 2024-06-01 13:45:23.000000 uwrapper-0.0.7/uwrapper/scripts/services/__init__.py
+-rw-rw-rw-   0        0        0      914 2024-06-01 15:40:05.000000 uwrapper-0.0.7/uwrapper/scripts/services/login.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:08.722839 uwrapper-0.0.7/uwrapper/scripts/src/
+-rw-rw-rw-   0        0        0        0 2024-06-01 13:45:51.000000 uwrapper-0.0.7/uwrapper/scripts/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:41:08.726839 uwrapper-0.0.7/uwrapper.egg-info/
+-rw-rw-rw-   0        0        0      787 2024-06-01 15:41:08.000000 uwrapper-0.0.7/uwrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-06-01 15:41:08.000000 uwrapper-0.0.7/uwrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:41:08.000000 uwrapper-0.0.7/uwrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-06-01 15:41:08.000000 uwrapper-0.0.7/uwrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 15:41:08.000000 uwrapper-0.0.7/uwrapper.egg-info/top_level.txt
```

### Comparing `uwrapper-0.0.6/PKG-INFO` & `uwrapper-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwrapper
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python library for upstox APIs
 Home-page: https://github.com/azachbot/upstox_api_wrapper
 Author: Zachbot
 Author-email: zachbot006@gmail.com
 Keywords: upstox,nse,python,sdk,trading,stock markets,wrapper
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `uwrapper-0.0.6/setup.py` & `uwrapper-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'uwrapper',
     packages=setuptools.find_packages(),
-    version = '0.0.6',
+    version = '0.0.7',
     include_package_data=True,
     description = 'Python library for upstox APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",  author = 'Zachbot',
     author_email = 'zachbot006@gmail.com',
     url = 'https://github.com/azachbot/upstox_api_wrapper',
     install_requires=['requests', 'pandas','upstox-python-sdk'],
```

### Comparing `uwrapper-0.0.6/uwrapper/scripts/services/login.py` & `uwrapper-0.0.7/uwrapper/scripts/services/login.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """upstox login"""
-from ...config.config import get_configs
 import urllib.parse
 import requests
 
 def login(apikey,secretkey,rurl):
     """ logging into upstox """
-    config=get_configs()
     rurl_parsed=urllib.parse.quote(rurl,safe="")
-    uri=f'{config["login_url"]}=code&client_id={apikey}&redirect_uri={rurl_parsed}'
+    uri=f'https://api-v2.upstox.com/login/authorization/dialog?response_type=code&client_id={apikey}&redirect_uri={rurl_parsed}'
     print("Visit the following URL to authorize your application:")
     print(uri)
     code = input("Enter the code: ")
-    url=f"{config['authorization_token_url']}"
+    url=f"https://api.upstox.com/v2/login/authorization/token"
     headers={'accept': "application/json",'Content-Type': "application/x-www-form-urlencoded"}
     data={'code':code,'client_id':apikey,'client_secret':secretkey,'redirect_uri':rurl,'grant_type':'authorization_code'}
     response=requests.post(url,headers=headers,data=data)
     json_response=response.json()
     access_token=json_response['access_token']
     print('access token created')
     return access_token
```

### Comparing `uwrapper-0.0.6/uwrapper.egg-info/PKG-INFO` & `uwrapper-0.0.7/uwrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwrapper
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python library for upstox APIs
 Home-page: https://github.com/azachbot/upstox_api_wrapper
 Author: Zachbot
 Author-email: zachbot006@gmail.com
 Keywords: upstox,nse,python,sdk,trading,stock markets,wrapper
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

