# Comparing `tmp/changy-0.3.0.tar.gz` & `tmp/changy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changy-0.3.0.tar", max compression
+gzip compressed data, was "changy-0.4.0.tar", max compression
```

## Comparing `changy-0.3.0.tar` & `changy-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2024-05-31 14:02:52.064836 changy-0.3.0/LICENSE
--rw-r--r--   0        0        0     2858 2024-05-31 14:02:52.064836 changy-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-31 14:02:52.068836 changy-0.3.0/changy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/__init__.py
--rw-r--r--   0        0        0      381 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/__main__.py
--rw-r--r--   0        0        0       34 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/application.py
--rw-r--r--   0        0        0      175 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/changelog.py
--rw-r--r--   0        0        0      287 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/unreleased.py
--rw-r--r--   0        0        0      262 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/version.py
--rw-r--r--   0        0        0      477 2024-05-31 14:02:52.068836 changy-0.3.0/changy/constants.py
--rw-r--r--   0        0        0     1500 2024-05-31 14:02:52.068836 changy-0.3.0/changy/errors.py
--rw-r--r--   0        0        0     3613 2024-05-31 14:02:52.068836 changy-0.3.0/changy/logic.py
--rw-r--r--   0        0        0      768 2024-05-31 14:02:52.068836 changy-0.3.0/changy/settings.py
--rw-r--r--   0        0        0        0 2024-05-31 14:02:52.068836 changy-0.3.0/changy/tests/__init__.py
--rw-r--r--   0        0        0       29 2024-05-31 14:02:52.068836 changy-0.3.0/changy/tests/test_logic.py
--rw-r--r--   0        0        0      231 2024-05-31 14:02:52.068836 changy-0.3.0/changy/utils.py
--rw-r--r--   0        0        0     1953 2024-05-31 14:03:00.952864 changy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 changy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-31 16:13:45.139579 changy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2740 2024-05-31 16:13:45.139579 changy-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 16:13:45.139579 changy-0.4.0/changy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:13:45.139579 changy-0.4.0/changy/cli/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-31 16:13:45.139579 changy-0.4.0/changy/cli/__main__.py
+-rw-r--r--   0        0        0       34 2024-05-31 16:13:45.139579 changy-0.4.0/changy/cli/application.py
+-rw-r--r--   0        0        0      175 2024-05-31 16:13:45.139579 changy-0.4.0/changy/cli/changelog.py
+-rw-r--r--   0        0        0      287 2024-05-31 16:13:45.139579 changy-0.4.0/changy/cli/unreleased.py
+-rw-r--r--   0        0        0      426 2024-05-31 16:13:45.139579 changy-0.4.0/changy/cli/version.py
+-rw-r--r--   0        0        0      409 2024-05-31 16:13:45.139579 changy-0.4.0/changy/constants.py
+-rw-r--r--   0        0        0     1592 2024-05-31 16:13:45.139579 changy-0.4.0/changy/errors.py
+-rw-r--r--   0        0        0     3881 2024-05-31 16:13:45.139579 changy-0.4.0/changy/logic.py
+-rw-r--r--   0        0        0      768 2024-05-31 16:13:45.139579 changy-0.4.0/changy/settings.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:13:45.139579 changy-0.4.0/changy/tests/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-31 16:13:45.139579 changy-0.4.0/changy/tests/test_logic.py
+-rw-r--r--   0        0        0      231 2024-05-31 16:13:45.139579 changy-0.4.0/changy/utils.py
+-rw-r--r--   0        0        0     1953 2024-05-31 16:13:53.871554 changy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 changy-0.4.0/PKG-INFO
```

### Comparing `changy-0.3.0/LICENSE` & `changy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `changy-0.3.0/README.md` & `changy-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -40,18 +40,15 @@
 Besides version files, there are some particular files:
 
 - `./changes/header.md` — Content placed at the top of the changelog.
 - `./changes/changes_template.md` — Template for version files. Changy copies this file to create new version files.
 - `./changes/unreleased.md` — Contains changes not yet released.
 - `./changes/next_release.md` — Contains changes approved for the next release.
 
-You may edit `./changes/unreleased.md` any time you want before making an actual release. This file has no special syntax but allows substitution of some variables:
-
-- `{version_header}` — base header of version (version number + date).
-
+You may edit `./changes/unreleased.md` any time you want before making an actual release. The file has no special syntax.
 
 # Usage
 
 ## Manual operations before release
 
 ```bash
 # edit ./changes/unreleased.md
```

### Comparing `changy-0.3.0/changy/errors.py` & `changy-0.4.0/changy/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,7 +42,11 @@
 
 class ApprovedChangesFileExists(ChangyError):
     message = "Approved changes file ({file}) should not exist at this point. Ensure you finished version generation by calling `changy version create`."  # noqa: E501
 
 
 class VersionAlreadyExists(ChangyError):
     message = "Version {version} already exists. See {file}"
+
+
+class VersionDoesNotExist(ChangyError):
+    message = "Version {version} does not exist."
```

### Comparing `changy-0.3.0/changy/logic.py` & `changy-0.4.0/changy/logic.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,14 +108,26 @@
     next_release_file.rename(next_version_file)
 
     create_unreleased()
 
     return next_version_file
 
 
+def show_version_changes(version: str) -> str:
+    config_dir_must_exist()
+
+    changes = load_changes()
+
+    for change in changes:
+        if change.version == version:
+            return change.text.strip()
+
+    raise errors.VersionDoesNotExist(version=version)
+
+
 def create_changelog() -> None:
     config_dir_must_exist()
 
     if next_release_file.exists():
         raise errors.ApprovedChangesFileExists(file=next_release_file)
 
     if not unreleased_changes_file.exists():
@@ -125,15 +137,16 @@
 
     releases = load_changes()
 
     content = [header]
 
     # add unreleased changes
     text = unreleased_changes_file.read_text()
-    unreleased_text = text.format(version_header="Unreleased")
+    unreleased_text = f"## Unreleased\n\n{text.strip()}"
     content.append(unreleased_text)
 
-    content.extend(change.text.format(version_header=change.version_header) for change in releases)
+    for change in releases:
+        content.append(f"## {change.version_header}\n\n{change.text.strip()}")
 
     content = [x.strip() for x in content]
 
     changelog_file.write_text("\n\n".join(content))
```

### Comparing `changy-0.3.0/changy/settings.py` & `changy-0.4.0/changy/settings.py`

 * *Files identical despite different names*

### Comparing `changy-0.3.0/pyproject.toml` & `changy-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changy"
-version = "0.3.0"
+version = "0.4.0"
 description = "Simplest changelog manager, oriented to human editing, not to special message formatting in commits and tags.."
 readme = "README.md"
 repository = "https://github.com/Tiendil/changy"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = "BSD-3-Clause"
 keywords = ["changelog", "release-notes", "release-automation", "release-management", "changelog-generator", "changelog-formatter"]
 classifiers = [
```

### Comparing `changy-0.3.0/PKG-INFO` & `changy-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simplest changelog manager, oriented to human editing, not to special message formatting in commits and tags..
 Home-page: https://github.com/Tiendil/changy
 License: BSD-3-Clause
 Keywords: changelog,release-notes,release-automation,release-management,changelog-generator,changelog-formatter
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.12,<4.0
@@ -65,18 +65,15 @@
 Besides version files, there are some particular files:
 
 - `./changes/header.md` — Content placed at the top of the changelog.
 - `./changes/changes_template.md` — Template for version files. Changy copies this file to create new version files.
 - `./changes/unreleased.md` — Contains changes not yet released.
 - `./changes/next_release.md` — Contains changes approved for the next release.
 
-You may edit `./changes/unreleased.md` any time you want before making an actual release. This file has no special syntax but allows substitution of some variables:
-
-- `{version_header}` — base header of version (version number + date).
-
+You may edit `./changes/unreleased.md` any time you want before making an actual release. The file has no special syntax.
 
 # Usage
 
 ## Manual operations before release
 
 ```bash
 # edit ./changes/unreleased.md
```

