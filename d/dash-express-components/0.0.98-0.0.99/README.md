# Comparing `tmp/dash_express_components-0.0.98.tar.gz` & `tmp/dash_express_components-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_express_components-0.0.98.tar", last modified: Thu May 30 13:10:53 2024, max compression
+gzip compressed data, was "dash_express_components-0.0.99.tar", last modified: Sat Jun  1 17:06:16 2024, max compression
```

## Comparing `dash_express_components-0.0.98.tar` & `dash_express_components-0.0.99.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.310763 dash_express_components-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-30 13:10:53.306763 dash_express_components-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.298763 dash_express_components-0.0.98/dash_express_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/AggrTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/AsType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/BarCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/BinTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/CategoryLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/CombinecatTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/ConfigReceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/CoreGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/DropnaTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/EvalTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/FilterIqrTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/GroupedSample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/HistogramLine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Localstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/MeltTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/MetaCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Parameterize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/PlotterBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/RenameTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/RequestStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/ScatterMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/StrSplitTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/SubComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Violin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/WideToLong.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/ZerosToNanTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (127)  1163624 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/async-excel.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/async-excel.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   722247 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/dash_express_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/dash_express_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    95280 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/package-info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.298763 dash_express_components-0.0.98/dash_express_components/plottypes/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_bar_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_histogram_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.302763 dash_express_components-0.0.98/dash_express_components/transformationtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_aggr.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_asType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_catlookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_combinecat.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_dropna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_groupby_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_iqrfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_melt.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_strsplit.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_wide_to_long.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_zerostonan.py
--rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.298763 dash_express_components-0.0.98/dash_express_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-30 13:10:53.000000 dash_express_components-0.0.98/dash_express_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.302763 dash_express_components-0.0.98/dash_express_components_base/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.306763 dash_express_components-0.0.98/dash_express_components_base/plottypes/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_bar_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_histogram_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.306763 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_aggr.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_asType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_catlookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_combinecat.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_dropna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_groupby_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_iqrfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_melt.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_strsplit.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_wide_to_long.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_zerostonan.py
--rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:10:53.310763 dash_express_components-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:06:16.619514 dash_express_components-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-06-01 17:06:16.619514 dash_express_components-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:06:16.611513 dash_express_components-0.0.99/dash_express_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/AggrTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/AsType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/BarCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/BinTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/CategoryLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/CombinecatTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/ConfigReceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/CoreGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/DataGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/DropnaTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/EvalTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/FilterIqrTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/GroupedSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/HistogramLine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Localstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/MeltTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/MetaCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/PlotterBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/RenameTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/RequestStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/ScatterMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/StrSplitTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/SubComponentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/Violin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/WideToLong.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/ZerosToNanTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1163624 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/async-excel.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/async-excel.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   732247 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/dash_express_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/dash_express_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    97625 2024-06-01 17:06:15.000000 dash_express_components-0.0.99/dash_express_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-06-01 17:06:14.000000 dash_express_components-0.0.99/dash_express_components/package-info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:06:16.611513 dash_express_components-0.0.99/dash_express_components/plottypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/plottypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/plottypes/_bar_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/plottypes/_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/plottypes/_histogram_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/plottypes/_imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/plottypes/_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/plottypes/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/plottypes/_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:06:16.615514 dash_express_components-0.0.99/dash_express_components/transformationtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_aggr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_asType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_catlookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_combinecat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_dropna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_groupby_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_iqrfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_melt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_strsplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_wide_to_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/transformationtypes/_zerostonan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-06-01 17:06:13.000000 dash_express_components-0.0.99/dash_express_components/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:06:16.611513 dash_express_components-0.0.99/dash_express_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-06-01 17:06:16.000000 dash_express_components-0.0.99/dash_express_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-06-01 17:06:16.000000 dash_express_components-0.0.99/dash_express_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:06:16.000000 dash_express_components-0.0.99/dash_express_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 17:06:16.000000 dash_express_components-0.0.99/dash_express_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 17:06:16.000000 dash_express_components-0.0.99/dash_express_components.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:06:16.615514 dash_express_components-0.0.99/dash_express_components_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:06:16.615514 dash_express_components-0.0.99/dash_express_components_base/plottypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/plottypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/plottypes/_bar_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/plottypes/_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/plottypes/_histogram_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/plottypes/_imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/plottypes/_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/plottypes/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/plottypes/_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:06:16.619514 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_aggr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_asType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_catlookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_combinecat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_dropna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_groupby_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_iqrfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_melt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_strsplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_wide_to_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_zerostonan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/dash_express_components_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:06:16.619514 dash_express_components-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-06-01 17:04:58.000000 dash_express_components-0.0.99/setup.py
```

### Comparing `dash_express_components-0.0.98/PKG-INFO` & `dash_express_components-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_express_components
-Version: 0.0.98
+Version: 0.0.99
 Summary: Simple widgets to add plotly express style plotting to dash
 Home-page: https://github.com/VK/dash-express-components
 Author: Viktor Krückl <viktor@krueckl.de>
 License: MIT
 Description: # Dash Express Components
         ![Publish release](https://github.com/VK/dash-express-components/workflows/Publish%20release/badge.svg)
         [![PyPI](https://img.shields.io/pypi/v/dash-express-components?logo=pypi)](https://pypi.org/project/dash-express-components)
```

### Comparing `dash_express_components-0.0.98/README.md` & `dash_express_components-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/AggrTransform.py` & `dash_express_components-0.0.99/dash_express_components/AggrTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/AsType.py` & `dash_express_components-0.0.99/dash_express_components/AsType.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Bar.py` & `dash_express_components-0.0.99/dash_express_components/Bar.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/BarCount.py` & `dash_express_components-0.0.99/dash_express_components/BarCount.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Base.py` & `dash_express_components-0.0.99/dash_express_components/Base.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/BinTransform.py` & `dash_express_components-0.0.99/dash_express_components/BinTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Box.py` & `dash_express_components-0.0.99/dash_express_components/Box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/CategoryLookup.py` & `dash_express_components-0.0.99/dash_express_components/CategoryLookup.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/CombinecatTransform.py` & `dash_express_components-0.0.99/dash_express_components/CombinecatTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/ConfigReceiver.py` & `dash_express_components-0.0.99/dash_express_components/ConfigReceiver.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Configurator.py` & `dash_express_components-0.0.99/dash_express_components/Configurator.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/CoreGraph.py` & `dash_express_components-0.0.99/dash_express_components/CoreGraph.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/DropnaTransform.py` & `dash_express_components-0.0.99/dash_express_components/DropnaTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/EvalTransform.py` & `dash_express_components-0.0.99/dash_express_components/EvalTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Filter.py` & `dash_express_components-0.0.99/dash_express_components/Filter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/FilterIqrTransform.py` & `dash_express_components-0.0.99/dash_express_components/FilterIqrTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Graph.py` & `dash_express_components-0.0.99/dash_express_components/Graph.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/GroupedSample.py` & `dash_express_components-0.0.99/dash_express_components/GroupedSample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/HistogramLine.py` & `dash_express_components-0.0.99/dash_express_components/HistogramLine.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Imshow.py` & `dash_express_components-0.0.99/dash_express_components/Imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Localstore.py` & `dash_express_components-0.0.99/dash_express_components/Localstore.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/MeltTransform.py` & `dash_express_components-0.0.99/dash_express_components/MeltTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/MetaCheck.py` & `dash_express_components-0.0.99/dash_express_components/MetaCheck.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Parameterize.py` & `dash_express_components-0.0.99/dash_express_components/Parameterize.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Plotter.py` & `dash_express_components-0.0.99/dash_express_components/Plotter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/PlotterBase.py` & `dash_express_components-0.0.99/dash_express_components/PlotterBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Probability.py` & `dash_express_components-0.0.99/dash_express_components/Probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/RenameTransform.py` & `dash_express_components-0.0.99/dash_express_components/RenameTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/RequestStore.py` & `dash_express_components-0.0.99/dash_express_components/RequestStore.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Scatter.py` & `dash_express_components-0.0.99/dash_express_components/Scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/ScatterMatrix.py` & `dash_express_components-0.0.99/dash_express_components/ScatterMatrix.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/StrSplitTransform.py` & `dash_express_components-0.0.99/dash_express_components/StrSplitTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/SubComponentBase.py` & `dash_express_components-0.0.99/dash_express_components/SubComponentBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Table.py` & `dash_express_components-0.0.99/dash_express_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Transform.py` & `dash_express_components-0.0.99/dash_express_components/Transform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/Violin.py` & `dash_express_components-0.0.99/dash_express_components/Violin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/WideToLong.py` & `dash_express_components-0.0.99/dash_express_components/WideToLong.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/ZerosToNanTransform.py` & `dash_express_components-0.0.99/dash_express_components/ZerosToNanTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/__init__.py` & `dash_express_components-0.0.99/dash_express_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/_imports_.py` & `dash_express_components-0.0.99/dash_express_components/_imports_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .ConfigReceiver import ConfigReceiver
 from .Configurator import Configurator
+from .DataGraph import DataGraph
 from .Filter import Filter
 from .Graph import Graph
 from .Localstore import Localstore
 from .MetaCheck import MetaCheck
 from .Parameterize import Parameterize
 from .Plotter import Plotter
 from .RequestStore import RequestStore
@@ -36,14 +37,15 @@
 from .SubComponentBase import SubComponentBase
 from .WideToLong import WideToLong
 from .ZerosToNanTransform import ZerosToNanTransform
 
 __all__ = [
     "ConfigReceiver",
     "Configurator",
+    "DataGraph",
     "Filter",
     "Graph",
     "Localstore",
     "MetaCheck",
     "Parameterize",
     "Plotter",
     "RequestStore",
```

### Comparing `dash_express_components-0.0.98/dash_express_components/async-excel.js` & `dash_express_components-0.0.99/dash_express_components/async-excel.js`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/dash_express_components.min.js` & `dash_express_components-0.0.99/dash_express_components/dash_express_components.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(l()),
                 n = c(e);
             if (!t) return n;
             var r = n.split("/"),
                 a = r.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_98m1717074633"), r.splice(-1, 1, a.join(".")), r.join("/")
+            return a.splice(1, 0, "v0_0_99m1717261557"), r.splice(-1, 1, a.join(".")), r.join("/")
         }
     }
     var u = window.webpackJsonpdash_express_components = window.webpackJsonpdash_express_components || [],
         s = u.push.bind(u);
     u.push = t, u = u.slice();
     for (var f = 0; f < u.length; f++) t(u[f]);
     var p = s;
@@ -245,33 +245,33 @@
     })), n.d(t, "getPreviousCenturyStart", (function() {
         return h
     })), n.d(t, "getNextCenturyStart", (function() {
         return m
     })), n.d(t, "getCenturyEnd", (function() {
         return b
     })), n.d(t, "getPreviousCenturyEnd", (function() {
-        return v
-    })), n.d(t, "getNextCenturyEnd", (function() {
         return y
+    })), n.d(t, "getNextCenturyEnd", (function() {
+        return v
     })), n.d(t, "getCenturyRange", (function() {
         return g
     })), n.d(t, "getDecadeStart", (function() {
         return O
     })), n.d(t, "getPreviousDecadeStart", (function() {
         return _
     })), n.d(t, "getNextDecadeStart", (function() {
         return w
     })), n.d(t, "getDecadeEnd", (function() {
         return E
     })), n.d(t, "getPreviousDecadeEnd", (function() {
         return j
     })), n.d(t, "getNextDecadeEnd", (function() {
-        return M
-    })), n.d(t, "getDecadeRange", (function() {
         return k
+    })), n.d(t, "getDecadeRange", (function() {
+        return M
     })), n.d(t, "getYearStart", (function() {
         return P
     })), n.d(t, "getPreviousYearStart", (function() {
         return x
     })), n.d(t, "getNextYearStart", (function() {
         return S
     })), n.d(t, "getYearEnd", (function() {
@@ -303,17 +303,17 @@
     })), n.d(t, "getNextDayStart", (function() {
         return U
     })), n.d(t, "getDayEnd", (function() {
         return K
     })), n.d(t, "getPreviousDayEnd", (function() {
         return Y
     })), n.d(t, "getNextDayEnd", (function() {
-        return Q
-    })), n.d(t, "getDayRange", (function() {
         return G
+    })), n.d(t, "getDayRange", (function() {
+        return Q
     })), n.d(t, "getDaysInMonth", (function() {
         return J
     })), n.d(t, "getHoursMinutes", (function() {
         return X
     })), n.d(t, "getHoursMinutesSeconds", (function() {
         return $
     })), n.d(t, "getISOLocalMonth", (function() {
@@ -322,30 +322,30 @@
         return te
     })), n.d(t, "getISOLocalDateTime", (function() {
         return ne
     }));
     var h = r(i, d, -100),
         m = r(i, d, 100),
         b = a(m),
-        v = r(i, b, -100),
-        y = r(i, b, 100),
+        y = r(i, b, -100),
+        v = r(i, b, 100),
         g = o([d, b]);
 
     function O(e) {
         var t = i(e),
             n = t + (1 - t) % 10,
             r = new Date;
         return r.setFullYear(n, 0, 1), r.setHours(0, 0, 0, 0), r
     }
     var _ = r(i, O, -10),
         w = r(i, O, 10),
         E = a(w),
         j = r(i, E, -10),
-        M = r(i, E, 10),
-        k = o([O, E]);
+        k = r(i, E, 10),
+        M = o([O, E]);
 
     function P(e) {
         var t = i(e),
             n = new Date;
         return n.setFullYear(t, 0, 1), n.setHours(0, 0, 0, 0), n
     }
     var x = r(i, P, -1),
@@ -396,16 +396,16 @@
             a = new Date;
         return a.setFullYear(t, n, r), a.setHours(0, 0, 0, 0), a
     }
     var V = F(W, -1),
         U = F(W, 1),
         K = a(U),
         Y = F(K, -1),
-        Q = F(K, 1),
-        G = o([W, K]);
+        G = F(K, 1),
+        Q = o([W, K]);
 
     function J(e) {
         return u(H(e))
     }
 
     function Z(e) {
         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 2,
@@ -552,31 +552,31 @@
         return n
     }
 
     function b(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
             t % 2 ? m(Object(n), !0).forEach((function(t) {
-                v(e, t, n[t])
+                y(e, t, n[t])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : m(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function v(e, t, n) {
+    function y(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    var y = function() {
+    var v = function() {
             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "transparent";
             return {
                 alignItems: "center",
                 display: "flex",
                 ":before": {
                     backgroundColor: e,
                     borderRadius: 10,
@@ -621,15 +621,15 @@
                         label: t,
                         value: t,
                         color: "#555555"
                     };
                     var t, n
                 })) : [],
                 onChange: function(e) {
-                    e && void 0 !== e && Array.isArray(e) && t(v({}, n, e.map((function(e) {
+                    e && void 0 !== e && Array.isArray(e) && t(y({}, n, e.map((function(e) {
                         return e.value
                     }))))
                 },
                 onInputChange: function(e, o) {
                     var i = o.action,
                         l = (o.prevInputValue, e.length > 0 ? e[e.length - 1] : "");
                     if ("input-change" === i && e && void 0 !== e && [" ", "\n", "\t"].includes(l)) {
@@ -642,15 +642,15 @@
                                     return e === t.label.toUpperCase()
                                 })).map((function(e) {
                                     return e.value
                                 })).filter((function(e) {
                                     return !a.includes(e)
                                 }));
                                 1 == t.length && u.push(t[0])
-                            })), u.length > 0) return t(v({}, n, [].concat(d(a), u))), ""
+                            })), u.length > 0) return t(y({}, n, [].concat(d(a), u))), ""
                     }
                 },
                 isMulti: !0,
                 closeMenuOnSelect: !1
             }
         },
         _ = {
@@ -690,22 +690,22 @@
                     cursor: r ? "not-allowed" : "default",
                     ":active": b(b({}, e[":active"]), {}, {
                         backgroundColor: r ? void 0 : i ? n.color : l.alpha(.3).css()
                     })
                 })
             },
             input: function(e) {
-                return b(b({}, e), y())
+                return b(b({}, e), v())
             },
             placeholder: function(e) {
-                return b(b({}, e), y("#ccc"))
+                return b(b({}, e), v("#ccc"))
             },
             singleValue: function(e, t) {
                 var n = t.data;
-                return b(b({}, e), y(n.color))
+                return b(b({}, e), v(n.color))
             }
         },
         w = {
             control: function(e) {
                 return b(b({}, e), {}, {
                     backgroundColor: "white"
                 })
@@ -1056,22 +1056,22 @@
 
     function b(e) {
         return (b = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
 
-    function v(e, t) {
+    function y(e, t) {
         return !t || "object" != typeof t && "function" != typeof t ? function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e) : t
     }
 
-    function y(e) {
+    function v(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -1080,15 +1080,15 @@
         }();
         return function() {
             var n, r = b(e);
             if (t) {
                 var a = b(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
-            return v(this, n)
+            return y(this, n)
         }
     }
     n.d(t, "a", (function() {
         return R
     })), n.d(t, "b", (function() {
         return B
     })), n.d(t, "c", (function() {
@@ -1098,25 +1098,25 @@
     })), n.d(t, "e", (function() {
         return w
     })), n.d(t, "f", (function() {
         return Ne
     })), n.d(t, "g", (function() {
         return I
     })), n.d(t, "h", (function() {
-        return M
+        return k
     })), n.d(t, "i", (function() {
         return E
     })), n.d(t, "j", (function() {
         return A
     })), n.d(t, "k", (function() {
         return O
     })), n.d(t, "l", (function() {
         return U
     })), n.d(t, "m", (function() {
-        return y
+        return v
     })), n.d(t, "n", (function() {
         return m
     })), n.d(t, "o", (function() {
         return de
     })), n.d(t, "p", (function() {
         return Te
     })), n.d(t, "q", (function() {
@@ -1134,15 +1134,15 @@
     })), n.d(t, "w", (function() {
         return he
     })), n.d(t, "x", (function() {
         return je
     })), n.d(t, "y", (function() {
         return be
     })), n.d(t, "z", (function() {
-        return G
+        return Q
     })), n.d(t, "A", (function() {
         return W
     })), n.d(t, "B", (function() {
         return K
     })), n.d(t, "C", (function() {
         return $
     })), n.d(t, "D", (function() {
@@ -1150,15 +1150,15 @@
     })), n.d(t, "E", (function() {
         return Se
     })), n.d(t, "F", (function() {
         return N
     })), n.d(t, "G", (function() {
         return Ae
     })), n.d(t, "H", (function() {
-        return Q
+        return G
     })), n.d(t, "I", (function() {
         return Re
     })), n.d(t, "J", (function() {
         return ze
     })), n.d(t, "K", (function() {
         return De
     })), n.d(t, "L", (function() {
@@ -1187,34 +1187,34 @@
             return t = e, Array.isArray(t) ? e.filter(Boolean) : "object" === i(e) && null !== e ? [e] : [];
             var t
         },
         j = function(e) {
             return e.className, e.clearValue, e.cx, e.getStyles, e.getValue, e.hasValue, e.isMulti, e.isRtl, e.options, e.selectOption, e.selectProps, e.setValue, e.theme, m({}, Object(o.a)(e, g))
         };
 
-    function M(e) {
+    function k(e) {
         return [document.documentElement, document.body, window].indexOf(e) > -1
     }
 
-    function k(e) {
-        return M(e) ? window.pageYOffset : e.scrollTop
+    function M(e) {
+        return k(e) ? window.pageYOffset : e.scrollTop
     }
 
     function P(e, t) {
-        M(e) ? window.scrollTo(0, t) : e.scrollTop = t
+        k(e) ? window.scrollTo(0, t) : e.scrollTop = t
     }
 
     function x(e, t, n, r) {
         return n * ((e = e / r - 1) * e * e + 1) + t
     }
 
     function S(e, t) {
         var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 200,
             r = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : O,
-            a = k(e),
+            a = M(e),
             o = t - a,
             i = 10,
             l = 0;
 
         function c() {
             var t = x(l += i, a, o, n);
             P(e, t), l < n ? window.requestAnimationFrame(c) : r(e)
@@ -1295,63 +1295,63 @@
         var s = c.getBoundingClientRect().height,
             f = n.getBoundingClientRect(),
             p = f.bottom,
             d = f.height,
             h = f.top,
             m = n.offsetParent.getBoundingClientRect().top,
             b = window.innerHeight,
-            v = k(c),
-            y = parseInt(getComputedStyle(n).marginBottom, 10),
+            y = M(c),
+            v = parseInt(getComputedStyle(n).marginBottom, 10),
             g = parseInt(getComputedStyle(n).marginTop, 10),
             O = m - g,
             _ = b - h,
-            w = O + v,
-            E = s - v - h,
-            j = p - b + v + y,
-            M = v + h - g;
+            w = O + y,
+            E = s - y - h,
+            j = p - b + y + v,
+            k = y + h - g;
         switch (a) {
             case "auto":
             case "bottom":
                 if (_ >= d) return {
                     placement: "bottom",
                     maxHeight: t
                 };
                 if (E >= d && !i) return o && S(c, j, 160), {
                     placement: "bottom",
                     maxHeight: t
                 };
                 if (!i && E >= r || i && _ >= r) return o && S(c, j, 160), {
                     placement: "bottom",
-                    maxHeight: i ? _ - y : E - y
+                    maxHeight: i ? _ - v : E - v
                 };
                 if ("auto" === a || i) {
                     var x = t,
                         A = i ? O : w;
-                    return A >= r && (x = Math.min(A - y - l.controlHeight, t)), {
+                    return A >= r && (x = Math.min(A - v - l.controlHeight, t)), {
                         placement: "top",
                         maxHeight: x
                     }
                 }
                 if ("bottom" === a) return o && P(c, j), {
                     placement: "bottom",
                     maxHeight: t
                 };
                 break;
             case "top":
                 if (O >= d) return {
                     placement: "top",
                     maxHeight: t
                 };
-                if (w >= d && !i) return o && S(c, M, 160), {
+                if (w >= d && !i) return o && S(c, k, 160), {
                     placement: "top",
                     maxHeight: t
                 };
                 if (!i && w >= r || i && O >= r) {
                     var C = t;
-                    return (!i && w >= r || i && O >= r) && (C = i ? O - g : w - g), o && S(c, M, 160), {
+                    return (!i && w >= r || i && O >= r) && (C = i ? O - g : w - g), o && S(c, k, 160), {
                         placement: "top",
                         maxHeight: C
                     }
                 }
                 return {
                     placement: "bottom", maxHeight: t
                 };
@@ -1379,15 +1379,15 @@
             }(n), "100%"), s(t, "backgroundColor", i.neutral0), s(t, "borderRadius", a), s(t, "boxShadow", "0 0 0 1px hsla(0, 0%, 0%, 0.1), 0 4px 11px hsla(0, 0%, 0%, 0.1)"), s(t, "marginBottom", o.menuGutter), s(t, "marginTop", o.menuGutter), s(t, "position", "absolute"), s(t, "width", "100%"), s(t, "zIndex", 1), t
         },
         V = Object(f.createContext)({
             getPortalPlacement: null
         }),
         U = function(e) {
             Object(u.a)(n, e);
-            var t = y(n);
+            var t = v(n);
 
             function n() {
                 var e;
                 Object(l.a)(this, n);
                 for (var r = arguments.length, a = new Array(r), o = 0; o < r; o++) a[o] = arguments[o];
                 return (e = t.call.apply(t, [this].concat(a))).state = {
                     maxHeight: e.props.maxMenuHeight,
@@ -1451,16 +1451,16 @@
                 n = t.spacing.baseUnit;
             return {
                 color: t.colors.neutral40,
                 padding: "".concat(2 * n, "px ").concat(3 * n, "px"),
                 textAlign: "center"
             }
         },
-        Q = Y,
         G = Y,
+        Q = Y,
         J = function(e) {
             var t = e.children,
                 n = e.className,
                 o = e.cx,
                 i = e.getStyles,
                 l = e.innerProps;
             return Object(a.c)("div", Object(r.a)({
@@ -1501,15 +1501,15 @@
                 top: n,
                 width: t.width,
                 zIndex: 1
             }
         },
         ee = function(e) {
             Object(u.a)(n, e);
-            var t = y(n);
+            var t = v(n);
 
             function n() {
                 var e;
                 Object(l.a)(this, n);
                 for (var r = arguments.length, a = new Array(r), o = 0; o < r; o++) a[o] = arguments[o];
                 return (e = t.call.apply(t, [this].concat(a))).state = {
                     placement: null
@@ -1544,30 +1544,30 @@
                                 left: t.left,
                                 right: t.right,
                                 top: t.top,
                                 width: t.width
                             }
                         }(i),
                         b = d ? 0 : window.pageYOffset,
-                        v = {
+                        y = {
                             offset: m[h] + b,
                             position: s,
                             rect: m
                         },
-                        y = Object(a.c)("div", Object(r.a)({
-                            css: f("menuPortal", v),
+                        v = Object(a.c)("div", Object(r.a)({
+                            css: f("menuPortal", y),
                             className: l({
                                 "menu-portal": !0
                             }, o)
                         }, c), n);
                     return Object(a.c)(V.Provider, {
                         value: {
                             getPortalPlacement: this.getPortalPlacement
                         }
-                    }, t ? Object(p.createPortal)(y, t) : y)
+                    }, t ? Object(p.createPortal)(v, t) : v)
                 }
             }]), n
         }(f.Component),
         te = function(e) {
             var t = e.isDisabled;
             return {
                 label: "container",
@@ -1684,15 +1684,15 @@
                 fontSize: n,
                 lineHeight: 1,
                 marginRight: n,
                 textAlign: "center",
                 verticalAlign: "middle"
             }
         },
-        ve = function(e) {
+        ye = function(e) {
             var t = e.delay,
                 n = e.offset;
             return Object(a.c)("span", {
                 css: Object(a.b)({
                     animation: "".concat(me, " 1s ease-in-out ").concat(t, "ms infinite;"),
                     backgroundColor: "currentColor",
                     borderRadius: "1em",
@@ -1700,38 +1700,38 @@
                     marginLeft: n ? "1em" : void 0,
                     height: "1em",
                     verticalAlign: "top",
                     width: "1em"
                 }, "", "")
             })
         },
-        ye = function(e) {
+        ve = function(e) {
             var t = e.className,
                 n = e.cx,
                 o = e.getStyles,
                 i = e.innerProps,
                 l = e.isRtl;
             return Object(a.c)("div", Object(r.a)({
                 css: o("loadingIndicator", e),
                 className: n({
                     indicator: !0,
                     "loading-indicator": !0
                 }, t)
-            }, i), Object(a.c)(ve, {
+            }, i), Object(a.c)(ye, {
                 delay: 0,
                 offset: l
-            }), Object(a.c)(ve, {
+            }), Object(a.c)(ye, {
                 delay: 160,
                 offset: !0
-            }), Object(a.c)(ve, {
+            }), Object(a.c)(ye, {
                 delay: 320,
                 offset: !l
             }))
         };
-    ye.defaultProps = {
+    ve.defaultProps = {
         size: 4
     };
     var ge = function(e) {
             var t = e.isDisabled,
                 n = e.isFocused,
                 r = e.theme,
                 a = r.colors,
@@ -1792,44 +1792,44 @@
             return m({
                 margin: a.baseUnit / 2,
                 paddingBottom: a.baseUnit / 2,
                 paddingTop: a.baseUnit / 2,
                 visibility: t ? "hidden" : "visible",
                 color: o.neutral80,
                 transform: n ? "translateZ(0)" : ""
-            }, ke)
+            }, Me)
         },
-        Me = {
+        ke = {
             gridArea: "1 / 2",
             font: "inherit",
             minWidth: "2px",
             border: 0,
             margin: 0,
             outline: 0,
             padding: 0
         },
-        ke = {
+        Me = {
             flex: "1 1 auto",
             display: "inline-grid",
             gridArea: "1 / 1 / 2 / 3",
             gridTemplateColumns: "0 min-content",
             "&:after": m({
                 content: 'attr(data-value) " "',
                 visibility: "hidden",
                 whiteSpace: "pre"
-            }, Me)
+            }, ke)
         },
         Pe = function(e) {
             return m({
                 label: "input",
                 color: "inherit",
                 background: 0,
                 opacity: e ? 0 : 1,
                 width: "100%"
-            }, Me)
+            }, ke)
         },
         xe = function(e) {
             var t = e.theme,
                 n = t.spacing,
                 r = t.borderRadius;
             return {
                 label: "multiValue",
@@ -2066,15 +2066,15 @@
                         input: !0
                     }, p),
                     ref: u,
                     style: Pe(f),
                     disabled: s
                 }, d)))
             },
-            LoadingIndicator: ye,
+            LoadingIndicator: ve,
             Menu: function(e) {
                 var t = e.children,
                     n = e.className,
                     o = e.cx,
                     i = e.getStyles,
                     l = e.innerRef,
                     c = e.innerProps;
@@ -2118,36 +2118,36 @@
                     s = e.removeProps,
                     f = e.selectProps,
                     p = r.Container,
                     d = r.Label,
                     h = r.Remove;
                 return Object(a.c)(a.a, null, (function(r) {
                     var b = r.css,
-                        v = r.cx;
+                        y = r.cx;
                     return Object(a.c)(p, {
                         data: i,
                         innerProps: m({
-                            className: v(b(l("multiValue", e)), o({
+                            className: y(b(l("multiValue", e)), o({
                                 "multi-value": !0,
                                 "multi-value--is-disabled": u
                             }, n))
                         }, c),
                         selectProps: f
                     }, Object(a.c)(d, {
                         data: i,
                         innerProps: {
-                            className: v(b(l("multiValueLabel", e)), o({
+                            className: y(b(l("multiValueLabel", e)), o({
                                 "multi-value__label": !0
                             }, n))
                         },
                         selectProps: f
                     }, t), Object(a.c)(h, {
                         data: i,
                         innerProps: m({
-                            className: v(b(l("multiValueRemove", e)), o({
+                            className: y(b(l("multiValueRemove", e)), o({
                                 "multi-value__remove": !0
                             }, n)),
                             "aria-label": "Remove ".concat(t || "option")
                         }, s),
                         selectProps: f
                     }))
                 }))
@@ -2413,28 +2413,28 @@
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }(e) || o(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
     var b = n(9),
-        v = Number.isNaN || function(e) {
+        y = Number.isNaN || function(e) {
             return "number" == typeof e && e != e
         };
 
-    function y(e, t) {
+    function v(e, t) {
         if (e.length !== t.length) return !1;
         for (var n = 0; n < e.length; n++)
-            if (r = e[n], a = t[n], !(r === a || v(r) && v(a))) return !1;
+            if (r = e[n], a = t[n], !(r === a || y(r) && y(a))) return !1;
         var r, a;
         return !0
     }
     var g = function(e, t) {
         var n;
-        void 0 === t && (t = y);
+        void 0 === t && (t = v);
         var r, a = [],
             o = !1;
         return function() {
             for (var i = [], l = 0; l < arguments.length; l++) i[l] = arguments[l];
             return o && n === this && t(i, a) || (r = e.apply(this, i), o = !0, n = this, a = i), r
         }
     };
@@ -2517,22 +2517,22 @@
                 l = e.selectValue,
                 s = e.selectProps,
                 f = e.id,
                 p = s.ariaLiveMessages,
                 d = s.getOptionLabel,
                 h = s.inputValue,
                 m = s.isMulti,
-                v = s.isOptionDisabled,
-                y = s.isSearchable,
+                y = s.isOptionDisabled,
+                v = s.isSearchable,
                 g = s.menuIsOpen,
                 O = s.options,
                 E = s.screenReaderStatus,
                 j = s.tabSelectsValue,
-                M = s["aria-label"],
-                k = s["aria-live"],
+                k = s["aria-label"],
+                M = s["aria-live"],
                 P = Object(c.useMemo)((function() {
                     return Object(r.n)(Object(r.n)({}, w), p || {})
                 }), [p]),
                 x = Object(c.useMemo)((function() {
                     var e, n = "";
                     if (t && P.onChange) {
                         var a = t.option,
@@ -2541,40 +2541,40 @@
                             c = t.removedValues,
                             u = t.value,
                             s = i || a || (e = u, Array.isArray(e) ? null : e),
                             f = s ? d(s) : "",
                             p = o || c || void 0,
                             h = p ? p.map(d) : [],
                             m = Object(r.n)({
-                                isDisabled: s && v(s, l),
+                                isDisabled: s && y(s, l),
                                 label: f,
                                 labels: h
                             }, t);
                         n = P.onChange(m)
                     }
                     return n
-                }), [t, P, v, l, d]),
+                }), [t, P, y, l, d]),
                 S = Object(c.useMemo)((function() {
                     var e = "",
                         t = n || a,
                         r = !!(n && l && l.includes(n));
                     if (t && P.onFocus) {
                         var o = {
                             focused: t,
                             label: d(t),
-                            isDisabled: v(t, l),
+                            isDisabled: y(t, l),
                             isSelected: r,
                             options: O,
                             context: t === n ? "menu" : "value",
                             selectValue: l
                         };
                         e = P.onFocus(o)
                     }
                     return e
-                }), [n, a, d, v, P, O, l]),
+                }), [n, a, d, y, P, O, l]),
                 A = Object(c.useMemo)((function() {
                     var e = "";
                     if (g && O.length && P.onFilter) {
                         var t = E({
                             count: o.length
                         });
                         e = P.onFilter({
@@ -2585,35 +2585,35 @@
                     return e
                 }), [o, h, g, P, O, E]),
                 C = Object(c.useMemo)((function() {
                     var e = "";
                     if (P.guidance) {
                         var t = a ? "value" : g ? "menu" : "input";
                         e = P.guidance({
-                            "aria-label": M,
+                            "aria-label": k,
                             context: t,
-                            isDisabled: n && v(n, l),
+                            isDisabled: n && y(n, l),
                             isMulti: m,
-                            isSearchable: y,
+                            isSearchable: v,
                             tabSelectsValue: j
                         })
                     }
                     return e
-                }), [M, n, a, m, v, y, g, P, l, j]),
+                }), [k, n, a, m, y, v, g, P, l, j]),
                 R = "".concat(S, " ").concat(A, " ").concat(C),
                 z = Object(b.c)(u.a.Fragment, null, Object(b.c)("span", {
                     id: "aria-selection"
                 }, x), Object(b.c)("span", {
                     id: "aria-context"
                 }, R)),
                 D = "initial-input-focus" === (null == t ? void 0 : t.action);
             return Object(b.c)(u.a.Fragment, null, Object(b.c)(_, {
                 id: f
             }, D && z), Object(b.c)(_, {
-                "aria-live": k,
+                "aria-live": M,
                 "aria-atomic": "false",
                 "aria-relevant": "additions text"
             }, i && !D && z))
         }, j = [{
             base: "A",
             letters: "AⒶＡÀÁÂẦẤẪẨÃĀĂẰẮẴẲȦǠÄǞẢÅǺǍȀȂẠẬẶḀĄȺⱯ"
         }, {
@@ -2861,21 +2861,21 @@
             letters: "xⓧｘẋẍ"
         }, {
             base: "y",
             letters: "yⓨｙỳýŷỹȳẏÿỷẙỵƴɏỿ"
         }, {
             base: "z",
             letters: "zⓩｚźẑżžẓẕƶȥɀⱬꝣ"
-        }], M = new RegExp("[" + j.map((function(e) {
+        }], k = new RegExp("[" + j.map((function(e) {
             return e.letters
-        })).join("") + "]", "g"), k = {}, P = 0; P < j.length; P++)
-        for (var x = j[P], S = 0; S < x.letters.length; S++) k[x.letters[S]] = x.base;
+        })).join("") + "]", "g"), M = {}, P = 0; P < j.length; P++)
+        for (var x = j[P], S = 0; S < x.letters.length; S++) M[x.letters[S]] = x.base;
     var A = function(e) {
-            return e.replace(M, (function(e) {
-                return k[e]
+            return e.replace(k, (function(e) {
+                return M[e]
             }))
         },
         C = g(A),
         R = function(e) {
             return e.replace(/^\s+|\s+$/g, "")
         },
         z = function(e) {
@@ -2990,26 +2990,26 @@
                         if (e) {
                             var t = !!r.F && {
                                 passive: !1
                             };
                             e.addEventListener("wheel", d, t), e.addEventListener("touchstart", h, t), e.addEventListener("touchmove", m, t)
                         }
                     }), [m, h, d]),
-                    v = Object(c.useCallback)((function(e) {
+                    y = Object(c.useCallback)((function(e) {
                         e && (e.removeEventListener("wheel", d, !1), e.removeEventListener("touchstart", h, !1), e.removeEventListener("touchmove", m, !1))
                     }), [m, h, d]);
                 return Object(c.useEffect)((function() {
                         if (t) {
                             var e = f.current;
                             return b(e),
                                 function() {
-                                    v(e)
+                                    y(e)
                                 }
                         }
-                    }), [t, b, v]),
+                    }), [t, b, y]),
                     function(e) {
                         f.current = e
                     }
             }({
                 isEnabled: void 0 === a || a,
                 onBottomArrive: e.onBottomArrive,
                 onBottomLeave: e.onBottomLeave,
@@ -3069,15 +3069,15 @@
         return Object(b.c)(u.a.Fragment, null, n && Object(b.c)("div", {
             onClick: U,
             css: K
         }), t((function(e) {
             o(e), i(e)
         })))
     }
-    var Q = {
+    var G = {
         clearIndicator: r.o,
         container: r.q,
         control: r.r,
         dropdownIndicator: r.s,
         group: r.t,
         groupHeading: r.u,
         indicatorsContainer: r.v,
@@ -3093,15 +3093,15 @@
         multiValueRemove: r.G,
         noOptionsMessage: r.H,
         option: r.I,
         placeholder: r.J,
         singleValue: r.K,
         valueContainer: r.L
     };
-    var G, J = {
+    var Q, J = {
             borderRadius: 4,
             colors: {
                 primary: "#2684FF",
                 primary75: "#4C9AFF",
                 primary50: "#B2D4FF",
                 primary25: "#DEEBFF",
                 danger: "#DE350B",
@@ -3138,15 +3138,15 @@
                 if (e.data.__isNew__) return !0;
                 var n = Object(r.n)({
                         ignoreCase: !0,
                         ignoreAccents: !0,
                         stringify: z,
                         trim: !0,
                         matchFrom: "any"
-                    }, G),
+                    }, Q),
                     a = n.ignoreCase,
                     o = n.ignoreAccents,
                     i = n.stringify,
                     l = n.trim,
                     c = n.matchFrom,
                     u = l ? R(t) : t,
                     s = l ? R(i(e)) : i(e);
@@ -3380,15 +3380,15 @@
                     for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
                     return r.e.apply(void 0, [a.props.classNamePrefix].concat(t))
                 }, a.getOptionLabel = function(e) {
                     return ne(a.props, e)
                 }, a.getOptionValue = function(e) {
                     return re(a.props, e)
                 }, a.getStyles = function(e, t) {
-                    var n = Q[e](t);
+                    var n = G[e](t);
                     n.boxSizing = "border-box";
                     var r = a.props.styles[e];
                     return r ? r(n, t) : n
                 }, a.getElementId = function(e) {
                     return "".concat(a.instancePrefix, "-").concat(e)
                 }, a.getComponents = function() {
                     return Object(r.f)(a.props)
@@ -3809,15 +3809,15 @@
                         c = e.menuIsOpen,
                         s = this.getComponents().Input,
                         p = this.state,
                         d = p.inputIsHidden,
                         h = p.ariaSelection,
                         m = this.commonProps,
                         b = a || this.getElementId("input"),
-                        v = Object(r.n)(Object(r.n)({
+                        y = Object(r.n)(Object(r.n)({
                             "aria-autocomplete": "list",
                             "aria-expanded": c,
                             "aria-haspopup": !0,
                             "aria-controls": this.getElementId("listbox"),
                             "aria-owns": this.getElementId("listbox"),
                             "aria-errormessage": this.props["aria-errormessage"],
                             "aria-invalid": this.props["aria-invalid"],
@@ -3843,26 +3843,26 @@
                         onChange: this.handleInputChange,
                         onFocus: this.onInputFocus,
                         spellCheck: "false",
                         tabIndex: i,
                         form: l,
                         type: "text",
                         value: o
-                    }, v)) : u.a.createElement(T, Object(f.a)({
+                    }, y)) : u.a.createElement(T, Object(f.a)({
                         id: b,
                         innerRef: this.getInputRef,
                         onBlur: this.onInputBlur,
                         onChange: r.k,
                         onFocus: this.onInputFocus,
                         disabled: t,
                         tabIndex: i,
                         inputMode: "none",
                         form: l,
                         value: ""
-                    }, v))
+                    }, y))
                 }
             }, {
                 key: "renderPlaceholderOrValue",
                 value: function() {
                     var e = this,
                         t = this.getComponents(),
                         n = t.MultiValue,
@@ -3874,27 +3874,27 @@
                         c = this.commonProps,
                         s = this.props,
                         p = s.controlShouldRenderValue,
                         d = s.isDisabled,
                         h = s.isMulti,
                         m = s.inputValue,
                         b = s.placeholder,
-                        v = this.state,
-                        y = v.selectValue,
-                        g = v.focusedValue,
-                        O = v.isFocused;
+                        y = this.state,
+                        v = y.selectValue,
+                        g = y.focusedValue,
+                        O = y.isFocused;
                     if (!this.hasValue() || !p) return m ? null : u.a.createElement(l, Object(f.a)({}, c, {
                         key: "placeholder",
                         isDisabled: d,
                         isFocused: O,
                         innerProps: {
                             id: this.getElementId("placeholder")
                         }
                     }), b);
-                    if (h) return y.map((function(t, i) {
+                    if (h) return v.map((function(t, i) {
                         var l = t === g,
                             s = "".concat(e.getOptionLabel(t), "-").concat(e.getOptionValue(t));
                         return u.a.createElement(n, Object(f.a)({}, c, {
                             components: {
                                 Container: r,
                                 Label: a,
                                 Remove: o
@@ -3914,15 +3914,15 @@
                                     e.preventDefault(), e.stopPropagation()
                                 }
                             },
                             data: t
                         }), e.formatOptionLabel(t, "value"))
                     }));
                     if (m) return null;
-                    var _ = y[0];
+                    var _ = v[0];
                     return u.a.createElement(i, Object(f.a)({}, c, {
                         data: _,
                         isDisabled: d
                     }), this.formatOptionLabel(_, "value"))
                 }
             }, {
                 key: "renderClearIndicator",
@@ -4009,24 +4009,24 @@
                         c = t.LoadingMessage,
                         s = t.NoOptionsMessage,
                         p = t.Option,
                         d = this.commonProps,
                         h = this.state.focusedOption,
                         m = this.props,
                         b = m.captureMenuScroll,
-                        v = m.inputValue,
-                        y = m.isLoading,
+                        y = m.inputValue,
+                        v = m.isLoading,
                         g = m.loadingMessage,
                         O = m.minMenuHeight,
                         _ = m.maxMenuHeight,
                         w = m.menuIsOpen,
                         E = m.menuPlacement,
                         j = m.menuPosition,
-                        M = m.menuPortalTarget,
-                        k = m.menuShouldBlockScroll,
+                        k = m.menuPortalTarget,
+                        M = m.menuShouldBlockScroll,
                         P = m.menuShouldScrollIntoView,
                         x = m.noOptionsMessage,
                         S = m.onMenuScrollToTop,
                         A = m.onMenuScrollToBottom;
                     if (!w) return null;
                     var C, R = function(t, n) {
                         var r = t.type,
@@ -4038,28 +4038,28 @@
                             s = h === a,
                             m = o ? void 0 : function() {
                                 return e.onOptionHover(a)
                             },
                             b = o ? void 0 : function() {
                                 return e.selectOption(a)
                             },
-                            v = "".concat(e.getElementId("option"), "-").concat(n),
-                            y = {
-                                id: v,
+                            y = "".concat(e.getElementId("option"), "-").concat(n),
+                            v = {
+                                id: y,
                                 onClick: b,
                                 onMouseMove: m,
                                 onMouseOver: m,
                                 tabIndex: -1
                             };
                         return u.a.createElement(p, Object(f.a)({}, d, {
-                            innerProps: y,
+                            innerProps: v,
                             data: a,
                             isDisabled: o,
                             isSelected: i,
-                            key: v,
+                            key: y,
                             label: l,
                             type: r,
                             value: c,
                             isFocused: s,
                             innerRef: s ? e.getFocusedOptionRef : void 0
                         }), e.formatOptionLabel(t.data, "menu"))
                     };
@@ -4082,23 +4082,23 @@
                                 label: e.formatGroupLabel(t.data)
                             }), t.options.map((function(e) {
                                 return R(e, "".concat(i, "-").concat(e.index))
                             })))
                         }
                         if ("option" === t.type) return R(t, "".concat(t.index))
                     }));
-                    else if (y) {
+                    else if (v) {
                         var z = g({
-                            inputValue: v
+                            inputValue: y
                         });
                         if (null === z) return null;
                         C = u.a.createElement(c, d, z)
                     } else {
                         var D = x({
-                            inputValue: v
+                            inputValue: y
                         });
                         if (null === D) return null;
                         C = u.a.createElement(s, d, D)
                     }
                     var T = {
                             minMenuHeight: O,
                             maxMenuHeight: _,
@@ -4114,34 +4114,34 @@
                             return u.a.createElement(o, Object(f.a)({}, d, T, {
                                 innerRef: n,
                                 innerProps: {
                                     onMouseDown: e.onMenuMouseDown,
                                     onMouseMove: e.onMenuMouseMove,
                                     id: e.getElementId("listbox")
                                 },
-                                isLoading: y,
+                                isLoading: v,
                                 placement: a
                             }), u.a.createElement(Y, {
                                 captureEnabled: b,
                                 onTopArrive: S,
                                 onBottomArrive: A,
-                                lockEnabled: k
+                                lockEnabled: M
                             }, (function(t) {
                                 return u.a.createElement(i, Object(f.a)({}, d, {
                                     innerRef: function(n) {
                                         e.getMenuListRef(n), t(n)
                                     },
-                                    isLoading: y,
+                                    isLoading: v,
                                     maxHeight: l,
                                     focusedOption: h
                                 }), C)
                             })))
                         }));
-                    return M || "fixed" === j ? u.a.createElement(l, Object(f.a)({}, d, {
-                        appendTo: M,
+                    return k || "fixed" === j ? u.a.createElement(l, Object(f.a)({}, d, {
+                        appendTo: k,
                         controlElement: this.controlRef,
                         menuPlacement: E,
                         menuPosition: j
                     }), N) : N
                 }
             }, {
                 key: "renderFormField",
@@ -4261,65 +4261,65 @@
                         d = e.isMulti,
                         h = Object(r.i)(s),
                         m = {};
                     if (n && (s !== n.value || u !== n.options || f !== n.menuIsOpen || p !== n.inputValue)) {
                         var b = f ? function(e, t) {
                                 return ee($(e, t))
                             }(e, h) : [],
-                            v = a ? function(e, t) {
+                            y = a ? function(e, t) {
                                 var n = e.focusedValue,
                                     r = e.selectValue.indexOf(n);
                                 if (r > -1) {
                                     if (t.indexOf(n) > -1) return n;
                                     if (r < t.length) return t[r]
                                 }
                                 return null
                             }(t, h) : null;
                         m = {
                             selectValue: h,
                             focusedOption: function(e, t) {
                                 var n = e.focusedOption;
                                 return n && t.indexOf(n) > -1 ? n : t[0]
                             }(t, b),
-                            focusedValue: v,
+                            focusedValue: y,
                             clearFocusValueOnUpdate: !1
                         }
                     }
-                    var y = null != o && e !== n ? {
+                    var v = null != o && e !== n ? {
                             inputIsHidden: o,
                             inputIsHiddenAfterUpdate: void 0
                         } : {},
                         g = i,
                         O = l && c;
                     return l && !O && (g = {
                         value: Object(r.d)(d, h, h[0] || null),
                         options: h,
                         action: "initial-input-focus"
-                    }, O = !c), "initial-input-focus" === (null == i ? void 0 : i.action) && (g = null), Object(r.n)(Object(r.n)(Object(r.n)({}, m), y), {}, {
+                    }, O = !c), "initial-input-focus" === (null == i ? void 0 : i.action) && (g = null), Object(r.n)(Object(r.n)(Object(r.n)({}, m), v), {}, {
                         prevProps: e,
                         ariaSelection: g,
                         prevWasFocused: O
                     })
                 }
             }]), n
         }(c.Component);
     ue.defaultProps = Z;
     var se = n(18),
         fe = n(48),
         pe = (n(121), n(125), n(127), n(131), n(132), n(133), n(15), u.a.forwardRef((function(e, t) {
-            var n, a, o, p, d, h, m, b, v, y, g, O, _, w, E, j, M, k, P, x, S, A, C, R, z, D, T, N, I, H, L, B = (a = (n = e).defaultInputValue, o = void 0 === a ? "" : a, p = n.defaultMenuIsOpen, d = void 0 !== p && p, h = n.defaultValue, m = void 0 === h ? null : h, b = n.inputValue, v = n.menuIsOpen, y = n.onChange, g = n.onInputChange, O = n.onMenuClose, _ = n.onMenuOpen, w = n.value, E = Object(l.a)(n, s), j = i(Object(c.useState)(void 0 !== b ? b : o), 2), M = j[0], k = j[1], P = i(Object(c.useState)(void 0 !== v ? v : d), 2), x = P[0], S = P[1], A = i(Object(c.useState)(void 0 !== w ? w : m), 2), C = A[0], R = A[1], z = Object(c.useCallback)((function(e, t) {
-                "function" == typeof y && y(e, t), R(e)
-            }), [y]), D = Object(c.useCallback)((function(e, t) {
+            var n, a, o, p, d, h, m, b, y, v, g, O, _, w, E, j, k, M, P, x, S, A, C, R, z, D, T, N, I, H, L, B = (a = (n = e).defaultInputValue, o = void 0 === a ? "" : a, p = n.defaultMenuIsOpen, d = void 0 !== p && p, h = n.defaultValue, m = void 0 === h ? null : h, b = n.inputValue, y = n.menuIsOpen, v = n.onChange, g = n.onInputChange, O = n.onMenuClose, _ = n.onMenuOpen, w = n.value, E = Object(l.a)(n, s), j = i(Object(c.useState)(void 0 !== b ? b : o), 2), k = j[0], M = j[1], P = i(Object(c.useState)(void 0 !== y ? y : d), 2), x = P[0], S = P[1], A = i(Object(c.useState)(void 0 !== w ? w : m), 2), C = A[0], R = A[1], z = Object(c.useCallback)((function(e, t) {
+                "function" == typeof v && v(e, t), R(e)
+            }), [v]), D = Object(c.useCallback)((function(e, t) {
                 var n;
-                "function" == typeof g && (n = g(e, t)), k(void 0 !== n ? n : e)
+                "function" == typeof g && (n = g(e, t)), M(void 0 !== n ? n : e)
             }), [g]), T = Object(c.useCallback)((function() {
                 "function" == typeof _ && _(), S(!0)
             }), [_]), N = Object(c.useCallback)((function() {
                 "function" == typeof O && O(), S(!1)
-            }), [O]), I = void 0 !== b ? b : M, H = void 0 !== v ? v : x, L = void 0 !== w ? w : C, Object(r.n)(Object(r.n)({}, E), {}, {
+            }), [O]), I = void 0 !== b ? b : k, H = void 0 !== y ? y : x, L = void 0 !== w ? w : C, Object(r.n)(Object(r.n)({}, E), {}, {
                 inputValue: I,
                 menuIsOpen: H,
                 onChange: z,
                 onInputChange: D,
                 onMenuClose: N,
                 onMenuOpen: T,
                 value: L
@@ -4386,35 +4386,35 @@
             return function() {
                 return r.current()
             }
         }), [])
     }
     var b = n(69);
 
-    function v(e) {
+    function y(e) {
         void 0 === e && (e = Object(c.a)());
         try {
             var t = e.activeElement;
             return t && t.nodeName ? t : null
         } catch (t) {
             return e.body
         }
     }
 
-    function y(e, t) {
+    function v(e, t) {
         return e.contains ? e.contains(t) : e.compareDocumentPosition ? e === t || !!(16 & e.compareDocumentPosition(t)) : void 0
     }
     var g = n(40),
         O = n(15),
         _ = n.n(O),
         w = n(54),
         E = n(55),
         j = n(20);
-    const M = "data-rr-ui-" + "modal-open";
-    var k = class {
+    const k = "data-rr-ui-" + "modal-open";
+    var M = class {
         constructor({
             ownerDocument: e,
             handleContainerOverflow: t = !0,
             isRTL: n = !1
         } = {}) {
             this.handleContainerOverflow = t, this.isRTL = n, this.modals = [], this.ownerDocument = e
         }
@@ -4434,22 +4434,22 @@
                     overflow: "hidden"
                 },
                 n = this.isRTL ? "paddingLeft" : "paddingRight",
                 r = this.getElement();
             e.style = {
                 overflow: r.style.overflow,
                 [n]: r.style[n]
-            }, e.scrollBarWidth && (t[n] = parseInt(Object(j.a)(r, n) || "0", 10) + e.scrollBarWidth + "px"), r.setAttribute(M, ""), Object(j.a)(r, t)
+            }, e.scrollBarWidth && (t[n] = parseInt(Object(j.a)(r, n) || "0", 10) + e.scrollBarWidth + "px"), r.setAttribute(k, ""), Object(j.a)(r, t)
         }
         reset() {
             [...this.modals].forEach(e => this.remove(e))
         }
         removeContainerStyle(e) {
             const t = this.getElement();
-            t.removeAttribute(M), Object.assign(t.style, e.style)
+            t.removeAttribute(k), Object.assign(t.style, e.style)
         }
         add(e) {
             let t = this.modals.indexOf(e);
             return -1 !== t ? t : (t = this.modals.length, this.modals.push(e), this.setModalAttributes(e), 0 !== t || (this.state = {
                 scrollBarWidth: this.getScrollbarWidth(),
                 style: {}
             }, this.handleContainerOverflow && this.setContainerStyle(this.state)), t)
@@ -4474,15 +4474,15 @@
     var A = n(2);
     const C = ["show", "role", "className", "style", "children", "backdrop", "keyboard", "onBackdropClick", "onEscapeKeyDown", "transition", "backdropTransition", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "renderDialog", "renderBackdrop", "manager", "container", "onShow", "onHide", "onExit", "onExited", "onExiting", "onEnter", "onEntering", "onEntered"];
     let R;
 
     function z(e) {
         const t = x(),
             n = e || function(e) {
-                return R || (R = new k({
+                return R || (R = new M({
                     ownerDocument: null == e ? void 0 : e.document
                 })), R
             }(t),
             r = Object(h.useRef)({
                 dialog: null,
                 backdrop: null
             });
@@ -4509,16 +4509,16 @@
             keyboard: u = !0,
             onBackdropClick: s,
             onEscapeKeyDown: f,
             transition: d,
             backdropTransition: b,
             autoFocus: O = !0,
             enforceFocus: j = !0,
-            restoreFocus: M = !0,
-            restoreFocusOptions: k,
+            restoreFocus: k = !0,
+            restoreFocusOptions: M,
             renderDialog: P,
             renderBackdrop: R = (e => Object(A.jsx)("div", Object.assign({}, e))),
             manager: D,
             container: T,
             onShow: N,
             onHide: I = (() => {}),
             onExit: H,
@@ -4546,53 +4546,53 @@
                 }, [t, r]), Object(h.useEffect)(() => {
                     const t = S(e);
                     t !== r && a(t)
                 }, [e, r]), r
             }(T),
             K = z(D),
             Y = Object(w.a)(),
-            Q = Object(E.a)(n),
-            [G, J] = Object(h.useState)(!n),
+            G = Object(E.a)(n),
+            [Q, J] = Object(h.useState)(!n),
             Z = Object(h.useRef)(null);
-        Object(h.useImperativeHandle)(t, () => K, [K]), l.a && !Q && n && (Z.current = v()), d || n || G ? n && G && J(!1) : J(!0);
+        Object(h.useImperativeHandle)(t, () => K, [K]), l.a && !G && n && (Z.current = y()), d || n || Q ? n && Q && J(!1) : J(!0);
         const X = Object(p.a)(() => {
                 if (K.add(), ae.current = Object(g.a)(document, "keydown", ne), re.current = Object(g.a)(document, "focus", () => setTimeout(ee), !0), N && N(), O) {
-                    const e = v(document);
-                    K.dialog && e && !y(K.dialog, e) && (Z.current = e, K.dialog.focus())
+                    const e = y(document);
+                    K.dialog && e && !v(K.dialog, e) && (Z.current = e, K.dialog.focus())
                 }
             }),
             $ = Object(p.a)(() => {
                 var e;
-                (K.remove(), null == ae.current || ae.current(), null == re.current || re.current(), M) && (null == (e = Z.current) || null == e.focus || e.focus(k), Z.current = null)
+                (K.remove(), null == ae.current || ae.current(), null == re.current || re.current(), k) && (null == (e = Z.current) || null == e.focus || e.focus(M), Z.current = null)
             });
         Object(h.useEffect)(() => {
             n && U && X()
         }, [n, U, X]), Object(h.useEffect)(() => {
-            G && $()
-        }, [G, $]), m(() => {
+            Q && $()
+        }, [Q, $]), m(() => {
             $()
         });
         const ee = Object(p.a)(() => {
                 if (!j || !Y() || !K.isTopModal()) return;
-                const e = v();
-                K.dialog && e && !y(K.dialog, e) && K.dialog.focus()
+                const e = y();
+                K.dialog && e && !v(K.dialog, e) && K.dialog.focus()
             }),
             te = Object(p.a)(e => {
                 e.target === e.currentTarget && (null == s || s(e), !0 === c && I())
             }),
             ne = Object(p.a)(e => {
                 u && 27 === e.keyCode && K.isTopModal() && (null == f || f(e), e.defaultPrevented || I())
             }),
             re = Object(h.useRef)(),
             ae = Object(h.useRef)(),
             oe = (...e) => {
                 J(!0), null == L || L(...e)
             },
             ie = d;
-        if (!U || !(n || ie && !G)) return null;
+        if (!U || !(n || ie && !Q)) return null;
         const le = Object.assign({
             role: r,
             ref: K.setDialogRef,
             "aria-modal": "dialog" === r || void 0
         }, V, {
             style: o,
             className: a,
@@ -4631,29 +4631,29 @@
             children: _.a.createPortal(Object(A.jsxs)(A.Fragment, {
                 children: [ue, ce]
             }), U)
         })
     });
     D.displayName = "Modal";
     var T = Object.assign(D, {
-        Manager: k
+        Manager: M
     });
     var N = Function.prototype.bind.call(Function.prototype.call, [].slice);
 
     function I(e, t) {
         return N(e.querySelectorAll(t))
     }
 
     function H(e, t) {
         return e.replace(new RegExp("(^|\\s)" + t + "(?:\\s|$)", "g"), "$1").replace(/\s+/g, " ").replace(/^\s*|\s*$/g, "")
     }
     const L = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
         B = ".sticky-top",
         q = ".navbar-toggler";
-    class F extends k {
+    class F extends M {
         adjustAndStore(e, t, n) {
             const r = t.style[e];
             t.dataset[e] = r, Object(j.a)(t, {
                 [e]: parseFloat(Object(j.a)(t, e)) + n + "px"
             })
         }
         restore(e, t) {
@@ -4686,40 +4686,40 @@
     let W;
     var V = n(39),
         U = n(22),
         K = Object(U.a)("modal-body");
     var Y = h.createContext({
             onHide() {}
         }),
-        Q = n(11);
-    const G = h.forwardRef(({
+        G = n(11);
+    const Q = h.forwardRef(({
         bsPrefix: e,
         className: t,
         contentClassName: n,
         centered: r,
         size: a,
         fullscreen: i,
         children: l,
         scrollable: c,
         ...u
     }, s) => {
-        const f = (e = Object(Q.a)(e, "modal")) + "-dialog",
+        const f = (e = Object(G.a)(e, "modal")) + "-dialog",
             p = "string" == typeof i ? `${e}-fullscreen-${i}` : e + "-fullscreen";
         return Object(A.jsx)("div", {
             ...u,
             ref: s,
             className: o()(f, t, a && `${e}-${a}`, r && f + "-centered", c && f + "-scrollable", i && p),
             children: Object(A.jsx)("div", {
                 className: o()(e + "-content", n),
                 children: l
             })
         })
     });
-    G.displayName = "ModalDialog";
-    var J = G,
+    Q.displayName = "ModalDialog";
+    var J = Q,
         Z = Object(U.a)("modal-footer"),
         X = n(66);
     const $ = h.forwardRef(({
         closeLabel: e,
         closeVariant: t,
         closeButton: n,
         onHide: r,
@@ -4745,15 +4745,15 @@
         closeButton: !1
     };
     var ee = $;
     const te = h.forwardRef(({
         bsPrefix: e,
         className: t,
         ...n
-    }, r) => (e = Object(Q.a)(e, "modal-header"), Object(A.jsx)(ee, {
+    }, r) => (e = Object(G.a)(e, "modal-header"), Object(A.jsx)(ee, {
         ref: r,
         ...n,
         className: o()(t, e)
     })));
     te.displayName = "ModalHeader", te.defaultProps = {
         closeLabel: "Close",
         closeButton: !1
@@ -4790,24 +4790,24 @@
     }
     const ue = h.forwardRef(({
         bsPrefix: e,
         className: t,
         style: n,
         dialogClassName: r,
         contentClassName: a,
-        children: v,
-        dialogAs: y,
+        children: y,
+        dialogAs: v,
         "aria-labelledby": g,
         show: O,
         animation: _,
         backdrop: w,
         keyboard: E,
         onEscapeKeyDown: j,
-        onShow: M,
-        onHide: k,
+        onShow: k,
+        onHide: M,
         container: P,
         autoFocus: x,
         enforceFocus: S,
         restoreFocus: C,
         restoreFocusOptions: R,
         onEntered: z,
         onExit: D,
@@ -4815,16 +4815,16 @@
         onEnter: I,
         onEntering: H,
         onExited: L,
         backdropClassName: B,
         manager: q,
         ...V
     }, U) => {
-        const [K, G] = Object(h.useState)({}), [J, Z] = Object(h.useState)(!1), X = Object(h.useRef)(!1), $ = Object(h.useRef)(!1), ee = Object(h.useRef)(null), [te, ne] = Object(f.a)(), re = Object(d.a)(U, ne), ae = Object(p.a)(k), oe = Object(Q.b)();
-        e = Object(Q.a)(e, "modal");
+        const [K, Q] = Object(h.useState)({}), [J, Z] = Object(h.useState)(!1), X = Object(h.useRef)(!1), $ = Object(h.useRef)(!1), ee = Object(h.useRef)(null), [te, ne] = Object(f.a)(), re = Object(d.a)(U, ne), ae = Object(p.a)(M), oe = Object(G.b)();
+        e = Object(G.a)(e, "modal");
         const ie = Object(h.useMemo)(() => ({
             onHide: ae
         }), [ae]);
 
         function ue() {
             return q || (e = {
                 isRTL: oe
@@ -4832,15 +4832,15 @@
             var e
         }
 
         function se(e) {
             if (!l.a) return;
             const t = ue().getScrollbarWidth() > 0,
                 n = e.scrollHeight > Object(c.a)(e).documentElement.clientHeight;
-            G({
+            Q({
                 paddingRight: t && !n ? s() : void 0,
                 paddingLeft: !t && n ? s() : void 0
             })
         }
         const fe = Object(p.a)(() => {
             te && se(te.dialog)
         });
@@ -4855,27 +4855,27 @@
             },
             he = () => {
                 Z(!0), ee.current = Object(b.a)(te.dialog, () => {
                     Z(!1)
                 })
             },
             me = e => {
-                "static" !== w ? $.current || e.target !== e.currentTarget ? $.current = !1 : null == k || k() : (e => {
+                "static" !== w ? $.current || e.target !== e.currentTarget ? $.current = !1 : null == M || M() : (e => {
                     e.target === e.currentTarget && he()
                 })(e)
             },
             be = Object(h.useCallback)(t => Object(A.jsx)("div", {
                 ...t,
                 className: o()(e + "-backdrop", B, !_ && "show")
             }), [_, B, e]),
-            ve = {
+            ye = {
                 ...n,
                 ...K
             };
-        _ || (ve.display = "block");
+        _ || (ye.display = "block");
         return Object(A.jsx)(Y.Provider, {
             value: ie,
             children: Object(A.jsx)(T, {
                 show: O,
                 ref: re,
                 backdrop: w,
                 container: P,
@@ -4883,16 +4883,16 @@
                 autoFocus: x,
                 enforceFocus: S,
                 restoreFocus: C,
                 restoreFocusOptions: R,
                 onEscapeKeyDown: e => {
                     E || "static" !== w ? E && j && j(e) : (e.preventDefault(), he())
                 },
-                onShow: M,
-                onHide: k,
+                onShow: k,
+                onHide: M,
                 onEnter: (e, t) => {
                     e && (e.style.display = "block", se(e)), null == I || I(e, t)
                 },
                 onEntering: (e, t) => {
                     null == H || H(e, t), Object(i.a)(window, "resize", fe)
                 },
                 onEntered: z,
@@ -4906,25 +4906,25 @@
                 manager: ue(),
                 transition: _ ? le : void 0,
                 backdropTransition: _ ? ce : void 0,
                 renderBackdrop: be,
                 renderDialog: n => Object(A.jsx)("div", {
                     role: "dialog",
                     ...n,
-                    style: ve,
+                    style: ye,
                     className: o()(t, e, J && e + "-static"),
                     onClick: w ? me : void 0,
                     onMouseUp: de,
                     "aria-labelledby": g,
-                    children: Object(A.jsx)(y, {
+                    children: Object(A.jsx)(v, {
                         ...V,
                         onMouseDown: pe,
                         className: r,
                         contentClassName: a,
-                        children: v
+                        children: y
                     })
                 })
             })
         })
     });
     ue.displayName = "Modal", ue.defaultProps = ie;
     t.a = Object.assign(ue, {
@@ -4954,31 +4954,31 @@
         className: s,
         isValid: f = !1,
         isInvalid: p = !1,
         plaintext: d,
         readOnly: h,
         as: m = "input",
         ...b
-    }, v) => {
+    }, y) => {
         const {
-            controlId: y
+            controlId: v
         } = Object(o.useContext)(l.a);
         let g;
         return e = Object(c.a)(e, "form-control"), g = d ? {
             [e + "-plaintext"]: !0
         } : {
             [e]: !0,
             [`${e}-${n}`]: n
         }, Object(u.jsx)(m, {
             ...b,
             type: t,
             size: r,
-            ref: v,
+            ref: y,
             readOnly: h,
-            id: i || y,
+            id: i || v,
             className: a()(s, g, f && "is-valid", p && "is-invalid", "color" === t && e + "-color")
         })
     });
     s.displayName = "FormControl", t.a = Object.assign(s, {
         Feedback: i.a
     })
 }, function(e, t, n) {
@@ -5027,15 +5027,15 @@
     t.a = a
 }, function(e, t, n) {
     "use strict";
     n.d(t, "a", (function() {
         return o
     }));
     var r = n(0),
-        a = n(25);
+        a = n(26);
 
     function o(e) {
         var t = Object(a.a)(e);
         return Object(r.useCallback)((function() {
             return t.current && t.current.apply(t, arguments)
         }), [t])
     }
@@ -5088,17 +5088,17 @@
             "string" == typeof e.className ? s = Object(o.a)(t.registered, u, e.className) : null != e.className && (s = e.className + " ");
             var d = Object(i.a)(u, void 0, Object(r.useContext)(f));
             Object(o.b)(t, d, "string" == typeof c);
             s += t.key + "-" + d.name;
             var m = {};
             for (var b in e) l.call(e, b) && "css" !== b && b !== p && (m[b] = e[b]);
             m.ref = n, m.className = s;
-            var v = Object(r.createElement)(c, m),
-                y = Object(r.createElement)(h, null);
-            return Object(r.createElement)(r.Fragment, null, y, v)
+            var y = Object(r.createElement)(c, m),
+                v = Object(r.createElement)(h, null);
+            return Object(r.createElement)(r.Fragment, null, v, y)
         }))
 }, function(e, t, n) {
     "use strict";
     var r = n(6),
         a = n.n(r),
         o = n(1),
         i = n.n(o),
@@ -5132,66 +5132,66 @@
         bsSwitchPrefix: n,
         inline: r = !1,
         disabled: o = !1,
         isValid: i = !1,
         isInvalid: d = !1,
         feedbackTooltip: m = !1,
         feedback: b,
-        feedbackType: v,
-        className: y,
+        feedbackType: y,
+        className: v,
         style: g,
         title: O = "",
         type: _ = "checkbox",
         label: w,
         children: E,
         as: j = "input",
-        ...M
-    }, k) => {
+        ...k
+    }, M) => {
         t = Object(f.a)(t, "form-check"), n = Object(f.a)(n, "form-switch");
         const {
             controlId: P
         } = Object(l.useContext)(s.a), x = Object(l.useMemo)(() => ({
             controlId: e || P
         }), [P, e]), S = !E && null != w && !1 !== w || function(e, t) {
             return l.Children.toArray(e).some(e => l.isValidElement(e) && e.type === t)
         }(E, h), A = Object(p.jsx)(u.a, {
-            ...M,
+            ...k,
             type: "switch" === _ ? "checkbox" : _,
-            ref: k,
+            ref: M,
             isValid: i,
             isInvalid: d,
             disabled: o,
             as: j
         });
         return Object(p.jsx)(s.a.Provider, {
             value: x,
             children: Object(p.jsx)("div", {
                 style: g,
-                className: a()(y, S && t, r && t + "-inline", "switch" === _ && n),
+                className: a()(v, S && t, r && t + "-inline", "switch" === _ && n),
                 children: E || Object(p.jsxs)(p.Fragment, {
                     children: [A, S && Object(p.jsx)(h, {
                         title: O,
                         children: w
                     }), b && Object(p.jsx)(c.a, {
-                        type: v,
+                        type: y,
                         tooltip: m,
                         children: b
                     })]
                 })
             })
         })
     });
     m.displayName = "FormCheck";
     var b = Object.assign(m, {
             Input: u.a,
             Label: h
         }),
-        v = n(13),
-        y = n(22),
-        g = Object(y.a)("form-floating");
+        y = n(13),
+        v = n(22),
+        g = Object(v.a)("form-floating");
     const O = l.forwardRef(({
         controlId: e,
         as: t = "div",
         ...n
     }, r) => {
         const a = Object(l.useMemo)(() => ({
             controlId: e
@@ -5248,15 +5248,15 @@
             ...r,
             ref: t,
             className: a()(n, !l.length && i)
         })
     });
     E.displayName = "Col";
     var j = E;
-    const M = l.forwardRef(({
+    const k = l.forwardRef(({
         as: e = "label",
         bsPrefix: t,
         column: n,
         visuallyHidden: r,
         className: o,
         htmlFor: i,
         ...c
@@ -5277,19 +5277,19 @@
         }) : Object(p.jsx)(e, {
             ref: u,
             className: m,
             htmlFor: i,
             ...c
         })
     });
-    M.displayName = "FormLabel", M.defaultProps = {
+    k.displayName = "FormLabel", k.defaultProps = {
         column: !1,
         visuallyHidden: !1
     };
-    var k = M;
+    var M = k;
     const P = l.forwardRef(({
         bsPrefix: e,
         className: t,
         id: n,
         ...r
     }, o) => {
         const {
@@ -5384,19 +5384,19 @@
             ...r,
             ref: o,
             className: a()(e, t && "was-validated")
         }));
     H.displayName = "Form", H.propTypes = I;
     t.a = Object.assign(H, {
         Group: _,
-        Control: v.a,
+        Control: y.a,
         Floating: g,
         Check: b,
         Switch: D,
-        Label: k,
+        Label: M,
         Text: R,
         Range: x,
         Select: A,
         FloatingLabel: N
     })
 }, function(e, t, n) {
     "use strict";
@@ -5485,15 +5485,15 @@
 }, function(e, t, n) {
     "use strict";
     var r = n(6),
         a = n.n(r),
         o = n(0),
         i = n(68),
         l = n(17);
-    n(53), n(25);
+    n(53), n(26);
     n(54), n(55);
     n(86), new WeakMap;
     var c = n(61),
         u = n(2);
     const s = ["onKeyDown"];
     const f = o.forwardRef((e, t) => {
         let {
@@ -5523,21 +5523,21 @@
     });
     f.displayName = "Anchor";
     var p = f,
         d = n(11),
         h = n(39),
         m = n(66),
         b = n(60),
-        v = n(22);
-    const y = Object(b.a)("h4");
-    y.displayName = "DivStyledAsH4";
-    const g = Object(v.a)("alert-heading", {
-            Component: y
+        y = n(22);
+    const v = Object(b.a)("h4");
+    v.displayName = "DivStyledAsH4";
+    const g = Object(y.a)("alert-heading", {
+            Component: v
         }),
-        O = Object(v.a)("alert-link", {
+        O = Object(y.a)("alert-link", {
             Component: p
         }),
         _ = {
             variant: "primary",
             show: !0,
             transition: h.a,
             closeLabel: "Close alert"
@@ -5548,27 +5548,27 @@
                 show: r,
                 closeLabel: o,
                 closeVariant: c,
                 className: s,
                 children: f,
                 variant: p,
                 onClose: b,
-                dismissible: v,
-                transition: y,
+                dismissible: y,
+                transition: v,
                 ...g
             } = Object(i.a)(e, {
                 show: "onClose"
             }), O = Object(d.a)(n, "alert"), _ = Object(l.a)(e => {
                 b && b(!1, e)
-            }), w = !0 === y ? h.a : y, E = Object(u.jsxs)("div", {
+            }), w = !0 === v ? h.a : v, E = Object(u.jsxs)("div", {
                 role: "alert",
                 ...w ? void 0 : g,
                 ref: t,
-                className: a()(s, O, p && `${O}-${p}`, v && O + "-dismissible"),
-                children: [v && Object(u.jsx)(m.a, {
+                className: a()(s, O, p && `${O}-${p}`, y && O + "-dismissible"),
+                children: [y && Object(u.jsx)(m.a, {
                     onClick: _,
                     "aria-label": o,
                     variant: c
                 }), f]
             });
             return w ? Object(u.jsx)(w, {
                 unmountOnExit: !0,
@@ -5579,15 +5579,15 @@
             }) : r ? E : null
         });
     w.displayName = "Alert", w.defaultProps = _;
     t.a = Object.assign(w, {
         Link: O,
         Heading: g
     })
-}, function(e, t, n) {
+}, , function(e, t, n) {
     "use strict";
     var r = n(0);
     t.a = function(e) {
         var t = Object(r.useRef)(e);
         return Object(r.useEffect)((function() {
             t.current = e
         }), [e]), t
@@ -5745,15 +5745,15 @@
         onEntering: b,
         onEntered: b,
         onExit: b,
         onExiting: b,
         onExited: b
     }, m.UNMOUNTED = "unmounted", m.EXITED = f, m.ENTERING = p, m.ENTERED = d, m.EXITING = h;
     t.e = m
-}, , function(e, t) {
+}, function(e, t) {
     e.exports = function(e) {
         var t = {};
 
         function n(r) {
             if (t[r]) return t[r].exports;
             var a = t[r] = {
                 i: r,
@@ -5871,21 +5871,21 @@
             try {
                 return Date.prototype.toString.call(Reflect.construct(Date, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }
 
-        function v(e) {
-            return (v = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+        function y(e) {
+            return (y = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                 return e.__proto__ || Object.getPrototypeOf(e)
             })(e)
         }
 
-        function y(e, t, n) {
+        function v(e, t, n) {
             return t in e ? Object.defineProperty(e, t, {
                 value: n,
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : e[t] = n, e
         }
@@ -5898,45 +5898,45 @@
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }), t && d(e, t)
             }(i, e);
             var t, n, r, o = (t = i, function() {
-                var e, n = v(t);
+                var e, n = y(t);
                 if (b()) {
-                    var r = v(this).constructor;
+                    var r = y(this).constructor;
                     e = Reflect.construct(n, arguments, r)
                 } else e = n.apply(this, arguments);
                 return h(this, e)
             });
 
             function i(e) {
                 var t;
                 return function(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                }(this, i), y(m(t = o.call(this, e)), "handleListItemChange", (function(e, n) {
+                }(this, i), v(m(t = o.call(this, e)), "handleListItemChange", (function(e, n) {
                     var r = s(t.state.list);
                     r[n] = e.target.value, t.setState({
                         list: r
                     }, (function() {
                         t.props.onListChange(t.state.list)
                     }))
-                })), y(m(t), "deleteItem", (function(e) {
+                })), v(m(t), "deleteItem", (function(e) {
                     var n = s(t.state.list);
                     n.splice(e, 1), t.setState({
                         list: n
                     }, (function() {
                         t.props.onListChange(t.state.list)
                     }))
-                })), y(m(t), "handleDeleteButtonClick", (function(e) {
+                })), v(m(t), "handleDeleteButtonClick", (function(e) {
                     return function(n) {
                         n.preventDefault(), t.deleteItem(e)
                     }
-                })), y(m(t), "getList", (function() {
+                })), v(m(t), "getList", (function() {
                     return t.state.list.map((function(e, n) {
                         return a.a.createElement("li", {
                             className: "input-field-container",
                             key: n
                         }, a.a.createElement("input", {
                             className: "input-field",
                             type: "text",
@@ -5950,17 +5950,17 @@
                             onClick: t.handleDeleteButtonClick(n)
                         }, a.a.createElement("img", {
                             className: "delete-img",
                             src: c.a,
                             alt: "Delete"
                         })))
                     }))
-                })), y(m(t), "onChange", (function(e) {
-                    t.setState(y({}, e.target.name, e.target.value))
-                })), y(m(t), "onKeyUp", (function(e) {
+                })), v(m(t), "onChange", (function(e) {
+                    t.setState(v({}, e.target.name, e.target.value))
+                })), v(m(t), "onKeyUp", (function(e) {
                     if ("Enter" === e.key && e.target.value.trim(" ").length > 0) {
                         var n = s(t.state.list);
                         t.setState({
                             list: n.concat(e.target.value),
                             newInput: ""
                         }, (function() {
                             t.props.onListChange(t.state.list)
@@ -6010,80 +6010,80 @@
             d = a ? Symbol.for("react.suspense") : 60113;
         a && Symbol.for("react.suspense_list");
         var h = a ? Symbol.for("react.memo") : 60115,
             m = a ? Symbol.for("react.lazy") : 60116;
         a && Symbol.for("react.fundamental"), a && Symbol.for("react.responder"), a && Symbol.for("react.scope");
         var b = "function" == typeof Symbol && Symbol.iterator;
 
-        function v(e) {
+        function y(e) {
             for (var t = "https://reactjs.org/docs/error-decoder.html?invariant=" + e, n = 1; n < arguments.length; n++) t += "&args[]=" + encodeURIComponent(arguments[n]);
             return "Minified React error #" + e + "; visit " + t + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
         }
-        var y = {
+        var v = {
                 isMounted: function() {
                     return !1
                 },
                 enqueueForceUpdate: function() {},
                 enqueueReplaceState: function() {},
                 enqueueSetState: function() {}
             },
             g = {};
 
         function O(e, t, n) {
-            this.props = e, this.context = t, this.refs = g, this.updater = n || y
+            this.props = e, this.context = t, this.refs = g, this.updater = n || v
         }
 
         function _() {}
 
         function w(e, t, n) {
-            this.props = e, this.context = t, this.refs = g, this.updater = n || y
+            this.props = e, this.context = t, this.refs = g, this.updater = n || v
         }
         O.prototype.isReactComponent = {}, O.prototype.setState = function(e, t) {
-            if ("object" != typeof e && "function" != typeof e && null != e) throw Error(v(85));
+            if ("object" != typeof e && "function" != typeof e && null != e) throw Error(y(85));
             this.updater.enqueueSetState(this, e, t, "setState")
         }, O.prototype.forceUpdate = function(e) {
             this.updater.enqueueForceUpdate(this, e, "forceUpdate")
         }, _.prototype = O.prototype;
         var E = w.prototype = new _;
         E.constructor = w, r(E, O.prototype), E.isPureReactComponent = !0;
         var j = {
                 current: null
             },
-            M = {
+            k = {
                 current: null
             },
-            k = Object.prototype.hasOwnProperty,
+            M = Object.prototype.hasOwnProperty,
             P = {
                 key: !0,
                 ref: !0,
                 __self: !0,
                 __source: !0
             };
 
         function x(e, t, n) {
             var r, a = {},
                 i = null,
                 l = null;
             if (null != t)
-                for (r in void 0 !== t.ref && (l = t.ref), void 0 !== t.key && (i = "" + t.key), t) k.call(t, r) && !P.hasOwnProperty(r) && (a[r] = t[r]);
+                for (r in void 0 !== t.ref && (l = t.ref), void 0 !== t.key && (i = "" + t.key), t) M.call(t, r) && !P.hasOwnProperty(r) && (a[r] = t[r]);
             var c = arguments.length - 2;
             if (1 === c) a.children = n;
             else if (1 < c) {
                 for (var u = Array(c), s = 0; s < c; s++) u[s] = arguments[s + 2];
                 a.children = u
             }
             if (e && e.defaultProps)
                 for (r in c = e.defaultProps) void 0 === a[r] && (a[r] = c[r]);
             return {
                 $$typeof: o,
                 type: e,
                 key: i,
                 ref: l,
                 props: a,
-                _owner: M.current
+                _owner: k.current
             }
         }
 
         function S(e) {
             return "object" == typeof e && null !== e && e.$$typeof === o
         }
         var A = /\/+/g,
@@ -6128,15 +6128,15 @@
                 if (c) return r(a, t, "" === n ? "." + T(t, 0) : n), 1;
                 if (c = 0, n = "" === n ? "." : n + ":", Array.isArray(t))
                     for (var u = 0; u < t.length; u++) {
                         var s = n + T(l = t[u], u);
                         c += e(l, s, r, a)
                     } else if ("function" == typeof(s = null === t || "object" != typeof t ? null : "function" == typeof(s = b && t[b] || t["@@iterator"]) ? s : null))
                         for (t = s.call(t), u = 0; !(l = t.next()).done;) c += e(l = l.value, s = n + T(l, u++), r, a);
-                    else if ("object" === l) throw r = "" + t, Error(v(31, "[object Object]" === r ? "object with keys {" + Object.keys(t).join(", ") + "}" : r, ""));
+                    else if ("object" === l) throw r = "" + t, Error(y(31, "[object Object]" === r ? "object with keys {" + Object.keys(t).join(", ") + "}" : r, ""));
                 return c
             }(e, "", t, n)
         }
 
         function T(e, t) {
             return "object" == typeof e && null !== e && null != e.key ? function(e) {
                 var t = {
@@ -6173,15 +6173,15 @@
         function H(e, t, n, r, a) {
             var o = "";
             null != n && (o = ("" + n).replace(A, "$&/") + "/"), D(e, I, t = R(t, o, r, a)), z(t)
         }
 
         function L() {
             var e = j.current;
-            if (null === e) throw Error(v(321));
+            if (null === e) throw Error(y(321));
             return e
         }
         var B = {
                 Children: {
                     map: function(e, t, n) {
                         if (null == e) return e;
                         var r = [];
@@ -6199,15 +6199,15 @@
                     toArray: function(e) {
                         var t = [];
                         return H(e, t, null, (function(e) {
                             return e
                         })), t
                     },
                     only: function(e) {
-                        if (!S(e)) throw Error(v(143));
+                        if (!S(e)) throw Error(y(143));
                         return e
                     }
                 },
                 createRef: function() {
                     return {
                         current: null
                     }
@@ -6279,22 +6279,22 @@
                 },
                 Fragment: l,
                 Profiler: u,
                 StrictMode: c,
                 Suspense: d,
                 createElement: x,
                 cloneElement: function(e, t, n) {
-                    if (null == e) throw Error(v(267, e));
+                    if (null == e) throw Error(y(267, e));
                     var a = r({}, e.props),
                         i = e.key,
                         l = e.ref,
                         c = e._owner;
                     if (null != t) {
-                        if (void 0 !== t.ref && (l = t.ref, c = M.current), void 0 !== t.key && (i = "" + t.key), e.type && e.type.defaultProps) var u = e.type.defaultProps;
-                        for (s in t) k.call(t, s) && !P.hasOwnProperty(s) && (a[s] = void 0 === t[s] && void 0 !== u ? u[s] : t[s])
+                        if (void 0 !== t.ref && (l = t.ref, c = k.current), void 0 !== t.key && (i = "" + t.key), e.type && e.type.defaultProps) var u = e.type.defaultProps;
+                        for (s in t) M.call(t, s) && !P.hasOwnProperty(s) && (a[s] = void 0 === t[s] && void 0 !== u ? u[s] : t[s])
                     }
                     var s = arguments.length - 2;
                     if (1 === s) a.children = n;
                     else if (1 < s) {
                         u = Array(s);
                         for (var f = 0; f < s; f++) u[f] = arguments[f + 2];
                         a.children = u
@@ -6315,15 +6315,15 @@
                 isValidElement: S,
                 version: "16.12.0",
                 __SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED: {
                     ReactCurrentDispatcher: j,
                     ReactCurrentBatchConfig: {
                         suspense: null
                     },
-                    ReactCurrentOwner: M,
+                    ReactCurrentOwner: k,
                     IsSomeRendererActing: {
                         current: !1
                     },
                     assign: r
                 }
             },
             q = {
@@ -6621,22 +6621,22 @@
             h = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 return new(Function.prototype.bind.apply(h.Color, [null].concat(e)))
             };
         h.Color = d, h.version = "2.1.2";
         var m = h,
             b = l.unpack,
-            v = Math.max,
-            y = function() {
+            y = Math.max,
+            v = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n = b(e, "rgb"),
                     r = n[0],
                     a = n[1],
                     o = n[2],
-                    i = 1 - v(r /= 255, v(a /= 255, o /= 255)),
+                    i = 1 - y(r /= 255, y(a /= 255, o /= 255)),
                     l = i < 1 ? 1 / (1 - i) : 0,
                     c = (1 - r - i) * l,
                     u = (1 - a - i) * l,
                     s = (1 - o - i) * l;
                 return [c, u, s, i]
             },
             g = l.unpack,
@@ -6648,35 +6648,35 @@
                     o = e[3],
                     i = e.length > 4 ? e[4] : 1;
                 return 1 === o ? [0, 0, 0, i] : [n >= 1 ? 0 : 255 * (1 - n) * (1 - o), r >= 1 ? 0 : 255 * (1 - r) * (1 - o), a >= 1 ? 0 : 255 * (1 - a) * (1 - o), i]
             },
             _ = l.unpack,
             w = l.type;
         d.prototype.cmyk = function() {
-            return y(this._rgb)
+            return v(this._rgb)
         }, m.cmyk = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
             return new(Function.prototype.bind.apply(d, [null].concat(e, ["cmyk"])))
         }, c.format.cmyk = O, c.autodetect.push({
             p: 2,
             test: function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 if (e = _(e, "cmyk"), "array" === w(e) && 4 === e.length) return "cmyk"
             }
         });
         var E = l.unpack,
             j = l.last,
-            M = function(e) {
+            k = function(e) {
                 return Math.round(100 * e) / 100
             },
-            k = function() {
+            M = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n = E(e, "hsla"),
                     r = j(e) || "lsa";
-                return n[0] = M(n[0] || 0), n[1] = M(100 * n[1]) + "%", n[2] = M(100 * n[2]) + "%", "hsla" === r || n.length > 3 && n[3] < 1 ? (n[3] = n.length > 3 ? n[3] : 1, r = "hsla") : n.length = 3, r + "(" + n.join(",") + ")"
+                return n[0] = k(n[0] || 0), n[1] = k(100 * n[1]) + "%", n[2] = k(100 * n[2]) + "%", "hsla" === r || n.length > 3 && n[3] < 1 ? (n[3] = n.length > 3 ? n[3] : 1, r = "hsla") : n.length = 3, r + "(" + n.join(",") + ")"
             },
             P = l.unpack,
             x = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n = (e = P(e, "rgba"))[0],
                     r = e[1],
                     a = e[2];
@@ -6689,15 +6689,15 @@
             S = l.unpack,
             A = l.last,
             C = Math.round,
             R = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n = S(e, "rgba"),
                     r = A(e) || "rgb";
-                return "hsl" == r.substr(0, 3) ? k(x(n), r) : (n[0] = C(n[0]), n[1] = C(n[1]), n[2] = C(n[2]), ("rgba" === r || n.length > 3 && n[3] < 1) && (n[3] = n.length > 3 ? n[3] : 1, r = "rgba"), r + "(" + n.slice(0, "rgb" === r ? 3 : 4).join(",") + ")")
+                return "hsl" == r.substr(0, 3) ? M(x(n), r) : (n[0] = C(n[0]), n[1] = C(n[1]), n[2] = C(n[2]), ("rgba" === r || n.length > 3 && n[3] < 1) && (n[3] = n.length > 3 ? n[3] : 1, r = "rgba"), r + "(" + n.slice(0, "rgb" === r ? 3 : 4).join(",") + ")")
             },
             z = l.unpack,
             D = Math.round,
             T = function() {
                 for (var e, t = [], n = arguments.length; n--;) t[n] = arguments[n];
                 var r, a, o, i = (t = z(t, "hsl"))[0],
                     l = t[1],
@@ -6782,71 +6782,71 @@
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
             return new(Function.prototype.bind.apply(d, [null].concat(e, ["gl"])))
         }, d.prototype.gl = function() {
             var e = this._rgb;
             return [e[0] / 255, e[1] / 255, e[2] / 255, e[3]]
         };
         var Y = l.unpack,
-            Q = function() {
+            G = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n, r = Y(e, "rgb"),
                     a = r[0],
                     o = r[1],
                     i = r[2],
                     l = Math.min(a, o, i),
                     c = Math.max(a, o, i),
                     u = c - l,
                     s = 100 * u / 255,
                     f = l / (255 - u) * 100;
                 return 0 === u ? n = Number.NaN : (a === c && (n = (o - i) / u), o === c && (n = 2 + (i - a) / u), i === c && (n = 4 + (a - o) / u), (n *= 60) < 0 && (n += 360)), [n, s, f]
             },
-            G = l.unpack,
+            Q = l.unpack,
             J = Math.floor,
             Z = function() {
                 for (var e, t, n, r, a, o, i = [], l = arguments.length; l--;) i[l] = arguments[l];
-                var c, u, s, f = (i = G(i, "hcg"))[0],
+                var c, u, s, f = (i = Q(i, "hcg"))[0],
                     p = i[1],
                     d = i[2];
                 d *= 255;
                 var h = 255 * p;
                 if (0 === p) c = u = s = d;
                 else {
                     360 === f && (f = 0), f > 360 && (f -= 360), f < 0 && (f += 360);
                     var m = J(f /= 60),
                         b = f - m,
-                        v = d * (1 - p),
-                        y = v + h * (1 - b),
-                        g = v + h * b,
-                        O = v + h;
+                        y = d * (1 - p),
+                        v = y + h * (1 - b),
+                        g = y + h * b,
+                        O = y + h;
                     switch (m) {
                         case 0:
-                            c = (e = [O, g, v])[0], u = e[1], s = e[2];
+                            c = (e = [O, g, y])[0], u = e[1], s = e[2];
                             break;
                         case 1:
-                            c = (t = [y, O, v])[0], u = t[1], s = t[2];
+                            c = (t = [v, O, y])[0], u = t[1], s = t[2];
                             break;
                         case 2:
-                            c = (n = [v, O, g])[0], u = n[1], s = n[2];
+                            c = (n = [y, O, g])[0], u = n[1], s = n[2];
                             break;
                         case 3:
-                            c = (r = [v, y, O])[0], u = r[1], s = r[2];
+                            c = (r = [y, v, O])[0], u = r[1], s = r[2];
                             break;
                         case 4:
-                            c = (a = [g, v, O])[0], u = a[1], s = a[2];
+                            c = (a = [g, y, O])[0], u = a[1], s = a[2];
                             break;
                         case 5:
-                            c = (o = [O, v, y])[0], u = o[1], s = o[2]
+                            c = (o = [O, y, v])[0], u = o[1], s = o[2]
                     }
                 }
                 return [c, u, s, i.length > 3 ? i[3] : 1]
             },
             X = l.unpack,
             $ = l.type;
         d.prototype.hcg = function() {
-            return Q(this._rgb)
+            return G(this._rgb)
         }, m.hcg = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
             return new(Function.prototype.bind.apply(d, [null].concat(e, ["hcg"])))
         }, c.format.hcg = Z, c.autodetect.push({
             p: 1,
             test: function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
@@ -6921,22 +6921,22 @@
                     c = (a + o + i) / 3,
                     u = c > 0 ? 1 - l / c : 0;
                 return 0 === u ? n = NaN : (n = (a - o + (a - i)) / 2, n /= fe((a - o) * (a - o) + (a - i) * (o - i)), n = pe(n), i > o && (n = ue - n), n /= ue), [360 * n, u, c]
             },
             he = l.unpack,
             me = l.limit,
             be = l.TWOPI,
-            ve = l.PITHIRD,
-            ye = Math.cos,
+            ye = l.PITHIRD,
+            ve = Math.cos,
             ge = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n, r, a, o = (e = he(e, "hsi"))[0],
                     i = e[1],
                     l = e[2];
-                return isNaN(o) && (o = 0), isNaN(i) && (i = 0), o > 360 && (o -= 360), o < 0 && (o += 360), (o /= 360) < 1 / 3 ? r = 1 - ((a = (1 - i) / 3) + (n = (1 + i * ye(be * o) / ye(ve - be * o)) / 3)) : o < 2 / 3 ? a = 1 - ((n = (1 - i) / 3) + (r = (1 + i * ye(be * (o -= 1 / 3)) / ye(ve - be * o)) / 3)) : n = 1 - ((r = (1 - i) / 3) + (a = (1 + i * ye(be * (o -= 2 / 3)) / ye(ve - be * o)) / 3)), [255 * (n = me(l * n * 3)), 255 * (r = me(l * r * 3)), 255 * (a = me(l * a * 3)), e.length > 3 ? e[3] : 1]
+                return isNaN(o) && (o = 0), isNaN(i) && (i = 0), o > 360 && (o -= 360), o < 0 && (o += 360), (o /= 360) < 1 / 3 ? r = 1 - ((a = (1 - i) / 3) + (n = (1 + i * ve(be * o) / ve(ye - be * o)) / 3)) : o < 2 / 3 ? a = 1 - ((n = (1 - i) / 3) + (r = (1 + i * ve(be * (o -= 1 / 3)) / ve(ye - be * o)) / 3)) : n = 1 - ((r = (1 - i) / 3) + (a = (1 + i * ve(be * (o -= 2 / 3)) / ve(ye - be * o)) / 3)), [255 * (n = me(l * n * 3)), 255 * (r = me(l * r * 3)), 255 * (a = me(l * a * 3)), e.length > 3 ? e[3] : 1]
             },
             Oe = l.unpack,
             _e = l.type;
         d.prototype.hsi = function() {
             return de(this._rgb)
         }, m.hsi = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
@@ -6959,23 +6959,23 @@
             p: 2,
             test: function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 if (e = we(e, "hsl"), "array" === Ee(e) && 3 === e.length) return "hsl"
             }
         });
         var je = l.unpack,
-            Me = Math.min,
-            ke = Math.max,
+            ke = Math.min,
+            Me = Math.max,
             Pe = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n, r, a, o = (e = je(e, "rgb"))[0],
                     i = e[1],
                     l = e[2],
-                    c = Me(o, i, l),
-                    u = ke(o, i, l),
+                    c = ke(o, i, l),
+                    u = Me(o, i, l),
                     s = u - c;
                 return a = u / 255, 0 === u ? (n = Number.NaN, r = 0) : (r = s / u, o === u && (n = (i - l) / s), i === u && (n = 2 + (l - o) / s), l === u && (n = 4 + (o - i) / s), (n *= 60) < 0 && (n += 360)), [n, r, a]
             },
             xe = l.unpack,
             Se = Math.floor,
             Ae = function() {
                 for (var e, t, n, r, a, o, i = [], l = arguments.length; l--;) i[l] = arguments[l];
@@ -6984,34 +6984,34 @@
                     d = i[2];
                 if (d *= 255, 0 === p) c = u = s = d;
                 else {
                     360 === f && (f = 0), f > 360 && (f -= 360), f < 0 && (f += 360);
                     var h = Se(f /= 60),
                         m = f - h,
                         b = d * (1 - p),
-                        v = d * (1 - p * m),
-                        y = d * (1 - p * (1 - m));
+                        y = d * (1 - p * m),
+                        v = d * (1 - p * (1 - m));
                     switch (h) {
                         case 0:
-                            c = (e = [d, y, b])[0], u = e[1], s = e[2];
+                            c = (e = [d, v, b])[0], u = e[1], s = e[2];
                             break;
                         case 1:
-                            c = (t = [v, d, b])[0], u = t[1], s = t[2];
+                            c = (t = [y, d, b])[0], u = t[1], s = t[2];
                             break;
                         case 2:
-                            c = (n = [b, d, y])[0], u = n[1], s = n[2];
+                            c = (n = [b, d, v])[0], u = n[1], s = n[2];
                             break;
                         case 3:
-                            c = (r = [b, v, d])[0], u = r[1], s = r[2];
+                            c = (r = [b, y, d])[0], u = r[1], s = r[2];
                             break;
                         case 4:
-                            c = (a = [y, b, d])[0], u = a[1], s = a[2];
+                            c = (a = [v, b, d])[0], u = a[1], s = a[2];
                             break;
                         case 5:
-                            c = (o = [d, b, v])[0], u = o[1], s = o[2]
+                            c = (o = [d, b, y])[0], u = o[1], s = o[2]
                     }
                 }
                 return [c, u, s, i.length > 3 ? i[3] : 1]
             },
             Ce = l.unpack,
             Re = l.type;
         d.prototype.hsv = function() {
@@ -7055,27 +7055,27 @@
                     l = i[0],
                     c = i[1],
                     u = i[2],
                     s = 116 * c - 16;
                 return [s < 0 ? 0 : s, 500 * (l - c), 200 * (c - u)]
             },
             Ye = l.unpack,
-            Qe = Math.pow,
-            Ge = function(e) {
-                return 255 * (e <= .00304 ? 12.92 * e : 1.055 * Qe(e, 1 / 2.4) - .055)
+            Ge = Math.pow,
+            Qe = function(e) {
+                return 255 * (e <= .00304 ? 12.92 * e : 1.055 * Ge(e, 1 / 2.4) - .055)
             },
             Je = function(e) {
                 return e > He ? e * e * e : Le * (e - Ie)
             },
             Ze = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n, r, a, o = (e = Ye(e, "lab"))[0],
                     i = e[1],
                     l = e[2];
-                return r = (o + 16) / 116, n = isNaN(i) ? r : r + i / 500, a = isNaN(l) ? r : r - l / 200, r = Te * Je(r), n = De * Je(n), a = Ne * Je(a), [Ge(3.2404542 * n - 1.5371385 * r - .4985314 * a), Ge(-.969266 * n + 1.8760108 * r + .041556 * a), Ge(.0556434 * n - .2040259 * r + 1.0572252 * a), e.length > 3 ? e[3] : 1]
+                return r = (o + 16) / 116, n = isNaN(i) ? r : r + i / 500, a = isNaN(l) ? r : r - l / 200, r = Te * Je(r), n = De * Je(n), a = Ne * Je(a), [Qe(3.2404542 * n - 1.5371385 * r - .4985314 * a), Qe(-.969266 * n + 1.8760108 * r + .041556 * a), Qe(.0556434 * n - .2040259 * r + 1.0572252 * a), e.length > 3 ? e[3] : 1]
             },
             Xe = l.unpack,
             $e = l.type;
         d.prototype.lab = function() {
             return Ke(this._rgb)
         }, m.lab = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
@@ -7145,16 +7145,16 @@
             },
             mt = l.unpack,
             bt = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n = mt(e, "hcl").reverse();
                 return ht.apply(void 0, n)
             },
-            vt = l.unpack,
-            yt = l.type;
+            yt = l.unpack,
+            vt = l.type;
         d.prototype.lch = function() {
             return lt(this._rgb)
         }, d.prototype.hcl = function() {
             return lt(this._rgb).reverse()
         }, m.lch = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
             return new(Function.prototype.bind.apply(d, [null].concat(e, ["lch"])))
@@ -7162,15 +7162,15 @@
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
             return new(Function.prototype.bind.apply(d, [null].concat(e, ["hcl"])))
         }, c.format.lch = ht, c.format.hcl = bt, ["lch", "hcl"].forEach((function(e) {
             return c.autodetect.push({
                 p: 2,
                 test: function() {
                     for (var t = [], n = arguments.length; n--;) t[n] = arguments[n];
-                    if (t = vt(t, e), "array" === yt(t) && 3 === t.length) return e
+                    if (t = yt(t, e), "array" === vt(t) && 3 === t.length) return e
                 }
             })
         }));
         var gt = {
                 aliceblue: "#f0f8ff",
                 antiquewhite: "#faebd7",
                 aqua: "#00ffff",
@@ -7354,48 +7354,48 @@
                 return (r << 16) + (a << 8) + o
             },
             Et = l.type,
             jt = function(e) {
                 if ("number" == Et(e) && e >= 0 && e <= 16777215) return [e >> 16, e >> 8 & 255, 255 & e, 1];
                 throw new Error("unknown num color: " + e)
             },
-            Mt = l.type;
+            kt = l.type;
         d.prototype.num = function() {
             return wt(this._rgb)
         }, m.num = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
             return new(Function.prototype.bind.apply(d, [null].concat(e, ["num"])))
         }, c.format.num = jt, c.autodetect.push({
             p: 5,
             test: function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
-                if (1 === e.length && "number" === Mt(e[0]) && e[0] >= 0 && e[0] <= 16777215) return "num"
+                if (1 === e.length && "number" === kt(e[0]) && e[0] >= 0 && e[0] <= 16777215) return "num"
             }
         });
-        var kt = l.unpack,
+        var Mt = l.unpack,
             Pt = l.type,
             xt = Math.round;
         d.prototype.rgb = function(e) {
             return void 0 === e && (e = !0), !1 === e ? this._rgb.slice(0, 3) : this._rgb.slice(0, 3).map(xt)
         }, d.prototype.rgba = function(e) {
             return void 0 === e && (e = !0), this._rgb.slice(0, 4).map((function(t, n) {
                 return n < 3 ? !1 === e ? t : xt(t) : t
             }))
         }, m.rgb = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
             return new(Function.prototype.bind.apply(d, [null].concat(e, ["rgb"])))
         }, c.format.rgb = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
-            var n = kt(e, "rgba");
+            var n = Mt(e, "rgba");
             return void 0 === n[3] && (n[3] = 1), n
         }, c.autodetect.push({
             p: 3,
             test: function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
-                if (e = kt(e, "rgba"), "array" === Pt(e) && (3 === e.length || 4 === e.length && "number" == Pt(e[3]) && e[3] >= 0 && e[3] <= 1)) return "rgb"
+                if (e = Mt(e, "rgba"), "array" === Pt(e) && (3 === e.length || 4 === e.length && "number" == Pt(e[3]) && e[3] >= 0 && e[3] <= 1)) return "rgb"
             }
         });
         var St = Math.log,
             At = function(e) {
                 var t, n, r, a = e / 100;
                 return a < 66 ? (t = 255, n = -155.25485562709179 - .44596950469579133 * (n = a - 2) + 104.49216199393888 * St(n), r = a < 20 ? 0 : .8274096064007395 * (r = a - 10) - 254.76935184120902 + 115.67994401066147 * St(r)) : (t = 351.97690566805693 + .114206453784165 * (t = a - 55) - 40.25366309332127 * St(t), n = 325.4494125711974 + .07943456536662342 * (n = a - 50) - 28.0852963507957 * St(n), r = 255), [t, n, r, 1]
             },
@@ -7559,28 +7559,28 @@
             return Ut(e, t, n, "hsi")
         }, Lt.hsl = function(e, t, n) {
             return Ut(e, t, n, "hsl")
         }, Lt.hsv = function(e, t, n) {
             return Ut(e, t, n, "hsv")
         };
         var Yt = l.clip_rgb,
-            Qt = Math.pow,
-            Gt = Math.sqrt,
+            Gt = Math.pow,
+            Qt = Math.sqrt,
             Jt = Math.PI,
             Zt = Math.cos,
             Xt = Math.sin,
             $t = Math.atan2,
             en = function(e, t) {
                 for (var n = e.length, r = [0, 0, 0, 0], a = 0; a < e.length; a++) {
                     var o = e[a],
                         i = t[a] / n,
                         l = o._rgb;
-                    r[0] += Qt(l[0], 2) * i, r[1] += Qt(l[1], 2) * i, r[2] += Qt(l[2], 2) * i, r[3] += l[3] * i
+                    r[0] += Gt(l[0], 2) * i, r[1] += Gt(l[1], 2) * i, r[2] += Gt(l[2], 2) * i, r[3] += l[3] * i
                 }
-                return r[0] = Gt(r[0]), r[1] = Gt(r[1]), r[2] = Gt(r[2]), r[3] > .9999999 && (r[3] = 1), new d(Yt(r))
+                return r[0] = Qt(r[0]), r[1] = Qt(r[1]), r[2] = Qt(r[2]), r[3] > .9999999 && (r[3] = 1), new d(Yt(r))
             },
             tn = l.type,
             nn = Math.pow,
             rn = function(e) {
                 var t = "rgb",
                     n = m("#ccc"),
                     r = 0,
@@ -7592,66 +7592,66 @@
                     u = !1,
                     s = 0,
                     f = 1,
                     p = !1,
                     d = {},
                     h = !0,
                     b = 1,
-                    v = function(e) {
+                    y = function(e) {
                         if ((e = e || ["#fff", "#000"]) && "string" === tn(e) && m.brewer && m.brewer[e.toLowerCase()] && (e = m.brewer[e.toLowerCase()]), "array" === tn(e)) {
                             1 === e.length && (e = [e[0], e[0]]), e = e.slice(0);
                             for (var t = 0; t < e.length; t++) e[t] = m(e[t]);
                             o.length = 0;
                             for (var n = 0; n < e.length; n++) o.push(n / (e.length - 1))
                         }
                         return _(), c = e
                     },
-                    y = function(e) {
+                    v = function(e) {
                         return e
                     },
                     g = function(e) {
                         return e
                     },
                     O = function(e, r) {
                         var a, u;
                         if (null == r && (r = !1), isNaN(e) || null === e) return n;
                         u = r ? e : l && l.length > 2 ? function(e) {
                             if (null != l) {
                                 for (var t = l.length - 1, n = 0; n < t && e >= l[n];) n++;
                                 return n - 1
                             }
                             return 0
-                        }(e) / (l.length - 2) : f !== s ? (e - s) / (f - s) : 1, u = g(u), r || (u = y(u)), 1 !== b && (u = nn(u, b)), u = i[0] + u * (1 - i[0] - i[1]), u = Math.min(1, Math.max(0, u));
+                        }(e) / (l.length - 2) : f !== s ? (e - s) / (f - s) : 1, u = g(u), r || (u = v(u)), 1 !== b && (u = nn(u, b)), u = i[0] + u * (1 - i[0] - i[1]), u = Math.min(1, Math.max(0, u));
                         var p = Math.floor(1e4 * u);
                         if (h && d[p]) a = d[p];
                         else {
                             if ("array" === tn(c))
-                                for (var v = 0; v < o.length; v++) {
-                                    var O = o[v];
+                                for (var y = 0; y < o.length; y++) {
+                                    var O = o[y];
                                     if (u <= O) {
-                                        a = c[v];
+                                        a = c[y];
                                         break
                                     }
-                                    if (u >= O && v === o.length - 1) {
-                                        a = c[v];
+                                    if (u >= O && y === o.length - 1) {
+                                        a = c[y];
                                         break
                                     }
-                                    if (u > O && u < o[v + 1]) {
-                                        u = (u - O) / (o[v + 1] - O), a = m.interpolate(c[v], c[v + 1], u, t);
+                                    if (u > O && u < o[y + 1]) {
+                                        u = (u - O) / (o[y + 1] - O), a = m.interpolate(c[y], c[y + 1], u, t);
                                         break
                                     }
                                 } else "function" === tn(c) && (a = c(u));
                             h && (d[p] = a)
                         }
                         return a
                     },
                     _ = function() {
                         return d = {}
                     };
-                v(e);
+                y(e);
                 var w = function(e) {
                     var t = m(O(e));
                     return u && t[u] ? t[u]() : t
                 };
                 return w.classes = function(e) {
                     if (null != e) {
                         if ("array" === tn(e)) l = e, a = [e[0], e[e.length - 1]];
@@ -7689,21 +7689,21 @@
                                 })
                             }
                         }
                     return a = [s, f], w
                 }, w.mode = function(e) {
                     return arguments.length ? (t = e, _(), w) : t
                 }, w.range = function(e, t) {
-                    return v(e), w
+                    return y(e), w
                 }, w.out = function(e) {
                     return u = e, w
                 }, w.spread = function(e) {
                     return arguments.length ? (r = e, w) : r
                 }, w.correctLightness = function(e) {
-                    return null == e && (e = !0), p = e, _(), y = p ? function(e) {
+                    return null == e && (e = !0), p = e, _(), v = p ? function(e) {
                         for (var t = O(0, !0).lab()[0], n = O(1, !0).lab()[0], r = t > n, a = O(e, !0).lab()[0], o = t + (n - t) * e, i = a - o, l = 0, c = 1, u = 20; Math.abs(i) > .01 && u-- > 0;) r && (i *= -1), i < 0 ? (l = e, e += .5 * (c - e)) : (c = e, e += .5 * (l - e)), a = O(e, !0).lab()[0], i = a - o;
                         return e
                     } : function(e) {
                         return e
                     }, w
                 }, w.padding = function(e) {
                     return null != e ? ("number" === tn(e) && (e = [e, e]), i = e, w) : i
@@ -7813,15 +7813,15 @@
         }))), ln.lighten = cn(un((function(e, t) {
             return e > t ? e : t
         }))), ln.dodge = cn(un((function(e, t) {
             return 255 === e || (e = t / 255 * 255 / (1 - e / 255)) > 255 ? 255 : e
         }))), ln.burn = cn(un((function(e, t) {
             return 255 * (1 - (1 - t / 255) / (e / 255))
         })));
-        for (var sn = ln, fn = l.type, pn = l.clip_rgb, dn = l.TWOPI, hn = Math.pow, mn = Math.sin, bn = Math.cos, vn = Math.floor, yn = Math.random, gn = Math.log, On = Math.pow, _n = Math.floor, wn = Math.abs, En = function(e, t) {
+        for (var sn = ln, fn = l.type, pn = l.clip_rgb, dn = l.TWOPI, hn = Math.pow, mn = Math.sin, bn = Math.cos, yn = Math.floor, vn = Math.random, gn = Math.log, On = Math.pow, _n = Math.floor, wn = Math.abs, En = function(e, t) {
                 void 0 === t && (t = null);
                 var n = {
                     min: Number.MAX_VALUE,
                     max: -1 * Number.MAX_VALUE,
                     sum: 0,
                     values: [],
                     count: 0
@@ -7860,55 +7860,55 @@
                         else {
                             var m = d - h;
                             l.push(i[h] * (1 - m) + i[h + 1] * m)
                         }
                     }
                     l.push(a)
                 } else if ("k" === t.substr(0, 1)) {
-                    var b, v = i.length,
-                        y = new Array(v),
+                    var b, y = i.length,
+                        v = new Array(y),
                         g = new Array(n),
                         O = !0,
                         _ = 0,
                         w = null;
                     (w = []).push(r);
                     for (var E = 1; E < n; E++) w.push(r + E / n * (a - r));
                     for (w.push(a); O;) {
                         for (var j = 0; j < n; j++) g[j] = 0;
-                        for (var M = 0; M < v; M++)
-                            for (var k = i[M], P = Number.MAX_VALUE, x = void 0, S = 0; S < n; S++) {
-                                var A = wn(w[S] - k);
-                                A < P && (P = A, x = S), g[x]++, y[M] = x
+                        for (var k = 0; k < y; k++)
+                            for (var M = i[k], P = Number.MAX_VALUE, x = void 0, S = 0; S < n; S++) {
+                                var A = wn(w[S] - M);
+                                A < P && (P = A, x = S), g[x]++, v[k] = x
                             }
                         for (var C = new Array(n), R = 0; R < n; R++) C[R] = null;
-                        for (var z = 0; z < v; z++) null === C[b = y[z]] ? C[b] = i[z] : C[b] += i[z];
+                        for (var z = 0; z < y; z++) null === C[b = v[z]] ? C[b] = i[z] : C[b] += i[z];
                         for (var D = 0; D < n; D++) C[D] *= 1 / g[D];
                         O = !1;
                         for (var T = 0; T < n; T++)
                             if (C[T] !== w[T]) {
                                 O = !0;
                                 break
                             } w = C, ++_ > 200 && (O = !1)
                     }
                     for (var N = {}, I = 0; I < n; I++) N[I] = [];
-                    for (var H = 0; H < v; H++) N[b = y[H]].push(i[H]);
+                    for (var H = 0; H < y; H++) N[b = v[H]].push(i[H]);
                     for (var L = [], B = 0; B < n; B++) L.push(N[B][0]), L.push(N[B][N[B].length - 1]);
                     L = L.sort((function(e, t) {
                         return e - t
                     })), l.push(L[0]);
                     for (var q = 1; q < L.length; q += 2) {
                         var F = L[q];
                         isNaN(F) || -1 !== l.indexOf(F) || l.push(F)
                     }
                 }
                 return l
-            }, Mn = {
+            }, kn = {
                 analyze: En,
                 limits: jn
-            }, kn = Math.sqrt, Pn = Math.atan2, xn = Math.abs, Sn = Math.cos, An = Math.PI, Cn = {
+            }, Mn = Math.sqrt, Pn = Math.atan2, xn = Math.abs, Sn = Math.cos, An = Math.PI, Cn = {
                 cool: function() {
                     return rn([m.hsl(180, 1, .9), m.hsl(250, .7, .4)])
                 },
                 hot: function() {
                     return rn(["#000", "#f00", "#ff0", "#fff"]).mode("rgb")
                 }
             }, Rn = {
@@ -8016,46 +8016,46 @@
                 return null == e ? n : ("array" === fn(n = e) ? 0 == (i = n[1] - n[0]) && (n = n[1]) : i = 0, l)
             }, l.lightness = function(e) {
                 return null == e ? a : ("array" === fn(e) ? (a = e, o = e[1] - e[0]) : (a = [e, e], o = 0), l)
             }, l.scale = function() {
                 return m.scale(l)
             }, l.hue(n), l
         }, m.mix = m.interpolate = qt, m.random = function() {
-            for (var e = "#", t = 0; t < 6; t++) e += "0123456789abcdef".charAt(vn(16 * yn()));
+            for (var e = "#", t = 0; t < 6; t++) e += "0123456789abcdef".charAt(yn(16 * vn()));
             return new d(e, "hex")
-        }, m.scale = rn, m.analyze = Mn.analyze, m.contrast = function(e, t) {
+        }, m.scale = rn, m.analyze = kn.analyze, m.contrast = function(e, t) {
             e = new d(e), t = new d(t);
             var n = e.luminance(),
                 r = t.luminance();
             return n > r ? (n + .05) / (r + .05) : (r + .05) / (n + .05)
         }, m.deltaE = function(e, t, n, r) {
             void 0 === n && (n = 1), void 0 === r && (r = 1), e = new d(e), t = new d(t);
-            for (var a = Array.from(e.lab()), o = a[0], i = a[1], l = a[2], c = Array.from(t.lab()), u = c[0], s = c[1], f = c[2], p = kn(i * i + l * l), h = kn(s * s + f * f), m = o < 16 ? .511 : .040975 * o / (1 + .01765 * o), b = .0638 * p / (1 + .0131 * p) + .638, v = p < 1e-6 ? 0 : 180 * Pn(l, i) / An; v < 0;) v += 360;
-            for (; v >= 360;) v -= 360;
-            var y = v >= 164 && v <= 345 ? .56 + xn(.2 * Sn(An * (v + 168) / 180)) : .36 + xn(.4 * Sn(An * (v + 35) / 180)),
+            for (var a = Array.from(e.lab()), o = a[0], i = a[1], l = a[2], c = Array.from(t.lab()), u = c[0], s = c[1], f = c[2], p = Mn(i * i + l * l), h = Mn(s * s + f * f), m = o < 16 ? .511 : .040975 * o / (1 + .01765 * o), b = .0638 * p / (1 + .0131 * p) + .638, y = p < 1e-6 ? 0 : 180 * Pn(l, i) / An; y < 0;) y += 360;
+            for (; y >= 360;) y -= 360;
+            var v = y >= 164 && y <= 345 ? .56 + xn(.2 * Sn(An * (y + 168) / 180)) : .36 + xn(.4 * Sn(An * (y + 35) / 180)),
                 g = p * p * p * p,
-                O = kn(g / (g + 1900)),
-                _ = b * (O * y + 1 - O),
+                O = Mn(g / (g + 1900)),
+                _ = b * (O * v + 1 - O),
                 w = p - h,
                 E = i - s,
                 j = l - f,
-                M = (o - u) / (n * m),
-                k = w / (r * b);
-            return kn(M * M + k * k + (E * E + j * j - w * w) / (_ * _))
+                k = (o - u) / (n * m),
+                M = w / (r * b);
+            return Mn(k * k + M * M + (E * E + j * j - w * w) / (_ * _))
         }, m.distance = function(e, t, n) {
             void 0 === n && (n = "lab"), e = new d(e), t = new d(t);
             var r = e.get(n),
                 a = t.get(n),
                 o = 0;
             for (var i in r) {
                 var l = (r[i] || 0) - (a[i] || 0);
                 o += l * l
             }
             return Math.sqrt(o)
-        }, m.limits = Mn.limits, m.valid = function() {
+        }, m.limits = kn.limits, m.valid = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
             try {
                 return new(Function.prototype.bind.apply(d, [null].concat(e))), !0
             } catch (e) {
                 return !1
             }
         }, m.scales = Cn, m.colors = gt, m.brewer = Nn, m
@@ -8089,15 +8089,15 @@
     })]);
     t.isRef = u
 }, function(e, t, n) {
     "use strict";
     var r = n(6),
         a = n.n(r),
         o = n(0),
-        i = n(26),
+        i = n(27),
         l = n(64),
         c = n(62),
         u = n(70),
         s = n(2);
     const f = {
             [i.b]: "show",
             [i.a]: "show"
@@ -8458,47 +8458,47 @@
     function b(e) {
         if (null === e.parentNode) return !1;
         e.parentNode.removeChild(e);
         var t = f.indexOf(e);
         t >= 0 && f.splice(t, 1)
     }
 
-    function v(e) {
+    function y(e) {
         var t = document.createElement("style");
         if (void 0 === e.attrs.type && (e.attrs.type = "text/css"), void 0 === e.attrs.nonce) {
             var r = function() {
                 0;
                 return n.nc
             }();
             r && (e.attrs.nonce = r)
         }
-        return y(t, e.attrs), m(e, t), t
+        return v(t, e.attrs), m(e, t), t
     }
 
-    function y(e, t) {
+    function v(e, t) {
         Object.keys(t).forEach((function(n) {
             e.setAttribute(n, t[n])
         }))
     }
 
     function g(e, t) {
         var n, r, a, o;
         if (t.transform && e.css) {
             if (!(o = "function" == typeof t.transform ? t.transform(e.css) : t.transform.default(e.css))) return function() {};
             e.css = o
         }
         if (t.singleton) {
             var i = s++;
-            n = u || (u = v(t)), r = w.bind(null, n, i, !1), a = w.bind(null, n, i, !0)
+            n = u || (u = y(t)), r = w.bind(null, n, i, !1), a = w.bind(null, n, i, !0)
         } else e.sourceMap && "function" == typeof URL && "function" == typeof URL.createObjectURL && "function" == typeof URL.revokeObjectURL && "function" == typeof Blob && "function" == typeof btoa ? (n = function(e) {
             var t = document.createElement("link");
-            return void 0 === e.attrs.type && (e.attrs.type = "text/css"), e.attrs.rel = "stylesheet", y(t, e.attrs), m(e, t), t
+            return void 0 === e.attrs.type && (e.attrs.type = "text/css"), e.attrs.rel = "stylesheet", v(t, e.attrs), m(e, t), t
         }(t), r = j.bind(null, n, t), a = function() {
             b(n), n.href && URL.revokeObjectURL(n.href)
-        }) : (n = v(t), r = E.bind(null, n), a = function() {
+        }) : (n = y(t), r = E.bind(null, n), a = function() {
             b(n)
         });
         return r(e),
             function(t) {
                 if (t) {
                     if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
                     r(e = t)
@@ -8735,19 +8735,19 @@
         return e.replace(t, n)
     }
 
     function b(e, t) {
         return e.indexOf(t)
     }
 
-    function v(e, t) {
+    function y(e, t) {
         return 0 | e.charCodeAt(t)
     }
 
-    function y(e, t, n) {
+    function v(e, t, n) {
         return e.slice(t, n)
     }
 
     function g(e) {
         return e.length
     }
 
@@ -8760,16 +8760,16 @@
     }
 
     function w(e, t) {
         return e.map(t).join("")
     }
     var E = 1,
         j = 1,
-        M = 0,
         k = 0,
+        M = 0,
         P = 0,
         x = "";
 
     function S(e, t, n, r, a, o, i) {
         return {
             value: e,
             root: t,
@@ -8787,31 +8787,31 @@
     function A(e, t) {
         return d(S("", null, null, "", null, null, 0), e, {
             length: -e.length
         }, t)
     }
 
     function C() {
-        return P = k > 0 ? v(x, --k) : 0, j--, 10 === P && (j = 1, E--), P
+        return P = M > 0 ? y(x, --M) : 0, j--, 10 === P && (j = 1, E--), P
     }
 
     function R() {
-        return P = k < M ? v(x, k++) : 0, j++, 10 === P && (j = 1, E++), P
+        return P = M < k ? y(x, M++) : 0, j++, 10 === P && (j = 1, E++), P
     }
 
     function z() {
-        return v(x, k)
+        return y(x, M)
     }
 
     function D() {
-        return k
+        return M
     }
 
     function T(e, t) {
-        return y(x, e, t)
+        return v(x, e, t)
     }
 
     function N(e) {
         switch (e) {
             case 0:
             case 9:
             case 10:
@@ -8840,37 +8840,37 @@
             case 93:
                 return 1
         }
         return 0
     }
 
     function I(e) {
-        return E = j = 1, M = g(x = e), k = 0, []
+        return E = j = 1, k = g(x = e), M = 0, []
     }
 
     function H(e) {
         return x = "", e
     }
 
     function L(e) {
-        return h(T(k - 1, function e(t) {
+        return h(T(M - 1, function e(t) {
             for (; R();) switch (P) {
                 case t:
-                    return k;
+                    return M;
                 case 34:
                 case 39:
                     34 !== t && 39 !== t && e(P);
                     break;
                 case 40:
                     41 === t && e(t);
                     break;
                 case 92:
                     R()
             }
-            return k
+            return M
         }(91 === e ? e + 2 : 40 === e ? e + 1 : e)))
     }
 
     function B(e) {
         for (;
             (P = z()) && P < 33;) R();
         return N(e) > 2 || N(P) > 3 ? "" : " "
@@ -8879,55 +8879,55 @@
     function q(e, t) {
         for (; --t && R() && !(P < 48 || P > 102 || P > 57 && P < 65 || P > 70 && P < 97););
         return T(e, D() + (t < 6 && 32 == z() && 32 == R()))
     }
 
     function F(e, t) {
         for (; R() && e + P !== 57 && (e + P !== 84 || 47 !== z()););
-        return "/*" + T(t, k - 1) + "*" + p(47 === e ? e : R())
+        return "/*" + T(t, M - 1) + "*" + p(47 === e ? e : R())
     }
 
     function W(e) {
         for (; !N(z());) R();
-        return T(e, k)
+        return T(e, M)
     }
 
     function V(e) {
         return H(function e(t, n, r, a, o, i, l, c, u) {
             var s = 0,
                 f = 0,
                 d = l,
                 h = 0,
-                v = 0,
                 y = 0,
+                v = 0,
                 O = 1,
                 w = 1,
                 E = 1,
                 j = 0,
-                M = "",
-                k = o,
+                k = "",
+                M = o,
                 P = i,
                 x = a,
-                S = M;
-            for (; w;) switch (y = j, j = R()) {
+                S = k;
+            for (; w;) switch (v = j, j = R()) {
                 case 40:
-                    if (108 != y && 58 == S.charCodeAt(d - 1)) {
+                    if (108 != v && 58 == S.charCodeAt(d - 1)) {
                         -1 != b(S += m(L(j), "&", "&\f"), "&\f") && (E = -1);
                         break
                     }
                 case 34:
                 case 39:
                 case 91:
                     S += L(j);
                     break;
                 case 9:
                 case 10:
                 case 13:
                 case 32:
-                    S += B(y);
+                    S += B(v);
                     break;
                 case 92:
                     S += q(D() - 1, 7);
                     continue;
                 case 47:
                     switch (z()) {
                         case 42:
@@ -8944,74 +8944,74 @@
                 case 59:
                 case 0:
                     switch (j) {
                         case 0:
                         case 125:
                             w = 0;
                         case 59 + f:
-                            v > 0 && g(S) - d && _(v > 32 ? Y(S + ";", a, r, d - 1) : Y(m(S, " ", "") + ";", a, r, d - 2), u);
+                            y > 0 && g(S) - d && _(y > 32 ? Y(S + ";", a, r, d - 1) : Y(m(S, " ", "") + ";", a, r, d - 2), u);
                             break;
                         case 59:
                             S += ";";
                         default:
-                            if (_(x = U(S, n, r, s, f, o, c, M, k = [], P = [], d), i), 123 === j)
-                                if (0 === f) e(S, n, x, x, k, i, d, c, P);
+                            if (_(x = U(S, n, r, s, f, o, c, k, M = [], P = [], d), i), 123 === j)
+                                if (0 === f) e(S, n, x, x, M, i, d, c, P);
                                 else switch (h) {
                                     case 100:
                                     case 109:
                                     case 115:
-                                        e(t, x, x, a && _(U(t, x, x, 0, 0, o, c, M, o, k = [], d), P), o, P, d, c, a ? k : P);
+                                        e(t, x, x, a && _(U(t, x, x, 0, 0, o, c, k, o, M = [], d), P), o, P, d, c, a ? M : P);
                                         break;
                                     default:
                                         e(S, x, x, x, [""], P, 0, c, P)
                                 }
                     }
-                    s = f = v = 0, O = E = 1, M = S = "", d = l;
+                    s = f = y = 0, O = E = 1, k = S = "", d = l;
                     break;
                 case 58:
-                    d = 1 + g(S), v = y;
+                    d = 1 + g(S), y = v;
                 default:
                     if (O < 1)
                         if (123 == j) --O;
                         else if (125 == j && 0 == O++ && 125 == C()) continue;
                     switch (S += p(j), j * O) {
                         case 38:
                             E = f > 0 ? 1 : (S += "\f", -1);
                             break;
                         case 44:
                             c[s++] = (g(S) - 1) * E, E = 1;
                             break;
                         case 64:
-                            45 === z() && (S += L(R())), h = z(), f = d = g(M = S += W(D())), j++;
+                            45 === z() && (S += L(R())), h = z(), f = d = g(k = S += W(D())), j++;
                             break;
                         case 45:
-                            45 === y && 2 == g(S) && (O = 0)
+                            45 === v && 2 == g(S) && (O = 0)
                     }
             }
             return i
         }("", null, null, null, [""], e = I(e), 0, [0], e))
     }
 
     function U(e, t, n, r, a, o, i, l, u, s, p) {
-        for (var d = a - 1, b = 0 === a ? o : [""], v = O(b), g = 0, _ = 0, w = 0; g < r; ++g)
-            for (var E = 0, j = y(e, d + 1, d = f(_ = i[g])), M = e; E < v; ++E)(M = h(_ > 0 ? b[E] + " " + j : m(j, /&\f/g, b[E]))) && (u[w++] = M);
+        for (var d = a - 1, b = 0 === a ? o : [""], y = O(b), g = 0, _ = 0, w = 0; g < r; ++g)
+            for (var E = 0, j = v(e, d + 1, d = f(_ = i[g])), k = e; E < y; ++E)(k = h(_ > 0 ? b[E] + " " + j : m(j, /&\f/g, b[E]))) && (u[w++] = k);
         return S(e, t, n, 0 === a ? c : l, u, s, p)
     }
 
     function K(e, t, n) {
-        return S(e, t, n, l, p(P), y(e, 2, -2), 0)
+        return S(e, t, n, l, p(P), v(e, 2, -2), 0)
     }
 
     function Y(e, t, n, r) {
-        return S(e, t, n, u, y(e, 0, r), y(e, r + 1, -1), r)
+        return S(e, t, n, u, v(e, 0, r), v(e, r + 1, -1), r)
     }
 
-    function Q(e, t) {
+    function G(e, t) {
         switch (function(e, t) {
-                return (((t << 2 ^ v(e, 0)) << 2 ^ v(e, 1)) << 2 ^ v(e, 2)) << 2 ^ v(e, 3)
+                return (((t << 2 ^ y(e, 0)) << 2 ^ y(e, 1)) << 2 ^ y(e, 2)) << 2 ^ y(e, 3)
             }(e, t)) {
             case 5103:
                 return i + "print-" + e + e;
             case 5737:
             case 4201:
             case 3177:
             case 3433:
@@ -9082,85 +9082,85 @@
             case 5701:
             case 4933:
             case 4677:
             case 5533:
             case 5789:
             case 5021:
             case 4765:
-                if (g(e) - 1 - t > 6) switch (v(e, t + 1)) {
+                if (g(e) - 1 - t > 6) switch (y(e, t + 1)) {
                     case 109:
-                        if (45 !== v(e, t + 4)) break;
+                        if (45 !== y(e, t + 4)) break;
                     case 102:
-                        return m(e, /(.+:)(.+)-([^]+)/, "$1" + i + "$2-$3$1" + o + (108 == v(e, t + 3) ? "$3" : "$2-$3")) + e;
+                        return m(e, /(.+:)(.+)-([^]+)/, "$1" + i + "$2-$3$1" + o + (108 == y(e, t + 3) ? "$3" : "$2-$3")) + e;
                     case 115:
-                        return ~b(e, "stretch") ? Q(m(e, "stretch", "fill-available"), t) + e : e
+                        return ~b(e, "stretch") ? G(m(e, "stretch", "fill-available"), t) + e : e
                 }
                 break;
             case 4949:
-                if (115 !== v(e, t + 1)) break;
+                if (115 !== y(e, t + 1)) break;
             case 6444:
-                switch (v(e, g(e) - 3 - (~b(e, "!important") && 10))) {
+                switch (y(e, g(e) - 3 - (~b(e, "!important") && 10))) {
                     case 107:
                         return m(e, ":", ":" + i) + e;
                     case 101:
-                        return m(e, /(.+:)([^;!]+)(;|!.+)?/, "$1" + i + (45 === v(e, 14) ? "inline-" : "") + "box$3$1" + i + "$2$3$1" + a + "$2box$3") + e
+                        return m(e, /(.+:)([^;!]+)(;|!.+)?/, "$1" + i + (45 === y(e, 14) ? "inline-" : "") + "box$3$1" + i + "$2$3$1" + a + "$2box$3") + e
                 }
                 break;
             case 5936:
-                switch (v(e, t + 11)) {
+                switch (y(e, t + 11)) {
                     case 114:
                         return i + e + a + m(e, /[svh]\w+-[tblr]{2}/, "tb") + e;
                     case 108:
                         return i + e + a + m(e, /[svh]\w+-[tblr]{2}/, "tb-rl") + e;
                     case 45:
                         return i + e + a + m(e, /[svh]\w+-[tblr]{2}/, "lr") + e
                 }
                 return i + e + a + e + e
         }
         return e
     }
 
-    function G(e, t) {
+    function Q(e, t) {
         for (var n = "", r = O(e), a = 0; a < r; a++) n += t(e[a], a, e, t) || "";
         return n
     }
 
     function J(e, t, n, r) {
         switch (e.type) {
             case "@import":
             case u:
                 return e.return = e.return || e.value;
             case l:
                 return "";
             case s:
-                return e.return = e.value + "{" + G(e.children, r) + "}";
+                return e.return = e.value + "{" + Q(e.children, r) + "}";
             case c:
                 e.value = e.props.join(",")
         }
-        return g(n = G(e.children, r)) ? e.return = e.value + "{" + n + "}" : ""
+        return g(n = Q(e.children, r)) ? e.return = e.value + "{" + n + "}" : ""
     }
 
     function Z(e) {
         return function(t) {
             t.root || (t = t.return) && e(t)
         }
     }
     n(47), n(73);
     var X = function(e, t, n) {
             for (var r = 0, a = 0; r = a, a = z(), 38 === r && 12 === a && (t[n] = 1), !N(a);) R();
-            return T(e, k)
+            return T(e, M)
         },
         $ = function(e, t) {
             return H(function(e, t) {
                 var n = -1,
                     r = 44;
                 do {
                     switch (N(r)) {
                         case 0:
-                            38 === r && 12 === z() && (t[n] = 1), e[n] += X(k - 1, t, n);
+                            38 === r && 12 === z() && (t[n] = 1), e[n] += X(M - 1, t, n);
                             break;
                         case 2:
                             e[n] += L(r);
                             break;
                         case 4:
                             if (44 === r) {
                                 e[++n] = 58 === z() ? "&\f" : "", t[n] = e[n].length;
@@ -9191,32 +9191,32 @@
                 var t = e.value;
                 108 === t.charCodeAt(0) && 98 === t.charCodeAt(2) && (e.return = "", e.value = "")
             }
         },
         re = [function(e, t, n, r) {
             if (e.length > -1 && !e.return) switch (e.type) {
                 case u:
-                    e.return = Q(e.value, e.length);
+                    e.return = G(e.value, e.length);
                     break;
                 case s:
-                    return G([A(e, {
+                    return Q([A(e, {
                         value: m(e.value, "@", "@" + i)
                     })], r);
                 case c:
                     if (e.length) return w(e.props, (function(t) {
                         switch (function(e, t) {
                                 return (e = t.exec(e)) ? e[0] : e
                             }(t, /(::plac\w+|:read-\w+)/)) {
                             case ":read-only":
                             case ":read-write":
-                                return G([A(e, {
+                                return Q([A(e, {
                                     props: [m(t, /:(read-\w+)/, ":-moz-$1")]
                                 })], r);
                             case "::placeholder":
-                                return G([A(e, {
+                                return Q([A(e, {
                                     props: [m(t, /:(plac\w+)/, ":" + i + "input-$1")]
                                 }), A(e, {
                                     props: [m(t, /:(plac\w+)/, ":-moz-$1")]
                                 }), A(e, {
                                     props: [m(t, /:(plac\w+)/, a + "input-$1")]
                                 })], r)
                         }
@@ -9247,15 +9247,15 @@
                 var t = O(e);
                 return function(n, r, a, o) {
                     for (var i = "", l = 0; l < t; l++) i += e[l](n, r, a, o) || "";
                     return i
                 }
             }(u.concat(a, f));
         i = function(e, t, n, r) {
-            s = n, G(V(e ? e + "{" + t.styles + "}" : t.styles), p), r && (d.inserted[t.name] = !0)
+            s = n, Q(V(e ? e + "{" + t.styles + "}" : t.styles), p), r && (d.inserted[t.name] = !0)
         };
         var d = {
             key: t,
             sheet: new r.a({
                 key: t,
                 container: o,
                 nonce: e.nonce,
@@ -9337,15 +9337,15 @@
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
     Object.defineProperty(t, "__esModule", {
         value: !0
-    }), t.default = v;
+    }), t.default = y;
     var a = f(n(0)),
         o = f(n(1)),
         i = f(n(21)),
         l = f(n(78)),
         c = function(e, t) {
             if (!t && e && e.__esModule) return e;
             if (null === e || "object" !== r(e) && "function" != typeof e) return {
@@ -9408,66 +9408,66 @@
                         return e && "selectionStart" in e && null !== e.selectionStart ? e.value.slice(e.selectionStart, e.selectionEnd) : "getSelection" in window ? window.getSelection().toString() : null
                     }(r);
                 o && (i || a.length < e) || t.preventDefault()
             }
         }
     }
 
-    function v(e) {
+    function y(e) {
         var t = e.ariaLabel,
             n = e.autoFocus,
             r = e.className,
             o = e.disabled,
             u = e.inputRef,
             s = e.max,
             f = e.min,
             p = e.name,
             d = e.nameForClass,
-            v = e.onChange,
-            y = e.onKeyDown,
+            y = e.onChange,
+            v = e.onKeyDown,
             g = e.onKeyUp,
             O = e.placeholder,
             _ = void 0 === O ? "--" : O,
             w = e.required,
             E = e.showLeadingZeros,
             j = e.step,
-            M = e.value,
-            k = E && M && M < 10 && ("0" === M || !M.toString().startsWith("0")),
+            k = e.value,
+            M = E && k && k < 10 && ("0" === k || !k.toString().startsWith("0")),
             P = s ? s.toString().length : null;
-        return [k && a.default.createElement("span", {
+        return [M && a.default.createElement("span", {
             key: "leadingZero",
             className: "".concat(r, "__leadingZero")
         }, "0"), a.default.createElement("input", {
             key: "input",
             "aria-label": t,
             autoComplete: "off",
             autoFocus: n,
-            className: (0, i.default)("".concat(r, "__input"), "".concat(r, "__").concat(d || p), k && "".concat(r, "__input--hasLeadingZero")),
+            className: (0, i.default)("".concat(r, "__input"), "".concat(r, "__").concat(d || p), M && "".concat(r, "__input--hasLeadingZero")),
             "data-input": "true",
             disabled: o,
             inputMode: "numeric",
             max: s,
             min: f,
             name: p,
-            onChange: v,
+            onChange: y,
             onFocus: h,
-            onKeyDown: y,
+            onKeyDown: v,
             onKeyPress: b(P),
             onKeyUp: function(e) {
                 (0, c.default)(e.target), g && g(e)
             },
             placeholder: _,
             ref: (0, l.default)(c.default, m, u),
             required: w,
             step: j,
             type: "number",
-            value: null !== M ? M : ""
+            value: null !== k ? k : ""
         })]
     }
-    v.propTypes = {
+    y.propTypes = {
         ariaLabel: o.default.string,
         autoFocus: o.default.bool,
         className: o.default.string.isRequired,
         disabled: o.default.bool,
         inputRef: u.isRef,
         max: o.default.number,
         min: o.default.number,
@@ -9804,45 +9804,45 @@
                     s = n.newParameterType,
                     f = n.newParameterName,
                     p = n.newOptionList,
                     d = n.newSelectedCol,
                     h = n.newSelectedCols,
                     m = n.newSelectedSubset,
                     b = this.state.parameters ? this.state.parameters : [],
-                    v = d ? i[d].cat.map((function(e) {
+                    y = d ? i[d].cat.map((function(e) {
                         return {
                             label: e,
                             value: e
                         }
                     })) : [],
-                    y = c;
-                delete y.parameterization;
+                    v = c;
+                delete v.parameterization;
                 try {
-                    y && u.forEach((function(e) {
-                        y = y[e]
+                    v && u.forEach((function(e) {
+                        v = v[e]
                     }))
                 } catch (e) {
                     this.setState({
                         newPath: []
                     })
                 }
                 var g = "",
                     O = !1,
                     _ = !1,
                     w = !1,
                     E = !1,
                     j = !1,
-                    M = !1;
-                if ("object" !== _typeof(y) || Array.isArray(y) && "object" !== _typeof(y[0])) {
-                    e = "", g = JSON.stringify(y), j = !0, O = "string" == typeof y, _ = "number" == typeof y;
+                    k = !1;
+                if ("object" !== _typeof(v) || Array.isArray(v) && "object" !== _typeof(v[0])) {
+                    e = "", g = JSON.stringify(v), j = !0, O = "string" == typeof v, _ = "number" == typeof v;
                     try {
-                        w = Array.isArray(y) && "string" == typeof y[0], E = Array.isArray(y) && "number" == typeof y[0], M = Array.isArray(y)
+                        w = Array.isArray(v) && "string" == typeof v[0], E = Array.isArray(v) && "number" == typeof v[0], k = Array.isArray(v)
                     } catch (e) {}
                 } else try {
-                    e = Object.keys(y).map((function(e) {
+                    e = Object.keys(v).map((function(e) {
                         return react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(react_bootstrap_Button__WEBPACK_IMPORTED_MODULE_4__.a, {
                             key: "to-" + e,
                             variant: "secondary",
                             className: "m-1",
                             onClick: function() {
                                 var n = [].concat(_toConsumableArray(u), [e]);
                                 t.setState({
@@ -9911,21 +9911,21 @@
                     value: "us"
                 }, "user defined string"), _ && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
                     value: "uf"
                 }, "user defined float"), w && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
                     value: "usa"
                 }, "user defined string array"), E && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
                     value: "ufa"
-                }, "user defined float array"), j && !M && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
+                }, "user defined float array"), j && !k && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
                     value: "o"
-                }, "meta options"), j && !M && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
+                }, "meta options"), j && !k && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
                     value: "mos"
-                }, "meta option subset"), j && !M && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
+                }, "meta option subset"), j && !k && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
                     value: "cos"
-                }, "column option subset"), j && !M && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
+                }, "column option subset"), j && !k && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("option", {
                     value: "mo"
                 }, "manual options"))), ["mo"].includes(s) && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("div", null, "Add some options and press enter to keep", react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(react_list_editable__WEBPACK_IMPORTED_MODULE_8___default.a, {
                     list: p,
                     className: "w-100",
                     onListChange: function(e) {
                         return t.setState({
                             newOptionList: e
@@ -9944,18 +9944,18 @@
                             newSelectedCol: void 0
                         })
                     },
                     isClearable: !0,
                     styles: _sub_Base_react__WEBPACK_IMPORTED_MODULE_1__.e,
                     components: _sub_Base_react__WEBPACK_IMPORTED_MODULE_1__.b
                 })), "mos" === s && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("div", null, "Select a column name is input value:", react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(react_select__WEBPACK_IMPORTED_MODULE_10__.a, _extends({
-                    options: v
+                    options: y
                 }, Object(_sub_Base_react__WEBPACK_IMPORTED_MODULE_1__.c)(this, (function(e) {
                     return t.setState(e)
-                }), "newSelectedSubset", v)))), "cos" === s && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("div", null, "Select the unique options as input value:", react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(react_select__WEBPACK_IMPORTED_MODULE_10__.a, _extends({
+                }), "newSelectedSubset", y)))), "cos" === s && react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement("div", null, "Select the unique options as input value:", react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(react_select__WEBPACK_IMPORTED_MODULE_10__.a, _extends({
                     options: r,
                     styles: _sub_Base_react__WEBPACK_IMPORTED_MODULE_1__.d,
                     components: _sub_Base_react__WEBPACK_IMPORTED_MODULE_1__.b
                 }, Object(_sub_Base_react__WEBPACK_IMPORTED_MODULE_1__.c)(this, (function(e) {
                     return t.setState(e)
                 }), "newSelectedCols", o))))), react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(react_bootstrap_Modal__WEBPACK_IMPORTED_MODULE_7__.a.Footer, null, react__WEBPACK_IMPORTED_MODULE_0___default.a.createElement(react_bootstrap_Button__WEBPACK_IMPORTED_MODULE_4__.a, {
                     variant: "secondary",
@@ -9968,15 +9968,15 @@
                         if (!(0 == f.length || b.filter((function(e) {
                                 return e.name === f
                             })).length > 0)) {
                             var n = {
                                 name: f,
                                 type: s,
                                 path: u,
-                                value: y
+                                value: v
                             };
                             "o" === s && (n.col = d, n.value = i[d].cat[0]), "mos" === s && (n.options = m, n.value = m[0]), "cos" === s && (n.options = h, n.value = h[0]), "mo" === s && (E && (p.map((function(e) {
                                 return parseFloat(e)
                             })), _readOnlyError("newOptionList")), n.options = p, n.value = p[0]);
                             var r = [].concat(_toConsumableArray(b), [n]);
                             t.setState({
                                 parameters: r
@@ -10428,16 +10428,16 @@
                         u = r.current;
                     return r.current = c, !c && u && i !== t && l(t), [c ? e : i, Object(o.useCallback)((function(e) {
                         for (var t = arguments.length, r = new Array(t > 1 ? t - 1 : 0), a = 1; a < t; a++) r[a - 1] = arguments[a];
                         n && n.apply(void 0, [e].concat(r)), l(e)
                     }), [n])]
                 }(p, f, e[h]),
                 b = m[0],
-                v = m[1];
-            return Object(r.a)({}, d, ((u = {})[c] = b, u[h] = v, u))
+                y = m[1];
+            return Object(r.a)({}, d, ((u = {})[c] = b, u[h] = y, u))
         }), e)
     }
     n(59);
 
     function u() {
         var e = this.constructor.getDerivedStateFromProps(this.props, this.state);
         null != e && this.setState(e)
@@ -10501,15 +10501,15 @@
     n.d(t, "a", (function() {
         return i
     }))
 }, function(e, t, n) {
     "use strict";
     var r = n(0),
         a = n.n(r),
-        o = n(26),
+        o = n(27),
         i = n(63),
         l = n(15),
         c = n.n(l);
     var u = n(2);
     const s = a.a.forwardRef(({
         onEnter: e,
         onEntering: t,
@@ -10518,41 +10518,41 @@
         onExiting: s,
         onExited: f,
         addEndListener: p,
         children: d,
         childRef: h,
         ...m
     }, b) => {
-        const v = Object(r.useRef)(null),
-            y = Object(i.a)(v, h),
+        const y = Object(r.useRef)(null),
+            v = Object(i.a)(y, h),
             g = e => {
                 var t;
-                y((t = e) && "setState" in t ? c.a.findDOMNode(t) : null != t ? t : null)
+                v((t = e) && "setState" in t ? c.a.findDOMNode(t) : null != t ? t : null)
             },
             O = e => t => {
-                e && v.current && e(v.current, t)
+                e && y.current && e(y.current, t)
             },
             _ = Object(r.useCallback)(O(e), [e]),
             w = Object(r.useCallback)(O(t), [t]),
             E = Object(r.useCallback)(O(n), [n]),
             j = Object(r.useCallback)(O(l), [l]),
-            M = Object(r.useCallback)(O(s), [s]),
-            k = Object(r.useCallback)(O(f), [f]),
+            k = Object(r.useCallback)(O(s), [s]),
+            M = Object(r.useCallback)(O(f), [f]),
             P = Object(r.useCallback)(O(p), [p]);
         return Object(u.jsx)(o.e, {
             ref: b,
             ...m,
             onEnter: _,
             onEntered: E,
             onEntering: w,
             onExit: j,
-            onExited: k,
-            onExiting: M,
+            onExited: M,
+            onExiting: k,
             addEndListener: P,
-            nodeRef: v,
+            nodeRef: y,
             children: "function" == typeof d ? (e, t) => d(e, {
                 ...t,
                 ref: g
             }) : a.a.cloneElement(d, {
                 ref: g
             })
         })
@@ -10566,15 +10566,15 @@
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
     Object.defineProperty(t, "__esModule", {
         value: !0
-    }), t.default = v;
+    }), t.default = y;
     var a = f(n(0)),
         o = f(n(1)),
         i = f(n(21)),
         l = f(n(78)),
         c = function(e, t) {
             if (!t && e && e.__esModule) return e;
             if (null === e || "object" !== r(e) && "function" != typeof e) return {
@@ -10637,66 +10637,66 @@
                         return e && "selectionStart" in e && null !== e.selectionStart ? e.value.slice(e.selectionStart, e.selectionEnd) : "getSelection" in window ? window.getSelection().toString() : null
                     }(r);
                 o && (i || a.length < e) || t.preventDefault()
             }
         }
     }
 
-    function v(e) {
+    function y(e) {
         var t = e.ariaLabel,
             n = e.autoFocus,
             r = e.className,
             o = e.disabled,
             u = e.inputRef,
             s = e.max,
             f = e.min,
             p = e.name,
             d = e.nameForClass,
-            v = e.onChange,
-            y = e.onKeyDown,
+            y = e.onChange,
+            v = e.onKeyDown,
             g = e.onKeyUp,
             O = e.placeholder,
             _ = void 0 === O ? "--" : O,
             w = e.required,
             E = e.showLeadingZeros,
             j = e.step,
-            M = e.value,
-            k = E && M && M < 10 && ("0" === M || !M.toString().startsWith("0")),
+            k = e.value,
+            M = E && k && k < 10 && ("0" === k || !k.toString().startsWith("0")),
             P = s ? s.toString().length : null;
-        return [k && a.default.createElement("span", {
+        return [M && a.default.createElement("span", {
             key: "leadingZero",
             className: "".concat(r, "__leadingZero")
         }, "0"), a.default.createElement("input", {
             key: "input",
             "aria-label": t,
             autoComplete: "off",
             autoFocus: n,
-            className: (0, i.default)("".concat(r, "__input"), "".concat(r, "__").concat(d || p), k && "".concat(r, "__input--hasLeadingZero")),
+            className: (0, i.default)("".concat(r, "__input"), "".concat(r, "__").concat(d || p), M && "".concat(r, "__input--hasLeadingZero")),
             "data-input": "true",
             disabled: o,
             inputMode: "numeric",
             max: s,
             min: f,
             name: p,
-            onChange: v,
+            onChange: y,
             onFocus: h,
-            onKeyDown: y,
+            onKeyDown: v,
             onKeyPress: b(P),
             onKeyUp: function(e) {
                 (0, c.default)(e.target), g && g(e)
             },
             placeholder: _,
             ref: (0, l.default)(c.default, m, u),
             required: w,
             step: j,
             type: "number",
-            value: null !== M ? M : ""
+            value: null !== k ? k : ""
         })]
     }
-    v.propTypes = {
+    y.propTypes = {
         ariaLabel: o.default.string,
         autoFocus: o.default.bool,
         className: o.default.string.isRequired,
         disabled: o.default.bool,
         inputRef: u.isRef,
         max: o.default.number,
         min: o.default.number,
@@ -10808,19 +10808,19 @@
             if (h) {
                 var a = d(n);
                 a && a !== h && e(t, a, r)
             }
             var i = s(n);
             f && (i = i.concat(f(n)));
             for (var l = c(t), m = c(n), b = 0; b < i.length; ++b) {
-                var v = i[b];
-                if (!(o[v] || r && r[v] || m && m[v] || l && l[v])) {
-                    var y = p(n, v);
+                var y = i[b];
+                if (!(o[y] || r && r[y] || m && m[y] || l && l[y])) {
+                    var v = p(n, y);
                     try {
-                        u(t, v, y)
+                        u(t, y, v)
                     } catch (e) {}
                 }
             }
         }
         return t
     }
 }, function(e, t, n) {
@@ -11133,25 +11133,25 @@
             var l = a.test(e);
             return l || o.test(e) ? i(e.slice(2), l ? 2 : 8) : r.test(e) ? NaN : +e
         }
         e.exports = function(e, t, n) {
             var r, a, o, i, l, c, u = 0,
                 s = !1,
                 b = !1,
-                v = !0;
+                y = !0;
             if ("function" != typeof e) throw new TypeError("Expected a function");
 
-            function y(t) {
+            function v(t) {
                 var n = r,
                     o = a;
                 return r = a = void 0, u = t, i = e.apply(o, n)
             }
 
             function g(e) {
-                return u = e, l = setTimeout(_, t), s ? y(e) : i
+                return u = e, l = setTimeout(_, t), s ? v(e) : i
             }
 
             function O(e) {
                 var n = e - c;
                 return void 0 === c || n >= t || n < 0 || b && e - u >= o
             }
 
@@ -11161,27 +11161,27 @@
                 l = setTimeout(_, function(e) {
                     var n = t - (e - c);
                     return b ? p(n, o - (e - u)) : n
                 }(e))
             }
 
             function w(e) {
-                return l = void 0, v && r ? y(e) : (r = a = void 0, i)
+                return l = void 0, y && r ? v(e) : (r = a = void 0, i)
             }
 
             function E() {
                 var e = d(),
                     n = O(e);
                 if (r = arguments, a = this, c = e, n) {
                     if (void 0 === l) return g(c);
-                    if (b) return l = setTimeout(_, t), y(c)
+                    if (b) return l = setTimeout(_, t), v(c)
                 }
                 return void 0 === l && (l = setTimeout(_, t)), i
             }
-            return t = m(t) || 0, h(n) && (s = !!n.leading, o = (b = "maxWait" in n) ? f(m(n.maxWait) || 0, t) : o, v = "trailing" in n ? !!n.trailing : v), E.cancel = function() {
+            return t = m(t) || 0, h(n) && (s = !!n.leading, o = (b = "maxWait" in n) ? f(m(n.maxWait) || 0, t) : o, y = "trailing" in n ? !!n.trailing : y), E.cancel = function() {
                 void 0 !== l && clearTimeout(l), u = 0, r = c = a = l = void 0
             }, E.flush = function() {
                 return void 0 === l ? i : w(d())
             }, E
         }
     }).call(this, n(50))
 }, function(e, t, n) {
@@ -11201,25 +11201,25 @@
                 return u.Date.now()
             };
 
         function h(e, t, n) {
             var r, a, o, i, l, c, u = 0,
                 s = !1,
                 h = !1,
-                v = !0;
+                y = !0;
             if ("function" != typeof e) throw new TypeError("Expected a function");
 
-            function y(t) {
+            function v(t) {
                 var n = r,
                     o = a;
                 return r = a = void 0, u = t, i = e.apply(o, n)
             }
 
             function g(e) {
-                return u = e, l = setTimeout(_, t), s ? y(e) : i
+                return u = e, l = setTimeout(_, t), s ? v(e) : i
             }
 
             function O(e) {
                 var n = e - c;
                 return void 0 === c || n >= t || n < 0 || h && e - u >= o
             }
 
@@ -11229,27 +11229,27 @@
                 l = setTimeout(_, function(e) {
                     var n = t - (e - c);
                     return h ? p(n, o - (e - u)) : n
                 }(e))
             }
 
             function w(e) {
-                return l = void 0, v && r ? y(e) : (r = a = void 0, i)
+                return l = void 0, y && r ? v(e) : (r = a = void 0, i)
             }
 
             function E() {
                 var e = d(),
                     n = O(e);
                 if (r = arguments, a = this, c = e, n) {
                     if (void 0 === l) return g(c);
-                    if (h) return l = setTimeout(_, t), y(c)
+                    if (h) return l = setTimeout(_, t), v(c)
                 }
                 return void 0 === l && (l = setTimeout(_, t)), i
             }
-            return t = b(t) || 0, m(n) && (s = !!n.leading, o = (h = "maxWait" in n) ? f(b(n.maxWait) || 0, t) : o, v = "trailing" in n ? !!n.trailing : v), E.cancel = function() {
+            return t = b(t) || 0, m(n) && (s = !!n.leading, o = (h = "maxWait" in n) ? f(b(n.maxWait) || 0, t) : o, y = "trailing" in n ? !!n.trailing : y), E.cancel = function() {
                 void 0 !== l && clearTimeout(l), u = 0, r = c = a = l = void 0
             }, E.flush = function() {
                 return void 0 === l ? i : w(d())
             }, E
         }
 
         function m(e) {
@@ -11341,16 +11341,16 @@
         s = r ? Symbol.for("react.context") : 60110,
         f = r ? Symbol.for("react.async_mode") : 60111,
         p = r ? Symbol.for("react.concurrent_mode") : 60111,
         d = r ? Symbol.for("react.forward_ref") : 60112,
         h = r ? Symbol.for("react.suspense") : 60113,
         m = r ? Symbol.for("react.suspense_list") : 60120,
         b = r ? Symbol.for("react.memo") : 60115,
-        v = r ? Symbol.for("react.lazy") : 60116,
-        y = r ? Symbol.for("react.block") : 60121,
+        y = r ? Symbol.for("react.lazy") : 60116,
+        v = r ? Symbol.for("react.block") : 60121,
         g = r ? Symbol.for("react.fundamental") : 60117,
         O = r ? Symbol.for("react.responder") : 60118,
         _ = r ? Symbol.for("react.scope") : 60119;
 
     function w(e) {
         if ("object" == typeof e && null !== e) {
             var t = e.$$typeof;
@@ -11364,15 +11364,15 @@
                         case l:
                         case h:
                             return e;
                         default:
                             switch (e = e && e.$$typeof) {
                                 case s:
                                 case d:
-                                case v:
+                                case y:
                                 case b:
                                 case u:
                                     return e;
                                 default:
                                     return t
                             }
                     }
@@ -11381,40 +11381,40 @@
             }
         }
     }
 
     function E(e) {
         return w(e) === p
     }
-    t.AsyncMode = f, t.ConcurrentMode = p, t.ContextConsumer = s, t.ContextProvider = u, t.Element = a, t.ForwardRef = d, t.Fragment = i, t.Lazy = v, t.Memo = b, t.Portal = o, t.Profiler = c, t.StrictMode = l, t.Suspense = h, t.isAsyncMode = function(e) {
+    t.AsyncMode = f, t.ConcurrentMode = p, t.ContextConsumer = s, t.ContextProvider = u, t.Element = a, t.ForwardRef = d, t.Fragment = i, t.Lazy = y, t.Memo = b, t.Portal = o, t.Profiler = c, t.StrictMode = l, t.Suspense = h, t.isAsyncMode = function(e) {
         return E(e) || w(e) === f
     }, t.isConcurrentMode = E, t.isContextConsumer = function(e) {
         return w(e) === s
     }, t.isContextProvider = function(e) {
         return w(e) === u
     }, t.isElement = function(e) {
         return "object" == typeof e && null !== e && e.$$typeof === a
     }, t.isForwardRef = function(e) {
         return w(e) === d
     }, t.isFragment = function(e) {
         return w(e) === i
     }, t.isLazy = function(e) {
-        return w(e) === v
+        return w(e) === y
     }, t.isMemo = function(e) {
         return w(e) === b
     }, t.isPortal = function(e) {
         return w(e) === o
     }, t.isProfiler = function(e) {
         return w(e) === c
     }, t.isStrictMode = function(e) {
         return w(e) === l
     }, t.isSuspense = function(e) {
         return w(e) === h
     }, t.isValidElementType = function(e) {
-        return "string" == typeof e || "function" == typeof e || e === i || e === p || e === c || e === l || e === h || e === m || "object" == typeof e && null !== e && (e.$$typeof === v || e.$$typeof === b || e.$$typeof === u || e.$$typeof === s || e.$$typeof === d || e.$$typeof === g || e.$$typeof === O || e.$$typeof === _ || e.$$typeof === y)
+        return "string" == typeof e || "function" == typeof e || e === i || e === p || e === c || e === l || e === h || e === m || "object" == typeof e && null !== e && (e.$$typeof === y || e.$$typeof === b || e.$$typeof === u || e.$$typeof === s || e.$$typeof === d || e.$$typeof === g || e.$$typeof === O || e.$$typeof === _ || e.$$typeof === v)
     }, t.typeOf = w
 }, function(e, t, n) {
     var r = n(97);
     "string" == typeof r && (r = [
         [e.i, r, ""]
     ]);
     var a = {
@@ -11456,15 +11456,15 @@
         value: !0
     }), t.default = void 0;
     var a = function(e, t) {
             if (!t && e && e.__esModule) return e;
             if (null === e || "object" !== r(e) && "function" != typeof e) return {
                 default: e
             };
-            var n = v(t);
+            var n = y(t);
             if (n && n.has(e)) return n.get(e);
             var a = {},
                 o = Object.defineProperty && Object.getOwnPropertyDescriptor;
             for (var i in e)
                 if ("default" !== i && Object.prototype.hasOwnProperty.call(e, i)) {
                     var l = o ? Object.getOwnPropertyDescriptor(e, i) : null;
                     l && (l.get || l.set) ? Object.defineProperty(a, i, l) : a[i] = e[i]
@@ -11485,24 +11485,24 @@
 
     function b(e) {
         return e && e.__esModule ? e : {
             default: e
         }
     }
 
-    function v(e) {
+    function y(e) {
         if ("function" != typeof WeakMap) return null;
         var t = new WeakMap,
             n = new WeakMap;
-        return (v = function(e) {
+        return (y = function(e) {
             return e ? n : t
         })(e)
     }
 
-    function y(e, t) {
+    function v(e, t) {
         if (null == e) return {};
         var n, r, a = function(e, t) {
             if (null == e) return {};
             var n, r, a = {},
                 o = Object.keys(e);
             for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
             return a
@@ -11576,15 +11576,15 @@
 
     function j(e, t) {
         return (j = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function M(e) {
+    function k(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -11593,19 +11593,19 @@
         }();
         return function() {
             var n, r = x(e);
             if (t) {
                 var a = x(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
-            return k(this, n)
+            return M(this, n)
         }
     }
 
-    function k(e, t) {
+    function M(e, t) {
         if (t && ("object" === r(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return P(e)
     }
 
     function P(e) {
         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
@@ -11636,15 +11636,15 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }), t && j(e, t)
             }(p, e);
-            var t, n, r, o = M(p);
+            var t, n, r, o = k(p);
 
             function p() {
                 var e;
                 w(this, p);
                 for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
                 return S(P(e = o.call.apply(o, [this].concat(n))), "state", {}), S(P(e), "onOutsideAction", (function(t) {
                     var n = "composedPath" in t ? t.composedPath()[0] : t.target;
@@ -11778,22 +11778,22 @@
                         u = e.dayPlaceholder,
                         s = e.disableCalendar,
                         p = e.disabled,
                         d = e.format,
                         h = e.hourAriaLabel,
                         m = e.hourPlaceholder,
                         b = e.locale,
-                        v = e.maxDate,
-                        y = e.maxDetail,
+                        y = e.maxDate,
+                        v = e.maxDetail,
                         _ = e.minDate,
                         w = e.minuteAriaLabel,
                         E = e.minutePlaceholder,
                         j = e.monthAriaLabel,
-                        M = e.monthPlaceholder,
-                        k = e.name,
+                        k = e.monthPlaceholder,
+                        M = e.name,
                         P = e.nativeInputAriaLabel,
                         x = e.required,
                         S = e.secondAriaLabel,
                         A = e.secondPlaceholder,
                         R = e.showLeadingZeros,
                         z = e.value,
                         D = e.yearAriaLabel,
@@ -11812,31 +11812,31 @@
                             secondAriaLabel: S,
                             yearAriaLabel: D
                         },
                         q = {
                             dayPlaceholder: u,
                             hourPlaceholder: m,
                             minutePlaceholder: E,
-                            monthPlaceholder: M,
+                            monthPlaceholder: k,
                             secondPlaceholder: A,
                             yearPlaceholder: T
                         };
                     return a.default.createElement("div", {
                         className: "".concat(C, "__wrapper")
                     }, a.default.createElement(f.default, g({}, B, q, {
                         autoFocus: n,
                         className: "".concat(C, "__inputGroup"),
                         disabled: p,
                         format: d,
                         isWidgetOpen: I || H,
                         locale: b,
-                        maxDate: v,
-                        maxDetail: y,
+                        maxDate: y,
+                        maxDetail: v,
                         minDate: _,
-                        name: k,
+                        name: M,
                         onChange: this.onChange,
                         placeholder: this.placeholder,
                         required: x,
                         showLeadingZeros: R,
                         value: L
                     })), null !== l && a.default.createElement("button", {
                         "aria-label": i,
@@ -11860,15 +11860,15 @@
                 value: function() {
                     var e = this.props.disableCalendar,
                         t = this.state.isCalendarOpen;
                     if (null === t || e) return null;
                     var n = this.props,
                         r = n.calendarClassName,
                         o = (n.className, n.maxDetail, n.onChange, n.value),
-                        i = y(n, d),
+                        i = v(n, d),
                         s = "".concat(C, "__calendar");
                     return a.default.createElement(u.default, null, a.default.createElement("div", {
                         className: (0, l.default)(s, "".concat(s, "--").concat(t ? "open" : "closed"))
                     }, a.default.createElement(c.default, g({
                         className: r,
                         onChange: this.onDateChange,
                         value: o || null
@@ -11880,15 +11880,15 @@
                     var e = this.props.disableClock,
                         t = this.state.isClockOpen;
                     if (null === t || e) return null;
                     var n = this.props,
                         r = n.clockClassName,
                         o = (n.className, n.maxDetail),
                         i = (n.onChange, n.value),
-                        c = y(n, h),
+                        c = v(n, h),
                         f = "".concat(C, "__clock"),
                         p = O([].concat(i), 1)[0],
                         d = A.indexOf(o);
                     return a.default.createElement(u.default, null, a.default.createElement("div", {
                         className: (0, l.default)(f, "".concat(f, "--").concat(t ? "open" : "closed"))
                     }, a.default.createElement(s.default, g({
                         className: r,
@@ -11902,15 +11902,15 @@
                 value: function() {
                     var e = this,
                         t = this.eventProps,
                         n = this.props,
                         r = n.className,
                         o = n.disabled,
                         i = this.state.isOpen,
-                        c = (t.onChange, y(t, m));
+                        c = (t.onChange, v(t, m));
                     return a.default.createElement("div", g({
                         className: (0, l.default)(C, "".concat(C, "--").concat(i ? "open" : "closed"), "".concat(C, "--").concat(o ? "disabled" : "enabled"), r)
                     }, c, {
                         onFocus: this.onFocus,
                         ref: function(t) {
                             t && (e.wrapper = t)
                         }
@@ -12042,17 +12042,17 @@
     })), n.d(t, "wheelEvents", (function() {
         return h
     })), n.d(t, "mediaEvents", (function() {
         return m
     })), n.d(t, "imageEvents", (function() {
         return b
     })), n.d(t, "animationEvents", (function() {
-        return v
-    })), n.d(t, "transitionEvents", (function() {
         return y
+    })), n.d(t, "transitionEvents", (function() {
+        return v
     })), n.d(t, "otherEvents", (function() {
         return g
     })), n.d(t, "allEvents", (function() {
         return O
     }));
     var r = ["onCopy", "onCut", "onPaste"],
         a = ["onCompositionEnd", "onCompositionStart", "onCompositionUpdate"],
@@ -12064,18 +12064,18 @@
         s = ["onPointerDown", "onPointerMove", "onPointerUp", "onPointerCancel", "onGotPointerCapture", "onLostPointerCapture", "onPointerEnter", "onPointerLeave", "onPointerOver", "onPointerOut"],
         f = ["onSelect"],
         p = ["onTouchCancel", "onTouchEnd", "onTouchMove", "onTouchStart"],
         d = ["onScroll"],
         h = ["onWheel"],
         m = ["onAbort", "onCanPlay", "onCanPlayThrough", "onDurationChange", "onEmptied", "onEncrypted", "onEnded", "onError", "onLoadedData", "onLoadedMetadata", "onLoadStart", "onPause", "onPlay", "onPlaying", "onProgress", "onRateChange", "onSeeked", "onSeeking", "onStalled", "onSuspend", "onTimeUpdate", "onVolumeChange", "onWaiting"],
         b = ["onLoad", "onError"],
-        v = ["onAnimationStart", "onAnimationEnd", "onAnimationIteration"],
-        y = ["onTransitionEnd"],
+        y = ["onAnimationStart", "onAnimationEnd", "onAnimationIteration"],
+        v = ["onTransitionEnd"],
         g = ["onToggle"],
-        O = [].concat(r, a, o, i, l, c, u, s, f, p, d, h, m, b, v, y, g);
+        O = [].concat(r, a, o, i, l, c, u, s, f, p, d, h, m, b, y, v, g);
     t.default = function(e, t) {
         var n = {};
         return O.forEach((function(r) {
             r in e && (n[r] = t ? function(n) {
                 return e[r](n, t(r))
             } : e[r])
         })), n
@@ -12117,16 +12117,16 @@
         s = w(n(107)),
         f = w(n(108)),
         p = w(n(110)),
         d = w(n(111)),
         h = w(n(112)),
         m = w(n(113)),
         b = w(n(114)),
-        v = w(n(115)),
-        y = n(81),
+        y = w(n(115)),
+        v = n(81),
         g = n(116),
         O = n(72),
         _ = n(117);
 
     function w(e) {
         return e && e.__esModule ? e : {
             default: e
@@ -12148,15 +12148,15 @@
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
 
-    function M(e, t) {
+    function k(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null == n) return;
             var r, a, o = [],
                 i = !0,
@@ -12174,15 +12174,15 @@
             }
             return o
         }(e, t) || T(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function k(e, t) {
+    function M(e, t) {
         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
     }
 
     function P(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
@@ -12311,30 +12311,30 @@
         } while (n && !U(n));
         return n
     }
 
     function Y(e) {
         e && e.focus()
     }
-    var Q = function(e) {
+    var G = function(e) {
         ! function(e, t) {
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             e.prototype = Object.create(t && t.prototype, {
                 constructor: {
                     value: e,
                     writable: !0,
                     configurable: !0
                 }
             }), t && x(e, t)
         }(O, e);
         var t, n, r, o = S(O);
 
         function O() {
             var e;
-            k(this, O);
+            M(this, O);
             for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
             return z(C(e = o.call.apply(o, [this].concat(n))), "state", {
                 amPm: null,
                 year: null,
                 month: null,
                 day: null,
                 hour: null,
@@ -12381,33 +12381,33 @@
                         e.setState(z({}, r, a), e.onChangeExternal)
                 }
             })), z(C(e), "onChangeNative", (function(t) {
                 var n = e.props.onChange,
                     r = t.target.value;
                 n && n(function() {
                     if (!r) return null;
-                    var e = M(r.split("T"), 2),
+                    var e = k(r.split("T"), 2),
                         t = e[0],
                         n = e[1],
-                        a = M(t.split("-"), 3),
+                        a = k(t.split("-"), 3),
                         o = a[0],
                         i = a[1],
                         l = a[2],
                         c = parseInt(o, 10),
                         u = parseInt(i, 10) - 1 || 0,
                         s = parseInt(l, 10) || 1,
-                        f = M(n.split(":"), 3),
+                        f = k(n.split(":"), 3),
                         p = f[0],
                         d = f[1],
                         h = f[2],
                         m = parseInt(p, 10) || 0,
                         b = parseInt(d, 10) || 0,
-                        v = parseInt(h, 10) || 0,
-                        y = new Date;
-                    return y.setFullYear(c, u, s), y.setHours(m, b, v, 0), y
+                        y = parseInt(h, 10) || 0,
+                        v = new Date;
+                    return v.setFullYear(c, u, s), v.setHours(m, b, y, 0), v
                 }(), !1)
             })), z(C(e), "onChangeAmPm", (function(t) {
                 var n = t.target.value;
                 e.setState({
                     amPm: n
                 }, e.onChangeExternal)
             })), z(C(e), "onChangeExternal", (function() {
@@ -12635,35 +12635,35 @@
                         return W({
                             value: e,
                             minDate: n,
                             maxDate: r
                         }, 1)
                     }))))) {
                     if (o) {
-                        var c = M((0, g.convert24to12)((0, i.getHours)(o)), 2);
+                        var c = k((0, g.convert24to12)((0, i.getHours)(o)), 2);
                         a.amPm = c[1], a.year = (0, i.getYear)(o).toString(), a.month = (0, i.getMonthHuman)(o).toString(), a.day = (0, i.getDate)(o).toString(), a.hour = (0, i.getHours)(o).toString(), a.minute = (0, i.getMinutes)(o).toString(), a.second = (0, i.getSeconds)(o).toString()
                     } else a.amPm = null, a.year = null, a.month = null, a.day = null, a.hour = null, a.minute = null, a.second = null;
                     a.value = o
                 }
                 return a
             }
         }], (n = [{
             key: "formatTime",
             get: function() {
                 var e = this.props.maxDetail,
                     t = {
                         hour: "numeric"
                     },
                     n = L.indexOf(e);
-                return n >= 1 && (t.minute = "numeric"), n >= 2 && (t.second = "numeric"), (0, y.getFormatter)(t)
+                return n >= 1 && (t.minute = "numeric"), n >= 2 && (t.second = "numeric"), (0, v.getFormatter)(t)
             }
         }, {
             key: "formatNumber",
             get: function() {
-                return (0, y.getFormatter)({
+                return (0, v.getFormatter)({
                     useGrouping: !1
                 })
             }
         }, {
             key: "dateDivider",
             get: function() {
                 return this.datePlaceholder.match(/[^0-9a-z]/i)[0]
@@ -12674,19 +12674,19 @@
                 return this.timePlaceholder.match(/[^0-9a-z]/i)[0]
             }
         }, {
             key: "datePlaceholder",
             get: function() {
                 var e = this.props.locale,
                     t = new Date(2017, 11, 11),
-                    n = (0, y.formatDate)(e, t),
+                    n = (0, v.formatDate)(e, t),
                     r = ["y", "M", "d"],
                     a = n;
                 return ["year", "month", "day"].forEach((function(n, o) {
-                    var i, l, c = (i = n, l = t, (0, y.getFormatter)(z({
+                    var i, l, c = (i = n, l = t, (0, v.getFormatter)(z({
                             useGrouping: !1
                         }, i, "numeric"))(e, l).match(/\d{1,}/)),
                         u = r[o];
                     a = a.replace(c, u)
                 })), a = a.replace("17", "y")
             }
         }, {
@@ -12796,15 +12796,15 @@
                     t = e.disabled,
                     n = e.maxDate,
                     r = e.minDate,
                     o = e.name,
                     i = e.nativeInputAriaLabel,
                     l = e.required,
                     c = this.state.value;
-                return a.default.createElement(v.default, {
+                return a.default.createElement(y.default, {
                     key: "time",
                     ariaLabel: i,
                     disabled: t,
                     maxDate: n || H,
                     minDate: r || I,
                     name: o,
                     onChange: this.onChangeNative,
@@ -12820,20 +12820,20 @@
                 return a.default.createElement("div", {
                     className: e,
                     onClick: this.onClick
                 }, this.renderNativeInput(), this.renderCustomInputs())
             }
         }]) && P(t.prototype, n), r && P(t, r), O
     }(a.PureComponent);
-    t.default = Q, Q.defaultProps = {
+    t.default = G, G.defaultProps = {
         maxDetail: "minute",
         name: "datetime"
     };
-    var G = o.default.oneOfType([o.default.string, o.default.instanceOf(Date)]);
-    Q.propTypes = {
+    var Q = o.default.oneOfType([o.default.string, o.default.instanceOf(Date)]);
+    G.propTypes = {
         amPmAriaLabel: o.default.string,
         autoFocus: o.default.bool,
         className: o.default.string.isRequired,
         dayAriaLabel: o.default.string,
         dayPlaceholder: o.default.string,
         disabled: o.default.bool,
         format: o.default.string,
@@ -12851,15 +12851,15 @@
         name: o.default.string,
         nativeInputAriaLabel: o.default.string,
         onChange: o.default.func,
         required: o.default.bool,
         secondAriaLabel: o.default.string,
         secondPlaceholder: o.default.string,
         showLeadingZeros: o.default.bool,
-        value: o.default.oneOfType([G, o.default.arrayOf(G)]),
+        value: o.default.oneOfType([Q, o.default.arrayOf(Q)]),
         yearAriaLabel: o.default.string,
         yearPlaceholder: o.default.string
     }
 }, function(e, t, n) {
     "use strict";
     Object.defineProperty(t, "__esModule", {
         value: !0
@@ -13091,47 +13091,47 @@
         var t = e.ariaLabel,
             n = e.className,
             a = e.inputRef,
             c = e.locale,
             f = e.maxDate,
             h = e.minDate,
             b = e.placeholder,
-            v = void 0 === b ? "--" : b,
-            y = e.short,
+            y = void 0 === b ? "--" : b,
+            v = e.short,
             g = e.value,
             O = e.year,
             _ = m(e, s);
 
         function w(e) {
             return e && O === (0, i.getYear)(e).toString()
         }
         var E = (0, u.safeMin)(12, w(f) && (0, i.getMonthHuman)(f)),
             j = (0, u.safeMax)(1, w(h) && (0, i.getMonthHuman)(h)),
-            M = d(Array(12)).map((function(e, t) {
+            k = d(Array(12)).map((function(e, t) {
                 return new Date(2019, t, 1)
             })),
-            k = y ? l.formatShortMonth : l.formatMonth;
+            M = v ? l.formatShortMonth : l.formatMonth;
         return r.default.createElement("select", p({
             "aria-label": t,
             className: (0, o.default)("".concat(n, "__input"), "".concat(n, "__").concat("month")),
             "data-input": "true",
             "data-select": "true",
             name: "month",
             ref: a,
             value: null !== g ? g : ""
         }, _), !g && r.default.createElement("option", {
             value: ""
-        }, v), M.map((function(e) {
+        }, y), k.map((function(e) {
             var t = (0, i.getMonthHuman)(e),
                 n = t < j || t > E;
             return r.default.createElement("option", {
                 key: t,
                 disabled: n,
                 value: t
-            }, k(c, e))
+            }, M(c, e))
         })))
     }
     b.propTypes = {
         ariaLabel: a.default.string,
         className: a.default.string.isRequired,
         disabled: a.default.bool,
         inputRef: c.isRef,
@@ -13341,26 +13341,26 @@
         return a
     }
 
     function b(e) {
         var t, n, a, c, f = e.amPm,
             h = (e.hour, e.maxTime),
             b = e.minTime,
-            v = e.value,
-            y = m(e, s),
+            y = e.value,
+            v = m(e, s),
             g = (0, u.safeMin)(12, h && (t = d((0, l.convert24to12)((0, o.getHours)(h)), 2), n = t[0], t[1] !== f ? null : n)),
             O = (0, u.safeMax)(1, b && (a = d((0, l.convert24to12)((0, o.getHours)(b)), 2), c = a[0], a[1] !== f || 12 === c ? null : c)),
-            _ = v ? (0, l.convert24to12)(v)[0].toString() : "";
+            _ = y ? (0, l.convert24to12)(y)[0].toString() : "";
         return r.default.createElement(i.default, p({
             max: g,
             min: O,
             name: "hour12",
             nameForClass: "hour",
             value: _
-        }, y))
+        }, v))
     }
     b.propTypes = {
         amPm: a.default.string,
         ariaLabel: a.default.string,
         className: a.default.string.isRequired,
         disabled: a.default.bool,
         hour: a.default.string,
@@ -13597,18 +13597,18 @@
             d = void 0 === s || s,
             h = p(e, u);
 
         function m(e) {
             return e && t === (0, o.getHours)(e).toString() && l === (0, o.getMinutes)(e).toString()
         }
         var b = (0, c.safeMin)(59, m(n) && (0, o.getSeconds)(n)),
-            v = (0, c.safeMax)(0, m(a) && (0, o.getSeconds)(a));
+            y = (0, c.safeMax)(0, m(a) && (0, o.getSeconds)(a));
         return r.default.createElement(i.default, f({
             max: b,
-            min: v,
+            min: y,
             name: "second",
             showLeadingZeros: d
         }, h))
     }
     d.propTypes = {
         ariaLabel: a.default.string,
         className: a.default.string.isRequired,
@@ -13691,16 +13691,16 @@
             c = e.inputRef,
             s = e.locale,
             p = e.maxTime,
             d = e.minTime,
             h = e.onChange,
             m = e.required,
             b = e.value,
-            v = d && "pm" === (0, l.convert24to12)((0, i.getHours)(d))[1],
-            y = p && "am" === (0, l.convert24to12)((0, i.getHours)(p))[1],
+            y = d && "pm" === (0, l.convert24to12)((0, i.getHours)(d))[1],
+            v = p && "am" === (0, l.convert24to12)((0, i.getHours)(p))[1],
             g = f((0, u.getAmPmLabels)(s), 2),
             O = g[0],
             _ = g[1];
         return r.default.createElement("select", {
             "aria-label": t,
             className: (0, o.default)("".concat(n, "__input"), "".concat(n, "__").concat("amPm")),
             "data-input": "true",
@@ -13710,18 +13710,18 @@
             onChange: h,
             ref: c,
             required: m,
             value: null !== b ? b : ""
         }, !b && r.default.createElement("option", {
             value: ""
         }, "--"), r.default.createElement("option", {
-            disabled: v,
+            disabled: y,
             value: "am"
         }, O), r.default.createElement("option", {
-            disabled: y,
+            disabled: v,
             value: "pm"
         }, _))
     }
     d.propTypes = {
         ariaLabel: a.default.string,
         className: a.default.string.isRequired,
         disabled: a.default.bool,
@@ -14097,15 +14097,15 @@
     var r = n(0),
         a = n.n(r),
         o = n(6),
         i = n.n(o),
         l = n(68),
         c = n(11),
         u = n(20),
-        s = n(26),
+        s = n(27),
         f = n(64);
     var p = function(...e) {
             return e.filter(e => null != e).reduce((e, t) => {
                 if ("function" != typeof t) throw new Error("Invalid Argument Type, must only provide functions, undefined, or null.");
                 return null === e ? t : function(...n) {
                     e.apply(this, n), t.apply(this, n)
                 }
@@ -14115,76 +14115,76 @@
         h = n(70),
         m = n(2);
     const b = {
         height: ["marginTop", "marginBottom"],
         width: ["marginLeft", "marginRight"]
     };
 
-    function v(e, t) {
+    function y(e, t) {
         const n = t[`offset${e[0].toUpperCase()}${e.slice(1)}`],
             r = b[e];
         return n + parseInt(Object(u.a)(t, r[0]), 10) + parseInt(Object(u.a)(t, r[1]), 10)
     }
-    const y = {
+    const v = {
             [s.c]: "collapse",
             [s.d]: "collapsing",
             [s.b]: "collapsing",
             [s.a]: "collapse show"
         },
         g = {
             in: !1,
             timeout: 300,
             mountOnEnter: !1,
             unmountOnExit: !1,
             appear: !1,
-            getDimensionValue: v
+            getDimensionValue: y
         },
         O = a.a.forwardRef(({
             onEnter: e,
             onEntering: t,
             onEntered: n,
             onExit: o,
             onExiting: l,
             className: c,
             children: u,
             dimension: s = "height",
-            getDimensionValue: b = v,
+            getDimensionValue: b = y,
             ...g
         }, O) => {
             const _ = "function" == typeof s ? s() : s,
                 w = Object(r.useMemo)(() => p(e => {
                     e.style[_] = "0"
                 }, e), [_, e]),
                 E = Object(r.useMemo)(() => p(e => {
                     const t = `scroll${_[0].toUpperCase()}${_.slice(1)}`;
                     e.style[_] = e[t] + "px"
                 }, t), [_, t]),
                 j = Object(r.useMemo)(() => p(e => {
                     e.style[_] = null
                 }, n), [_, n]),
-                M = Object(r.useMemo)(() => p(e => {
+                k = Object(r.useMemo)(() => p(e => {
                     e.style[_] = b(_, e) + "px", Object(d.a)(e)
                 }, o), [o, b, _]),
-                k = Object(r.useMemo)(() => p(e => {
+                M = Object(r.useMemo)(() => p(e => {
                     e.style[_] = null
                 }, l), [_, l]);
             return Object(m.jsx)(h.a, {
                 ref: O,
                 addEndListener: f.a,
                 ...g,
                 "aria-expanded": g.role ? g.in : null,
                 onEnter: w,
                 onEntering: E,
                 onEntered: j,
-                onExit: M,
-                onExiting: k,
+                onExit: k,
+                onExiting: M,
                 childRef: u.ref,
                 children: (e, t) => a.a.cloneElement(u, {
                     ...t,
-                    className: i()(c, u.props.className, y[e], "width" === _ && "collapse-horizontal")
+                    className: i()(c, u.props.className, v[e], "width" === _ && "collapse-horizontal")
                 })
             })
         });
     O.defaultProps = g;
     var _ = O;
     const w = r.createContext({});
     w.displayName = "AccordionContext";
@@ -14207,31 +14207,31 @@
             className: i()(n, t),
             children: Object(m.jsx)(e, {
                 children: r.Children.only(a)
             })
         })
     });
     j.displayName = "AccordionCollapse";
-    var M = j;
-    const k = r.createContext({
+    var k = j;
+    const M = r.createContext({
         eventKey: ""
     });
-    k.displayName = "AccordionItemContext";
-    var P = k;
+    M.displayName = "AccordionItemContext";
+    var P = M;
     const x = r.forwardRef(({
         as: e = "div",
         bsPrefix: t,
         className: n,
         ...a
     }, o) => {
         t = Object(c.a)(t, "accordion-body");
         const {
             eventKey: l
         } = Object(r.useContext)(P);
-        return Object(m.jsx)(M, {
+        return Object(m.jsx)(k, {
             eventKey: l,
             children: Object(m.jsx)(e, {
                 ref: o,
                 ...a,
                 className: i()(n, t)
             })
         })
@@ -14332,15 +14332,15 @@
                 className: i()(u, d, f && d + "-flush")
             })
         })
     });
     I.displayName = "Accordion";
     var H = Object.assign(I, {
             Button: C,
-            Collapse: M,
+            Collapse: k,
             Item: N,
             Header: D,
             Body: S
         }),
         L = n(12),
         B = n(14);
     const q = r.forwardRef(({
@@ -14365,16 +14365,16 @@
     };
     var F = q,
         W = n(1),
         V = n.n(W),
         U = n(4),
         K = n(24),
         Y = n(19),
-        Q = n(5),
-        G = n(13),
+        G = n(5),
+        Q = n(13),
         J = n(10),
         Z = n(85),
         X = n.n(Z);
 
     function $(e) {
         return ($ = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
@@ -14651,17 +14651,17 @@
                     s = t.categoryOptionsLarge,
                     f = t.manualCategories,
                     p = t.selectedDateTime,
                     d = t.filterType,
                     h = t.filterNumber,
                     m = t.filterIndex,
                     b = t.config,
-                    v = this.props,
-                    y = v.meta,
-                    g = v.id;
+                    y = this.props,
+                    v = y.meta,
+                    g = y.id;
                 return a.a.createElement(L.a, {
                     centered: !0,
                     backdrop: "static",
                     animation: !1,
                     show: o,
                     onHide: function() {
                         return e.handleClose()
@@ -14678,33 +14678,33 @@
                     key: g + "-selectOptions",
                     options: n,
                     value: r.filter((function(e) {
                         return e.value === i
                     }))[0],
                     onChange: function(t) {
                         var n = t.value,
-                            r = y[n].type;
+                            r = v[n].type;
                         "categorical" == r && e.setState({
-                            categoryOptions: y[n].cat.map((function(e) {
+                            categoryOptions: v[n].cat.map((function(e) {
                                 return {
                                     label: String(e),
                                     value: e
                                 }
                             })),
-                            categoryOptionsLarge: "large" in y[n] && y[n].large
+                            categoryOptionsLarge: "large" in v[n] && v[n].large
                         }), e.setState({
                             selectedColumn: n,
                             selectedType: r
                         })
                     },
                     styles: U.e,
                     components: U.b
-                }), "numerical" == l && a.a.createElement("div", null, "Select the numerical filtering you want to apply:", a.a.createElement(Q.a, {
+                }), "numerical" == l && a.a.createElement("div", null, "Select the numerical filtering you want to apply:", a.a.createElement(G.a, {
                     className: "mb-3"
-                }, a.a.createElement(Q.a.Text, {
+                }, a.a.createElement(G.a.Text, {
                     id: "basic-addon1"
                 }, "Type"), a.a.createElement(Y.a.Select, {
                     key: g + "-selectType",
                     value: d,
                     onChange: function(t) {
                         e.setState({
                             filterType: t.target.value
@@ -14720,30 +14720,30 @@
                     value: "lt"
                 }, "<"), a.a.createElement("option", {
                     value: "lte"
                 }, "≤"), a.a.createElement("option", {
                     value: "eq"
                 }, "="), a.a.createElement("option", {
                     value: "neq"
-                }, "≠"))), a.a.createElement(Q.a, {
+                }, "≠"))), a.a.createElement(G.a, {
                     className: "mb-3"
-                }, a.a.createElement(Q.a.Text, {
+                }, a.a.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "Value"), a.a.createElement(G.a, {
+                }, "Value"), a.a.createElement(Q.a, {
                     type: "number",
                     key: g + "-inputValue",
                     value: h,
                     onChange: function(t) {
                         e.setState({
                             filterNumber: t.target.value
                         })
                     }
-                }))), "categorical" == l && a.a.createElement("div", null, "Select which categories you want to filter:", a.a.createElement(Q.a, {
+                }))), "categorical" == l && a.a.createElement("div", null, "Select which categories you want to filter:", a.a.createElement(G.a, {
                     className: "mb-3"
-                }, a.a.createElement(Q.a.Text, {
+                }, a.a.createElement(G.a.Text, {
                     id: "basic-addon1"
                 }, "Type"), a.a.createElement(Y.a.Select, {
                     key: g + "-selectCatOption",
                     value: d,
                     onChange: function(t) {
                         e.setState({
                             filterType: t.target.value
@@ -14772,30 +14772,30 @@
                     onChange: function(t) {
                         t ? e.setState({
                             selectedCategories: t.value
                         }) : e.setState({
                             selectedCategories: void 0
                         })
                     }
-                }), ["isnotin", "isin", "eq"].includes(d) && s && a.a.createElement("div", null, a.a.createElement(G.a, {
+                }), ["isnotin", "isin", "eq"].includes(d) && s && a.a.createElement("div", null, a.a.createElement(Q.a, {
                     as: "textarea",
                     rows: 3,
                     value: f,
                     onChange: function(t) {
                         var n = t.target.value.split(/\r?\n/).map((function(e) {
                             return e.trimLeft().trimRight()
                         }));
                         "eq" === d && (n = t.target.value), e.setState({
                             manualCategories: t.target.value,
                             selectedCategories: n
                         })
                     }
-                }))), "temporal" == l && a.a.createElement("div", null, a.a.createElement(Q.a, {
+                }))), "temporal" == l && a.a.createElement("div", null, a.a.createElement(G.a, {
                     className: "mb-3"
-                }, a.a.createElement(Q.a.Text, {
+                }, a.a.createElement(G.a.Text, {
                     id: "basic-addon1"
                 }, "Type"), a.a.createElement(Y.a.Select, {
                     value: d,
                     key: g + "-selectTimeOptions",
                     onChange: function(t) {
                         e.setState({
                             filterType: t.target.value
@@ -14814,30 +14814,30 @@
                     value: p,
                     key: g + "-selectTime",
                     onChange: function(t) {
                         e.setState({
                             selectedDateTime: t
                         })
                     }
-                }), "lastn" === d && a.a.createElement(Q.a, {
+                }), "lastn" === d && a.a.createElement(G.a, {
                     className: "mb-3"
-                }, a.a.createElement(Q.a.Text, {
+                }, a.a.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "Value"), a.a.createElement(G.a, {
+                }, "Value"), a.a.createElement(Q.a, {
                     type: "number",
                     key: g + "-inputDeltaTime",
                     value: h,
                     onChange: function(t) {
                         e.setState({
                             filterNumber: t.target.value
                         })
                     }
-                }))), "bool" == l && a.a.createElement("div", null, "Select which flag you want to keep:", a.a.createElement(Q.a, {
+                }))), "bool" == l && a.a.createElement("div", null, "Select which flag you want to keep:", a.a.createElement(G.a, {
                     className: "mb-3"
-                }, a.a.createElement(Q.a.Text, {
+                }, a.a.createElement(G.a.Text, {
                     id: "basic-addon1"
                 }, "Type"), a.a.createElement(Y.a.Select, {
                     value: d,
                     key: g + "-selectBool",
                     onChange: function(t) {
                         e.setState({
                             filterType: t.target.value
@@ -14927,31 +14927,31 @@
         return (be = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function ve(e, t) {
+    function ye(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function ye(e) {
+    function ve(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? ve(Object(n), !0).forEach((function(t) {
+            t % 2 ? ye(Object(n), !0).forEach((function(t) {
                 ge(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ve(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ye(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function ge(e, t, n) {
@@ -15007,15 +15007,15 @@
     }
 
     function je(e) {
         return (je = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
-    var Me = function(e) {
+    var ke = function(e) {
         ! function(e, t) {
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             Object.defineProperty(e, "prototype", {
                 value: Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
@@ -15047,15 +15047,15 @@
             }
         }, {
             key: "eval",
             value: function(e) {
                 return {
                     error: !1,
                     message: "",
-                    new_meta: ye({}, e.meta)
+                    new_meta: ve({}, e.meta)
                 }
             }
         }, {
             key: "get_dummy_meta_entry",
             value: function(e, t) {
                 return "numerical" === e ? {
                     max: t,
@@ -15096,15 +15096,15 @@
                     catColOptions: e.catColOptions
                 })
             }
         }, {
             key: "setStateConfig",
             value: function(e) {
                 var t = this.config_from_state(e);
-                this.setState(ye(ye({}, e), {}, {
+                this.setState(ve(ve({}, e), {}, {
                     config: t
                 })), this.props.setProps({
                     config: t
                 })
             }
         }, {
             key: "config_from_state",
@@ -15119,16 +15119,16 @@
                 return !1
             }
         }]) && Oe(t.prototype, n), r && Oe(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
     }(r.Component);
 
-    function ke(e) {
-        return (ke = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Me(e) {
+        return (Me = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function Pe() {
@@ -15195,15 +15195,15 @@
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return ze(this, n)
         }
     }
 
     function ze(e, t) {
-        if (t && ("object" === ke(t) || "function" == typeof t)) return t;
+        if (t && ("object" === Me(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
@@ -15217,15 +15217,15 @@
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    Me.defaultProps = {}, Me.propTypes = (ge(he = {
+    ke.defaultProps = {}, ke.propTypes = (ge(he = {
         config: PropTypes.any,
         meta: PropTypes.any.isRequired,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired
     }, "allColOptions", PropTypes.any.isRequired), ge(he, "setProps", PropTypes.func), he);
     var Ne = function(e) {
@@ -15335,15 +15335,15 @@
                 }, Object(U.c)(this, (function(t) {
                     return e.update_state(t)
                 }), "types", o.aggr_types))))
             }
         }]) && Ae(t.prototype, n), r && Ae(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
     Te(Ne, "aggr_types", [{
         value: "min",
         label: "min"
     }, {
         value: "max",
         label: "max"
     }, {
@@ -15587,15 +15587,15 @@
                 var f = {
                         value: a,
                         error: i,
                         message: l,
                         type: c
                     },
                     p = Be({}, t);
-                return p[r] = Me.get_dummy_meta_entry(c, a), f.new_meta = p, f
+                return p[r] = ke.get_dummy_meta_entry(c, a), f.new_meta = p, f
             }
         }], (n = [{
             key: "config_from_state",
             value: function(e) {
                 return {
                     type: "eval",
                     col: e.newColName,
@@ -15609,31 +15609,31 @@
                     t = this.state,
                     n = t.newColName,
                     r = t.newColFormula,
                     a = t.newColComputeResult,
                     i = t.meta;
                 return React.createElement("div", null, React.createElement("div", {
                     className: "color-helper-blue"
-                }, "Create a new column computed by row data."), React.createElement(Q.a, {
+                }, "Create a new column computed by row data."), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "New column"), React.createElement(G.a, {
+                }, "New column"), React.createElement(Q.a, {
                     value: n,
                     onChange: function(t) {
                         e.setStateConfig({
                             newColName: t.target.value,
                             newColFormula: r
                         })
                     }
-                })), React.createElement(Q.a, {
+                })), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "Formula"), React.createElement(G.a, {
+                }, "Formula"), React.createElement(Q.a, {
                     as: "textarea",
                     rows: 3,
                     value: r,
                     onChange: function(t) {
                         var r = {
                             type: "eval",
                             col: n,
@@ -15651,26 +15651,26 @@
                 })), a && "error" in a && a.error && React.createElement(K.a, null, a.message), a && "error" in a && !a.error && React.createElement(K.a, {
                     variant: "success"
                 }, "New col: ", n, " (", a.type, ") e.q. ", a.value))
             }
         }]) && Fe(t.prototype, n), r && Fe(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
-    function Qe(e) {
-        return (Qe = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Ge(e) {
+        return (Ge = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function Ge() {
-        return (Ge = Object.assign || function(e) {
+    function Qe() {
+        return (Qe = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
@@ -15738,15 +15738,15 @@
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return nt(this, n)
         }
     }
 
     function nt(e, t) {
-        if (t && ("object" === Qe(t) || "function" == typeof t)) return t;
+        if (t && ("object" === Ge(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
@@ -15810,24 +15810,24 @@
                 if (a.forEach((function(e) {
                         e in t || (o = !0, i = "Missing column " + e + "\n")
                     })), o) return {
                     error: o,
                     message: i
                 };
                 var l = a.map((function(e) {
-                        return Me.get_col_or_median(t[e])
+                        return ke.get_col_or_median(t[e])
                     })).join("_"),
                     c = {
                         value: l,
                         error: !1,
                         message: "",
                         type: "categorical"
                     },
                     u = Ze({}, t),
-                    s = Me.get_dummy_meta_entry("categorical", l);
+                    s = ke.get_dummy_meta_entry("categorical", l);
                 s.cat = a;
                 var f = u[a[0]];
                 return a.forEach((function(e) {
                     delete u[e]
                 })), u[r] = s, u[n] = f, c.new_meta = u, c
             }
         }], (n = [{
@@ -15846,58 +15846,58 @@
                 var e = this,
                     t = this.state,
                     n = t.newColName,
                     r = t.newColNameTwo,
                     a = t.selectedCols,
                     o = t.allColOptions,
                     i = t.allOptions;
-                return React.createElement("div", null, React.createElement("div", null, "Choose the names of the new columns."), React.createElement(Q.a, {
+                return React.createElement("div", null, React.createElement("div", null, "Choose the names of the new columns."), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     className: "color-helper-blue",
                     id: "basic-addon1"
-                }, "Value"), React.createElement(G.a, {
+                }, "Value"), React.createElement(Q.a, {
                     value: n,
                     onChange: function(t) {
                         e.setStateConfig({
                             newColName: t.target.value,
                             newColNameTwo: r,
                             selectedCols: a
                         })
                     }
-                }), React.createElement(Q.a.Text, {
+                }), React.createElement(G.a.Text, {
                     className: "color-helper-red",
                     id: "basic-addon2"
-                }, "Type"), React.createElement(G.a, {
+                }, "Type"), React.createElement(Q.a, {
                     value: r,
                     onChange: function(t) {
                         e.setStateConfig({
                             newColName: n,
                             newColNameTwo: t.target.value,
                             selectedCols: a
                         })
                     }
                 })), React.createElement("div", {
                     className: "color-helper-green"
-                }, "Select the columns that should be combined:"), React.createElement(J.a, Ge({
+                }, "Select the columns that should be combined:"), React.createElement(J.a, Qe({
                     className: "mb-3",
                     options: o,
                     styles: U.d,
                     components: U.b
                 }, Object(U.c)(this, (function(t) {
                     return e.setStateConfig(Ze(Ze({}, t), {}, {
                         newColName: n,
                         newColNameTwo: r
                     }))
                 }), "selectedCols", i))))
             }
         }]) && $e(t.prototype, n), r && $e(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function ot(e) {
         return (ot = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -16044,24 +16044,24 @@
                 if (r.forEach((function(e) {
                         e in t || (a = !0)
                     })), a) return {
                     error: !0,
                     message: "Missing input columns"
                 };
                 var o = r.map((function(e) {
-                        return Me.get_col_or_median(t[e])
+                        return ke.get_col_or_median(t[e])
                     })).join("_"),
                     i = {
                         value: o,
                         error: !1,
                         message: "",
                         type: "categorical"
                     },
                     l = ct({}, t);
-                return l[n] = Me.get_dummy_meta_entry("categorical", o), i.new_meta = l, i
+                return l[n] = ke.get_dummy_meta_entry("categorical", o), i.new_meta = l, i
             }
         }], (n = [{
             key: "config_from_state",
             value: function(e) {
                 return {
                     type: "combinecat",
                     col: e.newColName,
@@ -16075,20 +16075,20 @@
                     t = this.state,
                     n = t.newColName,
                     r = t.selectedCols,
                     a = t.allColOptions,
                     o = t.allOptions;
                 return React.createElement("div", null, React.createElement("div", {
                     className: "color-helper-blue"
-                }, "Choose the name of a new category."), React.createElement(Q.a, {
+                }, "Choose the name of a new category."), React.createElement(G.a, {
                     className: "mb-3",
                     key: "selectName"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "New column"), React.createElement(G.a, {
+                }, "New column"), React.createElement(Q.a, {
                     value: n,
                     onChange: function(t) {
                         e.setStateConfig({
                             newColName: t.target.value,
                             selectedCols: r
                         })
                     }
@@ -16105,28 +16105,28 @@
                         newColName: n
                     }))
                 }), "selectedCols", o))))
             }
         }]) && st(t.prototype, n), r && st(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
     mt.defaultProps = {}, mt.propTypes = {
         config: PropTypes.any,
         meta: PropTypes.any.isRequired,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired,
         setProps: PropTypes.func
     };
     var bt = n(28),
-        vt = n.n(bt);
+        yt = n.n(bt);
 
-    function yt(e) {
-        return (yt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function vt(e) {
+        return (vt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function gt(e, t) {
@@ -16182,34 +16182,34 @@
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }();
         return function() {
-            var n, r = kt(e);
+            var n, r = Mt(e);
             if (t) {
-                var a = kt(this).constructor;
+                var a = Mt(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
-            return Mt(this, n)
+            return kt(this, n)
         }
     }
 
-    function Mt(e, t) {
-        if (t && ("object" === yt(t) || "function" == typeof t)) return t;
+    function kt(e, t) {
+        if (t && ("object" === vt(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
-    function kt(e) {
-        return (kt = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+    function Mt(e) {
+        return (Mt = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
     var Pt = function(e) {
         ! function(e, t) {
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             Object.defineProperty(e, "prototype", {
@@ -16267,23 +16267,23 @@
                 };
                 var o = a[Object.keys(a)[0]],
                     i = {
                         number: "numerical",
                         boolean: "bool",
                         string: "categorical",
                         undefined: "?"
-                    } [String(yt(o))],
+                    } [String(vt(o))],
                     l = {
                         value: o,
                         error: !1,
                         message: "",
                         type: i
                     },
                     c = Ot({}, t);
-                return c[n] = Me.get_dummy_meta_entry(i, o), l.new_meta = c, l
+                return c[n] = ke.get_dummy_meta_entry(i, o), l.new_meta = c, l
             }
         }], (n = [{
             key: "config_from_state",
             value: function(e) {
                 var t = null;
                 try {
                     t = e.values.map((function(e) {
@@ -16309,20 +16309,20 @@
                     a = t.meta,
                     o = this.state,
                     i = o.newColName,
                     l = o.selectedCol,
                     c = o.values;
                 return React.createElement("div", null, React.createElement("div", {
                     className: "color-helper-blue"
-                }, "Set the name of the new column with the lookup results."), React.createElement(Q.a, {
+                }, "Set the name of the new column with the lookup results."), React.createElement(G.a, {
                     className: "mb-3",
                     key: "selectName"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "New column"), React.createElement(G.a, {
+                }, "New column"), React.createElement(Q.a, {
                     value: i,
                     onChange: function(t) {
                         e.setStateConfig({
                             newColName: t.target.value,
                             selectedCol: l,
                             values: c
                         })
@@ -16346,15 +16346,15 @@
                         })), e.editablelist_ref.current.setState({
                             list: n.values
                         })), e.setStateConfig(n)
                     },
                     isClearable: !0,
                     styles: U.e,
                     components: U.b
-                }), "Define the new value for each category:", React.createElement(vt.a, {
+                }), "Define the new value for each category:", React.createElement(yt.a, {
                     ref: this.editablelist_ref,
                     list: c,
                     className: "w-100",
                     onListChange: function(t) {
                         return e.setStateConfig({
                             values: t,
                             newColName: i,
@@ -16363,15 +16363,15 @@
                     },
                     placeholder: "Enter a value"
                 }))
             }
         }]) && wt(t.prototype, n), r && wt(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function xt(e) {
         return (xt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -16548,15 +16548,15 @@
                 }, Object(U.c)(this, (function(t) {
                     return e.setStateConfig(Ct({}, t))
                 }), "selectedCols", r))))
             }
         }]) && zt(t.prototype, n), r && zt(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function Lt(e) {
         return (Lt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -16636,15 +16636,15 @@
 
     function Yt(e, t) {
         return (Yt = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function Qt(e) {
+    function Gt(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -16653,19 +16653,19 @@
         }();
         return function() {
             var n, r = Jt(e);
             if (t) {
                 var a = Jt(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
-            return Gt(this, n)
+            return Qt(this, n)
         }
     }
 
-    function Gt(e, t) {
+    function Qt(e, t) {
         if (t && ("object" === Lt(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
@@ -16693,15 +16693,15 @@
                         writable: !0,
                         configurable: !0
                     }
                 }),
                 writable: !1
             }), t && Yt(e, t)
         }(o, e);
-        var t, n, r, a = Qt(o);
+        var t, n, r, a = Gt(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
             }(this, o), (t = a.call(this, e)).state = Vt(Vt({}, t.state), {}, {
                 groupby: [],
@@ -16833,35 +16833,35 @@
                     u = c.filter((function(e) {
                         return "value" in e
                     }));
                 return c.forEach((function(e) {
                     "options" in e && (u = [].concat(qt(u), qt(e.options)))
                 })), React.createElement("div", null, React.createElement("div", {
                     className: "color-helper-blue"
-                }, "Extract a variable type from the input colum names:"), React.createElement(Q.a, {
+                }, "Extract a variable type from the input colum names:"), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "Type"), React.createElement(G.a, {
+                }, "Type"), React.createElement(Q.a, {
                     value: a,
                     onChange: function(t) {
                         e.update_state({
                             type: t.target.value
                         })
                     }
-                }), React.createElement(Q.a.Text, {
+                }), React.createElement(G.a.Text, {
                     id: "basic-addon2"
-                }, "sep"), React.createElement(G.a, {
+                }, "sep"), React.createElement(Q.a, {
                     value: i,
                     onChange: function(t) {
                         e.update_state({
                             sep: t.target.value
                         })
                     }
-                }), React.createElement(Q.a.Text, {
+                }), React.createElement(G.a.Text, {
                     id: "basic-addon2"
                 }, "Suffix"), React.createElement(Y.a.Select, {
                     value: l,
                     onChange: function(t) {
                         e.update_state({
                             suffix: t.target.value
                         })
@@ -16890,15 +16890,15 @@
                 }, Object(U.c)(this, (function(t) {
                     return e.update_state(t)
                 }), "groupby", r))))
             }
         }]) && Kt(t.prototype, n), r && Kt(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function Xt(e) {
         return (Xt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -17075,15 +17075,15 @@
                 }, Object(U.c)(this, (function(t) {
                     return e.setStateConfig(tn({}, t))
                 }), "selectedCols", r))))
             }
         }]) && rn(t.prototype, n), r && rn(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function sn(e) {
         return (sn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -17166,23 +17166,23 @@
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function vn(e, t) {
+    function yn(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
-    function yn(e, t) {
-        return (yn = Object.setPrototypeOf || function(e, t) {
+    function vn(e, t) {
+        return (vn = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
     function gn(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
@@ -17234,15 +17234,15 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }),
                 writable: !1
-            }), t && yn(e, t)
+            }), t && vn(e, t)
         }(o, e);
         var t, n, r, a = gn(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
@@ -17329,79 +17329,79 @@
                     t.values = t.selectedCols.map((function(e) {
                         return '"' + e + '": "' + e + '"'
                     })), e.editablelist_ref.current.setState({
                         list: t.values
                     }), e.setStateConfig(t)
                 }), "selectedCols", r))), React.createElement("div", {
                     className: "color-helper-blue"
-                }, "Define the new column names:"), React.createElement(vt.a, {
+                }, "Define the new column names:"), React.createElement(yt.a, {
                     ref: this.editablelist_ref,
                     list: o,
                     className: "w-100",
                     onListChange: function(t) {
                         return e.setStateConfig({
                             values: t
                         })
                     },
                     placeholder: "Enter a value"
                 }))
             }
-        }]) && vn(t.prototype, n), r && vn(t, r), Object.defineProperty(t, "prototype", {
+        }]) && yn(t.prototype, n), r && yn(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function En(e) {
         return (En = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function jn(e) {
         return function(e) {
-            if (Array.isArray(e)) return Mn(e)
+            if (Array.isArray(e)) return kn(e)
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }(e) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return Mn(e, t);
+            if ("string" == typeof e) return kn(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Mn(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return kn(e, t)
         }(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function Mn(e, t) {
+    function kn(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function kn(e, t) {
+    function Mn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
     function Pn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? kn(Object(n), !0).forEach((function(t) {
+            t % 2 ? Mn(Object(n), !0).forEach((function(t) {
                 xn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : kn(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Mn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function xn(e, t, n) {
@@ -17567,20 +17567,20 @@
                     r = t.selectedCol,
                     a = t.catColOptions,
                     o = t.sep,
                     i = t.start,
                     l = t.end;
                 return React.createElement("div", null, React.createElement("div", {
                     className: "color-helper-blue"
-                }, "Choose the name of a new column."), React.createElement(Q.a, {
+                }, "Choose the name of a new column."), React.createElement(G.a, {
                     className: "mb-3",
                     key: "selectName"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "New column"), React.createElement(G.a, {
+                }, "New column"), React.createElement(Q.a, {
                     value: n,
                     onChange: function(t) {
                         e.setStateConfig({
                             newColName: t.target.value,
                             selectedCol: r,
                             sep: o,
                             end: l,
@@ -17609,19 +17609,19 @@
                             selectedCol: void 0,
                             newColName: n,
                             sep: o,
                             end: l,
                             start: i
                         })
                     }
-                }), React.createElement("div", null, "Extract a substring via:"), React.createElement(Q.a, {
+                }), React.createElement("div", null, "Extract a substring via:"), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "Separator"), React.createElement(G.a, {
+                }, "Separator"), React.createElement(Q.a, {
                     value: o,
                     onChange: function(t) {
                         "" === t.target.value ? e.setStateConfig({
                             sep: "",
                             end: i + 1,
                             newColName: n,
                             selectedCol: r,
@@ -17630,17 +17630,17 @@
                             sep: t.target.value,
                             end: "",
                             newColName: n,
                             selectedCol: r,
                             start: i
                         })
                     }
-                }), React.createElement(Q.a.Text, {
+                }), React.createElement(G.a.Text, {
                     id: "basic-addon2"
-                }, "Start"), React.createElement(G.a, {
+                }, "Start"), React.createElement(Q.a, {
                     value: i,
                     onChange: function(t) {
                         var a = parseInt(t.target.value);
                         isNaN(a) ? e.setStateConfig({
                             start: "",
                             newColName: n,
                             selectedCol: r,
@@ -17650,17 +17650,17 @@
                             start: a,
                             newColName: n,
                             selectedCol: r,
                             end: l,
                             sep: o
                         })
                     }
-                }), React.createElement(Q.a.Text, {
+                }), React.createElement(G.a.Text, {
                     id: "basic-addon2"
-                }, "End"), React.createElement(G.a, {
+                }, "End"), React.createElement(Q.a, {
                     value: l,
                     onChange: function(t) {
                         var a = parseInt(t.target.value);
                         isNaN(a) ? e.setStateConfig({
                             end: "",
                             newColName: n,
                             selectedCol: r,
@@ -17675,15 +17675,15 @@
                         })
                     }
                 })))
             }
         }]) && Sn(t.prototype, n), r && Sn(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function Tn(e) {
         return (Tn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -17894,19 +17894,19 @@
                     i = t.overlapping,
                     l = t.numColOptions,
                     c = t.allOptions,
                     u = t.parse_error,
                     s = a.length < 1;
                 return React.createElement("div", null, React.createElement("div", {
                     className: "color-helper-blue"
-                }, "Create a new or multiply colums by applying a binning scheme."), React.createElement(Q.a, {
+                }, "Create a new or multiply colums by applying a binning scheme."), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "New column"), React.createElement(G.a, {
+                }, "New column"), React.createElement(Q.a, {
                     value: n,
                     onChange: function(t) {
                         e.setStateConfig({
                             name: t.target.value,
                             cols: r,
                             binning: a,
                             overlapping: i
@@ -17921,20 +17921,20 @@
                     components: U.b
                 }, Object(U.c)(this, (function(t) {
                     return e.setStateConfig(Hn(Hn({}, t), {}, {
                         name: n,
                         binning: a,
                         overlapping: i
                     }))
-                }), "cols", c))), React.createElement(Q.a, {
+                }), "cols", c))), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     className: "color-helper-red",
                     id: "basic-addon1"
-                }, "Binning"), React.createElement(G.a, {
+                }, "Binning"), React.createElement(Q.a, {
                     as: "textarea",
                     rows: 3,
                     value: o,
                     onChange: function(t) {
                         var o = {
                             name: n,
                             cols: r,
@@ -17995,15 +17995,15 @@
                     ],
                     name: "C"
                 }]))))
             }
         }]) && Bn(t.prototype, n), r && Bn(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function Kn(e) {
         return (Kn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -18015,31 +18015,31 @@
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
 
-    function Qn(e, t) {
+    function Gn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Gn(e) {
+    function Qn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Qn(Object(n), !0).forEach((function(t) {
+            t % 2 ? Gn(Object(n), !0).forEach((function(t) {
                 Jn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Qn(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Gn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function Jn(e, t, n) {
@@ -18123,20 +18123,20 @@
         }(o, e);
         var t, n, r, a = $n(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-            }(this, o), (t = a.call(this, e)).state = Gn(Gn({}, t.state), {}, {
+            }(this, o), (t = a.call(this, e)).state = Qn(Qn({}, t.state), {}, {
                 selectedCols: [],
                 col: void 0,
                 upper: void 0,
                 lower: void 0
-            }), "config" in e && (t.state = Gn(Gn({}, t.state), {}, {
+            }), "config" in e && (t.state = Qn(Qn({}, t.state), {}, {
                 selectedCols: "groupby" in e.config ? e.config.groupby : [],
                 col: "col" in e.config ? e.config.col : void 0,
                 upper: "upper" in e.config ? e.config.upper : void 0,
                 lower: "lower" in e.config ? e.config.lower : void 0
             })), t
         }
         return t = o, r = [{
@@ -18188,15 +18188,15 @@
                 }, "Select the columns to group the data"), React.createElement(J.a, Yn({
                     className: "mb-3",
                     key: "selectCols",
                     options: a,
                     styles: U.d,
                     components: U.b
                 }, Object(U.c)(this, (function(t) {
-                    return e.setStateConfig(Gn(Gn({}, t), {}, {
+                    return e.setStateConfig(Qn(Qn({}, t), {}, {
                         col: r,
                         upper: l,
                         lower: c
                     }))
                 }), "selectedCols", i))), React.createElement("div", {
                     className: "color-helper-blue mt-2"
                 }, "Select the column to filter"), React.createElement(J.a, {
@@ -18213,33 +18213,33 @@
                         e.setStateConfig({
                             col: r,
                             selectedCols: n,
                             upper: l,
                             lower: c
                         })
                     }
-                }), React.createElement(Q.a, {
+                }), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-lower-addon"
-                }, "lower"), React.createElement(G.a, {
+                }, "lower"), React.createElement(Q.a, {
                     type: "number",
                     key: "lower-value",
                     value: c,
                     onChange: function(t) {
                         e.setStateConfig({
                             col: r,
                             selectedCols: n,
                             lower: t.target.value,
                             upper: l
                         })
                     }
-                }), React.createElement(Q.a.Text, {
+                }), React.createElement(G.a.Text, {
                     id: "basic-upper-addon"
-                }, "upper"), React.createElement(G.a, {
+                }, "upper"), React.createElement(Q.a, {
                     type: "number",
                     key: "upper-value",
                     value: l,
                     onChange: function(t) {
                         e.setStateConfig({
                             col: r,
                             selectedCols: n,
@@ -18248,15 +18248,15 @@
                         })
                     }
                 })))
             }
         }]) && Zn(t.prototype, n), r && Zn(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function rr(e) {
         return (rr = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -18459,15 +18459,15 @@
                         error: !1,
                         message: "",
                         type: "numerical"
                     }, o = cr({}, t), i = 0, l = Object.entries(r); i < l.length; i++) {
                     var c = ar(l[i], 2),
                         u = c[0],
                         s = c[1];
-                    o[u] = "int" === s || "float" === s ? Me.get_dummy_meta_entry("numerical", 123) : "bool" === s ? Me.get_dummy_meta_entry("bool", !0) : "str" === s ? Me.get_dummy_meta_entry("categorical", "???") : Me.get_dummy_meta_entry("?", "?")
+                    o[u] = "int" === s || "float" === s ? ke.get_dummy_meta_entry("numerical", 123) : "bool" === s ? ke.get_dummy_meta_entry("bool", !0) : "str" === s ? ke.get_dummy_meta_entry("categorical", "???") : ke.get_dummy_meta_entry("?", "?")
                 }
                 return a.new_meta = o, a
             }
         }], (n = [{
             key: "config_from_state",
             value: function(e) {
                 var t = null;
@@ -18511,15 +18511,15 @@
                             return e.split(":")[0]
                         }));
                     t.selectedCol.forEach((function(e) {
                         e in a || r.push('"' + e + '": "float"')
                     })), e.editablelist_ref.current.setState({
                         list: r
                     }), n.values = r, e.setStateConfig(n)
-                }), "selectedCol", r))), 'Set the new dataformats like "int", "float", "str", "bool":', React.createElement(vt.a, {
+                }), "selectedCol", r))), 'Set the new dataformats like "int", "float", "str", "bool":', React.createElement(yt.a, {
                     ref: this.editablelist_ref,
                     list: i,
                     className: "w-100",
                     onListChange: function(t) {
                         return e.setStateConfig({
                             values: t,
                             selectedCol: o
@@ -18527,51 +18527,51 @@
                     },
                     placeholder: "Enter a value"
                 }))
             }
         }]) && sr(t.prototype, n), r && sr(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function br(e) {
         return (br = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function vr() {
-        return (vr = Object.assign || function(e) {
+    function yr() {
+        return (yr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
 
-    function yr(e, t) {
+    function vr(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
     function gr(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? yr(Object(n), !0).forEach((function(t) {
+            t % 2 ? vr(Object(n), !0).forEach((function(t) {
                 Or(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : yr(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : vr(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function Or(e, t, n) {
@@ -18604,17 +18604,17 @@
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }();
         return function() {
-            var n, r = Mr(e);
+            var n, r = kr(e);
             if (t) {
-                var a = Mr(this).constructor;
+                var a = kr(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return jr(this, n)
         }
     }
 
     function jr(e, t) {
@@ -18622,28 +18622,28 @@
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
-    function Mr(e) {
-        return (Mr = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+    function kr(e) {
+        return (kr = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
     mr.defaultProps = {}, mr.propTypes = {
         config: PropTypes.any,
         meta: PropTypes.any.isRequired,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired,
         setProps: PropTypes.func
     };
-    var kr = function(e) {
+    var Mr = function(e) {
         ! function(e, t) {
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             Object.defineProperty(e, "prototype", {
                 value: Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
@@ -18704,29 +18704,29 @@
                     t = this.state,
                     n = t.selectedCols,
                     r = t.catColOptions,
                     a = t.allOptions,
                     o = t.n;
                 return React.createElement("div", null, React.createElement("div", {
                     className: "color-helper-blue mt-3"
-                }, "Select the columns to group the data"), React.createElement(J.a, vr({
+                }, "Select the columns to group the data"), React.createElement(J.a, yr({
                     className: "mb-3",
                     key: "selectCols",
                     options: r,
                     styles: U.d,
                     components: U.b
                 }, Object(U.c)(this, (function(t) {
                     return e.setStateConfig(gr(gr({}, t), {}, {
                         n: o
                     }))
-                }), "selectedCols", a))), React.createElement(Q.a, {
+                }), "selectedCols", a))), React.createElement(G.a, {
                     className: "mb-3"
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     id: "basic-n-addon"
-                }, "n"), React.createElement(G.a, {
+                }, "n"), React.createElement(Q.a, {
                     type: "number",
                     key: "n-value",
                     value: o,
                     onChange: function(t) {
                         e.setStateConfig({
                             selectedCols: n,
                             n: function(e) {
@@ -18739,26 +18739,26 @@
                         })
                     }
                 })))
             }
         }]) && _r(t.prototype, n), r && _r(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Me);
+    }(ke);
 
     function Pr() {
         return (Pr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
-    kr.defaultProps = {}, kr.propTypes = {
+    Mr.defaultProps = {}, Mr.propTypes = {
         config: PropTypes.any,
         meta: PropTypes.any.isRequired,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired,
         setProps: PropTypes.func
     };
@@ -20009,15 +20009,15 @@
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
-    var Qr = ({
+    var Gr = ({
         styles: e = {},
         ...t
     }) => a.a.createElement("svg", Yr({
         xmlns: "http://www.w3.org/2000/svg",
         width: "300",
         height: "100",
         viewBox: "0 0 79.375 26.458"
@@ -20165,27 +20165,27 @@
         fontFamily: "Myriad Pro",
         "aria-label": "C",
         fontSize: "4.123",
         fill: "#fff",
         strokeWidth: ".265"
     })));
 
-    function Gr() {
-        return (Gr = Object.assign || function(e) {
+    function Qr() {
+        return (Qr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
     var Jr = ({
         styles: e = {},
         ...t
-    }) => a.a.createElement("svg", Gr({
+    }) => a.a.createElement("svg", Qr({
         width: "300",
         height: "100",
         viewBox: "0 0 79.375 26.458",
         xmlns: "http://www.w3.org/2000/svg"
     }, t), a.a.createElement("path", {
         d: "M36.43 11.88h4.473L39.2 10.179h1.413l2.28 2.222-2.28 2.222h-1.413l1.702-1.703H36.43z",
         "aria-label": "➔",
@@ -21032,15 +21032,15 @@
         type: "filteriqr",
         class: nr,
         label: "Apply a grouped IQR filter",
         svg: a.a.createElement(Jr, null)
     }, {
         group: "missing",
         type: "groupby_sample",
-        class: kr,
+        class: Mr,
         label: "Apply a grouped sampling",
         svg: a.a.createElement(ea, null)
     }, {
         group: "meta",
         type: "rename",
         class: wn,
         label: "Rename multiple columns",
@@ -21052,15 +21052,15 @@
         label: "Recast multiple columns",
         svg: a.a.createElement(Xr, null)
     }, {
         group: "col",
         type: "bin",
         class: Un,
         label: "Compute a binned variable",
-        svg: a.a.createElement(Qr, null)
+        svg: a.a.createElement(Gr, null)
     }]), ha.defaultProps = {}, ha.propTypes = {
         id: V.a.string.isRequired,
         config: V.a.any,
         meta: V.a.any.isRequired,
         meta_out: V.a.any,
         setProps: V.a.func
     };
@@ -21070,23 +21070,23 @@
         return (ba = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function va(e, t) {
+    function ya(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
-    function ya(e, t) {
-        return (ya = Object.setPrototypeOf || function(e, t) {
+    function va(e, t) {
+        return (va = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
     function ga(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
@@ -21130,15 +21130,15 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }),
                 writable: !1
-            }), t && ya(e, t)
+            }), t && va(e, t)
         }(i, e);
         var t, n, r, o = ga(i);
 
         function i(e) {
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
             }(this, i), o.call(this, [], e)
@@ -21185,28 +21185,28 @@
                         } [n];
                     return a.a.createElement("tr", {
                         className: r,
                         key: "tab-" + t
                     }, a.a.createElement("th", null, t), a.a.createElement("td", null, o), a.a.createElement("td", null, i))
                 })))))
             }
-        }]) && va(t.prototype, n), r && va(t, r), Object.defineProperty(t, "prototype", {
+        }]) && ya(t.prototype, n), r && ya(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), i
     }(U.a);
     wa.defaultProps = {}, wa.propTypes = {
         id: V.a.string.isRequired,
         config: V.a.any,
         meta: V.a.any.isRequired,
         meta_out: V.a.any,
         setProps: V.a.func
     };
     var Ea = wa;
     const ja = () => {},
-        Ma = r.forwardRef(({
+        ka = r.forwardRef(({
             bsPrefix: e,
             name: t,
             className: n,
             checked: r,
             type: a,
             onChange: o,
             value: l,
@@ -21231,16 +21231,16 @@
                 ref: d,
                 className: i()(n, u && "disabled"),
                 type: void 0,
                 as: "label",
                 htmlFor: s
             })]
         })));
-    Ma.displayName = "ToggleButton";
-    var ka = Ma;
+    ka.displayName = "ToggleButton";
+    var Ma = ka;
 
     function Pa(e) {
         return (Pa = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -21759,19 +21759,19 @@
                 return React.createElement("div", null, "Put you  plot config GUI here")
             }
         }, {
             key: "multiSelect",
             value: function(e, t, n) {
                 var r = this,
                     a = this.props.id;
-                return React.createElement(Q.a, {
+                return React.createElement(G.a, {
                     className: "mb-1 w-100",
                     id: a + "-group-" + t,
                     key: a + "-group-" + t
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     className: "d-flex flex-grow-1",
                     id: a + "-group-text-" + t,
                     key: a + "-group-text-" + t,
                     style: {
                         minWidth: 75
                     }
                 }, e), React.createElement("div", {
@@ -21789,19 +21789,19 @@
                 }), t, this.props.allOptions)))))
             }
         }, {
             key: "multiSelect_ExtraOption",
             value: function(e, t, n) {
                 var r = this,
                     a = this.props.id;
-                return React.createElement(Q.a, {
+                return React.createElement(G.a, {
                     className: "mb-1 w-100",
                     id: a + "-group-" + t,
                     key: a + "-group-" + t
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     className: "d-flex flex-grow-1",
                     id: a + "-group-text-" + t,
                     key: a + "-group-text-" + t,
                     style: {
                         minWidth: 75
                     }
                 }, e), React.createElement("div", {
@@ -21818,19 +21818,19 @@
             }
         }, {
             key: "singleSelect",
             value: function(e, t, n) {
                 var r = this,
                     a = this.props.id,
                     o = t in this.state ? this.state[t] : [];
-                return React.createElement(Q.a, {
+                return React.createElement(G.a, {
                     className: "mb-1 w-100",
                     id: a + "-group-" + t,
                     key: a + "-group-" + t
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     className: "d-flex flex-grow-1",
                     id: a + "-group-text-" + t,
                     key: a + "-group-text-" + t,
                     style: {
                         minWidth: 75
                     }
                 }, e), React.createElement("div", {
@@ -21854,19 +21854,19 @@
             }
         }, {
             key: "singleSelect_ExtraOption",
             value: function(e, t, n) {
                 var r = this,
                     a = this.props.id,
                     o = t in this.state ? this.state[t] : [];
-                return React.createElement(Q.a, {
+                return React.createElement(G.a, {
                     className: "mb-1 w-100",
                     id: a + "-group-" + t,
                     key: a + "-group-" + t
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     className: "d-flex flex-grow-1",
                     id: a + "-group-text-" + t,
                     key: a + "-group-text-" + t,
                     style: {
                         minWidth: 75
                     }
                 }, e), React.createElement("div", {
@@ -21893,27 +21893,27 @@
                     a = this.props.id,
                     o = n.map((function(e, n) {
                         return e in r.state ? r.state[e] : t in r.state ? r.state[t][n] : null
                     })),
                     i = n.map((function(e, t) {
                         return o[t]
                     }));
-                return React.createElement(Q.a, {
+                return React.createElement(G.a, {
                     className: "mb-1 w-100",
                     id: a + "-input-" + t,
                     key: a + "-input-" + t
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     className: "d-flex flex-grow-1",
                     id: a + "-group-text-" + t,
                     key: a + "-group-text-" + t,
                     style: {
                         maxWidth: 75
                     }
                 }, e), n.map((function(e, n) {
-                    return React.createElement(G.a, {
+                    return React.createElement(Q.a, {
                         type: "number",
                         step: "any",
                         value: o[n],
                         size: "sm",
                         id: a + "-input-" + t + "-" + String(n),
                         key: a + "-input-" + t + "-" + String(n),
                         onChange: function(a) {
@@ -21932,26 +21932,26 @@
             }
         }, {
             key: "range_ManualString",
             value: function(e, t) {
                 var n = this,
                     r = this.props.id,
                     a = t in this.state ? this.state[t] : "";
-                return React.createElement(Q.a, {
+                return React.createElement(G.a, {
                     className: "mb-1 w-100",
                     id: r + "-group-" + t,
                     key: r + "-group-" + t
-                }, React.createElement(Q.a.Text, {
+                }, React.createElement(G.a.Text, {
                     className: "d-flex flex-grow-1",
                     id: r + "-group-text-" + t,
                     key: r + "-group-text-" + t,
                     style: {
                         maxWidth: 75
                     }
-                }, e), React.createElement(G.a, {
+                }, e), React.createElement(Q.a, {
                     value: a,
                     size: "sm",
                     id: r + "-input-" + t,
                     key: r + "-input-" + t,
                     onChange: function(e) {
                         "titleadfasdfasdfs" === t ? n.setState(Na({}, t, e.target.value)) : n.setStateConfig(Na({}, t, e.target.value))
                     }
@@ -21959,15 +21959,15 @@
             }
         }, {
             key: "toggleSelect",
             value: function(e, t, n) {
                 var r = this,
                     a = this.props.id,
                     o = t in this.state ? this.state[t] : n[0];
-                return React.createElement(ka, {
+                return React.createElement(Ma, {
                     id: a + "-toggle-" + t,
                     key: a + "-toggle-" + t,
                     type: "checkbox",
                     variant: "outline-primary",
                     checked: o,
                     onChange: function(e) {
                         var a = o === n[0] ? n[1] : n[0];
@@ -22001,15 +22001,15 @@
                     n = this.props.id;
                 return React.createElement(F, {
                     "aria-label": n + "toggle-group-bar",
                     id: n + "toggle-group-bar",
                     key: n + "toggle-group-bar",
                     className: "w-100 mt-3 mb-2"
                 }, e.map((function(r) {
-                    return React.createElement(ka, {
+                    return React.createElement(Ma, {
                         id: n + "-toggle-" + r.id,
                         key: n + "-toggle-" + r.id,
                         type: "checkbox",
                         variant: "outline-primary",
                         checked: r.visible,
                         onChange: function(n) {
                             return t.toggle_optionsbar(r.id, e)
@@ -22241,39 +22241,39 @@
                 return React.createElement("div", null, this.multiSelect("X", "x", t), this.multiSelect("Y", "y", t), this.singleSelect("Color", "color", t), this.singleSelect("Symb.", "symbol", n), this.singleSelect("Size", "size", r), this.optionsBar(a), this.commonOptionBarControlls())
             }
         }]) && qa(t.prototype, n), r && qa(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
     }(Ia);
 
-    function Qa(e) {
-        return (Qa = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Ga(e) {
+        return (Ga = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function Ga(e, t) {
+    function Qa(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
     function Ja(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Ga(Object(n), !0).forEach((function(t) {
+            t % 2 ? Qa(Object(n), !0).forEach((function(t) {
                 no(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ga(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Qa(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function Za(e, t) {
@@ -22307,15 +22307,15 @@
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return eo(this, n)
         }
     }
 
     function eo(e, t) {
-        if (t && ("object" === Qa(t) || "function" == typeof t)) return t;
+        if (t && ("object" === Ga(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
@@ -22714,27 +22714,27 @@
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function vo(e) {
+    function yo(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
             t % 2 ? bo(Object(n), !0).forEach((function(t) {
                 Eo(e, t, n[t])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : bo(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function yo(e, t) {
+    function vo(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
     function go(e, t) {
@@ -22824,22 +22824,22 @@
         }(o, e);
         var t, n, r, a = Oo(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-            }(this, o), (t = a.call(this, e)).state = vo(vo({}, t.state), {}, {
+            }(this, o), (t = a.call(this, e)).state = yo(yo({}, t.state), {}, {
                 optionsbar: [t.option_dict.facet, t.option_dict.axis_onlycolor, t.option_dict.render]
             }), t.copy_params("imshow"), t.init_check_options(!0), t
         }
         return t = o, (n = [{
             key: "config_from_state",
             value: function(e) {
-                var t = vo(vo({}, this.base_config_from_state()), e);
+                var t = yo(yo({}, this.base_config_from_state()), e);
                 return "hover_data" in (t = this.preferSimple(t)) && "string" == typeof t.hover_data && (t.hover_data = [t.hover_data]), {
                     type: "imshow",
                     params: t
                 }
             }
         }, {
             key: "render",
@@ -22848,44 +22848,44 @@
                     t = e.allColOptions,
                     n = e.numColOptions,
                     r = e.optionsbar;
                 return React.createElement("div", {
                     key: "div-" + this.props.id
                 }, this.singleSelect("X", "x", n), this.singleSelect("Y", "y", n), this.multiSelect("Dim", "dimensions", t), this.optionsBar(r), this.commonOptionBarControlls())
             }
-        }]) && yo(t.prototype, n), r && yo(t, r), Object.defineProperty(t, "prototype", {
+        }]) && vo(t.prototype, n), r && vo(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
     }(Ia);
 
-    function Mo(e) {
-        return (Mo = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function ko(e) {
+        return (ko = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
-    function ko(e, t) {
+    function Mo(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
     function Po(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? ko(Object(n), !0).forEach((function(t) {
+            t % 2 ? Mo(Object(n), !0).forEach((function(t) {
                 zo(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ko(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Mo(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function xo(e, t) {
@@ -22919,15 +22919,15 @@
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return Co(this, n)
         }
     }
 
     function Co(e, t) {
-        if (t && ("object" === Mo(t) || "function" == typeof t)) return t;
+        if (t && ("object" === ko(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
@@ -23228,23 +23228,23 @@
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ko(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Qo(e, t) {
+    function Go(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
-    function Go(e, t) {
-        return (Go = Object.setPrototypeOf || function(e, t) {
+    function Qo(e, t) {
+        return (Qo = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
     function Jo(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
@@ -23340,15 +23340,15 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }),
                 writable: !1
-            }), t && Go(e, t)
+            }), t && Qo(e, t)
         }(o, e);
         var t, n, r, a = Jo(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
@@ -23371,15 +23371,15 @@
                 var e = this.state,
                     t = e.allColOptions,
                     n = e.catColOptions,
                     r = e.numColOptions,
                     a = e.optionsbar;
                 return React.createElement("div", null, this.multiSelect("Dim", "dimensions", t), this.singleSelect("Color", "color", t), this.singleSelect("Symb.", "symbol", n), this.singleSelect("Size", "size", r), this.optionsBar(a), this.commonOptionBarControlls())
             }
-        }]) && Qo(t.prototype, n), r && Qo(t, r), Object.defineProperty(t, "prototype", {
+        }]) && Go(t.prototype, n), r && Go(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
     }(Ia);
 
     function ti(e) {
         return (ti = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
@@ -23721,34 +23721,34 @@
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }();
         return function() {
-            var n, r = yi(e);
+            var n, r = vi(e);
             if (t) {
-                var a = yi(this).constructor;
+                var a = vi(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
-            return vi(this, n)
+            return yi(this, n)
         }
     }
 
-    function vi(e, t) {
+    function yi(e, t) {
         if (t && ("object" === fi(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
-    function yi(e) {
-        return (yi = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+    function vi(e) {
+        return (vi = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
 
     function gi(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
@@ -23867,21 +23867,21 @@
     function ji(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
-    function Mi(e, t) {
-        return (Mi = Object.setPrototypeOf || function(e, t) {
+    function ki(e, t) {
+        return (ki = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function ki(e) {
+    function Mi(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -24051,17 +24051,17 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }),
                 writable: !1
-            }), t && Mi(e, t)
+            }), t && ki(e, t)
         }(o, e);
-        var t, n, r, a = ki(o);
+        var t, n, r, a = Mi(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
             }(this, o), (t = a.call(this, e)).state = Ei(Ei({}, t.state), {}, {
                 optionsbar: []
@@ -24448,18 +24448,18 @@
         id: V.a.string.isRequired,
         config: V.a.any,
         meta: V.a.any.isRequired,
         meta_out: V.a.any,
         setProps: V.a.func
     };
     var Yi = Ki,
-        Qi = n(56);
+        Gi = n(56);
 
-    function Gi(e) {
-        return (Gi = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Qi(e) {
+        return (Qi = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function Ji(e, t) {
@@ -24540,15 +24540,15 @@
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return al(this, n)
         }
     }
 
     function al(e, t) {
-        if (t && ("object" === Gi(t) || "function" == typeof t)) return t;
+        if (t && ("object" === Qi(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
@@ -24631,15 +24631,15 @@
                     animation: !1,
                     show: n,
                     onHide: function() {
                         return e.handleLoadClose()
                     }
                 }, a.a.createElement(L.a.Header, {
                     closeButton: !0
-                }, a.a.createElement(L.a.Title, null, "Load and save config")), a.a.createElement(L.a.Body, null, a.a.createElement(Q.a, {
+                }, a.a.createElement(L.a.Title, null, "Load and save config")), a.a.createElement(L.a.Body, null, a.a.createElement(G.a, {
                     className: "mb-3"
                 }, a.a.createElement(Y.a.Select, {
                     value: i,
                     onChange: function(t) {
                         e.setState({
                             selectedName: t.target.value
                         })
@@ -24657,19 +24657,19 @@
                         if (n.length > 0) {
                             var r = n[0].config;
                             e.props.setProps({
                                 config: r
                             }), e.handleLoadClose()
                         }
                     }
-                }, "Load")), a.a.createElement(Q.a, {
+                }, "Load")), a.a.createElement(G.a, {
                     className: "mb-3"
-                }, a.a.createElement(Q.a.Text, {
+                }, a.a.createElement(G.a.Text, {
                     id: "basic-addon1"
-                }, "Save"), a.a.createElement(G.a, {
+                }, "Save"), a.a.createElement(Q.a, {
                     value: l,
                     onChange: function(t) {
                         e.setState({
                             newName: t.target.value
                         })
                     }
                 }), a.a.createElement(B.a, {
@@ -24795,25 +24795,25 @@
         }();
         return function() {
             var n, r = gl(e);
             if (t) {
                 var a = gl(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
-            return vl(this, n)
+            return yl(this, n)
         }
     }
 
-    function vl(e, t) {
+    function yl(e, t) {
         if (t && ("object" === ll(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-        return yl(e)
+        return vl(e)
     }
 
-    function yl(e) {
+    function vl(e) {
         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
     }
 
     function gl(e) {
         return (gl = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
@@ -24882,15 +24882,15 @@
                     if ("data" in e && "configuratorId" in e.data && e.data.configuratorId == r.props.id) {
                         r.setState({
                             showEditModal: !0,
                             eventConfig: r.fix_config(e.data.defs),
                             eventThumbnail: e.data.thumbnail,
                             eventGraphId: e.data.graphId
                         });
-                        var t = yl(r),
+                        var t = vl(r),
                             n = setTimeout((function() {
                                 t.handleClose()
                             }), 5e3);
                         r.setState({
                             modal_close_timeout: n
                         })
                     }
@@ -25073,15 +25073,15 @@
                             e.update_props()
                         },
                         size: "lg",
                         variant: "outline-primary"
                     }, "New Plot"), "" !== l && !1))), this.props.showParameterization && React.createElement(Ol, {
                         title: "Parameterize",
                         defaultOpen: !0
-                    }, React.createElement(Qi.a, {
+                    }, React.createElement(Gi.a, {
                         id: "".concat(t, "-parametrize"),
                         key: "".concat(t, "-parametrize"),
                         meta: o,
                         config: ul({}, u),
                         setProps: function(t) {
                             if ("config" in t) {
                                 var n = ul({}, t.config);
@@ -25172,23 +25172,23 @@
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
 
-    function Ml(e, t) {
+    function kl(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
-    function kl(e, t) {
-        return (kl = Object.setPrototypeOf || function(e, t) {
+    function Ml(e, t) {
+        return (Ml = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
     function Pl(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
@@ -25232,15 +25232,15 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }),
                 writable: !1
-            }), t && kl(e, t)
+            }), t && Ml(e, t)
         }(o, e);
         var t, n, r, a = Pl(o);
 
         function o(e) {
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
             }(this, o), a.call(this, e)
@@ -25252,15 +25252,15 @@
                     t = window.dash_core_components.Graph;
                 return React.createElement(t, jl({}, this.props, {
                     setProps: function(t) {
                         return e.props.setProps(t)
                     }
                 }))
             }
-        }]) && Ml(t.prototype, n), r && Ml(t, r), Object.defineProperty(t, "prototype", {
+        }]) && kl(t.prototype, n), r && kl(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
     }(r.Component);
     Al.defaultProps = {
         id: null,
         figure: {
             data: [],
@@ -25451,37 +25451,37 @@
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function Yl(e) {
         return function(e) {
-            if (Array.isArray(e)) return Ql(e)
+            if (Array.isArray(e)) return Gl(e)
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }(e) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return Ql(e, t);
+            if ("string" == typeof e) return Gl(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Ql(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Gl(e, t)
         }(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function Ql(e, t) {
+    function Gl(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Gl() {
-        return (Gl = Object.assign || function(e) {
+    function Ql() {
+        return (Ql = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
@@ -25691,15 +25691,15 @@
                         i = 0 !== this.state.virtualIndices.length;
                     return a.a.createElement("div", {
                         style: {
                             width: "100%",
                             height: "100%",
                             position: "relative"
                         }
-                    }, a.a.createElement(t, Gl({}, r, {
+                    }, a.a.createElement(t, Ql({}, r, {
                         ref: this.datatable_ref,
                         setProps: function(t) {
                             "selected_rows" in t ? (e.setState({
                                 selected_rows: t.selected_rows
                             }), e.props.setProps({
                                 selectedData: {
                                     points: t.selected_rows.map((function(t) {
@@ -26316,25 +26316,25 @@
         }();
         return function() {
             var n, r = gc(e);
             if (t) {
                 var a = gc(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
-            return vc(this, n)
+            return yc(this, n)
         }
     }
 
-    function vc(e, t) {
+    function yc(e, t) {
         if (t && ("object" === pc(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-        return yc(e)
+        return vc(e)
     }
 
-    function yc(e) {
+    function vc(e) {
         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
     }
 
     function gc(e) {
         return (gc = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
@@ -26369,15 +26369,15 @@
                     filter_query: "",
                     config_modal_open: !1,
                     defParams: e.defParams,
                     meta: e.meta,
                     internalFigure: {
                         data: []
                     }
-                }, t.clearState = t.clearState.bind(yc(t)), t.config_in_modal_ref = a.a.createRef(), t.config_modal_id = (n = function() {
+                }, t.clearState = t.clearState.bind(vc(t)), t.config_in_modal_ref = a.a.createRef(), t.config_modal_id = (n = function() {
                     return Math.floor(65536 * (1 + Math.random())).toString(16).substring(1)
                 })() + n() + "-" + n() + "-" + n() + "-" + n() + "-" + n() + n() + n(), t
             }
             return t = i, (n = [{
                 key: "componentDidMount",
                 value: function() {
                     if ("plotApi" in this.props && "defParams" in this.props) {
@@ -26779,21 +26779,21 @@
     function jc(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
-    function Mc(e, t) {
-        return (Mc = Object.setPrototypeOf || function(e, t) {
+    function kc(e, t) {
+        return (kc = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function kc(e) {
+    function Mc(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -26832,17 +26832,17 @@
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }),
                 writable: !1
-            }), t && Mc(e, t)
+            }), t && kc(e, t)
         }(o, e);
-        var t, n, r, a = kc(o);
+        var t, n, r, a = Mc(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
             }(this, o), t = a.call(this, e), window.addEventListener("message", (function(n) {
                 "data" in n && "token" in n.data && n.data.token == t.props.token && e.setProps({
@@ -26955,22 +26955,22 @@
             return null === e ? "Null" : void 0 === e ? "Undefined" : Object.prototype.toString.call(e).slice(8, -1)
         }));
 
     function Yc(e, t, n, r) {
         var a = Tc(e);
 
         function o(e, t) {
-            return Qc(e, t, n.slice(), r.slice())
+            return Gc(e, t, n.slice(), r.slice())
         }
         return !Nc((function(e, t) {
             return !Nc(o, t, e)
         }), Tc(t), a)
     }
 
-    function Qc(e, t, n, r) {
+    function Gc(e, t, n, r) {
         if (Hc(e, t)) return !0;
         var a, o, i = Kc(e);
         if (i !== Kc(t)) return !1;
         if (null == e || null == t) return !1;
         if ("function" == typeof e["fantasy-land/equals"] || "function" == typeof t["fantasy-land/equals"]) return "function" == typeof e["fantasy-land/equals"] && e["fantasy-land/equals"](t) && "function" == typeof t["fantasy-land/equals"] && t["fantasy-land/equals"](e);
         if ("function" == typeof e.equals || "function" == typeof t.equals) return "function" == typeof e.equals && e.equals(t) && "function" == typeof t.equals && t.equals(e);
         switch (i) {
@@ -27026,21 +27026,21 @@
         }
         var c = Uc(e);
         if (c.length !== Uc(t).length) return !1;
         var u = n.concat([e]),
             s = r.concat([t]);
         for (l = c.length - 1; l >= 0;) {
             var f = c[l];
-            if (!Ic(f, t) || !Qc(t[f], e[f], u, s)) return !1;
+            if (!Ic(f, t) || !Gc(t[f], e[f], u, s)) return !1;
             l -= 1
         }
         return !0
     }
-    var Gc = Dc((function(e, t) {
-        return Qc(e, t, [], [])
+    var Qc = Dc((function(e, t) {
+        return Gc(e, t, [], [])
     }));
 
     function Jc(e) {
         return (Jc = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
@@ -27319,15 +27319,15 @@
                         n = e.id,
                         r = e.data;
                     "memory" !== e.storage_type && window.addEventListener("storage", this.onStorageChange);
                     var a = this._backstore.getItem(n);
                     if (zc(a) && !zc(r)) return this._backstore.setItem(n, r), void t({
                         modified_timestamp: this._backstore.getModified(n)
                     });
-                    Gc(a, r) || t({
+                    Qc(a, r) || t({
                         data: a,
                         modified_timestamp: this._backstore.getModified(n)
                     })
                 }
             }, {
                 key: "componentDidMount",
                 value: function() {
@@ -27348,19 +27348,19 @@
                         l = t.config;
                     if (a) return this._backstore.removeItem(r), void o({
                         clear_data: !1,
                         data: null,
                         modified_timestamp: this._backstore.getModified(r)
                     });
                     var c = this._backstore.getItem(r);
-                    Gc(n, c) || (void 0 === n ? o({
+                    Qc(n, c) || (void 0 === n ? o({
                         data: c
                     }) : (this._backstore.setItem(r, n), o({
                         modified_timestamp: this._backstore.getModified(r)
-                    }))), i === e.url && Gc(l, e.config) || i && l && this.fetchData(i, l)
+                    }))), i === e.url && Qc(l, e.config) || i && l && this.fetchData(i, l)
                 }
             }, {
                 key: "componentWillUnmount",
                 value: function() {
                     "memory" !== this.props.storage_type && window.removeEventListener("storage", this.onStorageChange)
                 }
             }, {
@@ -27381,34 +27381,533 @@
         data: V.a.oneOfType([V.a.object, V.a.array, V.a.number, V.a.string, V.a.bool]),
         clear_data: V.a.bool,
         modified_timestamp: V.a.number,
         setProps: V.a.func,
         url: V.a.string,
         config: V.a.object,
         longCallback: V.a.bool
-    }, n.d(t, "Configurator", (function() {
+    };
+    var pu = Array.isArray || function(e) {
+        return null != e && e.length >= 0 && "[object Array]" === Object.prototype.toString.call(e)
+    };
+
+    function du(e) {
+        return null != e && "function" == typeof e["@@transducer/step"]
+    }
+
+    function hu(e, t, n) {
+        return function() {
+            if (0 === arguments.length) return n();
+            var r = Array.prototype.slice.call(arguments, 0),
+                a = r.pop();
+            if (!pu(a)) {
+                for (var o = 0; o < e.length;) {
+                    if ("function" == typeof a[e[o]]) return a[e[o]].apply(a, r);
+                    o += 1
+                }
+                if (du(a)) {
+                    var i = t.apply(null, r);
+                    return i(a)
+                }
+            }
+            return n.apply(this, arguments)
+        }
+    }
+    var mu = function() {
+            return this.xf["@@transducer/init"]()
+        },
+        bu = function() {
+            function e(e, t) {
+                this.xf = t, this.f = e, this.all = !0
+            }
+            return e.prototype["@@transducer/init"] = mu, e.prototype["@@transducer/result"] = function(e) {
+                return this.all && (e = this.xf["@@transducer/step"](e, !0)), this.xf["@@transducer/result"](e)
+            }, e.prototype["@@transducer/step"] = function(e, t) {
+                var n;
+                return this.f(t) || (this.all = !1, e = (n = this.xf["@@transducer/step"](e, !1)) && n["@@transducer/reduced"] ? n : {
+                    "@@transducer/value": n,
+                    "@@transducer/reduced": !0
+                }), e
+            }, e
+        }(),
+        yu = Dc(hu(["all"], Dc((function(e, t) {
+            return new bu(e, t)
+        })), (function(e, t) {
+            for (var n = 0; n < t.length;) {
+                if (!e(t[n])) return !1;
+                n += 1
+            }
+            return !0
+        }))),
+        vu = Dc((function(e, t) {
+            return yu((n = e, function() {
+                return !n.apply(this, arguments)
+            }), t);
+            var n
+        }));
+
+    function gu(e) {
+        return (gu = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+            return typeof e
+        } : function(e) {
+            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+        })(e)
+    }
+
+    function Ou(e) {
+        return function(e) {
+            if (Array.isArray(e)) return _u(e)
+        }(e) || function(e) {
+            if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
+        }(e) || function(e, t) {
+            if (!e) return;
+            if ("string" == typeof e) return _u(e, t);
+            var n = Object.prototype.toString.call(e).slice(8, -1);
+            "Object" === n && e.constructor && (n = e.constructor.name);
+            if ("Map" === n || "Set" === n) return Array.from(e);
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return _u(e, t)
+        }(e) || function() {
+            throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
+        }()
+    }
+
+    function _u(e, t) {
+        (null == t || t > e.length) && (t = e.length);
+        for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
+        return r
+    }
+
+    function wu(e, t) {
+        var n = Object.keys(e);
+        if (Object.getOwnPropertySymbols) {
+            var r = Object.getOwnPropertySymbols(e);
+            t && (r = r.filter((function(t) {
+                return Object.getOwnPropertyDescriptor(e, t).enumerable
+            }))), n.push.apply(n, r)
+        }
+        return n
+    }
+
+    function Eu(e) {
+        for (var t = 1; t < arguments.length; t++) {
+            var n = null != arguments[t] ? arguments[t] : {};
+            t % 2 ? wu(Object(n), !0).forEach((function(t) {
+                ju(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : wu(Object(n)).forEach((function(t) {
+                Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
+            }))
+        }
+        return e
+    }
+
+    function ju(e, t, n) {
+        return t in e ? Object.defineProperty(e, t, {
+            value: n,
+            enumerable: !0,
+            configurable: !0,
+            writable: !0
+        }) : e[t] = n, e
+    }
+
+    function ku(e, t) {
+        for (var n = 0; n < t.length; n++) {
+            var r = t[n];
+            r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
+        }
+    }
+
+    function Mu(e, t) {
+        return (Mu = Object.setPrototypeOf || function(e, t) {
+            return e.__proto__ = t, e
+        })(e, t)
+    }
+
+    function Pu(e) {
+        var t = function() {
+            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
+            if (Reflect.construct.sham) return !1;
+            if ("function" == typeof Proxy) return !0;
+            try {
+                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
+            } catch (e) {
+                return !1
+            }
+        }();
+        return function() {
+            var n, r = Au(e);
+            if (t) {
+                var a = Au(this).constructor;
+                n = Reflect.construct(r, arguments, a)
+            } else n = r.apply(this, arguments);
+            return xu(this, n)
+        }
+    }
+
+    function xu(e, t) {
+        if (t && ("object" === gu(t) || "function" == typeof t)) return t;
+        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
+        return Su(e)
+    }
+
+    function Su(e) {
+        if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+        return e
+    }
+
+    function Au(e) {
+        return (Au = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+            return e.__proto__ || Object.getPrototypeOf(e)
+        })(e)
+    }
+    var Cu = function(e) {
+        ! function(e, t) {
+            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
+            Object.defineProperty(e, "prototype", {
+                value: Object.create(t && t.prototype, {
+                    constructor: {
+                        value: e,
+                        writable: !0,
+                        configurable: !0
+                    }
+                }),
+                writable: !1
+            }), t && Mu(e, t)
+        }(i, e);
+        var t, n, r, o = Pu(i);
+
+        function i(e) {
+            var t;
+            ! function(e, t) {
+                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+            }(this, i), t = o.call(this, e);
+            var n = e.defParams || t.getDefaultDefParams(e.data);
+            return t.state = {
+                data: e.data,
+                defParams: n,
+                meta: t.getMeta(e.data),
+                figure: t.getFigure(n, e.data)
+            }, t.handleGraphSetProps = t.handleGraphSetProps.bind(Su(t)), t
+        }
+        return t = i, (n = [{
+            key: "componentDidUpdate",
+            value: function(e) {
+                if (e.defParams !== this.props.defParams || e.data !== this.props.data) {
+                    var t = this.props.defParams || this.getDefaultDefParams(this.props.data),
+                        n = this.getMeta(this.props.data),
+                        r = this.getFigure(t, this.props.data);
+                    this.setState({
+                        defParams: t,
+                        data: this.props.data,
+                        meta: n,
+                        figure: r
+                    }), this.props.setProps && this.props.setProps({
+                        defParams: t,
+                        data: this.props.data,
+                        meta: n,
+                        figure: r
+                    })
+                }
+            }
+        }, {
+            key: "handleGraphSetProps",
+            value: function(e) {
+                var t = e.defParams || this.state.defParams,
+                    n = e.data || this.state.data;
+                if (JSON.stringify(t) !== JSON.stringify(this.state.defParams)) {
+                    var r = this.getFigure(t, n);
+                    this.props.setProps && this.props.setProps(Eu(Eu({}, e), {}, {
+                        figure: r
+                    })), this.setState(Eu(Eu({}, e), {}, {
+                        figure: r,
+                        defParams: t
+                    }))
+                } else this.props.setProps && this.props.setProps(e), this.setState(e)
+            }
+        }, {
+            key: "getDefaultDefParams",
+            value: function(e) {
+                return {
+                    filter: [],
+                    transform: [],
+                    plot: {
+                        type: "table",
+                        params: {
+                            dimensions: Object.keys(e)
+                        }
+                    }
+                }
+            }
+        }, {
+            key: "getMeta",
+            value: function(e) {
+                function t(t, n) {
+                    if ("categorical" === n) {
+                        var r = Ou(new Set(e[t]));
+                        return r.length > 1e3 ? {
+                            type: "categorical",
+                            large: !0,
+                            cat: []
+                        } : {
+                            type: "categorical",
+                            cat: r
+                        }
+                    }
+                    if ("boolean" === n) return {
+                        type: "boolean"
+                    };
+                    if ("temporal" === n) {
+                        var a = e[t].filter((function(e) {
+                                return null != e
+                            })).map((function(e) {
+                                return new Date(e)
+                            })),
+                            o = new Date(Math.min.apply(null, a)),
+                            i = new Date(Math.max.apply(null, a));
+                        return {
+                            type: "temporal",
+                            median: new Date(a.sort((function(e, t) {
+                                return e - t
+                            }))[Math.floor(a.length / 2)]),
+                            min: o,
+                            max: i
+                        }
+                    }
+                    if ("numerical" === n) {
+                        var l = e[t].filter((function(e) {
+                                return null != e
+                            })).map(Number),
+                            c = Math.min.apply(Math, Ou(l)),
+                            u = Math.max.apply(Math, Ou(l));
+                        return {
+                            type: "numerical",
+                            median: l.sort((function(e, t) {
+                                return e - t
+                            }))[Math.floor(l.length / 2)],
+                            min: c,
+                            max: u
+                        }
+                    }
+                    return function(t) {
+                        var n = Ou(new Set(e[t]));
+                        return n.length > 1e3 ? {
+                            type: "categorical",
+                            large: !0,
+                            cat: []
+                        } : {
+                            type: "categorical",
+                            cat: n
+                        }
+                    }(t)
+                }
+                return Object.keys(e).reduce((function(n, r) {
+                    var a, o = e[r][0],
+                        i = gu(o);
+                    return a = "string" === i ? isNaN(Date.parse(o)) ? "categorical" : "temporal" : "boolean" === i ? "boolean" : "number" === i ? "numerical" : "categorical", n[r] = t(r, a), n
+                }), {})
+            }
+        }, {
+            key: "getFigure",
+            value: function(e, t) {
+                var n = this;
+                if (console.log(e), !e || !e.plot || !e.plot.params) return {
+                    data: [],
+                    layout: {}
+                };
+                var r = e.plot,
+                    a = r.type,
+                    o = r.params,
+                    i = {
+                        data: [],
+                        layout: {}
+                    };
+                if ("scatter" === a) {
+                    var l = o.x,
+                        c = o.y,
+                        u = o.color,
+                        s = o.symbol,
+                        f = o.size,
+                        p = o.facet_col,
+                        d = o.facet_row,
+                        h = o.facet_col_wrap,
+                        m = o.log_x,
+                        b = o.log_y,
+                        y = o.reversed_x,
+                        v = o.reversed_y,
+                        g = o.cat_x,
+                        O = o.cat_y,
+                        _ = o.range_x,
+                        w = o.range_y,
+                        E = o.indep_x,
+                        j = o.indep_y,
+                        k = function(e, r) {
+                            var a = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "x",
+                                o = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "y",
+                                i = {
+                                    x: e.data[l],
+                                    y: e.data[c],
+                                    mode: "markers",
+                                    type: "scatter",
+                                    name: r,
+                                    xaxis: a,
+                                    yaxis: o
+                                };
+                            return u && (n.isNumerical(t[u]) ? i.marker = {
+                                color: e.data[u]
+                            } : i.marker = {
+                                color: e.name
+                            }), s && (i.marker = Eu(Eu({}, i.marker), {}, {
+                                symbol: e.data.symbol
+                            })), f && (i.marker = Eu(Eu({}, i.marker), {}, {
+                                size: e.data.size
+                            })), g && (i.x = e.data[g]), O && (i.y = e.data[O]), i
+                        };
+                    if (p || d) {
+                        var M = this.groupData(t, {
+                                color: u,
+                                facet_col: p,
+                                facet_row: d
+                            }),
+                            P = d ? Ou(new Set(t[d])) : [null],
+                            x = p ? Ou(new Set(t[p])) : [null],
+                            S = P.length,
+                            A = x.length;
+                        h && !d && (S = Math.ceil(A / h), A = Math.min(A, h)), i.layout.grid = {
+                            rows: S,
+                            columns: A,
+                            subplots: [],
+                            roworder: "bottom to top",
+                            pattern: E || j ? "independent" : vu
+                        };
+                        var C = 0;
+                        P.forEach((function(e, t) {
+                            for (var n = function(t) {
+                                    var n, r = Math.floor(C / A),
+                                        a = C % A,
+                                        o = x[t],
+                                        u = M.find((function(t) {
+                                            return !(e && t.row !== e || o && t.col !== o)
+                                        })) || {
+                                            data: (n = {}, ju(n, l, []), ju(n, c, []), n),
+                                            name: "".concat(e, "-").concat(o)
+                                        },
+                                        s = k(u, u.colorName, "x".concat(a + 1 === 1 ? "" : a + 1), "y".concat(r + 1 === 1 ? "" : r + 1));
+                                    i.data.push(s), i.layout.grid.subplots[r] || (i.layout.grid.subplots[r] = []), i.layout.grid.subplots[r][a] = "".concat(s.xaxis).concat(s.yaxis), C++
+                                }, r = 0; r < x.length; r++) n(r)
+                        }))
+                    } else this.groupData(t, {
+                        color: u
+                    }).forEach((function(e) {
+                        var t = k(e, e.colorName);
+                        i.data.push(t)
+                    }));
+                    m && (i.layout.xaxis = {
+                        type: "log"
+                    }), b && (i.layout.yaxis = {
+                        type: "log"
+                    }), y && (i.layout.xaxis = Eu(Eu({}, i.layout.xaxis), {}, {
+                        autorange: "reversed"
+                    })), v && (i.layout.yaxis = Eu(Eu({}, i.layout.yaxis), {}, {
+                        autorange: "reversed"
+                    })), _ && (i.layout.xaxis = Eu(Eu({}, i.layout.xaxis), {}, {
+                        range: _
+                    })), w && (i.layout.yaxis = Eu(Eu({}, i.layout.yaxis), {}, {
+                        range: w
+                    }))
+                }
+                return "table" === a ? t : i
+            }
+        }, {
+            key: "groupData",
+            value: function(e, t) {
+                var n = t.color,
+                    r = t.facet_col,
+                    a = t.facet_row,
+                    o = [n, r, a].filter(Boolean);
+                if (0 === o.length) return [{
+                    data: e,
+                    name: "default",
+                    colorName: null
+                }];
+                var i = {},
+                    l = {};
+                return e[Object.keys(e)[0]].forEach((function(t, c) {
+                    var u = o.map((function(t) {
+                        return e[t][c]
+                    })).join("-");
+                    i[u] || (i[u] = {}, Object.keys(e).forEach((function(e) {
+                        return i[u][e] = []
+                    }))), Object.keys(e).forEach((function(t) {
+                        return i[u][t].push(e[t][c])
+                    })), l[u] || (l[u] = {
+                        name: u,
+                        colorName: n ? e[n][c] : null,
+                        row: a ? e[a][c] : null,
+                        col: r ? e[r][c] : null
+                    })
+                })), Object.keys(i).map((function(e) {
+                    return {
+                        data: i[e],
+                        name: l[e].name,
+                        colorName: l[e].colorName,
+                        col: l[e].col,
+                        row: l[e].row
+                    }
+                }))
+            }
+        }, {
+            key: "isNumerical",
+            value: function(e) {
+                return "number" == typeof e[0]
+            }
+        }, {
+            key: "render",
+            value: function() {
+                return a.a.createElement(wc, {
+                    id: this.props.id,
+                    defParams: this.state.defParams,
+                    meta: this.state.meta,
+                    figure: this.state.figure,
+                    setProps: this.handleGraphSetProps
+                })
+            }
+        }]) && ku(t.prototype, n), r && ku(t, r), Object.defineProperty(t, "prototype", {
+            writable: !1
+        }), i
+    }(r.Component);
+    Cu.propTypes = {
+        id: V.a.string.isRequired,
+        defParams: V.a.object,
+        data: V.a.object,
+        setProps: V.a.func
+    }, Cu.defaultProps = {
+        data: {}
+    };
+    var Ru = Cu;
+    n.d(t, "Configurator", (function() {
         return wl
     })), n.d(t, "Filter", (function() {
         return me
     })), n.d(t, "Transform", (function() {
         return ma
     })), n.d(t, "Plotter", (function() {
         return Yi
     })), n.d(t, "Parameterize", (function() {
-        return Qi.a
+        return Gi.a
     })), n.d(t, "Graph", (function() {
         return wc
     })), n.d(t, "MetaCheck", (function() {
         return Ea
     })), n.d(t, "Localstore", (function() {
         return il
     })), n.d(t, "ConfigReceiver", (function() {
         return Ac
     })), n.d(t, "RequestStore", (function() {
         return fu
+    })), n.d(t, "DataGraph", (function() {
+        return Ru
     }))
 }, function(e, t, n) {
     "use strict";
     n.r(t);
     var r, a = n(0),
         o = n.n(a),
         i = n(1),
@@ -27450,57 +27949,57 @@
             }
         }(d) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()).map((function(e, t) {
             return t
         }));
 
-    function v(e) {
+    function y(e) {
         return function(t, n) {
             return function(e) {
                 return function(t, n) {
                     return n.toLocaleString(t || Object(u.default)(), e)
                 }
             }(e)(t, function(e) {
                 var t = new Date(e);
                 return new Date(t.setHours(12))
             }(n))
         }
     }
-    v({
+    y({
         day: "numeric",
         month: "numeric",
         year: "numeric"
     });
-    var y = v({
+    var v = y({
             day: "numeric"
         }),
-        g = v({
+        g = y({
             day: "numeric",
             month: "long",
             year: "numeric"
         }),
-        O = v({
+        O = y({
             month: "long"
         }),
-        _ = v({
+        _ = y({
             month: "long",
             year: "numeric"
         }),
-        w = v({
+        w = y({
             weekday: "short"
         }),
-        E = v({
+        E = y({
             weekday: "long"
         }),
-        j = v({
+        j = y({
             year: "numeric"
         }),
-        M = b[0],
-        k = b[5],
+        k = b[0],
+        M = b[5],
         P = b[6];
 
     function x(e) {
         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : h.ISO_8601,
             n = e.getDay();
         switch (t) {
             case h.ISO_8601:
@@ -27610,18 +28109,18 @@
 
     function I(e) {
         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : h.ISO_8601,
             n = e.getDay();
         switch (t) {
             case h.ARABIC:
             case h.HEBREW:
-                return n === k || n === P;
+                return n === M || n === P;
             case h.ISO_8601:
             case h.US:
-                return n === P || n === M;
+                return n === P || n === k;
             default:
                 throw new Error("Unsupported calendar type.")
         }
     }
 
     function H(e) {
         return (H = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
@@ -27649,26 +28148,26 @@
             return a && r < a ? new Error("Invalid prop `".concat(t, "` of type `").concat(H(r), "` supplied to `").concat(n, "`, maxDate cannot be smaller than minDate.")) : null
         },
         U = l.a.oneOfType([l.a.func, l.a.shape({
             current: l.a.any
         })]),
         K = l.a.oneOfType([l.a.instanceOf(Date), l.a.arrayOf(l.a.instanceOf(Date))]),
         Y = l.a.arrayOf(l.a.oneOf(B)),
-        Q = function(e, t, n) {
+        G = function(e, t, n) {
             var r = e[t],
                 a = e.views || B;
             return void 0 !== r && -1 === a.indexOf(r) ? new Error("Invalid prop `".concat(t, "` of value `").concat(r, "` supplied to `").concat(n, "`, expected one of [").concat(a.map((function(e) {
                 return '"'.concat(e, '"')
             })).join(", "), "].")) : null
         };
-    Q.isRequired = function(e, t, n) {
+    G.isRequired = function(e, t, n) {
         var r = e[t];
-        return r ? Q(e, t, n) : new Error("The prop `".concat(t, "` is marked as required in `").concat(n, "`, but its value is `").concat(r, "`."))
+        return r ? G(e, t, n) : new Error("The prop `".concat(t, "` is marked as required in `").concat(n, "`, but its value is `").concat(r, "`."))
     };
-    var G = {
+    var Q = {
             activeStartDate: l.a.instanceOf(Date).isRequired,
             hover: l.a.instanceOf(Date),
             locale: l.a.string,
             maxDate: V,
             minDate: W,
             onClick: l.a.func,
             onMouseOver: l.a.func,
@@ -27702,23 +28201,23 @@
             c = void 0 === l ? j : l,
             f = e.locale,
             p = e.maxDate,
             d = e.minDate,
             h = e.navigationAriaLabel,
             m = void 0 === h ? "" : h,
             b = e.navigationAriaLive,
-            v = e.navigationLabel,
-            y = e.next2AriaLabel,
-            g = void 0 === y ? "" : y,
+            y = e.navigationLabel,
+            v = e.next2AriaLabel,
+            g = void 0 === v ? "" : v,
             O = e.next2Label,
             w = void 0 === O ? "»" : O,
             E = e.nextAriaLabel,
-            M = void 0 === E ? "" : E,
-            k = e.nextLabel,
-            P = void 0 === k ? "›" : k,
+            k = void 0 === E ? "" : E,
+            M = e.nextLabel,
+            P = void 0 === M ? "›" : M,
             x = e.prev2AriaLabel,
             S = void 0 === x ? "" : x,
             A = e.prev2Label,
             R = void 0 === A ? "«" : A,
             z = e.prevAriaLabel,
             D = void 0 === z ? "" : z,
             I = e.prevLabel,
@@ -27763,15 +28262,15 @@
                         return Object(s.getNextYearStart)(t, 10);
                     case "month":
                         return Object(s.getNextMonthStart)(t, 12);
                     default:
                         throw new Error("Invalid rangeType: ".concat(e))
                 }
             }(q, n),
-            Q = function() {
+            G = function() {
                 if (V.getFullYear() < 0) return !0;
                 var e = function(e, t) {
                     switch (e) {
                         case "century":
                             return Object(s.getPreviousCenturyEnd)(t);
                         case "decade":
                             return Object(s.getPreviousDecadeEnd)(t);
@@ -27781,15 +28280,15 @@
                             return Object(s.getPreviousMonthEnd)(t);
                         default:
                             throw new Error("Invalid rangeType: ".concat(e))
                     }
                 }(q, n);
                 return d && d >= e
             }(),
-            G = W && function() {
+            Q = W && function() {
                 if (U.getFullYear() < 0) return !0;
                 var e = function(e, t) {
                     switch (e) {
                         case "decade":
                             return Object(s.getPreviousDecadeEnd)(t, -100);
                         case "year":
                             return Object(s.getPreviousYearEnd)(t, -10);
@@ -27817,35 +28316,35 @@
                         return c(f, e);
                     case "month":
                         return i(f, e);
                     default:
                         throw new Error("Invalid view: ".concat(q, "."))
                 }
             }();
-            return v ? v({
+            return y ? y({
                 date: e,
                 label: t,
                 locale: f || Object(u.getUserLocale)(),
                 view: q
             }) : t
         }
         return o.a.createElement("div", {
             className: Z
         }, null !== R && W && o.a.createElement("button", {
             "aria-label": S,
             className: "".concat(Z, "__arrow ").concat(Z, "__prev2-button"),
-            disabled: G,
+            disabled: Q,
             onClick: function() {
                 L(U, "prev2")
             },
             type: "button"
         }, R), null !== H && o.a.createElement("button", {
             "aria-label": D,
             className: "".concat(Z, "__arrow ").concat(Z, "__prev-button"),
-            disabled: Q,
+            disabled: G,
             onClick: function() {
                 L(V, "prev")
             },
             type: "button"
         }, H), (t = "".concat(Z, "__label"), o.a.createElement("button", {
             "aria-label": m,
             "aria-live": b,
@@ -27859,15 +28358,15 @@
         }, o.a.createElement("span", {
             className: "".concat(t, "__labelText ").concat(t, "__labelText--from")
         }, $(n)), B && o.a.createElement(o.a.Fragment, null, o.a.createElement("span", {
             className: "".concat(t, "__divider")
         }, " ", "–", " "), o.a.createElement("span", {
             className: "".concat(t, "__labelText ").concat(t, "__labelText--to")
         }, $(K))))), null !== P && o.a.createElement("button", {
-            "aria-label": M,
+            "aria-label": k,
             className: "".concat(Z, "__arrow ").concat(Z, "__next-button"),
             disabled: J,
             onClick: function() {
                 L(K, "next")
             },
             type: "button"
         }, P), null !== w && W && o.a.createElement("button", {
@@ -27897,15 +28396,15 @@
         nextLabel: l.a.node,
         prev2AriaLabel: l.a.string,
         prev2Label: l.a.node,
         prevAriaLabel: l.a.string,
         prevLabel: l.a.node,
         setActiveStartDate: l.a.func.isRequired,
         showDoubleView: l.a.bool,
-        view: Q.isRequired,
+        view: G.isRequired,
         views: Y.isRequired
     };
     var $ = ["children", "className", "direction", "count", "offset", "style", "wrap"];
 
     function ee() {
         return (ee = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
@@ -28091,33 +28590,33 @@
         return n
     }
 
     function be(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
             t % 2 ? me(Object(n), !0).forEach((function(t) {
-                ve(e, t, n[t])
+                ye(e, t, n[t])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : me(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function ve(e, t, n) {
+    function ye(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function ye() {
-        return (ye = Object.assign || function(e) {
+    function ve() {
+        return (ve = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
@@ -28135,35 +28634,35 @@
             var o = Object.getOwnPropertySymbols(e);
             for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (a[n] = e[n])
         }
         return a
     }
 
     function Oe(e) {
-        for (var t = e.className, n = e.count, r = void 0 === n ? 3 : n, a = e.dateTransform, i = e.dateType, l = e.end, c = e.hover, u = e.offset, s = e.start, f = e.step, p = void 0 === f ? 1 : f, d = e.tile, h = e.value, m = e.valueType, b = ge(e, he), v = [], y = s; y <= l; y += p) {
-            var g = a(y);
-            v.push(o.a.createElement(d, ye({
+        for (var t = e.className, n = e.count, r = void 0 === n ? 3 : n, a = e.dateTransform, i = e.dateType, l = e.end, c = e.hover, u = e.offset, s = e.start, f = e.step, p = void 0 === f ? 1 : f, d = e.tile, h = e.value, m = e.valueType, b = ge(e, he), y = [], v = s; v <= l; v += p) {
+            var g = a(v);
+            y.push(o.a.createElement(d, ve({
                 key: g.getTime(),
                 classes: de({
                     value: h,
                     valueType: m,
                     date: g,
                     dateType: i,
                     hover: c
                 }),
                 date: g,
-                point: y
+                point: v
             }, b)))
         }
         return o.a.createElement(ie, {
             className: t,
             count: r,
             offset: u,
             wrap: !0
-        }, v)
+        }, y)
     }
 
     function _e(e) {
         return (_e = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
@@ -28193,23 +28692,23 @@
         return e
     }
 
     function je(e, t) {
         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
     }
 
-    function Me(e, t) {
+    function ke(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
-    function ke(e, t) {
-        return (ke = Object.setPrototypeOf || function(e, t) {
+    function Me(e, t) {
+        return (Me = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
     function Pe(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
@@ -28263,15 +28762,15 @@
             a = e.view;
         return "function" == typeof t ? t({
             activeStartDate: n,
             date: r,
             view: a
         }) : t
     }
-    Oe.propTypes = be(be({}, G), {}, {
+    Oe.propTypes = be(be({}, Q), {}, {
         activeStartDate: l.a.instanceOf(Date),
         count: l.a.number,
         dateTransform: l.a.func.isRequired,
         dateType: l.a.string,
         offset: l.a.number,
         step: l.a.number,
         tile: l.a.func.isRequired
@@ -28281,15 +28780,15 @@
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             e.prototype = Object.create(t && t.prototype, {
                 constructor: {
                     value: e,
                     writable: !0,
                     configurable: !0
                 }
-            }), t && ke(e, t)
+            }), t && Me(e, t)
         }(i, e);
         var t, n, r, a = Pe(i);
 
         function i() {
             var e;
             je(this, i);
             for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
@@ -28317,24 +28816,24 @@
                     s = e.maxDateTransform,
                     f = e.minDate,
                     p = e.minDateTransform,
                     d = e.onClick,
                     h = e.onMouseOver,
                     m = e.style,
                     b = e.tileDisabled,
-                    v = e.view,
-                    y = this.state,
-                    g = y.tileClassName,
-                    O = y.tileContent;
+                    y = e.view,
+                    v = this.state,
+                    g = v.tileClassName,
+                    O = v.tileContent;
                 return o.a.createElement("button", {
                     className: Object(c.default)(r, g),
                     disabled: f && p(f) > a || u && s(u) < a || b && b({
                         activeStartDate: t,
                         date: a,
-                        view: v
+                        view: y
                     }),
                     onClick: d && function(e) {
                         return d(a, e)
                     },
                     onFocus: h && function() {
                         return h(a)
                     },
@@ -28343,15 +28842,15 @@
                     },
                     style: m,
                     type: "button"
                 }, i ? o.a.createElement("abbr", {
                     "aria-label": i(l, a)
                 }, n) : n, O)
             }
-        }]) && Me(t.prototype, n), r && Me(t, r), i
+        }]) && ke(t.prototype, n), r && ke(t, r), i
     }(a.Component);
     ze.propTypes = Ee(Ee({}, J), {}, {
         children: l.a.node.isRequired,
         formatAbbr: l.a.func,
         maxDateTransform: l.a.func.isRequired,
         minDateTransform: l.a.func.isRequired
     });
@@ -28488,41 +28987,41 @@
             t % 2 ? qe(Object(n), !0).forEach((function(t) {
                 Fe(e, t, n[t])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : qe(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
-    }({}, G);
+    }({}, Q);
     var Ke = ["classes", "formatYear"];
 
     function Ye(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Qe(e) {
+    function Ge(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
             t % 2 ? Ye(Object(n), !0).forEach((function(t) {
-                Ge(e, t, n[t])
+                Qe(e, t, n[t])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ye(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Ge(e, t, n) {
+    function Qe(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
@@ -28616,27 +29115,27 @@
     }
 
     function rt(e) {
         return o.a.createElement("div", {
             className: "react-calendar__decade-view"
         }, o.a.createElement(nt, e))
     }
-    Xe.propTypes = Qe(Qe({}, J), {}, {
+    Xe.propTypes = Ge(Ge({}, J), {}, {
         formatYear: l.a.func
     }), nt.propTypes = function(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
             t % 2 ? $e(Object(n), !0).forEach((function(t) {
                 et(e, t, n[t])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : $e(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
-    }({}, G);
+    }({}, Q);
     var at = ["classes", "formatMonth", "formatMonthYear"];
 
     function ot(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
@@ -28773,36 +29272,36 @@
         return o.a.createElement("div", {
             className: "react-calendar__year-view"
         }, o.a.createElement(mt, e))
     }
     st.propTypes = it(it({}, J), {}, {
         formatMonth: l.a.func,
         formatMonthYear: l.a.func
-    }), mt.propTypes = pt(pt({}, G), {}, {
+    }), mt.propTypes = pt(pt({}, Q), {}, {
         locale: l.a.string
     });
-    var vt = ["formatDay", "formatLongDate", "calendarType", "classes", "currentMonthIndex"];
+    var yt = ["formatDay", "formatLongDate", "calendarType", "classes", "currentMonthIndex"];
 
-    function yt(e, t) {
+    function vt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
     function gt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? yt(Object(n), !0).forEach((function(t) {
+            t % 2 ? vt(Object(n), !0).forEach((function(t) {
                 Ot(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : yt(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : vt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function Ot(e, t, n) {
@@ -28839,21 +29338,21 @@
         }
         return a
     }
     var Et = "react-calendar__month-view__days__day";
 
     function jt(e) {
         var t = e.formatDay,
-            n = void 0 === t ? y : t,
+            n = void 0 === t ? v : t,
             r = e.formatLongDate,
             a = void 0 === r ? g : r,
             i = e.calendarType,
             l = e.classes,
             c = e.currentMonthIndex,
-            u = wt(e, vt),
+            u = wt(e, yt),
             f = u.date,
             p = u.locale;
         return o.a.createElement(ze, _t({}, u, {
             classes: [].concat(l, Et, I(f, i) ? "".concat(Et, "--weekend") : null, f.getMonth() !== c ? "".concat(Et, "--neighboringMonth") : null),
             formatAbbr: a,
             maxDateTransform: s.getDayEnd,
             minDateTransform: s.getDayStart,
@@ -28861,17 +29360,17 @@
         }), n(p, f))
     }
     jt.propTypes = gt(gt({}, J), {}, {
         currentMonthIndex: l.a.number.isRequired,
         formatDay: l.a.func,
         formatLongDate: l.a.func
     });
-    var Mt = ["showFixedNumberOfWeeks", "showNeighboringMonth"];
+    var kt = ["showFixedNumberOfWeeks", "showNeighboringMonth"];
 
-    function kt(e, t) {
+    function Mt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
@@ -28914,15 +29413,15 @@
     }
 
     function At(e) {
         var t = e.activeStartDate,
             n = e.calendarType,
             r = e.showFixedNumberOfWeeks,
             a = e.showNeighboringMonth,
-            i = St(e, Mt),
+            i = St(e, kt),
             l = Object(s.getYear)(t),
             c = Object(s.getMonth)(t),
             u = r || a,
             f = x(t, n),
             p = u ? 0 : f,
             d = 1 + (u ? -f : 0),
             h = function() {
@@ -28948,26 +29447,26 @@
             start: d,
             tile: jt
         }))
     }
     At.propTypes = function(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? kt(Object(n), !0).forEach((function(t) {
+            t % 2 ? Mt(Object(n), !0).forEach((function(t) {
                 Pt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : kt(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Mt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }({
         calendarType: q.isRequired,
         showFixedNumberOfWeeks: l.a.bool,
         showNeighboringMonth: l.a.bool
-    }, G);
+    }, Q);
 
     function Ct(e) {
         for (var t = e.calendarType, n = e.formatShortWeekday, r = void 0 === n ? w : n, a = e.locale, i = e.onMouseLeave, l = new Date, c = Object(s.getMonthStart)(l), u = Object(s.getYear)(c), f = Object(s.getMonth)(c), p = [], d = 1; d <= 7; d += 1) {
             var h = new Date(u, f, d - x(c, t)),
                 m = E(a, h);
             p.push(o.a.createElement("div", {
                 key: d,
@@ -29201,17 +29700,17 @@
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }();
         return function() {
-            var n, r = Qt(e);
+            var n, r = Gt(e);
             if (t) {
-                var a = Qt(this).constructor;
+                var a = Gt(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return Kt(this, n)
         }
     }
 
     function Kt(e, t) {
@@ -29221,37 +29720,37 @@
     }
 
     function Yt(e) {
         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
     }
 
-    function Qt(e) {
-        return (Qt = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+    function Gt(e) {
+        return (Gt = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
 
-    function Gt(e, t) {
+    function Qt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
     function Jt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Gt(Object(n), !0).forEach((function(t) {
+            t % 2 ? Qt(Object(n), !0).forEach((function(t) {
                 Zt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Gt(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Qt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function Zt(e, t, n) {
@@ -29605,15 +30104,15 @@
                         s = l.maxDate,
                         f = l.minDate,
                         p = l.selectRange,
                         d = l.tileClassName,
                         h = l.tileContent,
                         m = l.tileDisabled,
                         b = this.hover,
-                        v = {
+                        y = {
                             activeStartDate: e ? C(i, t) : A(i, t),
                             hover: b,
                             locale: u,
                             maxDate: s,
                             minDate: f,
                             onClick: this.drillDownAvailable ? this.drillDown : this.onChange,
                             onMouseOver: p ? n : null,
@@ -29621,53 +30120,53 @@
                             tileContent: h,
                             tileDisabled: m,
                             value: a,
                             valueType: r
                         };
                     switch (i) {
                         case "century":
-                            var y = this.props.formatYear;
+                            var v = this.props.formatYear;
                             return o.a.createElement(Ue, Bt({
-                                formatYear: y
-                            }, v));
+                                formatYear: v
+                            }, y));
                         case "decade":
                             var g = this.props.formatYear;
                             return o.a.createElement(rt, Bt({
                                 formatYear: g
-                            }, v));
+                            }, y));
                         case "year":
                             var O = this.props,
                                 _ = O.formatMonth,
                                 w = O.formatMonthYear;
                             return o.a.createElement(bt, Bt({
                                 formatMonth: _,
                                 formatMonthYear: w
-                            }, v));
+                            }, y));
                         case "month":
                             var E = this.props,
                                 j = E.formatDay,
-                                M = E.formatLongDate,
-                                k = E.formatShortWeekday,
+                                k = E.formatLongDate,
+                                M = E.formatShortWeekday,
                                 P = E.onClickWeekNumber,
                                 x = E.showDoubleView,
                                 S = E.showFixedNumberOfWeeks,
                                 R = E.showNeighboringMonth,
                                 z = E.showWeekNumbers,
                                 D = this.onMouseLeave;
                             return o.a.createElement(Ht, Bt({
                                 calendarType: c,
                                 formatDay: j,
-                                formatLongDate: M,
-                                formatShortWeekday: k,
+                                formatLongDate: k,
+                                formatShortWeekday: M,
                                 onClickWeekNumber: P,
                                 onMouseLeave: p ? D : null,
                                 showFixedNumberOfWeeks: S || x,
                                 showNeighboringMonth: R,
                                 showWeekNumbers: z
-                            }, v));
+                            }, y));
                         default:
                             throw new Error("Invalid view: ".concat(i, "."))
                     }
                 }
             }, {
                 key: "renderNavigation",
                 value: function() {
@@ -29684,16 +30183,16 @@
                         s = r.navigationAriaLabel,
                         f = r.navigationAriaLive,
                         p = r.navigationLabel,
                         d = r.next2AriaLabel,
                         h = r.next2Label,
                         m = r.nextAriaLabel,
                         b = r.nextLabel,
-                        v = r.prev2AriaLabel,
-                        y = r.prev2Label,
+                        y = r.prev2AriaLabel,
+                        v = r.prev2Label,
                         g = r.prevAriaLabel,
                         O = r.prevLabel,
                         _ = r.showDoubleView;
                     return o.a.createElement(X, {
                         activeStartDate: e,
                         drillUp: this.drillUp,
                         formatMonthYear: a,
@@ -29704,16 +30203,16 @@
                         navigationAriaLabel: s,
                         navigationAriaLive: f,
                         navigationLabel: p,
                         next2AriaLabel: d,
                         next2Label: h,
                         nextAriaLabel: m,
                         nextLabel: b,
-                        prev2AriaLabel: v,
-                        prev2Label: y,
+                        prev2AriaLabel: y,
+                        prev2Label: v,
                         prevAriaLabel: g,
                         prevLabel: O,
                         setActiveStartDate: this.setActiveStartDate,
                         showDoubleView: _,
                         view: t,
                         views: n
                     })
@@ -29746,23 +30245,23 @@
         minDate: en,
         minDetail: "century",
         returnValue: "start",
         showNavigation: !0,
         showNeighboringMonth: !0
     };
     var bn = l.a.instanceOf(Date),
-        vn = l.a.oneOfType([l.a.string, K]);
+        yn = l.a.oneOfType([l.a.string, K]);
     mn.propTypes = {
         activeStartDate: bn,
         allowPartialRange: l.a.bool,
         calendarType: q,
         className: F,
         defaultActiveStartDate: bn,
-        defaultValue: vn,
-        defaultView: Q,
+        defaultValue: yn,
+        defaultView: G,
         formatDay: l.a.func,
         formatLongDate: l.a.func,
         formatMonth: l.a.func,
         formatMonthYear: l.a.func,
         formatShortWeekday: l.a.func,
         formatYear: l.a.func,
         inputRef: U,
@@ -29798,16 +30297,16 @@
         showFixedNumberOfWeeks: l.a.bool,
         showNavigation: l.a.bool,
         showNeighboringMonth: l.a.bool,
         showWeekNumbers: l.a.bool,
         tileClassName: l.a.oneOfType([l.a.func, F]),
         tileContent: l.a.oneOfType([l.a.func, l.a.node]),
         tileDisabled: l.a.func,
-        value: vn,
-        view: Q
+        value: yn,
+        view: G
     }, n.d(t, "Calendar", (function() {
         return mn
     })), n.d(t, "CenturyView", (function() {
         return Ue
     })), n.d(t, "DecadeView", (function() {
         return rt
     })), n.d(t, "YearView", (function() {
@@ -29855,15 +30354,15 @@
                 if (r < 0) return new Error("Invalid prop `".concat(t, "` of type `").concat(s(r), "` supplied to `").concat(n, "`, width must be greater or equal to 0."))
             }
             return null
         },
         m = p,
         b = h;
 
-    function v(e) {
+    function y(e) {
         var t = e.angle,
             n = void 0 === t ? 0 : t,
             r = e.name,
             o = e.length,
             i = void 0 === o ? 100 : o,
             l = e.oppositeLength,
             c = void 0 === l ? 10 : l,
@@ -29880,15 +30379,15 @@
                 width: "".concat(s, "px"),
                 top: "".concat(50 - i / 2, "%"),
                 bottom: "".concat(50 - c / 2, "%")
             }
         }))
     }
 
-    function y(e) {
+    function v(e) {
         var t = e.angle,
             n = void 0 === t ? 0 : t,
             r = e.length,
             o = void 0 === r ? 10 : r,
             i = e.name,
             l = e.width,
             c = void 0 === l ? 1 : l,
@@ -29929,17 +30428,17 @@
             b = void 0 === m ? 70 : m,
             g = e.minuteHandOppositeLength,
             O = e.minuteHandWidth,
             _ = void 0 === O ? 2 : O,
             w = e.minuteMarksLength,
             E = void 0 === w ? 6 : w,
             j = e.minuteMarksWidth,
-            M = void 0 === j ? 1 : j,
-            k = e.renderHourMarks,
-            P = void 0 === k || k,
+            k = void 0 === j ? 1 : j,
+            M = e.renderHourMarks,
+            P = void 0 === M || M,
             x = e.renderMinuteHand,
             S = void 0 === x || x,
             A = e.renderMinuteMarks,
             C = void 0 === A || A,
             R = e.renderNumbers,
             z = e.renderSecondHand,
             D = void 0 === z || z,
@@ -29958,68 +30457,68 @@
                 width: "".concat(q, "px"),
                 height: "".concat(q, "px")
             }
         }, a.a.createElement("div", {
             className: "react-clock__face"
         }, function() {
             if (!C) return null;
-            for (var e = [], t = 1; t <= 60; t += 1) P && !(t % 5) || e.push(a.a.createElement(y, {
+            for (var e = [], t = 1; t <= 60; t += 1) P && !(t % 5) || e.push(a.a.createElement(v, {
                 key: "minute_".concat(t),
                 angle: 6 * t,
                 length: E,
                 name: "minute",
-                width: M
+                width: k
             }));
             return e
         }(), function() {
             if (!P) return null;
-            for (var e = [], t = 1; t <= 12; t += 1) e.push(a.a.createElement(y, {
+            for (var e = [], t = 1; t <= 12; t += 1) e.push(a.a.createElement(v, {
                 key: "hour_".concat(t),
                 angle: 30 * t,
                 length: p,
                 name: "hour",
                 number: R ? t : null,
                 width: h
             }));
             return e
-        }()), (t = F ? 30 * Object(c.getHours)(F) + Object(c.getMinutes)(F) / 2 + Object(c.getSeconds)(F) / 600 : 0, a.a.createElement(v, {
+        }()), (t = F ? 30 * Object(c.getHours)(F) + Object(c.getMinutes)(F) / 2 + Object(c.getSeconds)(F) / 600 : 0, a.a.createElement(y, {
             angle: t,
             length: o,
             name: "hour",
             oppositeLength: i,
             width: s
         })), function() {
             if (!S) return null;
             var e = F ? 360 * Object(c.getHours)(F) + 6 * Object(c.getMinutes)(F) + Object(c.getSeconds)(F) / 10 : 0;
-            return a.a.createElement(v, {
+            return a.a.createElement(y, {
                 angle: e,
                 length: b,
                 name: "minute",
                 oppositeLength: g,
                 width: _
             })
         }(), function() {
             if (!D) return null;
             var e = F ? 360 * Object(c.getMinutes)(F) + 6 * Object(c.getSeconds)(F) : 0;
-            return a.a.createElement(v, {
+            return a.a.createElement(y, {
                 angle: e,
                 length: N,
                 name: "second",
                 oppositeLength: I,
                 width: L
             })
         }())
     }
-    v.propTypes = {
+    y.propTypes = {
         angle: i.a.number,
         length: p,
         name: i.a.string.isRequired,
         oppositeLength: p,
         width: i.a.number
-    }, y.propTypes = {
+    }, v.propTypes = {
         angle: i.a.number,
         length: m,
         name: i.a.string.isRequired,
         number: i.a.number,
         width: b
     }, g.propTypes = {
         className: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string)]),
@@ -30124,25 +30623,25 @@
         }();
         return function() {
             var n, r = g(e);
             if (t) {
                 var a = g(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
-            return v(this, n)
+            return y(this, n)
         }
     }
 
-    function v(e, t) {
+    function y(e, t) {
         if (t && ("object" === j(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-        return y(e)
+        return v(e)
     }
 
-    function y(e) {
+    function v(e) {
         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
     }
 
     function g(e) {
         return (g = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
@@ -30200,17 +30699,17 @@
     function j(e) {
         return (j = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
-    var M = "undefined" != typeof window,
-        k = M && "CSS" in window && "supports" in window.CSS && CSS.supports("display", "contents"),
-        P = M && "MutationObserver" in window;
+    var k = "undefined" != typeof window,
+        M = k && "CSS" in window && "supports" in window.CSS && CSS.supports("display", "contents"),
+        P = k && "MutationObserver" in window;
 
     function x(e) {
         return e[0].toUpperCase() + e.slice(1)
     }
 
     function S(e) {
         if (e) {
@@ -30235,27 +30734,27 @@
             c = window.getComputedStyle(r),
             s = n.parentElement,
             p = u(s, i),
             d = u(s, document.documentElement),
             h = "x" === t,
             m = h ? "left" : "top",
             b = h ? "right" : "bottom",
-            v = h ? "width" : "height",
-            y = "overflow".concat(x(m)),
+            y = h ? "width" : "height",
+            v = "overflow".concat(x(m)),
             g = "overflow".concat(x(b)),
             O = "scroll".concat(x(m)),
-            _ = x(v),
+            _ = x(y),
             w = "offset".concat(_),
             E = "client".concat(_),
-            M = "min-".concat(v),
-            k = i[w] - i[E],
+            k = "min-".concat(y),
+            M = i[w] - i[E],
             P = "object" === j(l) ? l[m] : l,
-            S = -Math.max(p[y], d[y] + document.documentElement[O]) - P,
+            S = -Math.max(p[v], d[v] + document.documentElement[O]) - P,
             A = "object" === j(l) ? l[b] : l,
-            C = -Math.max(p[g], d[g] - document.documentElement[O]) - A - k;
+            C = -Math.max(p[g], d[g] - document.documentElement[O]) - A - M;
         o && (S += s[E], C += s[E]);
         var R = r[w];
 
         function z() {
             r.style[m] = "auto", r.style[b] = o ? "0" : "100%"
         }
 
@@ -30272,20 +30771,20 @@
             return T(S, z)
         }
 
         function I() {
             return T(C, D)
         }(a ? N() || I() : I() || N()) || function() {
             var e = S > C,
-                t = c[M] && parseInt(c[M], 10);
+                t = c[k] && parseInt(c[k], 10);
 
             function n(e) {
-                t && e < t && f("<Fit />'s child will not fit anywhere with its current ".concat(M, " of ").concat(t, "px."));
+                t && e < t && f("<Fit />'s child will not fit anywhere with its current ".concat(k, " of ").concat(t, "px."));
                 var n = Math.max(e, t || 0);
-                f("<Fit />'s child needed to have its ".concat(v, " decreased to ").concat(n, "px.")), r.style[v] = "".concat(n, "px")
+                f("<Fit />'s child needed to have its ".concat(y, " decreased to ").concat(n, "px.")), r.style[y] = "".concat(n, "px")
             }
             e ? (n(S), z()) : (n(C), D())
         }()
     }
 
     function C(e) {
         var t = e.invertAxis,
@@ -30318,18 +30817,18 @@
         }(l, e);
         var t, n, r, i = b(l);
 
         function l() {
             var e;
             d(this, l);
             for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
-            return E(y(e = i.call.apply(i, [this].concat(n))), "onMutation", (function() {
+            return E(v(e = i.call.apply(i, [this].concat(n))), "onMutation", (function() {
                 e.fit()
-            })), E(y(e), "mutationObserver", P && new MutationObserver(e.onMutation)), E(y(e), "fit", (function() {
-                var t = y(e),
+            })), E(v(e), "mutationObserver", P && new MutationObserver(e.onMutation)), E(v(e), "fit", (function() {
+                var t = v(e),
                     n = t.scrollContainer,
                     r = t.container,
                     a = t.element;
                 if (a) {
                     var o = a.clientWidth,
                         i = a.clientHeight;
                     if (e.elementWidth !== o || e.elementHeight !== i) {
@@ -30353,30 +30852,30 @@
                     }
                 }
             })), e
         }
         return t = l, (n = [{
             key: "componentDidMount",
             value: function() {
-                if (!k) {
+                if (!M) {
                     var e = Object(o.findDOMNode)(this);
                     this.container = e, this.element = e, this.scrollContainer = S(e)
                 }
                 this.fit(), P && this.mutationObserver.observe(this.element, {
                     attributes: !0,
                     attributeFilter: ["class", "style"]
                 })
             }
         }, {
             key: "render",
             value: function() {
                 var e = this,
                     t = this.props.children,
                     n = a.a.Children.only(t);
-                return k ? a.a.createElement("span", {
+                return M ? a.a.createElement("span", {
                     ref: function(t) {
                         e.container = t;
                         var n = t && t.firstChild;
                         e.element = n, e.scrollContainer = S(n)
                     },
                     style: {
                         display: "contents"
```

### Comparing `dash_express_components-0.0.98/dash_express_components/metadata.json` & `dash_express_components-0.0.99/dash_express_components/metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743589743589743%*

 * *Differences: {"'src/lib/components/DataGraph.react.js'": "OrderedDict([('description', ''), ('displayName', "*

 * *                                            "'DataGraph'), ('methods', [OrderedDict([('name', "*

 * *                                            "'handleGraphSetProps'), ('docblock', None), "*

 * *                                            "('modifiers', []), ('params', [OrderedDict([('name', "*

 * *                                            "'updatedProps'), ('type', None)])]), ('returns', "*

 * *                                 […]*

```diff
@@ -217,14 +217,134 @@
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             }
         }
     },
+    "src/lib/components/DataGraph.react.js": {
+        "description": "",
+        "displayName": "DataGraph",
+        "methods": [
+            {
+                "docblock": null,
+                "modifiers": [],
+                "name": "handleGraphSetProps",
+                "params": [
+                    {
+                        "name": "updatedProps",
+                        "type": null
+                    }
+                ],
+                "returns": null
+            },
+            {
+                "docblock": null,
+                "modifiers": [],
+                "name": "getDefaultDefParams",
+                "params": [
+                    {
+                        "name": "data",
+                        "type": null
+                    }
+                ],
+                "returns": null
+            },
+            {
+                "docblock": null,
+                "modifiers": [],
+                "name": "getMeta",
+                "params": [
+                    {
+                        "name": "data",
+                        "type": null
+                    }
+                ],
+                "returns": null
+            },
+            {
+                "docblock": null,
+                "modifiers": [],
+                "name": "getFigure",
+                "params": [
+                    {
+                        "name": "defParams",
+                        "type": null
+                    },
+                    {
+                        "name": "data",
+                        "type": null
+                    }
+                ],
+                "returns": null
+            },
+            {
+                "docblock": null,
+                "modifiers": [],
+                "name": "groupData",
+                "params": [
+                    {
+                        "name": "data",
+                        "type": null
+                    },
+                    {
+                        "name": "params",
+                        "type": null
+                    }
+                ],
+                "returns": null
+            },
+            {
+                "docblock": null,
+                "modifiers": [],
+                "name": "isNumerical",
+                "params": [
+                    {
+                        "name": "column",
+                        "type": null
+                    }
+                ],
+                "returns": null
+            }
+        ],
+        "props": {
+            "data": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "{}"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "defParams": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "id": {
+                "description": "",
+                "required": true,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "setProps": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "func"
+                }
+            }
+        }
+    },
     "src/lib/components/Filter.react.js": {
         "description": "<div style=\"width:450px; margin-left: 20px; float: right;  margin-top: -150px;\">\n<img src=\"https://raw.githubusercontent.com/VK/dash-express-components/main/.media/filter.png\"/>\n<img src=\"https://raw.githubusercontent.com/VK/dash-express-components/main/.media/filter-modal.png\"/>\n</div>\n\n\nThe filter component allows filters to be set on individual columns.\n\nThese are all combined with and.\n\nThere are the options like >, <, = for numerical, as well as isin etc. for categorical columns.\nPossible options are given by the `meta` props.\n\n\n@hideconstructor\n\n@example\nimport dash_express_components as dxc\nimport plotly.express as px\n\nmeta = dxc.get_meta(px.data.gapminder())\n\ndxc.Filter(\n  id=\"filter\",\n  meta=meta\n)\n@public",
         "displayName": "Filter",
         "methods": [
             {
                 "docblock": null,
                 "modifiers": [],
```

### Comparing `dash_express_components-0.0.98/dash_express_components/package-info.json` & `dash_express_components-0.0.99/dash_express_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.99'"}*

```diff
@@ -59,9 +59,9 @@
         "build:patch": "python _patch.py",
         "doc": "jsdoc -c ./jsdoc.conf.json -a public",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "test": "pytest --cov=dash_express_components tests --cov-report term-missing",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.98"
+    "version": "0.0.99"
 }
```

### Comparing `dash_express_components-0.0.98/dash_express_components/plottypes/_bar_count.py` & `dash_express_components-0.0.99/dash_express_components/plottypes/_bar_count.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/plottypes/_box.py` & `dash_express_components-0.0.99/dash_express_components/plottypes/_box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/plottypes/_histogram_line.py` & `dash_express_components-0.0.99/dash_express_components/plottypes/_histogram_line.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/plottypes/_imshow.py` & `dash_express_components-0.0.99/dash_express_components/plottypes/_imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/plottypes/_probability.py` & `dash_express_components-0.0.99/dash_express_components/plottypes/_probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/plottypes/_scatter.py` & `dash_express_components-0.0.99/dash_express_components/plottypes/_scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/transformationtypes/_aggr.py` & `dash_express_components-0.0.99/dash_express_components/transformationtypes/_aggr.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/transformationtypes/_bin.py` & `dash_express_components-0.0.99/dash_express_components/transformationtypes/_bin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/transformationtypes/_eval.py` & `dash_express_components-0.0.99/dash_express_components/transformationtypes/_eval.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/transformationtypes/_groupby_sample.py` & `dash_express_components-0.0.99/dash_express_components/transformationtypes/_groupby_sample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/transformationtypes/_iqrfilter.py` & `dash_express_components-0.0.99/dash_express_components/transformationtypes/_iqrfilter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/transformationtypes/_strsplit.py` & `dash_express_components-0.0.99/dash_express_components/transformationtypes/_strsplit.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/transformationtypes/_wide_to_long.py` & `dash_express_components-0.0.99/dash_express_components/transformationtypes/_wide_to_long.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components/utils.py` & `dash_express_components-0.0.99/dash_express_components/utils.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components.egg-info/PKG-INFO` & `dash_express_components-0.0.99/dash_express_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-express-components
-Version: 0.0.98
+Version: 0.0.99
 Summary: Simple widgets to add plotly express style plotting to dash
 Home-page: https://github.com/VK/dash-express-components
 Author: Viktor Krückl <viktor@krueckl.de>
 License: MIT
 Description: # Dash Express Components
         ![Publish release](https://github.com/VK/dash-express-components/workflows/Publish%20release/badge.svg)
         [![PyPI](https://img.shields.io/pypi/v/dash-express-components?logo=pypi)](https://pypi.org/project/dash-express-components)
```

### Comparing `dash_express_components-0.0.98/dash_express_components.egg-info/SOURCES.txt` & `dash_express_components-0.0.99/dash_express_components.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 dash_express_components/BinTransform.py
 dash_express_components/Box.py
 dash_express_components/CategoryLookup.py
 dash_express_components/CombinecatTransform.py
 dash_express_components/ConfigReceiver.py
 dash_express_components/Configurator.py
 dash_express_components/CoreGraph.py
+dash_express_components/DataGraph.py
 dash_express_components/DropnaTransform.py
 dash_express_components/EvalTransform.py
 dash_express_components/Filter.py
 dash_express_components/FilterIqrTransform.py
 dash_express_components/Graph.py
 dash_express_components/GroupedSample.py
 dash_express_components/HistogramLine.py
```

### Comparing `dash_express_components-0.0.98/dash_express_components_base/__init__.py` & `dash_express_components-0.0.99/dash_express_components_base/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/plottypes/_bar_count.py` & `dash_express_components-0.0.99/dash_express_components_base/plottypes/_bar_count.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/plottypes/_box.py` & `dash_express_components-0.0.99/dash_express_components_base/plottypes/_box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/plottypes/_histogram_line.py` & `dash_express_components-0.0.99/dash_express_components_base/plottypes/_histogram_line.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/plottypes/_imshow.py` & `dash_express_components-0.0.99/dash_express_components_base/plottypes/_imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/plottypes/_probability.py` & `dash_express_components-0.0.99/dash_express_components_base/plottypes/_probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/plottypes/_scatter.py` & `dash_express_components-0.0.99/dash_express_components_base/plottypes/_scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_aggr.py` & `dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_aggr.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_bin.py` & `dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_bin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_eval.py` & `dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_eval.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_groupby_sample.py` & `dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_groupby_sample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_iqrfilter.py` & `dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_iqrfilter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_strsplit.py` & `dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_strsplit.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_wide_to_long.py` & `dash_express_components-0.0.99/dash_express_components_base/transformationtypes/_wide_to_long.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/dash_express_components_base/utils.py` & `dash_express_components-0.0.99/dash_express_components_base/utils.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.98/package.json` & `dash_express_components-0.0.99/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.99'"}*

```diff
@@ -59,9 +59,9 @@
         "build:patch": "python _patch.py",
         "doc": "jsdoc -c ./jsdoc.conf.json -a public",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "test": "pytest --cov=dash_express_components tests --cov-report term-missing",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.98"
+    "version": "0.0.99"
 }
```

### Comparing `dash_express_components-0.0.98/setup.py` & `dash_express_components-0.0.99/setup.py`

 * *Files identical despite different names*

