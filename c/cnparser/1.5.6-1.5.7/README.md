# Comparing `tmp/cnparser-1.5.6.tar.gz` & `tmp/cnparser-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnparser-1.5.6.tar", last modified: Sun May 19 08:17:56 2024, max compression
+gzip compressed data, was "cnparser-1.5.7.tar", last modified: Sat Jun  1 13:08:48 2024, max compression
```

## Comparing `cnparser-1.5.6.tar` & `cnparser-1.5.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:17:56.185166 cnparser-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-19 08:17:42.000000 cnparser-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-19 08:17:56.185166 cnparser-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-19 08:17:42.000000 cnparser-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:17:56.181166 cnparser-1.5.6/cnparser/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:17:56.185166 cnparser-1.5.6/cnparser/config/
--rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/config/eng_kana.json
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/config/file_id.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/config/header.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/config/kind.json
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/config/legal_entity.json
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-19 08:17:42.000000 cnparser-1.5.6/cnparser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:17:56.185166 cnparser-1.5.6/cnparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-19 08:17:56.000000 cnparser-1.5.6/cnparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-19 08:17:56.000000 cnparser-1.5.6/cnparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:17:56.000000 cnparser-1.5.6/cnparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 08:17:56.000000 cnparser-1.5.6/cnparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 08:17:56.000000 cnparser-1.5.6/cnparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:17:56.185166 cnparser-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-19 08:17:42.000000 cnparser-1.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:17:56.185166 cnparser-1.5.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:17:42.000000 cnparser-1.5.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-19 08:17:42.000000 cnparser-1.5.6/test/test_enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-19 08:17:42.000000 cnparser-1.5.6/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:08:48.857650 cnparser-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-06-01 13:08:37.000000 cnparser-1.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-06-01 13:08:48.857650 cnparser-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-06-01 13:08:37.000000 cnparser-1.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:08:48.849650 cnparser-1.5.7/cnparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:08:48.853650 cnparser-1.5.7/cnparser/config/
+-rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/config/eng_kana.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/config/file_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/config/header.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/config/kind.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/config/legal_entity.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-06-01 13:08:37.000000 cnparser-1.5.7/cnparser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:08:48.853650 cnparser-1.5.7/cnparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-06-01 13:08:48.000000 cnparser-1.5.7/cnparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-01 13:08:48.000000 cnparser-1.5.7/cnparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:08:48.000000 cnparser-1.5.7/cnparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 13:08:48.000000 cnparser-1.5.7/cnparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 13:08:48.000000 cnparser-1.5.7/cnparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:08:48.857650 cnparser-1.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-06-01 13:08:37.000000 cnparser-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:08:48.853650 cnparser-1.5.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:08:37.000000 cnparser-1.5.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-06-01 13:08:37.000000 cnparser-1.5.7/test/test_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-06-01 13:08:37.000000 cnparser-1.5.7/test/test_load.py
```

### Comparing `cnparser-1.5.6/LICENSE` & `cnparser-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/PKG-INFO` & `cnparser-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.6
+Version: 1.5.7
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `cnparser-1.5.6/README.md` & `cnparser-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/cnparser/config/eng_kana.json` & `cnparser-1.5.7/cnparser/config/eng_kana.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/cnparser/config/header.json` & `cnparser-1.5.7/cnparser/config/header.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/cnparser/config/legal_entity.json` & `cnparser-1.5.7/cnparser/config/legal_entity.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/cnparser/enrich.py` & `cnparser-1.5.7/cnparser/enrich.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/cnparser/load.py` & `cnparser-1.5.7/cnparser/load.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/cnparser/utility.py` & `cnparser-1.5.7/cnparser/utility.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/cnparser.egg-info/PKG-INFO` & `cnparser-1.5.7/cnparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.6
+Version: 1.5.7
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `cnparser-1.5.6/setup.py` & `cnparser-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cnparser',
-    version='1.5.6',
+    version='1.5.7',
     author='new-village',
     url='https://github.com/new-village/cnparser',
     description='cnparser is a parser library of Corporate Number Publication Site data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPLv3+',
     install_requires=['requests', 'bs4', 'pandas', 'pandarallel', 'pykakasi'],
```

### Comparing `cnparser-1.5.6/test/test_enrich.py` & `cnparser-1.5.7/test/test_enrich.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.6/test/test_load.py` & `cnparser-1.5.7/test/test_load.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     def test_load(self):
         """Test the load function with 'Shimane' prefecture."""
         result = load(prefecture='Shimane')
 
         # Validate results
         self.assertIsInstance(result, pd.DataFrame)
         self.assertEqual(list(result.columns), self.expected_columns)
-        self.assertEqual(len(result), 22427)
-        self.assertEqual(result.iloc[7662]['corporate_number'], '4280001003400')
-        self.assertEqual(result.iloc[12517]['name'], '株式会社山陰合同銀行')
+        self.assertEqual(len(result), 22469)
+        self.assertEqual(result.iloc[7662]['corporate_number'], '4280001003202')
+        self.assertEqual(result.iloc[12517]['name'], 'グローバス株式会社')
 
     def test_read_csv(self):
         """Test the read_csv function with a specific CSV file."""
         result = read_csv('./test/data/31_tottori_test_20240329.csv')
 
         # Validate results
         self.assertIsInstance(result, pd.DataFrame)
```

