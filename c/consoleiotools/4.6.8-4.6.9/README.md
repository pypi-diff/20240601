# Comparing `tmp/consoleiotools-4.6.8.tar.gz` & `tmp/consoleiotools-4.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consoleiotools-4.6.8.tar", last modified: Tue May 28 15:08:50 2024, max compression
+gzip compressed data, was "consoleiotools-4.6.9.tar", last modified: Tue May 28 15:17:37 2024, max compression
```

## Comparing `consoleiotools-4.6.8.tar` & `consoleiotools-4.6.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:08:50.016669 consoleiotools-4.6.8/
--rw-r--r--   0 kyan001    (501) staff       (20)     1071 2023-11-19 07:58:26.000000 consoleiotools-4.6.8/LICENSE
--rw-r--r--   0 kyan001    (501) staff       (20)     7645 2024-05-28 15:08:50.016382 consoleiotools-4.6.8/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)     5544 2024-05-28 14:30:50.000000 consoleiotools-4.6.8/README.md
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:08:50.015022 consoleiotools-4.6.8/consoleiotools/
--rw-r--r--   0 kyan001    (501) staff       (20)    11637 2024-05-28 15:08:17.000000 consoleiotools-4.6.8/consoleiotools/__init__.py
--rw-r--r--   0 kyan001    (501) staff       (20)     2636 2023-11-19 07:58:26.000000 consoleiotools-4.6.8/consoleiotools/__main__.py
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:08:50.016054 consoleiotools-4.6.8/consoleiotools.egg-info/
--rw-r--r--   0 kyan001    (501) staff       (20)     7645 2024-05-28 15:08:50.000000 consoleiotools-4.6.8/consoleiotools.egg-info/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)      321 2024-05-28 15:08:50.000000 consoleiotools-4.6.8/consoleiotools.egg-info/SOURCES.txt
--rw-r--r--   0 kyan001    (501) staff       (20)        1 2024-05-28 15:08:50.000000 consoleiotools-4.6.8/consoleiotools.egg-info/dependency_links.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       12 2024-05-28 15:08:50.000000 consoleiotools-4.6.8/consoleiotools.egg-info/requires.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       20 2024-05-28 15:08:50.000000 consoleiotools-4.6.8/consoleiotools.egg-info/top_level.txt
--rw-r--r--   0 kyan001    (501) staff       (20)     1268 2024-03-26 12:04:27.000000 consoleiotools-4.6.8/pyproject.toml
--rw-r--r--   0 kyan001    (501) staff       (20)        5 2024-03-26 12:04:27.000000 consoleiotools-4.6.8/requirements.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       38 2024-05-28 15:08:50.016721 consoleiotools-4.6.8/setup.cfg
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:08:50.015822 consoleiotools-4.6.8/tests/
--rw-r--r--   0 kyan001    (501) staff       (20)    12775 2024-05-28 15:07:58.000000 consoleiotools-4.6.8/tests/test_consoleiotools.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:17:37.800877 consoleiotools-4.6.9/
+-rw-r--r--   0 kyan001    (501) staff       (20)     1071 2023-11-19 07:58:26.000000 consoleiotools-4.6.9/LICENSE
+-rw-r--r--   0 kyan001    (501) staff       (20)     7645 2024-05-28 15:17:37.800550 consoleiotools-4.6.9/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)     5544 2024-05-28 14:30:50.000000 consoleiotools-4.6.9/README.md
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:17:37.799008 consoleiotools-4.6.9/consoleiotools/
+-rw-r--r--   0 kyan001    (501) staff       (20)    11638 2024-05-28 15:17:31.000000 consoleiotools-4.6.9/consoleiotools/__init__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)     2636 2023-11-19 07:58:26.000000 consoleiotools-4.6.9/consoleiotools/__main__.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:17:37.800144 consoleiotools-4.6.9/consoleiotools.egg-info/
+-rw-r--r--   0 kyan001    (501) staff       (20)     7645 2024-05-28 15:17:37.000000 consoleiotools-4.6.9/consoleiotools.egg-info/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)      321 2024-05-28 15:17:37.000000 consoleiotools-4.6.9/consoleiotools.egg-info/SOURCES.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)        1 2024-05-28 15:17:37.000000 consoleiotools-4.6.9/consoleiotools.egg-info/dependency_links.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       12 2024-05-28 15:17:37.000000 consoleiotools-4.6.9/consoleiotools.egg-info/requires.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       20 2024-05-28 15:17:37.000000 consoleiotools-4.6.9/consoleiotools.egg-info/top_level.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)     1268 2024-03-26 12:04:27.000000 consoleiotools-4.6.9/pyproject.toml
+-rw-r--r--   0 kyan001    (501) staff       (20)        5 2024-03-26 12:04:27.000000 consoleiotools-4.6.9/requirements.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       38 2024-05-28 15:17:37.800947 consoleiotools-4.6.9/setup.cfg
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-05-28 15:17:37.799905 consoleiotools-4.6.9/tests/
+-rw-r--r--   0 kyan001    (501) staff       (20)    12776 2024-05-28 15:17:23.000000 consoleiotools-4.6.9/tests/test_consoleiotools.py
```

### Comparing `consoleiotools-4.6.8/LICENSE` & `consoleiotools-4.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleiotools-4.6.8/PKG-INFO` & `consoleiotools-4.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consoleiotools
-Version: 4.6.8
+Version: 4.6.9
 Summary: Console tools for inputs and outputs in Python
 Author-email: Kyan <kai@kyan001.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `consoleiotools-4.6.8/README.md` & `consoleiotools-4.6.9/README.md`

 * *Files identical despite different names*

### Comparing `consoleiotools-4.6.8/consoleiotools/__init__.py` & `consoleiotools-4.6.9/consoleiotools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import rich.text
 import rich.progress
 import rich.traceback
 import rich.markdown
 import rich.box
 import rich.markup
 
-__version__ = "4.6.8"
+__version__ = "4.6.9"
 __ascii__ = False
 theme = rich.theme.Theme({
     "echo": "bright_white",
     "echo-bar": "",
     "echo-pre": "dim bright_white",
     "echo-indent": "dim",
     "info": "",
@@ -117,15 +117,15 @@
     if bar:
         txt.append(f"{bar}", style=f"{style}-bar" if f"{style}-bar" in theme.styles else style)
         txt.append(" ")
     if pre:
         txt.append(f"({pre.capitalize()})", style=f"{style}-pre" if f"{style}-pre" in theme.styles else style)
         txt.append(" ")
     if indent:
-        indent_char_stem = "|   " if __ascii__ else "·   "
+        indent_char_stem = "|   " if __ascii__ else "╷   "
         indent_char_branch = "|-- " if __ascii__ else "├── "
         indent_char_leaf = "`-- " if __ascii__ else "╰── "
         if indent < 0:
             indent = -indent
             indent_deco = indent_char_leaf
         else:
             indent_deco = indent_char_branch
```

### Comparing `consoleiotools-4.6.8/consoleiotools/__main__.py` & `consoleiotools-4.6.9/consoleiotools/__main__.py`

 * *Files identical despite different names*

### Comparing `consoleiotools-4.6.8/consoleiotools.egg-info/PKG-INFO` & `consoleiotools-4.6.9/consoleiotools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consoleiotools
-Version: 4.6.8
+Version: 4.6.9
 Summary: Console tools for inputs and outputs in Python
 Author-email: Kyan <kai@kyan001.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `consoleiotools-4.6.8/pyproject.toml` & `consoleiotools-4.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `consoleiotools-4.6.8/tests/test_consoleiotools.py` & `consoleiotools-4.6.9/tests/test_consoleiotools.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         with patch("sys.stdout", new=StringIO()) as fake_out:
             cit.echo("ABC", indent=-1)
             self.assertEqual(fake_out.getvalue(), "│ ╰── ABC\n")
 
     def test_echo_indent_stem(self):
         with patch("sys.stdout", new=StringIO()) as fake_out:
             cit.echo("ABC", indent=2)
-            self.assertEqual(fake_out.getvalue(), "│ ·   ├── ABC\n")
+            self.assertEqual(fake_out.getvalue(), "│ ╷   ├── ABC\n")
 
     def test_markdown(self):
         with patch("sys.stdout", new=StringIO()) as fake_out:
             cit.markdown("### ABC")
             self.assertEqual(fake_out.getvalue().strip(), "ABC")
 
     def test_panel(self):
```

