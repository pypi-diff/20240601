# Comparing `tmp/whataspp_message_inforu_local-0.0.17.tar.gz` & `tmp/whataspp_message_inforu_local-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whataspp_message_inforu_local-0.0.17.tar", last modified: Wed May 29 11:42:23 2024, max compression
+gzip compressed data, was "whataspp_message_inforu_local-0.0.18.tar", last modified: Sat Jun  1 21:28:54 2024, max compression
```

## Comparing `whataspp_message_inforu_local-0.0.17.tar` & `whataspp_message_inforu_local-0.0.18.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:42:23.254638 whataspp_message_inforu_local-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 11:42:23.250638 whataspp_message_inforu_local-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-29 11:41:50.000000 whataspp_message_inforu_local-0.0.17/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-29 11:41:57.000000 whataspp_message_inforu_local-0.0.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:42:23.254638 whataspp_message_inforu_local-0.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-29 11:41:50.000000 whataspp_message_inforu_local-0.0.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:42:23.250638 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:42:23.250638 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 11:41:50.000000 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-29 11:41:50.000000 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:41:50.000000 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:42:23.250638 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 11:42:23.000000 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 11:42:23.000000 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:42:23.000000 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-29 11:42:23.000000 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 11:42:23.000000 whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:28:54.133371 whataspp_message_inforu_local-0.0.18/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 21:28:54.133371 whataspp_message_inforu_local-0.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-06-01 21:28:13.000000 whataspp_message_inforu_local-0.0.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-06-01 21:28:22.000000 whataspp_message_inforu_local-0.0.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 21:28:54.133371 whataspp_message_inforu_local-0.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-06-01 21:28:13.000000 whataspp_message_inforu_local-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:28:54.129371 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:28:54.133371 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-06-01 21:28:13.000000 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-06-01 21:28:13.000000 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:28:13.000000 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:28:54.133371 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 21:28:54.000000 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-06-01 21:28:54.000000 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:28:54.000000 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-01 21:28:54.000000 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 21:28:54.000000 whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local.egg-info/top_level.txt
```

### Comparing `whataspp_message_inforu_local-0.0.17/PKG-INFO` & `whataspp_message_inforu_local-0.0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whataspp-message-inforu-local
-Version: 0.0.17
+Version: 0.0.18
 Summary: PyPI Package for Circles whataspp_inforu_local Python
 Home-page: https://github.com/circles-zone/whatsapp-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `whataspp_message_inforu_local-0.0.17/README.md` & `whataspp_message_inforu_local-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.17/pyproject.toml` & `whataspp_message_inforu_local-0.0.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.17/setup.py` & `whataspp_message_inforu_local-0.0.18/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "whataspp-message-inforu-local" 
 # Since all PACAKGE_NAMEs are with an underscore, we don't need this. Why do we need it?
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.17',  # update only the minor version each time # https://pypi.org/project/whataspp-inforu-local/
+    version='0.0.18',  # update only the minor version each time # https://pypi.org/project/whataspp-message-inforu-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles whataspp_inforu_local Python",
     long_description="This is a package for sharing common whataspp_inforu_local function used in different repositories",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/whatsapp-message-inforu-local-python-package",
     # packages=setuptools.find_packages(),
```

### Comparing `whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py` & `whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py` & `whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.17/whataspp_message_inforu_local.egg-info/PKG-INFO` & `whataspp_message_inforu_local-0.0.18/whataspp_message_inforu_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whataspp-message-inforu-local
-Version: 0.0.17
+Version: 0.0.18
 Summary: PyPI Package for Circles whataspp_inforu_local Python
 Home-page: https://github.com/circles-zone/whatsapp-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

