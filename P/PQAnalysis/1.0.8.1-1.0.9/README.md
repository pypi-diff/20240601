# Comparing `tmp/pqanalysis-1.0.8.1.tar.gz` & `tmp/pqanalysis-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqanalysis-1.0.8.1.tar", last modified: Fri May 31 14:00:01 2024, max compression
+gzip compressed data, was "pqanalysis-1.0.9.tar", last modified: Fri May 31 22:01:57 2024, max compression
```

## Comparing `pqanalysis-1.0.8.1.tar` & `pqanalysis-1.0.9.tar`

### file list

```diff
@@ -1,463 +1,466 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.docstr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.502884 pqanalysis-1.0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.510884 pqanalysis-1.0.8.1/.github/.pylint_cache/
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/.pylint_cache/PQAnalysis_1.stats
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.510884 pqanalysis-1.0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.510884 pqanalysis-1.0.8.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/scripts/parse_pylint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.510884 pqanalysis-1.0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.514884 pqanalysis-1.0.8.1/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.514884 pqanalysis-1.0.8.1/PQAnalysis/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.514884 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.514884 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    24591 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/build_nep_traj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/gen2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/xyz2gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/core/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/atom/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/atom/element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/core/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/cell/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/cell/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/residue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/PQ_inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/rules.lark
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/selection.lark
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/terminals.lark
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.522884 pqanalysis-1.0.8.1/PQAnalysis/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/box_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/conversion_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/energy_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.522884 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/gen_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/gen_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/info_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.522884 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/input_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.522884 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/output_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/moldescriptor_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/nep/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/nep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/nep/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/nep/nep_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/restart_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/restart_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/topology_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/topology_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/frame_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/trajectory_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/trajectory_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/virial/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/virial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/virial/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/virial/virial_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/physical_data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/physical_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/physical_data/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/physical_data/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/tools/add_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/tools/traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/topology/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/_topology_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/bonded_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/shake_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/traj/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/type_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/PQAnalysis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/PQAnalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15249 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/benchmarks/core/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/benchmarks/core/benchmark_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/benchmarks/core/benchmark_traj_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/benchmarks/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/autodoc.sh
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.506884 pqanalysis-1.0.8.1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/_templates/package.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/docs/source/code/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.add_molecules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.continue_input.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.gen2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.rst2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.traj2box.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.xyz2gen.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.atom.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.atom.element.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.cell.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.residue.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.box_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.conversion_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.energy_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.info_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.nep.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.virial.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.virial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.write_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.physical_data.energy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.physical_data.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.physical_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.tools.add_molecule.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.shake_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.trajectory.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.type_checking.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.custom_logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.decorators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.random.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.units.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/docs/source/developerGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/developerGuide/developerGuide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/logo/PQAnalysis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/docs/source/userGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/userGuide/inputFile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/userGuide/userGuide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.506884 pqanalysis-1.0.8.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/examples/add_molecules/
--rw-r--r--   0 runner    (1001) docker     (127)   119066 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/add_molecules/mil68ga-md-01.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/add_molecules/perylene-md-05.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/add_molecules/perylene-md-05.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/examples/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/traj2box/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/traj2box/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/traj2box/acof_triclinic_2.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.558884 pqanalysis-1.0.8.1/examples/traj2comtraj/
--rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/traj2comtraj/umcm-9-md-01.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/pytest.sh
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 14:00:01.586885 pqanalysis-1.0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdfInputFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdfOutputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/atomicSystem/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/atomicSystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/atomicSystem/test_atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/atomicSystem/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/atomicSystem/test_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/test_continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/test_rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/test_traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/test_traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/core/atom/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/core/atom/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/core/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/core/test_residue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.506884 pqanalysis-1.0.8.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/n_not_matching.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/no_output_files.in
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/no_start_file.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-09.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-10.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/input.in
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/input_PQ.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/rdf/input.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/rdf/required_keys_not_given.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/readEnergyFile/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readEnergyFile/md-01.en
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readEnergyFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readEnergyFile/md-01_noinfo.en
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/readInfoFile/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readInfoFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readInfoFile/md-01.qmcfc.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.570885 pqanalysis-1.0.8.1/tests/data/readMoldescriptor/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readMoldescriptor/moldescriptor.dat
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readMoldescriptor/moldescriptor_withError.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.570885 pqanalysis-1.0.8.1/tests/data/readRestartFile/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readRestartFile/md-01.rst
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readRestartFile/moldescriptor.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.570885 pqanalysis-1.0.8.1/tests/data/rst2xyz/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/rst2xyz/md-01.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.570885 pqanalysis-1.0.8.1/tests/data/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2box/box.dat
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2box/box.vmd.xyz
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2box/test.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.574885 pqanalysis-1.0.8.1/tests/data/traj2qmcfc/
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2qmcfc/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2qmcfc/acof_triclinic_2.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2qmcfc/traj.qmcfc.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/io/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQ/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQAnalysis/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/test_inputDictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/test_inputFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_boxWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_energyFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_frameReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_infoFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_moldescriptorReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_restartReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_restartWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_trajectoryReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_trajectoryWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/physicalData/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/physicalData/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/physicalData/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/test_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/tools/test_traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/topology/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/tests/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_bondedTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/test_selectionTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/test_shakeTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/test_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/tests/traj/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/traj/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/traj/test_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/utils/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/utils/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/utils/test_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.027140 pqanalysis-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.docstr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.947140 pqanalysis-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.955140 pqanalysis-1.0.9/.github/.pylint_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.github/.pylint_cache/PQAnalysis_1.stats
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.955140 pqanalysis-1.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.955140 pqanalysis-1.0.9/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.github/scripts/parse_pylint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.959140 pqanalysis-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-31 22:01:57.027140 pqanalysis-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.959140 pqanalysis-1.0.9/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 22:01:56.000000 pqanalysis-1.0.9/PQAnalysis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.959140 pqanalysis-1.0.9/PQAnalysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.959140 pqanalysis-1.0.9/PQAnalysis/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/analysis/rdf/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/analysis/rdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/analysis/rdf/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.963140 pqanalysis-1.0.9/PQAnalysis/atomic_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/atomic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/atomic_system/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/atomic_system/_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/atomic_system/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/atomic_system/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24591 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/atomic_system/atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/atomic_system/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.963140 pqanalysis-1.0.9/PQAnalysis/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/build_nep_traj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/gen2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/cli/xyz2gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.963140 pqanalysis-1.0.9/PQAnalysis/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.963140 pqanalysis-1.0.9/PQAnalysis/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/atom/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/atom/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.967141 pqanalysis-1.0.9/PQAnalysis/core/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/cell/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/cell/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/core/residue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.967141 pqanalysis-1.0.9/PQAnalysis/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/grammar/PQ_inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/grammar/inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/grammar/rules.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/grammar/selection.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/grammar/terminals.lark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.967141 pqanalysis-1.0.9/PQAnalysis/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/box_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/conversion_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/energy_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.967141 pqanalysis-1.0.9/PQAnalysis/io/gen_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/gen_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/gen_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/gen_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/gen_file/gen_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/gen_file/gen_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/info_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.967141 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/input_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.971140 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq/output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.971140 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/moldescriptor_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.971140 pqanalysis-1.0.9/PQAnalysis/io/nep/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/nep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/nep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/nep/nep_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.971140 pqanalysis-1.0.9/PQAnalysis/io/restart_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/restart_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/restart_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/restart_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/restart_file/restart_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/restart_file/restart_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.971140 pqanalysis-1.0.9/PQAnalysis/io/topology_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/topology_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/topology_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/topology_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/topology_file/topology_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/topology_file/topology_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.975140 pqanalysis-1.0.9/PQAnalysis/io/traj_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/traj_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/traj_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/traj_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/traj_file/frame_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/traj_file/trajectory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/traj_file/trajectory_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.975140 pqanalysis-1.0.9/PQAnalysis/io/virial/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/virial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/virial/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/virial/virial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/io/write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.975140 pqanalysis-1.0.9/PQAnalysis/physical_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/physical_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/physical_data/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/physical_data/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.975140 pqanalysis-1.0.9/PQAnalysis/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/tools/add_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/tools/traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.975140 pqanalysis-1.0.9/PQAnalysis/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.975140 pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/_topology_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/bonded_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/shake_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/topology/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.979140 pqanalysis-1.0.9/PQAnalysis/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/traj/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/traj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/traj/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/traj/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.979140 pqanalysis-1.0.9/PQAnalysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/utils/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/PQAnalysis/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.027140 pqanalysis-1.0.9/PQAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-31 22:01:56.000000 pqanalysis-1.0.9/PQAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-05-31 22:01:56.000000 pqanalysis-1.0.9/PQAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:56.000000 pqanalysis-1.0.9/PQAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 22:01:56.000000 pqanalysis-1.0.9/PQAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-31 22:01:56.000000 pqanalysis-1.0.9/PQAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 22:01:56.000000 pqanalysis-1.0.9/PQAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.979140 pqanalysis-1.0.9/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.979140 pqanalysis-1.0.9/benchmarks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/benchmarks/core/benchmark_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/benchmarks/core/benchmark_traj_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/benchmarks/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.979140 pqanalysis-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/autodoc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.979140 pqanalysis-1.0.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.951140 pqanalysis-1.0.9/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.979140 pqanalysis-1.0.9/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.979140 pqanalysis-1.0.9/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/_templates/package.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.999141 pqanalysis-1.0.9/docs/source/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.analysis.rdf.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.analysis.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.add_molecules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.continue_input.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.gen2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.rst2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.traj2box.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.cli.xyz2gen.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.atom.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.atom.element.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.cell.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.residue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.box_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.conversion_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.energy_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.gen_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.gen_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.info_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.nep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.restart_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.restart_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.topology_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.topology_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.traj_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.traj_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.virial.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.virial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.write_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.physical_data.energy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.physical_data.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.physical_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.tools.add_molecule.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.shake_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.traj.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.traj.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.traj.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.traj.trajectory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.type_checking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.utils.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.utils.custom_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.utils.decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.utils.files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.utils.random.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/PQAnalysis.utils.units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/code/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.999141 pqanalysis-1.0.9/docs/source/developerGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/developerGuide/developerGuide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.999141 pqanalysis-1.0.9/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/logo/PQAnalysis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.999141 pqanalysis-1.0.9/docs/source/userGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/userGuide/inputFile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/docs/source/userGuide/userGuide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.951140 pqanalysis-1.0.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.999141 pqanalysis-1.0.9/examples/add_molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)   119066 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/add_molecules/mil68ga-md-01.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/add_molecules/perylene-md-05.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/add_molecules/perylene-md-05.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/add_molecules/shake_mil.top
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/add_molecules/shake_perylene.top
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.999141 pqanalysis-1.0.9/examples/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/traj2box/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/traj2box/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/traj2box/acof_triclinic_2.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.003141 pqanalysis-1.0.9/examples/traj2comtraj/
+-rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/examples/traj2comtraj/umcm-9-md-01.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 22:01:57.027140 pqanalysis-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.007140 pqanalysis-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.007140 pqanalysis-1.0.9/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.007140 pqanalysis-1.0.9/tests/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/analysis/rdf/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/analysis/rdf/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/analysis/rdf/test_rdfInputFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/analysis/rdf/test_rdfOutputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.007140 pqanalysis-1.0.9/tests/atomicSystem/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/atomicSystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/atomicSystem/test_atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/atomicSystem/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/atomicSystem/test_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.007140 pqanalysis-1.0.9/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/cli/test_continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/cli/test_rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/cli/test_traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/cli/test_traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.007140 pqanalysis-1.0.9/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/core/atom/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/core/atom/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/core/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/core/test_residue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:56.955140 pqanalysis-1.0.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/data/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/n_not_matching.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/no_output_files.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/no_start_file.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-09.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-10.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/inputFileReader/input_PQ.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/data/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/rdf/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/rdf/required_keys_not_given.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/data/readEnergyFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readEnergyFile/md-01.en
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readEnergyFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readEnergyFile/md-01_noinfo.en
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/data/readInfoFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readInfoFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readInfoFile/md-01.qmcfc.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/data/readMoldescriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readMoldescriptor/moldescriptor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readMoldescriptor/moldescriptor_withError.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/data/readRestartFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readRestartFile/md-01.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/readRestartFile/moldescriptor.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.011140 pqanalysis-1.0.9/tests/data/rst2xyz/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/rst2xyz/md-01.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.015141 pqanalysis-1.0.9/tests/data/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/traj2box/box.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/traj2box/box.vmd.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/traj2box/test.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.015141 pqanalysis-1.0.9/tests/data/traj2qmcfc/
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/traj2qmcfc/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/traj2qmcfc/acof_triclinic_2.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/data/traj2qmcfc/traj.qmcfc.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.023141 pqanalysis-1.0.9/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.023141 pqanalysis-1.0.9/tests/io/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.023141 pqanalysis-1.0.9/tests/io/inputFileReader/PQ/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/PQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.023141 pqanalysis-1.0.9/tests/io/inputFileReader/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/PQAnalysis/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/test_inputDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/test_inputFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/inputFileReader/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_boxWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_energyFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_frameReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_infoFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_moldescriptorReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_restartReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_restartWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_trajectoryReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_trajectoryWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/io/test_write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.023141 pqanalysis-1.0.9/tests/physicalData/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/physicalData/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/physicalData/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/test_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.023141 pqanalysis-1.0.9/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/tools/test_traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.023141 pqanalysis-1.0.9/tests/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.027140 pqanalysis-1.0.9/tests/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/bonded_topology/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/bonded_topology/test_bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/bonded_topology/test_bondedTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/bonded_topology/test_dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/test_selectionTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/test_shakeTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/topology/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.027140 pqanalysis-1.0.9/tests/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/traj/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/traj/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:01:57.027140 pqanalysis-1.0.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/utils/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/utils/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-31 22:01:46.000000 pqanalysis-1.0.9/tests/utils/test_math.py
```

### Comparing `pqanalysis-1.0.8.1/.codecov.yml` & `pqanalysis-1.0.9/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/.github/.pylint_cache/PQAnalysis_1.stats` & `pqanalysis-1.0.9/.github/.pylint_cache/PQAnalysis_1.stats`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 00000ae0: 8c28 5051 416e 616c 7973 6973 2e74 6f70  .(PQAnalysis.top
 00000af0: 6f6c 6f67 792e 626f 6e64 6564 5f74 6f70  ology.bonded_top
 00000b00: 6f6c 6f67 792e 626f 6e64 947d 9428 6818  ology.bond.}.(h.
 00000b10: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
 00000b20: 4b01 681d 4b10 681e 4b00 758c 1550 5141  K.h.K.h.K.u..PQA
 00000b30: 6e61 6c79 7369 732e 696f 2e66 6f72 6d61  nalysis.io.forma
 00000b40: 7473 947d 9428 6818 4b00 6819 4b00 681a  ts.}.(h.K.h.K.h.
-00000b50: 4b00 681b 4b00 681c 4b01 681d 4b52 681e  K.h.K.h.K.h.KRh.
+00000b50: 4b00 681b 4b00 681c 4b01 681d 4b51 681e  K.h.K.h.K.h.KQh.
 00000b60: 4b00 758c 2250 5141 6e61 6c79 7369 732e  K.u."PQAnalysis.
 00000b70: 696f 2e6d 6f6c 6465 7363 7269 7074 6f72  io.moldescriptor
 00000b80: 5f72 6561 6465 7294 7d94 2868 184b 0068  _reader.}.(h.K.h
 00000b90: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
 00000ba0: 1d4b 3968 1e4b 0275 8c16 5051 416e 616c  .K9h.K.u..PQAnal
 00000bb0: 7973 6973 2e69 6f2e 5f5f 696e 6974 5f5f  ysis.io.__init__
 00000bc0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
@@ -526,15 +526,15 @@
 000020d0: 746f 6d69 635f 7379 7374 656d 2e5f 5f69  tomic_system.__i
 000020e0: 6e69 745f 5f94 7d94 2868 184b 0068 194b  nit__.}.(h.K.h.K
 000020f0: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
 00002100: 0268 1e4b 0075 8c26 5051 416e 616c 7973  .h.K.u.&PQAnalys
 00002110: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
 00002120: 2e61 746f 6d69 635f 7379 7374 656d 947d  .atomic_system.}
 00002130: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00002140: 4b00 681c 4b06 681d 4ba5 681e 4b02 758c  K.h.K.h.K.h.K.u.
+00002140: 4b00 681c 4b06 681d 4ba5 681e 4b01 758c  K.h.K.h.K.h.K.u.
 00002150: 2450 5141 6e61 6c79 7369 732e 6174 6f6d  $PQAnalysis.atom
 00002160: 6963 5f73 7973 7465 6d2e 5f64 6563 6f72  ic_system._decor
 00002170: 6174 6f72 7394 7d94 2868 184b 0068 194b  ators.}.(h.K.h.K
 00002180: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
 00002190: 1868 1e4b 0075 8c2d 5051 416e 616c 7973  .h.K.u.-PQAnalys
 000021a0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
 000021b0: 2e5f 7374 616e 6461 7264 5f70 726f 7065  ._standard_prope
@@ -550,15 +550,15 @@
 00002250: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
 00002260: 0068 1b4b 0068 1c4b 0068 1d4b 1268 1e4b  .h.K.h.K.h.K.h.K
 00002270: 0075 8c24 5051 416e 616c 7973 6973 2e61  .u.$PQAnalysis.a
 00002280: 746f 6d69 635f 7379 7374 656d 2e5f 7072  tomic_system._pr
 00002290: 6f70 6572 7469 6573 947d 9428 6818 4b00  operties.}.(h.K.
 000022a0: 6819 4b00 681a 4b00 681b 4b00 681c 4b03  h.K.h.K.h.K.h.K.
 000022b0: 681d 4b28 681e 4b00 7575 8c06 6279 5f6d  h.K(h.K.uu..by_m
-000022c0: 7367 947d 9428 8c05 6669 786d 6594 4b0a  sg.}.(..fixme.K.
+000022c0: 7367 947d 9428 8c05 6669 786d 6594 4b09  sg.}.(..fixme.K.
 000022d0: 8c1f 706f 7373 6962 6c79 2d75 7365 642d  ..possibly-used-
 000022e0: 6265 666f 7265 2d61 7373 6967 6e6d 656e  before-assignmen
 000022f0: 7494 4b1e 8c1e 696e 636f 6e73 6973 7465  t.K...inconsiste
 00002300: 6e74 2d72 6574 7572 6e2d 7374 6174 656d  nt-return-statem
 00002310: 656e 7473 944b 098c 1274 6f6f 2d6d 616e  ents.K...too-man
 00002320: 792d 6172 6775 6d65 6e74 7394 4b12 8c0f  y-arguments.K...
 00002330: 746f 6f2d 6d61 6e79 2d6c 6f63 616c 7394  too-many-locals.
@@ -574,256 +574,256 @@
 000023d0: 656e 7494 4b01 8c1a 746f 6f2d 6d61 6e79  ent.K...too-many
 000023e0: 2d72 6574 7572 6e2d 7374 6174 656d 656e  -return-statemen
 000023f0: 7473 944b 018c 1774 6f6f 2d6d 616e 792d  ts.K...too-many-
 00002400: 7075 626c 6963 2d6d 6574 686f 6473 944b  public-methods.K
 00002410: 018c 0e64 7570 6c69 6361 7465 2d63 6f64  ...duplicate-cod
 00002420: 6594 4b03 758c 0f63 6f64 655f 7479 7065  e.K.u..code_type
 00002430: 5f63 6f75 6e74 947d 9428 8c04 636f 6465  _count.}.(..code
-00002440: 944d 7e1e 8c07 636f 6d6d 656e 7494 4d0d  .M~...comment.M.
-00002450: 018c 0964 6f63 7374 7269 6e67 944d 9421  ...docstring.M.!
-00002460: 8c05 656d 7074 7994 4d37 0b8c 0574 6f74  ..empty.M7...tot
+00002440: 944d 811e 8c07 636f 6d6d 656e 7494 4d09  .M....comment.M.
+00002450: 018c 0964 6f63 7374 7269 6e67 944d 9621  ...docstring.M.!
+00002460: 8c05 656d 7074 7994 4d36 0b8c 0574 6f74  ..empty.M6...tot
 00002470: 616c 944d 564c 758c 0c64 6570 656e 6465  al.MVLu..depende
 00002480: 6e63 6965 7394 7d94 288c 0d62 6561 7274  ncies.}.(..beart
 00002490: 7970 652e 636c 6177 948f 9428 6823 908c  ype.claw...(h#..
 000024a0: 1150 5141 6e61 6c79 7369 732e 636f 6e66  .PQAnalysis.conf
-000024b0: 6967 948f 9428 688f 68e5 68ed 6851 68eb  ig...(h.h.h.hQh.
-000024c0: 68ef 68f9 68f5 68f1 68e7 68d9 68f3 6895  h.h.h.h.h.h.h.h.
-000024d0: 6823 68e3 68f7 908c 1f50 5141 6e61 6c79  h#h.h....PQAnaly
+000024b0: 6967 948f 9428 68e3 68f3 68ef 68f5 6851  ig...(h.h.h.h.hQ
+000024c0: 68eb 68f7 68e5 68f1 68e7 68ed 68f9 6895  h.h.h.h.h.h.h.h.
+000024d0: 6823 68d9 688f 908c 1f50 5141 6e61 6c79  h#h.h....PQAnaly
 000024e0: 7369 732e 7574 696c 732e 6375 7374 6f6d  sis.utils.custom
-000024f0: 5f6c 6f67 6769 6e67 948f 9428 682f 683d  _logging...(h/h=
-00002500: 6859 6829 8c24 5051 416e 616c 7973 6973  hYh).$PQAnalysis
-00002510: 2e69 6f2e 7472 616a 5f66 696c 652e 6672  .io.traj_file.fr
-00002520: 616d 655f 7265 6164 6572 9468 9d68 3568  ame_reader.h.h5h
-00002530: c168 dd68 6968 6d8c 1250 5141 6e61 6c79  .h.hihm..PQAnaly
-00002540: 7369 732e 696f 2e62 6173 6594 68ab 687b  sis.io.base.h.h{
-00002550: 68bb 68b3 8c29 5051 416e 616c 7973 6973  h.h..)PQAnalysis
-00002560: 2e69 6f2e 7265 7374 6172 745f 6669 6c65  .io.restart_file
-00002570: 2e72 6573 7461 7274 5f72 6561 6465 7294  .restart_reader.
-00002580: 6875 6895 6873 6877 686f 6a0d 0100 0068  huh.hshwhoj....h
-00002590: c568 5768 5d8c 2650 5141 6e61 6c79 7369  .hWh].&PQAnalysi
-000025a0: 732e 696f 2e67 656e 5f66 696c 652e 6765  s.io.gen_file.ge
-000025b0: 6e5f 6669 6c65 5f72 6561 6465 7294 6a0b  n_file_reader.j.
-000025c0: 0100 0068 7f68 8f8c 2650 5141 6e61 6c79  ...h.h..&PQAnaly
-000025d0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
-000025e0: 6d2e 6174 6f6d 6963 5f73 7973 7465 6d94  m.atomic_system.
-000025f0: 68fd 6841 68d9 68a5 68cb 6823 908c 0f62  h.hAh.h.h.h#...b
+000024f0: 5f6c 6f67 6769 6e67 948f 9428 8c24 5051  _logging...(.$PQ
+00002500: 416e 616c 7973 6973 2e69 6f2e 7472 616a  Analysis.io.traj
+00002510: 5f66 696c 652e 6672 616d 655f 7265 6164  _file.frame_read
+00002520: 6572 9468 ab68 2368 b368 7768 3d68 3568  er.h.h#h.hwh=h5h
+00002530: d968 5d68 2f68 578c 2950 5141 6e61 6c79  .h]h/hW.)PQAnaly
+00002540: 7369 732e 696f 2e72 6573 7461 7274 5f66  sis.io.restart_f
+00002550: 696c 652e 7265 7374 6172 745f 7265 6164  ile.restart_read
+00002560: 6572 9468 296a 0d01 0000 6895 6873 689d  er.h)j....h.hsh.
+00002570: 8c26 5051 416e 616c 7973 6973 2e69 6f2e  .&PQAnalysis.io.
+00002580: 6765 6e5f 6669 6c65 2e67 656e 5f66 696c  gen_file.gen_fil
+00002590: 655f 7265 6164 6572 9468 bb68 598c 1250  e_reader.h.hY..P
+000025a0: 5141 6e61 6c79 7369 732e 696f 2e62 6173  QAnalysis.io.bas
+000025b0: 6594 686d 68fd 68c5 687f 68c1 68cb 68dd  e.hmh.h.h.h.h.h.
+000025c0: 68a5 686f 6a0b 0100 0068 7b68 7568 4168  h.hoj....h{huhAh
+000025d0: 6968 8f8c 2650 5141 6e61 6c79 7369 732e  ih..&PQAnalysis.
+000025e0: 6174 6f6d 6963 5f73 7973 7465 6d2e 6174  atomic_system.at
+000025f0: 6f6d 6963 5f73 7973 7465 6d94 908c 0f62  omic_system....b
 00002600: 6561 7274 7970 652e 7479 7069 6e67 948f  eartype.typing..
-00002610: 9428 688b 682f 8c24 5051 416e 616c 7973  .(h.h/.$PQAnalys
-00002620: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
-00002630: 2e5f 7072 6f70 6572 7469 6573 9468 8768  ._properties.h.h
-00002640: 3d68 4b8c 1a50 5141 6e61 6c79 7369 732e  =hK..PQAnalysis.
-00002650: 636f 7265 2e65 7863 6570 7469 6f6e 7394  core.exceptions.
-00002660: 6859 685b 684f 6829 6a3d 0100 0068 d78c  hYh[hOh)j=...h..
-00002670: 2450 5141 6e61 6c79 7369 732e 6174 6f6d  $PQAnalysis.atom
-00002680: 6963 5f73 7973 7465 6d2e 5f64 6563 6f72  ic_system._decor
-00002690: 6174 6f72 7394 689d 68bd 6835 68c1 6869  ators.h.h.h5h.hi
-000026a0: 8c23 5051 416e 616c 7973 6973 2e61 746f  .#PQAnalysis.ato
-000026b0: 6d69 635f 7379 7374 656d 2e5f 706f 7369  mic_system._posi
-000026c0: 7469 6f6e 7394 686d 6879 6a3e 0100 0068  tions.hmhyj>...h
-000026d0: ab68 bb68 256a 3f01 0000 68b3 68f1 6895  .h.h%j?...h.h.h.
-000026e0: 6873 68af 6851 686f 6a0d 0100 0068 5768  hsh.hQhoj....hWh
-000026f0: 5d68 2b6a 4001 0000 6a0b 0100 0068 7f68  ]h+j@...j....h.h
-00002700: 8f6a 0701 0000 6a41 0100 0068 6168 fd68  .j....jA...hah.h
-00002710: 4168 d968 a568 8d90 8c09 6465 636f 7261  Ah.h.h....decora
-00002720: 746f 7294 8f94 286a 4601 0000 684f 6829  tor...(jF...hOh)
+00002610: 9428 685b 6a3d 0100 0068 ab68 d768 4f68  .(h[j=...h.h.hOh
+00002620: b368 3d68 bd68 3568 d968 5d68 2f68 7968  .h=h.h5h.h]h/hyh
+00002630: 8b8c 2350 5141 6e61 6c79 7369 732e 6174  ..#PQAnalysis.at
+00002640: 6f6d 6963 5f73 7973 7465 6d2e 5f70 6f73  omic_system._pos
+00002650: 6974 696f 6e73 9468 576a 3e01 0000 6829  itions.hWj>...h)
+00002660: 688d 68f1 6a0d 0100 0068 9568 7368 9d6a  h.h.j....h.hsh.j
+00002670: 3f01 0000 68bb 6859 684b 686d 6a40 0100  ?...h.hYhKhmj@..
+00002680: 0068 fd68 7f68 c16a 0701 0000 682b 6887  .h.h.h.j....h+h.
+00002690: 68a5 686f 6a0b 0100 008c 1a50 5141 6e61  h.hoj......PQAna
+000026a0: 6c79 7369 732e 636f 7265 2e65 7863 6570  lysis.core.excep
+000026b0: 7469 6f6e 7394 8c24 5051 416e 616c 7973  tions..$PQAnalys
+000026c0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
+000026d0: 2e5f 6465 636f 7261 746f 7273 9468 5168  ._decorators.hQh
+000026e0: 2568 418c 2450 5141 6e61 6c79 7369 732e  %hA.$PQAnalysis.
+000026f0: 6174 6f6d 6963 5f73 7973 7465 6d2e 5f70  atomic_system._p
+00002700: 726f 7065 7274 6965 7394 68af 6869 688f  roperties.h.hih.
+00002710: 6a41 0100 0068 6190 8c09 6465 636f 7261  jA...ha...decora
+00002720: 746f 7294 8f94 2868 4f6a 4601 0000 6829  tor...(hOjF...h)
 00002730: 908c 0d62 6561 7274 7970 652e 646f 6f72  ...beartype.door
 00002740: 948f 9428 6829 908c 1550 5141 6e61 6c79  ...(h)...PQAnaly
 00002750: 7369 732e 6578 6365 7074 696f 6e73 948f  sis.exceptions..
-00002760: 9428 683d 6a45 0100 0068 5968 2968 378c  .(h=jE...hYh)h7.
-00002770: 2f50 5141 6e61 6c79 7369 732e 696f 2e69  /PQAnalysis.io.i
-00002780: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-00002790: 2e70 712e 6f75 7470 7574 5f66 696c 6573  .pq.output_files
-000027a0: 9468 3568 6968 816a 3e01 0000 68bb 68b3  .h5hih.j>...h.h.
-000027b0: 6875 6899 68b5 6877 6851 8c22 5051 416e  huh.h.hwhQ."PQAn
-000027c0: 616c 7973 6973 2e61 6e61 6c79 7369 732e  alysis.analysis.
-000027d0: 7264 662e 6578 6365 7074 696f 6e73 9468  rdf.exceptions.h
-000027e0: ad68 cf68 c568 5768 a36a 0b01 0000 8c23  .h.h.hWh.j.....#
-000027f0: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
-00002800: 635f 7379 7374 656d 2e65 7863 6570 7469  c_system.excepti
-00002810: 6f6e 7394 687f 688f 6a41 0100 0068 9368  ons.h.h.jA...h.h
-00002820: 5f68 cb68 4390 8c10 5051 416e 616c 7973  _h.hC...PQAnalys
-00002830: 6973 2e74 7970 6573 948f 9428 688b 6849  is.types...(h.hI
-00002840: 6a44 0100 0068 6768 3d68 5968 5b68 2968  jD...hgh=hYh[h)h
-00002850: 656a 3d01 0000 68d7 689d 6835 6869 6a47  ej=...h.h.h5hijG
-00002860: 0100 0068 6b6a 0501 0000 68bb 68b3 68ff  ...hkj....h.h.h.
-00002870: 6895 6883 6877 68c5 6857 685d 6a40 0100  h.h.hwh.hWh]j@..
-00002880: 0068 bf6a 0701 0000 6a41 0100 008c 2d50  .h.j....jA....-P
-00002890: 5141 6e61 6c79 7369 732e 6174 6f6d 6963  QAnalysis.atomic
-000028a0: 5f73 7973 7465 6d2e 5f73 7461 6e64 6172  _system._standar
-000028b0: 645f 7072 6f70 6572 7469 6573 9468 6168  d_properties.hah
-000028c0: fd68 4168 d990 8c05 6e75 6d70 7994 8f94  .hAh....numpy...
-000028d0: 2868 496a 4401 0000 683d 684b 6859 6a3d  (hIjD...h=hKhYj=
-000028e0: 0100 006a 4601 0000 689d 6835 6a47 0100  ...jF...h.h5jG..
-000028f0: 006a 0501 0000 6a3f 0100 0068 ff68 7568  .j....j?...h.huh
-00002900: 9568 8368 6f68 5768 5d6a 4001 0000 682b  .h.hohWh]j@...h+
-00002910: 6a07 0100 006a 4101 0000 68fd 6841 68d9  j....jA...h.hAh.
-00002920: 68cb 908c 0d62 6561 7274 7970 652e 7661  h....beartype.va
-00002930: 6c65 948f 9428 682b 6a07 0100 006a 0d01  le...(h+j....j..
-00002940: 0000 908c 0b6d 756c 7469 6d65 7468 6f64  .....multimethod
+00002760: 9428 6837 68a3 6843 68b3 6877 683d 6899  .(h7h.hCh.hwh=h.
+00002770: 6835 685f 68ad 68b5 6857 68cf 6829 6881  h5h_h.h.hWh.h)h.
+00002780: 8c22 5051 416e 616c 7973 6973 2e61 6e61  ."PQAnalysis.ana
+00002790: 6c79 7369 732e 7264 662e 6578 6365 7074  lysis.rdf.except
+000027a0: 696f 6e73 9468 bb68 596a 4001 0000 8c2f  ions.h.hYj@..../
+000027b0: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
+000027c0: 7075 745f 6669 6c65 5f72 6561 6465 722e  put_file_reader.
+000027d0: 7071 2e6f 7574 7075 745f 6669 6c65 7394  pq.output_files.
+000027e0: 68c5 687f 68cb 6a0b 0100 006a 4501 0000  h.h.h.j....jE...
+000027f0: 6893 6851 6875 8c23 5051 416e 616c 7973  h.hQhu.#PQAnalys
+00002800: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
+00002810: 2e65 7863 6570 7469 6f6e 7394 6869 688f  .exceptions.hih.
+00002820: 6a41 0100 0090 8c10 5051 416e 616c 7973  jA......PQAnalys
+00002830: 6973 2e74 7970 6573 948f 9428 685b 6a3d  is.types...(h[j=
+00002840: 0100 008c 2d50 5141 6e61 6c79 7369 732e  ....-PQAnalysis.
+00002850: 6174 6f6d 6963 5f73 7973 7465 6d2e 5f73  atomic_system._s
+00002860: 7461 6e64 6172 645f 7072 6f70 6572 7469  tandard_properti
+00002870: 6573 9468 6568 d76a 0501 0000 6867 68b3  es.heh.j....hgh.
+00002880: 6877 683d 6835 68d9 685d 68ff 688b 6a44  hwh=h5h.h]h.h.jD
+00002890: 0100 0068 5768 6b68 2968 4968 8368 9568  ...hWhkh)hIh.h.h
+000028a0: bf68 9d6a 3f01 0000 68bb 6859 68fd 68c5  .h.j?...h.hYh.h.
+000028b0: 6a07 0100 0068 416a 4701 0000 6869 6a41  j....hAjG...hijA
+000028c0: 0100 0068 6190 8c05 6e75 6d70 7994 8f94  ...ha...numpy...
+000028d0: 286a 3d01 0000 6a05 0100 0068 3d68 d968  (j=...j....h=h.h
+000028e0: 3568 5d68 ff6a 4401 0000 6857 6a3e 0100  5h]h.jD...hWj>..
+000028f0: 0068 4968 8368 956a 3f01 0000 689d 6859  .hIh.h.j?...h.hY
+00002900: 684b 68fd 68cb 6a07 0100 0068 2b68 6f6a  hKh.h.j....h+hoj
+00002910: 4601 0000 6875 6841 6a47 0100 006a 4101  F...huhAjG...jA.
+00002920: 0000 908c 0d62 6561 7274 7970 652e 7661  .....beartype.va
+00002930: 6c65 948f 9428 6a0d 0100 006a 0701 0000  le...(j....j....
+00002940: 682b 908c 0b6d 756c 7469 6d65 7468 6f64  h+...multimethod
 00002950: 948f 9428 682d 908c 1250 5141 6e61 6c79  ...(h-...PQAnaly
 00002960: 7369 732e 666f 726d 6174 7394 8f94 2868  sis.formats...(h
-00002970: af68 2f68 6d90 8c0a 5051 416e 616c 7973  .h/hm...PQAnalys
-00002980: 6973 948f 9428 682f 683d 6859 6a3d 0100  is...(h/h=hYj=..
-00002990: 0068 9d68 3568 c168 dd68 6968 6d6a 3e01  .h.h5h.h.hihmj>.
-000029a0: 0000 68ab 687b 68bb 68b3 6a3f 0100 0068  ..h.h{h.h.j?...h
-000029b0: 7568 9568 7368 7768 6f6a 0d01 0000 68c5  uh.hshwhoj....h.
-000029c0: 6857 685d 6a40 0100 006a 0b01 0000 687f  hWh]j@...j....h.
-000029d0: 688f 6a41 0100 0068 fd68 4168 d968 a568  h.jA...h.hAh.h.h
-000029e0: cb90 8c1a 5051 416e 616c 7973 6973 2e74  ....PQAnalysis.t
+00002970: 2f68 af68 6d90 8c0a 5051 416e 616c 7973  /h.hm...PQAnalys
+00002980: 6973 948f 9428 6a3d 0100 0068 ab68 b368  is...(j=...h.h.h
+00002990: 7768 3d68 3568 d968 5d68 2f68 576a 3e01  wh=h5h.h]h/hWj>.
+000029a0: 0000 6a0d 0100 0068 9568 7368 9d6a 3f01  ..j....h.hsh.j?.
+000029b0: 0000 68bb 6859 6a40 0100 0068 6d68 fd68  ..h.hYj@...hmh.h
+000029c0: c568 7f68 c168 cb68 dd68 a568 6f6a 0b01  .h.h.h.h.h.hoj..
+000029d0: 0000 687b 6875 6841 6869 688f 6a41 0100  ..h{huhAhih.jA..
+000029e0: 0090 8c1a 5051 416e 616c 7973 6973 2e74  ....PQAnalysis.t
 000029f0: 7261 6a2e 6578 6365 7074 696f 6e73 948f  raj.exceptions..
 00002a00: 9428 682f 8c0f 5051 416e 616c 7973 6973  .(h/..PQAnalysis
 00002a10: 2e74 7261 6a94 908c 1750 5141 6e61 6c79  .traj....PQAnaly
 00002a20: 7369 732e 7472 616a 2e66 6f72 6d61 7473  sis.traj.formats
 00002a30: 948f 9428 6a60 0100 0090 8c1a 5051 416e  ...(j`......PQAn
 00002a40: 616c 7973 6973 2e74 7261 6a2e 7472 616a  alysis.traj.traj
 00002a50: 6563 746f 7279 948f 9428 6a60 0100 0090  ectory...(j`....
 00002a60: 8c13 5051 416e 616c 7973 6973 2e74 7261  ..PQAnalysis.tra
 00002a70: 6a2e 6170 6994 8f94 286a 6001 0000 908c  j.api...(j`.....
 00002a80: 0f50 5141 6e61 6c79 7369 732e 636f 7265  .PQAnalysis.core
-00002a90: 948f 9428 6a40 0100 0068 8b68 8f6a 4101  ...(j@...h.h.jA.
-00002aa0: 0000 6a53 0100 006a 4701 0000 6a44 0100  ..jS...jG...jD..
-00002ab0: 0068 7968 6f6a 6501 0000 6a3f 0100 0068  .hyhoje...j?...h
-00002ac0: 5768 d96a 3d01 0000 685d 8c1e 5051 416e  Wh.j=...h]..PQAn
-00002ad0: 616c 7973 6973 2e69 6f2e 7265 7374 6172  alysis.io.restar
-00002ae0: 745f 6669 6c65 2e61 7069 9468 9d68 3590  t_file.api.h.h5.
+00002a90: 948f 9428 6879 688b 6a44 0100 0068 d968  ...(hyh.jD...h.h
+00002aa0: 576a 3d01 0000 6a53 0100 006a 3e01 0000  Wj=...jS...j>...
+00002ab0: 6a65 0100 006a 3f01 0000 6a47 0100 008c  je...j?...jG....
+00002ac0: 1e50 5141 6e61 6c79 7369 732e 696f 2e72  .PQAnalysis.io.r
+00002ad0: 6573 7461 7274 5f66 696c 652e 6170 6994  estart_file.api.
+00002ae0: 6a41 0100 0068 9d68 6f68 3568 8f68 5d90  jA...h.hoh5h.h].
 00002af0: 8c18 5051 416e 616c 7973 6973 2e74 7970  ..PQAnalysis.typ
-00002b00: 655f 6368 6563 6b69 6e67 948f 9428 688b  e_checking...(h.
-00002b10: 6887 6867 683d 6859 685b 6865 68d7 689d  h.hgh=hYh[heh.h.
-00002b20: 6835 68dd 6869 6a47 0100 0068 7968 6b68  h5h.hijG...hyhkh
-00002b30: ab6a 0501 0000 687b 6a3f 0100 0068 ff68  .j....h{j?...h.h
-00002b40: 756a 6901 0000 6895 6873 6883 68db 6877  uji...h.hsh.h.hw
-00002b50: 686f 6a0d 0100 0068 5768 5d6a 4001 0000  hoj....hWh]j@...
-00002b60: 6a0b 0100 0068 7f68 8f6a 0701 0000 6a41  j....h.h.j....jA
-00002b70: 0100 006a 5301 0000 68fd 6841 68a9 6a65  ...jS...h.hAh.je
-00002b80: 0100 0068 3b68 d968 a568 cb68 8d8c 1a50  ...h;h.h.h.h...P
-00002b90: 5141 6e61 6c79 7369 732e 696f 2e67 656e  QAnalysis.io.gen
-00002ba0: 5f66 696c 652e 6170 6994 908c 1350 5141  _file.api....PQA
+00002b00: 655f 6368 6563 6b69 6e67 948f 9428 685b  e_checking...(h[
+00002b10: 68ab 6a53 0100 0068 6568 3b68 d76a 6501  h.jS...heh;h.je.
+00002b20: 0000 6a05 0100 0068 6768 7768 3d68 3568  ..j....hghwh=h5h
+00002b30: d968 5d68 ff68 7968 8b6a 4401 0000 6857  .h]h.hyh.jD...hW
+00002b40: 686b 6a3e 0100 0068 8d6a 0d01 0000 6883  hkj>...h.j....h.
+00002b50: 6895 6873 689d 6a3f 0100 0068 5968 a968  h.hsh.j?...hYh.h
+00002b60: fd8c 1a50 5141 6e61 6c79 7369 732e 696f  ...PQAnalysis.io
+00002b70: 2e67 656e 5f66 696c 652e 6170 6994 68cb  .gen_file.api.h.
+00002b80: 687f 68dd 6a07 0100 0068 876a 6901 0000  h.h.j....h.ji...
+00002b90: 68a5 686f 6a0b 0100 0068 db68 7b68 7568  h.hoj....h.h{huh
+00002ba0: 4168 6968 8f6a 4101 0000 908c 1350 5141  Ahih.jA......PQA
 00002bb0: 6e61 6c79 7369 732e 746f 706f 6c6f 6779  nalysis.topology
-00002bc0: 948f 9428 688f 6a41 0100 0068 db6a 5301  ...(h.jA...h.jS.
-00002bd0: 0000 6a47 0100 0068 ab68 a96a 3f01 0000  ..jG...h.h.j?...
-00002be0: 68a5 68d9 6a3d 0100 0068 8d68 3590 8c18  h.h.j=...h.h5...
+00002bc0: 948f 9428 6a44 0100 0068 d96a 3d01 0000  ...(jD...h.j=...
+00002bd0: 68ab 6a53 0100 006a 3e01 0000 688d 68db  h.jS...j>...h.h.
+00002be0: 68a5 6835 688f 6a41 0100 0068 a990 8c18  h.h5h.jA...h....
 00002bf0: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
-00002c00: 635f 7379 7374 656d 948f 9428 6a40 0100  c_system...(j@..
-00002c10: 0068 8b68 8f68 cb68 3d68 9d6a 3f01 0000  .h.h.h.h=h.j?...
-00002c20: 6a3d 0100 006a 6901 0000 688d 6895 6a6c  j=...ji...h.h.jl
-00002c30: 0100 0068 3568 7f90 8c21 5051 416e 616c  ...h5h...!PQAnal
+00002c00: 635f 7379 7374 656d 948f 9428 688b 6a3d  c_system...(h.j=
+00002c10: 0100 006a 6c01 0000 68cb 687f 6a3e 0100  ...jl...h.h.j>..
+00002c20: 0068 8d6a 3f01 0000 6a69 0100 0068 9568  .h.j?...ji...h.h
+00002c30: 3d68 9d68 3568 8f90 8c21 5051 416e 616c  =h.h5h...!PQAnal
 00002c40: 7973 6973 2e74 6f6f 6c73 2e74 7261 6a5f  ysis.tools.traj_
 00002c50: 746f 5f63 6f6d 5f74 7261 6a94 8f94 288c  to_com_traj...(.
 00002c60: 1050 5141 6e61 6c79 7369 732e 746f 6f6c  .PQAnalysis.tool
 00002c70: 7394 908c 0f50 5141 6e61 6c79 7369 732e  s....PQAnalysis.
-00002c80: 7472 616a 948f 9428 688b 683d 685b 6859  traj...(h.h=h[hY
-00002c90: 6a3d 0100 0068 9d68 7968 7b68 f16a 3f01  j=...h.hyh{h.j?.
-00002ca0: 0000 6875 6a69 0100 0068 9568 7368 db68  ..huji...h.hsh.h
-00002cb0: 7f68 8f68 3b68 d968 8d90 8c15 5051 416e  .h.h;h.h....PQAn
+00002c80: 7472 616a 948f 9428 685b 6a3d 0100 0068  traj...(h[j=...h
+00002c90: 3b68 3d68 d968 7968 8b6a 3e01 0000 688d  ;h=h.hyh.j>...h.
+00002ca0: 68f1 6895 6873 689d 6859 687f 6a69 0100  h.h.hsh.hYh.ji..
+00002cb0: 0068 db68 7b68 7568 8f90 8c15 5051 416e  .h.h{huh....PQAn
 00002cc0: 616c 7973 6973 2e69 6f2e 666f 726d 6174  alysis.io.format
-00002cd0: 7394 8f94 2868 8b68 ed68 7968 cb6a 3e01  s...(h.h.hyh.j>.
-00002ce0: 0000 683d 68a9 68ab 687b 68f1 8c0d 5051  ..h=h.h.h{h...PQ
-00002cf0: 416e 616c 7973 6973 2e69 6f94 688d 689d  Analysis.io.h.h.
-00002d00: 6a6c 0100 0068 7f90 8c0d 5051 416e 616c  jl...h....PQAnal
-00002d10: 7973 6973 2e69 6f94 8f94 2868 dd68 e568  ysis.io...(h.h.h
-00002d20: db68 eb68 3d68 f968 5b68 5968 f368 d968  .h.h=h.h[hYh.h.h
-00002d30: f568 d768 9568 8368 f790 8c23 5051 416e  .h.h.h.h...#PQAn
+00002cd0: 7394 8f94 2868 7968 8b68 7b68 ab6a 6c01  s...(hyh.h{h.jl.
+00002ce0: 0000 68cb 687f 68a9 688d 68f1 68ed 683d  ..h.h.h.h.h.h.h=
+00002cf0: 689d 6a40 0100 008c 0d50 5141 6e61 6c79  h.j@.....PQAnaly
+00002d00: 7369 732e 696f 9490 8c0d 5051 416e 616c  sis.io....PQAnal
+00002d10: 7973 6973 2e69 6f94 8f94 2868 f368 5b68  ysis.io...(h.h[h
+00002d20: f568 eb68 f768 d768 dd68 e568 f968 9568  .h.h.h.h.h.h.h.h
+00002d30: 8368 3d68 d968 db68 5990 8c23 5051 416e  .h=h.h.hY..#PQAn
 00002d40: 616c 7973 6973 2e70 6879 7369 6361 6c5f  alysis.physical_
 00002d50: 6461 7461 2e65 7863 6570 7469 6f6e 7394  data.exceptions.
-00002d60: 8f94 2868 418c 1850 5141 6e61 6c79 7369  ..(hA..PQAnalysi
-00002d70: 732e 7068 7973 6963 616c 5f64 6174 6194  s.physical_data.
+00002d60: 8f94 288c 1850 5141 6e61 6c79 7369 732e  ..(..PQAnalysis.
+00002d70: 7068 7973 6963 616c 5f64 6174 6194 6841  physical_data.hA
 00002d80: 908c 1f50 5141 6e61 6c79 7369 732e 7068  ...PQAnalysis.ph
 00002d90: 7973 6963 616c 5f64 6174 612e 656e 6572  ysical_data.ener
 00002da0: 6779 948f 9428 6a7d 0100 0090 8c17 5051  gy...(j}......PQ
 00002db0: 416e 616c 7973 6973 2e75 7469 6c73 2e63  Analysis.utils.c
 00002dc0: 6f6d 6d6f 6e94 8f94 288c 1050 5141 6e61  ommon...(..PQAna
 00002dd0: 6c79 7369 732e 7574 696c 7394 68f1 908c  lysis.utils.h...
 00002de0: 1b50 5141 6e61 6c79 7369 732e 7574 696c  .PQAnalysis.util
 00002df0: 732e 6465 636f 7261 746f 7273 948f 9428  s.decorators...(
 00002e00: 6a82 0100 0090 8c10 5051 416e 616c 7973  j.......PQAnalys
-00002e10: 6973 2e75 7469 6c73 948f 9428 6851 687b  is.utils...(hQh{
-00002e20: 68d9 68d7 8c0e 5051 416e 616c 7973 6973  h.h...PQAnalysis
+00002e10: 6973 2e75 7469 6c73 948f 9428 687b 6851  is.utils...(h{hQ
+00002e20: 68d7 68d9 8c0e 5051 416e 616c 7973 6973  h.h...PQAnalysis
 00002e30: 2e63 6c69 9490 8c13 5051 416e 616c 7973  .cli....PQAnalys
 00002e40: 6973 2e5f 7665 7273 696f 6e94 8f94 2868  is._version...(h
-00002e50: f168 5390 8c1e 5051 416e 616c 7973 6973  .hS...PQAnalysis
+00002e50: 5368 f190 8c1e 5051 416e 616c 7973 6973  Sh....PQAnalysis
 00002e60: 2e74 6f70 6f6c 6f67 792e 6578 6365 7074  .topology.except
 00002e70: 696f 6e73 948f 9428 8c13 5051 416e 616c  ions...(..PQAnal
 00002e80: 7973 6973 2e74 6f70 6f6c 6f67 7994 685d  ysis.topology.h]
 00002e90: 908c 2850 5141 6e61 6c79 7369 732e 746f  ..(PQAnalysis.to
 00002ea0: 706f 6c6f 6779 2e62 6f6e 6465 645f 746f  pology.bonded_to
 00002eb0: 706f 6c6f 6779 2e62 6f6e 6494 8f94 286a  pology.bond...(j
-00002ec0: 8c01 0000 6869 6861 908c 2950 5141 6e61  ....hiha..)PQAna
+00002ec0: 8c01 0000 6861 6869 908c 2950 5141 6e61  ....hahi..)PQAna
 00002ed0: 6c79 7369 732e 746f 706f 6c6f 6779 2e62  lysis.topology.b
 00002ee0: 6f6e 6465 645f 746f 706f 6c6f 6779 2e61  onded_topology.a
-00002ef0: 6e67 6c65 948f 9428 6a8c 0100 0068 6968  ngle...(j....hih
-00002f00: 6190 8c2c 5051 416e 616c 7973 6973 2e74  a..,PQAnalysis.t
+00002ef0: 6e67 6c65 948f 9428 6a8c 0100 0068 6168  ngle...(j....hah
+00002f00: 6990 8c2c 5051 416e 616c 7973 6973 2e74  i..,PQAnalysis.t
 00002f10: 6f70 6f6c 6f67 792e 626f 6e64 6564 5f74  opology.bonded_t
 00002f20: 6f70 6f6c 6f67 792e 6469 6865 6472 616c  opology.dihedral
-00002f30: 948f 9428 6a8c 0100 0068 6968 6190 8c33  ...(j....hiha..3
+00002f30: 948f 9428 6a8c 0100 0068 6168 6990 8c33  ...(j....hahi..3
 00002f40: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
 00002f50: 6f67 792e 626f 6e64 6564 5f74 6f70 6f6c  ogy.bonded_topol
 00002f60: 6f67 792e 626f 6e64 6564 5f74 6f70 6f6c  ogy.bonded_topol
 00002f70: 6f67 7994 8f94 286a 8c01 0000 685d 908c  ogy...(j....h]..
 00002f80: 1d50 5141 6e61 6c79 7369 732e 746f 706f  .PQAnalysis.topo
 00002f90: 6c6f 6779 2e73 656c 6563 7469 6f6e 948f  logy.selection..
-00002fa0: 9428 6a8c 0100 0068 5b68 5990 8c1c 5051  .(j....h[hY...PQ
+00002fa0: 9428 6a8c 0100 0068 5968 5b90 8c1c 5051  .(j....hYh[...PQ
 00002fb0: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
 00002fc0: 792e 746f 706f 6c6f 6779 948f 9428 6a8c  y.topology...(j.
 00002fd0: 0100 0068 5790 8c04 6c61 726b 948f 9428  ...hW...lark...(
 00002fe0: 68b3 6857 908c 2250 5141 6e61 6c79 7369  h.hW.."PQAnalysi
 00002ff0: 732e 746f 706f 6c6f 6779 2e73 6861 6b65  s.topology.shake
 00003000: 5f74 6f70 6f6c 6f67 7994 8f94 2868 5b90  _topology...(h[.
 00003010: 8c1a 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
 00003020: 652e 6578 6365 7074 696f 6e73 948f 9428  e.exceptions...(
-00003030: 68fd 6a0d 0100 0068 5d6a 0b01 0000 8c0f  h.j....h]j......
-00003040: 5051 416e 616c 7973 6973 2e63 6f72 6594  PQAnalysis.core.
+00003030: 68fd 8c0f 5051 416e 616c 7973 6973 2e63  h...PQAnalysis.c
+00003040: 6f72 6594 6a0d 0100 006a 0b01 0000 685d  ore.j....j....h]
 00003050: 908c 3850 5141 6e61 6c79 7369 732e 746f  ..8PQAnalysis.to
 00003060: 706f 6c6f 6779 2e62 6f6e 6465 645f 746f  pology.bonded_to
 00003070: 706f 6c6f 6779 2e5f 746f 706f 6c6f 6779  pology._topology
 00003080: 5f70 726f 7065 7274 6965 7394 8f94 2868  _properties...(h
 00003090: 6990 8c18 5051 416e 616c 7973 6973 2e69  i...PQAnalysis.i
 000030a0: 6f2e 6578 6365 7074 696f 6e73 948f 9428  o.exceptions...(
-000030b0: 6a3e 0100 0068 6f68 6d68 7b90 8c12 5051  j>...hohmh{...PQ
+000030b0: 686f 687b 686d 6a40 0100 0090 8c12 5051  hoh{hmj@......PQ
 000030c0: 416e 616c 7973 6973 2e69 6f2e 6261 7365  Analysis.io.base
-000030d0: 948f 9428 6a40 0100 0068 8b68 8f68 cb68  ...(j@...h.h.h.h
-000030e0: 6f68 ab68 7b68 b36a 3f01 0000 68a5 6875  oh.h{h.j?...h.hu
-000030f0: 6a78 0100 0068 9d68 7390 8c22 5051 416e  jx...h.hs.."PQAn
+000030d0: 948f 9428 688b 687b 68ab 68cb 6875 6a3e  ...(h.h{h.h.huj>
+000030e0: 0100 006a 3f01 0000 68b3 68a5 6873 689d  ...j?...h.h.hsh.
+000030f0: 686f 688f 6a78 0100 0090 8c22 5051 416e  hoh.jx....."PQAn
 00003100: 616c 7973 6973 2e69 6f2e 6d6f 6c64 6573  alysis.io.moldes
 00003110: 6372 6970 746f 725f 7265 6164 6572 948f  criptor_reader..
-00003120: 9428 6a3f 0100 006a 7801 0000 908c 2950  .(j?...jx.....)P
+00003120: 9428 6a3e 0100 006a 7801 0000 908c 2950  .(j>...jx.....)P
 00003130: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
 00003140: 7461 7274 5f66 696c 652e 7265 7374 6172  tart_file.restar
 00003150: 745f 7772 6974 6572 948f 9428 8c1a 5051  t_writer...(..PQ
 00003160: 416e 616c 7973 6973 2e69 6f2e 7265 7374  Analysis.io.rest
 00003170: 6172 745f 6669 6c65 946a 7801 0000 908c  art_file.jx.....
 00003180: 2950 5141 6e61 6c79 7369 732e 696f 2e72  )PQAnalysis.io.r
 00003190: 6573 7461 7274 5f66 696c 652e 7265 7374  estart_file.rest
-000031a0: 6172 745f 7265 6164 6572 948f 9428 6a69  art_reader...(ji
-000031b0: 0100 006a aa01 0000 6a78 0100 0090 8c1e  ...j....jx......
+000031a0: 6172 745f 7265 6164 6572 948f 9428 6aaa  art_reader...(j.
+000031b0: 0100 006a 6901 0000 6a78 0100 0090 8c1e  ...ji...jx......
 000031c0: 5051 416e 616c 7973 6973 2e69 6f2e 7265  PQAnalysis.io.re
 000031d0: 7374 6172 745f 6669 6c65 2e61 7069 948f  start_file.api..
 000031e0: 9428 6879 6a78 0100 0090 8c29 5051 416e  .(hyjx.....)PQAn
 000031f0: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
 00003200: 696c 652e 7472 616a 6563 746f 7279 5f72  ile.trajectory_r
 00003210: 6561 6465 7294 8f94 288c 1750 5141 6e61  eader...(..PQAna
 00003220: 6c79 7369 732e 696f 2e74 7261 6a5f 6669  lysis.io.traj_fi
 00003230: 6c65 946a 7801 0000 908c 2950 5141 6e61  le.jx.....)PQAna
 00003240: 6c79 7369 732e 696f 2e74 7261 6a5f 6669  lysis.io.traj_fi
 00003250: 6c65 2e74 7261 6a65 6374 6f72 795f 7772  le.trajectory_wr
 00003260: 6974 6572 948f 9428 6ab1 0100 006a 7801  iter...(j....jx.
 00003270: 0000 908c 2450 5141 6e61 6c79 7369 732e  ....$PQAnalysis.
 00003280: 696f 2e74 7261 6a5f 6669 6c65 2e66 7261  io.traj_file.fra
-00003290: 6d65 5f72 6561 6465 7294 8f94 2868 8f6a  me_reader...(h.j
-000032a0: b101 0000 6a78 0100 0090 8c1b 5051 416e  ....jx......PQAn
+00003290: 6d65 5f72 6561 6465 7294 8f94 286a b101  me_reader...(j..
+000032a0: 0000 688f 6a78 0100 0090 8c1b 5051 416e  ..h.jx......PQAn
 000032b0: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
 000032c0: 696c 652e 6170 6994 8f94 2868 7968 7f6a  ile.api...(hyh.j
 000032d0: 7801 0000 908c 2650 5141 6e61 6c79 7369  x.....&PQAnalysi
 000032e0: 732e 696f 2e67 656e 5f66 696c 652e 6765  s.io.gen_file.ge
 000032f0: 6e5f 6669 6c65 5f72 6561 6465 7294 8f94  n_file_reader...
-00003300: 288c 1650 5141 6e61 6c79 7369 732e 696f  (..PQAnalysis.io
-00003310: 2e67 656e 5f66 696c 6594 6a6c 0100 006a  .gen_file.jl...j
+00003300: 286a 6c01 0000 8c16 5051 416e 616c 7973  (jl.....PQAnalys
+00003310: 6973 2e69 6f2e 6765 6e5f 6669 6c65 946a  is.io.gen_file.j
 00003320: 7801 0000 908c 2650 5141 6e61 6c79 7369  x.....&PQAnalysi
 00003330: 732e 696f 2e67 656e 5f66 696c 652e 6765  s.io.gen_file.ge
 00003340: 6e5f 6669 6c65 5f77 7269 7465 7294 8f94  n_file_writer...
-00003350: 286a ba01 0000 6a6c 0100 006a 7801 0000  (j....jl...jx...
+00003350: 286a 6c01 0000 6aba 0100 006a 7801 0000  (jl...j....jx...
 00003360: 908c 1a50 5141 6e61 6c79 7369 732e 696f  ...PQAnalysis.io
 00003370: 2e67 656e 5f66 696c 652e 6170 6994 8f94  .gen_file.api...
 00003380: 286a ba01 0000 6a78 0100 0090 8c1b 5051  (j....jx......PQ
 00003390: 416e 616c 7973 6973 2e69 6f2e 746f 706f  Analysis.io.topo
 000033a0: 6c6f 6779 5f66 696c 6594 8f94 286a 7801  logy_file...(jx.
 000033b0: 0000 908c 1f50 5141 6e61 6c79 7369 732e  .....PQAnalysis.
 000033c0: 696f 2e74 6f70 6f6c 6f67 795f 6669 6c65  io.topology_file
@@ -846,27 +846,27 @@
 000034d0: 8c17 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
 000034e0: 7772 6974 655f 6170 6994 8f94 286a 7801  write_api...(jx.
 000034f0: 0000 908c 1850 5141 6e61 6c79 7369 732e  .....PQAnalysis.
 00003500: 7068 7973 6963 616c 5f64 6174 6194 8f94  physical_data...
 00003510: 2868 7590 8c27 5051 416e 616c 7973 6973  (hu..'PQAnalysis
 00003520: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
 00003530: 6561 6465 722e 666f 726d 6174 7394 8f94  eader.formats...
-00003540: 2868 c168 778c 1f50 5141 6e61 6c79 7369  (h.hw..PQAnalysi
-00003550: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
-00003560: 7265 6164 6572 9468 c568 b390 8c17 5051  reader.h.h....PQ
+00003540: 2868 c568 c168 b368 778c 1f50 5141 6e61  (h.h.h.hw..PQAna
+00003550: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
+00003560: 696c 655f 7265 6164 6572 9490 8c17 5051  ile_reader....PQ
 00003570: 416e 616c 7973 6973 2e69 6f2e 7472 616a  Analysis.io.traj
-00003580: 5f66 696c 6594 8f94 2868 8d68 7990 8c16  _file...(h.hy...
+00003580: 5f66 696c 6594 8f94 2868 7968 8d90 8c16  _file...(hyh....
 00003590: 5051 416e 616c 7973 6973 2e69 6f2e 6765  PQAnalysis.io.ge
 000035a0: 6e5f 6669 6c65 948f 9428 6879 908c 2250  n_file...(hy.."P
 000035b0: 5141 6e61 6c79 7369 732e 696f 2e76 6972  QAnalysis.io.vir
 000035c0: 6961 6c2e 7669 7269 616c 5f72 6561 6465  ial.virial_reade
-000035d0: 7294 8f94 288c 1450 5141 6e61 6c79 7369  r...(..PQAnalysi
-000035e0: 732e 696f 2e76 6972 6961 6c94 6887 908c  s.io.virial.h...
-000035f0: 0974 7164 6d2e 6175 746f 948f 9428 688f  .tqdm.auto...(h.
-00003600: 68d9 908c 2250 5141 6e61 6c79 7369 732e  h..."PQAnalysis.
+000035d0: 7294 8f94 2868 878c 1450 5141 6e61 6c79  r...(h...PQAnaly
+000035e0: 7369 732e 696f 2e76 6972 6961 6c94 908c  sis.io.virial...
+000035f0: 0974 7164 6d2e 6175 746f 948f 9428 68d9  .tqdm.auto...(h.
+00003600: 688f 908c 2250 5141 6e61 6c79 7369 732e  h..."PQAnalysis.
 00003610: 696f 2e74 7261 6a5f 6669 6c65 2e65 7863  io.traj_file.exc
 00003620: 6570 7469 6f6e 7394 8f94 2868 8f6a 3d01  eptions...(h.j=.
 00003630: 0000 908c 1850 5141 6e61 6c79 7369 732e  .....PQAnalysis.
 00003640: 696f 2e76 6972 6961 6c2e 6170 6994 8f94  io.virial.api...
 00003650: 2868 9590 8c16 5051 416e 616c 7973 6973  (h....PQAnalysis
 00003660: 2e75 7469 6c73 2e75 6e69 7473 948f 9428  .utils.units...(
 00003670: 6895 908c 1650 5141 6e61 6c79 7369 732e  h....PQAnalysis.
@@ -874,15 +874,15 @@
 00003690: 9590 8c17 5051 416e 616c 7973 6973 2e75  ....PQAnalysis.u
 000036a0: 7469 6c73 2e72 616e 646f 6d94 8f94 2868  tils.random...(h
 000036b0: 956a 4101 0000 908c 1c50 5141 6e61 6c79  .jA......PQAnaly
 000036c0: 7369 732e 696f 2e6e 6570 2e65 7863 6570  sis.io.nep.excep
 000036d0: 7469 6f6e 7394 8f94 2868 9590 8c25 5051  tions...(h...%PQ
 000036e0: 416e 616c 7973 6973 2e69 6f2e 7265 7374  Analysis.io.rest
 000036f0: 6172 745f 6669 6c65 2e65 7863 6570 7469  art_file.excepti
-00003700: 6f6e 7394 8f94 2868 9d6a 3f01 0000 908c  ons...(h.j?.....
+00003700: 6f6e 7394 8f94 2868 9d6a 3e01 0000 908c  ons...(h.j>.....
 00003710: 2650 5141 6e61 6c79 7369 732e 696f 2e74  &PQAnalysis.io.t
 00003720: 6f70 6f6c 6f67 795f 6669 6c65 2e65 7863  opology_file.exc
 00003730: 6570 7469 6f6e 7394 8f94 2868 a568 ab90  eptions...(h.h..
 00003740: 8c30 5051 416e 616c 7973 6973 2e69 6f2e  .0PQAnalysis.io.
 00003750: 746f 706f 6c6f 6779 5f66 696c 652e 746f  topology_file.to
 00003760: 706f 6c6f 6779 5f66 696c 655f 7265 6164  pology_file_read
 00003770: 6572 948f 9428 68a9 8c1b 5051 416e 616c  er...(h...PQAnal
@@ -890,19 +890,19 @@
 00003790: 5f66 696c 6594 908c 3050 5141 6e61 6c79  _file...0PQAnaly
 000037a0: 7369 732e 696f 2e74 6f70 6f6c 6f67 795f  sis.io.topology_
 000037b0: 6669 6c65 2e74 6f70 6f6c 6f67 795f 6669  file.topology_fi
 000037c0: 6c65 5f77 7269 7465 7294 8f94 2868 a96a  le_writer...(h.j
 000037d0: f101 0000 908c 2a50 5141 6e61 6c79 7369  ......*PQAnalysi
 000037e0: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
 000037f0: 7265 6164 6572 2e65 7863 6570 7469 6f6e  reader.exception
-00003800: 7394 8f94 2868 bb68 c168 af68 dd90 8c31  s...(h.h.h.h...1
+00003800: 7394 8f94 2868 af68 bb68 dd68 c190 8c31  s...(h.h.h.h...1
 00003810: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
 00003820: 7075 745f 6669 6c65 5f72 6561 6465 722e  put_file_reader.
 00003830: 696e 7075 745f 6669 6c65 5f70 6172 7365  input_file_parse
-00003840: 7294 8f94 2868 bb68 c16a d501 0000 68c5  r...(h.h.j....h.
+00003840: 7294 8f94 2868 c56a d501 0000 68bb 68c1  r...(h.j....h.h.
 00003850: 908c 2250 5141 6e61 6c79 7369 732e 696f  .."PQAnalysis.io
 00003860: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
 00003870: 6572 2e70 7194 8f94 286a d501 0000 908c  er.pq...(j......
 00003880: 2b50 5141 6e61 6c79 7369 732e 696f 2e69  +PQAnalysis.io.i
 00003890: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
 000038a0: 2e70 715f 616e 616c 7973 6973 948f 9428  .pq_analysis...(
 000038b0: 6ad5 0100 0090 8c32 5051 416e 616c 7973  j......2PQAnalys
@@ -937,34 +937,34 @@
 00003a80: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
 00003a90: 696c 655f 7265 6164 6572 2e70 7194 908c  ile_reader.pq...
 00003aa0: 2f50 5141 6e61 6c79 7369 732e 696f 2e69  /PQAnalysis.io.i
 00003ab0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
 00003ac0: 2e70 712e 6f75 7470 7574 5f66 696c 6573  .pq.output_files
 00003ad0: 948f 9428 68c5 908c 2150 5141 6e61 6c79  ...(h...!PQAnaly
 00003ae0: 7369 732e 696f 2e67 656e 5f66 696c 652e  sis.io.gen_file.
-00003af0: 6578 6365 7074 696f 6e73 948f 9428 6a40  exceptions...(j@
+00003af0: 6578 6365 7074 696f 6e73 948f 9428 6a3f  exceptions...(j?
 00003b00: 0100 0090 8c17 5051 416e 616c 7973 6973  ......PQAnalysis
 00003b10: 2e61 6e61 6c79 7369 732e 7264 6694 8f94  .analysis.rdf...
 00003b20: 288c 1350 5141 6e61 6c79 7369 732e 616e  (..PQAnalysis.an
 00003b30: 616c 7973 6973 9490 8c1b 5051 416e 616c  alysis....PQAnal
 00003b40: 7973 6973 2e61 6e61 6c79 7369 732e 7264  ysis.analysis.rd
-00003b50: 662e 7264 6694 8f94 2868 db6a 1002 0000  f.rdf...(h.j....
-00003b60: 68e7 68d7 8c17 5051 416e 616c 7973 6973  h.h...PQAnalysis
-00003b70: 2e61 6e61 6c79 7369 732e 7264 6694 908c  .analysis.rdf...
+00003b50: 662e 7264 6694 8f94 288c 1750 5141 6e61  f.rdf...(..PQAna
+00003b60: 6c79 7369 732e 616e 616c 7973 6973 2e72  lysis.analysis.r
+00003b70: 6466 9468 d768 e76a 1002 0000 68db 908c  df.h.h.j....h...
 00003b80: 1b50 5141 6e61 6c79 7369 732e 616e 616c  .PQAnalysis.anal
 00003b90: 7973 6973 2e72 6466 2e61 7069 948f 9428  ysis.rdf.api...(
 00003ba0: 6a13 0200 0090 8c2d 5051 416e 616c 7973  j......-PQAnalys
 00003bb0: 6973 2e61 6e61 6c79 7369 732e 7264 662e  is.analysis.rdf.
 00003bc0: 7264 665f 696e 7075 745f 6669 6c65 5f72  rdf_input_file_r
 00003bd0: 6561 6465 7294 8f94 286a 1302 0000 68db  eader...(j....h.
 00003be0: 68e7 908c 2e50 5141 6e61 6c79 7369 732e  h....PQAnalysis.
 00003bf0: 616e 616c 7973 6973 2e72 6466 2e72 6466  analysis.rdf.rdf
 00003c00: 5f6f 7574 7075 745f 6669 6c65 5f77 7269  _output_file_wri
 00003c10: 7465 7294 8f94 286a 1302 0000 68db 906a  ter...(j....h..j
-00003c20: 4f01 0000 8f94 286a 1302 0000 68d9 908c  O.....(j....h...
+00003c20: 4e01 0000 8f94 286a 1302 0000 68d9 908c  N.....(j....h...
 00003c30: 1650 5141 6e61 6c79 7369 732e 636c 692e  .PQAnalysis.cli.
 00003c40: 7879 7a32 6765 6e94 8f94 2868 e390 8c19  xyz2gen...(h....
 00003c50: 5051 416e 616c 7973 6973 2e63 6c69 2e74  PQAnalysis.cli.t
 00003c60: 7261 6a32 716d 6366 6394 8f94 2868 e390  raj2qmcfc...(h..
 00003c70: 8c17 5051 416e 616c 7973 6973 2e63 6c69  ..PQAnalysis.cli
 00003c80: 2e74 7261 6a32 626f 7894 8f94 2868 e390  .traj2box...(h..
 00003c90: 8c16 5051 416e 616c 7973 6973 2e63 6c69  ..PQAnalysis.cli
@@ -978,28 +978,28 @@
 00003d10: 1c50 5141 6e61 6c79 7369 732e 636c 692e  .PQAnalysis.cli.
 00003d20: 6164 645f 6d6f 6c65 6375 6c65 7394 8f94  add_molecules...
 00003d30: 2868 e390 8c1d 5051 416e 616c 7973 6973  (h....PQAnalysis
 00003d40: 2e63 6c69 2e62 7569 6c64 5f6e 6570 5f74  .cli.build_nep_t
 00003d50: 7261 6a94 8f94 2868 e390 8c1f 5051 416e  raj...(h....PQAn
 00003d60: 616c 7973 6973 2e63 6c69 2e5f 6172 6775  alysis.cli._argu
 00003d70: 6d65 6e74 5f70 6172 7365 7294 8f94 2868  ment_parser...(h
-00003d80: e568 ed68 eb68 ef68 f968 f568 e768 f368  .h.h.h.h.h.h.h.h
-00003d90: e368 f790 8c18 5051 416e 616c 7973 6973  .h....PQAnalysis
+00003d80: e368 f368 ef68 f568 eb68 f768 e568 e768  .h.h.h.h.h.h.h.h
+00003d90: ed68 f990 8c18 5051 416e 616c 7973 6973  .h....PQAnalysis
 00003da0: 2e63 6c69 2e5f 636c 695f 6261 7365 948f  .cli._cli_base..
-00003db0: 9428 68e5 68ed 68eb 68ef 68f9 68f5 68e7  .(h.h.h.h.h.h.h.
-00003dc0: 68f3 68f7 908c 1d50 5141 6e61 6c79 7369  h.h....PQAnalysi
+00003db0: 9428 68f3 68ef 68f5 68eb 68f7 68e5 68e7  .(h.h.h.h.h.h.h.
+00003dc0: 68ed 68f9 908c 1d50 5141 6e61 6c79 7369  h.h....PQAnalysi
 00003dd0: 732e 746f 6f6c 732e 6164 645f 6d6f 6c65  s.tools.add_mole
 00003de0: 6375 6c65 948f 9428 68ed 908c 1c50 5141  cule...(h....PQA
 00003df0: 6e61 6c79 7369 732e 696f 2e6e 6570 2e6e  nalysis.io.nep.n
 00003e00: 6570 5f77 7269 7465 7294 8f94 2868 ef90  ep_writer...(h..
 00003e10: 8c0b 6172 6763 6f6d 706c 6574 6594 8f94  ..argcomplete...
 00003e20: 2868 f190 8c0d 7269 6368 5f61 7267 7061  (h....rich_argpa
 00003e30: 7273 6594 8f94 2868 f190 8c14 5051 416e  rse...(h....PQAn
 00003e40: 616c 7973 6973 2e63 6f72 652e 6365 6c6c  alysis.core.cell
-00003e50: 948f 9428 68ff 6a9f 0100 0090 8c14 5051  ...(h.j.......PQ
+00003e50: 948f 9428 6a9f 0100 0068 ff90 8c14 5051  ...(j....h....PQ
 00003e60: 416e 616c 7973 6973 2e63 6f72 652e 6174  Analysis.core.at
 00003e70: 6f6d 948f 9428 6a9f 0100 0068 fd90 8c17  om...(j....h....
 00003e80: 5051 416e 616c 7973 6973 2e63 6f72 652e  PQAnalysis.core.
 00003e90: 7265 7369 6475 6594 8f94 286a 9f01 0000  residue...(j....
 00003ea0: 908c 1350 5141 6e61 6c79 7369 732e 636f  ...PQAnalysis.co
 00003eb0: 7265 2e61 7069 948f 9428 6a9f 0100 0090  re.api...(j.....
 00003ec0: 8c19 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
@@ -1018,39 +1018,39 @@
 00003f90: 908c 1950 5141 6e61 6c79 7369 732e 636f  ...PQAnalysis.co
 00003fa0: 7265 2e61 746f 6d2e 6174 6f6d 948f 9428  re.atom.atom...(
 00003fb0: 6a4a 0200 0090 8c26 5051 416e 616c 7973  jJ.....&PQAnalys
 00003fc0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
 00003fd0: 2e61 746f 6d69 635f 7379 7374 656d 948f  .atomic_system..
 00003fe0: 9428 8c18 5051 416e 616c 7973 6973 2e61  .(..PQAnalysis.a
 00003ff0: 746f 6d69 635f 7379 7374 656d 9490 6a50  tomic_system..jP
-00004000: 0100 008f 9428 6a46 0100 006a 4101 0000  .....(jF...jA...
-00004010: 6a44 0100 006a 4f02 0000 908c 1773 6369  jD...jO......sci
+00004000: 0100 008f 9428 6a4f 0200 006a 4601 0000  .....(jO...jF...
+00004010: 6a41 0100 006a 4701 0000 908c 1773 6369  jA...jG......sci
 00004020: 7079 2e73 7061 7469 616c 2e74 7261 6e73  py.spatial.trans
 00004030: 666f 726d 948f 9428 6a41 0100 0090 8c24  form...(jA.....$
 00004040: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
 00004050: 635f 7379 7374 656d 2e5f 7072 6f70 6572  c_system._proper
 00004060: 7469 6573 948f 9428 6a41 0100 0090 8c2d  ties...(jA.....-
 00004070: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
 00004080: 635f 7379 7374 656d 2e5f 7374 616e 6461  c_system._standa
 00004090: 7264 5f70 726f 7065 7274 6965 7394 8f94  rd_properties...
 000040a0: 286a 4101 0000 908c 2350 5141 6e61 6c79  (jA.....#PQAnaly
 000040b0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
 000040c0: 6d2e 5f70 6f73 6974 696f 6e73 948f 9428  m._positions...(
 000040d0: 6a41 0100 0090 8c24 5051 416e 616c 7973  jA.....$PQAnalys
 000040e0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
 000040f0: 2e5f 6465 636f 7261 746f 7273 948f 9428  ._decorators...(
-00004100: 6a53 0100 006a 4401 0000 6a47 0100 0090  jS...jD...jG....
+00004100: 6a44 0100 006a 4701 0000 6a53 0100 0090  jD...jG...jS....
 00004110: 758c 1064 7570 6c69 6361 7465 645f 6c69  u..duplicated_li
 00004120: 6e65 7394 7d94 288c 136e 625f 6475 706c  nes.}.(..nb_dupl
 00004130: 6963 6174 6564 5f6c 696e 6573 944b 008c  icated_lines.K..
 00004140: 1870 6572 6365 6e74 5f64 7570 6c69 6361  .percent_duplica
 00004150: 7465 645f 6c69 6e65 7394 4700 0000 0000  ted_lines.G.....
 00004160: 0000 0075 8c0a 6e6f 6465 5f63 6f75 6e74  ...u..node_count
 00004170: 947d 9428 680e 4b4c 6809 4b75 680f 4d12  .}.(h.KLh.Kuh.M.
 00004180: 0268 104b 7d75 8c0c 756e 646f 6375 6d65  .h.K}u..undocume
 00004190: 6e74 6564 947d 9428 680e 4b00 6809 4b00  nted.}.(h.K.h.K.
 000041a0: 680f 4b00 6810 4b00 7568 184b 0168 194b  h.K.h.K.uh.K.h.K
 000041b0: 1f68 1a4b 0068 1b4b 0068 1c4b 3368 1d4d  .h.K.h.K.h.K3h.M
-000041c0: df11 681e 4b0b 8c0b 676c 6f62 616c 5f6e  ..h.K...global_n
-000041d0: 6f74 6594 4740 230c 07d5 7925 366a 5d02  ote.G@#...y%6j].
+000041c0: de11 681e 4b0a 8c0b 676c 6f62 616c 5f6e  ..h.K...global_n
+000041d0: 6f74 6594 4740 230d 18bc f320 936a 5d02  ote.G@#.... .j].
 000041e0: 0000 4b1b 6a5e 0200 0047 3fc1 f1e2 2523  ..K.j^...G?...%#
 000041f0: a31d 7562 2e                             ..ub.
```

### Comparing `pqanalysis-1.0.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `pqanalysis-1.0.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/.github/scripts/parse_pylint.py` & `pqanalysis-1.0.9/.github/scripts/parse_pylint.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/.github/workflows/ci.yml` & `pqanalysis-1.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/.github/workflows/docs.yml` & `pqanalysis-1.0.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/.github/workflows/pylint.yml` & `pqanalysis-1.0.9/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/.github/workflows/release.yml` & `pqanalysis-1.0.9/.github/workflows/release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -71,37 +71,44 @@
       id: previousTag
       run: |
         name=$(git --no-pager tag --sort=creatordate --merged ${{ github.ref_name }} | tail -2 | head -1)
         echo "previousTag: $name"
         echo "previousTag=$name" >> $GITHUB_ENV
         echo "::set-output name=previousTag::$name"
 
-    - name: Update CHANGELOG
-      id: changelog
-      uses: requarks/changelog-action@v1
-      with:
-        token: ${{ github.token }}
-        fromTag: ${{ github.ref_name }}
-        toTag: ${{ steps.previousTag.outputs.previousTag }}
-
-    - name: Commit CHANGELOG.md
-      uses: stefanzweifel/git-auto-commit-action@v4
-      with:
-        branch: main
-        commit_message: 'docs: update CHANGELOG.md for ${{ github.ref_name }} [skip ci]'
-        file_pattern: CHANGELOG.md
-
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
       run: >-
         gh release create
         '${{ github.ref_name }}'
         --repo '${{ github.repository }}'
-        --notes '${{ steps.changelog.outputs.changes }}'
+        --generate-notes
+
+    # - name: Create GitHub Changelog.md
+    #   env:
+    #     GITHUB_TOKEN: ${{ github.token }}
+    #   run: >-
+    #     gh release view
+    #     '${{ github.ref_name }}'
+
+    # - name: Add .github/.pylint_cache to the commit
+    #   run: |
+    #     git config --global user.email "github-actions[bot]@users.noreply.github.com"
+    #     git config --global user.name "github-actions[bot]"
+
+    #     git add CHANGELOG.md
+    #     git commit -m "Docs: Update CHANGELOG.md on release event"
+
+    # - name: Push changes
+    #   if: github.event_name == 'push'
+    #   uses: ad-m/github-push-action@master
+    #   with:
+    #     github_token: ${{ secrets.GITHUB_TOKEN }}
+    #     branch: 'main'
 
   pypi-release-update:
     name: >-
       Sign the Python distribution with Sigstore
       and upload them to GitHub Release
     needs:
     - publish-to-pypi
```

### Comparing `pqanalysis-1.0.8.1/.pylintrc` & `pqanalysis-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/CODE_OF_CONDUCT.md` & `pqanalysis-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/LICENSE` & `pqanalysis-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PKG-INFO` & `pqanalysis-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.8.1
+Version: 1.0.9
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,16 +33,14 @@
 Requires-Dist: sphinx-sitemap; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: better-apidoc; extra == "docs"
 Requires-Dist: six; extra == "docs"
 Requires-Dist: docstr-coverage; extra == "docs"
 
-<img src="docs/source/logo/PQAnalysis.png" width="250">
-
 # PQAnalysis
 
 [![CI](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml/badge.svg)](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml)
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/__init__.py` & `pqanalysis-1.0.9/PQAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/__init__.py` & `pqanalysis-1.0.9/PQAnalysis/analysis/rdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/api.py` & `pqanalysis-1.0.9/PQAnalysis/analysis/rdf/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/exceptions.py` & `pqanalysis-1.0.9/PQAnalysis/analysis/rdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf.py` & `pqanalysis-1.0.9/PQAnalysis/analysis/rdf/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf_input_file_reader.py` & `pqanalysis-1.0.9/PQAnalysis/analysis/rdf/rdf_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf_output_file_writer.py` & `pqanalysis-1.0.9/PQAnalysis/analysis/rdf/rdf_output_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_decorators.py` & `pqanalysis-1.0.9/PQAnalysis/atomic_system/_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_positions.py` & `pqanalysis-1.0.9/PQAnalysis/atomic_system/_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_properties.py` & `pqanalysis-1.0.9/PQAnalysis/atomic_system/_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_standard_properties.py` & `pqanalysis-1.0.9/PQAnalysis/atomic_system/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/atomic_system.py` & `pqanalysis-1.0.9/PQAnalysis/atomic_system/atomic_system.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/exceptions.py` & `pqanalysis-1.0.9/PQAnalysis/atomic_system/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/_argument_parser.py` & `pqanalysis-1.0.9/PQAnalysis/cli/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/_cli_base.py` & `pqanalysis-1.0.9/PQAnalysis/cli/_cli_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/add_molecules.py` & `pqanalysis-1.0.9/PQAnalysis/cli/add_molecules.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/build_nep_traj.py` & `pqanalysis-1.0.9/PQAnalysis/cli/build_nep_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/continue_input.py` & `pqanalysis-1.0.9/PQAnalysis/cli/continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/gen2xyz.py` & `pqanalysis-1.0.9/PQAnalysis/cli/gen2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/main.py` & `pqanalysis-1.0.9/PQAnalysis/cli/main.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/rdf.py` & `pqanalysis-1.0.9/PQAnalysis/cli/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/rst2xyz.py` & `pqanalysis-1.0.9/PQAnalysis/cli/rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/traj2box.py` & `pqanalysis-1.0.9/PQAnalysis/cli/traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/traj2qmcfc.py` & `pqanalysis-1.0.9/PQAnalysis/cli/traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/cli/xyz2gen.py` & `pqanalysis-1.0.9/PQAnalysis/cli/xyz2gen.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/core/__init__.py` & `pqanalysis-1.0.9/PQAnalysis/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/core/api.py` & `pqanalysis-1.0.9/PQAnalysis/core/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/core/atom/atom.py` & `pqanalysis-1.0.9/PQAnalysis/core/atom/atom.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/core/atom/element.py` & `pqanalysis-1.0.9/PQAnalysis/core/atom/element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/core/cell/_standard_properties.py` & `pqanalysis-1.0.9/PQAnalysis/core/cell/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/core/cell/cell.py` & `pqanalysis-1.0.9/PQAnalysis/core/cell/cell.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/core/exceptions.py` & `pqanalysis-1.0.9/PQAnalysis/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/core/residue.py` & `pqanalysis-1.0.9/PQAnalysis/core/residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/exceptions.py` & `pqanalysis-1.0.9/PQAnalysis/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/formats.py` & `pqanalysis-1.0.9/PQAnalysis/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/grammar/inputGrammar.lark` & `pqanalysis-1.0.9/PQAnalysis/grammar/inputGrammar.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/grammar/rules.lark` & `pqanalysis-1.0.9/PQAnalysis/grammar/rules.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/grammar/selection.lark` & `pqanalysis-1.0.9/PQAnalysis/grammar/selection.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/__init__.py` & `pqanalysis-1.0.9/PQAnalysis/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/api.py` & `pqanalysis-1.0.9/PQAnalysis/io/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/base.py` & `pqanalysis-1.0.9/PQAnalysis/io/base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/box_writer.py` & `pqanalysis-1.0.9/PQAnalysis/io/box_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/conversion_api.py` & `pqanalysis-1.0.9/PQAnalysis/io/conversion_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/energy_file_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/energy_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/exceptions.py` & `pqanalysis-1.0.9/PQAnalysis/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/formats.py` & `pqanalysis-1.0.9/PQAnalysis/io/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/api.py` & `pqanalysis-1.0.9/PQAnalysis/io/gen_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/gen_file_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/gen_file/gen_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/gen_file_writer.py` & `pqanalysis-1.0.9/PQAnalysis/io/gen_file/gen_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/info_file_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/info_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/exceptions.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/formats.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/input_file_parser.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/input_file_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/output_files.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq/output_files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/moldescriptor_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/moldescriptor_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/nep/nep_writer.py` & `pqanalysis-1.0.9/PQAnalysis/io/nep/nep_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/api.py` & `pqanalysis-1.0.9/PQAnalysis/io/restart_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/restart_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/restart_file/restart_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/restart_writer.py` & `pqanalysis-1.0.9/PQAnalysis/io/restart_file/restart_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/api.py` & `pqanalysis-1.0.9/PQAnalysis/io/topology_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/topology_file_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/topology_file/topology_file_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,25 +86,25 @@
             # remove all #.... parts from all lines
             lines = [line.split("#")[0] for line in lines]
 
             # remove all empty lines
             lines = [line for line in lines if line.strip()]
 
             # check if last line is END else raise error
-            if lines[-1].strip() != "END":
+            if lines[-1].strip().lower() != "end":
                 self.logger.error(
                     "Something went wrong. Each block should end with 'END'",
                     exception=TopologyFileError,
                 )
 
             # split all lines into blocks where each block ends with END
             blocks = []
             block = []
             for line in lines:
-                if line.strip().lower() == "END":
+                if line.strip().lower() == "end":
                     blocks.append(block)
                     block = []
                 else:
                     block.append(line)
 
             # make a dictionary for each block with the key
             # being the first word of the first line of each block
@@ -159,16 +159,15 @@
                 angles = self._parse_angles(value)
             elif key == "dihedrals":
                 dihedrals = self._parse_dihedrals(value)
             elif key == "impropers":
                 impropers = self._parse_impropers(value)
             else:
                 self.logger.error(
-                    f"Unknown block {key}",
-                    exception=TopologyFileError
+                    f"Unknown block {key}", exception=TopologyFileError
                 )
 
         return BondedTopology(
             bonds=bonds,
             angles=angles,
             dihedrals=dihedrals,
             impropers=impropers,
@@ -213,18 +212,18 @@
                 self.logger.error(
                     "Invalid number of columns in bond block. Expected 3 or 4.",
                     exception=TopologyFileError
                 )
 
             bonds.append(
                 Bond(
-                index1=int(index),
-                index2=int(target_index),
-                bond_type=int(bond_type),
-                is_linker=is_linker,
+                    index1=int(index),
+                    index2=int(target_index),
+                    bond_type=int(bond_type),
+                    is_linker=is_linker,
                 )
             )
 
         return bonds
 
     def _parse_angles(self, block: List[str]) -> List[Angle]:
         """
@@ -263,19 +262,19 @@
                 self.logger.error(
                     "Invalid number of columns in angle block. Expected 4 or 5.",
                     exception=TopologyFileError
                 )
 
             angles.append(
                 Angle(
-                index1=int(index1),
-                index2=int(index2),
-                index3=int(index3),
-                angle_type=int(angle_type),
-                is_linker=is_linker,
+                    index1=int(index1),
+                    index2=int(index2),
+                    index3=int(index3),
+                    angle_type=int(angle_type),
+                    is_linker=is_linker,
                 )
             )
 
         return angles
 
     def _parse_dihedrals(self, block: List[str]) -> List[Dihedral]:
         """
@@ -314,20 +313,20 @@
                 self.logger.error(
                     "Invalid number of columns in dihedral block. Expected 5 or 6.",
                     exception=TopologyFileError
                 )
 
             dihedrals.append(
                 Dihedral(
-                index1=int(index1),
-                index2=int(index2),
-                index3=int(index3),
-                index4=int(index4),
-                dihedral_type=int(dihedral_type),
-                is_linker=is_linker,
+                    index1=int(index1),
+                    index2=int(index2),
+                    index3=int(index3),
+                    index4=int(index4),
+                    dihedral_type=int(dihedral_type),
+                    is_linker=is_linker,
                 )
             )
 
         return dihedrals
 
     def _parse_impropers(self, block: List[str]) -> List[Dihedral]:
         """
@@ -366,21 +365,21 @@
                 self.logger.error(
                     "Invalid number of columns in dihedral block. Expected 5 or 6.",
                     exception=TopologyFileError
                 )
 
             dihedrals.append(
                 Dihedral(
-                index1=int(index1),
-                index2=int(index2),
-                index3=int(index3),
-                index4=int(index4),
-                dihedral_type=int(dihedral_type),
-                is_linker=is_linker,
-                is_improper=True,
+                    index1=int(index1),
+                    index2=int(index2),
+                    index3=int(index3),
+                    index4=int(index4),
+                    dihedral_type=int(dihedral_type),
+                    is_linker=is_linker,
+                    is_improper=True,
                 )
             )
 
         return dihedrals
 
     def _parse_shake(self, block: List[str]) -> List[Bond]:
         """
@@ -414,16 +413,16 @@
                 is_linker = True
             else:
                 index, target_index, distance = line.split()
                 is_linker = False
 
             shake_bonds.append(
                 Bond(
-                index1=int(index),
-                index2=int(target_index),
-                equilibrium_distance=float(distance),
-                is_linker=is_linker,
-                is_shake=True,
+                    index1=int(index),
+                    index2=int(target_index),
+                    equilibrium_distance=float(distance),
+                    is_linker=is_linker,
+                    is_shake=True,
                 )
             )
 
         return shake_bonds
```

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/topology_file_writer.py` & `pqanalysis-1.0.9/PQAnalysis/io/topology_file/topology_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/api.py` & `pqanalysis-1.0.9/PQAnalysis/io/traj_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/frame_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/traj_file/frame_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/trajectory_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/traj_file/trajectory_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/trajectory_writer.py` & `pqanalysis-1.0.9/PQAnalysis/io/traj_file/trajectory_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/virial/api.py` & `pqanalysis-1.0.9/PQAnalysis/io/virial/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/virial/virial_reader.py` & `pqanalysis-1.0.9/PQAnalysis/io/virial/virial_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/io/write_api.py` & `pqanalysis-1.0.9/PQAnalysis/io/write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/physical_data/energy.py` & `pqanalysis-1.0.9/PQAnalysis/physical_data/energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/tools/add_molecule.py` & `pqanalysis-1.0.9/PQAnalysis/tools/add_molecule.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/tools/traj_to_com_traj.py` & `pqanalysis-1.0.9/PQAnalysis/tools/traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/__init__.py` & `pqanalysis-1.0.9/PQAnalysis/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/api.py` & `pqanalysis-1.0.9/PQAnalysis/topology/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/_topology_properties.py` & `pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/_topology_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/angle.py` & `pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/bond.py` & `pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/bonded_topology.py` & `pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/bonded_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/dihedral.py` & `pqanalysis-1.0.9/PQAnalysis/topology/bonded_topology/dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/selection.py` & `pqanalysis-1.0.9/PQAnalysis/topology/selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/shake_topology.py` & `pqanalysis-1.0.9/PQAnalysis/topology/shake_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/topology/topology.py` & `pqanalysis-1.0.9/PQAnalysis/topology/topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/traj/api.py` & `pqanalysis-1.0.9/PQAnalysis/traj/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/traj/exceptions.py` & `pqanalysis-1.0.9/PQAnalysis/traj/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/traj/formats.py` & `pqanalysis-1.0.9/PQAnalysis/traj/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/traj/trajectory.py` & `pqanalysis-1.0.9/PQAnalysis/traj/trajectory.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/type_checking.py` & `pqanalysis-1.0.9/PQAnalysis/type_checking.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/types.py` & `pqanalysis-1.0.9/PQAnalysis/types.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/utils/common.py` & `pqanalysis-1.0.9/PQAnalysis/utils/common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/utils/custom_logging.py` & `pqanalysis-1.0.9/PQAnalysis/utils/custom_logging.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/utils/decorators.py` & `pqanalysis-1.0.9/PQAnalysis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/utils/files.py` & `pqanalysis-1.0.9/PQAnalysis/utils/files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/utils/math.py` & `pqanalysis-1.0.9/PQAnalysis/utils/math.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis/utils/random.py` & `pqanalysis-1.0.9/PQAnalysis/utils/random.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/PQAnalysis.egg-info/PKG-INFO` & `pqanalysis-1.0.9/PQAnalysis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.8.1
+Version: 1.0.9
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,16 +33,14 @@
 Requires-Dist: sphinx-sitemap; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: better-apidoc; extra == "docs"
 Requires-Dist: six; extra == "docs"
 Requires-Dist: docstr-coverage; extra == "docs"
 
-<img src="docs/source/logo/PQAnalysis.png" width="250">
-
 # PQAnalysis
 
 [![CI](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml/badge.svg)](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml)
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `pqanalysis-1.0.8.1/PQAnalysis.egg-info/SOURCES.txt` & `pqanalysis-1.0.9/PQAnalysis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .codecov.yml
 .docstr.yaml
 .gitignore
 .pylintrc
 .style.yapf
+CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE
 README.md
 pyproject.toml
 pytest.ini
 pytest.sh
 setup.cfg
@@ -280,14 +281,16 @@
 docs/source/developerGuide/developerGuide.rst
 docs/source/logo/PQAnalysis.png
 docs/source/userGuide/inputFile.rst
 docs/source/userGuide/userGuide.rst
 examples/add_molecules/mil68ga-md-01.rst
 examples/add_molecules/perylene-md-05.rst
 examples/add_molecules/perylene-md-05.xyz
+examples/add_molecules/shake_mil.top
+examples/add_molecules/shake_perylene.top
 examples/traj2box/.gitignore
 examples/traj2box/acof_triclinic.xyz
 examples/traj2box/acof_triclinic_2.xyz
 examples/traj2comtraj/umcm-9-md-01.xyz
 tests/__init__.py
 tests/conftest.py
 tests/test_formats.py
```

### Comparing `pqanalysis-1.0.8.1/README.md` & `pqanalysis-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-<img src="docs/source/logo/PQAnalysis.png" width="250">
-
 # PQAnalysis
 
 [![CI](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml/badge.svg)](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml)
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `pqanalysis-1.0.8.1/benchmarks/core/benchmark_traj_reader.py` & `pqanalysis-1.0.9/benchmarks/core/benchmark_traj_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/Makefile` & `pqanalysis-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/make.bat` & `pqanalysis-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/_templates/module.rst` & `pqanalysis-1.0.9/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/_templates/package.rst` & `pqanalysis-1.0.9/docs/source/_templates/package.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.atomic_system.exceptions.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.atomic_system.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.exceptions.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.api.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.io.traj_file.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.tools.add_molecule.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.tools.add_molecule.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.api.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.topology.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.custom_logging.rst` & `pqanalysis-1.0.9/docs/source/code/PQAnalysis.utils.custom_logging.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/conf.py` & `pqanalysis-1.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/developerGuide/developerGuide.rst` & `pqanalysis-1.0.9/docs/source/developerGuide/developerGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/logo/PQAnalysis.png` & `pqanalysis-1.0.9/docs/source/logo/PQAnalysis.png`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/userGuide/inputFile.rst` & `pqanalysis-1.0.9/docs/source/userGuide/inputFile.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/docs/source/userGuide/userGuide.rst` & `pqanalysis-1.0.9/docs/source/userGuide/userGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/examples/add_molecules/mil68ga-md-01.rst` & `pqanalysis-1.0.9/examples/add_molecules/mil68ga-md-01.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/examples/add_molecules/perylene-md-05.rst` & `pqanalysis-1.0.9/examples/add_molecules/perylene-md-05.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/examples/add_molecules/perylene-md-05.xyz` & `pqanalysis-1.0.9/examples/add_molecules/perylene-md-05.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/examples/traj2box/acof_triclinic.xyz` & `pqanalysis-1.0.9/examples/traj2box/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/examples/traj2box/acof_triclinic_2.xyz` & `pqanalysis-1.0.9/examples/traj2box/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/examples/traj2comtraj/umcm-9-md-01.xyz` & `pqanalysis-1.0.9/examples/traj2comtraj/umcm-9-md-01.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/pyproject.toml` & `pqanalysis-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/analysis/rdf/test_api.py` & `pqanalysis-1.0.9/tests/analysis/rdf/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdf.py` & `pqanalysis-1.0.9/tests/analysis/rdf/test_rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdfInputFileReader.py` & `pqanalysis-1.0.9/tests/analysis/rdf/test_rdfInputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdfOutputFileReader.py` & `pqanalysis-1.0.9/tests/analysis/rdf/test_rdfOutputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/atomicSystem/test_atomic_system.py` & `pqanalysis-1.0.9/tests/atomicSystem/test_atomic_system.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/atomicSystem/test_decorators.py` & `pqanalysis-1.0.9/tests/atomicSystem/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/atomicSystem/test_positions.py` & `pqanalysis-1.0.9/tests/atomicSystem/test_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/cli/test_continue_input.py` & `pqanalysis-1.0.9/tests/cli/test_continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/cli/test_rst2xyz.py` & `pqanalysis-1.0.9/tests/cli/test_rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/cli/test_traj2box.py` & `pqanalysis-1.0.9/tests/cli/test_traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/cli/test_traj2qmcfc.py` & `pqanalysis-1.0.9/tests/cli/test_traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/conftest.py` & `pqanalysis-1.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/core/atom/test_atom.py` & `pqanalysis-1.0.9/tests/core/atom/test_atom.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/core/atom/test_element.py` & `pqanalysis-1.0.9/tests/core/atom/test_element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/core/test_cell.py` & `pqanalysis-1.0.9/tests/core/test_cell.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/core/test_residue.py` & `pqanalysis-1.0.9/tests/core/test_residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/n_not_matching.in` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/n_not_matching.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/no_output_files.in` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/no_output_files.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/no_start_file.in` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/no_start_file.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-08.in` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-08.rpmd.in` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-08.rpmd.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-09.in.ref` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-09.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-10.in.ref` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-10.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref` & `pqanalysis-1.0.9/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/readEnergyFile/md-01.info` & `pqanalysis-1.0.9/tests/data/readEnergyFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/readInfoFile/md-01.info` & `pqanalysis-1.0.9/tests/data/readInfoFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/readInfoFile/md-01.qmcfc.info` & `pqanalysis-1.0.9/tests/data/readInfoFile/md-01.qmcfc.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/traj2qmcfc/acof_triclinic.xyz` & `pqanalysis-1.0.9/tests/data/traj2qmcfc/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/traj2qmcfc/acof_triclinic_2.xyz` & `pqanalysis-1.0.9/tests/data/traj2qmcfc/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/data/traj2qmcfc/traj.qmcfc.xyz` & `pqanalysis-1.0.9/tests/data/traj2qmcfc/traj.qmcfc.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py` & `pqanalysis-1.0.9/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/inputFileReader/PQAnalysis/test_parse.py` & `pqanalysis-1.0.9/tests/io/inputFileReader/PQAnalysis/test_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/inputFileReader/test_inputDictionary.py` & `pqanalysis-1.0.9/tests/io/inputFileReader/test_inputDictionary.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/inputFileReader/test_inputFileParser.py` & `pqanalysis-1.0.9/tests/io/inputFileReader/test_inputFileParser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/inputFileReader/test_transformers.py` & `pqanalysis-1.0.9/tests/io/inputFileReader/test_transformers.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/inputFileReader/test_visitors.py` & `pqanalysis-1.0.9/tests/io/inputFileReader/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_base.py` & `pqanalysis-1.0.9/tests/io/test_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_boxWriter.py` & `pqanalysis-1.0.9/tests/io/test_boxWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_energyFileReader.py` & `pqanalysis-1.0.9/tests/io/test_energyFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_frameReader.py` & `pqanalysis-1.0.9/tests/io/test_frameReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_infoFileReader.py` & `pqanalysis-1.0.9/tests/io/test_infoFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_moldescriptorReader.py` & `pqanalysis-1.0.9/tests/io/test_moldescriptorReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_restartReader.py` & `pqanalysis-1.0.9/tests/io/test_restartReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_restartWriter.py` & `pqanalysis-1.0.9/tests/io/test_restartWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_trajectoryReader.py` & `pqanalysis-1.0.9/tests/io/test_trajectoryReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_trajectoryWriter.py` & `pqanalysis-1.0.9/tests/io/test_trajectoryWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/io/test_write_api.py` & `pqanalysis-1.0.9/tests/io/test_write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/physicalData/test_energy.py` & `pqanalysis-1.0.9/tests/physicalData/test_energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/tools/test_traj_to_com_traj.py` & `pqanalysis-1.0.9/tests/tools/test_traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_angle.py` & `pqanalysis-1.0.9/tests/topology/bonded_topology/test_angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_bond.py` & `pqanalysis-1.0.9/tests/topology/bonded_topology/test_bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_bondedTopology.py` & `pqanalysis-1.0.9/tests/topology/bonded_topology/test_bondedTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_dihedral.py` & `pqanalysis-1.0.9/tests/topology/bonded_topology/test_dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/topology/test_selection.py` & `pqanalysis-1.0.9/tests/topology/test_selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/topology/test_selectionTransformer.py` & `pqanalysis-1.0.9/tests/topology/test_selectionTransformer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/topology/test_shakeTopology.py` & `pqanalysis-1.0.9/tests/topology/test_shakeTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/topology/test_topology.py` & `pqanalysis-1.0.9/tests/topology/test_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/traj/test_api.py` & `pqanalysis-1.0.9/tests/traj/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/traj/test_trajectory.py` & `pqanalysis-1.0.9/tests/traj/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/utils/test_common.py` & `pqanalysis-1.0.9/tests/utils/test_common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/utils/test_decorators.py` & `pqanalysis-1.0.9/tests/utils/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.8.1/tests/utils/test_math.py` & `pqanalysis-1.0.9/tests/utils/test_math.py`

 * *Files identical despite different names*

