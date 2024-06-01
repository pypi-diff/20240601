# Comparing `tmp/sxs-2023.1.2.tar.gz` & `tmp/sxs-2023.1.3.tar.gz`

## Comparing `sxs-2023.1.2.tar` & `sxs-2023.1.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2023.1.2/.codecov.yml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2023.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2023.1.2/CITATION.cff
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 sxs-2023.1.2/mkdocs.yml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sxs-2023.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2023.1.2/.github/scripts/parse_bump_rule.py
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 sxs-2023.1.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2023.1.2/.github/workflows/pr_rtd_link.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/index.md -> ../README.md
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/mathematica.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/api/catalog.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/api/horizons.md
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/api/load.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/api/metadata.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/api/time_series.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/api/waveforms.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/html/main.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/images/favicon.ico
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/javascript/mathjax.js
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/stylesheets/extra.css
--rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/tutorials/00-Introduction.ipynb
--rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/tutorials/01-Metadata.ipynb
--rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/tutorials/02-Catalog.ipynb
--rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/tutorials/03-Horizons.ipynb
--rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/tutorials/04-Waveforms.ipynb
--rw-r--r--   0        0        0  2744774 2020-02-02 00:00:00.000000 sxs-2023.1.2/docs/tutorials/05-PreprocessingForFFTs.ipynb
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/__version__.py
--rw-r--r--   0        0        0    20929 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/handlers.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/juliapkg.json
--rw-r--r--   0        0        0    39641 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/time_series.py
--rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/caltechdata/__init__.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/caltechdata/catalog.py
--rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/caltechdata/login.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/catalog/__init__.py
--rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/catalog/catalog.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/catalog/create.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/catalog/description.py
--rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/horizons/__init__.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/horizons/spec_horizons_h5.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/horizons/xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/julia/__init__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/metadata/__init__.py
--rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/metadata/metadata.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/__init__.py
--rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/bitwise.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/dicts.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/downloads.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/files.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/formats.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/inspire.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/monotonicity.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/pretty_print.py
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/select.py
--rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/smooth_functions.py
--rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/sxs_directories.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/sxs_identifiers.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/url.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/decimation/__init__.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/decimation/greedy_spline.py
--rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/decimation/linear_bisection.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/decimation/peak_greed.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/decimation/suppression.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/lvcnr/__init__.py
--rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/lvcnr/comparisons.py
--rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/lvcnr/conversion.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/lvcnr/dataset.py
--rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/lvcnr/horizons.py
--rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/lvcnr/metadata.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/lvcnr/waveform_amp_phase.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/lvcnr/waveforms.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/references/__init__.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/references/ads.py
--rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/references/arxiv.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/references/fairchild_report.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/references/inspire.py
--rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/references/journal_abbreviations.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/utilities/references/references.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/__init__.py
--rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/alignment.py
--rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/memory.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/mode_utilities.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/transformations.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/waveform_grid.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/waveform_mixin.py
--rw-r--r--   0        0        0    56594 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/waveform_modes.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/waveform_signal.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/format_handlers/__init__.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/format_handlers/lvc.py
--rw-r--r--   0        0        0    20431 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/format_handlers/nrar.py
--rw-r--r--   0        0        0    27340 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/waveforms/format_handlers/spectre_cce_v1.py
--rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/__init__.py
--rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/catalog.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/creators.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/simannex.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/surrogatemodeling.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/api/__init__.py
--rw-r--r--   0        0        0    36946 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/api/deposit.py
--rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/api/login.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2023.1.2/sxs/zenodo/api/records.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/__init__.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/conftest.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_catalog.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_horizons.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_loader.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_metadata.py
--rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_time_series.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_transformations.py
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_utilities.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_waveform_rotations.py
--rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sxs-2023.1.2/tests/test_waveforms.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 sxs-2023.1.2/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2023.1.2/LICENSE
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 sxs-2023.1.2/README.md
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 sxs-2023.1.2/pyproject.toml
--rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 sxs-2023.1.2/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2023.1.3/.codecov.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2023.1.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2023.1.3/CITATION.cff
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 sxs-2023.1.3/mkdocs.yml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sxs-2023.1.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2023.1.3/.github/scripts/parse_bump_rule.py
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 sxs-2023.1.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2023.1.3/.github/workflows/pr_rtd_link.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/mathematica.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/api/catalog.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/api/horizons.md
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/api/load.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/api/metadata.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/api/time_series.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/api/waveforms.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/html/main.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/images/favicon.ico
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/javascript/mathjax.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/tutorials/00-Introduction.ipynb
+-rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/tutorials/01-Metadata.ipynb
+-rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/tutorials/02-Catalog.ipynb
+-rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/tutorials/03-Horizons.ipynb
+-rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/tutorials/04-Waveforms.ipynb
+-rw-r--r--   0        0        0  2744774 2020-02-02 00:00:00.000000 sxs-2023.1.3/docs/tutorials/05-PreprocessingForFFTs.ipynb
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/__version__.py
+-rw-r--r--   0        0        0    20929 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/handlers.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/juliapkg.json
+-rw-r--r--   0        0        0    39641 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/time_series.py
+-rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/caltechdata/__init__.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/caltechdata/catalog.py
+-rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/caltechdata/login.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/catalog/__init__.py
+-rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/catalog/catalog.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/catalog/create.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/catalog/description.py
+-rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/horizons/__init__.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/horizons/spec_horizons_h5.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/horizons/xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/julia/__init__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/metadata/__init__.py
+-rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/metadata/metadata.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/__init__.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/bitwise.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/dicts.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/downloads.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/files.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/formats.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/inspire.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/monotonicity.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/pretty_print.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/select.py
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/smooth_functions.py
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/sxs_directories.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/sxs_identifiers.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/url.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/decimation/__init__.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/decimation/greedy_spline.py
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/decimation/linear_bisection.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/decimation/peak_greed.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/decimation/suppression.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/lvcnr/__init__.py
+-rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/lvcnr/comparisons.py
+-rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/lvcnr/conversion.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/lvcnr/dataset.py
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/lvcnr/horizons.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/lvcnr/metadata.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/lvcnr/waveform_amp_phase.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/lvcnr/waveforms.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/references/__init__.py
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/references/ads.py
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/references/arxiv.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/references/fairchild_report.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/references/inspire.py
+-rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/references/journal_abbreviations.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/utilities/references/references.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/__init__.py
+-rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/alignment.py
+-rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/memory.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/mode_utilities.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/transformations.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/waveform_grid.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/waveform_mixin.py
+-rw-r--r--   0        0        0    56594 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/waveform_modes.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/waveform_signal.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/format_handlers/__init__.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/format_handlers/lvc.py
+-rw-r--r--   0        0        0    20431 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/format_handlers/nrar.py
+-rw-r--r--   0        0        0    27340 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/waveforms/format_handlers/spectre_cce_v1.py
+-rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/__init__.py
+-rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/catalog.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/creators.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/simannex.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/surrogatemodeling.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/api/__init__.py
+-rw-r--r--   0        0        0    36946 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/api/deposit.py
+-rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/api/login.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2023.1.3/sxs/zenodo/api/records.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_catalog.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_horizons.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_loader.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_metadata.py
+-rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_time_series.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_transformations.py
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_utilities.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_waveform_rotations.py
+-rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sxs-2023.1.3/tests/test_waveforms.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 sxs-2023.1.3/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2023.1.3/LICENSE
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 sxs-2023.1.3/README.md
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 sxs-2023.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 sxs-2023.1.3/PKG-INFO
```

### Comparing `sxs-2023.1.2/mkdocs.yml` & `sxs-2023.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/.github/workflows/build.yml` & `sxs-2023.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/docs/mathematica.md` & `sxs-2023.1.3/docs/mathematica.md`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/docs/images/favicon.ico` & `sxs-2023.1.3/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/docs/tutorials/00-Introduction.ipynb` & `sxs-2023.1.3/docs/tutorials/00-Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/docs/tutorials/01-Metadata.ipynb` & `sxs-2023.1.3/docs/tutorials/01-Metadata.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/docs/tutorials/02-Catalog.ipynb` & `sxs-2023.1.3/docs/tutorials/02-Catalog.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/docs/tutorials/03-Horizons.ipynb` & `sxs-2023.1.3/docs/tutorials/03-Horizons.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/docs/tutorials/04-Waveforms.ipynb` & `sxs-2023.1.3/docs/tutorials/04-Waveforms.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/docs/tutorials/05-PreprocessingForFFTs.ipynb` & `sxs-2023.1.3/docs/tutorials/05-PreprocessingForFFTs.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/__init__.py` & `sxs-2023.1.3/sxs/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/handlers.py` & `sxs-2023.1.3/sxs/handlers.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/time_series.py` & `sxs-2023.1.3/sxs/time_series.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/caltechdata/__init__.py` & `sxs-2023.1.3/sxs/caltechdata/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/caltechdata/catalog.py` & `sxs-2023.1.3/sxs/caltechdata/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/caltechdata/login.py` & `sxs-2023.1.3/sxs/caltechdata/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/catalog/catalog.py` & `sxs-2023.1.3/sxs/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/catalog/create.py` & `sxs-2023.1.3/sxs/catalog/create.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/catalog/description.py` & `sxs-2023.1.3/sxs/catalog/description.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/horizons/__init__.py` & `sxs-2023.1.3/sxs/horizons/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/horizons/spec_horizons_h5.py` & `sxs-2023.1.3/sxs/horizons/spec_horizons_h5.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/horizons/xor_multishuffle_bzip2.py` & `sxs-2023.1.3/sxs/horizons/xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/julia/__init__.py` & `sxs-2023.1.3/sxs/julia/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import juliacall
 
 
 PostNewtonian = juliacall.newmodule("PN")
 PostNewtonian.seval("using PostNewtonian")
 
 
-def update():
-    """Update the Julia packages."""
+def pkg_update():
+    """Update all installed Julia packages (but not julia itself)."""
     PostNewtonian.seval("import Pkg")
     return PostNewtonian.seval("Pkg.update()")
 
 
 def PNWaveform(M1, M2, chi1, chi2, Omega_i, **kwargs):
     """Generate a PN waveform.
```

### Comparing `sxs-2023.1.2/sxs/metadata/metadata.py` & `sxs-2023.1.3/sxs/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/__init__.py` & `sxs-2023.1.3/sxs/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/bitwise.py` & `sxs-2023.1.3/sxs/utilities/bitwise.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/dicts.py` & `sxs-2023.1.3/sxs/utilities/dicts.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/downloads.py` & `sxs-2023.1.3/sxs/utilities/downloads.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/files.py` & `sxs-2023.1.3/sxs/utilities/files.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/formats.py` & `sxs-2023.1.3/sxs/utilities/formats.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/inspire.py` & `sxs-2023.1.3/sxs/utilities/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/monotonicity.py` & `sxs-2023.1.3/sxs/utilities/monotonicity.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/pretty_print.py` & `sxs-2023.1.3/sxs/utilities/pretty_print.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/select.py` & `sxs-2023.1.3/sxs/utilities/select.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/smooth_functions.py` & `sxs-2023.1.3/sxs/utilities/smooth_functions.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/sxs_directories.py` & `sxs-2023.1.3/sxs/utilities/sxs_directories.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/sxs_identifiers.py` & `sxs-2023.1.3/sxs/utilities/sxs_identifiers.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/url.py` & `sxs-2023.1.3/sxs/utilities/url.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/decimation/__init__.py` & `sxs-2023.1.3/sxs/utilities/decimation/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/decimation/greedy_spline.py` & `sxs-2023.1.3/sxs/utilities/decimation/greedy_spline.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/decimation/linear_bisection.py` & `sxs-2023.1.3/sxs/utilities/decimation/linear_bisection.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/decimation/peak_greed.py` & `sxs-2023.1.3/sxs/utilities/decimation/peak_greed.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/decimation/suppression.py` & `sxs-2023.1.3/sxs/utilities/decimation/suppression.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/lvcnr/__init__.py` & `sxs-2023.1.3/sxs/utilities/lvcnr/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/lvcnr/comparisons.py` & `sxs-2023.1.3/sxs/utilities/lvcnr/comparisons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/lvcnr/conversion.py` & `sxs-2023.1.3/sxs/utilities/lvcnr/conversion.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/lvcnr/dataset.py` & `sxs-2023.1.3/sxs/utilities/lvcnr/dataset.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/lvcnr/horizons.py` & `sxs-2023.1.3/sxs/utilities/lvcnr/horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/lvcnr/metadata.py` & `sxs-2023.1.3/sxs/utilities/lvcnr/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/lvcnr/waveform_amp_phase.py` & `sxs-2023.1.3/sxs/utilities/lvcnr/waveform_amp_phase.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/lvcnr/waveforms.py` & `sxs-2023.1.3/sxs/utilities/lvcnr/waveforms.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/references/ads.py` & `sxs-2023.1.3/sxs/utilities/references/ads.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/references/arxiv.py` & `sxs-2023.1.3/sxs/utilities/references/arxiv.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/references/fairchild_report.py` & `sxs-2023.1.3/sxs/utilities/references/fairchild_report.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/references/inspire.py` & `sxs-2023.1.3/sxs/utilities/references/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/utilities/references/journal_abbreviations.py` & `sxs-2023.1.3/sxs/utilities/references/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/__init__.py` & `sxs-2023.1.3/sxs/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/alignment.py` & `sxs-2023.1.3/sxs/waveforms/alignment.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/memory.py` & `sxs-2023.1.3/sxs/waveforms/memory.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/mode_utilities.py` & `sxs-2023.1.3/sxs/waveforms/mode_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/transformations.py` & `sxs-2023.1.3/sxs/waveforms/transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/waveform_mixin.py` & `sxs-2023.1.3/sxs/waveforms/waveform_mixin.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/waveform_modes.py` & `sxs-2023.1.3/sxs/waveforms/waveform_modes.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/format_handlers/lvc.py` & `sxs-2023.1.3/sxs/waveforms/format_handlers/lvc.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/format_handlers/nrar.py` & `sxs-2023.1.3/sxs/waveforms/format_handlers/nrar.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py` & `sxs-2023.1.3/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py` & `sxs-2023.1.3/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/waveforms/format_handlers/spectre_cce_v1.py` & `sxs-2023.1.3/sxs/waveforms/format_handlers/spectre_cce_v1.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/zenodo/__init__.py` & `sxs-2023.1.3/sxs/zenodo/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/zenodo/catalog.py` & `sxs-2023.1.3/sxs/zenodo/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/zenodo/creators.py` & `sxs-2023.1.3/sxs/zenodo/creators.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/zenodo/simannex.py` & `sxs-2023.1.3/sxs/zenodo/simannex.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/zenodo/surrogatemodeling.py` & `sxs-2023.1.3/sxs/zenodo/surrogatemodeling.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/zenodo/api/deposit.py` & `sxs-2023.1.3/sxs/zenodo/api/deposit.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/zenodo/api/login.py` & `sxs-2023.1.3/sxs/zenodo/api/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/sxs/zenodo/api/records.py` & `sxs-2023.1.3/sxs/zenodo/api/records.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/conftest.py` & `sxs-2023.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_catalog.py` & `sxs-2023.1.3/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_horizons.py` & `sxs-2023.1.3/tests/test_horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_loader.py` & `sxs-2023.1.3/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_metadata.py` & `sxs-2023.1.3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_time_series.py` & `sxs-2023.1.3/tests/test_time_series.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_transformations.py` & `sxs-2023.1.3/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_utilities.py` & `sxs-2023.1.3/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_waveform_rotations.py` & `sxs-2023.1.3/tests/test_waveform_rotations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/tests/test_waveforms.py` & `sxs-2023.1.3/tests/test_waveforms.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/.gitignore` & `sxs-2023.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/LICENSE` & `sxs-2023.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/README.md` & `sxs-2023.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/pyproject.toml` & `sxs-2023.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.2/PKG-INFO` & `sxs-2023.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sxs
-Version: 2023.1.2
+Version: 2023.1.3
 Summary: Interface to data produced by the Simulating eXtreme Spacetimes collaboration
 Project-URL: Homepage, https://github.com/sxs-collaboration/sxs
 Project-URL: Documentation, https://sxs.readthedocs.io/
 Author-email: Michael Boyle <michael.oliver.boyle@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Michael Boyle
```

