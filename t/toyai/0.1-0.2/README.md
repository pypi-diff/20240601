# Comparing `tmp/toyai-0.1.tar.gz` & `tmp/toyai-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toyai-0.1.tar", last modified: Sat Jun  1 06:00:29 2024, max compression
+gzip compressed data, was "toyai-0.2.tar", last modified: Sat Jun  1 06:08:37 2024, max compression
```

## Comparing `toyai-0.1.tar` & `toyai-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 supanutpgs   (501) staff       (20)        0 2024-06-01 06:00:29.954254 toyai-0.1/
--rw-r--r--   0 supanutpgs   (501) staff       (20)      410 2024-06-01 06:00:29.954034 toyai-0.1/PKG-INFO
--rw-r--r--   0 supanutpgs   (501) staff       (20)        0 2024-06-01 04:06:38.000000 toyai-0.1/README.md
--rw-r--r--   0 supanutpgs   (501) staff       (20)       38 2024-06-01 06:00:29.954303 toyai-0.1/setup.cfg
--rw-r--r--   0 supanutpgs   (501) staff       (20)     1197 2024-06-01 06:00:01.000000 toyai-0.1/setup.py
-drwxr-xr-x   0 supanutpgs   (501) staff       (20)        0 2024-06-01 06:00:29.953803 toyai-0.1/toyai.egg-info/
--rw-r--r--   0 supanutpgs   (501) staff       (20)      410 2024-06-01 06:00:29.000000 toyai-0.1/toyai.egg-info/PKG-INFO
--rw-r--r--   0 supanutpgs   (501) staff       (20)      134 2024-06-01 06:00:29.000000 toyai-0.1/toyai.egg-info/SOURCES.txt
--rw-r--r--   0 supanutpgs   (501) staff       (20)        1 2024-06-01 06:00:29.000000 toyai-0.1/toyai.egg-info/dependency_links.txt
--rw-r--r--   0 supanutpgs   (501) staff       (20)        1 2024-06-01 06:00:29.000000 toyai-0.1/toyai.egg-info/top_level.txt
+drwxr-xr-x   0 supanutpgs   (501) staff       (20)        0 2024-06-01 06:08:37.807080 toyai-0.2/
+-rw-r--r--   0 supanutpgs   (501) staff       (20)      357 2024-06-01 06:08:37.806885 toyai-0.2/PKG-INFO
+-rw-r--r--   0 supanutpgs   (501) staff       (20)        0 2024-06-01 04:06:38.000000 toyai-0.2/README.md
+-rw-r--r--   0 supanutpgs   (501) staff       (20)       38 2024-06-01 06:08:37.807130 toyai-0.2/setup.cfg
+-rw-r--r--   0 supanutpgs   (501) staff       (20)     1144 2024-06-01 06:07:47.000000 toyai-0.2/setup.py
+drwxr-xr-x   0 supanutpgs   (501) staff       (20)        0 2024-06-01 06:08:37.806669 toyai-0.2/toyai.egg-info/
+-rw-r--r--   0 supanutpgs   (501) staff       (20)      357 2024-06-01 06:08:37.000000 toyai-0.2/toyai.egg-info/PKG-INFO
+-rw-r--r--   0 supanutpgs   (501) staff       (20)      134 2024-06-01 06:08:37.000000 toyai-0.2/toyai.egg-info/SOURCES.txt
+-rw-r--r--   0 supanutpgs   (501) staff       (20)        1 2024-06-01 06:08:37.000000 toyai-0.2/toyai.egg-info/dependency_links.txt
+-rw-r--r--   0 supanutpgs   (501) staff       (20)        1 2024-06-01 06:08:37.000000 toyai-0.2/toyai.egg-info/top_level.txt
```

### Comparing `toyai-0.1/setup.py` & `toyai-0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 # here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 # pypi-AgEIcHlwaS5vcmcCJDc5ODU1YWNiLWQ2M2EtNDU2Ni1hZGMzLWQ3Y2FkNjI0Mzk3NgACKlszLCIzN2Y5NWZmYy00OGUyLTQ2NWYtYWFkNy02ODJhMGIwZTVhMjAiXQAABiDRffU2uinyXDCGaJvaDx0_QqofqIU5sKdtRbjvZvHlnw
 setup(
     name="toyai",
-    version="0.1",
+    version="0.2",
+    author="Supanut Panyagosa",
+    author_email="supanut.pgs@gmail.com",
+    description="A description of your package",
     # package_dir={"": ""},
     # packages=find_packages(where="modx"),
     packages=find_packages(),
     install_requires=[
         # ใส่ชื่อแพ็คเกจที่ต้องการใช้งานใน requirements.txt
     ],
-    author="Supanut Panyagosa",
-    author_email="supanut.pgs@gmail.com",
-    description="A description of your package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/yourusername/mypackage",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

