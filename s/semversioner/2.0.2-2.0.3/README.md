# Comparing `tmp/semversioner-2.0.2.tar.gz` & `tmp/semversioner-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semversioner-2.0.2.tar", last modified: Sat Mar  9 10:20:38 2024, max compression
+gzip compressed data, was "semversioner-2.0.3.tar", last modified: Sat Jun  1 04:17:53 2024, max compression
```

## Comparing `semversioner-2.0.2.tar` & `semversioner-2.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 10:20:38.538068 semversioner-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-09 10:20:27.000000 semversioner-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-09 10:20:27.000000 semversioner-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-03-09 10:20:38.538068 semversioner-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-03-09 10:20:27.000000 semversioner-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-09 10:20:27.000000 semversioner-2.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 10:20:38.538068 semversioner-2.0.2/semversioner/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-09 10:20:27.000000 semversioner-2.0.2/semversioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-09 10:20:37.000000 semversioner-2.0.2/semversioner/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-03-09 10:20:27.000000 semversioner-2.0.2/semversioner/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-03-09 10:20:27.000000 semversioner-2.0.2/semversioner/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-09 10:20:27.000000 semversioner-2.0.2/semversioner/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-03-09 10:20:27.000000 semversioner-2.0.2/semversioner/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 10:20:38.538068 semversioner-2.0.2/semversioner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-03-09 10:20:38.000000 semversioner-2.0.2/semversioner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-09 10:20:38.000000 semversioner-2.0.2/semversioner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 10:20:38.000000 semversioner-2.0.2/semversioner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-09 10:20:38.000000 semversioner-2.0.2/semversioner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-09 10:20:38.000000 semversioner-2.0.2/semversioner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-09 10:20:38.000000 semversioner-2.0.2/semversioner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-09 10:20:38.538068 semversioner-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-09 10:20:27.000000 semversioner-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 10:20:38.538068 semversioner-2.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 10:20:38.538068 semversioner-2.0.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 10:20:27.000000 semversioner-2.0.2/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:17:53.665621 semversioner-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-01 04:17:37.000000 semversioner-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-01 04:17:37.000000 semversioner-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-06-01 04:17:53.665621 semversioner-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-06-01 04:17:37.000000 semversioner-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-01 04:17:37.000000 semversioner-2.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:17:53.661620 semversioner-2.0.3/semversioner/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 04:17:37.000000 semversioner-2.0.3/semversioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 04:17:52.000000 semversioner-2.0.3/semversioner/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-06-01 04:17:37.000000 semversioner-2.0.3/semversioner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-06-01 04:17:37.000000 semversioner-2.0.3/semversioner/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-06-01 04:17:37.000000 semversioner-2.0.3/semversioner/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-06-01 04:17:37.000000 semversioner-2.0.3/semversioner/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:17:53.665621 semversioner-2.0.3/semversioner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-06-01 04:17:53.000000 semversioner-2.0.3/semversioner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-06-01 04:17:53.000000 semversioner-2.0.3/semversioner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:17:53.000000 semversioner-2.0.3/semversioner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-01 04:17:53.000000 semversioner-2.0.3/semversioner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 04:17:53.000000 semversioner-2.0.3/semversioner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 04:17:53.000000 semversioner-2.0.3/semversioner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-01 04:17:53.665621 semversioner-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-06-01 04:17:37.000000 semversioner-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:17:53.661620 semversioner-2.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:17:53.665621 semversioner-2.0.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:17:37.000000 semversioner-2.0.3/tests/resources/__init__.py
```

### Comparing `semversioner-2.0.2/LICENSE` & `semversioner-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `semversioner-2.0.2/PKG-INFO` & `semversioner-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semversioner
-Version: 2.0.2
+Version: 2.0.3
 Summary: Manage properly semver in your repository
 Home-page: https://github.com/raulgomis/semversioner
 Author: Raul Gomis
 Author-email: raulgomis@gmail.com
 License: MIT
 Description: # Semversioner
         
@@ -144,14 +144,18 @@
         ---
         Made with ♥ by `Raul Gomis <https://twitter.com/rgomis>`.
         
         
         # Changelog
         Note: version releases in the 0.x.y range may introduce breaking changes.
         
+        ## 2.0.3
+        
+        - patch: Bump jinja2 from 3.1.3 to 3.1.4 to patch CVE-2024-34064.
+        
         ## 2.0.2
         
         - patch: Bump jinja2 from 3.1.2 to 3.1.3 to fix CVE-2024-22195.
         
         ## 2.0.1
         
         - patch: Add documentation for custom attributes in the changelog template.
```

### Comparing `semversioner-2.0.2/README.md` & `semversioner-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `semversioner-2.0.2/semversioner/cli.py` & `semversioner-2.0.3/semversioner/cli.py`

 * *Files identical despite different names*

### Comparing `semversioner-2.0.2/semversioner/core.py` & `semversioner-2.0.3/semversioner/core.py`

 * *Files identical despite different names*

### Comparing `semversioner-2.0.2/semversioner/models.py` & `semversioner-2.0.3/semversioner/models.py`

 * *Files identical despite different names*

### Comparing `semversioner-2.0.2/semversioner/storage.py` & `semversioner-2.0.3/semversioner/storage.py`

 * *Files identical despite different names*

### Comparing `semversioner-2.0.2/semversioner.egg-info/PKG-INFO` & `semversioner-2.0.3/semversioner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semversioner
-Version: 2.0.2
+Version: 2.0.3
 Summary: Manage properly semver in your repository
 Home-page: https://github.com/raulgomis/semversioner
 Author: Raul Gomis
 Author-email: raulgomis@gmail.com
 License: MIT
 Description: # Semversioner
         
@@ -144,14 +144,18 @@
         ---
         Made with ♥ by `Raul Gomis <https://twitter.com/rgomis>`.
         
         
         # Changelog
         Note: version releases in the 0.x.y range may introduce breaking changes.
         
+        ## 2.0.3
+        
+        - patch: Bump jinja2 from 3.1.3 to 3.1.4 to patch CVE-2024-34064.
+        
         ## 2.0.2
         
         - patch: Bump jinja2 from 3.1.2 to 3.1.3 to fix CVE-2024-22195.
         
         ## 2.0.1
         
         - patch: Add documentation for custom attributes in the changelog template.
```

### Comparing `semversioner-2.0.2/setup.py` & `semversioner-2.0.3/setup.py`

 * *Files identical despite different names*

