# Comparing `tmp/PySide6-Fluent-Widgets-1.5.6.tar.gz` & `tmp/PySide6-Fluent-Widgets-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide6-Fluent-Widgets-1.5.6.tar", last modified: Tue May  7 03:43:54 2024, max compression
+gzip compressed data, was "dist\PySide6-Fluent-Widgets-1.5.7.tar", last modified: Sat Jun  1 03:30:45 2024, max compression
```

## Comparing `PySide6-Fluent-Widgets-1.5.6.tar` & `PySide6-Fluent-Widgets-1.5.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.214608 PySide6-Fluent-Widgets-1.5.6/
--rw-rw-rw-   0        0        0    35823 2024-05-07 03:40:07.000000 PySide6-Fluent-Widgets-1.5.6/LICENSE
--rw-rw-rw-   0        0        0     5360 2024-05-07 03:43:54.214095 PySide6-Fluent-Widgets-1.5.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.022369 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     5360 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4929 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 03:43:53.000000 PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4576 2024-05-07 03:40:41.000000 PySide6-Fluent-Widgets-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.023535 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/
--rw-rw-rw-   0        0        0      566 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.029018 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  3307368 2024-05-07 03:41:23.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.058560 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0    15208 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1589 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py
--rw-rw-rw-   0        0        0    11172 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      807 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    13725 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     5554 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0      664 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py
--rw-rw-rw-   0        0        0     4862 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    14471 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      454 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.065571 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.076755 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2569 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21813 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7630 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19331 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     6406 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.088949 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14892 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5896 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11413 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3179 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2873 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py
--rw-rw-rw-   0        0        0     2425 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.095022 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2716 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     7104 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1305 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.107119 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/
--rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py
--rw-rw-rw-   0        0        0     3129 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py
--rw-rw-rw-   0        0        0     3542 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py
--rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py
--rw-rw-rw-   0        0        0     6778 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py
--rw-rw-rw-   0        0        0     1187 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py
--rw-rw-rw-   0        0        0     1310 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.123019 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     9940 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py
--rw-rw-rw-   0        0        0    12954 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8771 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    24105 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    19679 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6823 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     5205 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.136873 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5280 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0    11031 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     4644 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2841 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    14031 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1590 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.197817 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     3316 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     8061 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    29986 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     7688 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     5808 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    16342 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19812 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     7934 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    13111 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py
--rw-rw-rw-   0        0        0    17080 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2229 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1496 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16653 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    18932 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0    14700 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    14221 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4579 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    40995 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0    11197 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py
--rw-rw-rw-   0        0        0     9173 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     7029 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2720 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17861 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     1167 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py
--rw-rw-rw-   0        0        0    10310 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     8637 2024-05-07 03:40:18.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6535 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5854 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8597 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    26330 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py
--rw-rw-rw-   0        0        0    11774 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    22912 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10581 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     4555 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.204023 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/
--rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/__init__.py
--rw-rw-rw-   0        0        0    11597 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py
--rw-rw-rw-   0        0        0     3887 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py
--rw-rw-rw-   0        0        0     2849 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:43:54.208601 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    12940 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2827 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1660 2024-05-07 03:40:08.000000 PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2024-05-07 03:43:54.214608 PySide6-Fluent-Widgets-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1219 2024-05-07 03:40:52.000000 PySide6-Fluent-Widgets-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.657948 PySide6-Fluent-Widgets-1.5.7/
+-rw-rw-rw-   0        0        0    35823 2024-06-01 03:22:17.000000 PySide6-Fluent-Widgets-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0     5360 2024-06-01 03:30:45.656476 PySide6-Fluent-Widgets-1.5.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.446273 PySide6-Fluent-Widgets-1.5.7/PySide6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5360 2024-06-01 03:30:45.000000 PySide6-Fluent-Widgets-1.5.7/PySide6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4929 2024-06-01 03:30:45.000000 PySide6-Fluent-Widgets-1.5.7/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 03:30:45.000000 PySide6-Fluent-Widgets-1.5.7/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-06-01 03:30:45.000000 PySide6-Fluent-Widgets-1.5.7/PySide6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 03:30:45.000000 PySide6-Fluent-Widgets-1.5.7/PySide6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4576 2024-06-01 03:22:17.000000 PySide6-Fluent-Widgets-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.447720 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/
+-rw-rw-rw-   0        0        0      566 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.451876 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  3307454 2024-06-01 03:23:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.486725 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0    15208 2024-06-01 03:22:17.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1589 2024-06-01 03:22:17.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/color.py
+-rw-rw-rw-   0        0        0    11177 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      807 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    13725 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     5554 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0      664 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/screen.py
+-rw-rw-rw-   0        0        0     4862 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    14476 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      454 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.488846 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.501875 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2569 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21813 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7630 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19331 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     6406 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.515144 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14892 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5896 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11413 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3288 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2873 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_box_base.py
+-rw-rw-rw-   0        0        0     2425 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.523818 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2716 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     7529 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1305 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.536781 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/
+-rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/__init__.py
+-rw-rw-rw-   0        0        0     3129 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_combo_box.py
+-rw-rw-rw-   0        0        0     3542 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_flyout.py
+-rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_line_edit.py
+-rw-rw-rw-   0        0        0     6778 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_menu.py
+-rw-rw-rw-   0        0        0     1187 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_tool_tip.py
+-rw-rw-rw-   0        0        0     1310 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.553370 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     9940 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/breadcrumb.py
+-rw-rw-rw-   0        0        0    12954 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8771 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    24105 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    20922 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6994 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     5205 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.566959 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5280 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0    11031 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     4644 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2841 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    14179 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1590 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.640572 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     3316 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8061 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    29986 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     7688 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     5808 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    16342 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19812 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     7934 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    13111 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flip_view.py
+-rw-rw-rw-   0        0        0    17080 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2229 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1496 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16713 2024-06-01 03:22:27.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    18932 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0    14700 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    14221 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4579 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    40995 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0    11197 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/pips_pager.py
+-rw-rw-rw-   0        0        0     9173 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     7029 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2720 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    19093 2024-06-01 03:23:55.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     1167 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/separator.py
+-rw-rw-rw-   0        0        0    10310 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     8637 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6535 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5854 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8597 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    26330 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tab_view.py
+-rw-rw-rw-   0        0        0    11774 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    22912 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10581 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     4555 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.647759 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/
+-rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/__init__.py
+-rw-rw-rw-   0        0        0    11597 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_play_bar.py
+-rw-rw-rw-   0        0        0     3887 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_player.py
+-rw-rw-rw-   0        0        0     2849 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/video_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:30:45.655444 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    12940 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2827 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1660 2024-06-01 03:22:18.000000 PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 03:30:45.657948 PySide6-Fluent-Widgets-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2024-06-01 03:23:04.000000 PySide6-Fluent-Widgets-1.5.7/setup.py
```

### Comparing `PySide6-Fluent-Widgets-1.5.6/LICENSE` & `PySide6-Fluent-Widgets-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/PKG-INFO` & `PySide6-Fluent-Widgets-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 1.5.6
+Version: 1.5.7
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.6 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.7 Summary: A
 fluent design widgets library based on PySide6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyside6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
```

### Comparing `PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/PKG-INFO` & `PySide6-Fluent-Widgets-1.5.7/PySide6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 1.5.6
+Version: 1.5.7
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.6 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 1.5.7 Summary: A
 fluent design widgets library based on PySide6 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Project-URL: Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues
 Keywords: pyside6 fluent widgets Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
```

### Comparing `PySide6-Fluent-Widgets-1.5.6/PySide6_Fluent_Widgets.egg-info/SOURCES.txt` & `PySide6-Fluent-Widgets-1.5.7/PySide6_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/README.md` & `PySide6-Fluent-Widgets-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6/examples.
 
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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -94419,42 +94419,42 @@
 8\xdb\xf3\xf9x\xba9t\xb5~\xb4\xc3\x87\x86\xd7\x89\
 \x13]/\xeas\xf0\xffJx_\x03\xc1\xa0I\xec\x1a\
 \xae!\xc1\xe5^\x9b\x8a2\xaa\xd5\xc7\xa0\x01E\xf7T\
 MI\xe9\x1a\xe9\xc6\xf4\xd0F8v\x03pC\xaaj\
 \xe0\xd5\x9a\x22\x90\xb6C\x1f\x9e\xf80\xd9\xd9\x8a\xcb\x00\
 \x1eSb\x89j\x9cn\xcf\x0f+2%\xa8\x15\xffJ\
 \x11\xf3O\xa3\x15u<\x7f\x00~\xba\xcf\xa4\
-\x00\x00\x01\x9e\
+\x00\x00\x01\x96\
 \x00\
-\x00\x06\xf2x\xda\x9dU\xd1n\x820\x14}7\xf1\x1f\
-\x9a\xece$\xba\x80\x0a*\xcb>\xc07\x13\x97\xeca\
-\xd9C\xa1WlVZ\xd2\x16g\xb2\xf8\xefk\x14T\
-\xa0J3B\x03\xedmO\xcf\xe5\x9c[\xd6t/\xf4\
-JC\x8e~\x87\x03d\xae\x02\x13By\x16\xa3\xc0/\
-\x0e(\x98\x14\x87\xd7s \x15L\xc8\x18%\x0c\xa7\xdf\
-\xd5Pb^3)JN\xc6UTK\xccU\x81%\
-p]\xcf\x11\x92\x80\x89p\xc1\xa1\x1a\x12\xa5f\x94C\
-c,\xc72\xa3<F\xbe\xe9\x1f\x87\x83\xe1`]\x13\
-\xfb\xa4j\x03\x0cR\x0d\xe4M\xcb\x12\xbe\xe2\x9d\xd8\x83\
-\xac\xf9V\x1b\xcb,\xc1\xcf\xfe\x08U\xf7K4\xf5\x1c\
-\x90\x0a\x09J\x01\xe9\xc1\x0a{\xb0\xb6\x98)g\xb0y\
-h\x01\xdba\xb5J\x05\xaf\x90ZR\x8c\x19lu|\
-+E\x1d\x904\xdb]#w0O\x99\xda!\xa7\x91\
-3d\x0d`\x91\xb3\xcf\x05'\x90\xa7=\x85\x9f\x0b\x88\
-\xcb\x8a\x0dd\xb9\xe9\x02y\x17\x82Y\x1d\x1a\x1a\x83.\
-M3Y\xa0\xc5\x95\xefe\xe1\x07%\x19\xe8\x11j \
-\x9d\x07\xef3i\xeb\xe5Of\x81\xd7\xf2r`6T\
-\x82Q\xd2\x9d\x1d\xce\x17\xcd\xd9c\x89\x09-U\x8c\x22\
-\x0bC\xbb\x93F\x96\xe4\xbb\xb3\xda\x92jQ\x18E;\
-\x82&Bk\x91\xdfF\xfeY\xb5\xd6tnK\xd7\xec\
-\x80&\xceI\x9e\xab\xd8-\xd5f\xc5\xf7i\xb6\xf4\x5c\
-)T\x15\xebH\xa2U\xdf}4\x22\xcf\xf2}f\xa6\
-U\xcf^\x92\xa7\xc2\xed\xe3f\xad\xee\x93\x15\xa2\xbbV\
-\xe8J\xe7;\x9b\xc3\x81rW\xd9\x87\x87\xafS\x86n\
-nyt\xa8\xd7\xff\xad\xe3\x1f%P0\x22\
+\x00\x06\xd4x\xda\x9dU\xd1j\xc20\x14}\x17\xfc\x87\
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
+\xd5\xad\xfe-\xc5\x0eo\x8a\xdd\x15\xc7s\x96\xdf\x81r\
+W\xbb\xbb\xc7\xabS\x87n\xf3p\xef\xd8\xae\xffL\xc7\
+\x7f\xac\x0e'\xa8\
 \x00\x00\x03\xb6\
 I\
 nfoBar {\x0d\x0a    bo\
 rder: 1px solid \
 rgb(29, 29, 29);\
 \x0d\x0a    border-rad\
 ius: 6px;\x0d\x0a    b\
@@ -95682,42 +95682,41 @@
 \xc7\x95\x96\xbf\x9f\x19>\x1cLZf\x8e7\xbfc\xda\
 \xc4\xa4\xfd\xbf\xd1\xddM>\x88\xa1\x18]\x03\xd43\x9b\
 WR\xcd\x91\xc1\x8c>\x05\x0a\x9arO\xc4\x1c\x5c>\
 4T\x8b1m\x0d\xfb\xa2,\xfb6\x9e2\xe2\x09q\
 \x81\x1aWA\x8f\xcf \x8c\x07\x84\xd4\xf2\x9c\xaeL\xa4\
 3\xa4\xd5?\xe6\xe3C.Z\xce\xe7\xb3\x03h\xb4\xd4\
 \xf9\xfc\x01\x1b{\xca\xd9\
-\x00\x00\x01\x92\
+\x00\x00\x01\x8a\
 \x00\
-\x00\x06Ux\xda\xa5T]k\x830\x14}/\xf4?\
-\x04\xf62\xc1\x16m\xa7k\x1d\xfb\x01}+t\xb0\x87\
-\xb1\x87\xd4\xdcj\x98&\x92\xc4\xb60\xf6\xdf\x97\xf9\xd1\
-n\x1a1\xdb\xc4(\xe6\xe4\x9e\x9c\xeb\xb97[z\xe4\
-j\xa3 G\xef\xd3\x09\xd2W\x81\x09\xa1,\x89\x90\xef\
-\x15g\xe4/\x8a\xf3C\x0d\xc4<\xe3\x22B\xa7\x94*\
-h\xa6\xf68~K\x04/\x19\x995\xa8\x12\x98\xc9\x02\
-\x0b`\xaa]\xc3\x05\x01\x8d0\xce\xda0^\xaa\x8c2\
-\xb8\xcc}L'\xd3\xc9\xb6\x15\xf2B\xe5\x0e2\x88\x15\
-\x90G%Jx\x8dR~\x04\xd1\xeak6\x12\xc9\x1e\
-\xdf.\x82\xc0E\xd7\x877\x0f\x97\x8e\x05_!@J\
- V\x8c\xc1\x08\xe3\x01g\xf2\x97\x94\xf7\x81\x812\xc5\
-r\x13s\xd6\xf0u\xcc\x98epP\xd1w3Z@\
-\xd0$\xbd\x22\x03\x9cU\xd6f\xcaehM\xd9\x12\x18\
-\x0c\x1d\xab\x83\x8a\xe4\xe6H\xe1t!\xb1\x89\xd8A\x92\
-\xebO O\x9cg\xc6\x1a\x0dt\x89\xae\xf5\xd0Y\xa0\
-\xd5U\xef%\xf0\x99\x92\x04\x94\xdb\xa1\xaag\x87\xa5T\
-\xb6y\xda\xaa\xfa\x9e\xfbN\xa7\x96}\xbd\x9d\xe4\x19%\
-\x03\x0e{\xab\x9f\x113\x81\x09-e\x84B\x83Fs\
-E\xb9\xa8\x97}\x7fQ\xd7S\xc5\x0bmi\xcf\xd1=\
-W\x8a\xe7\xdf\x91?6\xae1\x9b/ \xc7\x22\xa1\xac\
-\xda\x01-\xacs\xac\x1b\xdb5\x18=\xb4v\xc4\xb3\x8e\
-\x11k\xc7VH\xd3\xbe\x96R:\xcdn'&t\x0c\
-\xff\xeaN\x8f\xe6=*\xb5\xea\xe21\x85\xc6V\xaf\xca\
-\x22\x1c,\x8b\xbe\x8d\xde\x7f\x0e}\x9d\xc5'\x17\x15\xf3\
-\x1c\
+\x00\x067x\xda\xa5\x94\xdfj\x830\x14\xc6\xef\x0b}\
+\x87\xc0nV\xb0E[t\xadc\x0f\xd0\xbbB\x07\xbb\
+\x18\xbbH\xcd\xa9\x86i\x22Il\x0bc\xef\xbe\xcc\x7f\
+\xed4b\xb6\x89\x0a\xe6\xe4|\xf9\x0e\xbfs\xdc\xd1\x13\
+W[\x05\x19\xfa\x98N\x90\xberL\x08eq\x88<\
+7\xbf o\x99_\x1e\xab@\xc4S.BtN\xa8\
+\x82z\xe9\x80\xa3\xf7X\xf0\x82\x91y\x1dU\x023\x99\
+c\x01L5{\xb8 \xa0#\x8c\xb3&\x8d\x17*\xa5\
+\x0c\xda\xb5\xcf\xe9d:\xd95F^\xa9\xdcC\x0a\x91\
+\x02\xf2\xa4D\x01oa\xc2O \x1a\x7f\xf5A\x22>\
+\xe0\xfb\xa5\xef;\xe8\xfar\x17\xc1jf\xa1\x97\x0b\x90\
+\x12\x88\x95\xa2?\xa2x\xc4\xa9\xfc\xa5\xe4\x83o\x90L\
+\xb0\xdcF\x9c\xd5z\x1d\x18\xf3\x14\x8e*\xbc\x85\xd1\x04\
+\x04\x8d\x93kd@\xb3\xac\xda,\xb9\x0a\xac%\x1b\x01\
+\x03\xd0\xb1>(E\xeeN\x14\xce\xad\x88M\xc6\x1e\xe2\
+L\x7f\x02y\xe6<5\xf6\xa8\xaf[t\xa3\x1f]\x05\
+Z_\xfd\xb6\x89/\x94\xc4\xa0\x9c\x8eT\xb5:l\xa5\
+\xc4\xe6jT\xd5\xbd\xf0f\x9d^\xf6\xf4q\x92\xa7\x94\
+\x0c\x10v\xd7?3\xe6\x02\x13Z\xc8\x10\x05\x06\x8f\xe6\
+\x8erP\xaf\xfa\xfe\xa6.S\xc5s\x8d\xb4G\xf4\xc0\
+\x95\xe2\xd9m\xe4\x8f\x83k\xac\xe6;\x90a\x11SV\
+\x9e\x80\x5c\xeb\x1a\xab\xc1v\x0c\xa0\x87\xf6\x8e0\xeb\x80\
+\xd8\xccl\x8d\xd4\xe3ki\xa53\xecvf\x82q3\
+\xe5\x9c\x8ey0\x0es\x09>\x18\x04\xdf\x07\xe5\xfe\xe7\
+\xb7\xae\xab\xf8\x02\xf9\xbe\xea\xa2\
 "
 
 qt_resource_name = b"\
 \x00\x0e\
 \x07\x8dJ3\
 \x00q\
 \x00f\x00l\x00u\x00e\x00n\x00t\x00w\x00i\x00d\x00g\x00e\x00t\x00s\
@@ -98908,15 +98907,15 @@
 \x00\x00H\xac\x00\x00\x00\x00\x00\x01\x00\x16\x9a\x94\
 \x00\x00\x01\x8b1\x07M\x97\
 \x00\x00K\x0e\x00\x00\x00\x00\x00\x01\x00\x16\xb7\x12\
 \x00\x00\x01\x8b1\x07MW\
 \x00\x00I\x88\x00\x00\x00\x00\x00\x01\x00\x16\xa54\
 \x00\x00\x01\x8b1\x07M\x1d\
 \x00\x00I \x00\x01\x00\x00\x00\x01\x00\x16\xa1\xf5\
-\x00\x00\x01\x8fQ#I\xf6\
+\x00\x00\x01\x8f\xd1\xbd5\xf3\
 \x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\x85\xe5\
 \x00\x00\x01\x8b1\x07M:\
 \x00\x00I\xfe\x00\x01\x00\x00\x00\x01\x00\x16\xa9x\
 \x00\x00\x01\x8b1\x07M\x8f\
 \x00\x00K\xec\x00\x01\x00\x00\x00\x01\x00\x16\xc3\xe9\
 \x00\x00\x01\x8b1\x07L\xf6\
 \x00\x00K\xb4\x00\x00\x00\x00\x00\x01\x00\x16\xc0d\
@@ -98942,97 +98941,97 @@
 \x00\x00H\x96\x00\x01\x00\x00\x00\x01\x00\x16\x98\xac\
 \x00\x00\x01\x8bf\xa8\x0a\xf2\
 \x00\x00I>\x00\x00\x00\x00\x00\x01\x00\x16\xa4'\
 \x00\x00\x01\x8b1\x07L\xfc\
 \x00\x00KX\x00\x01\x00\x00\x00\x01\x00\x16\xbc\xdb\
 \x00\x00\x01\x8d\xa6\xd33\xe2\
 \x00\x00G\xc4\x00\x00\x00\x00\x00\x01\x00\x16\x89\xa5\
-\x00\x00\x01\x8fQ#I\xf4\
+\x00\x00\x01\x8f\xd1\xbd5\xee\
 \x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xb0u\
 \x00\x00\x01\x8b1\x07M,\
 \x00\x00H\x0e\x00\x00\x00\x00\x00\x01\x00\x16\x90T\
 \x00\x00\x01\x8b1\x07M^\
 \x00\x00L>\x00\x01\x00\x00\x00\x01\x00\x16\xc8\xdf\
-\x00\x00\x01\x8c\x00\xb0\x09\x8d\
+\x00\x00\x01\x8f\xd1\xd1\xed\x9b\
 \x00\x00I\x00\x00\x00\x00\x00\x00\x01\x00\x16\x9e\x9e\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa9\
 \x00\x00H\xca\x00\x00\x00\x00\x00\x01\x00\x16\x9c2\
 \x00\x00\x01\x8b1\x07M^\
 \x00\x00L\x18\x00\x01\x00\x00\x00\x01\x00\x16\xc5\xed\
 \x00\x00\x01\x8b1\x07M\x08\
 \x00\x00HJ\x00\x01\x00\x00\x00\x01\x00\x16\x95\x88\
 \x00\x00\x01\x8d\xa6\xd33\xe7\
-\x00\x00J\xf0\x00\x00\x00\x00\x00\x01\x00\x17\x00\xbb\
+\x00\x00J\xf0\x00\x00\x00\x00\x00\x01\x00\x17\x00\xb3\
 \x00\x00\x01\x8b1\x07L\xca\
-\x00\x00J\x22\x00\x01\x00\x00\x00\x01\x00\x16\xf5\x9c\
+\x00\x00J\x22\x00\x01\x00\x00\x00\x01\x00\x16\xf5\x94\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa3\
-\x00\x00Ib\x00\x00\x00\x00\x00\x01\x00\x16\xea\x0f\
+\x00\x00Ib\x00\x00\x00\x00\x00\x01\x00\x16\xea\x07\
 \x00\x00\x01\x8b1\x07L\x8e\
-\x00\x00K\x8c\x00\x01\x00\x00\x00\x01\x00\x17\x08\xe5\
+\x00\x00K\x8c\x00\x01\x00\x00\x00\x01\x00\x17\x08\xdd\
 \x00\x00\x01\x8c\x01\x8b~\xfb\
-\x00\x00I\xa8\x00\x00\x00\x00\x00\x01\x00\x16\xea\xc5\
+\x00\x00I\xa8\x00\x00\x00\x00\x00\x01\x00\x16\xea\xbd\
 \x00\x00\x01\x8d\xa6\xd33\xcc\
-\x00\x00I\xdc\x00\x00\x00\x00\x00\x01\x00\x16\xf3\x09\
+\x00\x00I\xdc\x00\x00\x00\x00\x00\x01\x00\x16\xf3\x01\
 \x00\x00\x01\x8b1\x07Lt\
-\x00\x00H\xac\x00\x00\x00\x00\x00\x01\x00\x16\xdfB\
+\x00\x00H\xac\x00\x00\x00\x00\x00\x01\x00\x16\xdf:\
 \x00\x00\x01\x8b1\x07L\xe3\
-\x00\x00K\x0e\x00\x00\x00\x00\x00\x01\x00\x17\x013\
+\x00\x00K\x0e\x00\x00\x00\x00\x00\x01\x00\x17\x01+\
 \x00\x00\x01\x8b1\x07L\x9b\
-\x00\x00I\x88\x00\x00\x00\x00\x00\x01\x00\x16\xea}\
+\x00\x00I\x88\x00\x00\x00\x00\x00\x01\x00\x16\xeau\
 \x00\x00\x01\x8b1\x07L\x5c\
-\x00\x00I \x00\x01\x00\x00\x00\x01\x00\x16\xe6\xf6\
-\x00\x00\x01\x8fQ#I\xf4\
-\x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xca\x81\
+\x00\x00I \x00\x01\x00\x00\x00\x01\x00\x16\xe6\xee\
+\x00\x00\x01\x8f\xd1\xbd5\xe9\
+\x00\x00G\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xcay\
 \x00\x00\x01\x8b1\x07L{\
-\x00\x00I\xfe\x00\x01\x00\x00\x00\x01\x00\x16\xf3M\
+\x00\x00I\xfe\x00\x01\x00\x00\x00\x01\x00\x16\xf3E\
 \x00\x00\x01\x8b1\x07L\xdc\
-\x00\x00K\xec\x00\x01\x00\x00\x00\x01\x00\x17\x0e%\
+\x00\x00K\xec\x00\x01\x00\x00\x00\x01\x00\x17\x0e\x1d\
 \x00\x00\x01\x8b1\x07L+\
-\x00\x00K\xb4\x00\x00\x00\x00\x00\x01\x00\x17\x0a\x9a\
+\x00\x00K\xb4\x00\x00\x00\x00\x00\x01\x00\x17\x0a\x92\
 \x00\x00\x01\x8c\x00\xb0\x09_\
-\x00\x00Hp\x00\x00\x00\x00\x00\x01\x00\x16\xdc@\
+\x00\x00Hp\x00\x00\x00\x00\x00\x01\x00\x16\xdc8\
 \x00\x00\x01\x8b1\x07L\xd6\
-\x00\x00G\xe4\x00\x00\x00\x00\x00\x01\x00\x16\xd3\xb4\
+\x00\x00G\xe4\x00\x00\x00\x00\x00\x01\x00\x16\xd3\xac\
 \x00\x00\x01\x8b1\x07L\xbc\
-\x00\x00K8\x00\x01\x00\x00\x00\x01\x00\x17\x04\x82\
+\x00\x00K8\x00\x01\x00\x00\x00\x01\x00\x17\x04z\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa3\
-\x00\x00JD\x00\x00\x00\x00\x00\x01\x00\x16\xf7\xb9\
+\x00\x00JD\x00\x00\x00\x00\x00\x01\x00\x16\xf7\xb1\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa2\
-\x00\x00J\x96\x00\x00\x00\x00\x00\x01\x00\x16\xfe\x95\
+\x00\x00J\x96\x00\x00\x00\x00\x00\x01\x00\x16\xfe\x8d\
 \x00\x00\x01\x8b1\x07L\xc4\
-\x00\x00K\xcc\x00\x00\x00\x00\x00\x01\x00\x17\x0cs\
+\x00\x00K\xcc\x00\x00\x00\x00\x00\x01\x00\x17\x0ck\
 \x00\x00\x01\x8c\xb4\xff\xf1\x9c\
-\x00\x00I\xc2\x00\x01\x00\x00\x00\x01\x00\x16\xf1j\
+\x00\x00I\xc2\x00\x01\x00\x00\x00\x01\x00\x16\xf1b\
 \x00\x00\x01\x8b1\x07L\xb0\
-\x00\x00H0\x00\x01\x00\x00\x00\x01\x00\x16\xd5s\
+\x00\x00H0\x00\x01\x00\x00\x00\x01\x00\x16\xd5k\
 \x00\x00\x01\x8d\xb652d\
-\x00\x00J\xbe\x00\x00\x00\x00\x00\x01\x00\x17\x00\x12\
+\x00\x00J\xbe\x00\x00\x00\x00\x00\x01\x00\x17\x00\x0a\
 \x00\x00\x01\x8b1\x07L\xaf\
-\x00\x00H\x96\x00\x01\x00\x00\x00\x01\x00\x16\xddl\
+\x00\x00H\x96\x00\x01\x00\x00\x00\x01\x00\x16\xddd\
 \x00\x00\x01\x8b1\x07L\x94\
-\x00\x00I>\x00\x00\x00\x00\x00\x01\x00\x16\xe9p\
+\x00\x00I>\x00\x00\x00\x00\x00\x01\x00\x16\xe9h\
 \x00\x00\x01\x8b1\x07L1\
-\x00\x00KX\x00\x01\x00\x00\x00\x01\x00\x17\x07\x16\
+\x00\x00KX\x00\x01\x00\x00\x00\x01\x00\x17\x07\x0e\
 \x00\x00\x01\x8d\xa6\xd33\xd1\
-\x00\x00G\xc4\x00\x00\x00\x00\x00\x01\x00\x16\xce;\
-\x00\x00\x01\x8fQ#I\xf3\
-\x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xfaA\
+\x00\x00G\xc4\x00\x00\x00\x00\x00\x01\x00\x16\xce3\
+\x00\x00\x01\x8f\xd1\xbd5\xe0\
+\x00\x00Jd\x00\x00\x00\x00\x00\x01\x00\x16\xfa9\
 \x00\x00\x01\x8b1\x07Ll\
-\x00\x00H\x0e\x00\x00\x00\x00\x00\x01\x00\x16\xd5*\
+\x00\x00H\x0e\x00\x00\x00\x00\x00\x01\x00\x16\xd5\x22\
 \x00\x00\x01\x8b1\x07L\xa7\
-\x00\x00L>\x00\x01\x00\x00\x00\x01\x00\x17\x13\x15\
-\x00\x00\x01\x8c\x00\xb0\x09f\
-\x00\x00I\x00\x00\x00\x00\x00\x00\x01\x00\x16\xe3i\
+\x00\x00L>\x00\x01\x00\x00\x00\x01\x00\x17\x13\x0d\
+\x00\x00\x01\x8f\xd1\xd1\xed\x99\
+\x00\x00I\x00\x00\x00\x00\x00\x00\x01\x00\x16\xe3a\
 \x00\x00\x01\x8c\xb4\xff\xf1\x9c\
-\x00\x00H\xca\x00\x00\x00\x00\x00\x01\x00\x16\xe1\x05\
+\x00\x00H\xca\x00\x00\x00\x00\x00\x01\x00\x16\xe0\xfd\
 \x00\x00\x01\x8b1\x07L\xa1\
-\x00\x00L\x18\x00\x01\x00\x00\x00\x01\x00\x17\x10)\
+\x00\x00L\x18\x00\x01\x00\x00\x00\x01\x00\x17\x10!\
 \x00\x00\x01\x8b1\x07LB\
-\x00\x00HJ\x00\x01\x00\x00\x00\x01\x00\x16\xdaJ\
-\x00\x00\x01\x8f\x00b\x17\xca\
+\x00\x00HJ\x00\x01\x00\x00\x00\x01\x00\x16\xdaB\
+\x00\x00\x01\x8fQ-y\xe5\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/config.py`

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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/screen.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/common/style_sheet.py`

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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files 4% similar despite different names*

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
                 re = QResizeEvent(e)
```

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_box_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/flow_layout.py`

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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_flyout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_widget.py`

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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/pivot.py`

 * *Files 3% similar despite different names*

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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card.py`

 * *Files 0% similar despite different names*

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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flip_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_badge.py`

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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/pips_pager.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files 6% similar despite different names*

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

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_play_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_player.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/video_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py` & `PySide6-Fluent-Widgets-1.5.7/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-1.5.6/setup.py` & `PySide6-Fluent-Widgets-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide6-Fluent-Widgets",
-    version="1.5.6",
+    version="1.5.7",
     keywords="pyside6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PySide6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

