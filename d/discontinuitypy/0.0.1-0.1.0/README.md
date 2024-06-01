# Comparing `tmp/discontinuitypy-0.0.1.tar.gz` & `tmp/discontinuitypy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discontinuitypy-0.0.1.tar", last modified: Sat Feb  3 21:29:37 2024, max compression
+gzip compressed data, was "discontinuitypy-0.1.0.tar", last modified: Sat Jun  1 07:29:08 2024, max compression
```

## Comparing `discontinuitypy-0.0.1.tar` & `discontinuitypy-0.1.0.tar`

### file list

```diff
@@ -1,72 +1,23 @@
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.127083 discontinuitypy-0.0.1/
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.111810 discontinuitypy-0.0.1/.github/
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.114355 discontinuitypy-0.0.1/.github/workflows/
--rw-r--r--   0 zijin      (501) staff       (20)     1267 2023-12-05 03:05:37.000000 discontinuitypy-0.0.1/.github/workflows/deploy.yaml
--rw-r--r--   0 zijin      (501) staff       (20)      221 2023-12-05 03:16:32.000000 discontinuitypy-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0 zijin      (501) staff       (20)     2016 2024-02-03 20:45:53.000000 discontinuitypy-0.0.1/.gitignore
--rw-r--r--   0 zijin      (501) staff       (20)     2858 2024-02-03 21:29:37.126806 discontinuitypy-0.0.1/PKG-INFO
--rw-r--r--   0 zijin      (501) staff       (20)     1933 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/README.md
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.115817 discontinuitypy-0.0.1/discontinuitypy/
--rw-r--r--   0 zijin      (501) staff       (20)      434 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/__init__.py
--rw-r--r--   0 zijin      (501) staff       (20)    28617 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/_modidx.py
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.117884 discontinuitypy-0.0.1/discontinuitypy/core/
--rw-r--r--   0 zijin      (501) staff       (20)        0 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/core/__init__.py
--rw-r--r--   0 zijin      (501) staff       (20)     9189 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/core/detection.py
--rw-r--r--   0 zijin      (501) staff       (20)      533 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/core/event.py
--rw-r--r--   0 zijin      (501) staff       (20)     2727 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/core/pipeline.py
--rw-r--r--   0 zijin      (501) staff       (20)     9980 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/core/propeties.py
--rw-r--r--   0 zijin      (501) staff       (20)     2383 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/datasets.py
--rw-r--r--   0 zijin      (501) staff       (20)     2003 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/datasets_kedro.py
--rw-r--r--   0 zijin      (501) staff       (20)     4926 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/integration.py
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.118533 discontinuitypy-0.0.1/discontinuitypy/propeties/
--rw-r--r--   0 zijin      (501) staff       (20)        0 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/propeties/__init__.py
--rw-r--r--   0 zijin      (501) staff       (20)     3492 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/propeties/duration.py
--rw-r--r--   0 zijin      (501) staff       (20)     6035 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/propeties/mva.py
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.120096 discontinuitypy-0.0.1/discontinuitypy/utils/
--rw-r--r--   0 zijin      (501) staff       (20)        0 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/utils/__init__.py
--rw-r--r--   0 zijin      (501) staff       (20)     1859 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/utils/analysis.py
--rw-r--r--   0 zijin      (501) staff       (20)     9309 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/utils/basic.py
--rw-r--r--   0 zijin      (501) staff       (20)      941 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/utils/kedro.py
--rw-r--r--   0 zijin      (501) staff       (20)     2140 2024-02-03 21:03:16.000000 discontinuitypy-0.0.1/discontinuitypy/utils/lbl.py
--rw-r--r--   0 zijin      (501) staff       (20)     4770 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/utils/plot.py
--rw-r--r--   0 zijin      (501) staff       (20)     2704 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/discontinuitypy/utils/polars.py
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.126494 discontinuitypy-0.0.1/discontinuitypy.egg-info/
--rw-r--r--   0 zijin      (501) staff       (20)     2858 2024-02-03 21:29:37.000000 discontinuitypy-0.0.1/discontinuitypy.egg-info/PKG-INFO
--rw-r--r--   0 zijin      (501) staff       (20)     1689 2024-02-03 21:29:37.000000 discontinuitypy-0.0.1/discontinuitypy.egg-info/SOURCES.txt
--rw-r--r--   0 zijin      (501) staff       (20)        1 2024-02-03 21:29:37.000000 discontinuitypy-0.0.1/discontinuitypy.egg-info/dependency_links.txt
--rw-r--r--   0 zijin      (501) staff       (20)       52 2024-02-03 21:29:37.000000 discontinuitypy-0.0.1/discontinuitypy.egg-info/entry_points.txt
--rw-r--r--   0 zijin      (501) staff       (20)        1 2024-02-03 20:56:09.000000 discontinuitypy-0.0.1/discontinuitypy.egg-info/not-zip-safe
--rw-r--r--   0 zijin      (501) staff       (20)      107 2024-02-03 21:29:37.000000 discontinuitypy-0.0.1/discontinuitypy.egg-info/requires.txt
--rw-r--r--   0 zijin      (501) staff       (20)       16 2024-02-03 21:29:37.000000 discontinuitypy-0.0.1/discontinuitypy.egg-info/top_level.txt
--rw-r--r--   0 zijin      (501) staff       (20)      662 2024-02-03 21:08:15.000000 discontinuitypy-0.0.1/environment.yml
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.120260 discontinuitypy-0.0.1/images/
--rw-r--r--   0 zijin      (501) staff       (20)      507 2023-12-05 01:34:41.000000 discontinuitypy-0.0.1/images/qrcode.png
--rw-r--r--   0 zijin      (501) staff       (20)     2372 2024-02-03 20:47:41.000000 discontinuitypy-0.0.1/justfile
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.124470 discontinuitypy-0.0.1/notebooks/
--rw-r--r--   0 zijin      (501) staff       (20)       10 2023-12-05 04:53:39.000000 discontinuitypy-0.0.1/notebooks/.gitignore
--rw-r--r--   0 zijin      (501) staff       (20)    13436 2024-02-03 21:06:09.000000 discontinuitypy-0.0.1/notebooks/00_ids_finder.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)    15288 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/01_ids_detection.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)    23029 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/02_ids_properties.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     8373 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/03_mag_plasma.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     4070 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/20_datasets.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     3386 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/21_datasets_kedro.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     1543 2024-02-03 06:25:19.000000 discontinuitypy-0.0.1/notebooks/21_event.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     1649 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/__init__.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)      706 2024-02-01 18:21:41.000000 discontinuitypy-0.0.1/notebooks/_quarto.yml
--rw-r--r--   0 zijin      (501) staff       (20)      512 2024-02-01 18:18:16.000000 discontinuitypy-0.0.1/notebooks/about.qmd
--rw-r--r--   0 zijin      (501) staff       (20)     2216 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/index.qmd
--rw-r--r--   0 zijin      (501) staff       (20)      293 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/notebooks/nbdev.yml
--rw-r--r--   0 zijin      (501) staff       (20)     1225 2023-11-15 23:19:38.000000 discontinuitypy-0.0.1/notebooks/pipelines.yaml
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.124873 discontinuitypy-0.0.1/notebooks/properties/
--rw-r--r--   0 zijin      (501) staff       (20)    11855 2024-02-03 21:11:29.000000 discontinuitypy-0.0.1/notebooks/properties/00_duration.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)    12726 2024-02-03 21:11:54.000000 discontinuitypy-0.0.1/notebooks/properties/00_mva.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)      612 2024-02-03 21:08:43.000000 discontinuitypy-0.0.1/notebooks/sidebar.yml
-drwxr-xr-x   0 zijin      (501) staff       (20)        0 2024-02-03 21:29:37.126211 discontinuitypy-0.0.1/notebooks/utils/
--rw-r--r--   0 zijin      (501) staff       (20)    14220 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/utils/00_basic.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     8256 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/utils/01_plotting.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     3432 2024-02-03 21:01:30.000000 discontinuitypy-0.0.1/notebooks/utils/02_analysis_utils.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     4731 2023-11-30 04:20:59.000000 discontinuitypy-0.0.1/notebooks/utils/10_polars.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     2803 2023-11-23 01:50:19.000000 discontinuitypy-0.0.1/notebooks/utils/15_kedro.ipynb
--rw-r--r--   0 zijin      (501) staff       (20)     1183 2024-02-03 20:52:01.000000 discontinuitypy-0.0.1/settings.ini
--rw-r--r--   0 zijin      (501) staff       (20)       38 2024-02-03 21:29:37.127135 discontinuitypy-0.0.1/setup.cfg
--rw-r--r--   0 zijin      (501) staff       (20)     2693 2023-10-20 06:18:12.000000 discontinuitypy-0.0.1/setup.py
+-rw-r--r--   0        0        0      201 2024-06-01 07:22:07.900334 discontinuitypy-0.1.0/discontinuitypy/__init__.py
+-rw-r--r--   0        0        0    32531 2024-06-01 07:22:08.492078 discontinuitypy-0.1.0/discontinuitypy/_modidx.py
+-rw-r--r--   0        0        0     4360 2024-06-01 07:22:07.662706 discontinuitypy-0.1.0/discontinuitypy/config.py
+-rw-r--r--   0        0        0        0 2024-06-01 07:22:07.900078 discontinuitypy-0.1.0/discontinuitypy/core/__init__.py
+-rw-r--r--   0        0        0     1218 2024-06-01 07:22:07.640486 discontinuitypy-0.1.0/discontinuitypy/core/detection.py
+-rw-r--r--   0        0        0      533 2024-05-11 20:31:59.512725 discontinuitypy-0.1.0/discontinuitypy/core/event.py
+-rw-r--r--   0        0        0     3500 2024-06-01 07:22:07.635749 discontinuitypy-0.1.0/discontinuitypy/core/pipeline.py
+-rw-r--r--   0        0        0    10195 2024-06-01 07:22:07.652828 discontinuitypy-0.1.0/discontinuitypy/core/propeties.py
+-rw-r--r--   0        0        0     6527 2024-06-01 07:22:07.660609 discontinuitypy-0.1.0/discontinuitypy/datasets.py
+-rw-r--r--   0        0        0     2003 2024-06-01 02:19:03.182732 discontinuitypy-0.1.0/discontinuitypy/datasets_kedro.py
+-rw-r--r--   0        0        0        0 2024-06-01 07:22:07.900239 discontinuitypy-0.1.0/discontinuitypy/detection/__init__.py
+-rw-r--r--   0        0        0     8277 2024-06-01 07:22:07.646876 discontinuitypy-0.1.0/discontinuitypy/detection/variance.py
+-rw-r--r--   0        0        0    11369 2024-06-01 07:22:07.657381 discontinuitypy-0.1.0/discontinuitypy/integration.py
+-rw-r--r--   0        0        0     1782 2024-06-01 07:22:07.663737 discontinuitypy-0.1.0/discontinuitypy/missions.py
+-rw-r--r--   0        0        0        0 2024-06-01 07:22:07.900128 discontinuitypy-0.1.0/discontinuitypy/propeties/__init__.py
+-rw-r--r--   0        0        0     3261 2024-06-01 07:22:07.633733 discontinuitypy-0.1.0/discontinuitypy/propeties/duration.py
+-rw-r--r--   0        0        0     7510 2024-06-01 07:22:07.639450 discontinuitypy-0.1.0/discontinuitypy/propeties/mva.py
+-rw-r--r--   0        0        0        0 2024-06-01 07:22:07.900172 discontinuitypy-0.1.0/discontinuitypy/utils/__init__.py
+-rw-r--r--   0        0        0     1859 2024-06-01 07:22:07.648383 discontinuitypy-0.1.0/discontinuitypy/utils/analysis.py
+-rw-r--r--   0        0        0     7925 2024-06-01 07:22:07.631768 discontinuitypy-0.1.0/discontinuitypy/utils/basic.py
+-rw-r--r--   0        0        0     5511 2024-06-01 07:22:07.643633 discontinuitypy-0.1.0/discontinuitypy/utils/plot.py
+-rw-r--r--   0        0        0      992 2024-06-01 07:29:08.417886 discontinuitypy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 discontinuitypy-0.1.0/PKG-INFO
```

### Comparing `discontinuitypy-0.0.1/discontinuitypy/_modidx.py` & `discontinuitypy-0.1.0/discontinuitypy/_modidx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,77 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/ids_finder',
                 'doc_host': 'https://Beforerr.github.io',
                 'git_url': 'https://github.com/Beforerr/ids_finder',
                 'lib_path': 'discontinuitypy'},
-  'syms': { 'discontinuitypy.core.detection': { 'discontinuitypy.core.detection._compute_indices': ( 'ids_detection.html#_compute_indices',
-                                                                                                     'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.add_neighbor_std': ( 'ids_detection.html#add_neighbor_std',
-                                                                                                     'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.compute_combinded_std': ( 'ids_detection.html#compute_combinded_std',
-                                                                                                          'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.compute_index_diff': ( 'ids_detection.html#compute_index_diff',
-                                                                                                       'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.compute_index_fluctuation': ( 'ids_detection.html#compute_index_fluctuation',
-                                                                                                              'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.compute_index_std': ( 'ids_detection.html#compute_index_std',
-                                                                                                      'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.compute_indices': ( 'ids_detection.html#compute_indices',
-                                                                                                    'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.compute_std': ( 'ids_detection.html#compute_std',
-                                                                                                'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.detect_events': ( 'ids_detection.html#detect_events',
+  'syms': { 'discontinuitypy.config': { 'discontinuitypy.config.IDsConfig': ('ids_config.html#idsconfig', 'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.IDsConfig.export': ( 'ids_config.html#idsconfig.export',
+                                                                                     'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.IDsConfig.fname': ( 'ids_config.html#idsconfig.fname',
+                                                                                    'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.IDsConfig.load': ( 'ids_config.html#idsconfig.load',
+                                                                                   'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.IDsConfig.path': ( 'ids_config.html#idsconfig.path',
+                                                                                   'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.IDsConfig.timeranges': ( 'ids_config.html#idsconfig.timeranges',
+                                                                                         'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig': ( 'ids_config.html#speasyidsconfig',
+                                                                                    'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig._get_and_process_data': ( 'ids_config.html#speasyidsconfig._get_and_process_data',
+                                                                                                          'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.e_temp_var': ( 'ids_config.html#speasyidsconfig.e_temp_var',
+                                                                                               'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.get_and_process_data': ( 'ids_config.html#speasyidsconfig.get_and_process_data',
+                                                                                                         'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.get_vars': ( 'ids_config.html#speasyidsconfig.get_vars',
+                                                                                             'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.get_vars_df': ( 'ids_config.html#speasyidsconfig.get_vars_df',
+                                                                                                'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.ion_temp_var': ( 'ids_config.html#speasyidsconfig.ion_temp_var',
+                                                                                                 'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.mag_vars': ( 'ids_config.html#speasyidsconfig.mag_vars',
+                                                                                             'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.model_post_init': ( 'ids_config.html#speasyidsconfig.model_post_init',
+                                                                                                    'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.plasma_vars': ( 'ids_config.html#speasyidsconfig.plasma_vars',
+                                                                                                'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.SpeasyIDsConfig.set_data_from_vars': ( 'ids_config.html#speasyidsconfig.set_data_from_vars',
+                                                                                                       'discontinuitypy/config.py'),
+                                        'discontinuitypy.config.standardize_plasma_data': ( 'ids_config.html#standardize_plasma_data',
+                                                                                            'discontinuitypy/config.py')},
+            'discontinuitypy.core.detection': { 'discontinuitypy.core.detection.detect_events': ( 'ids_detection.html#detect_events',
                                                                                                   'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.filter_indices': ( 'ids_detection.html#filter_indices',
-                                                                                                   'discontinuitypy/core/detection.py'),
-                                                'discontinuitypy.core.detection.pl_dvec': ( 'ids_detection.html#pl_dvec',
-                                                                                            'discontinuitypy/core/detection.py'),
                                                 'discontinuitypy.core.detection.pl_format_time': ( 'ids_detection.html#pl_format_time',
                                                                                                    'discontinuitypy/core/detection.py')},
             'discontinuitypy.core.event': { 'discontinuitypy.core.event.get_event_data': ( 'event.html#get_event_data',
                                                                                            'discontinuitypy/core/event.py')},
-            'discontinuitypy.core.pipeline': { 'discontinuitypy.core.pipeline.compress_data_by_cands': ( 'ids_finder.html#compress_data_by_cands',
-                                                                                                         'discontinuitypy/core/pipeline.py'),
+            'discontinuitypy.core.pipeline': { 'discontinuitypy.core.pipeline.compress_data_by_events': ( 'ids_finder.html#compress_data_by_events',
+                                                                                                          'discontinuitypy/core/pipeline.py'),
+                                               'discontinuitypy.core.pipeline.compress_data_by_intervals': ( 'ids_finder.html#compress_data_by_intervals',
+                                                                                                             'discontinuitypy/core/pipeline.py'),
+                                               'discontinuitypy.core.pipeline.compress_dfs_by_intervals': ( 'ids_finder.html#compress_dfs_by_intervals',
+                                                                                                            'discontinuitypy/core/pipeline.py'),
                                                'discontinuitypy.core.pipeline.extract_features': ( 'ids_finder.html#extract_features',
                                                                                                    'discontinuitypy/core/pipeline.py'),
                                                'discontinuitypy.core.pipeline.ids_finder': ( 'ids_finder.html#ids_finder',
                                                                                              'discontinuitypy/core/pipeline.py')},
-            'discontinuitypy.core.propeties': { 'discontinuitypy.core.propeties.IDsPipeline': ( 'ids_properties.html#idspipeline',
-                                                                                                'discontinuitypy/core/propeties.py'),
-                                                'discontinuitypy.core.propeties.IDsPipeline.__init__': ( 'ids_properties.html#idspipeline.__init__',
-                                                                                                         'discontinuitypy/core/propeties.py'),
-                                                'discontinuitypy.core.propeties.IDsPipeline.calc_duration': ( 'ids_properties.html#idspipeline.calc_duration',
-                                                                                                              'discontinuitypy/core/propeties.py'),
-                                                'discontinuitypy.core.propeties.IDsPipeline.calc_mva_features': ( 'ids_properties.html#idspipeline.calc_mva_features',
-                                                                                                                  'discontinuitypy/core/propeties.py'),
-                                                'discontinuitypy.core.propeties.IDsPipeline.calc_normal_direction': ( 'ids_properties.html#idspipeline.calc_normal_direction',
-                                                                                                                      'discontinuitypy/core/propeties.py'),
-                                                'discontinuitypy.core.propeties.IDsPipeline.calc_rotation_angle': ( 'ids_properties.html#idspipeline.calc_rotation_angle',
-                                                                                                                    'discontinuitypy/core/propeties.py'),
-                                                'discontinuitypy.core.propeties.IDsPipeline.calc_vec_change': ( 'ids_properties.html#idspipeline.calc_vec_change',
+            'discontinuitypy.core.propeties': { 'discontinuitypy.core.propeties.IDsPdPipeline': ( 'ids_properties.html#idspdpipeline',
+                                                                                                  'discontinuitypy/core/propeties.py'),
+                                                'discontinuitypy.core.propeties.IDsPdPipeline.calc_duration': ( 'ids_properties.html#idspdpipeline.calc_duration',
                                                                                                                 'discontinuitypy/core/propeties.py'),
+                                                'discontinuitypy.core.propeties.IDsPdPipeline.calc_mva_features': ( 'ids_properties.html#idspdpipeline.calc_mva_features',
+                                                                                                                    'discontinuitypy/core/propeties.py'),
+                                                'discontinuitypy.core.propeties.IDsPdPipeline.calc_normal_direction': ( 'ids_properties.html#idspdpipeline.calc_normal_direction',
+                                                                                                                        'discontinuitypy/core/propeties.py'),
+                                                'discontinuitypy.core.propeties.IDsPdPipeline.calc_rotation_angle': ( 'ids_properties.html#idspdpipeline.calc_rotation_angle',
+                                                                                                                      'discontinuitypy/core/propeties.py'),
+                                                'discontinuitypy.core.propeties.IDsPdPipeline.calc_vec_change': ( 'ids_properties.html#idspdpipeline.calc_vec_change',
+                                                                                                                  'discontinuitypy/core/propeties.py'),
                                                 'discontinuitypy.core.propeties.calc_candidate_duration': ( 'ids_properties.html#calc_candidate_duration',
                                                                                                             'discontinuitypy/core/propeties.py'),
                                                 'discontinuitypy.core.propeties.calc_events_normal_direction': ( 'ids_properties.html#calc_events_normal_direction',
                                                                                                                  'discontinuitypy/core/propeties.py'),
                                                 'discontinuitypy.core.propeties.calc_events_rotation_angle': ( 'ids_properties.html#calc_events_rotation_angle',
                                                                                                                'discontinuitypy/core/propeties.py'),
                                                 'discontinuitypy.core.propeties.calc_events_vec_change': ( 'ids_properties.html#calc_events_vec_change',
@@ -71,83 +88,125 @@
                                                                                                       'discontinuitypy/core/propeties.py'),
                                                 'discontinuitypy.core.propeties.pdp.ApplyToRows._transform': ( 'ids_properties.html#pdp.applytorows._transform',
                                                                                                                'discontinuitypy/core/propeties.py'),
                                                 'discontinuitypy.core.propeties.process_events': ( 'ids_properties.html#process_events',
                                                                                                    'discontinuitypy/core/propeties.py')},
             'discontinuitypy.datasets': { 'discontinuitypy.datasets.IDsDataset': ( 'datasets.html#idsdataset',
                                                                                    'discontinuitypy/datasets.py'),
-                                          'discontinuitypy.datasets.IDsDataset.Config': ( 'datasets.html#idsdataset.config',
-                                                                                          'discontinuitypy/datasets.py'),
-                                          'discontinuitypy.datasets.IDsDataset.get_candidate': ( 'datasets.html#idsdataset.get_candidate',
-                                                                                                 'discontinuitypy/datasets.py'),
-                                          'discontinuitypy.datasets.IDsDataset.get_candidate_data': ( 'datasets.html#idsdataset.get_candidate_data',
-                                                                                                      'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IDsDataset.plot': ( 'datasets.html#idsdataset.plot',
+                                                                                        'discontinuitypy/datasets.py'),
                                           'discontinuitypy.datasets.IDsDataset.plot_candidate': ( 'datasets.html#idsdataset.plot_candidate',
                                                                                                   'discontinuitypy/datasets.py'),
                                           'discontinuitypy.datasets.IDsDataset.plot_candidates': ( 'datasets.html#idsdataset.plot_candidates',
                                                                                                    'discontinuitypy/datasets.py'),
-                                          'discontinuitypy.datasets.IDsDataset.update_candidates_with_plasma_data': ( 'datasets.html#idsdataset.update_candidates_with_plasma_data',
-                                                                                                                      'discontinuitypy/datasets.py')},
+                                          'discontinuitypy.datasets.IDsDataset.update_events': ( 'datasets.html#idsdataset.update_events',
+                                                                                                 'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IDsDataset.update_events_with_plasma_data': ( 'datasets.html#idsdataset.update_events_with_plasma_data',
+                                                                                                                  'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IDsDataset.update_events_with_temp_data': ( 'datasets.html#idsdataset.update_events_with_temp_data',
+                                                                                                                'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IdsEvents': ('datasets.html#idsevents', 'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IdsEvents.Config': ( 'datasets.html#idsevents.config',
+                                                                                         'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IdsEvents.export': ( 'datasets.html#idsevents.export',
+                                                                                         'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IdsEvents.find_events': ( 'datasets.html#idsevents.find_events',
+                                                                                              'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IdsEvents.get_event': ( 'datasets.html#idsevents.get_event',
+                                                                                            'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IdsEvents.get_event_data': ( 'datasets.html#idsevents.get_event_data',
+                                                                                                 'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.IdsEvents.get_events': ( 'datasets.html#idsevents.get_events',
+                                                                                             'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.log_event_change': ( 'datasets.html#log_event_change',
+                                                                                         'discontinuitypy/datasets.py'),
+                                          'discontinuitypy.datasets.write': ('datasets.html#write', 'discontinuitypy/datasets.py')},
             'discontinuitypy.datasets_kedro': { 'discontinuitypy.datasets_kedro.E1IDsDataset': ( 'datasets_kedro.html#e1idsdataset',
                                                                                                  'discontinuitypy/datasets_kedro.py'),
                                                 'discontinuitypy.datasets_kedro.cIDsDataset': ( 'datasets_kedro.html#cidsdataset',
                                                                                                 'discontinuitypy/datasets_kedro.py'),
                                                 'discontinuitypy.datasets_kedro.cIDsDataset.__init__': ( 'datasets_kedro.html#cidsdataset.__init__',
                                                                                                          'discontinuitypy/datasets_kedro.py'),
                                                 'discontinuitypy.datasets_kedro.cIDsDataset.load_data': ( 'datasets_kedro.html#cidsdataset.load_data',
                                                                                                           'discontinuitypy/datasets_kedro.py'),
                                                 'discontinuitypy.datasets_kedro.cIDsDataset.load_events': ( 'datasets_kedro.html#cidsdataset.load_events',
                                                                                                             'discontinuitypy/datasets_kedro.py')},
+            'discontinuitypy.detection.variance': { 'discontinuitypy.detection.variance.add_neighbor_std': ( 'detection/variance.html#add_neighbor_std',
+                                                                                                             'discontinuitypy/detection/variance.py'),
+                                                    'discontinuitypy.detection.variance.compute_combinded_std': ( 'detection/variance.html#compute_combinded_std',
+                                                                                                                  'discontinuitypy/detection/variance.py'),
+                                                    'discontinuitypy.detection.variance.compute_index_diff': ( 'detection/variance.html#compute_index_diff',
+                                                                                                               'discontinuitypy/detection/variance.py'),
+                                                    'discontinuitypy.detection.variance.compute_index_fluctuation': ( 'detection/variance.html#compute_index_fluctuation',
+                                                                                                                      'discontinuitypy/detection/variance.py'),
+                                                    'discontinuitypy.detection.variance.compute_index_std': ( 'detection/variance.html#compute_index_std',
+                                                                                                              'discontinuitypy/detection/variance.py'),
+                                                    'discontinuitypy.detection.variance.compute_indices': ( 'detection/variance.html#compute_indices',
+                                                                                                            'discontinuitypy/detection/variance.py'),
+                                                    'discontinuitypy.detection.variance.compute_std': ( 'detection/variance.html#compute_std',
+                                                                                                        'discontinuitypy/detection/variance.py'),
+                                                    'discontinuitypy.detection.variance.filter_indices': ( 'detection/variance.html#filter_indices',
+                                                                                                           'discontinuitypy/detection/variance.py'),
+                                                    'discontinuitypy.detection.variance.pl_dvec': ( 'detection/variance.html#pl_dvec',
+                                                                                                    'discontinuitypy/detection/variance.py')},
             'discontinuitypy.integration': { 'discontinuitypy.integration.calc_combined_features': ( 'mag_plasma.html#calc_combined_features',
                                                                                                      'discontinuitypy/integration.py'),
+                                             'discontinuitypy.integration.calc_plasma_parameter_change': ( 'mag_plasma.html#calc_plasma_parameter_change',
+                                                                                                           'discontinuitypy/integration.py'),
                                              'discontinuitypy.integration.calc_rotation_angle_pl': ( 'mag_plasma.html#calc_rotation_angle_pl',
                                                                                                      'discontinuitypy/integration.py'),
                                              'discontinuitypy.integration.combine_features': ( 'mag_plasma.html#combine_features',
                                                                                                'discontinuitypy/integration.py'),
                                              'discontinuitypy.integration.compute_Alfven_current': ( 'mag_plasma.html#compute_alfven_current',
                                                                                                      'discontinuitypy/integration.py'),
-                                             'discontinuitypy.integration.compute_Alfven_speed': ( 'mag_plasma.html#compute_alfven_speed',
-                                                                                                   'discontinuitypy/integration.py'),
                                              'discontinuitypy.integration.compute_inertial_length': ( 'mag_plasma.html#compute_inertial_length',
                                                                                                       'discontinuitypy/integration.py'),
+                                             'discontinuitypy.integration.format_time': ( 'mag_plasma.html#format_time',
+                                                                                          'discontinuitypy/integration.py'),
+                                             'discontinuitypy.integration.interpolate': ( 'mag_plasma.html#interpolate',
+                                                                                          'discontinuitypy/integration.py'),
+                                             'discontinuitypy.integration.interpolate2': ( 'mag_plasma.html#interpolate2',
+                                                                                           'discontinuitypy/integration.py'),
                                              'discontinuitypy.integration.vector_project': ( 'mag_plasma.html#vector_project',
                                                                                              'discontinuitypy/integration.py'),
                                              'discontinuitypy.integration.vector_project_pl': ( 'mag_plasma.html#vector_project_pl',
                                                                                                 'discontinuitypy/integration.py')},
-            'discontinuitypy.propeties.duration': { 'discontinuitypy.propeties.duration.calc_d_duration': ( 'properties/duration.html#calc_d_duration',
-                                                                                                            'discontinuitypy/propeties/duration.py'),
-                                                    'discontinuitypy.propeties.duration.calc_duration': ( 'properties/duration.html#calc_duration',
+            'discontinuitypy.missions': { 'discontinuitypy.missions.WindConfig': ( 'mission_config.html#windconfig',
+                                                                                   'discontinuitypy/missions.py'),
+                                          'discontinuitypy.missions.WindMeta': ( 'mission_config.html#windmeta',
+                                                                                 'discontinuitypy/missions.py')},
+            'discontinuitypy.propeties.duration': { 'discontinuitypy.propeties.duration.calc_duration': ( 'properties/duration.html#calc_duration',
                                                                                                           'discontinuitypy/propeties/duration.py'),
                                                     'discontinuitypy.propeties.duration.find_start_end_times': ( 'properties/duration.html#find_start_end_times',
                                                                                                                  'discontinuitypy/propeties/duration.py'),
                                                     'discontinuitypy.propeties.duration.get_time_from_condition': ( 'properties/duration.html#get_time_from_condition',
                                                                                                                     'discontinuitypy/propeties/duration.py'),
                                                     'discontinuitypy.propeties.duration.ts_max_derivative': ( 'properties/duration.html#ts_max_derivative',
                                                                                                               'discontinuitypy/propeties/duration.py'),
                                                     'discontinuitypy.propeties.duration.ts_max_distance': ( 'properties/duration.html#ts_max_distance',
                                                                                                             'discontinuitypy/propeties/duration.py')},
             'discontinuitypy.propeties.mva': { 'discontinuitypy.propeties.mva.calc_candidate_mva_features': ( 'properties/mva.html#calc_candidate_mva_features',
                                                                                                               'discontinuitypy/propeties/mva.py'),
+                                               'discontinuitypy.propeties.mva.calc_maxiumum_variance_direction': ( 'properties/mva.html#calc_maxiumum_variance_direction',
+                                                                                                                   'discontinuitypy/propeties/mva.py'),
                                                'discontinuitypy.propeties.mva.calc_mva_features': ( 'properties/mva.html#calc_mva_features',
                                                                                                     'discontinuitypy/propeties/mva.py'),
                                                'discontinuitypy.propeties.mva.fit_maxiumum_variance_direction': ( 'properties/mva.html#fit_maxiumum_variance_direction',
                                                                                                                   'discontinuitypy/propeties/mva.py'),
                                                'discontinuitypy.propeties.mva.minvar': ( 'properties/mva.html#minvar',
                                                                                          'discontinuitypy/propeties/mva.py')},
             'discontinuitypy.utils.analysis': { 'discontinuitypy.utils.analysis.filter_before_jupiter': ( 'utils/analysis_utils.html#filter_before_jupiter',
                                                                                                           'discontinuitypy/utils/analysis.py'),
                                                 'discontinuitypy.utils.analysis.filter_tranges_ds': ( 'utils/analysis_utils.html#filter_tranges_ds',
                                                                                                       'discontinuitypy/utils/analysis.py'),
                                                 'discontinuitypy.utils.analysis.link_coord2dim': ( 'utils/analysis_utils.html#link_coord2dim',
                                                                                                    'discontinuitypy/utils/analysis.py'),
                                                 'discontinuitypy.utils.analysis.n2_normalize': ( 'utils/analysis_utils.html#n2_normalize',
                                                                                                  'discontinuitypy/utils/analysis.py')},
-            'discontinuitypy.utils.basic': { 'discontinuitypy.utils.basic.DataConfig': ( 'utils/basic.html#dataconfig',
-                                                                                         'discontinuitypy/utils/basic.py'),
-                                             'discontinuitypy.utils.basic._expand_selectors': ( 'utils/basic.html#_expand_selectors',
+            'discontinuitypy.utils.basic': { 'discontinuitypy.utils.basic._expand_selectors': ( 'utils/basic.html#_expand_selectors',
                                                                                                 'discontinuitypy/utils/basic.py'),
                                              'discontinuitypy.utils.basic.calc_vec_mag': ( 'utils/basic.html#calc_vec_mag',
                                                                                            'discontinuitypy/utils/basic.py'),
                                              'discontinuitypy.utils.basic.check_fgm': ( 'utils/basic.html#check_fgm',
                                                                                         'discontinuitypy/utils/basic.py'),
                                              'discontinuitypy.utils.basic.concat_df': ( 'utils/basic.html#concat_df',
                                                                                         'discontinuitypy/utils/basic.py'),
@@ -167,47 +226,15 @@
                                                                                                    'discontinuitypy/utils/basic.py'),
                                              'discontinuitypy.utils.basic.partition_data_by_year': ( 'utils/basic.html#partition_data_by_year',
                                                                                                      'discontinuitypy/utils/basic.py'),
                                              'discontinuitypy.utils.basic.partition_data_by_year_month': ( 'utils/basic.html#partition_data_by_year_month',
                                                                                                            'discontinuitypy/utils/basic.py'),
                                              'discontinuitypy.utils.basic.pl.DataFrame.plot': ( 'utils/basic.html#pl.dataframe.plot',
                                                                                                 'discontinuitypy/utils/basic.py'),
-                                             'discontinuitypy.utils.basic.pl_norm': ( 'utils/basic.html#pl_norm',
-                                                                                      'discontinuitypy/utils/basic.py'),
-                                             'discontinuitypy.utils.basic.pmap': ( 'utils/basic.html#pmap',
-                                                                                   'discontinuitypy/utils/basic.py'),
                                              'discontinuitypy.utils.basic.resample': ( 'utils/basic.html#resample',
                                                                                        'discontinuitypy/utils/basic.py')},
-            'discontinuitypy.utils.kedro': { 'discontinuitypy.utils.kedro.load_context': ( 'utils/kedro.html#load_context',
-                                                                                           'discontinuitypy/utils/kedro.py')},
-            'discontinuitypy.utils.lbl': { 'discontinuitypy.utils.lbl.LblDataset': ( 'utils/lbl.html#lbldataset',
-                                                                                     'discontinuitypy/utils/lbl.py'),
-                                           'discontinuitypy.utils.lbl.LblDataset.__init__': ( 'utils/lbl.html#lbldataset.__init__',
-                                                                                              'discontinuitypy/utils/lbl.py'),
-                                           'discontinuitypy.utils.lbl.LblDataset._describe': ( 'utils/lbl.html#lbldataset._describe',
-                                                                                               'discontinuitypy/utils/lbl.py'),
-                                           'discontinuitypy.utils.lbl.LblDataset._load': ( 'utils/lbl.html#lbldataset._load',
-                                                                                           'discontinuitypy/utils/lbl.py'),
-                                           'discontinuitypy.utils.lbl.LblDataset._save': ( 'utils/lbl.html#lbldataset._save',
-                                                                                           'discontinuitypy/utils/lbl.py'),
-                                           'discontinuitypy.utils.lbl.load_lbl': ( 'utils/lbl.html#load_lbl',
-                                                                                   'discontinuitypy/utils/lbl.py')},
             'discontinuitypy.utils.plot': { 'discontinuitypy.utils.plot.plot_candidate': ( 'utils/plotting.html#plot_candidate',
                                                                                            'discontinuitypy/utils/plot.py'),
-                                            'discontinuitypy.utils.plot.savefig': ( 'utils/plotting.html#savefig',
-                                                                                    'discontinuitypy/utils/plot.py'),
                                             'discontinuitypy.utils.plot.setup_mva_plot': ( 'utils/plotting.html#setup_mva_plot',
                                                                                            'discontinuitypy/utils/plot.py'),
                                             'discontinuitypy.utils.plot.time_stamp': ( 'utils/plotting.html#time_stamp',
-                                                                                       'discontinuitypy/utils/plot.py')},
-            'discontinuitypy.utils.polars': { 'discontinuitypy.utils.polars._expand_selectors': ( 'utils/polars.html#_expand_selectors',
-                                                                                                  'discontinuitypy/utils/polars.py'),
-                                              'discontinuitypy.utils.polars.convert_to_pd_dataframe': ( 'utils/polars.html#convert_to_pd_dataframe',
-                                                                                                        'discontinuitypy/utils/polars.py'),
-                                              'discontinuitypy.utils.polars.create_partitions': ( 'utils/polars.html#create_partitions',
-                                                                                                  'discontinuitypy/utils/polars.py'),
-                                              'discontinuitypy.utils.polars.decompose_vector': ( 'utils/polars.html#decompose_vector',
-                                                                                                 'discontinuitypy/utils/polars.py'),
-                                              'discontinuitypy.utils.polars.pl_norm': ( 'utils/polars.html#pl_norm',
-                                                                                        'discontinuitypy/utils/polars.py'),
-                                              'discontinuitypy.utils.polars.sort': ( 'utils/polars.html#sort',
-                                                                                     'discontinuitypy/utils/polars.py')}}}
+                                                                                       'discontinuitypy/utils/plot.py')}}}
```

### Comparing `discontinuitypy-0.0.1/discontinuitypy/core/detection.py` & `discontinuitypy-0.1.0/discontinuitypy/detection/variance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,56 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../notebooks/01_ids_detection.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../notebooks/detection/01_variance.ipynb.
 
 # %% auto 0
-__all__ = ['INDEX_STD_THRESHOLD', 'INDEX_FLUC_THRESHOLD', 'INDEX_DIFF_THRESHOLD', 'SPARSE_THRESHOLD', 'pl_format_time',
-           'compute_std', 'compute_combinded_std', 'add_neighbor_std', 'compute_index_std', 'compute_index_fluctuation',
-           'pl_dvec', 'compute_index_diff', 'compute_indices', 'filter_indices', 'detect_events']
+__all__ = ['INDEX_STD_THRESHOLD', 'INDEX_FLUC_THRESHOLD', 'INDEX_DIFF_THRESHOLD', 'SPARSE_THRESHOLD', 'compute_std',
+           'add_neighbor_std', 'compute_index_std', 'compute_combinded_std', 'compute_index_fluctuation', 'pl_dvec',
+           'compute_index_diff', 'compute_indices', 'filter_indices']
 
-# %% ../../notebooks/01_ids_detection.ipynb 3
-from datetime import timedelta
+# %% ../../notebooks/detection/01_variance.ipynb 3
 import polars as pl
+import polars.selectors as cs
+from datetime import timedelta
 
-from fastcore.utils import *
-from fastcore.test import *
-from ..utils.polars import pl_norm
-
-# %% ../../notebooks/01_ids_detection.ipynb 4
-from ..utils.basic import _expand_selectors
-
-# %% ../../notebooks/01_ids_detection.ipynb 5
-# some helper functions
-def pl_format_time(df: pl.LazyFrame | pl.DataFrame, tau: timedelta):
-    return df.with_columns(
-        tstart=pl.col("time"),
-        tstop=(pl.col("time") + tau),
-        time=(pl.col("time") + tau / 2),
-    )
+# %% ../../notebooks/detection/01_variance.ipynb 4
+from beforerr.polars import pl_norm
 
-# %% ../../notebooks/01_ids_detection.ipynb 6
 def compute_std(
-    df: pl.DataFrame | pl.LazyFrame,
+    df: pl.LazyFrame,
     period: timedelta,  # period to group by
-    b_cols=["BX", "BY", "BZ"],
+    index_column="time",
+    cols: list[str] = ["BX", "BY", "BZ"],
     every: timedelta = None,  # every to group by (default: period / 2)
+    result_column="std",
 ):
     if every is None:
         every = period / 2
-    b_std_cols = [col_name + "_std" for col_name in b_cols]
+
+    std_cols = [col_name + "_std" for col_name in cols]
 
     std_df = (
-        df.group_by_dynamic("time", every=every, period=period)
+        df.group_by_dynamic(index_column, every=every, period=period)
         .agg(
-            pl.count(),
-            pl.col(b_cols).std(ddof=0).map_alias(lambda col_name: col_name + "_std"),
+            pl.len(),
+            pl.col(cols).std(ddof=0).name.suffix("_std"),
         )
         .with_columns(
-            pl_norm(b_std_cols).alias("B_std"),
+            pl_norm(std_cols).alias(result_column),
         )
-        .drop(b_std_cols)
+        .drop(std_cols)
     )
     return std_df
 
-
-def compute_combinded_std(df: pl.DataFrame | pl.LazyFrame, tau, cols) -> pl.DataFrame:
-    combined_std_cols = [col_name + "_combined_std" for col_name in cols]
-    offsets = [0 * tau, tau / 2]
-    combined_std_dfs = []
-    for offset in offsets:
-        truncated_df = df.select(
-            (pl.col("time") - offset).dt.truncate(tau, offset=offset).alias("time"),
-            pl.col(cols),
-        )
-
-        prev_df = truncated_df.select(
-            (pl.col("time") + tau),
-            pl.col(cols),
-        )
-
-        next_df = truncated_df.select(
-            (pl.col("time") - tau),
-            pl.col(cols),
-        )
-
-        temp_combined_std_df = (
-            pl.concat([prev_df, next_df])
-            .group_by("time")
-            .agg(
-                pl.col(cols)
-                .std(ddof=0)
-                .map_alias(lambda col_name: col_name + "_combined_std"),
-            )
-            .with_columns(B_std_combined=pl_norm(combined_std_cols))
-            .drop(combined_std_cols)
-            .sort("time")
-        )
-
-        combined_std_dfs.append(temp_combined_std_df)
-
-    combined_std_df = pl.concat(combined_std_dfs)
-    return combined_std_df
-
-# %% ../../notebooks/01_ids_detection.ipynb 8
+# %% ../../notebooks/detection/01_variance.ipynb 5
 def add_neighbor_std(
-    df: pl.LazyFrame, tau: timedelta, join_strategy="inner"
-):  # noqa: F811
+    df: pl.LazyFrame,
+    tau: timedelta,
+    join_strategy="inner",
+    std_column="std",
+    time_column="time",
+):
     """
     Get the neighbor standard deviations
 
     Parameters
     ----------
     - df (pl.LazyFrame): The input DataFrame.
     - tau : The time interval value.
@@ -104,31 +59,32 @@
     -----
     Simply shift would not work correctly if data is missing, like `std_next = pl.col("B_std").shift(-2)`.
 
     """
 
     # Calculate the standard deviation index
     prev_std_df = df.select(
-        pl.col("time") + tau,
-        B_std_prev=pl.col("B_std"),
-        count_prev=pl.col("count"),
+        pl.col(time_column) + tau,
+        cs.by_name(std_column, "len").name.suffix("_prev"),
     )
 
     next_std_df = df.select(
-        pl.col("time") - tau,
-        B_std_next=pl.col("B_std"),
-        count_next=pl.col("count"),
+        pl.col(time_column) - tau,
+        cs.by_name(std_column, "len").name.suffix("_next"),
     )
 
-    return df.join(prev_std_df, on="time", how=join_strategy).join(
-        next_std_df, on="time", how=join_strategy
+    return df.join(prev_std_df, on=time_column, how=join_strategy).join(
+        next_std_df, on=time_column, how=join_strategy
     )
 
-# %% ../../notebooks/01_ids_detection.ipynb 9
-def compute_index_std(df: pl.LazyFrame):  # noqa: F811
+# %% ../../notebooks/detection/01_variance.ipynb 6
+def compute_index_std(
+    df: pl.LazyFrame,
+    std_column="std",
+):
     """
     Compute the standard deviation index based on the given DataFrame
 
     Parameters
     ----------
     - df (pl.LazyFrame): The input DataFrame.
 
@@ -139,75 +95,95 @@
     Examples
     --------
     >>> index_std_df = compute_index_std_pl(df)
     >>> index_std_df
     """
 
     return df.with_columns(
-        index_std=pl.col("B_std") / pl.max_horizontal("B_std_prev", "B_std_next"),
+        index_std=pl.col(std_column)
+        / pl.max_horizontal(f"{std_column}_prev", f"{std_column}_next"),
     )
 
-# %% ../../notebooks/01_ids_detection.ipynb 11
-def compute_index_fluctuation(df: pl.LazyFrame, base_col="B_std"):
-    std_combined = pl.col("B_std_combined")
-    std_added = pl.sum_horizontal("B_std_prev", "B_std_next")
-    return df.with_columns(index_fluctuation=std_combined / std_added)
+# %% ../../notebooks/detection/01_variance.ipynb 8
+def compute_combinded_std(
+    df: pl.LazyFrame,
+    cols: list[str],
+    every: timedelta,  # every to group by (default: period / 2)
+    period: timedelta = None,  # period to group by
+    index_column="time",
+    result_column="std_combined",
+):
+    prev_df = df.with_columns(pl.col(index_column) + period)
+    next_df = df.with_columns(pl.col(index_column) - period)
+    return (
+        pl.concat([prev_df, next_df])
+        .sort(index_column)
+        .group_by_dynamic(index_column, every=every, period=period)
+        .agg(cs.by_name(cols).std(ddof=0).name.suffix("_combined"))
+        .select(
+            index_column,
+            pl_norm([col_name + "_combined" for col_name in cols]).alias(result_column),
+        )
+    )
+
+
+# | export
+def compute_index_fluctuation(df: pl.LazyFrame, std_column="std", clean=True):
+    std_combined = pl.col(f"{std_column}_combined")
+    std_added = pl.sum_horizontal(f"{std_column}_prev", f"{std_column}_next")
+
+    index_df = df.with_columns(index_fluctuation=std_combined / std_added)
+    if clean:
+        return index_df.drop(f"{std_column}_combined")
+
+# %% ../../notebooks/detection/01_variance.ipynb 10
+from ..utils.basic import _expand_selectors
+
 
-# %% ../../notebooks/01_ids_detection.ipynb 13
 def pl_dvec(columns, *more_columns):
     all_columns = _expand_selectors(columns, *more_columns)
     return [
         (pl.col(column).first() - pl.col(column).last()).alias(f"d{column}_vec")
         for column in all_columns
     ]
 
-# %% ../../notebooks/01_ids_detection.ipynb 14
-def compute_index_diff(df: pl.LazyFrame, period: timedelta, cols):
+# %% ../../notebooks/detection/01_variance.ipynb 11
+def compute_index_diff(
+    df: pl.LazyFrame,
+    every: timedelta,
+    cols: list[str],
+    period: timedelta = None,
+    clean=True,
+):
     db_cols = ["d" + col + "_vec" for col in cols]
 
     index_diff = (
-        df.with_columns(B=pl_norm(cols))
-        .group_by_dynamic("time", every=period / 2, period=period)
+        df.with_columns(pl_norm(cols).alias("_vec_mag"))
+        .group_by_dynamic("time", every=every, period=period)
         .agg(
-            pl.col("B").mean().alias("B_mean"),
+            pl.col("_vec_mag").mean().name.suffix("_mean"),
             *pl_dvec(cols),
         )
-        .with_columns(dB_vec=pl_norm(db_cols))
-        .with_columns(index_diff=pl.col("dB_vec") / pl.col("B_mean"))
-        .drop(db_cols)
-    )
-
-    return index_diff
-
-# %% ../../notebooks/01_ids_detection.ipynb 15
-def _compute_indices(
-    df: pl.LazyFrame, tau: timedelta, cols: list[str] = ["BX", "BY", "BZ"]
-) -> pl.LazyFrame:
-    join_strategy = "inner"
-
-    std_df = compute_std(df, tau, cols)
-    stds_df = add_neighbor_std(std_df, tau)
-
-    combined_std_df = compute_combinded_std(df, tau, cols)
-    index_diff = compute_index_diff(df, tau, cols)
-
-    indices = (
-        stds_df.join(index_diff, on="time")
-        .join(combined_std_df, on="time", how=join_strategy)
-        .pipe(compute_index_std)
-        .pipe(compute_index_fluctuation)
-        .drop(["B_std_prev", "B_std_next", "B_added_std", "B_std_combined"])
+        .with_columns(pl_norm(db_cols).alias("_dvec_mag"))
+        .with_columns(index_diff=pl.col("_dvec_mag") / pl.col("_vec_mag_mean"))
     )
 
-    return indices
-
+    if clean:
+        return index_diff.drop("_vec_mag", "_vec_mag_mean", "_dvec_mag", *db_cols)
+    else:
+        return index_diff
 
+# %% ../../notebooks/detection/01_variance.ipynb 12
 def compute_indices(
-    df: pl.DataFrame, tau: timedelta, bcols: list[str] = ["BX", "BY", "BZ"]
-) -> pl.DataFrame:
+    df: pl.LazyFrame,
+    tau: timedelta,
+    cols: list[str] = ["BX", "BY", "BZ"],
+    clean=True,
+    join_strategy="inner",
+) -> pl.LazyFrame:
     """
     Compute all index based on the given DataFrame and tau value.
 
     Parameters
     ----------
     df : pl.DataFrame
         Input DataFrame.
@@ -233,48 +209,61 @@
         Because we could not tell if it is a real ID or just a partial wave
         from incomplete data without previous or/and next std.
         Hopefully we can pick up the lost ones with smaller tau.
     - TODO: Can be optimized further, but this is already fast enough.
         - TEST: if `join` can be improved by shift after filling the missing values.
         - TEST: if `list` in `polars` really fast?
     """
-    return _compute_indices(df.lazy(), tau, bcols).collect()
 
-# %% ../../notebooks/01_ids_detection.ipynb 17
-# from discontinuitypy import PARAMS
+    every = tau / 2
+    period = tau
+
+    stds_df = df.pipe(compute_std, period=period, cols=cols).pipe(
+        add_neighbor_std, tau=tau
+    )
+
+    combined_std_df = compute_combinded_std(df, cols, every=every, period=period)
+
+    indices = (
+        df.pipe(compute_index_diff, every=every, period=period, cols=cols)
+        .join(stds_df, on="time")
+        .join(combined_std_df, on="time", how=join_strategy)
+        .pipe(compute_index_std)
+        .pipe(compute_index_fluctuation)
+    )
+
+    if clean:
+        return indices.drop(
+            ["B_std_prev", "B_std_next", "B_added_std", "B_std_combined"]
+        )
+    else:
+        return indices
 
-# INDEX_STD_THRESHOLD = PARAMS['detection']['index_std_threshold']
-# INDEX_FLUC_THRESHOLD = PARAMS['detection']['index_fluc_threshold']
-# INDEX_DIFF_THRESHOLD = PARAMS['detection']['index_diff_threshold']
+# %% ../../notebooks/detection/01_variance.ipynb 14
 INDEX_STD_THRESHOLD = 2
 INDEX_FLUC_THRESHOLD = 1
 INDEX_DIFF_THRESHOLD = 0.1
 SPARSE_THRESHOLD = 15
 
-# %% ../../notebooks/01_ids_detection.ipynb 18
+# %% ../../notebooks/detection/01_variance.ipynb 15
 def filter_indices(
-    df: pl.DataFrame | pl.LazyFrame,
-    index_std_threshold : float = INDEX_STD_THRESHOLD,
-    index_fluc_threshold : float =INDEX_FLUC_THRESHOLD,
-    index_diff_threshold : float =INDEX_DIFF_THRESHOLD,
-    sparse_num : int = SPARSE_THRESHOLD,
-) -> pl.DataFrame | pl.LazyFrame:
+    df: pl.LazyFrame,
+    index_std_threshold: float = INDEX_STD_THRESHOLD,
+    index_fluc_threshold: float = INDEX_FLUC_THRESHOLD,
+    index_diff_threshold: float = INDEX_DIFF_THRESHOLD,
+    sparse_num: int = SPARSE_THRESHOLD,
+) -> pl.LazyFrame:
     # filter indices to get possible IDs
 
     return df.filter(
         pl.col("index_std") > index_std_threshold,
         pl.col("index_fluctuation") > index_fluc_threshold,
         pl.col("index_diff") > index_diff_threshold,
-        pl.col("index_std").is_finite(), # for cases where neighboring groups have std=0
-        pl.col("count") > sparse_num, 
-        pl.col("count_prev") > sparse_num, # filter out sparse intervals, which may give unreasonable results.
-        pl.col("count_next") > sparse_num # filter out sparse intervals, which may give unreasonable results.
-    ).drop(["count_prev", "count_next"])
-
-# %% ../../notebooks/01_ids_detection.ipynb 19
-def detect_events(data: pl.DataFrame, tau: timedelta, ts: timedelta, bcols):
-    indices = compute_indices(data, tau, bcols)
-    sparse_num = tau / ts // 3
-    events = indices.pipe(filter_indices, sparse_num=sparse_num).pipe(
-        pl_format_time, tau
-    )
-    return events
+        pl.col(
+            "index_std"
+        ).is_finite(),  # for cases where neighboring groups have std=0
+        pl.col("len") > sparse_num,
+        pl.col("len_prev")
+        > sparse_num,  # filter out sparse intervals, which may give unreasonable results.
+        pl.col("len_next")
+        > sparse_num,  # filter out sparse intervals, which may give unreasonable results.
+    ).drop(["len_prev", "len_next"])
```

### Comparing `discontinuitypy-0.0.1/discontinuitypy/core/event.py` & `discontinuitypy-0.1.0/discontinuitypy/core/event.py`

 * *Files identical despite different names*

### Comparing `discontinuitypy-0.0.1/discontinuitypy/core/propeties.py` & `discontinuitypy-0.1.0/discontinuitypy/core/propeties.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../notebooks/02_ids_properties.ipynb.
 
 # %% auto 0
 __all__ = ['get_candidate_data', 'get_candidates', 'calc_candidate_duration', 'get_data_at_times', 'calc_rotation_angle',
            'calc_events_rotation_angle', 'calc_normal_direction', 'calc_events_normal_direction',
-           'calc_events_vec_change', 'IDsPipeline', 'process_events']
+           'calc_events_vec_change', 'IDsPdPipeline', 'process_events']
 
 # %% ../../notebooks/02_ids_properties.ipynb 1
 #| code-summary: "Import all the packages needed for the project"
-from fastcore.utils import *
-from fastcore.test import *
 import polars as pl
 import xarray as xr
+from fastcore.all import patch
 
 try:
     import modin.pandas as pd
     import modin.pandas as mpd
     from modin.config import ProgressBar
     ProgressBar.enable()
 except ImportError:
@@ -23,31 +22,29 @@
     
 import numpy as np
 
 from datetime import timedelta
 
 from loguru import logger
 
-
 import pdpipe as pdp
 from pdpipe.util import out_of_place_col_insert
-from multipledispatch import dispatch
 
 # %% ../../notebooks/02_ids_properties.ipynb 2
-@dispatch(object, xr.DataArray)
 def get_candidate_data(
-    candidate, data, neighbor: int = 0
+    candidate: dict, data: xr.DataArray, neighbor: int = 0
 ) -> xr.DataArray:
     duration = candidate["tstop"] - candidate["tstart"]
     offset = neighbor * duration
     temp_tstart = candidate["tstart"] - offset
     temp_tstop = candidate["tstop"] + offset
 
     return data.sel(time=slice(temp_tstart, temp_tstop))
 
+
 def get_candidates(candidates: pd.DataFrame, candidate_type=None, num: int = 4):
     if candidate_type is not None:
         _candidates = candidates[candidates["type"] == candidate_type]
     else:
         _candidates = candidates
 
     # Sample a specific number of candidates if num is provided and it's less than the total number
@@ -58,53 +55,38 @@
         return _candidates.sample(num)
     else:
         return _candidates
 
 # %% ../../notebooks/02_ids_properties.ipynb 4
 from ..propeties.duration import calc_duration
 
-
-def calc_candidate_duration(candidate: pd.Series, data, method="distance"):
+# %% ../../notebooks/02_ids_properties.ipynb 5
+def calc_candidate_duration(candidate, data, **kwargs):
     try:
         candidate_data = get_candidate_data(candidate, data)
-        result = calc_duration(candidate_data)
+        result = calc_duration(candidate_data, **kwargs)
+        return pandas.Series(result)
     except Exception as e:
-        # logger.debug(f"Error for candidate {candidate} at {candidate['time']}: {str(e)}") # can not be serialized
-        print(f"Error for candidate {candidate} at {candidate['time']}: {str(e)}")
-        raise e
-
-    if method == "distance":
-        return pd.Series(
-            {
-                "d_tstart": result[0],
-                "d_tstop": result[1],
-            }
-        )
-    elif method == "derivative":
-        return pd.Series(
-            {
-                "d_tstart": result[0],
-                "d_tstop": result[1],
-                "d_time": result[2],
-                "d_star": result[3],
-            }
+        logger.debug(
+            f"Error for candidate {candidate} at {candidate['time']}: {str(e)}"
         )
+        raise e
 
-# %% ../../notebooks/02_ids_properties.ipynb 6
+# %% ../../notebooks/02_ids_properties.ipynb 7
 from ..propeties.mva import calc_candidate_mva_features
 
-# %% ../../notebooks/02_ids_properties.ipynb 8
+# %% ../../notebooks/02_ids_properties.ipynb 9
 def get_data_at_times(data: xr.DataArray, times) -> np.ndarray:
     """
     Select data at specified times.
     """
     # Use xarray's selection capability if data supports it
     return data.sel(time=times, method="nearest").to_numpy()
 
-# %% ../../notebooks/02_ids_properties.ipynb 9
+# %% ../../notebooks/02_ids_properties.ipynb 10
 def calc_rotation_angle(v1, v2):
     """
     Computes the rotation angle between two vectors.
     
     Parameters:
     - v1: The first vector(s).
     - v2: The second vector(s).
@@ -125,29 +107,29 @@
     
     angle = np.arccos(cosine_angle)
     
     # Convert the angles from radians to degrees
     return np.degrees(angle)
 
 
-# %% ../../notebooks/02_ids_properties.ipynb 10
+# %% ../../notebooks/02_ids_properties.ipynb 11
 def calc_events_rotation_angle(events, data: xr.DataArray):
     """
     Computes the rotation angle(s) at two different time steps.
     """
-    tstart = events['d_tstart'].to_numpy()
-    tstop = events['d_tstop'].to_numpy()
+    tstart = events['t.d_start'].to_numpy()
+    tstop = events['t.d_end'].to_numpy()
 
     vecs_before = get_data_at_times(data, tstart)
     vecs_after = get_data_at_times(data, tstop)
 
     rotation_angles = calc_rotation_angle(vecs_before, vecs_after)
     return rotation_angles
 
-# %% ../../notebooks/02_ids_properties.ipynb 12
+# %% ../../notebooks/02_ids_properties.ipynb 13
 def calc_normal_direction(v1, v2, normalize=True) -> np.ndarray:
     """
     Computes the normal direction of two vectors.
 
     Parameters
     ----------
     v1 : array_like 
@@ -155,44 +137,44 @@
     v2 : array_like 
         The second vector(s).
     """
     c = np.cross(v1, v2)
     return c / np.linalg.norm(c, axis=-1, keepdims=True)
 
 
-# %% ../../notebooks/02_ids_properties.ipynb 13
+# %% ../../notebooks/02_ids_properties.ipynb 14
 def calc_events_normal_direction(events, data: xr.DataArray):
     """
     Computes the normal directions(s) at two different time steps.
     """
-    tstart = events['d_tstart'].to_numpy()
-    tstop = events['d_tstop'].to_numpy()
+    tstart = events['t.d_start'].to_numpy()
+    tstop = events['t.d_end'].to_numpy()
 
     vecs_before = get_data_at_times(data, tstart)
     vecs_after = get_data_at_times(data, tstop)
 
     normal_directions = calc_normal_direction(vecs_before, vecs_after)
     # need to convert to list first, as only 1D array is supported
     return normal_directions.tolist()
 
 
-# %% ../../notebooks/02_ids_properties.ipynb 14
+# %% ../../notebooks/02_ids_properties.ipynb 15
 def calc_events_vec_change(events, data: xr.DataArray):
     """
     Utils function to calculate features related to the change of the magnetic field
     """
-    tstart = events['d_tstart'].to_numpy()
-    tstop = events['d_tstop'].to_numpy()
+    tstart = events['t.d_start'].to_numpy()
+    tstop = events['t.d_end'].to_numpy()
     
     vecs_before = get_data_at_times(data, tstart)
     vecs_after = get_data_at_times(data, tstop)
     return (vecs_after - vecs_before).tolist()
     
 
-# %% ../../notebooks/02_ids_properties.ipynb 17
+# %% ../../notebooks/02_ids_properties.ipynb 18
 @patch
 def _transform(self: pdp.ApplyToRows, X, verbose):
     new_cols = X.apply(self._func, axis=1)
     if isinstance(new_cols, (pd.Series, pandas.Series)):
         loc = len(X.columns)
         if self._follow_column:
             loc = X.columns.get_loc(self._follow_column) + 1
@@ -219,85 +201,105 @@
         }
         return X.assign(**assign_map)
     raise TypeError(  # pragma: no cover
         "Unexpected type generated by applying a function to a DataFrame."
         " Only Series and DataFrame are allowed."
     )
 
-# %% ../../notebooks/02_ids_properties.ipynb 19
-class IDsPipeline:
-    def __init__(self):
-        pass
-
-    def calc_duration(self, data: xr.DataArray):
+# %% ../../notebooks/02_ids_properties.ipynb 20
+class IDsPdPipeline:
+    @staticmethod
+    def calc_duration(data: xr.DataArray, **kwargs):
         return pdp.ApplyToRows(
-            lambda candidate: calc_candidate_duration(candidate, data),
-            func_desc="calculating duration parameters",
+            lambda df: calc_candidate_duration(df, data, **kwargs),
+            func_desc="calculating pre-duration parameters",
         )
 
-    def calc_mva_features(self, data):
+    @staticmethod
+    def calc_mva_features(data, **kwargs):
         return pdp.ApplyToRows(
-            lambda candidate: calc_candidate_mva_features(candidate, data),
-            func_desc='calculating MVA features',
+            lambda df: calc_candidate_mva_features(df, data, **kwargs),
+            func_desc="calculating MVA features",
         )
 
-    def calc_vec_change(self, data):
+    @staticmethod
+    def calc_vec_change(data, **kwargs):
         return pdp.ColByFrameFunc(
             "dB",
-            lambda candidate: calc_events_vec_change(candidate, data),
-            func_desc='calculating compound change',
+            lambda df: calc_events_vec_change(df, data, **kwargs),
+            func_desc="calculating compound change",
         )
 
-    def calc_rotation_angle(self, data):
+    @staticmethod
+    def calc_rotation_angle(data, **kwargs):
         return pdp.ColByFrameFunc(
             "rotation_angle",
-            lambda df: calc_events_rotation_angle(df, data),
+            lambda df: calc_events_rotation_angle(df, data, **kwargs),
             func_desc="calculating rotation angle",
         )
 
-    def calc_normal_direction(self, data):
+    @staticmethod
+    def calc_normal_direction(data, name="normal_direction", **kwargs):
         return pdp.ColByFrameFunc(
-            "normal_direction",
-            lambda df: calc_events_normal_direction(df, data),
+            name,
+            lambda df: calc_events_normal_direction(df, data, **kwargs),
             func_desc="calculating normal direction",
         )
 
-# %% ../../notebooks/02_ids_properties.ipynb 20
-from ..utils.polars import convert_to_pd_dataframe, decompose_vector  # noqa: E402
-
 # %% ../../notebooks/02_ids_properties.ipynb 21
+from beforerr.polars import convert_to_pd_dataframe, decompose_vector
+
+# %% ../../notebooks/02_ids_properties.ipynb 22
+from typing import Literal
+
+
 def process_events(
     candidates_pl: pl.DataFrame,  # potential candidates DataFrame
     sat_fgm: xr.DataArray,  # satellite FGM data
     data_resolution: timedelta,  # time resolution of the data
     modin=True,
+    method: Literal["fit", "derivative"]= "fit",
     **kwargs,
 ) -> pl.DataFrame:
     "Process candidates DataFrame"
 
-    candidates = convert_to_pd_dataframe(candidates_pl, modin=modin)
+    candidates = pd.DataFrame(convert_to_pd_dataframe(candidates_pl, modin=modin))
+    
+    if method == "fit":
+        duration_method = "distance"  
+    else:
+        duration_method = "derivative"
 
-    id_pipelines = IDsPipeline()
-    candidates = id_pipelines.calc_duration(sat_fgm).apply(candidates)
+    candidates = (
+        IDsPdPipeline.calc_duration(sat_fgm, method=duration_method, **kwargs)
+        .apply(candidates)
+        .dropna()
+    )  # Remove candidates with NaN values)
 
     ids = (
-        id_pipelines.calc_mva_features(sat_fgm)
-        + id_pipelines.calc_vec_change(sat_fgm)
-        + id_pipelines.calc_rotation_angle(sat_fgm)
-        + id_pipelines.calc_normal_direction(sat_fgm)
-    ).apply(
-        candidates.dropna()  # Remove candidates with NaN values)
-    )
+        IDsPdPipeline.calc_mva_features(sat_fgm, method=method, **kwargs)
+        + IDsPdPipeline.calc_vec_change(sat_fgm)
+        + IDsPdPipeline.calc_rotation_angle(sat_fgm)
+        + IDsPdPipeline.calc_normal_direction(sat_fgm, name="k")
+    ).apply(candidates)
 
     if isinstance(ids, mpd.DataFrame):
         ids = ids._to_pandas()
 
-    return (
-        pl.DataFrame(ids)
-        .pipe(decompose_vector, "dB")
-        .pipe(decompose_vector, "dB_lmn")
-        .pipe(decompose_vector, "normal_direction", name="k")
-        .pipe(decompose_vector, "Vl")
-        .pipe(decompose_vector, "Vn")
-        .drop(["dB", "dB_lmn", "normal_direction", "Vl", "Vn"])
-    )
+    vectors2decompose = ["dB", "dB_lmn", "k", "Vl", "Vn"]
+
+    df = pl.DataFrame(
+        ids.dropna(), schema_overrides={vec: pl.List for vec in vectors2decompose}
+    )  # ArrowInvalid: Could not convert [0.9799027968348948, -0.17761542644940076, -0.07309766783111293] with type list: tried to convert to double
+
+    if method == "fit":
+        duration_expr = pl.col("fit.vars.sigma") * 2
+    else:
+        duration_expr = (
+            pl.col("t.d_end") - pl.col("t.d_start")
+        ).dt.total_nanoseconds() / 1e9  # convert to seconds
+
+    for vec in vectors2decompose:
+        df = decompose_vector(df, vec)
+
+    return df.with_columns(duration=duration_expr).drop(vectors2decompose)
     # ValueError: Data type fixed_size_list[pyarrow] not supported by interchange protocol
```

### Comparing `discontinuitypy-0.0.1/discontinuitypy/datasets_kedro.py` & `discontinuitypy-0.1.0/discontinuitypy/datasets_kedro.py`

 * *Files identical despite different names*

### Comparing `discontinuitypy-0.0.1/discontinuitypy/propeties/duration.py` & `discontinuitypy-0.1.0/discontinuitypy/propeties/duration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../notebooks/properties/00_duration.ipynb.
 
 # %% auto 0
-__all__ = ['THRESHOLD_RATIO', 'AvailableMethod', 'ts_max_distance', 'ts_max_derivative', 'calc_d_duration',
-           'find_start_end_times', 'get_time_from_condition', 'calc_duration']
+__all__ = ['THRESHOLD_RATIO', 'AvailableMethod', 'ts_max_distance', 'ts_max_derivative', 'find_start_end_times',
+           'get_time_from_condition', 'calc_duration']
 
 # %% ../../notebooks/properties/00_duration.ipynb 1
 from scipy.spatial import distance_matrix
 import xarray as xr
 import numpy as np
 import pandas as pd
 from xarray_einstats import linalg
@@ -18,59 +18,56 @@
 ):
     "Compute the time interval when the timeseries has maxium cumulative variation"
     distance = distance_matrix(ts.data, ts.data)
     max_distance_index = np.unravel_index(np.argmax(distance), distance.shape)
     return ts[coord].values[list(max_distance_index)]
 
 # %% ../../notebooks/properties/00_duration.ipynb 6
-THRESHOLD_RATIO  = 1/4
+THRESHOLD_RATIO = 1 / 4
+
 
 def ts_max_derivative(vec: xr.DataArray, threshold_ratio=THRESHOLD_RATIO):
     # NOTE: gradient calculated at the edge is not reliable.
-    vec_diff = vec.differentiate("time", datetime_unit="s").isel(time=slice(1,-1))
-    vec_diff_mag = linalg.norm(vec_diff, dims='v_dim')
+    vec_diff = vec.differentiate("time", datetime_unit="s").isel(time=slice(1, -1))
+    vec_diff_mag = linalg.norm(vec_diff, dims="v_dim")
 
     # Determine d_star based on trend
     if vec_diff_mag.isnull().all():
-        raise ValueError("The differentiated vector magnitude contains only NaN values. Cannot compute duration.")
-    
+        raise ValueError(
+            "The differentiated vector magnitude contains only NaN values. Cannot compute duration."
+        )
+
     d_star_index = vec_diff_mag.argmax(dim="time")
     d_star = vec_diff_mag[d_star_index].item()
     d_time = vec_diff_mag.time[d_star_index].values
-    
+
     threshold = d_star * threshold_ratio
 
     start_time, end_time = find_start_end_times(vec_diff_mag, d_time, threshold)
-    
-    return start_time, end_time, d_time, d_star, threshold
 
-def calc_d_duration(vec: xr.DataArray, d_time, threshold) -> pd.Series:
-    vec_diff = vec.differentiate("time", datetime_unit="s")
-    vec_diff_mag = linalg.norm(vec_diff, dims='v_dim')
+    return start_time, end_time, d_time, d_star
 
-    start_time, end_time = find_start_end_times(vec_diff_mag, d_time, threshold)
 
-    return pd.Series({
-        'd_tstart': start_time,
-        'd_tstop': end_time,
-    })
- 
-def find_start_end_times(vec_diff_mag: xr.DataArray, d_time, threshold) -> tuple[pd.Timestamp, pd.Timestamp]:
+def find_start_end_times(
+    vec_diff_mag: xr.DataArray, d_time, threshold
+) -> tuple[pd.Timestamp, pd.Timestamp]:
     # Determine start time
     pre_vec_mag = vec_diff_mag.sel(time=slice(None, d_time))
     start_time = get_time_from_condition(pre_vec_mag, threshold, "last_below")
 
     # Determine stop time
     post_vec_mag = vec_diff_mag.sel(time=slice(d_time, None))
     end_time = get_time_from_condition(post_vec_mag, threshold, "first_below")
 
     return start_time, end_time
 
 
-def get_time_from_condition(vec: xr.DataArray, threshold, condition_type) -> pd.Timestamp:
+def get_time_from_condition(
+    vec: xr.DataArray, threshold, condition_type
+) -> pd.Timestamp:
     if condition_type == "first_below":
         condition = vec < threshold
         index_choice = 0
     elif condition_type == "last_below":
         condition = vec < threshold
         index_choice = -1
     else:
@@ -83,10 +80,15 @@
     return None
 
 # %% ../../notebooks/properties/00_duration.ipynb 7
 AvailableMethod = Literal["distance", "derivative"]
 
 def calc_duration(ts: xr.DataArray, method: AvailableMethod = "distance", **kwargs):
     if method == "distance":
-        return ts_max_distance(ts, **kwargs)
+        result = np.sort(ts_max_distance(ts))
+        keys = ["t.d_start", "t.d_end"]
+
     elif method == "derivative":
-        return ts_max_derivative(ts, **kwargs)
+        result = ts_max_derivative(ts)
+        keys = ["t.d_start", "t.d_end", "t.d_time", "d_star_max"]
+
+    return dict(zip(keys, result))
```

### Comparing `discontinuitypy-0.0.1/discontinuitypy/propeties/mva.py` & `discontinuitypy-0.1.0/discontinuitypy/propeties/mva.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../notebooks/properties/00_mva.ipynb.
 
 # %% auto 0
-__all__ = ['minvar', 'calc_mva_features', 'fit_maxiumum_variance_direction', 'calc_candidate_mva_features']
+__all__ = ['minvar', 'calc_mva_features', 'calc_maxiumum_variance_direction', 'fit_maxiumum_variance_direction',
+           'calc_candidate_mva_features']
 
 # %% ../../notebooks/properties/00_mva.ipynb 1
 import xarray as xr
 import numpy as np
 import pandas as pd
-from datetime import timedelta
 
-from lmfit.models import StepModel, ConstantModel, Model
+from lmfit.models import StepModel, ConstantModel
 from lmfit import Parameters
 
+from typing import Literal
+
 # %% ../../notebooks/properties/00_mva.ipynb 3
-def minvar(data):
+def minvar(data: np.ndarray):
     """
     see `pyspedas.cotrans.minvar`
 
     This program computes the principal variance directions and variances of a
     vector quantity as well as the associated eigenvalues.
 
     Parameters
@@ -100,113 +102,154 @@
     # Maximum variance direction eigenvector
     Vl = v[:, 0]
     Vn = v[:, 2]
 
     vec_mag = np.linalg.norm(vrot, axis=1)
 
     # Compute changes in each component of B_rot
-    dvec = [vrot[0, i] - vrot[-1, i] for i in range(3)]
+    dvec = vrot[0] - vrot[-1]
 
     # Compute mean values
     vec_mag_mean = np.mean(vec_mag)
     vec_n_mean = np.mean(vrot[:, 2])
     VnOverVmag = vec_n_mean / vec_mag_mean
 
     # Compute relative changes in magnitude
     dvec_mag = vec_mag[-1] - vec_mag[0]
     dBOverB = np.abs(dvec_mag / vec_mag_mean)
     dBOverB_max = (np.max(vec_mag) - np.min(vec_mag)) / vec_mag_mean
+    
+    result = {
+        "Vl": Vl,
+        "Vn": Vn,
+        "b_mag": vec_mag_mean,
+        "b_n": vec_n_mean,
+        'B.vec.before': vrot[0],
+        'B.vec.after': vrot[-1],
+        'B.before': vec_mag[0],
+        'B.after': vec_mag[-1],
+        "db_mag": dvec_mag,
+        "bn_over_b": VnOverVmag,
+        "db_over_b": dBOverB,
+        "db_over_b_max": dBOverB_max,
+        "dB_lmn": dvec,
+    }
+    
+    result = pd.Series(result)
+    return result, vrot
+
+# %% ../../notebooks/properties/00_mva.ipynb 6
+def calc_maxiumum_variance_direction(data: xr.DataArray, datetime_unit="s", **kwargs):
+    d_data = data.differentiate("time", datetime_unit=datetime_unit)
+    return pd.Series({"d_star": abs(d_data).max(dim="time").item()})
 
-    output_names = [
-        "Vl",
-        "Vn",
-        "b_mag",
-        "b_n",
-        "db_mag",
-        "bn_over_b",
-        "db_over_b",
-        "db_over_b_max",
-        "dB_lmn",
-    ]
-
-    results = [
-        Vl,
-        Vn,
-        vec_mag_mean,
-        vec_n_mean,
-        dvec_mag,
-        VnOverVmag,
-        dBOverB,
-        dBOverB_max,
-        dvec,
-    ]
-
-    return pd.Series(results, index=output_names), vrot
-
-# %% ../../notebooks/properties/00_mva.ipynb 8
+# %% ../../notebooks/properties/00_mva.ipynb 9
 def fit_maxiumum_variance_direction(
-    ts: xr.DataArray, datetime_unit="s", return_best_fit: bool = True, **kwargs
+    data: xr.DataArray, datetime_unit="s", return_best_fit: bool = True, **kwargs
 ):
     """
     Fit maximum variance direction data by model
 
-    Note: 
+    Note:
         - see `datetime_to_numeric` in `xarray.core.duck_array_ops` for more details about converting datetime to numeric
         - Xarray uses the numpy dtypes datetime64[ns] and timedelta64[ns] to represent datetime data.
     """
-    time = ts["time"].values
+    time = data["time"].values
     x = (time - min(time)) / np.timedelta64(1, datetime_unit)
-    y = ts.values
+    y = data.values
 
-    xmin, xmax = min(x), max(x)
-    ymin, ymax = min(y), max(y)
+    x_min, x_max = min(x), max(x)
+    x_width = x_max - x_min
 
     # Create a model
     step_mod = StepModel(form="logistic")
     const_mod = ConstantModel()
     mod = step_mod + const_mod
 
     # Create parameters
     params = Parameters()
-    params.add("c", value=0)
-    params.add("center", value=(xmax + xmin) / 2.0, min=xmin, max=xmax)
-    params.add("amplitude", value=(ymax - ymin))
-    params.add("sigma", value=(xmax - xmin) / 7.0, min=0)
-
-    out = mod.fit(y, params, x=x)
-
-    amplitude = out.params["amplitude"].value
-    sigma = out.params["sigma"].value
-    center = out.params["center"].value
+
+    init_amplitude = y[-1] - y[0]
+
+    params.add(
+        "center",
+        value=(x_max + x_min) / 2.0,
+        # min=x_min + x_width / 7.0,
+        # max=x_max - x_width / 7.0,
+    )
+    params.add(
+        "amplitude",
+        value=init_amplitude,
+        max=abs(init_amplitude) * 2.0,
+        min=-abs(init_amplitude) * 2.0,
+    )
+    params.add("sigma", value=x_width / 7.0, min=0)
+
+    if True:
+        int_center_y = (y[-1] + y[0]) / 2.0
+        c1 = 1 / 8
+        params.add(
+            "center_y",
+            min=int_center_y - c1 * np.abs(init_amplitude),
+            max=int_center_y + c1 * np.abs(init_amplitude),
+        )
+        params.add("c", expr="center_y - amplitude / 2.0")
+
+    # Ensure there are enough data points to fit the model
+    if len(y) < 4:
+        # Not enough data points, return None or an empty result instead of raising an error
+        amplitude = np.nan
+        sigma = np.nan
+        center = np.nan
+        rsquared = np.nan
+        chisqr = np.nan
+        c = np.nan
+        best_fit = np.nan
+    else:
+        out = mod.fit(y, params, x=x)
+        amplitude = out.params["amplitude"].value
+        sigma = out.params["sigma"].value
+        center = out.params["center"].value
+        c = out.params["c"].value
+        rsquared = out.rsquared
+        chisqr = out.chisqr
+        best_fit = out.best_fit
+
     max_df = amplitude / (4 * sigma)
 
-    d_time = min(time) + center * np.timedelta64(1, datetime_unit).astype("timedelta64[ns]")
+    d_time = min(time) + center * np.timedelta64(1, datetime_unit).astype(
+        "timedelta64[ns]"
+    )
 
     result = pd.Series(
         {
             "fit.vars.amplitude": amplitude,
             "fit.vars.sigma": sigma,
-            "d_time": d_time,
+            "t.d_time": d_time,
             "d_star": max_df,
-            "fit.vars.c": out.params["c"].value,
-            "fit.stat.rsquared": out.rsquared,
-            "fit.stat.chisqr": out.chisqr,
+            "fit.vars.c": c,
+            "fit.stat.rsquared": rsquared,
+            "fit.stat.chisqr": chisqr,
         }
     )
     if return_best_fit:
-        result["fit.best_fit"] = out.best_fit
+        result["fit.best_fit"] = best_fit
         result["fit.time"] = time
     return result
 
-# %% ../../notebooks/properties/00_mva.ipynb 9
-def calc_candidate_mva_features(event, data: xr.DataArray, **kwargs):
-    event_data = data.sel(time=slice(event["d_tstart"], event["d_tstop"]))
+# %% ../../notebooks/properties/00_mva.ipynb 10
+def calc_candidate_mva_features(
+    event, data: xr.DataArray, method=Literal["fit", "derivative"], **kwargs
+):
+    event_data = data.sel(time=slice(event["t.d_start"], event["t.d_end"]))
 
     mva_features, vrot = calc_mva_features(event_data.to_numpy())
 
     event_data_l = xr.DataArray(
         vrot[:, 0], dims=["time"], coords={"time": event_data.time}
     )
 
-    fit_result = fit_maxiumum_variance_direction(event_data_l, **kwargs)
-
-    return pd.concat([mva_features, fit_result])
+    if method == "fit":
+        result = fit_maxiumum_variance_direction(event_data_l, **kwargs)
+    elif method == "derivative":
+        result = calc_maxiumum_variance_direction(event_data_l, **kwargs)
+    return pd.concat([mva_features, result])
```

### Comparing `discontinuitypy-0.0.1/discontinuitypy/utils/analysis.py` & `discontinuitypy-0.1.0/discontinuitypy/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `discontinuitypy-0.0.1/discontinuitypy/utils/basic.py` & `discontinuitypy-0.1.0/discontinuitypy/utils/basic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../notebooks/utils/00_basic.ipynb.
 
 # %% auto 0
-__all__ = ['load_catalog', 'load_params', 'DF_TYPE', 'pmap', 'DataConfig', 'filter_tranges', 'filter_tranges_df', 'pl_norm',
-           'partition_data_by_ts', 'partition_data_by_year', 'partition_data_by_year_month', 'partition_data_by_time',
-           'concat_df', 'concat_partitions', 'format_timedelta', 'resample', 'df2ts', 'calc_vec_mag', 'check_fgm']
+__all__ = ['DF_TYPE', 'filter_tranges', 'filter_tranges_df', 'partition_data_by_ts', 'partition_data_by_year',
+           'partition_data_by_year_month', 'partition_data_by_time', 'concat_df', 'concat_partitions',
+           'format_timedelta', 'resample', 'df2ts', 'calc_vec_mag', 'check_fgm']
 
 # %% ../../notebooks/utils/00_basic.ipynb 1
-from .. import ROOT_DIR
-from .kedro import load_context
-
-from functools import partial
-
 from typing import overload
 
-# %% ../../notebooks/utils/00_basic.ipynb 2
-load_catalog = partial(load_context, project_path=ROOT_DIR, catalog_only=True)
-load_params = partial(load_context, project_path=ROOT_DIR, params_only=True)
-
-# %% ../../notebooks/utils/00_basic.ipynb 4
+# %% ../../notebooks/utils/00_basic.ipynb 3
 import polars as pl
 import polars.selectors as cs
 
 import pandas as pd
 import xarray as xr
 
 import pandas
@@ -33,41 +24,18 @@
 from loguru import logger
 
 from xarray import DataArray
 from typing import Union, Collection, Callable, Optional, Tuple
 from typing import Any, Dict
 
 
-# %% ../../notebooks/utils/00_basic.ipynb 5
-from pipe import select
-from fastcore.utils import partial
-
 # %% ../../notebooks/utils/00_basic.ipynb 6
-def pmap(func, *args, **kwargs):
-    """
-    map with `partial`
-    """
-    return select(partial(func, *args, **kwargs))
-
-# %% ../../notebooks/utils/00_basic.ipynb 9
-from pydantic import BaseModel
-from datetime import datetime, timedelta
-from pandas import Timedelta
-
-class DataConfig(BaseModel):
-    sat_id: str = None
-    start: datetime = None
-    end: datetime = None
-    ts: timedelta = None
-    coord: str = None
-
-# %% ../../notebooks/utils/00_basic.ipynb 11
 from fastcore.utils import patch
 
-# %% ../../notebooks/utils/00_basic.ipynb 12
+# %% ../../notebooks/utils/00_basic.ipynb 7
 def filter_tranges(time: pl.Series, tranges: Tuple[list, list]):
     """
     - Filter data by time ranges, return the indices of the time that are in the time ranges (left inclusive, right exclusive)
     """
 
     starts = tranges[0]
     ends = tranges[1]
@@ -87,20 +55,20 @@
     - Filter data by time ranges
     """
 
     time = df[time_col]
     filtered_indices = filter_tranges(time, tranges)
     return df[filtered_indices]
 
-# %% ../../notebooks/utils/00_basic.ipynb 13
+# %% ../../notebooks/utils/00_basic.ipynb 8
 @patch
 def plot(self:pl.DataFrame, *args, **kwargs):
     return self.to_pandas().plot(*args, **kwargs)
 
-# %% ../../notebooks/utils/00_basic.ipynb 14
+# %% ../../notebooks/utils/00_basic.ipynb 9
 def _expand_selectors(items: Any, *more_items: Any) -> list[Any]:
     """
     See `_expand_selectors` in `polars`.
     """
     expanded: list[Any] = []
     for item in (
         *(
@@ -109,30 +77,15 @@
             else [items]
         ),
         *more_items,
     ):
         expanded.append(item)
     return expanded
 
-def pl_norm(columns, *more_columns) -> pl.Expr:
-    """
-    Computes the square root of the sum of squares for the given columns.
-
-    Args:
-    *columns (str): Names of the columns.
-
-    Returns:
-    pl.Expr: Expression representing the square root of the sum of squares.
-    """
-    all_columns = _expand_selectors(columns, *more_columns)
-    squares = [pl.col(column).pow(2) for column in all_columns]
-
-    return sum(squares).sqrt()
-
-# %% ../../notebooks/utils/00_basic.ipynb 16
+# %% ../../notebooks/utils/00_basic.ipynb 11
 def partition_data_by_ts(df: pl.DataFrame, ts: timedelta) -> Dict[str, pl.DataFrame]:
     """Partition the dataset by time
 
     Args:
         df: Input DataFrame.
         ts: Time interval.
 
@@ -190,15 +143,15 @@
         return partition_data_by_year(df)
     elif method == "year_month":
         return partition_data_by_year_month(df)
     else:
         ts = pd.Timedelta(method)
         return partition_data_by_ts(df, ts)
 
-# %% ../../notebooks/utils/00_basic.ipynb 17
+# %% ../../notebooks/utils/00_basic.ipynb 12
 DF_TYPE = Union[pl.DataFrame, pl.LazyFrame, pd.DataFrame]
 def concat_df(dfs: list[DF_TYPE]) -> DF_TYPE:
     """Concatenate a list of DataFrames into one DataFrame.
     """
     
     match type(dfs[0]):
         case pl.DataFrame | pl.LazyFrame:
@@ -219,27 +172,27 @@
     partitions_data = [
         partition_load_func() for partition_load_func in partitioned_input.values()
     ]  # load the actual partition data
     
     result = concat_df(partitions_data)
     return result
 
-# %% ../../notebooks/utils/00_basic.ipynb 19
+# %% ../../notebooks/utils/00_basic.ipynb 14
 def format_timedelta(time):
     """Format timedelta to `timedelta`"""
     if isinstance(time, timedelta):
         return time
     elif isinstance(time, str):
         return pd.Timedelta(time)
     elif isinstance(time, int):
         return pd.Timedelta(seconds=time)
     else:
         raise TypeError(f"Unsupported type: {type(time)}")
 
-# %% ../../notebooks/utils/00_basic.ipynb 20
+# %% ../../notebooks/utils/00_basic.ipynb 15
 @overload
 def resample(
     df: pl.DataFrame,
     every: timedelta,
     period: timedelta = None,
     offset: timedelta = None,
     shift: timedelta = None,
@@ -274,55 +227,55 @@
     return (
         df.sort(time_column)
         .group_by_dynamic(time_column, every=every, period=period, offset=offset)
         .agg(cs.numeric().mean())
         .with_columns((pl.col(time_column) + shift))
     )
 
-# %% ../../notebooks/utils/00_basic.ipynb 21
+# %% ../../notebooks/utils/00_basic.ipynb 16
 def df2ts(
     df: Union[pandas.DataFrame, pl.DataFrame, pl.LazyFrame],
-    cols = None,
-    time_col = "time",
+    cols=None,
+    time_col="time",
     attrs=None,
     name=None,
 ):
     """Convert DataFrame to TimeSeries"""
-    
+
     if cols is None:
         if isinstance(df, (pl.DataFrame, pl.LazyFrame)):
             cols = df.columns
             cols.remove(time_col)
         else:
             cols = df.columns.tolist()
-    
+
     if isinstance(df, pl.LazyFrame):
         df = df.collect()
 
     # Prepare data
     data = df[cols].to_numpy()
 
     # Prepare coordinates
     time = df.index if isinstance(df, pandas.DataFrame) else df[time_col]
     if isinstance(cols, str) and len(data.shape) > 1:
         element_len = data.shape[1]
         v_dim = [cols + str(i) for i in range(element_len)]
     else:
         v_dim = cols
-        
+
     # Create the DataArray
     coords = {"time": time, "v_dim": v_dim}
 
     return xr.DataArray(data, coords=coords, attrs=attrs, name=name)
 
 
 def calc_vec_mag(vec) -> DataArray:
     return linalg.norm(vec, dims="v_dim")
 
-# %% ../../notebooks/utils/00_basic.ipynb 22
+# %% ../../notebooks/utils/00_basic.ipynb 17
 def check_fgm(vec: xr.DataArray):
     # check if time is monotonic increasing
     logger.info("Check if time is monotonic increasing")
     assert vec.time.to_series().is_monotonic_increasing
     # check available time difference
     logger.info(
         f"Available time delta: {vec.time.diff(dim='time').to_series().unique()}"
```

### Comparing `discontinuitypy-0.0.1/discontinuitypy/utils/plot.py` & `discontinuitypy-0.1.0/discontinuitypy/utils/plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../notebooks/utils/01_plotting.ipynb.
 
 # %% auto 0
-__all__ = ['savefig', 'time_stamp', 'setup_mva_plot', 'plot_candidate']
+__all__ = ['time_stamp', 'setup_mva_plot', 'plot_candidate']
 
-# %% ../../notebooks/utils/01_plotting.ipynb 1
+# %% ../../notebooks/utils/01_plotting.ipynb 0
 import matplotlib.pyplot as plt
 
-# %% ../../notebooks/utils/01_plotting.ipynb 2
-def savefig(name, **kwargs):
-    plt.savefig(f"../figures/{name}.png", bbox_inches="tight", **kwargs)
-    plt.savefig(f"../figures/{name}.pdf", bbox_inches="tight", **kwargs)
-
-# %% ../../notebooks/utils/01_plotting.ipynb 4
 import xarray as xr
 import pandas as pd
 from datetime import datetime
 
 from pyspedas.cotrans.minvar_matrix_make import minvar_matrix_make
 from pyspedas import tvector_rotate
 from pyspedas.analysis.tvectot import tvectot
 
 from pytplot import tplot
-from pytplot import store_data, get_data, split_vec, join_vec
-from pytplot import timebar, highlight, degap, options
-
+from pytplot import store_data
+from pytplot import timebar, degap, options
 
-# %% ../../notebooks/utils/01_plotting.ipynb 5
-import matplotlib.pyplot as plt
-from .plot import savefig
+from matplotlib.pyplot import Axes
 
+# %% ../../notebooks/utils/01_plotting.ipynb 2
 try:
     import scienceplots
     plt.style.use(['science', 'nature', 'notebook'])
 except ImportError:
     pass
 
-# %% ../../notebooks/utils/01_plotting.ipynb 6
+# %% ../../notebooks/utils/01_plotting.ipynb 3
 def time_stamp(ts):
     "Return POSIX timestamp as float."
     return pd.Timestamp(ts, tz="UTC").timestamp()
 
 
 def setup_mva_plot(
     data: xr.DataArray,
@@ -65,90 +57,122 @@
     
     tvar2plot = tvectot(tvar, join_component=True)
     legend_names = legend_names + [r"$B_{total}$"]
 
     options(tvar2plot, "ytitle", "$B$")
     options(tvar2plot, "ysubtitle", ysubtitle)
     options(tvar2plot, "legend_names", legend_names)
-    
-    options(tvar2plot, "thick", 2)
-    options(tvar2plot, "char_size", 16)
-    
-    # tstart_ts = time_stamp(tstart)
-    # tstop_ts = time_stamp(tstop)
-    # highlight(tvar2plot, [tstart_ts, tstop_ts])
+
     degap(tvar2plot)
     return tvar2plot
 
-# %% ../../notebooks/utils/01_plotting.ipynb 8
-from matplotlib import lines
-
+# %% ../../notebooks/utils/01_plotting.ipynb 5
+from pyspedas.analysis.deriv_data import deriv_data
+from ..integration import J_FACTOR
+import pytplot
+from pytplot import split_vec
 
 def plot_candidate(
-    candidate: dict,
+    event: dict,
     data: xr.DataArray,
+    add_ids_properties=True,
+    plot_current_density=False,
+    plot_fit_data=False,
     add_timebars=True,
     add_plasma_params=False,
-    plot_fit_data=False,
     **kwargs,
 ):
-    if pd.notnull(candidate.get("d_tstart")) and pd.notnull(candidate.get("d_tstop")):
+    if pd.notnull(event.get("t.d_start")) and pd.notnull(event.get("t.d_end")):
         tvar = setup_mva_plot(
             data,
-            candidate["tstart"],
-            candidate["tstop"],
-            candidate["d_tstart"],
-            candidate["d_tstop"],
+            event["tstart"],
+            event["tstop"],
+            event["t.d_start"],
+            event["t.d_end"],
         )
     else:
-        tvar = setup_mva_plot(data, candidate["tstart"], candidate["tstop"])
+        tvar = setup_mva_plot(data, event["tstart"], event["tstop"])
+    
+    tvars2plot = [tvar]
+
+    if plot_current_density:
+        Bl = split_vec(tvar)[0]
+        dBldt = deriv_data(Bl)[0]
+        v_k = event.get("v_k")
+        pytplot.data_quants[dBldt] = pytplot.data_quants[dBldt] / v_k * J_FACTOR.value
+        tvars2plot.append(dBldt)
+        
+        options(dBldt, "ytitle", "$J$")
+        options(dBldt, "ysubtitle", "[nA/m$^2$]")
+        options(dBldt, "legend_names", "$J_m$")
 
     if add_timebars:
-        d_time = candidate.get("d_time")
-        d_start = candidate.get("d_tstart")
-        d_stop = candidate.get("d_tstop")
+        d_time = event.get("t.d_time")
+        d_start = event.get("t.d_start")
+        d_stop = event.get("t.d_end")
 
         if d_time:
             timebar(time_stamp(d_time), color="red")
         if d_start and pd.notnull(d_start):
             timebar(time_stamp(d_start))
         if d_stop and pd.notnull(d_stop):
             timebar(time_stamp(d_stop))
 
     title = ""
     
+    if add_ids_properties:
+        thickness = event.get("L_k")
+        current_density = event.get("j0_k")
+        title += "#Discontinuity properties# "
+        if thickness:
+            title += rf"$L: {thickness:.2f} \mathrm{{km}}$"
+        if current_density:
+            title += rf", $j: {current_density:.2f} \mathrm{{nA/m}}^2$"
+    
     if add_plasma_params:
-        plasma_speed = candidate.get("plasma_speed")
-        plasma_density = candidate.get("plasma_density")
-        plasma_temperature = candidate.get("plasma_temperature")
+        plasma_speed = event.get("plasma_speed")
+        plasma_density = event.get("plasma_density")
+        plasma_temperature = event.get("plasma_temperature")
 
-        title += "#Plasma parameters# "
+        title += "\n#Plasma parameters# "
         if plasma_speed:
             title += rf"$V_i: {plasma_speed:.2f} \mathrm{{km/s}}$"
         if plasma_density:
             title += rf", $n_i: {plasma_density:.2f} \mathrm{{cm}}^{{-3}}$"
         if plasma_temperature:
             title += rf", $T_i: {plasma_temperature:.2f} \mathrm{{eV}}$"
 
         # options(tvar, "title", title)
+        
+    for tvar2plot in tvars2plot:
+        options(tvar2plot, "thick", 2)
+        options(tvar2plot, "char_size", 16)
+
+    fig, axes = tplot(tvars2plot, return_plot_objects=True)
+    if isinstance(axes, Axes):
+        axes = [axes]
 
-    fig, axes = tplot(tvar, return_plot_objects=True, **kwargs)
+    base_axis = axes[0]
 
     if plot_fit_data:
-        fit_data = candidate.get("fit.best_fit")
-        fit_time = candidate.get("fit.time")
+        fit_data = event.get("fit.best_fit")
+        fit_time = event.get("fit.time")
 
-        c = candidate.get("fit.vars.c")
-        amp = candidate.get("fit.vars.amplitude")
+        c = event.get("fit.vars.c")
+        amp = event.get("fit.vars.amplitude")
+        sigma = event.get('fit.vars.sigma')
         
-        d_star = candidate.get("d_star")
-        rsquared = candidate.get("fit.stat.rsquared")
-        chisqr = candidate.get("fit.stat.chisqr")
-
-        plt.plot(d_time, c + amp / 2, marker="o", markersize=10, color="red")
-        plt.plot(fit_time, fit_data, label="Fit", color="black", linestyle="--")
+        d_star = event.get("d_star")
+        rsquared = event.get("fit.stat.rsquared")
+        chisqr = event.get("fit.stat.chisqr")
+        
+        base_axis.plot(d_time, c + amp / 2, marker="o", markersize=10, color="red")
+        if fit_time is not None and fit_data is not None:
+            base_axis.plot(fit_time, fit_data, label="Fit", color="black", linestyle="--")
         
         title += f"\n#Fit# $\max dB/dt$: {d_star:.2f}, $R^2$: {rsquared:.2f}, $\chi^2$: {chisqr:.2f}"
-    
-    plt.title(title)
+        title += f"\n#Fit# $c$: {c:.2f}, $Amp$: {amp:.2f}, $\Sigma$: {sigma:.2f}"
+
+    # add title to the first plot
+    base_axis.set_title(title)
 
     return fig, axes
```

