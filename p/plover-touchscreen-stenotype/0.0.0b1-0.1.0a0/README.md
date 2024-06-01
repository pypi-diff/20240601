# Comparing `tmp/plover-touchscreen-stenotype-0.0.0b1.tar.gz` & `tmp/plover-touchscreen-stenotype-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-touchscreen-stenotype-0.0.0b1.tar", last modified: Thu Nov 10 23:11:46 2022, max compression
+gzip compressed data, was "plover-touchscreen-stenotype-0.1.0a0.tar", last modified: Tue Feb 20 20:05:12 2024, max compression
```

## Comparing `plover-touchscreen-stenotype-0.0.0b1.tar` & `plover-touchscreen-stenotype-0.1.0a0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 23:11:46.459476 plover-touchscreen-stenotype-0.0.0b1/
--rw-rw-rw-   0        0        0       57 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0     2340 2022-11-10 23:11:46.459476 plover-touchscreen-stenotype-0.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     2056 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-10 23:11:46.379896 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/
--rw-rw-rw-   0        0        0     8113 2022-11-10 21:49:50.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/Main.py
--rw-rw-rw-   0        0        0        0 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/__init__.py
--rw-rw-rw-   0        0        0     1401 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/settings.py
--rw-rw-rw-   0        0        0     2296 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/util.py
-drwxrwxrwx   0        0        0        0 2022-11-10 23:11:46.457473 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/
--rw-rw-rw-   0        0        0     1735 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/KeyWidget.py
--rw-rw-rw-   0        0        0     5852 2022-11-10 07:13:04.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/KeyboardWidget.py
--rw-rw-rw-   0        0        0     4071 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/SettingsDialog.py
--rw-rw-rw-   0        0        0     7875 2022-11-10 07:40:17.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/StrokePreview.py
--rw-rw-rw-   0        0        0        0 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/__init__.py
--rw-rw-rw-   0        0        0    14126 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/build_keyboard.py
-drwxrwxrwx   0        0        0        0 2022-11-10 23:11:46.442437 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/
--rw-rw-rw-   0        0        0     2340 2022-11-10 23:11:46.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      875 2022-11-10 23:11:46.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 23:11:46.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2022-11-10 23:11:46.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2022-11-10 23:11:46.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2022-11-10 23:11:46.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-29 19:52:36.000000 plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/zip-safe
--rw-rw-rw-   0        0        0      721 2022-11-10 23:11:46.462457 plover-touchscreen-stenotype-0.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0       37 2022-11-09 22:13:34.000000 plover-touchscreen-stenotype-0.0.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-20 20:05:12.877260 plover-touchscreen-stenotype-0.1.0a0/
+-rw-rw-rw-   0        0        0       57 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3056 2024-02-20 20:05:12.876253 plover-touchscreen-stenotype-0.1.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2023-09-20 17:11:04.000000 plover-touchscreen-stenotype-0.1.0a0/README.md
+drwxrwxrwx   0        0        0        0 2024-02-20 20:05:12.803319 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/
+-rw-rw-rw-   0        0        0     7556 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/Main.py
+-rw-rw-rw-   0        0        0      516 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/NoneMachine.py
+-rw-rw-rw-   0        0        0        0 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/__init__.py
+-rw-rw-rw-   0        0        0     5641 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/settings.py
+-rw-rw-rw-   0        0        0    10149 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/util.py
+drwxrwxrwx   0        0        0        0 2024-02-20 20:05:12.866764 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/
+-rw-rw-rw-   0        0        0     4810 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/FloatInput.py
+-rw-rw-rw-   0        0        0     1735 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/KeyWidget.py
+-rw-rw-rw-   0        0        0     8602 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/KeyboardWidget.py
+-rw-rw-rw-   0        0        0     5422 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/RotatableKeyContainer.py
+-rw-rw-rw-   0        0        0    10749 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/SettingsDialog.py
+-rw-rw-rw-   0        0        0     8977 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/StrokePreview.py
+-rw-rw-rw-   0        0        0        0 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/__init__.py
+-rw-rw-rw-   0        0        0    17716 2023-08-20 00:55:23.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/build_keyboard.py
+drwxrwxrwx   0        0        0        0 2024-02-20 20:05:12.873256 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/build_keyboard_config/
+-rw-rw-rw-   0        0        0    11134 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/build_keyboard_config/english_stenotype.py
+-rw-rw-rw-   0        0        0    12046 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/build_keyboard_config/stenotype_extended_custom.py
+drwxrwxrwx   0        0        0        0 2024-02-20 20:05:12.875251 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/
+-rw-rw-rw-   0        0        0     3056 2024-02-20 20:05:12.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1200 2024-02-20 20:05:12.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-20 20:05:12.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2024-02-20 20:05:12.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2024-02-20 20:05:12.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-02-20 20:05:12.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-20 00:42:22.000000 plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1000 2024-02-20 20:05:12.890063 plover-touchscreen-stenotype-0.1.0a0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-08-20 00:36:45.000000 plover-touchscreen-stenotype-0.1.0a0/setup.py
```

### Comparing `plover-touchscreen-stenotype-0.0.0b1/PKG-INFO` & `plover-touchscreen-stenotype-0.1.0a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-Metadata-Version: 2.1
-Name: plover-touchscreen-stenotype
-Version: 0.0.0b1
-Summary: Touchscreen stenotype that utilizes multi-touch
-Home-page: https://github.com/wooningeire/plover-touchscreen-stenotype
-Keywords: plover plover_plugin
-Description-Content-Type: text/markdown
-
 # Plover touchscreen stenotype
 On-screen touch stenotype plugin for Plover.
 
 <!-- This nested embed will appear as a video on GitHub, but elsewhere it will embed the image -->
 [
 Demo recording (if below is playing slowly or not playing)<br /> <!-- <br /> used to resolve a spacing issue in the Plover Plugins Manager markdown renderer -->
-![](https://user-images.githubusercontent.com/22846982/200047983-64c948df-cbca-4590-a6b7-c397ecff4724.gif)
-](https://user-images.githubusercontent.com/22846982/199911422-0c08d1f0-7ce9-4d74-8658-8384142ab3ee.mp4)
+![](https://user-images.githubusercontent.com/22846982/236664546-8afe8d21-2dc6-48b4-8486-fc5be10a7be0.gif)
+](https://user-images.githubusercontent.com/22846982/236663907-51b4064b-2925-4da0-8359-d7419302dd8b.mp4)
 
 
 ## Additional setup / troubleshooting
 Operating systems may have built-in touchscreen gestures that sometimes prevent the window from receiving touches.
 
 On Windows 11: This works best after disabling 3- and 4-finger touch gestures in Settings (`Bluetooth & devices` > `Touch`, or navigate to `ms-settings:devices-touch` from the browser).
 
-On Windows 10/11: The default touch keyboard can be stopped from automatically appearing whenever a textbox is touched (sometimes) by disabling “Show the touch keyboard when … there’s no keyboard attached” in the touch keyboard settings (under `Time & language` > `Typing` on Windows 11, `Devices` > `Typing` on Windows 10, or `ms-settings:typing` from the browser).
+On Windows 11 22H2: The default touch keyboard can be stopped from automatically appearing by setting “Show the touch keyboard” to “Never” in the “Touch keyboard” settings (under `Time & language` > `Typing` on Windows 11, or `ms-settings:typing` from the browser).
+* On Windows 10 or older Windows 11: The default keyboard can be stopped from automatically appearing, to varying degrees of success, by disabling “Show the touch keyboard when … there’s no keyboard attached” in the “Touch keyboard” settings (under `Time & language` > `Typing` on Windows 11, `Devices` > `Typing` on Windows 10, or `ms-settings:typing` from the browser).
 
-On Linux+GNOME: There are [GNOME extensions that can disable touch gestures](https://extensions.gnome.org/extension/1140/disable-gestures/), but there is additionally a delay before windows receive touch inputs, which will have to be dealt with as well (check `xinput` and `libinput`?).
+On Linux+GNOME: There are [GNOME extensions that can disable touch gestures](https://extensions.gnome.org/extension/1140/disable-gestures/), but there is additionally a delay before windows receive touch inputs. Unless dealt with (check `xinput` and `libinput`?), this will require users to hold down a stroke for a brief period of time (~200 ms?) before releasing; releasing early will cause each touch to be registered as a stroke individually.
 
 
 ## Notes
 
 The key layout is currently based on the default English Stenotype system. This works best on touchscreens that support at least 10 simultaneous touch points. On Windows 10/11, the maximum number of touch points can be found alongside the device specifications in Settings (`System` > `About`, or navigate to `ms-settings:about` from the browser).
 
-After the plugin is installed, Plover may need to be restarted for the plugin GUI button to appear in the toolbar.
+After the plugin is installed, Plover may need to be restarted for the plugin GUI button to appear in the toolbar.
```

### Comparing `plover-touchscreen-stenotype-0.0.0b1/README.md` & `plover-touchscreen-stenotype-0.1.0a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,40 @@
+Metadata-Version: 2.1
+Name: plover-touchscreen-stenotype
+Version: 0.1.0a0
+Summary: Touchscreen stenotype that utilizes multi-touch
+Keywords: plover plover_plugin
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Requires-Dist: plover[gui_qt]>=4.0.0.dev12
+Requires-Dist: pywin32>=304.0.0; platform_system == "Windows"
+
 # Plover touchscreen stenotype
 On-screen touch stenotype plugin for Plover.
 
 <!-- This nested embed will appear as a video on GitHub, but elsewhere it will embed the image -->
 [
 Demo recording (if below is playing slowly or not playing)<br /> <!-- <br /> used to resolve a spacing issue in the Plover Plugins Manager markdown renderer -->
-![](https://user-images.githubusercontent.com/22846982/200047983-64c948df-cbca-4590-a6b7-c397ecff4724.gif)
-](https://user-images.githubusercontent.com/22846982/199911422-0c08d1f0-7ce9-4d74-8658-8384142ab3ee.mp4)
+![](https://user-images.githubusercontent.com/22846982/236664546-8afe8d21-2dc6-48b4-8486-fc5be10a7be0.gif)
+](https://user-images.githubusercontent.com/22846982/236663907-51b4064b-2925-4da0-8359-d7419302dd8b.mp4)
 
 
 ## Additional setup / troubleshooting
 Operating systems may have built-in touchscreen gestures that sometimes prevent the window from receiving touches.
 
 On Windows 11: This works best after disabling 3- and 4-finger touch gestures in Settings (`Bluetooth & devices` > `Touch`, or navigate to `ms-settings:devices-touch` from the browser).
 
-On Windows 10/11: The default touch keyboard can be stopped from automatically appearing whenever a textbox is touched (sometimes) by disabling “Show the touch keyboard when … there’s no keyboard attached” in the touch keyboard settings (under `Time & language` > `Typing` on Windows 11, `Devices` > `Typing` on Windows 10, or `ms-settings:typing` from the browser).
+On Windows 11 22H2: The default touch keyboard can be stopped from automatically appearing by setting “Show the touch keyboard” to “Never” in the “Touch keyboard” settings (under `Time & language` > `Typing` on Windows 11, or `ms-settings:typing` from the browser).
+* On Windows 10 or older Windows 11: The default keyboard can be stopped from automatically appearing, to varying degrees of success, by disabling “Show the touch keyboard when … there’s no keyboard attached” in the “Touch keyboard” settings (under `Time & language` > `Typing` on Windows 11, `Devices` > `Typing` on Windows 10, or `ms-settings:typing` from the browser).
 
-On Linux+GNOME: There are [GNOME extensions that can disable touch gestures](https://extensions.gnome.org/extension/1140/disable-gestures/), but there is additionally a delay before windows receive touch inputs, which will have to be dealt with as well (check `xinput` and `libinput`?).
+On Linux+GNOME: There are [GNOME extensions that can disable touch gestures](https://extensions.gnome.org/extension/1140/disable-gestures/), but there is additionally a delay before windows receive touch inputs. Unless dealt with (check `xinput` and `libinput`?), this will require users to hold down a stroke for a brief period of time (~200 ms?) before releasing; releasing early will cause each touch to be registered as a stroke individually.
 
 
 ## Notes
 
 The key layout is currently based on the default English Stenotype system. This works best on touchscreens that support at least 10 simultaneous touch points. On Windows 10/11, the maximum number of touch points can be found alongside the device specifications in Settings (`System` > `About`, or navigate to `ms-settings:about` from the browser).
 
-After the plugin is installed, Plover may need to be restarted for the plugin GUI button to appear in the toolbar.
+After the plugin is installed, Plover may need to be restarted for the plugin GUI button to appear in the toolbar.
```

### Comparing `plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/Main.py` & `plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/Main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from plover.gui_qt.tool import Tool
 from plover.gui_qt.utils import ToolBar
-# from plover.gui_qt import Engine
-from plover.engine import StenoEngine
+from plover.gui_qt.engine import Engine
 from plover.steno import Stroke
 from plover.oslayer import PLATFORM
 
 from PyQt5.QtCore import (
     Qt,
     QSize,
     QSettings,
@@ -16,53 +15,50 @@
     QAction,
 )
 from PyQt5.QtGui import (
     QIcon,
 )
 
 
-from plover_touchscreen_stenotype.settings import Settings
-from plover_touchscreen_stenotype.widgets.KeyboardWidget import KeyboardWidget
-from plover_touchscreen_stenotype.widgets.StrokePreview import StrokePreview
-from plover_touchscreen_stenotype.widgets.SettingsDialog import SettingsDialog
+from .settings import Settings
+from .util import Ref, watch
+from .widgets.KeyboardWidget import KeyboardWidget
+from .widgets.StrokePreview import StrokePreview
+from .widgets.SettingsDialog import SettingsDialog
 
 
 class Main(Tool):
     #region Overrides
 
     TITLE = "Touchscreen stenotype"
     ICON = ""
     ROLE = "touchscreen_stenotype"
 
-    def __init__(self, engine: StenoEngine):
+    def __init__(self, engine: Engine):
         super().__init__(engine)
 
         self.engine = engine # Override for type hint
         self.__last_stroke_from_widget = False
         """Whether the last emitted stroke originated from this Tool"""
         self.__last_stroke_keys: set[str] | None = None
         self.__last_stroke_engine_enabled = False
 
         self.__settings = Settings()
         self.restore_state()
         self.finished.connect(self.save_state)
         self.__setup_ui()
 
-        engine.signal_stroked.connect(self._on_stroked)
+        engine.signal_stroked.connect(self.__on_stroked)
 
 
     def _restore_state(self, settings: QSettings):
-        self.__settings.key_layout = settings.value("key_layout", self.__settings.key_layout)
-        self.__settings.stroke_preview_stroke = settings.value("stroke_preview_stroke", self.__settings.stroke_preview_stroke, type=bool)
-        self.__settings.stroke_preview_translation = settings.value("stroke_preview_translation", self.__settings.stroke_preview_translation, type=bool)
+        self.__settings.load(settings)
 
     def _save_state(self, settings: QSettings):
-        settings.setValue("key_layout", self.__settings.key_layout)
-        settings.setValue("stroke_preview_stroke", self.__settings.stroke_preview_stroke)
-        settings.setValue("stroke_preview_translation", self.__settings.stroke_preview_translation)
+        self.__settings.save(settings)
 
     #endregion
 
     def __setup_ui(self):
         self.setAttribute(Qt.WA_AcceptTouchEvents)
         # self.setAttribute(Qt.WA_ShowWithoutActivating)
         # self.setFocusPolicy(Qt.NoFocus)
@@ -72,19 +68,21 @@
         self.setWindowFlags(Qt.WindowStaysOnTopHint | Qt.WindowMinimizeButtonHint | Qt.WindowCloseButtonHint)
 
         # For some reason (tested on Windows only), this has to be called before KeyboardWidget is created. Other attributes
         # must also be set before this, otherwise the window will steal focus again
         self.__prevent_window_focus()
 
 
-        self.translation_display = translation_display = StrokePreview(self.engine, self.__settings, self)
+        left_right_width_diff = Ref(0)
 
-        stenotype = KeyboardWidget(self.__settings, self)
-        stenotype.end_stroke.connect(self._on_stenotype_input)
-        stenotype.current_stroke_change.connect(self._on_stroke_change)
+        self.stroke_preview = stroke_preview = StrokePreview(self.engine, self.__settings, left_right_width_diff, self)
+
+        stenotype = KeyboardWidget(self.__settings, left_right_width_diff, self)
+        stenotype.end_stroke.connect(self.__on_stenotype_input)
+        stenotype.current_stroke_change.connect(self.__on_stroke_change)
 
         settings_action = QAction(self)
         settings_action.setText("Settings")
         settings_action.setIcon(QIcon(r":/settings.svg")) # Loads from Plover's application-wide application resources
         settings_action.triggered.connect(self.__launch_settings_dialog)
 
         toolbar = ToolBar(settings_action)
@@ -92,21 +90,23 @@
         for button in toolbar.findChildren(QWidget):
             button.setFocusPolicy(Qt.NoFocus)
 
         toolbar.setIconSize(QSize(48, 48))
 
 
         layout = QGridLayout(self)
-        layout.addWidget(translation_display, 0, 0)
+        layout.addWidget(stroke_preview, 0, 0)
         layout.addWidget(toolbar, 0, 0, Qt.AlignBottom | Qt.AlignLeft)
         layout.addWidget(stenotype, 0, 0)
         self.setLayout(layout)
 
 
-        self.setWindowOpacity(0.9375)
+        @watch(self.__settings.window_opacity_ref.change)
+        def set_window_opacity():
+            self.setWindowOpacity(self.__settings.window_opacity)
 
 
     # https://stackoverflow.com/questions/24582525/how-to-show-clickable-qframe-without-loosing-focus-from-main-window
     # https://stackoverflow.com/questions/68276479/how-to-use-setwindowlongptr-hwnd-gwl-exstyle-ws-ex-noactivate
 
     # https://docs.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-setwindowlongptrw
     def __prevent_window_focus(self):
@@ -132,19 +132,18 @@
             user32.SetWindowLongPtrW(
                 window_handle,
                 win32con.GWL_EXSTYLE,
                 user32.GetWindowLongPtrW(window_handle, win32con.GWL_EXSTYLE) | win32con.WS_EX_NOACTIVATE | win32con.WS_EX_APPWINDOW,
             )
 
         # elif PLATFORM == "linux":
-        #     self.setWindowFlag(Qt.WindowDoesNotAcceptFocus)
         #     # self.setAttribute(Qt.WA_X11DoNotAcceptFocus)
 
 
-    def _on_stenotype_input(self, stroke_keys: set[str]):
+    def __on_stenotype_input(self, stroke_keys: set[str]):
         # Temporarily enable steno output (if not already waiting for a `stroked` hook dispatch)
         if not self.__last_stroke_from_widget:
             self.__last_stroke_engine_enabled = self.engine.output
             self.engine.output = True
 
         self.__last_stroke_from_widget = True
         self.__last_stroke_keys = stroke_keys
@@ -152,51 +151,49 @@
 
         # Wait until `stroked` hook is dispatched to reset `self.engine.output`, since it must be True for Suggestions to be shown
 
         # TODO The current implementation is not infallible because the `stroked` handler does not verify that the stroke it
         # received is the same stroke sent from this method. Multiple strokes may also be sent before the handler is called
         # (can use deque to resolve this)
 
-        self.translation_display.finish_stroke()
+        self.stroke_preview.finish_stroke()
 
-    def _on_stroked(self, stroke: Stroke):
+    def __on_stroked(self, stroke: Stroke):
         if not self.__last_stroke_from_widget or self.__last_stroke_keys != set(stroke.keys()): return
 
-        # self.last_stroke_label.setText(stroke.rtfcre or "…")
-        self.engine.output = self.__last_stroke_engine_enabled
+        if self.engine.output == False:
+            # The engine output was disabled before it was set again; {PLOVER:TOGGLE} was likely triggered
+            self.engine.output = not self.__last_stroke_engine_enabled
+        else:
+            self.engine.output = self.__last_stroke_engine_enabled
         
         self.__last_stroke_from_widget = False
         self.__last_stroke_keys = None
 
 
-    def _on_stroke_change(self, stroke_keys: set[str]):
-        self.translation_display.display_keys(stroke_keys)
+    def __on_stroke_change(self, stroke_keys: set[str]):
+        self.stroke_preview.display_keys(stroke_keys)
 
 
-    def resize_from_center(self, width: int, height: int):
-        try:
-            rect = self.geometry()
-            old_center = rect.center()
-
-            # In practice, the new size will be constrained to the minimum size, so it is not necessarily the given size
-            new_size = QSize(
-                max(self.minimumWidth(), width),
-                max(self.minimumHeight(), height),
-            )
+    """ def resize_from_center(self, width: int, height: int):
+        rect = self.geometry()
+        old_center = rect.center()
+
+        # In practice, the new size will be constrained to the minimum size, so it is not necessarily the given size
+        new_size = QSize(
+            max(self.minimumWidth(), width),
+            max(self.minimumHeight(), height),
+        )
 
-            rect.setSize(new_size)
-            rect.moveCenter(old_center)
-            
-            self.setGeometry(rect)
-
-        except Exception as error:
-            # self.last_stroke_label.setText(str(error))
-            pass
+        rect.setSize(new_size)
+        rect.moveCenter(old_center)
+        
+        self.setGeometry(rect) """
 
 
     def __launch_settings_dialog(self):
         dialog = SettingsDialog(self.__settings, self)
         dialog.open()
 
-# def command_open_window(engine: StenoEngine, arg: str):
+# def command_open_window(engine: Engine, arg: str):
 #     new_window = Main(engine)
 #     new_window.show()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/KeyWidget.py` & `plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/KeyWidget.py`

 * *Files identical despite different names*

### Comparing `plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype/widgets/StrokePreview.py` & `plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype/widgets/StrokePreview.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,138 @@
-from typing import Iterable
-from plover.engine import StenoEngine
+from plover.gui_qt.engine import Engine
 from plover.steno import Stroke
 
 from plover import system
 from plover.translation import Translation, Translator, _mapping_to_macro # TODO access violation
 
 from PyQt5.QtCore import (
     Qt,
 )
 from PyQt5.QtWidgets import (
     QWidget,
     QLabel,
     QGridLayout,
     QVBoxLayout,
     QSpacerItem,
+    QSizePolicy,
 )
 from PyQt5.QtGui import (
     QFont,
 )
 
 
-from plover_touchscreen_stenotype.settings import Settings, KeyLayout
-from plover_touchscreen_stenotype.util import UseDpi, FONT_FAMILY
-from plover_touchscreen_stenotype.widgets.build_keyboard import KEY_WIDTH
+from math import cos, radians
+from typing import Iterable
+
+from ..settings import Settings, KeyLayout
+from ..util import UseDpi, Ref, watch, watch_many, FONT_FAMILY
 
 class StrokePreview(QWidget):
-    def __init__(self, engine: StenoEngine, settings: Settings, parent: QWidget=None):
+    def __init__(self, engine: Engine, settings: Settings, right_left_width_diff: Ref[float], parent: QWidget=None):
         super().__init__(parent)
 
         self.__engine = engine
         self.__settings = settings
 
         self.__last_translation: Translation | None = None
         self.__last_stroke_matched = True
 
-        self.__setup_ui()
+        self.__setup_ui(right_left_width_diff)
 
-    def __setup_ui(self):
+    def __setup_ui(self, right_left_width_diff: Ref[float]):
         dpi = UseDpi(self)
 
         #region Labels
         self.__stroke_label = stroke_label = QLabel(self)
         self.__translation_label = translation_label = QLabel(self)
 
         stroke_label.setTextFormat(Qt.PlainText)
         translation_label.setTextFormat(Qt.PlainText)
 
+        # The horizontal size policies of the labels must be set to Ignored, or otherwise they will cause the window to
+        # resize to fit the text if the text is too long. However, that alone just causes the labels to resize to the
+        # widest item in the QVBoxLayout `labels_layout`, which would have a width of 0 since the label widths are
+        # ignored and the rest of the items are spacers. The strut is therefore needed to set the width of the layout
+        # to the width of the parent column in the QGridLayout `display_alignment_layout`, allowing the labels the full
+        # column width to display the text yet limiting them to that width so they do not resize the window.
+        strut = QWidget(self)
+        strut.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Fixed)
+        # https://stackoverflow.com/questions/21739119/qt-hboxlayout-stop-mainwindow-from-resizing-to-contents
+        stroke_label.setSizePolicy(QSizePolicy.Ignored, QSizePolicy.Fixed)
+        translation_label.setSizePolicy(QSizePolicy.Ignored, QSizePolicy.Fixed)
+
         labels_layout = QVBoxLayout()
         
-        top_spacer = QSpacerItem(0, 0)
-        labels_layout.addSpacerItem(top_spacer)
+        labels_layout.addSpacerItem(top_spacer := QSpacerItem(0, 0))
         labels_layout.addWidget(stroke_label, 0, Qt.AlignCenter)
         labels_layout.addSpacerItem(middle_spacer := QSpacerItem(0, 0))
         labels_layout.addWidget(translation_label, 0, Qt.AlignCenter)
+        labels_layout.addWidget(strut)
+
 
-        def resize_labels(): # Set font sizes in px rather than pt so they fit in the keyboard gaps
+        @watch(dpi.change)
+        def resize_label_fonts(): # Set font sizes in px rather than pt so they fit in the keyboard gaps
             stroke_label_font = QFont(FONT_FAMILY)
             translation_label_font = QFont(FONT_FAMILY)
 
             stroke_label_font.setPixelSize(dpi.dp(16.8 if self.__settings.stroke_preview_translation else 21))
             translation_label_font.setPixelSize(dpi.dp(21))
 
             stroke_label.setFont(stroke_label_font)
             middle_spacer.changeSize(0, dpi.dp(-4) if self.__settings.stroke_preview_full else 0)
             translation_label.setFont(translation_label_font)
 
             labels_layout.invalidate()
-        resize_labels()
-        dpi.change.connect(resize_labels)
 
         labels_layout.setSpacing(0)
         #endregion
 
 
         #region Display alignment
         display_alignment_layout = QGridLayout()
         display_alignment_layout.setColumnStretch(0, 1)
         display_alignment_layout.setColumnStretch(1, 0)
 
+        @watch_many(dpi.change, right_left_width_diff.change)
         def resize_display_alignment():
-            display_alignment_layout.setColumnMinimumWidth(1, dpi.cm(KEY_WIDTH))
-        resize_display_alignment()
-        dpi.change.connect(resize_display_alignment)
+            display_alignment_layout.setColumnMinimumWidth(1, right_left_width_diff.value)
+                    # dpi.cm(self.__settings.key_width) * cos(radians(self.__settings.main_rows_angle)))
+            # TODO replace MAIN_ROWS_ANGLE import with setting value when this becomes a setting
 
 
         display_alignment_layout.addLayout(labels_layout, 0, 0)
-        def move_translation_display():
+
+        @watch_many(dpi.change, self.__settings.key_layout_ref.change)
+        def reposition_labels():
             if self.__settings.key_layout == KeyLayout.GRID:
-                labels_layout.setAlignment(Qt.AlignBottom | Qt.AlignHCenter)
+                labels_layout.setAlignment(Qt.AlignBottom)
                 top_spacer.changeSize(0, 0)
             else:
-                labels_layout.setAlignment(Qt.AlignTop | Qt.AlignHCenter)
+                labels_layout.setAlignment(Qt.AlignTop)
                 top_spacer.changeSize(0, -8)
 
             labels_layout.invalidate()  # Must be called for layout to move
-        move_translation_display()
-        self.__settings.key_layout_change.connect(move_translation_display)
-        dpi.change.connect(move_translation_display)
         
         display_alignment_layout.addItem(QSpacerItem(0, 0), 0, 1)
         display_alignment_layout.setSpacing(0)
         display_alignment_layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(display_alignment_layout)
         #endregion
 
 
         #region Settings reactivity
+        @watch(self.__settings.stroke_preview_change)
         def on_settings_change():
             stroke_label.setVisible(self.__settings.stroke_preview_stroke)
             translation_label.setVisible(self.__settings.stroke_preview_translation)
 
-            resize_labels()
+            resize_label_fonts()
 
             self.__display_translation(self.__last_translation, self.__last_stroke_matched)
             self.finish_stroke()
-        on_settings_change()
-        self.__settings.stroke_preview_change.connect(on_settings_change)
         #endregion
 
 
     def display_keys(self, stroke_keys: Iterable[str]):
         if not self.__settings.stroke_preview_visible:
             # The coming translation will not be computed
             # When the stroke preview is reenabled, this will cause the placeholder to be shown again instead of an old
@@ -162,15 +175,15 @@
 
 
     def finish_stroke(self):
         self.__stroke_label.setStyleSheet("")
         self.__translation_label.setStyleSheet(f"""color: #{"ff" if self.__last_stroke_matched else "3f"}000000;""")
 
 
-def _coming_translation(engine: StenoEngine, keys: Iterable[str]) -> tuple[Translation, bool]:
+def _coming_translation(engine: Engine, keys: Iterable[str]) -> tuple[Translation, bool]:
     """Computes the translation that will result if the stroke defined by `keys` is sent to the engine.
     
     :returns: The translation that will result, and if a match was found
     :rtype: tuple[Translation, bool]
     """
     # TODO access violations
```

### Comparing `plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/PKG-INFO` & `plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: plover-touchscreen-stenotype
-Version: 0.0.0b1
+Version: 0.1.0a0
 Summary: Touchscreen stenotype that utilizes multi-touch
-Home-page: https://github.com/wooningeire/plover-touchscreen-stenotype
 Keywords: plover plover_plugin
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Requires-Dist: plover[gui_qt]>=4.0.0.dev12
+Requires-Dist: pywin32>=304.0.0; platform_system == "Windows"
 
 # Plover touchscreen stenotype
 On-screen touch stenotype plugin for Plover.
 
 <!-- This nested embed will appear as a video on GitHub, but elsewhere it will embed the image -->
 [
 Demo recording (if below is playing slowly or not playing)<br /> <!-- <br /> used to resolve a spacing issue in the Plover Plugins Manager markdown renderer -->
-![](https://user-images.githubusercontent.com/22846982/200047983-64c948df-cbca-4590-a6b7-c397ecff4724.gif)
-](https://user-images.githubusercontent.com/22846982/199911422-0c08d1f0-7ce9-4d74-8658-8384142ab3ee.mp4)
+![](https://user-images.githubusercontent.com/22846982/236664546-8afe8d21-2dc6-48b4-8486-fc5be10a7be0.gif)
+](https://user-images.githubusercontent.com/22846982/236663907-51b4064b-2925-4da0-8359-d7419302dd8b.mp4)
 
 
 ## Additional setup / troubleshooting
 Operating systems may have built-in touchscreen gestures that sometimes prevent the window from receiving touches.
 
 On Windows 11: This works best after disabling 3- and 4-finger touch gestures in Settings (`Bluetooth & devices` > `Touch`, or navigate to `ms-settings:devices-touch` from the browser).
 
-On Windows 10/11: The default touch keyboard can be stopped from automatically appearing whenever a textbox is touched (sometimes) by disabling “Show the touch keyboard when … there’s no keyboard attached” in the touch keyboard settings (under `Time & language` > `Typing` on Windows 11, `Devices` > `Typing` on Windows 10, or `ms-settings:typing` from the browser).
+On Windows 11 22H2: The default touch keyboard can be stopped from automatically appearing by setting “Show the touch keyboard” to “Never” in the “Touch keyboard” settings (under `Time & language` > `Typing` on Windows 11, or `ms-settings:typing` from the browser).
+* On Windows 10 or older Windows 11: The default keyboard can be stopped from automatically appearing, to varying degrees of success, by disabling “Show the touch keyboard when … there’s no keyboard attached” in the “Touch keyboard” settings (under `Time & language` > `Typing` on Windows 11, `Devices` > `Typing` on Windows 10, or `ms-settings:typing` from the browser).
 
-On Linux+GNOME: There are [GNOME extensions that can disable touch gestures](https://extensions.gnome.org/extension/1140/disable-gestures/), but there is additionally a delay before windows receive touch inputs, which will have to be dealt with as well (check `xinput` and `libinput`?).
+On Linux+GNOME: There are [GNOME extensions that can disable touch gestures](https://extensions.gnome.org/extension/1140/disable-gestures/), but there is additionally a delay before windows receive touch inputs. Unless dealt with (check `xinput` and `libinput`?), this will require users to hold down a stroke for a brief period of time (~200 ms?) before releasing; releasing early will cause each touch to be registered as a stroke individually.
 
 
 ## Notes
 
 The key layout is currently based on the default English Stenotype system. This works best on touchscreens that support at least 10 simultaneous touch points. On Windows 10/11, the maximum number of touch points can be found alongside the device specifications in Settings (`System` > `About`, or navigate to `ms-settings:about` from the browser).
 
 After the plugin is installed, Plover may need to be restarted for the plugin GUI button to appear in the toolbar.
```

### Comparing `plover-touchscreen-stenotype-0.0.0b1/plover_touchscreen_stenotype.egg-info/SOURCES.txt` & `plover-touchscreen-stenotype-0.1.0a0/plover_touchscreen_stenotype.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 plover_touchscreen_stenotype/Main.py
+plover_touchscreen_stenotype/NoneMachine.py
 plover_touchscreen_stenotype/__init__.py
 plover_touchscreen_stenotype/settings.py
 plover_touchscreen_stenotype/util.py
 plover_touchscreen_stenotype.egg-info/PKG-INFO
 plover_touchscreen_stenotype.egg-info/SOURCES.txt
 plover_touchscreen_stenotype.egg-info/dependency_links.txt
 plover_touchscreen_stenotype.egg-info/entry_points.txt
 plover_touchscreen_stenotype.egg-info/requires.txt
 plover_touchscreen_stenotype.egg-info/top_level.txt
 plover_touchscreen_stenotype.egg-info/zip-safe
+plover_touchscreen_stenotype/widgets/FloatInput.py
 plover_touchscreen_stenotype/widgets/KeyWidget.py
 plover_touchscreen_stenotype/widgets/KeyboardWidget.py
+plover_touchscreen_stenotype/widgets/RotatableKeyContainer.py
 plover_touchscreen_stenotype/widgets/SettingsDialog.py
 plover_touchscreen_stenotype/widgets/StrokePreview.py
 plover_touchscreen_stenotype/widgets/__init__.py
-plover_touchscreen_stenotype/widgets/build_keyboard.py
+plover_touchscreen_stenotype/widgets/build_keyboard.py
+plover_touchscreen_stenotype/widgets/build_keyboard_config/english_stenotype.py
+plover_touchscreen_stenotype/widgets/build_keyboard_config/stenotype_extended_custom.py
```

