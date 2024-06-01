# Comparing `tmp/omicsdata-1.1.tar.gz` & `tmp/omicsdata-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omicsdata-1.1.tar", last modified: Fri May 31 20:47:01 2024, max compression
+gzip compressed data, was "omicsdata-1.2.tar", last modified: Sat Jun  1 15:18:17 2024, max compression
```

## Comparing `omicsdata-1.1.tar` & `omicsdata-1.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.551123 omicsdata-1.1/
--rw-r--r--   0 ethank     (501) staff       (20)     1064 2023-06-28 14:55:04.000000 omicsdata-1.1/LICENSE
--rw-r--r--   0 ethank     (501) staff       (20)     1100 2024-05-31 20:47:01.550951 omicsdata-1.1/PKG-INFO
--rw-r--r--   0 ethank     (501) staff       (20)      584 2023-07-11 22:14:55.000000 omicsdata-1.1/README.md
--rw-r--r--   0 ethank     (501) staff       (20)      583 2024-05-31 15:14:41.000000 omicsdata-1.1/pyproject.toml
--rw-r--r--   0 ethank     (501) staff       (20)       38 2024-05-31 20:47:01.551167 omicsdata-1.1/setup.cfg
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.543040 omicsdata-1.1/src/
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.544279 omicsdata-1.1/src/omicsdata/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/__init__.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.544825 omicsdata-1.1/src/omicsdata/cn/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-12-20 16:09:45.000000 omicsdata-1.1/src/omicsdata/cn/estimate.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.544907 omicsdata-1.1/src/omicsdata/csv/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-12-21 15:38:04.000000 omicsdata-1.1/src/omicsdata/csv/parse.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.545078 omicsdata-1.1/src/omicsdata/npz/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-07-04 21:32:15.000000 omicsdata-1.1/src/omicsdata/npz/__init__.py
--rw-r--r--   0 ethank     (501) staff       (20)     4952 2023-06-28 17:29:10.000000 omicsdata-1.1/src/omicsdata/npz/archive.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.547180 omicsdata-1.1/src/omicsdata/ssm/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/ssm/__init__.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.547669 omicsdata-1.1/src/omicsdata/ssm/_convert/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2024-05-31 15:29:09.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/__init__.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.549553 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/
--rw-r--r--   0 ethank     (501) staff       (20)     6953 2023-06-28 18:17:26.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_base_converter.py
--rw-r--r--   0 ethank     (501) staff       (20)     2659 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_fastclone.py
--rw-r--r--   0 ethank     (501) staff       (20)     2931 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_mobster_tsv.py
--rw-r--r--   0 ethank     (501) staff       (20)     2758 2024-03-15 14:30:29.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_pcvi_tsv.py
--rw-r--r--   0 ethank     (501) staff       (20)     3712 2023-06-28 16:21:44.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_scc_tsv.py
--rw-r--r--   0 ethank     (501) staff       (20)     2419 2024-05-31 14:45:42.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_viber_tsv.py
--rw-r--r--   0 ethank     (501) staff       (20)     6788 2023-06-28 18:32:54.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/vcf_to_ssm.py
--rw-r--r--   0 ethank     (501) staff       (20)     3420 2024-05-31 14:59:22.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/ssm_to_pyclone.py
--rw-r--r--   0 ethank     (501) staff       (20)     5364 2024-05-31 15:50:54.000000 omicsdata-1.1/src/omicsdata/ssm/_convert/ssm_to_viber.py
--rw-r--r--   0 ethank     (501) staff       (20)      918 2023-06-28 18:10:15.000000 omicsdata-1.1/src/omicsdata/ssm/columns.py
--rw-r--r--   0 ethank     (501) staff       (20)     1345 2023-06-28 18:10:10.000000 omicsdata-1.1/src/omicsdata/ssm/common.py
--rw-r--r--   0 ethank     (501) staff       (20)      628 2023-06-28 18:10:22.000000 omicsdata-1.1/src/omicsdata/ssm/constants.py
--rw-r--r--   0 ethank     (501) staff       (20)     5444 2024-05-31 19:28:45.000000 omicsdata-1.1/src/omicsdata/ssm/convert.py
--rw-r--r--   0 ethank     (501) staff       (20)     7916 2024-05-31 14:35:35.000000 omicsdata-1.1/src/omicsdata/ssm/parse.py
--rw-r--r--   0 ethank     (501) staff       (20)     3420 2024-05-31 14:59:22.000000 omicsdata-1.1/src/omicsdata/ssm/ssm_to_pyclone.py
--rw-r--r--   0 ethank     (501) staff       (20)     8255 2024-02-06 20:46:12.000000 omicsdata-1.1/src/omicsdata/ssm/supervariants.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.550576 omicsdata-1.1/src/omicsdata/tree/
--rw-r--r--   0 ethank     (501) staff       (20)        0 2023-07-11 20:46:56.000000 omicsdata-1.1/src/omicsdata/tree/__init__.py
--rw-r--r--   0 ethank     (501) staff       (20)     1645 2023-07-05 16:15:15.000000 omicsdata-1.1/src/omicsdata/tree/adj.py
--rw-r--r--   0 ethank     (501) staff       (20)     1711 2024-05-31 14:37:46.000000 omicsdata-1.1/src/omicsdata/tree/newick.py
--rw-r--r--   0 ethank     (501) staff       (20)      583 2023-06-28 14:55:04.000000 omicsdata-1.1/src/omicsdata/tree/parents.py
-drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-05-31 20:47:01.550745 omicsdata-1.1/src/omicsdata.egg-info/
--rw-r--r--   0 ethank     (501) staff       (20)     1100 2024-05-31 20:47:01.000000 omicsdata-1.1/src/omicsdata.egg-info/PKG-INFO
--rw-r--r--   0 ethank     (501) staff       (20)     1231 2024-05-31 20:47:01.000000 omicsdata-1.1/src/omicsdata.egg-info/SOURCES.txt
--rw-r--r--   0 ethank     (501) staff       (20)        1 2024-05-31 20:47:01.000000 omicsdata-1.1/src/omicsdata.egg-info/dependency_links.txt
--rw-r--r--   0 ethank     (501) staff       (20)       10 2024-05-31 20:47:01.000000 omicsdata-1.1/src/omicsdata.egg-info/top_level.txt
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.739611 omicsdata-1.2/
+-rw-r--r--   0 ethank     (501) staff       (20)     1064 2024-05-31 20:51:22.000000 omicsdata-1.2/LICENSE
+-rw-r--r--   0 ethank     (501) staff       (20)     1100 2024-06-01 15:18:17.739424 omicsdata-1.2/PKG-INFO
+-rw-r--r--   0 ethank     (501) staff       (20)      584 2023-07-11 22:14:55.000000 omicsdata-1.2/README.md
+-rw-r--r--   0 ethank     (501) staff       (20)      583 2024-06-01 15:01:39.000000 omicsdata-1.2/pyproject.toml
+-rw-r--r--   0 ethank     (501) staff       (20)       38 2024-06-01 15:18:17.739658 omicsdata-1.2/setup.cfg
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.730703 omicsdata-1.2/src/
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.731875 omicsdata-1.2/src/omicsdata/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-06-28 14:55:04.000000 omicsdata-1.2/src/omicsdata/__init__.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.732426 omicsdata-1.2/src/omicsdata/cn/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-12-20 16:09:45.000000 omicsdata-1.2/src/omicsdata/cn/estimate.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.732511 omicsdata-1.2/src/omicsdata/csv/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-12-21 15:38:04.000000 omicsdata-1.2/src/omicsdata/csv/parse.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.732689 omicsdata-1.2/src/omicsdata/npz/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-07-04 21:32:15.000000 omicsdata-1.2/src/omicsdata/npz/__init__.py
+-rw-r--r--   0 ethank     (501) staff       (20)     4952 2023-06-28 17:29:10.000000 omicsdata-1.2/src/omicsdata/npz/archive.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.734821 omicsdata-1.2/src/omicsdata/ssm/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-06-28 14:55:04.000000 omicsdata-1.2/src/omicsdata/ssm/__init__.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.735358 omicsdata-1.2/src/omicsdata/ssm/_convert/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2024-05-31 15:29:09.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/__init__.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.737474 omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/
+-rw-r--r--   0 ethank     (501) staff       (20)     6953 2023-06-28 18:17:26.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_base_converter.py
+-rw-r--r--   0 ethank     (501) staff       (20)     2659 2023-06-28 14:55:04.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_fastclone.py
+-rw-r--r--   0 ethank     (501) staff       (20)     2931 2023-06-28 14:55:04.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_mobster_tsv.py
+-rw-r--r--   0 ethank     (501) staff       (20)     2758 2024-03-15 14:30:29.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_pcvi_tsv.py
+-rw-r--r--   0 ethank     (501) staff       (20)     3712 2023-06-28 16:21:44.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_scc_tsv.py
+-rw-r--r--   0 ethank     (501) staff       (20)     2419 2024-05-31 14:45:42.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_viber_tsv.py
+-rw-r--r--   0 ethank     (501) staff       (20)     6788 2023-06-28 18:32:54.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/vcf_to_ssm.py
+-rw-r--r--   0 ethank     (501) staff       (20)     3420 2024-05-31 14:59:22.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/ssm_to_pyclone.py
+-rw-r--r--   0 ethank     (501) staff       (20)     5364 2024-05-31 15:50:54.000000 omicsdata-1.2/src/omicsdata/ssm/_convert/ssm_to_viber.py
+-rw-r--r--   0 ethank     (501) staff       (20)      918 2023-06-28 18:10:15.000000 omicsdata-1.2/src/omicsdata/ssm/columns.py
+-rw-r--r--   0 ethank     (501) staff       (20)     1345 2023-06-28 18:10:10.000000 omicsdata-1.2/src/omicsdata/ssm/common.py
+-rw-r--r--   0 ethank     (501) staff       (20)      628 2023-06-28 18:10:22.000000 omicsdata-1.2/src/omicsdata/ssm/constants.py
+-rw-r--r--   0 ethank     (501) staff       (20)     5444 2024-05-31 19:28:45.000000 omicsdata-1.2/src/omicsdata/ssm/convert.py
+-rw-r--r--   0 ethank     (501) staff       (20)     7916 2024-05-31 14:35:35.000000 omicsdata-1.2/src/omicsdata/ssm/parse.py
+-rw-r--r--   0 ethank     (501) staff       (20)     3420 2024-05-31 14:59:22.000000 omicsdata-1.2/src/omicsdata/ssm/ssm_to_pyclone.py
+-rw-r--r--   0 ethank     (501) staff       (20)     8255 2024-02-06 20:46:12.000000 omicsdata-1.2/src/omicsdata/ssm/supervariants.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.738930 omicsdata-1.2/src/omicsdata/tree/
+-rw-r--r--   0 ethank     (501) staff       (20)        0 2023-07-11 20:46:56.000000 omicsdata-1.2/src/omicsdata/tree/__init__.py
+-rw-r--r--   0 ethank     (501) staff       (20)     1645 2023-07-05 16:15:15.000000 omicsdata-1.2/src/omicsdata/tree/adj.py
+-rw-r--r--   0 ethank     (501) staff       (20)     1684 2024-06-01 14:34:02.000000 omicsdata-1.2/src/omicsdata/tree/neutree.py
+-rw-r--r--   0 ethank     (501) staff       (20)     1711 2024-05-31 14:37:46.000000 omicsdata-1.2/src/omicsdata/tree/newick.py
+-rw-r--r--   0 ethank     (501) staff       (20)      583 2023-06-28 14:55:04.000000 omicsdata-1.2/src/omicsdata/tree/parents.py
+drwxr-xr-x   0 ethank     (501) staff       (20)        0 2024-06-01 15:18:17.739237 omicsdata-1.2/src/omicsdata.egg-info/
+-rw-r--r--   0 ethank     (501) staff       (20)     1100 2024-06-01 15:18:17.000000 omicsdata-1.2/src/omicsdata.egg-info/PKG-INFO
+-rw-r--r--   0 ethank     (501) staff       (20)     1261 2024-06-01 15:18:17.000000 omicsdata-1.2/src/omicsdata.egg-info/SOURCES.txt
+-rw-r--r--   0 ethank     (501) staff       (20)        1 2024-06-01 15:18:17.000000 omicsdata-1.2/src/omicsdata.egg-info/dependency_links.txt
+-rw-r--r--   0 ethank     (501) staff       (20)       10 2024-06-01 15:18:17.000000 omicsdata-1.2/src/omicsdata.egg-info/top_level.txt
```

### Comparing `omicsdata-1.1/LICENSE` & `omicsdata-1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Ethan K.
+Copyright (c) 2024 Ethan K.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `omicsdata-1.1/PKG-INFO` & `omicsdata-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omicsdata
-Version: 1.1
+Version: 1.2
 Summary: A package for manipulating omics data file types
 Author-email: ethanumn <kulma009@umn.edu>
 Project-URL: Homepage, https://github.com/ethanumn/omicsdata
 Project-URL: Bug Tracker, https://github.com/ethanumn/omicsdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `omicsdata-1.1/README.md` & `omicsdata-1.2/README.md`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/pyproject.toml` & `omicsdata-1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "omicsdata"
-version = "1.01"
+version = "1.02"
 authors = [{name="ethanumn", email="kulma009@umn.edu"}]
 description = "A package for manipulating omics data file types"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `omicsdata-1.1/src/omicsdata/npz/archive.py` & `omicsdata-1.2/src/omicsdata/npz/archive.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_base_converter.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_base_converter.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_fastclone.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_fastclone.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_mobster_tsv.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_mobster_tsv.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_pcvi_tsv.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_pcvi_tsv.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_scc_tsv.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_scc_tsv.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/ssm_to_viber_tsv.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/ssm_to_viber_tsv.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/convert_extra/vcf_to_ssm.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/convert_extra/vcf_to_ssm.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/ssm_to_pyclone.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/ssm_to_pyclone.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/_convert/ssm_to_viber.py` & `omicsdata-1.2/src/omicsdata/ssm/_convert/ssm_to_viber.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/columns.py` & `omicsdata-1.2/src/omicsdata/ssm/columns.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/common.py` & `omicsdata-1.2/src/omicsdata/ssm/common.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/constants.py` & `omicsdata-1.2/src/omicsdata/ssm/constants.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/convert.py` & `omicsdata-1.2/src/omicsdata/ssm/convert.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/parse.py` & `omicsdata-1.2/src/omicsdata/ssm/parse.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/ssm_to_pyclone.py` & `omicsdata-1.2/src/omicsdata/ssm/ssm_to_pyclone.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/ssm/supervariants.py` & `omicsdata-1.2/src/omicsdata/ssm/supervariants.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/tree/adj.py` & `omicsdata-1.2/src/omicsdata/tree/adj.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/tree/newick.py` & `omicsdata-1.2/src/omicsdata/tree/newick.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata/tree/parents.py` & `omicsdata-1.2/src/omicsdata/tree/parents.py`

 * *Files identical despite different names*

### Comparing `omicsdata-1.1/src/omicsdata.egg-info/PKG-INFO` & `omicsdata-1.2/src/omicsdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omicsdata
-Version: 1.1
+Version: 1.2
 Summary: A package for manipulating omics data file types
 Author-email: ethanumn <kulma009@umn.edu>
 Project-URL: Homepage, https://github.com/ethanumn/omicsdata
 Project-URL: Bug Tracker, https://github.com/ethanumn/omicsdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `omicsdata-1.1/src/omicsdata.egg-info/SOURCES.txt` & `omicsdata-1.2/src/omicsdata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,10 @@
 src/omicsdata/ssm/_convert/convert_extra/ssm_to_mobster_tsv.py
 src/omicsdata/ssm/_convert/convert_extra/ssm_to_pcvi_tsv.py
 src/omicsdata/ssm/_convert/convert_extra/ssm_to_scc_tsv.py
 src/omicsdata/ssm/_convert/convert_extra/ssm_to_viber_tsv.py
 src/omicsdata/ssm/_convert/convert_extra/vcf_to_ssm.py
 src/omicsdata/tree/__init__.py
 src/omicsdata/tree/adj.py
+src/omicsdata/tree/neutree.py
 src/omicsdata/tree/newick.py
 src/omicsdata/tree/parents.py
```

