# Comparing `tmp/PyQt-Fluent-Widgets-1.5.6.tar.gz` & `tmp/PyQt-Fluent-Widgets-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt-Fluent-Widgets-1.5.6.tar", last modified: Tue May  7 03:23:00 2024, max compression
+gzip compressed data, was "dist\PyQt-Fluent-Widgets-1.5.7.tar", last modified: Sat Jun  1 03:54:32 2024, max compression
```

## Comparing `PyQt-Fluent-Widgets-1.5.6.tar` & `PyQt-Fluent-Widgets-1.5.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.272001 PyQt-Fluent-Widgets-1.5.6/
--rw-rw-rw-   0        0        0    35825 2024-05-04 07:38:18.000000 PyQt-Fluent-Widgets-1.5.6/LICENSE
--rw-rw-rw-   0        0        0     5554 2024-05-07 03:23:00.270993 PyQt-Fluent-Widgets-1.5.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.028885 PyQt-Fluent-Widgets-1.5.6/PyQt_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     5554 2024-05-07 03:22:59.000000 PyQt-Fluent-Widgets-1.5.6/PyQt_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4914 2024-05-07 03:22:59.000000 PyQt-Fluent-Widgets-1.5.6/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:22:59.000000 PyQt-Fluent-Widgets-1.5.6/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2024-05-07 03:22:59.000000 PyQt-Fluent-Widgets-1.5.6/PyQt_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 03:22:59.000000 PyQt-Fluent-Widgets-1.5.6/PyQt_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4791 2024-05-07 03:19:21.000000 PyQt-Fluent-Widgets-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.031406 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/
--rw-rw-rw-   0        0        0      549 2024-05-07 03:20:06.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.035941 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  6502800 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.085977 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0    15238 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0     1587 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py
--rw-rw-rw-   0        0        0    11192 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      803 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    13751 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     5537 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3866 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0      658 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py
--rw-rw-rw-   0        0        0     4851 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0    14407 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      452 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.088976 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.101999 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2581 2024-05-07 03:07:09.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21800 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7629 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19337 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     6439 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.117659 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14788 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5860 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11337 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3173 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2879 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py
--rw-rw-rw-   0        0        0     2500 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.128178 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2750 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     7112 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1301 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.147610 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/
--rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py
--rw-rw-rw-   0        0        0     3006 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py
--rw-rw-rw-   0        0        0     3536 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py
--rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py
--rw-rw-rw-   0        0        0     6276 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py
--rw-rw-rw-   0        0        0     1181 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py
--rw-rw-rw-   0        0        0     1431 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.167008 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     9961 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py
--rw-rw-rw-   0        0        0    12968 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8773 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    24107 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    19705 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6825 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     5211 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.183946 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5282 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0    11031 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     4648 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2843 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    14036 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1586 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.252030 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     3328 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     8063 2024-05-05 11:22:36.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    30016 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     7700 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     5802 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    15825 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0    19594 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py
--rw-rw-rw-   0        0        0     7881 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0    13091 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py
--rw-rw-rw-   0        0        0    17086 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py
--rw-rw-rw-   0        0        0     2223 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1498 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    16647 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py
--rw-rw-rw-   0        0        0    18934 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0    14724 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    14139 2024-05-04 07:47:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     4812 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    40458 2024-05-07 03:16:04.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0    11189 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py
--rw-rw-rw-   0        0        0     9199 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     7033 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2718 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17887 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     1204 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py
--rw-rw-rw-   0        0        0    10220 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     8629 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6534 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5790 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8631 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0    26348 2024-05-04 07:38:19.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py
--rw-rw-rw-   0        0        0    11538 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    22906 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10563 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     4484 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.260630 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/
--rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/__init__.py
--rw-rw-rw-   0        0        0    11617 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py
--rw-rw-rw-   0        0        0     3585 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py
--rw-rw-rw-   0        0        0     2845 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:23:00.268383 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/window/
--rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    12934 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     2846 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py
--rw-rw-rw-   0        0        0     1664 2024-05-04 07:38:20.000000 PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2024-05-07 03:23:00.272001 PyQt-Fluent-Widgets-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1193 2024-05-07 03:19:53.000000 PyQt-Fluent-Widgets-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.923010 PyQt-Fluent-Widgets-1.5.7/
+-rw-rw-rw-   0        0        0    35825 2024-06-01 03:41:39.000000 PyQt-Fluent-Widgets-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0     5554 2024-06-01 03:54:32.922009 PyQt-Fluent-Widgets-1.5.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.714746 PyQt-Fluent-Widgets-1.5.7/PyQt_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     5554 2024-06-01 03:54:32.000000 PyQt-Fluent-Widgets-1.5.7/PyQt_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4914 2024-06-01 03:54:32.000000 PyQt-Fluent-Widgets-1.5.7/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 03:54:32.000000 PyQt-Fluent-Widgets-1.5.7/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-06-01 03:54:32.000000 PyQt-Fluent-Widgets-1.5.7/PyQt_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 03:54:32.000000 PyQt-Fluent-Widgets-1.5.7/PyQt_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4791 2024-06-01 03:54:20.000000 PyQt-Fluent-Widgets-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.717756 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/
+-rw-rw-rw-   0        0        0      549 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.720754 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-10-15 01:50:42.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  6502733 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.762415 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      664 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0    15238 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     4742 2023-12-29 09:55:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0     1587 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/color.py
+-rw-rw-rw-   0        0        0    11197 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      803 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    13751 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     5537 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3866 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0      658 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/screen.py
+-rw-rw-rw-   0        0        0     4851 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0    14412 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      452 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.764628 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.775404 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2581 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21800 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7629 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19337 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     6439 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.788974 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      216 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14788 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5860 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11337 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3282 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2879 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_box_base.py
+-rw-rw-rw-   0        0        0     2500 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.797082 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2750 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     7525 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1301 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.810115 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/
+-rw-rw-rw-   0        0        0      538 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/__init__.py
+-rw-rw-rw-   0        0        0     3006 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_combo_box.py
+-rw-rw-rw-   0        0        0     3536 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_flyout.py
+-rw-rw-rw-   0        0        0      763 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_line_edit.py
+-rw-rw-rw-   0        0        0     6276 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_menu.py
+-rw-rw-rw-   0        0        0     1181 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_tool_tip.py
+-rw-rw-rw-   0        0        0     1431 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.826425 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      716 2023-11-24 09:36:26.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     9961 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/breadcrumb.py
+-rw-rw-rw-   0        0        0    12968 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8773 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    24107 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    20948 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6996 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     5211 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.839227 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5282 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0    11031 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     4648 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2843 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    14184 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1586 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.905045 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     3328 2024-06-01 03:41:40.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8063 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    30016 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     7700 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     5802 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    15825 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0    19594 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/command_bar.py
+-rw-rw-rw-   0        0        0     7881 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0    13091 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flip_view.py
+-rw-rw-rw-   0        0        0    17086 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2223 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1498 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    16707 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_badge.py
+-rw-rw-rw-   0        0        0    18934 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0    14724 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    14139 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     4812 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    40458 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0    11189 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/pips_pager.py
+-rw-rw-rw-   0        0        0     9199 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     7033 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2718 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    19123 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     1204 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/separator.py
+-rw-rw-rw-   0        0        0    10220 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     8629 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6534 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5790 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8631 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0    26348 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tab_view.py
+-rw-rw-rw-   0        0        0    11538 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    22906 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10563 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     4484 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.912778 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/
+-rw-rw-rw-   0        0        0      183 2023-10-15 01:50:44.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/__init__.py
+-rw-rw-rw-   0        0        0    11617 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_play_bar.py
+-rw-rw-rw-   0        0        0     3585 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_player.py
+-rw-rw-rw-   0        0        0     2845 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/video_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:54:32.919996 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0      187 2024-04-13 06:56:28.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    12934 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     2846 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/window/splash_screen.py
+-rw-rw-rw-   0        0        0     1664 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 03:54:32.923010 PyQt-Fluent-Widgets-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2024-06-01 03:54:21.000000 PyQt-Fluent-Widgets-1.5.7/setup.py
```

### Comparing `PyQt-Fluent-Widgets-1.5.6/LICENSE` & `PyQt-Fluent-Widgets-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/PKG-INFO` & `PyQt-Fluent-Widgets-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 1.5.6
+Version: 1.5.7
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.5.6 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.5.7 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL:
 Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords:
 pyqt fluent widgets Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
```

### Comparing `PyQt-Fluent-Widgets-1.5.6/PyQt_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt-Fluent-Widgets-1.5.7/PyQt_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 1.5.6
+Version: 1.5.7
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://qfluentwidgets.com
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://qfluentwidgets.com/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.5.6 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 1.5.7 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://
 qfluentwidgets.com Author: zhiyiYo Author-email: shokokawaii@outlook.com
 License: GPLv3 Project-URL: Documentation, https://qfluentwidgets.com/ Project-
 URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL:
 Bug Tracker, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords:
 pyqt fluent widgets Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
```

### Comparing `PyQt-Fluent-Widgets-1.5.6/PyQt_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt-Fluent-Widgets-1.5.7/PyQt_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/README.md` & `PyQt-Fluent-Widgets-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/__init__.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/master/examples.
 
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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/_rc/resource.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/_rc/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -94186,42 +94186,42 @@
 \x00\x00\x00\x45\
 \x50\
 \x69\x70\x73\x50\x61\x67\x65\x72\x20\x7b\x0d\x0a\x20\x20\x20\x20\
 \x62\x6f\x72\x64\x65\x72\x3a\x20\x6e\x6f\x6e\x65\x3b\x0d\x0a\x20\
 \x20\x20\x20\x62\x61\x63\x6b\x67\x72\x6f\x75\x6e\x64\x2d\x63\x6f\
 \x6c\x6f\x72\x3a\x20\x74\x72\x61\x6e\x73\x70\x61\x72\x65\x6e\x74\
 \x3b\x0d\x0a\x7d\
-\x00\x00\x01\x9f\
+\x00\x00\x01\x97\
 \x00\
-\x00\x06\xf2\x78\x9c\x9d\x55\xdd\x6e\x82\x30\x18\xbd\x37\xf1\x1d\
-\x9a\xec\x66\x24\xba\x80\x0a\x2a\xcb\x1e\xc0\x3b\x13\x97\xec\x62\
-\xd9\x45\xa1\x9f\xd8\xac\xb4\xa4\x14\x67\xb2\xf8\xee\x6b\xb0\xf8\
-\x03\x55\x9a\x11\x08\xd0\xaf\x9c\x9e\x8f\x73\x0e\xac\xe9\x5e\xa8\
-\x95\x82\x1c\xfd\x0e\x07\x48\x6f\x05\x26\x84\xf2\x2c\x46\x81\x5f\
-\x1c\x50\x30\x29\x0e\xaf\xa7\x42\x2a\x98\x90\x31\x4a\x18\x4e\xbf\
-\xcd\x50\xa2\x2f\x33\x29\x2a\x4e\xc6\xa6\xaa\x24\xe6\x65\x81\x25\
-\x70\xd5\xcc\x11\x92\x80\xae\x70\xc1\xc1\x0c\x89\x4a\x31\xca\xe1\
-\x66\x2c\xc7\x32\xa3\x3c\x46\xbe\xbe\x3f\x0e\x07\xc3\xc1\xba\x21\
-\xf6\x49\xcb\x0d\x30\x48\x15\x90\x37\x25\x2b\xf8\x8a\x77\x62\x0f\
-\xb2\xe1\x6b\x16\x96\x59\x82\x9f\xfd\x11\x32\xfb\x4b\x34\xf5\x1c\
-\x90\x0a\x09\x65\x09\xa4\x07\x2b\xec\xc1\xda\x62\x56\x3a\x83\xcd\
-\x43\x0b\xd8\x0e\x97\xab\x54\x70\x83\xd4\x92\x62\xcc\x60\xab\xe2\
-\x6b\x29\x9a\x82\xa4\xd9\xee\x52\xb9\x83\x59\x77\x6a\x87\x9c\x46\
-\xce\x90\x0d\x80\x45\xce\x3e\x17\xd4\x20\x4f\x7b\x0a\x3f\x67\x10\
-\x97\x27\x36\x90\xe5\xfa\x16\xc8\xbb\x10\xcc\xea\xd0\x50\x1b\x74\
-\xa9\x0f\xdd\x05\x5a\x5c\xf8\x9e\x1f\xfc\xa0\x24\x03\x35\x42\x37\
-\x48\xa7\xc1\xfb\x4c\xda\x7a\xf9\x93\x59\xe0\xb5\xbc\x1c\xe8\x05\
-\x4b\xc1\x28\xe9\xce\x0e\xe7\x8b\xdb\xd9\x63\x89\x09\xad\xca\x18\
-\x45\x16\x86\x76\x27\x8d\x2c\xcd\x77\x67\xb5\x25\x55\xa2\xd0\x8a\
-\x76\x04\x4d\x84\x52\x22\xbf\xae\xfc\x33\xb5\xd6\x76\xae\xa3\xab\
-\x57\x40\x13\xe7\x26\x4f\x29\x76\x6b\xf5\x36\xf1\x7d\x9a\x2d\x3d\
-\x57\x0a\x26\xb1\x8e\x24\x5a\xf9\xee\xa3\x11\x79\x96\xf7\x33\xd3\
-\x87\x39\xf7\x92\xac\x83\xdb\xc7\xcd\x9a\xee\xda\x0a\xdd\x6c\x37\
-\x56\xe8\x4a\xe7\x3b\x9b\xc3\x81\x72\x57\xd9\x87\x1f\x5f\xa7\x0e\
-\xdd\xdc\xf2\xe8\xa3\xde\xfc\xb7\x8e\x7f\x25\x50\x30\x22\
+\x00\x06\xd4\x78\x9c\x9d\x55\xd1\x6a\xc2\x30\x14\x7d\x17\xfc\x87\
+\xc0\x5e\x26\xe8\x68\x75\xad\xda\xb1\x0f\xf0\x4d\x70\xb0\x87\xb1\
+\x87\xb4\xb9\xd6\xb0\x34\x29\x49\xea\x84\xe1\xbf\x2f\xd4\x56\x6d\
+\x1b\x6d\xb0\xb4\xd0\xe4\xde\x9e\x7b\x2e\xe7\x9e\x74\x4d\xf7\x42\
+\xaf\x34\x64\xe8\x6f\x38\x40\xe6\xca\x31\x21\x94\xa7\x11\xf2\xbd\
+\xfc\x80\xfc\x69\x7e\x78\x3b\x05\x12\xc1\x84\x8c\x50\xcc\x70\xf2\
+\x53\x6d\xc5\xe6\x35\x95\xa2\xe0\x64\x52\x45\xb5\xc4\x5c\xe5\x58\
+\x02\xd7\x75\x8e\x90\x04\x4c\x84\x0b\x0e\xd5\x96\x28\x34\xa3\x1c\
+\x1a\x7b\x19\x96\x29\xe5\x11\xf2\xcc\xfa\x38\x1c\x0c\x07\xeb\x9a\
+\xd8\x17\x55\x1b\x60\x90\x68\x20\xef\x5a\x16\xf0\x1d\xed\xc4\x1e\
+\x64\xcd\xb7\x2a\x2c\xd3\x18\x3f\x7b\x63\x54\xdd\x2f\xe1\x6c\xe4\
+\x80\x94\x4b\x50\x0a\x48\x0f\x56\xd0\x83\xb5\xc5\x4c\x39\x83\xcd\
+\x03\x0b\xd8\x0e\xab\x55\x22\x78\x85\xd4\x92\x62\xc2\x60\xab\xa3\
+\x6b\x29\xea\x80\xa4\xe9\xee\x12\xb9\x81\x59\x76\x6a\x87\x9c\x85\
+\xce\x90\x35\x80\x45\xce\xbe\x29\x28\x41\x9e\xf6\x14\x7e\xcf\x20\
+\x2e\x5f\x6c\x20\xcd\xcc\x12\xc8\x87\x10\xcc\x3a\xa1\x81\x19\xd0\
+\xa5\x79\x4c\x17\x68\x71\xe1\x7b\xfe\xf0\x93\x92\x14\xf4\x18\x35\
+\x90\x4e\x9b\xb7\x99\xb4\xf5\xf2\xa6\xaf\xfe\xa8\x35\xcb\xbe\x29\
+\xa8\x04\xa3\xa4\x9b\x1d\xcc\x17\xcd\xec\x89\xc4\x84\x16\x2a\x42\
+\xa1\x85\xa1\x7d\x92\xc6\x96\xe6\xbb\x59\x6d\x49\xb5\xc8\x8d\xa2\
+\x1d\x41\x63\xa1\xb5\xc8\xae\x23\x0f\xba\xd6\xda\xce\xb5\x75\x4d\
+\x05\xe4\x39\x37\x79\x72\xb1\x5b\xab\x4d\xc7\xf7\x69\xb6\x1c\xb9\
+\x52\xa8\x1c\xeb\x48\xa2\xe5\xef\x3e\x1a\x61\x3f\x8d\xd2\x9a\x7d\
+\xd5\xad\xfe\x2d\xc5\xee\xba\xb7\x16\xbb\x2b\x8e\xe7\x2c\xbf\x03\
+\xe5\xae\x76\x77\x8f\x57\xa7\x0e\xdd\xe6\xe1\xde\xb1\x5d\xff\x99\
+\x8e\xff\xac\x0e\x27\xa8\
 \x00\x00\x03\x53\
 \x43\
 \x6f\x6d\x62\x6f\x42\x6f\x78\x20\x7b\x0d\x0a\x20\x20\x20\x20\x62\
 \x6f\x72\x64\x65\x72\x3a\x20\x31\x70\x78\x20\x73\x6f\x6c\x69\x64\
 \x20\x72\x67\x62\x61\x28\x30\x2c\x20\x30\x2c\x20\x30\x2c\x20\x30\
 \x2e\x30\x37\x33\x29\x3b\x0d\x0a\x20\x20\x20\x20\x62\x6f\x72\x64\
 \x65\x72\x2d\x72\x61\x64\x69\x75\x73\x3a\x20\x35\x70\x78\x3b\x0d\
@@ -95450,42 +95450,41 @@
 \x00\x00\x00\x45\
 \x50\
 \x69\x70\x73\x50\x61\x67\x65\x72\x20\x7b\x0d\x0a\x20\x20\x20\x20\
 \x62\x6f\x72\x64\x65\x72\x3a\x20\x6e\x6f\x6e\x65\x3b\x0d\x0a\x20\
 \x20\x20\x20\x62\x61\x63\x6b\x67\x72\x6f\x75\x6e\x64\x2d\x63\x6f\
 \x6c\x6f\x72\x3a\x20\x74\x72\x61\x6e\x73\x70\x61\x72\x65\x6e\x74\
 \x3b\x0d\x0a\x7d\
-\x00\x00\x01\x93\
+\x00\x00\x01\x8b\
 \x00\
-\x00\x06\x55\x78\x9c\xa5\x54\x5d\x6f\x82\x30\x14\x7d\x37\xf1\x3f\
-\x34\xd9\xcb\x48\xc4\x80\x0e\xa6\x2c\xfb\x01\xbe\x99\xb8\x64\x0f\
-\xcb\x1e\x2a\xbd\x42\x33\x68\x49\x5b\xd4\x64\xd9\x7f\x5f\xc7\x87\
-\x3a\xa8\xa3\xdb\x08\x85\xd0\xd3\x7b\x7a\x2e\xe7\xde\xae\xe9\x9e\
-\xab\x95\x82\x1c\xbd\x8f\x47\x48\x5f\x05\x26\x84\xb2\x24\x42\xbe\
-\x57\x1c\x91\x3f\x2b\x8e\x0f\x35\x10\xf3\x8c\x8b\x08\x1d\x52\xaa\
-\xa0\x99\xda\xe2\xf8\x2d\x11\xbc\x64\xc4\x6d\x50\x25\x30\x93\x05\
-\x16\xc0\x54\xbb\x86\x0b\x02\x1a\x61\x9c\xb5\x61\xbc\x54\x19\x65\
-\x70\x9a\xfb\x18\x8f\xc6\xa3\x75\x2b\xe4\x85\xca\x0d\x64\x10\x2b\
-\x20\x8f\x4a\x94\xf0\x1a\xa5\x7c\x0f\xa2\xd5\xd7\x6c\x24\x92\x2d\
-\xbe\x9d\x05\xc1\x04\x9d\x1f\xde\x34\x9c\x3b\x16\x7c\x85\x00\x29\
-\x81\x58\x31\x06\x03\x8c\x3b\x9c\xc9\x5f\x52\xde\x07\x06\xca\x14\
-\xcb\x55\xcc\x59\xc3\xd7\x31\xc3\xcd\x60\xa7\xa2\x4b\x33\x5a\x40\
-\xd0\x24\x3d\x23\x57\x38\xab\xac\xcd\x94\xf3\xd0\x9a\xb2\x25\x30\
-\x18\x3a\x54\x07\x15\xc9\xcd\x9e\xc2\xe1\x44\x62\x13\xb1\x81\x24\
-\xd7\x9f\x40\x9e\x38\xcf\x8c\x35\x1a\xe8\x12\x5d\xea\xa1\xb3\x40\
-\x8b\xb3\xde\x53\xe0\x33\x25\x09\xa8\x49\x87\xaa\x9e\xbd\x2e\xa5\
-\xb2\xcd\xd3\x56\xd5\xf7\xd4\x77\x3a\xb5\xec\xeb\xed\x24\xcf\x28\
-\xb9\xe2\xb0\xb7\xf8\x1e\xe1\x0a\x4c\x68\x29\x23\x14\x1a\x34\x9a\
-\x2b\x6a\x82\x7a\xd9\xf7\x17\x75\x3d\x55\xbc\xd0\x96\xf6\x1c\xdd\
-\x72\xa5\x78\x7e\x89\xfc\xb1\x71\x8d\xd9\x7c\x01\x39\x16\x09\x65\
-\xd5\x0e\x68\x66\x9d\x63\xdd\xd8\x5d\x77\x7e\x5a\x3b\xe0\x59\xc7\
-\x88\xa5\x63\x2b\xa4\x69\x5f\x4b\x29\x9d\x66\xb7\x13\x13\x3a\x86\
-\x7f\x75\xa7\x47\xf3\x1e\x94\x5a\x75\xf1\x90\x42\x63\xab\x57\x65\
-\xd1\x6f\xf4\xb6\x2c\xfa\x36\x7a\xff\x39\xf4\x75\x16\x9f\x17\x15\
-\xf3\x1c\
+\x00\x06\x37\x78\x9c\xa5\x94\x51\x6b\x83\x30\x10\xc7\xdf\x0b\xfd\
+\x0e\x81\xbd\xac\xd0\x16\x6d\xd1\xb5\x8e\x7d\x80\xbe\x15\x3a\xd8\
+\xc3\xd8\x43\x6a\xae\x1a\xa6\x39\x49\x62\x5b\x18\xfb\xee\xcb\xac\
+\xb6\x9b\xa6\x33\xdb\x44\x05\x73\xb9\x7f\xfe\xc7\xef\xce\x35\xdf\
+\xa3\x5e\x69\xc8\xc9\xdb\x70\x40\xcc\x55\x50\xc6\xb8\x48\x22\xe2\
+\x7b\xc5\x91\xf8\xb3\xe2\x78\x7f\x0a\xc4\x98\xa1\x8c\xc8\x21\xe5\
+\x1a\xea\xa5\x2d\x8d\x5f\x13\x89\xa5\x60\x93\x3a\xaa\x25\x15\xaa\
+\xa0\x12\x84\x6e\xf6\xa0\x64\x60\x22\x02\x45\x93\x86\xa5\xce\xb8\
+\x80\xf3\xda\xfb\x70\x30\x1c\xac\x1b\x23\xcf\x5c\x6d\x20\x83\x58\
+\x03\x7b\xd0\xb2\x84\x97\x28\xc5\x3d\xc8\xc6\x5f\x7d\x90\x4c\xb6\
+\xf4\x76\x16\x04\x63\x72\x79\x79\xd3\x70\x3e\x72\xd0\x2b\x24\x28\
+\x05\xcc\x49\x31\xe8\x51\xdc\xd1\x4c\xfd\x52\xf2\x2e\xb0\x48\xa6\
+\x54\xad\x62\x14\xb5\x5e\x0b\xc6\x24\x83\x9d\x8e\xbe\xc2\x68\x02\
+\x92\x27\xe9\x25\x72\x45\xb3\xaa\xda\x2e\x39\x0f\x9d\x25\x1b\x01\
+\x0b\xd0\xbe\x3e\xa8\x44\x6e\xf6\x1c\x0e\x67\x11\x97\x8c\x0d\x24\
+\xb9\xf9\x04\xf6\x88\x98\x59\x7b\x34\x30\x2d\xba\x34\x8f\xa9\x82\
+\x2c\x2e\x7e\xcf\x89\x4f\x9c\x25\xa0\xc7\x2d\xa9\xd3\xea\x75\x2b\
+\x15\x36\xcf\xa0\x3a\xdd\x53\x7f\xd4\xea\x65\xdf\x1c\xa7\x30\xe3\
+\xec\x0a\x61\x6f\xf1\x3d\x63\x22\x29\xe3\xa5\x8a\x48\x68\xf1\x68\
+\xef\xa8\x31\xe9\x54\xdf\xdd\xd4\x66\xaa\xb1\x30\x48\x3b\x44\xb7\
+\xa8\x35\xe6\x5f\x23\x7f\x1c\x5c\x6b\x35\x9f\x81\x9c\xca\x84\x8b\
+\xea\x04\xe2\x39\xd7\x78\x1a\xec\x36\x9d\x9f\xf6\xf6\x30\x6b\x81\
+\x58\x8e\x5c\x8d\xd4\xe3\xeb\x68\xa5\x35\xec\x6e\x66\xc2\x7e\x33\
+\xd5\x9c\xf6\x79\xb0\x0e\x73\x05\xbe\x3b\xca\x0d\xf8\x2e\x28\xef\
+\x3f\xbf\x75\x53\xc5\x07\xf9\xbe\xea\xa2\
 \x00\x00\x03\x89\
 \x43\
 \x6f\x6d\x62\x6f\x42\x6f\x78\x20\x7b\x0d\x0a\x20\x20\x20\x20\x62\
 \x6f\x72\x64\x65\x72\x3a\x20\x31\x70\x78\x20\x73\x6f\x6c\x69\x64\
 \x20\x72\x67\x62\x61\x28\x32\x35\x35\x2c\x20\x32\x35\x35\x2c\x20\
 \x32\x35\x35\x2c\x20\x30\x2e\x30\x35\x33\x29\x3b\x0d\x0a\x20\x20\
 \x20\x20\x62\x6f\x72\x64\x65\x72\x2d\x72\x61\x64\x69\x75\x73\x3a\
@@ -98393,52 +98392,52 @@
 \x00\x00\x4a\xba\x00\x01\x00\x00\x00\x01\x00\x16\xb0\x53\
 \x00\x00\x4a\xd0\x00\x00\x00\x00\x00\x01\x00\x16\xb2\x3e\
 \x00\x00\x4a\xf4\x00\x01\x00\x00\x00\x01\x00\x16\xb2\xdd\
 \x00\x00\x4b\x28\x00\x01\x00\x00\x00\x01\x00\x16\xb4\xbb\
 \x00\x00\x4b\x48\x00\x00\x00\x00\x00\x01\x00\x16\xb6\x4f\
 \x00\x00\x4b\x7a\x00\x00\x00\x00\x00\x01\x00\x16\xba\x5c\
 \x00\x00\x4b\x9c\x00\x01\x00\x00\x00\x01\x00\x16\xba\xa5\
-\x00\x00\x4b\xb4\x00\x00\x00\x00\x00\x01\x00\x16\xbc\x48\
-\x00\x00\x4b\xd4\x00\x00\x00\x00\x00\x01\x00\x16\xbf\x9f\
-\x00\x00\x4c\x0a\x00\x01\x00\x00\x00\x01\x00\x16\xc2\x0b\
-\x00\x00\x4c\x30\x00\x01\x00\x00\x00\x01\x00\x16\xc4\xfd\
-\x00\x00\x47\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xc6\xf5\
-\x00\x00\x47\xc4\x00\x01\x00\x00\x00\x01\x00\x16\xc7\x6d\
-\x00\x00\x47\xe6\x00\x00\x00\x00\x00\x01\x00\x16\xc9\x8a\
-\x00\x00\x48\x0c\x00\x01\x00\x00\x00\x01\x00\x16\xc9\xf8\
-\x00\x00\x48\x34\x00\x00\x00\x00\x00\x01\x00\x16\xcb\xad\
-\x00\x00\x48\x4e\x00\x00\x00\x00\x00\x01\x00\x16\xd2\x52\
-\x00\x00\x48\x70\x00\x00\x00\x00\x00\x01\x00\x16\xd2\x96\
-\x00\x00\x48\x8e\x00\x00\x00\x00\x00\x01\x00\x16\xd4\x59\
-\x00\x00\x48\xb8\x00\x00\x00\x00\x00\x01\x00\x16\xd7\xa8\
-\x00\x00\x48\xd8\x00\x01\x00\x00\x00\x01\x00\x16\xd7\xf0\
-\x00\x00\x48\xf6\x00\x00\x00\x00\x00\x01\x00\x16\xda\x6a\
-\x00\x00\x49\x14\x00\x01\x00\x00\x00\x01\x00\x16\xde\x24\
-\x00\x00\x49\x38\x00\x01\x00\x00\x00\x01\x00\x16\xe0\x73\
-\x00\x00\x49\x64\x00\x00\x00\x00\x00\x01\x00\x16\xe2\x78\
-\x00\x00\x49\x7c\x00\x00\x00\x00\x00\x01\x00\x16\xe4\x51\
-\x00\x00\x49\xa2\x00\x00\x00\x00\x00\x01\x00\x16\xe5\x7d\
-\x00\x00\x49\xcc\x00\x01\x00\x00\x00\x01\x00\x16\xe6\xf3\
-\x00\x00\x49\xec\x00\x00\x00\x00\x00\x01\x00\x16\xe9\x88\
-\x00\x00\x4a\x0c\x00\x00\x00\x00\x00\x01\x00\x16\xec\x10\
-\x00\x00\x4a\x34\x00\x00\x00\x00\x00\x01\x00\x16\xed\x8d\
-\x00\x00\x4a\x54\x00\x01\x00\x00\x00\x01\x00\x16\xef\x3f\
-\x00\x00\x4a\x6e\x00\x01\x00\x00\x00\x01\x00\x16\xf0\xe4\
-\x00\x00\x4a\x88\x00\x00\x00\x00\x00\x01\x00\x16\xf5\xc2\
-\x00\x00\x4a\xba\x00\x01\x00\x00\x00\x01\x00\x16\xf6\x6b\
-\x00\x00\x4a\xd0\x00\x00\x00\x00\x00\x01\x00\x16\xf8\x44\
-\x00\x00\x4a\xf4\x00\x01\x00\x00\x00\x01\x00\x16\xf8\xe3\
-\x00\x00\x4b\x28\x00\x00\x00\x00\x00\x01\x00\x16\xfa\xb2\
-\x00\x00\x4b\x48\x00\x00\x00\x00\x00\x01\x00\x17\x00\x2b\
-\x00\x00\x4b\x7a\x00\x00\x00\x00\x00\x01\x00\x17\x04\x7f\
-\x00\x00\x4b\x9c\x00\x01\x00\x00\x00\x01\x00\x17\x04\xc8\
-\x00\x00\x4b\xb4\x00\x00\x00\x00\x00\x01\x00\x17\x06\x5f\
-\x00\x00\x4b\xd4\x00\x00\x00\x00\x00\x01\x00\x17\x09\xec\
-\x00\x00\x4c\x0a\x00\x01\x00\x00\x00\x01\x00\x17\x0c\x50\
-\x00\x00\x4c\x30\x00\x01\x00\x00\x00\x01\x00\x17\x0f\x3c\
+\x00\x00\x4b\xb4\x00\x00\x00\x00\x00\x01\x00\x16\xbc\x40\
+\x00\x00\x4b\xd4\x00\x00\x00\x00\x00\x01\x00\x16\xbf\x97\
+\x00\x00\x4c\x0a\x00\x01\x00\x00\x00\x01\x00\x16\xc2\x03\
+\x00\x00\x4c\x30\x00\x01\x00\x00\x00\x01\x00\x16\xc4\xf5\
+\x00\x00\x47\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xc6\xed\
+\x00\x00\x47\xc4\x00\x01\x00\x00\x00\x01\x00\x16\xc7\x65\
+\x00\x00\x47\xe6\x00\x00\x00\x00\x00\x01\x00\x16\xc9\x82\
+\x00\x00\x48\x0c\x00\x01\x00\x00\x00\x01\x00\x16\xc9\xf0\
+\x00\x00\x48\x34\x00\x00\x00\x00\x00\x01\x00\x16\xcb\xa5\
+\x00\x00\x48\x4e\x00\x00\x00\x00\x00\x01\x00\x16\xd2\x4a\
+\x00\x00\x48\x70\x00\x00\x00\x00\x00\x01\x00\x16\xd2\x8e\
+\x00\x00\x48\x8e\x00\x00\x00\x00\x00\x01\x00\x16\xd4\x51\
+\x00\x00\x48\xb8\x00\x00\x00\x00\x00\x01\x00\x16\xd7\xa0\
+\x00\x00\x48\xd8\x00\x01\x00\x00\x00\x01\x00\x16\xd7\xe8\
+\x00\x00\x48\xf6\x00\x00\x00\x00\x00\x01\x00\x16\xda\x62\
+\x00\x00\x49\x14\x00\x01\x00\x00\x00\x01\x00\x16\xde\x1c\
+\x00\x00\x49\x38\x00\x01\x00\x00\x00\x01\x00\x16\xe0\x6b\
+\x00\x00\x49\x64\x00\x00\x00\x00\x00\x01\x00\x16\xe2\x70\
+\x00\x00\x49\x7c\x00\x00\x00\x00\x00\x01\x00\x16\xe4\x49\
+\x00\x00\x49\xa2\x00\x00\x00\x00\x00\x01\x00\x16\xe5\x75\
+\x00\x00\x49\xcc\x00\x01\x00\x00\x00\x01\x00\x16\xe6\xeb\
+\x00\x00\x49\xec\x00\x00\x00\x00\x00\x01\x00\x16\xe9\x80\
+\x00\x00\x4a\x0c\x00\x00\x00\x00\x00\x01\x00\x16\xec\x08\
+\x00\x00\x4a\x34\x00\x00\x00\x00\x00\x01\x00\x16\xed\x85\
+\x00\x00\x4a\x54\x00\x01\x00\x00\x00\x01\x00\x16\xef\x37\
+\x00\x00\x4a\x6e\x00\x01\x00\x00\x00\x01\x00\x16\xf0\xdc\
+\x00\x00\x4a\x88\x00\x00\x00\x00\x00\x01\x00\x16\xf5\xba\
+\x00\x00\x4a\xba\x00\x01\x00\x00\x00\x01\x00\x16\xf6\x63\
+\x00\x00\x4a\xd0\x00\x00\x00\x00\x00\x01\x00\x16\xf8\x3c\
+\x00\x00\x4a\xf4\x00\x01\x00\x00\x00\x01\x00\x16\xf8\xdb\
+\x00\x00\x4b\x28\x00\x00\x00\x00\x00\x01\x00\x16\xfa\xaa\
+\x00\x00\x4b\x48\x00\x00\x00\x00\x00\x01\x00\x17\x00\x23\
+\x00\x00\x4b\x7a\x00\x00\x00\x00\x00\x01\x00\x17\x04\x77\
+\x00\x00\x4b\x9c\x00\x01\x00\x00\x00\x01\x00\x17\x04\xc0\
+\x00\x00\x4b\xb4\x00\x00\x00\x00\x00\x01\x00\x17\x06\x4f\
+\x00\x00\x4b\xd4\x00\x00\x00\x00\x00\x01\x00\x17\x09\xdc\
+\x00\x00\x4c\x0a\x00\x01\x00\x00\x00\x01\x00\x17\x0c\x40\
+\x00\x00\x4c\x30\x00\x01\x00\x00\x00\x01\x00\x17\x0f\x2c\
 "
 
 qt_resource_struct_v2 = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
@@ -99405,15 +99404,15 @@
 \x00\x00\x48\x70\x00\x00\x00\x00\x00\x01\x00\x16\x8c\xe2\
 \x00\x00\x01\x8b\x31\x07\x4d\x97\
 \x00\x00\x48\x8e\x00\x00\x00\x00\x00\x01\x00\x16\x8e\x80\
 \x00\x00\x01\x8b\x31\x07\x4d\x57\
 \x00\x00\x48\xb8\x00\x00\x00\x00\x00\x01\x00\x16\x91\xc4\
 \x00\x00\x01\x8b\x31\x07\x4d\x1d\
 \x00\x00\x48\xd8\x00\x01\x00\x00\x00\x01\x00\x16\x92\x0c\
-\x00\x00\x01\x8f\x42\x14\x13\x31\
+\x00\x00\x01\x8f\xd1\xbd\x35\xf3\
 \x00\x00\x48\xf6\x00\x00\x00\x00\x00\x01\x00\x16\x94\x3e\
 \x00\x00\x01\x8b\x31\x07\x4d\x3a\
 \x00\x00\x49\x14\x00\x01\x00\x00\x00\x01\x00\x16\x97\xfe\
 \x00\x00\x01\x8b\x31\x07\x4d\x8f\
 \x00\x00\x49\x38\x00\x01\x00\x00\x00\x01\x00\x16\x9a\x55\
 \x00\x00\x01\x8b\x31\x07\x4c\xf6\
 \x00\x00\x49\x64\x00\x00\x00\x00\x00\x01\x00\x16\x9c\x5a\
@@ -99439,97 +99438,97 @@
 \x00\x00\x4a\xba\x00\x01\x00\x00\x00\x01\x00\x16\xb0\x53\
 \x00\x00\x01\x8b\x66\xa8\x0a\xf2\
 \x00\x00\x4a\xd0\x00\x00\x00\x00\x00\x01\x00\x16\xb2\x3e\
 \x00\x00\x01\x8b\x31\x07\x4c\xfc\
 \x00\x00\x4a\xf4\x00\x01\x00\x00\x00\x01\x00\x16\xb2\xdd\
 \x00\x00\x01\x8d\xa6\xd3\x33\xe2\
 \x00\x00\x4b\x28\x00\x01\x00\x00\x00\x01\x00\x16\xb4\xbb\
-\x00\x00\x01\x8f\x42\x15\x6f\x70\
+\x00\x00\x01\x8f\xd1\xbd\x35\xee\
 \x00\x00\x4b\x48\x00\x00\x00\x00\x00\x01\x00\x16\xb6\x4f\
 \x00\x00\x01\x8b\x31\x07\x4d\x2c\
 \x00\x00\x4b\x7a\x00\x00\x00\x00\x00\x01\x00\x16\xba\x5c\
 \x00\x00\x01\x8b\x31\x07\x4d\x5e\
 \x00\x00\x4b\x9c\x00\x01\x00\x00\x00\x01\x00\x16\xba\xa5\
-\x00\x00\x01\x8c\x00\xb0\x09\x8d\
-\x00\x00\x4b\xb4\x00\x00\x00\x00\x00\x01\x00\x16\xbc\x48\
+\x00\x00\x01\x8f\xd1\xc5\x76\x94\
+\x00\x00\x4b\xb4\x00\x00\x00\x00\x00\x01\x00\x16\xbc\x40\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa9\
-\x00\x00\x4b\xd4\x00\x00\x00\x00\x00\x01\x00\x16\xbf\x9f\
+\x00\x00\x4b\xd4\x00\x00\x00\x00\x00\x01\x00\x16\xbf\x97\
 \x00\x00\x01\x8b\x31\x07\x4d\x5e\
-\x00\x00\x4c\x0a\x00\x01\x00\x00\x00\x01\x00\x16\xc2\x0b\
+\x00\x00\x4c\x0a\x00\x01\x00\x00\x00\x01\x00\x16\xc2\x03\
 \x00\x00\x01\x8b\x31\x07\x4d\x08\
-\x00\x00\x4c\x30\x00\x01\x00\x00\x00\x01\x00\x16\xc4\xfd\
+\x00\x00\x4c\x30\x00\x01\x00\x00\x00\x01\x00\x16\xc4\xf5\
 \x00\x00\x01\x8d\xa6\xd3\x33\xe7\
-\x00\x00\x47\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xc6\xf5\
+\x00\x00\x47\xa6\x00\x00\x00\x00\x00\x01\x00\x16\xc6\xed\
 \x00\x00\x01\x8b\x31\x07\x4c\xca\
-\x00\x00\x47\xc4\x00\x01\x00\x00\x00\x01\x00\x16\xc7\x6d\
+\x00\x00\x47\xc4\x00\x01\x00\x00\x00\x01\x00\x16\xc7\x65\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa3\
-\x00\x00\x47\xe6\x00\x00\x00\x00\x00\x01\x00\x16\xc9\x8a\
+\x00\x00\x47\xe6\x00\x00\x00\x00\x00\x01\x00\x16\xc9\x82\
 \x00\x00\x01\x8b\x31\x07\x4c\x8e\
-\x00\x00\x48\x0c\x00\x01\x00\x00\x00\x01\x00\x16\xc9\xf8\
+\x00\x00\x48\x0c\x00\x01\x00\x00\x00\x01\x00\x16\xc9\xf0\
 \x00\x00\x01\x8c\x01\x8b\x7e\xfb\
-\x00\x00\x48\x34\x00\x00\x00\x00\x00\x01\x00\x16\xcb\xad\
+\x00\x00\x48\x34\x00\x00\x00\x00\x00\x01\x00\x16\xcb\xa5\
 \x00\x00\x01\x8d\xa6\xd3\x33\xcc\
-\x00\x00\x48\x4e\x00\x00\x00\x00\x00\x01\x00\x16\xd2\x52\
+\x00\x00\x48\x4e\x00\x00\x00\x00\x00\x01\x00\x16\xd2\x4a\
 \x00\x00\x01\x8b\x31\x07\x4c\x74\
-\x00\x00\x48\x70\x00\x00\x00\x00\x00\x01\x00\x16\xd2\x96\
+\x00\x00\x48\x70\x00\x00\x00\x00\x00\x01\x00\x16\xd2\x8e\
 \x00\x00\x01\x8b\x31\x07\x4c\xe3\
-\x00\x00\x48\x8e\x00\x00\x00\x00\x00\x01\x00\x16\xd4\x59\
+\x00\x00\x48\x8e\x00\x00\x00\x00\x00\x01\x00\x16\xd4\x51\
 \x00\x00\x01\x8b\x31\x07\x4c\x9b\
-\x00\x00\x48\xb8\x00\x00\x00\x00\x00\x01\x00\x16\xd7\xa8\
+\x00\x00\x48\xb8\x00\x00\x00\x00\x00\x01\x00\x16\xd7\xa0\
 \x00\x00\x01\x8b\x31\x07\x4c\x5c\
-\x00\x00\x48\xd8\x00\x01\x00\x00\x00\x01\x00\x16\xd7\xf0\
-\x00\x00\x01\x8f\x42\x14\x77\xcc\
-\x00\x00\x48\xf6\x00\x00\x00\x00\x00\x01\x00\x16\xda\x6a\
+\x00\x00\x48\xd8\x00\x01\x00\x00\x00\x01\x00\x16\xd7\xe8\
+\x00\x00\x01\x8f\xd1\xbd\x35\xe9\
+\x00\x00\x48\xf6\x00\x00\x00\x00\x00\x01\x00\x16\xda\x62\
 \x00\x00\x01\x8b\x31\x07\x4c\x7b\
-\x00\x00\x49\x14\x00\x01\x00\x00\x00\x01\x00\x16\xde\x24\
+\x00\x00\x49\x14\x00\x01\x00\x00\x00\x01\x00\x16\xde\x1c\
 \x00\x00\x01\x8b\x31\x07\x4c\xdc\
-\x00\x00\x49\x38\x00\x01\x00\x00\x00\x01\x00\x16\xe0\x73\
+\x00\x00\x49\x38\x00\x01\x00\x00\x00\x01\x00\x16\xe0\x6b\
 \x00\x00\x01\x8b\x31\x07\x4c\x2b\
-\x00\x00\x49\x64\x00\x00\x00\x00\x00\x01\x00\x16\xe2\x78\
+\x00\x00\x49\x64\x00\x00\x00\x00\x00\x01\x00\x16\xe2\x70\
 \x00\x00\x01\x8c\x00\xb0\x09\x5f\
-\x00\x00\x49\x7c\x00\x00\x00\x00\x00\x01\x00\x16\xe4\x51\
+\x00\x00\x49\x7c\x00\x00\x00\x00\x00\x01\x00\x16\xe4\x49\
 \x00\x00\x01\x8b\x31\x07\x4c\xd6\
-\x00\x00\x49\xa2\x00\x00\x00\x00\x00\x01\x00\x16\xe5\x7d\
+\x00\x00\x49\xa2\x00\x00\x00\x00\x00\x01\x00\x16\xe5\x75\
 \x00\x00\x01\x8b\x31\x07\x4c\xbc\
-\x00\x00\x49\xcc\x00\x01\x00\x00\x00\x01\x00\x16\xe6\xf3\
+\x00\x00\x49\xcc\x00\x01\x00\x00\x00\x01\x00\x16\xe6\xeb\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa3\
-\x00\x00\x49\xec\x00\x00\x00\x00\x00\x01\x00\x16\xe9\x88\
+\x00\x00\x49\xec\x00\x00\x00\x00\x00\x01\x00\x16\xe9\x80\
 \x00\x00\x01\x8c\xb4\xff\xf1\xa2\
-\x00\x00\x4a\x0c\x00\x00\x00\x00\x00\x01\x00\x16\xec\x10\
+\x00\x00\x4a\x0c\x00\x00\x00\x00\x00\x01\x00\x16\xec\x08\
 \x00\x00\x01\x8b\x31\x07\x4c\xc4\
-\x00\x00\x4a\x34\x00\x00\x00\x00\x00\x01\x00\x16\xed\x8d\
+\x00\x00\x4a\x34\x00\x00\x00\x00\x00\x01\x00\x16\xed\x85\
 \x00\x00\x01\x8c\xb4\xff\xf1\x9c\
-\x00\x00\x4a\x54\x00\x01\x00\x00\x00\x01\x00\x16\xef\x3f\
+\x00\x00\x4a\x54\x00\x01\x00\x00\x00\x01\x00\x16\xef\x37\
 \x00\x00\x01\x8b\x31\x07\x4c\xb0\
-\x00\x00\x4a\x6e\x00\x01\x00\x00\x00\x01\x00\x16\xf0\xe4\
+\x00\x00\x4a\x6e\x00\x01\x00\x00\x00\x01\x00\x16\xf0\xdc\
 \x00\x00\x01\x8d\xb6\x35\x32\x64\
-\x00\x00\x4a\x88\x00\x00\x00\x00\x00\x01\x00\x16\xf5\xc2\
+\x00\x00\x4a\x88\x00\x00\x00\x00\x00\x01\x00\x16\xf5\xba\
 \x00\x00\x01\x8b\x31\x07\x4c\xaf\
-\x00\x00\x4a\xba\x00\x01\x00\x00\x00\x01\x00\x16\xf6\x6b\
+\x00\x00\x4a\xba\x00\x01\x00\x00\x00\x01\x00\x16\xf6\x63\
 \x00\x00\x01\x8b\x31\x07\x4c\x94\
-\x00\x00\x4a\xd0\x00\x00\x00\x00\x00\x01\x00\x16\xf8\x44\
+\x00\x00\x4a\xd0\x00\x00\x00\x00\x00\x01\x00\x16\xf8\x3c\
 \x00\x00\x01\x8b\x31\x07\x4c\x31\
-\x00\x00\x4a\xf4\x00\x01\x00\x00\x00\x01\x00\x16\xf8\xe3\
+\x00\x00\x4a\xf4\x00\x01\x00\x00\x00\x01\x00\x16\xf8\xdb\
 \x00\x00\x01\x8d\xa6\xd3\x33\xd1\
-\x00\x00\x4b\x28\x00\x00\x00\x00\x00\x01\x00\x16\xfa\xb2\
-\x00\x00\x01\x8f\x42\x15\xc6\xa2\
-\x00\x00\x4b\x48\x00\x00\x00\x00\x00\x01\x00\x17\x00\x2b\
+\x00\x00\x4b\x28\x00\x00\x00\x00\x00\x01\x00\x16\xfa\xaa\
+\x00\x00\x01\x8f\xd1\xbd\x35\xe0\
+\x00\x00\x4b\x48\x00\x00\x00\x00\x00\x01\x00\x17\x00\x23\
 \x00\x00\x01\x8b\x31\x07\x4c\x6c\
-\x00\x00\x4b\x7a\x00\x00\x00\x00\x00\x01\x00\x17\x04\x7f\
+\x00\x00\x4b\x7a\x00\x00\x00\x00\x00\x01\x00\x17\x04\x77\
 \x00\x00\x01\x8b\x31\x07\x4c\xa7\
-\x00\x00\x4b\x9c\x00\x01\x00\x00\x00\x01\x00\x17\x04\xc8\
-\x00\x00\x01\x8c\x00\xb0\x09\x66\
-\x00\x00\x4b\xb4\x00\x00\x00\x00\x00\x01\x00\x17\x06\x5f\
+\x00\x00\x4b\x9c\x00\x01\x00\x00\x00\x01\x00\x17\x04\xc0\
+\x00\x00\x01\x8f\xd1\xc5\xbe\x8b\
+\x00\x00\x4b\xb4\x00\x00\x00\x00\x00\x01\x00\x17\x06\x4f\
 \x00\x00\x01\x8c\xb4\xff\xf1\x9c\
-\x00\x00\x4b\xd4\x00\x00\x00\x00\x00\x01\x00\x17\x09\xec\
+\x00\x00\x4b\xd4\x00\x00\x00\x00\x00\x01\x00\x17\x09\xdc\
 \x00\x00\x01\x8b\x31\x07\x4c\xa1\
-\x00\x00\x4c\x0a\x00\x01\x00\x00\x00\x01\x00\x17\x0c\x50\
+\x00\x00\x4c\x0a\x00\x01\x00\x00\x00\x01\x00\x17\x0c\x40\
 \x00\x00\x01\x8b\x31\x07\x4c\x42\
-\x00\x00\x4c\x30\x00\x01\x00\x00\x00\x01\x00\x17\x0f\x3c\
-\x00\x00\x01\x8f\x00\x62\x17\xca\
+\x00\x00\x4c\x30\x00\x01\x00\x00\x00\x01\x00\x17\x0f\x2c\
+\x00\x00\x01\x8f\x51\x2d\x79\xe5\
 "
 
 qt_version = [int(v) for v in QtCore.qVersion().split('.')]
 if qt_version < [5, 8, 0]:
     rcc_version = 1
     qt_resource_struct = qt_resource_struct_v1
 else:
```

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/__init__.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/animation.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/auto_wrap.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/color.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/color.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/config.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/config.py`

 * *Files 1% similar despite different names*

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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/exception_handler.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/font.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/icon.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/image_utils.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/overload.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/router.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/screen.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/screen.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/smooth_scroll.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/common/style_sheet.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/common/style_sheet.py`

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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_picker.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/calendar_view.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/date_picker.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/picker_base.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/date_time/time_picker.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files 3% similar despite different names*

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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_box_base.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_box_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/expand_layout.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/flow_layout.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/flow_layout.py`

 * *Files 8% similar despite different names*

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
@@ -129,15 +143,15 @@
 
     def heightForWidth(self, width: int):
         """ get the minimal height according to width """
         return self._doLayout(QRect(0, 0, width, 0), False)
 
     def setGeometry(self, rect: QRect):
         super().setGeometry(rect)
-        
+
         if self.needAni:
             self._deBounceTimer.start(80)
         else:
             self._doLayout(rect, True)
 
     def sizeHint(self):
         return self.minimumSize()
@@ -164,15 +178,15 @@
     def setHorizontalSpacing(self, spacing: int):
         """ set horizontal spacing between widgets """
         self._horizontalSpacing = spacing
 
     def horizontalSpacing(self):
         """ get horizontal spacing between widgets """
         return self._horizontalSpacing
-    
+
     def eventFilter(self, obj: QObject, event: QEvent) -> bool:
         if obj in [w.widget() for w in self._items] and event.type() == QEvent.Type.ParentChange:
             self._wParent = obj.parent()
             obj.parent().installEventFilter(self)
             self._isInstalledEventFilter = True
 
         if obj == self._wParent and event.type() == QEvent.Type.Show:
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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/__init__.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_combo_box.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_flyout.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_line_edit.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_menu.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_menu.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_tool_tip.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/material/acrylic_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/material/acrylic_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/__init__.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/breadcrumb.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_bar.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files 9% similar despite different names*

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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/pivot.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/pivot.py`

 * *Files 4% similar despite different names*

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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/navigation/segmented_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/__init__.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card.py`

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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/__init__.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/button.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/card_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/check_box.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/combo_box.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/command_bar.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flip_view.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flip_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/flyout.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/flyout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/frameless_window.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_badge.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_badge.py`

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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/info_bar.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/label.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/line_edit.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/list_view.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/menu.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/pips_pager.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/pips_pager.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_bar.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/progress_ring.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/scroll_bar.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/scroll_bar.py`

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
+    opacity = pyqtProperty(float, getOpacity, setOpacity)
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

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/separator.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/slider.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/spin_box.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/switch_button.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tab_view.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/table_view.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/teaching_tip.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/components/widgets/tree_view.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_play_bar.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_play_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/media_player.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/media_player.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/multimedia/video_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/multimedia/video_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/window/fluent_window.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/window/splash_screen.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/window/splash_screen.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/qfluentwidgets/window/stacked_widget.py` & `PyQt-Fluent-Widgets-1.5.7/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-1.5.6/setup.py` & `PyQt-Fluent-Widgets-1.5.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt-Fluent-Widgets",
-    version="1.5.6",
+    version="1.5.7",
     keywords="pyqt fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt5",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

