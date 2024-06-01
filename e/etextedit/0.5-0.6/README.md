# Comparing `tmp/etextedit-0.5.tar.gz` & `tmp/etextedit-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etextedit-0.5.tar", last modified: Mon Nov 27 10:17:51 2023, max compression
+gzip compressed data, was "etextedit-0.6.tar", last modified: Sat Jun  1 16:04:28 2024, max compression
```

## Comparing `etextedit-0.5.tar` & `etextedit-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 office     (503) staff       (20)        0 2023-11-27 10:17:51.149416 etextedit-0.5/
--rw-r--r--   0 office     (503) staff       (20)     3108 2023-11-27 10:17:51.149198 etextedit-0.5/PKG-INFO
-drwxr-xr-x   0 office     (503) staff       (20)        0 2023-11-27 10:17:51.147698 etextedit-0.5/etextedit/
--rw-r--r--   0 office     (503) staff       (20)     1907 2023-11-27 10:17:51.000000 etextedit-0.5/etextedit/README.md
--rw-r--r--   0 office     (503) staff       (20)    29565 2023-11-26 20:59:53.000000 etextedit-0.5/etextedit/etextedit.py
--rw-r--r--   0 office     (503) staff       (20)       42 2023-11-26 20:45:17.000000 etextedit-0.5/etextedit/requirements.txt
-drwxr-xr-x   0 office     (503) staff       (20)        0 2023-11-27 10:17:51.148829 etextedit-0.5/etextedit.egg-info/
--rw-r--r--   0 office     (503) staff       (20)     3108 2023-11-27 10:17:51.000000 etextedit-0.5/etextedit.egg-info/PKG-INFO
--rw-r--r--   0 office     (503) staff       (20)      278 2023-11-27 10:17:51.000000 etextedit-0.5/etextedit.egg-info/SOURCES.txt
--rw-r--r--   0 office     (503) staff       (20)        1 2023-11-27 10:17:51.000000 etextedit-0.5/etextedit.egg-info/dependency_links.txt
--rw-r--r--   0 office     (503) staff       (20)       55 2023-11-27 10:17:51.000000 etextedit-0.5/etextedit.egg-info/entry_points.txt
--rw-r--r--   0 office     (503) staff       (20)       43 2023-11-27 10:17:51.000000 etextedit-0.5/etextedit.egg-info/requires.txt
--rw-r--r--   0 office     (503) staff       (20)       10 2023-11-27 10:17:51.000000 etextedit-0.5/etextedit.egg-info/top_level.txt
--rw-r--r--   0 office     (503) staff       (20)       38 2023-11-27 10:17:51.149464 etextedit-0.5/setup.cfg
--rw-r--r--   0 office     (503) staff       (20)     2670 2023-11-27 10:17:29.000000 etextedit-0.5/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-06-01 16:04:28.326166 etextedit-0.6/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3005 2024-06-01 16:04:28.326166 etextedit-0.6/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-06-01 16:04:28.326166 etextedit-0.6/etextedit/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1907 2024-06-01 16:04:28.000000 etextedit-0.6/etextedit/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29708 2024-06-01 16:03:27.000000 etextedit-0.6/etextedit/etextedit.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       42 2024-06-01 16:02:42.000000 etextedit-0.6/etextedit/requirements.txt
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-06-01 16:04:28.326166 etextedit-0.6/etextedit.egg-info/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3005 2024-06-01 16:04:28.000000 etextedit-0.6/etextedit.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      278 2024-06-01 16:04:28.000000 etextedit-0.6/etextedit.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-06-01 16:04:28.000000 etextedit-0.6/etextedit.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       55 2024-06-01 16:04:28.000000 etextedit-0.6/etextedit.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       43 2024-06-01 16:04:28.000000 etextedit-0.6/etextedit.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-06-01 16:04:28.000000 etextedit-0.6/etextedit.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-06-01 16:04:28.326166 etextedit-0.6/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2670 2024-06-01 16:03:56.000000 etextedit-0.6/setup.py
```

### Comparing `etextedit-0.5/PKG-INFO` & `etextedit-0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etextedit
-Version: 0.5
+Version: 0.6
 Summary: eTextEdit, a lightweight text editor built on prompt-toolkit
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/eTextEdit
 Project-URL: Tracker, https://github.com/eliranwong/eTextEdit/issues
@@ -18,18 +18,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
-Requires-Dist: datetime
-Requires-Dist: prompt_toolkit
-Requires-Dist: pygments
-Requires-Dist: pyperclip
 
 # eTextEdit
 Extensible Text Editor; built with prompt toolkit
 
 Originally a simple text editor created by Jonathan Slenders
 Source: https://github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/full-screen/text-editor.py
```

### Comparing `etextedit-0.5/etextedit/README.md` & `etextedit-0.6/etextedit/README.md`

 * *Files identical despite different names*

### Comparing `etextedit-0.5/etextedit/etextedit.py` & `etextedit-0.6/etextedit/etextedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,14 +455,17 @@
 def _(event):
     search_state = event.app.current_search_state
     previous_search_text = search_state.text
     if previous_search_text:
         search_toolbar.search_buffer.text = previous_search_text
         search_toolbar.search_buffer.cursor_position = len(previous_search_text)
     do_find()
+@bindings.add("c-b")
+def _(_):
+    do_find_reverse()
 @bindings.add("c-r")
 def _(_):
     do_find_replace()
 
 # file operations
 @bindings.add("c-n")
 def _(_):
@@ -776,15 +779,16 @@
                 MenuItem("-", disabled=True),
                 MenuItem("[C] Copy", handler=do_copy),
                 MenuItem("[V] Paste", handler=do_paste),
                 MenuItem("[X] Cut", handler=do_cut),
                 MenuItem("[D] Delete", handler=do_delete),
                 MenuItem("-", disabled=True),
                 MenuItem("[F] Find", handler=do_find),
-                MenuItem("[R] Find & Replace", handler=do_find_reverse),
+                MenuItem("[B] Find Backward", handler=do_find_reverse),
+                MenuItem("[R] Find & Replace", handler=do_find_replace),
                 #MenuItem("Find next", handler=do_find_next),
                 #MenuItem("Replace"),
                 MenuItem("[L] Go To Line", handler=do_go_to),
                 MenuItem("-", disabled=True),
                 MenuItem("[I] Spaces", handler=do_add_spaces),
                 MenuItem("Time / Date", handler=do_time_date),
             ],
@@ -898,8 +902,9 @@
         input_text = sys.stdin.read()
         text = launch(input_text=input_text)
     else:
         text = launch()
     #print(text)
 
 if __name__ == "__main__":
-    main()
+    main()
+    clear_title()
```

### Comparing `etextedit-0.5/etextedit.egg-info/PKG-INFO` & `etextedit-0.6/etextedit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etextedit
-Version: 0.5
+Version: 0.6
 Summary: eTextEdit, a lightweight text editor built on prompt-toolkit
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/eTextEdit
 Project-URL: Tracker, https://github.com/eliranwong/eTextEdit/issues
@@ -18,18 +18,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
-Requires-Dist: datetime
-Requires-Dist: prompt_toolkit
-Requires-Dist: pygments
-Requires-Dist: pyperclip
 
 # eTextEdit
 Extensible Text Editor; built with prompt toolkit
 
 Originally a simple text editor created by Jonathan Slenders
 Source: https://github.com/prompt-toolkit/python-prompt-toolkit/blob/master/examples/full-screen/text-editor.py
```

### Comparing `etextedit-0.5/setup.py` & `etextedit-0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         mod = line.strip()
         if mod:
             install_requires.append(mod)
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.5",
+    version="0.6",
     python_requires=">=3.7",
     description="eTextEdit, a lightweight text editor built on prompt-toolkit",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     packages=[
         package,
```

