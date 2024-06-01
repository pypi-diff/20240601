# Comparing `tmp/dcd_mapping-0.1.0.tar.gz` & `tmp/dcd_mapping-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcd_mapping-0.1.0.tar", last modified: Sat Jun  1 00:51:59 2024, max compression
+gzip compressed data, was "dcd_mapping-0.1.1.tar", last modified: Sat Jun  1 01:13:49 2024, max compression
```

## Comparing `dcd_mapping-0.1.0.tar` & `dcd_mapping-0.1.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.932825 dcd_mapping-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.892825 dcd_mapping-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.896825 dcd_mapping-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/.github/workflows/checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-06-01 00:51:59.928825 dcd_mapping-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.892825 dcd_mapping-0.1.0/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.896825 dcd_mapping-0.1.0/notebooks/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.896825 dcd_mapping-0.1.0/notebooks/analysis/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/.ipynb_checkpoints/mave_target_reference_analysis-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/experiment_scoresets.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/mapping_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/mave_mapping_fig_3b.R
--rw-r--r--   0 runner    (1001) docker     (127)    32792 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/mavedb_mapping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17047 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/mavedb_scoreset_breakdown.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.900825 dcd_mapping-0.1.0/notebooks/analysis/results/
--rw-r--r--   0 runner    (1001) docker     (127) 13856316 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/notebooks/analysis/results/vrs_mappings_noncoding.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.920825 dcd_mapping-0.1.0/sample_mappings/
--rw-r--r--   0 runner    (1001) docker     (127)    38229 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000001-a-4.json
--rw-r--r--   0 runner    (1001) docker     (127)    24288 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000001-c-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    24794 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000001-c-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    27022 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000005-a-6.json
--rw-r--r--   0 runner    (1001) docker     (127)    23241 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000041-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    24530 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000043-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    65183 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000043-a-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    23893 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000045-c-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    24097 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000045-k-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    23359 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000048-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    24109 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000049-a-3.json
--rw-r--r--   0 runner    (1001) docker     (127)    25005 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000049-a-7.json
--rw-r--r--   0 runner    (1001) docker     (127)    25007 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000050-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    22029 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000055-0-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    25377 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000060-a-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    22271 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000061-d-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    22277 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000061-i-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    22622 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000067-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    23564 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000068-b-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000069-a-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000078-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    27666 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000081-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    23002 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000094-a-14.json
--rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000094-a-5.json
--rw-r--r--   0 runner    (1001) docker     (127)    22437 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000094-a-6.json
--rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000098-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    24174 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000099-a-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    22190 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/sample_mappings/00000103-c-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    33845 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/schema.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:51:59.932825 dcd_mapping-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.896825 dcd_mapping-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.924825 dcd_mapping-0.1.0/src/dcd_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    18720 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/mavedb_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/transcripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/vrs_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/src/dcd_mapping/vrs_v1_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.928825 dcd_mapping-0.1.0/src/dcd_mapping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-06-01 00:51:59.000000 dcd_mapping-0.1.0/src/dcd_mapping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-06-01 00:51:59.000000 dcd_mapping-0.1.0/src/dcd_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:51:59.000000 dcd_mapping-0.1.0/src/dcd_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 00:51:59.000000 dcd_mapping-0.1.0/src/dcd_mapping.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 00:51:59.000000 dcd_mapping-0.1.0/src/dcd_mapping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 00:51:59.000000 dcd_mapping-0.1.0/src/dcd_mapping.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.924825 dcd_mapping-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:59.928825 dcd_mapping-0.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/align_result.json
--rw-r--r--   0 runner    (1001) docker     (127)     8605 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/scoreset_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    23317 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/scoreset_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/transcript_result.json
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000001-b-2_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000002-a-2_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000018-a-1_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)   160153 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000024-a-1_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000041-a-1_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000068-a-1_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)    69310 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000093-a-1_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000099-a-1_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000103-c-1_scores.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/fixtures/vrs_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/test_mavedb_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/test_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-06-01 00:51:55.000000 dcd_mapping-0.1.0/tests/test_vrs_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.190786 dcd_mapping-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.150786 dcd_mapping-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.154786 dcd_mapping-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/.github/workflows/checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-06-01 01:13:49.190786 dcd_mapping-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.150786 dcd_mapping-0.1.1/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.158786 dcd_mapping-0.1.1/notebooks/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.158786 dcd_mapping-0.1.1/notebooks/analysis/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/.ipynb_checkpoints/mave_target_reference_analysis-checkpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/experiment_scoresets.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/mapping_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/mave_mapping_fig_3b.R
+-rw-r--r--   0 runner    (1001) docker     (127)    32792 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/mavedb_mapping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17047 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/mavedb_scoreset_breakdown.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.158786 dcd_mapping-0.1.1/notebooks/analysis/results/
+-rw-r--r--   0 runner    (1001) docker     (127) 13856316 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/notebooks/analysis/results/vrs_mappings_noncoding.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.182786 dcd_mapping-0.1.1/sample_mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)    38229 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000001-a-4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24288 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000001-c-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24794 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000001-c-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27022 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000005-a-6.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23241 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000041-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24530 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000043-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    65183 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000043-a-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23893 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000045-c-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24097 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000045-k-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23359 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000048-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24109 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000049-a-3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25005 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000049-a-7.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25007 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000050-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22029 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000055-0-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25377 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000060-a-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22271 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000061-d-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22277 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000061-i-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22622 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000067-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23564 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000068-b-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24772 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000069-a-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000078-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27666 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000081-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23002 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000094-a-14.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000094-a-5.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22437 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000094-a-6.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21964 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000098-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24174 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000099-a-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22190 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/sample_mappings/00000103-c-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33845 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:13:49.190786 dcd_mapping-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.154786 dcd_mapping-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.182786 dcd_mapping-0.1.1/src/dcd_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18720 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/mavedb_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/transcripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/vrs_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/src/dcd_mapping/vrs_v1_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.190786 dcd_mapping-0.1.1/src/dcd_mapping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-06-01 01:13:49.000000 dcd_mapping-0.1.1/src/dcd_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-06-01 01:13:49.000000 dcd_mapping-0.1.1/src/dcd_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:13:49.000000 dcd_mapping-0.1.1/src/dcd_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 01:13:49.000000 dcd_mapping-0.1.1/src/dcd_mapping.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 01:13:49.000000 dcd_mapping-0.1.1/src/dcd_mapping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 01:13:49.000000 dcd_mapping-0.1.1/src/dcd_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.186786 dcd_mapping-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:49.186786 dcd_mapping-0.1.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/align_result.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8605 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/scoreset_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23317 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/scoreset_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/transcript_result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000001-b-2_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000002-a-2_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000018-a-1_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   160153 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000024-a-1_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000041-a-1_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000068-a-1_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    69310 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000093-a-1_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000099-a-1_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000103-c-1_scores.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/fixtures/vrs_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/test_mavedb_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/test_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-06-01 01:13:44.000000 dcd_mapping-0.1.1/tests/test_vrs_map.py
```

### Comparing `dcd_mapping-0.1.0/.github/workflows/checks.yaml` & `dcd_mapping-0.1.1/.github/workflows/checks.yaml`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/.github/workflows/release.yaml` & `dcd_mapping-0.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/.gitignore` & `dcd_mapping-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/LICENSE` & `dcd_mapping-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/PKG-INFO` & `dcd_mapping-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcd-mapping
-Version: 0.1.0
+Version: 0.1.1
 Summary: Map MaveDB scoresets to VRS objects
 Author-email: Alex Handler Wagner <Alex.Wagner@nationwidechildrens.org>, Jeremy Arbesfeld <Jeremy.Arbesfeld@nationwidechildrens.org>, Samriddhi Singh <todo@todo.org>, James Stevenson <James.Stevenson@nationwidechildrens.org>
 License: MIT License
         
         Copyright (c) 2022-2024 Atlas of Variant Effects
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,14 +27,15 @@
         
 Project-URL: Homepage, https://www.varianteffect.org/
 Project-URL: Documentation, https://github.com/ave-dcd/dcd_mapping/README.md
 Project-URL: Source, https://github.com/ave-dcd/dcd_mapping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 2
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dcd_mapping-0.1.0/README.md` & `dcd_mapping-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/TODO.md` & `dcd_mapping-0.1.1/TODO.md`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/notebooks/analysis/.ipynb_checkpoints/mave_target_reference_analysis-checkpoint.ipynb` & `dcd_mapping-0.1.1/notebooks/analysis/.ipynb_checkpoints/mave_target_reference_analysis-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/notebooks/analysis/README.md` & `dcd_mapping-0.1.1/notebooks/analysis/README.md`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/notebooks/analysis/experiment_scoresets.txt` & `dcd_mapping-0.1.1/notebooks/analysis/experiment_scoresets.txt`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/notebooks/analysis/mapping_analysis.ipynb` & `dcd_mapping-0.1.1/notebooks/analysis/mapping_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/notebooks/analysis/mave_mapping_fig_3b.R` & `dcd_mapping-0.1.1/notebooks/analysis/mave_mapping_fig_3b.R`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/notebooks/analysis/mavedb_mapping.ipynb` & `dcd_mapping-0.1.1/notebooks/analysis/mavedb_mapping.ipynb`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/notebooks/analysis/mavedb_scoreset_breakdown.ipynb` & `dcd_mapping-0.1.1/notebooks/analysis/mavedb_scoreset_breakdown.ipynb`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/notebooks/analysis/results/vrs_mappings_noncoding.pickle` & `dcd_mapping-0.1.1/notebooks/analysis/results/vrs_mappings_noncoding.pickle`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/pyproject.toml` & `dcd_mapping-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 2",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Intended Audience :: Science/Research",
```

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000001-a-4.json` & `dcd_mapping-0.1.1/sample_mappings/00000001-a-4.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000001-c-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000001-c-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000001-c-2.json` & `dcd_mapping-0.1.1/sample_mappings/00000001-c-2.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000005-a-6.json` & `dcd_mapping-0.1.1/sample_mappings/00000005-a-6.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000041-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000041-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000043-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000043-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000043-a-2.json` & `dcd_mapping-0.1.1/sample_mappings/00000043-a-2.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000045-c-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000045-c-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000045-k-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000045-k-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000048-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000048-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000049-a-3.json` & `dcd_mapping-0.1.1/sample_mappings/00000049-a-3.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000049-a-7.json` & `dcd_mapping-0.1.1/sample_mappings/00000049-a-7.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000050-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000050-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000055-0-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000055-0-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000060-a-2.json` & `dcd_mapping-0.1.1/sample_mappings/00000060-a-2.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000061-d-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000061-d-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000061-i-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000061-i-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000067-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000067-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000068-b-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000068-b-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000069-a-2.json` & `dcd_mapping-0.1.1/sample_mappings/00000069-a-2.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000078-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000078-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000081-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000081-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000094-a-14.json` & `dcd_mapping-0.1.1/sample_mappings/00000094-a-14.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000094-a-5.json` & `dcd_mapping-0.1.1/sample_mappings/00000094-a-5.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000094-a-6.json` & `dcd_mapping-0.1.1/sample_mappings/00000094-a-6.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000098-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000098-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000099-a-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000099-a-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/sample_mappings/00000103-c-1.json` & `dcd_mapping-0.1.1/sample_mappings/00000103-c-1.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/schema.json` & `dcd_mapping-0.1.1/schema.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/align.py` & `dcd_mapping-0.1.1/src/dcd_mapping/align.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/annotate.py` & `dcd_mapping-0.1.1/src/dcd_mapping/annotate.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/cli.py` & `dcd_mapping-0.1.1/src/dcd_mapping/cli.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/lookup.py` & `dcd_mapping-0.1.1/src/dcd_mapping/lookup.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/main.py` & `dcd_mapping-0.1.1/src/dcd_mapping/main.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/mavedb_data.py` & `dcd_mapping-0.1.1/src/dcd_mapping/mavedb_data.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/resource_utils.py` & `dcd_mapping-0.1.1/src/dcd_mapping/resource_utils.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/schemas.py` & `dcd_mapping-0.1.1/src/dcd_mapping/schemas.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/transcripts.py` & `dcd_mapping-0.1.1/src/dcd_mapping/transcripts.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/vrs_map.py` & `dcd_mapping-0.1.1/src/dcd_mapping/vrs_map.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping/vrs_v1_schemas.py` & `dcd_mapping-0.1.1/src/dcd_mapping/vrs_v1_schemas.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping.egg-info/PKG-INFO` & `dcd_mapping-0.1.1/src/dcd_mapping.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcd-mapping
-Version: 0.1.0
+Version: 0.1.1
 Summary: Map MaveDB scoresets to VRS objects
 Author-email: Alex Handler Wagner <Alex.Wagner@nationwidechildrens.org>, Jeremy Arbesfeld <Jeremy.Arbesfeld@nationwidechildrens.org>, Samriddhi Singh <todo@todo.org>, James Stevenson <James.Stevenson@nationwidechildrens.org>
 License: MIT License
         
         Copyright (c) 2022-2024 Atlas of Variant Effects
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,14 +27,15 @@
         
 Project-URL: Homepage, https://www.varianteffect.org/
 Project-URL: Documentation, https://github.com/ave-dcd/dcd_mapping/README.md
 Project-URL: Source, https://github.com/ave-dcd/dcd_mapping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 2
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dcd_mapping-0.1.0/src/dcd_mapping.egg-info/SOURCES.txt` & `dcd_mapping-0.1.1/src/dcd_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/conftest.py` & `dcd_mapping-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/align_result.json` & `dcd_mapping-0.1.1/tests/fixtures/align_result.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/scoreset_metadata.json` & `dcd_mapping-0.1.1/tests/fixtures/scoreset_metadata.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/scoreset_metadata_response.json` & `dcd_mapping-0.1.1/tests/fixtures/scoreset_metadata_response.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/transcript_result.json` & `dcd_mapping-0.1.1/tests/fixtures/transcript_result.json`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000002-a-2_scores.csv` & `dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000002-a-2_scores.csv`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000018-a-1_scores.csv` & `dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000018-a-1_scores.csv`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000024-a-1_scores.csv` & `dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000024-a-1_scores.csv`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000041-a-1_scores.csv` & `dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000041-a-1_scores.csv`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000068-a-1_scores.csv` & `dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000068-a-1_scores.csv`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000093-a-1_scores.csv` & `dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000093-a-1_scores.csv`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000099-a-1_scores.csv` & `dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000099-a-1_scores.csv`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/fixtures/urn:mavedb:00000103-c-1_scores.csv` & `dcd_mapping-0.1.1/tests/fixtures/urn:mavedb:00000103-c-1_scores.csv`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/test_align.py` & `dcd_mapping-0.1.1/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/test_mavedb_data.py` & `dcd_mapping-0.1.1/tests/test_mavedb_data.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/test_transcript.py` & `dcd_mapping-0.1.1/tests/test_transcript.py`

 * *Files identical despite different names*

### Comparing `dcd_mapping-0.1.0/tests/test_vrs_map.py` & `dcd_mapping-0.1.1/tests/test_vrs_map.py`

 * *Files identical despite different names*

