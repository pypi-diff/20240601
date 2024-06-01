# Comparing `tmp/Subdora-0.0.2.tar.gz` & `tmp/subdora-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subdora-0.0.2.tar", last modified: Tue Mar  5 15:24:43 2024, max compression
+gzip compressed data, was "E:\Subdora\Subdora_v0.1.0\Package\Subdora\dist\.tmp-sd9arspo\subdora-0.1.0.tar", last modified: Sun May  5 09:50:48 2024, max compression
```

## Comparing `Subdora-0.0.2.tar` & `subdora-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxr-x   0 laksh     (1000) laksh     (1000)        0 2024-03-05 15:24:43.747931 Subdora-0.0.2/
--rw-rw-r--   0 laksh     (1000) laksh     (1000)      750 2024-03-05 14:46:14.000000 Subdora-0.0.2/MANIFEST.in
--rw-r--r--   0 laksh     (1000) laksh     (1000)     1869 2024-03-05 15:24:43.747931 Subdora-0.0.2/PKG-INFO
--rw-rw-r--   0 laksh     (1000) laksh     (1000)     1317 2024-03-05 15:24:03.000000 Subdora-0.0.2/README.md
-drwxrwxr-x   0 laksh     (1000) laksh     (1000)        0 2024-03-05 15:24:43.743931 Subdora-0.0.2/Subdora/
--rw-rw-r--   0 laksh     (1000) laksh     (1000)       56 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/__init__.py
-drwxrwxr-x   0 laksh     (1000) laksh     (1000)        0 2024-03-05 15:24:43.743931 Subdora-0.0.2/Subdora/corex64/
--rw-rw-r--   0 laksh     (1000) laksh     (1000)        0 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/__init__.py
-drwxrwxr-x   0 laksh     (1000) laksh     (1000)        0 2024-03-05 15:24:43.743931 Subdora-0.0.2/Subdora/corex64/linux/
--rwxrwxr-x   0 laksh     (1000) laksh     (1000)    63480 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/linux/Subdora.so
--rw-rw-r--   0 laksh     (1000) laksh     (1000)        0 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/linux/__init__.py
-drwxrwxr-x   0 laksh     (1000) laksh     (1000)        0 2024-03-05 15:24:43.747931 Subdora-0.0.2/Subdora/corex64/win/
--rw-rw-r--   0 laksh     (1000) laksh     (1000)    40960 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/Subdora.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)        0 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/__init__.py
--rw-rw-r--   0 laksh     (1000) laksh     (1000)   322672 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/concrt140.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)   346624 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/libsodium.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)   573008 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/msvcp140.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)    35920 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/msvcp140_1.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)   268392 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/msvcp140_2.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)    50280 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/msvcp140_atomic_wait.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)    31856 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/msvcp140_codecvt_ids.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)   412752 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/vcamp140.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)   348784 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/vccorlib140.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)   196688 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/vcomp140.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)   119376 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/vcruntime140.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)    49744 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/vcruntime140_1.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)    38512 2024-03-05 14:46:06.000000 Subdora-0.0.2/Subdora/corex64/win/vcruntime140_threads.dll
--rw-rw-r--   0 laksh     (1000) laksh     (1000)     2072 2024-03-05 15:12:27.000000 Subdora-0.0.2/Subdora/subdora.py
-drwxrwxr-x   0 laksh     (1000) laksh     (1000)        0 2024-03-05 15:24:43.747931 Subdora-0.0.2/Subdora.egg-info/
--rw-r--r--   0 laksh     (1000) laksh     (1000)     1869 2024-03-05 15:24:43.000000 Subdora-0.0.2/Subdora.egg-info/PKG-INFO
--rw-rw-r--   0 laksh     (1000) laksh     (1000)      849 2024-03-05 15:24:43.000000 Subdora-0.0.2/Subdora.egg-info/SOURCES.txt
--rw-rw-r--   0 laksh     (1000) laksh     (1000)        1 2024-03-05 15:24:43.000000 Subdora-0.0.2/Subdora.egg-info/dependency_links.txt
--rw-rw-r--   0 laksh     (1000) laksh     (1000)        8 2024-03-05 15:24:43.000000 Subdora-0.0.2/Subdora.egg-info/top_level.txt
--rw-rw-r--   0 laksh     (1000) laksh     (1000)      102 2024-03-05 14:46:34.000000 Subdora-0.0.2/project.toml
--rw-rw-r--   0 laksh     (1000) laksh     (1000)       38 2024-03-05 15:24:43.747931 Subdora-0.0.2/setup.cfg
--rw-rw-r--   0 laksh     (1000) laksh     (1000)     1153 2024-03-05 14:47:52.000000 Subdora-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 09:50:48.873428 subdora-0.1.0/
+-rw-rw-rw-   0        0        0      120 2024-05-01 09:50:01.000000 subdora-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2252 2024-05-05 09:50:48.853425 subdora-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1633 2024-05-05 09:38:09.000000 subdora-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 09:50:44.155395 subdora-0.1.0/Subdora/
+-rw-rw-rw-   0        0        0       57 2024-05-03 12:30:53.000000 subdora-0.1.0/Subdora/__init__.py
+-rw-rw-rw-   0        0        0     2583 2024-05-05 09:39:50.000000 subdora-0.1.0/Subdora/_subdora.py
+-rw-rw-rw-   0        0        0     1808 2024-05-04 17:45:55.000000 subdora-0.1.0/Subdora/_subdora_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-05 09:50:43.988849 subdora-0.1.0/Subdora/corex64/
+drwxrwxrwx   0        0        0        0 2024-05-05 09:50:44.375887 subdora-0.1.0/Subdora/corex64/linux/
+-rw-rw-rw-   0        0        0   132128 2024-05-03 12:14:40.000000 subdora-0.1.0/Subdora/corex64/linux/Subdora.so
+drwxrwxrwx   0        0        0        0 2024-05-05 09:50:48.797827 subdora-0.1.0/Subdora/corex64/win/
+-rw-rw-rw-   0        0        0    65024 2024-05-05 08:20:34.000000 subdora-0.1.0/Subdora/corex64/win/Subdora.dll
+-rw-rw-rw-   0        0        0   322672 2024-02-02 20:31:00.000000 subdora-0.1.0/Subdora/corex64/win/concrt140.dll
+-rw-rw-rw-   0        0        0   346624 2024-01-07 18:32:18.000000 subdora-0.1.0/Subdora/corex64/win/libsodium.dll
+-rw-rw-rw-   0        0        0   573008 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140.dll
+-rw-rw-rw-   0        0        0    35920 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140_1.dll
+-rw-rw-rw-   0        0        0   268392 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140_2.dll
+-rw-rw-rw-   0        0        0    50280 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140_atomic_wait.dll
+-rw-rw-rw-   0        0        0    31856 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/msvcp140_codecvt_ids.dll
+-rw-rw-rw-   0        0        0   412752 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcamp140.dll
+-rw-rw-rw-   0        0        0   348784 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vccorlib140.dll
+-rw-rw-rw-   0        0        0   196688 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcomp140.dll
+-rw-rw-rw-   0        0        0   119376 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcruntime140.dll
+-rw-rw-rw-   0        0        0    49744 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcruntime140_1.dll
+-rw-rw-rw-   0        0        0    38512 2024-02-02 20:31:01.000000 subdora-0.1.0/Subdora/corex64/win/vcruntime140_threads.dll
+drwxrwxrwx   0        0        0        0 2024-05-05 09:50:48.827339 subdora-0.1.0/Subdora.egg-info/
+-rw-rw-rw-   0        0        0     2252 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-05-05 09:50:43.000000 subdora-0.1.0/Subdora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2024-05-01 09:50:14.000000 subdora-0.1.0/project.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 09:50:48.873428 subdora-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2024-05-05 09:38:54.000000 subdora-0.1.0/setup.py
```

### Comparing `Subdora-0.0.2/Subdora/corex64/win/concrt140.dll` & `subdora-0.1.0/Subdora/corex64/win/concrt140.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/libsodium.dll` & `subdora-0.1.0/Subdora/corex64/win/libsodium.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/msvcp140.dll` & `subdora-0.1.0/Subdora/corex64/win/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/msvcp140_1.dll` & `subdora-0.1.0/Subdora/corex64/win/msvcp140_1.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/msvcp140_2.dll` & `subdora-0.1.0/Subdora/corex64/win/msvcp140_2.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/msvcp140_atomic_wait.dll` & `subdora-0.1.0/Subdora/corex64/win/msvcp140_atomic_wait.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/msvcp140_codecvt_ids.dll` & `subdora-0.1.0/Subdora/corex64/win/msvcp140_codecvt_ids.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/vcamp140.dll` & `subdora-0.1.0/Subdora/corex64/win/vcamp140.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/vccorlib140.dll` & `subdora-0.1.0/Subdora/corex64/win/vccorlib140.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/vcomp140.dll` & `subdora-0.1.0/Subdora/corex64/win/vcomp140.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/vcruntime140.dll` & `subdora-0.1.0/Subdora/corex64/win/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/vcruntime140_1.dll` & `subdora-0.1.0/Subdora/corex64/win/vcruntime140_1.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/Subdora/corex64/win/vcruntime140_threads.dll` & `subdora-0.1.0/Subdora/corex64/win/vcruntime140_threads.dll`

 * *Files identical despite different names*

### Comparing `Subdora-0.0.2/setup.py` & `subdora-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2' 
-DESCRIPTION = 'Subdora : A python package that takes care of obfuscation and encryption of buisness logic.'
+VERSION = '0.1.0' 
+DESCRIPTION = 'Subdora : A python package that takes care of obfuscation of python scripts'
 LONG_DESCRIPTION = long_description
 
 
 setup(
         name="Subdora", 
         version=VERSION,
         author="Lakshit Karsoliya",
@@ -31,8 +31,11 @@
         keywords=['python', 'file encryption','security','obfuscation'],
         classifiers= [
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3",
             "Operating System :: Unix",
             "Operating System :: Microsoft :: Windows",
         ],
+        entry_points={
+            "console_scripts":["subdora = Subdora._subdora_cli:main"],
+        }
 )
```

