# Comparing `tmp/sportident-1.2.7.tar.gz` & `tmp/sportident-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportident-1.2.7.tar", max compression
+gzip compressed data, was "sportident-1.2.8.tar", max compression
```

## Comparing `sportident-1.2.7.tar` & `sportident-1.2.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35068 2024-03-27 08:54:03.121216 sportident-1.2.7/LICENSE
--rw-r--r--   0        0        0     1373 2024-03-27 08:54:03.121216 sportident-1.2.7/README.md
--rw-r--r--   0        0        0     2450 2024-03-27 08:54:03.121216 sportident-1.2.7/pyproject.toml
--rw-r--r--   0        0        0    56658 2024-03-27 08:54:03.121216 sportident-1.2.7/sportident.py
--rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 sportident-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0    35068 2024-06-01 20:37:32.600429 sportident-1.2.8/LICENSE
+-rw-r--r--   0        0        0     1373 2024-06-01 20:37:32.600429 sportident-1.2.8/README.md
+-rw-r--r--   0        0        0     2450 2024-06-01 20:37:32.600429 sportident-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0    56659 2024-06-01 20:37:32.600429 sportident-1.2.8/sportident.py
+-rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 sportident-1.2.8/PKG-INFO
```

### Comparing `sportident-1.2.7/LICENSE` & `sportident-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sportident-1.2.7/README.md` & `sportident-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `sportident-1.2.7/pyproject.toml` & `sportident-1.2.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.7"
+version = "1.2.8"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "sportident"
-version = "1.2.7"
+version = "1.2.8"
 description = "Python module to communicate with SportIdent main stations"
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "GPLv3+"
 readme = "README.md"
 repository = "https://github.com/sportorg/sireader"
 homepage = "https://github.com/sportorg/sireader"
 keywords = ["sportident", "orienteering", "sportorg"]
```

### Comparing `sportident-1.2.7/sportident.py` & `sportident-1.2.8/sportident.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
             "CTD": 8,
             "CT": 10,
             "LTD": None,
             "LT": None,
             "RC": 22,
             "P1": 128,  # would be 512 if all blocks were read, but blocks 1-3 are skipped on readout
             "PL": 4,
-            "PM": 64,
+            "PM": 128,
             "PTD": 0,  # Day of week byte, SI6 and newer
             "CN": 1,
             "PTH": 2,
             "PTL": 3,
             "BC": 8,
         },
         # tCard support
```

### Comparing `sportident-1.2.7/PKG-INFO` & `sportident-1.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sportident
-Version: 1.2.7
+Version: 1.2.8
 Summary: Python module to communicate with SportIdent main stations
 Home-page: https://github.com/sportorg/sireader
 License: GPLv3+
 Keywords: sportident,orienteering,sportorg
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

