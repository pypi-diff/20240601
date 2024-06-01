# Comparing `tmp/musiclib-2.4.0.tar.gz` & `tmp/musiclib-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musiclib-2.4.0.tar", last modified: Fri Feb 23 21:09:47 2024, max compression
+gzip compressed data, was "musiclib-2.5.0.tar", last modified: Sat Jun  1 08:37:31 2024, max compression
```

## Comparing `musiclib-2.4.0.tar` & `musiclib-2.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.072524 musiclib-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-23 21:09:47.072524 musiclib-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-23 21:09:29.000000 musiclib-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-02-23 21:09:29.000000 musiclib-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 21:09:47.072524 musiclib-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.064524 musiclib-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.064524 musiclib-2.4.0/src/musiclib/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/intervalset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.068524 musiclib-2.4.0/src/musiclib/midi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/midi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/midi/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/midi/pitchbend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/midi/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/note.py
--rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/noteset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/pitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/progression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/rhythm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.068524 musiclib-2.4.0/src/musiclib/svg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/card.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.068524 musiclib-2.4.0/src/musiclib/svg/isomorphic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/isomorphic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/isomorphic/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/isomorphic/hexagonal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/isomorphic/piano.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/isomorphic/squared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/isomorphic/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/piano.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/pianoroll.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/svg/reprsvg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/tempo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.068524 musiclib-2.4.0/src/musiclib/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/util/etc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.068524 musiclib-2.4.0/src/musiclib/voice_leading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/voice_leading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/voice_leading/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-23 21:09:29.000000 musiclib-2.4.0/src/musiclib/voice_leading/transition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:09:47.068524 musiclib-2.4.0/src/musiclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-23 21:09:47.000000 musiclib-2.4.0/src/musiclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-23 21:09:47.000000 musiclib-2.4.0/src/musiclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 21:09:47.000000 musiclib-2.4.0/src/musiclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-23 21:09:47.000000 musiclib-2.4.0/src/musiclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 21:09:47.000000 musiclib-2.4.0/src/musiclib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.469125 musiclib-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 08:37:31.469125 musiclib-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-06-01 08:37:21.000000 musiclib-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-06-01 08:37:21.000000 musiclib-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 08:37:31.469125 musiclib-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.461125 musiclib-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.465125 musiclib-2.5.0/src/musiclib/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/intervalset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.465125 musiclib-2.5.0/src/musiclib/midi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/midi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/midi/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/midi/pitchbend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/midi/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/noteset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/pitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/progression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/rhythm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.465125 musiclib-2.5.0/src/musiclib/svg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.469125 musiclib-2.5.0/src/musiclib/svg/isomorphic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/isomorphic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11609 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/isomorphic/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/isomorphic/hexagonal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/isomorphic/piano.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/isomorphic/squared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/isomorphic/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/piano.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/pianoroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/svg/reprsvg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/tempo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.469125 musiclib-2.5.0/src/musiclib/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/util/etc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.469125 musiclib-2.5.0/src/musiclib/voice_leading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/voice_leading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/voice_leading/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-06-01 08:37:21.000000 musiclib-2.5.0/src/musiclib/voice_leading/transition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:37:31.469125 musiclib-2.5.0/src/musiclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 08:37:31.000000 musiclib-2.5.0/src/musiclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-06-01 08:37:31.000000 musiclib-2.5.0/src/musiclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:37:31.000000 musiclib-2.5.0/src/musiclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-01 08:37:31.000000 musiclib-2.5.0/src/musiclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 08:37:31.000000 musiclib-2.5.0/src/musiclib.egg-info/top_level.txt
```

### Comparing `musiclib-2.4.0/PKG-INFO` & `musiclib-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: musiclib
-Version: 2.4.0
+Version: 2.5.0
 Summary: set of tools to work with scales, modes, modulations, chord progressions, voice leading, rhythm and more
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/musiclib
 Project-URL: issues, https://gitlab.tandav.me/tandav/notes/-/issues/?label_name=musiclib
 Project-URL: release notes, https://github.com/tandav/musiclib/releases
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: colortool>=0.5.3
+Requires-Dist: colortool>=0.6.0
 Requires-Dist: opseq>=0.1.2
 Requires-Dist: mido>=1.3.0
 Requires-Dist: svg.py
 Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: bumpver==2023.1129; extra == "dev"
 Requires-Dist: hypothesis==6.98.8; extra == "dev"
```

### Comparing `musiclib-2.4.0/README.md` & `musiclib-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/pyproject.toml` & `musiclib-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "musiclib"
-version = "2.4.0"
+version = "2.5.0"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = "set of tools to work with scales, modes, modulations, chord progressions, voice leading, rhythm and more"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
-    "colortool>=0.5.3",
+    "colortool>=0.6.0",
     "opseq>=0.1.2",
     "mido>=1.3.0",
     "svg.py",
     "numpy",
 ]
 
 [project.optional-dependencies]
@@ -47,15 +47,15 @@
 
 # [tool.setuptools.packages.find]
 # exclude = ["data*"]
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v2.4.0"
+current_version = "v2.5.0"
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
@@ -96,15 +96,15 @@
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
 
 # ==============================================================================
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "E501",  # line too long
     "PLR0913", # too-many-arguments
     "Q", # quotes
     "D", # docstrings
     "ERA001",
@@ -124,26 +124,26 @@
     "TD004",
     "FIX002",
     "FIX004",
     "B028",
     "PTH123",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = [
     "S101",
     "PLR2004",
     "ANN",
     "PT001",
     "PT011",
     "PT023",
     "N806",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 
 # ==============================================================================
 
 [tool.pylint.MASTER]
 # load-plugins=[
 #     "pylint_per_file_ignores",
```

### Comparing `musiclib-2.4.0/src/musiclib/config.py` & `musiclib-2.5.0/src/musiclib/config.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/interval.py` & `musiclib-2.5.0/src/musiclib/interval.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/intervalset.py` & `musiclib-2.5.0/src/musiclib/intervalset.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/midi/parse.py` & `musiclib-2.5.0/src/musiclib/midi/parse.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/midi/pitchbend.py` & `musiclib-2.5.0/src/musiclib/midi/pitchbend.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/midi/player.py` & `musiclib-2.5.0/src/musiclib/midi/player.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/note.py` & `musiclib-2.5.0/src/musiclib/note.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/noteset.py` & `musiclib-2.5.0/src/musiclib/noteset.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/pitch.py` & `musiclib-2.5.0/src/musiclib/pitch.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,53 +6,39 @@
 
 
 class Pitch:
     def __init__(
         self,
         hz_tuning: float = 440,
         origin_note: SpecificNote = A4,
-        transpose: float = 0,
     ) -> None:
         """
-        origin_note: in midi format, A4 midi (A3 in ableton) ~ 440Hz
+        origin_note: in midi format, A4 midi ~ 440Hz ~ midi number i=69
         """
         self.hz_tuning = hz_tuning
         self.origin_note = origin_note
-        self.transpose = transpose
 
     def i_to_hz(self, i: float) -> float:
-        return self.hz_tuning * 2 ** ((i + self.transpose) / 12)
+        return self.hz_tuning * 2 ** ((i - self.origin_note.i) / 12)
 
     def hz_to_i(self, hz: float) -> float:
-        return 12 * math.log2(hz / self.hz_tuning) - self.transpose
-
-    def note_i_to_hz(self, note_i: float) -> float:
-        return self.i_to_hz(note_i - self.origin_note.i)
-
-    def hz_to_note_i(self, hz: float) -> float:
-        return self.origin_note.i + self.hz_to_i(hz)
+        return 12 * math.log2(hz / self.hz_tuning) + self.origin_note.i
 
     def note_to_hz(self, note: SpecificNote) -> float:
-        return self.note_i_to_hz(note.i)
+        return self.i_to_hz(note.i)
 
     def hz_to_note(self, hz: float) -> SpecificNote:
-        return SpecificNote.from_i(round(self.hz_to_note_i(hz)))
-
-    def note_to_i(self, note: SpecificNote) -> float:
-        return note.i - self.origin_note.i
-
-    def i_to_note(self, i: float) -> SpecificNote:
-        return SpecificNote.from_i(round(self.origin_note.i + i))
+        return SpecificNote.from_i(round(self.hz_to_i(hz)))
 
     @staticmethod
     def hz_to_px(hz: float, hz_min: float, hz_max: float, px_max: float) -> float:
         """Convert Hz to pixel position (using logarithmic scale)"""
         return math.log2(hz / hz_min) / math.log2(hz_max / hz_min) * px_max
 
     @staticmethod
     def px_to_hz(px: float, hz_min: float, hz_max: float, px_max: float) -> float:
         """Convert pixel position to hz (assuming pixel using logarithmic scale)"""
         c = px / px_max
         return hz_min ** (1 - c) * hz_max ** c  # type: ignore[no-any-return]
 
     def __repr__(self) -> str:
-        return f'Pitch(hz_tuning={self.hz_tuning!r}, origin_note={self.origin_note!r}, transpose={self.transpose!r})'
+        return f'Pitch(hz_tuning={self.hz_tuning!r}, origin_note={self.origin_note!r})'
```

### Comparing `musiclib-2.4.0/src/musiclib/progression.py` & `musiclib-2.5.0/src/musiclib/progression.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/rhythm.py` & `musiclib-2.5.0/src/musiclib/rhythm.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/scale.py` & `musiclib-2.5.0/src/musiclib/scale.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/card.py` & `musiclib-2.5.0/src/musiclib/svg/card.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/header.py` & `musiclib-2.5.0/src/musiclib/svg/header.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/isomorphic/base.py` & `musiclib-2.5.0/src/musiclib/svg/isomorphic/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
                 continue
             self.elements.append(svg.Text(**value))
 
         # transparent polygon on top for mouse events and recoloring
         polygon = svg.Polygon(
             class_=['polygon-transparent'],
             points=points,  # type: ignore[arg-type]
-            fill=Color.from_rgba_int((0, 0, 0, 0)).css_rgba,
+            fill=Color.from_rgba_int((0, 0, 0, 0)).css_rgb,
         )
         polygon.interval = interval  # type: ignore[attr-defined]
         polygon.abstract_interval = abstract_interval.interval  # type: ignore[attr-defined]
         polygon.abstract_interval_base12 = abstract_interval  # type: ignore[attr-defined]
         self.elements.append(polygon)
 
     @abc.abstractmethod
```

### Comparing `musiclib-2.4.0/src/musiclib/svg/isomorphic/hexagonal.py` & `musiclib-2.5.0/src/musiclib/svg/isomorphic/hexagonal.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/isomorphic/piano.py` & `musiclib-2.5.0/src/musiclib/svg/isomorphic/piano.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/isomorphic/squared.py` & `musiclib-2.5.0/src/musiclib/svg/isomorphic/squared.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/isomorphic/text.py` & `musiclib-2.5.0/src/musiclib/svg/isomorphic/text.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/nested.py` & `musiclib-2.5.0/src/musiclib/svg/nested.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/piano.py` & `musiclib-2.5.0/src/musiclib/svg/piano.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/pianoroll.py` & `musiclib-2.5.0/src/musiclib/svg/pianoroll.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/svg/reprsvg.py` & `musiclib-2.5.0/src/musiclib/svg/reprsvg.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/tempo.py` & `musiclib-2.5.0/src/musiclib/tempo.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/util/cache.py` & `musiclib-2.5.0/src/musiclib/util/cache.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/util/etc.py` & `musiclib-2.5.0/src/musiclib/util/etc.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/voice_leading/checks.py` & `musiclib-2.5.0/src/musiclib/voice_leading/checks.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib/voice_leading/transition.py` & `musiclib-2.5.0/src/musiclib/voice_leading/transition.py`

 * *Files identical despite different names*

### Comparing `musiclib-2.4.0/src/musiclib.egg-info/PKG-INFO` & `musiclib-2.5.0/src/musiclib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: musiclib
-Version: 2.4.0
+Version: 2.5.0
 Summary: set of tools to work with scales, modes, modulations, chord progressions, voice leading, rhythm and more
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/musiclib
 Project-URL: issues, https://gitlab.tandav.me/tandav/notes/-/issues/?label_name=musiclib
 Project-URL: release notes, https://github.com/tandav/musiclib/releases
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: colortool>=0.5.3
+Requires-Dist: colortool>=0.6.0
 Requires-Dist: opseq>=0.1.2
 Requires-Dist: mido>=1.3.0
 Requires-Dist: svg.py
 Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: bumpver==2023.1129; extra == "dev"
 Requires-Dist: hypothesis==6.98.8; extra == "dev"
```

### Comparing `musiclib-2.4.0/src/musiclib.egg-info/SOURCES.txt` & `musiclib-2.5.0/src/musiclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

