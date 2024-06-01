# Comparing `tmp/PySide2-Fluent-Widgets-1.5.6.tar.gz` & `tmp/PySide2-Fluent-Widgets-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Fluent-Widgets-1.5.6.tar", last modified: Tue May  7 03:47:19 2024, max compression
+gzip compressed data, was "dist\PySide2-Fluent-Widgets-1.5.7.tar", last modified: Sat Jun  1 03:36:18 2024, max compression
```

## Comparing `PySide2-Fluent-Widgets-1.5.6.tar` & `PySide2-Fluent-Widgets-1.5.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.542672 PySide2-Fluent-Widgets-1.5.6/
--rw-rw-rw-   0        0        0    35821 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/LICENSE
--rw-rw-rw-   0        0        0     5311 2024-05-07 03:47:19.542672 PySide2-Fluent-Widgets-1.5.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.357791 PySide2-Fluent-Widgets-1.5.6/PySide2_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     5311 2024-05-07 03:47:19.000000 PySide2-Fluent-Widgets-1.5.6/PySide2_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4929 2024-05-07 03:47:19.000000 PySide2-Fluent-Widgets-1.5.6/PySide2_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:47:19.000000 PySide2-Fluent-Widgets-1.5.6/PySide2_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-05-07 03:47:19.000000 PySide2-Fluent-Widgets-1.5.6/PySide2_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 03:47:19.000000 PySide2-Fluent-Widgets-1.5.6/PySide2_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4527 2024-05-07 03:45:26.000000 PySide2-Fluent-Widgets-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.359810 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/
--rw-rw-rw-   0        0        0      558 2024-05-07 03:45:16.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.362874 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  3306803 2024-05-07 03:45:47.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.395451 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0    15206 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1589 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py
--rw-rw-rw-   0        0        0    11172 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      807 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    13755 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     5541 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0      664 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py
--rw-rw-rw-   0        0        0     4865 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    14413 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      454 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.397471 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.408237 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2567 2024-05-07 03:45:16.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21795 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7615 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19331 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     6413 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.420094 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14789 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5838 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11331 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3140 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2873 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py
--rw-rw-rw-   0        0        0     2492 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.427805 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2716 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     7104 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1305 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.439233 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/
--rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py
--rw-rw-rw-   0        0        0     3010 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py
--rw-rw-rw-   0        0        0     3542 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py
--rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py
--rw-rw-rw-   0        0        0     6282 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py
--rw-rw-rw-   0        0        0     1187 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py
--rw-rw-rw-   0        0        0     1425 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.454270 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     9940 2024-05-07 03:45:16.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py
--rw-rw-rw-   0        0        0    12954 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8722 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    24091 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    19679 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6823 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     5205 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.466403 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5280 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0    11029 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     4610 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2841 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    14030 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1590 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.527034 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     3316 2024-05-07 03:40:08.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     8061 2024-05-07 03:45:16.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    29986 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     7688 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     5808 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    16286 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19596 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     7879 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    13089 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py
--rw-rw-rw-   0        0        0    17080 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2229 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1496 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16653 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    18932 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0    14721 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    14106 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4794 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    40493 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0    11175 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py
--rw-rw-rw-   0        0        0     9173 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     7029 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2759 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17861 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     1167 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py
--rw-rw-rw-   0        0        0    10219 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     8634 2024-05-07 03:45:16.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6535 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5795 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8597 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    26315 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py
--rw-rw-rw-   0        0        0    11534 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    22912 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10581 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     4526 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.533989 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/
--rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/__init__.py
--rw-rw-rw-   0        0        0    11611 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py
--rw-rw-rw-   0        0        0     3555 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py
--rw-rw-rw-   0        0        0     2849 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:47:19.540226 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    12940 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2854 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1660 2024-05-07 03:45:06.000000 PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2024-05-07 03:47:19.543586 PySide2-Fluent-Widgets-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1218 2024-05-07 03:45:30.000000 PySide2-Fluent-Widgets-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.902734 PySide2-Fluent-Widgets-1.5.7/
+-rw-rw-rw-   0        0        0    35821 2024-06-01 03:33:58.000000 PySide2-Fluent-Widgets-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0     5311 2024-06-01 03:36:18.901726 PySide2-Fluent-Widgets-1.5.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.709255 PySide2-Fluent-Widgets-1.5.7/PySide2_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5311 2024-06-01 03:36:18.000000 PySide2-Fluent-Widgets-1.5.7/PySide2_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4929 2024-06-01 03:36:18.000000 PySide2-Fluent-Widgets-1.5.7/PySide2_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 03:36:18.000000 PySide2-Fluent-Widgets-1.5.7/PySide2_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-06-01 03:36:18.000000 PySide2-Fluent-Widgets-1.5.7/PySide2_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 03:36:18.000000 PySide2-Fluent-Widgets-1.5.7/PySide2_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4527 2024-06-01 03:33:58.000000 PySide2-Fluent-Widgets-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.711252 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/
+-rw-rw-rw-   0        0        0      558 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.714251 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  3306805 2024-06-01 03:34:52.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.747878 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0    15206 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1589 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/color.py
+-rw-rw-rw-   0        0        0    11177 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      807 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    13755 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     5541 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0      664 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/screen.py
+-rw-rw-rw-   0        0        0     4865 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    14418 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      454 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.748957 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.760655 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2567 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21795 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7615 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19331 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     6413 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.774288 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14789 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5838 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11331 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3249 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2873 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_box_base.py
+-rw-rw-rw-   0        0        0     2492 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.780195 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2716 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     7529 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1305 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.793100 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/
+-rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/__init__.py
+-rw-rw-rw-   0        0        0     3010 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_combo_box.py
+-rw-rw-rw-   0        0        0     3542 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_flyout.py
+-rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_line_edit.py
+-rw-rw-rw-   0        0        0     6282 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_menu.py
+-rw-rw-rw-   0        0        0     1187 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_tool_tip.py
+-rw-rw-rw-   0        0        0     1425 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.808733 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     9940 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/breadcrumb.py
+-rw-rw-rw-   0        0        0    12954 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8722 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    24091 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    20922 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6994 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     5205 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.821524 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5280 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0    11029 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     4610 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2841 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    14178 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1590 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.885698 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     3316 2024-06-01 03:22:18.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8061 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    29986 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     7688 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     5808 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    16286 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19596 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     7879 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    13089 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flip_view.py
+-rw-rw-rw-   0        0        0    17080 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2229 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1496 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16713 2024-06-01 03:34:07.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    18932 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0    14721 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    14106 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4794 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    40493 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0    11175 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/pips_pager.py
+-rw-rw-rw-   0        0        0     9173 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     7029 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2759 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    19093 2024-06-01 03:34:34.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     1167 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/separator.py
+-rw-rw-rw-   0        0        0    10219 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     8634 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6535 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5795 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8597 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    26315 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tab_view.py
+-rw-rw-rw-   0        0        0    11534 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    22912 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10581 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     4526 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.892709 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/
+-rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/__init__.py
+-rw-rw-rw-   0        0        0    11611 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_play_bar.py
+-rw-rw-rw-   0        0        0     3555 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_player.py
+-rw-rw-rw-   0        0        0     2849 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/video_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:36:18.900367 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    12940 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2854 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1660 2024-06-01 03:33:59.000000 PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 03:36:18.902734 PySide2-Fluent-Widgets-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1218 2024-06-01 03:34:23.000000 PySide2-Fluent-Widgets-1.5.7/setup.py
```

### Comparing `PySide2-Fluent-Widgets-1.5.6/LICENSE` & `PySide2-Fluent-Widgets-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/PKG-INFO` & `PySide2-Fluent-Widgets-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Fluent-Widgets
-Version: 1.5.6
+Version: 1.5.7
 Summary: A fluent design widgets library based on PySide2
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 1.5.6 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 1.5.7 Summary: A
 fluent design widgets library based on PySide2 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyside2 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
```

### Comparing `PySide2-Fluent-Widgets-1.5.6/PySide2_Fluent_Widgets.egg-info/PKG-INFO` & `PySide2-Fluent-Widgets-1.5.7/PySide2_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Fluent-Widgets
-Version: 1.5.6
+Version: 1.5.7
 Summary: A fluent design widgets library based on PySide2
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 1.5.6 Summary: A
+Metadata-Version: 2.1 Name: PySide2-Fluent-Widgets Version: 1.5.7 Summary: A
 fluent design widgets library based on PySide2 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyside2 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
```

### Comparing `PySide2-Fluent-Widgets-1.5.6/PySide2_Fluent_Widgets.egg-info/SOURCES.txt` & `PySide2-Fluent-Widgets-1.5.7/PySide2_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/README.md` & `PySide2-Fluent-Widgets-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide2/examples.
 
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

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -93724,42 +93724,42 @@
 transparent;\x0d\x0a  \
   border: none;\x0d\
 \x0a}\x0d\x0a\x0d\x0aSwitchButt\
 on>QLabel:disabl\
 ed {\x0d\x0a    color:\
  rgba(0, 0, 0, 0\
 .36);\x0d\x0a}\x0d\x0a\x0d\x0a\
-\x00\x00\x01\x9f\
+\x00\x00\x01\x97\
 \x00\
-\x00\x06\xf2x\x9c\x9dU\xddn\x820\x18\xbd7\xf1\x1d\
-\x9a\xecf$\xba\x80\x0a*\xcb\x1e\xc0;\x13\x97\xecb\
-\xd9E\xa1\x9f\xd8\xac\xb4\xa4\x14g\xb2\xf8\xeek\xb0\xf8\
-\x03U\x9a\x11\x08\xd0\xaf\x9c\x9e\x8fs\x0e\xac\xe9^\xa8\
-\x95\x82\x1c\xfd\x0e\x07Ho\x05&\x84\xf2,F\x81_\
-\x1cP0)\x0e\xaf\xa7B*\x98\x901J\x18N\xbf\
-\xcdP\xa2/3)*N\xc6\xa6\xaa$\xe6e\x81%\
-p\xd5\xcc\x11\x92\x80\xaep\xc1\xc1\x0c\x89J1\xca\xe1\
-f,\xc72\xa3<F\xbe\xbe?\x0e\x07\xc3\xc1\xba!\
-\xf6I\xcb\x0d0H\x15\x907%+\xf8\x8awb\x0f\
-\xb2\xe1k\x16\x96Y\x82\x9f\xfd\x112\xfbK4\xf5\x1c\
-\x90\x0a\x09e\x09\xa4\x07+\xec\xc1\xdabV:\x83\xcd\
-C\x0b\xd8\x0e\x97\xabTp\x83\xd4\x92b\xcc`\xab\xe2\
-k)\x9a\x82\xa4\xd9\xeeR\xb9\x83Ywj\x87\x9cF\
-\xce\x90\x0d\x80E\xce>\x17\xd4 O{\x0a?g\x10\
-\x97'6\x90\xe5\xfa\x16\xc8\xbb\x10\xcc\xea\xd0P\x1bt\
-\xa9\x0f\xdd\x05Z\x5c\xf8\x9e\x1f\xfc\xa0$\x035B7\
-H\xa7\xc1\xfbL\xdaz\xf9\x93Y\xe0\xb5\xbc\x1c\xe8\x05\
-K\xc1(\xe9\xce\x0e\xe7\x8b\xdb\xd9c\x89\x09\xad\xca\x18\
-E\x16\x86v'\x8d,\xcdwg\xb5%U\xa2\xd0\x8a\
-v\x04M\x84R\x22\xbf\xae\xfc3\xb5\xd6v\xae\xa3\xab\
-W@\x13\xe7&O)vk\xf56\xf1}\x9a-=\
-W\x0a&\xb1\x8e$Z\xf9\xee\xa3\x11y\x96\xf73\xd3\
-\x879\xf7\x92\xac\x83\xdb\xc7\xcd\x9a\xee\xda\x0a\xddl7\
-V\xe8J\xe7;\x9b\xc3\x81rW\xd9\x87\x1f_\xa7\x0e\
-\xdd\xdc\xf2\xe8\xa3\xde\xfc\xb7\x8e\x7f%P0\x22\
+\x00\x06\xd4x\x9c\x9dU\xd1j\xc20\x14}\x17\xfc\x87\
+\xc0^&\xe8hu\xad\xda\xb1\x0f\xf0Mp\xb0\x87\xb1\
+\x87\xb4\xb9\xd6\xb04)I\xea\x84\xe1\xbf/\xd4Vm\
+\x1bm\xb0\xb4\xd0\xe4\xde\x9e{.\xe7\x9etM\xf7B\
+\xaf4d\xe8o8@\xe6\xca1!\x94\xa7\x11\xf2\xbd\
+\xfc\x80\xfci~x;\x05\x12\xc1\x84\x8cP\xccp\xf2\
+Sm\xc5\xe65\x95\xa2\xe0dRE\xb5\xc4\x5c\xe5X\
+\x02\xd7u\x8e\x90\x04L\x84\x0b\x0e\xd5\x96(4\xa3\x1c\
+\x1a{\x19\x96)\xe5\x11\xf2\xcc\xfa8\x1c\x0c\x07\xeb\x9a\
+\xd8\x17U\x1b`\x90h \xefZ\x16\xf0\x1d\xed\xc4\x1e\
+d\xcd\xb7*,\xd3\x18?{cT\xdd/\xe1l\xe4\
+\x80\x94KP\x0aH\x0fV\xd0\x83\xb5\xc5L9\x83\xcd\
+\x03\x0b\xd8\x0e\xabU\x22x\x85\xd4\x92b\xc2`\xab\xa3\
+k)\xea\x80\xa4\xe9\xee\x12\xb9\x81Yvj\x87\x9c\x85\
+\xce\x905\x80E\xce\xbe)(A\x9e\xf6\x14~\xcf \
+._l \xcd\xcc\x12\xc8\x87\x10\xcc:\xa1\x81\x19\xd0\
+\xa5yL\x17hq\xe1{\xfe\xf0\x93\x92\x14\xf4\x185\
+\x90N\x9b\xb7\x99\xb4\xf5\xf2\xa6\xaf\xfe\xa85\xcb\xbe)\
+\xa8\x04\xa3\xa4\x9b\x1d\xcc\x17\xcd\xec\x89\xc4\x84\x16*B\
+\xa1\x85\xa1}\x92\xc6\x96\xe6\xbbYmI\xb5\xc8\x8d\xa2\
+\x1dAc\xa1\xb5\xc8\xae#\x0f\xba\xd6\xda\xce\xb5uM\
+\x05\xe497yr\xb1[\xabM\xc7\xf7i\xb6\x1c\xb9\
+R\xa8\x1c\xebH\xa2\xe5\xef>\x1aa?\x8d\xd2\x9a}\
+\xd5\xad\xfe-\xc5\xee\xba\xb7\x16\xbb+\x8e\xe7,\xbf\x03\
+\xe5\xaevw\x8fW\xa7\x0e\xdd\xe6\xe1\xde\xb1]\xff\x99\
+\x8e\xff\xac\x0e'\xa8\
 \x00\x00\x02\x01\
 \x00\
 \x00\x07{x\x9c\xcdT\xdbj\xe30\x10}\x0f\xe4\x1f\
 \x04}H\x0cqqnn\x9ae_\xda\xb2\x17\xd8\x85\
 B\xd8\x85e\xe9\xc3\xd8\x9a8\x22\xaaddy\x93e\
 \xe9\xbfW\xce\xcau}Q\x9a\xd2\x97\x86\xa0\x84\xd1\xcc\
 \x99\x99sFs\xa6\x99\xe6x\x95k-\x05\xf9\xd7\xef\
@@ -94841,42 +94841,41 @@
 t;\x0d\x0a    border: \
 none;\x0d\x0a}\x0d\x0a\x0d\x0aSwit\
 chButton>QLabel:\
 disabled {\x0d\x0a    \
 color: rgba(255,\
  255, 255, 0.36)\
 ;\x0d\x0a}\x0d\x0a\x0d\x0a\
-\x00\x00\x01\x93\
+\x00\x00\x01\x8b\
 \x00\
-\x00\x06Ux\x9c\xa5T]o\x820\x14}7\xf1?\
-4\xd9\xcbH\xc4\x80\x0e\xa6,\xfb\x01\xbe\x99\xb8d\x0f\
-\xcb\x1e*\xbdB3hI[\xd4d\xd9\x7f_\xc7\x87\
-:\xa8\xa3\xdb\x08\x85\xd0\xd3{z.\xe7\xde\xae\xe9\x9e\
-\xab\x95\x82\x1c\xbd\x8fGH_\x05&\x84\xb2$B\xbe\
-W\x1c\x91?+\x8e\x0f5\x10\xf3\x8c\x8b\x08\x1dR\xaa\
-\xa0\x99\xda\xe2\xf8-\x11\xbcd\xc4mP%0\x93\x05\
-\x16\xc0T\xbb\x86\x0b\x02\x1aa\x9c\xb5a\xbcT\x19e\
-p\x9a\xfb\x18\x8f\xc6\xa3u+\xe4\x85\xca\x0dd\x10+\
- \x8fJ\x94\xf0\x1a\xa5|\x0f\xa2\xd5\xd7l$\x92-\
-\xbe\x9d\x05\xc1\x04\x9d\x1f\xde4\x9c;\x16|\x85\x00)\
-\x81X1\x06\x03\x8c;\x9c\xc9_R\xde\x07\x06\xca\x14\
-\xcbU\xccY\xc3\xd71\xc3\xcd`\xa7\xa2K3Z@\
-\xd0$=#W8\xab\xac\xcd\x94\xf3\xd0\x9a\xb2%0\
-\x18:T\x07\x15\xc9\xcd\x9e\xc2\xe1Db\x13\xb1\x81$\
-\xd7\x9f@\x9e8\xcf\x8c5\x1a\xe8\x12]\xea\xa1\xb3@\
-\x8b\xb3\xdeS\xe03%\x09\xa8I\x87\xaa\x9e\xbd.\xa5\
-\xb2\xcd\xd3V\xd5\xf7\xd4w:\xb5\xec\xeb\xed$\xcf(\
-\xb9\xe2\xb0\xb7\xf8\x1e\xe1\x0aLh)#\x14\x1a4\x9a\
-+j\x82z\xd9\xf7\x17u=U\xbc\xd0\x96\xf6\x1c\xdd\
-r\xa5x~\x89\xfc\xb1q\x8d\xd9|\x019\x16\x09e\
-\xd5\x0ehf\x9dc\xdd\xd8]w~Z;\xe0Y\xc7\
-\x88\xa5c+\xa4i_K)\x9df\xb7\x13\x13:\x86\
-\x7fu\xa7G\xf3\x1e\x94Zu\xf1\x90Bc\xabWe\
-\xd1o\xf4\xb6,\xfa6z\xff9\xf4u\x16\x9f\x17\x15\
-\xf3\x1c\
+\x00\x067x\x9c\xa5\x94Qk\x830\x10\xc7\xdf\x0b\xfd\
+\x0e\x81\xbd\xac\xd0\x16m\xd1\xb5\x8e}\x80\xbe\x15:\xd8\
+\xc3\xd8Cj\xae\x1a\xa69Ib[\x18\xfb\xee\xcb\xac\
+\xb6\x9b\xa63\xdbD\x05s\xb9\x7f\xfe\xc7\xef\xce5\xdf\
+\xa3^i\xc8\xc9\xdbp@\xccUP\xc6\xb8H\x22\xe2\
+{\xc5\x91\xf8\xb3\xe2x\x7f\x0a\xc4\x98\xa1\x8c\xc8!\xe5\
+\x1a\xea\xa5-\x8d_\x13\x89\xa5`\x93:\xaa%\x15\xaa\
+\xa0\x12\x84n\xf6\xa0d`\x22\x02E\x93\x86\xa5\xce\xb8\
+\x80\xf3\xda\xfbp0\x1c\xac\x1b#\xcf\x5cm \x83X\
+\x03{\xd0\xb2\x84\x97(\xc5=\xc8\xc6_}\x90L\xb6\
+\xf4v\x16\x04cryy\xd3p>r\xd0+$(\
+\x05\xccI1\xe8Q\xdc\xd1L\xfdR\xf2.\xb0H\xa6\
+T\xadb\x14\xb5^\x0b\xc6$\x83\x9d\x8e\xbe\xc2h\x02\
+\x92'\xe9%rE\xb3\xaa\xda.9\x0f\x9d%\x1b\x01\
+\x0b\xd0\xbe>\xa8Dn\xf6\x1c\x0eg\x11\x97\x8c\x0d$\
+\xb9\xf9\x04\xf6\x88\x98Y{40-\xba4\x8f\xa9\x82\
+,.~\xcf\x89O\x9c%\xa0\xc7-\xa9\xd3\xeau+\
+\x156\xcf\xa0:\xddS\x7f\xd4\xeae\xdf\x1c\xa70\xe3\
+\xec\x0aao\xf1=c\x22)\xe3\xa5\x8aHh\xf1h\
+\xef\xa81\xe9T\xdf\xdd\xd4f\xaa\xb10H;D\xb7\
+\xa85\xe6_#\x7f\x1c\x5ck5\x9f\x81\x9c\xca\x84\x8b\
+\xea\x04\xe29\xd7x\x1a\xec6\x9d\x9f\xf6\xf60k\x81\
+X\x8e\x5c\x8d\xd4\xe3\xebh\xa55\xecnf\xc2~3\
+\xd5\x9c\xf6y\xb0\x0es\x05\xbe;\xca\x0d\xf8.(\xef\
+?\xbfuS\xc5\x07\xf9\xbe\xea\xa2\
 \x00\x00\x02\x01\
 \x00\
 \x00\x07\xc1x\x9c\xcdT]k\xdb0\x14}\x0f\xe4?\
 \x08\xfa\x90\x18\xe2\xe18\xb1\xe7f\xec\xa5-k\x07\x1b\
 \x14\xc2\x06c\xecA\xb6o\x1c\x11U2\xb2\xdcd\x8c\
 \xfe\xf7]'\xfehl+]:\x18\x0b\xc8\x01\xe9\xea\
 \xdc{\xcf9\xba\x17\x9ai\x0eW\xb9\xd6R\x90_\xc3\
@@ -98836,150 +98835,150 @@
 \x00\x00\x01\x8d\xa6\xd33\xb3\
 \x00\x00F\xb8\x00\x00\x00\x00\x00\x01\x00\x16@\x08\
 \x00\x00\x01\x8b1\x07F\x91\
 \x00\x00G\x88\x00\x02\x00\x00\x00\x22\x00\x00\x01\xfe\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00G\x96\x00\x02\x00\x00\x00\x22\x00\x00\x01\xdc\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00K4\x00\x00\x00\x00\x00\x01\x00\x16\xba\x0a\
+\x00\x00K4\x00\x00\x00\x00\x00\x01\x00\x16\xba\x02\
 \x00\x00\x01\x8b1\x07Mz\
 \x00\x00HZ\x00\x01\x00\x00\x00\x01\x00\x16\x8c\x08\
 \x00\x00\x01\x8d\xa5\x92\xa6D\
-\x00\x00K\x9e\x00\x00\x00\x00\x00\x01\x00\x16\xbe\x83\
+\x00\x00K\x9e\x00\x00\x00\x00\x00\x01\x00\x16\xbe{\
 \x00\x00\x01\x8b1\x07MG\
-\x00\x00KR\x00\x01\x00\x00\x00\x01\x00\x16\xba\x82\
+\x00\x00KR\x00\x01\x00\x00\x00\x01\x00\x16\xbaz\
 \x00\x00\x01\x8c\x01\x8b~\xfe\
-\x00\x00Jd\x00\x01\x00\x00\x00\x01\x00\x16\xad\xe4\
+\x00\x00Jd\x00\x01\x00\x00\x00\x01\x00\x16\xad\xdc\
 \x00\x00\x01\x8d\xa6\xd33\xdd\
-\x00\x00J\xd6\x00\x00\x00\x00\x00\x01\x00\x16\xb5\xf6\
+\x00\x00J\xd6\x00\x00\x00\x00\x00\x01\x00\x16\xb5\xee\
 \x00\x00\x01\x8b1\x07M2\
-\x00\x00J\xf8\x00\x00\x00\x00\x00\x01\x00\x16\xb6:\
+\x00\x00J\xf8\x00\x00\x00\x00\x00\x01\x00\x16\xb62\
 \x00\x00\x01\x8b1\x07M\x97\
-\x00\x00I\x98\x00\x00\x00\x00\x00\x01\x00\x16\xa3\xfe\
+\x00\x00I\x98\x00\x00\x00\x00\x00\x01\x00\x16\xa3\xf6\
 \x00\x00\x01\x8b1\x07MW\
-\x00\x00K\xc4\x00\x00\x00\x00\x00\x01\x00\x16\xbe\xf1\
+\x00\x00K\xc4\x00\x00\x00\x00\x00\x01\x00\x16\xbe\xe9\
 \x00\x00\x01\x8b1\x07M\x1d\
-\x00\x00K\x16\x00\x01\x00\x00\x00\x01\x00\x16\xb7\xd8\
-\x00\x00\x01\x8fQ'\xd5\x92\
+\x00\x00K\x16\x00\x01\x00\x00\x00\x01\x00\x16\xb7\xd0\
+\x00\x00\x01\x8f\xd1\xbd5\xf3\
 \x00\x00H\xd4\x00\x00\x00\x00\x00\x01\x00\x16\x92\xdc\
 \x00\x00\x01\x8b1\x07M:\
-\x00\x00Kz\x00\x01\x00\x00\x00\x01\x00\x16\xbc,\
+\x00\x00Kz\x00\x01\x00\x00\x00\x01\x00\x16\xbc$\
 \x00\x00\x01\x8b1\x07M\x8f\
-\x00\x00Il\x00\x01\x00\x00\x00\x01\x00\x16\xa1\xf9\
+\x00\x00Il\x00\x01\x00\x00\x00\x01\x00\x16\xa1\xf1\
 \x00\x00\x01\x8b1\x07L\xf6\
-\x00\x00J\x9e\x00\x00\x00\x00\x00\x01\x00\x16\xb1\x91\
+\x00\x00J\x9e\x00\x00\x00\x00\x00\x01\x00\x16\xb1\x89\
 \x00\x00\x01\x8c\x00\xb0\x09\x84\
 \x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\x85\xf3\
 \x00\x00\x01\x8b1\x07M\x87\
-\x00\x00I\xe2\x00\x00\x00\x00\x00\x01\x00\x16\xa8\xd6\
+\x00\x00I\xe2\x00\x00\x00\x00\x00\x01\x00\x16\xa8\xce\
 \x00\x00\x01\x8b1\x07Ms\
 \x00\x00H\xb4\x00\x01\x00\x00\x00\x01\x00\x16\x90V\
 \x00\x00\x01\x8c\xb4\xff\xf1\xb5\
-\x00\x00J\xb6\x00\x00\x00\x00\x00\x01\x00\x16\xb3j\
+\x00\x00J\xb6\x00\x00\x00\x00\x00\x01\x00\x16\xb3b\
 \x00\x00\x01\x8c\xb4\xff\xf1\xaf\
 \x00\x00I,\x00\x00\x00\x00\x00\x01\x00\x16\x9e\xe5\
 \x00\x00\x01\x8b1\x07My\
-\x00\x00J~\x00\x00\x00\x00\x00\x01\x00\x16\xaf\xe5\
+\x00\x00J~\x00\x00\x00\x00\x00\x01\x00\x16\xaf\xdd\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa9\
-\x00\x00L\x0a\x00\x01\x00\x00\x00\x01\x00\x16\xc11\
+\x00\x00L\x0a\x00\x01\x00\x00\x00\x01\x00\x16\xc1)\
 \x00\x00\x01\x8b1\x07Mf\
 \x00\x00I\x12\x00\x01\x00\x00\x00\x01\x00\x16\x99\xf3\
 \x00\x00\x01\x8d\xb652e\
-\x00\x00J2\x00\x00\x00\x00\x00\x01\x00\x16\xad=\
+\x00\x00J2\x00\x00\x00\x00\x00\x01\x00\x16\xad5\
 \x00\x00\x01\x8b1\x07Mf\
 \x00\x00H\x9e\x00\x01\x00\x00\x00\x01\x00\x16\x8ek\
 \x00\x00\x01\x8bf\xa8\x0a\xf2\
 \x00\x00G\xcc\x00\x00\x00\x00\x00\x01\x00\x16\x87\x1f\
 \x00\x00\x01\x8b1\x07L\xfc\
 \x00\x00H&\x00\x01\x00\x00\x00\x01\x00\x16\x8a*\
 \x00\x00\x01\x8d\xa6\xd33\xe2\
-\x00\x00I\xc2\x00\x01\x00\x00\x00\x01\x00\x16\xa7B\
-\x00\x00\x01\x8fQ'\xd5\x91\
-\x00\x00L$\x00\x00\x00\x00\x00\x01\x00\x16\xc2\xe8\
+\x00\x00I\xc2\x00\x01\x00\x00\x00\x01\x00\x16\xa7:\
+\x00\x00\x01\x8f\xd1\xbd5\xee\
+\x00\x00L$\x00\x00\x00\x00\x00\x01\x00\x16\xc2\xe0\
 \x00\x00\x01\x8b1\x07M,\
 \x00\x00H|\x00\x00\x00\x00\x00\x01\x00\x16\x8e\x22\
 \x00\x00\x01\x8b1\x07M^\
 \x00\x00IT\x00\x01\x00\x00\x00\x01\x00\x16\xa0V\
-\x00\x00\x01\x8c\x00\xb0\x09\x8d\
+\x00\x00\x01\x8f\xd1\xdc\x9e\xbd\
 \x00\x00H\xf2\x00\x00\x00\x00\x00\x01\x00\x16\x96\x9c\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa9\
 \x00\x00G\xf0\x00\x00\x00\x00\x00\x01\x00\x16\x87\xbe\
 \x00\x00\x01\x8b1\x07M^\
-\x00\x00J\x0c\x00\x01\x00\x00\x00\x01\x00\x16\xaaK\
+\x00\x00J\x0c\x00\x01\x00\x00\x00\x01\x00\x16\xaaC\
 \x00\x00\x01\x8b1\x07M\x08\
-\x00\x00K\xe4\x00\x01\x00\x00\x00\x01\x00\x16\xbf9\
+\x00\x00K\xe4\x00\x01\x00\x00\x00\x01\x00\x16\xbf1\
 \x00\x00\x01\x8d\xa6\xd33\xe7\
-\x00\x00K4\x00\x00\x00\x00\x00\x01\x00\x17\x04\x11\
+\x00\x00K4\x00\x00\x00\x00\x00\x01\x00\x17\x04\x01\
 \x00\x00\x01\x8b1\x07L\xca\
-\x00\x00HZ\x00\x01\x00\x00\x00\x01\x00\x16\xcc\xf3\
+\x00\x00HZ\x00\x01\x00\x00\x00\x01\x00\x16\xcc\xeb\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa3\
-\x00\x00K\x9e\x00\x00\x00\x00\x00\x01\x00\x17\x08\x8d\
+\x00\x00K\x9e\x00\x00\x00\x00\x00\x01\x00\x17\x08}\
 \x00\x00\x01\x8b1\x07L\x8e\
-\x00\x00KR\x00\x01\x00\x00\x00\x01\x00\x17\x04\x89\
+\x00\x00KR\x00\x01\x00\x00\x00\x01\x00\x17\x04y\
 \x00\x00\x01\x8c\x01\x8b~\xfb\
-\x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xf2\xd8\
+\x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xf2\xc8\
 \x00\x00\x01\x8d\xa6\xd33\xcc\
-\x00\x00J\xd6\x00\x00\x00\x00\x00\x01\x00\x16\xff\x90\
+\x00\x00J\xd6\x00\x00\x00\x00\x00\x01\x00\x16\xff\x80\
 \x00\x00\x01\x8b1\x07Lt\
-\x00\x00J\xf8\x00\x00\x00\x00\x00\x01\x00\x16\xff\xd4\
+\x00\x00J\xf8\x00\x00\x00\x00\x00\x01\x00\x16\xff\xc4\
 \x00\x00\x01\x8b1\x07L\xe3\
-\x00\x00I\x98\x00\x00\x00\x00\x00\x01\x00\x16\xe5\x05\
+\x00\x00I\x98\x00\x00\x00\x00\x00\x01\x00\x16\xe4\xf5\
 \x00\x00\x01\x8b1\x07L\x9b\
-\x00\x00K\xc4\x00\x00\x00\x00\x00\x01\x00\x17\x08\xfb\
+\x00\x00K\xc4\x00\x00\x00\x00\x00\x01\x00\x17\x08\xeb\
 \x00\x00\x01\x8b1\x07L\x5c\
-\x00\x00K\x16\x00\x01\x00\x00\x00\x01\x00\x17\x01\x97\
-\x00\x00\x01\x8fQ'\xd5\x90\
-\x00\x00H\xd4\x00\x00\x00\x00\x00\x01\x00\x16\xd3\xc7\
+\x00\x00K\x16\x00\x01\x00\x00\x00\x01\x00\x17\x01\x87\
+\x00\x00\x01\x8f\xd1\xbd5\xe9\
+\x00\x00H\xd4\x00\x00\x00\x00\x00\x01\x00\x16\xd3\xbf\
 \x00\x00\x01\x8b1\x07L{\
-\x00\x00Kz\x00\x01\x00\x00\x00\x01\x00\x17\x06>\
+\x00\x00Kz\x00\x01\x00\x00\x00\x01\x00\x17\x06.\
 \x00\x00\x01\x8b1\x07L\xdc\
-\x00\x00Il\x00\x01\x00\x00\x00\x01\x00\x16\xe3\x00\
+\x00\x00Il\x00\x01\x00\x00\x00\x01\x00\x16\xe2\xf0\
 \x00\x00\x01\x8b1\x07L+\
-\x00\x00J\x9e\x00\x00\x00\x00\x00\x01\x00\x16\xfb/\
+\x00\x00J\x9e\x00\x00\x00\x00\x00\x01\x00\x16\xfb\x1f\
 \x00\x00\x01\x8c\x00\xb0\x09_\
-\x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xc6\xf5\
+\x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xc6\xed\
 \x00\x00\x01\x8b1\x07L\xd6\
-\x00\x00I\xe2\x00\x00\x00\x00\x00\x01\x00\x16\xed\xcd\
+\x00\x00I\xe2\x00\x00\x00\x00\x00\x01\x00\x16\xed\xbd\
 \x00\x00\x01\x8b1\x07L\xbc\
-\x00\x00H\xb4\x00\x01\x00\x00\x00\x01\x00\x16\xd12\
+\x00\x00H\xb4\x00\x01\x00\x00\x00\x01\x00\x16\xd1*\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa3\
-\x00\x00J\xb6\x00\x00\x00\x00\x00\x01\x00\x16\xfd\x08\
+\x00\x00J\xb6\x00\x00\x00\x00\x00\x01\x00\x16\xfc\xf8\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa2\
-\x00\x00I,\x00\x00\x00\x00\x00\x01\x00\x16\xdf\xec\
+\x00\x00I,\x00\x00\x00\x00\x00\x01\x00\x16\xdf\xe4\
 \x00\x00\x01\x8b1\x07L\xc4\
-\x00\x00J~\x00\x00\x00\x00\x00\x01\x00\x16\xf9}\
+\x00\x00J~\x00\x00\x00\x00\x00\x01\x00\x16\xf9m\
 \x00\x00\x01\x8c\xb4\xff\xf1\x9c\
-\x00\x00L\x0a\x00\x01\x00\x00\x00\x01\x00\x17\x0b;\
+\x00\x00L\x0a\x00\x01\x00\x00\x00\x01\x00\x17\x0b+\
 \x00\x00\x01\x8b1\x07L\xb0\
-\x00\x00I\x12\x00\x01\x00\x00\x00\x01\x00\x16\xdb\x0e\
+\x00\x00I\x12\x00\x01\x00\x00\x00\x01\x00\x16\xdb\x06\
 \x00\x00\x01\x8d\xb652d\
-\x00\x00J2\x00\x00\x00\x00\x00\x01\x00\x16\xf2/\
+\x00\x00J2\x00\x00\x00\x00\x00\x01\x00\x16\xf2\x1f\
 \x00\x00\x01\x8b1\x07L\xaf\
-\x00\x00H\x9e\x00\x01\x00\x00\x00\x01\x00\x16\xcfY\
+\x00\x00H\x9e\x00\x01\x00\x00\x00\x01\x00\x16\xcfQ\
 \x00\x00\x01\x8b1\x07L\x94\
-\x00\x00G\xcc\x00\x00\x00\x00\x00\x01\x00\x16\xc8!\
+\x00\x00G\xcc\x00\x00\x00\x00\x00\x01\x00\x16\xc8\x19\
 \x00\x00\x01\x8b1\x07L1\
-\x00\x00H&\x00\x01\x00\x00\x00\x01\x00\x16\xcb$\
+\x00\x00H&\x00\x01\x00\x00\x00\x01\x00\x16\xcb\x1c\
 \x00\x00\x01\x8d\xa6\xd33\xd1\
-\x00\x00I\xc2\x00\x00\x00\x00\x00\x01\x00\x16\xe8T\
-\x00\x00\x01\x8fQ'\xd5\x8f\
-\x00\x00L$\x00\x00\x00\x00\x00\x01\x00\x17\x0c\xe0\
+\x00\x00I\xc2\x00\x00\x00\x00\x00\x01\x00\x16\xe8D\
+\x00\x00\x01\x8f\xd1\xbd5\xe0\
+\x00\x00L$\x00\x00\x00\x00\x00\x01\x00\x17\x0c\xd0\
 \x00\x00\x01\x8b1\x07Ll\
-\x00\x00H|\x00\x00\x00\x00\x00\x01\x00\x16\xcf\x10\
+\x00\x00H|\x00\x00\x00\x00\x00\x01\x00\x16\xcf\x08\
 \x00\x00\x01\x8b1\x07L\xa7\
-\x00\x00IT\x00\x01\x00\x00\x00\x01\x00\x16\xe1i\
-\x00\x00\x01\x8c\x00\xb0\x09f\
-\x00\x00H\xf2\x00\x00\x00\x00\x00\x01\x00\x16\xd7\x81\
+\x00\x00IT\x00\x01\x00\x00\x00\x01\x00\x16\xe1a\
+\x00\x00\x01\x8f\xd1\xdc\x9e\xba\
+\x00\x00H\xf2\x00\x00\x00\x00\x00\x01\x00\x16\xd7y\
 \x00\x00\x01\x8c\xb4\xff\xf1\x9c\
-\x00\x00G\xf0\x00\x00\x00\x00\x00\x01\x00\x16\xc8\xc0\
+\x00\x00G\xf0\x00\x00\x00\x00\x00\x01\x00\x16\xc8\xb8\
 \x00\x00\x01\x8b1\x07L\xa1\
-\x00\x00J\x0c\x00\x01\x00\x00\x00\x01\x00\x16\xefC\
+\x00\x00J\x0c\x00\x01\x00\x00\x00\x01\x00\x16\xef3\
 \x00\x00\x01\x8b1\x07LB\
-\x00\x00K\xe4\x00\x01\x00\x00\x00\x01\x00\x17\x09C\
-\x00\x00\x01\x8f\x00b\x17\xca\
+\x00\x00K\xe4\x00\x01\x00\x00\x00\x01\x00\x17\x093\
+\x00\x00\x01\x8fQ-y\xe5\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
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

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/screen.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/common/style_sheet.py`

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

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,30 +49,34 @@
         opacityEffect = QGraphicsOpacityEffect(self)
         self.setGraphicsEffect(opacityEffect)
         opacityAni = QPropertyAnimation(opacityEffect, b'opacity', self)
         opacityAni.setStartValue(0)
         opacityAni.setEndValue(1)
         opacityAni.setDuration(200)
         opacityAni.setEasingCurve(QEasingCurve.InSine)
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
             if e.type() == QEvent.Resize:
                 self.resize(e.size())
```

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_box_base.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/flow_layout.py`

 * *Files 9% similar despite different names*

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
     def setAnimation(self, duration, ease=QEasingCurve.Linear):
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

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_flyout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_menu.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files 6% similar despite different names*

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
         painter.drawText(QRectF(left, 0, self.width()-13-left-pr, self.height()), Qt.AlignVCenter, self.text())
 
 
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
@@ -510,15 +548,15 @@
         # draw avatar
         painter.setBrush(QBrush(self.avatar))
         painter.translate(8, 6)
         painter.drawEllipse(0, 0, 24, 24)
         painter.translate(-8, -6)
 
         if not self.isCompacted:
-            painter.setPen(Qt.white if isDarkTheme() else Qt.black)
+            painter.setPen(self.textColor())
             painter.setFont(self.font())
             painter.drawText(QRect(44, 0, 255, 36), Qt.AlignVCenter, self.name)
 
 
 @InfoBadgeManager.register(InfoBadgePosition.NAVIGATION_ITEM)
 class NavigationItemInfoBadgeManager(InfoBadgeManager):
     """ Navigation item info badge manager """
```

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/pivot.py`

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

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card.py`

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
         painter.setRenderHints(QPainter.Antialiasing)
 
         if isDarkTheme():
             painter.setBrush(QColor(255, 255, 255, 13))
             painter.setPen(QColor(0, 0, 0, 50))
```

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flip_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_badge.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self.lightBackgroundColor = None
         self.darkBackgroundColor = None
         self.manager = None  # type: InfoBadgeManager
         self.setLevel(level)
 
         setFont(self, 11)
         self.setAttribute(Qt.WA_TranslucentBackground)
+        self.setAttribute(Qt.WA_TransparentForMouseEvents)
         self.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Fixed)
         FluentStyleSheet.INFO_BADGE.apply(self)
 
     @__init__.register
     def _(self, text: str, parent: QWidget = None, level=InfoLevel.ATTENTION):
         self.__init__(parent, level)
         self.setText(text)
```

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/pips_pager.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files 7% similar despite different names*

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
         painter.setRenderHints(QPainter.Antialiasing)
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
         if orient == Qt.Vertical:
             self.setFixedWidth(12)
             self.upButton = ArrowButton(FluentIcon.CARE_UP_SOLID, self)
             self.downButton = ArrowButton(FluentIcon.CARE_DOWN_SOLID, self)
             self.setLayout(QVBoxLayout(self))
             self.layout().addWidget(self.upButton, 0, Qt.AlignHCenter)
             self.layout().addStretch(1)
@@ -46,41 +54,55 @@
             self.downButton = ArrowButton(FluentIcon.CARE_RIGHT_SOLID, self)
             self.setLayout(QHBoxLayout(self))
             self.layout().addWidget(self.upButton, 0, Qt.AlignVCenter)
             self.layout().addStretch(1)
             self.layout().addWidget(self.downButton, 0, Qt.AlignVCenter)
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
         painter.setRenderHints(QPainter.Antialiasing)
+        painter.setOpacity(self.opacity)
         painter.setPen(Qt.NoPen)
 
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
+    opacity = Property(float, getOpacity, setOpacity)
+
 
 class ScrollBarHandle(QWidget):
     """ Scroll bar handle """
 
     def __init__(self, orient: Qt.Orientation, parent=None):
         super().__init__(parent)
         self.orient = orient
@@ -369,15 +391,15 @@
     def _isSlideResion(self, pos: QPoint):
         if self.orientation() == Qt.Vertical:
             return self._padding <= pos.y() <= self.height() - self._padding
 
         return self._padding <= pos.x() <= self.width() - self._padding
 
     def _onOpacityAniValueChanged(self):
-        opacity = self.groove.opacityEffect.opacity()
+        opacity = self.groove.opacity
         if self.orientation() == Qt.Vertical:
             self.handle.setFixedWidth(int(3 + opacity * 3))
         else:
             self.handle.setFixedHeight(int(3 + opacity * 3))
 
         self._adjustHandlePos()
 
@@ -497,15 +519,26 @@
             parent.horizontalScrollBar().setStyleSheet("QScrollBar:horizontal{height: 0px}")
 
         parent.viewport().installEventFilter(self)
         parent.setVerticalScrollBarPolicy = self.setVerticalScrollBarPolicy
         parent.setHorizontalScrollBarPolicy = self.setHorizontalScrollBarPolicy
 
     def eventFilter(self, obj, e: QEvent):
-        if e.type() == QEvent.Wheel:
+        if e.type() == QEvent.Type.Wheel:
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

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_play_bar.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_player.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/video_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py` & `PySide2-Fluent-Widgets-1.5.7/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide2-Fluent-Widgets-1.5.6/setup.py` & `PySide2-Fluent-Widgets-1.5.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Fluent-Widgets",
-    version="1.5.6",
+    version="1.5.7",
     keywords="pyside2 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PySide2",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

