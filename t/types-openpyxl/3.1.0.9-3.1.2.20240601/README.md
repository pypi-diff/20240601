# Comparing `tmp/types-openpyxl-3.1.0.9.tar.gz` & `tmp/types-openpyxl-3.1.2.20240601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-openpyxl-3.1.0.9.tar", last modified: Mon Jun 12 15:15:14 2023, max compression
+gzip compressed data, was "types-openpyxl-3.1.2.20240601.tar", last modified: Sat Jun  1 02:27:15 2024, max compression
```

## Comparing `types-openpyxl-3.1.0.9.tar` & `types-openpyxl-3.1.2.20240601.tar`

### file list

```diff
@@ -1,221 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.717801 types-openpyxl-3.1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-12 15:15:12.000000 types-openpyxl-3.1.0.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 15:15:12.000000 types-openpyxl-3.1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-12 15:15:14.717801 types-openpyxl-3.1.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.685801 types-openpyxl-3.1.0.9/openpyxl-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-12 15:15:12.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/_constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.689801 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/rich_text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/text.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.693801 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/_3d.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/area_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/axis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/bar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/bubble_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/chartspace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/data_source.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/error_bar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/label.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/layout.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/legend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/line_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/marker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/pie_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/pivot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/plotarea.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/radar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/scatter_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/series.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/series_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/shapes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/stock_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/surface_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/title.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/trendline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/updown_bars.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.697801 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/chartsheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/publish.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.697801 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/author.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/comment_sheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/comments.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/shape_writer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.697801 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/product.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/singleton.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/strings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/nested.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/sequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/serialisable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/slots.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/connector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/effect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/fill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/graphic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/line.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/xdr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/formatting.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/rule.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/formula/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formula/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formula/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formula/translate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/extended.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/interface.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/relationship.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.705801 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25468 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/record.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34798 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.705801 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/drawings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.705801 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/alignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/borders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/builtins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/cell_style.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/differential.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/fills.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/named_styles.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/styleable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/stylesheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.709801 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/bound_dictionary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/dataframe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/escape.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/formulas.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/indexed_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/inference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/units.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.709801 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/child.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/defined_name.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.709801 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_link/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_link/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_link/external.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/function_group.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/smart_tags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/web.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.713801 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_write_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/cell_range.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/cell_watch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/controls.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/copier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/datavalidation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/dimensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/formula.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/header_footer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/hyperlink.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/ole.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/page.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/pagebreak.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/related.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/scenario.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/smart_tag.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/worksheet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.713801 types-openpyxl-3.1.0.9/openpyxl-stubs/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/writer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/writer/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/writer/theme.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.713801 types-openpyxl-3.1.0.9/openpyxl-stubs/xml/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/xml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/xml/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/xml/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:15:14.717801 types-openpyxl-3.1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-12 15:15:11.000000 types-openpyxl-3.1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.717801 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-12 15:15:14.000000 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-06-12 15:15:14.000000 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:15:14.000000 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:15:14.000000 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.979124 types-openpyxl-3.1.2.20240601/
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-06-01 02:27:14.000000 types-openpyxl-3.1.2.20240601/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 02:27:14.000000 types-openpyxl-3.1.2.20240601/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-06-01 02:27:15.979124 types-openpyxl-3.1.2.20240601/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.955124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-01 02:27:14.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/_constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.955124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/rich_text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/text.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.959124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/_3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/area_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/axis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/bar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/bubble_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/chartspace.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/data_source.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/error_bar.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/label.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/layout.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/legend.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/line_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/marker.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/pie_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/pivot.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/plotarea.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/radar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/scatter_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/series.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/series_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/shapes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/stock_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/surface_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/title.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/trendline.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/updown_bars.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.963124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/chartsheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/publish.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.963124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/comments/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/comments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/comments/author.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/comments/comment_sheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/comments/comments.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/comments/shape_writer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.963124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/compat/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/compat/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/compat/product.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/compat/singleton.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/compat/strings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.963124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12295 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/nested.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/sequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/serialisable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/slots.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.967124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17638 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/connector.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/effect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/fill.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/graphic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/line.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/xdr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.967124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/formatting/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/formatting/formatting.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/formatting/rule.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.967124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/formula/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/formula/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/formula/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/formula/translate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.967124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/extended.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/interface.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/relationship.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.971124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25828 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/record.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35189 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:14.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.971124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/reader/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/reader/drawings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/reader/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/reader/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/reader/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.971124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/alignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/borders.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/builtins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/cell_style.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/differential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/fills.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/named_styles.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/styleable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/stylesheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.975124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/bound_dictionary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/dataframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/escape.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/formulas.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/indexed_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/inference.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/utils/units.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.975124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/child.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/defined_name.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.975124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/external_link/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/external_link/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/external_link/external.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/external_reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/function_group.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/smart_tags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/web.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.979124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/_read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/_reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/_write_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/cell_range.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/cell_watch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/controls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/copier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/datavalidation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/dimensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/formula.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/header_footer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/hyperlink.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/ole.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/page.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/pagebreak.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/related.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/scenario.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/smart_tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/worksheet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.979124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/writer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/writer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/writer/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/writer/theme.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.979124 types-openpyxl-3.1.2.20240601/openpyxl-stubs/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/xml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/xml/_functions_overloads.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/xml/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-06-01 02:27:05.000000 types-openpyxl-3.1.2.20240601/openpyxl-stubs/xml/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 02:27:15.979124 types-openpyxl-3.1.2.20240601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-06-01 02:27:14.000000 types-openpyxl-3.1.2.20240601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:15.979124 types-openpyxl-3.1.2.20240601/types_openpyxl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-06-01 02:27:15.000000 types-openpyxl-3.1.2.20240601/types_openpyxl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-06-01 02:27:15.000000 types-openpyxl-3.1.2.20240601/types_openpyxl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 02:27:15.000000 types-openpyxl-3.1.2.20240601/types_openpyxl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-01 02:27:15.000000 types-openpyxl-3.1.2.20240601/types_openpyxl.egg-info/top_level.txt
```

### Comparing `types-openpyxl-3.1.0.9/PKG-INFO` & `types-openpyxl-3.1.2.20240601/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.9
+Version: 3.1.2.20240601
 Summary: Typing stubs for openpyxl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for openpyxl
 
-This is a PEP 561 type stub package for the `openpyxl` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`openpyxl`](https://foss.heptapod.net/openpyxl/openpyxl) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`openpyxl`. The source for this package can be found at
+`openpyxl`.
+
+This version of `types-openpyxl` aims to provide accurate annotations
+for `openpyxl==3.1.2`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8c582c4459cc3e7c67531cd90bfd6cef5b71c7d3`.
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
+pytype 2024.4.11.
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/cell/cell.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/read_only.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,70 @@
 from _typeshed import Incomplete
-from datetime import date, datetime, time, timedelta
-from decimal import Decimal
-from typing import overload
-from typing_extensions import TypeAlias
+from typing import Final
 
-from openpyxl.cell.rich_text import CellRichText
-from openpyxl.comments.comments import Comment
+from openpyxl.cell import _CellValue
+from openpyxl.styles.alignment import Alignment
+from openpyxl.styles.borders import Border
 from openpyxl.styles.cell_style import StyleArray
-from openpyxl.styles.styleable import StyleableObject
-from openpyxl.worksheet.formula import ArrayFormula, DataTableFormula
-from openpyxl.worksheet.hyperlink import Hyperlink
-from openpyxl.worksheet.worksheet import Worksheet
-
-_CellValue: TypeAlias = (  # if numpy is installed also numpy bool and number types
-    bool | float | Decimal | str | CellRichText | date | time | timedelta | DataTableFormula | ArrayFormula
-)
-
-__docformat__: str
-TIME_TYPES: Incomplete
-TIME_FORMATS: Incomplete
-STRING_TYPES: Incomplete
-KNOWN_TYPES: Incomplete
-ILLEGAL_CHARACTERS_RE: Incomplete
-ERROR_CODES: Incomplete
-TYPE_STRING: str
-TYPE_FORMULA: str
-TYPE_NUMERIC: str
-TYPE_BOOL: str
-TYPE_NULL: str
-TYPE_INLINE: str
-TYPE_ERROR: str
-TYPE_FORMULA_CACHE_STRING: str
-VALID_TYPES: Incomplete
-
-def get_type(t: type, value: object) -> str | None: ...
-def get_time_format(t: datetime) -> str: ...
-
-class Cell(StyleableObject):
-    row: int
-    column: int
-    data_type: str
+from openpyxl.styles.fills import Fill
+from openpyxl.styles.fonts import Font
+from openpyxl.styles.protection import Protection
+from openpyxl.workbook.child import _WorkbookChild
+from openpyxl.worksheet._read_only import ReadOnlyWorksheet
+
+class ReadOnlyCell:
+    parent: _WorkbookChild | ReadOnlyWorksheet
+    row: Incomplete
+    column: Incomplete
+    data_type: Incomplete
     def __init__(
-        self,
-        worksheet: Worksheet,
-        row: int | None = None,
-        column: int | None = None,
-        value: str | float | datetime | None = None,
-        style_array: StyleArray | None = None,
+        self, sheet: _WorkbookChild | ReadOnlyWorksheet, row, column, value, data_type: str = "n", style_id: int = 0
     ) -> None: ...
+    def __eq__(self, other: object) -> bool: ...
+    def __ne__(self, other: object) -> bool: ...
+    # Same as Cell.coordinate
+    # https://github.com/python/mypy/issues/6700
+    # Defined twice in the implementation
     @property
     def coordinate(self) -> str: ...
-    @property
-    def col_idx(self) -> int: ...
+    # Same as Cell.column_letter
+    # https://github.com/python/mypy/issues/6700
     @property
     def column_letter(self) -> str: ...
     @property
-    def encoding(self) -> str: ...
+    def style_array(self) -> StyleArray: ...
     @property
-    def base_date(self) -> datetime: ...
-    @overload
-    def check_string(self, value: None) -> None: ...
-    @overload
-    def check_string(self, value: str | bytes) -> str: ...
-    def check_error(self, value: object) -> str: ...
+    def has_style(self) -> bool: ...
     @property
-    def value(self) -> _CellValue: ...
-    @value.setter
-    def value(self, value: _CellValue | bytes | None) -> None: ...
+    def number_format(self) -> str: ...
     @property
-    def internal_value(self) -> _CellValue: ...
+    def font(self) -> Font: ...
     @property
-    def hyperlink(self) -> Hyperlink | None: ...
-    @hyperlink.setter
-    def hyperlink(self, val: Hyperlink | str | None) -> None: ...
+    def fill(self) -> Fill: ...
+    @property
+    def border(self) -> Border: ...
+    @property
+    def alignment(self) -> Alignment: ...
+    @property
+    def protection(self) -> Protection: ...
+    # Same as Cell.is_date
+    # https://github.com/python/mypy/issues/6700
     @property
     def is_date(self) -> bool: ...
-    def offset(self, row: int = 0, column: int = 0) -> Cell: ...
     @property
-    def comment(self) -> Comment | None: ...
-    @comment.setter
-    def comment(self, value: Comment | None) -> None: ...
+    def internal_value(self) -> _CellValue | None: ...
+    @property
+    def value(self) -> _CellValue | None: ...
+    @value.setter
+    def value(self, value: None) -> None: ...
 
-class MergedCell(StyleableObject):
+class EmptyCell:
+    value: Incomplete
+    is_date: bool
+    font: Incomplete
+    border: Incomplete
+    fill: Incomplete
+    number_format: Incomplete
+    alignment: Incomplete
     data_type: str
-    comment: Comment | None
-    hyperlink: Hyperlink | None
-    row: int
-    column: int
-    def __init__(self, worksheet: Worksheet, row: int | None = None, column: int | None = None) -> None: ...
-    @property
-    def coordinate(self) -> str: ...
-    value: str | float | int | datetime | None
 
-def WriteOnlyCell(ws: Worksheet | None = None, value: str | float | datetime | None = None) -> Cell: ...
+EMPTY_CELL: Final[EmptyCell]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/cell/rich_text.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/rich_text.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from collections.abc import Iterable
-from typing import overload
-from typing_extensions import Literal, Self
+from typing import Literal, overload
+from typing_extensions import Self
 
 from openpyxl.cell.text import InlineFont
 from openpyxl.descriptors import Strict, String, Typed
+from openpyxl.descriptors.serialisable import _ChildSerialisableTreeElement
 
 class TextBlock(Strict):
     font: Typed[InlineFont, Literal[False]]
     text: String[Literal[False]]
 
     def __init__(self, font: InlineFont, text: str) -> None: ...
     def __eq__(self, other: TextBlock) -> bool: ...  # type: ignore[override]
 
 class CellRichText(list[str | TextBlock]):
     @overload
-    def __init__(self, __args: list[str] | list[TextBlock] | list[str | TextBlock] | tuple[str | TextBlock, ...]) -> None: ...
+    def __init__(self, args: list[str] | list[TextBlock] | list[str | TextBlock] | tuple[str | TextBlock, ...], /) -> None: ...
     @overload
     def __init__(self, *args: str | TextBlock) -> None: ...
     @classmethod
-    def from_tree(cls, node) -> Self: ...
+    def from_tree(cls, node: _ChildSerialisableTreeElement) -> Self: ...
     def __add__(self, arg: Iterable[str | TextBlock]) -> CellRichText: ...  # type: ignore[override]
     def append(self, arg: str | TextBlock) -> None: ...
     def extend(self, arg: Iterable[str | TextBlock]) -> None: ...
     def as_list(self) -> list[str]: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/cell/text.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/extended.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,94 +1,83 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Unused
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors.base import Alias, Integer, NoneSet, Typed, _ConvertibleToInt
-from openpyxl.descriptors.nested import NestedString, NestedText
+from openpyxl.descriptors.base import Typed
+from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.styles.fonts import Font
+from openpyxl.xml.functions import Element
 
-_PhoneticPropertiesType: TypeAlias = Literal["halfwidthKatakana", "fullwidthKatakana", "Hiragana", "noConversion"]
-_PhoneticPropertiesAlignment: TypeAlias = Literal["noControl", "left", "center", "distributed"]
+def get_version(): ...
 
-class PhoneticProperties(Serialisable):
-    tagname: str
-    fontId: Integer[Literal[False]]
-    type: NoneSet[_PhoneticPropertiesType]
-    alignment: NoneSet[_PhoneticPropertiesAlignment]
-    def __init__(
-        self,
-        fontId: _ConvertibleToInt,
-        type: _PhoneticPropertiesType | Literal["none"] | None = None,
-        alignment: _PhoneticPropertiesAlignment | Literal["none"] | None = None,
-    ) -> None: ...
-
-_PhoneticProperties: TypeAlias = PhoneticProperties
+class DigSigBlob(Serialisable):
+    __elements__: ClassVar[tuple[str, ...]]
+    __attrs__: ClassVar[tuple[str, ...]]
 
-class PhoneticText(Serialisable):
-    tagname: str
-    sb: Integer[Literal[False]]
-    eb: Integer[Literal[False]]
-    t: NestedText[str, Literal[False]]
-    text: Alias
-    def __init__(self, sb: _ConvertibleToInt, eb: _ConvertibleToInt, t: object = None) -> None: ...
-
-class InlineFont(Font):
-    tagname: str
-    rFont: NestedString[Literal[True]]
-    charset: Incomplete
-    family: Incomplete
-    b: Incomplete
-    i: Incomplete
-    strike: Incomplete
-    outline: Incomplete
-    shadow: Incomplete
-    condense: Incomplete
-    extend: Incomplete
-    color: Incomplete
-    sz: Incomplete
-    u: Incomplete
-    vertAlign: Incomplete
-    scheme: Incomplete
+class VectorLpstr(Serialisable):
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(
-        self,
-        rFont: object = None,
-        charset: Incomplete | None = None,
-        family: Incomplete | None = None,
-        b: Incomplete | None = None,
-        i: Incomplete | None = None,
-        strike: Incomplete | None = None,
-        outline: Incomplete | None = None,
-        shadow: Incomplete | None = None,
-        condense: Incomplete | None = None,
-        extend: Incomplete | None = None,
-        color: Incomplete | None = None,
-        sz: Incomplete | None = None,
-        u: Incomplete | None = None,
-        vertAlign: Incomplete | None = None,
-        scheme: Incomplete | None = None,
-    ) -> None: ...
+    __attrs__: ClassVar[tuple[str, ...]]
 
-class RichText(Serialisable):
-    tagname: str
-    rPr: Typed[InlineFont, Literal[True]]
-    font: Alias
-    t: NestedText[str, Literal[True]]
-    text: Alias
+class VectorVariant(Serialisable):
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, rPr: InlineFont | None = None, t: object = None) -> None: ...
+    __attrs__: ClassVar[tuple[str, ...]]
 
-class Text(Serialisable):
-    tagname: str
-    t: NestedText[str, Literal[True]]
-    plain: Alias
-    r: Incomplete
-    formatted: Alias
-    rPh: Incomplete
-    phonetic: Alias
-    phoneticPr: Typed[_PhoneticProperties, Literal[True]]
-    PhoneticProperties: Alias
+class ExtendedProperties(Serialisable):
+    tagname: ClassVar[str]
+    Template: NestedText[str, Literal[True]]
+    Manager: NestedText[str, Literal[True]]
+    Company: NestedText[str, Literal[True]]
+    Pages: NestedText[int, Literal[True]]
+    Words: NestedText[int, Literal[True]]
+    Characters: NestedText[int, Literal[True]]
+    PresentationFormat: NestedText[str, Literal[True]]
+    Lines: NestedText[int, Literal[True]]
+    Paragraphs: NestedText[int, Literal[True]]
+    Slides: NestedText[int, Literal[True]]
+    Notes: NestedText[int, Literal[True]]
+    TotalTime: NestedText[int, Literal[True]]
+    HiddenSlides: NestedText[int, Literal[True]]
+    MMClips: NestedText[int, Literal[True]]
+    ScaleCrop: NestedText[str, Literal[True]]
+    HeadingPairs: Typed[VectorVariant, Literal[True]]
+    TitlesOfParts: Typed[VectorLpstr, Literal[True]]
+    LinksUpToDate: NestedText[str, Literal[True]]
+    CharactersWithSpaces: NestedText[int, Literal[True]]
+    SharedDoc: NestedText[str, Literal[True]]
+    HyperlinkBase: NestedText[str, Literal[True]]
+    HLinks: Typed[VectorVariant, Literal[True]]
+    HyperlinksChanged: NestedText[str, Literal[True]]
+    DigSig: Typed[DigSigBlob, Literal[True]]
+    Application: NestedText[str, Literal[True]]
+    AppVersion: NestedText[str, Literal[True]]
+    DocSecurity: NestedText[int, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, t: object = None, r=(), rPh=(), phoneticPr: _PhoneticProperties | None = None) -> None: ...
-    @property
-    def content(self): ...
+    def __init__(
+        self,
+        Template: object = None,
+        Manager: object = None,
+        Company: object = None,
+        Pages: ConvertibleToInt | None = None,
+        Words: ConvertibleToInt | None = None,
+        Characters: ConvertibleToInt | None = None,
+        PresentationFormat: object = None,
+        Lines: ConvertibleToInt | None = None,
+        Paragraphs: ConvertibleToInt | None = None,
+        Slides: ConvertibleToInt | None = None,
+        Notes: ConvertibleToInt | None = None,
+        TotalTime: ConvertibleToInt | None = None,
+        HiddenSlides: ConvertibleToInt | None = None,
+        MMClips: ConvertibleToInt | None = None,
+        ScaleCrop: object = None,
+        HeadingPairs: Unused = None,
+        TitlesOfParts: Unused = None,
+        LinksUpToDate: object = None,
+        CharactersWithSpaces: ConvertibleToInt | None = None,
+        SharedDoc: object = None,
+        HyperlinkBase: object = None,
+        HLinks: Unused = None,
+        HyperlinksChanged: object = None,
+        DigSig: Unused = None,
+        Application: object = "Microsoft Excel",
+        AppVersion: object = None,
+        DocSecurity: ConvertibleToInt | None = None,
+    ) -> None: ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/_3d.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/_3d.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-from _typeshed import Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Unused
+from typing import ClassVar, Literal
 
 from openpyxl.chart.picture import PictureOptions
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedMinMax, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedMinMax
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 class View3D(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     rotX: NestedMinMax[float, Literal[True]]
     x_rotation: Alias
     hPercent: NestedMinMax[float, Literal[True]]
     height_percent: Alias
     rotY: NestedInteger[Literal[True]]
     y_rotation: Alias
     depthPercent: NestedInteger[Literal[True]]
     rAngAx: NestedBool[Literal[True]]
     right_angle_axes: Alias
     perspective: NestedInteger[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        rotX: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = 15,
-        hPercent: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        rotY: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = 20,
-        depthPercent: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        rotX: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = 15,
+        hPercent: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        rotY: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = 20,
+        depthPercent: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         rAngAx: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = True,
-        perspective: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        perspective: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class Surface(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     thickness: NestedInteger[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     pictureOptions: Typed[PictureOptions, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        thickness: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        thickness: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         spPr: GraphicalProperties | None = None,
         pictureOptions: PictureOptions | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class _3DBase(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     view3D: Typed[View3D, Literal[True]]
     floor: Typed[Surface, Literal[True]]
     sideWall: Typed[Surface, Literal[True]]
     backWall: Typed[Surface, Literal[True]]
     def __init__(
         self,
         view3D: View3D | None = None,
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/__init__.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/_chart.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-from _typeshed import Incomplete, Unused
-from abc import abstractmethod
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.legend import Legend
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Bool, Integer, MinMax, Set, Typed, _ConvertibleToInt
+from openpyxl.chart.title import TitleDescriptor
+from openpyxl.descriptors.base import Alias, Bool, Integer, MinMax, Set, Typed
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.xml.functions import Element
 
 _ChartBaseDisplayBlanks: TypeAlias = Literal["span", "gap", "zero"]
 
 class AxId(Serialisable):
     val: Integer[Literal[False]]
-    def __init__(self, val: _ConvertibleToInt) -> None: ...
+    def __init__(self, val: ConvertibleToInt) -> None: ...
 
 def PlotArea(): ...
 
 class ChartBase(Serialisable):
     legend: Typed[Legend, Literal[True]]
     layout: Typed[Layout, Literal[True]]
     roundedCorners: Bool[Literal[True]]
     axId: Incomplete
     visible_cells_only: Bool[Literal[True]]
     display_blanks: Set[_ChartBaseDisplayBlanks]
     ser: Incomplete
     series: Alias
-    title: Incomplete
+    title: TitleDescriptor
     anchor: str
     width: int
     height: float
     style: MinMax[float, Literal[True]]
     mime_type: str
     graphical_properties: Typed[GraphicalProperties, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     plot_area: Incomplete
     pivotSource: Incomplete
     pivotFormats: Incomplete
     idx_base: int
     def __init__(self, axId=(), **kw: Unused) -> None: ...
     def __hash__(self) -> int: ...
     def __iadd__(self, other): ...
-    def to_tree(self, namespace: Incomplete | None = None, tagname: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
+    # namespace is in the wrong order to respect the override. This is an issue in openpyxl itself
+    def to_tree(self, namespace: Unused = None, tagname: str | None = None, idx: Unused = None) -> Element: ...  # type: ignore[override]
     def set_categories(self, labels) -> None: ...
     def add_data(self, data, from_rows: bool = False, titles_from_data: bool = False) -> None: ...
     def append(self, value) -> None: ...
     @property
-    def path(self): ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
+    def path(self) -> str: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/area_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/plotarea.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 from _typeshed import Incomplete, Unused
-from abc import abstractmethod
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal
+from typing_extensions import Self
 
-from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
-from openpyxl.chart.label import DataLabelList
+from openpyxl.chart.layout import Layout
+from openpyxl.chart.shapes import GraphicalProperties
+from openpyxl.chart.text import RichText
 from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedSet, _HasTagAndGet
-
-from ._chart import ChartBase
-
-_AreaChartBaseGrouping: TypeAlias = Literal["percentStacked", "standard", "stacked"]
-
-class _AreaChartBase(ChartBase):
-    grouping: NestedSet[_AreaChartBaseGrouping]
-    varyColors: NestedBool[Literal[True]]
-    ser: Incomplete
-    dLbls: Typed[DataLabelList, Literal[True]]
-    dataLabels: Alias
-    dropLines: Typed[ChartLines, Literal[True]]
+from openpyxl.descriptors.nested import NestedBool
+from openpyxl.descriptors.serialisable import Serialisable, _ChildSerialisableTreeElement
+from openpyxl.xml.functions import Element
+
+from ..xml._functions_overloads import _HasTagAndGet
+
+class DataTable(Serialisable):
+    tagname: ClassVar[str]
+    showHorzBorder: NestedBool[Literal[True]]
+    showVertBorder: NestedBool[Literal[True]]
+    showOutline: NestedBool[Literal[True]]
+    showKeys: NestedBool[Literal[True]]
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        grouping: _HasTagAndGet[_AreaChartBaseGrouping] | _AreaChartBaseGrouping = "standard",
-        varyColors: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        ser=(),
-        dLbls: DataLabelList | None = None,
-        dropLines: ChartLines | None = None,
+        showHorzBorder: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showVertBorder: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showOutline: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showKeys: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
+        extLst: Unused = None,
     ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
 
-class AreaChart(_AreaChartBase):
-    tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    x_axis: Typed[TextAxis, Literal[False]]
-    y_axis: Typed[NumericAxis, Literal[False]]
+class PlotArea(Serialisable):
+    tagname: ClassVar[str]
+    layout: Typed[Layout, Literal[True]]
+    dTable: Typed[DataTable, Literal[True]]
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
+    areaChart: Incomplete
+    area3DChart: Incomplete
+    lineChart: Incomplete
+    line3DChart: Incomplete
+    stockChart: Incomplete
+    radarChart: Incomplete
+    scatterChart: Incomplete
+    pieChart: Incomplete
+    pie3DChart: Incomplete
+    doughnutChart: Incomplete
+    barChart: Incomplete
+    bar3DChart: Incomplete
+    ofPieChart: Incomplete
+    surfaceChart: Incomplete
+    surface3DChart: Incomplete
+    bubbleChart: Incomplete
+    valAx: Incomplete
+    catAx: Incomplete
+    dateAx: Incomplete
+    serAx: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, axId: Unused = None, extLst: Unused = None, **kw) -> None: ...
-
-class AreaChart3D(AreaChart):
-    tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
-    gapDepth: Incomplete
-    x_axis: Typed[TextAxis, Literal[False]]
-    y_axis: Typed[NumericAxis, Literal[False]]
-    z_axis: Typed[SeriesAxis, Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, gapDepth: Incomplete | None = None, **kw) -> None: ...
+    def __init__(
+        self,
+        layout: Layout | None = None,
+        dTable: DataTable | None = None,
+        spPr: GraphicalProperties | None = None,
+        _charts=(),
+        _axes=(),
+        extLst: Unused = None,
+    ) -> None: ...
+    def to_tree(self, tagname: str | None = None, idx: Unused = None, namespace: Unused = None) -> Element: ...
+    @classmethod
+    def from_tree(cls, node: _ChildSerialisableTreeElement) -> Self: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/axis.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/axis.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from _typeshed import Incomplete, Unused
-from abc import abstractmethod
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal, overload
+from typing_extensions import Self, TypeAlias
 
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText, Text
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
+from openpyxl.chart.title import Title, TitleDescriptor
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.nested import (
     NestedBool,
     NestedFloat,
     NestedInteger,
     NestedMinMax,
     NestedNoneSet,
     NestedSet,
-    _HasTagAndGet,
     _NestedNoneSetParam,
 )
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet, _SupportsFindAndIterAndAttribAndText
+
 _ScalingOrientation: TypeAlias = Literal["maxMin", "minMax"]
 _BaseAxisAxPos: TypeAlias = Literal["b", "l", "r", "t"]
 _BaseAxisTickMark: TypeAlias = Literal["cross", "in", "out"]
 _BaseAxisTickLblPos: TypeAlias = Literal["high", "low", "nextTo"]
 _BaseAxisCrosses: TypeAlias = Literal["autoZero", "max", "min"]
 _DisplayUnitsLabelListBuiltInUnit: TypeAlias = Literal[
     "hundreds",
@@ -37,44 +38,44 @@
     "trillions",
 ]
 _NumericAxisCrossBetween: TypeAlias = Literal["between", "midCat"]
 _TextAxisLblAlgn: TypeAlias = Literal["ctr", "l", "r"]
 _DateAxisTimeUnit: TypeAlias = Literal["days", "months", "years"]
 
 class ChartLines(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     def __init__(self, spPr: GraphicalProperties | None = None) -> None: ...
 
 class Scaling(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     logBase: NestedFloat[Literal[True]]
     orientation: NestedSet[_ScalingOrientation]
     max: NestedFloat[Literal[True]]
     min: NestedFloat[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        logBase: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        logBase: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         orientation: _HasTagAndGet[_ScalingOrientation] | _ScalingOrientation = "minMax",
-        max: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        min: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        max: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        min: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class _BaseAxis(Serialisable):
     axId: NestedInteger[Literal[False]]
     scaling: Typed[Scaling, Literal[False]]
     delete: NestedBool[Literal[True]]
     axPos: NestedSet[_BaseAxisAxPos]
     majorGridlines: Typed[ChartLines, Literal[True]]
     minorGridlines: Typed[ChartLines, Literal[True]]
-    title: Incomplete
+    title: TitleDescriptor
     numFmt: Incomplete
     number_format: Alias
     majorTickMark: NestedNoneSet[_BaseAxisTickMark]
     minorTickMark: NestedNoneSet[_BaseAxisTickMark]
     tickLblPos: NestedNoneSet[_BaseAxisTickLblPos]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
@@ -83,58 +84,55 @@
     crossAx: NestedInteger[Literal[False]]
     crosses: NestedNoneSet[_BaseAxisCrosses]
     crossesAt: NestedFloat[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
-        axId: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt,
+        axId: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt,
         scaling: Scaling | None,
         delete: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None,
         axPos: _HasTagAndGet[_BaseAxisAxPos] | _BaseAxisAxPos,
         majorGridlines: ChartLines | None,
         minorGridlines: ChartLines | None,
-        title: Incomplete | None,
+        title: str | Title | None,
         numFmt: Incomplete | None,
         majorTickMark: _NestedNoneSetParam[_BaseAxisTickMark],
         minorTickMark: _NestedNoneSetParam[_BaseAxisTickMark],
         tickLblPos: _NestedNoneSetParam[_BaseAxisTickLblPos],
         spPr: GraphicalProperties | None,
         txPr: RichText | None,
-        crossAx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt,
+        crossAx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt,
         crosses: _NestedNoneSetParam[_BaseAxisCrosses] = None,
-        crossesAt: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        crossesAt: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        axId: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt,
+        axId: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt,
         scaling: Scaling | None = None,
         delete: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         axPos: _HasTagAndGet[_BaseAxisAxPos] | _BaseAxisAxPos = "l",
         majorGridlines: ChartLines | None = None,
         minorGridlines: ChartLines | None = None,
-        title: Incomplete | None = None,
+        title: str | Title | None = None,
         numFmt: Incomplete | None = None,
         majorTickMark: Incomplete | None = None,
         minorTickMark: Incomplete | None = None,
         tickLblPos: Incomplete | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
         *,
-        crossAx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt,
+        crossAx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt,
         crosses: Incomplete | None = None,
-        crossesAt: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        crossesAt: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
     ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
 
 class DisplayUnitsLabel(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     layout: Typed[Layout, Literal[True]]
     tx: Typed[Text, Literal[True]]
     text: Alias
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
     textPropertes: Alias
@@ -144,167 +142,170 @@
         layout: Layout | None = None,
         tx: Text | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
     ) -> None: ...
 
 class DisplayUnitsLabelList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     custUnit: NestedFloat[Literal[True]]
     builtInUnit: NestedNoneSet[_DisplayUnitsLabelListBuiltInUnit]
     dispUnitsLbl: Typed[DisplayUnitsLabel, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        custUnit: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        builtInUnit: _HasTagAndGet[_DisplayUnitsLabelListBuiltInUnit]
-        | _DisplayUnitsLabelListBuiltInUnit
-        | Literal["none"]
-        | None = None,
+        custUnit: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        builtInUnit: (
+            _HasTagAndGet[_DisplayUnitsLabelListBuiltInUnit] | _DisplayUnitsLabelListBuiltInUnit | Literal["none"] | None
+        ) = None,
         dispUnitsLbl: DisplayUnitsLabel | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class NumericAxis(_BaseAxis):
-    tagname: str
-    axId: Incomplete
-    scaling: Incomplete
-    delete: Incomplete
-    axPos: Incomplete
-    majorGridlines: Incomplete
-    minorGridlines: Incomplete
-    title: Incomplete
-    numFmt: Incomplete
-    majorTickMark: Incomplete
-    minorTickMark: Incomplete
-    tickLblPos: Incomplete
-    spPr: Incomplete
-    txPr: Incomplete
-    crossAx: Incomplete
-    crosses: Incomplete
-    crossesAt: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent
+    # axId = _BaseAxis.axId
+    # scaling = _BaseAxis.scaling
+    # delete = _BaseAxis.delete
+    # axPos = _BaseAxis.axPos
+    # majorGridlines = _BaseAxis.majorGridlines
+    # minorGridlines = _BaseAxis.minorGridlines
+    # title = _BaseAxis.title
+    # numFmt = _BaseAxis.numFmt
+    # majorTickMark = _BaseAxis.majorTickMark
+    # minorTickMark = _BaseAxis.minorTickMark
+    # tickLblPos = _BaseAxis.tickLblPos
+    # spPr = _BaseAxis.spPr
+    # txPr = _BaseAxis.txPr
+    # crossAx = _BaseAxis.crossAx
+    # crosses = _BaseAxis.crosses
+    # crossesAt = _BaseAxis.crossesAt
     crossBetween: NestedNoneSet[_NumericAxisCrossBetween]
     majorUnit: NestedFloat[Literal[True]]
     minorUnit: NestedFloat[Literal[True]]
     dispUnits: Typed[DisplayUnitsLabelList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         crossBetween: _NestedNoneSetParam[_NumericAxisCrossBetween] = None,
-        majorUnit: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        minorUnit: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        majorUnit: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        minorUnit: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         dispUnits: DisplayUnitsLabelList | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
     @classmethod
-    def from_tree(cls, node): ...
+    def from_tree(cls, node: _SupportsFindAndIterAndAttribAndText) -> Self: ...
 
 class TextAxis(_BaseAxis):
-    tagname: str
-    axId: Incomplete
-    scaling: Incomplete
-    delete: Incomplete
-    axPos: Incomplete
-    majorGridlines: Incomplete
-    minorGridlines: Incomplete
-    title: Incomplete
-    numFmt: Incomplete
-    majorTickMark: Incomplete
-    minorTickMark: Incomplete
-    tickLblPos: Incomplete
-    spPr: Incomplete
-    txPr: Incomplete
-    crossAx: Incomplete
-    crosses: Incomplete
-    crossesAt: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent
+    # axId = _BaseAxis.axId
+    # scaling = _BaseAxis.scaling
+    # delete = _BaseAxis.delete
+    # axPos = _BaseAxis.axPos
+    # majorGridlines = _BaseAxis.majorGridlines
+    # minorGridlines = _BaseAxis.minorGridlines
+    # title = _BaseAxis.title
+    # numFmt = _BaseAxis.numFmt
+    # majorTickMark = _BaseAxis.majorTickMark
+    # minorTickMark = _BaseAxis.minorTickMark
+    # tickLblPos = _BaseAxis.tickLblPos
+    # spPr = _BaseAxis.spPr
+    # txPr = _BaseAxis.txPr
+    # crossAx = _BaseAxis.crossAx
+    # crosses = _BaseAxis.crosses
+    # crossesAt = _BaseAxis.crossesAt
     auto: NestedBool[Literal[True]]
     lblAlgn: NestedNoneSet[_TextAxisLblAlgn]
     lblOffset: NestedMinMax[float, Literal[False]]
     tickLblSkip: NestedInteger[Literal[True]]
     tickMarkSkip: NestedInteger[Literal[True]]
     noMultiLvlLbl: NestedBool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         auto: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         lblAlgn: _NestedNoneSetParam[_TextAxisLblAlgn] = None,
-        lblOffset: _HasTagAndGet[_ConvertibleToFloat] | _ConvertibleToFloat = 100,
-        tickLblSkip: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        tickMarkSkip: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        lblOffset: _HasTagAndGet[ConvertibleToFloat] | ConvertibleToFloat = 100,
+        tickLblSkip: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        tickMarkSkip: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         noMultiLvlLbl: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
 
 class DateAxis(TextAxis):
-    tagname: str
-    axId: Incomplete
-    scaling: Incomplete
-    delete: Incomplete
-    axPos: Incomplete
-    majorGridlines: Incomplete
-    minorGridlines: Incomplete
-    title: Incomplete
-    numFmt: Incomplete
-    majorTickMark: Incomplete
-    minorTickMark: Incomplete
-    tickLblPos: Incomplete
-    spPr: Incomplete
-    txPr: Incomplete
-    crossAx: Incomplete
-    crosses: Incomplete
-    crossesAt: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent and grandparent
+    # axId = _BaseAxis.axId
+    # scaling = _BaseAxis.scaling
+    # delete = _BaseAxis.delete
+    # axPos = _BaseAxis.axPos
+    # majorGridlines = _BaseAxis.majorGridlines
+    # minorGridlines = _BaseAxis.minorGridlines
+    # title = _BaseAxis.title
+    # numFmt = _BaseAxis.numFmt
+    # majorTickMark = _BaseAxis.majorTickMark
+    # minorTickMark = _BaseAxis.minorTickMark
+    # tickLblPos = _BaseAxis.tickLblPos
+    # spPr = _BaseAxis.spPr
+    # txPr = _BaseAxis.txPr
+    # crossAx = _BaseAxis.crossAx
+    # crosses = _BaseAxis.crosses
+    # crossesAt = _BaseAxis.crossesAt
     auto: NestedBool[Literal[True]]
     lblOffset: NestedInteger[Literal[True]]  # type: ignore[assignment]
     baseTimeUnit: NestedNoneSet[_DateAxisTimeUnit]
     majorUnit: NestedFloat[Literal[True]]
     majorTimeUnit: NestedNoneSet[_DateAxisTimeUnit]
     minorUnit: NestedFloat[Literal[True]]
     minorTimeUnit: NestedNoneSet[_DateAxisTimeUnit]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         auto: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        lblOffset: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        lblOffset: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         baseTimeUnit: _NestedNoneSetParam[_DateAxisTimeUnit] = None,
-        majorUnit: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        majorUnit: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         majorTimeUnit: _NestedNoneSetParam[_DateAxisTimeUnit] = None,
-        minorUnit: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        minorUnit: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         minorTimeUnit: _NestedNoneSetParam[_DateAxisTimeUnit] = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
 
 class SeriesAxis(_BaseAxis):
-    tagname: str
-    axId: Incomplete
-    scaling: Incomplete
-    delete: Incomplete
-    axPos: Incomplete
-    majorGridlines: Incomplete
-    minorGridlines: Incomplete
-    title: Incomplete
-    numFmt: Incomplete
-    majorTickMark: Incomplete
-    minorTickMark: Incomplete
-    tickLblPos: Incomplete
-    spPr: Incomplete
-    txPr: Incomplete
-    crossAx: Incomplete
-    crosses: Incomplete
-    crossesAt: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent
+    # axId = _BaseAxis.axId
+    # scaling = _BaseAxis.scaling
+    # delete = _BaseAxis.delete
+    # axPos = _BaseAxis.axPos
+    # majorGridlines = _BaseAxis.majorGridlines
+    # minorGridlines = _BaseAxis.minorGridlines
+    # title = _BaseAxis.title
+    # numFmt = _BaseAxis.numFmt
+    # majorTickMark = _BaseAxis.majorTickMark
+    # minorTickMark = _BaseAxis.minorTickMark
+    # tickLblPos = _BaseAxis.tickLblPos
+    # spPr = _BaseAxis.spPr
+    # txPr = _BaseAxis.txPr
+    # crossAx = _BaseAxis.crossAx
+    # crosses = _BaseAxis.crosses
+    # crossesAt = _BaseAxis.crossesAt
     tickLblSkip: NestedInteger[Literal[True]]
     tickMarkSkip: NestedInteger[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        tickLblSkip: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        tickMarkSkip: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        tickLblSkip: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        tickMarkSkip: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/bar_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/bar_chart.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from _typeshed import Incomplete, Unused
-from abc import abstractmethod
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
 from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedNoneSet, NestedSet, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedBool, NestedNoneSet, NestedSet, _NestedNoneSetParam
 
+from ..xml._functions_overloads import _HasTagAndGet
 from ._3d import _3DBase
 from ._chart import ChartBase
 
 _BarChartBaseBarDir: TypeAlias = Literal["bar", "col"]
 _BarChartBaseGrouping: TypeAlias = Literal["percentStacked", "clustered", "standard", "stacked"]
 _BarChart3DShape: TypeAlias = Literal["cone", "coneToMax", "box", "cylinder", "pyramid", "pyramidToMax"]
 
@@ -30,25 +30,23 @@
         barDir: _HasTagAndGet[_BarChartBaseBarDir] | _BarChartBaseBarDir = "col",
         grouping: _HasTagAndGet[_BarChartBaseGrouping] | _BarChartBaseGrouping = "clustered",
         varyColors: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
         **kw,
     ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
 
 class BarChart(_BarChartBase):
-    tagname: str
-    barDir: Incomplete
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent
+    # barDir = _BarChartBase.barDir
+    # grouping = _BarChartBase.grouping
+    # varyColors = _BarChartBase.varyColors
+    # ser = _BarChartBase.ser
+    # dLbls = _BarChartBase.dLbls
     gapWidth: Incomplete
     overlap: Incomplete
     serLines: Typed[ChartLines, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
@@ -59,24 +57,25 @@
         overlap: Incomplete | None = None,
         serLines: ChartLines | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
 
 class BarChart3D(_BarChartBase, _3DBase):
-    tagname: str
-    barDir: Incomplete
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    view3D: Incomplete
-    floor: Incomplete
-    sideWall: Incomplete
-    backWall: Incomplete
+    tagname: ClassVar[str]
+    # Same as parents
+    # barDir = _BarChartBase.barDir
+    # grouping = _BarChartBase.grouping
+    # varyColors = _BarChartBase.varyColors
+    # ser = _BarChartBase.ser
+    # dLbls = _BarChartBase.dLbls
+    # view3D = _3DBase.view3D
+    # floor = _3DBase.floor
+    # sideWall = _3DBase.sideWall
+    # backWall = _3DBase.backWall
     gapWidth: Incomplete
     gapDepth: Incomplete
     shape: NestedNoneSet[_BarChart3DShape]
     serLines: Typed[ChartLines, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/bubble_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/bubble_chart.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.axis import NumericAxis
 from openpyxl.chart.label import DataLabelList
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToFloat
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedMinMax, NestedNoneSet, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedBool, NestedMinMax, NestedNoneSet, _NestedNoneSetParam
 
+from ..xml._functions_overloads import _HasTagAndGet
 from ._chart import ChartBase
 
 _BubbleChartSizeRepresents: TypeAlias = Literal["area", "w"]
 
 class BubbleChart(ChartBase):
-    tagname: str
+    tagname: ClassVar[str]
     varyColors: NestedBool[Literal[True]]
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
     bubble3D: NestedBool[Literal[True]]
     bubbleScale: NestedMinMax[float, Literal[True]]
     showNegBubbles: NestedBool[Literal[True]]
@@ -28,13 +29,13 @@
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         varyColors: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
         bubble3D: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        bubbleScale: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        bubbleScale: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         showNegBubbles: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         sizeRepresents: _NestedNoneSetParam[_BubbleChartSizeRepresents] = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/chartspace.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/chartspace.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,69 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, Incomplete, Unused
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
+from openpyxl.chart._3d import Surface, View3D
 from openpyxl.chart.legend import Legend
 from openpyxl.chart.pivot import PivotSource
 from openpyxl.chart.plotarea import PlotArea
 from openpyxl.chart.print_settings import PrintSettings
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
 from openpyxl.chart.title import Title
-from openpyxl.descriptors.base import Alias, String, Typed, _ConvertibleToBool, _ConvertibleToFloat
+from openpyxl.descriptors.base import Alias, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedMinMax, NestedNoneSet, NestedString, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedBool, NestedMinMax, NestedNoneSet, NestedString, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.colors import ColorMapping
+from openpyxl.xml.functions import Element
+
+from ..xml._functions_overloads import _HasTagAndGet
 
 _ChartContainerDispBlanksAs: TypeAlias = Literal["span", "gap", "zero"]
 
 class ChartContainer(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     title: Typed[Title, Literal[True]]
     autoTitleDeleted: NestedBool[Literal[True]]
     pivotFmts: Incomplete
-    view3D: Incomplete
-    floor: Incomplete
-    sideWall: Incomplete
-    backWall: Incomplete
+
+    # Same as _3DBase
+    # https://github.com/python/mypy/issues/6700
+    view3D: Typed[View3D, Literal[True]]
+    floor: Typed[Surface, Literal[True]]
+    sideWall: Typed[Surface, Literal[True]]
+    backWall: Typed[Surface, Literal[True]]
+
     plotArea: Typed[PlotArea, Literal[False]]
     legend: Typed[Legend, Literal[True]]
     plotVisOnly: NestedBool[Literal[False]]
     dispBlanksAs: NestedNoneSet[_ChartContainerDispBlanksAs]
     showDLblsOverMax: NestedBool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         title: Title | None = None,
         autoTitleDeleted: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         pivotFmts=(),
-        view3D: Incomplete | None = None,
-        floor: Incomplete | None = None,
-        sideWall: Incomplete | None = None,
-        backWall: Incomplete | None = None,
+        view3D: View3D | None = None,
+        floor: Surface | None = None,
+        sideWall: Surface | None = None,
+        backWall: Surface | None = None,
         plotArea: PlotArea | None = None,
         legend: Legend | None = None,
         plotVisOnly: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = True,
         dispBlanksAs: _NestedNoneSetParam[_ChartContainerDispBlanksAs] = "gap",
         showDLblsOverMax: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class Protection(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     chartObject: NestedBool[Literal[True]]
     data: NestedBool[Literal[True]]
     formatting: NestedBool[Literal[True]]
     selection: NestedBool[Literal[True]]
     userInterface: NestedBool[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
@@ -64,50 +72,50 @@
         data: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         formatting: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         selection: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         userInterface: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class ExternalData(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     autoUpdate: NestedBool[Literal[True]]
     id: String[Literal[False]]
     @overload
     def __init__(
         self, autoUpdate: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None, *, id: str
     ) -> None: ...
     @overload
     def __init__(self, autoUpdate: Incomplete | None, id: str) -> None: ...
 
 class ChartSpace(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     date1904: NestedBool[Literal[True]]
     lang: NestedString[Literal[True]]
     roundedCorners: NestedBool[Literal[True]]
     style: NestedMinMax[float, Literal[True]]
     clrMapOvr: Typed[ColorMapping, Literal[True]]
     pivotSource: Typed[PivotSource, Literal[True]]
     protection: Typed[Protection, Literal[True]]
     chart: Typed[ChartContainer, Literal[False]]
     spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
+    graphical_properties: Alias
     txPr: Typed[RichText, Literal[True]]
     textProperties: Alias
     externalData: Typed[ExternalData, Literal[True]]
     printSettings: Typed[PrintSettings, Literal[True]]
     userShapes: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         date1904: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         lang: object = None,
         roundedCorners: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        style: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        style: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         clrMapOvr: ColorMapping | None = None,
         pivotSource: PivotSource | None = None,
         protection: Protection | None = None,
         *,
         chart: ChartContainer,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
@@ -118,20 +126,20 @@
     ) -> None: ...
     @overload
     def __init__(
         self,
         date1904: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None,
         lang: object,
         roundedCorners: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None,
-        style: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None,
+        style: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None,
         clrMapOvr: ColorMapping | None,
         pivotSource: PivotSource | None,
         protection: Protection | None,
         chart: ChartContainer,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
         externalData: ExternalData | None = None,
         printSettings: PrintSettings | None = None,
         userShapes: Incomplete | None = None,
         extLst: Unused = None,
     ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    def to_tree(self, tagname: Unused = None, idx: Unused = None, namespace: Unused = None) -> Element: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/data_source.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/data_source.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,108 +1,109 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, NoReturn, overload
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal, NoReturn, overload
 
 from openpyxl.descriptors import Strict
-from openpyxl.descriptors.base import Alias, Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedInteger, NestedText, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedInteger, NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 class NumFmt(Serialisable):
     formatCode: String[Literal[False]]
     sourceLinked: Bool[Literal[False]]
     def __init__(self, formatCode: str, sourceLinked: _ConvertibleToBool = False) -> None: ...
 
 class NumberValueDescriptor(NestedText[Incomplete, Incomplete]):
     allow_none: bool
     expected_type: type[Incomplete]
     def __set__(self, instance: Serialisable | Strict, value) -> None: ...  # type: ignore[override]
 
 class NumVal(Serialisable):
     idx: Integer[Literal[False]]
     formatCode: NestedText[str, Literal[True]]
     v: Incomplete
-    def __init__(self, idx: _ConvertibleToInt, formatCode: object = None, v: Incomplete | None = None) -> None: ...
+    def __init__(self, idx: ConvertibleToInt, formatCode: object = None, v: Incomplete | None = None) -> None: ...
 
 class NumData(Serialisable):
     formatCode: NestedText[str, Literal[True]]
     ptCount: NestedInteger[Literal[True]]
     pt: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         formatCode: object = None,
-        ptCount: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        ptCount: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         pt=(),
         extLst: Unused = None,
     ) -> None: ...
 
 class NumRef(Serialisable):
     f: NestedText[str, Literal[False]]
     ref: Alias
     numCache: Typed[NumData, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, f: object = None, numCache: NumData | None = None, extLst: Unused = None) -> None: ...
 
 class StrVal(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     idx: Integer[Literal[False]]
     v: NestedText[str, Literal[False]]
-    def __init__(self, idx: _ConvertibleToInt = 0, v: object = None) -> None: ...
+    def __init__(self, idx: ConvertibleToInt = 0, v: object = None) -> None: ...
 
 class StrData(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ptCount: NestedInteger[Literal[True]]
     pt: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
-        self, ptCount: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None, pt=(), extLst: Unused = None
+        self, ptCount: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None, pt=(), extLst: Unused = None
     ) -> None: ...
 
 class StrRef(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     f: NestedText[str, Literal[True]]
     strCache: Typed[StrData, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, f: object = None, strCache: StrData | None = None, extLst: Unused = None) -> None: ...
 
 class NumDataSource(Serialisable):
     numRef: Typed[NumRef, Literal[True]]
     numLit: Typed[NumData, Literal[True]]
     def __init__(self, numRef: NumRef | None = None, numLit: NumData | None = None) -> None: ...
 
 class Level(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     pt: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, pt=()) -> None: ...
 
 class MultiLevelStrData(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ptCount: Integer[Literal[True]]
     lvl: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, ptCount: _ConvertibleToInt | None = None, lvl=(), extLst: Unused = None) -> None: ...
+    def __init__(self, ptCount: ConvertibleToInt | None = None, lvl=(), extLst: Unused = None) -> None: ...
 
 class MultiLevelStrRef(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     f: NestedText[str, Literal[False]]
     multiLvlStrCache: Typed[MultiLevelStrData, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, f: object = None, multiLvlStrCache: MultiLevelStrData | None = None, extLst: Unused = None) -> None: ...
 
 class AxDataSource(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     numRef: Typed[NumRef, Literal[True]]
     numLit: Typed[NumData, Literal[True]]
     strRef: Typed[StrRef, Literal[True]]
     strLit: Typed[StrData, Literal[True]]
     multiLvlStrRef: Typed[MultiLevelStrRef, Literal[True]]
     @overload
     def __init__(
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/descriptors.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/descriptors.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing_extensions import Literal
+from typing import Literal
 
 from openpyxl.chart.data_source import NumFmt
 from openpyxl.descriptors import Strict, Typed
 from openpyxl.descriptors.nested import NestedMinMax
 from openpyxl.descriptors.serialisable import Serialisable
 
 class NestedGapAmount(NestedMinMax[float, bool]):
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/error_bar.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/error_bar.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from _typeshed import Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.data_source import NumDataSource
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToFloat
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedFloat, NestedNoneSet, NestedSet, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedBool, NestedFloat, NestedNoneSet, NestedSet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _ErrorBarsErrBarType: TypeAlias = Literal["both", "minus", "plus"]
 _ErrorBarsErrValType: TypeAlias = Literal["cust", "fixedVal", "percentage", "stdDev", "stdErr"]
 _ErrorBarsErrDir: TypeAlias = Literal["x", "y"]
 
 class ErrorBars(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     errDir: NestedNoneSet[_ErrorBarsErrDir]
     direction: Alias
     errBarType: NestedSet[_ErrorBarsErrBarType]
     style: Alias
     errValType: NestedSet[_ErrorBarsErrValType]
     size: Alias
     noEndCap: NestedBool[Literal[True]]
@@ -33,11 +35,11 @@
         self,
         errDir: _NestedNoneSetParam[_ErrorBarsErrDir] = None,
         errBarType: _HasTagAndGet[_ErrorBarsErrBarType] | _ErrorBarsErrBarType = "both",
         errValType: _HasTagAndGet[_ErrorBarsErrValType] | _ErrorBarsErrValType = "fixedVal",
         noEndCap: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         plus: NumDataSource | None = None,
         minus: NumDataSource | None = None,
-        val: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        val: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         spPr: GraphicalProperties | None = None,
         extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/label.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/label.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from _typeshed import Incomplete, Unused
-from abc import abstractmethod
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedNoneSet, NestedString, _HasTagAndGet, _NestedNoneSetParam
-from openpyxl.descriptors.serialisable import Serialisable as Serialisable
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedNoneSet, NestedString, _NestedNoneSetParam
+from openpyxl.descriptors.serialisable import Serialisable
+
+from ..xml._functions_overloads import _HasTagAndGet
 
 _DataLabelBaseDLblPos: TypeAlias = Literal["bestFit", "b", "ctr", "inBase", "inEnd", "l", "outEnd", "r", "t"]
 
 class _DataLabelBase(Serialisable):
     numFmt: NestedString[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
@@ -42,51 +43,50 @@
         showSerName: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         showPercent: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         showBubbleSize: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         showLeaderLines: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         separator: object = None,
         extLst: Unused = None,
     ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
 
 class DataLabel(_DataLabelBase):
-    tagname: str
+    tagname: ClassVar[str]
     idx: NestedInteger[Literal[False]]
-    numFmt: Incomplete
-    spPr: Incomplete
-    txPr: Incomplete
-    dLblPos: Incomplete
-    showLegendKey: Incomplete
-    showVal: Incomplete
-    showCatName: Incomplete
-    showSerName: Incomplete
-    showPercent: Incomplete
-    showBubbleSize: Incomplete
-    showLeaderLines: Incomplete
-    separator: Incomplete
-    extLst: Incomplete
+    # Same as parent
+    # numFmt = _DataLabelBase.numFmt
+    # spPr = _DataLabelBase.spPr
+    # txPr = _DataLabelBase.txPr
+    # dLblPos = _DataLabelBase.dLblPos
+    # showLegendKey = _DataLabelBase.showLegendKey
+    # showVal = _DataLabelBase.showVal
+    # showCatName = _DataLabelBase.showCatName
+    # showSerName = _DataLabelBase.showSerName
+    # showPercent = _DataLabelBase.showPercent
+    # showBubbleSize = _DataLabelBase.showBubbleSize
+    # showLeaderLines = _DataLabelBase.showLeaderLines
+    # separator = _DataLabelBase.separator
+    # extLst = _DataLabelBase.extLst
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0, **kw) -> None: ...
+    def __init__(self, idx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt = 0, **kw) -> None: ...
 
 class DataLabelList(_DataLabelBase):
-    tagname: str
+    tagname: ClassVar[str]
     dLbl: Incomplete
     delete: NestedBool[Literal[True]]
-    numFmt: Incomplete
-    spPr: Incomplete
-    txPr: Incomplete
-    dLblPos: Incomplete
-    showLegendKey: Incomplete
-    showVal: Incomplete
-    showCatName: Incomplete
-    showSerName: Incomplete
-    showPercent: Incomplete
-    showBubbleSize: Incomplete
-    showLeaderLines: Incomplete
-    separator: Incomplete
-    extLst: Incomplete
+    # Same as parent
+    # numFmt = _DataLabelBase.numFmt
+    # spPr = _DataLabelBase.spPr
+    # txPr = _DataLabelBase.txPr
+    # dLblPos = _DataLabelBase.dLblPos
+    # showLegendKey = _DataLabelBase.showLegendKey
+    # showVal = _DataLabelBase.showVal
+    # showCatName = _DataLabelBase.showCatName
+    # showSerName = _DataLabelBase.showSerName
+    # showPercent = _DataLabelBase.showPercent
+    # showBubbleSize = _DataLabelBase.showBubbleSize
+    # showLeaderLines = _DataLabelBase.showLeaderLines
+    # separator = _DataLabelBase.separator
+    # extLst = _DataLabelBase.extLst
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, dLbl=(), delete: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None, **kw
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/layout.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/layout.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from _typeshed import Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToFloat
+from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedMinMax, NestedNoneSet, NestedSet, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedMinMax, NestedNoneSet, NestedSet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _ManualLayoutMode: TypeAlias = Literal["edge", "factor"]
 _ManualLayoutLayoutTarget: TypeAlias = Literal["inner", "outer"]
 
 class ManualLayout(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     layoutTarget: NestedNoneSet[_ManualLayoutLayoutTarget]
     xMode: NestedNoneSet[_ManualLayoutMode]
     yMode: NestedNoneSet[_ManualLayoutMode]
     wMode: NestedSet[_ManualLayoutMode]
     hMode: NestedSet[_ManualLayoutMode]
     x: NestedMinMax[float, Literal[True]]
     y: NestedMinMax[float, Literal[True]]
@@ -28,20 +30,20 @@
     def __init__(
         self,
         layoutTarget: _NestedNoneSetParam[_ManualLayoutLayoutTarget] = None,
         xMode: _NestedNoneSetParam[_ManualLayoutMode] = None,
         yMode: _NestedNoneSetParam[_ManualLayoutMode] = None,
         wMode: _HasTagAndGet[_ManualLayoutMode] | _ManualLayoutMode = "factor",
         hMode: _HasTagAndGet[_ManualLayoutMode] | _ManualLayoutMode = "factor",
-        x: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        y: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        w: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        h: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        x: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        y: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        w: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        h: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class Layout(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     manualLayout: Typed[ManualLayout, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, manualLayout: ManualLayout | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/legend.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/legend.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedSet, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedSet
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _LegendLegendPos: TypeAlias = Literal["b", "tr", "l", "r", "t"]
 
 class LegendEntry(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     idx: NestedInteger[Literal[False]]
     delete: NestedBool[Literal[False]]
     txPr: Typed[RichText, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0,
+        idx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt = 0,
         delete: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = False,
         txPr: RichText | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class Legend(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     legendPos: NestedSet[_LegendLegendPos]
     position: Alias
     legendEntry: Incomplete
     layout: Typed[Layout, Literal[True]]
     overlay: NestedBool[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/line_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/line_chart.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from _typeshed import Incomplete, Unused
-from abc import abstractmethod
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.axis import ChartLines, NumericAxis, _BaseAxis
 from openpyxl.chart.label import DataLabelList
 from openpyxl.chart.updown_bars import UpDownBars
 from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedSet, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedBool, NestedSet
 
+from ..xml._functions_overloads import _HasTagAndGet
 from ._chart import ChartBase
 
 _LineChartBaseGrouping: TypeAlias = Literal["percentStacked", "standard", "stacked"]
 
 class _LineChartBase(ChartBase):
     grouping: NestedSet[_LineChartBaseGrouping]
     varyColors: NestedBool[Literal[True]]
@@ -27,25 +27,23 @@
         grouping: _HasTagAndGet[_LineChartBaseGrouping] | _LineChartBaseGrouping = "standard",
         varyColors: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
         dropLines: ChartLines | None = None,
         **kw,
     ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
 
 class LineChart(_LineChartBase):
-    tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent
+    # grouping = _LineChartBase.grouping
+    # varyColors = _LineChartBase.varyColors
+    # ser = _LineChartBase.ser
+    # dLbls = _LineChartBase.dLbls
+    # dropLines = _LineChartBase.dropLines
     hiLowLines: Typed[ChartLines, Literal[True]]
     upDownBars: Typed[UpDownBars, Literal[True]]
     marker: NestedBool[Literal[True]]
     smooth: NestedBool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[_BaseAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
@@ -57,20 +55,21 @@
         marker: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         smooth: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
 
 class LineChart3D(_LineChartBase):
-    tagname: str
-    grouping: Incomplete
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    dropLines: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent
+    # grouping = _LineChartBase.grouping
+    # varyColors = _LineChartBase.varyColors
+    # ser = _LineChartBase.ser
+    # dLbls = _LineChartBase.dLbls
+    # dropLines = _LineChartBase.dropLines
     gapDepth: Incomplete
     hiLowLines: Typed[ChartLines, Literal[True]]
     upDownBars: Typed[UpDownBars, Literal[True]]
     marker: NestedBool[Literal[True]]
     smooth: NestedBool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[ExtensionList, Literal[False]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/marker.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/marker.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-from _typeshed import Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.picture import PictureOptions
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedMinMax, NestedNoneSet, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedMinMax, NestedNoneSet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _MarkerSymbol: TypeAlias = Literal[
     "circle", "dash", "diamond", "dot", "picture", "plus", "square", "star", "triangle", "x", "auto"
 ]
 
 class Marker(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     symbol: NestedNoneSet[_MarkerSymbol]
     size: NestedMinMax[float, Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         symbol: _NestedNoneSetParam[_MarkerSymbol] = None,
-        size: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        size: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
         spPr: GraphicalProperties | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class DataPoint(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     idx: NestedInteger[Literal[False]]
     invertIfNegative: NestedBool[Literal[True]]
     marker: Typed[Marker, Literal[True]]
     bubble3D: NestedBool[Literal[True]]
     explosion: NestedInteger[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     pictureOptions: Typed[PictureOptions, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt,
+        idx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt,
         invertIfNegative: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         marker: Marker | None = None,
         bubble3D: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        explosion: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        explosion: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         spPr: GraphicalProperties | None = None,
         pictureOptions: PictureOptions | None = None,
         extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/picture.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/picture.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import _ConvertibleToBool, _ConvertibleToFloat
-from openpyxl.descriptors.nested import NestedBool, NestedFloat, NestedNoneSet, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.base import _ConvertibleToBool
+from openpyxl.descriptors.nested import NestedBool, NestedFloat, NestedNoneSet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _PictureOptionsPictureFormat: TypeAlias = Literal["stretch", "stack", "stackScale"]
 
 class PictureOptions(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     applyToFront: NestedBool[Literal[True]]
     applyToSides: NestedBool[Literal[True]]
     applyToEnd: NestedBool[Literal[True]]
     pictureFormat: NestedNoneSet[_PictureOptionsPictureFormat]
     pictureStackUnit: NestedFloat[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         applyToFront: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         applyToSides: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         applyToEnd: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         pictureFormat: _NestedNoneSetParam[_PictureOptionsPictureFormat] = None,
-        pictureStackUnit: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        pictureStackUnit: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/pivot.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/pivot.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-from _typeshed import Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Unused
+from typing import ClassVar, Literal, overload
 
 from openpyxl.chart.label import DataLabel as _DataLabel
 from openpyxl.chart.marker import Marker
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedInteger, NestedText, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedInteger, NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 class PivotSource(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: NestedText[str, Literal[False]]
     fmtId: NestedInteger[Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
-        self, name: object, fmtId: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt, extLst: Unused = None
+        self, name: object, fmtId: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt, extLst: Unused = None
     ) -> None: ...
     @overload
     def __init__(
-        self, name: object = None, *, fmtId: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt, extLst: Unused = None
+        self, name: object = None, *, fmtId: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt, extLst: Unused = None
     ) -> None: ...
 
 class PivotFormat(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     idx: NestedInteger[Literal[False]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
     TextBody: Alias
     marker: Typed[Marker, Literal[True]]
     dLbl: Typed[_DataLabel, Literal[True]]
     DataLabel: Alias
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0,
+        idx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt = 0,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
         marker: Marker | None = None,
         dLbl: _DataLabel | None = None,
         extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/plotarea.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/trendline.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,69 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
+from openpyxl.chart.data_source import NumFmt
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
+from openpyxl.chart.text import RichText, Text
+from openpyxl.descriptors.base import Alias, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedBool, NestedFloat, NestedInteger, NestedSet
 from openpyxl.descriptors.serialisable import Serialisable
 
-class DataTable(Serialisable):
-    tagname: str
-    showHorzBorder: NestedBool[Literal[True]]
-    showVertBorder: NestedBool[Literal[True]]
-    showOutline: NestedBool[Literal[True]]
-    showKeys: NestedBool[Literal[True]]
+from ..xml._functions_overloads import _HasTagAndGet
+
+_TrendlineTrendlineType: TypeAlias = Literal["exp", "linear", "log", "movingAvg", "poly", "power"]
+
+class TrendlineLabel(Serialisable):
+    tagname: ClassVar[str]
+    layout: Typed[Layout, Literal[True]]
+    tx: Typed[Text, Literal[True]]
+    numFmt: Typed[NumFmt, Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
+    textProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        showHorzBorder: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        showVertBorder: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        showOutline: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        showKeys: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        layout: Layout | None = None,
+        tx: Text | None = None,
+        numFmt: NumFmt | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
-class PlotArea(Serialisable):
-    tagname: str
-    layout: Typed[Layout, Literal[True]]
-    dTable: Typed[DataTable, Literal[True]]
-    spPr: Typed[GraphicalProperties, Literal[True]]
+class Trendline(Serialisable):
+    tagname: ClassVar[str]
+    name: String[Literal[True]]
+    spPr: Typed[ExtensionList, Literal[True]]
     graphicalProperties: Alias
+    trendlineType: NestedSet[_TrendlineTrendlineType]
+    order: NestedInteger[Literal[True]]
+    period: NestedInteger[Literal[True]]
+    forward: NestedFloat[Literal[True]]
+    backward: NestedFloat[Literal[True]]
+    intercept: NestedFloat[Literal[True]]
+    dispRSqr: NestedBool[Literal[True]]
+    dispEq: NestedBool[Literal[True]]
+    trendlineLbl: Typed[ExtensionList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    areaChart: Incomplete
-    area3DChart: Incomplete
-    lineChart: Incomplete
-    line3DChart: Incomplete
-    stockChart: Incomplete
-    radarChart: Incomplete
-    scatterChart: Incomplete
-    pieChart: Incomplete
-    pie3DChart: Incomplete
-    doughnutChart: Incomplete
-    barChart: Incomplete
-    bar3DChart: Incomplete
-    ofPieChart: Incomplete
-    surfaceChart: Incomplete
-    surface3DChart: Incomplete
-    bubbleChart: Incomplete
-    valAx: Incomplete
-    catAx: Incomplete
-    dateAx: Incomplete
-    serAx: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        layout: Layout | None = None,
-        dTable: DataTable | None = None,
-        spPr: GraphicalProperties | None = None,
-        _charts=(),
-        _axes=(),
+        name: str | None = None,
+        spPr: ExtensionList | None = None,
+        trendlineType: _HasTagAndGet[_TrendlineTrendlineType] | _TrendlineTrendlineType = "linear",
+        order: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        period: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        forward: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        backward: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        intercept: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        dispRSqr: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        dispEq: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        trendlineLbl: ExtensionList | None = None,
         extLst: Unused = None,
     ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
-    @classmethod
-    def from_tree(cls, node): ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/print_settings.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/print_settings.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToFloat
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors.base import Alias, Float, Typed, _ConvertibleToFloat
+from openpyxl.descriptors.base import Alias, Float, Typed
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.header_footer import HeaderFooter
 from openpyxl.worksheet.page import PrintPageSetup
 
 class PageMargins(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     l: Float[Literal[False]]
     left: Alias
     r: Float[Literal[False]]
     right: Alias
     t: Float[Literal[False]]
     top: Alias
     b: Float[Literal[False]]
     bottom: Alias
     header: Float[Literal[False]]
     footer: Float[Literal[False]]
     def __init__(
         self,
-        l: _ConvertibleToFloat = 0.75,
-        r: _ConvertibleToFloat = 0.75,
-        t: _ConvertibleToFloat = 1,
-        b: _ConvertibleToFloat = 1,
-        header: _ConvertibleToFloat = 0.5,
-        footer: _ConvertibleToFloat = 0.5,
+        l: ConvertibleToFloat = 0.75,
+        r: ConvertibleToFloat = 0.75,
+        t: ConvertibleToFloat = 1,
+        b: ConvertibleToFloat = 1,
+        header: ConvertibleToFloat = 0.5,
+        footer: ConvertibleToFloat = 0.5,
     ) -> None: ...
 
 class PrintSettings(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     headerFooter: Typed[HeaderFooter, Literal[True]]
     pageMargins: Typed[PageMargins, Literal[True]]
     pageSetup: Typed[PrintPageSetup, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         headerFooter: HeaderFooter | None = None,
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/radar_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/radar_chart.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.axis import NumericAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
 from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedSet, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedBool, NestedSet
 
+from ..xml._functions_overloads import _HasTagAndGet
 from ._chart import ChartBase
 
 _RadarChartRadarStyle: TypeAlias = Literal["standard", "marker", "filled"]
 
 class RadarChart(ChartBase):
-    tagname: str
+    tagname: ClassVar[str]
     radarStyle: NestedSet[_RadarChartRadarStyle]
     type: Alias
     varyColors: NestedBool[Literal[True]]
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
     extLst: Typed[ExtensionList, Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/scatter_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/scatter_chart.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.axis import NumericAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
 from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedNoneSet, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedBool, NestedNoneSet, _NestedNoneSetParam
 
+from ..xml._functions_overloads import _HasTagAndGet
 from ._chart import ChartBase as ChartBase
 
 _ScatterChartScatterStyle: TypeAlias = Literal["line", "lineMarker", "marker", "smooth", "smoothMarker"]
 
 class ScatterChart(ChartBase):
-    tagname: str
+    tagname: ClassVar[str]
     scatterStyle: NestedNoneSet[_ScatterChartScatterStyle]
     varyColors: NestedBool[Literal[True]]
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[NumericAxis | TextAxis, Literal[False]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/series.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/series.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.chart.data_source import AxDataSource, NumDataSource, StrRef
 from openpyxl.chart.error_bar import ErrorBars
 from openpyxl.chart.label import DataLabelList
 from openpyxl.chart.marker import Marker
 from openpyxl.chart.picture import PictureOptions
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.trendline import Trendline
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedNoneSet, NestedText, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedNoneSet, NestedText, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.xml.functions import Element
+
+from ..xml._functions_overloads import _HasTagAndGet
 
 _SeriesShape: TypeAlias = Literal["cone", "coneToMax", "box", "cylinder", "pyramid", "pyramidToMax"]
 
 attribute_mapping: Incomplete
 
 class SeriesLabel(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     strRef: Typed[StrRef, Literal[True]]
     v: NestedText[str, Literal[True]]
     value: Alias
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, strRef: StrRef | None = None, v: object = None) -> None: ...
 
 class Series(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     idx: NestedInteger[Literal[False]]
     order: NestedInteger[Literal[False]]
     tx: Typed[SeriesLabel, Literal[True]]
     title: Alias
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Incomplete
     pictureOptions: Typed[PictureOptions, Literal[True]]
@@ -54,16 +57,16 @@
     bubble3D: NestedBool[Literal[True]]
     marker: Typed[Marker, Literal[True]]
     smooth: NestedBool[Literal[True]]
     explosion: NestedInteger[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0,
-        order: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0,
+        idx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt = 0,
+        order: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt = 0,
         tx: SeriesLabel | None = None,
         spPr: GraphicalProperties | None = None,
         pictureOptions: PictureOptions | None = None,
         dPt=(),
         dLbls: DataLabelList | None = None,
         trendline: Trendline | None = None,
         errBars: ErrorBars | None = None,
@@ -73,28 +76,30 @@
         shape: _NestedNoneSetParam[_SeriesShape] = None,
         xVal: AxDataSource | None = None,
         yVal: NumDataSource | None = None,
         bubbleSize: NumDataSource | None = None,
         bubble3D: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         marker: Marker | None = None,
         smooth: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        explosion: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        explosion: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         extLst: Unused = None,
     ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
+    def to_tree(self, tagname: str | None = None, idx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt | None = None) -> Element: ...  # type: ignore[override]
 
 class XYSeries(Series):
-    idx: Incomplete
-    order: Incomplete
-    tx: Incomplete
-    spPr: Incomplete
-    dPt: Incomplete
-    dLbls: Incomplete
-    trendline: Incomplete
-    errBars: Incomplete
-    xVal: Incomplete
-    yVal: Incomplete
-    invertIfNegative: Incomplete
-    bubbleSize: Incomplete
-    bubble3D: Incomplete
-    marker: Incomplete
-    smooth: Incomplete
+    # Same as parent
+    # idx = Series.idx
+    # order = Series.order
+    # tx = Series.tx
+    # spPr = Series.spPr
+    # dPt = Series.dPt
+    # dLbls = Series.dLbls
+    # trendline = Series.trendline
+    # errBars = Series.errBars
+    # xVal = Series.xVal
+    # yVal = Series.yVal
+    # invertIfNegative = Series.invertIfNegative
+    # bubbleSize = Series.bubbleSize
+    # bubble3D = Series.bubble3D
+    # marker = Series.marker
+    # smooth = Series.smooth
+    ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/shapes.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/shapes.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.descriptors.base import Alias, NoneSet, Typed, _ConvertibleToBool
-from openpyxl.descriptors.nested import EmptyTag, _HasTagAndGet
+from openpyxl.descriptors.nested import EmptyTag
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.drawing.colors import ColorChoice, ColorChoiceDescriptor
 from openpyxl.drawing.fill import GradientFillProperties, PatternFillProperties
 from openpyxl.drawing.geometry import CustomGeometry2D, PresetGeometry2D, Scene3D, Shape3D, Transform2D
 from openpyxl.drawing.line import LineProperties
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _GraphicalPropertiesBwMode: TypeAlias = Literal[
     "clr", "auto", "gray", "ltGray", "invGray", "grayWhite", "blackGray", "blackWhite", "black", "white", "hidden"
 ]
 
 class GraphicalProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     bwMode: NoneSet[_GraphicalPropertiesBwMode]
     xfrm: Typed[Transform2D, Literal[True]]
     transform: Alias
     custGeom: Typed[CustomGeometry2D, Literal[True]]
     prstGeom: Typed[PresetGeometry2D, Literal[True]]
     noFill: EmptyTag[Literal[False]]
-    solidFill: Incomplete
+    solidFill: ColorChoiceDescriptor
     gradFill: Typed[GradientFillProperties, Literal[True]]
     pattFill: Typed[PatternFillProperties, Literal[True]]
     ln: Typed[LineProperties, Literal[True]]
     line: Alias
     scene3d: Typed[Scene3D, Literal[True]]
     sp3d: Typed[Shape3D, Literal[True]]
     shape3D: Alias
     extLst: Typed[Incomplete, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         bwMode: _GraphicalPropertiesBwMode | Literal["none"] | None = None,
         xfrm: Transform2D | None = None,
         noFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
-        solidFill: Incomplete | None = None,
+        solidFill: str | ColorChoice | None = None,
         gradFill: GradientFillProperties | None = None,
         pattFill: PatternFillProperties | None = None,
         ln: Incomplete | None = None,
         scene3d: Scene3D | None = None,
         custGeom: CustomGeometry2D | None = None,
         prstGeom: PresetGeometry2D | None = None,
         sp3d: Shape3D | None = None,
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/stock_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/stock_chart.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
 from openpyxl.chart.axis import ChartLines, NumericAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
 from openpyxl.chart.updown_bars import UpDownBars
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 
 from ._chart import ChartBase
 
 class StockChart(ChartBase):
-    tagname: str
+    tagname: ClassVar[str]
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
     dropLines: Typed[ChartLines, Literal[True]]
     hiLowLines: Typed[ChartLines, Literal[True]]
     upDownBars: Typed[UpDownBars, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/surface_chart.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/surface_chart.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-from _typeshed import Incomplete
-from abc import abstractmethod
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
 
 from openpyxl.chart.axis import NumericAxis, SeriesAxis, TextAxis
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedInteger, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedBool, NestedInteger
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
 from ._3d import _3DBase
 from ._chart import ChartBase
 
 class BandFormat(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     idx: NestedInteger[Literal[False]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
-        self, idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0, spPr: GraphicalProperties | None = None
+        self, idx: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt = 0, spPr: GraphicalProperties | None = None
     ) -> None: ...
 
 class BandFormatList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     bandFmt: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, bandFmt=()) -> None: ...
 
 class _SurfaceChartBase(ChartBase):
     wireframe: NestedBool[Literal[True]]
     ser: Incomplete
@@ -37,31 +36,30 @@
     def __init__(
         self,
         wireframe: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         ser=(),
         bandFmts: BandFormatList | None = None,
         **kw,
     ) -> None: ...
-    @property
-    @abstractmethod
-    def tagname(self) -> str: ...
 
 class SurfaceChart3D(_SurfaceChartBase, _3DBase):
-    tagname: str
-    wireframe: Incomplete
-    ser: Incomplete
-    bandFmts: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent
+    # wireframe = _SurfaceChartBase.wireframe
+    # ser = _SurfaceChartBase.ser
+    # bandFmts = _SurfaceChartBase.bandFmts
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
     z_axis: Typed[SeriesAxis, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, **kw) -> None: ...
 
 class SurfaceChart(SurfaceChart3D):
-    tagname: str
-    wireframe: Incomplete
-    ser: Incomplete
-    bandFmts: Incomplete
+    tagname: ClassVar[str]
+    # Same as parent and grandparent
+    # wireframe = _SurfaceChartBase.wireframe
+    # ser = _SurfaceChartBase.ser
+    # bandFmts = _SurfaceChartBase.bandFmts
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, **kw) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/text.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/text.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import Incomplete, Unused
+from typing import ClassVar, Literal
 
 from openpyxl.chart.data_source import StrRef
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.text import ListStyle, RichTextProperties
+from openpyxl.xml.functions import Element
 
 class RichText(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     bodyPr: Typed[RichTextProperties, Literal[False]]
     properties: Alias
     lstStyle: Typed[ListStyle, Literal[True]]
     p: Incomplete
     paragraphs: Alias
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, bodyPr: RichTextProperties | None = None, lstStyle: ListStyle | None = None, p: Incomplete | None = None
     ) -> None: ...
 
 class Text(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     strRef: Typed[StrRef, Literal[True]]
     rich: Typed[RichText, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, strRef: StrRef | None = None, rich: RichText | None = None) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    def to_tree(self, tagname: str | None = None, idx: Unused = None, namespace: str | None = None) -> Element: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/title.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/title.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import Unused
+from typing import ClassVar, Literal
 
 from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText, Text
 from openpyxl.descriptors import Strict, Typed
 from openpyxl.descriptors.base import Alias, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedBool
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 class Title(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     tx: Typed[Text, Literal[True]]
     text: Alias
     layout: Typed[Layout, Literal[True]]
     overlay: NestedBool[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
@@ -29,13 +30,13 @@
         layout: Layout | None = None,
         overlay: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
-def title_maker(text): ...
+def title_maker(text) -> Title: ...
 
-class TitleDescriptor(Typed[Title, Incomplete]):
+class TitleDescriptor(Typed[Title, Literal[True]]):
     expected_type: type[Title]
     allow_none: Literal[True]
-    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
+    def __set__(self, instance: Serialisable | Strict, value: str | Title | None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/trendline.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/picture.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,81 @@
-from _typeshed import Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import Incomplete, Unused
+from typing import ClassVar, Literal
 
-from openpyxl.chart.data_source import NumFmt
-from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.chart.text import RichText, Text
-from openpyxl.descriptors.base import Alias, String, Typed, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedBool, NestedFloat, NestedInteger, NestedSet, _HasTagAndGet
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.drawing.fill import BlipFillProperties
+from openpyxl.drawing.geometry import ShapeStyle
+from openpyxl.drawing.properties import NonVisualDrawingProps
 
-_TrendlineTrendlineType: TypeAlias = Literal["exp", "linear", "log", "movingAvg", "poly", "power"]
-
-class TrendlineLabel(Serialisable):
-    tagname: str
-    layout: Typed[Layout, Literal[True]]
-    tx: Typed[Text, Literal[True]]
-    numFmt: Typed[NumFmt, Literal[True]]
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
-    txPr: Typed[RichText, Literal[True]]
-    textProperties: Alias
+class PictureLocking(Serialisable):
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
+    noCrop: Bool[Literal[True]]
+    noGrp: Bool[Literal[True]]
+    noSelect: Bool[Literal[True]]
+    noRot: Bool[Literal[True]]
+    noChangeAspect: Bool[Literal[True]]
+    noMove: Bool[Literal[True]]
+    noResize: Bool[Literal[True]]
+    noEditPoints: Bool[Literal[True]]
+    noAdjustHandles: Bool[Literal[True]]
+    noChangeArrowheads: Bool[Literal[True]]
+    noChangeShapeType: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        layout: Layout | None = None,
-        tx: Text | None = None,
-        numFmt: NumFmt | None = None,
-        spPr: GraphicalProperties | None = None,
-        txPr: RichText | None = None,
+        noCrop: _ConvertibleToBool | None = None,
+        noGrp: _ConvertibleToBool | None = None,
+        noSelect: _ConvertibleToBool | None = None,
+        noRot: _ConvertibleToBool | None = None,
+        noChangeAspect: _ConvertibleToBool | None = None,
+        noMove: _ConvertibleToBool | None = None,
+        noResize: _ConvertibleToBool | None = None,
+        noEditPoints: _ConvertibleToBool | None = None,
+        noAdjustHandles: _ConvertibleToBool | None = None,
+        noChangeArrowheads: _ConvertibleToBool | None = None,
+        noChangeShapeType: _ConvertibleToBool | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
-class Trendline(Serialisable):
-    tagname: str
-    name: String[Literal[True]]
-    spPr: Typed[ExtensionList, Literal[True]]
-    graphicalProperties: Alias
-    trendlineType: NestedSet[_TrendlineTrendlineType]
-    order: NestedInteger[Literal[True]]
-    period: NestedInteger[Literal[True]]
-    forward: NestedFloat[Literal[True]]
-    backward: NestedFloat[Literal[True]]
-    intercept: NestedFloat[Literal[True]]
-    dispRSqr: NestedBool[Literal[True]]
-    dispEq: NestedBool[Literal[True]]
-    trendlineLbl: Typed[ExtensionList, Literal[True]]
+class NonVisualPictureProperties(Serialisable):
+    tagname: ClassVar[str]
+    preferRelativeResize: Bool[Literal[True]]
+    picLocks: Typed[PictureLocking, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
+        self, preferRelativeResize: _ConvertibleToBool | None = None, picLocks: Incomplete | None = None, extLst: Unused = None
+    ) -> None: ...
+
+class PictureNonVisual(Serialisable):
+    tagname: ClassVar[str]
+    cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
+    cNvPicPr: Typed[NonVisualPictureProperties, Literal[False]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(
+        self, cNvPr: NonVisualDrawingProps | None = None, cNvPicPr: NonVisualPictureProperties | None = None
+    ) -> None: ...
+
+class PictureFrame(Serialisable):
+    tagname: ClassVar[str]
+    macro: String[Literal[True]]
+    fPublished: Bool[Literal[True]]
+    nvPicPr: Typed[PictureNonVisual, Literal[False]]
+    blipFill: Typed[BlipFillProperties, Literal[False]]
+    spPr: Typed[GraphicalProperties, Literal[False]]
+    graphicalProperties: Alias
+    style: Typed[ShapeStyle, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(
         self,
-        name: str | None = None,
-        spPr: ExtensionList | None = None,
-        trendlineType: _HasTagAndGet[_TrendlineTrendlineType] | _TrendlineTrendlineType = "linear",
-        order: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        period: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        forward: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        backward: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        intercept: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        dispRSqr: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        dispEq: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        trendlineLbl: ExtensionList | None = None,
-        extLst: Unused = None,
+        macro: str | None = None,
+        fPublished: _ConvertibleToBool | None = None,
+        nvPicPr: PictureNonVisual | None = None,
+        blipFill: BlipFillProperties | None = None,
+        spPr: GraphicalProperties | None = None,
+        style: ShapeStyle | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/updown_bars.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chart/updown_bars.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
 from openpyxl.chart.axis import ChartLines
 from openpyxl.descriptors.base import Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 class UpDownBars(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     gapWidth: Incomplete
     upBars: Typed[ChartLines, Literal[True]]
     downBars: Typed[ChartLines, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, gapWidth: int = 150, upBars: ChartLines | None = None, downBars: ChartLines | None = None, extLst: Unused = None
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/chartsheet.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/chartsheet.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import Unused
+from typing import ClassVar, Literal
 
+from openpyxl import _Decodable, _VisibilityType
 from openpyxl.chartsheet.custom import CustomChartsheetViews
 from openpyxl.chartsheet.properties import ChartsheetProperties
 from openpyxl.chartsheet.protection import ChartsheetProtection
 from openpyxl.chartsheet.publish import WebPublishItems
 from openpyxl.chartsheet.relation import DrawingHF, SheetBackgroundPicture
 from openpyxl.chartsheet.views import ChartsheetViewList
 from openpyxl.descriptors.base import Alias, Set, Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.workbook.child import _WorkbookChild
+from openpyxl.workbook.workbook import Workbook
 from openpyxl.worksheet.drawing import Drawing
 from openpyxl.worksheet.header_footer import HeaderFooter as _HeaderFooter
 from openpyxl.worksheet.page import PageMargins, PrintPageSetup
-
-_ChartsheetSheetState: TypeAlias = Literal["visible", "hidden", "veryHidden"]
+from openpyxl.xml.functions import Element
 
 class Chartsheet(_WorkbookChild, Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     mime_type: str
     sheetPr: Typed[ChartsheetProperties, Literal[True]]
     sheetViews: Typed[ChartsheetViewList, Literal[False]]
     sheetProtection: Typed[ChartsheetProtection, Literal[True]]
     customSheetViews: Typed[CustomChartsheetViews, Literal[True]]
     pageMargins: Typed[PageMargins, Literal[True]]
     pageSetup: Typed[PrintPageSetup, Literal[True]]
     drawing: Typed[Drawing, Literal[True]]
     drawingHF: Typed[DrawingHF, Literal[True]]
     picture: Typed[SheetBackgroundPicture, Literal[True]]
     webPublishItems: Typed[WebPublishItems, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    sheet_state: Set[_ChartsheetSheetState]
+    sheet_state: Set[_VisibilityType]
     headerFooter: Typed[_HeaderFooter, Literal[False]]
-    HeaderFooter: Alias
+    HeaderFooter: Alias  # type: ignore[assignment] # Different from parent class
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         sheetPr: ChartsheetProperties | None = None,
         sheetViews: ChartsheetViewList | None = None,
         sheetProtection: ChartsheetProtection | None = None,
@@ -47,13 +47,13 @@
         pageSetup: PrintPageSetup | None = None,
         headerFooter: _HeaderFooter | None = None,
         drawing: Unused = None,
         drawingHF: DrawingHF | None = None,
         picture: SheetBackgroundPicture | None = None,
         webPublishItems: WebPublishItems | None = None,
         extLst: Unused = None,
-        parent: Incomplete | None = None,
-        title: str = "",
-        sheet_state: _ChartsheetSheetState = "visible",
+        parent: Workbook | None = None,
+        title: str | _Decodable | None = "",
+        sheet_state: _VisibilityType = "visible",
     ) -> None: ...
     def add_chart(self, chart) -> None: ...
-    def to_tree(self): ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/custom.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/custom.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-from _typeshed import Incomplete
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal, overload
 
-from openpyxl.descriptors.base import Bool, Integer, Set, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl import _VisibilityType
+from openpyxl.descriptors.base import Bool, Integer, Set, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.header_footer import HeaderFooter
 from openpyxl.worksheet.page import PageMargins, PrintPageSetup
 
-_CustomChartsheetViewState: TypeAlias = Literal["visible", "hidden", "veryHidden"]
-
 class CustomChartsheetView(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     guid: Incomplete
     scale: Integer[Literal[False]]
-    state: Set[_CustomChartsheetViewState]
+    state: Set[_VisibilityType]
     zoomToFit: Bool[Literal[True]]
     pageMargins: Typed[PageMargins, Literal[True]]
     pageSetup: Typed[PrintPageSetup, Literal[True]]
     headerFooter: Typed[HeaderFooter, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         guid: Incomplete | None = None,
         *,
-        scale: _ConvertibleToInt,
-        state: _CustomChartsheetViewState = "visible",
+        scale: ConvertibleToInt,
+        state: _VisibilityType = "visible",
         zoomToFit: _ConvertibleToBool | None = None,
         pageMargins: PageMargins | None = None,
         pageSetup: PrintPageSetup | None = None,
         headerFooter: HeaderFooter | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         guid: Incomplete | None,
-        scale: _ConvertibleToInt,
-        state: _CustomChartsheetViewState = "visible",
+        scale: ConvertibleToInt,
+        state: _VisibilityType = "visible",
         zoomToFit: _ConvertibleToBool | None = None,
         pageMargins: PageMargins | None = None,
         pageSetup: PrintPageSetup | None = None,
         headerFooter: HeaderFooter | None = None,
     ) -> None: ...
 
 class CustomChartsheetViews(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     customSheetView: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, customSheetView: Incomplete | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/properties.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/properties.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
 from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
-from openpyxl.descriptors.serialisable import Serialisable as Serialisable
+from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.colors import Color
 
 class ChartsheetProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     published: Bool[Literal[True]]
     codeName: String[Literal[True]]
     tabColor: Typed[Color, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, published: _ConvertibleToBool | None = None, codeName: str | None = None, tabColor: Color | None = None
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/protection.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/protection.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.protection import _Protected
 
 class ChartsheetProtection(Serialisable, _Protected):
-    tagname: str
+    tagname: ClassVar[str]
     algorithmName: String[Literal[True]]
     hashValue: Incomplete
     saltValue: Incomplete
     spinCount: Integer[Literal[True]]
     content: Bool[Literal[True]]
     objects: Bool[Literal[True]]
     __attrs__: ClassVar[tuple[str, ...]]
     password: Incomplete
     def __init__(
         self,
         content: _ConvertibleToBool | None = None,
         objects: _ConvertibleToBool | None = None,
         hashValue: Incomplete | None = None,
-        spinCount: _ConvertibleToInt | None = None,
+        spinCount: ConvertibleToInt | None = None,
         saltValue: Incomplete | None = None,
         algorithmName: str | None = None,
         password: Incomplete | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/publish.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/publish.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from _typeshed import Incomplete
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Bool, Integer, Set, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, Set, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 _WebPublishItemSourceType: TypeAlias = Literal[
     "sheet", "printArea", "autoFilter", "range", "chart", "pivotTable", "query", "label"
 ]
 
 class WebPublishItem(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     id: Integer[Literal[False]]
     divId: String[Literal[False]]
     sourceType: Set[_WebPublishItemSourceType]
     sourceRef: String[Literal[False]]
     sourceObject: String[Literal[True]]
     destinationFile: String[Literal[False]]
     title: String[Literal[True]]
     autoRepublish: Bool[Literal[True]]
     @overload
     def __init__(
         self,
-        id: _ConvertibleToInt,
+        id: ConvertibleToInt,
         divId: str,
         sourceType: _WebPublishItemSourceType,
         sourceRef: str,
         sourceObject: str | None = None,
         *,
         destinationFile: str,
         title: str | None = None,
         autoRepublish: _ConvertibleToBool | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        id: _ConvertibleToInt,
+        id: ConvertibleToInt,
         divId: str,
         sourceType: _WebPublishItemSourceType,
         sourceRef: str,
         sourceObject: str | None,
         destinationFile: str,
         title: str | None = None,
         autoRepublish: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class WebPublishItems(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     count: Integer[Literal[True]]
     webPublishItem: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt | None = None, webPublishItem: Incomplete | None = None) -> None: ...
+    def __init__(self, count: ConvertibleToInt | None = None, webPublishItem: Incomplete | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/relation.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/relation.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from _typeshed import Incomplete
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors.base import Alias, Integer, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Integer
 from openpyxl.descriptors.serialisable import Serialisable
 
 class SheetBackgroundPicture(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     id: Incomplete
     def __init__(self, id) -> None: ...
 
 class DrawingHF(Serialisable):
     id: Incomplete
     lho: Integer[Literal[True]]
     leftHeaderOddPages: Alias
@@ -46,26 +46,26 @@
     rfe: Integer[Literal[True]]
     rightFooterEvenPages: Alias
     rff: Integer[Literal[True]]
     rightFooterFirstPage: Alias
     def __init__(
         self,
         id: Incomplete | None = None,
-        lho: _ConvertibleToInt | None = None,
-        lhe: _ConvertibleToInt | None = None,
-        lhf: _ConvertibleToInt | None = None,
-        cho: _ConvertibleToInt | None = None,
-        che: _ConvertibleToInt | None = None,
-        chf: _ConvertibleToInt | None = None,
-        rho: _ConvertibleToInt | None = None,
-        rhe: _ConvertibleToInt | None = None,
-        rhf: _ConvertibleToInt | None = None,
-        lfo: _ConvertibleToInt | None = None,
-        lfe: _ConvertibleToInt | None = None,
-        lff: _ConvertibleToInt | None = None,
-        cfo: _ConvertibleToInt | None = None,
-        cfe: _ConvertibleToInt | None = None,
-        cff: _ConvertibleToInt | None = None,
-        rfo: _ConvertibleToInt | None = None,
-        rfe: _ConvertibleToInt | None = None,
-        rff: _ConvertibleToInt | None = None,
+        lho: ConvertibleToInt | None = None,
+        lhe: ConvertibleToInt | None = None,
+        lhf: ConvertibleToInt | None = None,
+        cho: ConvertibleToInt | None = None,
+        che: ConvertibleToInt | None = None,
+        chf: ConvertibleToInt | None = None,
+        rho: ConvertibleToInt | None = None,
+        rhe: ConvertibleToInt | None = None,
+        rhf: ConvertibleToInt | None = None,
+        lfo: ConvertibleToInt | None = None,
+        lfe: ConvertibleToInt | None = None,
+        lff: ConvertibleToInt | None = None,
+        cfo: ConvertibleToInt | None = None,
+        cfe: ConvertibleToInt | None = None,
+        cff: ConvertibleToInt | None = None,
+        rfo: ConvertibleToInt | None = None,
+        rfe: ConvertibleToInt | None = None,
+        rff: ConvertibleToInt | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/views.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/chartsheet/views.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 class ChartsheetView(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     tabSelected: Bool[Literal[True]]
     zoomScale: Integer[Literal[True]]
     workbookViewId: Integer[Literal[False]]
     zoomToFit: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         tabSelected: _ConvertibleToBool | None = None,
-        zoomScale: _ConvertibleToInt | None = None,
-        workbookViewId: _ConvertibleToInt = 0,
+        zoomScale: ConvertibleToInt | None = None,
+        workbookViewId: ConvertibleToInt = 0,
         zoomToFit: _ConvertibleToBool | None = True,
         extLst: Unused = None,
     ) -> None: ...
 
 class ChartsheetViewList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     sheetView: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, sheetView: Incomplete | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/comments/comment_sheet.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/text.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,121 +1,98 @@
-from _typeshed import Incomplete, Unused
-from collections.abc import Generator
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
-
-from openpyxl.cell.text import Text
-from openpyxl.comments.author import AuthorList
-from openpyxl.descriptors.base import Bool, Integer, Set, String, Typed, _ConvertibleToBool, _ConvertibleToInt
-from openpyxl.descriptors.excel import ExtensionList
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
+
+from openpyxl.descriptors.base import Alias, Integer, NoneSet, Typed, _ConvertibleToBool
+from openpyxl.descriptors.nested import NestedString, NestedText, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.worksheet.ole import ObjectAnchor
+from openpyxl.styles.colors import Color
+from openpyxl.styles.fonts import Font, _FontScheme, _FontU, _FontVertAlign
 
-_PropertiesTextHAlign: TypeAlias = Literal["left", "center", "right", "justify", "distributed"]
-_PropertiesTextVAlign: TypeAlias = Literal["top", "center", "bottom", "justify", "distributed"]
+from ..xml._functions_overloads import _HasTagAndGet
 
-class Properties(Serialisable):
-    locked: Bool[Literal[True]]
-    defaultSize: Bool[Literal[True]]
-    _print: Bool[Literal[True]]  # Not private. Avoids name clash
-    disabled: Bool[Literal[True]]
-    uiObject: Bool[Literal[True]]
-    autoFill: Bool[Literal[True]]
-    autoLine: Bool[Literal[True]]
-    altText: String[Literal[True]]
-    textHAlign: Set[_PropertiesTextHAlign]
-    textVAlign: Set[_PropertiesTextVAlign]
-    lockText: Bool[Literal[True]]
-    justLastX: Bool[Literal[True]]
-    autoScale: Bool[Literal[True]]
-    rowHidden: Bool[Literal[True]]
-    colHidden: Bool[Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
-    anchor: ObjectAnchor | None
-    @overload
-    def __init__(
-        self,
-        locked: _ConvertibleToBool | None = None,
-        defaultSize: _ConvertibleToBool | None = None,
-        _print: _ConvertibleToBool | None = None,
-        disabled: _ConvertibleToBool | None = None,
-        uiObject: _ConvertibleToBool | None = None,
-        autoFill: _ConvertibleToBool | None = None,
-        autoLine: _ConvertibleToBool | None = None,
-        altText: str | None = None,
-        *,
-        textHAlign: _PropertiesTextHAlign,
-        textVAlign: _PropertiesTextVAlign,
-        lockText: _ConvertibleToBool | None = None,
-        justLastX: _ConvertibleToBool | None = None,
-        autoScale: _ConvertibleToBool | None = None,
-        rowHidden: _ConvertibleToBool | None = None,
-        colHidden: _ConvertibleToBool | None = None,
-        anchor: ObjectAnchor | None = None,
-    ) -> None: ...
-    @overload
+_PhoneticPropertiesType: TypeAlias = Literal["halfwidthKatakana", "fullwidthKatakana", "Hiragana", "noConversion"]
+_PhoneticPropertiesAlignment: TypeAlias = Literal["noControl", "left", "center", "distributed"]
+
+class PhoneticProperties(Serialisable):
+    tagname: ClassVar[str]
+    fontId: Integer[Literal[False]]
+    type: NoneSet[_PhoneticPropertiesType]
+    alignment: NoneSet[_PhoneticPropertiesAlignment]
     def __init__(
         self,
-        locked: _ConvertibleToBool | None,
-        defaultSize: _ConvertibleToBool | None,
-        _print: _ConvertibleToBool | None,
-        disabled: _ConvertibleToBool | None,
-        uiObject: _ConvertibleToBool | None,
-        autoFill: _ConvertibleToBool | None,
-        autoLine: _ConvertibleToBool | None,
-        altText: str | None,
-        textHAlign: _PropertiesTextHAlign,
-        textVAlign: _PropertiesTextVAlign,
-        lockText: _ConvertibleToBool | None = None,
-        justLastX: _ConvertibleToBool | None = None,
-        autoScale: _ConvertibleToBool | None = None,
-        rowHidden: _ConvertibleToBool | None = None,
-        colHidden: _ConvertibleToBool | None = None,
-        anchor: ObjectAnchor | None = None,
+        fontId: ConvertibleToInt,
+        type: _PhoneticPropertiesType | Literal["none"] | None = None,
+        alignment: _PhoneticPropertiesAlignment | Literal["none"] | None = None,
     ) -> None: ...
 
-class CommentRecord(Serialisable):
-    tagname: str
-    ref: String[Literal[False]]
-    authorId: Integer[Literal[False]]
-    guid: Incomplete
-    shapeId: Integer[Literal[True]]
-    text: Typed[Text, Literal[False]]
-    commentPr: Typed[Properties, Literal[True]]
-    author: String[Literal[True]]
+_PhoneticProperties: TypeAlias = PhoneticProperties
+
+class PhoneticText(Serialisable):
+    tagname: ClassVar[str]
+    sb: Integer[Literal[False]]
+    eb: Integer[Literal[False]]
+    t: NestedText[str, Literal[False]]
+    text: Alias
+    def __init__(self, sb: ConvertibleToInt, eb: ConvertibleToInt, t: object = None) -> None: ...
+
+class InlineFont(Font):
+    tagname: ClassVar[str]
+    rFont: NestedString[Literal[True]]
+    # Same as parent
+    # charset = Font.charset
+    # family = Font.family
+    # b = Font.b
+    # i = Font.i
+    # strike = Font.strike
+    # outline = Font.outline
+    # shadow = Font.shadow
+    # condense = Font.condense
+    # extend = Font.extend
+    # color = Font.color
+    # sz = Font.sz
+    # u = Font.u
+    # vertAlign = Font.vertAlign
+    # scheme = Font.scheme
     __elements__: ClassVar[tuple[str, ...]]
-    __attrs__: ClassVar[tuple[str, ...]]
-    height: Incomplete
-    width: Incomplete
     def __init__(
         self,
-        ref: str = "",
-        authorId: _ConvertibleToInt = 0,
-        guid: Incomplete | None = None,
-        shapeId: _ConvertibleToInt | None = 0,
-        text: Text | None = None,
-        commentPr: Properties | None = None,
-        author: str | None = None,
-        height: int = 79,
-        width: int = 144,
+        rFont: object = None,
+        charset: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        family: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        b: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        i: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        strike: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        outline: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        shadow: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        condense: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        extend: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        color: Color | None = None,
+        sz: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        u: _NestedNoneSetParam[_FontU] = None,
+        vertAlign: _NestedNoneSetParam[_FontVertAlign] = None,
+        scheme: _NestedNoneSetParam[_FontScheme] = None,
     ) -> None: ...
-    @classmethod
-    def from_cell(cls, cell): ...
-    @property
-    def content(self): ...
 
-class CommentSheet(Serialisable):
-    tagname: str
-    authors: Typed[AuthorList, Literal[False]]
-    commentList: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    mime_type: str
+class RichText(Serialisable):
+    tagname: ClassVar[str]
+    rPr: Typed[InlineFont, Literal[True]]
+    font: Alias
+    t: NestedText[str, Literal[True]]
+    text: Alias
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, authors: AuthorList, commentList: Incomplete | None = None, extLst: Unused = None) -> None: ...
-    def to_tree(self): ...
-    @property
-    def comments(self) -> Generator[Incomplete, None, None]: ...
-    @classmethod
-    def from_comments(cls, comments): ...
-    def write_shapes(self, vml: Incomplete | None = None): ...
+    def __init__(self, rPr: InlineFont | None = None, t: object = None) -> None: ...
+
+class Text(Serialisable):
+    tagname: ClassVar[str]
+    t: NestedText[str, Literal[True]]
+    plain: Alias
+    r: Incomplete
+    formatted: Alias
+    rPh: Incomplete
+    phonetic: Alias
+    phoneticPr: Typed[_PhoneticProperties, Literal[True]]
+    PhoneticProperties: Alias
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, t: object = None, r=(), rPh=(), phoneticPr: _PhoneticProperties | None = None) -> None: ...
     @property
-    def path(self): ...
+    def content(self) -> str: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/base.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,55 @@
-from _typeshed import Incomplete, ReadableBuffer, SupportsTrunc, Unused
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, ReadableBuffer, Unused
 from collections.abc import Iterable, Sized
 from datetime import datetime
 from re import Pattern
-from typing import Any, Generic, SupportsFloat, SupportsInt, TypeVar, overload
-from typing_extensions import Literal, SupportsIndex, TypeAlias
+from typing import Any, Generic, Literal, TypeVar, overload
+from typing_extensions import TypeAlias
 
 from openpyxl.descriptors import Strict
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.fill import Blip
 from openpyxl.worksheet.cell_range import CellRange, MultiCellRange
 
 _T = TypeVar("_T")
 _P = TypeVar("_P", str, ReadableBuffer)
 _N = TypeVar("_N", bound=bool)
 _L = TypeVar("_L", bound=Sized)
 _M = TypeVar("_M", int, float)
 
 _ExpectedTypeParam: TypeAlias = type[_T] | tuple[type[_T], ...]
 _ConvertibleToMultiCellRange: TypeAlias = MultiCellRange | str | Iterable[CellRange]
-_ConvertibleToInt: TypeAlias = int | str | ReadableBuffer | SupportsInt | SupportsIndex | SupportsTrunc
-_ConvertibleToFloat: TypeAlias = float | SupportsFloat | SupportsIndex | str | ReadableBuffer
-# Since everything is convertible to a bool, this restricts to only intended expected types
+# Since everything is convertible to a bool, this restricts to only intended expected types of intended literals
 _ConvertibleToBool: TypeAlias = bool | str | int | None  # True | False | "true" | "t" | "false" | "f" | 1 | 0 | None
 
 class Descriptor(Generic[_T]):
     name: str | None
     def __init__(self, name: str | None = None, **kw: object) -> None: ...
     def __get__(self, instance: Serialisable | Strict, cls: type | None) -> _T: ...
     def __set__(self, instance: Serialisable | Strict, value: _T) -> None: ...
 
 class Typed(Descriptor[_T], Generic[_T, _N]):
+    __doc__: str
+    # Members optional in __init__
     expected_type: type[_T]
     allow_none: _N
     nested: bool
-    __doc__: Incomplete
 
     @overload
     def __init__(
-        self: Typed[_T, Literal[True]],
+        self: Typed[_T, Literal[True]],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         name: str | None = None,
         *,
         expected_type: _ExpectedTypeParam[_T],
         allow_none: Literal[True],
         nested: bool = False,
     ) -> None: ...
     @overload
     def __init__(
-        self: Typed[_T, Literal[False]],
+        self: Typed[_T, Literal[False]],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         name: str | None = None,
         *,
         expected_type: _ExpectedTypeParam[_T],
         allow_none: Literal[False] = False,
         nested: bool = False,
     ) -> None: ...
     @overload
@@ -61,67 +60,65 @@
     def __set__(self: Typed[_T, Literal[True]], instance: Serialisable | Strict, value: _T | None) -> None: ...
     @overload
     def __set__(self: Typed[_T, Literal[False]], instance: Serialisable | Strict, value: _T) -> None: ...
 
 class Convertible(Typed[_T, _N]):
     @overload
     def __init__(
-        self: Convertible[_T, Literal[True]],
+        self: Convertible[_T, Literal[True]],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         name: str | None = None,
         *,
         expected_type: _ExpectedTypeParam[_T],
         allow_none: Literal[True],
     ) -> None: ...
     @overload
     def __init__(
-        self: Convertible[_T, Literal[False]],
+        self: Convertible[_T, Literal[False]],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         name: str | None = None,
         *,
         expected_type: _ExpectedTypeParam[_T],
         allow_none: Literal[False] = False,
     ) -> None: ...
     # NOTE: It is currently impossible to make a generic based on the parameter type of another generic
-    # So we implement explicitely the types used internally
+    # So we implement explicitly the types used internally
     # MultiCellRange
     @overload
     def __set__(
         self: Convertible[MultiCellRange, Literal[True]],
         instance: Serialisable | Strict,
         value: _ConvertibleToMultiCellRange | None,
     ) -> None: ...
     @overload
     def __set__(
         self: Convertible[MultiCellRange, Literal[False]], instance: Serialisable | Strict, value: _ConvertibleToMultiCellRange
     ) -> None: ...
     # str | Blip
     @overload
     def __set__(
-        self: Convertible[str, bool] | Convertible[Blip, bool],
+        self: Convertible[str, _N] | Convertible[Blip, _N],
         instance: Serialisable | Strict,
         value: object,  # Not[None] when _N = False
     ) -> None: ...
     # bool
     @overload
-    def __set__(self: Convertible[bool, bool], instance: Serialisable | Strict, value: _ConvertibleToBool) -> None: ...
+    def __set__(self: Convertible[bool, _N], instance: Serialisable | Strict, value: _ConvertibleToBool) -> None: ...
     # int
     @overload
     def __set__(
-        self: Convertible[int, Literal[True]], instance: Serialisable | Strict, value: _ConvertibleToInt | None
+        self: Convertible[int, Literal[True]], instance: Serialisable | Strict, value: ConvertibleToInt | None
     ) -> None: ...
     @overload
-    def __set__(self: Convertible[int, Literal[False]], instance: Serialisable | Strict, value: _ConvertibleToInt) -> None: ...
+    def __set__(self: Convertible[int, Literal[False]], instance: Serialisable | Strict, value: ConvertibleToInt) -> None: ...
     # float
     @overload
     def __set__(
-        self: Convertible[float, Literal[True]], instance: Serialisable | Strict, value: _ConvertibleToFloat | None
+        self: Convertible[float, Literal[True]], instance: Serialisable | Strict, value: ConvertibleToFloat | None
     ) -> None: ...
     @overload
-    def __set__(
-        self: Convertible[float, Literal[False]], instance: Serialisable | Strict, value: _ConvertibleToFloat
-    ) -> None: ...
+    def __set__(self: Convertible[float, Literal[False]], instance: Serialisable | Strict, value: ConvertibleToFloat) -> None: ...
     # Anything else
     @overload
     def __set__(self: Convertible[_T, Literal[True]], instance: Serialisable | Strict, value: _T | int | Any | None) -> None: ...
 
 class Max(Convertible[_M, _N]):
     expected_type: type[_M]
     allow_none: _N
@@ -143,22 +140,22 @@
     def __init__(
         self: Max[float, Literal[False]],
         *,
         expected_type: _ExpectedTypeParam[float] = ...,
         allow_none: Literal[False] = False,
         max: float,
     ) -> None: ...
-    @overload  # type:ignore[override]  # Different restrictions
-    def __set__(self: Max[int, Literal[True]], instance: Serialisable | Strict, value: _ConvertibleToInt | None) -> None: ...
+    @overload  # type: ignore[override]  # Different restrictions
+    def __set__(self: Max[int, Literal[True]], instance: Serialisable | Strict, value: ConvertibleToInt | None) -> None: ...
     @overload
-    def __set__(self: Max[int, Literal[False]], instance: Serialisable | Strict, value: _ConvertibleToInt) -> None: ...
+    def __set__(self: Max[int, Literal[False]], instance: Serialisable | Strict, value: ConvertibleToInt) -> None: ...
     @overload
-    def __set__(self: Max[float, Literal[True]], instance: Serialisable | Strict, value: _ConvertibleToFloat | None) -> None: ...
+    def __set__(self: Max[float, Literal[True]], instance: Serialisable | Strict, value: ConvertibleToFloat | None) -> None: ...
     @overload
-    def __set__(self: Max[float, Literal[False]], instance: Serialisable | Strict, value: _ConvertibleToFloat) -> None: ...
+    def __set__(self: Max[float, Literal[False]], instance: Serialisable | Strict, value: ConvertibleToFloat) -> None: ...
 
 class Min(Convertible[_M, _N]):
     expected_type: type[_M]
     allow_none: _N
     min: float
     @overload
     def __init__(
@@ -177,22 +174,22 @@
     def __init__(
         self: Min[float, Literal[False]],
         *,
         expected_type: _ExpectedTypeParam[float] = ...,
         allow_none: Literal[False] = False,
         min: float,
     ) -> None: ...
-    @overload  # type:ignore[override]  # Different restrictions
-    def __set__(self: Min[int, Literal[True]], instance: Serialisable | Strict, value: _ConvertibleToInt | None) -> None: ...
+    @overload  # type: ignore[override]  # Different restrictions
+    def __set__(self: Min[int, Literal[True]], instance: Serialisable | Strict, value: ConvertibleToInt | None) -> None: ...
     @overload
-    def __set__(self: Min[int, Literal[False]], instance: Serialisable | Strict, value: _ConvertibleToInt) -> None: ...
+    def __set__(self: Min[int, Literal[False]], instance: Serialisable | Strict, value: ConvertibleToInt) -> None: ...
     @overload
-    def __set__(self: Min[float, Literal[True]], instance: Serialisable | Strict, value: _ConvertibleToFloat | None) -> None: ...
+    def __set__(self: Min[float, Literal[True]], instance: Serialisable | Strict, value: ConvertibleToFloat | None) -> None: ...
     @overload
-    def __set__(self: Min[float, Literal[False]], instance: Serialisable | Strict, value: _ConvertibleToFloat) -> None: ...
+    def __set__(self: Min[float, Literal[False]], instance: Serialisable | Strict, value: ConvertibleToFloat) -> None: ...
 
 class MinMax(Min[_M, _N], Max[_M, _N]):
     expected_type: type[_M]
     allow_none: _N
     @overload
     def __init__(
         self: MinMax[int, Literal[True]],
@@ -260,17 +257,15 @@
 class Bool(Convertible[bool, _N]):
     expected_type: type[bool]
     allow_none: _N
     @overload
     def __init__(self: Bool[Literal[True]], name: str | None = None, *, allow_none: Literal[True]) -> None: ...
     @overload
     def __init__(self: Bool[Literal[False]], name: str | None = None, *, allow_none: Literal[False] = False) -> None: ...
-    def __set__(  # type:ignore[override]  # Different restrictions
-        self, instance: Serialisable | Strict, value: _ConvertibleToBool
-    ) -> None: ...
+    def __set__(self, instance: Serialisable | Strict, value: _ConvertibleToBool) -> None: ...
 
 class String(Typed[str, _N]):
     allow_none: _N
     expected_type: type[str]
     @overload
     def __init__(self: String[Literal[True]], name: str | None = None, *, allow_none: Literal[True]) -> None: ...
     @overload
@@ -292,20 +287,20 @@
 
 class Default(Typed[_T, _N]):  # unused
     def __init__(
         self, name: Unused = None, *, expected_type: _ExpectedTypeParam[_T], allow_none: bool = False, defaults: Unused = {}
     ) -> None: ...
     def __call__(self) -> _T: ...
 
-# Note: Aliases types can't be infered. Anyway an alias means there's another option
-# incomplete: Make it generic with explicit getter/setter type arguments ?
+# Note: Aliases types can't be inferred. Anyway an alias means there's another option.
+# Incomplete: Make it generic with explicit getter/setter type arguments?
 class Alias(Descriptor[Incomplete]):
     alias: str
     def __init__(self, alias: str) -> None: ...
-    def __set__(self, instance: Serialisable | Strict, value: Incomplete) -> None: ...
+    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
     def __get__(self, instance: Serialisable | Strict, cls: Unused): ...
 
 class MatchPattern(Descriptor[_P], Generic[_P, _N]):
     allow_none: _N
     test_pattern: Pattern[bytes] | Pattern[str]
     pattern: str | Pattern[str] | bytes | Pattern[bytes]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/excel.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/excel.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from _typeshed import Incomplete
-from typing import TypeVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
 from . import Integer, MatchPattern, MinMax, Strict, String
+from .base import _M, _N
 from .serialisable import Serialisable
 
-_N = TypeVar("_N", bound=bool)
-_M = TypeVar("_M", int, float)
-
 class HexBinary(MatchPattern[str, Incomplete]):
     pattern: str
 
 class UniversalMeasure(MatchPattern[str, Incomplete]):
     pattern: str
 
 class TextPoint(MinMax[_M, _N]):
@@ -21,26 +18,26 @@
 
 Coordinate = Integer
 
 class Percentage(MinMax[float, Incomplete]):
     pattern: str
     min: float
     max: float
-    def __set__(self, instance: Serialisable | Strict, value: Incomplete) -> None: ...
+    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
 
 class Extension(Serialisable):
     uri: String[Literal[False]]
     def __init__(self, uri: str) -> None: ...
 
 class ExtensionList(Serialisable):
     ext: Incomplete
     def __init__(self, ext=()) -> None: ...
 
 class Relation(String[Incomplete]):
-    namespace: Incomplete
+    namespace: ClassVar[str]
     allow_none: bool
 
 class Base64Binary(MatchPattern[str, Incomplete]):
     pattern: str
 
 class Guid(MatchPattern[str, Incomplete]):
     pattern: str
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/nested.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/descriptors/nested.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,161 +1,167 @@
-from _typeshed import Incomplete, Unused
-from collections.abc import Callable
-from typing import Any, ClassVar, NoReturn, Protocol, TypeVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Unused
+from collections.abc import Iterable
+from typing import Any, ClassVar, Literal, NoReturn, overload
+from typing_extensions import TypeAlias
 
 from openpyxl.descriptors import Strict
 from openpyxl.descriptors.base import Bool, Convertible, Descriptor, Float, Integer, MinMax, NoneSet, Set, String
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.fill import Blip
 from openpyxl.xml.functions import Element
 
-from .base import _M, _N, _T, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt, _ExpectedTypeParam
-
-_T_co = TypeVar("_T_co", covariant=True)
-
-# Usually an Element() from either lxml or xml.etree (has a 'tag' element)
-class _HasTagAndGet(Protocol[_T_co]):
-    tag: Any  # str | None | Callable[..., Any]
-    def get(self, __value: str) -> _T_co | None: ...
-
-class _HasTagAndText(Protocol):
-    tag: str | Callable[..., Any]
-    text: str
+from ..xml._functions_overloads import _HasGet, _HasTagAndGet, _HasText
+from .base import _M, _N, _T, _ConvertibleToBool, _ExpectedTypeParam
 
 _NestedNoneSetParam: TypeAlias = _HasTagAndGet[_T | Literal["none"] | None] | _T | Literal["none"] | None
 
 # NOTE: type: ignore[misc]: Class does not reimplement the relevant methods, so runtime also has incompatible supertypes
 
 class Nested(Descriptor[_T]):
     nested: ClassVar[Literal[True]]
     attribute: ClassVar[str]
+    # Members optional in __init__
+    expected_type: type[_T]
+    allow_none: bool
+    namespace: str | None
+    # In usage, "Nested" is closed to "Typed" than "Descriptor", but doesn't use allow_none
+    def __init__(
+        self: Nested[_T],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
+        name: str | None = None,
+        *,
+        expected_type: _ExpectedTypeParam[_T],
+        allow_none: bool = False,
+        nested: Unused = True,
+        namespace: str | None = None,
+    ) -> None: ...
     def __get__(self, instance: Serialisable | Strict, cls: type | None) -> _T: ...
     def __set__(self, instance: Serialisable | Strict, value: _HasTagAndGet[_T] | _T) -> None: ...
-    def from_tree(self, node: _HasTagAndGet[_T]) -> _T: ...
-    def to_tree(
-        self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
-    ) -> Element: ...
+    def from_tree(self, node: _HasGet[_T]) -> _T: ...
+    @overload
+    def to_tree(self, tagname: Unused = None, value: None = None, namespace: Unused = None) -> None: ...  # type: ignore[overload-overlap]
+    @overload
+    def to_tree(self, tagname: str, value: object, namespace: str | None = None) -> Element: ...
 
 class NestedValue(Nested[_T], Convertible[_T, _N]):  # type: ignore[misc]
     @overload
     def __init__(
-        self: NestedValue[_T, Literal[True]],
+        self: NestedValue[_T, Literal[True]],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         name: str | None = None,
         *,
         expected_type: _ExpectedTypeParam[_T],
         allow_none: Literal[True],
     ) -> None: ...
     @overload
     def __init__(
-        self: NestedValue[_T, Literal[False]],
+        self: NestedValue[_T, Literal[False]],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         name: str | None = None,
         *,
         expected_type: _ExpectedTypeParam[_T],
         allow_none: Literal[False] = False,
     ) -> None: ...
     @overload
     def __get__(self: NestedValue[_T, Literal[True]], instance: Serialisable | Strict, cls: type | None = None) -> _T | None: ...
     @overload
     def __get__(self: NestedValue[_T, Literal[False]], instance: Serialisable | Strict, cls: type | None = None) -> _T: ...
     # NOTE: It is currently impossible to make a generic based on the parameter type of another generic
-    # So we implement explicitely the types used internally
+    # So we implement explicitly the types used internally
     # str | Blip
     @overload
     def __set__(
-        self: NestedValue[str, bool] | NestedValue[Blip, bool],
+        self: NestedValue[str, _N] | NestedValue[Blip, _N],
         instance: Serialisable | Strict,
         value: object,  # Not[None] when _N = False
     ) -> None: ...
     # bool
     @overload
     def __set__(
-        self: NestedValue[bool, bool],
+        self: NestedValue[bool, _N],
         instance: Serialisable | Strict,
         value: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool,
     ) -> None: ...
     # int
     @overload
     def __set__(
         self: NestedValue[int, Literal[True]],
         instance: Serialisable | Strict,
-        value: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
+        value: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
     ) -> None: ...
     @overload
     def __set__(
         self: NestedValue[int, Literal[False]],
         instance: Serialisable | Strict,
-        value: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt,
+        value: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt,
     ) -> None: ...
     # float
     @overload
     def __set__(
         self: NestedValue[float, Literal[True]],
         instance: Serialisable | Strict,
-        value: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None,
+        value: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None,
     ) -> None: ...
     @overload
     def __set__(
         self: NestedValue[float, Literal[False]],
         instance: Serialisable | Strict,
-        value: _HasTagAndGet[_ConvertibleToFloat] | _ConvertibleToFloat,
+        value: _HasTagAndGet[ConvertibleToFloat] | ConvertibleToFloat,
     ) -> None: ...
     # Anything else
     @overload
     def __set__(
         self: NestedValue[_T, Literal[True]],
         instance: Serialisable | Strict,
         value: _HasTagAndGet[_T | int | Any] | _T | int | Any | None,
     ) -> None: ...
 
 class NestedText(NestedValue[_T, _N]):
     @overload
     def __init__(
-        self: NestedText[_T, Literal[True]],
+        self: NestedText[_T, Literal[True]],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         name: str | None = None,
         *,
         expected_type: _ExpectedTypeParam[_T],
         allow_none: Literal[True],
     ) -> None: ...
     @overload
     def __init__(
-        self: NestedText[_T, Literal[False]],
+        self: NestedText[_T, Literal[False]],  # pyright: ignore[reportInvalidTypeVarUse]  #11780
         name: str | None = None,
         *,
         expected_type: _ExpectedTypeParam[_T],
         allow_none: Literal[False] = False,
     ) -> None: ...
     @overload
     def __get__(self: NestedText[_T, Literal[True]], instance: Serialisable | Strict, cls: type | None = None) -> _T | None: ...
     @overload
     def __get__(self: NestedText[_T, Literal[False]], instance: Serialisable | Strict, cls: type | None = None) -> _T: ...
     # NOTE: It is currently impossible to make a generic based on the parameter type of another generic
-    # So we implement explicitely the types used internally
+    # So we implement explicitly the types used internally
     # str
     @overload
-    def __set__(  # type: ignore[misc] # Incompatible return type because of NoReturn
-        self: NestedValue[str, bool], instance: Serialisable | Strict, value: object  # Not[None] when _N = False
+    def __set__(  # type: ignore[overload-overlap]
+        self: NestedText[str, _N], instance: Serialisable | Strict, value: object  # Not[None] when _N = False
     ) -> None: ...
     # int
     @overload
     def __set__(
-        self: NestedValue[int, Literal[True]], instance: Serialisable | Strict, value: _ConvertibleToInt | None
+        self: NestedText[int, Literal[True]], instance: Serialisable | Strict, value: ConvertibleToInt | None
     ) -> None: ...
     @overload
-    def __set__(self: NestedValue[int, Literal[False]], instance: Serialisable | Strict, value: _ConvertibleToInt) -> None: ...
+    def __set__(self: NestedText[int, Literal[False]], instance: Serialisable | Strict, value: ConvertibleToInt) -> None: ...
     # If expected type (_T) is not str, it's impossible to use an Element as the value
     @overload
-    def __set__(self: NestedValue[_T, Literal[True]], instance: Serialisable | Strict, value: _HasTagAndGet[Any]) -> NoReturn: ...
+    def __set__(self: NestedText[_T, Literal[True]], instance: Serialisable | Strict, value: _HasTagAndGet[Any]) -> NoReturn: ...
     # Anything else
     @overload
-    def __set__(self: NestedValue[_T, Literal[True]], instance: Serialisable | Strict, value: _T | int | Any | None) -> None: ...
-    def from_tree(self, node: _HasTagAndText) -> str: ...  # type: ignore[override]
-    def to_tree(
-        self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
-    ) -> Element: ...
+    def __set__(self: NestedText[_T, Literal[True]], instance: Serialisable | Strict, value: _T | int | Any | None) -> None: ...
+    def from_tree(self, node: _HasText) -> str: ...  # type: ignore[override]
+    @overload
+    def to_tree(self, tagname: Unused = None, value: None = None, namespace: Unused = None) -> None: ...  # type: ignore[overload-overlap]
+    @overload
+    def to_tree(self, tagname: str, value: object, namespace: str | None = None) -> Element: ...
 
 class NestedFloat(NestedValue[float, _N], Float[_N]):  # type: ignore[misc]
     @overload
     def __init__(self: NestedFloat[Literal[True]], name: str | None = None, *, allow_none: Literal[True]) -> None: ...
     @overload
     def __init__(self: NestedFloat[Literal[False]], name: str | None = None, *, allow_none: Literal[False] = False) -> None: ...
 
@@ -172,23 +178,23 @@
     def __init__(self: NestedString[Literal[False]], name: str | None = None, *, allow_none: Literal[False] = False) -> None: ...
 
 class NestedBool(NestedValue[bool, _N], Bool[_N]):  # type: ignore[misc]
     @overload
     def __init__(self: NestedBool[Literal[True]], name: str | None = None, *, allow_none: Literal[True]) -> None: ...
     @overload
     def __init__(self: NestedBool[Literal[False]], name: str | None = None, *, allow_none: Literal[False] = False) -> None: ...
-    def __set__(  # type:ignore[override]  # Different restrictions
-        self, instance: Serialisable | Strict, value: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool
-    ) -> None: ...
-    def from_tree(self, node) -> bool: ...  # type: ignore[override]  # Actual overriden return type
+    def __set__(self, instance: Serialisable | Strict, value: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool) -> None: ...
+    def from_tree(self, node: _HasGet[bool]) -> bool: ...
 
-class NestedNoneSet(Nested[_T | None], NoneSet[_T]):  # type: ignore[misc]
+class NestedNoneSet(Nested[_T | None], NoneSet[_T]):
+    def __init__(self, name: str | None = None, *, values: Iterable[_T | None]) -> None: ...
     def __set__(self, instance: Serialisable | Strict, value: _NestedNoneSetParam[_T]) -> None: ...
 
-class NestedSet(Nested[_T], Set[_T]): ...
+class NestedSet(Nested[_T], Set[_T]):
+    def __init__(self, name: str | None = None, *, values: Iterable[_T]) -> None: ...
 
 class NestedMinMax(Nested[_M], MinMax[_M, _N]):  # type: ignore[misc]
     @overload
     def __init__(
         self: NestedMinMax[int, Literal[True]],
         *,
         expected_type: _ExpectedTypeParam[int],
@@ -224,48 +230,49 @@
         min: float,
         max: float,
     ) -> None: ...
     @overload
     def __get__(self: NestedMinMax[_M, Literal[True]], instance: Serialisable | Strict, cls: type | None = None) -> _M | None: ...
     @overload
     def __get__(self: NestedMinMax[_M, Literal[False]], instance: Serialisable | Strict, cls: type | None = None) -> _M: ...
-    @overload  # type:ignore[override]  # Different restrictions
+    @overload  # type: ignore[override]  # Different restrictions
     def __set__(
         self: NestedMinMax[int, Literal[True]],
         instance: Serialisable | Strict,
-        value: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
+        value: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
     ) -> None: ...
     @overload
     def __set__(
         self: NestedMinMax[int, Literal[False]],
         instance: Serialisable | Strict,
-        value: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt,
+        value: _HasTagAndGet[ConvertibleToInt] | ConvertibleToInt,
     ) -> None: ...
     @overload
     def __set__(
         self: NestedMinMax[float, Literal[True]],
         instance: Serialisable | Strict,
-        value: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None,
+        value: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None,
     ) -> None: ...
     @overload
     def __set__(
         self: NestedMinMax[float, Literal[False]],
         instance: Serialisable | Strict,
-        value: _HasTagAndGet[_ConvertibleToFloat] | _ConvertibleToFloat,
+        value: _HasTagAndGet[ConvertibleToFloat] | ConvertibleToFloat,
     ) -> None: ...
 
 class EmptyTag(Nested[bool], Bool[_N]):  # type: ignore[misc]
     @overload
     def __init__(self: EmptyTag[Literal[True]], name: str | None = None, *, allow_none: Literal[True]) -> None: ...
     @overload
     def __init__(self: EmptyTag[Literal[False]], name: str | None = None, *, allow_none: Literal[False] = False) -> None: ...
     @overload
     def __get__(self: EmptyTag[Literal[True]], instance: Serialisable | Strict, cls: type | None = None) -> bool | None: ...
     @overload
     def __get__(self: EmptyTag[Literal[False]], instance: Serialisable | Strict, cls: type | None = None) -> bool: ...
-    def __set__(  # type:ignore[override]  # Different restrictions
-        self, instance: Serialisable | Strict, value: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool
+    def __set__(self, instance: Serialisable | Strict, value: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool) -> None: ...
+    def from_tree(self, node: Unused) -> Literal[True]: ...
+    @overload
+    def to_tree(  # type: ignore[overload-overlap]
+        self, tagname: Unused = None, value: None = None, namespace: Unused = None
     ) -> None: ...
-    def from_tree(self, node: Unused) -> Literal[True]: ...  # type: ignore[override]  # Actual overriden return type
-    def to_tree(
-        self, tagname: Incomplete | None = None, value: Incomplete | None = None, namespace: Incomplete | None = None
-    ) -> Element: ...
+    @overload
+    def to_tree(self, tagname: str, value: object, namespace: str | None = None) -> Element: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/serialisable.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/merge.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from typing import ClassVar
 
-from openpyxl.descriptors import MetaSerialisable
+from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.worksheet.worksheet import Worksheet
 
-KEYWORDS: Incomplete
-seq_types: Incomplete
+from .cell_range import CellRange
 
-class Serialisable(metaclass=MetaSerialisable):
-    # These dunders are always set at runtime by MetaSerialisable so they can't be None
+class MergeCell(CellRange):
+    tagname: ClassVar[str]
+    # Same as CellRange.coord
+    # https://github.com/python/mypy/issues/6700
+    @property
+    def ref(self) -> str: ...
     __attrs__: ClassVar[tuple[str, ...]]
-    __nested__: ClassVar[tuple[str, ...]]
+    def __init__(self, ref: Incomplete | None = None) -> None: ...
+    def __copy__(self): ...
+
+class MergeCells(Serialisable):
+    tagname: ClassVar[str]
+    # Overwritten by property below
+    # count: Integer
+    mergeCell: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    __namespaced__: ClassVar[tuple[tuple[str, str], ...]]
-    idx_base: int
+    __attrs__: ClassVar[tuple[str, ...]]
+    def __init__(self, count: Unused = None, mergeCell=()) -> None: ...
     @property
-    # TODO: needs overrides in many sub-classes
-    # @abstractmethod
-    def tagname(self) -> str: ...
-    namespace: Incomplete
-    @classmethod
-    def from_tree(cls, node): ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
-    def __iter__(self): ...
-    def __eq__(self, other): ...
-    def __ne__(self, other): ...
-    def __hash__(self) -> int: ...
-    def __add__(self, other): ...
+    def count(self) -> int: ...
+
+class MergedCellRange(CellRange):
+    ws: Worksheet
+    start_cell: Incomplete
+    def __init__(self, worksheet: Worksheet, coord) -> None: ...
+    def format(self) -> None: ...
+    def __contains__(self, coord: str) -> bool: ...
     def __copy__(self): ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/colors.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/colors.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from _typeshed import Incomplete
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete
+from typing import ClassVar, Final, Literal, overload
+from typing_extensions import TypeAlias
 
 from openpyxl.descriptors import Strict, Typed
-from openpyxl.descriptors.base import Alias, Integer, MinMax, Set, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Integer, MinMax, Set, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import EmptyTag, NestedInteger, NestedNoneSet, NestedValue, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import EmptyTag, NestedInteger, NestedNoneSet, NestedValue, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _ColorSetType: TypeAlias = Literal[
     "dk1", "lt1", "dk2", "lt2", "accent1", "accent2", "accent3", "accent4", "accent5", "accent6", "hlink", "folHlink"
 ]
 _SystemColorVal: TypeAlias = Literal[
     "scrollBar",
     "background",
     "activeCaption",
@@ -39,15 +41,15 @@
     "infoBk",
     "hotLight",
     "gradientActiveCaption",
     "gradientInactiveCaption",
     "menuHighlight",
     "menuBar",
 ]
-_SchemeColorVal: TypeAlias = Literal[
+_SchemeColors: TypeAlias = Literal[
     "bg1",
     "tx1",
     "bg2",
     "tx2",
     "accent1",
     "accent2",
     "accent3",
@@ -251,22 +253,22 @@
     "wheat",
     "white",
     "whiteSmoke",
     "yellow",
     "yellowGreen",
 ]
 
-PRESET_COLORS: list[_PresetColors]
-SCHEME_COLORS: Incomplete
+PRESET_COLORS: Final[list[_PresetColors]]
+SCHEME_COLORS: Final[list[_SchemeColors]]
 
 class Transform(Serialisable): ...
 
 class SystemColor(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     tint: NestedInteger[Literal[True]]
     shade: NestedInteger[Literal[True]]
     comp: Typed[Transform, Literal[True]]
     inv: Typed[Transform, Literal[True]]
     gray: Typed[Transform, Literal[True]]
     alpha: NestedInteger[Literal[True]]
     alphaOff: NestedInteger[Literal[True]]
@@ -294,63 +296,63 @@
     val: Set[_SystemColorVal]
     lastClr: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         val: _SystemColorVal = "windowText",
         lastClr: Incomplete | None = None,
-        tint: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        shade: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        tint: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        shade: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         comp: Transform | None = None,
         inv: Transform | None = None,
         gray: Transform | None = None,
-        alpha: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        alphaOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        alphaMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        hue: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        hueOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        hueMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        sat: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        satOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        satMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        lum: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        lumOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        lumMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        red: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        redOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        redMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        green: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        greenOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        greenMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        blue: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        blueOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        blueMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        alpha: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        alphaOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        alphaMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        hue: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        hueOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        hueMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        sat: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        satOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        satMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        lum: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        lumOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        lumMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        red: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        redOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        redMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        green: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        greenOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        greenMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        blue: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        blueOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        blueMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         gamma: Transform | None = None,
         invGamma: Transform | None = None,
     ) -> None: ...
 
 class HSLColor(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     hue: Integer[Literal[False]]
     sat: MinMax[float, Literal[False]]
     lum: MinMax[float, Literal[False]]
-    def __init__(self, hue: _ConvertibleToInt, sat: _ConvertibleToFloat, lum: _ConvertibleToFloat) -> None: ...
+    def __init__(self, hue: ConvertibleToInt, sat: ConvertibleToFloat, lum: ConvertibleToFloat) -> None: ...
 
 class RGBPercent(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     r: MinMax[float, Literal[False]]
     g: MinMax[float, Literal[False]]
     b: MinMax[float, Literal[False]]
-    def __init__(self, r: _ConvertibleToFloat, g: _ConvertibleToFloat, b: _ConvertibleToFloat) -> None: ...
+    def __init__(self, r: ConvertibleToFloat, g: ConvertibleToFloat, b: ConvertibleToFloat) -> None: ...
 
 _RGBPercent: TypeAlias = RGBPercent
 
 class SchemeColor(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     tint: NestedInteger[Literal[True]]
     shade: NestedInteger[Literal[True]]
     comp: EmptyTag[Literal[True]]
     inv: NestedInteger[Literal[True]]
     gray: NestedInteger[Literal[True]]
     alpha: NestedInteger[Literal[True]]
     alphaOff: NestedInteger[Literal[True]]
@@ -371,87 +373,87 @@
     greenOff: NestedInteger[Literal[True]]
     greenMod: NestedInteger[Literal[True]]
     blue: NestedInteger[Literal[True]]
     blueOff: NestedInteger[Literal[True]]
     blueMod: NestedInteger[Literal[True]]
     gamma: EmptyTag[Literal[True]]
     invGamma: EmptyTag[Literal[True]]
-    val: Set[_SchemeColorVal]
+    val: Set[_SchemeColors]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
-        tint: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        shade: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        tint: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        shade: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         comp: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        inv: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        gray: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        alpha: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        alphaOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        alphaMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        hue: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        hueOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        hueMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        sat: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        satOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        satMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        lum: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        lumOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        lumMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        red: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        redOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        redMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        green: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        greenOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        greenMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        blue: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        blueOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        blueMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        inv: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        gray: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        alpha: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        alphaOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        alphaMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        hue: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        hueOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        hueMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        sat: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        satOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        satMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        lum: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        lumOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        lumMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        red: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        redOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        redMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        green: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        greenOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        greenMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        blue: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        blueOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        blueMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         gamma: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         invGamma: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         *,
-        val: _SchemeColorVal,
+        val: _SchemeColors,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        tint: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        shade: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
+        tint: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        shade: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
         comp: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None,
-        inv: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        gray: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        alpha: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        alphaOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        alphaMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        hue: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        hueOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        hueMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        sat: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        satOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        satMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        lum: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        lumOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        lumMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        red: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        redOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        redMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        green: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        greenOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        greenMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        blue: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        blueOff: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
-        blueMod: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None,
+        inv: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        gray: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        alpha: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        alphaOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        alphaMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        hue: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        hueOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        hueMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        sat: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        satOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        satMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        lum: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        lumOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        lumMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        red: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        redOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        redMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        green: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        greenOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        greenMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        blue: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        blueOff: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
+        blueMod: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None,
         gamma: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None,
         invGamma: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None,
-        val: _SchemeColorVal,
+        val: _SchemeColors,
     ) -> None: ...
 
 class ColorChoice(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     scrgbClr: Typed[_RGBPercent, Literal[True]]
     RGBPercent: Alias
     srgbClr: NestedValue[_RGBPercent, Literal[True]]
     RGB: Alias
     hslClr: Typed[HSLColor, Literal[True]]
     sysClr: Typed[SystemColor, Literal[True]]
     schemeClr: Typed[SystemColor, Literal[True]]
@@ -463,18 +465,18 @@
         srgbClr: _HasTagAndGet[_RGBPercent | None] | _RGBPercent | None = None,
         hslClr: HSLColor | None = None,
         sysClr: SystemColor | None = None,
         schemeClr: SystemColor | None = None,
         prstClr: _NestedNoneSetParam[_PresetColors] = None,
     ) -> None: ...
 
-_COLOR_SET: tuple[_ColorSetType, ...]
+_COLOR_SET: Final[tuple[_ColorSetType, ...]]
 
 class ColorMapping(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     bg1: Set[_ColorSetType]
     tx1: Set[_ColorSetType]
     bg2: Set[_ColorSetType]
     tx2: Set[_ColorSetType]
     accent1: Set[_ColorSetType]
     accent2: Set[_ColorSetType]
     accent3: Set[_ColorSetType]
@@ -497,11 +499,12 @@
         accent5: str = "accent5",
         accent6: str = "accent6",
         hlink: str = "hlink",
         folHlink: str = "folHlink",
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
-class ColorChoiceDescriptor(Typed[ColorChoice, Incomplete]):
+class ColorChoiceDescriptor(Typed[ColorChoice, Literal[True]]):
     expected_type: type[ColorChoice]
     allow_none: Literal[True]
-    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
+    def __init__(self, name: str | None = None) -> None: ...
+    def __set__(self, instance: Serialisable | Strict, value: str | ColorChoice | None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/connector.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/connector.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import ClassVar, overload
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt
+from typing import ClassVar, Literal, overload
 
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
 from openpyxl.descriptors import Typed
-from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.geometry import ShapeStyle
 from openpyxl.drawing.properties import NonVisualDrawingProps, NonVisualDrawingShapeProps
 
 class Connection(Serialisable):
     id: Integer[Literal[False]]
     idx: Integer[Literal[False]]
-    def __init__(self, id: _ConvertibleToInt, idx: _ConvertibleToInt) -> None: ...
+    def __init__(self, id: ConvertibleToInt, idx: ConvertibleToInt) -> None: ...
 
 class ConnectorLocking(Serialisable):
     extLst: Typed[ExtensionList, Literal[True]]
     def __init__(self, extLst: ExtensionList | None = None) -> None: ...
 
 class NonVisualConnectorProperties(Serialisable):
     cxnSpLocks: Typed[ConnectorLocking, Literal[True]]
@@ -35,15 +35,15 @@
 class ConnectorNonVisual(Serialisable):
     cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
     cNvCxnSpPr: Typed[NonVisualConnectorProperties, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cNvPr: NonVisualDrawingProps, cNvCxnSpPr: NonVisualConnectorProperties) -> None: ...
 
 class ConnectorShape(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     nvCxnSpPr: Typed[ConnectorNonVisual, Literal[False]]
     spPr: Typed[GraphicalProperties, Literal[False]]
     style: Typed[ShapeStyle, Literal[True]]
     macro: String[Literal[True]]
     fPublished: Bool[Literal[True]]
     def __init__(
         self,
@@ -51,15 +51,15 @@
         spPr: GraphicalProperties,
         style: ShapeStyle | None = None,
         macro: str | None = None,
         fPublished: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class ShapeMeta(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
     cNvSpPr: Typed[NonVisualDrawingShapeProps, Literal[False]]
     def __init__(self, cNvPr: NonVisualDrawingProps, cNvSpPr: NonVisualDrawingShapeProps) -> None: ...
 
 class Shape(Serialisable):
     macro: String[Literal[True]]
     textlink: String[Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/drawing.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/drawing.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from _typeshed import Incomplete
 
+from .spreadsheet_drawing import AbsoluteAnchor, OneCellAnchor
+
 class Drawing:
     count: int
     name: str
     description: str
     coordinates: Incomplete
     left: int
     top: int
     resize_proportional: bool
     rotation: int
     anchortype: str
     anchorcol: int
     anchorrow: int
     def __init__(self) -> None: ...
     @property
-    def width(self): ...
+    def width(self) -> int: ...
     @width.setter
-    def width(self, w) -> None: ...
+    def width(self, w: int) -> None: ...
     @property
-    def height(self): ...
+    def height(self) -> int: ...
     @height.setter
-    def height(self, h) -> None: ...
+    def height(self, h: int) -> None: ...
     def set_dimension(self, w: int = 0, h: int = 0) -> None: ...
     @property
-    def anchor(self): ...
+    def anchor(self) -> AbsoluteAnchor | OneCellAnchor: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/effect.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/effect.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-from _typeshed import Incomplete
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
-
-from openpyxl.descriptors.base import (
-    Bool,
-    Float,
-    Integer,
-    Set,
-    String,
-    Typed,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from _typeshed import ConvertibleToFloat, ConvertibleToInt
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
+
+from openpyxl.descriptors.base import Bool, Float, Integer, Set, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 from .colors import ColorChoice
 
 _FillOverlayEffectBlend: TypeAlias = Literal["over", "mult", "screen", "darken", "lighten"]
 _EffectContainerType: TypeAlias = Literal["sib", "tree"]
 _Algn: TypeAlias = Literal["tl", "t", "tr", "l", "ctr", "r", "bl", "b", "br"]
@@ -40,33 +30,33 @@
     "shdw17",
     "shdw18",
     "shdw19",
     "shdw20",
 ]
 
 class TintEffect(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     hue: Integer[Literal[False]]
     amt: Integer[Literal[False]]
-    def __init__(self, hue: _ConvertibleToInt = 0, amt: _ConvertibleToInt = 0) -> None: ...
+    def __init__(self, hue: ConvertibleToInt = 0, amt: ConvertibleToInt = 0) -> None: ...
 
 class LuminanceEffect(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     bright: Integer[Literal[False]]
     contrast: Integer[Literal[False]]
-    def __init__(self, bright: _ConvertibleToInt = 0, contrast: _ConvertibleToInt = 0) -> None: ...
+    def __init__(self, bright: ConvertibleToInt = 0, contrast: ConvertibleToInt = 0) -> None: ...
 
 class HSLEffect(Serialisable):
     hue: Integer[Literal[False]]
     sat: Integer[Literal[False]]
     lum: Integer[Literal[False]]
-    def __init__(self, hue: _ConvertibleToInt, sat: _ConvertibleToInt, lum: _ConvertibleToInt) -> None: ...
+    def __init__(self, hue: ConvertibleToInt, sat: ConvertibleToInt, lum: ConvertibleToInt) -> None: ...
 
 class GrayscaleEffect(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
 
 class FillOverlayEffect(Serialisable):
     blend: Set[_FillOverlayEffectBlend]
     def __init__(self, blend: _FillOverlayEffectBlend) -> None: ...
 
 class DuotoneEffect(Serialisable): ...
 class ColorReplaceEffect(Serialisable): ...
@@ -80,27 +70,27 @@
     def __init__(self, useA: _ConvertibleToBool | None = None, *, clrFrom: Color, clrTo: Color) -> None: ...
     @overload
     def __init__(self, useA: _ConvertibleToBool | None, clrFrom: Color, clrTo: Color) -> None: ...
 
 class BlurEffect(Serialisable):
     rad: Float[Literal[False]]
     grow: Bool[Literal[True]]
-    def __init__(self, rad: _ConvertibleToFloat, grow: _ConvertibleToBool | None = None) -> None: ...
+    def __init__(self, rad: ConvertibleToFloat, grow: _ConvertibleToBool | None = None) -> None: ...
 
 class BiLevelEffect(Serialisable):
     thresh: Integer[Literal[False]]
-    def __init__(self, thresh: _ConvertibleToInt) -> None: ...
+    def __init__(self, thresh: ConvertibleToInt) -> None: ...
 
 class AlphaReplaceEffect(Serialisable):
     a: Integer[Literal[False]]
-    def __init__(self, a: _ConvertibleToInt) -> None: ...
+    def __init__(self, a: ConvertibleToInt) -> None: ...
 
 class AlphaModulateFixedEffect(Serialisable):
     amt: Integer[Literal[False]]
-    def __init__(self, amt: _ConvertibleToInt) -> None: ...
+    def __init__(self, amt: ConvertibleToInt) -> None: ...
 
 class EffectContainer(Serialisable):
     type: Set[_EffectContainerType]
     name: String[Literal[True]]
     def __init__(self, type: _EffectContainerType, name: str | None = None) -> None: ...
 
 class AlphaModulateEffect(Serialisable):
@@ -109,100 +99,104 @@
 
 class AlphaInverseEffect(Serialisable): ...
 class AlphaFloorEffect(Serialisable): ...
 class AlphaCeilingEffect(Serialisable): ...
 
 class AlphaBiLevelEffect(Serialisable):
     thresh: Integer[Literal[False]]
-    def __init__(self, thresh: _ConvertibleToInt) -> None: ...
+    def __init__(self, thresh: ConvertibleToInt) -> None: ...
 
 class GlowEffect(ColorChoice):
     rad: Float[Literal[False]]
-    scrgbClr: Incomplete
-    srgbClr: Incomplete
-    hslClr: Incomplete
-    sysClr: Incomplete
-    schemeClr: Incomplete
-    prstClr: Incomplete
+    # Same as parent
+    # scrgbClr = ColorChoice.scrgbClr
+    # srgbClr = ColorChoice.srgbClr
+    # hslClr = ColorChoice.hslClr
+    # sysClr = ColorChoice.sysClr
+    # schemeClr = ColorChoice.schemeClr
+    # prstClr = ColorChoice.prstClr
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, rad: _ConvertibleToFloat, **kw) -> None: ...
+    def __init__(self, rad: ConvertibleToFloat, **kw) -> None: ...
 
 class InnerShadowEffect(ColorChoice):
     blurRad: Float[Literal[False]]
     dist: Float[Literal[False]]
     dir: Integer[Literal[False]]
-    scrgbClr: Incomplete
-    srgbClr: Incomplete
-    hslClr: Incomplete
-    sysClr: Incomplete
-    schemeClr: Incomplete
-    prstClr: Incomplete
+    # Same as parent
+    # scrgbClr = ColorChoice.scrgbClr
+    # srgbClr = ColorChoice.srgbClr
+    # hslClr = ColorChoice.hslClr
+    # sysClr = ColorChoice.sysClr
+    # schemeClr = ColorChoice.schemeClr
+    # prstClr = ColorChoice.prstClr
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, blurRad: _ConvertibleToFloat, dist: _ConvertibleToFloat, dir: _ConvertibleToInt, **kw) -> None: ...
+    def __init__(self, blurRad: ConvertibleToFloat, dist: ConvertibleToFloat, dir: ConvertibleToInt, **kw) -> None: ...
 
 class OuterShadow(ColorChoice):
-    tagname: str
+    tagname: ClassVar[str]
     blurRad: Float[Literal[True]]
     dist: Float[Literal[True]]
     dir: Integer[Literal[True]]
     sx: Integer[Literal[True]]
     sy: Integer[Literal[True]]
     kx: Integer[Literal[True]]
     ky: Integer[Literal[True]]
     algn: Set[_Algn]
     rotWithShape: Bool[Literal[True]]
-    scrgbClr: Incomplete
-    srgbClr: Incomplete
-    hslClr: Incomplete
-    sysClr: Incomplete
-    schemeClr: Incomplete
-    prstClr: Incomplete
+    # Same as parent
+    # scrgbClr = ColorChoice.scrgbClr
+    # srgbClr = ColorChoice.srgbClr
+    # hslClr = ColorChoice.hslClr
+    # sysClr = ColorChoice.sysClr
+    # schemeClr = ColorChoice.schemeClr
+    # prstClr = ColorChoice.prstClr
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
-        blurRad: _ConvertibleToFloat | None = None,
-        dist: _ConvertibleToFloat | None = None,
-        dir: _ConvertibleToInt | None = None,
-        sx: _ConvertibleToInt | None = None,
-        sy: _ConvertibleToInt | None = None,
-        kx: _ConvertibleToInt | None = None,
-        ky: _ConvertibleToInt | None = None,
+        blurRad: ConvertibleToFloat | None = None,
+        dist: ConvertibleToFloat | None = None,
+        dir: ConvertibleToInt | None = None,
+        sx: ConvertibleToInt | None = None,
+        sy: ConvertibleToInt | None = None,
+        kx: ConvertibleToInt | None = None,
+        ky: ConvertibleToInt | None = None,
         *,
         algn: _Algn,
         rotWithShape: _ConvertibleToBool | None = None,
         **kw,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        blurRad: _ConvertibleToFloat | None,
-        dist: _ConvertibleToFloat | None,
-        dir: _ConvertibleToInt | None,
-        sx: _ConvertibleToInt | None,
-        sy: _ConvertibleToInt | None,
-        kx: _ConvertibleToInt | None,
-        ky: _ConvertibleToInt | None,
+        blurRad: ConvertibleToFloat | None,
+        dist: ConvertibleToFloat | None,
+        dir: ConvertibleToInt | None,
+        sx: ConvertibleToInt | None,
+        sy: ConvertibleToInt | None,
+        kx: ConvertibleToInt | None,
+        ky: ConvertibleToInt | None,
         algn: _Algn,
         rotWithShape: _ConvertibleToBool | None = None,
         **kw,
     ) -> None: ...
 
 class PresetShadowEffect(ColorChoice):
     prst: Set[_PresetShadowEffectPrst]
     dist: Float[Literal[False]]
     dir: Integer[Literal[False]]
-    scrgbClr: Incomplete
-    srgbClr: Incomplete
-    hslClr: Incomplete
-    sysClr: Incomplete
-    schemeClr: Incomplete
-    prstClr: Incomplete
+    # Same as parent
+    # scrgbClr = ColorChoice.scrgbClr
+    # srgbClr = ColorChoice.srgbClr
+    # hslClr = ColorChoice.hslClr
+    # sysClr = ColorChoice.sysClr
+    # schemeClr = ColorChoice.schemeClr
+    # prstClr = ColorChoice.prstClr
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, prst: _PresetShadowEffectPrst, dist: _ConvertibleToFloat, dir: _ConvertibleToInt, **kw) -> None: ...
+    def __init__(self, prst: _PresetShadowEffectPrst, dist: ConvertibleToFloat, dir: ConvertibleToInt, **kw) -> None: ...
 
 class ReflectionEffect(Serialisable):
     blurRad: Float[Literal[False]]
     stA: Integer[Literal[False]]
     stPos: Integer[Literal[False]]
     endA: Integer[Literal[False]]
     endPos: Integer[Literal[False]]
@@ -213,33 +207,33 @@
     sy: Integer[Literal[False]]
     kx: Integer[Literal[False]]
     ky: Integer[Literal[False]]
     algn: Set[_Algn]
     rotWithShape: Bool[Literal[True]]
     def __init__(
         self,
-        blurRad: _ConvertibleToFloat,
-        stA: _ConvertibleToInt,
-        stPos: _ConvertibleToInt,
-        endA: _ConvertibleToInt,
-        endPos: _ConvertibleToInt,
-        dist: _ConvertibleToFloat,
-        dir: _ConvertibleToInt,
-        fadeDir: _ConvertibleToInt,
-        sx: _ConvertibleToInt,
-        sy: _ConvertibleToInt,
-        kx: _ConvertibleToInt,
-        ky: _ConvertibleToInt,
+        blurRad: ConvertibleToFloat,
+        stA: ConvertibleToInt,
+        stPos: ConvertibleToInt,
+        endA: ConvertibleToInt,
+        endPos: ConvertibleToInt,
+        dist: ConvertibleToFloat,
+        dir: ConvertibleToInt,
+        fadeDir: ConvertibleToInt,
+        sx: ConvertibleToInt,
+        sy: ConvertibleToInt,
+        kx: ConvertibleToInt,
+        ky: ConvertibleToInt,
         algn: _Algn,
         rotWithShape: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class SoftEdgesEffect(Serialisable):
     rad: Float[Literal[False]]
-    def __init__(self, rad: _ConvertibleToFloat) -> None: ...
+    def __init__(self, rad: ConvertibleToFloat) -> None: ...
 
 class EffectList(Serialisable):
     blur: Typed[BlurEffect, Literal[True]]
     fillOverlay: Typed[FillOverlayEffect, Literal[True]]
     glow: Typed[GlowEffect, Literal[True]]
     innerShdw: Typed[InnerShadowEffect, Literal[True]]
     outerShdw: Typed[OuterShadow, Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/fill.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/fill.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
-
-from openpyxl.descriptors.base import (
-    Alias,
-    Bool,
-    Integer,
-    MinMax,
-    NoneSet,
-    Set,
-    Typed,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
+
+from openpyxl.descriptors.base import Alias, Bool, Integer, MinMax, NoneSet, Set, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedNoneSet, NestedValue, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import NestedNoneSet, NestedValue, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.colors import ColorChoice, HSLColor, RGBPercent as _RGBPercent, SchemeColor, SystemColor, _PresetColors
 from openpyxl.drawing.effect import (
     AlphaBiLevelEffect,
     AlphaCeilingEffect,
     AlphaFloorEffect,
     AlphaInverseEffect,
@@ -34,14 +23,16 @@
     FillOverlayEffect,
     GrayscaleEffect,
     HSLEffect,
     LuminanceEffect,
     TintEffect,
 )
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _PatternFillPropertiesPrst: TypeAlias = Literal[
     "pct5",
     "pct10",
     "pct20",
     "pct25",
     "pct30",
     "pct40",
@@ -96,16 +87,16 @@
 ]
 _PropertiesFlip: TypeAlias = Literal["x", "y", "xy"]
 _TileInfoPropertiesAlgn: TypeAlias = Literal["tl", "t", "tr", "l", "ctr", "r", "bl", "b", "br"]
 _BlipCstate: TypeAlias = Literal["email", "screen", "print", "hqprint"]
 _PathShadePropertiesPath: TypeAlias = Literal["shape", "circle", "rect"]
 
 class PatternFillProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     prst: NoneSet[_PatternFillPropertiesPrst]
     preset: Alias
     fgClr: Typed[ColorChoice, Literal[True]]
     foreground: Alias
     bgClr: Typed[ColorChoice, Literal[True]]
     background: Alias
     __elements__: ClassVar[tuple[str, ...]]
@@ -113,75 +104,75 @@
         self,
         prst: _PatternFillPropertiesPrst | Literal["none"] | None = None,
         fgClr: ColorChoice | None = None,
         bgClr: ColorChoice | None = None,
     ) -> None: ...
 
 class RelativeRect(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     l: Incomplete
     left: Alias
     t: Incomplete
     top: Alias
     r: Incomplete
     right: Alias
     b: Incomplete
     bottom: Alias
     def __init__(
         self, l: Incomplete | None = None, t: Incomplete | None = None, r: Incomplete | None = None, b: Incomplete | None = None
     ) -> None: ...
 
 class StretchInfoProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     fillRect: Typed[RelativeRect, Literal[True]]
     def __init__(self, fillRect: RelativeRect = ...) -> None: ...
 
 class GradientStop(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     pos: MinMax[float, Literal[True]]
     scrgbClr: Typed[_RGBPercent, Literal[True]]
     RGBPercent: Alias
     srgbClr: NestedValue[_RGBPercent, Literal[True]]
     RGB: Alias
     hslClr: Typed[HSLColor, Literal[True]]
     sysClr: Typed[SystemColor, Literal[True]]
     schemeClr: Typed[SchemeColor, Literal[True]]
     prstClr: NestedNoneSet[_PresetColors]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        pos: _ConvertibleToFloat | None = None,
+        pos: ConvertibleToFloat | None = None,
         scrgbClr: _RGBPercent | None = None,
         srgbClr: _HasTagAndGet[_RGBPercent | None] | _RGBPercent | None = None,
         hslClr: HSLColor | None = None,
         sysClr: SystemColor | None = None,
         schemeClr: SchemeColor | None = None,
         prstClr: _NestedNoneSetParam[_PresetColors] = None,
     ) -> None: ...
 
 class LinearShadeProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     ang: Integer[Literal[False]]
     scaled: Bool[Literal[True]]
-    def __init__(self, ang: _ConvertibleToInt, scaled: _ConvertibleToBool | None = None) -> None: ...
+    def __init__(self, ang: ConvertibleToInt, scaled: _ConvertibleToBool | None = None) -> None: ...
 
 class PathShadeProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     path: Set[_PathShadePropertiesPath]
     fillToRect: Typed[RelativeRect, Literal[True]]
     def __init__(self, path: _PathShadePropertiesPath, fillToRect: RelativeRect | None = None) -> None: ...
 
 class GradientFillProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     flip: NoneSet[_PropertiesFlip]
     rotWithShape: Bool[Literal[True]]
     gsLst: Incomplete
     stop_list: Alias
     lin: Typed[LinearShadeProperties, Literal[True]]
     linear: Alias
     path: Typed[PathShadeProperties, Literal[True]]
@@ -194,15 +185,15 @@
         gsLst=(),
         lin: LinearShadeProperties | None = None,
         path: PathShadeProperties | None = None,
         tileRect: RelativeRect | None = None,
     ) -> None: ...
 
 class SolidColorFillProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     scrgbClr: Typed[_RGBPercent, Literal[True]]
     RGBPercent: Alias
     srgbClr: NestedValue[_RGBPercent, Literal[True]]
     RGB: Alias
     hslClr: Typed[HSLColor, Literal[True]]
     sysClr: Typed[SystemColor, Literal[True]]
     schemeClr: Typed[SchemeColor, Literal[True]]
@@ -215,16 +206,16 @@
         hslClr: HSLColor | None = None,
         sysClr: SystemColor | None = None,
         schemeClr: SchemeColor | None = None,
         prstClr: _NestedNoneSetParam[_PresetColors] = None,
     ) -> None: ...
 
 class Blip(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     cstate: NoneSet[_BlipCstate]
     embed: Incomplete
     link: Incomplete
     noGrp: Bool[Literal[True]]
     noSelect: Bool[Literal[True]]
     noRot: Bool[Literal[True]]
     noChangeAspect: Bool[Literal[True]]
@@ -293,34 +284,34 @@
     ty: Integer[Literal[True]]
     sx: Integer[Literal[True]]
     sy: Integer[Literal[True]]
     flip: NoneSet[_PropertiesFlip]
     algn: Set[_TileInfoPropertiesAlgn]
     def __init__(
         self,
-        tx: _ConvertibleToInt | None = None,
-        ty: _ConvertibleToInt | None = None,
-        sx: _ConvertibleToInt | None = None,
-        sy: _ConvertibleToInt | None = None,
+        tx: ConvertibleToInt | None = None,
+        ty: ConvertibleToInt | None = None,
+        sx: ConvertibleToInt | None = None,
+        sy: ConvertibleToInt | None = None,
         flip: _PropertiesFlip | Literal["none"] | None = None,
         *,
         algn: _TileInfoPropertiesAlgn,
     ) -> None: ...
 
 class BlipFillProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     dpi: Integer[Literal[True]]
     rotWithShape: Bool[Literal[True]]
     blip: Typed[Blip, Literal[True]]
     srcRect: Typed[RelativeRect, Literal[True]]
     tile: Typed[TileInfoProperties, Literal[True]]
     stretch: Typed[StretchInfoProperties, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        dpi: _ConvertibleToInt | None = None,
+        dpi: ConvertibleToInt | None = None,
         rotWithShape: _ConvertibleToBool | None = None,
         blip: Blip | None = None,
         tile: TileInfoProperties | None = None,
         stretch: StretchInfoProperties = ...,
         srcRect: RelativeRect | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/geometry.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/geometry.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
-
-from openpyxl.descriptors.base import (
-    Alias,
-    Bool,
-    Float,
-    Integer,
-    MinMax,
-    NoneSet,
-    Set,
-    String,
-    Typed,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
+
+from openpyxl.descriptors.base import Alias, Bool, Float, Integer, MinMax, NoneSet, Set, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import Coordinate, ExtensionList, Percentage
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.colors import Color
 
 _BevelPrst: TypeAlias = Literal[
     "relaxedInset",
     "circle",
@@ -334,114 +321,114 @@
     "plaqueTabs",
     "chartX",
     "chartStar",
     "chartPlus",
 ]
 
 class Point2D(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     x: Incomplete
     y: Incomplete
     def __init__(self, x: Incomplete | None = None, y: Incomplete | None = None) -> None: ...
 
 class PositiveSize2D(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     cx: Integer[Literal[False]]
     width: Alias
     cy: Integer[Literal[False]]
     height: Alias
-    def __init__(self, cx: _ConvertibleToInt, cy: _ConvertibleToInt) -> None: ...
+    def __init__(self, cx: ConvertibleToInt, cy: ConvertibleToInt) -> None: ...
 
 class Transform2D(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     rot: Integer[Literal[True]]
     flipH: Bool[Literal[True]]
     flipV: Bool[Literal[True]]
     off: Typed[Point2D, Literal[True]]
     ext: Typed[PositiveSize2D, Literal[True]]
     chOff: Typed[Point2D, Literal[True]]
     chExt: Typed[PositiveSize2D, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        rot: _ConvertibleToInt | None = None,
+        rot: ConvertibleToInt | None = None,
         flipH: _ConvertibleToBool | None = None,
         flipV: _ConvertibleToBool | None = None,
         off: Point2D | None = None,
         ext: PositiveSize2D | None = None,
         chOff: Point2D | None = None,
         chExt: PositiveSize2D | None = None,
     ) -> None: ...
 
 class GroupTransform2D(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     rot: Integer[Literal[True]]
     flipH: Bool[Literal[True]]
     flipV: Bool[Literal[True]]
     off = Typed(expected_type=Point2D, allow_none=True)
     ext = Typed(expected_type=PositiveSize2D, allow_none=True)
     chOff = Typed(expected_type=Point2D, allow_none=True)
     chExt = Typed(expected_type=PositiveSize2D, allow_none=True)
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        rot: _ConvertibleToInt | None = 0,
+        rot: ConvertibleToInt | None = 0,
         flipH: _ConvertibleToBool | None = None,
         flipV: _ConvertibleToBool | None = None,
         off: Point2D | None = None,
         ext: PositiveSize2D | None = None,
         chOff: Point2D | None = None,
         chExt: PositiveSize2D | None = None,
     ) -> None: ...
 
 class SphereCoords(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     lat: Integer[Literal[False]]
     lon: Integer[Literal[False]]
     rev: Integer[Literal[False]]
-    def __init__(self, lat: _ConvertibleToInt, lon: _ConvertibleToInt, rev: _ConvertibleToInt) -> None: ...
+    def __init__(self, lat: ConvertibleToInt, lon: ConvertibleToInt, rev: ConvertibleToInt) -> None: ...
 
 class Camera(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     prst: Set[_CameraPrst]
     fov: Integer[Literal[True]]
     zoom: Typed[Percentage, Literal[True]]
     rot: Typed[SphereCoords, Literal[True]]
     def __init__(
         self,
         prst: _CameraPrst,
-        fov: _ConvertibleToInt | None = None,
+        fov: ConvertibleToInt | None = None,
         zoom: Percentage | None = None,
         rot: SphereCoords | None = None,
     ) -> None: ...
 
 class LightRig(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     rig: Set[_LightRigRig]
     dir: Set[_LightRigDir]
     rot: Typed[SphereCoords, Literal[True]]
     def __init__(self, rig: _LightRigRig, dir: _LightRigDir, rot: SphereCoords | None = None) -> None: ...
 
 class Vector3D(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     dx: Integer[Literal[False]]
     dy: Integer[Literal[False]]
     dz: Integer[Literal[False]]
-    def __init__(self, dx: _ConvertibleToInt, dy: _ConvertibleToInt, dz: _ConvertibleToInt) -> None: ...
+    def __init__(self, dx: ConvertibleToInt, dy: ConvertibleToInt, dz: ConvertibleToInt) -> None: ...
 
 class Point3D(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     x: Integer[Literal[False]]
     y: Integer[Literal[False]]
     z: Integer[Literal[False]]
-    def __init__(self, x: _ConvertibleToInt, y: _ConvertibleToInt, z: _ConvertibleToInt) -> None: ...
+    def __init__(self, x: ConvertibleToInt, y: ConvertibleToInt, z: ConvertibleToInt) -> None: ...
 
 class Backdrop(Serialisable):
     anchor: Typed[Point3D, Literal[False]]
     norm: Typed[Vector3D, Literal[False]]
     up: Typed[Vector3D, Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
     def __init__(self, anchor: Point3D, norm: Vector3D, up: Vector3D, extLst: ExtensionList | None = None) -> None: ...
@@ -452,36 +439,36 @@
     backdrop: Typed[Backdrop, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     def __init__(
         self, camera: Camera, lightRig: LightRig, backdrop: Backdrop | None = None, extLst: ExtensionList | None = None
     ) -> None: ...
 
 class Bevel(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     w: Integer[Literal[False]]
     h: Integer[Literal[False]]
     prst: NoneSet[_BevelPrst]
-    def __init__(self, w: _ConvertibleToInt, h: _ConvertibleToInt, prst: _BevelPrst | Literal["none"] | None = None) -> None: ...
+    def __init__(self, w: ConvertibleToInt, h: ConvertibleToInt, prst: _BevelPrst | Literal["none"] | None = None) -> None: ...
 
 class Shape3D(Serialisable):
-    namespace: Incomplete
+    namespace: ClassVar[str]
     z: Typed[Coordinate[bool], Literal[True]]
     extrusionH: Integer[Literal[True]]
     contourW: Integer[Literal[True]]
     prstMaterial: NoneSet[_Shape3DPrstMaterial]
     bevelT: Typed[Bevel, Literal[True]]
     bevelB: Typed[Bevel, Literal[True]]
     extrusionClr: Typed[Color, Literal[True]]
     contourClr: Typed[Color, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     def __init__(
         self,
         z: Coordinate[bool] | None = None,
-        extrusionH: _ConvertibleToInt | None = None,
-        contourW: _ConvertibleToInt | None = None,
+        extrusionH: ConvertibleToInt | None = None,
+        contourW: ConvertibleToInt | None = None,
         prstMaterial: _Shape3DPrstMaterial | Literal["none"] | None = None,
         bevelT: Bevel | None = None,
         bevelB: Bevel | None = None,
         extrusionClr: Color | None = None,
         contourClr: Color | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
@@ -490,16 +477,16 @@
     w: Float[Literal[False]]
     h: Float[Literal[False]]
     fill: NoneSet[_Path2DFill]
     stroke: Bool[Literal[True]]
     extrusionOk: Bool[Literal[True]]
     def __init__(
         self,
-        w: _ConvertibleToFloat,
-        h: _ConvertibleToFloat,
+        w: ConvertibleToFloat,
+        h: ConvertibleToFloat,
         fill: _Path2DFill | Literal["none"] | None = None,
         stroke: _ConvertibleToBool | None = None,
         extrusionOk: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class Path2DList(Serialisable):
     path: Typed[Path2D, Literal[True]]
@@ -518,15 +505,15 @@
     x: Incomplete
     y: Incomplete
     def __init__(self, x: Incomplete | None = None, y: Incomplete | None = None) -> None: ...
 
 class ConnectionSite(Serialisable):
     ang: MinMax[float, Literal[False]]
     pos: Typed[AdjPoint2D, Literal[False]]
-    def __init__(self, ang: _ConvertibleToFloat, pos: AdjPoint2D) -> None: ...
+    def __init__(self, ang: ConvertibleToFloat, pos: AdjPoint2D) -> None: ...
 
 class ConnectionSiteList(Serialisable):
     cxn: Typed[ConnectionSite, Literal[True]]
     def __init__(self, cxn: ConnectionSite | None = None) -> None: ...
 
 class AdjustHandleList(Serialisable): ...
 
@@ -565,26 +552,26 @@
         ahLst: AdjustHandleList | None,
         cxnLst: ConnectionSiteList | None,
         rect: Unused,
         pathLst: Path2DList,
     ) -> None: ...
 
 class PresetGeometry2D(Serialisable):
-    namespace: Incomplete
+    namespace: ClassVar[str]
     prst: Set[_PresetGeometry2DPrst]
     avLst: Typed[GeomGuideList, Literal[True]]
     def __init__(self, prst: _PresetGeometry2DPrst, avLst: GeomGuideList | None = None) -> None: ...
 
 class FontReference(Serialisable):
     idx: NoneSet[_FontReferenceIdx]
     def __init__(self, idx: _FontReferenceIdx | Literal["none"] | None = None) -> None: ...
 
 class StyleMatrixReference(Serialisable):
     idx: Integer[Literal[False]]
-    def __init__(self, idx: _ConvertibleToInt) -> None: ...
+    def __init__(self, idx: ConvertibleToInt) -> None: ...
 
 class ShapeStyle(Serialisable):
     lnRef: Typed[StyleMatrixReference, Literal[False]]
     fillRef: Typed[StyleMatrixReference, Literal[False]]
     effectRef: Typed[StyleMatrixReference, Literal[False]]
     fontRef: Typed[FontReference, Literal[False]]
     def __init__(
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/graphic.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/graphic.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
 from openpyxl.descriptors.base import Alias, Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.picture import PictureFrame
 from openpyxl.drawing.properties import GroupShapeProperties, NonVisualGroupShape
 from openpyxl.drawing.relation import ChartRelation
@@ -26,41 +25,41 @@
         noChangeAspect: _ConvertibleToBool | None = None,
         noMove: _ConvertibleToBool | None = None,
         noResize: _ConvertibleToBool | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class NonVisualGraphicFrameProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     graphicFrameLocks: Typed[GraphicFrameLocking, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     def __init__(self, graphicFrameLocks: GraphicFrameLocking | None = None, extLst: ExtensionList | None = None) -> None: ...
 
 class NonVisualGraphicFrame(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     cNvPr: Typed[ExtensionList, Literal[False]]
     cNvGraphicFramePr: Typed[ExtensionList, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cNvPr: Incomplete | None = None, cNvGraphicFramePr: Incomplete | None = None) -> None: ...
 
 class GraphicData(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     uri: String[Literal[False]]
     chart: Typed[ChartRelation, Literal[True]]
     def __init__(self, uri: str = ..., chart: ChartRelation | None = None) -> None: ...
 
 class GraphicObject(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     graphicData: Typed[GraphicData, Literal[False]]
     def __init__(self, graphicData: GraphicData | None = None) -> None: ...
 
 class GraphicFrame(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     nvGraphicFramePr: Typed[NonVisualGraphicFrame, Literal[False]]
     xfrm: Typed[XDRTransform2D, Literal[False]]
     graphic: Typed[GraphicObject, Literal[False]]
     macro: String[Literal[True]]
     fPublished: Bool[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/line.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/line.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,95 +1,89 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
-
-from openpyxl.descriptors.base import (
-    Alias,
-    Integer,
-    MinMax,
-    NoneSet,
-    Typed,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
+
+from openpyxl.descriptors.base import Alias, Integer, MinMax, NoneSet, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import EmptyTag, NestedInteger, NestedNoneSet, _HasTagAndGet, _NestedNoneSetParam
+from openpyxl.descriptors.nested import EmptyTag, NestedInteger, NestedNoneSet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.drawing.colors import ColorChoice, ColorChoiceDescriptor
 from openpyxl.drawing.fill import GradientFillProperties, PatternFillProperties
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _LineEndPropertiesType: TypeAlias = Literal["none", "triangle", "stealth", "diamond", "oval", "arrow"]
 _LineEndPropertiesWLen: TypeAlias = Literal["sm", "med", "lg"]
 _LinePropertiesCap: TypeAlias = Literal["rnd", "sq", "flat"]
 _LinePropertiesCmpd: TypeAlias = Literal["sng", "dbl", "thickThin", "thinThick", "tri"]
 _LinePropertiesAlgn: TypeAlias = Literal["ctr", "in"]
 _LinePropertiesPrstDash: TypeAlias = Literal[
     "solid", "dot", "dash", "lgDash", "dashDot", "lgDashDot", "lgDashDotDot", "sysDash", "sysDot", "sysDashDot", "sysDashDotDot"
 ]
 
 class LineEndProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     type: NoneSet[_LineEndPropertiesType]
     w: NoneSet[_LineEndPropertiesWLen]
     len: NoneSet[_LineEndPropertiesWLen]
     def __init__(
         self,
         type: _LineEndPropertiesType | Literal["none"] | None = None,
         w: _LineEndPropertiesWLen | Literal["none"] | None = None,
         len: _LineEndPropertiesWLen | Literal["none"] | None = None,
     ) -> None: ...
 
 class DashStop(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     d: Integer[Literal[False]]
     length: Alias
     sp: Integer[Literal[False]]
     space: Alias
-    def __init__(self, d: _ConvertibleToInt = 0, sp: _ConvertibleToInt = 0) -> None: ...
+    def __init__(self, d: ConvertibleToInt = 0, sp: ConvertibleToInt = 0) -> None: ...
 
 class DashStopList(Serialisable):
     ds: Incomplete
     def __init__(self, ds: Incomplete | None = None) -> None: ...
 
 class LineProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     w: MinMax[float, Literal[True]]
     width: Alias
     cap: NoneSet[_LinePropertiesCap]
     cmpd: NoneSet[_LinePropertiesCmpd]
     algn: NoneSet[_LinePropertiesAlgn]
     noFill: EmptyTag[Literal[False]]
-    solidFill: Incomplete
+    solidFill: ColorChoiceDescriptor
     gradFill: Typed[GradientFillProperties, Literal[True]]
     pattFill: Typed[PatternFillProperties, Literal[True]]
     prstDash: NestedNoneSet[_LinePropertiesPrstDash]
     dashStyle: Alias
     custDash: Typed[DashStop, Literal[True]]
     round: EmptyTag[Literal[False]]
     bevel: EmptyTag[Literal[False]]
     miter: NestedInteger[Literal[True]]
     headEnd: Typed[LineEndProperties, Literal[True]]
     tailEnd: Typed[LineEndProperties, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        w: _ConvertibleToFloat | None = None,
+        w: ConvertibleToFloat | None = None,
         cap: _LinePropertiesCap | Literal["none"] | None = None,
         cmpd: _LinePropertiesCmpd | Literal["none"] | None = None,
         algn: _LinePropertiesAlgn | Literal["none"] | None = None,
         noFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
-        solidFill: Incomplete | None = None,
+        solidFill: str | ColorChoice | None = None,
         gradFill: GradientFillProperties | None = None,
         pattFill: PatternFillProperties | None = None,
         prstDash: _NestedNoneSetParam[_LinePropertiesPrstDash] = None,
         custDash: DashStop | None = None,
         round: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         bevel: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
-        miter: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        miter: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         headEnd: LineEndProperties | None = None,
         tailEnd: LineEndProperties | None = None,
         extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/picture.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/controls.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,64 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal, overload
 
-from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Bool, String, Typed, _ConvertibleToBool
-from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.drawing.fill import BlipFillProperties
-from openpyxl.drawing.geometry import ShapeStyle
-from openpyxl.drawing.properties import NonVisualDrawingProps
+from openpyxl.worksheet.ole import ObjectAnchor
 
-class PictureLocking(Serialisable):
-    tagname: str
-    namespace: Incomplete
-    noCrop: Bool[Literal[True]]
-    noGrp: Bool[Literal[True]]
-    noSelect: Bool[Literal[True]]
-    noRot: Bool[Literal[True]]
-    noChangeAspect: Bool[Literal[True]]
-    noMove: Bool[Literal[True]]
-    noResize: Bool[Literal[True]]
-    noEditPoints: Bool[Literal[True]]
-    noAdjustHandles: Bool[Literal[True]]
-    noChangeArrowheads: Bool[Literal[True]]
-    noChangeShapeType: Bool[Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
+class ControlProperty(Serialisable):
+    tagname: ClassVar[str]
+    anchor: Typed[ObjectAnchor, Literal[False]]
+    locked: Bool[Literal[True]]
+    defaultSize: Bool[Literal[True]]
+    _print: Bool[Literal[True]]  # Not private. Avoids name clash
+    disabled: Bool[Literal[True]]
+    recalcAlways: Bool[Literal[True]]
+    uiObject: Bool[Literal[True]]
+    autoFill: Bool[Literal[True]]
+    autoLine: Bool[Literal[True]]
+    autoPict: Bool[Literal[True]]
+    macro: String[Literal[True]]
+    altText: String[Literal[True]]
+    linkedCell: String[Literal[True]]
+    listFillRange: String[Literal[True]]
+    cf: String[Literal[True]]
+    id: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        noCrop: _ConvertibleToBool | None = None,
-        noGrp: _ConvertibleToBool | None = None,
-        noSelect: _ConvertibleToBool | None = None,
-        noRot: _ConvertibleToBool | None = None,
-        noChangeAspect: _ConvertibleToBool | None = None,
-        noMove: _ConvertibleToBool | None = None,
-        noResize: _ConvertibleToBool | None = None,
-        noEditPoints: _ConvertibleToBool | None = None,
-        noAdjustHandles: _ConvertibleToBool | None = None,
-        noChangeArrowheads: _ConvertibleToBool | None = None,
-        noChangeShapeType: _ConvertibleToBool | None = None,
-        extLst: Unused = None,
+        anchor: ObjectAnchor,
+        locked: _ConvertibleToBool | None = True,
+        defaultSize: _ConvertibleToBool | None = True,
+        _print: _ConvertibleToBool | None = True,
+        disabled: _ConvertibleToBool | None = False,
+        recalcAlways: _ConvertibleToBool | None = False,
+        uiObject: _ConvertibleToBool | None = False,
+        autoFill: _ConvertibleToBool | None = True,
+        autoLine: _ConvertibleToBool | None = True,
+        autoPict: _ConvertibleToBool | None = True,
+        macro: str | None = None,
+        altText: str | None = None,
+        linkedCell: str | None = None,
+        listFillRange: str | None = None,
+        cf: str | None = "pict",
+        id: Incomplete | None = None,
     ) -> None: ...
 
-class NonVisualPictureProperties(Serialisable):
-    tagname: str
-    preferRelativeResize: Bool[Literal[True]]
-    picLocks: Typed[PictureLocking, Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
+class Control(Serialisable):
+    tagname: ClassVar[str]
+    controlPr: Typed[ControlProperty, Literal[True]]
+    shapeId: Integer[Literal[False]]
+    name: String[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
+    @overload
     def __init__(
-        self, preferRelativeResize: _ConvertibleToBool | None = None, picLocks: Incomplete | None = None, extLst: Unused = None
+        self, controlPr: ControlProperty | None = None, *, shapeId: ConvertibleToInt, name: str | None = None
     ) -> None: ...
+    @overload
+    def __init__(self, controlPr: ControlProperty | None, shapeId: ConvertibleToInt, name: str | None = None) -> None: ...
 
-class PictureNonVisual(Serialisable):
-    tagname: str
-    cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
-    cNvPicPr: Typed[NonVisualPictureProperties, Literal[False]]
+class Controls(Serialisable):
+    tagname: ClassVar[str]
+    control: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(
-        self, cNvPr: NonVisualDrawingProps | None = None, cNvPicPr: NonVisualPictureProperties | None = None
-    ) -> None: ...
-
-class PictureFrame(Serialisable):
-    tagname: str
-    macro: String[Literal[True]]
-    fPublished: Bool[Literal[True]]
-    nvPicPr: Typed[PictureNonVisual, Literal[False]]
-    blipFill: Typed[BlipFillProperties, Literal[False]]
-    spPr: Typed[GraphicalProperties, Literal[False]]
-    graphicalProperties: Alias
-    style: Typed[ShapeStyle, Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(
-        self,
-        macro: str | None = None,
-        fPublished: _ConvertibleToBool | None = None,
-        nvPicPr: PictureNonVisual | None = None,
-        blipFill: BlipFillProperties | None = None,
-        spPr: GraphicalProperties | None = None,
-        style: ShapeStyle | None = None,
-    ) -> None: ...
+    def __init__(self, control=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/properties.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/properties.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
 from openpyxl.descriptors.base import Bool, NoneSet, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.geometry import GroupTransform2D, Scene3D
 from openpyxl.drawing.text import Hyperlink
 
 _GroupShapePropertiesBwMode: TypeAlias = Literal[
     "clr", "auto", "gray", "ltGray", "invGray", "grayWhite", "blackGray", "blackWhite", "black", "white", "hidden"
 ]
 
 class GroupShapeProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     bwMode: NoneSet[_GroupShapePropertiesBwMode]
     xfrm: Typed[GroupTransform2D, Literal[True]]
     scene3d: Typed[Scene3D, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     def __init__(
         self,
         bwMode: _GroupShapePropertiesBwMode | Literal["none"] | None = None,
         xfrm: GroupTransform2D | None = None,
         scene3d: Scene3D | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class GroupLocking(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     noGrp: Bool[Literal[True]]
     noUngrp: Bool[Literal[True]]
     noSelect: Bool[Literal[True]]
     noRot: Bool[Literal[True]]
     noChangeAspect: Bool[Literal[True]]
     noMove: Bool[Literal[True]]
     noResize: Bool[Literal[True]]
@@ -55,33 +55,33 @@
         noEditPoints: _ConvertibleToBool | None = None,
         noAdjustHandles: _ConvertibleToBool | None = None,
         noChangeShapeType: _ConvertibleToBool | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class NonVisualGroupDrawingShapeProps(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     grpSpLocks: Typed[GroupLocking, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, grpSpLocks: Incomplete | None = None, extLst: Unused = None) -> None: ...
 
 class NonVisualDrawingShapeProps(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     spLocks: Typed[GroupLocking, Literal[True]]
     txBax: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     txBox: Incomplete
     def __init__(
         self, spLocks: Incomplete | None = None, txBox: _ConvertibleToBool | None = None, extLst: Unused = None
     ) -> None: ...
 
 class NonVisualDrawingProps(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     id: Incomplete
     name: String[Literal[False]]
     descr: String[Literal[True]]
     hidden: Bool[Literal[True]]
     title: String[Literal[True]]
     hlinkClick: Typed[Hyperlink, Literal[True]]
     hlinkHover: Typed[Hyperlink, Literal[True]]
@@ -111,12 +111,12 @@
         title: str | None = None,
         hlinkClick: Hyperlink | None = None,
         hlinkHover: Hyperlink | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class NonVisualGroupShape(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
     cNvGrpSpPr: Typed[NonVisualGroupDrawingShapeProps, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cNvPr: NonVisualDrawingProps, cNvGrpSpPr: NonVisualGroupDrawingShapeProps) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/spreadsheet_drawing.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/spreadsheet_drawing.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
 from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.connector import Shape
 from openpyxl.drawing.graphic import GraphicFrame, GroupShape
 from openpyxl.drawing.picture import PictureFrame
 from openpyxl.drawing.xdr import XDRPoint2D, XDRPositiveSize2D
 
@@ -16,21 +16,21 @@
     fLocksWithSheet: Bool[Literal[True]]
     fPrintsWithSheet: Bool[Literal[True]]
     def __init__(
         self, fLocksWithSheet: _ConvertibleToBool | None = None, fPrintsWithSheet: _ConvertibleToBool | None = None
     ) -> None: ...
 
 class AnchorMarker(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     col: NestedText[int, Literal[False]]
     colOff: NestedText[int, Literal[False]]
     row: NestedText[int, Literal[False]]
     rowOff: NestedText[int, Literal[False]]
     def __init__(
-        self, col: _ConvertibleToInt = 0, colOff: _ConvertibleToInt = 0, row: _ConvertibleToInt = 0, rowOff: _ConvertibleToInt = 0
+        self, col: ConvertibleToInt = 0, colOff: ConvertibleToInt = 0, row: ConvertibleToInt = 0, rowOff: ConvertibleToInt = 0
     ) -> None: ...
 
 class _AnchorBase(Serialisable):
     sp: Typed[Shape, Literal[True]]
     shape: Alias
     grpSp: Typed[GroupShape, Literal[True]]
     groupShape: Alias
@@ -49,70 +49,73 @@
         graphicFrame: GraphicFrame | None = None,
         cxnSp: Shape | None = None,
         pic: PictureFrame | None = None,
         contentPart: Incomplete | None = None,
     ) -> None: ...
 
 class AbsoluteAnchor(_AnchorBase):
-    tagname: str
+    tagname: ClassVar[str]
     pos: Typed[XDRPoint2D, Literal[False]]
     ext: Typed[XDRPositiveSize2D, Literal[False]]
-    sp: Incomplete
-    grpSp: Incomplete
-    graphicFrame: Incomplete
-    cxnSp: Incomplete
-    pic: Incomplete
-    contentPart: Incomplete
-    clientData: Incomplete
+    # Same as parent
+    # sp = _AnchorBase.sp
+    # grpSp = _AnchorBase.grpSp
+    # graphicFrame = _AnchorBase.graphicFrame
+    # cxnSp = _AnchorBase.cxnSp
+    # pic = _AnchorBase.pic
+    # contentPart = _AnchorBase.contentPart
+    # clientData = _AnchorBase.clientData
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, pos: XDRPoint2D | None = None, ext: XDRPositiveSize2D | None = None, **kw) -> None: ...
 
 class OneCellAnchor(_AnchorBase):
-    tagname: str
+    tagname: ClassVar[str]
     _from: Typed[AnchorMarker, Literal[False]]  # Not private. Avoids name clash
     ext: Typed[XDRPositiveSize2D, Literal[False]]
-    sp: Incomplete
-    grpSp: Incomplete
-    graphicFrame: Incomplete
-    cxnSp: Incomplete
-    pic: Incomplete
-    contentPart: Incomplete
-    clientData: Incomplete
+    # Same as parent
+    # sp = _AnchorBase.sp
+    # grpSp = _AnchorBase.grpSp
+    # graphicFrame = _AnchorBase.graphicFrame
+    # cxnSp = _AnchorBase.cxnSp
+    # pic = _AnchorBase.pic
+    # contentPart = _AnchorBase.contentPart
+    # clientData = _AnchorBase.clientData
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, _from: AnchorMarker | None = None, ext: XDRPositiveSize2D | None = None, **kw) -> None: ...
 
 class TwoCellAnchor(_AnchorBase):
-    tagname: str
+    tagname: ClassVar[str]
     editAs: NoneSet[_TwoCellAnchorEditAs]
     _from: Typed[AnchorMarker, Literal[False]]  # Not private. Avoids name clash
     to: Typed[AnchorMarker, Literal[False]]
-    sp: Incomplete
-    grpSp: Incomplete
-    graphicFrame: Incomplete
-    cxnSp: Incomplete
-    pic: Incomplete
-    contentPart: Incomplete
-    clientData: Incomplete
+    # Same as parent
+    # sp = _AnchorBase.sp
+    # grpSp = _AnchorBase.grpSp
+    # graphicFrame = _AnchorBase.graphicFrame
+    # cxnSp = _AnchorBase.cxnSp
+    # pic = _AnchorBase.pic
+    # contentPart = _AnchorBase.contentPart
+    # clientData = _AnchorBase.clientData
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         editAs: _TwoCellAnchorEditAs | Literal["none"] | None = None,
         _from: AnchorMarker | None = None,
         to: AnchorMarker | None = None,
         **kw,
     ) -> None: ...
 
 class SpreadsheetDrawing(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     mime_type: str
     PartName: str
     twoCellAnchor: Incomplete
     oneCellAnchor: Incomplete
     absoluteAnchor: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     charts: Incomplete
     images: Incomplete
     def __init__(self, twoCellAnchor=(), oneCellAnchor=(), absoluteAnchor=()) -> None: ...
     def __hash__(self) -> int: ...
     def __bool__(self) -> bool: ...
     @property
-    def path(self): ...
+    def path(self) -> str: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/text.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/drawing/text.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
-
-from openpyxl.descriptors.base import (
-    Alias,
-    Bool,
-    Integer,
-    MinMax,
-    NoneSet,
-    Set,
-    String,
-    Typed,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
+
+from openpyxl.descriptors.base import Alias, Bool, Integer, MinMax, NoneSet, Set, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import Coordinate, ExtensionList
-from openpyxl.descriptors.nested import EmptyTag, NestedBool, NestedInteger, NestedText, NestedValue, _HasTagAndGet
+from openpyxl.descriptors.nested import EmptyTag, NestedBool, NestedInteger, NestedText, NestedValue
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.drawing.colors import ColorChoice, ColorChoiceDescriptor
 from openpyxl.drawing.effect import Color, EffectContainer, EffectList
 from openpyxl.drawing.fill import Blip, BlipFillProperties, GradientFillProperties, PatternFillProperties
 from openpyxl.drawing.geometry import Scene3D
 from openpyxl.drawing.line import LineProperties
 
+from ..xml._functions_overloads import _HasTagAndGet
+
 _CharacterPropertiesU: TypeAlias = Literal[
     "words",
     "sng",
     "dbl",
     "heavy",
     "dotted",
     "dottedHeavy",
@@ -142,16 +133,16 @@
 ]
 
 class EmbeddedWAVAudioFile(Serialisable):
     name: String[Literal[True]]
     def __init__(self, name: str | None = None) -> None: ...
 
 class Hyperlink(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     invalidUrl: String[Literal[True]]
     action: String[Literal[True]]
     tgtFrame: String[Literal[True]]
     tooltip: String[Literal[True]]
     history: Bool[Literal[True]]
     highlightClick: Bool[Literal[True]]
     endSnd: Bool[Literal[True]]
@@ -170,31 +161,31 @@
         endSnd: _ConvertibleToBool | None = None,
         snd: EmbeddedWAVAudioFile | None = None,
         extLst: ExtensionList | None = None,
         id: Incomplete | None = None,
     ) -> None: ...
 
 class Font(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     typeface: String[Literal[False]]
     panose: Incomplete
     pitchFamily: MinMax[float, Literal[True]]
     charset: Integer[Literal[True]]
     def __init__(
         self,
         typeface: str,
         panose: Incomplete | None = None,
-        pitchFamily: _ConvertibleToFloat | None = None,
-        charset: _ConvertibleToInt | None = None,
+        pitchFamily: ConvertibleToFloat | None = None,
+        charset: ConvertibleToInt | None = None,
     ) -> None: ...
 
 class CharacterProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     kumimoji: Bool[Literal[True]]
     lang: String[Literal[True]]
     altLang: String[Literal[True]]
     sz: MinMax[float, Literal[True]]
     b: Bool[Literal[True]]
     i: Bool[Literal[True]]
     u: NoneSet[_CharacterPropertiesU]
@@ -217,15 +208,15 @@
     cs: Typed[Font, Literal[True]]
     sym: Typed[Font, Literal[True]]
     hlinkClick: Typed[Hyperlink, Literal[True]]
     hlinkMouseOver: Typed[Hyperlink, Literal[True]]
     rtl: NestedBool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     noFill: EmptyTag[Literal[False]]
-    solidFill: Incomplete
+    solidFill: ColorChoiceDescriptor
     gradFill: Typed[GradientFillProperties, Literal[True]]
     blipFill: Typed[BlipFillProperties, Literal[True]]
     pattFill: Typed[PatternFillProperties, Literal[True]]
     grpFill: EmptyTag[Literal[False]]
     effectLst: Typed[EffectList, Literal[True]]
     effectDag: Typed[EffectContainer, Literal[True]]
     uLnTx: EmptyTag[Literal[False]]
@@ -234,42 +225,42 @@
     uFill: EmptyTag[Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         kumimoji: _ConvertibleToBool | None = None,
         lang: str | None = None,
         altLang: str | None = None,
-        sz: _ConvertibleToFloat | None = None,
+        sz: ConvertibleToFloat | None = None,
         b: _ConvertibleToBool | None = None,
         i: _ConvertibleToBool | None = None,
         u: _CharacterPropertiesU | Literal["none"] | None = None,
         strike: _CharacterPropertiesStrike | Literal["none"] | None = None,
-        kern: _ConvertibleToInt | None = None,
+        kern: ConvertibleToInt | None = None,
         cap: _CharacterPropertiesCap | Literal["none"] | None = None,
-        spc: _ConvertibleToInt | None = None,
+        spc: ConvertibleToInt | None = None,
         normalizeH: _ConvertibleToBool | None = None,
-        baseline: _ConvertibleToInt | None = None,
+        baseline: ConvertibleToInt | None = None,
         noProof: _ConvertibleToBool | None = None,
         dirty: _ConvertibleToBool | None = None,
         err: _ConvertibleToBool | None = None,
         smtClean: _ConvertibleToBool | None = None,
-        smtId: _ConvertibleToInt | None = None,
+        smtId: ConvertibleToInt | None = None,
         bmk: str | None = None,
         ln: LineProperties | None = None,
         highlight: Color | None = None,
         latin: Font | None = None,
         ea: Font | None = None,
         cs: Font | None = None,
         sym: Font | None = None,
         hlinkClick: Hyperlink | None = None,
         hlinkMouseOver: Hyperlink | None = None,
         rtl: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        extLst: ExtensionList | None = None,
+        extLst: Unused = None,
         noFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
-        solidFill: Incomplete | None = None,
+        solidFill: str | ColorChoice | None = None,
         gradFill: GradientFillProperties | None = None,
         blipFill: BlipFillProperties | None = None,
         pattFill: PatternFillProperties | None = None,
         grpFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         effectLst: EffectList | None = None,
         effectDag: EffectContainer | None = None,
         uLnTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
@@ -289,26 +280,26 @@
 
 class Spacing(Serialisable):
     spcPct: NestedInteger[Literal[True]]
     spcPts: NestedInteger[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        spcPct: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        spcPts: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        spcPct: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        spcPts: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
     ) -> None: ...
 
 class AutonumberBullet(Serialisable):
     type: Set[_AutonumberBulletType]
     startAt: Integer[Literal[False]]
-    def __init__(self, type: _AutonumberBulletType, startAt: _ConvertibleToInt) -> None: ...
+    def __init__(self, type: _AutonumberBulletType, startAt: ConvertibleToInt) -> None: ...
 
 class ParagraphProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     marL: Integer[Literal[True]]
     marR: Integer[Literal[True]]
     lvl: Integer[Literal[True]]
     indent: Integer[Literal[True]]
     algn: NoneSet[_ParagraphPropertiesAlgn]
     defTabSz: Integer[Literal[True]]
     rtl: Bool[Literal[True]]
@@ -332,47 +323,47 @@
     buNone: EmptyTag[Literal[False]]
     buAutoNum: EmptyTag[Literal[False]]
     buChar: NestedValue[str, Literal[True]]
     buBlip: NestedValue[Blip, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        marL: _ConvertibleToInt | None = None,
-        marR: _ConvertibleToInt | None = None,
-        lvl: _ConvertibleToInt | None = None,
-        indent: _ConvertibleToInt | None = None,
+        marL: ConvertibleToInt | None = None,
+        marR: ConvertibleToInt | None = None,
+        lvl: ConvertibleToInt | None = None,
+        indent: ConvertibleToInt | None = None,
         algn: _ParagraphPropertiesAlgn | Literal["none"] | None = None,
-        defTabSz: _ConvertibleToInt | None = None,
+        defTabSz: ConvertibleToInt | None = None,
         rtl: _ConvertibleToBool | None = None,
         eaLnBrk: _ConvertibleToBool | None = None,
         fontAlgn: _ParagraphPropertiesFontAlgn | Literal["none"] | None = None,
         latinLnBrk: _ConvertibleToBool | None = None,
         hangingPunct: _ConvertibleToBool | None = None,
         lnSpc: Spacing | None = None,
         spcBef: Spacing | None = None,
         spcAft: Spacing | None = None,
         tabLst: TabStopList | None = None,
         defRPr: CharacterProperties | None = None,
         extLst: ExtensionList | None = None,
         buClrTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         buClr: Color | None = None,
         buSzTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
-        buSzPct: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        buSzPts: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        buSzPct: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        buSzPts: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         buFontTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         buFont: Font | None = None,
         buNone: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         buAutoNum: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         buChar: object = None,
         buBlip: object = None,
     ) -> None: ...
 
 class ListStyle(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     defPPr: Typed[ParagraphProperties, Literal[True]]
     lvl1pPr: Typed[ParagraphProperties, Literal[True]]
     lvl2pPr: Typed[ParagraphProperties, Literal[True]]
     lvl3pPr: Typed[ParagraphProperties, Literal[True]]
     lvl4pPr: Typed[ParagraphProperties, Literal[True]]
     lvl5pPr: Typed[ParagraphProperties, Literal[True]]
     lvl6pPr: Typed[ParagraphProperties, Literal[True]]
@@ -393,26 +384,26 @@
         lvl7pPr: ParagraphProperties | None = None,
         lvl8pPr: ParagraphProperties | None = None,
         lvl9pPr: ParagraphProperties | None = None,
         extLst: ParagraphProperties | None = None,
     ) -> None: ...
 
 class RegularTextRun(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     rPr: Typed[CharacterProperties, Literal[True]]
     properties: Alias
     t: NestedText[str, Literal[False]]
     value: Alias
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, rPr: CharacterProperties | None = None, t: object = "") -> None: ...
 
 class LineBreak(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     rPr: Typed[CharacterProperties, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, rPr: CharacterProperties | None = None) -> None: ...
 
 class TextField(Serialisable):
     id: String[Literal[False]]
     type: String[Literal[True]]
@@ -426,16 +417,16 @@
         type: str | None = None,
         rPr: CharacterProperties | None = None,
         pPr: CharacterProperties | None = None,
         t: str | None = None,
     ) -> None: ...
 
 class Paragraph(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     pPr: Typed[ParagraphProperties, Literal[True]]
     properties: Alias
     endParaRPr: Typed[CharacterProperties, Literal[True]]
     r: Incomplete
     text: Alias
     br: Typed[LineBreak, Literal[True]]
     fld: Typed[TextField, Literal[True]]
@@ -462,19 +453,19 @@
     prst: Typed[Set[_PresetTextShapePrst], Literal[False]]
     avLst: Typed[GeomGuideList, Literal[True]]
     def __init__(self, prst: Set[_PresetTextShapePrst], avLst: GeomGuideList | None = None) -> None: ...
 
 class TextNormalAutofit(Serialisable):
     fontScale: Integer[Literal[False]]
     lnSpcReduction: Integer[Literal[False]]
-    def __init__(self, fontScale: _ConvertibleToInt, lnSpcReduction: _ConvertibleToInt) -> None: ...
+    def __init__(self, fontScale: ConvertibleToInt, lnSpcReduction: ConvertibleToInt) -> None: ...
 
 class RichTextProperties(Serialisable):
-    tagname: str
-    namespace: Incomplete
+    tagname: ClassVar[str]
+    namespace: ClassVar[str]
     rot: Integer[Literal[True]]
     spcFirstLastPara: Bool[Literal[True]]
     vertOverflow: NoneSet[_RichTextPropertiesVertOverflow]
     horzOverflow: NoneSet[_RichTextPropertiesHorzOverflow]
     vert: NoneSet[_RichTextPropertiesVert]
     wrap: NoneSet[_RichTextPropertiesWrap]
     lIns: Integer[Literal[True]]
@@ -496,34 +487,34 @@
     noAutofit: EmptyTag[Literal[False]]
     normAutofit: EmptyTag[Literal[False]]
     spAutoFit: EmptyTag[Literal[False]]
     flatTx: NestedInteger[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        rot: _ConvertibleToInt | None = None,
+        rot: ConvertibleToInt | None = None,
         spcFirstLastPara: _ConvertibleToBool | None = None,
         vertOverflow: _RichTextPropertiesVertOverflow | Literal["none"] | None = None,
         horzOverflow: _RichTextPropertiesHorzOverflow | Literal["none"] | None = None,
         vert: _RichTextPropertiesVert | Literal["none"] | None = None,
         wrap: _RichTextPropertiesWrap | Literal["none"] | None = None,
-        lIns: _ConvertibleToInt | None = None,
-        tIns: _ConvertibleToInt | None = None,
-        rIns: _ConvertibleToInt | None = None,
-        bIns: _ConvertibleToInt | None = None,
-        numCol: _ConvertibleToInt | None = None,
-        spcCol: _ConvertibleToInt | None = None,
+        lIns: ConvertibleToInt | None = None,
+        tIns: ConvertibleToInt | None = None,
+        rIns: ConvertibleToInt | None = None,
+        bIns: ConvertibleToInt | None = None,
+        numCol: ConvertibleToInt | None = None,
+        spcCol: ConvertibleToInt | None = None,
         rtlCol: _ConvertibleToBool | None = None,
         fromWordArt: _ConvertibleToBool | None = None,
         anchor: _RichTextPropertiesAnchor | Literal["none"] | None = None,
         anchorCtr: _ConvertibleToBool | None = None,
         forceAA: _ConvertibleToBool | None = None,
         upright: _ConvertibleToBool | None = None,
         compatLnSpc: _ConvertibleToBool | None = None,
         prstTxWarp: PresetTextShape | None = None,
         scene3d: Scene3D | None = None,
         extLst: Unused = None,
         noAutofit: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         normAutofit: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         spAutoFit: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
-        flatTx: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        flatTx: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/formatting.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/formatting/formatting.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from _typeshed import Incomplete, Unused
-from typing_extensions import Literal
+from collections.abc import Iterator
+from typing import ClassVar, Literal
 
 from openpyxl.descriptors.base import Alias, Bool, Convertible, _ConvertibleToBool, _ConvertibleToMultiCellRange
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.worksheet.cell_range import MultiCellRange
+from openpyxl.worksheet.cell_range import CellRange, MultiCellRange
 
 class ConditionalFormatting(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     sqref: Convertible[MultiCellRange, Literal[False]]
     cells: Alias
     pivot: Bool[Literal[True]]
     cfRule: Incomplete
     rules: Alias
     def __init__(
         self, sqref: _ConvertibleToMultiCellRange = (), pivot: _ConvertibleToBool | None = None, cfRule=(), extLst: Unused = None
     ) -> None: ...
-    def __eq__(self, other): ...
+    def __eq__(self, other: object) -> bool: ...
     def __hash__(self) -> int: ...
-    def __contains__(self, coord): ...
+    def __contains__(self, coord: str | CellRange) -> bool: ...
 
 class ConditionalFormattingList:
     max_priority: int
     def __init__(self) -> None: ...
     def add(self, range_string, cfRule) -> None: ...
     def __bool__(self) -> bool: ...
     def __len__(self) -> int: ...
-    def __iter__(self): ...
+    def __iter__(self) -> Iterator[ConditionalFormatting]: ...
     def __getitem__(self, key): ...
     def __delitem__(self, key) -> None: ...
     def __setitem__(self, key, rule) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/rule.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/formatting/rule.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
 from openpyxl.descriptors import Float, Strict
-from openpyxl.descriptors.base import Bool, Integer, NoneSet, Set, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, NoneSet, Set, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles.colors import Color, ColorDescriptor
 from openpyxl.styles.differential import DifferentialStyle
 
 _IconSetIconSet: TypeAlias = Literal[
     "3Arrows",
     "3ArrowsGray",
     "3Flags",
     "3TrafficLights1",
@@ -64,32 +65,32 @@
     "notContainsErrors",
     "timePeriod",
     "aboveAverage",
 ]
 
 class ValueDescriptor(Float[Incomplete]):
     expected_type: type[Incomplete]
-    def __set__(self, instance: Serialisable | Strict, value) -> None: ...  # type: ignore[override]
+    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
 
 class FormatObject(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     type: Set[_FormatObjectType]
     val: Incomplete
     gte: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, type: _FormatObjectType, val: Incomplete | None = None, gte: _ConvertibleToBool | None = None, extLst: Unused = None
     ) -> None: ...
 
 class RuleType(Serialisable):
     cfvo: Incomplete
 
 class IconSet(RuleType):
-    tagname: str
+    tagname: ClassVar[str]
     iconSet: NoneSet[_IconSetIconSet]
     showValue: Bool[Literal[True]]
     percent: Bool[Literal[True]]
     reverse: Bool[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     cfvo: Incomplete
     def __init__(
@@ -98,39 +99,50 @@
         showValue: _ConvertibleToBool | None = None,
         percent: _ConvertibleToBool | None = None,
         reverse: _ConvertibleToBool | None = None,
         cfvo: Incomplete | None = None,
     ) -> None: ...
 
 class DataBar(RuleType):
-    tagname: str
+    tagname: ClassVar[str]
     minLength: Integer[Literal[True]]
     maxLength: Integer[Literal[True]]
     showValue: Bool[Literal[True]]
-    color: Incomplete
+    color: ColorDescriptor[Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     cfvo: Incomplete
+    @overload
     def __init__(
         self,
-        minLength: _ConvertibleToInt | None = None,
-        maxLength: _ConvertibleToInt | None = None,
+        minLength: ConvertibleToInt | None = None,
+        maxLength: ConvertibleToInt | None = None,
         showValue: _ConvertibleToBool | None = None,
         cfvo: Incomplete | None = None,
-        color: Incomplete | None = None,
+        *,
+        color: str | Color,
+    ) -> None: ...
+    @overload
+    def __init__(
+        self,
+        minLength: ConvertibleToInt | None,
+        maxLength: ConvertibleToInt | None,
+        showValue: _ConvertibleToBool | None,
+        cfvo: Incomplete | None,
+        color: str | Color,
     ) -> None: ...
 
 class ColorScale(RuleType):
-    tagname: str
+    tagname: ClassVar[str]
     color: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     cfvo: Incomplete
     def __init__(self, cfvo: Incomplete | None = None, color: Incomplete | None = None) -> None: ...
 
 class Rule(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     type: Set[_RuleType]
     dxfId: Integer[Literal[True]]
     priority: Integer[Literal[False]]
     stopIfTrue: Bool[Literal[True]]
     aboveAverage: Bool[Literal[True]]
     percent: Bool[Literal[True]]
     bottom: Bool[Literal[True]]
@@ -147,25 +159,25 @@
     extLst: Typed[ExtensionList, Literal[True]]
     dxf: Typed[DifferentialStyle, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         type: _RuleType,
-        dxfId: _ConvertibleToInt | None = None,
-        priority: _ConvertibleToInt = 0,
+        dxfId: ConvertibleToInt | None = None,
+        priority: ConvertibleToInt = 0,
         stopIfTrue: _ConvertibleToBool | None = None,
         aboveAverage: _ConvertibleToBool | None = None,
         percent: _ConvertibleToBool | None = None,
         bottom: _ConvertibleToBool | None = None,
         operator: _RuleOperator | Literal["none"] | None = None,
         text: str | None = None,
         timePeriod: _RuleTimePeriod | Literal["none"] | None = None,
-        rank: _ConvertibleToInt | None = None,
-        stdDev: _ConvertibleToInt | None = None,
+        rank: ConvertibleToInt | None = None,
+        stdDev: ConvertibleToInt | None = None,
         equalAverage: _ConvertibleToBool | None = None,
         formula=(),
         colorScale: ColorScale | None = None,
         dataBar: DataBar | None = None,
         iconSet: IconSet | None = None,
         extLst: Unused = None,
         dxf: DifferentialStyle | None = None,
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/custom.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/custom.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-from _typeshed import Incomplete
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete
 from collections.abc import Iterator
 from datetime import datetime
-from typing import Any, Generic, TypeVar
-from typing_extensions import Literal, Self
+from typing import Any, Final, Generic, Literal, TypeVar
+from typing_extensions import Self, TypeAlias
 
 from openpyxl.descriptors import Sequence, Strict
-from openpyxl.descriptors.base import (
-    Bool,
-    DateTime,
-    Float,
-    Integer,
-    String,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from openpyxl.descriptors.base import Bool, DateTime, Float, Integer, String, _ConvertibleToBool
 from openpyxl.descriptors.nested import NestedText
+from openpyxl.descriptors.serialisable import _ChildSerialisableTreeElement
+from openpyxl.xml.functions import Element
 
 _T = TypeVar("_T")
 
 # Does not reimplement anything, so runtime also has incompatible supertypes
 class NestedBoolText(Bool[Incomplete], NestedText[Incomplete, Incomplete]): ...  # type: ignore[misc]
 
 class _TypedProperty(Strict, Generic[_T]):
     name: String[Literal[False]]
     # Since this is internal, just list all possible values
-    value: Integer[Literal[False]] | Float[Literal[False]] | String[Literal[True]] | DateTime[Literal[False]] | Bool[
-        Literal[False]
-    ] | String[Literal[False]]
+    value: (
+        Integer[Literal[False]]
+        | Float[Literal[False]]
+        | String[Literal[True]]
+        | DateTime[Literal[False]]
+        | Bool[Literal[False]]
+        | String[Literal[False]]
+    )
     def __init__(self, name: str, value: _T) -> None: ...
     def __eq__(self, other: _TypedProperty[Any]) -> bool: ...  # type: ignore[override]
 
-class IntProperty(_TypedProperty[_ConvertibleToInt]):
+class IntProperty(_TypedProperty[ConvertibleToInt]):
     value: Integer[Literal[False]]
 
-class FloatProperty(_TypedProperty[_ConvertibleToFloat]):
+class FloatProperty(_TypedProperty[ConvertibleToFloat]):
     value: Float[Literal[False]]
 
 class StringProperty(_TypedProperty[str | None]):
     value: String[Literal[True]]
 
 class DateTimeProperty(_TypedProperty[datetime]):
     value: DateTime[Literal[False]]
 
 class BoolProperty(_TypedProperty[_ConvertibleToBool]):
     value: Bool[Literal[False]]
 
 class LinkProperty(_TypedProperty[str]):
     value: String[Literal[False]]
 
-CLASS_MAPPING: Incomplete
-XML_MAPPING: Incomplete
+_MappingPropertyType: TypeAlias = StringProperty | IntProperty | FloatProperty | DateTimeProperty | BoolProperty | LinkProperty
+CLASS_MAPPING: Final[dict[type[_MappingPropertyType], str]]
+XML_MAPPING: Final[dict[str, type[_MappingPropertyType]]]
 
-class CustomPropertyList(Strict):
+class CustomPropertyList(Strict, Generic[_T]):
     props: Sequence
     def __init__(self) -> None: ...
     @classmethod
-    def from_tree(cls, tree) -> Self: ...
+    def from_tree(cls, tree: _ChildSerialisableTreeElement) -> Self: ...
     def append(self, prop) -> None: ...
-    def to_tree(self): ...
+    def to_tree(self) -> Element: ...
     def __len__(self) -> int: ...
     @property
     def names(self) -> list[str]: ...
     def __getitem__(self, name): ...
     def __delitem__(self, name) -> None: ...
-    def __iter__(self) -> Iterator[Incomplete]: ...
+    def __iter__(self) -> Iterator[_TypedProperty[_T]]: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/extended.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/fonts.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,77 @@
-from _typeshed import Unused
-from typing import ClassVar
-from typing_extensions import Literal
-
-from openpyxl.descriptors.base import Typed, _ConvertibleToInt
-from openpyxl.descriptors.nested import NestedText
+from _typeshed import ConvertibleToFloat, ConvertibleToInt
+from typing import ClassVar, Final, Literal
+from typing_extensions import Self, TypeAlias
+
+from openpyxl.descriptors.base import Alias, _ConvertibleToBool
+from openpyxl.descriptors.nested import (
+    NestedBool,
+    NestedFloat,
+    NestedInteger,
+    NestedMinMax,
+    NestedNoneSet,
+    NestedString,
+    _NestedNoneSetParam,
+)
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles.colors import Color, ColorDescriptor
 
-def get_version(): ...
-
-class DigSigBlob(Serialisable):
-    __elements__: ClassVar[tuple[str, ...]]
-    __attrs__: ClassVar[tuple[str, ...]]
-
-class VectorLpstr(Serialisable):
-    __elements__: ClassVar[tuple[str, ...]]
-    __attrs__: ClassVar[tuple[str, ...]]
-
-class VectorVariant(Serialisable):
-    __elements__: ClassVar[tuple[str, ...]]
-    __attrs__: ClassVar[tuple[str, ...]]
+from ..xml._functions_overloads import _HasTagAndGet, _SupportsFindAndIterAndAttribAndText
 
-class ExtendedProperties(Serialisable):
-    tagname: str
-    Template: NestedText[str, Literal[True]]
-    Manager: NestedText[str, Literal[True]]
-    Company: NestedText[str, Literal[True]]
-    Pages: NestedText[int, Literal[True]]
-    Words: NestedText[int, Literal[True]]
-    Characters: NestedText[int, Literal[True]]
-    PresentationFormat: NestedText[str, Literal[True]]
-    Lines: NestedText[int, Literal[True]]
-    Paragraphs: NestedText[int, Literal[True]]
-    Slides: NestedText[int, Literal[True]]
-    Notes: NestedText[int, Literal[True]]
-    TotalTime: NestedText[int, Literal[True]]
-    HiddenSlides: NestedText[int, Literal[True]]
-    MMClips: NestedText[int, Literal[True]]
-    ScaleCrop: NestedText[str, Literal[True]]
-    HeadingPairs: Typed[VectorVariant, Literal[True]]
-    TitlesOfParts: Typed[VectorLpstr, Literal[True]]
-    LinksUpToDate: NestedText[str, Literal[True]]
-    CharactersWithSpaces: NestedText[int, Literal[True]]
-    SharedDoc: NestedText[str, Literal[True]]
-    HyperlinkBase: NestedText[str, Literal[True]]
-    HLinks: Typed[VectorVariant, Literal[True]]
-    HyperlinksChanged: NestedText[str, Literal[True]]
-    DigSig: Typed[DigSigBlob, Literal[True]]
-    Application: NestedText[str, Literal[True]]
-    AppVersion: NestedText[str, Literal[True]]
-    DocSecurity: NestedText[int, Literal[True]]
+_FontU: TypeAlias = Literal["single", "double", "singleAccounting", "doubleAccounting"]
+_FontVertAlign: TypeAlias = Literal["superscript", "subscript", "baseline"]
+_FontScheme: TypeAlias = Literal["major", "minor"]
+
+class Font(Serialisable):
+    UNDERLINE_DOUBLE: Final = "double"
+    UNDERLINE_DOUBLE_ACCOUNTING: Final = "doubleAccounting"
+    UNDERLINE_SINGLE: Final = "single"
+    UNDERLINE_SINGLE_ACCOUNTING: Final = "singleAccounting"
+    name: NestedString[Literal[True]]
+    charset: NestedInteger[Literal[True]]
+    family: NestedMinMax[float, Literal[True]]
+    sz: NestedFloat[Literal[True]]
+    size: Alias
+    b: NestedBool[Literal[False]]
+    bold: Alias
+    i: NestedBool[Literal[False]]
+    italic: Alias
+    strike: NestedBool[Literal[True]]
+    strikethrough: Alias
+    outline: NestedBool[Literal[True]]
+    shadow: NestedBool[Literal[True]]
+    condense: NestedBool[Literal[True]]
+    extend: NestedBool[Literal[True]]
+    u: NestedNoneSet[_FontU]
+    underline: Alias
+    vertAlign: NestedNoneSet[_FontVertAlign]
+    color: ColorDescriptor[Literal[True]]
+    scheme: NestedNoneSet[_FontScheme]
+    tagname: ClassVar[str]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        Template: object = None,
-        Manager: object = None,
-        Company: object = None,
-        Pages: _ConvertibleToInt | None = None,
-        Words: _ConvertibleToInt | None = None,
-        Characters: _ConvertibleToInt | None = None,
-        PresentationFormat: object = None,
-        Lines: _ConvertibleToInt | None = None,
-        Paragraphs: _ConvertibleToInt | None = None,
-        Slides: _ConvertibleToInt | None = None,
-        Notes: _ConvertibleToInt | None = None,
-        TotalTime: _ConvertibleToInt | None = None,
-        HiddenSlides: _ConvertibleToInt | None = None,
-        MMClips: _ConvertibleToInt | None = None,
-        ScaleCrop: object = None,
-        HeadingPairs: Unused = None,
-        TitlesOfParts: Unused = None,
-        LinksUpToDate: object = None,
-        CharactersWithSpaces: _ConvertibleToInt | None = None,
-        SharedDoc: object = None,
-        HyperlinkBase: object = None,
-        HLinks: Unused = None,
-        HyperlinksChanged: object = None,
-        DigSig: Unused = None,
-        Application: object = "Microsoft Excel",
-        AppVersion: object = None,
-        DocSecurity: _ConvertibleToInt | None = None,
+        name: object = None,
+        sz: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        b: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        i: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        charset: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
+        u: _NestedNoneSetParam[_FontU] = None,
+        strike: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        color: str | Color | None = None,
+        scheme: _NestedNoneSetParam[_FontScheme] = None,
+        family: _HasTagAndGet[ConvertibleToFloat | None] | ConvertibleToFloat | None = None,
+        size: _HasTagAndGet[ConvertibleToFloat] | ConvertibleToFloat | None = None,
+        bold: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
+        italic: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
+        strikethrough: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
+        underline: _NestedNoneSetParam[_FontU] = None,
+        vertAlign: _NestedNoneSetParam[_FontVertAlign] = None,
+        outline: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        shadow: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        condense: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        extend: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
     ) -> None: ...
-    def to_tree(self): ...
+    @classmethod
+    def from_tree(cls, node: _SupportsFindAndIterAndAttribAndText) -> Self: ...
+
+DEFAULT_FONT: Final[Font]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/manifest.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/manifest.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from _typeshed import Incomplete
 from collections.abc import Generator
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Final, Literal
 
 from openpyxl.descriptors.base import String
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.xml.functions import Element
 
 mimetypes: Incomplete
 
 class FileExtension(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     Extension: String[Literal[False]]
     ContentType: String[Literal[False]]
     def __init__(self, Extension: str, ContentType: str) -> None: ...
 
 class Override(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     PartName: String[Literal[False]]
     ContentType: String[Literal[False]]
     def __init__(self, PartName: str, ContentType: str) -> None: ...
 
-DEFAULT_TYPES: Incomplete
-DEFAULT_OVERRIDE: Incomplete
+DEFAULT_TYPES: Final[list[FileExtension]]
+DEFAULT_OVERRIDE: Final[list[Override]]
 
 class Manifest(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     Default: Incomplete
     Override: Incomplete
     path: str
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, Default=(), Override=()) -> None: ...
     @property
-    def filenames(self): ...
+    def filenames(self) -> list[str]: ...
     @property
-    def extensions(self): ...
-    def to_tree(self): ...
-    def __contains__(self, content_type): ...
+    def extensions(self) -> list[tuple[str, str]]: ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
+    def __contains__(self, content_type: str) -> bool: ...
     def find(self, content_type): ...
     def findall(self, content_type) -> Generator[Incomplete, None, None]: ...
     def append(self, obj) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/relationship.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/relationship.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from _typeshed import Incomplete, Unused
 from collections.abc import Generator
-from typing import overload
-from typing_extensions import Literal
+from typing import ClassVar, Literal, TypeVar, overload
+from zipfile import ZipFile
 
 from openpyxl.descriptors.base import Alias, String
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.pivot.cache import CacheDefinition
+from openpyxl.pivot.record import RecordList
+from openpyxl.pivot.table import TableDefinition
+from openpyxl.xml.functions import Element
+
+_SerialisableT = TypeVar("_SerialisableT", bound=Serialisable)
+_SerialisableRelTypeT = TypeVar("_SerialisableRelTypeT", bound=CacheDefinition | RecordList | TableDefinition)
 
 class Relationship(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     Type: String[Literal[False]]
     Target: String[Literal[False]]
     target: Alias
     TargetMode: String[Literal[True]]
     Id: String[Literal[True]]
     id: Alias
     @overload
@@ -22,20 +29,33 @@
     def __init__(self, Id: str, Type: Unused, type: str, Target: str | None = None, TargetMode: str | None = None) -> None: ...
     @overload
     def __init__(
         self, Id: str, Type: str, type: None = None, Target: str | None = None, TargetMode: str | None = None
     ) -> None: ...
 
 class RelationshipList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     Relationship: Incomplete
     def __init__(self, Relationship=()) -> None: ...
     def append(self, value) -> None: ...
     def __len__(self) -> int: ...
     def __bool__(self) -> bool: ...
     def find(self, content_type) -> Generator[Incomplete, None, None]: ...
     def __getitem__(self, key): ...
-    def to_tree(self): ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
 
 def get_rels_path(path): ...
-def get_dependents(archive, filename): ...
-def get_rel(archive, deps, id: Incomplete | None = None, cls: Incomplete | None = None): ...
+def get_dependents(archive: ZipFile, filename: str) -> RelationshipList: ...
+
+# If `id` is None, `cls` needs to have ClassVar `rel_type`.
+# The `deps` attribute used at runtime is for internal use immediately after the return.
+# `cls` cannot be None
+@overload
+def get_rel(
+    archive: ZipFile, deps: RelationshipList, id: None = None, *, cls: type[_SerialisableRelTypeT]
+) -> _SerialisableRelTypeT | None: ...
+@overload
+def get_rel(
+    archive: ZipFile, deps: RelationshipList, id: None, cls: type[_SerialisableRelTypeT]
+) -> _SerialisableRelTypeT | None: ...
+@overload
+def get_rel(archive: ZipFile, deps: RelationshipList, id: str, cls: type[_SerialisableT]) -> _SerialisableT: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/workbook.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/packaging/workbook.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,70 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Alias, Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl import _VisibilityType
+from openpyxl.descriptors.base import Alias, Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.nested import NestedString
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.workbook.defined_name import DefinedNameList
 from openpyxl.workbook.function_group import FunctionGroupList
 from openpyxl.workbook.properties import CalcProperties, FileVersion, WorkbookProperties
 from openpyxl.workbook.protection import FileSharing, WorkbookProtection
 from openpyxl.workbook.smart_tags import SmartTagList, SmartTagProperties
 from openpyxl.workbook.web import WebPublishing, WebPublishObjectList
+from openpyxl.xml.functions import Element
 
-_ChildSheetState: TypeAlias = Literal["visible", "hidden", "veryHidden"]
 _WorkbookPackageConformance: TypeAlias = Literal["strict", "transitional"]
 
 class FileRecoveryProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     autoRecover: Bool[Literal[True]]
     crashSave: Bool[Literal[True]]
     dataExtractLoad: Bool[Literal[True]]
     repairLoad: Bool[Literal[True]]
     def __init__(
         self,
         autoRecover: _ConvertibleToBool | None = None,
         crashSave: _ConvertibleToBool | None = None,
         dataExtractLoad: _ConvertibleToBool | None = None,
         repairLoad: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class ChildSheet(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     sheetId: Integer[Literal[False]]
-    state: NoneSet[_ChildSheetState]
+    state: NoneSet[_VisibilityType]
     id: Incomplete
     def __init__(
         self,
         name: str,
-        sheetId: _ConvertibleToInt,
-        state: _ChildSheetState | Literal["none"] | None = "visible",
+        sheetId: ConvertibleToInt,
+        state: _VisibilityType | Literal["none"] | None = "visible",
         id: Incomplete | None = None,
     ) -> None: ...
 
 class PivotCache(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     cacheId: Integer[Literal[False]]
     id: Incomplete
-    def __init__(self, cacheId: _ConvertibleToInt, id: Incomplete | None = None) -> None: ...
+    def __init__(self, cacheId: ConvertibleToInt, id: Incomplete | None = None) -> None: ...
 
 class WorkbookPackage(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     conformance: NoneSet[_WorkbookPackageConformance]
     fileVersion: Typed[FileVersion, Literal[True]]
     fileSharing: Typed[FileSharing, Literal[True]]
     workbookPr: Typed[WorkbookProperties, Literal[True]]
     properties: Alias
     workbookProtection: Typed[WorkbookProtection, Literal[True]]
     bookViews: Incomplete
-    sheets: Incomplete
+    sheets: Incomplete  # NestedSequence[ChildSheet]
     functionGroups: Typed[FunctionGroupList, Literal[True]]
     externalReferences: Incomplete
     definedNames: Typed[DefinedNameList, Literal[True]]
     calcPr: Typed[CalcProperties, Literal[True]]
     oleSize: NestedString[Literal[True]]
     customWorkbookViews: Incomplete
     pivotCaches: Incomplete
@@ -95,10 +96,10 @@
         smartTagTypes: SmartTagList | None = None,
         webPublishing: WebPublishing | None = None,
         fileRecoveryPr: FileRecoveryProperties | None = None,
         webPublishObjects: WebPublishObjectList | None = None,
         extLst: Unused = None,
         Ignorable: Unused = None,
     ) -> None: ...
-    def to_tree(self): ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
     @property
-    def active(self): ...
+    def active(self) -> int: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/cache.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/cache.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,50 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, Unused
 from datetime import datetime
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import (
-    Bool,
-    DateTime,
-    Float,
-    Integer,
-    Set,
-    String,
-    Typed,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from openpyxl.descriptors.base import Bool, DateTime, Float, Integer, Set, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.nested import NestedInteger, _HasTagAndGet
+from openpyxl.descriptors.nested import NestedInteger
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.pivot.fields import Error, Missing, Number, Text, TupleList
 from openpyxl.pivot.table import PivotArea
+from openpyxl.xml.functions import Element
+
+from ..xml._functions_overloads import _HasTagAndGet
 
 _RangePrGroupBy: TypeAlias = Literal["range", "seconds", "minutes", "hours", "days", "months", "quarters", "years"]
 _CacheSourceType: TypeAlias = Literal["worksheet", "external", "consolidation", "scenario"]
 
 class MeasureDimensionMap(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     measureGroup: Integer[Literal[True]]
     dimension: Integer[Literal[True]]
-    def __init__(self, measureGroup: _ConvertibleToInt | None = None, dimension: _ConvertibleToInt | None = None) -> None: ...
+    def __init__(self, measureGroup: ConvertibleToInt | None = None, dimension: ConvertibleToInt | None = None) -> None: ...
 
 class MeasureGroup(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     caption: String[Literal[False]]
     def __init__(self, name: str, caption: str) -> None: ...
 
 class PivotDimension(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     measure: Bool[Literal[False]]
     name: String[Literal[False]]
     uniqueName: String[Literal[False]]
     caption: String[Literal[False]]
     @overload
     def __init__(self, measure: _ConvertibleToBool = None, *, name: str, uniqueName: str, caption: str) -> None: ...
     @overload
     def __init__(self, measure: _ConvertibleToBool, name: str, uniqueName: str, caption: str) -> None: ...
 
 class CalculatedMember(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     mdx: String[Literal[False]]
     memberName: String[Literal[False]]
     hierarchy: String[Literal[False]]
     parent: String[Literal[False]]
     solveOrder: Integer[Literal[False]]
     set: Bool[Literal[False]]
@@ -61,103 +53,103 @@
     def __init__(
         self,
         name: str,
         mdx: str,
         memberName: str,
         hierarchy: str,
         parent: str,
-        solveOrder: _ConvertibleToInt,
+        solveOrder: ConvertibleToInt,
         set: _ConvertibleToBool = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class CalculatedItem(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     field: Integer[Literal[True]]
     formula: String[Literal[False]]
     pivotArea: Typed[PivotArea, Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
-        self, field: _ConvertibleToInt | None = None, *, formula: str, pivotArea: PivotArea, extLst: Incomplete | None = None
+        self, field: ConvertibleToInt | None = None, *, formula: str, pivotArea: PivotArea, extLst: Incomplete | None = None
     ) -> None: ...
     @overload
     def __init__(
-        self, field: _ConvertibleToInt | None, formula: str, pivotArea: PivotArea, extLst: Incomplete | None = None
+        self, field: ConvertibleToInt | None, formula: str, pivotArea: PivotArea, extLst: Incomplete | None = None
     ) -> None: ...
 
 class ServerFormat(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     culture: String[Literal[True]]
     format: String[Literal[True]]
     def __init__(self, culture: str | None = None, format: str | None = None) -> None: ...
 
 class ServerFormatList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     serverFormat: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, serverFormat: Incomplete | None = None) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class Query(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     mdx: String[Literal[False]]
     tpls: Typed[TupleList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, mdx: str, tpls: TupleList | None = None) -> None: ...
 
 class QueryCache(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     count: Integer[Literal[False]]
     query: Typed[Query, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, query: Query) -> None: ...
+    def __init__(self, count: ConvertibleToInt, query: Query) -> None: ...
 
 class OLAPSet(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     count: Integer[Literal[False]]
     maxRank: Integer[Literal[False]]
     setDefinition: String[Literal[False]]
     sortType: Incomplete
     queryFailed: Bool[Literal[False]]
     tpls: Typed[TupleList, Literal[True]]
     sortByTuple: Typed[TupleList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        count: _ConvertibleToInt,
-        maxRank: _ConvertibleToInt,
+        count: ConvertibleToInt,
+        maxRank: ConvertibleToInt,
         setDefinition: str,
         sortType: Incomplete | None = None,
         queryFailed: _ConvertibleToBool = None,
         tpls: TupleList | None = None,
         sortByTuple: TupleList | None = None,
     ) -> None: ...
 
 class OLAPSets(Serialisable):
     count: Integer[Literal[False]]
     set: Typed[OLAPSet, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, set: OLAPSet) -> None: ...
+    def __init__(self, count: ConvertibleToInt, set: OLAPSet) -> None: ...
 
 class PCDSDTCEntries(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     count: Integer[Literal[False]]
     m: Typed[Missing, Literal[False]]
     n: Typed[Number, Literal[False]]
     e: Typed[Error, Literal[False]]
     s: Typed[Text, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, m: Missing, n: Number, e: Error, s: Text) -> None: ...
+    def __init__(self, count: ConvertibleToInt, m: Missing, n: Number, e: Error, s: Text) -> None: ...
 
 class TupleCache(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     entries: Typed[PCDSDTCEntries, Literal[True]]
     sets: Typed[OLAPSets, Literal[True]]
     queryCache: Typed[QueryCache, Literal[True]]
     serverFormats: Typed[ServerFormatList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
@@ -166,15 +158,15 @@
         sets: OLAPSets | None = None,
         queryCache: QueryCache | None = None,
         serverFormats: ServerFormatList | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class PCDKPI(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     uniqueName: String[Literal[False]]
     caption: String[Literal[True]]
     displayFolder: String[Literal[False]]
     measureGroup: String[Literal[False]]
     parent: String[Literal[False]]
     value: String[Literal[False]]
     goal: String[Literal[False]]
@@ -211,47 +203,47 @@
         status: str,
         trend: str,
         weight: str,
         time: str,
     ) -> None: ...
 
 class GroupMember(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     uniqueName: String[Literal[False]]
     group: Bool[Literal[False]]
     def __init__(self, uniqueName: str, group: _ConvertibleToBool = None) -> None: ...
 
 class GroupMembers(Serialisable):
     count: Integer[Literal[False]]
     groupMember: Typed[GroupMember, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, groupMember: GroupMember) -> None: ...
+    def __init__(self, count: ConvertibleToInt, groupMember: GroupMember) -> None: ...
 
 class LevelGroup(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     uniqueName: String[Literal[False]]
     caption: String[Literal[False]]
     uniqueParent: String[Literal[False]]
     id: Integer[Literal[False]]
     groupMembers: Typed[GroupMembers, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
-        self, name: str, uniqueName: str, caption: str, uniqueParent: str, id: _ConvertibleToInt, groupMembers: GroupMembers
+        self, name: str, uniqueName: str, caption: str, uniqueParent: str, id: ConvertibleToInt, groupMembers: GroupMembers
     ) -> None: ...
 
 class Groups(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     count: Integer[Literal[False]]
     group: Typed[LevelGroup, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, group: LevelGroup) -> None: ...
+    def __init__(self, count: ConvertibleToInt, group: LevelGroup) -> None: ...
 
 class GroupLevel(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     uniqueName: String[Literal[False]]
     caption: String[Literal[False]]
     user: Bool[Literal[False]]
     customRollUp: Bool[Literal[False]]
     groups: Typed[Groups, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
@@ -265,29 +257,29 @@
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class GroupLevels(Serialisable):
     count: Integer[Literal[False]]
     groupLevel: Typed[GroupLevel, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, groupLevel: GroupLevel) -> None: ...
+    def __init__(self, count: ConvertibleToInt, groupLevel: GroupLevel) -> None: ...
 
 class FieldUsage(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     x: Integer[Literal[False]]
-    def __init__(self, x: _ConvertibleToInt) -> None: ...
+    def __init__(self, x: ConvertibleToInt) -> None: ...
 
 class FieldsUsage(Serialisable):
     count: Integer[Literal[False]]
     fieldUsage: Typed[FieldUsage, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, fieldUsage: FieldUsage | None = None) -> None: ...
+    def __init__(self, count: ConvertibleToInt, fieldUsage: FieldUsage | None = None) -> None: ...
 
 class CacheHierarchy(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     uniqueName: String[Literal[False]]
     caption: String[Literal[True]]
     measure: Bool[Literal[False]]
     set: Bool[Literal[False]]
     parentSet: Integer[Literal[True]]
     iconSet: Integer[Literal[False]]
     attribute: Bool[Literal[False]]
@@ -313,131 +305,131 @@
     @overload
     def __init__(
         self,
         uniqueName: str = "",
         caption: str | None = None,
         measure: _ConvertibleToBool = None,
         set: _ConvertibleToBool = None,
-        parentSet: _ConvertibleToInt | None = None,
-        iconSet: _ConvertibleToInt = 0,
+        parentSet: ConvertibleToInt | None = None,
+        iconSet: ConvertibleToInt = 0,
         attribute: _ConvertibleToBool = None,
         time: _ConvertibleToBool = None,
         keyAttribute: _ConvertibleToBool = None,
         defaultMemberUniqueName: str | None = None,
         allUniqueName: str | None = None,
         allCaption: str | None = None,
         dimensionUniqueName: str | None = None,
         displayFolder: str | None = None,
         measureGroup: str | None = None,
         measures: _ConvertibleToBool = None,
         *,
-        count: _ConvertibleToInt,
+        count: ConvertibleToInt,
         oneField: _ConvertibleToBool = None,
-        memberValueDatatype: _ConvertibleToInt | None = None,
+        memberValueDatatype: ConvertibleToInt | None = None,
         unbalanced: _ConvertibleToBool | None = None,
         unbalancedGroup: _ConvertibleToBool | None = None,
         hidden: _ConvertibleToBool = None,
         fieldsUsage: FieldsUsage | None = None,
         groupLevels: GroupLevels | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         uniqueName: str,
         caption: str | None,
         measure: _ConvertibleToBool,
         set: _ConvertibleToBool,
-        parentSet: _ConvertibleToInt | None,
-        iconSet: _ConvertibleToInt,
+        parentSet: ConvertibleToInt | None,
+        iconSet: ConvertibleToInt,
         attribute: _ConvertibleToBool,
         time: _ConvertibleToBool,
         keyAttribute: _ConvertibleToBool,
         defaultMemberUniqueName: str | None,
         allUniqueName: str | None,
         allCaption: str | None,
         dimensionUniqueName: str | None,
         displayFolder: str | None,
         measureGroup: str | None,
         measures: _ConvertibleToBool,
-        count: _ConvertibleToInt,
+        count: ConvertibleToInt,
         oneField: _ConvertibleToBool = None,
-        memberValueDatatype: _ConvertibleToInt | None = None,
+        memberValueDatatype: ConvertibleToInt | None = None,
         unbalanced: _ConvertibleToBool | None = None,
         unbalancedGroup: _ConvertibleToBool | None = None,
         hidden: _ConvertibleToBool = None,
         fieldsUsage: FieldsUsage | None = None,
         groupLevels: GroupLevels | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class GroupItems(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     m: Incomplete
     n: Incomplete
     b: Incomplete
     e: Incomplete
     s: Incomplete
     d: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, m=(), n=(), b=(), e=(), s=(), d=()) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class DiscretePr(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     count: Integer[Literal[False]]
     x: NestedInteger[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
-        self, count: _ConvertibleToInt, x: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None
+        self, count: ConvertibleToInt, x: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None
     ) -> None: ...
 
 class RangePr(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     autoStart: Bool[Literal[True]]
     autoEnd: Bool[Literal[True]]
     groupBy: Set[_RangePrGroupBy]
     startNum: Float[Literal[True]]
     endNum: Float[Literal[True]]
     startDate: DateTime[Literal[True]]
     endDate: DateTime[Literal[True]]
     groupInterval: Float[Literal[True]]
     def __init__(
         self,
         autoStart: _ConvertibleToBool | None = True,
         autoEnd: _ConvertibleToBool | None = True,
         groupBy: _RangePrGroupBy = "range",
-        startNum: _ConvertibleToFloat | None = None,
-        endNum: _ConvertibleToFloat | None = None,
+        startNum: ConvertibleToFloat | None = None,
+        endNum: ConvertibleToFloat | None = None,
         startDate: datetime | str | None = None,
         endDate: datetime | str | None = None,
-        groupInterval: _ConvertibleToFloat | None = 1,
+        groupInterval: ConvertibleToFloat | None = 1,
     ) -> None: ...
 
 class FieldGroup(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     par: Integer[Literal[True]]
     base: Integer[Literal[True]]
     rangePr: Typed[RangePr, Literal[True]]
     discretePr: Typed[DiscretePr, Literal[True]]
     groupItems: Typed[GroupItems, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        par: _ConvertibleToInt | None = None,
-        base: _ConvertibleToInt | None = None,
+        par: ConvertibleToInt | None = None,
+        base: ConvertibleToInt | None = None,
         rangePr: RangePr | None = None,
         discretePr: DiscretePr | None = None,
         groupItems: GroupItems | None = None,
     ) -> None: ...
 
 class SharedItems(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     m: Incomplete
     n: Incomplete
     b: Incomplete
     e: Incomplete
     s: Incomplete
     d: Incomplete
     containsSemiMixedTypes: Bool[Literal[True]]
@@ -461,26 +453,26 @@
         containsNonDate: _ConvertibleToBool | None = None,
         containsDate: _ConvertibleToBool | None = None,
         containsString: _ConvertibleToBool | None = None,
         containsBlank: _ConvertibleToBool | None = None,
         containsMixedTypes: _ConvertibleToBool | None = None,
         containsNumber: _ConvertibleToBool | None = None,
         containsInteger: _ConvertibleToBool | None = None,
-        minValue: _ConvertibleToFloat | None = None,
-        maxValue: _ConvertibleToFloat | None = None,
+        minValue: ConvertibleToFloat | None = None,
+        maxValue: ConvertibleToFloat | None = None,
         minDate: datetime | str | None = None,
         maxDate: datetime | str | None = None,
         count: Unused = None,
         longText: _ConvertibleToBool | None = None,
     ) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class CacheField(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     sharedItems: Typed[SharedItems, Literal[True]]
     fieldGroup: Typed[FieldGroup, Literal[True]]
     mpMap: NestedInteger[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     name: String[Literal[False]]
     caption: String[Literal[True]]
     propertyName: String[Literal[True]]
@@ -496,136 +488,136 @@
     memberPropertyField: Bool[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         sharedItems: SharedItems | None = None,
         fieldGroup: FieldGroup | None = None,
-        mpMap: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        mpMap: _HasTagAndGet[ConvertibleToInt | None] | ConvertibleToInt | None = None,
         extLst: ExtensionList | None = None,
         *,
         name: str,
         caption: str | None = None,
         propertyName: str | None = None,
         serverField: _ConvertibleToBool | None = None,
         uniqueList: _ConvertibleToBool | None = True,
-        numFmtId: _ConvertibleToInt | None = None,
+        numFmtId: ConvertibleToInt | None = None,
         formula: str | None = None,
-        sqlType: _ConvertibleToInt | None = 0,
-        hierarchy: _ConvertibleToInt | None = 0,
-        level: _ConvertibleToInt | None = 0,
+        sqlType: ConvertibleToInt | None = 0,
+        hierarchy: ConvertibleToInt | None = 0,
+        level: ConvertibleToInt | None = 0,
         databaseField: _ConvertibleToBool | None = True,
-        mappingCount: _ConvertibleToInt | None = None,
+        mappingCount: ConvertibleToInt | None = None,
         memberPropertyField: _ConvertibleToBool | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         sharedItems: SharedItems | None,
         fieldGroup: FieldGroup | None,
         mpMap: Incomplete | None,
         extLst: ExtensionList | None,
         name: str,
         caption: str | None = None,
         propertyName: str | None = None,
         serverField: _ConvertibleToBool | None = None,
         uniqueList: _ConvertibleToBool | None = True,
-        numFmtId: _ConvertibleToInt | None = None,
+        numFmtId: ConvertibleToInt | None = None,
         formula: str | None = None,
-        sqlType: _ConvertibleToInt | None = 0,
-        hierarchy: _ConvertibleToInt | None = 0,
-        level: _ConvertibleToInt | None = 0,
+        sqlType: ConvertibleToInt | None = 0,
+        hierarchy: ConvertibleToInt | None = 0,
+        level: ConvertibleToInt | None = 0,
         databaseField: _ConvertibleToBool | None = True,
-        mappingCount: _ConvertibleToInt | None = None,
+        mappingCount: ConvertibleToInt | None = None,
         memberPropertyField: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class RangeSet(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     i1: Integer[Literal[True]]
     i2: Integer[Literal[True]]
     i3: Integer[Literal[True]]
     i4: Integer[Literal[True]]
     ref: String[Literal[False]]
     name: String[Literal[True]]
     sheet: String[Literal[True]]
     @overload
     def __init__(
         self,
-        i1: _ConvertibleToInt | None = None,
-        i2: _ConvertibleToInt | None = None,
-        i3: _ConvertibleToInt | None = None,
-        i4: _ConvertibleToInt | None = None,
+        i1: ConvertibleToInt | None = None,
+        i2: ConvertibleToInt | None = None,
+        i3: ConvertibleToInt | None = None,
+        i4: ConvertibleToInt | None = None,
         *,
         ref: str,
         name: str | None = None,
         sheet: str | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        i1: _ConvertibleToInt | None,
-        i2: _ConvertibleToInt | None,
-        i3: _ConvertibleToInt | None,
-        i4: _ConvertibleToInt | None,
+        i1: ConvertibleToInt | None,
+        i2: ConvertibleToInt | None,
+        i3: ConvertibleToInt | None,
+        i4: ConvertibleToInt | None,
         ref: str,
         name: str | None = None,
         sheet: str | None = None,
     ) -> None: ...
 
 class PageItem(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     def __init__(self, name: str) -> None: ...
 
 class Page(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     pageItem: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, pageItem: Incomplete | None = None) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class Consolidation(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     autoPage: Bool[Literal[True]]
     pages: Incomplete
     rangeSets: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, autoPage: _ConvertibleToBool | None = None, pages=(), rangeSets=()) -> None: ...
 
 class WorksheetSource(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ref: String[Literal[True]]
     name: String[Literal[True]]
     sheet: String[Literal[True]]
     def __init__(self, ref: str | None = None, name: str | None = None, sheet: str | None = None) -> None: ...
 
 class CacheSource(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     type: Set[_CacheSourceType]
     connectionId: Integer[Literal[True]]
     worksheetSource: Typed[WorksheetSource, Literal[True]]
     consolidation: Typed[Consolidation, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         type: _CacheSourceType,
-        connectionId: _ConvertibleToInt | None = None,
+        connectionId: ConvertibleToInt | None = None,
         worksheetSource: WorksheetSource | None = None,
         consolidation: Consolidation | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class CacheDefinition(Serialisable):
     mime_type: str
     rel_type: str
     records: Incomplete
-    tagname: str
+    tagname: ClassVar[str]
     invalid: Bool[Literal[True]]
     saveData: Bool[Literal[True]]
     refreshOnLoad: Bool[Literal[True]]
     optimizeMemory: Bool[Literal[True]]
     enableRefresh: Bool[Literal[True]]
     refreshedBy: String[Literal[True]]
     refreshedDate: Float[Literal[True]]
@@ -657,22 +649,22 @@
         self,
         invalid: _ConvertibleToBool | None = None,
         saveData: _ConvertibleToBool | None = None,
         refreshOnLoad: _ConvertibleToBool | None = None,
         optimizeMemory: _ConvertibleToBool | None = None,
         enableRefresh: _ConvertibleToBool | None = None,
         refreshedBy: str | None = None,
-        refreshedDate: _ConvertibleToFloat | None = None,
+        refreshedDate: ConvertibleToFloat | None = None,
         refreshedDateIso: datetime | str | None = None,
         backgroundQuery: _ConvertibleToBool | None = None,
-        missingItemsLimit: _ConvertibleToInt | None = None,
-        createdVersion: _ConvertibleToInt | None = None,
-        refreshedVersion: _ConvertibleToInt | None = None,
-        minRefreshableVersion: _ConvertibleToInt | None = None,
-        recordCount: _ConvertibleToInt | None = None,
+        missingItemsLimit: ConvertibleToInt | None = None,
+        createdVersion: ConvertibleToInt | None = None,
+        refreshedVersion: ConvertibleToInt | None = None,
+        minRefreshableVersion: ConvertibleToInt | None = None,
+        recordCount: ConvertibleToInt | None = None,
         upgradeOnRefresh: _ConvertibleToBool | None = None,
         tupleCache: TupleCache | None = None,
         supportSubquery: _ConvertibleToBool | None = None,
         supportAdvancedDrill: _ConvertibleToBool | None = None,
         *,
         cacheSource: CacheSource,
         cacheFields=(),
@@ -691,22 +683,22 @@
         self,
         invalid: _ConvertibleToBool | None,
         saveData: _ConvertibleToBool | None,
         refreshOnLoad: _ConvertibleToBool | None,
         optimizeMemory: _ConvertibleToBool | None,
         enableRefresh: _ConvertibleToBool | None,
         refreshedBy: str | None,
-        refreshedDate: _ConvertibleToFloat | None,
+        refreshedDate: ConvertibleToFloat | None,
         refreshedDateIso: datetime | str | None,
         backgroundQuery: _ConvertibleToBool | None,
-        missingItemsLimit: _ConvertibleToInt | None,
-        createdVersion: _ConvertibleToInt | None,
-        refreshedVersion: _ConvertibleToInt | None,
-        minRefreshableVersion: _ConvertibleToInt | None,
-        recordCount: _ConvertibleToInt | None,
+        missingItemsLimit: ConvertibleToInt | None,
+        createdVersion: ConvertibleToInt | None,
+        refreshedVersion: ConvertibleToInt | None,
+        minRefreshableVersion: ConvertibleToInt | None,
+        recordCount: ConvertibleToInt | None,
         upgradeOnRefresh: _ConvertibleToBool | None,
         tupleCache: TupleCache | None,
         supportSubquery: _ConvertibleToBool | None,
         supportAdvancedDrill: _ConvertibleToBool | None,
         cacheSource: CacheSource,
         cacheFields=(),
         cacheHierarchies=(),
@@ -715,10 +707,10 @@
         calculatedMembers=(),
         dimensions=(),
         measureGroups=(),
         maps=(),
         extLst: ExtensionList | None = None,
         id: Incomplete | None = None,
     ) -> None: ...
-    def to_tree(self): ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
     @property
-    def path(self): ...
+    def path(self) -> str: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/fields.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/fields.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,36 @@
-from _typeshed import Incomplete
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete
 from datetime import datetime
-from typing import ClassVar, overload
-from typing_extensions import Literal
+from typing import ClassVar, Literal, overload
 
-from openpyxl.descriptors.base import (
-    Bool,
-    DateTime,
-    Float,
-    Integer,
-    String,
-    Typed,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from openpyxl.descriptors.base import Bool, DateTime, Float, Integer, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Index(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     v: Integer[Literal[True]]
-    def __init__(self, v: _ConvertibleToInt | None = 0) -> None: ...
+    def __init__(self, v: ConvertibleToInt | None = 0) -> None: ...
 
 class Tuple(Serialisable):
     fld: Integer[Literal[False]]
     hier: Integer[Literal[False]]
     item: Integer[Literal[False]]
-    def __init__(self, fld: _ConvertibleToInt, hier: _ConvertibleToInt, item: _ConvertibleToInt) -> None: ...
+    def __init__(self, fld: ConvertibleToInt, hier: ConvertibleToInt, item: ConvertibleToInt) -> None: ...
 
 class TupleList(Serialisable):
     c: Integer[Literal[True]]
     tpl: Typed[Tuple, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
-    def __init__(self, c: _ConvertibleToInt | None = None, *, tpl: Tuple) -> None: ...
+    def __init__(self, c: ConvertibleToInt | None = None, *, tpl: Tuple) -> None: ...
     @overload
-    def __init__(self, c: _ConvertibleToInt | None, tpl: Tuple) -> None: ...
+    def __init__(self, c: ConvertibleToInt | None, tpl: Tuple) -> None: ...
 
 class Missing(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     tpls: Incomplete
     x: Incomplete
     u: Bool[Literal[True]]
     f: Bool[Literal[True]]
     c: String[Literal[True]]
     cp: Integer[Literal[True]]
     _in: Integer[Literal[True]]  # Not private. Avoids name clash
@@ -55,26 +44,26 @@
     def __init__(
         self,
         tpls=(),
         x=(),
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
-        cp: _ConvertibleToInt | None = None,
-        _in: _ConvertibleToInt | None = None,
+        cp: ConvertibleToInt | None = None,
+        _in: ConvertibleToInt | None = None,
         bc: Incomplete | None = None,
         fc: Incomplete | None = None,
         i: _ConvertibleToBool | None = None,
         un: _ConvertibleToBool | None = None,
         st: _ConvertibleToBool | None = None,
         b: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class Number(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     tpls: Incomplete
     x: Incomplete
     v: Float[Literal[False]]
     u: Bool[Literal[True]]
     f: Bool[Literal[True]]
     c: String[Literal[True]]
     cp: Integer[Literal[True]]
@@ -88,48 +77,48 @@
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         tpls=(),
         x=(),
         *,
-        v: _ConvertibleToFloat,
+        v: ConvertibleToFloat,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
-        cp: _ConvertibleToInt | None = None,
-        _in: _ConvertibleToInt | None = None,
+        cp: ConvertibleToInt | None = None,
+        _in: ConvertibleToInt | None = None,
         bc: Incomplete | None = None,
         fc: Incomplete | None = None,
         i: _ConvertibleToBool | None = None,
         un: _ConvertibleToBool | None = None,
         st: _ConvertibleToBool | None = None,
         b: _ConvertibleToBool | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         tpls,
         x,
-        v: _ConvertibleToFloat,
+        v: ConvertibleToFloat,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
-        cp: _ConvertibleToInt | None = None,
-        _in: _ConvertibleToInt | None = None,
+        cp: ConvertibleToInt | None = None,
+        _in: ConvertibleToInt | None = None,
         bc: Incomplete | None = None,
         fc: Incomplete | None = None,
         i: _ConvertibleToBool | None = None,
         un: _ConvertibleToBool | None = None,
         st: _ConvertibleToBool | None = None,
         b: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class Error(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     tpls: Typed[TupleList, Literal[True]]
     x: Incomplete
     v: String[Literal[False]]
     u: Bool[Literal[True]]
     f: Bool[Literal[True]]
     c: String[Literal[True]]
     cp: Integer[Literal[True]]
@@ -147,16 +136,16 @@
         tpls: TupleList | None = None,
         x=(),
         *,
         v: str,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
-        cp: _ConvertibleToInt | None = None,
-        _in: _ConvertibleToInt | None = None,
+        cp: ConvertibleToInt | None = None,
+        _in: ConvertibleToInt | None = None,
         bc: Incomplete | None = None,
         fc: Incomplete | None = None,
         i: _ConvertibleToBool | None = None,
         un: _ConvertibleToBool | None = None,
         st: _ConvertibleToBool | None = None,
         b: _ConvertibleToBool | None = None,
     ) -> None: ...
@@ -165,45 +154,45 @@
         self,
         tpls: TupleList | None,
         x,
         v: str,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
-        cp: _ConvertibleToInt | None = None,
-        _in: _ConvertibleToInt | None = None,
+        cp: ConvertibleToInt | None = None,
+        _in: ConvertibleToInt | None = None,
         bc: Incomplete | None = None,
         fc: Incomplete | None = None,
         i: _ConvertibleToBool | None = None,
         un: _ConvertibleToBool | None = None,
         st: _ConvertibleToBool | None = None,
         b: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class Boolean(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     x: Incomplete
     v: Bool[Literal[False]]
     u: Bool[Literal[True]]
     f: Bool[Literal[True]]
     c: String[Literal[True]]
     cp: Integer[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         x=(),
         v: _ConvertibleToBool = None,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
-        cp: _ConvertibleToInt | None = None,
+        cp: ConvertibleToInt | None = None,
     ) -> None: ...
 
 class Text(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     tpls: Incomplete
     x: Incomplete
     v: String[Literal[False]]
     u: Bool[Literal[True]]
     f: Bool[Literal[True]]
     c: String[Literal[True]]
     cp: Integer[Literal[True]]
@@ -219,35 +208,35 @@
         self,
         tpls=(),
         x=(),
         v: Incomplete | None = None,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: Incomplete | None = None,
-        cp: _ConvertibleToInt | None = None,
-        _in: _ConvertibleToInt | None = None,
+        cp: ConvertibleToInt | None = None,
+        _in: ConvertibleToInt | None = None,
         bc: Incomplete | None = None,
         fc: Incomplete | None = None,
         i: _ConvertibleToBool | None = None,
         un: _ConvertibleToBool | None = None,
         st: _ConvertibleToBool | None = None,
         b: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class DateTimeField(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     x: Incomplete
     v: DateTime[Literal[False]]
     u: Bool[Literal[True]]
     f: Bool[Literal[True]]
     c: String[Literal[True]]
     cp: Integer[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         x=(),
         v: datetime | str | None = None,
         u: _ConvertibleToBool | None = None,
         f: _ConvertibleToBool | None = None,
         c: str | None = None,
-        cp: _ConvertibleToInt | None = None,
+        cp: ConvertibleToInt | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/record.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/record.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
 from openpyxl.descriptors.base import Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.xml.functions import Element
 
 class Record(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     m: Incomplete
     n: Incomplete
     b: Incomplete
     e: Incomplete
     s: Incomplete
     d: Incomplete
     x: Incomplete
@@ -26,18 +26,18 @@
         d: Incomplete | None = None,
         x: Incomplete | None = None,
     ) -> None: ...
 
 class RecordList(Serialisable):
     mime_type: str
     rel_type: str
-    tagname: str
+    tagname: ClassVar[str]
     r: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, r=(), extLst: ExtensionList | None = None) -> None: ...
     @property
-    def count(self): ...
-    def to_tree(self): ...
+    def count(self) -> int: ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
     @property
-    def path(self): ...
+    def path(self) -> str: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/table.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/pivot/table.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Bool, Integer, NoneSet, Set, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, NoneSet, Set, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.filters import AutoFilter
+from openpyxl.xml.functions import Element
 
 _PivotAreaType: TypeAlias = Literal["normal", "data", "all", "origin", "button", "topEnd", "topRight"]
 _PivotAxis: TypeAlias = Literal["axisRow", "axisCol", "axisPage", "axisValues"]
 _ConditionalFormatType: TypeAlias = Literal["all", "row", "column"]
 _FormatAction: TypeAlias = Literal["blank", "formatting", "drill", "formula"]
 _PivotFilterType: TypeAlias = Literal[
     "unknown",
@@ -102,38 +103,38 @@
     "varP",
     "grand",
     "blank",
 ]
 _PivotFieldSortType: TypeAlias = Literal["manual", "ascending", "descending"]
 
 class HierarchyUsage(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     hierarchyUsage: Integer[Literal[False]]
-    def __init__(self, hierarchyUsage: _ConvertibleToInt) -> None: ...
+    def __init__(self, hierarchyUsage: ConvertibleToInt) -> None: ...
 
 class ColHierarchiesUsage(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     colHierarchyUsage: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, colHierarchyUsage=()) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class RowHierarchiesUsage(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     rowHierarchyUsage: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Incomplete | None = None, rowHierarchyUsage=()) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class PivotFilter(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     fld: Integer[Literal[False]]
     mpFld: Integer[Literal[True]]
     type: Set[_PivotFilterType]
     evalOrder: Integer[Literal[True]]
     id: Integer[Literal[False]]
     iMeasureHier: Integer[Literal[True]]
     iMeasureFld: Integer[Literal[True]]
@@ -143,55 +144,55 @@
     stringValue2: String[Literal[True]]
     autoFilter: Typed[AutoFilter, Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
-        fld: _ConvertibleToInt,
-        mpFld: _ConvertibleToInt | None = None,
+        fld: ConvertibleToInt,
+        mpFld: ConvertibleToInt | None = None,
         *,
         type: _PivotFilterType,
-        evalOrder: _ConvertibleToInt | None = None,
-        id: _ConvertibleToInt,
-        iMeasureHier: _ConvertibleToInt | None = None,
-        iMeasureFld: _ConvertibleToInt | None = None,
+        evalOrder: ConvertibleToInt | None = None,
+        id: ConvertibleToInt,
+        iMeasureHier: ConvertibleToInt | None = None,
+        iMeasureFld: ConvertibleToInt | None = None,
         name: str | None = None,
         description: str | None = None,
         stringValue1: str | None = None,
         stringValue2: str | None = None,
         autoFilter: AutoFilter,
         extLst: ExtensionList | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        fld: _ConvertibleToInt,
-        mpFld: _ConvertibleToInt | None,
+        fld: ConvertibleToInt,
+        mpFld: ConvertibleToInt | None,
         type: _PivotFilterType,
-        evalOrder: _ConvertibleToInt | None,
-        id: _ConvertibleToInt,
-        iMeasureHier: _ConvertibleToInt | None,
-        iMeasureFld: _ConvertibleToInt | None,
+        evalOrder: ConvertibleToInt | None,
+        id: ConvertibleToInt,
+        iMeasureHier: ConvertibleToInt | None,
+        iMeasureFld: ConvertibleToInt | None,
         name: str | None,
         description: str | None,
         stringValue1: str | None,
         stringValue2: str | None,
         autoFilter: AutoFilter,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class PivotFilters(Serialisable):
     count: Integer[Literal[False]]
     filter: Typed[PivotFilter, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, filter: PivotFilter | None = None) -> None: ...
+    def __init__(self, count: ConvertibleToInt, filter: PivotFilter | None = None) -> None: ...
 
 class PivotTableStyle(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[True]]
     showRowHeaders: Bool[Literal[False]]
     showColHeaders: Bool[Literal[False]]
     showRowStripes: Bool[Literal[False]]
     showColStripes: Bool[Literal[False]]
     showLastColumn: Bool[Literal[False]]
     def __init__(
@@ -201,24 +202,24 @@
         showColHeaders: _ConvertibleToBool = None,
         showRowStripes: _ConvertibleToBool = None,
         showColStripes: _ConvertibleToBool = None,
         showLastColumn: _ConvertibleToBool = None,
     ) -> None: ...
 
 class MemberList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     level: Integer[Literal[True]]
     member: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: Incomplete | None = None, level: _ConvertibleToInt | None = None, member=()) -> None: ...
+    def __init__(self, count: Incomplete | None = None, level: ConvertibleToInt | None = None, member=()) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class MemberProperty(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[True]]
     showCell: Bool[Literal[True]]
     showTip: Bool[Literal[True]]
     showAsCaption: Bool[Literal[True]]
     nameLen: Integer[Literal[True]]
     pPos: Integer[Literal[True]]
     pLen: Integer[Literal[True]]
@@ -227,37 +228,37 @@
     @overload
     def __init__(
         self,
         name: str | None = None,
         showCell: _ConvertibleToBool | None = None,
         showTip: _ConvertibleToBool | None = None,
         showAsCaption: _ConvertibleToBool | None = None,
-        nameLen: _ConvertibleToInt | None = None,
-        pPos: _ConvertibleToInt | None = None,
-        pLen: _ConvertibleToInt | None = None,
-        level: _ConvertibleToInt | None = None,
+        nameLen: ConvertibleToInt | None = None,
+        pPos: ConvertibleToInt | None = None,
+        pLen: ConvertibleToInt | None = None,
+        level: ConvertibleToInt | None = None,
         *,
-        field: _ConvertibleToInt,
+        field: ConvertibleToInt,
     ) -> None: ...
     @overload
     def __init__(
         self,
         name: str | None,
         showCell: _ConvertibleToBool | None,
         showTip: _ConvertibleToBool | None,
         showAsCaption: _ConvertibleToBool | None,
-        nameLen: _ConvertibleToInt | None,
-        pPos: _ConvertibleToInt | None,
-        pLen: _ConvertibleToInt | None,
-        level: _ConvertibleToInt | None,
-        field: _ConvertibleToInt,
+        nameLen: ConvertibleToInt | None,
+        pPos: ConvertibleToInt | None,
+        pLen: ConvertibleToInt | None,
+        level: ConvertibleToInt | None,
+        field: ConvertibleToInt,
     ) -> None: ...
 
 class PivotHierarchy(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     outline: Bool[Literal[False]]
     multipleItemSelectionAllowed: Bool[Literal[False]]
     subtotalTop: Bool[Literal[False]]
     showInFieldList: Bool[Literal[False]]
     dragToRow: Bool[Literal[False]]
     dragToCol: Bool[Literal[False]]
     dragToPage: Bool[Literal[False]]
@@ -284,15 +285,15 @@
         caption: str | None = None,
         mps=(),
         members: MemberList | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class Reference(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     field: Integer[Literal[True]]
     selected: Bool[Literal[True]]
     byPosition: Bool[Literal[True]]
     relative: Bool[Literal[True]]
     defaultSubtotal: Bool[Literal[True]]
     sumSubtotal: Bool[Literal[True]]
     countASubtotal: Bool[Literal[True]]
@@ -306,15 +307,15 @@
     varSubtotal: Bool[Literal[True]]
     varPSubtotal: Bool[Literal[True]]
     x: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        field: _ConvertibleToInt | None = None,
+        field: ConvertibleToInt | None = None,
         count: Unused = None,
         selected: _ConvertibleToBool | None = None,
         byPosition: _ConvertibleToBool | None = None,
         relative: _ConvertibleToBool | None = None,
         defaultSubtotal: _ConvertibleToBool | None = None,
         sumSubtotal: _ConvertibleToBool | None = None,
         countASubtotal: _ConvertibleToBool | None = None,
@@ -327,18 +328,18 @@
         stdDevPSubtotal: _ConvertibleToBool | None = None,
         varSubtotal: _ConvertibleToBool | None = None,
         varPSubtotal: _ConvertibleToBool | None = None,
         x: Incomplete | None = (),
         extLst: ExtensionList | None = None,
     ) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class PivotArea(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     references: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     field: Integer[Literal[True]]
     type: NoneSet[_PivotAreaType]
     dataOnly: Bool[Literal[True]]
     labelOnly: Bool[Literal[True]]
     grandRow: Bool[Literal[True]]
@@ -350,184 +351,184 @@
     axis: NoneSet[_PivotAxis]
     fieldPosition: Integer[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         references=(),
         extLst: ExtensionList | None = None,
-        field: _ConvertibleToInt | None = None,
+        field: ConvertibleToInt | None = None,
         type: _PivotAreaType | Literal["none"] | None = "normal",
         dataOnly: _ConvertibleToBool | None = True,
         labelOnly: _ConvertibleToBool | None = None,
         grandRow: _ConvertibleToBool | None = None,
         grandCol: _ConvertibleToBool | None = None,
         cacheIndex: _ConvertibleToBool | None = None,
         outline: _ConvertibleToBool | None = True,
         offset: str | None = None,
         collapsedLevelsAreSubtotals: _ConvertibleToBool | None = None,
         axis: _PivotAxis | Literal["none"] | None = None,
-        fieldPosition: _ConvertibleToInt | None = None,
+        fieldPosition: ConvertibleToInt | None = None,
     ) -> None: ...
 
 class ChartFormat(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     chart: Integer[Literal[False]]
     format: Integer[Literal[False]]
     series: Bool[Literal[False]]
     pivotArea: Typed[PivotArea, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
-        self, chart: _ConvertibleToInt, format: _ConvertibleToInt, series: _ConvertibleToBool = None, *, pivotArea: PivotArea
+        self, chart: ConvertibleToInt, format: ConvertibleToInt, series: _ConvertibleToBool = None, *, pivotArea: PivotArea
     ) -> None: ...
     @overload
     def __init__(
-        self, chart: _ConvertibleToInt, format: _ConvertibleToInt, series: _ConvertibleToBool, pivotArea: PivotArea
+        self, chart: ConvertibleToInt, format: ConvertibleToInt, series: _ConvertibleToBool, pivotArea: PivotArea
     ) -> None: ...
 
 class ConditionalFormat(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     scope: Set[_ConditionalFormatScope]
     type: NoneSet[_ConditionalFormatType]
     priority: Integer[Literal[False]]
     pivotAreas: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         scope: _ConditionalFormatScope = "selection",
         type: _ConditionalFormatType | Literal["none"] | None = None,
         *,
-        priority: _ConvertibleToInt,
+        priority: ConvertibleToInt,
         pivotAreas=(),
         extLst: ExtensionList | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         scope: _ConditionalFormatScope,
         type: _ConditionalFormatType | Literal["none"] | None,
-        priority: _ConvertibleToInt,
+        priority: ConvertibleToInt,
         pivotAreas=(),
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class ConditionalFormatList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     conditionalFormat: Incomplete
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, conditionalFormat=..., count: Incomplete | None = ...) -> None: ...
     def by_priority(self): ...
     @property
-    def count(self): ...
-    def to_tree(self, tagname: Incomplete | None = ...): ...  # type: ignore[override]
+    def count(self) -> int: ...
+    def to_tree(self, tagname: str | None = None) -> Element: ...  # type: ignore[override]
 
 class Format(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     action: NoneSet[_FormatAction]
     dxfId: Integer[Literal[True]]
     pivotArea: Typed[PivotArea, Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         action: _FormatAction | Literal["none"] | None = "formatting",
-        dxfId: _ConvertibleToInt | None = None,
+        dxfId: ConvertibleToInt | None = None,
         *,
         pivotArea: PivotArea,
         extLst: ExtensionList | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         action: _FormatAction | Literal["none"] | None,
-        dxfId: _ConvertibleToInt | None,
+        dxfId: ConvertibleToInt | None,
         pivotArea: PivotArea,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class DataField(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[True]]
     fld: Integer[Literal[False]]
     subtotal: Set[_DataFieldSubtotal]
     showDataAs: Set[_DataFieldShowDataAs]
     baseField: Integer[Literal[False]]
     baseItem: Integer[Literal[False]]
     numFmtId: Integer[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         name: str | None = None,
         *,
-        fld: _ConvertibleToInt,
+        fld: ConvertibleToInt,
         subtotal: str = "sum",
         showDataAs: str = "normal",
-        baseField: _ConvertibleToInt = -1,
-        baseItem: _ConvertibleToInt = 1048832,
-        numFmtId: _ConvertibleToInt | None = None,
+        baseField: ConvertibleToInt = -1,
+        baseItem: ConvertibleToInt = 1048832,
+        numFmtId: ConvertibleToInt | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         name: str | None,
-        fld: _ConvertibleToInt,
+        fld: ConvertibleToInt,
         subtotal: str = "sum",
         showDataAs: str = "normal",
-        baseField: _ConvertibleToInt = -1,
-        baseItem: _ConvertibleToInt = 1048832,
-        numFmtId: _ConvertibleToInt | None = None,
+        baseField: ConvertibleToInt = -1,
+        baseItem: ConvertibleToInt = 1048832,
+        numFmtId: ConvertibleToInt | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class PageField(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     fld: Integer[Literal[False]]
     item: Integer[Literal[True]]
     hier: Integer[Literal[True]]
     name: String[Literal[True]]
     cap: String[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        fld: _ConvertibleToInt,
-        item: _ConvertibleToInt | None = None,
-        hier: _ConvertibleToInt | None = None,
+        fld: ConvertibleToInt,
+        item: ConvertibleToInt | None = None,
+        hier: ConvertibleToInt | None = None,
         name: str | None = None,
         cap: str | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class RowColItem(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     t: Set[_ItemType]
     r: Integer[Literal[False]]
     i: Integer[Literal[False]]
     x: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, t: _ItemType = "data", r: _ConvertibleToInt = 0, i: _ConvertibleToInt = 0, x=()) -> None: ...
+    def __init__(self, t: _ItemType = "data", r: ConvertibleToInt = 0, i: ConvertibleToInt = 0, x=()) -> None: ...
 
 class RowColField(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     x: Integer[Literal[False]]
-    def __init__(self, x: _ConvertibleToInt) -> None: ...
+    def __init__(self, x: ConvertibleToInt) -> None: ...
 
 class AutoSortScope(Serialisable):
     pivotArea: Typed[PivotArea, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, pivotArea: PivotArea) -> None: ...
 
 class FieldItem(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     n: String[Literal[True]]
     t: Set[_ItemType]
     h: Bool[Literal[True]]
     s: Bool[Literal[True]]
     sd: Bool[Literal[True]]
     f: Bool[Literal[True]]
     m: Bool[Literal[True]]
@@ -541,21 +542,21 @@
         t: _ItemType = "data",
         h: _ConvertibleToBool | None = None,
         s: _ConvertibleToBool | None = None,
         sd: _ConvertibleToBool | None = True,
         f: _ConvertibleToBool | None = None,
         m: _ConvertibleToBool | None = None,
         c: _ConvertibleToBool | None = None,
-        x: _ConvertibleToInt | None = None,
+        x: ConvertibleToInt | None = None,
         d: _ConvertibleToBool | None = None,
         e: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class PivotField(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     items: Incomplete
     autoSortScope: Typed[AutoSortScope, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     name: String[Literal[True]]
     axis: NoneSet[_PivotAxis]
     dataField: Bool[Literal[True]]
     subtotalCaption: String[Literal[True]]
@@ -613,15 +614,15 @@
         dataField: _ConvertibleToBool | None = None,
         subtotalCaption: str | None = None,
         showDropDowns: _ConvertibleToBool | None = True,
         hiddenLevel: _ConvertibleToBool | None = None,
         uniqueMemberProperty: str | None = None,
         compact: _ConvertibleToBool | None = True,
         allDrilled: _ConvertibleToBool | None = None,
-        numFmtId: _ConvertibleToInt | None = None,
+        numFmtId: ConvertibleToInt | None = None,
         outline: _ConvertibleToBool | None = True,
         subtotalTop: _ConvertibleToBool | None = True,
         dragToRow: _ConvertibleToBool | None = True,
         dragToCol: _ConvertibleToBool | None = True,
         multipleItemSelectionAllowed: _ConvertibleToBool | None = None,
         dragToPage: _ConvertibleToBool | None = True,
         dragToData: _ConvertibleToBool | None = True,
@@ -631,19 +632,19 @@
         serverField: _ConvertibleToBool | None = None,
         insertPageBreak: _ConvertibleToBool | None = None,
         autoShow: _ConvertibleToBool | None = None,
         topAutoShow: _ConvertibleToBool | None = True,
         hideNewItems: _ConvertibleToBool | None = None,
         measureFilter: _ConvertibleToBool | None = None,
         includeNewItemsInFilter: _ConvertibleToBool | None = None,
-        itemPageCount: _ConvertibleToInt | None = 10,
+        itemPageCount: ConvertibleToInt | None = 10,
         sortType: _PivotFieldSortType = "manual",
         dataSourceSort: _ConvertibleToBool | None = None,
         nonAutoSortDefault: _ConvertibleToBool | None = None,
-        rankBy: _ConvertibleToInt | None = None,
+        rankBy: ConvertibleToInt | None = None,
         defaultSubtotal: _ConvertibleToBool | None = True,
         sumSubtotal: _ConvertibleToBool | None = None,
         countASubtotal: _ConvertibleToBool | None = None,
         avgSubtotal: _ConvertibleToBool | None = None,
         maxSubtotal: _ConvertibleToBool | None = None,
         minSubtotal: _ConvertibleToBool | None = None,
         productSubtotal: _ConvertibleToBool | None = None,
@@ -656,35 +657,35 @@
         showPropTip: _ConvertibleToBool | None = None,
         showPropAsCaption: _ConvertibleToBool | None = None,
         defaultAttributeDrillState: _ConvertibleToBool | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class Location(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ref: String[Literal[False]]
     firstHeaderRow: Integer[Literal[False]]
     firstDataRow: Integer[Literal[False]]
     firstDataCol: Integer[Literal[False]]
     rowPageCount: Integer[Literal[True]]
     colPageCount: Integer[Literal[True]]
     def __init__(
         self,
         ref: str,
-        firstHeaderRow: _ConvertibleToInt,
-        firstDataRow: _ConvertibleToInt,
-        firstDataCol: _ConvertibleToInt,
-        rowPageCount: _ConvertibleToInt | None = None,
-        colPageCount: _ConvertibleToInt | None = None,
+        firstHeaderRow: ConvertibleToInt,
+        firstDataRow: ConvertibleToInt,
+        firstDataCol: ConvertibleToInt,
+        rowPageCount: ConvertibleToInt | None = None,
+        colPageCount: ConvertibleToInt | None = None,
     ) -> None: ...
 
 class TableDefinition(Serialisable):
     mime_type: str
     rel_type: str
-    tagname: str
+    tagname: ClassVar[str]
     cache: Incomplete
     name: String[Literal[False]]
     cacheId: Integer[Literal[False]]
     dataOnRows: Bool[Literal[False]]
     dataPosition: Integer[Literal[True]]
     dataCaption: String[Literal[False]]
     grandTotalCaption: String[Literal[True]]
@@ -769,30 +770,30 @@
     extLst: Typed[ExtensionList, Literal[True]]
     id: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         name: str,
-        cacheId: _ConvertibleToInt,
+        cacheId: ConvertibleToInt,
         dataOnRows: _ConvertibleToBool = False,
-        dataPosition: _ConvertibleToInt | None = None,
+        dataPosition: ConvertibleToInt | None = None,
         *,
         dataCaption: str,
         grandTotalCaption: str | None = None,
         errorCaption: str | None = None,
         showError: _ConvertibleToBool = False,
         missingCaption: str | None = None,
         showMissing: _ConvertibleToBool = True,
         pageStyle: str | None = None,
         pivotTableStyle: str | None = None,
         vacatedStyle: str | None = None,
         tag: str | None = None,
-        updatedVersion: _ConvertibleToInt = 0,
-        minRefreshableVersion: _ConvertibleToInt = 0,
+        updatedVersion: ConvertibleToInt = 0,
+        minRefreshableVersion: ConvertibleToInt = 0,
         asteriskTotals: _ConvertibleToBool = False,
         showItems: _ConvertibleToBool = True,
         editData: _ConvertibleToBool = False,
         disableFieldList: _ConvertibleToBool = False,
         showCalcMbrs: _ConvertibleToBool = True,
         visualTotals: _ConvertibleToBool = True,
         showMultipleLabel: _ConvertibleToBool = True,
@@ -802,43 +803,43 @@
         showMemberPropertyTips: _ConvertibleToBool = True,
         showDataTips: _ConvertibleToBool = True,
         enableWizard: _ConvertibleToBool = True,
         enableDrill: _ConvertibleToBool = True,
         enableFieldProperties: _ConvertibleToBool = True,
         preserveFormatting: _ConvertibleToBool = True,
         useAutoFormatting: _ConvertibleToBool = False,
-        pageWrap: _ConvertibleToInt = 0,
+        pageWrap: ConvertibleToInt = 0,
         pageOverThenDown: _ConvertibleToBool = False,
         subtotalHiddenItems: _ConvertibleToBool = False,
         rowGrandTotals: _ConvertibleToBool = True,
         colGrandTotals: _ConvertibleToBool = True,
         fieldPrintTitles: _ConvertibleToBool = False,
         itemPrintTitles: _ConvertibleToBool = False,
         mergeItem: _ConvertibleToBool = False,
         showDropZones: _ConvertibleToBool = True,
-        createdVersion: _ConvertibleToInt = 0,
-        indent: _ConvertibleToInt = 1,
+        createdVersion: ConvertibleToInt = 0,
+        indent: ConvertibleToInt = 1,
         showEmptyRow: _ConvertibleToBool = False,
         showEmptyCol: _ConvertibleToBool = False,
         showHeaders: _ConvertibleToBool = True,
         compact: _ConvertibleToBool = True,
         outline: _ConvertibleToBool = False,
         outlineData: _ConvertibleToBool = False,
         compactData: _ConvertibleToBool = True,
         published: _ConvertibleToBool = False,
         gridDropZones: _ConvertibleToBool = False,
         immersive: _ConvertibleToBool = True,
         multipleFieldFilters: _ConvertibleToBool = None,
-        chartFormat: _ConvertibleToInt = 0,
+        chartFormat: ConvertibleToInt = 0,
         rowHeaderCaption: str | None = None,
         colHeaderCaption: str | None = None,
         fieldListSortAscending: _ConvertibleToBool = None,
         mdxSubqueries: _ConvertibleToBool = None,
         customListSort: _ConvertibleToBool | None = None,
-        autoFormatId: _ConvertibleToInt | None = None,
+        autoFormatId: ConvertibleToInt | None = None,
         applyNumberFormats: _ConvertibleToBool = False,
         applyBorderFormats: _ConvertibleToBool = False,
         applyFontFormats: _ConvertibleToBool = False,
         applyPatternFormats: _ConvertibleToBool = False,
         applyAlignmentFormats: _ConvertibleToBool = False,
         applyWidthHeightFormats: _ConvertibleToBool = False,
         location: Location,
@@ -860,29 +861,29 @@
         extLst: ExtensionList | None = None,
         id: Incomplete | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         name: str,
-        cacheId: _ConvertibleToInt,
+        cacheId: ConvertibleToInt,
         dataOnRows: _ConvertibleToBool,
-        dataPosition: _ConvertibleToInt | None,
+        dataPosition: ConvertibleToInt | None,
         dataCaption: str,
         grandTotalCaption: str | None,
         errorCaption: str | None,
         showError: _ConvertibleToBool,
         missingCaption: str | None,
         showMissing: _ConvertibleToBool,
         pageStyle: str | None,
         pivotTableStyle: str | None,
         vacatedStyle: str | None,
         tag: str | None,
-        updatedVersion: _ConvertibleToInt,
-        minRefreshableVersion: _ConvertibleToInt,
+        updatedVersion: ConvertibleToInt,
+        minRefreshableVersion: ConvertibleToInt,
         asteriskTotals: _ConvertibleToBool,
         showItems: _ConvertibleToBool,
         editData: _ConvertibleToBool,
         disableFieldList: _ConvertibleToBool,
         showCalcMbrs: _ConvertibleToBool,
         visualTotals: _ConvertibleToBool,
         showMultipleLabel: _ConvertibleToBool,
@@ -892,43 +893,43 @@
         showMemberPropertyTips: _ConvertibleToBool,
         showDataTips: _ConvertibleToBool,
         enableWizard: _ConvertibleToBool,
         enableDrill: _ConvertibleToBool,
         enableFieldProperties: _ConvertibleToBool,
         preserveFormatting: _ConvertibleToBool,
         useAutoFormatting: _ConvertibleToBool,
-        pageWrap: _ConvertibleToInt,
+        pageWrap: ConvertibleToInt,
         pageOverThenDown: _ConvertibleToBool,
         subtotalHiddenItems: _ConvertibleToBool,
         rowGrandTotals: _ConvertibleToBool,
         colGrandTotals: _ConvertibleToBool,
         fieldPrintTitles: _ConvertibleToBool,
         itemPrintTitles: _ConvertibleToBool,
         mergeItem: _ConvertibleToBool,
         showDropZones: _ConvertibleToBool,
-        createdVersion: _ConvertibleToInt,
-        indent: _ConvertibleToInt,
+        createdVersion: ConvertibleToInt,
+        indent: ConvertibleToInt,
         showEmptyRow: _ConvertibleToBool,
         showEmptyCol: _ConvertibleToBool,
         showHeaders: _ConvertibleToBool,
         compact: _ConvertibleToBool,
         outline: _ConvertibleToBool,
         outlineData: _ConvertibleToBool,
         compactData: _ConvertibleToBool,
         published: _ConvertibleToBool,
         gridDropZones: _ConvertibleToBool,
         immersive: _ConvertibleToBool,
         multipleFieldFilters: _ConvertibleToBool,
-        chartFormat: _ConvertibleToInt,
+        chartFormat: ConvertibleToInt,
         rowHeaderCaption: str | None,
         colHeaderCaption: str | None,
         fieldListSortAscending: _ConvertibleToBool,
         mdxSubqueries: _ConvertibleToBool,
         customListSort: _ConvertibleToBool | None,
-        autoFormatId: _ConvertibleToInt | None,
+        autoFormatId: ConvertibleToInt | None,
         applyNumberFormats: _ConvertibleToBool,
         applyBorderFormats: _ConvertibleToBool,
         applyFontFormats: _ConvertibleToBool,
         applyPatternFormats: _ConvertibleToBool,
         applyAlignmentFormats: _ConvertibleToBool,
         applyWidthHeightFormats: _ConvertibleToBool,
         location: Location,
@@ -946,10 +947,13 @@
         pivotTableStyleInfo: PivotTableStyle | None = None,
         filters=(),
         rowHierarchiesUsage: RowHierarchiesUsage | None = None,
         colHierarchiesUsage: ColHierarchiesUsage | None = None,
         extLst: ExtensionList | None = None,
         id: Incomplete | None = None,
     ) -> None: ...
-    def to_tree(self): ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
     @property
-    def path(self): ...
+    def path(self) -> str: ...
+    def formatted_fields(self) -> dict[Incomplete, list[Incomplete]]: ...
+    @property
+    def summary(self) -> str: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/reader/excel.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/reader/excel.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-from _typeshed import Incomplete, StrPath, SupportsRead
+from typing import Final, Literal
+from typing_extensions import TypeAlias
 from zipfile import ZipFile
 
+from openpyxl import _ZipFileFileProtocol
 from openpyxl.chartsheet.chartsheet import Chartsheet
 from openpyxl.packaging.manifest import Manifest
 from openpyxl.packaging.relationship import Relationship
 from openpyxl.reader.workbook import WorkbookParser
 from openpyxl.workbook import Workbook
 
-SUPPORTED_FORMATS: Incomplete
+_SupportedFormats: TypeAlias = Literal[".xlsx", ".xlsm", ".xltx", ".xltm"]
+SUPPORTED_FORMATS: Final[tuple[_SupportedFormats, ...]]
 
 class ExcelReader:
     archive: ZipFile
     valid_files: list[str]
     read_only: bool
     keep_vba: bool
     data_only: bool
     keep_links: bool
     rich_text: bool
-    shared_strings: list[Incomplete]
+    shared_strings: list[str]
     package: Manifest  # defined after call to read_manifest()
     parser: WorkbookParser  # defined after call to read_workbook()
     wb: Workbook  # defined after call to read_workbook()
 
     def __init__(
         self,
-        fn: SupportsRead[bytes] | str,
+        fn: _ZipFileFileProtocol,
         read_only: bool = False,
         keep_vba: bool = False,
         data_only: bool = False,
         keep_links: bool = True,
         rich_text: bool = False,
     ) -> None: ...
     def read_manifest(self) -> None: ...
     def read_strings(self) -> None: ...
     def read_workbook(self) -> None: ...
     def read_properties(self) -> None: ...
+    def read_custom(self) -> None: ...
     def read_theme(self) -> None: ...
     def read_chartsheet(self, sheet: Chartsheet, rel: Relationship) -> None: ...
     def read_worksheets(self) -> None: ...
     def read(self) -> None: ...
 
 def load_workbook(
-    filename: SupportsRead[bytes] | StrPath,
+    filename: _ZipFileFileProtocol,
     read_only: bool = False,
     keep_vba: bool = False,
     data_only: bool = False,
     keep_links: bool = True,
     rich_text: bool = False,
 ) -> Workbook: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/__init__.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/alignment.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/alignment.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from _typeshed import Incomplete
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, Incomplete
+from collections.abc import Iterator
+from typing import ClassVar, Final, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Alias, Bool, Min, MinMax, NoneSet, _ConvertibleToBool, _ConvertibleToFloat
+from openpyxl.descriptors.base import Alias, Bool, Min, MinMax, NoneSet, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 _HorizontalAlignmentsType: TypeAlias = Literal[
     "general", "left", "center", "right", "fill", "justify", "centerContinuous", "distributed"
 ]
 _VerticalAlignmentsType: TypeAlias = Literal["top", "center", "bottom", "justify", "distributed"]
 
-horizontal_alignments: tuple[_HorizontalAlignmentsType, ...]
-vertical_aligments: tuple[_VerticalAlignmentsType, ...]
+horizontal_alignments: Final[tuple[_HorizontalAlignmentsType, ...]]
+vertical_aligments: Final[tuple[_VerticalAlignmentsType, ...]]
 
 class Alignment(Serialisable):
-    tagname: str
-    __fields__: Incomplete
+    tagname: ClassVar[str]
+    __fields__: ClassVar[tuple[str, ...]]
     horizontal: NoneSet[_HorizontalAlignmentsType]
     vertical: NoneSet[_VerticalAlignmentsType]
     textRotation: NoneSet[int]
     text_rotation: Alias
     wrapText: Bool[Literal[True]]
     wrap_text: Alias
     shrinkToFit: Bool[Literal[True]]
@@ -30,17 +32,17 @@
     def __init__(
         self,
         horizontal: Incomplete | None = None,
         vertical: Incomplete | None = None,
         textRotation: int = 0,
         wrapText: _ConvertibleToBool | None = None,
         shrinkToFit: _ConvertibleToBool | None = None,
-        indent: _ConvertibleToFloat = 0,
-        relativeIndent: _ConvertibleToFloat = 0,
+        indent: ConvertibleToFloat = 0,
+        relativeIndent: ConvertibleToFloat = 0,
         justifyLastLine: _ConvertibleToBool | None = None,
-        readingOrder: _ConvertibleToFloat = 0,
+        readingOrder: ConvertibleToFloat = 0,
         text_rotation: Incomplete | None = None,
         wrap_text: Incomplete | None = None,
         shrink_to_fit: Incomplete | None = None,
         mergeCell: Incomplete | None = None,
     ) -> None: ...
-    def __iter__(self): ...
+    def __iter__(self) -> Iterator[tuple[str, str]]: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/borders.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/table.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,80 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
+from openpyxl.descriptors.base import Bool, Integer, Set, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
-_SideStyle: TypeAlias = Literal[
-    "dashDot",
-    "dashDotDot",
-    "dashed",
-    "dotted",
-    "double",
-    "hair",
-    "medium",
-    "mediumDashDot",
-    "mediumDashDotDot",
-    "mediumDashed",
-    "slantDashDot",
-    "thick",
-    "thin",
+_TableStyleElementType: TypeAlias = Literal[
+    "wholeTable",
+    "headerRow",
+    "totalRow",
+    "firstColumn",
+    "lastColumn",
+    "firstRowStripe",
+    "secondRowStripe",
+    "firstColumnStripe",
+    "secondColumnStripe",
+    "firstHeaderCell",
+    "lastHeaderCell",
+    "firstTotalCell",
+    "lastTotalCell",
+    "firstSubtotalColumn",
+    "secondSubtotalColumn",
+    "thirdSubtotalColumn",
+    "firstSubtotalRow",
+    "secondSubtotalRow",
+    "thirdSubtotalRow",
+    "blankRow",
+    "firstColumnSubheading",
+    "secondColumnSubheading",
+    "thirdColumnSubheading",
+    "firstRowSubheading",
+    "secondRowSubheading",
+    "thirdRowSubheading",
+    "pageFieldLabels",
+    "pageFieldValues",
 ]
 
-BORDER_NONE: Incomplete
-BORDER_DASHDOT: str
-BORDER_DASHDOTDOT: str
-BORDER_DASHED: str
-BORDER_DOTTED: str
-BORDER_DOUBLE: str
-BORDER_HAIR: str
-BORDER_MEDIUM: str
-BORDER_MEDIUMDASHDOT: str
-BORDER_MEDIUMDASHDOTDOT: str
-BORDER_MEDIUMDASHED: str
-BORDER_SLANTDASHDOT: str
-BORDER_THICK: str
-BORDER_THIN: str
+class TableStyleElement(Serialisable):
+    tagname: ClassVar[str]
+    type: Set[_TableStyleElementType]
+    size: Integer[Literal[True]]
+    dxfId: Integer[Literal[True]]
+    def __init__(
+        self, type: _TableStyleElementType, size: ConvertibleToInt | None = None, dxfId: ConvertibleToInt | None = None
+    ) -> None: ...
 
-class Side(Serialisable):
-    __fields__: Incomplete
-    color: Incomplete
-    style: NoneSet[_SideStyle]
-    border_style: Alias
+class TableStyle(Serialisable):
+    tagname: ClassVar[str]
+    name: String[Literal[False]]
+    pivot: Bool[Literal[True]]
+    table: Bool[Literal[True]]
+    count: Integer[Literal[True]]
+    tableStyleElement: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        style: _SideStyle | Literal["none"] | None = None,
-        color: Incomplete | None = None,
-        border_style: Incomplete | None = None,
+        name: str,
+        pivot: _ConvertibleToBool | None = None,
+        table: _ConvertibleToBool | None = None,
+        count: ConvertibleToInt | None = None,
+        tableStyleElement=(),
     ) -> None: ...
 
-class Border(Serialisable):
-    tagname: str
-    __fields__: Incomplete
+class TableStyleList(Serialisable):
+    tagname: ClassVar[str]
+    defaultTableStyle: String[Literal[True]]
+    defaultPivotStyle: String[Literal[True]]
+    tableStyle: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    start: Typed[Side, Literal[True]]
-    end: Typed[Side, Literal[True]]
-    left: Typed[Side, Literal[True]]
-    right: Typed[Side, Literal[True]]
-    top: Typed[Side, Literal[True]]
-    bottom: Typed[Side, Literal[True]]
-    diagonal: Typed[Side, Literal[True]]
-    vertical: Typed[Side, Literal[True]]
-    horizontal: Typed[Side, Literal[True]]
-    outline: Bool[Literal[False]]
-    diagonalUp: Bool[Literal[False]]
-    diagonalDown: Bool[Literal[False]]
-    diagonal_direction: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        left: Side | None = None,
-        right: Side | None = None,
-        top: Side | None = None,
-        bottom: Side | None = None,
-        diagonal: Side | None = None,
-        diagonal_direction: Incomplete | None = None,
-        vertical: Side | None = None,
-        horizontal: Side | None = None,
-        diagonalUp: _ConvertibleToBool = False,
-        diagonalDown: _ConvertibleToBool = False,
-        outline: _ConvertibleToBool = True,
-        start: Side | None = None,
-        end: Side | None = None,
+        count: Unused = None,
+        defaultTableStyle: str | None = "TableStyleMedium9",
+        defaultPivotStyle: str | None = "PivotStyleLight16",
+        tableStyle=(),
     ) -> None: ...
-    def __iter__(self): ...
-
-DEFAULT_BORDER: Incomplete
+    @property
+    def count(self) -> int: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/builtins.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/builtins.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/cell_style.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/scenario.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,87 @@
-from _typeshed import Incomplete, Unused
-from array import array
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal, overload
 
-from openpyxl.descriptors import Strict
-from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool, _ConvertibleToInt
-from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.base import Bool, Convertible, Integer, String, _ConvertibleToBool, _ConvertibleToMultiCellRange
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.styles.alignment import Alignment
-from openpyxl.styles.protection import Protection
+from openpyxl.worksheet.cell_range import MultiCellRange
 
-class ArrayDescriptor:
-    key: Incomplete
-    def __init__(self, key) -> None: ...
-    def __get__(self, instance: Serialisable | Strict, cls: Unused): ...
-    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
+class InputCells(Serialisable):
+    tagname: ClassVar[str]
+    r: String[Literal[False]]
+    deleted: Bool[Literal[True]]
+    undone: Bool[Literal[True]]
+    val: String[Literal[False]]
+    numFmtId: Integer[Literal[True]]
 
-class StyleArray(array[Incomplete]):
-    tagname: str
-    fontId: Incomplete
-    fillId: Incomplete
-    borderId: Incomplete
-    numFmtId: Incomplete
-    protectionId: Incomplete
-    alignmentId: Incomplete
-    pivotButton: Incomplete
-    quotePrefix: Incomplete
-    xfId: Incomplete
-    def __new__(cls, args=[0, 0, 0, 0, 0, 0, 0, 0, 0]): ...
-    def __hash__(self) -> int: ...
-    def __copy__(self): ...
-    def __deepcopy__(self, memo): ...
+    @overload
+    def __init__(
+        self,
+        r: str,
+        deleted: _ConvertibleToBool | None = False,
+        undone: _ConvertibleToBool | None = False,
+        *,
+        val: str,
+        numFmtId: ConvertibleToInt | None = None,
+    ) -> None: ...
+    @overload
+    def __init__(
+        self,
+        r: str,
+        deleted: _ConvertibleToBool | None,
+        undone: _ConvertibleToBool | None,
+        val: str,
+        numFmtId: ConvertibleToInt | None = None,
+    ) -> None: ...
 
-class CellStyle(Serialisable):
-    tagname: str
-    numFmtId: Integer[Literal[False]]
-    fontId: Integer[Literal[False]]
-    fillId: Integer[Literal[False]]
-    borderId: Integer[Literal[False]]
-    xfId: Integer[Literal[True]]
-    quotePrefix: Bool[Literal[True]]
-    pivotButton: Bool[Literal[True]]
-    applyNumberFormat: Bool[Literal[True]]
-    applyFont: Bool[Literal[True]]
-    applyFill: Bool[Literal[True]]
-    applyBorder: Bool[Literal[True]]
-    # Overwritten by properties below
-    # applyAlignment: Bool[Literal[True]]
-    # applyProtection: Bool[Literal[True]]
-    alignment: Typed[Alignment, Literal[True]]
-    protection: Typed[Protection, Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
+class Scenario(Serialisable):
+    tagname: ClassVar[str]
+    inputCells: Incomplete
+    name: String[Literal[False]]
+    locked: Bool[Literal[True]]
+    hidden: Bool[Literal[True]]
+    user: String[Literal[True]]
+    comment: String[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
+    @overload
     def __init__(
         self,
-        numFmtId: _ConvertibleToInt = 0,
-        fontId: _ConvertibleToInt = 0,
-        fillId: _ConvertibleToInt = 0,
-        borderId: _ConvertibleToInt = 0,
-        xfId: _ConvertibleToInt | None = None,
-        quotePrefix: _ConvertibleToBool | None = None,
-        pivotButton: _ConvertibleToBool | None = None,
-        applyNumberFormat: _ConvertibleToBool | None = None,
-        applyFont: _ConvertibleToBool | None = None,
-        applyFill: _ConvertibleToBool | None = None,
-        applyBorder: _ConvertibleToBool | None = None,
-        applyAlignment: Unused = None,
-        applyProtection: Unused = None,
-        alignment: Alignment | None = None,
-        protection: Protection | None = None,
-        extLst: Unused = None,
+        inputCells=(),
+        *,
+        name: str,
+        locked: _ConvertibleToBool | None = False,
+        hidden: _ConvertibleToBool | None = False,
+        count: Unused = None,
+        user: str | None = None,
+        comment: str | None = None,
+    ) -> None: ...
+    @overload
+    def __init__(
+        self,
+        inputCells,
+        name: str,
+        locked: _ConvertibleToBool | None = False,
+        hidden: _ConvertibleToBool | None = False,
+        count: Unused = None,
+        user: str | None = None,
+        comment: str | None = None,
     ) -> None: ...
-    def to_array(self): ...
-    @classmethod
-    def from_array(cls, style): ...
-    @property
-    def applyProtection(self): ...
     @property
-    def applyAlignment(self): ...
+    def count(self) -> int: ...
 
-class CellStyleList(Serialisable):
-    tagname: str
-    __attrs__: ClassVar[tuple[str, ...]]
-    # Overwritten by property below
-    # count: Integer
-    xf: Incomplete
-    alignment: Incomplete
-    protection: Incomplete
+class ScenarioList(Serialisable):
+    tagname: ClassVar[str]
+    scenario: Incomplete
+    current: Integer[Literal[True]]
+    show: Integer[Literal[True]]
+    sqref: Convertible[MultiCellRange, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: Unused = None, xf=()) -> None: ...
-    @property
-    def count(self): ...
-    def __getitem__(self, idx): ...
+    def __init__(
+        self,
+        scenario=(),
+        current: ConvertibleToInt | None = None,
+        show: ConvertibleToInt | None = None,
+        sqref: _ConvertibleToMultiCellRange | None = None,
+    ) -> None: ...
+    def append(self, scenario) -> None: ...
+    def __bool__(self) -> bool: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/colors.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/pagebreak.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,48 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors import Strict, Typed
-from openpyxl.descriptors.base import Bool, Integer, MinMax, String, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
-COLOR_INDEX: Incomplete
-BLACK: Incomplete
-WHITE: Incomplete
-BLUE: Incomplete
-aRGB_REGEX: Incomplete
-
-class RGB(Typed[str, Incomplete]):
-    expected_type: type[str]
-    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
-
-class Color(Serialisable):
-    tagname: str
-    rgb: Incomplete
-    indexed: Integer[Literal[False]]
-    auto: Bool[Literal[False]]
-    theme: Integer[Literal[False]]
-    tint: MinMax[float, Literal[False]]
-    type: String[Literal[False]]
+class Break(Serialisable):
+    tagname: ClassVar[str]
+    id: Integer[Literal[True]]
+    min: Integer[Literal[True]]
+    max: Integer[Literal[True]]
+    man: Bool[Literal[True]]
+    pt: Bool[Literal[True]]
     def __init__(
         self,
-        rgb="00000000",
-        indexed: _ConvertibleToInt | None = None,
-        auto: _ConvertibleToBool | None = None,
-        theme: _ConvertibleToInt | None = None,
-        tint: _ConvertibleToFloat = 0.0,
-        index: _ConvertibleToInt | None = None,
-        type: Unused = "rgb",
+        id: ConvertibleToInt | None = 0,
+        min: ConvertibleToInt | None = 0,
+        max: ConvertibleToInt | None = 16383,
+        man: _ConvertibleToBool | None = True,
+        pt: _ConvertibleToBool | None = None,
     ) -> None: ...
-    @property
-    def value(self): ...
-    @value.setter
-    def value(self, value) -> None: ...
-    def __iter__(self): ...
-    @property
-    def index(self): ...
-    def __add__(self, other): ...
-
-class ColorDescriptor(Typed[Color, Incomplete]):
-    expected_type: type[Color]
-    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
 
-class RgbColor(Serialisable):
-    tagname: str
-    rgb: Incomplete
-    def __init__(self, rgb: Incomplete | None = None) -> None: ...
-
-class ColorList(Serialisable):
-    tagname: str
-    indexedColors: Incomplete
-    mruColors: Incomplete
+class RowBreak(Serialisable):
+    tagname: ClassVar[str]
+    # Overwritten by properties below
+    # count: Integer
+    # manualBreakCount: Integer
+    brk: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, indexedColors=(), mruColors=()) -> None: ...
+    __attrs__: ClassVar[tuple[str, ...]]
+    def __init__(self, count: Unused = None, manualBreakCount: Unused = None, brk=()) -> None: ...
     def __bool__(self) -> bool: ...
+    def __len__(self) -> int: ...
+    @property
+    def count(self) -> int: ...
     @property
-    def index(self): ...
+    def manualBreakCount(self) -> int: ...
+    def append(self, brk: Incomplete | None = None) -> None: ...
+
+PageBreak = RowBreak
+
+class ColBreak(RowBreak):
+    tagname: ClassVar[str]
+    # Same as parent
+    # count = RowBreak.count
+    # manualBreakCount = RowBreak.manualBreakCount
+    # brk = RowBreak.brk
+    __attrs__: ClassVar[tuple[str, ...]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/differential.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/differential.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import Incomplete, Unused
+from typing import ClassVar, Literal, SupportsIndex
 
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles import Alignment, Border, Fill, Font, Protection
 from openpyxl.styles.numbers import NumberFormat
 
 class DifferentialStyle(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     __elements__: ClassVar[tuple[str, ...]]
     font: Typed[Font, Literal[True]]
     numFmt: Typed[NumberFormat, Literal[True]]
     fill: Typed[Fill, Literal[True]]
     alignment: Typed[Alignment, Literal[True]]
     border: Typed[Border, Literal[True]]
     protection: Typed[Protection, Literal[True]]
@@ -26,18 +25,18 @@
         alignment: Alignment | None = None,
         border: Border | None = None,
         protection: Protection | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
 
 class DifferentialStyleList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     dxf: Incomplete
     styles: Alias
     __attrs__: ClassVar[tuple[str, ...]]
-    def __init__(self, dxf=(), count: Incomplete | None = None) -> None: ...
-    def append(self, dxf) -> None: ...
-    def add(self, dxf): ...
+    def __init__(self, dxf=(), count: Unused = None) -> None: ...
+    def append(self, dxf: DifferentialStyle) -> None: ...
+    def add(self, dxf: DifferentialStyle) -> int: ...
     def __bool__(self) -> bool: ...
-    def __getitem__(self, idx): ...
+    def __getitem__(self, idx: SupportsIndex) -> DifferentialStyle: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/fills.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/fills.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Final, Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, Incomplete, Unused
+from collections.abc import Iterable, Iterator, Sequence as ABCSequence
+from typing import ClassVar, Final, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors import Sequence
-from openpyxl.descriptors.base import Alias, Float, MinMax, NoneSet, Set, _ConvertibleToFloat
+from openpyxl.descriptors import Sequence, Strict
+from openpyxl.descriptors.base import Alias, Float, MinMax, NoneSet, Set
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles.colors import Color, ColorDescriptor
+from openpyxl.xml.functions import Element
+
+from ..xml._functions_overloads import _SupportsIterAndAttribAndTextAndTag
 
 FILL_NONE: Final = "none"
 FILL_SOLID: Final = "solid"
 FILL_PATTERN_DARKDOWN: Final = "darkDown"
 FILL_PATTERN_DARKGRAY: Final = "darkGray"
 FILL_PATTERN_DARKGRID: Final = "darkGrid"
 FILL_PATTERN_DARKHORIZONTAL: Final = "darkHorizontal"
@@ -24,15 +29,14 @@
 FILL_PATTERN_LIGHTTRELLIS: Final = "lightTrellis"
 FILL_PATTERN_LIGHTUP: Final = "lightUp"
 FILL_PATTERN_LIGHTVERTICAL: Final = "lightVertical"
 FILL_PATTERN_MEDIUMGRAY: Final = "mediumGray"
 
 _GradientFillType: TypeAlias = Literal["linear", "path"]
 _FillsType: TypeAlias = Literal[
-    "none",
     "solid",
     "darkDown",
     "darkGray",
     "darkGrid",
     "darkHorizontal",
     "darkTrellis",
     "darkUp",
@@ -44,69 +48,71 @@
     "lightGrid",
     "lightHorizontal",
     "lightTrellis",
     "lightUp",
     "lightVertical",
     "mediumGray",
 ]
-fills: tuple[_FillsType, ...]
+fills: Final[tuple[_FillsType, ...]]
 
 class Fill(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     @classmethod
-    def from_tree(cls, el): ...
+    def from_tree(cls, el: Iterable[ABCSequence[_SupportsIterAndAttribAndTextAndTag]]) -> PatternFill | GradientFill | None: ...
 
 class PatternFill(Fill):
-    tagname: str
+    tagname: ClassVar[str]
     __elements__: ClassVar[tuple[str, ...]]
     patternType: NoneSet[_FillsType]
     fill_type: Alias
-    fgColor: Incomplete
+    fgColor: ColorDescriptor[Literal[False]]
     start_color: Alias
-    bgColor: Incomplete
+    bgColor: ColorDescriptor[Literal[False]]
     end_color: Alias
     def __init__(
         self,
-        patternType: Incomplete | None = None,
-        fgColor=...,
-        bgColor=...,
-        fill_type: Incomplete | None = None,
-        start_color: Incomplete | None = None,
-        end_color: Incomplete | None = None,
+        patternType: _FillsType | Literal["none"] | None = None,
+        fgColor: str | Color = ...,
+        bgColor: str | Color = ...,
+        fill_type: _FillsType | Literal["none"] | None = None,
+        start_color: str | Color | None = None,
+        end_color: str | Color | None = None,
     ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
+    def to_tree(self, tagname: Unused = None, idx: Unused = None) -> Element: ...  # type: ignore[override]
 
-DEFAULT_EMPTY_FILL: Incomplete
-DEFAULT_GRAY_FILL: Incomplete
+DEFAULT_EMPTY_FILL: Final[PatternFill]
+DEFAULT_GRAY_FILL: Final[PatternFill]
 
 class Stop(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     position: MinMax[float, Literal[False]]
     color: Incomplete
-    def __init__(self, color, position: _ConvertibleToFloat) -> None: ...
+    def __init__(self, color, position: ConvertibleToFloat) -> None: ...
 
 class StopList(Sequence):
     expected_type: type[Incomplete]
-    def __set__(self, obj, values) -> None: ...
+    def __set__(self, obj: Serialisable | Strict, values) -> None: ...
 
 class GradientFill(Fill):
-    tagname: str
+    tagname: ClassVar[str]
     type: Set[_GradientFillType]
     fill_type: Alias
     degree: Float[Literal[False]]
     left: Float[Literal[False]]
     right: Float[Literal[False]]
     top: Float[Literal[False]]
     bottom: Float[Literal[False]]
     stop: Incomplete
     def __init__(
         self,
         type: _GradientFillType = "linear",
-        degree: _ConvertibleToFloat = 0,
-        left: _ConvertibleToFloat = 0,
-        right: _ConvertibleToFloat = 0,
-        top: _ConvertibleToFloat = 0,
-        bottom: _ConvertibleToFloat = 0,
+        degree: ConvertibleToFloat = 0,
+        left: ConvertibleToFloat = 0,
+        right: ConvertibleToFloat = 0,
+        top: ConvertibleToFloat = 0,
+        bottom: ConvertibleToFloat = 0,
         stop=(),
     ) -> None: ...
-    def __iter__(self): ...
-    def to_tree(self, tagname: Incomplete | None = None, namespace: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
+    def __iter__(self) -> Iterator[tuple[str, str]]: ...
+    def to_tree(  # type: ignore[override]
+        self, tagname: Unused = None, namespace: Unused = None, idx: Unused = None
+    ) -> Element: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/fonts.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/protection.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,76 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal, overload
 
-from openpyxl.descriptors.base import Alias, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
-from openpyxl.descriptors.nested import (
-    NestedBool,
-    NestedFloat,
-    NestedInteger,
-    NestedMinMax,
-    NestedNoneSet,
-    NestedString,
-    _HasTagAndGet,
-    _NestedNoneSetParam,
-)
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
-_FontU: TypeAlias = Literal["single", "double", "singleAccounting", "doubleAccounting"]
-_FontVertAlign: TypeAlias = Literal["superscript", "subscript", "baseline"]
-_FontScheme: TypeAlias = Literal["major", "minor"]
+class _Protected:
+    @overload
+    def set_password(self, value: str = "", already_hashed: Literal[False] = False) -> None: ...
+    @overload
+    def set_password(self, value: str | None, already_hashed: Literal[True]) -> None: ...
+    @overload
+    def set_password(self, value: str | None = "", *, already_hashed: Literal[True]) -> None: ...
+    @property
+    def password(self) -> str | None: ...
+    @password.setter
+    def password(self, value: str) -> None: ...
 
-class Font(Serialisable):
-    UNDERLINE_DOUBLE: str
-    UNDERLINE_DOUBLE_ACCOUNTING: str
-    UNDERLINE_SINGLE: str
-    UNDERLINE_SINGLE_ACCOUNTING: str
-    name: NestedString[Literal[True]]
-    charset: NestedInteger[Literal[True]]
-    family: NestedMinMax[float, Literal[True]]
-    sz: NestedFloat[Literal[True]]
-    size: Alias
-    b: NestedBool[Literal[False]]
-    bold: Alias
-    i: NestedBool[Literal[False]]
-    italic: Alias
-    strike: NestedBool[Literal[True]]
-    strikethrough: Alias
-    outline: NestedBool[Literal[True]]
-    shadow: NestedBool[Literal[True]]
-    condense: NestedBool[Literal[True]]
-    extend: NestedBool[Literal[True]]
-    u: NestedNoneSet[_FontU]
-    underline: Alias
-    vertAlign: NestedNoneSet[_FontVertAlign]
-    color: Incomplete
-    scheme: NestedNoneSet[_FontScheme]
-    tagname: str
-    __elements__: ClassVar[tuple[str, ...]]
+class SheetProtection(Serialisable, _Protected):
+    tagname: ClassVar[str]
+    sheet: Bool[Literal[False]]
+    enabled: Alias
+    objects: Bool[Literal[False]]
+    scenarios: Bool[Literal[False]]
+    formatCells: Bool[Literal[False]]
+    formatColumns: Bool[Literal[False]]
+    formatRows: Bool[Literal[False]]
+    insertColumns: Bool[Literal[False]]
+    insertRows: Bool[Literal[False]]
+    insertHyperlinks: Bool[Literal[False]]
+    deleteColumns: Bool[Literal[False]]
+    deleteRows: Bool[Literal[False]]
+    selectLockedCells: Bool[Literal[False]]
+    selectUnlockedCells: Bool[Literal[False]]
+    sort: Bool[Literal[False]]
+    autoFilter: Bool[Literal[False]]
+    pivotTables: Bool[Literal[False]]
+    saltValue: Incomplete
+    spinCount: Integer[Literal[True]]
+    algorithmName: String[Literal[True]]
+    hashValue: Incomplete
+    __attrs__: ClassVar[tuple[str, ...]]
+    password: Incomplete
     def __init__(
         self,
-        name: object = None,
-        sz: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        b: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
-        i: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
-        charset: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
-        u: _NestedNoneSetParam[_FontU] = None,
-        strike: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        color: Incomplete | None = None,
-        scheme: _NestedNoneSetParam[_FontScheme] = None,
-        family: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
-        size: _HasTagAndGet[_ConvertibleToFloat] | _ConvertibleToFloat | None = None,
-        bold: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
-        italic: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
-        strikethrough: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
-        underline: _NestedNoneSetParam[_FontU] = None,
-        vertAlign: _NestedNoneSetParam[_FontVertAlign] = None,
-        outline: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        shadow: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        condense: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
-        extend: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        sheet: _ConvertibleToBool = False,
+        objects: _ConvertibleToBool = False,
+        scenarios: _ConvertibleToBool = False,
+        formatCells: _ConvertibleToBool = True,
+        formatRows: _ConvertibleToBool = True,
+        formatColumns: _ConvertibleToBool = True,
+        insertColumns: _ConvertibleToBool = True,
+        insertRows: _ConvertibleToBool = True,
+        insertHyperlinks: _ConvertibleToBool = True,
+        deleteColumns: _ConvertibleToBool = True,
+        deleteRows: _ConvertibleToBool = True,
+        selectLockedCells: _ConvertibleToBool = False,
+        selectUnlockedCells: _ConvertibleToBool = False,
+        sort: _ConvertibleToBool = True,
+        autoFilter: _ConvertibleToBool = True,
+        pivotTables: _ConvertibleToBool = True,
+        password: Incomplete | None = None,
+        algorithmName: str | None = None,
+        saltValue: Incomplete | None = None,
+        spinCount: ConvertibleToInt | None = None,
+        hashValue: Incomplete | None = None,
     ) -> None: ...
-    @classmethod
-    def from_tree(cls, node): ...
-
-DEFAULT_FONT: Incomplete
+    @overload
+    def set_password(self, value: str = "", already_hashed: Literal[False] = False) -> None: ...
+    @overload
+    def set_password(self, value: str | None, already_hashed: Literal[True]) -> None: ...
+    @overload
+    def set_password(self, value: str | None = "", *, already_hashed: Literal[True]) -> None: ...
+    def enable(self) -> None: ...
+    def disable(self) -> None: ...
+    def __bool__(self) -> bool: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/named_styles.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/named_styles.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from collections.abc import Iterator
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.alignment import Alignment
 from openpyxl.styles.borders import Border
+from openpyxl.styles.cell_style import CellStyle, StyleArray
 from openpyxl.styles.fills import Fill
 from openpyxl.styles.fonts import Font
 from openpyxl.styles.protection import Protection
+from openpyxl.workbook.workbook import Workbook
 
 class NamedStyle(Serialisable):
     font: Typed[Font, Literal[False]]
     fill: Typed[Fill, Literal[False]]
     border: Typed[Border, Literal[False]]
     alignment: Typed[Alignment, Literal[False]]
     number_format: Incomplete
@@ -28,58 +30,58 @@
         name: str = "Normal",
         font: Font | None = None,
         fill: Fill | None = None,
         border: Border | None = None,
         alignment: Alignment | None = None,
         number_format: Incomplete | None = None,
         protection: Protection | None = None,
-        builtinId: _ConvertibleToInt | None = None,
+        builtinId: ConvertibleToInt | None = None,
         hidden: _ConvertibleToBool | None = False,
         xfId: Unused = None,
     ) -> None: ...
     def __setattr__(self, attr: str, value) -> None: ...
-    def __iter__(self): ...
+    def __iter__(self) -> Iterator[tuple[str, str]]: ...
     @property
-    def xfId(self): ...
-    def bind(self, wb) -> None: ...
-    def as_tuple(self): ...
-    def as_xf(self): ...
-    def as_name(self): ...
+    def xfId(self) -> int | None: ...
+    def bind(self, wb: Workbook) -> None: ...
+    def as_tuple(self) -> StyleArray: ...
+    def as_xf(self) -> CellStyle: ...
+    def as_name(self) -> _NamedCellStyle: ...
 
-class NamedStyleList(list[Incomplete]):
+class NamedStyleList(list[NamedStyle]):
     @property
-    def names(self): ...
-    def __getitem__(self, key): ...
-    def append(self, style) -> None: ...
+    def names(self) -> list[str]: ...
+    def __getitem__(self, key: int | str) -> NamedStyle: ...  # type: ignore[override]
+    def append(self, style: NamedStyle) -> None: ...
 
 class _NamedCellStyle(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     xfId: Integer[Literal[False]]
     builtinId: Integer[Literal[True]]
     iLevel: Integer[Literal[True]]
     hidden: Bool[Literal[True]]
     customBuiltin: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         name: str,
-        xfId: _ConvertibleToInt,
-        builtinId: _ConvertibleToInt | None = None,
-        iLevel: _ConvertibleToInt | None = None,
+        xfId: ConvertibleToInt,
+        builtinId: ConvertibleToInt | None = None,
+        iLevel: ConvertibleToInt | None = None,
         hidden: _ConvertibleToBool | None = None,
         customBuiltin: _ConvertibleToBool | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class _NamedCellStyleList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     # Overwritten by property below
     # count: Integer
     cellStyle: Incomplete
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, cellStyle=()) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
     @property
-    def names(self): ...
+    def names(self) -> NamedStyleList: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/stylesheet.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/stylesheet.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal, TypeVar
+from typing_extensions import Self
+from zipfile import ZipFile
 
 from openpyxl.descriptors.base import Typed
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.descriptors.serialisable import Serialisable, _ChildSerialisableTreeElement
 from openpyxl.styles.cell_style import CellStyleList
 from openpyxl.styles.colors import ColorList
 from openpyxl.styles.named_styles import _NamedCellStyleList
 from openpyxl.styles.numbers import NumberFormatList
 from openpyxl.styles.table import TableStyleList
+from openpyxl.workbook.workbook import Workbook
+from openpyxl.xml.functions import Element
+
+_WorkbookT = TypeVar("_WorkbookT", bound=Workbook)
 
 class Stylesheet(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     numFmts: Typed[NumberFormatList, Literal[False]]
     fonts: Incomplete
     fills: Incomplete
     borders: Incomplete
     cellStyleXfs: Typed[CellStyleList, Literal[False]]
     cellXfs: Typed[CellStyleList, Literal[False]]
     cellStyles: Typed[_NamedCellStyleList, Literal[False]]
@@ -41,14 +46,14 @@
         cellStyles: _NamedCellStyleList | None = None,
         dxfs=(),
         tableStyles: TableStyleList | None = None,
         colors: ColorList | None = None,
         extLst: Unused = None,
     ) -> None: ...
     @classmethod
-    def from_tree(cls, node): ...
+    def from_tree(cls, node: _ChildSerialisableTreeElement) -> Self: ...
     @property
-    def custom_formats(self): ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    def custom_formats(self) -> dict[int, str]: ...
+    def to_tree(self, tagname: str | None = None, idx: Unused = None, namespace: str | None = None) -> Element: ...
 
-def apply_stylesheet(archive, wb): ...
-def write_stylesheet(wb): ...
+def apply_stylesheet(archive: ZipFile, wb: _WorkbookT) -> _WorkbookT | None: ...
+def write_stylesheet(wb: Workbook): ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/_writer.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/_writer.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from _typeshed import Incomplete
 
-def get_active_sheet(wb): ...
+from openpyxl.workbook.workbook import Workbook
+
+def get_active_sheet(wb: Workbook) -> int | None: ...
 
 class WorkbookWriter:
-    wb: Incomplete
+    wb: Workbook
     rels: Incomplete
     package: Incomplete
-    def __init__(self, wb) -> None: ...
+    def __init__(self, wb: Workbook) -> None: ...
     def write_properties(self) -> None: ...
     def write_worksheets(self) -> None: ...
     def write_refs(self) -> None: ...
     def write_names(self) -> None: ...
     def write_pivots(self) -> None: ...
     def write_views(self) -> None: ...
     def write(self): ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/defined_name.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/defined_name.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from _typeshed import Incomplete
+from _typeshed import ConvertibleToInt, Incomplete
 from collections import defaultdict
-from collections.abc import Generator
+from collections.abc import Generator, Iterator
 from re import Pattern
-from typing_extensions import Literal
+from typing import ClassVar, Final, Literal
 
 from openpyxl.descriptors import Sequence
-from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.formula.tokenizer import _TokenOperandSubtypes, _TokenTypesNotOperand
 
-RESERVED: frozenset[str]
-RESERVED_REGEX: Pattern[str]
+RESERVED: Final[frozenset[str]]
+RESERVED_REGEX: Final[Pattern[str]]
 
 class DefinedName(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     comment: String[Literal[True]]
     customMenu: String[Literal[True]]
     description: String[Literal[True]]
     help: String[Literal[True]]
     statusBar: String[Literal[True]]
     localSheetId: Integer[Literal[True]]
@@ -34,37 +35,37 @@
         self,
         name: str,
         comment: str | None = None,
         customMenu: str | None = None,
         description: str | None = None,
         help: str | None = None,
         statusBar: str | None = None,
-        localSheetId: _ConvertibleToInt | None = None,
+        localSheetId: ConvertibleToInt | None = None,
         hidden: _ConvertibleToBool | None = None,
         function: _ConvertibleToBool | None = None,
         vbProcedure: _ConvertibleToBool | None = None,
         xlm: _ConvertibleToBool | None = None,
-        functionGroupId: _ConvertibleToInt | None = None,
+        functionGroupId: ConvertibleToInt | None = None,
         shortcutKey: str | None = None,
         publishToServer: _ConvertibleToBool | None = None,
         workbookParameter: _ConvertibleToBool | None = None,
         attr_text: Incomplete | None = None,
     ) -> None: ...
     @property
-    def type(self): ...
+    def type(self) -> _TokenTypesNotOperand | _TokenOperandSubtypes: ...
     @property
-    def destinations(self) -> Generator[Incomplete, None, None]: ...
+    def destinations(self) -> Generator[tuple[str, str], None, None]: ...
     @property
-    def is_reserved(self): ...
+    def is_reserved(self) -> str | None: ...
     @property
-    def is_external(self): ...
-    def __iter__(self): ...
+    def is_external(self) -> bool: ...
+    def __iter__(self) -> Iterator[tuple[str, str]]: ...
 
 class DefinedNameDict(dict[str, DefinedName]):
     def add(self, value: DefinedName) -> None: ...
 
 class DefinedNameList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     definedName: Sequence
     def __init__(self, definedName=()) -> None: ...
     def by_sheet(self) -> defaultdict[int, DefinedNameDict]: ...
     def __len__(self) -> int: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_link/external.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/external_link/external.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,79 +1,81 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
+from zipfile import ZipFile
 
-from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.packaging.relationship import Relationship
+from openpyxl.xml.functions import Element
 
 _ExternalCellType: TypeAlias = Literal["b", "d", "n", "e", "s", "str", "inlineStr"]
 
 class ExternalCell(Serialisable):
     r: String[Literal[False]]
     t: NoneSet[_ExternalCellType]
     vm: Integer[Literal[True]]
     v: NestedText[str, Literal[True]]
     def __init__(
-        self, r: str, t: _ExternalCellType | Literal["none"] | None = None, vm: _ConvertibleToInt | None = None, v: object = None
+        self, r: str, t: _ExternalCellType | Literal["none"] | None = None, vm: ConvertibleToInt | None = None, v: object = None
     ) -> None: ...
 
 class ExternalRow(Serialisable):
     r: Integer[Literal[False]]
     cell: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, r: _ConvertibleToInt, cell: Incomplete | None = None) -> None: ...
+    def __init__(self, r: ConvertibleToInt, cell: Incomplete | None = None) -> None: ...
 
 class ExternalSheetData(Serialisable):
     sheetId: Integer[Literal[False]]
     refreshError: Bool[Literal[True]]
     row: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, sheetId: _ConvertibleToInt, refreshError: _ConvertibleToBool | None = None, row=()) -> None: ...
+    def __init__(self, sheetId: ConvertibleToInt, refreshError: _ConvertibleToBool | None = None, row=()) -> None: ...
 
 class ExternalSheetDataSet(Serialisable):
     sheetData: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, sheetData: Incomplete | None = None) -> None: ...
 
 class ExternalSheetNames(Serialisable):
     sheetName: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, sheetName=()) -> None: ...
 
 class ExternalDefinedName(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     refersTo: String[Literal[True]]
     sheetId: Integer[Literal[True]]
-    def __init__(self, name: str, refersTo: str | None = None, sheetId: _ConvertibleToInt | None = None) -> None: ...
+    def __init__(self, name: str, refersTo: str | None = None, sheetId: ConvertibleToInt | None = None) -> None: ...
 
 class ExternalBook(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     sheetNames: Typed[ExternalSheetNames, Literal[True]]
     definedNames: Incomplete
     sheetDataSet: Typed[ExternalSheetDataSet, Literal[True]]
     id: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         sheetNames: ExternalSheetNames | None = None,
         definedNames=(),
         sheetDataSet: ExternalSheetDataSet | None = None,
         id: Incomplete | None = None,
     ) -> None: ...
 
 class ExternalLink(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     mime_type: str
     externalBook: Typed[ExternalBook, Literal[True]]
     file_link: Typed[Relationship, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, externalBook: ExternalBook | None = None, ddeLink: Unused = None, oleLink: Unused = None, extLst: Unused = None
     ) -> None: ...
-    def to_tree(self): ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
     @property
-    def path(self): ...
+    def path(self) -> str: ...
 
-def read_external_link(archive, book_path): ...
+def read_external_link(archive: ZipFile, book_path: str) -> ExternalLink: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/function_group.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/function_group.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors.base import Integer, String, _ConvertibleToInt
+from openpyxl.descriptors.base import Integer, String
 from openpyxl.descriptors.serialisable import Serialisable
 
 class FunctionGroup(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     def __init__(self, name: str) -> None: ...
 
 class FunctionGroupList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     builtInGroupCount: Integer[Literal[True]]
     functionGroup: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, builtInGroupCount: _ConvertibleToInt | None = 16, functionGroup=()) -> None: ...
+    def __init__(self, builtInGroupCount: ConvertibleToInt | None = 16, functionGroup=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/properties.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/properties.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-from _typeshed import Incomplete
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import (
-    Bool,
-    Float,
-    Integer,
-    NoneSet,
-    String,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from openpyxl.descriptors.base import Bool, Float, Integer, NoneSet, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 _WorkbookPropertiesShowObjects: TypeAlias = Literal["all", "placeholders"]
 _WorkbookPropertiesUpdateLinks: TypeAlias = Literal["userSet", "never", "always"]
 _CalcPropertiesCalcMode: TypeAlias = Literal["manual", "auto", "autoNoTable"]
 _CalcPropertiesRefMode: TypeAlias = Literal["A1", "R1C1"]
 
 class WorkbookProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     date1904: Bool[Literal[True]]
     dateCompatibility: Bool[Literal[True]]
     showObjects: NoneSet[_WorkbookPropertiesShowObjects]
     showBorderUnselectedTables: Bool[Literal[True]]
     filterPrivacy: Bool[Literal[True]]
     promptedSolutions: Bool[Literal[True]]
     showInkAnnotation: Bool[Literal[True]]
@@ -55,19 +47,19 @@
         hidePivotFieldList: _ConvertibleToBool | None = None,
         showPivotChartFilter: _ConvertibleToBool | None = None,
         allowRefreshQuery: _ConvertibleToBool | None = None,
         publishItems: _ConvertibleToBool | None = None,
         checkCompatibility: _ConvertibleToBool | None = None,
         autoCompressPictures: _ConvertibleToBool | None = None,
         refreshAllConnections: _ConvertibleToBool | None = None,
-        defaultThemeVersion: _ConvertibleToInt | None = None,
+        defaultThemeVersion: ConvertibleToInt | None = None,
     ) -> None: ...
 
 class CalcProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     calcId: Integer[Literal[False]]
     calcMode: NoneSet[_CalcPropertiesCalcMode]
     fullCalcOnLoad: Bool[Literal[True]]
     refMode: NoneSet[_CalcPropertiesRefMode]
     iterate: Bool[Literal[True]]
     iterateCount: Integer[Literal[True]]
     iterateDelta: Float[Literal[True]]
@@ -75,31 +67,31 @@
     calcCompleted: Bool[Literal[True]]
     calcOnSave: Bool[Literal[True]]
     concurrentCalc: Bool[Literal[True]]
     concurrentManualCount: Integer[Literal[True]]
     forceFullCalc: Bool[Literal[True]]
     def __init__(
         self,
-        calcId: _ConvertibleToInt = 124519,
+        calcId: ConvertibleToInt = 124519,
         calcMode: _CalcPropertiesCalcMode | Literal["none"] | None = None,
         fullCalcOnLoad: _ConvertibleToBool | None = True,
         refMode: _CalcPropertiesRefMode | Literal["none"] | None = None,
         iterate: _ConvertibleToBool | None = None,
-        iterateCount: _ConvertibleToInt | None = None,
-        iterateDelta: _ConvertibleToFloat | None = None,
+        iterateCount: ConvertibleToInt | None = None,
+        iterateDelta: ConvertibleToFloat | None = None,
         fullPrecision: _ConvertibleToBool | None = None,
         calcCompleted: _ConvertibleToBool | None = None,
         calcOnSave: _ConvertibleToBool | None = None,
         concurrentCalc: _ConvertibleToBool | None = None,
-        concurrentManualCount: _ConvertibleToInt | None = None,
+        concurrentManualCount: ConvertibleToInt | None = None,
         forceFullCalc: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class FileVersion(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     appName: String[Literal[True]]
     lastEdited: String[Literal[True]]
     lowestEdited: String[Literal[True]]
     rupBuild: String[Literal[True]]
     codeName: Incomplete
     def __init__(
         self,
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/protection.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/protection.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal, overload
+from typing_extensions import Self
 
-from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..xml._functions_overloads import _SupportsIterAndAttribAndTextAndGet
+
 class WorkbookProtection(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     workbook_password: Alias
     workbookPasswordCharacterSet: String[Literal[True]]
     revision_password: Alias
     revisionsPasswordCharacterSet: String[Literal[True]]
     lockStructure: Bool[Literal[True]]
     lock_structure: Alias
     lockWindows: Bool[Literal[True]]
@@ -34,37 +36,47 @@
         revisionsPasswordCharacterSet: str | None = None,
         lockStructure: _ConvertibleToBool | None = None,
         lockWindows: _ConvertibleToBool | None = None,
         lockRevision: _ConvertibleToBool | None = None,
         revisionsAlgorithmName: str | None = None,
         revisionsHashValue: Incomplete | None = None,
         revisionsSaltValue: Incomplete | None = None,
-        revisionsSpinCount: _ConvertibleToInt | None = None,
+        revisionsSpinCount: ConvertibleToInt | None = None,
         workbookAlgorithmName: str | None = None,
         workbookHashValue: Incomplete | None = None,
         workbookSaltValue: Incomplete | None = None,
-        workbookSpinCount: _ConvertibleToInt | None = None,
+        workbookSpinCount: ConvertibleToInt | None = None,
     ) -> None: ...
-    def set_workbook_password(self, value: str = "", already_hashed: bool = False) -> None: ...
+    @overload
+    def set_workbook_password(self, value: str = "", already_hashed: Literal[False] = False) -> None: ...
+    @overload
+    def set_workbook_password(self, value: str | None, already_hashed: Literal[True]) -> None: ...
+    @overload
+    def set_workbook_password(self, value: str | None = "", *, already_hashed: Literal[True]) -> None: ...
     @property
-    def workbookPassword(self): ...
+    def workbookPassword(self) -> str | None: ...
     @workbookPassword.setter
-    def workbookPassword(self, value) -> None: ...
-    def set_revisions_password(self, value: str = "", already_hashed: bool = False) -> None: ...
+    def workbookPassword(self, value: str) -> None: ...
+    @overload
+    def set_revisions_password(self, value: str = "", already_hashed: Literal[False] = False) -> None: ...
+    @overload
+    def set_revisions_password(self, value: str | None, already_hashed: Literal[True]) -> None: ...
+    @overload
+    def set_revisions_password(self, value: str | None = "", *, already_hashed: Literal[True]) -> None: ...
     @property
-    def revisionsPassword(self): ...
+    def revisionsPassword(self) -> str | None: ...
     @revisionsPassword.setter
-    def revisionsPassword(self, value) -> None: ...
+    def revisionsPassword(self, value: str) -> None: ...
     @classmethod
-    def from_tree(cls, node): ...
+    def from_tree(cls, node: _SupportsIterAndAttribAndTextAndGet) -> Self: ...
 
 DocumentSecurity = WorkbookProtection
 
 class FileSharing(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     readOnlyRecommended: Bool[Literal[True]]
     userName: String[Literal[True]]
     reservationPassword: Incomplete
     algorithmName: String[Literal[True]]
     hashValue: Incomplete
     saltValue: Incomplete
     spinCount: Integer[Literal[True]]
@@ -72,9 +84,9 @@
         self,
         readOnlyRecommended: _ConvertibleToBool | None = None,
         userName: str | None = None,
         reservationPassword: Incomplete | None = None,
         algorithmName: str | None = None,
         hashValue: Incomplete | None = None,
         saltValue: Incomplete | None = None,
-        spinCount: _ConvertibleToInt | None = None,
+        spinCount: ConvertibleToInt | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/smart_tags.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/smart_tags.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
 
 from openpyxl.descriptors.base import Bool, NoneSet, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 _SmartTagPropertiesShow: TypeAlias = Literal["all", "noIndicator"]
 
 class SmartTag(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     namespaceUri: String[Literal[True]]
     name: String[Literal[True]]
     url: String[Literal[True]]
     def __init__(self, namespaceUri: str | None = None, name: str | None = None, url: str | None = None) -> None: ...
 
 class SmartTagList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     smartTagType: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, smartTagType=()) -> None: ...
 
 class SmartTagProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     embed: Bool[Literal[True]]
     show: NoneSet[_SmartTagPropertiesShow]
     def __init__(
         self, embed: _ConvertibleToBool | None = None, show: _SmartTagPropertiesShow | Literal["none"] | None = None
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/views.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/views.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl import _VisibilityType
+from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-_BookViewVilibility: TypeAlias = Literal["visible", "hidden", "veryHidden"]
 _CustomWorkbookViewShowComments: TypeAlias = Literal["commNone", "commIndicator", "commIndAndComment"]
 _CustomWorkbookViewShowObjects: TypeAlias = Literal["all", "placeholders"]
 
 class BookView(Serialisable):
-    tagname: str
-    visibility: NoneSet[_BookViewVilibility]
+    tagname: ClassVar[str]
+    visibility: NoneSet[_VisibilityType]
     minimized: Bool[Literal[True]]
     showHorizontalScroll: Bool[Literal[True]]
     showVerticalScroll: Bool[Literal[True]]
     showSheetTabs: Bool[Literal[True]]
     xWindow: Integer[Literal[True]]
     yWindow: Integer[Literal[True]]
     windowWidth: Integer[Literal[True]]
@@ -25,32 +25,32 @@
     firstSheet: Integer[Literal[True]]
     activeTab: Integer[Literal[True]]
     autoFilterDateGrouping: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        visibility: _BookViewVilibility | Literal["none"] | None = "visible",
+        visibility: _VisibilityType | Literal["none"] | None = "visible",
         minimized: _ConvertibleToBool | None = False,
         showHorizontalScroll: _ConvertibleToBool | None = True,
         showVerticalScroll: _ConvertibleToBool | None = True,
         showSheetTabs: _ConvertibleToBool | None = True,
-        xWindow: _ConvertibleToInt | None = None,
-        yWindow: _ConvertibleToInt | None = None,
-        windowWidth: _ConvertibleToInt | None = None,
-        windowHeight: _ConvertibleToInt | None = None,
-        tabRatio: _ConvertibleToInt | None = 600,
-        firstSheet: _ConvertibleToInt | None = 0,
-        activeTab: _ConvertibleToInt | None = 0,
+        xWindow: ConvertibleToInt | None = None,
+        yWindow: ConvertibleToInt | None = None,
+        windowWidth: ConvertibleToInt | None = None,
+        windowHeight: ConvertibleToInt | None = None,
+        tabRatio: ConvertibleToInt | None = 600,
+        firstSheet: ConvertibleToInt | None = 0,
+        activeTab: ConvertibleToInt | None = 0,
         autoFilterDateGrouping: _ConvertibleToBool | None = True,
         extLst: Unused = None,
     ) -> None: ...
 
 class CustomWorkbookView(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[False]]
     guid: Incomplete
     autoUpdate: Bool[Literal[True]]
     mergeInterval: Integer[Literal[True]]
     changesSavedWin: Bool[Literal[True]]
     onlySync: Bool[Literal[True]]
     personalView: Bool[Literal[True]]
@@ -75,60 +75,60 @@
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         name: str,
         guid: Incomplete | None = None,
         autoUpdate: _ConvertibleToBool | None = None,
-        mergeInterval: _ConvertibleToInt | None = None,
+        mergeInterval: ConvertibleToInt | None = None,
         changesSavedWin: _ConvertibleToBool | None = None,
         onlySync: _ConvertibleToBool | None = None,
         personalView: _ConvertibleToBool | None = None,
         includePrintSettings: _ConvertibleToBool | None = None,
         includeHiddenRowCol: _ConvertibleToBool | None = None,
         maximized: _ConvertibleToBool | None = None,
         minimized: _ConvertibleToBool | None = None,
         showHorizontalScroll: _ConvertibleToBool | None = None,
         showVerticalScroll: _ConvertibleToBool | None = None,
         showSheetTabs: _ConvertibleToBool | None = None,
         *,
-        xWindow: _ConvertibleToInt,
-        yWindow: _ConvertibleToInt,
-        windowWidth: _ConvertibleToInt,
-        windowHeight: _ConvertibleToInt,
-        tabRatio: _ConvertibleToInt | None = None,
-        activeSheetId: _ConvertibleToInt,
+        xWindow: ConvertibleToInt,
+        yWindow: ConvertibleToInt,
+        windowWidth: ConvertibleToInt,
+        windowHeight: ConvertibleToInt,
+        tabRatio: ConvertibleToInt | None = None,
+        activeSheetId: ConvertibleToInt,
         showFormulaBar: _ConvertibleToBool | None = None,
         showStatusbar: _ConvertibleToBool | None = None,
         showComments: _CustomWorkbookViewShowComments | Literal["none"] | None = "commIndicator",
         showObjects: _CustomWorkbookViewShowObjects | Literal["none"] | None = "all",
         extLst: Unused = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         name: str,
         guid: Incomplete | None,
         autoUpdate: _ConvertibleToBool | None,
-        mergeInterval: _ConvertibleToInt | None,
+        mergeInterval: ConvertibleToInt | None,
         changesSavedWin: _ConvertibleToBool | None,
         onlySync: _ConvertibleToBool | None,
         personalView: _ConvertibleToBool | None,
         includePrintSettings: _ConvertibleToBool | None,
         includeHiddenRowCol: _ConvertibleToBool | None,
         maximized: _ConvertibleToBool | None,
         minimized: _ConvertibleToBool | None,
         showHorizontalScroll: _ConvertibleToBool | None,
         showVerticalScroll: _ConvertibleToBool | None,
         showSheetTabs: _ConvertibleToBool | None,
-        xWindow: _ConvertibleToInt,
-        yWindow: _ConvertibleToInt,
-        windowWidth: _ConvertibleToInt,
-        windowHeight: _ConvertibleToInt,
-        tabRatio: _ConvertibleToInt | None,
-        activeSheetId: _ConvertibleToInt,
+        xWindow: ConvertibleToInt,
+        yWindow: ConvertibleToInt,
+        windowWidth: ConvertibleToInt,
+        windowHeight: ConvertibleToInt,
+        tabRatio: ConvertibleToInt | None,
+        activeSheetId: ConvertibleToInt,
         showFormulaBar: _ConvertibleToBool | None = None,
         showStatusbar: _ConvertibleToBool | None = None,
         showComments: _CustomWorkbookViewShowComments | Literal["none"] | None = "commIndicator",
         showObjects: _CustomWorkbookViewShowObjects | Literal["none"] | None = "all",
         extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/web.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/workbook/web.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 _WebPublishingTargetScreenSize: TypeAlias = Literal[
     "544x376",
     "640x480",
     "720x512",
     "800x600",
@@ -16,55 +16,55 @@
     "1280x1024",
     "1600x1200",
     "1800x1440",
     "1920x1200",
 ]
 
 class WebPublishObject(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     id: Integer[Literal[False]]
     divId: String[Literal[False]]
     sourceObject: String[Literal[True]]
     destinationFile: String[Literal[False]]
     title: String[Literal[True]]
     autoRepublish: Bool[Literal[True]]
     @overload
     def __init__(
         self,
-        id: _ConvertibleToInt,
+        id: ConvertibleToInt,
         divId: str,
         sourceObject: str | None = None,
         *,
         destinationFile: str,
         title: str | None = None,
         autoRepublish: _ConvertibleToBool | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        id: _ConvertibleToInt,
+        id: ConvertibleToInt,
         divId: str,
         sourceObject: str | None,
         destinationFile: str,
         title: str | None = None,
         autoRepublish: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class WebPublishObjectList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     # Overwritten by property below
     # count: Integer
     webPublishObject: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, webPublishObject=()) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
 
 class WebPublishing(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     css: Bool[Literal[True]]
     thicket: Bool[Literal[True]]
     longFileNames: Bool[Literal[True]]
     vml: Bool[Literal[True]]
     allowPng: Bool[Literal[True]]
     targetScreenSize: NoneSet[_WebPublishingTargetScreenSize]
     dpi: Integer[Literal[True]]
@@ -74,11 +74,11 @@
         self,
         css: _ConvertibleToBool | None = None,
         thicket: _ConvertibleToBool | None = None,
         longFileNames: _ConvertibleToBool | None = None,
         vml: _ConvertibleToBool | None = None,
         allowPng: _ConvertibleToBool | None = None,
         targetScreenSize: _WebPublishingTargetScreenSize | Literal["none"] | None = "800x600",
-        dpi: _ConvertibleToInt | None = None,
-        codePage: _ConvertibleToInt | None = None,
+        dpi: ConvertibleToInt | None = None,
+        codePage: ConvertibleToInt | None = None,
         characterSet: str | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/workbook.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/cell/cell.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,99 @@
-from _typeshed import Incomplete, StrPath
-from collections.abc import Iterator
+from _typeshed import ReadableBuffer
 from datetime import datetime
-from typing import IO
+from re import Pattern
+from typing import Final, Literal, overload
 
-from openpyxl.chartsheet.chartsheet import Chartsheet
-from openpyxl.styles.named_styles import NamedStyle
+from openpyxl.cell import _CellValue, _TimeTypes
+from openpyxl.comments.comments import Comment
+from openpyxl.compat.numbers import NUMERIC_TYPES as NUMERIC_TYPES  # cell numeric types
+from openpyxl.styles.cell_style import StyleArray
+from openpyxl.styles.styleable import StyleableObject
 from openpyxl.workbook.child import _WorkbookChild
-from openpyxl.worksheet._write_only import WriteOnlyWorksheet
-from openpyxl.worksheet.worksheet import Worksheet
+from openpyxl.worksheet._read_only import ReadOnlyWorksheet
+from openpyxl.worksheet.hyperlink import Hyperlink
 
-INTEGER_TYPES: Incomplete
+__docformat__: Final = "restructuredtext en"
+TIME_TYPES: Final[tuple[type, ...]]
+TIME_FORMATS: Final[dict[type[_TimeTypes], str]]
+STRING_TYPES: Final[tuple[type, ...]]
+KNOWN_TYPES: Final[tuple[type, ...]]
 
-class Workbook:
-    template: bool
-    path: str
-    defined_names: Incomplete
-    properties: Incomplete
-    security: Incomplete
-    shared_strings: Incomplete
-    loaded_theme: Incomplete
-    vba_archive: Incomplete
-    is_template: bool
-    code_name: Incomplete
-    encoding: str
-    iso_dates: Incomplete
-    rels: Incomplete
-    calculation: Incomplete
-    views: Incomplete
-    def __init__(self, write_only: bool = False, iso_dates: bool = False) -> None: ...
-    @property
-    def epoch(self) -> datetime: ...
-    @epoch.setter
-    def epoch(self, value: datetime) -> None: ...
-    @property
-    def read_only(self) -> bool: ...
-    @property
-    def data_only(self) -> bool: ...
-    @property
-    def write_only(self) -> bool: ...
-    @property
-    def excel_base_date(self) -> datetime: ...
-    @property
-    def active(self) -> _WorkbookChild | None: ...
-    @active.setter
-    def active(self, value: _WorkbookChild | int) -> None: ...
-    def create_sheet(self, title: str | None = None, index: int | None = None): ...
-    def move_sheet(self, sheet: Worksheet | str, offset: int = 0) -> None: ...
-    def remove(self, worksheet: Worksheet) -> None: ...
-    def remove_sheet(self, worksheet: Worksheet) -> None: ...
-    def create_chartsheet(self, title: str | None = None, index: int | None = None) -> Chartsheet: ...
-    def get_sheet_by_name(self, name: str) -> Worksheet: ...
-    def __contains__(self, key: str) -> bool: ...
-    def index(self, worksheet: Worksheet) -> int: ...
-    def get_index(self, worksheet: Worksheet) -> int: ...
-    def __getitem__(self, key: str) -> Worksheet: ...
-    def __delitem__(self, key: str) -> None: ...
-    def __iter__(self) -> Iterator[Worksheet]: ...
-    def get_sheet_names(self) -> list[Worksheet]: ...
+ILLEGAL_CHARACTERS_RE: Final[Pattern[str]]
+ERROR_CODES: Final[tuple[str, ...]]
+
+TYPE_STRING: Final = "s"
+TYPE_FORMULA: Final = "f"
+TYPE_NUMERIC: Final = "n"
+TYPE_BOOL: Final = "b"
+TYPE_NULL: Final = "n"
+TYPE_INLINE: Final = "inlineStr"
+TYPE_ERROR: Final = "e"
+TYPE_FORMULA_CACHE_STRING: Final = "str"
+
+VALID_TYPES: Final[tuple[str, ...]]
+
+def get_type(t: type, value: object) -> Literal["n", "s", "d", "f"] | None: ...
+def get_time_format(t: _TimeTypes) -> str: ...
+
+class Cell(StyleableObject):
+    row: int
+    column: int
+    data_type: str
+    # row and column are never meant to be None and would lead to errors
+    def __init__(
+        self,
+        worksheet: _WorkbookChild | ReadOnlyWorksheet,
+        row: int,
+        column: int,
+        value: str | float | datetime | None = None,
+        style_array: StyleArray | None = None,
+    ) -> None: ...
     @property
-    def worksheets(self) -> list[Worksheet]: ...
+    def coordinate(self) -> str: ...
     @property
-    def chartsheets(self) -> list[Chartsheet]: ...
+    def col_idx(self) -> int: ...
     @property
-    def sheetnames(self) -> list[str]: ...
-    def create_named_range(
-        self,
-        name: str,
-        worksheet: Worksheet | None = None,
-        value: str | Incomplete | None = None,
-        scope: Incomplete | None = None,
-    ) -> None: ...
-    def add_named_style(self, style: NamedStyle) -> None: ...
+    def column_letter(self) -> str: ...
     @property
-    def named_styles(self) -> list[str]: ...
+    def encoding(self) -> str: ...
     @property
-    def mime_type(self) -> str: ...
-    def save(self, filename: StrPath | IO[bytes]) -> None: ...
+    def base_date(self) -> datetime: ...
+    @overload
+    def check_string(self, value: None) -> None: ...
+    @overload
+    def check_string(self, value: str | ReadableBuffer) -> str: ...
+    def check_error(self, value: object) -> str: ...
     @property
-    def style_names(self) -> list[str]: ...
-    def copy_worksheet(self, from_worksheet: Worksheet) -> Worksheet | WriteOnlyWorksheet: ...
-    def close(self) -> None: ...
+    def value(self) -> _CellValue | None: ...
+    @value.setter
+    def value(self, value: _CellValue | bytes | None) -> None: ...
+    @property
+    def internal_value(self) -> _CellValue | None: ...
+    @property
+    def hyperlink(self) -> Hyperlink | None: ...
+    @hyperlink.setter
+    def hyperlink(self, val: Hyperlink | str | None) -> None: ...
+    @property
+    def is_date(self) -> bool: ...
+    def offset(self, row: int = 0, column: int = 0) -> Cell: ...
+    @property
+    def comment(self) -> Comment | None: ...
+    @comment.setter
+    def comment(self, value: Comment | None) -> None: ...
+
+class MergedCell(StyleableObject):
+    data_type: str
+    comment: Comment | None
+    hyperlink: Hyperlink | None
+    row: int | None
+    column: int | None
+    def __init__(
+        self, worksheet: _WorkbookChild | ReadOnlyWorksheet, row: int | None = None, column: int | None = None
+    ) -> None: ...
+    # Same as Cell.coordinate
+    # https://github.com/python/mypy/issues/6700
+    @property
+    def coordinate(self) -> str: ...
+    value: str | float | int | datetime | None
+
+def WriteOnlyCell(ws: _WorkbookChild | ReadOnlyWorksheet, value: str | float | datetime | None = None) -> Cell: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/cell_range.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/cell_range.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,104 @@
-from _typeshed import Incomplete, Unused
-from collections.abc import Generator
-from typing import overload
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete
+from collections.abc import Generator, Iterator
+from itertools import product
+from typing import Any, Literal, overload
 
 from openpyxl.descriptors import Strict
-from openpyxl.descriptors.base import MinMax, _ConvertibleToInt
+from openpyxl.descriptors.base import MinMax
 from openpyxl.descriptors.serialisable import Serialisable
 
 class CellRange(Serialisable):
     min_col: MinMax[int, Literal[False]]
     min_row: MinMax[int, Literal[False]]
     max_col: MinMax[int, Literal[False]]
     max_row: MinMax[int, Literal[False]]
-    title: Incomplete
+    title: str | None
 
+    # With `range_string`, min/max parameters go unused.
+    # Enforcing `None` to avoid confusion upon which params get used
+    # if the user still tries to pass a `ConvertibleToInt`.
     @overload
     def __init__(
         self,
-        range_string: Incomplete,
-        min_col: Unused = None,
-        min_row: Unused = None,
-        max_col: Unused = None,
-        max_row: Unused = None,
-        title: Incomplete | None = None,
+        range_string: str,
+        min_col: None = None,
+        min_row: None = None,
+        max_col: None = None,
+        max_row: None = None,
+        title: str | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         range_string: None = None,
         *,
-        min_col: _ConvertibleToInt,
-        min_row: _ConvertibleToInt,
-        max_col: _ConvertibleToInt,
-        max_row: _ConvertibleToInt,
-        title: Incomplete | None = None,
+        min_col: ConvertibleToInt,
+        min_row: ConvertibleToInt,
+        max_col: ConvertibleToInt,
+        max_row: ConvertibleToInt,
+        title: str | None = None,
+    ) -> None: ...
+    @overload
+    def __init__(
+        self,
+        range_string: None,
+        min_col: ConvertibleToInt,
+        min_row: ConvertibleToInt,
+        max_col: ConvertibleToInt,
+        max_row: ConvertibleToInt,
+        title: str | None = None,
     ) -> None: ...
     @property
-    def bounds(self): ...
+    def bounds(self) -> tuple[int, int, int, int]: ...
     @property
-    def coord(self): ...
+    def coord(self) -> str: ...
     @property
-    def rows(self) -> Generator[Incomplete, None, None]: ...
+    def rows(self) -> Generator[list[tuple[int, int]], None, None]: ...
     @property
-    def cols(self) -> Generator[Incomplete, None, None]: ...
+    def cols(self) -> Generator[list[tuple[int, int]], None, None]: ...
     @property
-    def cells(self): ...
+    def cells(self) -> product[tuple[int, int]]: ...
     def __copy__(self): ...
     def shift(self, col_shift: int = 0, row_shift: int = 0) -> None: ...
-    def __ne__(self, other): ...
-    def __eq__(self, other): ...
-    def issubset(self, other): ...
-    __le__: Incomplete
-    def __lt__(self, other): ...
-    def issuperset(self, other): ...
-    __ge__: Incomplete
-    def __contains__(self, coord): ...
-    def __gt__(self, other): ...
-    def isdisjoint(self, other): ...
+    def __ne__(self, other: object) -> bool: ...
+    def __eq__(self, other: object) -> bool: ...
+    def issubset(self, other: CellRange) -> bool: ...
+    __le__ = issubset
+    def __lt__(self, other: CellRange) -> bool: ...
+    def issuperset(self, other: CellRange) -> bool: ...
+    __ge__ = issuperset
+    def __contains__(self, coord: str) -> bool: ...
+    def __gt__(self, other: CellRange) -> bool: ...
+    def isdisjoint(self, other: CellRange) -> bool: ...
     def intersection(self, other): ...
-    __and__: Incomplete
+    __and__ = intersection
     def union(self, other): ...
-    __or__: Incomplete
-    def __iter__(self): ...
+    __or__ = union
+    # Iterates over class attributes. Value could be anything.
+    def __iter__(self) -> Iterator[tuple[str, Any]]: ...
     def expand(self, right: int = 0, down: int = 0, left: int = 0, up: int = 0) -> None: ...
     def shrink(self, right: int = 0, bottom: int = 0, left: int = 0, top: int = 0) -> None: ...
     @property
-    def size(self): ...
+    def size(self) -> dict[str, int]: ...
     @property
-    def top(self): ...
+    def top(self) -> list[tuple[int, int]]: ...
     @property
-    def bottom(self): ...
+    def bottom(self) -> list[tuple[int, int]]: ...
     @property
-    def left(self): ...
+    def left(self) -> list[tuple[int, int]]: ...
     @property
-    def right(self): ...
+    def right(self) -> list[tuple[int, int]]: ...
 
 class MultiCellRange(Strict):
     ranges: Incomplete
     def __init__(self, ranges=...) -> None: ...
-    def __contains__(self, coord): ...
+    def __contains__(self, coord: str | CellRange) -> bool: ...
+    def sorted(self) -> list[CellRange]: ...
     def add(self, coord) -> None: ...
     def __iadd__(self, coord): ...
-    def __eq__(self, other): ...
-    def __ne__(self, other): ...
+    def __eq__(self, other: str | MultiCellRange) -> bool: ...  # type: ignore[override]
+    def __ne__(self, other: str | MultiCellRange) -> bool: ...  # type: ignore[override]
     def __bool__(self) -> bool: ...
     def remove(self, coord) -> None: ...
-    def __iter__(self): ...
+    def __iter__(self) -> Iterator[CellRange]: ...
     def __copy__(self): ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/controls.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/properties.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,56 @@
-from _typeshed import Incomplete
-from typing import ClassVar, overload
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
-from openpyxl.descriptors.base import Bool, Integer, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.worksheet.ole import ObjectAnchor
+from openpyxl.styles.colors import Color, ColorDescriptor
 
-class ControlProperty(Serialisable):
-    tagname: str
-    anchor: Typed[ObjectAnchor, Literal[False]]
-    locked: Bool[Literal[True]]
-    defaultSize: Bool[Literal[True]]
-    _print: Bool[Literal[True]]  # Not private. Avoids name clash
-    disabled: Bool[Literal[True]]
-    recalcAlways: Bool[Literal[True]]
-    uiObject: Bool[Literal[True]]
-    autoFill: Bool[Literal[True]]
-    autoLine: Bool[Literal[True]]
-    autoPict: Bool[Literal[True]]
-    macro: String[Literal[True]]
-    altText: String[Literal[True]]
-    linkedCell: String[Literal[True]]
-    listFillRange: String[Literal[True]]
-    cf: String[Literal[True]]
-    id: Incomplete
-    __elements__: ClassVar[tuple[str, ...]]
+class Outline(Serialisable):
+    tagname: ClassVar[str]
+    applyStyles: Bool[Literal[True]]
+    summaryBelow: Bool[Literal[True]]
+    summaryRight: Bool[Literal[True]]
+    showOutlineSymbols: Bool[Literal[True]]
     def __init__(
         self,
-        anchor: ObjectAnchor,
-        locked: _ConvertibleToBool | None = True,
-        defaultSize: _ConvertibleToBool | None = True,
-        _print: _ConvertibleToBool | None = True,
-        disabled: _ConvertibleToBool | None = False,
-        recalcAlways: _ConvertibleToBool | None = False,
-        uiObject: _ConvertibleToBool | None = False,
-        autoFill: _ConvertibleToBool | None = True,
-        autoLine: _ConvertibleToBool | None = True,
-        autoPict: _ConvertibleToBool | None = True,
-        macro: str | None = None,
-        altText: str | None = None,
-        linkedCell: str | None = None,
-        listFillRange: str | None = None,
-        cf: str | None = "pict",
-        id: Incomplete | None = None,
+        applyStyles: _ConvertibleToBool | None = None,
+        summaryBelow: _ConvertibleToBool | None = None,
+        summaryRight: _ConvertibleToBool | None = None,
+        showOutlineSymbols: _ConvertibleToBool | None = None,
     ) -> None: ...
 
-class Control(Serialisable):
-    tagname: str
-    controlPr: Typed[ControlProperty, Literal[True]]
-    shapeId: Integer[Literal[False]]
-    name: String[Literal[True]]
+class PageSetupProperties(Serialisable):
+    tagname: ClassVar[str]
+    autoPageBreaks: Bool[Literal[True]]
+    fitToPage: Bool[Literal[True]]
+    def __init__(self, autoPageBreaks: _ConvertibleToBool | None = None, fitToPage: _ConvertibleToBool | None = None) -> None: ...
+
+class WorksheetProperties(Serialisable):
+    tagname: ClassVar[str]
+    codeName: String[Literal[True]]
+    enableFormatConditionsCalculation: Bool[Literal[True]]
+    filterMode: Bool[Literal[True]]
+    published: Bool[Literal[True]]
+    syncHorizontal: Bool[Literal[True]]
+    syncRef: String[Literal[True]]
+    syncVertical: Bool[Literal[True]]
+    transitionEvaluation: Bool[Literal[True]]
+    transitionEntry: Bool[Literal[True]]
+    tabColor: ColorDescriptor[Literal[True]]
+    outlinePr: Typed[Outline, Literal[True]]
+    pageSetUpPr: Typed[PageSetupProperties, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    @overload
     def __init__(
-        self, controlPr: ControlProperty | None = None, *, shapeId: _ConvertibleToInt, name: str | None = None
+        self,
+        codeName: str | None = None,
+        enableFormatConditionsCalculation: _ConvertibleToBool | None = None,
+        filterMode: _ConvertibleToBool | None = None,
+        published: _ConvertibleToBool | None = None,
+        syncHorizontal: _ConvertibleToBool | None = None,
+        syncRef: str | None = None,
+        syncVertical: _ConvertibleToBool | None = None,
+        transitionEvaluation: _ConvertibleToBool | None = None,
+        transitionEntry: _ConvertibleToBool | None = None,
+        tabColor: str | Color | None = None,
+        outlinePr: Outline | None = None,
+        pageSetUpPr: PageSetupProperties | None = None,
     ) -> None: ...
-    @overload
-    def __init__(self, controlPr: ControlProperty | None, shapeId: _ConvertibleToInt, name: str | None = None) -> None: ...
-
-class Controls(Serialisable):
-    tagname: str
-    control: Incomplete
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, control=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/datavalidation.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/datavalidation.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal, Protocol
+from typing_extensions import TypeAlias
 
 from openpyxl.descriptors.base import (
     Alias,
     Bool,
     Convertible,
     Integer,
     NoneSet,
     String,
     _ConvertibleToBool,
-    _ConvertibleToInt,
     _ConvertibleToMultiCellRange,
 )
 from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.worksheet.cell_range import MultiCellRange
+from openpyxl.worksheet.cell_range import CellRange, MultiCellRange
+from openpyxl.xml.functions import Element
 
 _DataValidationType: TypeAlias = Literal["whole", "decimal", "list", "date", "time", "textLength", "custom"]
 _DataValidationErrorStyle: TypeAlias = Literal["stop", "warning", "information"]
 _DataValidationImeMode: TypeAlias = Literal[
     "noControl",
     "off",
     "on",
@@ -32,19 +32,22 @@
     "fullHangul",
     "halfHangul",
 ]
 _DataValidationOperator: TypeAlias = Literal[
     "between", "notBetween", "equal", "notEqual", "lessThan", "lessThanOrEqual", "greaterThan", "greaterThanOrEqual"
 ]
 
+class _HasCoordinate(Protocol):
+    coordinate: str | CellRange
+
 def collapse_cell_addresses(cells, input_ranges=()): ...
 def expand_cell_ranges(range_string): ...
 
 class DataValidation(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     sqref: Convertible[MultiCellRange, Literal[False]]
     cells: Alias
     ranges: Alias
     showDropDown: Bool[Literal[True]]
     hide_drop_down: Alias
     showInputMessage: Bool[Literal[True]]
     showErrorMessage: Bool[Literal[True]]
@@ -77,30 +80,30 @@
         prompt: str | None = None,
         errorTitle: str | None = None,
         imeMode: _DataValidationImeMode | Literal["none"] | None = None,
         operator: _DataValidationOperator | Literal["none"] | None = None,
         allow_blank: Incomplete | None = False,
     ) -> None: ...
     def add(self, cell) -> None: ...
-    def __contains__(self, cell): ...
+    def __contains__(self, cell: _HasCoordinate | str | CellRange) -> bool: ...
 
 class DataValidationList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     disablePrompts: Bool[Literal[True]]
     xWindow: Integer[Literal[True]]
     yWindow: Integer[Literal[True]]
     dataValidation: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         disablePrompts: _ConvertibleToBool | None = None,
-        xWindow: _ConvertibleToInt | None = None,
-        yWindow: _ConvertibleToInt | None = None,
+        xWindow: ConvertibleToInt | None = None,
+        yWindow: ConvertibleToInt | None = None,
         count: Incomplete | None = None,
         dataValidation=(),
     ) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
     def __len__(self) -> int: ...
     def append(self, dv) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None): ...  # type: ignore[override]
+    def to_tree(self, tagname: str | None = None) -> Element: ...  # type: ignore[override]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/dimensions.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/dimensions.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, Unused
 from collections.abc import Callable, Iterator
-from typing import ClassVar, Generic, TypeVar
-from typing_extensions import Literal, Self
+from typing import ClassVar, Generic, Literal, TypeVar
+from typing_extensions import Self
 
 from openpyxl.descriptors import Strict
-from openpyxl.descriptors.base import (
-    Alias,
-    Bool,
-    Float,
-    Integer,
-    String,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from openpyxl.descriptors.base import Alias, Bool, Float, Integer, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.styles.styleable import StyleableObject
 from openpyxl.utils.bound_dictionary import BoundDictionary
+from openpyxl.utils.cell import _RangeBoundariesTuple
 from openpyxl.worksheet.worksheet import Worksheet
 from openpyxl.xml.functions import Element
 
 _DimT = TypeVar("_DimT", bound=Dimension)
 
 class Dimension(Strict, StyleableObject):
     __fields__: ClassVar[tuple[str, ...]]
 
     index: Integer[Literal[False]]
     hidden: Bool[Literal[False]]
     outlineLevel: Integer[Literal[True]]
     outline_level: Alias
     collapsed: Bool[Literal[False]]
-    style: Alias
+    style: Alias  # type: ignore[assignment]
+
+    # Dimensions are only meant to be used on Worksheet objects
+    parent: Worksheet
 
     def __init__(
         self,
-        index: _ConvertibleToInt,
+        index: ConvertibleToInt,
         hidden: _ConvertibleToBool,
-        outlineLevel: _ConvertibleToInt | None,
+        outlineLevel: ConvertibleToInt | None,
         collapsed: _ConvertibleToBool,
         worksheet: Worksheet,
         visible: Unused = True,
         style: Incomplete | None = None,
     ) -> None: ...
     def __iter__(self) -> Iterator[tuple[str, str]]: ...
     def __copy__(self) -> Self: ...
@@ -52,21 +47,21 @@
     height: Alias
     thickBot: Bool[Literal[False]]
     thickTop: Bool[Literal[False]]
     def __init__(
         self,
         worksheet: Worksheet,
         index: int = 0,
-        ht: _ConvertibleToFloat | None = None,
+        ht: ConvertibleToFloat | None = None,
         customHeight: Unused = None,
         s: Incomplete | None = None,
         customFormat: Unused = None,
         hidden: _ConvertibleToBool = None,
-        outlineLevel: _ConvertibleToInt | None = 0,
-        outline_level: _ConvertibleToInt | None = None,
+        outlineLevel: ConvertibleToInt | None = 0,
+        outline_level: ConvertibleToInt | None = None,
         collapsed: _ConvertibleToBool = None,
         visible: Incomplete | None = None,
         height: Incomplete | None = None,
         r: Incomplete | None = None,
         spans: Unused = None,
         thickBot: _ConvertibleToBool = None,
         thickTop: _ConvertibleToBool = None,
@@ -77,32 +72,32 @@
     @property
     def customHeight(self) -> bool: ...
 
 class ColumnDimension(Dimension):
     width: Float[Literal[False]]
     bestFit: Bool[Literal[False]]
     auto_size: Alias
-    index: String[Literal[False]]  # type:ignore[assignment]
+    index: String[Literal[False]]  # type: ignore[assignment]
     min: Integer[Literal[True]]
     max: Integer[Literal[True]]
     collapsed: Bool[Literal[False]]
 
     def __init__(
         self,
         worksheet: Worksheet,
         index: str = "A",
-        width: _ConvertibleToFloat = 13,
+        width: ConvertibleToFloat = 13,
         bestFit: _ConvertibleToBool = False,
         hidden: _ConvertibleToBool = False,
-        outlineLevel: _ConvertibleToInt | None = 0,
-        outline_level: _ConvertibleToInt | None = None,
+        outlineLevel: ConvertibleToInt | None = 0,
+        outline_level: ConvertibleToInt | None = None,
         collapsed: _ConvertibleToBool = False,
         style: Incomplete | None = None,
-        min: _ConvertibleToInt | None = None,
-        max: _ConvertibleToInt | None = None,
+        min: ConvertibleToInt | None = None,
+        max: ConvertibleToInt | None = None,
         customWidth: Unused = False,
         visible: bool | None = None,
         auto_size: _ConvertibleToBool | None = None,
     ) -> None: ...
     @property
     def customWidth(self) -> bool: ...
     def reindex(self) -> None: ...
@@ -116,36 +111,36 @@
     def __init__(
         self, worksheet: Worksheet, reference: str = "index", default_factory: Callable[[], _DimT] | None = None
     ) -> None: ...
     def group(self, start: str, end: str | None = None, outline_level: int = 1, hidden: bool = False) -> None: ...
     def to_tree(self) -> Element | None: ...
 
 class SheetFormatProperties(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     baseColWidth: Integer[Literal[True]]
     defaultColWidth: Float[Literal[True]]
     defaultRowHeight: Float[Literal[False]]
     customHeight: Bool[Literal[True]]
     zeroHeight: Bool[Literal[True]]
     thickTop: Bool[Literal[True]]
     thickBottom: Bool[Literal[True]]
     outlineLevelRow: Integer[Literal[True]]
     outlineLevelCol: Integer[Literal[True]]
     def __init__(
         self,
-        baseColWidth: _ConvertibleToInt | None = 8,
-        defaultColWidth: _ConvertibleToFloat | None = None,
-        defaultRowHeight: _ConvertibleToFloat = 15,
+        baseColWidth: ConvertibleToInt | None = 8,
+        defaultColWidth: ConvertibleToFloat | None = None,
+        defaultRowHeight: ConvertibleToFloat = 15,
         customHeight: _ConvertibleToBool | None = None,
         zeroHeight: _ConvertibleToBool | None = None,
         thickTop: _ConvertibleToBool | None = None,
         thickBottom: _ConvertibleToBool | None = None,
-        outlineLevelRow: _ConvertibleToInt | None = None,
-        outlineLevelCol: _ConvertibleToInt | None = None,
+        outlineLevelRow: ConvertibleToInt | None = None,
+        outlineLevelCol: ConvertibleToInt | None = None,
     ) -> None: ...
 
 class SheetDimension(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ref: String[Literal[False]]
     def __init__(self, ref: str) -> None: ...
     @property
-    def boundaries(self): ...
+    def boundaries(self) -> _RangeBoundariesTuple: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/errors.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/errors.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
 from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Extension(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     uri: String[Literal[True]]
     def __init__(self, uri: str | None = None) -> None: ...
 
 class ExtensionList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ext: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, ext=()) -> None: ...
 
 class IgnoredError(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     sqref: Incomplete
     evalError: Bool[Literal[True]]
     twoDigitTextYear: Bool[Literal[True]]
     numberStoredAsText: Bool[Literal[True]]
     formula: Bool[Literal[True]]
     formulaRange: Bool[Literal[True]]
     unlockedFormula: Bool[Literal[True]]
@@ -39,12 +38,12 @@
         unlockedFormula: _ConvertibleToBool | None = False,
         emptyCellReference: _ConvertibleToBool | None = False,
         listDataValidation: _ConvertibleToBool | None = False,
         calculatedColumn: _ConvertibleToBool | None = False,
     ) -> None: ...
 
 class IgnoredErrors(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ignoredError: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, ignoredError=(), extLst: ExtensionList | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/filters.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/filters.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, Unused
 from datetime import datetime
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from re import Pattern
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
+from openpyxl.descriptors import Strict
 from openpyxl.descriptors.base import (
     Alias,
     Bool,
+    Convertible,
     DateTime,
     Float,
     Integer,
     MinMax,
     NoneSet,
     Set,
     String,
     Typed,
     _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
 )
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
+from ..descriptors.base import _N
+
 _SortConditionSortBy: TypeAlias = Literal["value", "cellColor", "fontColor", "icon"]
 _IconSet: TypeAlias = Literal[
     "3Arrows",
     "3ArrowsGray",
     "3Flags",
     "3TrafficLights1",
     "3TrafficLights2",
@@ -96,35 +99,35 @@
     "M10",
     "M11",
     "M12",
 ]
 _DateGroupItemDateTimeGrouping: TypeAlias = Literal["year", "month", "day", "hour", "minute", "second"]
 
 class SortCondition(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     descending: Bool[Literal[True]]
     sortBy: NoneSet[_SortConditionSortBy]
     ref: Incomplete
     customList: String[Literal[True]]
     dxfId: Integer[Literal[True]]
     iconSet: NoneSet[_IconSet]
     iconId: Integer[Literal[True]]
     def __init__(
         self,
         ref: Incomplete | None = None,
         descending: _ConvertibleToBool | None = None,
         sortBy: _SortConditionSortBy | Literal["none"] | None = None,
         customList: str | None = None,
-        dxfId: _ConvertibleToInt | None = None,
+        dxfId: ConvertibleToInt | None = None,
         iconSet: _IconSet | Literal["none"] | None = None,
-        iconId: _ConvertibleToInt | None = None,
+        iconId: ConvertibleToInt | None = None,
     ) -> None: ...
 
 class SortState(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     columnSort: Bool[Literal[True]]
     caseSensitive: Bool[Literal[True]]
     sortMethod: NoneSet[_SortStateSortMethod]
     ref: Incomplete
     sortCondition: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
@@ -136,160 +139,172 @@
         ref: Incomplete | None = None,
         sortCondition=(),
         extLst: Unused = None,
     ) -> None: ...
     def __bool__(self) -> bool: ...
 
 class IconFilter(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     iconSet: Set[_IconSet]
     iconId: Integer[Literal[True]]
-    def __init__(self, iconSet: _IconSet, iconId: _ConvertibleToInt | None = None) -> None: ...
+    def __init__(self, iconSet: _IconSet, iconId: ConvertibleToInt | None = None) -> None: ...
 
 class ColorFilter(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     dxfId: Integer[Literal[True]]
     cellColor: Bool[Literal[True]]
-    def __init__(self, dxfId: _ConvertibleToInt | None = None, cellColor: _ConvertibleToBool | None = None) -> None: ...
+    def __init__(self, dxfId: ConvertibleToInt | None = None, cellColor: _ConvertibleToBool | None = None) -> None: ...
 
 class DynamicFilter(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     type: Set[_DynamicFilterType]
     val: Float[Literal[True]]
     valIso: DateTime[Literal[True]]
     maxVal: Float[Literal[True]]
     maxValIso: DateTime[Literal[True]]
     def __init__(
         self,
         type: _DynamicFilterType,
-        val: _ConvertibleToFloat | None = None,
+        val: ConvertibleToFloat | None = None,
         valIso: datetime | str | None = None,
-        maxVal: _ConvertibleToFloat | None = None,
+        maxVal: ConvertibleToFloat | None = None,
         maxValIso: datetime | str | None = None,
     ) -> None: ...
 
+class CustomFilterValueDescriptor(Convertible[float | str, _N]):
+    pattern: Pattern[str]
+    expected_type: type[float | str]
+    @overload  # type: ignore[override]  # Different restrictions
+    def __set__(
+        self: CustomFilterValueDescriptor[Literal[True]], instance: Serialisable | Strict, value: str | ConvertibleToFloat | None
+    ) -> None: ...
+    @overload
+    def __set__(
+        self: CustomFilterValueDescriptor[Literal[False]], instance: Serialisable | Strict, value: str | ConvertibleToFloat
+    ) -> None: ...
+
 class CustomFilter(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     operator: NoneSet[_CustomFilterOperator]
     val: Incomplete
     def __init__(
         self, operator: _CustomFilterOperator | Literal["none"] | None = None, val: Incomplete | None = None
     ) -> None: ...
 
 class CustomFilters(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     _and: Bool[Literal[True]]  # Not private. Avoids name clash
     customFilter: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, _and: _ConvertibleToBool | None = False, customFilter=()) -> None: ...
 
 class Top10(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     top: Bool[Literal[True]]
     percent: Bool[Literal[True]]
     val: Float[Literal[False]]
     filterVal: Float[Literal[True]]
     @overload
     def __init__(
         self,
         top: _ConvertibleToBool | None = None,
         percent: _ConvertibleToBool | None = None,
         *,
-        val: _ConvertibleToFloat,
-        filterVal: _ConvertibleToFloat | None = None,
+        val: ConvertibleToFloat,
+        filterVal: ConvertibleToFloat | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
         top: _ConvertibleToBool | None,
         percent: _ConvertibleToBool | None,
-        val: _ConvertibleToFloat,
-        filterVal: _ConvertibleToFloat | None = None,
+        val: ConvertibleToFloat,
+        filterVal: ConvertibleToFloat | None = None,
     ) -> None: ...
 
 class DateGroupItem(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     year: Integer[Literal[False]]
     month: MinMax[float, Literal[True]]
     day: MinMax[float, Literal[True]]
     hour: MinMax[float, Literal[True]]
     minute: MinMax[float, Literal[True]]
     second: Integer[Literal[True]]
     dateTimeGrouping: Set[_DateGroupItemDateTimeGrouping]
     @overload
     def __init__(
         self,
-        year: _ConvertibleToInt,
-        month: _ConvertibleToFloat | None = None,
-        day: _ConvertibleToFloat | None = None,
-        hour: _ConvertibleToFloat | None = None,
-        minute: _ConvertibleToFloat | None = None,
-        second: _ConvertibleToInt | None = None,
+        year: ConvertibleToInt,
+        month: ConvertibleToFloat | None = None,
+        day: ConvertibleToFloat | None = None,
+        hour: ConvertibleToFloat | None = None,
+        minute: ConvertibleToFloat | None = None,
+        second: ConvertibleToInt | None = None,
         *,
         dateTimeGrouping: _DateGroupItemDateTimeGrouping,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        year: _ConvertibleToInt,
-        month: _ConvertibleToFloat | None,
-        day: _ConvertibleToFloat | None,
-        hour: _ConvertibleToFloat | None,
-        minute: _ConvertibleToFloat | None,
-        second: _ConvertibleToInt | None,
+        year: ConvertibleToInt,
+        month: ConvertibleToFloat | None,
+        day: ConvertibleToFloat | None,
+        hour: ConvertibleToFloat | None,
+        minute: ConvertibleToFloat | None,
+        second: ConvertibleToInt | None,
         dateTimeGrouping: _DateGroupItemDateTimeGrouping,
     ) -> None: ...
 
 class Filters(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     blank: Bool[Literal[True]]
     calendarType: NoneSet[_FiltersCalendarType]
     filter: Incomplete
     dateGroupItem: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         blank: _ConvertibleToBool | None = None,
         calendarType: _FiltersCalendarType | Literal["none"] | None = None,
         filter=(),
         dateGroupItem=(),
     ) -> None: ...
 
 class FilterColumn(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     colId: Integer[Literal[False]]
     col_id: Alias
     hiddenButton: Bool[Literal[True]]
     showButton: Bool[Literal[True]]
     filters: Typed[Filters, Literal[True]]
     top10: Typed[Top10, Literal[True]]
     customFilters: Typed[CustomFilters, Literal[True]]
     dynamicFilter: Typed[DynamicFilter, Literal[True]]
     colorFilter: Typed[ColorFilter, Literal[True]]
     iconFilter: Typed[IconFilter, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        colId: _ConvertibleToInt,
+        colId: ConvertibleToInt,
         hiddenButton: _ConvertibleToBool | None = False,
         showButton: _ConvertibleToBool | None = True,
         filters: Filters | None = None,
         top10: Top10 | None = None,
         customFilters: CustomFilters | None = None,
         dynamicFilter: DynamicFilter | None = None,
         colorFilter: ColorFilter | None = None,
         iconFilter: IconFilter | None = None,
         extLst: Unused = None,
         blank: Incomplete | None = None,
         vals: Incomplete | None = None,
     ) -> None: ...
 
 class AutoFilter(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ref: Incomplete
     filterColumn: Incomplete
     sortState: Typed[SortState, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self, ref: Incomplete | None = None, filterColumn=(), sortState: SortState | None = None, extLst: Unused = None
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/formula.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/formula.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/header_footer.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/header_footer.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt
+from re import Pattern
+from typing import ClassVar, Final, Literal
+from typing_extensions import Self
 
 from openpyxl.descriptors import Strict
-from openpyxl.descriptors.base import Alias, Bool, Integer, MatchPattern, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Bool, Integer, MatchPattern, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.xml.functions import Element
 
-FONT_PATTERN: str
-COLOR_PATTERN: str
-SIZE_REGEX: str
-FORMAT_REGEX: Incomplete
+from ..xml._functions_overloads import _HasText
+
+FONT_PATTERN: Final = '&"(?P<font>.+)"'
+COLOR_PATTERN: Final = "&K(?P<color>[A-F0-9]{6})"
+SIZE_REGEX: Final = r"&(?P<size>\d+\s?)"
+FORMAT_REGEX: Final[Pattern[str]]
 
 class _HeaderFooterPart(Strict):
     text: String[Literal[True]]
     font: String[Literal[True]]
     size: Integer[Literal[True]]
-    RGB: str
+    RGB: ClassVar[str]
     color: MatchPattern[str, Literal[True]]
     def __init__(
-        self, text: str | None = None, font: str | None = None, size: _ConvertibleToInt | None = None, color: str | None = None
+        self, text: str | None = None, font: str | None = None, size: ConvertibleToInt | None = None, color: str | None = None
     ) -> None: ...
     def __bool__(self) -> bool: ...
     @classmethod
     def from_str(cls, text): ...
 
 class HeaderFooterItem(Strict):
     left: Typed[_HeaderFooterPart, Literal[False]]
@@ -32,20 +36,20 @@
     def __init__(
         self,
         left: _HeaderFooterPart | None = None,
         right: _HeaderFooterPart | None = None,
         center: _HeaderFooterPart | None = None,
     ) -> None: ...
     def __bool__(self) -> bool: ...
-    def to_tree(self, tagname): ...
+    def to_tree(self, tagname: str) -> Element: ...
     @classmethod
-    def from_tree(cls, node): ...
+    def from_tree(cls, node: _HasText) -> Self: ...
 
 class HeaderFooter(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     differentOddEven: Bool[Literal[True]]
     differentFirst: Bool[Literal[True]]
     scaleWithDoc: Bool[Literal[True]]
     alignWithMargins: Bool[Literal[True]]
     oddHeader: Typed[HeaderFooterItem, Literal[True]]
     oddFooter: Typed[HeaderFooterItem, Literal[True]]
     evenHeader: Typed[HeaderFooterItem, Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/hyperlink.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/hyperlink.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from typing import ClassVar, Literal
 
 from openpyxl.descriptors.base import String
 from openpyxl.descriptors.serialisable import Serialisable
 
 class Hyperlink(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     ref: String[Literal[False]]
     location: String[Literal[True]]
     tooltip: String[Literal[True]]
     display: String[Literal[True]]
     id: Incomplete
     target: String[Literal[True]]
     __attrs__: ClassVar[tuple[str, ...]]
@@ -21,13 +20,13 @@
         tooltip: str | None = None,
         display: str | None = None,
         id: Incomplete | None = None,
         target: str | None = None,
     ) -> None: ...
 
 class HyperlinkList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     hyperlink: Incomplete
     def __init__(self, hyperlink=()) -> None: ...
     def __bool__(self) -> bool: ...
     def __len__(self) -> int: ...
     def append(self, value) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/ole.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/ole.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from _typeshed import Incomplete
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal, overload
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Bool, Integer, Set, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, Set, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.spreadsheet_drawing import AnchorMarker
 
 _OleObjectDvAspect: TypeAlias = Literal["DVASPECT_CONTENT", "DVASPECT_ICON"]
 _OleObjectOleUpdate: TypeAlias = Literal["OLEUPDATE_ALWAYS", "OLEUPDATE_ONCALL"]
 
 class ObjectAnchor(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     _from: Typed[AnchorMarker, Literal[False]]  # Not private. Avoids name clash
     to: Typed[AnchorMarker, Literal[False]]
     moveWithCells: Bool[Literal[True]]
     sizeWithCells: Bool[Literal[True]]
     z_order: Integer[Literal[True]]
     def __init__(
         self,
         _from: AnchorMarker,
         to: AnchorMarker,
         moveWithCells: _ConvertibleToBool | None = False,
         sizeWithCells: _ConvertibleToBool | None = False,
-        z_order: _ConvertibleToInt | None = None,
+        z_order: ConvertibleToInt | None = None,
     ) -> None: ...
 
 class ObjectPr(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     anchor: Typed[ObjectAnchor, Literal[False]]
     locked: Bool[Literal[True]]
     defaultSize: Bool[Literal[True]]
     _print: Bool[Literal[True]]  # Not private. Avoids name clash
     disabled: Bool[Literal[True]]
     uiObject: Bool[Literal[True]]
     autoFill: Bool[Literal[True]]
@@ -71,15 +71,15 @@
         autoPict: _ConvertibleToBool | None,
         macro: str,
         altText: str | None = None,
         dde: _ConvertibleToBool | None = False,
     ) -> None: ...
 
 class OleObject(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     objectPr: Typed[ObjectPr, Literal[True]]
     progId: String[Literal[True]]
     dvAspect: Set[_OleObjectDvAspect]
     link: String[Literal[True]]
     oleUpdate: Set[_OleObjectOleUpdate]
     autoLoad: Bool[Literal[True]]
     shapeId: Integer[Literal[False]]
@@ -90,26 +90,26 @@
         objectPr: ObjectPr | None = None,
         progId: str | None = None,
         dvAspect: _OleObjectDvAspect = "DVASPECT_CONTENT",
         link: str | None = None,
         *,
         oleUpdate: _OleObjectOleUpdate,
         autoLoad: _ConvertibleToBool | None = False,
-        shapeId: _ConvertibleToInt,
+        shapeId: ConvertibleToInt,
     ) -> None: ...
     @overload
     def __init__(
         self,
         objectPr: ObjectPr | None,
         progId: str | None,
         dvAspect: _OleObjectDvAspect,
         link: str | None,
         oleUpdate: _OleObjectOleUpdate,
         autoLoad: _ConvertibleToBool | None,
-        shapeId: _ConvertibleToInt,
+        shapeId: ConvertibleToInt,
     ) -> None: ...
 
 class OleObjects(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     oleObject: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, oleObject=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/page.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/page.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from _typeshed import Incomplete
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal
+from typing_extensions import Self, TypeAlias
 
-from openpyxl.descriptors.base import Bool, Float, Integer, NoneSet, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
-from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.descriptors.base import Bool, Float, Integer, NoneSet, _ConvertibleToBool
+from openpyxl.descriptors.serialisable import Serialisable, _ChildSerialisableTreeElement
+from openpyxl.worksheet.properties import PageSetupProperties
 
 _PrintPageSetupOrientation: TypeAlias = Literal["default", "portrait", "landscape"]
 _PrintPageSetupPageOrder: TypeAlias = Literal["downThenOver", "overThenDown"]
 _PrintPageSetupCellComments: TypeAlias = Literal["asDisplayed", "atEnd"]
 _PrintPageSetupErrors: TypeAlias = Literal["displayed", "blank", "dash", "NA"]
 
 class PrintPageSetup(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     orientation: NoneSet[_PrintPageSetupOrientation]
     paperSize: Integer[Literal[True]]
     scale: Integer[Literal[True]]
     fitToHeight: Integer[Literal[True]]
     fitToWidth: Integer[Literal[True]]
     firstPageNumber: Integer[Literal[True]]
     useFirstPageNumber: Bool[Literal[True]]
@@ -30,49 +32,49 @@
     verticalDpi: Integer[Literal[True]]
     copies: Integer[Literal[True]]
     id: Incomplete
     def __init__(
         self,
         worksheet: Incomplete | None = None,
         orientation: _PrintPageSetupOrientation | Literal["none"] | None = None,
-        paperSize: _ConvertibleToInt | None = None,
-        scale: _ConvertibleToInt | None = None,
-        fitToHeight: _ConvertibleToInt | None = None,
-        fitToWidth: _ConvertibleToInt | None = None,
-        firstPageNumber: _ConvertibleToInt | None = None,
+        paperSize: ConvertibleToInt | None = None,
+        scale: ConvertibleToInt | None = None,
+        fitToHeight: ConvertibleToInt | None = None,
+        fitToWidth: ConvertibleToInt | None = None,
+        firstPageNumber: ConvertibleToInt | None = None,
         useFirstPageNumber: _ConvertibleToBool | None = None,
         paperHeight: Incomplete | None = None,
         paperWidth: Incomplete | None = None,
         pageOrder: _PrintPageSetupPageOrder | Literal["none"] | None = None,
         usePrinterDefaults: _ConvertibleToBool | None = None,
         blackAndWhite: _ConvertibleToBool | None = None,
         draft: _ConvertibleToBool | None = None,
         cellComments: _PrintPageSetupCellComments | Literal["none"] | None = None,
         errors: _PrintPageSetupErrors | Literal["none"] | None = None,
-        horizontalDpi: _ConvertibleToInt | None = None,
-        verticalDpi: _ConvertibleToInt | None = None,
-        copies: _ConvertibleToInt | None = None,
+        horizontalDpi: ConvertibleToInt | None = None,
+        verticalDpi: ConvertibleToInt | None = None,
+        copies: ConvertibleToInt | None = None,
         id: Incomplete | None = None,
     ) -> None: ...
     def __bool__(self) -> bool: ...
     @property
-    def sheet_properties(self): ...
+    def sheet_properties(self) -> PageSetupProperties | None: ...
     @property
-    def fitToPage(self): ...
+    def fitToPage(self) -> bool | None: ...
     @fitToPage.setter
-    def fitToPage(self, value) -> None: ...
+    def fitToPage(self, value: _ConvertibleToBool | None) -> None: ...
     @property
-    def autoPageBreaks(self): ...
+    def autoPageBreaks(self) -> bool | None: ...
     @autoPageBreaks.setter
-    def autoPageBreaks(self, value) -> None: ...
+    def autoPageBreaks(self, value: _ConvertibleToBool | None) -> None: ...
     @classmethod
-    def from_tree(cls, node): ...
+    def from_tree(cls, node: _ChildSerialisableTreeElement) -> Self: ...
 
 class PrintOptions(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     horizontalCentered: Bool[Literal[True]]
     verticalCentered: Bool[Literal[True]]
     headings: Bool[Literal[True]]
     gridLines: Bool[Literal[True]]
     gridLinesSet: Bool[Literal[True]]
     def __init__(
         self,
@@ -81,23 +83,23 @@
         headings: _ConvertibleToBool | None = None,
         gridLines: _ConvertibleToBool | None = None,
         gridLinesSet: _ConvertibleToBool | None = None,
     ) -> None: ...
     def __bool__(self) -> bool: ...
 
 class PageMargins(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     left: Float[Literal[False]]
     right: Float[Literal[False]]
     top: Float[Literal[False]]
     bottom: Float[Literal[False]]
     header: Float[Literal[False]]
     footer: Float[Literal[False]]
     def __init__(
         self,
-        left: _ConvertibleToFloat = 0.75,
-        right: _ConvertibleToFloat = 0.75,
-        top: _ConvertibleToFloat = 1,
-        bottom: _ConvertibleToFloat = 1,
-        header: _ConvertibleToFloat = 0.5,
-        footer: _ConvertibleToFloat = 0.5,
+        left: ConvertibleToFloat = 0.75,
+        right: ConvertibleToFloat = 0.75,
+        top: ConvertibleToFloat = 1,
+        bottom: ConvertibleToFloat = 1,
+        header: ConvertibleToFloat = 0.5,
+        footer: ConvertibleToFloat = 0.5,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/print_settings.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/print_settings.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import ConvertibleToInt, Unused
 from re import Pattern
-from typing import overload
-from typing_extensions import Literal, Self
+from typing import Final, Literal, overload
+from typing_extensions import Self
 
 from openpyxl.descriptors import Integer, Strict, String
-from openpyxl.descriptors.base import Typed, _ConvertibleToInt
+from openpyxl.descriptors.base import Typed
 from openpyxl.utils.cell import SHEETRANGE_RE as SHEETRANGE_RE
 
 from .cell_range import MultiCellRange
 
-COL_RANGE: str
-COL_RANGE_RE: Pattern[str]
-ROW_RANGE: str
-ROW_RANGE_RE: Pattern[str]
-TITLES_REGEX: Pattern[str]
-PRINT_AREA_RE: Pattern[str]
+COL_RANGE: Final[str]
+COL_RANGE_RE: Final[Pattern[str]]
+ROW_RANGE: Final[str]
+ROW_RANGE_RE: Final[Pattern[str]]
+TITLES_REGEX: Final[Pattern[str]]
+PRINT_AREA_RE: Final[Pattern[str]]
 
 class ColRange(Strict):
     min_col: String[Literal[False]]
     max_col: String[Literal[False]]
     @overload
     def __init__(self, range_string: None = None, *, min_col: str, max_col: str) -> None: ...
     @overload
-    def __init__(self, range_string: Incomplete, min_col: Unused = None, max_col: Unused = None) -> None: ...
+    def __init__(self, range_string, min_col: Unused = None, max_col: Unused = None) -> None: ...
     def __eq__(self, other: object) -> bool: ...
 
 class RowRange(Strict):
     min_row: Integer[Literal[False]]
     max_row: Integer[Literal[False]]
     @overload
-    def __init__(self, range_string: None, min_row: _ConvertibleToInt, max_row: _ConvertibleToInt) -> None: ...
+    def __init__(self, range_string: None, min_row: ConvertibleToInt, max_row: ConvertibleToInt) -> None: ...
     @overload
-    def __init__(self, range_string: Incomplete, min_row: Unused = None, max_row: Unused = None) -> None: ...
+    def __init__(self, range_string, min_row: Unused = None, max_row: Unused = None) -> None: ...
     def __eq__(self, other: object) -> bool: ...
 
 class PrintTitles(Strict):
     cols: Typed[ColRange, Literal[True]]
     rows: Typed[RowRange, Literal[True]]
     title: String[Literal[False]]
     def __init__(self, cols: ColRange | None = None, rows: RowRange | None = None, title: str = "") -> None: ...
     @classmethod
-    def from_string(cls, value) -> Self: ...
+    def from_string(cls, value: str) -> Self: ...
     def __eq__(self, other: object) -> bool: ...
 
 class PrintArea(MultiCellRange):
     title: str
     @classmethod
     def from_string(cls, value) -> Self: ...
-    def __init__(self, ranges=(), title: str = "") -> None: ...
-    def __eq__(self, other): ...
+    def __init__(self, ranges=(), title: Unused = "") -> None: ...
+    def __eq__(self, other: str | MultiCellRange) -> bool: ...  # type: ignore[override]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/properties.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/borders.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,88 @@
 from _typeshed import Incomplete
-from typing import ClassVar
-from typing_extensions import Literal
+from collections.abc import Iterator
+from typing import ClassVar, Final, Literal
+from typing_extensions import TypeAlias
 
-from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
+from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles.colors import Color, ColorDescriptor
 
-class Outline(Serialisable):
-    tagname: str
-    applyStyles: Bool[Literal[True]]
-    summaryBelow: Bool[Literal[True]]
-    summaryRight: Bool[Literal[True]]
-    showOutlineSymbols: Bool[Literal[True]]
+_SideStyle: TypeAlias = Literal[
+    "dashDot",
+    "dashDotDot",
+    "dashed",
+    "dotted",
+    "double",
+    "hair",
+    "medium",
+    "mediumDashDot",
+    "mediumDashDotDot",
+    "mediumDashed",
+    "slantDashDot",
+    "thick",
+    "thin",
+]
+
+BORDER_NONE: Final = None
+BORDER_DASHDOT: Final = "dashDot"
+BORDER_DASHDOTDOT: Final = "dashDotDot"
+BORDER_DASHED: Final = "dashed"
+BORDER_DOTTED: Final = "dotted"
+BORDER_DOUBLE: Final = "double"
+BORDER_HAIR: Final = "hair"
+BORDER_MEDIUM: Final = "medium"
+BORDER_MEDIUMDASHDOT: Final = "mediumDashDot"
+BORDER_MEDIUMDASHDOTDOT: Final = "mediumDashDotDot"
+BORDER_MEDIUMDASHED: Final = "mediumDashed"
+BORDER_SLANTDASHDOT: Final = "slantDashDot"
+BORDER_THICK: Final = "thick"
+BORDER_THIN: Final = "thin"
+
+class Side(Serialisable):
+    __fields__: ClassVar[tuple[str, ...]]
+    color: ColorDescriptor[Literal[True]]
+    style: NoneSet[_SideStyle]
+    border_style: Alias
     def __init__(
         self,
-        applyStyles: _ConvertibleToBool | None = None,
-        summaryBelow: _ConvertibleToBool | None = None,
-        summaryRight: _ConvertibleToBool | None = None,
-        showOutlineSymbols: _ConvertibleToBool | None = None,
+        style: _SideStyle | Literal["none"] | None = None,
+        color: str | Color | None = None,
+        border_style: Incomplete | None = None,
     ) -> None: ...
 
-class PageSetupProperties(Serialisable):
-    tagname: str
-    autoPageBreaks: Bool[Literal[True]]
-    fitToPage: Bool[Literal[True]]
-    def __init__(self, autoPageBreaks: _ConvertibleToBool | None = None, fitToPage: _ConvertibleToBool | None = None) -> None: ...
-
-class WorksheetProperties(Serialisable):
-    tagname: str
-    codeName: String[Literal[True]]
-    enableFormatConditionsCalculation: Bool[Literal[True]]
-    filterMode: Bool[Literal[True]]
-    published: Bool[Literal[True]]
-    syncHorizontal: Bool[Literal[True]]
-    syncRef: String[Literal[True]]
-    syncVertical: Bool[Literal[True]]
-    transitionEvaluation: Bool[Literal[True]]
-    transitionEntry: Bool[Literal[True]]
-    tabColor: Incomplete
-    outlinePr: Typed[Outline, Literal[True]]
-    pageSetUpPr: Typed[PageSetupProperties, Literal[True]]
+class Border(Serialisable):
+    tagname: ClassVar[str]
+    __fields__: ClassVar[tuple[str, ...]]
     __elements__: ClassVar[tuple[str, ...]]
+    start: Typed[Side, Literal[True]]
+    end: Typed[Side, Literal[True]]
+    left: Typed[Side, Literal[True]]
+    right: Typed[Side, Literal[True]]
+    top: Typed[Side, Literal[True]]
+    bottom: Typed[Side, Literal[True]]
+    diagonal: Typed[Side, Literal[True]]
+    vertical: Typed[Side, Literal[True]]
+    horizontal: Typed[Side, Literal[True]]
+    outline: Bool[Literal[False]]
+    diagonalUp: Bool[Literal[False]]
+    diagonalDown: Bool[Literal[False]]
+    diagonal_direction: Incomplete
     def __init__(
         self,
-        codeName: str | None = None,
-        enableFormatConditionsCalculation: _ConvertibleToBool | None = None,
-        filterMode: _ConvertibleToBool | None = None,
-        published: _ConvertibleToBool | None = None,
-        syncHorizontal: _ConvertibleToBool | None = None,
-        syncRef: str | None = None,
-        syncVertical: _ConvertibleToBool | None = None,
-        transitionEvaluation: _ConvertibleToBool | None = None,
-        transitionEntry: _ConvertibleToBool | None = None,
-        tabColor: Incomplete | None = None,
-        outlinePr: Outline | None = None,
-        pageSetUpPr: PageSetupProperties | None = None,
+        left: Side | None = None,
+        right: Side | None = None,
+        top: Side | None = None,
+        bottom: Side | None = None,
+        diagonal: Side | None = None,
+        diagonal_direction: Incomplete | None = None,
+        vertical: Side | None = None,
+        horizontal: Side | None = None,
+        diagonalUp: _ConvertibleToBool = False,
+        diagonalDown: _ConvertibleToBool = False,
+        outline: _ConvertibleToBool = True,
+        start: Side | None = None,
+        end: Side | None = None,
     ) -> None: ...
+    def __iter__(self) -> Iterator[tuple[str, str]]: ...
+
+DEFAULT_BORDER: Final[Border]
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/scenario.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/styles/cell_style.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,98 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal
-
-from openpyxl.descriptors.base import (
-    Bool,
-    Convertible,
-    Integer,
-    String,
-    _ConvertibleToBool,
-    _ConvertibleToInt,
-    _ConvertibleToMultiCellRange,
-)
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from array import array
+from collections.abc import Iterable, MutableSequence
+from typing import ClassVar, Generic, Literal, TypeVar
+from typing_extensions import Self
+
+from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool
+from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.worksheet.cell_range import MultiCellRange
+from openpyxl.styles.alignment import Alignment
+from openpyxl.styles.protection import Protection
 
-class InputCells(Serialisable):
-    tagname: str
-    r: String[Literal[False]]
-    deleted: Bool[Literal[True]]
-    undone: Bool[Literal[True]]
-    val: String[Literal[False]]
-    numFmtId: Integer[Literal[True]]
+_T = TypeVar("_T")
 
-    @overload
-    def __init__(
-        self,
-        r: str,
-        deleted: _ConvertibleToBool | None = False,
-        undone: _ConvertibleToBool | None = False,
-        *,
-        val: str,
-        numFmtId: _ConvertibleToInt | None = None,
-    ) -> None: ...
-    @overload
-    def __init__(
-        self,
-        r: str,
-        deleted: _ConvertibleToBool | None,
-        undone: _ConvertibleToBool | None,
-        val: str,
-        numFmtId: _ConvertibleToInt | None = None,
-    ) -> None: ...
+class ArrayDescriptor(Generic[_T]):
+    key: int
+    def __init__(self, key: int) -> None: ...
+    def __get__(self, instance: MutableSequence[_T], cls: Unused) -> _T: ...
+    def __set__(self, instance: MutableSequence[_T], value: _T) -> None: ...
 
-class Scenario(Serialisable):
-    tagname: str
-    inputCells: Incomplete
-    name: String[Literal[False]]
-    locked: Bool[Literal[True]]
-    hidden: Bool[Literal[True]]
-    user: String[Literal[True]]
-    comment: String[Literal[True]]
+class StyleArray(array[int]):
+    tagname: ClassVar[str]
+    fontId: ArrayDescriptor[int]
+    fillId: ArrayDescriptor[int]
+    borderId: ArrayDescriptor[int]
+    numFmtId: ArrayDescriptor[int]
+    protectionId: ArrayDescriptor[int]
+    alignmentId: ArrayDescriptor[int]
+    pivotButton: ArrayDescriptor[int]
+    quotePrefix: ArrayDescriptor[int]
+    xfId: ArrayDescriptor[int]
+    def __new__(cls, args: bytes | bytearray | Iterable[int] = [0, 0, 0, 0, 0, 0, 0, 0, 0]) -> Self: ...
+    def __init__(self, args: bytes | bytearray | Iterable[int] = [0, 0, 0, 0, 0, 0, 0, 0, 0]) -> None: ...
+    def __hash__(self) -> int: ...
+    def __copy__(self) -> StyleArray: ...
+    def __deepcopy__(self, memo: Unused) -> StyleArray: ...
+
+class CellStyle(Serialisable):
+    tagname: ClassVar[str]
+    numFmtId: Integer[Literal[False]]
+    fontId: Integer[Literal[False]]
+    fillId: Integer[Literal[False]]
+    borderId: Integer[Literal[False]]
+    xfId: Integer[Literal[True]]
+    quotePrefix: Bool[Literal[True]]
+    pivotButton: Bool[Literal[True]]
+    applyNumberFormat: Bool[Literal[True]]
+    applyFont: Bool[Literal[True]]
+    applyFill: Bool[Literal[True]]
+    applyBorder: Bool[Literal[True]]
+    # Overwritten by properties below
+    # applyAlignment: Bool[Literal[True]]
+    # applyProtection: Bool[Literal[True]]
+    alignment: Typed[Alignment, Literal[True]]
+    protection: Typed[Protection, Literal[True]]
+    extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
-    @overload
     def __init__(
         self,
-        inputCells=(),
-        *,
-        name: str,
-        locked: _ConvertibleToBool | None = False,
-        hidden: _ConvertibleToBool | None = False,
-        count: Unused = None,
-        user: str | None = None,
-        comment: str | None = None,
-    ) -> None: ...
-    @overload
-    def __init__(
-        self,
-        inputCells,
-        name: str,
-        locked: _ConvertibleToBool | None = False,
-        hidden: _ConvertibleToBool | None = False,
-        count: Unused = None,
-        user: str | None = None,
-        comment: str | None = None,
+        numFmtId: ConvertibleToInt = 0,
+        fontId: ConvertibleToInt = 0,
+        fillId: ConvertibleToInt = 0,
+        borderId: ConvertibleToInt = 0,
+        xfId: ConvertibleToInt | None = None,
+        quotePrefix: _ConvertibleToBool | None = None,
+        pivotButton: _ConvertibleToBool | None = None,
+        applyNumberFormat: _ConvertibleToBool | None = None,
+        applyFont: _ConvertibleToBool | None = None,
+        applyFill: _ConvertibleToBool | None = None,
+        applyBorder: _ConvertibleToBool | None = None,
+        applyAlignment: Unused = None,
+        applyProtection: Unused = None,
+        alignment: Alignment | None = None,
+        protection: Protection | None = None,
+        extLst: Unused = None,
     ) -> None: ...
+    def to_array(self): ...
+    @classmethod
+    def from_array(cls, style): ...
     @property
-    def count(self): ...
+    def applyProtection(self) -> Literal[True] | None: ...
+    @property
+    def applyAlignment(self) -> Literal[True] | None: ...
 
-class ScenarioList(Serialisable):
-    tagname: str
-    scenario: Incomplete
-    current: Integer[Literal[True]]
-    show: Integer[Literal[True]]
-    sqref: Convertible[MultiCellRange, Literal[True]]
+class CellStyleList(Serialisable):
+    tagname: ClassVar[str]
+    __attrs__: ClassVar[tuple[str, ...]]
+    # Overwritten by property below
+    # count: Integer
+    xf: Incomplete
+    alignment: Incomplete
+    protection: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(
-        self,
-        scenario=(),
-        current: _ConvertibleToInt | None = None,
-        show: _ConvertibleToInt | None = None,
-        sqref: _ConvertibleToMultiCellRange | None = None,
-    ) -> None: ...
-    def append(self, scenario) -> None: ...
-    def __bool__(self) -> bool: ...
+    def __init__(self, count: Unused = None, xf=()) -> None: ...
+    @property
+    def count(self) -> int: ...
+    def __getitem__(self, idx): ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/smart_tag.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/smart_tag.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-from _typeshed import Incomplete
-from typing import ClassVar, overload
-from typing_extensions import Literal
+from _typeshed import ConvertibleToInt, Incomplete
+from typing import ClassVar, Literal, overload
 
-from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
 class CellSmartTagPr(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     key: String[Literal[False]]
     val: String[Literal[False]]
     def __init__(self, key: str, val: str) -> None: ...
 
 class CellSmartTag(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     cellSmartTagPr: Incomplete
     type: Integer[Literal[False]]
     deleted: Bool[Literal[True]]
     xmlBased: Bool[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         cellSmartTagPr=(),
         *,
-        type: _ConvertibleToInt,
+        type: ConvertibleToInt,
         deleted: _ConvertibleToBool | None = False,
         xmlBased: _ConvertibleToBool | None = False,
     ) -> None: ...
     @overload
     def __init__(
         self,
         cellSmartTagPr,
-        type: _ConvertibleToInt,
+        type: ConvertibleToInt,
         deleted: _ConvertibleToBool | None = False,
         xmlBased: _ConvertibleToBool | None = False,
     ) -> None: ...
 
 class CellSmartTags(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     cellSmartTag: Incomplete
     r: String[Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cellSmartTag, r: str) -> None: ...
 
 class SmartTags(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     cellSmartTags: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, cellSmartTags=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/table.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/table.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
-from typing_extensions import Literal, TypeAlias
+from _typeshed import ConvertibleToInt, Incomplete, Unused
+from collections.abc import Iterator
+from typing import ClassVar, Final, Literal, overload
+from typing_extensions import Self, TypeAlias
 
 from openpyxl.descriptors import Strict, String
-from openpyxl.descriptors.base import Alias, Bool, Integer, NoneSet, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, Bool, Integer, NoneSet, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.descriptors.serialisable import Serialisable, _ChildSerialisableTreeElement
 from openpyxl.worksheet.filters import AutoFilter, SortState
+from openpyxl.xml.functions import Element
 
 _TableColumnTotalsRowFunction: TypeAlias = Literal[
     "sum", "min", "max", "average", "count", "countNums", "stdDev", "var", "custom"
 ]
 _TableTableType: TypeAlias = Literal["worksheet", "xml", "queryTable"]
 
-TABLESTYLES: Incomplete
-PIVOTSTYLES: Incomplete
+TABLESTYLES: Final[tuple[str, ...]]
+PIVOTSTYLES: Final[tuple[str, ...]]
 
 class TableStyleInfo(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     name: String[Literal[True]]
     showFirstColumn: Bool[Literal[True]]
     showLastColumn: Bool[Literal[True]]
     showRowStripes: Bool[Literal[True]]
     showColumnStripes: Bool[Literal[True]]
     def __init__(
         self,
@@ -29,50 +31,50 @@
         showFirstColumn: _ConvertibleToBool | None = None,
         showLastColumn: _ConvertibleToBool | None = None,
         showRowStripes: _ConvertibleToBool | None = None,
         showColumnStripes: _ConvertibleToBool | None = None,
     ) -> None: ...
 
 class XMLColumnProps(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     mapId: Integer[Literal[False]]
     xpath: String[Literal[False]]
     denormalized: Bool[Literal[True]]
     xmlDataType: String[Literal[False]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
-        mapId: _ConvertibleToInt,
+        mapId: ConvertibleToInt,
         xpath: str,
         denormalized: _ConvertibleToBool | None = None,
         *,
         xmlDataType: str,
         extLst: Unused = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        mapId: _ConvertibleToInt,
+        mapId: ConvertibleToInt,
         xpath: str,
         denormalized: _ConvertibleToBool | None,
         xmlDataType: str,
         extLst: Unused = None,
     ) -> None: ...
 
 class TableFormula(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     array: Bool[Literal[True]]
     attr_text: Incomplete
     text: Alias
     def __init__(self, array: _ConvertibleToBool | None = None, attr_text: Incomplete | None = None) -> None: ...
 
 class TableColumn(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     id: Integer[Literal[False]]
     uniqueName: String[Literal[True]]
     name: String[Literal[False]]
     totalsRowFunction: NoneSet[_TableColumnTotalsRowFunction]
     totalsRowLabel: String[Literal[True]]
     queryTableFieldId: Integer[Literal[True]]
     headerRowDxfId: Integer[Literal[True]]
@@ -85,62 +87,62 @@
     totalsRowFormula: Typed[TableFormula, Literal[True]]
     xmlColumnPr: Typed[XMLColumnProps, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
-        id: _ConvertibleToInt,
+        id: ConvertibleToInt,
         uniqueName: str | None = None,
         *,
         name: str,
         totalsRowFunction: _TableColumnTotalsRowFunction | Literal["none"] | None = None,
         totalsRowLabel: str | None = None,
-        queryTableFieldId: _ConvertibleToInt | None = None,
-        headerRowDxfId: _ConvertibleToInt | None = None,
-        dataDxfId: _ConvertibleToInt | None = None,
-        totalsRowDxfId: _ConvertibleToInt | None = None,
+        queryTableFieldId: ConvertibleToInt | None = None,
+        headerRowDxfId: ConvertibleToInt | None = None,
+        dataDxfId: ConvertibleToInt | None = None,
+        totalsRowDxfId: ConvertibleToInt | None = None,
         headerRowCellStyle: str | None = None,
         dataCellStyle: str | None = None,
         totalsRowCellStyle: str | None = None,
         calculatedColumnFormula: TableFormula | None = None,
         totalsRowFormula: TableFormula | None = None,
         xmlColumnPr: XMLColumnProps | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
     @overload
     def __init__(
         self,
-        id: _ConvertibleToInt,
+        id: ConvertibleToInt,
         uniqueName: str | None,
         name: str,
         totalsRowFunction: _TableColumnTotalsRowFunction | Literal["none"] | None = None,
         totalsRowLabel: str | None = None,
-        queryTableFieldId: _ConvertibleToInt | None = None,
-        headerRowDxfId: _ConvertibleToInt | None = None,
-        dataDxfId: _ConvertibleToInt | None = None,
-        totalsRowDxfId: _ConvertibleToInt | None = None,
+        queryTableFieldId: ConvertibleToInt | None = None,
+        headerRowDxfId: ConvertibleToInt | None = None,
+        dataDxfId: ConvertibleToInt | None = None,
+        totalsRowDxfId: ConvertibleToInt | None = None,
         headerRowCellStyle: str | None = None,
         dataCellStyle: str | None = None,
         totalsRowCellStyle: str | None = None,
         calculatedColumnFormula: TableFormula | None = None,
         totalsRowFormula: TableFormula | None = None,
         xmlColumnPr: XMLColumnProps | None = None,
         extLst: ExtensionList | None = None,
     ) -> None: ...
-    def __iter__(self): ...
+    def __iter__(self) -> Iterator[tuple[str, str]]: ...
     @classmethod
-    def from_tree(cls, node): ...
+    def from_tree(cls, node: _ChildSerialisableTreeElement) -> Self: ...
 
 class TableNameDescriptor(String[Incomplete]):
     def __set__(self, instance: Serialisable | Strict, value) -> None: ...
 
 class Table(Serialisable):
     mime_type: str
-    tagname: str
+    tagname: ClassVar[str]
     id: Integer[Literal[False]]
     name: String[Literal[True]]
     displayName: Incomplete
     comment: String[Literal[True]]
     ref: Incomplete
     tableType: NoneSet[_TableTableType]
     headerRowCount: Integer[Literal[True]]
@@ -163,58 +165,58 @@
     sortState: Typed[SortState, Literal[True]]
     tableColumns: Incomplete
     tableStyleInfo: Typed[TableStyleInfo, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        id: _ConvertibleToInt = 1,
+        id: ConvertibleToInt = 1,
         displayName: Incomplete | None = None,
         ref: Incomplete | None = None,
         name: str | None = None,
         comment: str | None = None,
         tableType: _TableTableType | Literal["none"] | None = None,
-        headerRowCount: _ConvertibleToInt | None = 1,
+        headerRowCount: ConvertibleToInt | None = 1,
         insertRow: _ConvertibleToBool | None = None,
         insertRowShift: _ConvertibleToBool | None = None,
-        totalsRowCount: _ConvertibleToInt | None = None,
+        totalsRowCount: ConvertibleToInt | None = None,
         totalsRowShown: _ConvertibleToBool | None = None,
         published: _ConvertibleToBool | None = None,
-        headerRowDxfId: _ConvertibleToInt | None = None,
-        dataDxfId: _ConvertibleToInt | None = None,
-        totalsRowDxfId: _ConvertibleToInt | None = None,
-        headerRowBorderDxfId: _ConvertibleToInt | None = None,
-        tableBorderDxfId: _ConvertibleToInt | None = None,
-        totalsRowBorderDxfId: _ConvertibleToInt | None = None,
+        headerRowDxfId: ConvertibleToInt | None = None,
+        dataDxfId: ConvertibleToInt | None = None,
+        totalsRowDxfId: ConvertibleToInt | None = None,
+        headerRowBorderDxfId: ConvertibleToInt | None = None,
+        tableBorderDxfId: ConvertibleToInt | None = None,
+        totalsRowBorderDxfId: ConvertibleToInt | None = None,
         headerRowCellStyle: str | None = None,
         dataCellStyle: str | None = None,
         totalsRowCellStyle: str | None = None,
-        connectionId: _ConvertibleToInt | None = None,
+        connectionId: ConvertibleToInt | None = None,
         autoFilter: AutoFilter | None = None,
         sortState: SortState | None = None,
         tableColumns=(),
         tableStyleInfo: TableStyleInfo | None = None,
         extLst: Unused = None,
     ) -> None: ...
-    def to_tree(self): ...
+    def to_tree(self) -> Element: ...  # type: ignore[override]
     @property
-    def path(self): ...
+    def path(self) -> str: ...
     @property
-    def column_names(self): ...
+    def column_names(self) -> list[str]: ...
 
 class TablePartList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     # Overwritten by property below
     # count: Integer
     tablePart: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     __attrs__: ClassVar[tuple[str, ...]]
     def __init__(self, count: Unused = None, tablePart=()) -> None: ...
     def append(self, part) -> None: ...
     @property
-    def count(self): ...
+    def count(self) -> int: ...
     def __bool__(self) -> bool: ...
 
 class TableList(dict[Incomplete, Incomplete]):
     def add(self, table) -> None: ...
     def get(self, name: Incomplete | None = None, table_range: Incomplete | None = None): ...
     def items(self): ...
```

### Comparing `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/views.pyi` & `types-openpyxl-3.1.2.20240601/openpyxl-stubs/worksheet/views.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
-from typing_extensions import Literal, TypeAlias
-
-from openpyxl.descriptors.base import (
-    Bool,
-    Float,
-    Integer,
-    NoneSet,
-    Set,
-    String,
-    Typed,
-    _ConvertibleToBool,
-    _ConvertibleToFloat,
-    _ConvertibleToInt,
-)
+from _typeshed import ConvertibleToFloat, ConvertibleToInt, Incomplete, Unused
+from typing import ClassVar, Literal
+from typing_extensions import TypeAlias
+
+from openpyxl.descriptors.base import Bool, Float, Integer, NoneSet, Set, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
 _Pane: TypeAlias = Literal["bottomRight", "topRight", "bottomLeft", "topLeft"]
 _SheetViewView: TypeAlias = Literal["normal", "pageBreakPreview", "pageLayout"]
 _PaneState: TypeAlias = Literal["split", "frozen", "frozenSplit"]
 
@@ -25,36 +14,36 @@
     xSplit: Float[Literal[True]]
     ySplit: Float[Literal[True]]
     topLeftCell: String[Literal[True]]
     activePane: Set[_Pane]
     state: Set[_PaneState]
     def __init__(
         self,
-        xSplit: _ConvertibleToFloat | None = None,
-        ySplit: _ConvertibleToFloat | None = None,
+        xSplit: ConvertibleToFloat | None = None,
+        ySplit: ConvertibleToFloat | None = None,
         topLeftCell: str | None = None,
         activePane: _Pane = "topLeft",
         state: _PaneState = "split",
     ) -> None: ...
 
 class Selection(Serialisable):
     pane: NoneSet[_Pane]
     activeCell: String[Literal[True]]
     activeCellId: Integer[Literal[True]]
     sqref: String[Literal[True]]
     def __init__(
         self,
         pane: _Pane | Literal["none"] | None = None,
         activeCell: str | None = "A1",
-        activeCellId: _ConvertibleToInt | None = None,
+        activeCellId: ConvertibleToInt | None = None,
         sqref: str | None = "A1",
     ) -> None: ...
 
 class SheetView(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     windowProtection: Bool[Literal[True]]
     showFormulas: Bool[Literal[True]]
     showGridLines: Bool[Literal[True]]
     showRowColHeaders: Bool[Literal[True]]
     showZeros: Bool[Literal[True]]
     rightToLeft: Bool[Literal[True]]
     tabSelected: Bool[Literal[True]]
@@ -84,24 +73,24 @@
         tabSelected: _ConvertibleToBool | None = None,
         showRuler: _ConvertibleToBool | None = None,
         showOutlineSymbols: _ConvertibleToBool | None = None,
         defaultGridColor: _ConvertibleToBool | None = None,
         showWhiteSpace: _ConvertibleToBool | None = None,
         view: _SheetViewView | Literal["none"] | None = None,
         topLeftCell: str | None = None,
-        colorId: _ConvertibleToInt | None = None,
-        zoomScale: _ConvertibleToInt | None = None,
-        zoomScaleNormal: _ConvertibleToInt | None = None,
-        zoomScaleSheetLayoutView: _ConvertibleToInt | None = None,
-        zoomScalePageLayoutView: _ConvertibleToInt | None = None,
+        colorId: ConvertibleToInt | None = None,
+        zoomScale: ConvertibleToInt | None = None,
+        zoomScaleNormal: ConvertibleToInt | None = None,
+        zoomScaleSheetLayoutView: ConvertibleToInt | None = None,
+        zoomScalePageLayoutView: ConvertibleToInt | None = None,
         zoomToFit: _ConvertibleToBool | None = None,
-        workbookViewId: _ConvertibleToInt | None = 0,
+        workbookViewId: ConvertibleToInt | None = 0,
         selection: Incomplete | None = None,
         pane: Pane | None = None,
     ) -> None: ...
 
 class SheetViewList(Serialisable):
-    tagname: str
+    tagname: ClassVar[str]
     sheetView: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, sheetView: Incomplete | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.9/setup.py` & `types-openpyxl-3.1.2.20240601/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from setuptools import setup
 
 name = "types-openpyxl"
 description = "Typing stubs for openpyxl"
 long_description = '''
 ## Typing stubs for openpyxl
 
-This is a PEP 561 type stub package for the `openpyxl` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`openpyxl`](https://foss.heptapod.net/openpyxl/openpyxl) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`openpyxl`. The source for this package can be found at
+`openpyxl`.
+
+This version of `types-openpyxl` aims to provide accurate annotations
+for `openpyxl==3.1.2`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8c582c4459cc3e7c67531cd90bfd6cef5b71c7d3`.
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.1.0.9",
+      version="3.1.2.20240601",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['openpyxl-stubs'],
-      package_data={'openpyxl-stubs': ['__init__.pyi', '_constants.pyi', 'cell/__init__.pyi', 'cell/_writer.pyi', 'cell/cell.pyi', 'cell/read_only.pyi', 'cell/rich_text.pyi', 'cell/text.pyi', 'chart/_3d.pyi', 'chart/__init__.pyi', 'chart/_chart.pyi', 'chart/area_chart.pyi', 'chart/axis.pyi', 'chart/bar_chart.pyi', 'chart/bubble_chart.pyi', 'chart/chartspace.pyi', 'chart/data_source.pyi', 'chart/descriptors.pyi', 'chart/error_bar.pyi', 'chart/label.pyi', 'chart/layout.pyi', 'chart/legend.pyi', 'chart/line_chart.pyi', 'chart/marker.pyi', 'chart/picture.pyi', 'chart/pie_chart.pyi', 'chart/pivot.pyi', 'chart/plotarea.pyi', 'chart/print_settings.pyi', 'chart/radar_chart.pyi', 'chart/reader.pyi', 'chart/reference.pyi', 'chart/scatter_chart.pyi', 'chart/series.pyi', 'chart/series_factory.pyi', 'chart/shapes.pyi', 'chart/stock_chart.pyi', 'chart/surface_chart.pyi', 'chart/text.pyi', 'chart/title.pyi', 'chart/trendline.pyi', 'chart/updown_bars.pyi', 'chartsheet/__init__.pyi', 'chartsheet/chartsheet.pyi', 'chartsheet/custom.pyi', 'chartsheet/properties.pyi', 'chartsheet/protection.pyi', 'chartsheet/publish.pyi', 'chartsheet/relation.pyi', 'chartsheet/views.pyi', 'comments/__init__.pyi', 'comments/author.pyi', 'comments/comment_sheet.pyi', 'comments/comments.pyi', 'comments/shape_writer.pyi', 'compat/__init__.pyi', 'compat/abc.pyi', 'compat/numbers.pyi', 'compat/product.pyi', 'compat/singleton.pyi', 'compat/strings.pyi', 'descriptors/__init__.pyi', 'descriptors/base.pyi', 'descriptors/excel.pyi', 'descriptors/namespace.pyi', 'descriptors/nested.pyi', 'descriptors/sequence.pyi', 'descriptors/serialisable.pyi', 'descriptors/slots.pyi', 'drawing/__init__.pyi', 'drawing/colors.pyi', 'drawing/connector.pyi', 'drawing/drawing.pyi', 'drawing/effect.pyi', 'drawing/fill.pyi', 'drawing/geometry.pyi', 'drawing/graphic.pyi', 'drawing/image.pyi', 'drawing/line.pyi', 'drawing/picture.pyi', 'drawing/properties.pyi', 'drawing/relation.pyi', 'drawing/spreadsheet_drawing.pyi', 'drawing/text.pyi', 'drawing/xdr.pyi', 'formatting/__init__.pyi', 'formatting/formatting.pyi', 'formatting/rule.pyi', 'formula/__init__.pyi', 'formula/tokenizer.pyi', 'formula/translate.pyi', 'packaging/__init__.pyi', 'packaging/core.pyi', 'packaging/custom.pyi', 'packaging/extended.pyi', 'packaging/interface.pyi', 'packaging/manifest.pyi', 'packaging/relationship.pyi', 'packaging/workbook.pyi', 'pivot/__init__.pyi', 'pivot/cache.pyi', 'pivot/fields.pyi', 'pivot/record.pyi', 'pivot/table.pyi', 'reader/__init__.pyi', 'reader/drawings.pyi', 'reader/excel.pyi', 'reader/strings.pyi', 'reader/workbook.pyi', 'styles/__init__.pyi', 'styles/alignment.pyi', 'styles/borders.pyi', 'styles/builtins.pyi', 'styles/cell_style.pyi', 'styles/colors.pyi', 'styles/differential.pyi', 'styles/fills.pyi', 'styles/fonts.pyi', 'styles/named_styles.pyi', 'styles/numbers.pyi', 'styles/protection.pyi', 'styles/proxy.pyi', 'styles/styleable.pyi', 'styles/stylesheet.pyi', 'styles/table.pyi', 'utils/__init__.pyi', 'utils/bound_dictionary.pyi', 'utils/cell.pyi', 'utils/dataframe.pyi', 'utils/datetime.pyi', 'utils/escape.pyi', 'utils/exceptions.pyi', 'utils/formulas.pyi', 'utils/indexed_list.pyi', 'utils/inference.pyi', 'utils/protection.pyi', 'utils/units.pyi', 'workbook/__init__.pyi', 'workbook/_writer.pyi', 'workbook/child.pyi', 'workbook/defined_name.pyi', 'workbook/external_link/__init__.pyi', 'workbook/external_link/external.pyi', 'workbook/external_reference.pyi', 'workbook/function_group.pyi', 'workbook/properties.pyi', 'workbook/protection.pyi', 'workbook/smart_tags.pyi', 'workbook/views.pyi', 'workbook/web.pyi', 'workbook/workbook.pyi', 'worksheet/__init__.pyi', 'worksheet/_read_only.pyi', 'worksheet/_reader.pyi', 'worksheet/_write_only.pyi', 'worksheet/_writer.pyi', 'worksheet/cell_range.pyi', 'worksheet/cell_watch.pyi', 'worksheet/controls.pyi', 'worksheet/copier.pyi', 'worksheet/custom.pyi', 'worksheet/datavalidation.pyi', 'worksheet/dimensions.pyi', 'worksheet/drawing.pyi', 'worksheet/errors.pyi', 'worksheet/filters.pyi', 'worksheet/formula.pyi', 'worksheet/header_footer.pyi', 'worksheet/hyperlink.pyi', 'worksheet/merge.pyi', 'worksheet/ole.pyi', 'worksheet/page.pyi', 'worksheet/pagebreak.pyi', 'worksheet/picture.pyi', 'worksheet/print_settings.pyi', 'worksheet/properties.pyi', 'worksheet/protection.pyi', 'worksheet/related.pyi', 'worksheet/scenario.pyi', 'worksheet/smart_tag.pyi', 'worksheet/table.pyi', 'worksheet/views.pyi', 'worksheet/worksheet.pyi', 'writer/__init__.pyi', 'writer/excel.pyi', 'writer/theme.pyi', 'xml/__init__.pyi', 'xml/constants.pyi', 'xml/functions.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'openpyxl-stubs': ['__init__.pyi', '_constants.pyi', 'cell/__init__.pyi', 'cell/_writer.pyi', 'cell/cell.pyi', 'cell/read_only.pyi', 'cell/rich_text.pyi', 'cell/text.pyi', 'chart/_3d.pyi', 'chart/__init__.pyi', 'chart/_chart.pyi', 'chart/area_chart.pyi', 'chart/axis.pyi', 'chart/bar_chart.pyi', 'chart/bubble_chart.pyi', 'chart/chartspace.pyi', 'chart/data_source.pyi', 'chart/descriptors.pyi', 'chart/error_bar.pyi', 'chart/label.pyi', 'chart/layout.pyi', 'chart/legend.pyi', 'chart/line_chart.pyi', 'chart/marker.pyi', 'chart/picture.pyi', 'chart/pie_chart.pyi', 'chart/pivot.pyi', 'chart/plotarea.pyi', 'chart/print_settings.pyi', 'chart/radar_chart.pyi', 'chart/reader.pyi', 'chart/reference.pyi', 'chart/scatter_chart.pyi', 'chart/series.pyi', 'chart/series_factory.pyi', 'chart/shapes.pyi', 'chart/stock_chart.pyi', 'chart/surface_chart.pyi', 'chart/text.pyi', 'chart/title.pyi', 'chart/trendline.pyi', 'chart/updown_bars.pyi', 'chartsheet/__init__.pyi', 'chartsheet/chartsheet.pyi', 'chartsheet/custom.pyi', 'chartsheet/properties.pyi', 'chartsheet/protection.pyi', 'chartsheet/publish.pyi', 'chartsheet/relation.pyi', 'chartsheet/views.pyi', 'comments/__init__.pyi', 'comments/author.pyi', 'comments/comment_sheet.pyi', 'comments/comments.pyi', 'comments/shape_writer.pyi', 'compat/__init__.pyi', 'compat/abc.pyi', 'compat/numbers.pyi', 'compat/product.pyi', 'compat/singleton.pyi', 'compat/strings.pyi', 'descriptors/__init__.pyi', 'descriptors/base.pyi', 'descriptors/excel.pyi', 'descriptors/namespace.pyi', 'descriptors/nested.pyi', 'descriptors/sequence.pyi', 'descriptors/serialisable.pyi', 'descriptors/slots.pyi', 'drawing/__init__.pyi', 'drawing/colors.pyi', 'drawing/connector.pyi', 'drawing/drawing.pyi', 'drawing/effect.pyi', 'drawing/fill.pyi', 'drawing/geometry.pyi', 'drawing/graphic.pyi', 'drawing/image.pyi', 'drawing/line.pyi', 'drawing/picture.pyi', 'drawing/properties.pyi', 'drawing/relation.pyi', 'drawing/spreadsheet_drawing.pyi', 'drawing/text.pyi', 'drawing/xdr.pyi', 'formatting/__init__.pyi', 'formatting/formatting.pyi', 'formatting/rule.pyi', 'formula/__init__.pyi', 'formula/tokenizer.pyi', 'formula/translate.pyi', 'packaging/__init__.pyi', 'packaging/core.pyi', 'packaging/custom.pyi', 'packaging/extended.pyi', 'packaging/interface.pyi', 'packaging/manifest.pyi', 'packaging/relationship.pyi', 'packaging/workbook.pyi', 'pivot/__init__.pyi', 'pivot/cache.pyi', 'pivot/fields.pyi', 'pivot/record.pyi', 'pivot/table.pyi', 'reader/__init__.pyi', 'reader/drawings.pyi', 'reader/excel.pyi', 'reader/strings.pyi', 'reader/workbook.pyi', 'styles/__init__.pyi', 'styles/alignment.pyi', 'styles/borders.pyi', 'styles/builtins.pyi', 'styles/cell_style.pyi', 'styles/colors.pyi', 'styles/differential.pyi', 'styles/fills.pyi', 'styles/fonts.pyi', 'styles/named_styles.pyi', 'styles/numbers.pyi', 'styles/protection.pyi', 'styles/proxy.pyi', 'styles/styleable.pyi', 'styles/stylesheet.pyi', 'styles/table.pyi', 'utils/__init__.pyi', 'utils/bound_dictionary.pyi', 'utils/cell.pyi', 'utils/dataframe.pyi', 'utils/datetime.pyi', 'utils/escape.pyi', 'utils/exceptions.pyi', 'utils/formulas.pyi', 'utils/indexed_list.pyi', 'utils/inference.pyi', 'utils/protection.pyi', 'utils/units.pyi', 'workbook/__init__.pyi', 'workbook/_writer.pyi', 'workbook/child.pyi', 'workbook/defined_name.pyi', 'workbook/external_link/__init__.pyi', 'workbook/external_link/external.pyi', 'workbook/external_reference.pyi', 'workbook/function_group.pyi', 'workbook/properties.pyi', 'workbook/protection.pyi', 'workbook/smart_tags.pyi', 'workbook/views.pyi', 'workbook/web.pyi', 'workbook/workbook.pyi', 'worksheet/__init__.pyi', 'worksheet/_read_only.pyi', 'worksheet/_reader.pyi', 'worksheet/_write_only.pyi', 'worksheet/_writer.pyi', 'worksheet/cell_range.pyi', 'worksheet/cell_watch.pyi', 'worksheet/controls.pyi', 'worksheet/copier.pyi', 'worksheet/custom.pyi', 'worksheet/datavalidation.pyi', 'worksheet/dimensions.pyi', 'worksheet/drawing.pyi', 'worksheet/errors.pyi', 'worksheet/filters.pyi', 'worksheet/formula.pyi', 'worksheet/header_footer.pyi', 'worksheet/hyperlink.pyi', 'worksheet/merge.pyi', 'worksheet/ole.pyi', 'worksheet/page.pyi', 'worksheet/pagebreak.pyi', 'worksheet/picture.pyi', 'worksheet/print_settings.pyi', 'worksheet/properties.pyi', 'worksheet/protection.pyi', 'worksheet/related.pyi', 'worksheet/scenario.pyi', 'worksheet/smart_tag.pyi', 'worksheet/table.pyi', 'worksheet/views.pyi', 'worksheet/worksheet.pyi', 'writer/__init__.pyi', 'writer/excel.pyi', 'writer/theme.pyi', 'xml/__init__.pyi', 'xml/_functions_overloads.pyi', 'xml/constants.pyi', 'xml/functions.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-openpyxl-3.1.0.9/types_openpyxl.egg-info/PKG-INFO` & `types-openpyxl-3.1.2.20240601/types_openpyxl.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.9
+Version: 3.1.2.20240601
 Summary: Typing stubs for openpyxl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for openpyxl
 
-This is a PEP 561 type stub package for the `openpyxl` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`openpyxl`](https://foss.heptapod.net/openpyxl/openpyxl) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`openpyxl`. The source for this package can be found at
+`openpyxl`.
+
+This version of `types-openpyxl` aims to provide accurate annotations
+for `openpyxl==3.1.2`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `8c582c4459cc3e7c67531cd90bfd6cef5b71c7d3`.
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
+pytype 2024.4.11.
```

### Comparing `types-openpyxl-3.1.0.9/types_openpyxl.egg-info/SOURCES.txt` & `types-openpyxl-3.1.2.20240601/types_openpyxl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CHANGELOG.md
 MANIFEST.in
 setup.py
 openpyxl-stubs/METADATA.toml
 openpyxl-stubs/__init__.pyi
 openpyxl-stubs/_constants.pyi
+openpyxl-stubs/py.typed
 openpyxl-stubs/cell/__init__.pyi
 openpyxl-stubs/cell/_writer.pyi
 openpyxl-stubs/cell/cell.pyi
 openpyxl-stubs/cell/read_only.pyi
 openpyxl-stubs/cell/rich_text.pyi
 openpyxl-stubs/cell/text.pyi
 openpyxl-stubs/chart/_3d.pyi
@@ -185,13 +186,14 @@
 openpyxl-stubs/worksheet/table.pyi
 openpyxl-stubs/worksheet/views.pyi
 openpyxl-stubs/worksheet/worksheet.pyi
 openpyxl-stubs/writer/__init__.pyi
 openpyxl-stubs/writer/excel.pyi
 openpyxl-stubs/writer/theme.pyi
 openpyxl-stubs/xml/__init__.pyi
+openpyxl-stubs/xml/_functions_overloads.pyi
 openpyxl-stubs/xml/constants.pyi
 openpyxl-stubs/xml/functions.pyi
 types_openpyxl.egg-info/PKG-INFO
 types_openpyxl.egg-info/SOURCES.txt
 types_openpyxl.egg-info/dependency_links.txt
 types_openpyxl.egg-info/top_level.txt
```

