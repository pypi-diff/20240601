# Comparing `tmp/plegui-1.1.9.tar.gz` & `tmp/plegui-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plegui-1.1.9.tar", last modified: Wed May 29 22:19:19 2024, max compression
+gzip compressed data, was "plegui-1.2.4.tar", last modified: Sat Jun  1 13:36:48 2024, max compression
```

## Comparing `plegui-1.1.9.tar` & `plegui-1.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 22:19:19.449875 plegui-1.1.9/
--rw-rw-rw-   0        0        0     1202 2024-05-29 22:19:19.449875 plegui-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      779 2024-05-23 21:22:00.000000 plegui-1.1.9/README.md
--rw-rw-rw-   0        0        0     1103 2024-05-15 20:32:47.000000 plegui-1.1.9/license
-drwxrwxrwx   0        0        0        0 2024-05-29 22:19:19.449875 plegui-1.1.9/plegui.egg-info/
--rw-rw-rw-   0        0        0     1202 2024-05-29 22:19:19.000000 plegui-1.1.9/plegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-29 22:19:19.000000 plegui-1.1.9/plegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 22:19:19.000000 plegui-1.1.9/plegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 22:19:19.000000 plegui-1.1.9/plegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 22:19:19.449875 plegui-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      737 2024-05-29 22:18:42.000000 plegui-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:36:48.524811 plegui-1.2.4/
+-rw-rw-rw-   0        0        0     1842 2024-06-01 13:36:48.519799 plegui-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1421 2024-06-01 13:36:00.000000 plegui-1.2.4/README.md
+-rw-rw-rw-   0        0        0     1103 2024-05-15 20:32:47.000000 plegui-1.2.4/license
+drwxrwxrwx   0        0        0        0 2024-06-01 13:36:48.518188 plegui-1.2.4/plegui.egg-info/
+-rw-rw-rw-   0        0        0     1842 2024-06-01 13:36:48.000000 plegui-1.2.4/plegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-06-01 13:36:48.000000 plegui-1.2.4/plegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:36:48.000000 plegui-1.2.4/plegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:36:48.000000 plegui-1.2.4/plegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 13:36:48.524811 plegui-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      737 2024-06-01 13:36:21.000000 plegui-1.2.4/setup.py
```

### Comparing `plegui-1.1.9/license` & `plegui-1.2.4/license`

 * *Files identical despite different names*

### Comparing `plegui-1.1.9/setup.py` & `plegui-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="plegui",
-    version="1.1.9",
+    version="1.2.4",
     description="A library used to make GUIs and Messages boxes and other..",
     long_description=README,
     long_description_content_type="text/markdown",
     author="PyGaps CEO",
     author_email="soqratiakram33@gmail.com",
     packages=find_packages(),
     classifiers=[
```

