# Comparing `tmp/devdeck_core-1.0.7.tar.gz` & `tmp/devdeck_core-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devdeck_core-1.0.7.tar", last modified: Sat Jul  3 11:10:28 2021, max compression
+gzip compressed data, was "devdeck_core-1.0.8.tar", last modified: Sat Jun  1 10:58:14 2024, max compression
```

## Comparing `devdeck_core-1.0.7.tar` & `devdeck_core-1.0.8.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.876132 devdeck_core-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-07-03 11:10:28.876132 devdeck_core-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      658 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.872132 devdeck_core-1.0.7/devdeck_core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.872132 devdeck_core-1.0.7/devdeck_core/assets/
--rw-r--r--   0 runner    (1001) docker     (121)    10402 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/assets/Roboto License.txt
--rw-r--r--   0 runner    (1001) docker     (121)   158604 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/assets/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)      432 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/control_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.872132 devdeck_core-1.0.7/devdeck_core/controls/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/controls/deck_control.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/deck_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.872132 devdeck_core-1.0.7/devdeck_core/decks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/decks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/decks/deck_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/mock_deck_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.872132 devdeck_core-1.0.7/devdeck_core/rendering/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/rendering/badge_count_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/rendering/emoji_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/rendering/image_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/rendering/text_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.876132 devdeck_core-1.0.7/devdeck_core/settings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/settings/cerberus_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/devdeck_core/settings/control_validation_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.872132 devdeck_core-1.0.7/devdeck_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-07-03 11:10:28.000000 devdeck_core-1.0.7/devdeck_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2021-07-03 11:10:28.000000 devdeck_core-1.0.7/devdeck_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-03 11:10:28.000000 devdeck_core-1.0.7/devdeck_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-07-03 11:10:28.000000 devdeck_core-1.0.7/devdeck_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-07-03 11:10:28.000000 devdeck_core-1.0.7/devdeck_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-03 11:10:28.876132 devdeck_core-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      894 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.876132 devdeck_core-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.876132 devdeck_core-1.0.7/tests/devdeck/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/tests/devdeck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.876132 devdeck_core-1.0.7/tests/devdeck/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/tests/devdeck/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:28.876132 devdeck_core-1.0.7/tests/devdeck/core/settings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/tests/devdeck/core/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2021-07-03 11:10:21.000000 devdeck_core-1.0.7/tests/devdeck/core/settings/test_control_validation_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.756166 devdeck_core-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-01 10:58:14.756166 devdeck_core-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/devdeck_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/devdeck_core/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    10402 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/assets/Roboto License.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   158604 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/assets/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/control_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/devdeck_core/controls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/controls/deck_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/deck_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/devdeck_core/decks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/decks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/decks/deck_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/mock_deck_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/devdeck_core/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/rendering/badge_count_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/rendering/emoji_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/rendering/image_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/rendering/text_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/devdeck_core/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/settings/cerberus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/devdeck_core/settings/control_validation_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.756166 devdeck_core-1.0.8/devdeck_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-01 10:58:14.000000 devdeck_core-1.0.8/devdeck_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-06-01 10:58:14.000000 devdeck_core-1.0.8/devdeck_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:58:14.000000 devdeck_core-1.0.8/devdeck_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-01 10:58:14.000000 devdeck_core-1.0.8/devdeck_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 10:58:14.000000 devdeck_core-1.0.8/devdeck_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 10:58:14.756166 devdeck_core-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/tests/devdeck/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/tests/devdeck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.752166 devdeck_core-1.0.8/tests/devdeck/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/tests/devdeck/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:14.756166 devdeck_core-1.0.8/tests/devdeck/core/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/tests/devdeck/core/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-06-01 10:58:06.000000 devdeck_core-1.0.8/tests/devdeck/core/settings/test_control_validation_error.py
```

### Comparing `devdeck_core-1.0.7/README.md` & `devdeck_core-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/assets/Roboto License.txt` & `devdeck_core-1.0.8/devdeck_core/assets/Roboto License.txt`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/assets/Roboto-Regular.ttf` & `devdeck_core-1.0.8/devdeck_core/assets/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/controls/deck_control.py` & `devdeck_core-1.0.8/devdeck_core/controls/deck_control.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/deck_context.py` & `devdeck_core-1.0.8/devdeck_core/deck_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,14 @@
             font_size = kwargs['font_size']
         if 'fill' in kwargs:
             fill = kwargs['fill']
         font = ImageFont.truetype(os.path.join(os.path.dirname(__file__), "assets", 'Roboto-Regular.ttf'), font_size)
 
         image = Image.new("RGB", (512, 512))
         draw = ImageDraw.Draw(image)
-        label_w, label_h = draw.textsize('%s' % text, font=font)
-        label_pos = ((512 - label_w) // 2, (512 - label_h) // 2)
+        left, top, right, bottom = draw.textbbox((0, 0), '%s' % text, font=font)
+        label_pos = ((512 - (right - left)) // 2, (512 - (bottom - top)) // 2)
         draw.text(label_pos, text=text, font=font, fill=fill)
         self.set_key_image_native(key_no, image)
 
     def get_image(self):
-        return self.image
+        return self.image
```

### Comparing `devdeck_core-1.0.7/devdeck_core/decks/deck_controller.py` & `devdeck_core-1.0.8/devdeck_core/decks/deck_controller.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/mock_deck_context.py` & `devdeck_core-1.0.8/devdeck_core/mock_deck_context.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/renderer.py` & `devdeck_core-1.0.8/devdeck_core/renderer.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/rendering/badge_count_renderer.py` & `devdeck_core-1.0.8/devdeck_core/rendering/badge_count_renderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,22 @@
         self._font_size = size
         return self
 
     def end(self):
         font = ImageFont.truetype(self.font_filename, self._font_size)
 
         draw = ImageDraw.Draw(self.renderer.img)
-        label_w, label_h = draw.textsize('%s' % self.text, font=font, stroke_width=4)
+        left, top, right, bottom = draw.textbbox((0, 0), '%s' % self.text, font=font, stroke_width=4)
 
         # Circle
 
         draw.ellipse((self.renderer.img.width - self.circle_size - self.corner_offset,
                       self.renderer.img.height - self.circle_size - self.corner_offset,
                       self.renderer.img.width - self.corner_offset,
                       self.renderer.img.height - self.corner_offset), fill='red')
 
         # Label
-        label_pos = (self.renderer.img.width - (self.circle_size / 2) - self.corner_offset - (label_w / 2),
-                     self.renderer.img.height - (self.circle_size / 2) - self.corner_offset - (label_h / 2))
+        label_pos = (self.renderer.img.width - (self.circle_size / 2) - self.corner_offset - ((right - left) / 2),
+                     self.renderer.img.height - (self.circle_size / 2) - self.corner_offset - ((bottom - top) / 2))
         draw.text(label_pos, text=self.text, font=font, fill=self.fill, stroke_width=4)
 
         return self.renderer
```

### Comparing `devdeck_core-1.0.7/devdeck_core/rendering/emoji_renderer.py` & `devdeck_core-1.0.8/devdeck_core/rendering/emoji_renderer.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/rendering/image_renderer.py` & `devdeck_core-1.0.8/devdeck_core/rendering/image_renderer.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/rendering/text_renderer.py` & `devdeck_core-1.0.8/devdeck_core/rendering/text_renderer.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         self.align = align
         return self
 
     def end(self):
         font = ImageFont.truetype(self.font_filename, self._font_size)
 
         draw = ImageDraw.Draw(self.renderer.img)
-        label_w, label_h = draw.textsize('%s' % self.text, font=font)
+        left, top, right, bottom = draw.textbbox((0, 0), '%s' % self.text, font=font)
 
         # Positioning
         label_pos = (self._x, self._y)
         if self.center_vertical is not None:
-            label_pos = (label_pos[0], ((self.renderer.img.height - label_h) // 2) + self.center_vertical)
+            label_pos = (label_pos[0], ((self.renderer.img.height - (bottom - top)) // 2) + self.center_vertical)
         if self.center_horizontal is not None:
-            label_pos = (((self.renderer.img.width - label_w) // 2) + self.center_horizontal, label_pos[1])
+            label_pos = (((self.renderer.img.width - (right - left)) // 2) + self.center_horizontal, label_pos[1])
 
         draw.text(label_pos, text=self.text, font=font, fill=self.fill, align=self.align)
 
         return self.renderer
```

### Comparing `devdeck_core-1.0.7/devdeck_core/settings/cerberus_utils.py` & `devdeck_core-1.0.8/devdeck_core/settings/cerberus_utils.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core/settings/control_validation_error.py` & `devdeck_core-1.0.8/devdeck_core/settings/control_validation_error.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/devdeck_core.egg-info/SOURCES.txt` & `devdeck_core-1.0.8/devdeck_core.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 devdeck_core/__init__.py
 devdeck_core/control_context.py
 devdeck_core/deck_context.py
```

### Comparing `devdeck_core-1.0.7/setup.py` & `devdeck_core-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `devdeck_core-1.0.7/tests/devdeck/core/settings/test_control_validation_error.py` & `devdeck_core-1.0.8/tests/devdeck/core/settings/test_control_validation_error.py`

 * *Files identical despite different names*

