# Comparing `tmp/libschrodinger-1.2.2.tar.gz` & `tmp/libschrodinger-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libschrodinger-1.2.2.tar", last modified: Fri May 31 08:42:11 2024, max compression
+gzip compressed data, was "libschrodinger-1.2.3.tar", last modified: Sat Jun  1 12:00:09 2024, max compression
```

## Comparing `libschrodinger-1.2.2.tar` & `libschrodinger-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 08:42:11.654036 libschrodinger-1.2.2/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.2.2/LICENSE
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1961 2024-05-31 08:42:11.653547 libschrodinger-1.2.2/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1298 2024-05-31 07:32:02.000000 libschrodinger-1.2.2/README.md
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 08:42:11.650089 libschrodinger-1.2.2/libschrodinger/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1000 2024-05-31 07:49:50.000000 libschrodinger-1.2.2/libschrodinger/__init__.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 20:12:35.000000 libschrodinger-1.2.2/libschrodinger/config.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:13:30.000000 libschrodinger-1.2.2/libschrodinger/constants.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5046 2024-05-31 07:49:50.000000 libschrodinger-1.2.2/libschrodinger/electron.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      793 2024-05-31 07:49:50.000000 libschrodinger-1.2.2/libschrodinger/figlocation.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2825 2024-05-31 07:49:50.000000 libschrodinger-1.2.2/libschrodinger/gauss.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4710 2024-05-31 07:49:59.000000 libschrodinger-1.2.2/libschrodinger/graphs.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      991 2024-05-31 07:49:50.000000 libschrodinger-1.2.2/libschrodinger/interaction.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2078 2024-05-31 07:49:50.000000 libschrodinger-1.2.2/libschrodinger/particle.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-05-31 07:49:59.000000 libschrodinger-1.2.2/libschrodinger/potential.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      905 2024-05-31 07:49:50.000000 libschrodinger-1.2.2/libschrodinger/waveutils.py
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-31 08:42:11.653134 libschrodinger-1.2.2/libschrodinger.egg-info/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1961 2024-05-31 08:42:11.000000 libschrodinger-1.2.2/libschrodinger.egg-info/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      520 2024-05-31 08:42:11.000000 libschrodinger-1.2.2/libschrodinger.egg-info/SOURCES.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-31 08:42:11.000000 libschrodinger-1.2.2/libschrodinger.egg-info/dependency_links.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       23 2024-05-31 08:42:11.000000 libschrodinger-1.2.2/libschrodinger.egg-info/requires.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-31 08:42:11.000000 libschrodinger-1.2.2/libschrodinger.egg-info/top_level.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      849 2024-05-31 08:41:30.000000 libschrodinger-1.2.2/pyproject.toml
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-31 08:42:11.654127 libschrodinger-1.2.2/setup.cfg
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-06-01 12:00:09.684629 libschrodinger-1.2.3/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.2.3/LICENSE
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1961 2024-06-01 12:00:09.684251 libschrodinger-1.2.3/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1298 2024-05-31 07:32:02.000000 libschrodinger-1.2.3/README.md
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-06-01 12:00:09.678527 libschrodinger-1.2.3/libschrodinger/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1000 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/__init__.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-06-01 11:52:05.000000 libschrodinger-1.2.3/libschrodinger/config.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/constants.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5046 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/electron.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      793 2024-05-31 07:49:50.000000 libschrodinger-1.2.3/libschrodinger/figlocation.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2825 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/gauss.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4710 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/graphs.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      991 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/interaction.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2078 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/particle.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/potential.py
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-06-01 12:00:09.683305 libschrodinger-1.2.3/libschrodinger/quark/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      166 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/quark/__init__.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     7104 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/quark/baryon.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2639 2024-06-01 11:52:58.000000 libschrodinger-1.2.3/libschrodinger/quark/color.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3171 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/quark/hadron.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2939 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/quark/meson.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3257 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/quark/quark.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      905 2024-06-01 11:54:00.000000 libschrodinger-1.2.3/libschrodinger/waveutils.py
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-06-01 12:00:09.683773 libschrodinger-1.2.3/libschrodinger.egg-info/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1961 2024-06-01 12:00:09.000000 libschrodinger-1.2.3/libschrodinger.egg-info/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      705 2024-06-01 12:00:09.000000 libschrodinger-1.2.3/libschrodinger.egg-info/SOURCES.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-06-01 12:00:09.000000 libschrodinger-1.2.3/libschrodinger.egg-info/dependency_links.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       23 2024-06-01 12:00:09.000000 libschrodinger-1.2.3/libschrodinger.egg-info/requires.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-06-01 12:00:09.000000 libschrodinger-1.2.3/libschrodinger.egg-info/top_level.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      873 2024-06-01 11:56:46.000000 libschrodinger-1.2.3/pyproject.toml
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-06-01 12:00:09.684711 libschrodinger-1.2.3/setup.cfg
```

### Comparing `libschrodinger-1.2.2/LICENSE` & `libschrodinger-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/PKG-INFO` & `libschrodinger-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.2.2
+Version: 1.2.3
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `libschrodinger-1.2.2/README.md` & `libschrodinger-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/__init__.py` & `libschrodinger-1.2.3/libschrodinger/__init__.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/config.py` & `libschrodinger-1.2.3/libschrodinger/config.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/constants.py` & `libschrodinger-1.2.3/libschrodinger/constants.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/electron.py` & `libschrodinger-1.2.3/libschrodinger/electron.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/figlocation.py` & `libschrodinger-1.2.3/libschrodinger/figlocation.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/gauss.py` & `libschrodinger-1.2.3/libschrodinger/gauss.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/graphs.py` & `libschrodinger-1.2.3/libschrodinger/graphs.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/interaction.py` & `libschrodinger-1.2.3/libschrodinger/interaction.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/particle.py` & `libschrodinger-1.2.3/libschrodinger/particle.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/potential.py` & `libschrodinger-1.2.3/libschrodinger/potential.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger/waveutils.py` & `libschrodinger-1.2.3/libschrodinger/waveutils.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.2.2/libschrodinger.egg-info/PKG-INFO` & `libschrodinger-1.2.3/libschrodinger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.2.2
+Version: 1.2.3
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `libschrodinger-1.2.2/libschrodinger.egg-info/SOURCES.txt` & `libschrodinger-1.2.3/libschrodinger.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -12,8 +12,14 @@
 libschrodinger/particle.py
 libschrodinger/potential.py
 libschrodinger/waveutils.py
 libschrodinger.egg-info/PKG-INFO
 libschrodinger.egg-info/SOURCES.txt
 libschrodinger.egg-info/dependency_links.txt
 libschrodinger.egg-info/requires.txt
-libschrodinger.egg-info/top_level.txt
+libschrodinger.egg-info/top_level.txt
+libschrodinger/quark/__init__.py
+libschrodinger/quark/baryon.py
+libschrodinger/quark/color.py
+libschrodinger/quark/hadron.py
+libschrodinger/quark/meson.py
+libschrodinger/quark/quark.py
```

### Comparing `libschrodinger-1.2.2/pyproject.toml` & `libschrodinger-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libschrodinger"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="1p22geo", email="1p22geodecki@gmail.com" },
   { name="KacperTZSTI", email="kacper.m.trzop@gmail.com" },
 ]
 description = "A small package for simulating quantum-scale physics."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -23,8 +23,8 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/1p22geo/schrodinger"
 Issues = "https://github.com/1p22geo/schrodinger/issues"
 
 [tool.setuptools.packages.find]
-include = ["libschrodinger"]
+include = ["libschrodinger", "libschrodinger.quark"]
```

