# Comparing `tmp/pucoti-0.2.0.tar.gz` & `tmp/pucoti-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pucoti-0.2.0.tar", max compression
+gzip compressed data, was "pucoti-0.3.0.tar", max compression
```

## Comparing `pucoti-0.2.0.tar` & `pucoti-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.2.0/COPYING
--rw-r--r--   0        0        0     1261 2024-06-01 03:48:36.793862 pucoti-0.2.0/README.md
--rw-r--r--   0        0        0    52252 2024-05-31 22:06:43.242609 pucoti-0.2.0/Wellbutrin.ttf
--rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.2.0/bell.mp3
--rwxr-xr-x   0        0        0    13770 2024-06-01 03:41:51.533013 pucoti-0.2.0/pucoti.py
--rw-r--r--   0        0        0      641 2024-06-01 03:49:43.257735 pucoti-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 pucoti-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.3.0/COPYING
+-rw-r--r--   0        0        0     1261 2024-06-01 03:48:36.793862 pucoti-0.3.0/README.md
+-rw-r--r--   0        0        0    52252 2024-05-31 22:06:43.242609 pucoti-0.3.0/Wellbutrin.ttf
+-rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.3.0/bell.mp3
+-rwxr-xr-x   0        0        0    13931 2024-06-01 04:28:19.112523 pucoti-0.3.0/pucoti.py
+-rw-r--r--   0        0        0      641 2024-06-01 04:29:54.116505 pucoti-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 pucoti-0.3.0/PKG-INFO
```

### Comparing `pucoti-0.2.0/COPYING` & `pucoti-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `pucoti-0.2.0/README.md` & `pucoti-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pucoti-0.2.0/Wellbutrin.ttf` & `pucoti-0.3.0/Wellbutrin.ttf`

 * *Files identical despite different names*

### Comparing `pucoti-0.2.0/bell.mp3` & `pucoti-0.3.0/bell.mp3`

 * *Files identical despite different names*

### Comparing `pucoti-0.2.0/pucoti.py` & `pucoti-0.3.0/pucoti.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,29 +204,43 @@
 
 class Scene(Enum):
     MAIN = "main"
     HELP = "help"
     PURPOSE_HISTORY = "purpose_history"
     ENTERING_PURPOSE = "entering_purpose"
 
-    def mk_layout(self, screen_size: tuple[int, int]) -> dict[str, pygame.Rect]:
+    def mk_layout(self, screen_size: tuple[int, int], has_purpose: bool) -> dict[str, pygame.Rect]:
         width, height = screen_size
         screen = pygame.Rect((0, 0), screen_size)
 
         if self == Scene.HELP:
             return {"help": screen}
         elif self == Scene.PURPOSE_HISTORY:
             return {"purpose_history": screen}
-        elif self in (Scene.MAIN, Scene.ENTERING_PURPOSE):
+        elif self == Scene.ENTERING_PURPOSE:
+            if height < 60:
+                return {"purpose": screen}
+            elif height < 120:
+                purpose, time = vsplit(screen, 2, 1)
+                return {"purpose": purpose, "time": time}
+            else:
+                purpose, time, bottom = vsplit(screen, 2, 1, 1)
+                return {"purpose": purpose, "time": time, "total_time": bottom}
+        elif self == Scene.MAIN:
             if height < 60:
                 return {"time": screen}
             elif height < 120:
+                if not has_purpose:
+                    return {"time": screen}
                 purpose, time = vsplit(screen, 1, 2)
                 return {"purpose": purpose, "time": time}
             else:
+                if not has_purpose:
+                    time, bottom = vsplit(screen, 3, 1)
+                    return {"time": time, "total_time": bottom}
                 purpose, time, bottom = vsplit(screen, 1, 2, 1)
                 return {"purpose": purpose, "time": time, "total_time": bottom}
         else:
             raise ValueError(f"Invalid scene: {self}")
 
 
 app = typer.Typer(add_completion=False, pretty_exceptions_show_locals=False)
@@ -283,67 +297,59 @@
     nb_rings = 0
 
     purpose = ""
     purpose_history = []
 
     last_scene = None
     scene = Scene.MAIN
-    layout = scene.mk_layout(window.size)
 
     while True:
         last_scene = scene
         for event in pygame.event.get():
             if event.type == QUIT:
                 sys.exit()
-            elif event.type == VIDEORESIZE:
-                layout = scene.mk_layout(window.size)
             elif event.type == KEYDOWN:
                 if scene in (Scene.HELP, Scene.PURPOSE_HISTORY):
                     scene = Scene.MAIN
-                    layout = scene.mk_layout(window.size)
                 if scene == Scene.ENTERING_PURPOSE:
                     if event.key == K_BACKSPACE:
                         purpose = purpose[:-1]
                     elif event.key in (K_RETURN, K_KP_ENTER, K_ESCAPE):
                         scene = Scene.MAIN
-                        layout = scene.mk_layout(window.size)
                     elif event.unicode:
                         purpose += event.unicode
                 elif event.key == K_j:
                     timer -= 60
                 elif event.key == K_k:
                     timer += 60
                 elif event.key == K_r:
                     # +1 to more likely show visually round time -> more satisfying
                     timer = initial_duration + (time() - start) + 1
                 elif event.key == K_MINUS:
                     window.size = (window.size[0] / WINDOW_SCALE, window.size[1] / WINDOW_SCALE)
-                    layout = scene.mk_layout(window.size)
                 elif event.key == K_EQUALS:
                     window.size = (window.size[0] * WINDOW_SCALE, window.size[1] * WINDOW_SCALE)
-                    layout = scene.mk_layout(window.size)
                 elif event.key == K_p:
                     position = (position + 1) % len(POSITIONS)
                     place_window(window, *POSITIONS[position])
                 elif event.key in (K_RETURN, K_KP_ENTER):
                     scene = Scene.ENTERING_PURPOSE
-                    layout = scene.mk_layout(window.size)
                 elif event.key in (K_h, K_QUESTION):
                     scene = Scene.HELP
-                    layout = scene.mk_layout(window.size)
                 elif event.key == K_l:
                     scene = Scene.PURPOSE_HISTORY
-                    layout = scene.mk_layout(window.size)
 
         if last_scene == Scene.ENTERING_PURPOSE and scene != last_scene:
             if purpose and (not purpose_history or purpose != purpose_history[-1].text):
                 purpose_history.append(Purpose(purpose, time()))
                 with history_file.open("a") as f:
                     f.write(json.dumps(purpose_history[-1].__dict__) + "\n")
 
+        layout = scene.mk_layout(window.size, bool(purpose))
+
         screen.fill(background_color)
 
         # Render purpose, if there is space.
         if purpose_rect := layout.get("purpose"):
             t = text(purpose, purpose_rect.size, purpose_color)
             r = screen.blit(t, t.get_rect(center=purpose_rect.center))
             if scene == Scene.ENTERING_PURPOSE and (time() % 1) < 0.7:
```

### Comparing `pucoti-0.2.0/pyproject.toml` & `pucoti-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pucoti"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Purposeful Countdown Timer"
 authors = ["ddorn <diego.dorn@free.fr>"]
 readme = "README.md"
 license = "GPL-3.0"
 homepage = "https://github.com/ddorn/pucoti"
 repository = "https://github.com/ddorn/pucoti"
 keywords = ["timer", "countdown", "pygame"]
```

### Comparing `pucoti-0.2.0/PKG-INFO` & `pucoti-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pucoti
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Purposeful Countdown Timer
 Home-page: https://github.com/ddorn/pucoti
 License: GPL-3.0
 Keywords: timer,countdown,pygame
 Author: ddorn
 Author-email: diego.dorn@free.fr
 Requires-Python: >=3.12,<4.0
```

