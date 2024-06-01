# Comparing `tmp/whotfis_py-0.0.6.tar.gz` & `tmp/whotfis_py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whotfis_py-0.0.6.tar", last modified: Fri May 31 05:50:39 2024, max compression
+gzip compressed data, was "whotfis_py-0.0.7.tar", last modified: Sat Jun  1 07:20:52 2024, max compression
```

## Comparing `whotfis_py-0.0.6.tar` & `whotfis_py-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-31 05:50:39.063536 whotfis_py-0.0.6/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.6/LICENSE
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       68 2024-05-30 19:22:27.000000 whotfis_py-0.0.6/MANIFEST.in
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2400 2024-05-31 05:50:39.063322 whotfis_py-0.0.6/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1818 2024-05-31 05:50:18.000000 whotfis_py-0.0.6/README.md
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-31 05:50:39.063588 whotfis_py-0.0.6/setup.cfg
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      837 2024-05-31 05:50:37.000000 whotfis_py-0.0.6/setup.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-31 05:50:39.062196 whotfis_py-0.0.6/whotfis_py/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      699 2024-05-31 05:19:12.000000 whotfis_py-0.0.6/whotfis_py/__init__.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2419 2024-05-31 05:16:32.000000 whotfis_py-0.0.6/whotfis_py/parser.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1659 2024-05-31 05:50:08.000000 whotfis_py-0.0.6/whotfis_py/registries.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4161 2024-05-31 05:31:35.000000 whotfis_py-0.0.6/whotfis_py/result.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-31 05:50:39.063047 whotfis_py-0.0.6/whotfis_py.egg-info/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2400 2024-05-31 05:50:39.000000 whotfis_py-0.0.6/whotfis_py.egg-info/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      264 2024-05-31 05:50:39.000000 whotfis_py-0.0.6/whotfis_py.egg-info/SOURCES.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-31 05:50:39.000000 whotfis_py-0.0.6/whotfis_py.egg-info/dependency_links.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-05-31 05:50:39.000000 whotfis_py-0.0.6/whotfis_py.egg-info/top_level.txt
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-06-01 07:20:52.082548 whotfis_py-0.0.7/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.7/LICENSE
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       68 2024-05-30 19:22:27.000000 whotfis_py-0.0.7/MANIFEST.in
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2602 2024-06-01 07:20:52.082378 whotfis_py-0.0.7/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2020 2024-06-01 07:20:45.000000 whotfis_py-0.0.7/README.md
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-06-01 07:20:52.082582 whotfis_py-0.0.7/setup.cfg
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      837 2024-06-01 07:20:45.000000 whotfis_py-0.0.7/setup.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-06-01 07:20:52.081583 whotfis_py-0.0.7/whotfis_py/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      696 2024-05-31 06:11:59.000000 whotfis_py-0.0.7/whotfis_py/__init__.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2419 2024-05-31 05:16:32.000000 whotfis_py-0.0.7/whotfis_py/parser.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1659 2024-05-31 05:50:08.000000 whotfis_py-0.0.7/whotfis_py/registries.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4334 2024-05-31 06:09:47.000000 whotfis_py-0.0.7/whotfis_py/result.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-06-01 07:20:52.082215 whotfis_py-0.0.7/whotfis_py.egg-info/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2602 2024-06-01 07:20:52.000000 whotfis_py-0.0.7/whotfis_py.egg-info/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      264 2024-06-01 07:20:52.000000 whotfis_py-0.0.7/whotfis_py.egg-info/SOURCES.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-06-01 07:20:52.000000 whotfis_py-0.0.7/whotfis_py.egg-info/dependency_links.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-06-01 07:20:52.000000 whotfis_py-0.0.7/whotfis_py.egg-info/top_level.txt
```

### Comparing `whotfis_py-0.0.6/LICENSE` & `whotfis_py-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.6/PKG-INFO` & `whotfis_py-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple package to interact with the whois command line tool
 Home-page: https://github.com/xV4L3x/whotfis-py
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
 License: Apache 2
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Avaiability
+| Platform | Status               |
+|----------|----------------------|
+| MacOS    | Supported ✅          |
+| Linux    | In Progress 🚧       |
+| Windows  | Not supported yet  ❌ |
+
+
 # Installation
 To install the package, just run the following command:
 ```bash
 pip install whotfis-py
 ```
 # Usage
 ```python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `whotfis_py-0.0.6/README.md` & `whotfis_py-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Avaiability
+| Platform | Status               |
+|----------|----------------------|
+| MacOS    | Supported ✅          |
+| Linux    | In Progress 🚧       |
+| Windows  | Not supported yet  ❌ |
+
+
 # Installation
 To install the package, just run the following command:
 ```bash
 pip install whotfis-py
 ```
 # Usage
 ```python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `whotfis_py-0.0.6/setup.py` & `whotfis_py-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = "Simple package to interact with the whois command line tool"
 
 setup(
     name="whotfis-py",
     version=VERSION,
     author="Valerio Pio De Nicola",
     author_email="valeriopio02@gmail.com",
```

### Comparing `whotfis_py-0.0.6/whotfis_py/__init__.py` & `whotfis_py-0.0.7/whotfis_py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     if registry == registries.CUSTOM:
         if custom_server == "" or custom_server is None:
             raise ValueError("Custom server must be specified when using the CUSTOM registry")
 
     command = "whois {} {} {}".format(registry, custom_server, query)
     results = os.popen(command).read()
     parsed_results = parse(results, registry)
-    return parsed_results[0]
+    return parsed_results
 
 
 if __name__ == "__main__":
     whois_result = lookup("34.160.38.1", registries.CUSTOM, "whois.radb.net")
     print(whois_result.dict())
```

### Comparing `whotfis_py-0.0.6/whotfis_py/parser.py` & `whotfis_py-0.0.7/whotfis_py/parser.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.6/whotfis_py/registries.py` & `whotfis_py-0.0.7/whotfis_py/registries.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.6/whotfis_py/result.py` & `whotfis_py-0.0.7/whotfis_py/result.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
     def router(self):
         return self.route.split("/")[0] if self.route is not None else None
 
     def mask(self):
         return self.route.split("/")[1] if self.route is not None else None
 
+    def dict(self):
+        parent_dict = super().dict()
+        parent_dict["router"] = self.router()
+        parent_dict["mask"] = self.mask()
+        return parent_dict
+
     def __init__(self,
                  route=None,
                  origin=None,
                  descr=None,
                  notify=None,
                  mnt_by=None,
                  changed=None,
```

### Comparing `whotfis_py-0.0.6/whotfis_py.egg-info/PKG-INFO` & `whotfis_py-0.0.7/whotfis_py.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple package to interact with the whois command line tool
 Home-page: https://github.com/xV4L3x/whotfis-py
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
 License: Apache 2
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Avaiability
+| Platform | Status               |
+|----------|----------------------|
+| MacOS    | Supported ✅          |
+| Linux    | In Progress 🚧       |
+| Windows  | Not supported yet  ❌ |
+
+
 # Installation
 To install the package, just run the following command:
 ```bash
 pip install whotfis-py
 ```
 # Usage
 ```python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

