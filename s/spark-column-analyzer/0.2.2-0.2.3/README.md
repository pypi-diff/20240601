# Comparing `tmp/spark_column_analyzer-0.2.2.tar.gz` & `tmp/spark-column-analyzer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_column_analyzer-0.2.2.tar", last modified: Mon May 20 22:13:05 2024, max compression
+gzip compressed data, was "spark-column-analyzer-0.2.3.tar", last modified: Sat Jun  1 13:09:39 2024, max compression
```

## Comparing `spark_column_analyzer-0.2.2.tar` & `spark-column-analyzer-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-05-20 22:13:05.282390 spark_column_analyzer-0.2.2/
--rw-r--r--   0 hduser    (1005) hadoop    (1005)        0 2024-05-17 08:32:37.000000 spark_column_analyzer-0.2.2/LICENSE
--rw-r--r--   0 hduser    (1005) hadoop    (1005)       67 2024-05-20 15:44:02.000000 spark_column_analyzer-0.2.2/MANIFEST.in
--rw-r--r--   0 hduser    (1005) hadoop    (1005)      110 2024-05-20 22:13:05.282390 spark_column_analyzer-0.2.2/PKG-INFO
--rw-r--r--   0 hduser    (1005) hadoop    (1005)     1760 2024-05-17 18:54:19.000000 spark_column_analyzer-0.2.2/README.md
--rw-r--r--   0 hduser    (1005) hadoop    (1005)       38 2024-05-20 22:13:05.282390 spark_column_analyzer-0.2.2/setup.cfg
--rw-r--r--   0 hduser    (1005) hadoop    (1005)      279 2024-05-20 22:11:54.000000 spark_column_analyzer-0.2.2/setup.py
-drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-05-20 22:13:05.280390 spark_column_analyzer-0.2.2/src/
-drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-05-20 22:13:05.280390 spark_column_analyzer-0.2.2/src/spark_column_analyzer/
--rw-r--r--   0 hduser    (1005) hadoop    (1005)        0 2024-05-20 22:10:08.000000 spark_column_analyzer-0.2.2/src/spark_column_analyzer/__init__.py
--rw-r--r--   0 hduser    (1005) hadoop    (1005)     4702 2024-05-17 13:48:38.000000 spark_column_analyzer-0.2.2/src/spark_column_analyzer/column_analyzer.py
-drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-05-20 22:13:05.282390 spark_column_analyzer-0.2.2/src/spark_column_analyzer.egg-info/
--rw-r--r--   0 hduser    (1005) hadoop    (1005)      110 2024-05-20 22:13:05.000000 spark_column_analyzer-0.2.2/src/spark_column_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 hduser    (1005) hadoop    (1005)      436 2024-05-20 22:13:05.000000 spark_column_analyzer-0.2.2/src/spark_column_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 hduser    (1005) hadoop    (1005)        1 2024-05-20 22:13:05.000000 spark_column_analyzer-0.2.2/src/spark_column_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 hduser    (1005) hadoop    (1005)        1 2024-05-20 22:13:05.000000 spark_column_analyzer-0.2.2/src/spark_column_analyzer.egg-info/not-zip-safe
--rw-r--r--   0 hduser    (1005) hadoop    (1005)        8 2024-05-20 22:13:05.000000 spark_column_analyzer-0.2.2/src/spark_column_analyzer.egg-info/requires.txt
--rw-r--r--   0 hduser    (1005) hadoop    (1005)       22 2024-05-20 22:13:05.000000 spark_column_analyzer-0.2.2/src/spark_column_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-05-20 22:13:05.281390 spark_column_analyzer-0.2.2/tests/
--rw-r--r--   0 hduser    (1005) hadoop    (1005)     1746 2024-05-17 14:57:55.000000 spark_column_analyzer-0.2.2/tests/test_analyzer.py
+drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-06-01 13:09:39.616485 spark-column-analyzer-0.2.3/
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)        0 2024-05-17 08:32:37.000000 spark-column-analyzer-0.2.3/LICENSE
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)       67 2024-05-20 15:44:02.000000 spark-column-analyzer-0.2.3/MANIFEST.in
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)     3133 2024-06-01 13:09:39.616485 spark-column-analyzer-0.2.3/PKG-INFO
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)     2478 2024-06-01 12:07:56.000000 spark-column-analyzer-0.2.3/README.md
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)       38 2024-06-01 13:09:39.616485 spark-column-analyzer-0.2.3/setup.cfg
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)      910 2024-06-01 12:49:20.000000 spark-column-analyzer-0.2.3/setup.py
+drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-06-01 13:09:39.614485 spark-column-analyzer-0.2.3/spark_column_analyzer.egg-info/
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)     3133 2024-06-01 13:09:39.000000 spark-column-analyzer-0.2.3/spark_column_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)      431 2024-06-01 13:09:39.000000 spark-column-analyzer-0.2.3/spark_column_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)        1 2024-06-01 13:09:39.000000 spark-column-analyzer-0.2.3/spark_column_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)       33 2024-06-01 13:09:39.000000 spark-column-analyzer-0.2.3/spark_column_analyzer.egg-info/requires.txt
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)       10 2024-06-01 13:09:39.000000 spark-column-analyzer-0.2.3/spark_column_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-06-01 13:09:39.615485 spark-column-analyzer-0.2.3/src/
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)        0 2024-05-17 08:32:37.000000 spark-column-analyzer-0.2.3/src/__init__.py
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)      913 2024-05-31 09:36:03.000000 spark-column-analyzer-0.2.3/src/load_data.py
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)     2145 2024-05-26 20:35:15.000000 spark-column-analyzer-0.2.3/src/main.py
+drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-06-01 13:09:39.615485 spark-column-analyzer-0.2.3/src/spark_column_analyzer/
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)        0 2024-05-20 22:10:08.000000 spark-column-analyzer-0.2.3/src/spark_column_analyzer/__init__.py
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)     6015 2024-06-01 11:52:22.000000 spark-column-analyzer-0.2.3/src/spark_column_analyzer/column_analyzer.py
+drwxr-xr-x   0 hduser    (1005) hadoop    (1005)        0 2024-06-01 13:09:39.615485 spark-column-analyzer-0.2.3/tests/
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)        0 2024-05-17 14:34:11.000000 spark-column-analyzer-0.2.3/tests/__init__.py
+-rw-r--r--   0 hduser    (1005) hadoop    (1005)     1392 2024-05-21 12:51:19.000000 spark-column-analyzer-0.2.3/tests/test_analyzer.py
```

### Comparing `spark_column_analyzer-0.2.2/README.md` & `spark-column-analyzer-0.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,39 @@
+Metadata-Version: 2.1
+Name: spark-column-analyzer
+Version: 0.2.3
+Summary: A package for analyzing Spark DataFrame columns
+Home-page: https://github.com/michTalebzadeh/spark_column_analyzer
+Author: Mich Talebzadeh
+Author-email: mich.talebzadeh@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # Spark Column Analyzer
 
 ## Overview
 
-Spark Column Analyzer is a Python package that provides functions for analyzing columns in PySpark DataFrames. It calculates various statistics such as null count, null percentage, distinct count, and distinct percentage for each column.
+Spark Column Analyzer is a Python package that provides functions for analyzing columns in PySpark DataFrames. It calculates various statistics such as null count, null percentage, distinct count, distinct percentage, min_value, max_value, avg_value and historams
+for each column. It also create a plot and saves it to the directory you are running the code from.
 
 ## Installation
 
 You can install Spark Column Analyzer using pip:
 
+```sh
 pip install spark-column-analyzer
 
-makefile
-Copy code
 
 ## Usage
 
 ### Analyzing Columns
 
 To analyze columns in a PySpark DataFrame, you can use the `analyze_column` function provided by the package. Here's an example:
 
@@ -41,30 +58,58 @@
 # Analyze a specific column
 result = analyze_column(df, "Value")
 print(result)
 Running Tests
 To run tests for Spark Column Analyzer, follow these steps:
 
 Clone the repository:
-bash
-Copy code
 git clone https://github.com/michTalebzadeh/spark_column_analyzer.git
 Navigate to the project directory:
-bash
-Copy code
 cd spark_column_analyzer
 Install the dependencies:
-Copy code
 pip install -r requirements.txt
 Run the tests:
-Copy code
 python -m unittest discover tests
 Contributing
 If you'd like to contribute to Spark Column Analyzer, please open an issue or submit a pull request on GitHub.
 
 License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 vbnet
-Copy code
 
-Feel free to customize this template according to your project's specific details and require
+Feel free to customize this template according to your project's specific details and require
+
+Example
+
+Doing analysis for column Postcode
+
+Json formatted output
+
+{
+    "PricePaid": {
+        "exists": true,
+        "num_rows": 1819,
+        "data_type": "int",
+        "null_count": 0,
+        "null_percentage": 0.0,
+        "distinct_count": 1133,
+        "distinct_percentage": 62.29,
+        "min_value": 10000001,
+        "max_value": 448500000,
+        "avg_value": 32620476.65,
+        "histogram": {
+            "bins": [
+                10000001.0,
+                14216347.144230768,
+               448500000.0,
+
+            ],
+            "counts": [
+                468,
+                286,
+                258,
+
+            ]
+        }
+    }
+}
```

### Comparing `spark_column_analyzer-0.2.2/tests/test_analyzer.py` & `spark-column-analyzer-0.2.3/tests/test_analyzer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import sys
 import unittest
 from pyspark.sql import SparkSession
-sys.path.append('/home/hduser/dba/bin/python/spark_column_analyzer/')
-sys.path.append('/home/hduser/dba/bin/python/spark_column_analyzer/conf')
-sys.path.append('/home/hduser/dba/bin/python/spark_column_analyzer/othermisc')
-sys.path.append('/home/hduser/dba/bin/python/spark_column_analyzer/src')
-sys.path.append('/home/hduser/dba/bin/python/spark_column_analyzer/tests')
-
-from src.column_analyzer import analyze_column
+from spark_column_analyzer.column_analyzer import analyze_column
 
 class TestColumnAnalyzer(unittest.TestCase):
     def setUp(self):
         # Initialize SparkSession for testing
         self.spark = SparkSession.builder \
             .appName("test_analyzer") \
             .master("local[2]") \
```

