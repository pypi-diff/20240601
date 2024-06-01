# Comparing `tmp/tanjiro-0.2.0.tar.gz` & `tmp/tanjiro-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tanjiro-0.2.0.tar", last modified: Thu May 30 15:28:38 2024, max compression
+gzip compressed data, was "tanjiro-0.2.2.tar", last modified: Sat Jun  1 09:42:27 2024, max compression
```

## Comparing `tanjiro-0.2.0.tar` & `tanjiro-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-30 15:28:38.660569 tanjiro-0.2.0/
--rw-r--r--   0 runner    (1000) runner    (1000)      375 2024-05-30 15:28:38.656569 tanjiro-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       61 2024-05-30 08:54:06.000000 tanjiro-0.2.0/README.md
--rw-------   0 runner    (1000) runner    (1000)      567 2024-05-30 08:46:13.000000 tanjiro-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-30 15:28:38.660569 tanjiro-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      542 2024-05-30 15:27:31.000000 tanjiro-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-30 15:28:38.656569 tanjiro-0.2.0/tanjiro/
--rw-r--r--   0 runner    (1000) runner    (1000)       75 2024-05-30 15:25:30.000000 tanjiro-0.2.0/tanjiro/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      957 2024-05-30 08:50:06.000000 tanjiro-0.2.0/tanjiro/chatgpt.py
--rw-r--r--   0 runner    (1000) runner    (1000)      399 2024-05-30 15:24:52.000000 tanjiro-0.2.0/tanjiro/maths.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-30 15:28:38.656569 tanjiro-0.2.0/tanjiro.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      375 2024-05-30 15:28:38.000000 tanjiro-0.2.0/tanjiro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      213 2024-05-30 15:28:38.000000 tanjiro-0.2.0/tanjiro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-30 15:28:38.000000 tanjiro-0.2.0/tanjiro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-05-30 15:28:38.000000 tanjiro-0.2.0/tanjiro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-06-01 09:42:27.692202 tanjiro-0.2.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-06-01 09:42:27.692202 tanjiro-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       61 2024-05-30 08:54:06.000000 tanjiro-0.2.2/README.md
+-rw-------   0 runner    (1000) runner    (1000)      567 2024-05-30 08:46:13.000000 tanjiro-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-06-01 09:42:27.692202 tanjiro-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      732 2024-06-01 09:39:39.000000 tanjiro-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-06-01 09:42:27.680201 tanjiro-0.2.2/tanjiro/
+-rw-r--r--   0 runner    (1000) runner    (1000)      751 2024-05-30 16:27:32.000000 tanjiro-0.2.2/tanjiro/YouTube.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      136 2024-06-01 09:25:26.000000 tanjiro-0.2.2/tanjiro/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      633 2024-06-01 09:24:46.000000 tanjiro-0.2.2/tanjiro/chatbot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      957 2024-05-30 08:50:06.000000 tanjiro-0.2.2/tanjiro/chatgpt.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      399 2024-05-30 16:14:23.000000 tanjiro-0.2.2/tanjiro/maths.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-06-01 09:42:27.688201 tanjiro-0.2.2/tanjiro.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      531 2024-06-01 09:42:27.000000 tanjiro-0.2.2/tanjiro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      281 2024-06-01 09:42:27.000000 tanjiro-0.2.2/tanjiro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-06-01 09:42:27.000000 tanjiro-0.2.2/tanjiro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-06-01 09:42:27.000000 tanjiro-0.2.2/tanjiro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-06-01 09:42:27.000000 tanjiro-0.2.2/tanjiro.egg-info/top_level.txt
```

### Comparing `tanjiro-0.2.0/pyproject.toml` & `tanjiro-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tanjiro-0.2.0/setup.py` & `tanjiro-0.2.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='tanjiro',
-    version='0.2.0',
+    version='0.2.2',  # Update this line
     packages=find_packages(),
-    description='A simple library to interact with a ChatGPT API',
-    author='vikas ',
+    description='A simple library to interact with various APIs including ChatGPT, YouTube, Instagram, and more.',
+    author='Vikas',
     author_email='vgboss91@gmail.com',
     url='https://github.com/tanjiro-851/tanjiro',  # Update with your actual URL
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+    install_requires=[
+        'requests',
+        'undetected-chromedriver',
+        'selenium',
+        'pytube',
+    ],
     python_requires='>=3.6',
 )
```

### Comparing `tanjiro-0.2.0/tanjiro/chatgpt.py` & `tanjiro-0.2.2/tanjiro/chatgpt.py`

 * *Files identical despite different names*

