# Comparing `tmp/neura_library-0.0.6.tar.gz` & `tmp/neura_library-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neura_library-0.0.6.tar", last modified: Sun May 26 11:56:37 2024, max compression
+gzip compressed data, was "neura_library-0.0.7.tar", last modified: Sat Jun  1 20:53:24 2024, max compression
```

## Comparing `neura_library-0.0.6.tar` & `neura_library-0.0.7.tar`

### file list

```diff
@@ -1,188 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-26 11:56:33.000000 neura_library-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-26 11:56:37.762143 neura_library-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-26 11:56:33.000000 neura_library-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-26 11:56:33.000000 neura_library-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-26 11:56:33.000000 neura_library-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:56:37.762143 neura_library-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.734143 neura_library-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/src/neura_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 11:56:37.000000 neura_library-0.0.6/src/neura_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.738143 neura_library-0.0.6/src/neuralib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.742143 neura_library-0.0.6/src/neuralib/argp/
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/argp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/argp/_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/argp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/argp/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.742143 neura_library-0.0.6/src/neuralib/atlas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.742143 neura_library-0.0.6/src/neuralib/atlas/brainrender/
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/main_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/probe_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/roi_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/brainrender/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.742143 neura_library-0.0.6/src/neuralib/atlas/ccf/
--rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ccf/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/atlas/cellatlas/
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/cellatlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/cellatlas/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/atlas/ibl/
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ibl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/ibl/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    55607 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/atlas/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/bokeh_model/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/example_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/bokeh_model/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_animal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_figure.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/bokeh_model/view_brain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/calimg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/calimg/scan_image/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scan_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scan_image/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.746143 neura_library-0.0.6/src/neuralib/calimg/scanbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scanbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scanbox/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/scanbox/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/calimg/suite2p/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/suite2p/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/suite2p/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/calimg/suite2p/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/imglib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/labeller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/imglib/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/model/bayes_decoding/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/model/bayes_decoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/model/bayes_decoding/position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/persistence/cli_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/persistence/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.750143 neura_library-0.0.6/src/neuralib/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/colormap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/plot/venn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.754143 neura_library-0.0.6/src/neuralib/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/scanner/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/scanner/czi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/scanner/lsm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.754143 neura_library-0.0.6/src/neuralib/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.754143 neura_library-0.0.6/src/neuralib/segmentation/cellpose/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/cellpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/cellpose/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/cellpose/run_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/cellpose/run_subproc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.754143 neura_library-0.0.6/src/neuralib/segmentation/stardist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/stardist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/segmentation/stardist/run_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/stimpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/baselog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/baseprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/camlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/math_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/protocol_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/stimpy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    24923 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/stimpy_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/stimpy_pyv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/stimulus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/stimpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/tools/pkl_parq_view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/pkl_parq_view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/pkl_parq_view/main_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/tools/slack_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/slack_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/tools/slack_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/color_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/profile_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/segement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/util_clazz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/util_cv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/util_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/util_verbose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.758143 neura_library-0.0.6/src/neuralib/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/src/neuralib/wrapper/facemap/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/facemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/facemap/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/facemap/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/src/neuralib/wrapper/rastermap/
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-26 11:56:33.000000 neura_library-0.0.6/src/neuralib/wrapper/rastermap/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:56:37.762143 neura_library-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_argp.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_argp_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_csv_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_persistence_autoinc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_protocol_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_pyvstim_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    62204 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_stimpy_bitbucket_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_stimpy_github_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-26 11:56:33.000000 neura_library-0.0.6/test/test_util_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.943242 neura_library-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-06-01 20:53:20.000000 neura_library-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-06-01 20:53:24.943242 neura_library-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-06-01 20:53:20.000000 neura_library-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-06-01 20:53:20.000000 neura_library-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-01 20:53:20.000000 neura_library-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:53:24.943242 neura_library-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.911242 neura_library-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.943242 neura_library-0.0.7/src/neura_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-06-01 20:53:24.000000 neura_library-0.0.7/src/neura_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-01 20:53:24.000000 neura_library-0.0.7/src/neura_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:53:24.000000 neura_library-0.0.7/src/neura_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-01 20:53:24.000000 neura_library-0.0.7/src/neura_library.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-01 20:53:24.000000 neura_library-0.0.7/src/neura_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 20:53:24.000000 neura_library-0.0.7/src/neura_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.919242 neura_library-0.0.7/src/neuralib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.919242 neura_library-0.0.7/src/neuralib/argp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/argp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/argp/_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/argp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/argp/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.919242 neura_library-0.0.7/src/neuralib/atlas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.919242 neura_library-0.0.7/src/neuralib/atlas/brainrender/
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/brainrender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/brainrender/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/brainrender/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/brainrender/main_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/brainrender/probe_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/brainrender/roi_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/brainrender/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.923242 neura_library-0.0.7/src/neuralib/atlas/ccf/
+-rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/ccf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/ccf/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/ccf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/ccf/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/ccf/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.923242 neura_library-0.0.7/src/neuralib/atlas/cellatlas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/cellatlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/cellatlas/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.923242 neura_library-0.0.7/src/neuralib/atlas/ibl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/ibl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/ibl/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55607 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/atlas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.923242 neura_library-0.0.7/src/neuralib/bokeh_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/example_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.923242 neura_library-0.0.7/src/neuralib/bokeh_model/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/examples/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/examples/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/examples/view_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/examples/view_animal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/examples/view_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/bokeh_model/view_brain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.923242 neura_library-0.0.7/src/neuralib/calimg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.923242 neura_library-0.0.7/src/neuralib/calimg/scan_image/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/scan_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/scan_image/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.923242 neura_library-0.0.7/src/neuralib/calimg/scanbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/scanbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/scanbox/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/scanbox/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.927242 neura_library-0.0.7/src/neuralib/calimg/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/suite2p/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/suite2p/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/calimg/suite2p/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.927242 neura_library-0.0.7/src/neuralib/imglib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/imglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/imglib/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/imglib/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/imglib/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/imglib/labeller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/imglib/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/imglib/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.927242 neura_library-0.0.7/src/neuralib/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.927242 neura_library-0.0.7/src/neuralib/model/bayes_decoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/model/bayes_decoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/model/bayes_decoding/position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.927242 neura_library-0.0.7/src/neuralib/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/persistence/cli_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/persistence/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.927242 neura_library-0.0.7/src/neuralib/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/plot/venn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.931242 neura_library-0.0.7/src/neuralib/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/scanner/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/scanner/czi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/scanner/lsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.931242 neura_library-0.0.7/src/neuralib/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/segmentation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.931242 neura_library-0.0.7/src/neuralib/segmentation/cellpose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/segmentation/cellpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/segmentation/cellpose/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/segmentation/cellpose/run_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/segmentation/cellpose/run_subproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.931242 neura_library-0.0.7/src/neuralib/segmentation/stardist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/segmentation/stardist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/segmentation/stardist/run_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.931242 neura_library-0.0.7/src/neuralib/sqlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.935242 neura_library-0.0.7/src/neuralib/sqlp/dot/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/dot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/dot/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24625 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/func_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/func_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/func_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/func_win.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30923 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/table_nt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/sqlp/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.935242 neura_library-0.0.7/src/neuralib/stimpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/baselog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/baseprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/camlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/math_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/protocol_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/stimpy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24949 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/stimpy_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/stimpy_pyv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/stimulus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/stimpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.935242 neura_library-0.0.7/src/neuralib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.935242 neura_library-0.0.7/src/neuralib/tools/pkl_parq_view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/tools/pkl_parq_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/tools/pkl_parq_view/main_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.935242 neura_library-0.0.7/src/neuralib/tools/slack_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/tools/slack_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/tools/slack_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.939242 neura_library-0.0.7/src/neuralib/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/color_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/segement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/util_clazz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/util_cv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/util_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/util_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.939242 neura_library-0.0.7/src/neuralib/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.939242 neura_library-0.0.7/src/neuralib/wrapper/deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/deeplabcut/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/deeplabcut/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.939242 neura_library-0.0.7/src/neuralib/wrapper/facemap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/facemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/facemap/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/facemap/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.939242 neura_library-0.0.7/src/neuralib/wrapper/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-06-01 20:53:20.000000 neura_library-0.0.7/src/neuralib/wrapper/rastermap/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:53:24.943242 neura_library-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-06-01 20:53:20.000000 neura_library-0.0.7/test/test_csv_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-06-01 20:53:20.000000 neura_library-0.0.7/test/test_persistence_autoinc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-06-01 20:53:20.000000 neura_library-0.0.7/test/test_protocol_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-06-01 20:53:20.000000 neura_library-0.0.7/test/test_pyvstim_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62204 2024-06-01 20:53:20.000000 neura_library-0.0.7/test/test_stimpy_bitbucket_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-06-01 20:53:20.000000 neura_library-0.0.7/test/test_stimpy_github_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-06-01 20:53:20.000000 neura_library-0.0.7/test/test_util_func.py
```

### Comparing `neura_library-0.0.6/LICENSE` & `neura_library-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/PKG-INFO` & `neura_library-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neura-library
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utility tools for system neuroscience research, including Open Source Wrapper or Parser
 Author-email: Yu-Ting Wei <ytsimon2004@gmail.com>, Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, YT.WEI
         
         Redistribution and use in source and binary forms, with or without
@@ -54,15 +54,15 @@
 Requires-Dist: scipy>=1.12
 Requires-Dist: scikit-image
 Requires-Dist: pandas~=1.5.0
 Requires-Dist: polars>=0.20.9
 Requires-Dist: pyarrow
 Requires-Dist: tifffile==2023.4.12
 Requires-Dist: opencv-python~=4.8.0.76
-Requires-Dist: tqdm~=4.62.3
+Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: typing_extensions
 
 
 # neuralib
```

### Comparing `neura_library-0.0.6/README.md` & `neura_library-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/pyproject.toml` & `neura_library-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neura-library"
-version = "0.0.6"
+version = "0.0.7"
 requires-python = ">=3.9"
 description = "Utility tools for system neuroscience research, including Open Source Wrapper or Parser"
 authors = [
     { name = "Yu-Ting Wei", email = "ytsimon2004@gmail.com" },
     { name = "Ta-Shun Su", email = "antoniost29@gmail.com" }
 ]
 license = { file = "LICENSE" }
```

### Comparing `neura_library-0.0.6/src/neura_library.egg-info/PKG-INFO` & `neura_library-0.0.7/src/neura_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neura-library
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utility tools for system neuroscience research, including Open Source Wrapper or Parser
 Author-email: Yu-Ting Wei <ytsimon2004@gmail.com>, Ta-Shun Su <antoniost29@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, YT.WEI
         
         Redistribution and use in source and binary forms, with or without
@@ -54,15 +54,15 @@
 Requires-Dist: scipy>=1.12
 Requires-Dist: scikit-image
 Requires-Dist: pandas~=1.5.0
 Requires-Dist: polars>=0.20.9
 Requires-Dist: pyarrow
 Requires-Dist: tifffile==2023.4.12
 Requires-Dist: opencv-python~=4.8.0.76
-Requires-Dist: tqdm~=4.62.3
+Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: typing_extensions
 
 
 # neuralib
```

### Comparing `neura_library-0.0.6/src/neura_library.egg-info/SOURCES.txt` & `neura_library-0.0.7/src/neura_library.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -90,14 +90,30 @@
 src/neuralib/segmentation/base.py
 src/neuralib/segmentation/cellpose/__init__.py
 src/neuralib/segmentation/cellpose/core.py
 src/neuralib/segmentation/cellpose/run_api.py
 src/neuralib/segmentation/cellpose/run_subproc.py
 src/neuralib/segmentation/stardist/__init__.py
 src/neuralib/segmentation/stardist/run_2d.py
+src/neuralib/sqlp/__init__.py
+src/neuralib/sqlp/cli.py
+src/neuralib/sqlp/connection.py
+src/neuralib/sqlp/expr.py
+src/neuralib/sqlp/func.py
+src/neuralib/sqlp/func_date.py
+src/neuralib/sqlp/func_dec.py
+src/neuralib/sqlp/func_stat.py
+src/neuralib/sqlp/func_win.py
+src/neuralib/sqlp/literal.py
+src/neuralib/sqlp/stat.py
+src/neuralib/sqlp/table.py
+src/neuralib/sqlp/table_nt.py
+src/neuralib/sqlp/util.py
+src/neuralib/sqlp/dot/__init__.py
+src/neuralib/sqlp/dot/core.py
 src/neuralib/stimpy/__init__.py
 src/neuralib/stimpy/baselog.py
 src/neuralib/stimpy/baseprot.py
 src/neuralib/stimpy/camlog.py
 src/neuralib/stimpy/event.py
 src/neuralib/stimpy/math_eval.py
 src/neuralib/stimpy/preference.py
@@ -136,16 +152,14 @@
 src/neuralib/wrapper/deeplabcut/core.py
 src/neuralib/wrapper/deeplabcut/util.py
 src/neuralib/wrapper/facemap/__init__.py
 src/neuralib/wrapper/facemap/core.py
 src/neuralib/wrapper/facemap/plot.py
 src/neuralib/wrapper/rastermap/__init__.py
 src/neuralib/wrapper/rastermap/core.py
-test/test_argp.py
-test/test_argp_dispatch.py
 test/test_csv_context_manager.py
 test/test_persistence_autoinc.py
 test/test_protocol_parser.py
 test/test_pyvstim_parser.py
 test/test_stimpy_bitbucket_parser.py
 test/test_stimpy_github_parser.py
 test/test_util_func.py
```

### Comparing `neura_library-0.0.6/src/neuralib/argp/__init__.py` & `neura_library-0.0.7/src/neuralib/argp/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/argp/_type.py` & `neura_library-0.0.7/src/neuralib/argp/_type.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/argp/core.py` & `neura_library-0.0.7/src/neuralib/argp/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/argp/dispatch.py` & `neura_library-0.0.7/src/neuralib/argp/dispatch.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/_structure.py` & `neura_library-0.0.7/src/neuralib/atlas/_structure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/brainrender/__init__.py` & `neura_library-0.0.7/src/neuralib/atlas/brainrender/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/brainrender/core.py` & `neura_library-0.0.7/src/neuralib/atlas/brainrender/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/brainrender/main_app.py` & `neura_library-0.0.7/src/neuralib/atlas/brainrender/main_app.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/brainrender/probe_rst.py` & `neura_library-0.0.7/src/neuralib/atlas/brainrender/probe_rst.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/brainrender/roi_rst.py` & `neura_library-0.0.7/src/neuralib/atlas/brainrender/roi_rst.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/brainrender/util.py` & `neura_library-0.0.7/src/neuralib/atlas/brainrender/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/ccf/__init__.py` & `neura_library-0.0.7/src/neuralib/atlas/ccf/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/ccf/classifier.py` & `neura_library-0.0.7/src/neuralib/atlas/ccf/classifier.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/ccf/core.py` & `neura_library-0.0.7/src/neuralib/atlas/ccf/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/ccf/norm.py` & `neura_library-0.0.7/src/neuralib/atlas/ccf/norm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/ccf/query.py` & `neura_library-0.0.7/src/neuralib/atlas/ccf/query.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/cellatlas/__init__.py` & `neura_library-0.0.7/src/neuralib/atlas/cellatlas/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/cellatlas/core.py` & `neura_library-0.0.7/src/neuralib/atlas/cellatlas/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/data.py` & `neura_library-0.0.7/src/neuralib/atlas/data.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/ibl/__init__.py` & `neura_library-0.0.7/src/neuralib/atlas/ibl/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/ibl/plot.py` & `neura_library-0.0.7/src/neuralib/atlas/ibl/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/map.py` & `neura_library-0.0.7/src/neuralib/atlas/map.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/plot.py` & `neura_library-0.0.7/src/neuralib/atlas/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/util.py` & `neura_library-0.0.7/src/neuralib/atlas/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/atlas/view.py` & `neura_library-0.0.7/src/neuralib/atlas/view.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/base.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/base.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/example.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/example.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/example_multi.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/example_multi.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_all.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/examples/view_all.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_animal.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/examples/view_animal.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/examples/view_figure.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/examples/view_figure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/tool.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/tool.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/util.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/bokeh_model/view_brain.py` & `neura_library-0.0.7/src/neuralib/bokeh_model/view_brain.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/calimg/scan_image/wrapper.py` & `neura_library-0.0.7/src/neuralib/calimg/scan_image/wrapper.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/calimg/scanbox/__init__.py` & `neura_library-0.0.7/src/neuralib/calimg/scanbox/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -59,25 +59,25 @@
 
 
 Use CLI
 ------------
 
 See help::
 
-    python */scanbox/viewer.py -h
+    python -m neuralib.calimg.scanbox.viewer -h
 
 
-Example playing the 100-200 Frames::
+Example playing the 100-200 frames::
 
-    python */scanbox/viewer.py -D <DIR> -P <OPTIC_PLANE> -C <PMT_CHANNEL> -F 100,200
+    python -m neuralib.calimg.scanbox.viewer -D <DIR> -P <OPTIC_PLANE> -C <PMT_CHANNEL> -F 100,200
 
 
 Example save 100-200 Frames as tiff::
 
-    python */scanbox/viewer.py -D <DIR> -P <OPTIC_PLANE> -C <PMT_CHANNEL> -F 100,200 -O test.tiff
+    python -m neuralib.calimg.scanbox.viewer -D <DIR> -P <OPTIC_PLANE> -C <PMT_CHANNEL> -F 100,200 -O test.tiff
 
 
 
 Use API call
 --------------
 
 .. code-block:: python
```

### Comparing `neura_library-0.0.6/src/neuralib/calimg/scanbox/core.py` & `neura_library-0.0.7/src/neuralib/calimg/scanbox/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/calimg/scanbox/viewer.py` & `neura_library-0.0.7/src/neuralib/calimg/scanbox/viewer.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/calimg/suite2p/__init__.py` & `neura_library-0.0.7/src/neuralib/calimg/suite2p/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/calimg/suite2p/core.py` & `neura_library-0.0.7/src/neuralib/calimg/suite2p/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/calimg/suite2p/plot.py` & `neura_library-0.0.7/src/neuralib/calimg/suite2p/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/calimg/suite2p/signals.py` & `neura_library-0.0.7/src/neuralib/calimg/suite2p/signals.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/imglib/color.py` & `neura_library-0.0.7/src/neuralib/imglib/color.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/imglib/factory.py` & `neura_library-0.0.7/src/neuralib/imglib/factory.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/imglib/io.py` & `neura_library-0.0.7/src/neuralib/imglib/io.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/imglib/labeller.py` & `neura_library-0.0.7/src/neuralib/imglib/labeller.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/imglib/norm.py` & `neura_library-0.0.7/src/neuralib/imglib/norm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/imglib/transform.py` & `neura_library-0.0.7/src/neuralib/imglib/transform.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/model/bayes_decoding/position.py` & `neura_library-0.0.7/src/neuralib/model/bayes_decoding/position.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/persistence/cli_persistence.py` & `neura_library-0.0.7/src/neuralib/persistence/cli_persistence.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/persistence/persistence.py` & `neura_library-0.0.7/src/neuralib/persistence/persistence.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/plot/animation.py` & `neura_library-0.0.7/src/neuralib/plot/animation.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/plot/colormap.py` & `neura_library-0.0.7/src/neuralib/plot/colormap.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/plot/figure.py` & `neura_library-0.0.7/src/neuralib/plot/figure.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/plot/misc.py` & `neura_library-0.0.7/src/neuralib/plot/misc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/plot/plot.py` & `neura_library-0.0.7/src/neuralib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/plot/setting.py` & `neura_library-0.0.7/src/neuralib/plot/setting.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/plot/tools.py` & `neura_library-0.0.7/src/neuralib/plot/tools.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/plot/venn.py` & `neura_library-0.0.7/src/neuralib/plot/venn.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/scanner/__init__.py` & `neura_library-0.0.7/src/neuralib/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/scanner/core.py` & `neura_library-0.0.7/src/neuralib/scanner/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/scanner/czi.py` & `neura_library-0.0.7/src/neuralib/scanner/czi.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/scanner/lsm.py` & `neura_library-0.0.7/src/neuralib/scanner/lsm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/segmentation/base.py` & `neura_library-0.0.7/src/neuralib/segmentation/base.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/segmentation/cellpose/core.py` & `neura_library-0.0.7/src/neuralib/segmentation/cellpose/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/segmentation/cellpose/run_api.py` & `neura_library-0.0.7/src/neuralib/segmentation/cellpose/run_api.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/segmentation/cellpose/run_subproc.py` & `neura_library-0.0.7/src/neuralib/segmentation/cellpose/run_subproc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/segmentation/stardist/run_2d.py` & `neura_library-0.0.7/src/neuralib/segmentation/stardist/run_2d.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/__init__.py` & `neura_library-0.0.7/src/neuralib/stimpy/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/baselog.py` & `neura_library-0.0.7/src/neuralib/stimpy/baselog.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/baseprot.py` & `neura_library-0.0.7/src/neuralib/stimpy/baseprot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/camlog.py` & `neura_library-0.0.7/src/neuralib/stimpy/camlog.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/event.py` & `neura_library-0.0.7/src/neuralib/stimpy/event.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/math_eval.py` & `neura_library-0.0.7/src/neuralib/stimpy/math_eval.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/preference.py` & `neura_library-0.0.7/src/neuralib/stimpy/preference.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/protocol_parser.py` & `neura_library-0.0.7/src/neuralib/stimpy/protocol_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/session.py` & `neura_library-0.0.7/src/neuralib/stimpy/session.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/stimpy_core.py` & `neura_library-0.0.7/src/neuralib/stimpy/stimpy_core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/stimpy_git.py` & `neura_library-0.0.7/src/neuralib/stimpy/stimpy_git.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,16 +493,15 @@
 
         log = load_stimlog(file, string_key=True)  # get dataframe using keyname
         print(log['PhotoIndicator'])
 
         log = load_stimlog(file, string_key=False)  # get dataframe using code int
         print(log[1])
 
-
-    :param file:
+    :param file: file path for the .stimlog
     :param string_key: show key as str type, otherwise, int type
     :return: Code:DataFrame dictionary
     """
 
     log_info = {}
     log_header = {}
     log_data = {}
```

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/stimpy_pyv.py` & `neura_library-0.0.7/src/neuralib/stimpy/stimpy_pyv.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/stimulus.py` & `neura_library-0.0.7/src/neuralib/stimpy/stimulus.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/stimpy/util.py` & `neura_library-0.0.7/src/neuralib/stimpy/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/tools/pkl_parq_view/main_app.py` & `neura_library-0.0.7/src/neuralib/tools/pkl_parq_view/main_app.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/tools/slack_bot/bot.py` & `neura_library-0.0.7/src/neuralib/tools/slack_bot/bot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/cli_args.py` & `neura_library-0.0.7/src/neuralib/util/cli_args.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,7 +44,16 @@
             return [self.flag]
 
         # flag + arg
         elif self.flag is not None and self.args is not None:
             return [self.flag, self.args]
         else:
             raise RuntimeError('')
+
+    @classmethod
+    def concat_command(cls, args: list[CliArgs]) -> list[str]:
+        """concat multiple ``CliArgs`` as list of subprocess command line"""
+        ret = []
+        for arg in args:
+            ret.extend(arg.as_command())
+
+        return ret
```

### Comparing `neura_library-0.0.6/src/neuralib/util/color_logging.py` & `neura_library-0.0.7/src/neuralib/util/color_logging.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/csv.py` & `neura_library-0.0.7/src/neuralib/util/csv.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/func.py` & `neura_library-0.0.7/src/neuralib/util/func.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/gpu.py` & `neura_library-0.0.7/src/neuralib/util/gpu.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/io.py` & `neura_library-0.0.7/src/neuralib/util/io.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/json.py` & `neura_library-0.0.7/src/neuralib/util/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 
 import json
 from pathlib import Path
+from typing import Any
 
 import numpy as np
 
 __all__ = ['JsonEncodeHandler',
            #
            'load_from_json',
            'save_to_json']
 
 
 class JsonEncodeHandler(json.JSONEncoder):
-    """extend from the JSONEncoder class and handle the conversions in a default method"""
+    """Extend from the JSONEncoder class and handle the conversions in a default method"""
 
-    def default(self, obj):
+    def default(self, obj: Any):
         if isinstance(obj, np.integer):
             return int(obj)
-        if isinstance(obj, np.floating):
+        elif isinstance(obj, np.floating):
             return float(obj)
-        if isinstance(obj, np.ndarray):
+        elif isinstance(obj, np.ndarray):
             return obj.tolist()
-        if isinstance(obj, Path):
+        elif isinstance(obj, Path):
             return str(obj)
+        elif isinstance(obj, np.bool_):
+            return bool(obj)
 
         return json.JSONEncoder.default(self, obj)
 
 
 def load_from_json(filepath: str | Path) -> dict:
     with open(filepath, "r") as file:
         return json.load(file)
```

### Comparing `neura_library-0.0.6/src/neuralib/util/profile_test.py` & `neura_library-0.0.7/src/neuralib/util/profile_test.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/segement.py` & `neura_library-0.0.7/src/neuralib/util/segement.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/table.py` & `neura_library-0.0.7/src/neuralib/util/table.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/tqdm.py` & `neura_library-0.0.7/src/neuralib/util/tqdm.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/util_clazz.py` & `neura_library-0.0.7/src/neuralib/util/util_clazz.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/util_cv2.py` & `neura_library-0.0.7/src/neuralib/util/util_cv2.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/util_type.py` & `neura_library-0.0.7/src/neuralib/util/util_type.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/util_verbose.py` & `neura_library-0.0.7/src/neuralib/util/util_verbose.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/utils.py` & `neura_library-0.0.7/src/neuralib/util/utils.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/util/version.py` & `neura_library-0.0.7/src/neuralib/util/version.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/core.py` & `neura_library-0.0.7/src/neuralib/wrapper/deeplabcut/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/wrapper/deeplabcut/util.py` & `neura_library-0.0.7/src/neuralib/wrapper/deeplabcut/util.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/wrapper/facemap/__init__.py` & `neura_library-0.0.7/src/neuralib/wrapper/facemap/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/wrapper/facemap/core.py` & `neura_library-0.0.7/src/neuralib/wrapper/facemap/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/wrapper/facemap/plot.py` & `neura_library-0.0.7/src/neuralib/wrapper/facemap/plot.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/wrapper/rastermap/__init__.py` & `neura_library-0.0.7/src/neuralib/wrapper/rastermap/__init__.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/src/neuralib/wrapper/rastermap/core.py` & `neura_library-0.0.7/src/neuralib/wrapper/rastermap/core.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/test/test_csv_context_manager.py` & `neura_library-0.0.7/test/test_csv_context_manager.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/test/test_persistence_autoinc.py` & `neura_library-0.0.7/test/test_persistence_autoinc.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/test/test_protocol_parser.py` & `neura_library-0.0.7/test/test_protocol_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/test/test_pyvstim_parser.py` & `neura_library-0.0.7/test/test_pyvstim_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/test/test_stimpy_bitbucket_parser.py` & `neura_library-0.0.7/test/test_stimpy_bitbucket_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/test/test_stimpy_github_parser.py` & `neura_library-0.0.7/test/test_stimpy_github_parser.py`

 * *Files identical despite different names*

### Comparing `neura_library-0.0.6/test/test_util_func.py` & `neura_library-0.0.7/test/test_util_func.py`

 * *Files identical despite different names*

