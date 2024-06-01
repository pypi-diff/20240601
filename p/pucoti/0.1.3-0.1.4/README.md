# Comparing `tmp/pucoti-0.1.3.tar.gz` & `tmp/pucoti-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pucoti-0.1.3.tar", max compression
+gzip compressed data, was "pucoti-0.1.4.tar", max compression
```

## Comparing `pucoti-0.1.3.tar` & `pucoti-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.1.3/COPYING
--rw-r--r--   0        0        0     1222 2024-06-01 02:40:08.335744 pucoti-0.1.3/README.md
--rw-r--r--   0        0        0    52252 2024-05-31 22:06:43.242609 pucoti-0.1.3/Wellbutrin.ttf
--rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.1.3/bell.mp3
--rwxr-xr-x   0        0        0    12849 2024-06-01 02:26:57.467326 pucoti-0.1.3/pucoti.py
--rw-r--r--   0        0        0      641 2024-06-01 02:49:19.526031 pucoti-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 pucoti-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.1.4/COPYING
+-rw-r--r--   0        0        0     1222 2024-06-01 02:40:08.335744 pucoti-0.1.4/README.md
+-rw-r--r--   0        0        0    52252 2024-05-31 22:06:43.242609 pucoti-0.1.4/Wellbutrin.ttf
+-rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.1.4/bell.mp3
+-rwxr-xr-x   0        0        0    12921 2024-06-01 02:52:06.599105 pucoti-0.1.4/pucoti.py
+-rw-r--r--   0        0        0      641 2024-06-01 02:53:34.718142 pucoti-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 pucoti-0.1.4/PKG-INFO
```

### Comparing `pucoti-0.1.3/COPYING` & `pucoti-0.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.3/README.md` & `pucoti-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.3/Wellbutrin.ttf` & `pucoti-0.1.4/Wellbutrin.ttf`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.3/bell.mp3` & `pucoti-0.1.4/bell.mp3`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.3/pucoti.py` & `pucoti-0.1.4/pucoti.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 os.environ["SDL_VIDEODRIVER"] = "x11"
 
 import pygame
 from pygame.locals import *
 import pygame._sdl2 as sdl2
 
 
-BELL = Path("./bell.mp3")
+BELL = Path(__file__).parent / "bell.mp3"
+BIG_FONT = Path(__file__).parent / "Wellbutrin.ttf"
+SMALL_FONT = BIG_FONT
 RING_INTERVAL = 20
 PURPOSE_COLOR = (183, 255, 183)
 TIMER_COLOR = (255, 224, 145)
 TEXT_TIMES_UP_COLOR = (255, 0, 0)
 TOTAL_TIME_COLOR = (183, 183, 255)
 BACKGROUND_COLOR = (0, 0, 0)
 HELP_COLOR = TIMER_COLOR
@@ -82,15 +84,15 @@
         return "%d:%02d:%02d" % (hours, minutes, seconds)
     else:
         return "%02d:%02d" % (minutes, seconds)
 
 
 @lru_cache(maxsize=40)
 def font(size: int, big: bool = True):
-    name = "./Wellbutrin.ttf" if big else "./Wellbutrin.ttf"
+    name = BIG_FONT if big else SMALL_FONT
     f = pygame.font.Font(name, size)
     # f.align = FONT_CENTER
     return f
 
 
 @lru_cache(maxsize=100)
 def text(
```

### Comparing `pucoti-0.1.3/pyproject.toml` & `pucoti-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pucoti"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Purposeful Countdown Timer"
 authors = ["ddorn <diego.dorn@free.fr>"]
 readme = "README.md"
 license = "GPL-3.0"
 homepage = "https://github.com/ddorn/pucoti"
 repository = "https://github.com/ddorn/pucoti"
 keywords = ["timer", "countdown", "pygame"]
```

### Comparing `pucoti-0.1.3/PKG-INFO` & `pucoti-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pucoti
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Purposeful Countdown Timer
 Home-page: https://github.com/ddorn/pucoti
 License: GPL-3.0
 Keywords: timer,countdown,pygame
 Author: ddorn
 Author-email: diego.dorn@free.fr
 Requires-Python: >=3.12,<4.0
```

