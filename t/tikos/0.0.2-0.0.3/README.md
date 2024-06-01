# Comparing `tmp/tikos-0.0.2.tar.gz` & `tmp/tikos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikos-0.0.2.tar", last modified: Fri May 24 20:56:18 2024, max compression
+gzip compressed data, was "tikos-0.0.3.tar", last modified: Sat Jun  1 07:43:23 2024, max compression
```

## Comparing `tikos-0.0.2.tar` & `tikos-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 20:56:18.518545 tikos-0.0.2/
--rw-rw-rw-   0        0        0        0 2024-05-24 08:40:33.000000 tikos-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      457 2024-05-24 20:56:18.517544 tikos-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-24 08:40:07.000000 tikos-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 20:56:18.518545 tikos-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      863 2024-05-24 20:56:11.000000 tikos-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:56:18.504034 tikos-0.0.2/tikos/
--rw-rw-rw-   0        0        0      142 2024-05-24 19:37:29.000000 tikos-0.0.2/tikos/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-24 20:54:47.000000 tikos-0.0.2/tikos/config.py
--rw-rw-rw-   0        0        0     1147 2024-05-24 19:45:54.000000 tikos-0.0.2/tikos/tikos.py
-drwxrwxrwx   0        0        0        0 2024-05-24 20:56:18.516546 tikos-0.0.2/tikos.egg-info/
--rw-rw-rw-   0        0        0      457 2024-05-24 20:56:18.000000 tikos-0.0.2/tikos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-24 20:56:18.000000 tikos-0.0.2/tikos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 20:56:18.000000 tikos-0.0.2/tikos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-24 20:56:18.000000 tikos-0.0.2/tikos.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 20:56:18.000000 tikos-0.0.2/tikos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-24 20:56:18.000000 tikos-0.0.2/tikos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 07:43:23.399007 tikos-0.0.3/
+-rw-rw-rw-   0        0        0       57 2024-06-01 07:41:54.000000 tikos-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      830 2024-06-01 07:43:23.398006 tikos-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-06-01 06:30:30.000000 tikos-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 07:43:23.399007 tikos-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      891 2024-06-01 07:09:57.000000 tikos-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:43:23.372008 tikos-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1209 2024-06-01 07:42:46.000000 tikos-0.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:43:23.375005 tikos-0.0.3/tikos/
+-rw-rw-rw-   0        0        0      324 2024-06-01 07:39:39.000000 tikos-0.0.3/tikos/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-06-01 06:24:00.000000 tikos-0.0.3/tikos/config.py
+-rw-rw-rw-   0        0        0     3032 2024-06-01 07:38:50.000000 tikos-0.0.3/tikos/tikos.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:43:23.397018 tikos-0.0.3/tikos.egg-info/
+-rw-rw-rw-   0        0        0      830 2024-06-01 07:43:23.000000 tikos-0.0.3/tikos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-06-01 07:43:23.000000 tikos-0.0.3/tikos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 07:43:23.000000 tikos-0.0.3/tikos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-06-01 07:43:23.000000 tikos-0.0.3/tikos.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 07:43:23.000000 tikos-0.0.3/tikos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-01 07:43:23.000000 tikos-0.0.3/tikos.egg-info/top_level.txt
```

### Comparing `tikos-0.0.2/setup.py` & `tikos-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="tikos",
-    version="0.0.2",
+    version="0.0.3",
     author="Don Liyanage, Tikos Technologies Ltd",
     author_email="don.liyanage@tikos.tech",
     description=("Tikos Platform Library"),
     license="Apache-2.0",
-    keywords="Tokis",
+    keywords="Tikos",
     url="http://packages.python.org/tikos",
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests.*", "tests"]),
     long_description=read('README.md'),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: Apache Software License",
     ],
     install_requires=['requests'],
```

