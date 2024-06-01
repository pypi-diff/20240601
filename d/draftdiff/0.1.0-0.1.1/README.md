# Comparing `tmp/draftdiff-0.1.0.tar.gz` & `tmp/draftdiff-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draftdiff-0.1.0.tar", max compression
+gzip compressed data, was "draftdiff-0.1.1.tar", max compression
```

## Comparing `draftdiff-0.1.0.tar` & `draftdiff-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2024-05-30 22:59:22.761225 draftdiff-0.1.0/LICENSE
--rw-r--r--   0        0        0     2225 2024-05-30 22:59:22.761225 draftdiff-0.1.0/README.md
--rw-r--r--   0        0        0      887 2024-05-30 22:59:22.765225 draftdiff-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4382 2024-05-30 22:59:22.765225 draftdiff-0.1.0/src/aggregation.py
--rw-r--r--   0        0        0     7899 2024-05-30 22:59:22.765225 draftdiff-0.1.0/src/dotabuff.py
--rw-r--r--   0        0        0     4626 2024-05-30 22:59:22.765225 draftdiff-0.1.0/src/dotaherocounterpull.py
--rw-r--r--   0        0        0     1145 2024-05-30 22:59:22.765225 draftdiff-0.1.0/src/sheets.py
--rw-r--r--   0        0        0     4912 2024-05-30 22:59:22.765225 draftdiff-0.1.0/src/stratz.py
--rw-r--r--   0        0        0     2445 2024-05-30 22:59:22.765225 draftdiff-0.1.0/src/writetosheets.py
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 draftdiff-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-06-01 00:41:46.117215 draftdiff-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2225 2024-06-01 00:41:46.117215 draftdiff-0.1.1/README.md
+-rw-r--r--   0        0        0      887 2024-06-01 00:41:46.117215 draftdiff-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4445 2024-06-01 00:41:46.117215 draftdiff-0.1.1/src/aggregation.py
+-rw-r--r--   0        0        0     7899 2024-06-01 00:41:46.117215 draftdiff-0.1.1/src/dotabuff.py
+-rw-r--r--   0        0        0     4626 2024-06-01 00:41:46.117215 draftdiff-0.1.1/src/dotaherocounterpull.py
+-rw-r--r--   0        0        0     1145 2024-06-01 00:41:46.117215 draftdiff-0.1.1/src/sheets.py
+-rw-r--r--   0        0        0     4912 2024-06-01 00:41:46.117215 draftdiff-0.1.1/src/stratz.py
+-rw-r--r--   0        0        0     2445 2024-06-01 00:41:46.117215 draftdiff-0.1.1/src/writetosheets.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 draftdiff-0.1.1/PKG-INFO
```

### Comparing `draftdiff-0.1.0/LICENSE` & `draftdiff-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `draftdiff-0.1.0/README.md` & `draftdiff-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `draftdiff-0.1.0/pyproject.toml` & `draftdiff-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "draftdiff"
-version = "0.1.0"
+version = "0.1.1"
 description = "creating dota2 counterpicker"
 authors = ["Jeff", "Luke"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "src", from = "." }
 ]
 
 [tool.poetry.dependencies]
-python = "3.12.3"
+python = "3.11.0"
 beautifulsoup4 = "^4.12.3"
 pandas = "^2.2.1"
 loguru = "^0.7.2"
 tqdm = "^4.66.2"
 requests = "^2.31.0"
 google-api-python-client = "^2.125.0"
 oauth2client = "^4.1.3"
```

### Comparing `draftdiff-0.1.0/src/aggregation.py` & `draftdiff-0.1.1/src/aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,18 @@
     token = os.environ["STRATZ_API_TOKEN"]
 
     build_target_heroes_counter_heroes_df_for_dotabuff_id_in_last_n_days(
         token, "181567803", 30
     )
 
 
+def databricks_print_test():
+    print("draftdiff imported")
+
+
 def main():
     import doctest
 
     doctest.testmod()
 
 
 if __name__ == "__main__":
```

### Comparing `draftdiff-0.1.0/src/dotabuff.py` & `draftdiff-0.1.1/src/dotabuff.py`

 * *Files identical despite different names*

### Comparing `draftdiff-0.1.0/src/dotaherocounterpull.py` & `draftdiff-0.1.1/src/dotaherocounterpull.py`

 * *Files identical despite different names*

### Comparing `draftdiff-0.1.0/src/sheets.py` & `draftdiff-0.1.1/src/sheets.py`

 * *Files identical despite different names*

### Comparing `draftdiff-0.1.0/src/stratz.py` & `draftdiff-0.1.1/src/stratz.py`

 * *Files identical despite different names*

### Comparing `draftdiff-0.1.0/src/writetosheets.py` & `draftdiff-0.1.1/src/writetosheets.py`

 * *Files identical despite different names*

### Comparing `draftdiff-0.1.0/PKG-INFO` & `draftdiff-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: draftdiff
-Version: 0.1.0
+Version: 0.1.1
 Summary: creating dota2 counterpicker
 License: MIT
 Author: Jeff
-Requires-Python: ==3.12.3
+Requires-Python: ==3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: google-api-python-client (>=2.125.0,<3.0.0)
 Requires-Dist: google-auth (>=2.29.0,<3.0.0)
 Requires-Dist: gspread (>=6.1.0,<7.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
```

