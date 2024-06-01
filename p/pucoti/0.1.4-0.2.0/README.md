# Comparing `tmp/pucoti-0.1.4.tar.gz` & `tmp/pucoti-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pucoti-0.1.4.tar", max compression
+gzip compressed data, was "pucoti-0.2.0.tar", max compression
```

## Comparing `pucoti-0.1.4.tar` & `pucoti-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.1.4/COPYING
--rw-r--r--   0        0        0     1222 2024-06-01 02:40:08.335744 pucoti-0.1.4/README.md
--rw-r--r--   0        0        0    52252 2024-05-31 22:06:43.242609 pucoti-0.1.4/Wellbutrin.ttf
--rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.1.4/bell.mp3
--rwxr-xr-x   0        0        0    12921 2024-06-01 02:52:06.599105 pucoti-0.1.4/pucoti.py
--rw-r--r--   0        0        0      641 2024-06-01 02:53:34.718142 pucoti-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 pucoti-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.2.0/COPYING
+-rw-r--r--   0        0        0     1261 2024-06-01 03:48:36.793862 pucoti-0.2.0/README.md
+-rw-r--r--   0        0        0    52252 2024-05-31 22:06:43.242609 pucoti-0.2.0/Wellbutrin.ttf
+-rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.2.0/bell.mp3
+-rwxr-xr-x   0        0        0    13770 2024-06-01 03:41:51.533013 pucoti-0.2.0/pucoti.py
+-rw-r--r--   0        0        0      641 2024-06-01 03:49:43.257735 pucoti-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 pucoti-0.2.0/PKG-INFO
```

### Comparing `pucoti-0.1.4/COPYING` & `pucoti-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.4/README.md` & `pucoti-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,11 +27,15 @@
 1. **Install PUCOTI:**
    ```sh
    pip install pucoti
    ```
 
 2. **Run PUCOTI:**
    ```sh
-   pucoti
+   pucoti 5m
    ```
 
 That's it! PUCOTI should now be up and running.
+
+## Usage
+
+![Usage](./cli-help.png)
```

### Comparing `pucoti-0.1.4/Wellbutrin.ttf` & `pucoti-0.2.0/Wellbutrin.ttf`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.4/bell.mp3` & `pucoti-0.2.0/bell.mp3`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.4/pucoti.py` & `pucoti-0.2.0/pucoti.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,38 +26,29 @@
 import subprocess
 import sys
 from time import time
 from typing import Annotated
 from pathlib import Path
 import re
 import typer
+from typer import Argument, Option
 from enum import Enum
 
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "hide"
 os.environ["SDL_VIDEODRIVER"] = "x11"
 
 import pygame
 from pygame.locals import *
 import pygame._sdl2 as sdl2
 
 
 BELL = Path(__file__).parent / "bell.mp3"
-BIG_FONT = Path(__file__).parent / "Wellbutrin.ttf"
-SMALL_FONT = BIG_FONT
-RING_INTERVAL = 20
-PURPOSE_COLOR = (183, 255, 183)
-TIMER_COLOR = (255, 224, 145)
-TEXT_TIMES_UP_COLOR = (255, 0, 0)
-TOTAL_TIME_COLOR = (183, 183, 255)
-BACKGROUND_COLOR = (0, 0, 0)
-HELP_COLOR = TIMER_COLOR
+FONT = Path(__file__).parent / "Wellbutrin.ttf"
 WINDOW_SCALE = 1.2
 POSITIONS = [(-5, -5), (5, 5), (5, -5), (-5, 5)]
-INITIAL_SIZE = (180, 70)
-PURPOSE_HISTORY_FILE = Path("~/logs/dtimer_purpose_history.jsonl").expanduser()
 SHORTCUTS = """
 J/K: -/+ 1 minute
 R: reset timer
 RETURN: enter purpose
 L: list purpose history
 P: reposition window
 -/=: (in/de)crease window size
@@ -68,91 +59,84 @@
 
 {SHORTCUTS}
 
 Press any key to dismiss this message.
 """.strip()
 
 
-PURPOSE_HISTORY_FILE.parent.mkdir(parents=True, exist_ok=True)
-
-
 def fmt_time(seconds):
     if seconds < 0:
         return "-" + fmt_time(-seconds)
     minutes, seconds = divmod(seconds, 60)
     hours, minutes = divmod(minutes, 60)
     if hours:
         return "%d:%02d:%02d" % (hours, minutes, seconds)
     else:
         return "%02d:%02d" % (minutes, seconds)
 
 
 @lru_cache(maxsize=40)
-def font(size: int, big: bool = True):
-    name = BIG_FONT if big else SMALL_FONT
-    f = pygame.font.Font(name, size)
-    # f.align = FONT_CENTER
-    return f
+def get_font(size: int):
+    return pygame.font.Font(FONT, size)
 
 
 @lru_cache(maxsize=100)
 def text(
     text: str,
     size: int | tuple[int, int],
     color: tuple,
-    big: bool = True,
     monospaced_time: bool = False,
 ):
     if not isinstance(size, int):
         if monospaced_time:
             # Use the font size that fits a text equivalent to the time.
             # We use 0s to make sure the text is as wide as possible and doesn't jitter.
-            size = auto_size(re.sub(r"\d", "0", text), size, big)
+            size = auto_size(re.sub(r"\d", "0", text), size)
         else:
-            size = auto_size(text, size, big)
+            size = auto_size(text, size)
 
     if not monospaced_time:
-        return font(size, big).render(text, True, color)
+        return get_font(size).render(text, True, color)
     else:
         digits = "0123456789"
         # We render each char independently to make sure they are monospaced.
-        chars = [font(size, big).render(c, True, color) for c in text]
+        chars = [get_font(size).render(c, True, color) for c in text]
         # Make each digit the size of a 0.
-        width = font(size, big).size("0")[0]
+        width = get_font(size).size("0")[0]
         full_width = sum(s.get_width() if c not in digits else width for c, s in zip(text, chars))
         # Create a surface with the correct width.
-        surf = pygame.Surface((full_width, chars[0].get_height()))
+        surf = pygame.Surface((full_width, chars[0].get_height()), SRCALPHA)
         # Blit each char at the correct position.
         x = 0
         for c, s in zip(text, chars):
             if c in digits:
                 blit_x = x + (width - s.get_width()) // 2
             else:
                 blit_x = x
             surf.blit(s, (blit_x, 0))
             x += s.get_width() if c not in digits else width
         return surf
 
 
-def size_with_newlines(text: str, size: int, big: bool = True):
+def size_with_newlines(text: str, size: int):
     """Return the size of the text with newlines."""
     lines = text.split("\n")
-    line_height = font(size, big).get_linesize()
-    return (max(font(size, big).size(line)[0] for line in lines), len(lines) * line_height)
+    line_height = get_font(size).get_linesize()
+    return (max(get_font(size).size(line)[0] for line in lines), len(lines) * line_height)
 
 
-def auto_size(text: str, max_rect: tuple[int, int], big_font: bool = True):
+def auto_size(text: str, max_rect: tuple[int, int]):
     """Find the largest font size that will fit text in max_rect."""
     # Use dichotomy to find the largest font size that will fit text in max_rect.
 
     min_size = 1
     max_size = max_rect[1]
     while min_size < max_size:
         font_size = (min_size + max_size) // 2
-        text_size = size_with_newlines(text, font_size, big_font)
+        text_size = size_with_newlines(text, font_size)
 
         if text_size[0] <= max_rect[0] and text_size[1] <= max_rect[1]:
             min_size = font_size + 1
         else:
             max_size = font_size
     return min_size - 1
 
@@ -166,14 +150,18 @@
     size = info.current_w, info.current_h
 
     if x < 0:
         x = size[0] + x - window.size[0]
     if y < 0:
         y = size[1] + y - window.size[1]
 
+    # Is there a way to know if this worked? It doesn't on sway.
+    # It works on some platforms.
+    window.position = (x, y)
+
     try:
         cmd = f'swaymsg "[title=\\"DTimer\\"] move absolute position {x} {y}"'
         subprocess.check_output(cmd, shell=True)
     except subprocess.CalledProcessError as e:
         print(e.output)
 
 
@@ -189,21 +177,21 @@
     cummulative_ratios = [0] + [sum(ratios[:i]) for i in range(1, len(ratios) + 1)]
     ys = [int(rect.height * r) for r in cummulative_ratios]
     return [
         pygame.Rect(rect.left, ys[i], rect.width, ys[i + 1] - ys[i]) for i in range(len(ratios))
     ]
 
 
-def human_duration(*duration: str) -> int:
+def human_duration(duration: str) -> int:
     """Convert a human duration to seconds."""
 
     # Parse the duration.
     total = 0
     multiplier = {"s": 1, "m": 60, "h": 3600, "d": 86400}
-    for part in duration:
+    for part in duration.split():
         try:
             total += int(part[:-1]) * multiplier[part[-1]]
         except (ValueError, KeyError):
             raise ValueError(f"Invalid duration part: {part}")
 
     return total
 
@@ -237,44 +225,66 @@
             else:
                 purpose, time, bottom = vsplit(screen, 1, 2, 1)
                 return {"purpose": purpose, "time": time, "total_time": bottom}
         else:
             raise ValueError(f"Invalid scene: {self}")
 
 
-app = typer.Typer(add_completion=False)
+app = typer.Typer(add_completion=False, pretty_exceptions_show_locals=False)
 
 
 @app.command()
-def main(initial_timer: list[str]):
+def main(
+    # fmt: off
+    initial_timer: Annotated[str, Argument(help="The initial timer duration.")] = "5m",
+    bell: Annotated[Path, Option(help="Path to the bell sound file.")] = BELL,
+    ring_every: Annotated[int, Option(help="The time between rings, in seconds.")] = 20,
+    ring_count: Annotated[int, Option(help="Number of rings played when the time is up.")] = -1,
+    font: Annotated[Path, Option(help="Path to the font for all text.")] = FONT,
+    background_color: tuple[int, int, int] = (0, 0, 0),
+    timer_color: tuple[int, int, int] = (255, 224, 145),
+    timer_up_color: tuple[int, int, int] = (255, 0, 0),
+    purpose_color: tuple[int, int, int] = (183, 255, 183),
+    total_time_color: tuple[int, int, int] = (183, 183, 255),
+    window_position: tuple[int, int] = (-5, -5),
+    window_size: tuple[int, int] = (180, 70),
+    history_file: Annotated[Path, Option(help="Path to the file where the purpose history is stored.")] = Path("~/.pucoti_history"),
+    # fmt: on
+) -> None:
     """
-    DTimer is simple but flexible countdown timer.
+    Stay on task with PUCOTI, a countdown timer built for simplicity and purpose.
 
     Help is available by pressing h or ?.
     """
 
+    global FONT
+    FONT = font
+    history_file = history_file.expanduser()
+    history_file.parent.mkdir(parents=True, exist_ok=True)
+
     pygame.init()
     pygame.mixer.init()
     pygame.key.set_repeat(300, 20)
 
     pygame.print_debug_info()
-    window = sdl2.Window("DTimer", INITIAL_SIZE, borderless=True, always_on_top=True)
+    window = sdl2.Window("DTimer", window_size, borderless=True, always_on_top=True)
     window.get_surface().fill((0, 0, 0))
     window.flip()
 
     screen = window.get_surface()
     clock = pygame.time.Clock()
 
     position = 0
-    place_window(window, *POSITIONS[position])
+    place_window(window, *window_position)
 
-    initial_duration = human_duration(*initial_timer)
+    initial_duration = human_duration(initial_timer)
     start = time()
     timer = initial_duration
     last_rung = 0
+    nb_rings = 0
 
     purpose = ""
     purpose_history = []
 
     last_scene = None
     scene = Scene.MAIN
     layout = scene.mk_layout(window.size)
@@ -323,61 +333,64 @@
                 elif event.key == K_l:
                     scene = Scene.PURPOSE_HISTORY
                     layout = scene.mk_layout(window.size)
 
         if last_scene == Scene.ENTERING_PURPOSE and scene != last_scene:
             if purpose and (not purpose_history or purpose != purpose_history[-1].text):
                 purpose_history.append(Purpose(purpose, time()))
-                with PURPOSE_HISTORY_FILE.open("a") as f:
+                with history_file.open("a") as f:
                     f.write(json.dumps(purpose_history[-1].__dict__) + "\n")
 
-        screen.fill(BACKGROUND_COLOR)
+        screen.fill(background_color)
 
         # Render purpose, if there is space.
         if purpose_rect := layout.get("purpose"):
-            t = text(purpose, purpose_rect.size, PURPOSE_COLOR)
+            t = text(purpose, purpose_rect.size, purpose_color)
             r = screen.blit(t, t.get_rect(center=purpose_rect.center))
             if scene == Scene.ENTERING_PURPOSE and (time() % 1) < 0.7:
                 if r.height == 0:
                     r.height = purpose_rect.height
                 if r.right >= purpose_rect.right:
                     r.right = purpose_rect.right - 3
-                pygame.draw.line(screen, PURPOSE_COLOR, r.topright, r.bottomright, 2)
+                pygame.draw.line(screen, purpose_color, r.topright, r.bottomright, 2)
 
         # Render time.
         if time_rect := layout.get("time"):
             remaining = timer - (time() - start)
-            color = TEXT_TIMES_UP_COLOR if remaining < 0 else TIMER_COLOR
+            color = timer_up_color if remaining < 0 else timer_color
             t = text(fmt_time(abs(remaining)), time_rect.size, color, monospaced_time=True)
             screen.blit(t, t.get_rect(center=time_rect.center))
 
         if total_time_rect := layout.get("total_time"):
             t = text(
                 fmt_time(time() - start),
                 total_time_rect.size,
-                TOTAL_TIME_COLOR,
+                total_time_color,
                 monospaced_time=True,
             )
             screen.blit(t, t.get_rect(center=total_time_rect.center))
 
         if help_rect := layout.get("help"):
-            screen.fill(BACKGROUND_COLOR)
-            t = text(HELP, help_rect.size, HELP_COLOR, big=False)
+            screen.fill(background_color)
+            t = text(HELP, help_rect.size, timer_color)
             screen.blit(t, t.get_rect(center=help_rect.center))
 
         if purpose_history_rect := layout.get("purpose_history"):
-            screen.fill(BACKGROUND_COLOR)
+            screen.fill(background_color)
             t = "\n".join(f"({fmt_time(p.timestamp - start)}) {p.text}" for p in purpose_history)
-            t = text("HISTORY\n" + t, purpose_history_rect.size, PURPOSE_COLOR, big=False)
+            t = text("HISTORY\n" + t, purpose_history_rect.size, purpose_color)
             screen.blit(t, t.get_rect(center=purpose_history_rect.center))
 
         # Ring the bell if the time is up.
-        if remaining < 0 and time() - last_rung > RING_INTERVAL:
-            play(BELL)
+        if remaining < 0 and time() - last_rung > ring_every and nb_rings != ring_count:
+            play(bell)
             last_rung = time()
+            nb_rings += 1
+        elif remaining > 0:
+            nb_rings = 0
 
         window.flip()
         clock.tick(60)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `pucoti-0.1.4/pyproject.toml` & `pucoti-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pucoti"
-version = "0.1.4"
+version = "0.2.0"
 description = "A Purposeful Countdown Timer"
 authors = ["ddorn <diego.dorn@free.fr>"]
 readme = "README.md"
 license = "GPL-3.0"
 homepage = "https://github.com/ddorn/pucoti"
 repository = "https://github.com/ddorn/pucoti"
 keywords = ["timer", "countdown", "pygame"]
```

### Comparing `pucoti-0.1.4/PKG-INFO` & `pucoti-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pucoti
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Purposeful Countdown Timer
 Home-page: https://github.com/ddorn/pucoti
 License: GPL-3.0
 Keywords: timer,countdown,pygame
 Author: ddorn
 Author-email: diego.dorn@free.fr
 Requires-Python: >=3.12,<4.0
@@ -45,12 +45,16 @@
 1. **Install PUCOTI:**
    ```sh
    pip install pucoti
    ```
 
 2. **Run PUCOTI:**
    ```sh
-   pucoti
+   pucoti 5m
    ```
 
 That's it! PUCOTI should now be up and running.
 
+## Usage
+
+![Usage](./cli-help.png)
+
```

