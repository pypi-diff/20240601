# Comparing `tmp/nnops-0.0.0.tar.gz` & `tmp/nnops-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnops-0.0.0.tar", last modified: Thu Jul 27 14:16:12 2023, max compression
+gzip compressed data, was "nnops-0.0.1.tar", last modified: Fri May 31 23:46:05 2024, max compression
```

## Comparing `nnops-0.0.0.tar` & `nnops-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:12.382213 nnops-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 14:16:02.000000 nnops-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-27 14:16:12.382213 nnops-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:02.000000 nnops-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:12.382213 nnops-0.0.0/nnops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:02.000000 nnops-0.0.0/nnops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:12.382213 nnops-0.0.0/nnops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-27 14:16:12.000000 nnops-0.0.0/nnops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 14:16:12.000000 nnops-0.0.0/nnops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:16:12.000000 nnops-0.0.0/nnops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 14:16:12.000000 nnops-0.0.0/nnops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:16:12.382213 nnops-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-27 14:16:02.000000 nnops-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:46:05.134832 nnops-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-31 23:45:57.000000 nnops-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-31 23:45:57.000000 nnops-0.0.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-31 23:45:57.000000 nnops-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-31 23:45:57.000000 nnops-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 23:46:05.134832 nnops-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-31 23:45:57.000000 nnops-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:46:05.130832 nnops-0.0.1/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 23:45:57.000000 nnops-0.0.1/csrc/python.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:46:05.130832 nnops-0.0.1/nnops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:57.000000 nnops-0.0.1/nnops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:46:05.134832 nnops-0.0.1/nnops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-31 23:45:57.000000 nnops-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 23:46:05.134832 nnops-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-31 23:45:57.000000 nnops-0.0.1/setup.py
```

### Comparing `nnops-0.0.0/setup.py` & `nnops-0.0.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,40 @@
-from setuptools import setup, find_packages
+[build-system]
+requires = [
+    "build",
+    "setuptools >= 42",
+    "wheel",
+    "ninja",
+    "cmake >= 3.15",
+    "nanobind >= 1.9.2",
+]
+build-backend = "setuptools.build_meta"
 
-setup(
-    name = 'nnops',
-    packages = find_packages(exclude=['examples']),
-    version = '0.0.0',
-    license='MIT',
-    description = 'Neural Network Operators',
-    author = 'JiauZhang',
-    author_email = 'jiauzhang@163.com',
-    url = 'https://github.com/JiauZhang/nnops',
-    long_description=open("README.md", "r", encoding="utf-8").read(),
-    long_description_content_type = 'text/markdown',
-    keywords = [
-        'Deep Learning',
-        'Neural Network Operators',
-        'Artificial Intelligence',
-    ],
-    install_requires=[
-    ],
-    classifiers=[
-        'Intended Audience :: Developers',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.8',
-    ],
-)
+[project]
+name = "nnops"
+version = "0.0.1"
+description = "Neural Network Operators"
+readme = "README.md"
+authors = [
+    {name = "Jiau Zhang", email = "jiauzhang@163.com"},
+]
+classifiers = [
+    'Intended Audience :: Developers',
+    'Topic :: Scientific/Engineering :: Artificial Intelligence',
+    'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
+    'Programming Language :: Python :: 3.8',
+]
+keywords = [
+    'Deep Learning',
+    'Neural Network Operators',
+    'Artificial Intelligence',
+]
+requires-python = ">= 3.8"
+dependencies = [
+    "numpy",
+]
+
+[project.urls]
+Homepage = "https://github.com/jiauzhang/nnops"
+
+[tool.setuptools]
+packages = ["nnops"]
```

