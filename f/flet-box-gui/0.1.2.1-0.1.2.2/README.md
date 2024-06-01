# Comparing `tmp/flet-box-gui-0.1.2.1.tar.gz` & `tmp/flet-box-gui-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-box-gui-0.1.2.1.tar", last modified: Tue May 28 14:44:11 2024, max compression
+gzip compressed data, was "flet-box-gui-0.1.2.2.tar", last modified: Sat Jun  1 20:51:10 2024, max compression
```

## Comparing `flet-box-gui-0.1.2.1.tar` & `flet-box-gui-0.1.2.2.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.601719 flet-box-gui-0.1.2.1/
--rw-r--r--   0 mjay      (1000) mjay      (1000)     3189 2024-05-28 14:43:54.000000 flet-box-gui-0.1.2.1/CHANGELOG.md
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11340 2024-03-27 02:45:35.000000 flet-box-gui-0.1.2.1/LICENSE
--rw-r--r--   0 mjay      (1000) mjay      (1000)       81 2024-05-28 03:22:40.000000 flet-box-gui-0.1.2.1/MANIFEST.in
--rw-r--r--   0 mjay      (1000) mjay      (1000)    23643 2024-05-28 14:44:11.601719 flet-box-gui-0.1.2.1/PKG-INFO
--rw-r--r--   0 mjay      (1000) mjay      (1000)    14602 2024-05-28 14:10:23.000000 flet-box-gui-0.1.2.1/README.md
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.577719 flet-box-gui-0.1.2.1/flet_box/
--rw-r--r--   0 mjay      (1000) mjay      (1000)       29 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/__init__.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/assets/
--rw-r--r--   0 mjay      (1000) mjay      (1000)    13575 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/avatar.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)    22379 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/avatar.png
--rw-r--r--   0 mjay      (1000) mjay      (1000)    97142 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/dragg_container.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)    51971 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/dragg_container3.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)   195620 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/image.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)   141033 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/img.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)    82936 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/logo.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)   135590 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/logo_mark.png
--rw-r--r--   0 mjay      (1000) mjay      (1000)   226793 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/my_avatar.png
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11864 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/no_imagen.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)   204659 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/splash.jpg
--rw-r--r--   0 mjay      (1000) mjay      (1000)    27549 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/assets/wallpaper.jpg
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/__init__.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/about/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/about/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    18687 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/about/about.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/alert/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/alert/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     1711 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/alert/alert_selected.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    14328 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/gpt_browser.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     6033 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/library_chatgpt.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.585719 flet-box-gui-0.1.2.1/flet_box/extra_utils/color_browser/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/color_browser/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11954 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/color_browser/color_browser.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.589719 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    16681 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/blur_color_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11564 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/bool_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    13019 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/color_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    12624 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/double_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    16368 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/four_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    30959 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/gradient_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    18393 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/selection_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    13712 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/single_entry.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    41661 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/widget_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.589719 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     8947 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/dragg_widget.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    27864 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/infinity_box_layer_one.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    25298 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/widget_drag_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.589719 flet-box-gui-0.1.2.1/flet_box/extra_utils/icon_browser/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/icon_browser/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11552 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/icon_browser/icon_browser.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     8164 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/footer_bar_menu_phone.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     2374 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/selected_widget.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_right_phone/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_right_phone/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    22984 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_right_phone/right_bar_menu_phone.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_left_phone/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_left_phone/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    11184 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     7973 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     1762 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    19563 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.593719 flet-box-gui-0.1.2.1/flet_box/extra_utils/phone_container/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/phone_container/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     7335 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/phone_container/widget_phone_editor.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.597719 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    30641 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/screen_manager.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     2336 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/settings_screens.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)      636 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/write_file_proyect.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.597719 flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    53915 2024-05-27 01:26:15.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/save_export.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     3986 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/settings_widget.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.597719 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/
--rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/__init__.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    10218 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/color_hight_light_editor.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)     3305 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/tree_view.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    17067 2024-05-26 13:45:19.000000 flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/tree_view_text_editor.py
--rw-r--r--   0 mjay      (1000) mjay      (1000)    15513 2024-05-28 02:42:28.000000 flet-box-gui-0.1.2.1/flet_box/flet_box.py
-drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-05-28 14:44:11.601719 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/
--rw-r--r--   0 mjay      (1000) mjay      (1000)    23643 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/PKG-INFO
--rw-r--r--   0 mjay      (1000) mjay      (1000)     3329 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/SOURCES.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)        1 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/dependency_links.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)       47 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/entry_points.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)       42 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/requires.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)        9 2024-05-28 14:44:11.000000 flet-box-gui-0.1.2.1/flet_box_gui.egg-info/top_level.txt
--rw-r--r--   0 mjay      (1000) mjay      (1000)       38 2024-05-28 14:44:11.601719 flet-box-gui-0.1.2.1/setup.cfg
--rw-r--r--   0 mjay      (1000) mjay      (1000)     4780 2024-05-28 14:41:09.000000 flet-box-gui-0.1.2.1/setup.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.701034 flet-box-gui-0.1.2.2/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     3306 2024-06-01 20:48:59.000000 flet-box-gui-0.1.2.2/CHANGELOG.md
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11340 2024-05-31 22:05:32.000000 flet-box-gui-0.1.2.2/LICENSE
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       81 2024-05-31 22:05:32.000000 flet-box-gui-0.1.2.2/MANIFEST.in
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    18628 2024-06-01 20:51:10.697034 flet-box-gui-0.1.2.2/PKG-INFO
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    14695 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/README.md
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.673033 flet-box-gui-0.1.2.2/flet_box/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       29 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/__init__.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.681033 flet-box-gui-0.1.2.2/flet_box/assets/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    13575 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/avatar.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    22379 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/avatar.png
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    97142 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/dragg_container.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    51971 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/dragg_container3.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   195620 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/image.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   141033 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/img.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    82936 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/logo.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   135590 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/logo_mark.png
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   226793 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/my_avatar.png
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11864 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/no_imagen.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)   204659 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/splash.jpg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    27549 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/assets/wallpaper.jpg
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.681033 flet-box-gui-0.1.2.2/flet_box/extra_utils/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/__init__.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.685033 flet-box-gui-0.1.2.2/flet_box/extra_utils/about/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/about/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    18687 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/about/about.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.685033 flet-box-gui-0.1.2.2/flet_box/extra_utils/alert/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/alert/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     1711 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/alert/alert_selected.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.685033 flet-box-gui-0.1.2.2/flet_box/extra_utils/chat_gpt_browser/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/chat_gpt_browser/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    14328 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/chat_gpt_browser/gpt_browser.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     6033 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/chat_gpt_browser/library_chatgpt.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.685033 flet-box-gui-0.1.2.2/flet_box/extra_utils/color_browser/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/color_browser/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11954 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/color_browser/color_browser.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.689033 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    16681 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/blur_color_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11564 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/bool_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    13019 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/color_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    12624 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/double_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    16368 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/four_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    30959 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/gradient_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    18393 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/selection_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    13741 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/single_entry.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    43618 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/widget_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.689033 flet-box-gui-0.1.2.2/flet_box/extra_utils/drag_container/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/drag_container/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     9035 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/drag_container/dragg_widget.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    27943 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/drag_container/infinity_box_layer_one.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    25293 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/drag_container/widget_drag_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.689033 flet-box-gui-0.1.2.2/flet_box/extra_utils/icon_browser/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/icon_browser/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11552 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/icon_browser/icon_browser.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.689033 flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_down_phone/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_down_phone/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     8164 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_down_phone/footer_bar_menu_phone.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     2374 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_down_phone/selected_widget.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.693034 flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_right_phone/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_right_phone/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    24353 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_right_phone/right_bar_menu_phone.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.693034 flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_left_phone/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_left_phone/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11184 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.693034 flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_up_phone/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_up_phone/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     7973 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     1762 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    19563 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.693034 flet-box-gui-0.1.2.2/flet_box/extra_utils/phone_container/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/phone_container/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     2646 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/phone_container/nested_dict.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    11916 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/phone_container/widget_phone_editor.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.697034 flet-box-gui-0.1.2.2/flet_box/extra_utils/screen_manager/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/screen_manager/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    36478 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/screen_manager/screen_manager.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     2336 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/screen_manager/settings_screens.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)      636 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/screen_manager/write_file_proyect.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.697034 flet-box-gui-0.1.2.2/flet_box/extra_utils/settings_var/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/settings_var/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    54075 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/settings_var/save_export.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     3789 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/settings_var/settings_widget.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.697034 flet-box-gui-0.1.2.2/flet_box/extra_utils/tree_view/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/tree_view/__init__.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    10218 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/tree_view/color_hight_light_editor.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     4320 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/tree_view/tree_view.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    17067 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/extra_utils/tree_view/tree_view_text_editor.py
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    16302 2024-06-01 20:36:37.000000 flet-box-gui-0.1.2.2/flet_box/flet_box.py
+drwxr-xr-x   0 mjay      (1000) mjay      (1000)        0 2024-06-01 20:51:10.697034 flet-box-gui-0.1.2.2/flet_box_gui.egg-info/
+-rw-r--r--   0 mjay      (1000) mjay      (1000)    18628 2024-06-01 20:51:10.000000 flet-box-gui-0.1.2.2/flet_box_gui.egg-info/PKG-INFO
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     3381 2024-06-01 20:51:10.000000 flet-box-gui-0.1.2.2/flet_box_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        1 2024-06-01 20:51:10.000000 flet-box-gui-0.1.2.2/flet_box_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       47 2024-06-01 20:51:10.000000 flet-box-gui-0.1.2.2/flet_box_gui.egg-info/entry_points.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       42 2024-06-01 20:51:10.000000 flet-box-gui-0.1.2.2/flet_box_gui.egg-info/requires.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)        9 2024-06-01 20:51:10.000000 flet-box-gui-0.1.2.2/flet_box_gui.egg-info/top_level.txt
+-rw-r--r--   0 mjay      (1000) mjay      (1000)       38 2024-06-01 20:51:10.701034 flet-box-gui-0.1.2.2/setup.cfg
+-rw-r--r--   0 mjay      (1000) mjay      (1000)     5161 2024-06-01 20:50:54.000000 flet-box-gui-0.1.2.2/setup.py
```

### Comparing `flet-box-gui-0.1.2.1/CHANGELOG.md` & `flet-box-gui-0.1.2.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## 0.1.2.2 (June 01, 2024)
+  - start stable screen manager still have minor issues need fix export code to new code
+
 ## 0.1.2.1 (May 28, 2024)
   - fix readme
   - pypi aviable
   - first test app release
 
 ## 0.1.2 (May 27, 2024)
   - start dev screens
```

### Comparing `flet-box-gui-0.1.2.1/LICENSE` & `flet-box-gui-0.1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/README.md` & `flet-box-gui-0.1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,17 @@
 | ft.filledtonalbutton     | ✔ | ft.cupertinocheckbox     | ✔ | ft.cupertinoappbar       | ✘ |
 | ft.iconbutton            | ✔ | ft.cupertinoradio        | ✔ | ft.navigationdrawer      | ✘ |
 | ft.elevatedbutton        | ✔ | ft.cupertinoslider       | ✔ | ft.navigationrail        | ✘ |
 | ft.chip                  | ✔ | ft.cupertinoswitch       | ✔ | ft.menubar               | ✘ |
 | ft.outlinedbutton        | ✔ | ft.submenubutton         | ✘ | ft.appbar                | ✘ |
 | ft.bottomappbar          | ✘ | ft.dropdown              | ✘ | ft.cupertinonavigationbar| ✘ |
 | ft.bottomsheet           | ✘ | ft.datepicker            | ✘ | ft.searchbar             | ✘ |
-| ft.segmentedbutton       | ✘ | ft.timepicker            | ✘ |
-| ft.floatingactionbutton  | ✘ | ft.filepicker            | ✘ |
-|                          |   | ft.radio                 | ✘ |
+| ft.segmentedbutton       | ✘ | ft.timepicker            | ✘ |                          |   |
+| ft.floatingactionbutton  | ✘ | ft.filepicker            | ✘ |                          |   |
+|                          |   | ft.radio                 | ✘ |                          |   |
 |                          |   |                          |   |                          |   |
 | **WIDGETS STATUS**       |   |
 | ft.slider                | ✘ |
 | ft.progressbar           | ✘ |
 | ft.progressring          | ✘ |
 | ft.alertdialog           | ✘ |
 | ft.rangeslider           | ✘ |
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/avatar.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/avatar.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/avatar.png` & `flet-box-gui-0.1.2.2/flet_box/assets/avatar.png`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/dragg_container.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/dragg_container.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/dragg_container3.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/dragg_container3.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/image.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/image.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/img.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/img.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/logo.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/logo.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/logo_mark.png` & `flet-box-gui-0.1.2.2/flet_box/assets/logo_mark.png`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/my_avatar.png` & `flet-box-gui-0.1.2.2/flet_box/assets/my_avatar.png`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/no_imagen.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/no_imagen.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/splash.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/splash.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/assets/wallpaper.jpg` & `flet-box-gui-0.1.2.2/flet_box/assets/wallpaper.jpg`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/about/about.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/about/about.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/alert/alert_selected.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/alert/alert_selected.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/gpt_browser.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/chat_gpt_browser/gpt_browser.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/chat_gpt_browser/library_chatgpt.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/chat_gpt_browser/library_chatgpt.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/color_browser/color_browser.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/color_browser/color_browser.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/blur_color_entry.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/blur_color_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/bool_entry.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/bool_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/color_entry.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/color_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/double_entry.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/double_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/four_entry.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/four_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/gradient_entry.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/gradient_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/selection_entry.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/selection_entry.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/single_entry.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/single_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     """
     widget_content = 'data'
     def __init__(self,config_widget='exemple [value,bgcolor,width,height] ....',widget='',id_name_widget_dict=None):
         super().__init__()
 
         self.widget              = widget
+        # print(self.widget)
         self.widget_content      = self.widget_content
         self.id_name_widget_dict = id_name_widget_dict
 
         #: WE SET NEW NAME
         if config_widget == 'width':
             self.new_name         = 'Width - Height'
             self.attribute_widget = config_widget
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/config_container/widget_editor.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/config_container/widget_editor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,248 +1,277 @@
+import flet as ft
 
-from .double_entry    import DoubleEntry
-from .color_entry     import ColorEntry
-from .bool_entry      import BoolEntry
-from .four_entry      import FourEntry
-from .single_entry    import SingleEntry
-from .selection_entry import SelectionEntry
-from .gradient_entry  import GradientEntry
+from .double_entry     import DoubleEntry
+from .color_entry      import ColorEntry
+from .bool_entry       import BoolEntry
+from .four_entry       import FourEntry
+from .single_entry     import SingleEntry
+from .selection_entry  import SelectionEntry
+from .gradient_entry   import GradientEntry
 from .blur_color_entry import BlurColorEntry
-import flet as ft
 
 from ..settings_var.settings_widget import GLOBAL_VAR
 
 
 class BoxConfigContainer(ft.Stack):
-
-    def __init__(self,title=str(),controls=list()):
+    """
+    RIGHT BOX THAT CONTENT ALL WIDGET TO MODY ATTRIBUTES WILL SHOW OR NOT DEPENDING PREES CONFIGURATION ACTION BUTTON
+    """
+    def __init__(self,
+                 title: str="",
+                 controls: list=[]
+                 ):
         super().__init__()
         self.title    = title
         self.controls = controls
 
     def build(self):
         Drop_BoxConfigContainer = ft.Container(
                               padding = ft.padding.only(left=4, top=4, right=4, bottom=4),
                          content = ft.Column(
                                    controls = [
 
-
                                              ft.Container(
                                                        border_radius = ft.border_radius.all(20),
                                                        bgcolor       = ft.colors.BLACK26,
                                                        padding       = ft.padding.only(left=8, top=2, right=8, bottom=2),
-                                                       margin       = ft.margin.only(left=8, top=2, right=20, bottom=2),
-                                                       gradient      = ft.LinearGradient( begin=ft.alignment.top_center,end=ft.alignment.bottom_center,colors=[ft.colors.TEAL, ft.colors.BLACK38],),
+                                                       margin        = ft.margin.only( left=8, top=2, right=20, bottom=2),
+                                                       gradient      = ft.LinearGradient(
+                                                                                          begin = ft.alignment.top_center,
+                                                                                          end   = ft.alignment.bottom_center,
+                                                                                          colors= [ft.colors.TEAL, ft.colors.BLACK38],),
                                                   content=ft.Text(
                                                                  value       = self.title,
                                                                  text_align  = ft.TextAlign.CENTER,
 
                                                                  font_family = "Consolas", #"Consolas ,RobotoSlab
                                                                  color       = ft.colors.WHITE,
                                                        ),
                                                   ),
                                              ft.Container(
                                                        bgcolor       = ft.colors.BLACK38,
-                                                       width=425,
+                                                       width         = 425,
                                                        padding       = ft.padding.only(left=6, top=6, right=6, bottom=6),
                                                        border_radius = ft.border_radius.all(20),
                                                   content=ft.Row(
                                                                  wrap= True,
                                                             controls = self.controls
                                                        ,),),
                                                   ], #: <<<< controls
                                              ),      #: <<<< column
                                         )            #: <<<< container
         return Drop_BoxConfigContainer
 
 class Build_Editor(ft.Stack):
      """
-     Builder editor is a Row Container that will content all widgets editors inside
+     MAIN BUILDER EDITOR: IT'S A ROW CONTAINER THAT WILL CONTENT ALL WIDGET INSIDE WILL CALL BoxConfigContainer
+     FUNCTION THAT HAVE THE BOX TO SHOW ASACTLY THE WIDGET ATTRIBUTES TO MODIFY
 
      Tabs:
         Container:
                 edit_Container: value
         Widget:
                 edit_Widget: value
 
      NOTE:
         Is necessary put class widget of the widget to edit Attributes
      """
 
-     def __init__(self,widget='Erase this test'):
+     def __init__(self,widget=""):
           super().__init__()
-          self.widget = widget
+          #: VERY IMPORTANT
+          #: WIDGET PHONE SELECTED TO MODIFY ATTRIBUTES
+          # if not widget == "":
+          #      self.widget = widget
+          # else:
+          #      print('hello world')
+          # self.widget = GLOBAL_VAR(get_global_var='main_screen').build()
+          # self.widget = ""
+          # print(self.widget.uid ,'<<<<<<< WIDGER')
+          # self.build()
+          self.widget = ''
 
      def build(self):
           """
           ALL IN THIS APP IS A MODULE THAT'S WAY YOU MAY TAKE THE PART THAT YOU WANT REBUILD
 
           widgets_dict <= IS A DICT THAT CONTAIN ALL WIDGET THAT ARE WATING TO SHOW BECOUS BY DEFAULD ARE VISIBLE = OFF
           """
           global Drop_Build_Editor
+          # self.selected_screen           = GLOBAL_VAR(get_global_var='SELECT_SCREEN')
+
+          # self.main_phone                 = self.widget
+          # self.main_phone                 = GLOBAL_VAR(get_global_var='SELECTED_SCREEN')
+
+          # self.main_phone                 = GLOBAL_VAR(get_global_var='PHONE_MAIN')
+          # self.main_phone                 = GLOBAL_VAR(get_global_var='PHONE_MAIN')
+          # self.main_phone_conainer        = GLOBAL_VAR(get_global_var='PHONE_CONTAINER')
+          # self.main_phone_conainer_conent = GLOBAL_VAR(get_global_var='PHONE_CONTAINER_CONTENT')
+
 
-          self.main_phone                 = GLOBAL_VAR(get_global_var='PHONE_MAIN')
-          self.main_phone_conainer        = GLOBAL_VAR(get_global_var='PHONE_CONTAINER')
-          self.main_phone_conainer_conent = GLOBAL_VAR(get_global_var='PHONE_CONTAINER_CONTENT')
+          # print(self.main_phone,'main_phone')
+          self.main_phone                 = GLOBAL_VAR(get_global_var='SELECTED_SCREEN')            # main_phone
+          self.main_phone_conainer        =  self.main_phone.content.content.content                # main_phone_conainer
+          self.main_phone_conainer_conent =  self.main_phone.content.content.content.content        # main_phone_conainer_conent
 
           self.container_widget           = GLOBAL_VAR(get_global_var='SELECT_DROPP_WIDGET_CONTAINER')
           self.container_widget_content   = GLOBAL_VAR(get_global_var='SELECT_DROPP_WIDGET_CONTAINER_CONTENT')
 
           widgets_dict = {
 
                #: ESPECIAL WIDGETS ONLY FOR PHONE
 
-               'phone_margin'       :FourEntry(      config_widget = 'padding'                ,widget = self.main_phone_conainer),
+               'phone_margin'       :FourEntry(      config_widget='padding'               ,widget=self.main_phone_conainer        ,id_name_widget_dict="main_phone_conainer"),
 
-               'phone_image_src'    :SingleEntry(    config_widget = 'image_src'             ,widget = self.main_phone),
-               'phone_image_opacity':SingleEntry(    config_widget = 'image_opacity'         ,widget = self.main_phone),
-              'column_phone_spacing':SingleEntry(    config_widget = 'spacing'               ,widget = self.main_phone_conainer_conent),
+               'phone_image_src'    :SingleEntry(    config_widget='image_src'             ,widget=self.main_phone                 ,id_name_widget_dict='main_phone'),
+               'phone_image_opacity':SingleEntry(    config_widget='image_opacity'         ,widget=self.main_phone                 ,id_name_widget_dict='main_phone'),
+              'column_phone_spacing':SingleEntry(    config_widget='spacing'               ,widget=self.main_phone_conainer_conent ,id_name_widget_dict="main_phone_conainer_conent"),
 
-               'phone_bgcolor'      :ColorEntry(     config_widget = 'bgcolor'               ,widget = self.main_phone_conainer),
+               'phone_bgcolor'      :ColorEntry(     config_widget='bgcolor'               ,widget=self.main_phone_conainer        ,id_name_widget_dict="main_phone_conainer"),
 
-               'column_phone_wrap'  :BoolEntry(      config_widget = 'wrap'                  ,widget = self.main_phone_conainer_conent),
-               'column_phone_tight' :BoolEntry(      config_widget = 'tight'                 ,widget = self.main_phone_conainer_conent),
-               'column_phone_scroll':BoolEntry(      config_widget = 'scroll'                ,widget = self.main_phone_conainer_conent),
+               'column_phone_wrap'  :BoolEntry(      config_widget='wrap'                  ,widget=self.main_phone_conainer_conent ,id_name_widget_dict="main_phone_conainer_conent"),
+               'column_phone_tight' :BoolEntry(      config_widget='tight'                 ,widget=self.main_phone_conainer_conent ,id_name_widget_dict="main_phone_conainer_conent"),
+               'column_phone_scroll':BoolEntry(      config_widget='scroll'                ,widget=self.main_phone_conainer_conent ,id_name_widget_dict="main_phone_conainer_conent"),
 
-               'phone_image_fit'    :SelectionEntry( config_widget = 'image_fit'             ,widget = self.main_phone),
-           'column_phone_alignment' :SelectionEntry( config_widget = 'alignment'             ,widget = self.main_phone_conainer_conent),
-'column_phone_horizontal_alignment' :SelectionEntry( config_widget = 'horizontal_alignment'  ,widget = self.main_phone_conainer_conent),
+               'phone_image_fit'    :SelectionEntry( config_widget='image_fit'             ,widget=self.main_phone                 ,id_name_widget_dict='main_phone'),
+           'column_phone_alignment' :SelectionEntry( config_widget='alignment'             ,widget=self.main_phone_conainer_conent ,id_name_widget_dict="main_phone_conainer_conent"),
+'column_phone_horizontal_alignment' :SelectionEntry( config_widget='horizontal_alignment'  ,widget=self.main_phone_conainer_conent ,id_name_widget_dict="main_phone_conainer_conent"),
 
-               'phone_gradient'     :GradientEntry(  config_widget = 'gradient'              ,widget = self.main_phone),
-               'phone_blur'         :DoubleEntry(    config_widget = 'blur'                  ,widget = self.main_phone_conainer),
+               'phone_gradient'     :GradientEntry(  config_widget='gradient'              ,widget=self.main_phone                 ,id_name_widget_dict='main_phone'),
+               'phone_blur'         :DoubleEntry(    config_widget='blur'                  ,widget=self.main_phone_conainer        ,id_name_widget_dict="main_phone_conainer"),
 
                #: ESPECIAL WIDGETS ONLY FOR CONTAINERS
 
-               'container_rotate'   :SingleEntry(    config_widget = 'rotate'                ,widget = self.container_widget),
-               'container_scale'    :SingleEntry(    config_widget = 'scale'                 ,widget = self.container_widget),
-               'container_padding'  :FourEntry(      config_widget = 'padding'               ,widget = self.container_widget),
-               'container_margin'   :FourEntry(      config_widget = 'margin'                ,widget = self.container_widget),
-               'container_offset'   :DoubleEntry(    config_widget = 'offset'                ,widget = self.container_widget),
-               'container_alignment':SelectionEntry( config_widget = 'alignment '            ,widget = self.container_widget),
-
-               'container_width'    :DoubleEntry(    config_widget = 'width'                 ,widget = self.container_widget),
-               'container_scale'    :SingleEntry(    config_widget = 'scale'                 ,widget = self.container_widget),
-               'container_border'   :DoubleEntry(    config_widget = 'border'                ,widget = self.container_widget),
-               'container_expand'   :BoolEntry(      config_widget = 'expand'                ,widget = self.container_widget),
-               'container_ink'      :BoolEntry(      config_widget = 'ink'                   ,widget = self.container_widget),
-               'container_visible'  :BoolEntry(      config_widget = 'visible'               ,widget = self.container_widget),
-           'container_border_radius':FourEntry(      config_widget = 'border_radius'         ,widget = self.container_widget),
-
-               # 'container_blur'     :DoubleEntry(    config_widget = 'blur'                  ,widget = self.container_widget),
-               'container_bgcolor'  :ColorEntry(     config_widget = 'bgcolor'               ,widget = self.container_widget),
-               'BlurColorEntry'     :BlurColorEntry( config_widget = 'blur'                  ,widget = self.container_widget),
-
-               'shadow_color'       :ColorEntry(     config_widget = 'shadow_color'          ,widget = self.container_widget),
-               'container_gradient' :GradientEntry(  config_widget = 'gradient'              ,widget = self.container_widget),
-
-           'container_image_src'    :SingleEntry(    config_widget = 'image_src'             ,widget = self.container_widget),
-           'container_image_opacity':SingleEntry(    config_widget = 'image_opacity'         ,widget = self.container_widget),
-           'container_image_fit'    :SelectionEntry( config_widget = 'image_fit'             ,widget = self.container_widget),
+               'container_rotate'   :SingleEntry(    config_widget='rotate'                ,widget=self.container_widget),
+               'container_scale'    :SingleEntry(    config_widget='scale'                 ,widget=self.container_widget),
+               'container_padding'  :FourEntry(      config_widget='padding'               ,widget=self.container_widget),
+               'container_margin'   :FourEntry(      config_widget='margin'                ,widget=self.container_widget),
+               'container_offset'   :DoubleEntry(    config_widget='offset'                ,widget=self.container_widget),
+               'container_alignment':SelectionEntry( config_widget='alignment '            ,widget=self.container_widget),
+
+               'container_width'    :DoubleEntry(    config_widget='width'                 ,widget=self.container_widget),
+               'container_scale'    :SingleEntry(    config_widget='scale'                 ,widget=self.container_widget),
+               'container_border'   :DoubleEntry(    config_widget='border'                ,widget=self.container_widget),
+               'container_expand'   :BoolEntry(      config_widget='expand'                ,widget=self.container_widget),
+               'container_ink'      :BoolEntry(      config_widget='ink'                   ,widget=self.container_widget),
+               'container_visible'  :BoolEntry(      config_widget='visible'               ,widget=self.container_widget),
+           'container_border_radius':FourEntry(      config_widget='border_radius'         ,widget=self.container_widget),
+
+               # 'container_blur'     :DoubleEntry(    config_widget='blur'                  ,widget=self.container_widget),
+               'container_bgcolor'  :ColorEntry(     config_widget='bgcolor'               ,widget=self.container_widget),
+               'BlurColorEntry'     :BlurColorEntry( config_widget='blur'                  ,widget=self.container_widget),
+
+               'shadow_color'       :ColorEntry(     config_widget='shadow_color'          ,widget=self.container_widget),
+               'container_gradient' :GradientEntry(  config_widget='gradient'              ,widget=self.container_widget),
+
+           'container_image_src'    :SingleEntry(    config_widget='image_src'             ,widget=self.container_widget),
+           'container_image_opacity':SingleEntry(    config_widget='image_opacity'         ,widget=self.container_widget),
+           'container_image_fit'    :SelectionEntry( config_widget='image_fit'             ,widget=self.container_widget),
 
                #: ESPECIAL WIDGETS ONLY FOR WIDGET
 
-               'text'                :SingleEntry(config_widget = 'text'             ,widget = self.container_widget_content , id_name_widget_dict='text'),
-               'name'                :SingleEntry(config_widget = 'name'             ,widget = self.container_widget_content , id_name_widget_dict='name'),
-               'size'                :SingleEntry(config_widget = 'size'             ,widget = self.container_widget_content , id_name_widget_dict='size'),
-               'label'               :SingleEntry(config_widget = 'label'            ,widget = self.container_widget_content , id_name_widget_dict='label'),
-               'value'               :SingleEntry(config_widget = 'value'            ,widget = self.container_widget_content , id_name_widget_dict='value'),
-
-               'hint_text'           :SingleEntry(config_widget = 'hint_text'        ,widget = self.container_widget_content , id_name_widget_dict='hint_text'),
-               'counter_text'        :SingleEntry(config_widget = 'counter_text'     ,widget = self.container_widget_content , id_name_widget_dict='counter_text'),
-               'suffix_text'         :SingleEntry(config_widget = 'suffix_text'      ,widget = self.container_widget_content , id_name_widget_dict='suffix_text'),
-               'url'                 :SingleEntry(config_widget = 'url'              ,widget = self.container_widget_content , id_name_widget_dict='url'),
-               'url_target'          :SingleEntry(config_widget = 'url_target'       ,widget = self.container_widget_content , id_name_widget_dict='url_target'),
-               'icon'                :SingleEntry(config_widget = 'icon'             ,widget = self.container_widget_content , id_name_widget_dict='icon'),
-               'tooltip'             :SingleEntry(config_widget = 'tooltip'          ,widget = self.container_widget_content , id_name_widget_dict='tooltip'),
-               'src'                 :SingleEntry(config_widget = 'src'              ,widget = self.container_widget_content , id_name_widget_dict='src'),
-               'data'                :SingleEntry(config_widget = 'data'             ,widget = self.container_widget_content , id_name_widget_dict='data'),
-               'semantics_label'     :SingleEntry(config_widget = 'semantics_label'  ,widget = self.container_widget_content , id_name_widget_dict='semantics_label'),
-               'src_base64'          :SingleEntry(config_widget = 'src_base64'       ,widget = self.container_widget_content , id_name_widget_dict='src_base64'),
-               'image_src'           :SingleEntry(config_widget = 'image_src'        ,widget = self.container_widget_content , id_name_widget_dict='image_src'),
-               'blur_radius'         :SingleEntry(config_widget = 'blur_radius'      ,widget = self.container_widget_content , id_name_widget_dict='blur_radius'),
-               'spread_radius'       :SingleEntry(config_widget = 'spread_radius'    ,widget = self.container_widget_content , id_name_widget_dict='spread_radius'),
-               'elevation'           :SingleEntry(config_widget = 'elevation'        ,widget = self.container_widget_content , id_name_widget_dict='elevation'),
-               'rotate'              :SingleEntry(config_widget = 'rotate'           ,widget = self.container_widget_content , id_name_widget_dict='rotate'),
-               'scale'               :SingleEntry(config_widget = 'scale'            ,widget = self.container_widget_content , id_name_widget_dict='scale'),
-               'aspect_ratio'        :SingleEntry(config_widget = 'aspect_ratio'     ,widget = self.container_widget_content , id_name_widget_dict='aspect_ratio'),
-               'runs_count'          :SingleEntry(config_widget = 'runs_count'       ,widget = self.container_widget_content , id_name_widget_dict='runs_count'),
-               'run_spacing'         :SingleEntry(config_widget = 'run_spacing'      ,widget = self.container_widget_content , id_name_widget_dict='run_spacing'),
-               'spacing'             :SingleEntry(config_widget = 'spacing'          ,widget = self.container_widget_content , id_name_widget_dict='spacing'),
-               'child_aspect_ratio'  :SingleEntry(config_widget ='child_aspect_ratio',widget = self.container_widget_content , id_name_widget_dict='child_aspect_ratio'),
-               'max_extent'          :SingleEntry(config_widget = 'max_extent'       ,widget = self.container_widget_content , id_name_widget_dict='max_extent'),
-               'min_lines'           :SingleEntry(config_widget = 'min_lines'        ,widget = self.container_widget_content , id_name_widget_dict='min_lines'),
-               'max_lines'           :SingleEntry(config_widget = 'max_lines'        ,widget = self.container_widget_content , id_name_widget_dict='max_lines'),
-               'border_width'        :SingleEntry(config_widget = 'border_width'     ,widget = self.container_widget_content , id_name_widget_dict='border_width'),
-               'text_size'           :SingleEntry(config_widget = 'text_size'        ,widget = self.container_widget_content , id_name_widget_dict='text_size'),
-               'image_opacity'       :SingleEntry(config_widget = 'image_opacity'    ,widget = self.container_widget_content , id_name_widget_dict='image_opacity'),
-               'opacity'             :SingleEntry(config_widget = 'opacity'          ,widget = self.container_widget_content , id_name_widget_dict='opacity'),
+               'text'                :SingleEntry(config_widget='text'             ,widget=self.container_widget_content , id_name_widget_dict='text'),
+               'name'                :SingleEntry(config_widget='name'             ,widget=self.container_widget_content , id_name_widget_dict='name'),
+               'size'                :SingleEntry(config_widget='size'             ,widget=self.container_widget_content , id_name_widget_dict='size'),
+               'label'               :SingleEntry(config_widget='label'            ,widget=self.container_widget_content , id_name_widget_dict='label'),
+               'value'               :SingleEntry(config_widget='value'            ,widget=self.container_widget_content , id_name_widget_dict='value'),
+
+               'hint_text'           :SingleEntry(config_widget='hint_text'        ,widget=self.container_widget_content , id_name_widget_dict='hint_text'),
+               'counter_text'        :SingleEntry(config_widget='counter_text'     ,widget=self.container_widget_content , id_name_widget_dict='counter_text'),
+               'suffix_text'         :SingleEntry(config_widget='suffix_text'      ,widget=self.container_widget_content , id_name_widget_dict='suffix_text'),
+               'url'                 :SingleEntry(config_widget='url'              ,widget=self.container_widget_content , id_name_widget_dict='url'),
+               'url_target'          :SingleEntry(config_widget='url_target'       ,widget=self.container_widget_content , id_name_widget_dict='url_target'),
+               'icon'                :SingleEntry(config_widget='icon'             ,widget=self.container_widget_content , id_name_widget_dict='icon'),
+               'tooltip'             :SingleEntry(config_widget='tooltip'          ,widget=self.container_widget_content , id_name_widget_dict='tooltip'),
+               'src'                 :SingleEntry(config_widget='src'              ,widget=self.container_widget_content , id_name_widget_dict='src'),
+               'data'                :SingleEntry(config_widget='data'             ,widget=self.container_widget_content , id_name_widget_dict='data'),
+               'semantics_label'     :SingleEntry(config_widget='semantics_label'  ,widget=self.container_widget_content , id_name_widget_dict='semantics_label'),
+               'src_base64'          :SingleEntry(config_widget='src_base64'       ,widget=self.container_widget_content , id_name_widget_dict='src_base64'),
+               'image_src'           :SingleEntry(config_widget='image_src'        ,widget=self.container_widget_content , id_name_widget_dict='image_src'),
+               'blur_radius'         :SingleEntry(config_widget='blur_radius'      ,widget=self.container_widget_content , id_name_widget_dict='blur_radius'),
+               'spread_radius'       :SingleEntry(config_widget='spread_radius'    ,widget=self.container_widget_content , id_name_widget_dict='spread_radius'),
+               'elevation'           :SingleEntry(config_widget='elevation'        ,widget=self.container_widget_content , id_name_widget_dict='elevation'),
+               'rotate'              :SingleEntry(config_widget='rotate'           ,widget=self.container_widget_content , id_name_widget_dict='rotate'),
+               'scale'               :SingleEntry(config_widget='scale'            ,widget=self.container_widget_content , id_name_widget_dict='scale'),
+               'aspect_ratio'        :SingleEntry(config_widget='aspect_ratio'     ,widget=self.container_widget_content , id_name_widget_dict='aspect_ratio'),
+               'runs_count'          :SingleEntry(config_widget='runs_count'       ,widget=self.container_widget_content , id_name_widget_dict='runs_count'),
+               'run_spacing'         :SingleEntry(config_widget='run_spacing'      ,widget=self.container_widget_content , id_name_widget_dict='run_spacing'),
+               'spacing'             :SingleEntry(config_widget='spacing'          ,widget=self.container_widget_content , id_name_widget_dict='spacing'),
+               'child_aspect_ratio'  :SingleEntry(config_widget ='child_aspect_ratio',widget=self.container_widget_content , id_name_widget_dict='child_aspect_ratio'),
+               'max_extent'          :SingleEntry(config_widget='max_extent'       ,widget=self.container_widget_content , id_name_widget_dict='max_extent'),
+               'min_lines'           :SingleEntry(config_widget='min_lines'        ,widget=self.container_widget_content , id_name_widget_dict='min_lines'),
+               'max_lines'           :SingleEntry(config_widget='max_lines'        ,widget=self.container_widget_content , id_name_widget_dict='max_lines'),
+               'border_width'        :SingleEntry(config_widget='border_width'     ,widget=self.container_widget_content , id_name_widget_dict='border_width'),
+               'text_size'           :SingleEntry(config_widget='text_size'        ,widget=self.container_widget_content , id_name_widget_dict='text_size'),
+               'image_opacity'       :SingleEntry(config_widget='image_opacity'    ,widget=self.container_widget_content , id_name_widget_dict='image_opacity'),
+               'opacity'             :SingleEntry(config_widget='opacity'          ,widget=self.container_widget_content , id_name_widget_dict='opacity'),
 
                #: DOUBLE SELECTION ENTRY
 
-               'width'               :DoubleEntry(config_widget = 'width'            ,widget = self.container_widget_content , id_name_widget_dict='width'),
-               'border'              :DoubleEntry(config_widget = 'border'           ,widget = self.container_widget_content , id_name_widget_dict='border'),
-               'offset'              :DoubleEntry(config_widget = 'offset'           ,widget = self.container_widget_content , id_name_widget_dict='offset'),
-               'blur'                :DoubleEntry(config_widget = 'blur'             ,widget = self.container_widget_content , id_name_widget_dict='blur'),
+               'width'               :DoubleEntry(config_widget='width'            ,widget=self.container_widget_content , id_name_widget_dict='width'),
+               'border'              :DoubleEntry(config_widget='border'           ,widget=self.container_widget_content , id_name_widget_dict='border'),
+               'offset'              :DoubleEntry(config_widget='offset'           ,widget=self.container_widget_content , id_name_widget_dict='offset'),
+               'blur'                :DoubleEntry(config_widget='blur'             ,widget=self.container_widget_content , id_name_widget_dict='blur'),
 
                #: 4 SELECTION ENTRIE S
 
-               'padding'             :FourEntry(config_widget = 'padding'            ,widget = self.container_widget_content , id_name_widget_dict='padding'),
-               'margin'              :FourEntry(config_widget = 'margin'             ,widget = self.container_widget_content , id_name_widget_dict='margin'),
-               'border_radius'       :FourEntry(config_widget = 'border_radius'      ,widget = self.container_widget_content , id_name_widget_dict='border_radius'),
+               'padding'             :FourEntry(config_widget='padding'            ,widget=self.container_widget_content , id_name_widget_dict='padding'),
+               'margin'              :FourEntry(config_widget='margin'             ,widget=self.container_widget_content , id_name_widget_dict='margin'),
+               'border_radius'       :FourEntry(config_widget='border_radius'      ,widget=self.container_widget_content , id_name_widget_dict='border_radius'),
 
                #: COLOR ENTRY ['RED' ...]
 
-               'bgcolor'             :ColorEntry(config_widget= 'bgcolor'            ,widget = self.container_widget_content , id_name_widget_dict='bgcolor'),
-               'color'               :ColorEntry(config_widget= 'color'              ,widget = self.container_widget_content , id_name_widget_dict='color'),
-               'icon_color'          :ColorEntry(config_widget= 'icon_color'         ,widget = self.container_widget_content , id_name_widget_dict='icon_color'),
-               'check_color'         :ColorEntry(config_widget= 'check_color'        ,widget = self.container_widget_content , id_name_widget_dict='check_color'),
-               'fill_color'          :ColorEntry(config_widget= 'fill_color'         ,widget = self.container_widget_content , id_name_widget_dict='fill_color'),
-               'border_color'        :ColorEntry(config_widget= 'border_color'       ,widget = self.container_widget_content , id_name_widget_dict='border_color'),
-               'focused_bgcolor'     :ColorEntry(config_widget= 'focused_bgcolor'    ,widget = self.container_widget_content , id_name_widget_dict='focused_bgcolor'),
-               'focused_border_color':ColorEntry(config_widget= 'focused_border_color',widget = self.container_widget_content, id_name_widget_dict='focused_border_color'),
-               'box_shadow'          :ColorEntry(config_widget= 'box_shadow',         widget = self.container_widget_content , id_name_widget_dict='box_shadow'),
+               'bgcolor'             :ColorEntry(config_widget= 'bgcolor'            ,widget=self.container_widget_content , id_name_widget_dict='bgcolor'),
+               'color'               :ColorEntry(config_widget= 'color'              ,widget=self.container_widget_content , id_name_widget_dict='color'),
+               'icon_color'          :ColorEntry(config_widget= 'icon_color'         ,widget=self.container_widget_content , id_name_widget_dict='icon_color'),
+               'check_color'         :ColorEntry(config_widget= 'check_color'        ,widget=self.container_widget_content , id_name_widget_dict='check_color'),
+               'fill_color'          :ColorEntry(config_widget= 'fill_color'         ,widget=self.container_widget_content , id_name_widget_dict='fill_color'),
+               'border_color'        :ColorEntry(config_widget= 'border_color'       ,widget=self.container_widget_content , id_name_widget_dict='border_color'),
+               'focused_bgcolor'     :ColorEntry(config_widget= 'focused_bgcolor'    ,widget=self.container_widget_content , id_name_widget_dict='focused_bgcolor'),
+               'focused_border_color':ColorEntry(config_widget= 'focused_border_color',widget=self.container_widget_content, id_name_widget_dict='focused_border_color'),
+               'box_shadow'          :ColorEntry(config_widget= 'box_shadow',         widget=self.container_widget_content , id_name_widget_dict='box_shadow'),
 
                #: BOOL ENTRY [TRUE FALSE]
 
-               'expand':             BoolEntry(config_widget = 'expand'              ,widget = self.container_widget_content , id_name_widget_dict='expand'),
-               'ink':                BoolEntry(config_widget = 'ink'                 ,widget = self.container_widget_content , id_name_widget_dict='ink'),
-               'scroll':             BoolEntry(config_widget = 'scroll'              ,widget = self.container_widget_content , id_name_widget_dict='scroll'),
-               'wrap':               BoolEntry(config_widget = 'wrap'                ,widget = self.container_widget_content , id_name_widget_dict='wrap'),
-               'tight':              BoolEntry(config_widget = 'tight'               ,widget = self.container_widget_content , id_name_widget_dict='tight'),
-               'visible':            BoolEntry(config_widget = 'visible'             ,widget = self.container_widget_content , id_name_widget_dict='visible'),
-               'multiline':          BoolEntry(config_widget = 'multiline'           ,widget = self.container_widget_content , id_name_widget_dict='multiline'),
-               'disabled':           BoolEntry(config_widget = 'disabled'            ,widget = self.container_widget_content , id_name_widget_dict='disabled'),
-               'read_only':          BoolEntry(config_widget = 'read_only'           ,widget = self.container_widget_content , id_name_widget_dict='read_only'),
-               'password':           BoolEntry(config_widget = 'password'            ,widget = self.container_widget_content , id_name_widget_dict='password'),
-               'filled':             BoolEntry(config_widget = 'filled'              ,widget = self.container_widget_content , id_name_widget_dict='filled'),
-               'adaptive':           BoolEntry(config_widget = 'adaptive'            ,widget = self.container_widget_content , id_name_widget_dict='adaptive'),
-               'tristate':           BoolEntry(config_widget = 'tristate'            ,widget = self.container_widget_content , id_name_widget_dict='tristate'),
-               'autofocus':          BoolEntry(config_widget = 'autofocus'           ,widget = self.container_widget_content , id_name_widget_dict='read_only'),
-               'horizontal':         BoolEntry(config_widget = 'horizontal'          ,widget = self.container_widget_content , id_name_widget_dict='horizontal'),
-               'can_reveal_password':BoolEntry(config_widget = 'can_reveal_password' ,widget = self.container_widget_content , id_name_widget_dict='can_reveal_password'),
-               'capitalization':     BoolEntry(config_widget = 'capitalization'      ,widget = self.container_widget_content , id_name_widget_dict='capitalization'),
-               'gapless_playback':   BoolEntry(config_widget = 'gapless_playback'    ,widget = self.container_widget_content , id_name_widget_dict='gapless_playback'),
+               'expand':             BoolEntry(config_widget='expand'              ,widget=self.container_widget_content , id_name_widget_dict='expand'),
+               'ink':                BoolEntry(config_widget='ink'                 ,widget=self.container_widget_content , id_name_widget_dict='ink'),
+               'scroll':             BoolEntry(config_widget='scroll'              ,widget=self.container_widget_content , id_name_widget_dict='scroll'),
+               'wrap':               BoolEntry(config_widget='wrap'                ,widget=self.container_widget_content , id_name_widget_dict='wrap'),
+               'tight':              BoolEntry(config_widget='tight'               ,widget=self.container_widget_content , id_name_widget_dict='tight'),
+               'visible':            BoolEntry(config_widget='visible'             ,widget=self.container_widget_content , id_name_widget_dict='visible'),
+               'multiline':          BoolEntry(config_widget='multiline'           ,widget=self.container_widget_content , id_name_widget_dict='multiline'),
+               'disabled':           BoolEntry(config_widget='disabled'            ,widget=self.container_widget_content , id_name_widget_dict='disabled'),
+               'read_only':          BoolEntry(config_widget='read_only'           ,widget=self.container_widget_content , id_name_widget_dict='read_only'),
+               'password':           BoolEntry(config_widget='password'            ,widget=self.container_widget_content , id_name_widget_dict='password'),
+               'filled':             BoolEntry(config_widget='filled'              ,widget=self.container_widget_content , id_name_widget_dict='filled'),
+               'adaptive':           BoolEntry(config_widget='adaptive'            ,widget=self.container_widget_content , id_name_widget_dict='adaptive'),
+               'tristate':           BoolEntry(config_widget='tristate'            ,widget=self.container_widget_content , id_name_widget_dict='tristate'),
+               'autofocus':          BoolEntry(config_widget='autofocus'           ,widget=self.container_widget_content , id_name_widget_dict='read_only'),
+               'horizontal':         BoolEntry(config_widget='horizontal'          ,widget=self.container_widget_content , id_name_widget_dict='horizontal'),
+               'can_reveal_password':BoolEntry(config_widget='can_reveal_password' ,widget=self.container_widget_content , id_name_widget_dict='can_reveal_password'),
+               'capitalization':     BoolEntry(config_widget='capitalization'      ,widget=self.container_widget_content , id_name_widget_dict='capitalization'),
+               'gapless_playback':   BoolEntry(config_widget='gapless_playback'    ,widget=self.container_widget_content , id_name_widget_dict='gapless_playback'),
 
                #: SELECTION ENTRY
 
-               'image_fit':          SelectionEntry(config_widget = 'image_fit'           ,widget = self.container_widget_content , id_name_widget_dict='image_fit'),
-               'weight':             SelectionEntry(config_widget = 'weight'              ,widget = self.container_widget_content , id_name_widget_dict='weight'),
-               'keyboard_type':      SelectionEntry(config_widget = 'keyboard_type'       ,widget = self.container_widget_content , id_name_widget_dict='keyboard_type'),
-               'text_align':         SelectionEntry(config_widget = 'text_align'          ,widget = self.container_widget_content , id_name_widget_dict='text_align'),
-               'alignment':          SelectionEntry(config_widget = 'alignment'           ,widget = self.container_widget_content , id_name_widget_dict='alignment'),
-               'content_alignment':  SelectionEntry(config_widget = 'content_alignment'   ,widget = self.container_widget_content , id_name_widget_dict='content_alignment'),
-               'vertical_alignment' :SelectionEntry(config_widget = 'vertical_alignment'  ,widget = self.container_widget_content , id_name_widget_dict='vertical_alignment'),
-              'horizontal_alignment':SelectionEntry(config_widget = 'horizontal_alignment',widget = self.container_widget_content , id_name_widget_dict='horizontal_alignment'),
+               'image_fit':          SelectionEntry(config_widget='image_fit'           ,widget=self.container_widget_content , id_name_widget_dict='image_fit'),
+               'weight':             SelectionEntry(config_widget='weight'              ,widget=self.container_widget_content , id_name_widget_dict='weight'),
+               'keyboard_type':      SelectionEntry(config_widget='keyboard_type'       ,widget=self.container_widget_content , id_name_widget_dict='keyboard_type'),
+               'text_align':         SelectionEntry(config_widget='text_align'          ,widget=self.container_widget_content , id_name_widget_dict='text_align'),
+               'alignment':          SelectionEntry(config_widget='alignment'           ,widget=self.container_widget_content , id_name_widget_dict='alignment'),
+               'content_alignment':  SelectionEntry(config_widget='content_alignment'   ,widget=self.container_widget_content , id_name_widget_dict='content_alignment'),
+               'vertical_alignment' :SelectionEntry(config_widget='vertical_alignment'  ,widget=self.container_widget_content , id_name_widget_dict='vertical_alignment'),
+              'horizontal_alignment':SelectionEntry(config_widget='horizontal_alignment',widget=self.container_widget_content , id_name_widget_dict='horizontal_alignment'),
 
                #: GRADIEN ENTRY
 
-               'gradient':           GradientEntry(config_widget  = 'gradient'            ,widget = self.container_widget_content , id_name_widget_dict='gradient'),
+               'gradient':           GradientEntry(config_widget ='gradient'            ,widget=self.container_widget_content , id_name_widget_dict='gradient'),
           }
 
-          self.main_phone =ft.Container(
+          self.main_phone_tab_1 =ft.Container(
                                    padding = ft.padding.only(left=4, top=4, right=4, bottom=4),
                               content = ft.Column(
                                              scroll="HIDDEN",
                                              controls = [
                                                        BoxConfigContainer(
                                                                  title='Color Phone Container',
                                                             controls=[
@@ -454,30 +483,30 @@
                               content  = ft.Tabs(
                                              label_color             = 'BLUE',
                                              indicator_border_radius = ft.border_radius.all(20),
                                         tabs = [
                                                        ft.Tab(
                                                                  text    = "Box Phone",
 
-                                                            content = self.main_phone
+                                                            content = self.main_phone_tab_1
                                                        ),
                                                        ft.Tab(
                                                                  text    = "Box Container",
                                                             content = self.widget_container
                                                        ),
                                                        ft.Tab(
                                                                  text    = "Box Widget",
                                                             content = self.widget_container_content,
                                                          ),
                                              ],
                                             ),
                               )
 
           GLOBAL_VAR(set_global_var={
-                                        'CONFIG_TABS_PHONE':self.main_phone,
+                                        'CONFIG_TABS_PHONE':self.main_phone_tab_1,
                                    'CONFIG_TABS_CONTAINERS':self.widget_container,
                            'CONFIG_TABS_CONTAINERS_CONTENT':self.widget_container_content,
                                       'LIST_KEYS_DICT_USED':widgets_dict.keys(),
                                    } )
 
           return Drop_Build_Editor
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/dragg_widget.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/drag_container/dragg_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,18 @@
           """
           NOTE:
 
           1. SET IN GLOBAL VAR THE SELECTED WIDGET
           2. RESET THE LIST listWidgetUpdate
 
           """
+
           CHECK_DATA = GLOBAL_VAR(get_global_var='BOOL_SHOW_SELECTED')
+          GLOBAL_VAR(set_global_var={'LIST_SELECTED_WIDGETS':[]})
+
 
           if CHECK_DATA:
 
                #: HIDE TABS IF CLICK PRESS IS NO IN PHONE CONTAINER WIDGET
                CONFIG_TABS_CONTAINERS                 = GLOBAL_VAR(get_global_var='CONFIG_TABS_CONTAINERS')
                CONFIG_TABS_CONTAINERS.visible         = False
                CONFIG_TABS_CONTAINERS.update()
@@ -128,15 +131,15 @@
           TEXT_DRAGG_WIDGET.controls[0].update()
 
           if selected_widget_clicked:
                selected_widget_clicked.border = ft.border.all(0, ft.colors.TRANSPARENT)
                selected_widget_clicked.update()
 
           #: run  only in production
-          print(data,'<=== selected DRAGG widget')
+          print(data,'<=== SELECTED DRAG WIDGET: file drag_widget.py')
 
           #: NEED ACTIVATE ALER OF SELECTED WIDGET
           selected_widget         = GLOBAL_VAR( get_global_var='ALERT_WIDGET')
           selected_widget.offset  = (0,-7)
           selected_widget.visible = True
           selected_widget.update()
           time.sleep(0.5)
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/infinity_box_layer_one.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/drag_container/infinity_box_layer_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,19 +242,19 @@
 
 
           #: SET WIDGET DROPPED TO DICT DATABASE TO EXPORT PROYECT
           #: GLOBAL_VAR(set_global_var={'EXPORT_DATA_PHONE':{self.infinityDropWidget[0].id:self.infinityDropWidget[0]}})
 
           print('============')
           print(f"""
-[+]             selected_widget: {self.dataPassed},
-[+]             ID_widget: {numWidget},
-[+]             UID: {self.infinityDropWidget[0].uid}
-[+]             ID tooltip: {self.infinityDropWidget[0].tooltip}
-[+]  Content: {self.infinityDropWidget}""")
+                [+]             selected_widget: {self.dataPassed},
+                [+]             ID_widget: {numWidget},
+                [+]             UID: {self.infinityDropWidget[0].uid}
+                [+]             ID tooltip: {self.infinityDropWidget[0].tooltip}
+                [+]  Content: {self.infinityDropWidget}""")
           print('============')
 
           self.drag_boxs =ft.DragTarget(
                                              group     = "GroupDragg",
                                              content   = self.infinityDropWidget[0],
 
                                         on_will_accept = self.drag_will_accept,           # Traslate Drop
@@ -295,15 +295,14 @@
 
           WE PASS TO Build_Editor => self.infinityDropWidget[0] THAT IS CLICKED SELECTION
           Build_Editor.update_widget_attributes(widget_cliked=ft.Container(content=ft.Text()))
 
           """
           global numClick
 
-
           CHECK_DATA = GLOBAL_VAR(get_global_var='BOOL_SHOW_SELECTED')
 
           click_time      = time.time()
           last_click_time = GLOBAL_VAR(get_global_var='CHECK_CURRENT_TIME_DOBLE_CLICKS')  #< == DEFAULD 0
 
 
           #: CHECK IF SCAPE DOBLE CLICKS PEASE DON'T EDIT THIS LINE IF NO HAVE SOLUTION IMPLEMENTED
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/drag_container/widget_drag_editor.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/drag_container/widget_drag_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
+import flet as ft
 
 from .dragg_widget import DraggWidget
-
 from ..settings_var.settings_widget import GLOBAL_VAR
 
-import flet as ft
-
-
 class Build_Drag_Editor(ft.Stack):
      """
     Center Box that contain the phone to add Widget
 
     Note:
         How build Dragging Widget.
 
@@ -53,18 +50,16 @@
                                        ],),),
               ],
 
      """
 
      def __init__(self,data='Erase this test'):
           super().__init__()
-
           self.title=data
 
-
      def build(self):
 
           #: CONTROLS
 
           #: VIEW_COLUMN_ROUNDED
           #: TABLE_ROWS_ROUNDED
           #: WIDGETS_ROUNDED
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/icon_browser/icon_browser.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/icon_browser/icon_browser.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/footer_bar_menu_phone.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_down_phone/footer_bar_menu_phone.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_down_phone/selected_widget.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_down_phone/selected_widget.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/lite_menu_bar_right_phone/right_bar_menu_phone.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/lite_menu_bar_right_phone/right_bar_menu_phone.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 from ..tree_view.tree_view import TreeView
 import flet as ft
 
 class LiteMenuUpContainer(ft.Stack):
 
      def __init__(self,main_page= None , phone_widget_container= None,menu_left_container= None , menu_right_container= None, space_widget = None):
           super().__init__()
-          self.main_page              = main_page
+          # self.main_page              = main_page
+          # self.menu_left_container    = menu_left_container
+          # self.phone_widget_container = phone_widget_container
+          # self.menu_right_container   = menu_right_container
+
+          self.main_page              = GLOBAL_VAR(get_global_var='PAGE')
           self.menu_left_container    = menu_left_container
-          self.phone_widget_container = phone_widget_container
-          self.menu_right_container   = menu_right_container
+
+          #: SET IN MAIN_SCREEN WIDGET TO EDIT STREAMING
+          self.widget_to_edit         = GLOBAL_VAR(get_global_var='main_screen')
+
+          self.phone_widget_container = self.widget_to_edit
+          self.menu_right_container   = self.widget_to_edit.build()
 
           # HEIGHT
           self.height                 = 500
 
           self.space_widget_1 , self.space_widget_2 = space_widget
 
           #: only in production
@@ -71,15 +80,14 @@
                                                     ],
                                                   ),
                             )#<=== NOTE COMA
 
           return self.Drop_LiteMenuUpContainer
 
      def modify_widget_in_phone_container(self):
-          print('Im modificating....')
 
           """
           GLOBAL VARS:
                          CONFIG_TABS_CONTAINERS
                          CONFIG_TABS_CONTAINERS_CONTENT
 
           NOTE:
@@ -104,23 +112,24 @@
           CONFIG_TABS_CONTAINERS_CONTENT        = GLOBAL_VAR(get_global_var='CONFIG_TABS_CONTAINERS_CONTENT')
 
           SELECT_DROPP_WIDGET_CONTAINER         = GLOBAL_VAR(get_global_var='SELECT_DROPP_WIDGET_CONTAINER')
           SELECT_DROPP_WIDGET_CONTAINER_CONTENT = GLOBAL_VAR(get_global_var='SELECT_DROPP_WIDGET_CONTAINER_CONTENT')
 
           #: 'Position','Modification','Color','Image',
           control_tab_2 = CONFIG_TABS_CONTAINERS.content.controls
-
           control_tab_3 = CONFIG_TABS_CONTAINERS_CONTENT.content.controls
 
+          print(F'Im modificating....{CONFIG_TABS_CONTAINERS}')
+
           def insert_data_in_box_container(column_tab):
                """
                THIS METOD WALK IN TABS number #2 EACH COLUMN WITH WIDGETS INSIDE 4 COLUMNS
 
                """
-
+               print('tab {control_tab_2}')
                #: TAB 2
 
                if column_tab == '2_0':
                     control_2_inside = control_tab_2[0]  #
                     tmp_value = control_2_inside.controls[0].content.controls[1].content.controls
 
                if column_tab == '2_1':
@@ -310,21 +319,39 @@
                    # print(page_control,get_control_id,'simple erase')
 
                    page_control.controls.pop()                                                      #: <===== ERASE CONTROL WIDGET
                    touch_widget_in_phone = GLOBAL_VAR(set_global_var={'LIST_SELECTED_WIDGETS':None})#: <===== RESET SELECTED WIDGET TO NONE
                    del main_page._index[get_control_id]                                             #: <===== DELETE INDEX IN MAIN PAGE
                    page_control.update()                                                            #: <===== UPDATE PAGE
 
+                   # self.current_screen = GLOBAL_VAR(get_global_var='SELECTED_SCREEN').uid
+                   # self.edit_dict = GLOBAL_VAR(get_global_var='ALL_SCREEN_IN_DICT').get(self.current_screen)
+                   # print(self.edit_dict,'ALLLL <<<<<<<<<')
+
           if action == 'clear':
                #: ERASE ALL WIDGETS FROM CRONTROLS
-               main_phone = GLOBAL_VAR(get_global_var='PHONE_CONTAINER')
+               main_phone     = GLOBAL_VAR(get_global_var='SELECTED_SCREEN')
+               self.edit_dict = GLOBAL_VAR(get_global_var='ALL_SCREEN_IN_DICT')
+               # xxxdict = GLOBAL_VAR(get_global_var='EXPORT_DATA_PHONE')
+
+               print(self.edit_dict)
+               print(main_phone.uid,'selected')
+               # print(xxxdict)
+
                GLOBAL_VAR(set_global_var={'EXPORT_DATA_PHONE':dict()})                              #: <=====
-               main_phone.content.controls.clear()
+               main_phone.content.content.content.content.controls.clear()
                main_phone.update()                                                                  #: <===== UPDATE PAGE
 
+               if self.edit_dict:
+                    #: RESET ALL_SCREEN_IN_DICT DICT
+                    self.current_screen = GLOBAL_VAR(get_global_var='SELECTED_SCREEN').uid
+                    GLOBAL_VAR(set_global_var={'ALL_SCREEN_IN_DICT':{self.current_screen: dict()}})
+
+                    # print(self.edit_dict)
+
           if action == 'TREE':
                TreeView.visible_view()
 
 
           if action == 'rotation':
                self.phone_widget_container.controls[0].width , self.phone_widget_container.controls[0].height = self.phone_widget_container.controls[0].height , self.phone_widget_container.controls[0].width
                self.phone_widget_container.controls[0].update()
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/screen_manager.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/screen_manager/screen_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,65 +8,173 @@
 #: VERY IMPORTANT IT'S MAIN PHONE THAT WILL CONTENT ALL SCREENS
 from extra_utils.phone_container.widget_phone_editor import Build_Phone_Editor
 
 all_screens_in_app: dict = {
 
                             }
 
+
+# tmp_screen = Build_Phone_Editor(color_data='Blue')
+
+# row_box_content_phone = GLOBAL_VAR(get_global_var='row_phone')
+# tmp_new_phone = Build_Phone_Editor(color_data=ft.colors.TRANSPARENT).build()        #: ADD SCREEN PHONE IN DICT all_screens_in_app
+# row_box_content_phone.controls.append(tmp_new_phone)                    #: ADD PHONE inside row_box_content_phone
+# GLOBAL_VAR(set_global_var= {'main_screen':row_box_content_phone.controls[0]})
+
+# print(row_box_content_phone)
+
+
 def screen_manager(
                    add_screen:    str = "",
                    delete_screen: str = "" ,
-                   update_screen: str = "" ,
+                   selected_screen: str = "" ,
                    load_screen:   str = "",
-                   clear_screen: bool = False,
                    set_screen:    str = "",
                    get_screen:    str = "",
-
+                   clear_screen: bool = False,
                    ):
+
+    #: THIS METOD WILL MANAGE ALL SCREENS INSIDE LET'US MODIFY EXACLTY SELECTED SCREEN
     global all_screens_in_app
     if add_screen:
-        #: ADD SCREEN PHONE IN DICT SCREENS
-        all_screens_in_app[add_screen] = Build_Phone_Editor(color_data='Blue')
-        GLOBAL_VAR(set_global_var={add_screen:Build_Phone_Editor(color_data='Blue')})
+        """
+        add_screen var is sleceted widget name in screen manager buton on menu fotter bar
+
+        1. take name snew screen
+        2. add new screen inside row_box_content_phone
+        3. row_box_content_phone update
+        3. add to global var dict
+        """
+        tmp_new_screen_name   = add_screen                                      #: take only name of new screen
+        row_box_content_phone = GLOBAL_VAR(get_global_var='row_phone')
+
+        # ============================== SCREEN PHONE IN DICT ====================================
+        #: ADD SCREEN PHONE IN DICT all_screens_in_app
+        tree_view_new_phone = Build_Phone_Editor(
+                                                 color_data     = ft.colors.TRANSPARENT,
+                                                 )
+
+        tmp_new_phone = tree_view_new_phone.build()          #: ADD SCREEN PHONE IN DICT all_screens_in_app
+        row_box_content_phone.controls.append(tmp_new_phone) #: ADD PHONE inside row_box_content_phone
+        row_box_content_phone.update()
+        # ========================================================================================
+
+        #: ADD SCREEN PHONE IN DICT DATA_GLOBAL
+        #: PATH extra_utils/settings_var/settings_widget.py
+        #: WIDGET AFTER PASS TO ROW GET ID
+        GLOBAL_VAR( set_global_var= {tmp_new_screen_name:tmp_new_phone})
+
+
+        #: HIDE NEW SCREEN CONTAINER BOX
+        tmp_new_phone.visible = False
+        tmp_new_phone.update()
+
+        #: HIDE SCREEN MANAGER CONTAINER BOX
+        show_screen_manager = GLOBAL_VAR(get_global_var='SCREEN_CONTAINER')
+        show_screen_manager.visible = False
+        show_screen_manager.update()
+
+        # ========================================================================================
+        #: CREATE NEW SCREEN IN ALL SCREENS DICT VERY IMPORTATN CONTAIN ALL SCREENS IN
+        current_screen_id = GLOBAL_VAR(get_global_var='SELECTED_SCREEN').uid
+        GLOBAL_VAR(set_global_var = {'ALL_SCREEN_IN_DICT':{current_screen_id: dict() }})
+        # ========================================================================================
 
     elif delete_screen:
         #: DELETE SCREEN PHONE IN DICT SCREENS
         del all_screens_in_app[delete_screen]
 
-    elif update_screen:
-        #: UPDATE SCREEN PHONE IN DICT SCREENS
-        # GLOBAL_VAR(set_global_var={'main_screen':all_screens_in_app.get(update_screen)})
-
-        # data = GLOBAL_VAR(get_global_var='phone_testing')
-        # data.controls[0].bgcolor = 'Blue'
-        # data.update()
-        # print(data.controls[0])
-        # print(GLOBAL_VAR(get_global_var='phone_testing'))
-
-        row_phone = GLOBAL_VAR(get_global_var='row_phone')
-
-        # current_screen = all_screens_in_app.get(update_screen)
-        current_screen = GLOBAL_VAR(get_global_var=update_screen)
-
-        row_phone.controls[2]= current_screen
-        row_phone.update()
-
-        print(current_screen.controls[0].content.content.content.content.controls)
-
-        GLOBAL_VAR(set_global_var={'row_phone':row_phone})
-
-        # print(all_screens_in_app.get(update_screen))
+    elif selected_screen:
+        #: ROW_PHONE IT'S MAIN ROW THAT HAVE PHONE WIDGET INSIDE WILL BE HOT RELOAD EVERY TIME WE CALL
+        #: THAT'S WHY I WILL PAS TO A GLOVAL VAR NAME "SCREEN_CONTAINER"
+
+        #: ROW_PHONE IT'S MAIN ROW THAT HAVE PHONE WIDGET INSIDE WILL BE HOT RELOAD EVERY TIME WE CALL
+        #: THAT'S WHY I WILL PAS TO A G
+        # GLOVAL VAR NAME "SCREEN_CONTAINER"
+
+        row_box_content_phone = GLOBAL_VAR(get_global_var='row_phone')
+        tmp_new_screen_name = selected_screen
+
+
+
+
+        #: HIDE OLD SCREEN CONTAINER BOX
+        old_selected_screen = GLOBAL_VAR(get_global_var='SELECTED_SCREEN')
+        new_selected_screen = GLOBAL_VAR(get_global_var=tmp_new_screen_name)
+
+        #: SWITCH VISIBLE ON OFF BETEWNS SCREENS
+        old_selected_screen.visible, new_selected_screen.visible = new_selected_screen.visible ,old_selected_screen.visible
+        # old_selected_screen.visible = True
+        # new_selected_screen.visible = True
+
+        tab_one_confic_container = GLOBAL_VAR(get_global_var='CONFIG_TABS_PHONE')
+        tab_one = tab_one_confic_container.content.controls
+        #: TAB 0 NAME COLOR PHONE
+        color_phone           = tab_one[0]
+        color_phone_controls  = color_phone.controls[0].content.controls[1].content
+        #: TAB 0 NAME IMAGE PHONE
+        image_phone           = tab_one[1]
+        image_phone_controls  = image_phone.controls[0].content.controls[1].content
+        #: TAB 0 NAME COLUMN PHONE
+        column_phone          = tab_one[2]
+        column_phone_controls = column_phone.controls[0].content.controls[1].content
+
+        def update_widget_config_container(widget_update,widget_to_edit):
+            """WIL UPDATE WIDGET TO CONFIG STRAMING IN SCREEN MANAGER BOX"""
+
+            for _ in widget_update:
+
+                if _.id_name_widget_dict == "main_phone":
+                    _.widget = widget_to_edit
+
+                if _.id_name_widget_dict == "main_phone_conainer":
+                    _.widget = widget_to_edit.content.content.content
+
+                if _.id_name_widget_dict == "main_phone_conainer_conent":
+                    _.widget = widget_to_edit.content.content.content.content
+
+
+        update_widget_config_container(
+                                       widget_update  = color_phone_controls.controls,
+                                       widget_to_edit = new_selected_screen
+                                       )
+
+        update_widget_config_container(
+                                       widget_update  = image_phone_controls.controls,
+                                       widget_to_edit = new_selected_screen
+                                       )
+        update_widget_config_container(
+                                       widget_update  = column_phone_controls.controls,
+                                       widget_to_edit = new_selected_screen
+                                       )
+        old_selected_screen.update()
+        new_selected_screen.update()
+        row_box_content_phone.update()
+
+        GLOBAL_VAR(set_global_var={'SELECTED_SCREEN':new_selected_screen})
+        # GLOBAL_VAR(set_global_var={'EXPORT_DATA_PHONE':new_selected_screen})
+
+        # print(new_selected_screen._get_children())
+
+        # GLOBAL_VAR(set_global_var={'EXPORT_DATA_PHONE':{'INAMGE':new_selected_screen}})
+        # ========================================================================================
+        #: CREATE NEW SCREEN IN ALL SCREENS DICT VERY IMPORTATN CONTAIN ALL SCREENS IN
+        current_screen_id = GLOBAL_VAR(get_global_var='SELECTED_SCREEN').uid
+        get_curent_id = GLOBAL_VAR(get_global_var='ALL_SCREEN_IN_DICT').get(current_screen_id)
+        # ========================================================================================
 
     elif clear_screen:
         #: CLEAR ALL SCREENS PHONES IN DICT SCREENS
+
         tmp_main_screen = all_screens_in_app.pop("main_screen")
         all_screens_in_app = {"main_screen":tmp_main_screen}
 
+
     elif set_screen:
-        all_screens_in_app["main_screen"]=set_screen
+        all_screens_in_app["main_screen"]= GLOBAL_VAR(get_global_var="main_screen")
 
     elif get_screen:
         return all_screens_in_app.get(get_screen)
 
     # print(all_screens_in_app)
 
 CURRENT_PATH: str = os.path.join('./flet_box/extra_utils/screen_manager','screens.js')
@@ -86,14 +194,17 @@
         self.blur          = (12,12)
         # self.on_click    = lambda _:self.escape_data_in_sqlite()
         self.right  = 0
         self.left   = 0
         self.top    = 0
         self.bottom = 0
 
+
+
+
     def build(self):
 
         self.content = ft.Container(
                     ink       = False,
                     padding   = ft.padding.all(16),
                     margin    = ft.margin.all(8),
                     alignment = ft.alignment.center,
@@ -297,28 +408,28 @@
         #: ADD AND CLEAN BUTTON SCREEN
         if self.container_editor:
             self.content  = ft.Container(
                                 alignment = ft.alignment.center,
                                 padding   = ft.padding.all(8),
                                 content   = ft.Column(
                                         # scroll="HIDDEN",
-                                        alignment= ft.MainAxisAlignment.SPACE_BETWEEN,
-                                        horizontal_alignment=ft.CrossAxisAlignment.CENTER,
+                                        alignment            = ft.MainAxisAlignment.SPACE_BETWEEN,
+                                        horizontal_alignment = ft.CrossAxisAlignment.CENTER,
                                         controls= [
                                                     ft.Container(height=24),
                                                     ft.Icon(
                                                             name=ft.icons.ADD,
                                                             color=ft.colors.BLUE_900,
 
                                                             ),
 
                                                     ft.ElevatedButton(
                                                                     text='CLEAN',
                                                                     bgcolor=ft.colors.RED_900,
-                                                                    on_click=lambda _:self.remove_all(),
+                                                                    on_click=lambda _:self.remove_all(id_name= self.id_name),
                                                                     ),
                                                     ],
                                         ),
                                 )
             self.on_click = lambda _:self.show_screen_name()
 
         else:
@@ -402,27 +513,33 @@
 
         screen_name: str = self.screen_selected.content.controls[1].content.value
 
         change_text_screen = GLOBAL_VAR(get_global_var='change_text_screen')
         change_text_screen.value = screen_name
         change_text_screen.update()
 
-        #:===================================================
-        #: UPDATE SELECTED WIDGET DICT
-        print(f"UPDATE Widget {screen_name} <====")
-        screen_manager(update_screen=screen_name)
+        # #:===================================================
+        # #: UPDATE SELECTED WIDGET DICT
+        # print(f"UPDATE Widget {screen_name} <====")
+        # print(screen_name,'<<< this is <<<<<<<<<<<<<<<<<<')
+        # screen_now = GLOBAL_VAR(get_global_var=screen_name)
+        screen_manager(selected_screen=screen_name)
+        # screen_manager(selected_screen=screen_now)
+
+        # print(screen_name)
         #:===================================================
 
+        # print(screen_now,'<<< this is <<<<<<<<<<<<<<<<<<')
 
     def show_screen_name(self):
         # ONLY FUNCTIONALITY IS SHOW BOX INPUT DIALOG
         name_screen.visible = True
         name_screen.update()
 
-    def remove_all(self):
+    def remove_all(self,id_name):
         with open(CURRENT_PATH,'w') as f:
             f.write('{}')
 
         # SCREEN_GLOBAL_VAR(empty_list=True)
         data = SCREEN_GLOBAL_VAR(get_global_var='javier').get('GridView')
         data_ = data.controls
         data.controls = data_[:2]
@@ -433,14 +550,15 @@
         SCREEN_GLOBAL_VAR(set_global_var = {'widget_selected':defauld_color})
         defauld_color.bgcolor     = ft.colors.RED_900
         defauld_color.update()
 
         #:===================================================
         #: REMOVE ALL REAL SCREEN TO DICT WITH ALL REAL SCREENS
         screen_manager(clear_screen=True)
+        # print(id_name,'idname')
         #:===================================================
 
 
     def delete_id_name(self,id_name):
         # GET INDEX NUMBER FROM LIST TO DELETE IN CONTROLS
         my_list = SCREEN_GLOBAL_VAR(get_index_list=id_name)
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/settings_screens.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/screen_manager/settings_screens.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/screen_manager/write_file_proyect.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/screen_manager/write_file_proyect.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/save_export.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/settings_var/save_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     container_string_node = ''
     contents__string_node = ''
     tmp_controls_all_node = []
 
     def __init__(self,):
         super().__init__()
 
+        # data = GLOBAL_VAR(get_global_var='EXPORT_DATA_PHONE')
         self.show_tree_nodews(widget_show=GLOBAL_VAR(get_global_var='EXPORT_DATA_PHONE'))
+        # print(data)
 
     def show_tree_nodews(self,widget_show):
         """
         BUILDER TREE WITH ALL WIDGET INSIDE CALLING ONE BY ONE
         TO MAKE A TREE WITH ALL WIDGETS OREDERER
 
 
@@ -26,14 +28,15 @@
         contents__string_node = ''                  #: CONTENT OF MAIN CONTAINER
         tmp_controls_all_node = []                  #: LIST WITH ALL WIDGET TO SHOW IN TREVIEW
 
         self.data = '\n'.join(self.all_data_list)   #: WILL TRANSFOR FROM LIST TO STRING
 
         """
         self.all_widgets = widget_show
+        print(self.all_widgets,'hello')
 
         list_controls  = ['row','column','stack','gridview']
 
         #: self.container_string_node = self.main_node
         #: self.contents__string_node = self.container_string_node.content
         #: self.all_data_list.append(f"0 ⫺ {self.container_string_node._get_control_name()}")
         #: self.all_data_list.append(f"0 ⫺ {self.contents__string_node._get_control_name()}")
@@ -397,18 +400,19 @@
         check_second_4 = True
         check_second_5 = True
         check_second_6 = True
         check_second_7 = True
         check_second_8 = True
 
         #: testing data
-        PHONE_MAIN      = GLOBAL_VAR(get_global_var='PHONE_MAIN')
-        PHONE_CONTAINER = GLOBAL_VAR(get_global_var='PHONE_CONTAINER')
-        PHONE_COLUMN    = PHONE_CONTAINER.content
+        # PHONE_MAIN      = GLOBAL_VAR(get_global_var='PHONE_MAIN')
+        # PHONE_CONTAINER = GLOBAL_VAR(get_global_var='PHONE_CONTAINER')
+        # PHONE_COLUMN    = PHONE_CONTAINER.content
 
+        # print(PHONE_MAIN)
         # #: THIS CODE IS ONE EXTRACT OF PHONE NECCESARY TO HAVE PHONE ATTRIBUES BY DEFAULD
         # tmp_data_1 = dict()                                       #: TMP DICT()
         # tmp_data_2 = dict()                                       #: TMP DICT()
         # tmp_data_3 = dict()                                       #: TMP DICT()
 
         # tmp_data_1.update({'WIDGET_NAME':'PHONE_BOX'})
         # PHONE_MAIN.copy_attrs(dest=tmp_data_1)                    #: NEW COPY ATTRIBUTES
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/settings_var/settings_widget.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/settings_var/settings_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,15 @@
          'SHOW_TEXT_SELECTED_PHONE_WIDGET': 'None', # <== LITE CONTAINER THAT SHOW SELECTED PHONE WIDGET TO CONFIG
          'SHOW_TEXT_SELECTED_DRAGG_WIDGET': 'None', # <== LITE CONTAINER THAT SHOW SELECTED DRAGG WIDGET TO CONFIG
 
                       'CONFIG_TABS_PHONE' : None,   # <== CONFIGURATION PHONE     BOX THAT CONTAIN ALL WIDGET TO MODIFY PROPERTY
                  'CONFIG_TABS_CONTAINERS' : None,   # <== CONFIGURATION CONTAINER BOX THAT CONTAIN ALL WIDGET TO MODIFY PROPERTY
          'CONFIG_TABS_CONTAINERS_CONTENT' : None,   # <== CONFIGURATION CONTENT   BOX THAT CONTAIN ALL WIDGET TO MODIFY PROPERTY
 
-
-                             'PHONE_MAIN' : None,   # <== PHONE MAIN CONTAINER ONLY APPLY IMAGEN
-                        'PHONE_CONTAINER' : None,   # <== PHONE MAIN CONTENT CONTAINER TO APPLY BLUR COLOR
-                'PHONE_CONTAINER_CONTENT' : None,   # <== PHONE CONTENT
+                        'SELECTED_SCREEN' : None,   # <== SELECTED PHONE SCREEN
 
           'SELECT_DROPP_WIDGET_CONTAINER' : None,   # <== SELECTED WIDGET IN PHONE
   'SELECT_DROPP_WIDGET_CONTAINER_CONTENT' : None,   # <== SELECTED WIDGET IN PHONE CONTENT
 
                  'ICON_BROWSER_CONTAINER' : None,   # <== BOX CONTAINER WITH SEARCH ICON
                 'COLOR_BROWSER_CONTAINER' : None,   # <== BOX CONTAINER WITH SEARCH COLORS
                   'GPT_BROWSER_CONTAINER' : None,   # <== BOX CONTAINER WITH SEARCH GPT
```

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/color_hight_light_editor.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/tree_view/color_hight_light_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/extra_utils/tree_view/tree_view_text_editor.py` & `flet-box-gui-0.1.2.2/flet_box/extra_utils/tree_view/tree_view_text_editor.py`

 * *Files identical despite different names*

### Comparing `flet-box-gui-0.1.2.1/flet_box/flet_box.py` & `flet-box-gui-0.1.2.2/flet_box/flet_box.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,22 +53,30 @@
 
      #: GLOBAL_VAR PAGE
      GLOBAL_VAR(set_global_var={'PAGE':page})
      #: GLOBAL_VAR PAGE
 
      drag_container_to_phone = Build_Drag_Editor()
 
-     phone_testing           = Build_Phone_Editor(color_data="Red")
-     screen_manager(set_screen=phone_testing)
-     GLOBAL_VAR(set_global_var={'main_screen':phone_testing})
+     #: PHONE BOX CONTAINER TO GLOBAL VAR WITH NAME "main_screen"
+     # phone_testing           = Build_Phone_Editor(color_data="Red")
+     phone_testing           = Build_Phone_Editor(color_data=ft.colors.TRANSPARENT).build()
+     # phone_testing           = Build_Phone_Editor(color_data=ft.colors.TRANSPARENT).build()
 
-     right_config_container  = Build_Editor(widget=screen_manager(get_screen='main_screen').build())
-     # right_config_container  = Build_Editor(widget=phone_testing.build())
-     space_widget_1 = ft.Container( expand = True)
-     space_widget_2 = ft.Container( expand = True)
+     # print(phone_testing.build().content)
+
+     GLOBAL_VAR(set_global_var= {'main_screen':phone_testing})
+     GLOBAL_VAR(set_global_var= {'SELECTED_SCREEN':phone_testing})
+
+
+     screen_manager(set_screen= True)
+
+     #: ITS VERY IMPORTANT GET WIDGET INSIDE BECOUSE WILL MODIFY MAIN PHONE BOX CONTAINER
+     right_config_container  = Build_Editor()
+     GLOBAL_VAR(set_global_var= {'build_Editor':right_config_container})
 
      #: ICON BROWSER
      Icon_Browser = IconBrowser(blur_effect=True)
      IconBrowserContainer = ft.Container(
                visible= False,
                right  = 240,
                left   = 240,
@@ -141,122 +149,138 @@
           content=ft.Column(
                     controls = [
                                  right_config_container,
                                    ],
                               ),
                           )
 
+
      #: SCREEN MANAGER
      Screen_Manager = ScreenManager()
 
      ScreenContainer = ft.Container(
-               visible= False,
-               right  = 8,
-               left   = 8,
-               top    = 8,
-               bottom = 8,
-          content=Screen_Manager,
-          )
+                              visible= False,
+                              right  = 8,
+                              left   = 8,
+                              top    = 8,
+                              bottom = 8,
+                         content=Screen_Manager,
+                         )
+
      GLOBAL_VAR(set_global_var={'SCREEN_CONTAINER':ScreenContainer})
 
+     #: THIS SPACE WILL SHOW DEPENDING SIZE OF THE PHONE OR SCREEN
+     space_widget_1 = ft.Container( expand = True)
+     space_widget_2 = ft.Container( expand = True)
+
+     #: ROW_PHONE IT'S MAIN ROW THAT HAVE PHONE WIDGET INSIDE WILL BE HOT RELOAD EVERY TIME WE CALL
+     #: THAT'S WHY I WILL PAS TO A GLOVAL VAR NAME "SCREEN_CONTAINER"
+
+
+
      row_phone = ft.Row(
-                  spacing     = 0,
-                  run_spacing = 0,
-                 controls = [
-                            space_widget_1,
-                            TreeView(),
-                            screen_manager(get_screen='main_screen'),
-                            space_widget_1,
-                            LiteMenuUpContainer(
-                                     menu_left_container    = drag_container_to_phone,
-                                     phone_widget_container = screen_manager(get_screen='main_screen'),
-                                     menu_right_container   = screen_manager(get_screen='main_screen').build(),
-                                     main_page              = page,
-                                     space_widget           = [space_widget_1,space_widget_2],
-                                     ),
-                           ],)
+                        scroll=True,
+               controls= [
+                    # screen_manager(get_screen='main_screen')
+                    phone_testing,
+                    ],
+                  )
+     container_phone = ft.Container(
+                                    # bgcolor="red",
+                                    width=295,
+                                    # width=560,
+                                    # height=620,
+                                    alignment = ft.alignment.center,
+                         content=row_phone
+                                    )
+     #: WE SET AS GLOBAL VAR
      GLOBAL_VAR(set_global_var={"row_phone":row_phone})
+
      screen_1 = ft.Container(
                     ink             = False,
                     bgcolor         = ft.colors.BLACK54,
                     padding         = ft.padding.only(left=0, top=0, right=0, bottom=0),
                     margin          = ft.margin.all(0),    #outside box
                     alignment       = ft.alignment.center,
                     border          = ft.border.all(6, ft.colors.BLACK12),
                     height          = 768,
                content=ft.Row(
                          controls=[
                               MenuLeftContainer(),
                               ft.Container(
-                                      expand    = True,
-                                      ink       = False,
-                                      padding   = ft.padding.only(left=0, top=4, right=0, bottom=4),
-                                      margin    = ft.margin.all(0),
-                                      alignment = ft.alignment.center,
-                                  content=ft.Column(
+                                        expand    = True,
+                                        ink       = False,
+                                        padding   = ft.padding.only(left=0, top=4, right=0, bottom=4),
+                                        margin    = ft.margin.all(0),
+                                        alignment = ft.alignment.center,
+                                   content=ft.Column(
                                                   expand = True,
                                               controls=[
 
                                                      MenuUpContainer(main_page = page),
 
                                                      ft.Container( #: CENTER MAIN CONTAINER THAT HAVE ['LEFT DRAG', 'MIDDLE PHONE' ,'RIGHT CONFIG']
-                                                                 ink       = False,
-                                                                 padding   = ft.padding.all(0),
-                                                                 margin    = ft.margin.all(0),    #outside box
-                                                                 alignment = ft.alignment.center,
-                                                                 height    = 680,
+                                                            ink       = False,
+                                                            padding   = ft.padding.all(0),
+                                                            margin    = ft.margin.all(0),    #outside box
+                                                            alignment = ft.alignment.center,
+                                                            height    = 680,
                                                          content = ft.Row(
                                                                      controls=[
                                                                        drag_container_to_phone,
                                                                        ft.Container( #: MIDDLE CONTAINER
-                                                                                   expand    = True,
-                                                                                   ink       = False,
-                                                                                   padding   = ft.padding.all(0),
-                                                                                   margin    = ft.margin.all(0),
-                                                                                   alignment = ft.alignment.center,
-                                                                                   height    = 675,
+                                                                                expand    = True,
+                                                                                ink       = False,
+                                                                                padding   = ft.padding.all(0),
+                                                                                margin    = ft.margin.all(0),
+                                                                                alignment = ft.alignment.center,
+                                                                                height    = 675,
                                                                            content=ft.Column(
-                                                                                           horizontal_alignment   = ft.CrossAxisAlignment.CENTER,
-                                                                                           spacing              = 2,
-                                                                                           run_spacing          = 2,
-                                                                                       controls=[
-                                                                                         ft.Container(
-                                                                                                    padding = ft.padding.all(0),
-                                                                                                    margin  = ft.margin.all(0),
-                                                                                                    height  = 620,
-                                                                                              # content = ft.Row(
-                                                                                              #                 spacing     = 0,
-                                                                                              #                 run_spacing = 0,
-                                                                                              #                controls = [
-                                                                                              #                           space_widget_1,
-                                                                                              #                           TreeView(),
-                                                                                              #                           screen_manager(get_screen='main_screen'),
-                                                                                              #                           space_widget_1,
-                                                                                              #                           LiteMenuUpContainer(
-                                                                                              #                                    menu_left_container    = drag_container_to_phone,
-                                                                                              #                                    phone_widget_container = screen_manager(get_screen='main_screen'),
-                                                                                              #                                    menu_right_container   = screen_manager(get_screen='main_screen').build(),
-                                                                                              #                                    main_page              = page,
-                                                                                              #                                    space_widget           = [space_widget_1,space_widget_2],
-                                                                                              #                                    ),
-                                                                                              #                          ],),
-                                                                                                    content=row_phone,
-                                                                                                             ),
-                                                                                         LiteMenuDownContainer(),
+                                                                                          horizontal_alignment   = ft.CrossAxisAlignment.CENTER,
+                                                                                          spacing              = 2,
+                                                                                          run_spacing          = 2,
+                                                                                     controls=[
+                                                                                          ft.Container(
+                                                                                               padding = ft.padding.all(0),
+                                                                                               margin  = ft.margin.all(0),
+                                                                                               height  = 620,
+                                                                                               # width=400,
+                                                                                               # bgcolor='Red',
+                                                                                               #: IT'S A ROW THAT HAVE THE MAIN PHONE INSIDE
+                                                                                               content = ft.Row(
+                                                                                                              spacing     = 0,
+                                                                                                              run_spacing = 0,
+                                                                                                              controls = [
+                                                                                                              space_widget_1,
+                                                                                                              TreeView(),
+                                                                                                              #: CALL WIDGET SCREEN IN DICT INSIDE screen_manager
+                                                                                                              container_phone,
+
+                                                                                                              space_widget_1,
+                                                                                                              LiteMenuUpContainer(
+                                                                                                                   menu_left_container    = drag_container_to_phone,
+                                                                                                                   # phone_widget_container = screen_manager(get_screen='main_screen'),
+                                                                                                                   # menu_right_container   = screen_manager(get_screen='main_screen').build(),
+                                                                                                                   # main_page              = page,
+                                                                                                                   space_widget           = [space_widget_1,space_widget_2],
+                                                                                                                   ),
+                                                                                                              ],),
+                                                                                                        ),
+                                                                                          LiteMenuDownContainer(),
                                                                                                 ],
-                                                                                   ),
-                                                                                 ),
+                                                                                     ),
+                                                                                ),
                                                                                 right_config_container,
                                                                               ],),
-                                                          ),
+                                                            ),
                                                       AlertSelected(),
                                                        ],
                                               ),
-                                  ),
-                           ],),
+                                   ),
+                         ],),
           )
 
      data_stack = ft.Stack(
                     controls = [
                                    screen_1,
                                    IconBrowserContainer,
                                    ColorBrowserContainer,
@@ -270,16 +294,19 @@
      #: only use in production
      # print(page.views)
 
 
      page.add(data_stack)
 
      # AFTER ADD TAKE ID
-     GLOBAL_VAR(set_global_var={'phone_testing':phone_testing})
-     print(phone_testing.uid,'<<<<<')
+     # GLOBAL_VAR(set_global_var={'phone_testing':phone_testing})
+     # print(phone_testing.uid,'<<<<<')
+     GLOBAL_VAR(set_global_var= {'ALL_SCREEN_IN_DICT':{phone_testing.uid:dict()}})
+     # print(GLOBAL_VAR(get_global_var='ALL_SCREEN_IN_DICT'))
+
      page.update()
 
 def run_app():
      #: ONLY FOR PYINSTALLER
      ft.app(
                target = main,
           )
```

### Comparing `flet-box-gui-0.1.2.1/flet_box_gui.egg-info/SOURCES.txt` & `flet-box-gui-0.1.2.2/flet_box_gui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 flet_box/extra_utils/menu_tab_left_phone/__init__.py
 flet_box/extra_utils/menu_tab_left_phone/widget_menu_left_editor.py
 flet_box/extra_utils/menu_tab_up_phone/__init__.py
 flet_box/extra_utils/menu_tab_up_phone/basic_menu_tab_up.py
 flet_box/extra_utils/menu_tab_up_phone/skeleton_class_screens.py
 flet_box/extra_utils/menu_tab_up_phone/widget_menu_tab_editor.py
 flet_box/extra_utils/phone_container/__init__.py
+flet_box/extra_utils/phone_container/nested_dict.py
 flet_box/extra_utils/phone_container/widget_phone_editor.py
 flet_box/extra_utils/screen_manager/__init__.py
 flet_box/extra_utils/screen_manager/screen_manager.py
 flet_box/extra_utils/screen_manager/settings_screens.py
 flet_box/extra_utils/screen_manager/write_file_proyect.py
 flet_box/extra_utils/settings_var/__init__.py
 flet_box/extra_utils/settings_var/save_export.py
```

### Comparing `flet-box-gui-0.1.2.1/setup.py` & `flet-box-gui-0.1.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+from pathlib import Path
 from setuptools import setup , find_packages
 import os
-import pypandoc
+# import pypandoc
 import sys
 
+# NECESARY TO CREATE PACKAGES
+# pip install pathlib
+# pip install pypandoc
+# pip install twine
+# pip install wheel
+
+# sudo apt-get install python3-dev
+# sudo apt-get install python3-pip
+
 #: MAKE A SETUP INSTALL
 # python3 setup.py sdist bdist_wheel
 # python3 setup.py bdist_wheel
 # python3 setup.py register -r pypi
 # python3 setup.py sdist upload -r pypi
 
-# $ python setup.py sdist
-# $ twine upload dist/* -r pypi
-# $ twine upload dist/* -r flet_box_gui
+# python setup.py sdist
+# twine upload dist/* -r pypi
+# twine upload dist/* -r flet_box_gui
 
-# $ python setup.py sdist bdist_wheel --universal
-# $ twine upload dist/* -r pypi
+# python setup.py sdist bdist_wheel --universal
+# twine upload dist/* -r pypi
 
 # pip install twine ,pypandoc
 # twine upload dist/*
+# twine check dist/*
 # PACKAGE META-DATA
 
 # python3 -m pip install --upgrade pip
 # pip install pypandoc
 # pip install pypandoc_binary
 
 # errors pip
@@ -53,24 +64,30 @@
 "console_scripts": [
 "flet_box      = flet_box:run_app",
 ],
 }
 
 PYPY_KEYWORDS_TO_FIND = ["flet-box-gui", "flet",'flet-gui','flet-builder','flet-sdk']
 
-here = os.path.abspath(os.path.dirname(__file__))
+# read the contents of your README file
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
-try:
-    long_description = pypandoc.convert_file('README.md', 'rst')
-except(IOError, ImportError):
-    long_description = open('README.md').read()
-    data = "\n\tpip install pypandoc\n\tpip install pypandoc_binary"
-    print(f'Please install {data}')
+
+
+# try:
+#     long_description = pypandoc.convert_file('README.md', 'rst')
+# except(IOError, ImportError):
+#     long_description = open('README.md').read()
+#     data = "\n\tpip install pypandoc\n\tpip install pypandoc_binary"
+#     print(f'Please install {data}')
 
 #: MANAGE VERSION
+here = os.path.abspath(os.path.dirname(__file__))
+
 try:
     with open(os.path.join(here, 'VERSION'), encoding='utf-8') as f:
         VERSION = f.read()
 
 except FileNotFoundError:
     VERSION = '0.1.0'
```

