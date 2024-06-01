# Comparing `tmp/dcnum-0.20.4.tar.gz` & `tmp/dcnum-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.20.4.tar", last modified: Fri May 31 08:57:40 2024, max compression
+gzip compressed data, was "dcnum-0.21.0.tar", last modified: Sat Jun  1 15:31:39 2024, max compression
```

## Comparing `dcnum-0.20.4.tar` & `dcnum-0.21.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.760693 dcnum-0.20.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.740693 dcnum-0.20.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-31 08:57:35.000000 dcnum-0.20.4/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-31 08:57:35.000000 dcnum-0.20.4/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-31 08:57:35.000000 dcnum-0.20.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 08:57:35.000000 dcnum-0.20.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-05-31 08:57:35.000000 dcnum-0.20.4/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-31 08:57:35.000000 dcnum-0.20.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-31 08:57:40.760693 dcnum-0.20.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-31 08:57:35.000000 dcnum-0.20.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-31 08:57:35.000000 dcnum-0.20.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-31 08:57:35.000000 dcnum-0.20.4/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-31 08:57:35.000000 dcnum-0.20.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 08:57:35.000000 dcnum-0.20.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-31 08:57:35.000000 dcnum-0.20.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:57:40.760693 dcnum-0.20.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.740693 dcnum-0.20.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/src/dcnum/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/src/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)    20709 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/feat/feat_contour/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_contour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_contour/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_contour/moments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_contour/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15700 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34792 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/logic/ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/logic/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/logic/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/meta/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/hdf5_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/mapped.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.752693 dcnum-0.20.4/src/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.752693 dcnum-0.20.4/src/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.760693 dcnum-0.20.4/src/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.756693 dcnum-0.20.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.760693 dcnum-0.20.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
--rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_shapein_empty.zip
--rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_background_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_background_bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_background_bg_sparsemed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_event_extractor_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_moments_based_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_logic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_logic_join.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_logic_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    37009 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_logic_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_bg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_feat.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_hdf5_basins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_hdf5_index_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_segm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_segm_no_mask_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_write_queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.198604 dcnum-0.21.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.178604 dcnum-0.21.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.178604 dcnum-0.21.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-06-01 15:31:35.000000 dcnum-0.21.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-06-01 15:31:35.000000 dcnum-0.21.0/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-06-01 15:31:35.000000 dcnum-0.21.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-01 15:31:35.000000 dcnum-0.21.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-06-01 15:31:35.000000 dcnum-0.21.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-01 15:31:35.000000 dcnum-0.21.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-06-01 15:31:39.198604 dcnum-0.21.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-06-01 15:31:35.000000 dcnum-0.21.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.182604 dcnum-0.21.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-06-01 15:31:35.000000 dcnum-0.21.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.182604 dcnum-0.21.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-06-01 15:31:35.000000 dcnum-0.21.0/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-01 15:31:35.000000 dcnum-0.21.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-01 15:31:35.000000 dcnum-0.21.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-01 15:31:35.000000 dcnum-0.21.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 15:31:39.198604 dcnum-0.21.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.178604 dcnum-0.21.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.182604 dcnum-0.21.0/src/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-01 15:31:39.000000 dcnum-0.21.0/src/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.182604 dcnum-0.21.0/src/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.182604 dcnum-0.21.0/src/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_background/bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20709 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.182604 dcnum-0.21.0/src/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.182604 dcnum-0.21.0/src/dcnum/feat/feat_contour/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_contour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_contour/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_contour/moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_contour/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.186604 dcnum-0.21.0/src/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15700 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.186604 dcnum-0.21.0/src/dcnum/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34792 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/logic/ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/logic/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/logic/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.186604 dcnum-0.21.0/src/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/meta/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.186604 dcnum-0.21.0/src/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/read/hdf5_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/read/mapped.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.186604 dcnum-0.21.0/src/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.186604 dcnum-0.21.0/src/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-06-01 15:31:35.000000 dcnum-0.21.0/src/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.194604 dcnum-0.21.0/src/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-06-01 15:31:39.000000 dcnum-0.21.0/src/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-06-01 15:31:39.000000 dcnum-0.21.0/src/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 15:31:39.000000 dcnum-0.21.0/src/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-01 15:31:39.000000 dcnum-0.21.0/src/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 15:31:39.000000 dcnum-0.21.0/src/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.194604 dcnum-0.21.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:31:39.194604 dcnum-0.21.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/data/fmt-hdf5_shapein_empty.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_background_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_background_bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_background_bg_sparsemed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_event_extractor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_moments_based_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_feat_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_logic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_logic_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_logic_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37009 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_logic_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_meta_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_meta_ppid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_meta_ppid_bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_meta_ppid_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_meta_ppid_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_meta_ppid_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_meta_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_read_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_read_hdf5_basins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_read_hdf5_index_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_segm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_segm_no_mask_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_write_queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-06-01 15:31:35.000000 dcnum-0.21.0/tests/test_write_writer.py
```

### Comparing `dcnum-0.20.4/.github/workflows/check.yml` & `dcnum-0.21.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/.github/workflows/deploy_pypi.yml` & `dcnum-0.21.0/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/.gitignore` & `dcnum-0.21.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/CHANGELOG` & `dcnum-0.21.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.21.0
+ - fix: GPUSegmenter did not perform mask postprocessing
+ - ref: enable mask postprocessing by default for all segmenters
+ - ref: increment DCNUM_PPID_GENERATION to 9
 0.20.4
  - fix: slot_chunks were not performed in increasing order, making it
    impossible for writer to continue writing and consequent OOM
  - enh: reserve one CPU for writer thread and control logic
  - enh: disentangle logging and debugging keyword arguments
  - enh: do not initialize slot_chunks and slot_states with lock
 0.20.3
```

### Comparing `dcnum-0.20.4/LICENSE` & `dcnum-0.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/PKG-INFO` & `dcnum-0.21.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.20.4
+Version: 0.21.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.20.4/README.rst` & `dcnum-0.21.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/docs/conf.py` & `dcnum-0.21.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/docs/extensions/github_changelog.py` & `dcnum-0.21.0/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/pyproject.toml` & `dcnum-0.21.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.21.0/src/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/feat_background/base.py` & `dcnum-0.21.0/src/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/feat_background/bg_copy.py` & `dcnum-0.21.0/src/dcnum/feat/feat_background/bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.21.0/src/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.21.0/src/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.21.0/src/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/feat_contour/moments.py` & `dcnum-0.21.0/src/dcnum/feat/feat_contour/moments.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/feat_contour/volume.py` & `dcnum-0.21.0/src/dcnum/feat/feat_contour/volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.21.0/src/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/gate.py` & `dcnum-0.21.0/src/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/feat/queue_event_extractor.py` & `dcnum-0.21.0/src/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/logic/ctrl.py` & `dcnum-0.21.0/src/dcnum/logic/ctrl.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/logic/job.py` & `dcnum-0.21.0/src/dcnum/logic/job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/logic/json_encoder.py` & `dcnum-0.21.0/src/dcnum/logic/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/meta/paths.py` & `dcnum-0.21.0/src/dcnum/meta/paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/meta/ppid.py` & `dcnum-0.21.0/src/dcnum/meta/ppid.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pathlib
 from typing import Dict, List, Protocol
 import warnings
 
 
 #: Increment this string if there are breaking changes that make
 #: previous pipelines unreproducible.
-DCNUM_PPID_GENERATION = "8"
+DCNUM_PPID_GENERATION = "9"
 
 
 class ClassWithPPIDCapabilities(Protocol):
     def get_ppid(self) -> str:
         """full pipeline identifier for the class (instance method)"""
         pass
```

### Comparing `dcnum-0.20.4/src/dcnum/read/cache.py` & `dcnum-0.21.0/src/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/read/hdf5_data.py` & `dcnum-0.21.0/src/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/read/mapped.py` & `dcnum-0.21.0/src/dcnum/read/mapped.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/segm/segm_thresh.py` & `dcnum-0.21.0/src/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/segm/segmenter.py` & `dcnum-0.21.0/src/dcnum/segm/segmenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class Segmenter(abc.ABC):
     #: Required hardware ("cpu" or "gpu") defined in first-level subclass.
     hardware_processor = "none"
     #: Whether to enable mask post-processing. If disabled, you should
     #: make sure that your mask is properly defined and cleaned or you
     #: have to call `process_mask` in your `segment_approach` implementation.
-    mask_postprocessing = False
+    mask_postprocessing = True
     #: Default keyword arguments for mask post-processing. See `process_mask`
     #: for available options.
     mask_default_kwargs = {}
     #: If the segmenter requires a background-corrected image, set this to True
     requires_background_correction = False
 
     def __init__(self,
```

### Comparing `dcnum-0.20.4/src/dcnum/segm/segmenter_cpu.py` & `dcnum-0.21.0/src/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/segm/segmenter_gpu.py` & `dcnum-0.21.0/src/dcnum/segm/segmenter_gpu.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 
 from .segmenter import Segmenter
 
 
 class GPUSegmenter(Segmenter, abc.ABC):
     hardware_processor = "gpu"
-    mask_postprocessing = False
 
     def __init__(self,
                  *,
                  num_workers: int = None,
                  kwargs_mask: Dict = None,
                  debug: bool = False,
                  **kwargs
```

### Comparing `dcnum-0.20.4/src/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.21.0/src/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/write/deque_writer_thread.py` & `dcnum-0.21.0/src/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/write/queue_collector_thread.py` & `dcnum-0.21.0/src/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum/write/writer.py` & `dcnum-0.21.0/src/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/src/dcnum.egg-info/PKG-INFO` & `dcnum-0.21.0/src/dcnum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.20.4
+Version: 0.21.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.20.4/src/dcnum.egg-info/SOURCES.txt` & `dcnum-0.21.0/src/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/conftest.py` & `dcnum-0.21.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip` & `dcnum-0.21.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.21.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip` & `dcnum-0.21.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.21.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/data/fmt-hdf5_shapein_empty.zip` & `dcnum-0.21.0/tests/data/fmt-hdf5_shapein_empty.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip` & `dcnum-0.21.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/helper_methods.py` & `dcnum-0.21.0/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_background_base.py` & `dcnum-0.21.0/tests/test_feat_background_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_background_bg_copy.py` & `dcnum-0.21.0/tests/test_feat_background_bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.21.0/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_background_bg_sparsemed.py` & `dcnum-0.21.0/tests/test_feat_background_bg_sparsemed.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_brightness.py` & `dcnum-0.21.0/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_event_extractor_manager.py` & `dcnum-0.21.0/tests/test_feat_event_extractor_manager.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_gate.py` & `dcnum-0.21.0/tests/test_feat_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_haralick.py` & `dcnum-0.21.0/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_moments_based.py` & `dcnum-0.21.0/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_moments_based_extended.py` & `dcnum-0.21.0/tests/test_feat_moments_based_extended.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_feat_volume.py` & `dcnum-0.21.0/tests/test_feat_volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_logic_job.py` & `dcnum-0.21.0/tests/test_logic_job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_logic_join.py` & `dcnum-0.21.0/tests/test_logic_join.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_logic_pipeline.py` & `dcnum-0.21.0/tests/test_logic_pipeline.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_meta_paths.py` & `dcnum-0.21.0/tests/test_meta_paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_meta_ppid_base.py` & `dcnum-0.21.0/tests/test_meta_ppid_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_meta_ppid_bg.py` & `dcnum-0.21.0/tests/test_meta_ppid_bg.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_meta_ppid_data.py` & `dcnum-0.21.0/tests/test_meta_ppid_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_meta_ppid_feat.py` & `dcnum-0.21.0/tests/test_meta_ppid_feat.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_meta_ppid_gate.py` & `dcnum-0.21.0/tests/test_meta_ppid_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_meta_ppid_segm.py` & `dcnum-0.21.0/tests/test_meta_ppid_segm.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_read_basin.py` & `dcnum-0.21.0/tests/test_read_basin.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_read_concat_hdf5.py` & `dcnum-0.21.0/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_read_hdf5.py` & `dcnum-0.21.0/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_read_hdf5_basins.py` & `dcnum-0.21.0/tests/test_read_hdf5_basins.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_read_hdf5_index_mapping.py` & `dcnum-0.21.0/tests/test_read_hdf5_index_mapping.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_segm_base.py` & `dcnum-0.21.0/tests/test_segm_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 
     def get_chunk(self, chunk_index):
         image = np.array(-(10 + chunk_index) * self.mask, dtype=np.int16)
         chunk = np.stack([image] * 100, dtype=np.int16)
         return chunk
 
 
+def test_segmenter_properties():
+    assert segm.CPUSegmenter.mask_postprocessing  # sanity check
+    assert segm.GPUSegmenter.mask_postprocessing  # fixed in 0.21.0
+    assert segm.Segmenter.mask_postprocessing  # new default in 0.21.0
+
+
 def test_segmenter_labeled_mask():
     mask = np.array([
         [0, 0, 0, 0, 0, 0, 0, 0],
         [0, 0, 1, 1, 1, 0, 0, 0],
         [0, 0, 1, 0, 1, 0, 0, 0],  # filled, 1
         [0, 0, 1, 1, 1, 0, 0, 0],
         [0, 0, 0, 0, 0, 0, 0, 0],
```

### Comparing `dcnum-0.20.4/tests/test_segm_no_mask_proc.py` & `dcnum-0.21.0/tests/test_segm_no_mask_proc.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_segm_thresh.py` & `dcnum-0.21.0/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_write_deque_writer_thread.py` & `dcnum-0.21.0/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_write_queue_collector_thread.py` & `dcnum-0.21.0/tests/test_write_queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.4/tests/test_write_writer.py` & `dcnum-0.21.0/tests/test_write_writer.py`

 * *Files identical despite different names*

