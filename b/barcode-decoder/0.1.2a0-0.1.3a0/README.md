# Comparing `tmp/barcode_decoder-0.1.2a0.tar.gz` & `tmp/barcode_decoder-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barcode_decoder-0.1.2a0.tar", last modified: Sat Jun  1 13:00:39 2024, max compression
+gzip compressed data, was "barcode_decoder-0.1.3a0.tar", last modified: Sat Jun  1 13:11:01 2024, max compression
```

## Comparing `barcode_decoder-0.1.2a0.tar` & `barcode_decoder-0.1.3a0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:39.944010 barcode_decoder-0.1.2a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:39.940010 barcode_decoder-0.1.2a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:39.940010 barcode_decoder-0.1.2a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-06-01 13:00:39.944010 barcode_decoder-0.1.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-06-01 13:00:39.944010 barcode_decoder-0.1.2a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:39.940010 barcode_decoder-0.1.2a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:39.944010 barcode_decoder-0.1.2a0/src/barcode_decoder/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/barcode_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/digi_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/farnell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/mouser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/tme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/src/barcode_decoder/wurth_elektronik.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:39.944010 barcode_decoder-0.1.2a0/src/barcode_decoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-06-01 13:00:39.000000 barcode_decoder-0.1.2a0/src/barcode_decoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-06-01 13:00:39.000000 barcode_decoder-0.1.2a0/src/barcode_decoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:00:39.000000 barcode_decoder-0.1.2a0/src/barcode_decoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 13:00:39.000000 barcode_decoder-0.1.2a0/src/barcode_decoder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 13:00:39.000000 barcode_decoder-0.1.2a0/src/barcode_decoder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:39.944010 barcode_decoder-0.1.2a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/tests/test_digi_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/tests/test_farnell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/tests/test_mouser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/tests/test_tme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-06-01 13:00:32.000000 barcode_decoder-0.1.2a0/tests/test_wurth_elektronik.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:01.295245 barcode_decoder-0.1.3a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:01.287245 barcode_decoder-0.1.3a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:01.291245 barcode_decoder-0.1.3a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-06-01 13:11:01.295245 barcode_decoder-0.1.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-06-01 13:11:01.295245 barcode_decoder-0.1.3a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:01.291245 barcode_decoder-0.1.3a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:01.291245 barcode_decoder-0.1.3a0/src/barcode_decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/barcode_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/digi_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/farnell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/mouser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/tme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/src/barcode_decoder/wurth_elektronik.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:01.295245 barcode_decoder-0.1.3a0/src/barcode_decoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-06-01 13:11:01.000000 barcode_decoder-0.1.3a0/src/barcode_decoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-06-01 13:11:01.000000 barcode_decoder-0.1.3a0/src/barcode_decoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:11:01.000000 barcode_decoder-0.1.3a0/src/barcode_decoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 13:11:01.000000 barcode_decoder-0.1.3a0/src/barcode_decoder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 13:11:01.000000 barcode_decoder-0.1.3a0/src/barcode_decoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:11:01.295245 barcode_decoder-0.1.3a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/tests/test_digi_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/tests/test_farnell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/tests/test_mouser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/tests/test_tme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-06-01 13:10:54.000000 barcode_decoder-0.1.3a0/tests/test_wurth_elektronik.py
```

### Comparing `barcode_decoder-0.1.2a0/.github/workflows/tests.yml` & `barcode_decoder-0.1.3a0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/.gitignore` & `barcode_decoder-0.1.3a0/.gitignore`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/LICENSE` & `barcode_decoder-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/PKG-INFO` & `barcode_decoder-0.1.3a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 Metadata-Version: 2.1
 Name: barcode_decoder
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: Library to convert electronic components distributors  barcodes and QR codes to unified format. Library allows to extract information about: partnumber, ordered quantity, order number, part LOT and origin.
 Home-page: https://github.com/partmanager/barcode-decoder
 Author: sakoPO
 Project-URL: Bug Tracker, https://github.com/partmanager/barcode-decoder/issues
 Project-URL: Changelog, https://github.com/partmanager/barcode-decoder/releases
 Project-URL: Source Code, https://github.com/partmanager/barcode-decoder
 Project-URL: Documentation, https://partmanager.github.io/barcode-decoder
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # barcode-decoder
 Barcode and QR decoder
 
 Simple application for decoding barcodes and QR codes from various distributors and converting them to standardized output.
 
+## Usage
+### Installation
+`pip install barcode_decoder`
+
+### Command line usage
+`$ barcode_decoder`
+
+### Usage as library
+```
+from barcode_decoder import barcode_decoder
+
+result = barcode_decoder.decode(barcode_string)
+```
+
 ### Currently supported distributors:
 - Farnell
 - Mouser
 - TME
 - Wurth Elektronik
 
 ### Setting your scaner
```

### Comparing `barcode_decoder-0.1.2a0/setup.cfg` & `barcode_decoder-0.1.3a0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = barcode_decoder
 description = Library to convert electronic components distributors  barcodes and QR codes to unified format. Library allows to extract information about: partnumber, ordered quantity, order number, part LOT and origin.
-long_description_content_type = text/x-rst
+long_description_content_type = text/markdown
 long_description = file: README.md
 author = sakoPO
 readme = "README"
 url = https://github.com/partmanager/barcode-decoder
 project_urls = 
 	Bug Tracker = https://github.com/partmanager/barcode-decoder/issues
 	Changelog = https://github.com/partmanager/barcode-decoder/releases
```

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder/barcode_decoder.py` & `barcode_decoder-0.1.3a0/src/barcode_decoder/barcode_decoder.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder/digi_key.py` & `barcode_decoder-0.1.3a0/src/barcode_decoder/digi_key.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder/farnell.py` & `barcode_decoder-0.1.3a0/src/barcode_decoder/farnell.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder/mouser.py` & `barcode_decoder-0.1.3a0/src/barcode_decoder/mouser.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder/result.py` & `barcode_decoder-0.1.3a0/src/barcode_decoder/result.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder/scanner.py` & `barcode_decoder-0.1.3a0/src/barcode_decoder/scanner.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder/tme.py` & `barcode_decoder-0.1.3a0/src/barcode_decoder/tme.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder/wurth_elektronik.py` & `barcode_decoder-0.1.3a0/src/barcode_decoder/wurth_elektronik.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder.egg-info/PKG-INFO` & `barcode_decoder-0.1.3a0/src/barcode_decoder.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 Metadata-Version: 2.1
 Name: barcode_decoder
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: Library to convert electronic components distributors  barcodes and QR codes to unified format. Library allows to extract information about: partnumber, ordered quantity, order number, part LOT and origin.
 Home-page: https://github.com/partmanager/barcode-decoder
 Author: sakoPO
 Project-URL: Bug Tracker, https://github.com/partmanager/barcode-decoder/issues
 Project-URL: Changelog, https://github.com/partmanager/barcode-decoder/releases
 Project-URL: Source Code, https://github.com/partmanager/barcode-decoder
 Project-URL: Documentation, https://partmanager.github.io/barcode-decoder
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # barcode-decoder
 Barcode and QR decoder
 
 Simple application for decoding barcodes and QR codes from various distributors and converting them to standardized output.
 
+## Usage
+### Installation
+`pip install barcode_decoder`
+
+### Command line usage
+`$ barcode_decoder`
+
+### Usage as library
+```
+from barcode_decoder import barcode_decoder
+
+result = barcode_decoder.decode(barcode_string)
+```
+
 ### Currently supported distributors:
 - Farnell
 - Mouser
 - TME
 - Wurth Elektronik
 
 ### Setting your scaner
```

### Comparing `barcode_decoder-0.1.2a0/src/barcode_decoder.egg-info/SOURCES.txt` & `barcode_decoder-0.1.3a0/src/barcode_decoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/tests/test_digi_key.py` & `barcode_decoder-0.1.3a0/tests/test_digi_key.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/tests/test_farnell.py` & `barcode_decoder-0.1.3a0/tests/test_farnell.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/tests/test_mouser.py` & `barcode_decoder-0.1.3a0/tests/test_mouser.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/tests/test_tme.py` & `barcode_decoder-0.1.3a0/tests/test_tme.py`

 * *Files identical despite different names*

### Comparing `barcode_decoder-0.1.2a0/tests/test_wurth_elektronik.py` & `barcode_decoder-0.1.3a0/tests/test_wurth_elektronik.py`

 * *Files identical despite different names*

