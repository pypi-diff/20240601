# Comparing `tmp/PyQt6-Fluent-Widgets-1.5.6.tar.gz` & `tmp/PyQt6-Fluent-Widgets-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Fluent-Widgets-1.5.6.tar", last modified: Tue May  7 03:50:30 2024, max compression
+gzip compressed data, was "dist\PyQt6-Fluent-Widgets-1.5.7.tar", last modified: Sat Jun  1 03:50:00 2024, max compression
```

## Comparing `PyQt6-Fluent-Widgets-1.5.6.tar` & `PyQt6-Fluent-Widgets-1.5.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.692561 PyQt6-Fluent-Widgets-1.5.6/
--rw-rw-rw-   0        0        0    35825 2024-05-07 03:47:53.000000 PyQt6-Fluent-Widgets-1.5.6/LICENSE
--rw-rw-rw-   0        0        0     5230 2024-05-07 03:50:30.691563 PyQt6-Fluent-Widgets-1.5.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.501443 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     5230 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4919 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 03:50:30.000000 PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4454 2024-05-07 03:48:38.000000 PyQt6-Fluent-Widgets-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.502543 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/
--rw-rw-rw-   0        0        0      550 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.506112 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  6502800 2024-05-07 03:49:15.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.544397 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0    22679 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1587 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py
--rw-rw-rw-   0        0        0    11167 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      817 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    13818 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     5549 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3866 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0      658 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py
--rw-rw-rw-   0        0        0     4847 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    14425 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      452 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.546397 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.556107 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2594 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    22447 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7658 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19774 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     6439 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.568013 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    15056 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     6001 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11791 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3157 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2967 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py
--rw-rw-rw-   0        0        0     2424 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.574296 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2727 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     7110 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1262 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.586181 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/
--rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py
--rw-rw-rw-   0        0        0     3032 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py
--rw-rw-rw-   0        0        0     3580 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py
--rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py
--rw-rw-rw-   0        0        0     6314 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py
--rw-rw-rw-   0        0        0     1181 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py
--rw-rw-rw-   0        0        0     1453 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.600454 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0    10126 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py
--rw-rw-rw-   0        0        0    13248 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8745 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    24728 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    19994 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6888 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     5254 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.613788 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5354 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0    11296 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     4697 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2843 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    14288 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1544 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.675267 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     3328 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     8188 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    30220 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     7755 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     5835 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    15886 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19946 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     8072 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    13322 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py
--rw-rw-rw-   0        0        0    17277 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2318 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1552 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16747 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    19320 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0    14940 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    14414 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4750 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    40909 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0    11379 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py
--rw-rw-rw-   0        0        0     9269 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     7143 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2758 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    18352 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     1226 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py
--rw-rw-rw-   0        0        0    10206 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     8850 2024-05-07 03:48:16.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6564 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5923 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8768 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    26737 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py
--rw-rw-rw-   0        0        0    11626 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    23075 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10674 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     4671 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.682143 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/
--rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/__init__.py
--rw-rw-rw-   0        0        0    11775 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py
--rw-rw-rw-   0        0        0     3943 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py
--rw-rw-rw-   0        0        0     2947 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:50:30.689561 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    13085 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2840 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1685 2024-05-07 03:47:54.000000 PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2024-05-07 03:50:30.692861 PyQt6-Fluent-Widgets-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1205 2024-05-07 03:48:44.000000 PyQt6-Fluent-Widgets-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.857221 PyQt6-Fluent-Widgets-1.5.7/
+-rw-rw-rw-   0        0        0    35825 2024-06-01 03:41:39.000000 PyQt6-Fluent-Widgets-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0     5230 2024-06-01 03:50:00.854221 PyQt6-Fluent-Widgets-1.5.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.523265 PyQt6-Fluent-Widgets-1.5.7/PyQt6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5230 2024-06-01 03:50:00.000000 PyQt6-Fluent-Widgets-1.5.7/PyQt6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4919 2024-06-01 03:50:00.000000 PyQt6-Fluent-Widgets-1.5.7/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 03:50:00.000000 PyQt6-Fluent-Widgets-1.5.7/PyQt6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 03:50:00.000000 PyQt6-Fluent-Widgets-1.5.7/PyQt6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 03:50:00.000000 PyQt6-Fluent-Widgets-1.5.7/PyQt6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4454 2024-06-01 03:41:39.000000 PyQt6-Fluent-Widgets-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.524509 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/
+-rw-rw-rw-   0        0        0      550 2024-06-01 03:41:51.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.528573 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  3307458 2024-06-01 03:44:47.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.562799 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0    22679 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1587 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/color.py
+-rw-rw-rw-   0        0        0    11172 2024-06-01 03:41:51.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      817 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    13818 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     5549 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3866 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0      658 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/screen.py
+-rw-rw-rw-   0        0        0     4847 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    14430 2024-06-01 03:41:51.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      452 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.565001 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.576654 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2594 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    22447 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7658 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19774 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     6439 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.591804 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    15056 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     6001 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11791 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3266 2024-06-01 03:43:46.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2967 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_box_base.py
+-rw-rw-rw-   0        0        0     2424 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.604501 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2727 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     7535 2024-06-01 03:43:34.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1262 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.631222 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/
+-rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/__init__.py
+-rw-rw-rw-   0        0        0     3032 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_combo_box.py
+-rw-rw-rw-   0        0        0     3580 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_flyout.py
+-rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_line_edit.py
+-rw-rw-rw-   0        0        0     6314 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_menu.py
+-rw-rw-rw-   0        0        0     1181 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_tool_tip.py
+-rw-rw-rw-   0        0        0     1453 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.662492 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0    10126 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/breadcrumb.py
+-rw-rw-rw-   0        0        0    13248 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8745 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    24728 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    21213 2024-06-01 03:43:23.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     7059 2024-06-01 03:41:51.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     5254 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.691088 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5354 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0    11296 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     4697 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2843 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    14436 2024-06-01 03:41:51.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1544 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.818093 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     3328 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8188 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    30220 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     7755 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     5835 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    15886 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19946 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     8072 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    13322 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flip_view.py
+-rw-rw-rw-   0        0        0    17277 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2318 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1552 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16823 2024-06-01 03:43:10.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    19320 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0    14940 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    14414 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4750 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    40909 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0    11379 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/pips_pager.py
+-rw-rw-rw-   0        0        0     9269 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     7143 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2758 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    19583 2024-06-01 03:42:45.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     1226 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/separator.py
+-rw-rw-rw-   0        0        0    10206 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     8850 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6564 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5923 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8768 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    26737 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tab_view.py
+-rw-rw-rw-   0        0        0    11626 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    23075 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10674 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     4671 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.831618 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/
+-rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/__init__.py
+-rw-rw-rw-   0        0        0    11775 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_play_bar.py
+-rw-rw-rw-   0        0        0     3943 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_player.py
+-rw-rw-rw-   0        0        0     2947 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/video_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:50:00.850704 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    13085 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2840 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1685 2024-06-01 03:41:40.000000 PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 03:50:00.857221 PyQt6-Fluent-Widgets-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2024-06-01 03:44:02.000000 PyQt6-Fluent-Widgets-1.5.7/setup.py
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/LICENSE` & `PyQt6-Fluent-Widgets-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/PKG-INFO` & `PyQt6-Fluent-Widgets-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Fluent-Widgets
-Version: 1.5.6
+Version: 1.5.7
 Summary: A fluent design widgets library based on PyQt6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 1.5.6 Summary: A
+Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 1.5.7 Summary: A
 fluent design widgets library based on PyQt6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyqt6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt6-Fluent-Widgets-1.5.7/PyQt6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Fluent-Widgets
-Version: 1.5.6
+Version: 1.5.7
 Summary: A fluent design widgets library based on PyQt6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 1.5.6 Summary: A
+Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 1.5.7 Summary: A
 fluent design widgets library based on PyQt6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyqt6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt6-Fluent-Widgets-1.5.7/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/README.md` & `PyQt6-Fluent-Widgets-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3 for non-commercial project, see README for more details.
 """
 
-__version__ = "1.5.6"
+__version__ = "1.5.7"
 __author__ = "zhiyiYo"
 
 from .components import *
 from .common import *
 from .window import *
 from ._rc import resource
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
                 items[k].deserializeFrom(v)
             elif isinstance(v, dict):
                 for key, value in v.items():
                     key = k + "." + key
                     if items.get(key) is not None:
                         items[key].deserializeFrom(value)
 
-        self.theme = self.get(self.themeMode)
+        self.theme = self.get(self._cfg.themeMode)
 
     @property
     def theme(self):
         """ get theme mode, can be `Theme.Light` or `Theme.Dark` """
         return self._cfg._theme
 
     @theme.setter
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/screen.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/common/style_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,15 @@
     LIGHT_2 = "ThemeColorLight2"
     LIGHT_3 = "ThemeColorLight3"
 
     def name(self):
         return self.color().name()
 
     def color(self):
-        color = qconfig.get(qconfig.themeColor)  # type:QColor
+        color = qconfig.get(qconfig._cfg.themeColor)  # type:QColor
 
         # transform color into hsv space
         h, s, v, _ = color.getHsvF()
 
         if isDarkTheme():
             s *= 0.84
             v = 1
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,30 +49,34 @@
         opacityEffect = QGraphicsOpacityEffect(self)
         self.setGraphicsEffect(opacityEffect)
         opacityAni = QPropertyAnimation(opacityEffect, b'opacity', self)
         opacityAni.setStartValue(0)
         opacityAni.setEndValue(1)
         opacityAni.setDuration(200)
         opacityAni.setEasingCurve(QEasingCurve.Type.InSine)
-        opacityAni.finished.connect(opacityEffect.deleteLater)
+        opacityAni.finished.connect(lambda: self.setGraphicsEffect(None))
         opacityAni.start()
         super().showEvent(e)
 
     def done(self, code):
         """ fade out """
         self.widget.setGraphicsEffect(None)
         opacityEffect = QGraphicsOpacityEffect(self)
         self.setGraphicsEffect(opacityEffect)
         opacityAni = QPropertyAnimation(opacityEffect, b'opacity', self)
         opacityAni.setStartValue(1)
         opacityAni.setEndValue(0)
         opacityAni.setDuration(100)
-        opacityAni.finished.connect(lambda: QDialog.done(self, code))
+        opacityAni.finished.connect(lambda: self._onDone(code))
         opacityAni.start()
 
+    def _onDone(self, code):
+        self.setGraphicsEffect(None)
+        QDialog.done(self, code)
+
     def resizeEvent(self, e):
         self.windowMask.resize(self.size())
 
     def eventFilter(self, obj, e: QEvent):
         if obj is self.window():
             if e.type() == QEvent.Type.Resize:
                 self.resize(e.size())
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_box_base.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/flow_layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,27 @@
         self._deBounceTimer.timeout.connect(lambda: self._doLayout(self.geometry(), True))
         self._wParent = None
         self._isInstalledEventFilter = False
 
     def addItem(self, item):
         self._items.append(item)
 
+    def insertItem(self, index, item):
+        self._items.insert(index, item)
+
     def addWidget(self, w):
         super().addWidget(w)
+        self._onWidgetAdded(w)
+
+    def insertWidget(self, index, w):
+        self.insertItem(index, QWidgetItem(w))
+        self.addChildWidget(w)
+        self._onWidgetAdded(w, index)
 
+    def _onWidgetAdded(self, w, index=-1):
         if not self._isInstalledEventFilter:
             if w.parent():
                 self._wParent = w.parent()
                 w.parent().installEventFilter(self)
             else:
                 w.installEventFilter(self)
 
@@ -54,17 +64,21 @@
             return
 
         ani = QPropertyAnimation(w, b'geometry')
         ani.setEndValue(QRect(QPoint(0, 0), w.size()))
         ani.setDuration(self.duration)
         ani.setEasingCurve(self.ease)
         w.setProperty('flowAni', ani)
-        self._anis.append(ani)
         self._aniGroup.addAnimation(ani)
 
+        if index == -1:
+            self._anis.append(ani)
+        else:
+            self._anis.insert(index, ani)
+
     def setAnimation(self, duration, ease=QEasingCurve.Type.Linear):
         """ set the moving animation
 
         Parameters
         ----------
         duration: int
             the duration of animation in milliseconds
@@ -193,15 +207,15 @@
 
         for i, item in enumerate(self._items):
             if item.widget() and not item.widget().isVisible() and self.isTight:
                 continue
 
             nextX = x + item.sizeHint().width() + spaceX
 
-            if nextX - spaceX > rect.right() and rowHeight > 0:
+            if nextX - spaceX > rect.right() - margin.right() and rowHeight > 0:
                 x = rect.x() + margin.left()
                 y = y + rowHeight + spaceY
                 nextX = x + item.sizeHint().width() + spaceX
                 rowHeight = 0
 
             if move:
                 target = QRect(QPoint(x, y), item.sizeHint())
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_menu.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,19 @@
         self.isCompacted = True
         self.isSelected = False
         self.isPressed = False
         self.isEnter = False
         self.isSelectable = isSelectable
         self.treeParent = None
         self.nodeDepth = 0
+
+        # text color
+        self.lightTextColor = QColor(0, 0, 0)
+        self.darkTextColor = QColor(255, 255, 255)
+
         self.setFixedSize(40, 36)
 
     def enterEvent(self, e):
         self.isEnter = True
         self.update()
 
     def leaveEvent(self, e):
@@ -81,14 +86,32 @@
         if not self.isSelectable:
             return
 
         self.isSelected = isSelected
         self.update()
         self.selectedChanged.emit(isSelected)
 
+    def textColor(self):
+        return self.darkTextColor if isDarkTheme() else self.lightTextColor
+
+    def setLightTextColor(self, color):
+        """ set the text color in light theme mode """
+        self.lightTextColor = QColor(color)
+        self.update()
+
+    def setDarkTextColor(self, color):
+        """ set the text color in dark theme mode """
+        self.darkTextColor = QColor(color)
+        self.update()
+
+    def setTextColor(self, light, dark):
+        """ set the text color in light/dark theme mode """
+        self.setLightTextColor(light)
+        self.setDarkTextColor(dark)
+
 
 class NavigationPushButton(NavigationWidget):
     """ Navigation push button """
 
     def __init__(self, icon: Union[str, QIcon, FIF], text: str, isSelectable: bool, parent=None):
         """
         Parameters
@@ -157,15 +180,15 @@
         drawIcon(self._icon, painter, QRectF(11.5+pl, 10, 16, 16))
 
         # draw text
         if self.isCompacted:
             return
 
         painter.setFont(self.font())
-        painter.setPen(QColor(c, c, c))
+        painter.setPen(self.textColor())
 
         left = 44 + pl if not self.icon().isNull() else pl + 16
         painter.drawText(QRectF(left, 0, self.width()-13-left-pr, self.height()), Qt.AlignmentFlag.AlignVCenter, self.text())
 
 
 class NavigationToolButton(NavigationPushButton):
     """ Navigation tool button """
@@ -362,14 +385,29 @@
 
     def setText(self, text):
         self.itemWidget.setText(text)
 
     def setIcon(self, icon: Union[str, QIcon, FIF]):
         self.itemWidget.setIcon(icon)
 
+    def textColor(self):
+        return self.itemWidget.textColor()
+
+    def setLightTextColor(self, color):
+        """ set the text color in light theme mode """
+        self.itemWidget.setLightTextColor(color)
+
+    def setDarkTextColor(self, color):
+        """ set the text color in dark theme mode """
+        self.itemWidget.setDarkTextColor(color)
+
+    def setTextColor(self, light, dark):
+        """ set the text color in light/dark theme mode """
+        self.itemWidget.setTextColor(light, dark)
+
     def setFont(self, font: QFont):
         super().setFont(font)
         self.itemWidget.setFont(font)
 
     def clone(self):
         root = NavigationTreeWidget(self._icon, self.text(), self.isSelectable, self.parent())
         root.setSelected(self.isSelected)
@@ -511,15 +549,15 @@
         # draw avatar
         painter.setBrush(QBrush(self.avatar))
         painter.translate(8, 6)
         painter.drawEllipse(0, 0, 24, 24)
         painter.translate(-8, -6)
 
         if not self.isCompacted:
-            painter.setPen(Qt.GlobalColor.white if isDarkTheme() else Qt.GlobalColor.black)
+            painter.setPen(self.textColor())
             painter.setFont(self.font())
             painter.drawText(QRect(44, 0, 255, 36), Qt.AlignmentFlag.AlignVCenter, self.name)
 
 
 @InfoBadgeManager.register(InfoBadgePosition.NAVIGATION_ITEM)
 class NavigationItemInfoBadgeManager(InfoBadgeManager):
     """ Navigation item info badge manager """
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/pivot.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,18 @@
 
         self._currentRouteKey = routeKey
         self.slideAni.startAnimation(self.widget(routeKey).x())
 
         for k, item in self.items.items():
             item.setSelected(k == routeKey)
 
+    def showEvent(self, e):
+        super().showEvent(e)
+        self._adjustIndicatorPos()
+
     def setItemFontSize(self, size: int):
         """ set the pixel font size of items """
         for item in self.items.values():
             font = item.font()
             font.setPixelSize(size)
             item.setFont(font)
             item.adjustSize()
@@ -212,21 +216,24 @@
         self.setCurrentItem(item.property('routeKey'))
 
     def widget(self, routeKey: str):
         if routeKey not in self.items:
             raise RouteKeyError(f"`{routeKey}` is illegal.")
 
         return self.items[routeKey]
-    
+
     def resizeEvent(self, e) -> None:
-            super().resizeEvent(e)
+        super().resizeEvent(e)
+        self._adjustIndicatorPos()
 
-            item = self.currentItem()
-            if item is not None:
-                self.slideAni.setValue(item.x())
+    def _adjustIndicatorPos(self):
+        item = self.currentItem()
+        if item:
+            self.slideAni.stop()
+            self.slideAni.setValue(item.x())
 
     def paintEvent(self, e):
         super().paintEvent(e)
 
         if not self.currentItem():
             return
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,18 @@
         self.contentLabel.setText(content)
         self.contentLabel.setVisible(bool(content))
 
     def setValue(self, value):
         """ set the value of config item """
         pass
 
+    def setIconSize(self, width: int, height: int):
+        """ set the icon fixed size """
+        self.iconLabel.setFixedSize(width, height)
+
     def paintEvent(self, e):
         painter = QPainter(self)
         painter.setRenderHints(QPainter.RenderHint.Antialiasing)
 
         if isDarkTheme():
             painter.setBrush(QColor(255, 255, 255, 13))
             painter.setPen(QColor(0, 0, 0, 50))
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flip_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_badge.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self.lightBackgroundColor = None
         self.darkBackgroundColor = None
         self.manager = None  # type: InfoBadgeManager
         self.setLevel(level)
 
         setFont(self, 11)
         self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
+        self.setAttribute(Qt.WidgetAttribute.WA_TransparentForMouseEvents)
         self.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed)
         FluentStyleSheet.INFO_BADGE.apply(self)
 
     @__init__.register
     def _(self, text: str, parent: QWidget = None, level=InfoLevel.ATTENTION):
         self.__init__(parent, level)
         self.setText(text)
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/pips_pager.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,37 @@
 class ArrowButton(QToolButton):
     """ Arrow button """
 
     def __init__(self, icon: FluentIcon, parent=None):
         super().__init__(parent=parent)
         self.setFixedSize(10, 10)
         self._icon = icon
+        self.opacity = 1
+
+    def setOpacity(self, opacity):
+        self.opacity = opacity
+        self.update()
 
     def paintEvent(self, e):
         painter = QPainter(self)
         painter.setRenderHints(QPainter.RenderHint.Antialiasing)
+        painter.setOpacity(self.opacity)
 
         s = 7 if self.isDown() else 8
         x = (self.width() - s) / 2
         self._icon.render(painter, QRectF(x, x, s, s), fill="#858789")
 
 
 class ScrollBarGroove(QWidget):
     """ Scroll bar groove """
 
     def __init__(self, orient: Qt.Orientation, parent):
         super().__init__(parent=parent)
+        self._opacity = 1
+
         if orient == Qt.Orientation.Vertical:
             self.setFixedWidth(12)
             self.upButton = ArrowButton(FluentIcon.CARE_UP_SOLID, self)
             self.downButton = ArrowButton(FluentIcon.CARE_DOWN_SOLID, self)
             self.setLayout(QVBoxLayout(self))
             self.layout().addWidget(self.upButton, 0, Qt.AlignmentFlag.AlignHCenter)
             self.layout().addStretch(1)
@@ -46,41 +54,55 @@
             self.downButton = ArrowButton(FluentIcon.CARE_RIGHT_SOLID, self)
             self.setLayout(QHBoxLayout(self))
             self.layout().addWidget(self.upButton, 0, Qt.AlignmentFlag.AlignVCenter)
             self.layout().addStretch(1)
             self.layout().addWidget(self.downButton, 0, Qt.AlignmentFlag.AlignVCenter)
             self.layout().setContentsMargins(3, 0, 3, 0)
 
-        self.opacityEffect = QGraphicsOpacityEffect(self)
-        self.opacityAni = QPropertyAnimation(self.opacityEffect, b'opacity', self)
-        self.setGraphicsEffect(self.opacityEffect)
-        self.opacityEffect.setOpacity(0)
+        self.opacityAni = QPropertyAnimation(self, b'opacity', self)
+        self.setOpacity(0)
 
     def fadeIn(self):
+        self.opacityAni.stop()
+        self.opacityAni.setStartValue(self.opacity)
         self.opacityAni.setEndValue(1)
         self.opacityAni.setDuration(150)
         self.opacityAni.start()
 
     def fadeOut(self):
+        self.opacityAni.stop()
+        self.opacityAni.setStartValue(self.opacity)
         self.opacityAni.setEndValue(0)
         self.opacityAni.setDuration(150)
         self.opacityAni.start()
 
     def paintEvent(self, e):
         painter = QPainter(self)
         painter.setRenderHints(QPainter.RenderHint.Antialiasing)
+        painter.setOpacity(self.opacity)
         painter.setPen(Qt.PenStyle.NoPen)
 
         if not isDarkTheme():
             painter.setBrush(QColor(252, 252, 252, 217))
         else:
             painter.setBrush(QColor(44, 44, 44, 245))
 
         painter.drawRoundedRect(self.rect(), 6, 6)
 
+    def setOpacity(self, opacity: float):
+        self._opacity = opacity
+        self.upButton.setOpacity(opacity)
+        self.downButton.setOpacity(opacity)
+        self.update()
+
+    def getOpacity(self) -> float:
+        return self._opacity
+
+    opacity = pyqtProperty(float, getOpacity, setOpacity)
+
 
 class ScrollBarHandle(QWidget):
     """ Scroll bar handle """
 
     def __init__(self, orient: Qt.Orientation, parent=None):
         super().__init__(parent)
         self.orient = orient
@@ -369,15 +391,15 @@
     def _isSlideResion(self, pos: QPoint):
         if self.orientation() == Qt.Orientation.Vertical:
             return self._padding <= pos.y() <= self.height() - self._padding
 
         return self._padding <= pos.x() <= self.width() - self._padding
 
     def _onOpacityAniValueChanged(self):
-        opacity = self.groove.opacityEffect.opacity()
+        opacity = self.groove.opacity
         if self.orientation() == Qt.Orientation.Vertical:
             self.handle.setFixedWidth(int(3 + opacity * 3))
         else:
             self.handle.setFixedHeight(int(3 + opacity * 3))
 
         self._adjustHandlePos()
 
@@ -498,14 +520,25 @@
 
         parent.viewport().installEventFilter(self)
         parent.setVerticalScrollBarPolicy = self.setVerticalScrollBarPolicy
         parent.setHorizontalScrollBarPolicy = self.setHorizontalScrollBarPolicy
 
     def eventFilter(self, obj, e: QEvent):
         if e.type() == QEvent.Type.Wheel:
+            # Check if the vertical scroll is at its limit
+            verticalAtEnd = (e.angleDelta().y() < 0 and self.vScrollBar.value() == self.vScrollBar.maximum()) or \
+                            (e.angleDelta().y() > 0 and self.vScrollBar.value() == self.vScrollBar.minimum())
+
+            # Check if the horizontal scroll is at its limit
+            horizontalAtEnd = (e.angleDelta().x() < 0 and self.hScrollBar.value() == self.hScrollBar.maximum()) or \
+                              (e.angleDelta().x() > 0 and self.hScrollBar.value() == self.hScrollBar.minimum())
+
+            if verticalAtEnd or horizontalAtEnd:
+                return False
+
             if e.angleDelta().y() != 0:
                 if not self.useAni:
                     self.verticalSmoothScroll.wheelEvent(e)
                 else:
                     self.vScrollBar.scrollValue(-e.angleDelta().y())
             else:
                 if not self.useAni:
```

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_play_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_player.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/video_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py` & `PyQt6-Fluent-Widgets-1.5.7/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-1.5.6/setup.py` & `PyQt6-Fluent-Widgets-1.5.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Fluent-Widgets",
-    version="1.5.6",
+    version="1.5.7",
     keywords="pyqt6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

