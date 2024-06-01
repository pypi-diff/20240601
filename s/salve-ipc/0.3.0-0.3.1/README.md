# Comparing `tmp/salve_ipc-0.3.0.tar.gz` & `tmp/salve_ipc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salve_ipc-0.3.0.tar", last modified: Sat Jun  1 11:04:58 2024, max compression
+gzip compressed data, was "salve_ipc-0.3.1.tar", last modified: Sat Jun  1 11:10:54 2024, max compression
```

## Comparing `salve_ipc-0.3.0.tar` & `salve_ipc-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/salve_ipc/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/salve_ipc/highlight/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/highlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/highlight/highlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/ipc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/server_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/salve_ipc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:10:54.712672 salve_ipc-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-06-01 11:10:54.712672 salve_ipc-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:10:54.712672 salve_ipc-0.3.1/salve_ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/salve_ipc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:10:54.712672 salve_ipc-0.3.1/salve_ipc/highlight/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/salve_ipc/highlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/salve_ipc/highlight/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/salve_ipc/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/salve_ipc/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/salve_ipc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/salve_ipc/server_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:10:54.712672 salve_ipc-0.3.1/salve_ipc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-06-01 11:10:54.000000 salve_ipc-0.3.1/salve_ipc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-06-01 11:10:54.000000 salve_ipc-0.3.1/salve_ipc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:10:54.000000 salve_ipc-0.3.1/salve_ipc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 11:10:54.000000 salve_ipc-0.3.1/salve_ipc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 11:10:54.000000 salve_ipc-0.3.1/salve_ipc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 11:10:54.712672 salve_ipc-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-06-01 11:10:46.000000 salve_ipc-0.3.1/setup.py
```

### Comparing `salve_ipc-0.3.0/LICENSE` & `salve_ipc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.3.0/PKG-INFO` & `salve_ipc-0.3.1/salve_ipc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: salve_ipc
-Version: 0.3.0
+Name: salve-ipc
+Version: 0.3.1
 Summary: A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor
 Home-page: https://github.com/Moosems/salve
 Author: Moosems
 Author-email: moosems.j@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `salve_ipc-0.3.0/README.md` & `salve_ipc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.3.0/salve_ipc/highlight/highlight.py` & `salve_ipc-0.3.1/salve_ipc/highlight/highlight.py`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.3.0/salve_ipc/ipc.py` & `salve_ipc-0.3.1/salve_ipc/ipc.py`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.3.0/salve_ipc/misc.py` & `salve_ipc-0.3.1/salve_ipc/misc.py`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.3.0/salve_ipc/server.py` & `salve_ipc-0.3.1/salve_ipc/server.py`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.3.0/salve_ipc/server_functions.py` & `salve_ipc-0.3.1/salve_ipc/server_functions.py`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.3.0/salve_ipc.egg-info/PKG-INFO` & `salve_ipc-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: salve-ipc
-Version: 0.3.0
+Name: salve_ipc
+Version: 0.3.1
 Summary: A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor
 Home-page: https://github.com/Moosems/salve
 Author: Moosems
 Author-email: moosems.j@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `salve_ipc-0.3.0/setup.py` & `salve_ipc-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 setup(
     name="salve_ipc",
-    version="0.3.0",
+    version="0.3.1",
     description="A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor",
     author="Moosems",
     author_email="moosems.j@gmail.com",
     url="https://github.com/Moosems/salve",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[line for line in open("requirements.txt").readlines()],
+    install_requires=["pygments"],
     python_requires=">=3.9",
     license="MIT license",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Typing :: Typed",
     ],
```

