# Comparing `tmp/subspy-1.1.1.tar.gz` & `tmp/subspy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subspy-1.1.1.tar", last modified: Sat Jun  1 05:16:07 2024, max compression
+gzip compressed data, was "subspy-2.2.2.tar", last modified: Sat Jun  1 05:55:03 2024, max compression
```

## Comparing `subspy-1.1.1.tar` & `subspy-2.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 05:16:07.450798 subspy-1.1.1/
--rw-rw-rw-   0        0        0     2426 2024-06-01 05:16:07.450798 subspy-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1687 2024-06-01 05:10:53.000000 subspy-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 05:16:07.450798 subspy-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1252 2024-06-01 05:15:18.000000 subspy-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:16:07.419552 subspy-1.1.1/subspy/
--rw-rw-rw-   0        0        0      258 2024-06-01 05:10:53.000000 subspy-1.1.1/subspy/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-06-01 05:10:53.000000 subspy-1.1.1/subspy/cli.py
--rw-rw-rw-   0        0        0       59 2024-06-01 05:10:53.000000 subspy-1.1.1/subspy/default_subdomains.txt
--rw-rw-rw-   0        0        0     1458 2024-06-01 05:10:53.000000 subspy-1.1.1/subspy/subdomain.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:16:07.450798 subspy-1.1.1/subspy.egg-info/
--rw-rw-rw-   0        0        0     2426 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 05:55:03.772989 subspy-2.2.2/
+-rw-rw-rw-   0        0        0     2426 2024-06-01 05:55:03.772989 subspy-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1687 2024-06-01 05:54:51.000000 subspy-2.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 05:55:03.772989 subspy-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2024-06-01 05:54:51.000000 subspy-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:55:03.741755 subspy-2.2.2/subspy/
+-rw-rw-rw-   0        0        0      258 2024-06-01 05:54:51.000000 subspy-2.2.2/subspy/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-06-01 05:54:51.000000 subspy-2.2.2/subspy/cli.py
+-rw-rw-rw-   0        0        0    72949 2024-06-01 05:54:51.000000 subspy-2.2.2/subspy/default_subdomains.txt
+-rw-rw-rw-   0        0        0     1458 2024-06-01 05:54:51.000000 subspy-2.2.2/subspy/subdomain.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:55:03.772989 subspy-2.2.2/subspy.egg-info/
+-rw-rw-rw-   0        0        0     2426 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 05:55:03.000000 subspy-2.2.2/subspy.egg-info/top_level.txt
```

### Comparing `subspy-1.1.1/PKG-INFO` & `subspy-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subspy
-Version: 1.1.1
+Version: 2.2.2
 Summary: SubSpy: A tool for subdomain enumeration.
 Home-page: https://mrfidal.in/cyber-security/subspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: subspy,subdomain,enumeration,scanning,mrfidal,cyber security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `subspy-1.1.1/README.md` & `subspy-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `subspy-1.1.1/setup.py` & `subspy-2.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='subspy',
-    version='1.1.1',
+    version='2.2.2',
     description='SubSpy: A tool for subdomain enumeration.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/subspy',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `subspy-1.1.1/subspy/cli.py` & `subspy-2.2.2/subspy/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 from subspy.subdomain import test_subdomains, get_default_subdomains, is_subdomain_available
 
-VERSION = "1.0.0"
+VERSION = "2.2.2"
 AUTHOR_INFO = "Author: Fidal, Contact : https://mrfidal.in/contact"
 
 def save_to_file(filename, data):
     with open(filename, "w") as file:
         file.write(data)
     print(f"[+] Results saved to {filename}")
```

### Comparing `subspy-1.1.1/subspy/subdomain.py` & `subspy-2.2.2/subspy/subdomain.py`

 * *Files identical despite different names*

### Comparing `subspy-1.1.1/subspy.egg-info/PKG-INFO` & `subspy-2.2.2/subspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subspy
-Version: 1.1.1
+Version: 2.2.2
 Summary: SubSpy: A tool for subdomain enumeration.
 Home-page: https://mrfidal.in/cyber-security/subspy
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: subspy,subdomain,enumeration,scanning,mrfidal,cyber security
 Classifier: Development Status :: 5 - Production/Stable
```

