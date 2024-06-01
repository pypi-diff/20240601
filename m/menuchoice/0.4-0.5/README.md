# Comparing `tmp/menuchoice-0.4.tar.gz` & `tmp/menuchoice-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menuchoice-0.4.tar", last modified: Thu May 16 03:47:23 2024, max compression
+gzip compressed data, was "menuchoice-0.5.tar", last modified: Sat Jun  1 09:34:17 2024, max compression
```

## Comparing `menuchoice-0.4.tar` & `menuchoice-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-16 03:47:23.256565 menuchoice-0.4/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-05-16 03:47:23.256565 menuchoice-0.4/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1055 2024-05-12 03:45:48.000000 menuchoice-0.4/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-16 03:47:23.255565 menuchoice-0.4/menuchoice/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     5408 2024-05-14 04:16:08.000000 menuchoice-0.4/menuchoice/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      643 2024-05-10 05:16:56.000000 menuchoice-0.4/menuchoice/_validator.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-16 03:47:23.255565 menuchoice-0.4/menuchoice/cursor_control/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     7161 2024-05-16 03:40:53.000000 menuchoice-0.4/menuchoice/cursor_control/_cursorInput.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      882 2024-05-14 10:44:56.000000 menuchoice-0.4/menuchoice/cursor_control/_textHandler.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      142 2024-05-10 03:13:36.000000 menuchoice-0.4/menuchoice/exceptions.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-16 03:47:23.256565 menuchoice-0.4/menuchoice.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-05-16 03:47:23.000000 menuchoice-0.4/menuchoice.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      311 2024-05-16 03:47:23.000000 menuchoice-0.4/menuchoice.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-16 03:47:23.000000 menuchoice-0.4/menuchoice.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-05-16 03:47:23.000000 menuchoice-0.4/menuchoice.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-16 03:47:23.256565 menuchoice-0.4/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1078 2024-05-16 03:44:34.000000 menuchoice-0.4/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 09:34:17.952098 menuchoice-0.5/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-06-01 09:34:17.952098 menuchoice-0.5/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1055 2024-05-12 03:45:48.000000 menuchoice-0.5/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 09:34:17.952098 menuchoice-0.5/menuchoice/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5408 2024-06-01 09:34:13.000000 menuchoice-0.5/menuchoice/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      643 2024-05-10 05:16:56.000000 menuchoice-0.5/menuchoice/_validator.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 09:34:17.952098 menuchoice-0.5/menuchoice/cursor_control/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     7257 2024-06-01 03:47:37.000000 menuchoice-0.5/menuchoice/cursor_control/_cursorInput.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      882 2024-05-14 10:44:56.000000 menuchoice-0.5/menuchoice/cursor_control/_textHandler.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      142 2024-05-10 03:13:36.000000 menuchoice-0.5/menuchoice/exceptions.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 09:34:17.952098 menuchoice-0.5/menuchoice.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-06-01 09:34:17.000000 menuchoice-0.5/menuchoice.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      311 2024-06-01 09:34:17.000000 menuchoice-0.5/menuchoice.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-06-01 09:34:17.000000 menuchoice-0.5/menuchoice.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-06-01 09:34:17.000000 menuchoice-0.5/menuchoice.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-06-01 09:34:17.952098 menuchoice-0.5/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1078 2024-05-16 03:44:34.000000 menuchoice-0.5/setup.py
```

### Comparing `menuchoice-0.4/PKG-INFO` & `menuchoice-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menuchoice
-Version: 0.4
+Version: 0.5
 Summary: Command line menu selector.
 Home-page: https://github.com/xyzpw/menuchoice/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: menu selector,item selector,ansi
 Classifier: Programming Language :: Python :: 3
```

### Comparing `menuchoice-0.4/README.md` & `menuchoice-0.5/README.md`

 * *Files identical despite different names*

### Comparing `menuchoice-0.4/menuchoice/__init__.py` & `menuchoice-0.5/menuchoice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import curses
 import re
 from .cursor_control import _cursorInput
 from .exceptions import *
 from . import _validator
 
-__version__ = "0.4"
+__version__ = "0.5"
 __author__ = "xyzpw"
 __description__ = "Command line menu selector."
 __license__ = "MIT"
 
 class MenuSelector:
     """Contains items which can be prompted via a menu selector."""
     def __init__(self, items: list | dict, title: str = None, description: str = None):
```

### Comparing `menuchoice-0.4/menuchoice/_validator.py` & `menuchoice-0.5/menuchoice/_validator.py`

 * *Files identical despite different names*

### Comparing `menuchoice-0.4/menuchoice/cursor_control/_cursorInput.py` & `menuchoice-0.5/menuchoice/cursor_control/_cursorInput.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     for i in range(len(menuLines)):
         if i != currentMenuLine:
             menuLines[i] = str(len(menuArrow) * " ") + " %s" % menuLines[i]
     return "\n".join(menuLines)
 
 def cursorArrowMenu(stdscr, menuString: str, menuArrow: str, center: bool = False):
     curses.curs_set(0)
+    curses.use_default_colors()
     currentLineIndex = 0
     stdscr.refresh()
     while True:
         stdscr.clear()
         stdscr.refresh()
         menuLines, menuMeta = getMenuComponents(menuString)
         rewrittenMenu = rewriteMenu(menuString, menuArrow, currentLineIndex)
@@ -83,14 +84,15 @@
         # centeredStr += "\n" * (pos[1]//2 + len(targetStrLines)//2) # Adds additional spacing (arbitrary)
     else:
         centeredStr = f"{chr(10)*pos[1]}{' '*pos[0]}{targetStr}"
     return centeredStr
 
 def cursorArrowMultiselectMenu(stdscr, menuString: str, maxItemCount: int = None, allowAll: bool = False, center: bool = False):
     curses.curs_set(0)
+    curses.use_default_colors()
     currentLineIndex = 0
     selectedItems = []
     if allowAll:
         menuString += "Select All\n"
     menuString += "Confirm Selection\n"
     stdscr.refresh()
     while True:
@@ -120,14 +122,15 @@
                 if currentLineIndex not in selectedItems and (maxItemCount <= len(selectedItems) if maxItemCount != None else False):
                     continue
                 selectedItems.append(currentLineIndex) if not currentLineIndex in selectedItems else selectedItems.pop(selectedItems.index(currentLineIndex))
 
 
 def highlightSelectMenu(stdscr, menuComponents: tuple, center: bool = False):
     curses.curs_set(0)
+    curses.use_default_colors()
     currentLineIndex = 0
     menuLines: list = menuComponents[0]
     menuTitle, menuDescription = menuComponents[1], menuComponents[2]
     centerSpacing = _textHandler.getItemSpacing(menuLines)
     while True:
         stdscr.clear()
         stdscr.refresh()
```

### Comparing `menuchoice-0.4/menuchoice/cursor_control/_textHandler.py` & `menuchoice-0.5/menuchoice/cursor_control/_textHandler.py`

 * *Files identical despite different names*

### Comparing `menuchoice-0.4/menuchoice.egg-info/PKG-INFO` & `menuchoice-0.5/menuchoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menuchoice
-Version: 0.4
+Version: 0.5
 Summary: Command line menu selector.
 Home-page: https://github.com/xyzpw/menuchoice/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: menu selector,item selector,ansi
 Classifier: Programming Language :: Python :: 3
```

### Comparing `menuchoice-0.4/setup.py` & `menuchoice-0.5/setup.py`

 * *Files identical despite different names*

