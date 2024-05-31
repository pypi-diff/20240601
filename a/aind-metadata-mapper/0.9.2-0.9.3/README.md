# Comparing `tmp/aind_metadata_mapper-0.9.2.tar.gz` & `tmp/aind_metadata_mapper-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_mapper-0.9.2.tar", last modified: Fri May 31 17:45:29 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.9.3.tar", last modified: Fri May 31 18:53:21 2024, max compression
```

## Comparing `aind_metadata_mapper-0.9.2.tar` & `aind_metadata_mapper-0.9.3.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.200739 aind_metadata_mapper-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.172739 aind_metadata_mapper-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.176739 aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.176739 aind_metadata_mapper-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-31 17:45:29.200739 aind_metadata_mapper-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.176739 aind_metadata_mapper-0.9.2/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/scripts/singularity_build.def
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:45:29.200739 aind_metadata_mapper-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.172739 aind_metadata_mapper-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/exaspim/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/exaspim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/fip/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/fip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/fip/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/gather_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.176739 aind_metadata_mapper-0.9.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.188738 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/sync_rig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.188738 aind_metadata_mapper-0.9.2/tests/resources/fip/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/fip/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/fip/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/fip/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.188738 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_funding_multiple_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_funding_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_procedures_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_subject_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.188738 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/acquisition.json
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/data_description.json
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/instrument.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)    20774 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/session.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.192739 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.192739 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.192739 aind_metadata_mapper-0.9.2/tests/resources/smartspim/
--rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_ASI_logging_afternoon.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_ASI_logging_morning.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38440 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/smartspim/local_json.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_bergamo/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_fip/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_fip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_fip/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    28919 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_gather_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_legacy_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_mesoscope/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_open_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_open_ephys/test_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_open_ephys/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_smartspim/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_smartspim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_smartspim/test_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_smartspim/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.303392 aind_metadata_mapper-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.275391 aind_metadata_mapper-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.279392 aind_metadata_mapper-0.9.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.279392 aind_metadata_mapper-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-31 18:53:21.303392 aind_metadata_mapper-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.283392 aind_metadata_mapper-0.9.3/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.283392 aind_metadata_mapper-0.9.3/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.283392 aind_metadata_mapper-0.9.3/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.283392 aind_metadata_mapper-0.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.283392 aind_metadata_mapper-0.9.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:53:21.303392 aind_metadata_mapper-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.275391 aind_metadata_mapper-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.283392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.283392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.287392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.287392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/exaspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/exaspim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.287392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/fip/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/fip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/fip/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.287392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.287392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/open_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/open_ephys/rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/open_ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.287392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/smartspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/smartspim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/smartspim/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/smartspim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.303392 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-31 18:53:21.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-31 18:53:21.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:53:21.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 18:53:21.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 18:53:21.000000 aind_metadata_mapper-0.9.3/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.287392 aind_metadata_mapper-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.279392 aind_metadata_mapper-0.9.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.291391 aind_metadata_mapper-0.9.3/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.291391 aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/sync_rig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.291391 aind_metadata_mapper-0.9.3/tests/resources/fip/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/fip/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/fip/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/fip/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.291391 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/example_funding_multiple_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/example_funding_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.295392 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/acquisition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/instrument.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20774 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.295392 aind_metadata_mapper-0.9.3/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.299392 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.299392 aind_metadata_mapper-0.9.3/tests/resources/smartspim/
+-rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/smartspim/example_ASI_logging_afternoon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/smartspim/example_ASI_logging_morning.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38440 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/smartspim/example_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/resources/smartspim/local_json.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.299392 aind_metadata_mapper-0.9.3/tests/test_bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_bergamo/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.299392 aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.299392 aind_metadata_mapper-0.9.3/tests/test_fip/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_fip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_fip/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30506 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_legacy_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.299392 aind_metadata_mapper-0.9.3/tests/test_mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_mesoscope/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.303392 aind_metadata_mapper-0.9.3/tests/test_open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_open_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_open_ephys/test_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_open_ephys/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:53:21.303392 aind_metadata_mapper-0.9.3/tests/test_smartspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_smartspim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_smartspim/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-31 18:53:10.000000 aind_metadata_mapper-0.9.3/tests/test_smartspim/test_utils.py
```

### Comparing `aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.9.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/.github/workflows/tag_and_publish.yml` & `aind_metadata_mapper-0.9.3/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.9.3/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/.gitignore` & `aind_metadata_mapper-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/CONTRIBUTING.md` & `aind_metadata_mapper-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/LICENSE` & `aind_metadata_mapper-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/PKG-INFO` & `aind_metadata_mapper-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.9.2/README.md` & `aind_metadata_mapper-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/doc_template/Makefile` & `aind_metadata_mapper-0.9.3/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/doc_template/make.bat` & `aind_metadata_mapper-0.9.3/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.9.3/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.9.3/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.9.3/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/doc_template/source/conf.py` & `aind_metadata_mapper-0.9.3/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/examples/bergamo_session.py` & `aind_metadata_mapper-0.9.3/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/pyproject.toml` & `aind_metadata_mapper-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/sync_rig.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/utils.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/dynamic_routing/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/fip/session.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/fip/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/gather_metadata.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/gather_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
             """
             if filepath is not None and filepath.is_file():
                 with open(filepath, "r") as f:
                     contents = json.load(f)
                 try:
                     output = model.model_validate_json(json.dumps(contents))
-                except ValidationError:
+                except (ValidationError, AttributeError, ValueError, KeyError):
                     output = model.model_construct(**contents)
 
                 return output
             else:
                 return None
 
         subject = load_model(
@@ -408,27 +408,42 @@
         instrument = load_model(
             self.settings.metadata_settings.instrument_filepath, Instrument
         )
         processing = load_model(
             self.settings.metadata_settings.processing_filepath, Processing
         )
 
-        metadata = Metadata(
-            name=self.settings.metadata_settings.name,
-            location=self.settings.metadata_settings.location,
-            subject=subject,
-            data_description=data_description,
-            procedures=procedures,
-            session=session,
-            rig=rig,
-            processing=processing,
-            acquisition=acquisition,
-            instrument=instrument,
-        )
-        return metadata
+        try:
+            metadata = Metadata(
+                name=self.settings.metadata_settings.name,
+                location=self.settings.metadata_settings.location,
+                subject=subject,
+                data_description=data_description,
+                procedures=procedures,
+                session=session,
+                rig=rig,
+                processing=processing,
+                acquisition=acquisition,
+                instrument=instrument,
+            )
+            return metadata
+        except (ValidationError, ValueError, AttributeError, KeyError):
+            metadata = Metadata.model_construct(
+                name=self.settings.metadata_settings.name,
+                location=self.settings.metadata_settings.location,
+                subject=subject,
+                data_description=data_description,
+                procedures=procedures,
+                session=session,
+                rig=rig,
+                processing=processing,
+                acquisition=acquisition,
+                instrument=instrument,
+            )
+            return metadata
 
     def _write_json_file(self, filename: str, contents: dict) -> None:
         """
         Write a json file
         Parameters
         ----------
         filename : str
```

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/rig.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/open_ephys/rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/session.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/open_ephys/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/acquisition.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/smartspim/acquisition.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/utils.py` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper/smartspim/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.9.2
+Version: 0.9.3
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind_metadata_mapper-0.9.3/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.9.3/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.9.3/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.9.3/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.9.3/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/base-missing-probe_rig.json` & `aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/base-missing-probe_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/base_rig.json` & `aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/base_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/mvr.ini` & `aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/mvr_rig.json` & `aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/mvr_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/sync.yml` & `aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/sync.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/sync_rig.json` & `aind_metadata_mapper-0.9.3/tests/resources/dynamic_routing/sync_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/fip/000000_ophys_rig.json` & `aind_metadata_mapper-0.9.3/tests/resources/fip/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/fip/000000_ophys_session.json` & `aind_metadata_mapper-0.9.3/tests/resources/fip/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_funding_multiple_response.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/example_funding_multiple_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_procedures_response.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/example_procedures_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_subject_response.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/example_subject_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/acquisition.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/acquisition.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/data_description.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/data_description.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/instrument.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/instrument.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/procedures.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/procedures.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/processing.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/processing.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/rig.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/session.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/subject.json` & `aind_metadata_mapper-0.9.3/tests/resources/gather_metadata_job/metadata_files/subject.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.9.3/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.9.3/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.9.3/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.9.3/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.9.3/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.9.3/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/ephys_session.json` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/newscale_main.csv` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/open-ephys-inferred_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/open-ephys_rig.json` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/open-ephys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.xml` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings_main.xml` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.9.3/tests/resources/open_ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_ASI_logging_afternoon.txt` & `aind_metadata_mapper-0.9.3/tests/resources/smartspim/example_ASI_logging_afternoon.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_ASI_logging_morning.txt` & `aind_metadata_mapper-0.9.3/tests/resources/smartspim/example_ASI_logging_morning.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_metadata.py` & `aind_metadata_mapper-0.9.3/tests/resources/smartspim/example_metadata.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_bergamo/test_session.py` & `aind_metadata_mapper-0.9.3/tests/test_bergamo/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_mvr_rig.py` & `aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/test_mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_neuropixels_rig.py` & `aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/test_neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_sync_rig.py` & `aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/test_sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_utils.py` & `aind_metadata_mapper-0.9.3/tests/test_dynamic_routing/test_utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_fip/test_session.py` & `aind_metadata_mapper-0.9.3/tests/test_fip/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_gather_metadata.py` & `aind_metadata_mapper-0.9.3/tests/test_gather_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -604,14 +604,44 @@
         self.assertEqual(
             "s3://some-bucket/ecephys_632269_2023-10-10_10-10-10",
             main_metadata.location,
         )
         self.assertEqual("Invalid", main_metadata.metadata_status.value)
         self.assertEqual("632269", main_metadata.subject.subject_id)
 
+    def test_get_main_metadata_with_validation_errors(self):
+        """Tests get_main_metadata method handles validation errors"""
+        job_settings = JobSettings(
+            directory_to_write_to=RESOURCES_DIR,
+            metadata_settings=MetadataSettings(
+                name="ecephys_632269_2023-10-10_10-10-10",
+                location="s3://some-bucket/ecephys_632269_2023-10-10_10-10-10",
+                subject_filepath=(METADATA_DIR / "subject.json"),
+                data_description_filepath=(
+                    METADATA_DIR / "data_description.json"
+                ),
+                procedures_filepath=(METADATA_DIR / "procedures.json"),
+                session_filepath=(METADATA_DIR / "session.json"),
+                rig_filepath=(METADATA_DIR / "rig.json"),
+                processing_filepath=(METADATA_DIR / "processing.json"),
+                acquisition_filepath=(METADATA_DIR / "acquisition.json"),
+                instrument_filepath=(METADATA_DIR / "instrument.json"),
+            ),
+        )
+        metadata_job = GatherMetadataJob(settings=job_settings)
+        main_metadata = metadata_job.get_main_metadata()
+        self.assertIsNotNone(main_metadata.subject)
+        self.assertIsNotNone(main_metadata.procedures)
+        self.assertIsNotNone(main_metadata.data_description)
+        self.assertIsNotNone(main_metadata.session)
+        self.assertIsNotNone(main_metadata.rig)
+        self.assertIsNotNone(main_metadata.processing)
+        self.assertIsNotNone(main_metadata.acquisition)
+        self.assertIsNotNone(main_metadata.instrument)
+
     @patch("builtins.open", new_callable=mock_open())
     @patch("json.dump")
     def test_write_json_file(
         self, mock_json_dump: MagicMock, mock_file: MagicMock
     ):
         """Tests write_json_file method"""
         mock_file.return_value.__enter__.return_value = (
```

### Comparing `aind_metadata_mapper-0.9.2/tests/test_legacy_core.py` & `aind_metadata_mapper-0.9.3/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_mesoscope/test_session.py` & `aind_metadata_mapper-0.9.3/tests/test_mesoscope/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_open_ephys/test_rig.py` & `aind_metadata_mapper-0.9.3/tests/test_open_ephys/test_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_open_ephys/test_session.py` & `aind_metadata_mapper-0.9.3/tests/test_open_ephys/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_smartspim/test_acquisition.py` & `aind_metadata_mapper-0.9.3/tests/test_smartspim/test_acquisition.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.2/tests/test_smartspim/test_utils.py` & `aind_metadata_mapper-0.9.3/tests/test_smartspim/test_utils.py`

 * *Files identical despite different names*

