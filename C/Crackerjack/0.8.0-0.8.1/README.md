# Comparing `tmp/crackerjack-0.8.0.tar.gz` & `tmp/crackerjack-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.8.0.tar", last modified: Sat Jun  1 11:10:25 2024, max compression
+gzip compressed data, was "crackerjack-0.8.1.tar", last modified: Sat Jun  1 14:15:39 2024, max compression
```

## Comparing `crackerjack-0.8.0.tar` & `crackerjack-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.8.0/LICENSE
--rw-r--r--   0        0        0     6261 2024-06-01 11:05:46.530942 crackerjack-0.8.0/README.md
--rw-r--r--   0        0        0      197 2024-06-01 11:09:57.660429 crackerjack-0.8.0/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2024-06-01 11:09:57.667134 crackerjack-0.8.0/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2264 2024-06-01 11:09:57.663819 crackerjack-0.8.0/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.8.0/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0      248 2024-01-06 07:37:34.391552 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.11/3256171999636029978
--rw-r--r--   0        0        0      248 2024-01-24 12:53:52.172690 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.14/602324811142551221
--rw-r--r--   0        0        0      248 2023-11-06 09:35:44.665597 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.4/10355199064880463147
--rw-r--r--   0        0        0      248 2023-11-30 19:47:12.985430 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.6/15140459877605758699
--rw-r--r--   0        0        0      248 2023-12-09 08:32:10.697985 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.7/1790508110482614856
--rw-r--r--   0        0        0      248 2023-12-25 16:57:47.788926 crackerjack-0.8.0/crackerjack/.ruff_cache/0.1.9/17041001205004563469
--rw-r--r--   0        0        0      248 2024-02-04 19:42:45.746383 crackerjack-0.8.0/crackerjack/.ruff_cache/0.2.0/10047773857155985907
--rw-r--r--   0        0        0      248 2024-02-08 21:29:34.013736 crackerjack-0.8.0/crackerjack/.ruff_cache/0.2.1/8522267973936635051
--rw-r--r--   0        0        0      248 2024-02-19 14:09:40.345898 crackerjack-0.8.0/crackerjack/.ruff_cache/0.2.2/18053836298936336950
--rw-r--r--   0        0        0      248 2024-03-02 11:27:50.943765 crackerjack-0.8.0/crackerjack/.ruff_cache/0.3.0/12548816621480535786
--rw-r--r--   0        0        0      248 2024-03-18 07:54:31.415399 crackerjack-0.8.0/crackerjack/.ruff_cache/0.3.3/11081883392474770722
--rw-r--r--   0        0        0      248 2024-03-27 22:01:10.025644 crackerjack-0.8.0/crackerjack/.ruff_cache/0.3.4/676973378459347183
--rw-r--r--   0        0        0      248 2024-04-02 07:04:47.506968 crackerjack-0.8.0/crackerjack/.ruff_cache/0.3.5/16311176246009842383
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.8.0/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.8.0/crackerjack/__init__.py
--rw-r--r--   0        0        0     1767 2024-06-01 09:32:10.833253 crackerjack-0.8.0/crackerjack/__main__.py
--rw-r--r--   0        0        0     7906 2024-06-01 10:39:46.039848 crackerjack-0.8.0/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     2776 2024-06-01 11:09:59.406480 crackerjack-0.8.0/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2775 2024-06-01 11:10:25.704923 crackerjack-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7760 1970-01-01 00:00:00.000000 crackerjack-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.8.1/LICENSE
+-rw-r--r--   0        0        0     6261 2024-06-01 11:05:46.530942 crackerjack-0.8.1/README.md
+-rw-r--r--   0        0        0      197 2024-06-01 14:15:14.232808 crackerjack-0.8.1/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2024-06-01 14:15:14.239850 crackerjack-0.8.1/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2264 2024-06-01 14:15:14.236144 crackerjack-0.8.1/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.8.1/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0      248 2024-01-06 07:37:34.391552 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.11/3256171999636029978
+-rw-r--r--   0        0        0      248 2024-01-24 12:53:52.172690 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.14/602324811142551221
+-rw-r--r--   0        0        0      248 2023-11-06 09:35:44.665597 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.4/10355199064880463147
+-rw-r--r--   0        0        0      248 2023-11-30 19:47:12.985430 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.6/15140459877605758699
+-rw-r--r--   0        0        0      248 2023-12-09 08:32:10.697985 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.7/1790508110482614856
+-rw-r--r--   0        0        0      248 2023-12-25 16:57:47.788926 crackerjack-0.8.1/crackerjack/.ruff_cache/0.1.9/17041001205004563469
+-rw-r--r--   0        0        0      248 2024-02-04 19:42:45.746383 crackerjack-0.8.1/crackerjack/.ruff_cache/0.2.0/10047773857155985907
+-rw-r--r--   0        0        0      248 2024-02-08 21:29:34.013736 crackerjack-0.8.1/crackerjack/.ruff_cache/0.2.1/8522267973936635051
+-rw-r--r--   0        0        0      248 2024-02-19 14:09:40.345898 crackerjack-0.8.1/crackerjack/.ruff_cache/0.2.2/18053836298936336950
+-rw-r--r--   0        0        0      248 2024-03-02 11:27:50.943765 crackerjack-0.8.1/crackerjack/.ruff_cache/0.3.0/12548816621480535786
+-rw-r--r--   0        0        0      248 2024-03-18 07:54:31.415399 crackerjack-0.8.1/crackerjack/.ruff_cache/0.3.3/11081883392474770722
+-rw-r--r--   0        0        0      248 2024-03-27 22:01:10.025644 crackerjack-0.8.1/crackerjack/.ruff_cache/0.3.4/676973378459347183
+-rw-r--r--   0        0        0      248 2024-04-02 07:04:47.506968 crackerjack-0.8.1/crackerjack/.ruff_cache/0.3.5/16311176246009842383
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.8.1/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.8.1/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1767 2024-06-01 09:32:10.833253 crackerjack-0.8.1/crackerjack/__main__.py
+-rw-r--r--   0        0        0     7906 2024-06-01 10:39:46.039848 crackerjack-0.8.1/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     2799 2024-06-01 14:15:15.801398 crackerjack-0.8.1/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2799 2024-06-01 14:15:39.847169 crackerjack-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7760 1970-01-01 00:00:00.000000 crackerjack-0.8.1/PKG-INFO
```

### Comparing `crackerjack-0.8.0/LICENSE` & `crackerjack-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.8.0/README.md` & `crackerjack-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.8.0/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.8.1/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.8.0/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.8.1/crackerjack/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.8.0/crackerjack/__main__.py` & `crackerjack-0.8.1/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.8.0/crackerjack/crackerjack.py` & `crackerjack-0.8.1/crackerjack/crackerjack.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.8.0/crackerjack/pyproject.toml` & `crackerjack-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 ignore = [
     "F821",
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
+    "D105",
+    "D106",
     "D107",
 ]
 extend-select = [
     "I",
     "C901",
     "D",
 ]
@@ -83,15 +85,15 @@
 reportUnknownArgumentType = false
 reportPrivateUsage = "warning"
 pythonVersion = "3.12"
 pythonPlatform = "Darwin"
 
 [project]
 name = "Crackerjack"
-version = "0.7.36"
+version = "0.8.1"
 description = "Crackerjack code style"
 requires-python = ">=3.12"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.8.0/pyproject.toml` & `crackerjack-0.8.1/crackerjack/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 ignore = [
     "F821",
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
+    "D105",
+    "D106",
     "D107",
 ]
 extend-select = [
     "I",
     "C901",
     "D",
 ]
```

### Comparing `crackerjack-0.8.0/PKG-INFO` & `crackerjack-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.8.0
+Version: 0.8.1
 Summary: Crackerjack code style
 Keywords: black,ruff,mypy,creosote,refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

