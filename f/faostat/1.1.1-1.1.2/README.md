# Comparing `tmp/faostat-1.1.1.tar.gz` & `tmp/faostat-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faostat-1.1.1.tar", last modified: Fri May 24 15:24:56 2024, max compression
+gzip compressed data, was "faostat-1.1.2.tar", last modified: Sat Jun  1 11:38:15 2024, max compression
```

## Comparing `faostat-1.1.1.tar` & `faostat-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 15:24:56.050810 faostat-1.1.1/
--rw-rw-rw-   0        0        0     1102 2024-05-24 13:20:54.000000 faostat-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       85 2024-03-05 16:39:44.000000 faostat-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    15852 2024-05-24 15:24:56.050810 faostat-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    14796 2024-05-24 09:38:47.000000 faostat-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 15:24:55.997435 faostat-1.1.1/faostat/
--rw-rw-rw-   0        0        0      796 2024-04-22 13:43:37.000000 faostat-1.1.1/faostat/__init__.py
--rw-rw-rw-   0        0        0    14640 2024-05-24 09:07:53.000000 faostat-1.1.1/faostat/faostat.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:24:56.035184 faostat-1.1.1/faostat.egg-info/
--rw-rw-rw-   0        0        0    15852 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-24 15:24:55.000000 faostat-1.1.1/faostat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 15:24:56.050810 faostat-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1615 2024-05-24 13:20:25.000000 faostat-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:24:56.035184 faostat-1.1.1/test/
--rw-rw-rw-   0        0        0     1056 2024-03-19 15:44:24.000000 faostat-1.1.1/test/test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:38:15.679569 faostat-1.1.2/
+-rw-rw-rw-   0        0        0     1102 2024-05-24 13:20:54.000000 faostat-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       85 2024-03-05 16:39:44.000000 faostat-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    15908 2024-06-01 11:38:15.679569 faostat-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14852 2024-05-31 15:24:21.000000 faostat-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 11:38:15.601461 faostat-1.1.2/faostat/
+-rw-rw-rw-   0        0        0      796 2024-04-22 13:43:37.000000 faostat-1.1.2/faostat/__init__.py
+-rw-rw-rw-   0        0        0    14577 2024-05-31 15:19:26.000000 faostat-1.1.2/faostat/faostat.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:38:15.664103 faostat-1.1.2/faostat.egg-info/
+-rw-rw-rw-   0        0        0    15908 2024-06-01 11:38:15.000000 faostat-1.1.2/faostat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-06-01 11:38:15.000000 faostat-1.1.2/faostat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 11:38:15.000000 faostat-1.1.2/faostat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-01 11:38:15.000000 faostat-1.1.2/faostat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 11:38:15.000000 faostat-1.1.2/faostat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 11:38:15.679569 faostat-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-05-31 15:26:10.000000 faostat-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:38:15.648325 faostat-1.1.2/test/
+-rw-rw-rw-   0        0        0     1056 2024-05-31 15:24:41.000000 faostat-1.1.2/test/test.py
```

### Comparing `faostat-1.1.1/LICENSE.txt` & `faostat-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `faostat-1.1.1/PKG-INFO` & `faostat-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faostat
-Version: 1.1.1
+Version: 1.1.2
 Summary: Faostat Python Package
 Author: Noemi Emanuela Cazzaniga
 Author-email: noemi.cazzaniga@polimi.it
 License: MIT
 Project-URL: Source, https://bitbucket.org/noemicazzaniga/faostat/src/master/
 Keywords: faostat statistics data economics science
 Classifier: Development Status :: 5 - Production/Stable
@@ -355,14 +355,18 @@
 
 * Python package [pandas][pd]: Python Data Analysis Library.
 * Python package [eurostat][es]: Tools to read data from Eurostat.
 
 
 ## History:
 
+### version 1.1.2 (June 2024):
+
+* Internal bug fix
+
 ### version 1.1.1 (May 2024):
 
 * Removed the functions get_areas, get_years, get_items and get_elements.
 * Implemented all codings.
 * set_requests_args and get_requests_args replace https_proxy args.
 * Changed the base url.
 * https input parameter is deprecated.
```

### Comparing `faostat-1.1.1/README.md` & `faostat-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,18 @@
 
 * Python package [pandas][pd]: Python Data Analysis Library.
 * Python package [eurostat][es]: Tools to read data from Eurostat.
 
 
 ## History:
 
+### version 1.1.2 (June 2024):
+
+* Internal bug fix
+
 ### version 1.1.1 (May 2024):
 
 * Removed the functions get_areas, get_years, get_items and get_elements.
 * Implemented all codings.
 * set_requests_args and get_requests_args replace https_proxy args.
 * Changed the base url.
 * https input parameter is deprecated.
```

### Comparing `faostat-1.1.1/faostat/__init__.py` & `faostat-1.1.2/faostat/__init__.py`

 * *Files identical despite different names*

### Comparing `faostat-1.1.1/faostat/faostat.py` & `faostat-1.1.2/faostat/faostat.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 
 def set_requests_args(**kwargs):
     """
     Allows to set some arguments for "requests":
     - timeout: how long to wait for the server before raising an error. (optional)
         Default: 120 sec.
     - proxies : dict with protocol, user and password. (optional)
-        For the Eurostat API, only https proxy.
+        For the Faostat API, only https proxy.
         Examples: {'https': 'http://myuser:mypass@123.45.67.89:1234'}
                   {'https': 'https://123.45.67.89:1234'}
         Default: None.
     - verify : for the server’s TLS certificate. (optional)
         Default: None.
     - cert : user-provided SSL certificate. (optional)
        Default: None.
 
     Returns
     -------
     None.
 
     """
-    assert set(kwargs.keys()).issubset(["timeout", "proxies", "verify", "cert"]), "Wrong arguments."
+    assert set(kwargs.keys()).issubset({"timeout", "proxies", "verify", "cert"}), "Wrong arguments."
     global __ra__
     for k in kwargs:
         __ra__[k] = kwargs[k]
 
 
 def get_requests_args():
     """
@@ -94,17 +94,16 @@
     -------
     l : list
         list of available datasets and some metadata.
     **kwargs:
         https_proxy, deprecated
 
     """
-    if len(kwargs) > 0:
-        set_requests_args(__depr__(**kwargs))
-        kwargs.pop('https_proxy', None)
+    assert set(kwargs.keys()).issubset({'https_proxy',}), "Wrong argument."
+    __depr__(**kwargs)
     
     l = [('code',
           'label',
           'date_update',
           'note_update',
           'release_current',
           'state_current',
@@ -165,17 +164,16 @@
     -------
     d : list
         parameters for data filtering.
     **kwargs:
         https_proxy, deprecated
 
     """
-    if len(kwargs) > 0:
-        set_requests_args(__depr__(**kwargs))
-        kwargs.pop('https_proxy', None)
+    assert set(kwargs.keys()).issubset({'https_proxy',}), "Wrong argument."
+    __depr__(**kwargs)
 
     url = __BASE_URL__ + 'dimensions/' + code
     d = [('parameter code', 'coding_systems', 'subdimensions {code: meaning}')]
     response = __getresp__(url)
     data = response.json()['data']
     for par in data:
         code = par['id']
@@ -224,17 +222,16 @@
     -------
     d : dict
         {label: code, ...}.
     **kwargs:
         https_proxy, deprecated
 
     """
-    if len(kwargs) > 0:
-        set_requests_args(__depr__(**kwargs))
-        kwargs.pop('https_proxy', None)
+    assert set(kwargs.keys()).issubset({'https_proxy',}), "Wrong argument."
+    __depr__(**kwargs)
 
     url = __BASE_URL__ + 'codes/' + par + '/' + code
     response = __getresp__(url)
     data = response.json()['data']
     d = dict()
     for el in data:
         d[el['label']] = el['code']
@@ -258,17 +255,16 @@
     -------
     d : dataframe
          with label, code, aggregate type.
     **kwargs:
         https_proxy, deprecated
 
     """
-    if len(kwargs) > 0:
-        set_requests_args(__depr__(**kwargs))
-        kwargs.pop('https_proxy', None)
+    assert set(kwargs.keys()).issubset({'https_proxy',}), "Wrong argument."
+    __depr__(**kwargs)
 
     url = __BASE_URL__ + 'codes/' + par + '/' + code
     response = __getresp__(url)
     data = response.json()['data']
     d = []
     for el in data:
         d.append((el['label'], el['code'], el['aggregate_type']))
@@ -312,19 +308,18 @@
 
     Returns
     -------
     l : list
         data with header.
 
     """
-    assert set(kwargs.keys()).issubset(['pars', 'coding', 'show_flags', 'null_values', 
-                 'show_notes', 'strval', 'https_proxy']), "Error: unexpected kwarg."
-    if 'https_proxy' in set(kwargs.keys()):
-        set_requests_args(__depr__(**kwargs))
-        kwargs.pop('https_proxy', None)
+    assert set(kwargs.keys()).issubset({'pars', 'coding', 'show_flags', 'null_values', 
+                 'show_notes', 'strval', 'https_proxy'}), "Error: unexpected kwarg."
+
+    __depr__(**kwargs)
 
     pars = kwargs.get('pars', {})
     coding = kwargs.get('coding', {})
     show_flags = kwargs.get('show_flags', False)
     null_values = kwargs.get('null_values', False)
     show_notes = kwargs.get('show_notes', False)
     strval = kwargs.get('strval', True)
@@ -509,19 +504,21 @@
         {label: code, ...}.
 
     """
     return get_par(code, 'items', **kwargs)
 
 
 def __depr__(**kwargs):
-    assert kwargs.keys()[0]=="https_proxy", "Wrong arguments."
-    https_proxy = kwargs['https_proxy']
-    if https_proxy == None:
-        return None
-    elif ':' not in https_proxy[2]:
-        print("Error in proxy host. It must be in the form: 'url:port'")
-        raise
-    proxydic = {'https': 'https://' +\
-                https_proxy[0] + ':' +\
-                requests.compat.quote(https_proxy[1]) + '@' +\
-                https_proxy[2]}
-    return proxydic
+    if 'https_proxy' in set(kwargs.keys()):
+        https_proxy = kwargs['https_proxy']
+        if https_proxy == None:
+            return
+        elif ':' not in https_proxy[2]:
+            print("Error in proxy host. It must be in the form: 'url:port'")
+            raise
+        proxydic = {'https': 'https://' +\
+                    https_proxy[0] + ':' +\
+                    requests.compat.quote(https_proxy[1]) + '@' +\
+                    https_proxy[2]}
+        set_requests_args(proxies=proxydic)
+        kwargs.pop('https_proxy', None)
+    return
```

### Comparing `faostat-1.1.1/faostat.egg-info/PKG-INFO` & `faostat-1.1.2/faostat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faostat
-Version: 1.1.1
+Version: 1.1.2
 Summary: Faostat Python Package
 Author: Noemi Emanuela Cazzaniga
 Author-email: noemi.cazzaniga@polimi.it
 License: MIT
 Project-URL: Source, https://bitbucket.org/noemicazzaniga/faostat/src/master/
 Keywords: faostat statistics data economics science
 Classifier: Development Status :: 5 - Production/Stable
@@ -355,14 +355,18 @@
 
 * Python package [pandas][pd]: Python Data Analysis Library.
 * Python package [eurostat][es]: Tools to read data from Eurostat.
 
 
 ## History:
 
+### version 1.1.2 (June 2024):
+
+* Internal bug fix
+
 ### version 1.1.1 (May 2024):
 
 * Removed the functions get_areas, get_years, get_items and get_elements.
 * Implemented all codings.
 * set_requests_args and get_requests_args replace https_proxy args.
 * Changed the base url.
 * https input parameter is deprecated.
```

### Comparing `faostat-1.1.1/setup.py` & `faostat-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_descr = f.read()
 
 setup(name='faostat',
-      version='1.1.1',
+      version='1.1.2',
       license='MIT',
       date='2024',
       description="Faostat Python Package",
       long_description=long_descr,
       long_description_content_type='text/markdown',
       author='Noemi Emanuela Cazzaniga',
       author_email='noemi.cazzaniga@polimi.it',
```

### Comparing `faostat-1.1.1/test/test.py` & `faostat-1.1.2/test/test.py`

 * *Files identical despite different names*

