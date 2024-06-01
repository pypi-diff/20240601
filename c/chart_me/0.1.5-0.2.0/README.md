# Comparing `tmp/chart_me-0.1.5.tar.gz` & `tmp/chart_me-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chart_me-0.1.5.tar", last modified: Sat May 28 21:08:36 2022, max compression
+gzip compressed data, was "chart_me-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `chart_me-0.1.5.tar` & `chart_me-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      186 2022-05-28 21:06:41.650210 chart_me-0.1.5/.bumpversion.cfg
--rw-r--r--   0        0        0     1245 2022-05-28 19:00:54.312570 chart_me-0.1.5/.circleci/config.yml
--rw-r--r--   0        0        0      515 2022-05-28 20:08:14.572230 chart_me-0.1.5/.github/workflows/action_tox.yml
--rw-r--r--   0        0        0      177 2022-05-28 11:04:03.176389 chart_me-0.1.5/.gitignore
--rw-r--r--   0        0        0      811 2022-05-28 11:59:39.324038 chart_me-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      208 2022-05-23 01:37:25.943009 chart_me-0.1.5/.readthedocs.yml
--rw-r--r--   0        0        0       16 2022-05-22 20:41:31.276174 chart_me-0.1.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1099 2022-05-01 12:07:10.583278 chart_me-0.1.5/LICENSE
--rw-r--r--   0        0        0      638 2022-05-01 12:50:48.638319 chart_me-0.1.5/Makefile
--rw-r--r--   0        0        0    13811 2022-05-24 11:28:36.233236 chart_me-0.1.5/Notes_Requirements.xlsx
--rw-r--r--   0        0        0     1952 2022-05-28 21:06:41.648209 chart_me-0.1.5/README.md
--rw-r--r--   0        0        0      638 2022-05-01 12:56:23.171866 chart_me-0.1.5/docs/Makefile
--rwxr-xr-x   0        0        0      804 2022-05-01 12:56:23.174861 chart_me-0.1.5/docs/make.bat
--rw-r--r--   0        0        0    20751 2022-05-23 01:06:46.496142 chart_me-0.1.5/docs/source/_static/Example_Screenshot.png
--rw-r--r--   0        0        0      102 2022-05-23 01:11:34.530546 chart_me-0.1.5/docs/source/architecture.md
--rw-r--r--   0        0        0      375 2022-05-23 10:45:47.264127 chart_me-0.1.5/docs/source/backlog.md
--rw-r--r--   0        0        0     2127 2022-05-27 13:07:37.349470 chart_me-0.1.5/docs/source/conf.py
--rw-r--r--   0        0        0       61 2022-05-22 20:40:49.581345 chart_me-0.1.5/docs/source/contributing.md
--rw-r--r--   0        0        0    80831 2022-05-28 21:04:18.951504 chart_me-0.1.5/docs/source/example.ipynb
--rw-r--r--   0        0        0      146 2022-05-23 01:46:30.103399 chart_me-0.1.5/docs/source/index.md
--rw-r--r--   0        0        0       42 2022-05-28 11:04:03.092389 chart_me-0.1.5/docs/source/requirements.txt
--rw-r--r--   0        0        0   165666 2022-05-28 21:04:16.254844 chart_me-0.1.5/examples/sample_1_univariate.ipynb
--rw-r--r--   0        0        0     1114 2022-05-26 10:57:39.758836 chart_me-0.1.5/interrogate_badge.svg
--rw-r--r--   0        0        0      232 2022-05-25 12:36:18.459856 chart_me-0.1.5/interrogate_report_manual.py
--rwxr-xr-x   0        0        0      804 2022-05-01 12:50:48.641320 chart_me-0.1.5/make.bat
--rw-r--r--   0        0        0     1050 2022-05-28 12:06:55.143107 chart_me-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       53 2022-05-28 11:04:03.129390 chart_me-0.1.5/setup.cfg
--rw-r--r--   0        0        0      257 2022-05-28 21:06:41.649210 chart_me-0.1.5/src/chart_me/__init__.py
--rw-r--r--   0        0        0      885 2022-05-28 12:38:47.381671 chart_me-0.1.5/src/chart_me/chart_configs.py
--rw-r--r--   0        0        0     1622 2022-05-28 12:38:14.449558 chart_me-0.1.5/src/chart_me/chart_me_logic.py
--rw-r--r--   0        0        0     4400 2022-05-27 12:32:34.223699 chart_me-0.1.5/src/chart_me/charting_assembly_strategy/__init__.py
--rw-r--r--   0        0        0    11641 2022-05-28 11:57:30.811510 chart_me-0.1.5/src/chart_me/charting_assembly_strategy/bivariate.py
--rw-r--r--   0        0        0     3224 2022-05-27 13:01:52.658945 chart_me-0.1.5/src/chart_me/charting_assembly_strategy/univariate.py
--rw-r--r--   0        0        0     2473 2022-05-28 20:21:14.942227 chart_me-0.1.5/src/chart_me/data_validation_strategy.py
--rw-r--r--   0        0        0     8885 2022-05-28 12:36:16.253077 chart_me-0.1.5/src/chart_me/datatype_infer_strategy.py
--rw-r--r--   0        0        0     1035 2022-05-27 12:51:38.828327 chart_me-0.1.5/src/chart_me/errors.py
--rw-r--r--   0        0        0     2329 2022-05-28 21:04:40.250783 chart_me-0.1.5/src/chart_me/pandas_util.py
--rw-r--r--   0        0        0     3194 2022-05-27 13:05:41.311421 chart_me-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     5676 2022-05-27 13:06:26.858643 chart_me-0.1.5/tests/test_datatype_infer_strategy.py
--rw-r--r--   0        0        0     1331 2022-05-27 13:06:31.837819 chart_me-0.1.5/tests/test_validate_strategy.py
--rw-r--r--   0        0        0      553 2022-05-28 11:04:03.145389 chart_me-0.1.5/tox.ini
--rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 chart_me-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      186 2022-05-28 21:06:41.650210 chart_me-0.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1245 2022-05-28 19:00:54.312570 chart_me-0.2.0/.circleci/config.yml
+-rw-r--r--   0        0        0      553 2024-06-01 00:01:11.771285 chart_me-0.2.0/.github/workflows/action_tox.yml
+-rw-r--r--   0        0        0      177 2022-05-28 11:04:03.176389 chart_me-0.2.0/.gitignore
+-rw-r--r--   0        0        0      628 2024-05-31 21:43:46.212967 chart_me-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      252 2024-06-01 13:58:31.098930 chart_me-0.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0       16 2022-05-22 20:41:31.276174 chart_me-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1099 2022-05-01 12:07:10.583278 chart_me-0.2.0/LICENSE
+-rw-r--r--   0        0        0      638 2022-05-01 12:50:48.638319 chart_me-0.2.0/Makefile
+-rw-r--r--   0        0        0    13811 2022-05-24 11:28:36.233236 chart_me-0.2.0/Notes_Requirements.xlsx
+-rw-r--r--   0        0        0     1952 2022-05-28 21:06:41.648209 chart_me-0.2.0/README.md
+-rw-r--r--   0        0        0      638 2022-05-01 12:56:23.171866 chart_me-0.2.0/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2022-05-01 12:56:23.174861 chart_me-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0    20751 2022-05-23 01:06:46.496142 chart_me-0.2.0/docs/source/_static/Example_Screenshot.png
+-rw-r--r--   0        0        0       95 2024-05-31 22:43:26.029600 chart_me-0.2.0/docs/source/architecture.md
+-rw-r--r--   0        0        0      375 2022-05-23 10:45:47.264127 chart_me-0.2.0/docs/source/backlog.md
+-rw-r--r--   0        0        0     2127 2022-05-27 13:07:37.349470 chart_me-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0       61 2022-05-22 20:40:49.581345 chart_me-0.2.0/docs/source/contributing.md
+-rw-r--r--   0        0        0    80831 2022-05-28 21:04:18.951504 chart_me-0.2.0/docs/source/example.ipynb
+-rw-r--r--   0        0        0      146 2022-05-23 01:46:30.103399 chart_me-0.2.0/docs/source/index.md
+-rw-r--r--   0        0        0       42 2022-05-28 11:04:03.092389 chart_me-0.2.0/docs/source/requirements.txt
+-rw-r--r--   0        0        0   165531 2024-05-19 18:15:07.119022 chart_me-0.2.0/examples/sample_1_univariate.ipynb
+-rw-r--r--   0        0        0     1114 2022-05-26 10:57:39.758836 chart_me-0.2.0/interrogate_badge.svg
+-rw-r--r--   0        0        0      232 2022-05-25 12:36:18.459856 chart_me-0.2.0/interrogate_report_manual.py
+-rwxr-xr-x   0        0        0      804 2022-05-01 12:50:48.641320 chart_me-0.2.0/make.bat
+-rw-r--r--   0        0        0     1116 2024-06-01 00:08:32.376970 chart_me-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       53 2022-05-28 11:04:03.129390 chart_me-0.2.0/setup.cfg
+-rw-r--r--   0        0        0      257 2024-06-01 13:23:07.543323 chart_me-0.2.0/src/chart_me/__init__.py
+-rw-r--r--   0        0        0      205 2024-06-01 00:02:03.026873 chart_me-0.2.0/src/chart_me/__main__.py
+-rw-r--r--   0        0        0      885 2022-05-28 12:38:47.381671 chart_me-0.2.0/src/chart_me/chart_configs.py
+-rw-r--r--   0        0        0     1622 2022-05-28 12:38:14.449558 chart_me-0.2.0/src/chart_me/chart_me_logic.py
+-rw-r--r--   0        0        0     4400 2022-05-27 12:32:34.223699 chart_me-0.2.0/src/chart_me/charting_assembly_strategy/__init__.py
+-rw-r--r--   0        0        0    11641 2022-05-28 11:57:30.811510 chart_me-0.2.0/src/chart_me/charting_assembly_strategy/bivariate.py
+-rw-r--r--   0        0        0     3224 2022-05-27 13:01:52.658945 chart_me-0.2.0/src/chart_me/charting_assembly_strategy/univariate.py
+-rw-r--r--   0        0        0     2473 2022-05-28 20:21:14.942227 chart_me-0.2.0/src/chart_me/data_validation_strategy.py
+-rw-r--r--   0        0        0     8885 2022-05-28 12:36:16.253077 chart_me-0.2.0/src/chart_me/datatype_infer_strategy.py
+-rw-r--r--   0        0        0     1035 2022-05-27 12:51:38.828327 chart_me-0.2.0/src/chart_me/errors.py
+-rw-r--r--   0        0        0     2329 2022-05-28 21:04:40.250783 chart_me-0.2.0/src/chart_me/pandas_util.py
+-rw-r--r--   0        0        0     3194 2022-05-27 13:05:41.311421 chart_me-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     5676 2022-05-27 13:06:26.858643 chart_me-0.2.0/tests/test_datatype_infer_strategy.py
+-rw-r--r--   0        0        0     1331 2022-05-27 13:06:31.837819 chart_me-0.2.0/tests/test_validate_strategy.py
+-rw-r--r--   0        0        0      550 2024-05-31 23:55:36.379999 chart_me-0.2.0/tox.ini
+-rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 chart_me-0.2.0/PKG-INFO
```

### Comparing `chart_me-0.1.5/.circleci/config.yml` & `chart_me-0.2.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/.github/workflows/action_tox.yml` & `chart_me-0.2.0/.github/workflows/action_tox.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 name: Python package
 
-on: [push]
+on:
+  push:
+    branches:
+      - "master"
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python: ["3.7", "3.8", "3.9"]
+        python: ["3.10", "3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python }}
```

### Comparing `chart_me-0.1.5/.pre-commit-config.yaml` & `chart_me-0.2.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 default_language_version:
-  python: python3.9
+  python: python3.12
 exclude: "venv"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
@@ -17,19 +17,12 @@
 
   - repo: https://github.com/ambv/black
     rev: 22.3.0
     hooks:
       - id: black
         language_version: python3.9
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
-    hooks:
-      - id: flake8
-        language: python_venv
-        additional_dependencies: ["flake8-comprehensions"]
-
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.960
     hooks:
       - id: mypy
         exclude: ^tests/
```

### Comparing `chart_me-0.1.5/LICENSE` & `chart_me-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/Makefile` & `chart_me-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/Notes_Requirements.xlsx` & `chart_me-0.2.0/Notes_Requirements.xlsx`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/README.md` & `chart_me-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/docs/Makefile` & `chart_me-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/docs/make.bat` & `chart_me-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/docs/source/_static/Example_Screenshot.png` & `chart_me-0.2.0/docs/source/_static/Example_Screenshot.png`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/docs/source/conf.py` & `chart_me-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/docs/source/example.ipynb` & `chart_me-0.2.0/docs/source/example.ipynb`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/examples/sample_1_univariate.ipynb` & `chart_me-0.2.0/examples/sample_1_univariate.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9528220399787336%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'data': {'text/html': {insert: [(1, '<div "*

 * *            'id="altair-viz-b4a3abd5fe204d288fb2ce08eedcf317"></div>\\n\'), (6, \'    if '*

 * *            '(outputDiv.id !== "altair-viz-b4a3abd5fe204d288fb2ce08eedcf317") {\\n\'), (7, \'      '*

 * *            'outputDiv = '*

 * *            'document.getElementById("altair-viz-b4a3abd5fe204d288fb2ce08eedcf317");\\n\'), (53, '*

 * *            '\'  })({"config": {"view": {"continuousWidth": 400, "continuousHeight": 300}}, '*

 * *            '"data": { […]*

```diff
@@ -39,21 +39,21 @@
             "id": "31c0aef1",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
-                            "<div id=\"altair-viz-8333cb2b19d2476e8e1e59d8634646d4\"></div>\n",
+                            "<div id=\"altair-viz-b4a3abd5fe204d288fb2ce08eedcf317\"></div>\n",
                             "<script type=\"text/javascript\">\n",
                             "  var VEGA_DEBUG = (typeof VEGA_DEBUG == \"undefined\") ? {} : VEGA_DEBUG;\n",
                             "  (function(spec, embedOpt){\n",
                             "    let outputDiv = document.currentScript.previousElementSibling;\n",
-                            "    if (outputDiv.id !== \"altair-viz-8333cb2b19d2476e8e1e59d8634646d4\") {\n",
-                            "      outputDiv = document.getElementById(\"altair-viz-8333cb2b19d2476e8e1e59d8634646d4\");\n",
+                            "    if (outputDiv.id !== \"altair-viz-b4a3abd5fe204d288fb2ce08eedcf317\") {\n",
+                            "      outputDiv = document.getElementById(\"altair-viz-b4a3abd5fe204d288fb2ce08eedcf317\");\n",
                             "    }\n",
                             "    const paths = {\n",
                             "      \"vega\": \"https://cdn.jsdelivr.net/npm//vega@5?noext\",\n",
                             "      \"vega-lib\": \"https://cdn.jsdelivr.net/npm//vega-lib?noext\",\n",
                             "      \"vega-lite\": \"https://cdn.jsdelivr.net/npm//vega-lite@4.17.0?noext\",\n",
                             "      \"vega-embed\": \"https://cdn.jsdelivr.net/npm//vega-embed@6?noext\",\n",
                             "    };\n",
@@ -91,35 +91,35 @@
                             "    } else {\n",
                             "      maybeLoadScript(\"vega\", \"5\")\n",
                             "        .then(() => maybeLoadScript(\"vega-lite\", \"4.17.0\"))\n",
                             "        .then(() => maybeLoadScript(\"vega-embed\", \"6\"))\n",
                             "        .catch(showError)\n",
                             "        .then(() => displayChart(vegaEmbed));\n",
                             "    }\n",
-                            "  })({\"config\": {\"view\": {\"continuousWidth\": 400, \"continuousHeight\": 300}}, \"data\": {\"name\": \"data-afd92ce098b244d7faf66ffdf6a0c43d\"}, \"mark\": \"bar\", \"encoding\": {\"x\": {\"bin\": true, \"field\": \"__day_diff__\", \"type\": \"quantitative\"}, \"y\": {\"aggregate\": \"count\", \"type\": \"quantitative\"}}, \"$schema\": \"https://vega.github.io/schema/vega-lite/v4.17.0.json\", \"datasets\": {\"data-afd92ce098b244d7faf66ffdf6a0c43d\": [{\"integers\": 1, \"floaties\": 0.06364715271755828, \"floaties2\": 0.0315311125602078, \"floaties_key\": 0, \"stringy_key\": \"BlhPz\", \"integer_bools\": true, \"stringer\": \"rabbit\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2020-01-01T00:00:00\", \"datie_dates2\": \"2020-01-02T00:00:00\", \"datie_dates_m_y\": \"2020-01\", \"datie_dates2_m_y\": \"2020-01\", \"__day_diff__\": -1, \"_counts_\": 1}, {\"integers\": 2, \"floaties\": 0.4538630302276755, \"floaties2\": 0.23938815518637113, \"floaties_key\": 1, \"stringy_key\": \"teXkv\", \"integer_bools\": false, \"stringer\": \"leopard\", \"stringer2\": \"leopard\", \"datie_dates\": \"2021-02-03T00:00:00\", \"datie_dates2\": \"2021-02-02T00:00:00\", \"datie_dates_m_y\": \"2021-02\", \"datie_dates2_m_y\": \"2021-02\", \"__day_diff__\": 1, \"_counts_\": 1}, {\"integers\": 3, \"floaties\": 0.3400872179052117, \"floaties2\": 0.14220203068389037, \"floaties_key\": 2, \"stringy_key\": \"QezXS\", \"integer_bools\": true, \"stringer\": \"leopard\", \"stringer2\": \"leopard\", \"datie_dates\": \"2021-04-03T00:00:00\", \"datie_dates2\": \"2021-04-05T00:00:00\", \"datie_dates_m_y\": \"2021-04\", \"datie_dates2_m_y\": \"2021-04\", \"__day_diff__\": -2, \"_counts_\": 1}, {\"integers\": 1, \"floaties\": 0.9749252373100369, \"floaties2\": 0.09470185833101763, \"floaties_key\": 3, \"stringy_key\": \"GsTPn\", \"integer_bools\": true, \"stringer\": \"leopard\", \"stringer2\": \"leopard\", \"datie_dates\": \"2020-01-01T00:00:00\", \"datie_dates2\": \"2020-01-02T00:00:00\", \"datie_dates_m_y\": \"2020-01\", \"datie_dates2_m_y\": \"2020-01\", \"__day_diff__\": -1, \"_counts_\": 1}, {\"integers\": 2, \"floaties\": 0.06506097058889238, \"floaties2\": 0.987181833460357, \"floaties_key\": 4, \"stringy_key\": \"NuyDB\", \"integer_bools\": true, \"stringer\": \"rabbit\", \"stringer2\": \"leopard\", \"datie_dates\": \"2021-02-03T00:00:00\", \"datie_dates2\": \"2021-02-02T00:00:00\", \"datie_dates_m_y\": \"2021-02\", \"datie_dates2_m_y\": \"2021-02\", \"__day_diff__\": 1, \"_counts_\": 1}, {\"integers\": 3, \"floaties\": 0.12144016250461942, \"floaties2\": 0.23969660890668598, \"floaties_key\": 5, \"stringy_key\": \"TCYtg\", \"integer_bools\": false, \"stringer\": \"rabbit\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2021-04-03T00:00:00\", \"datie_dates2\": \"2021-04-05T00:00:00\", \"datie_dates_m_y\": \"2021-04\", \"datie_dates2_m_y\": \"2021-04\", \"__day_diff__\": -2, \"_counts_\": 1}, {\"integers\": 1, \"floaties\": 0.7421891230865129, \"floaties2\": 0.42535315256884176, \"floaties_key\": 6, \"stringy_key\": \"eNtOl\", \"integer_bools\": true, \"stringer\": \"rabbit\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2020-01-01T00:00:00\", \"datie_dates2\": \"2020-01-02T00:00:00\", \"datie_dates_m_y\": \"2020-01\", \"datie_dates2_m_y\": \"2020-01\", \"__day_diff__\": -1, \"_counts_\": 1}, {\"integers\": 2, \"floaties\": 0.8430212651076163, \"floaties2\": 0.05182867645739353, \"floaties_key\": 7, \"stringy_key\": \"oYJTB\", \"integer_bools\": false, \"stringer\": \"leopard\", \"stringer2\": \"leopard\", \"datie_dates\": \"2021-02-03T00:00:00\", \"datie_dates2\": \"2021-02-02T00:00:00\", \"datie_dates_m_y\": \"2021-02\", \"datie_dates2_m_y\": \"2021-02\", \"__day_diff__\": 1, \"_counts_\": 1}, {\"integers\": 3, \"floaties\": 0.8981479611000056, \"floaties2\": 0.1430286885423342, \"floaties_key\": 8, \"stringy_key\": \"iDTyF\", \"integer_bools\": true, \"stringer\": \"leopard\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2021-04-03T00:00:00\", \"datie_dates2\": \"2021-04-05T00:00:00\", \"datie_dates_m_y\": \"2021-04\", \"datie_dates2_m_y\": \"2021-04\", \"__day_diff__\": -2, \"_counts_\": 1}]}}, {\"mode\": \"vega-lite\"});\n",
+                            "  })({\"config\": {\"view\": {\"continuousWidth\": 400, \"continuousHeight\": 300}}, \"data\": {\"name\": \"data-c1feb92598f46f3dd3f69219a5e2bb6f\"}, \"mark\": \"bar\", \"encoding\": {\"x\": {\"bin\": true, \"field\": \"__day_diff__\", \"type\": \"quantitative\"}, \"y\": {\"aggregate\": \"count\", \"type\": \"quantitative\"}}, \"$schema\": \"https://vega.github.io/schema/vega-lite/v4.17.0.json\", \"datasets\": {\"data-c1feb92598f46f3dd3f69219a5e2bb6f\": [{\"integers\": 1, \"floaties\": 0.37662456287145674, \"floaties2\": 0.6302000514523506, \"floaties_key\": 0, \"stringy_key\": \"prlSG\", \"integer_bools\": false, \"stringer\": \"rabbit\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2020-01-01T00:00:00\", \"datie_dates2\": \"2020-01-02T00:00:00\", \"datie_dates_m_y\": \"2020-01\", \"datie_dates2_m_y\": \"2020-01\", \"__day_diff__\": -1, \"_counts_\": 1}, {\"integers\": 2, \"floaties\": 0.5196445124897988, \"floaties2\": 0.08155707270051471, \"floaties_key\": 1, \"stringy_key\": \"VsUlQ\", \"integer_bools\": false, \"stringer\": \"leopard\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2021-02-03T00:00:00\", \"datie_dates2\": \"2021-02-02T00:00:00\", \"datie_dates_m_y\": \"2021-02\", \"datie_dates2_m_y\": \"2021-02\", \"__day_diff__\": 1, \"_counts_\": 1}, {\"integers\": 3, \"floaties\": 0.5167396805010707, \"floaties2\": 0.693865627500929, \"floaties_key\": 2, \"stringy_key\": \"oWBLc\", \"integer_bools\": false, \"stringer\": \"leopard\", \"stringer2\": \"leopard\", \"datie_dates\": \"2021-04-03T00:00:00\", \"datie_dates2\": \"2021-04-05T00:00:00\", \"datie_dates_m_y\": \"2021-04\", \"datie_dates2_m_y\": \"2021-04\", \"__day_diff__\": -2, \"_counts_\": 1}, {\"integers\": 1, \"floaties\": 0.9881771108690396, \"floaties2\": 0.51166659207171, \"floaties_key\": 3, \"stringy_key\": \"jyEGY\", \"integer_bools\": true, \"stringer\": \"rabbit\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2020-01-01T00:00:00\", \"datie_dates2\": \"2020-01-02T00:00:00\", \"datie_dates_m_y\": \"2020-01\", \"datie_dates2_m_y\": \"2020-01\", \"__day_diff__\": -1, \"_counts_\": 1}, {\"integers\": 2, \"floaties\": 0.3927405581826563, \"floaties2\": 0.38598744659782036, \"floaties_key\": 4, \"stringy_key\": \"lCZRY\", \"integer_bools\": true, \"stringer\": \"rabbit\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2021-02-03T00:00:00\", \"datie_dates2\": \"2021-02-02T00:00:00\", \"datie_dates_m_y\": \"2021-02\", \"datie_dates2_m_y\": \"2021-02\", \"__day_diff__\": 1, \"_counts_\": 1}, {\"integers\": 3, \"floaties\": 0.6009257869945802, \"floaties2\": 0.8012496959685177, \"floaties_key\": 5, \"stringy_key\": \"fZsmG\", \"integer_bools\": true, \"stringer\": \"rabbit\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2021-04-03T00:00:00\", \"datie_dates2\": \"2021-04-05T00:00:00\", \"datie_dates_m_y\": \"2021-04\", \"datie_dates2_m_y\": \"2021-04\", \"__day_diff__\": -2, \"_counts_\": 1}, {\"integers\": 1, \"floaties\": 0.503556363529904, \"floaties2\": 0.86666302768916, \"floaties_key\": 6, \"stringy_key\": \"VgGiH\", \"integer_bools\": false, \"stringer\": \"rabbit\", \"stringer2\": \"rabbit\", \"datie_dates\": \"2020-01-01T00:00:00\", \"datie_dates2\": \"2020-01-02T00:00:00\", \"datie_dates_m_y\": \"2020-01\", \"datie_dates2_m_y\": \"2020-01\", \"__day_diff__\": -1, \"_counts_\": 1}, {\"integers\": 2, \"floaties\": 0.609907404739495, \"floaties2\": 0.738519742291172, \"floaties_key\": 7, \"stringy_key\": \"hceCy\", \"integer_bools\": true, \"stringer\": \"leopard\", \"stringer2\": \"leopard\", \"datie_dates\": \"2021-02-03T00:00:00\", \"datie_dates2\": \"2021-02-02T00:00:00\", \"datie_dates_m_y\": \"2021-02\", \"datie_dates2_m_y\": \"2021-02\", \"__day_diff__\": 1, \"_counts_\": 1}, {\"integers\": 3, \"floaties\": 0.5572262941742752, \"floaties2\": 0.08046368682174398, \"floaties_key\": 8, \"stringy_key\": \"HTQCx\", \"integer_bools\": true, \"stringer\": \"rabbit\", \"stringer2\": \"leopard\", \"datie_dates\": \"2021-04-03T00:00:00\", \"datie_dates2\": \"2021-04-05T00:00:00\", \"datie_dates_m_y\": \"2021-04\", \"datie_dates2_m_y\": \"2021-04\", \"__day_diff__\": -2, \"_counts_\": 1}]}}, {\"mode\": \"vega-lite\"});\n",
                             "</script>"
                         ],
                         "text/plain": [
                             "alt.Chart(...)"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
-                            "<div id=\"altair-viz-9c973ffb9d214d1e9dea521474f4211d\"></div>\n",
+                            "<div id=\"altair-viz-a80de2e2035c43568c0b5dbd5c679726\"></div>\n",
                             "<script type=\"text/javascript\">\n",
                             "  var VEGA_DEBUG = (typeof VEGA_DEBUG == \"undefined\") ? {} : VEGA_DEBUG;\n",
                             "  (function(spec, embedOpt){\n",
                             "    let outputDiv = document.currentScript.previousElementSibling;\n",
-                            "    if (outputDiv.id !== \"altair-viz-9c973ffb9d214d1e9dea521474f4211d\") {\n",
-                            "      outputDiv = document.getElementById(\"altair-viz-9c973ffb9d214d1e9dea521474f4211d\");\n",
+                            "    if (outputDiv.id !== \"altair-viz-a80de2e2035c43568c0b5dbd5c679726\") {\n",
+                            "      outputDiv = document.getElementById(\"altair-viz-a80de2e2035c43568c0b5dbd5c679726\");\n",
                             "    }\n",
                             "    const paths = {\n",
                             "      \"vega\": \"https://cdn.jsdelivr.net/npm//vega@5?noext\",\n",
                             "      \"vega-lib\": \"https://cdn.jsdelivr.net/npm//vega-lib?noext\",\n",
                             "      \"vega-lite\": \"https://cdn.jsdelivr.net/npm//vega-lite@4.17.0?noext\",\n",
                             "      \"vega-embed\": \"https://cdn.jsdelivr.net/npm//vega-embed@6?noext\",\n",
                             "    };\n",
@@ -169,15 +169,15 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "ce.chart_me(df, \"datie_dates\", \"datie_dates2\")\n"
+                "ce.chart_me(df, \"datie_dates\", \"datie_dates2\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "3a144419",
             "metadata": {},
@@ -1432,31 +1432,28 @@
             ],
             "source": [
                 "df.groupby(['Key', 'A']).agg({'Key' : ['count']}).reset_index()"
             ]
         }
     ],
     "metadata": {
-        "interpreter": {
-            "hash": "0e079e32dd2d4c656647c105cf14eaef36c8c60cb9bf2bcd011be3a8f4a35a63"
-        },
         "kernelspec": {
-            "display_name": "Python 3.9.13 ('venv': venv)",
+            "display_name": "env_chart_me",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.12.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `chart_me-0.1.5/interrogate_badge.svg` & `chart_me-0.2.0/interrogate_badge.svg`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/make.bat` & `chart_me-0.2.0/make.bat`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/pyproject.toml` & `chart_me-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 
 [project]
 name = "chart_me"
 authors = [{name = "Luke Garzia", email = "garzia.luke@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version"]
-dependencies = ['pandas', 'altair', 'typing-extensions']
+dependencies = ['pandas', 'altair', 'typing-extensions', 'typer']
 readme = "README.md"
 description = "Charting that keeps you in the EDA flow"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 test = ["pytest", "vega_datasets", "notebook",
  "pre-commit", "interrogate", "pytest-cov", "tox",
  "mypy", "black", "flake8", "isort", "bump2version", "flake8-comprehensions", "types-python-dateutil"]
 doc = ["sphinx", "myst-nb", "sphinx-rtd-theme", "sphinx-autoapi"]
 
+[project.scripts]
+chart_me = "chart_me.__main__:main"
 
 [project.urls]
 Home = "https://github.com/lgarzia/chart_me"
 
 [tool.isort]
 multi_line_output = 3
 profile = "black"
```

### Comparing `chart_me-0.1.5/src/chart_me/chart_configs.py` & `chart_me-0.2.0/src/chart_me/chart_configs.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/src/chart_me/chart_me_logic.py` & `chart_me-0.2.0/src/chart_me/chart_me_logic.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/src/chart_me/charting_assembly_strategy/__init__.py` & `chart_me-0.2.0/src/chart_me/charting_assembly_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/src/chart_me/charting_assembly_strategy/bivariate.py` & `chart_me-0.2.0/src/chart_me/charting_assembly_strategy/bivariate.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/src/chart_me/charting_assembly_strategy/univariate.py` & `chart_me-0.2.0/src/chart_me/charting_assembly_strategy/univariate.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/src/chart_me/data_validation_strategy.py` & `chart_me-0.2.0/src/chart_me/data_validation_strategy.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/src/chart_me/datatype_infer_strategy.py` & `chart_me-0.2.0/src/chart_me/datatype_infer_strategy.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/src/chart_me/errors.py` & `chart_me-0.2.0/src/chart_me/errors.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/src/chart_me/pandas_util.py` & `chart_me-0.2.0/src/chart_me/pandas_util.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/tests/conftest.py` & `chart_me-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/tests/test_datatype_infer_strategy.py` & `chart_me-0.2.0/tests/test_datatype_infer_strategy.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/tests/test_validate_strategy.py` & `chart_me-0.2.0/tests/test_validate_strategy.py`

 * *Files identical despite different names*

### Comparing `chart_me-0.1.5/tox.ini` & `chart_me-0.2.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 00000000: 5b74 6f78 5d0d 0a69 736f 6c61 7465 645f  [tox]..isolated_
 00000010: 6275 696c 6420 3d20 5472 7565 0d0a 656e  build = True..en
-00000020: 766c 6973 7420 3d20 7079 3337 2c20 7079  vlist = py37, py
-00000030: 3338 2c20 7079 3339 2c20 7079 3331 302c  38, py39, py310,
-00000040: 2062 6c61 636b 2c20 666c 616b 6538 2c20   black, flake8, 
-00000050: 6973 6f72 740d 0a73 6b69 705f 6d69 7373  isort..skip_miss
-00000060: 696e 675f 696e 7465 7270 7265 7465 7273  ing_interpreters
-00000070: 203d 2054 7275 650d 0a0d 0a5b 7465 7374   = True....[test
-00000080: 656e 765d 0d0a 6465 7073 203d 0d0a 2020  env]..deps =..  
-00000090: 2020 7079 7465 7374 0d0a 2020 2020 7079    pytest..    py
-000000a0: 7465 7374 2d63 6f76 0d0a 2020 2020 7061  test-cov..    pa
-000000b0: 6e64 6173 0d0a 636f 6d6d 616e 6473 203d  ndas..commands =
-000000c0: 0d0a 2020 2020 7079 7468 6f6e 202d 6d20  ..    python -m 
-000000d0: 7079 7465 7374 202d 2d63 6f76 3d63 6861  pytest --cov=cha
-000000e0: 7274 5f6d 6520 2d2d 636f 762d 6661 696c  rt_me --cov-fail
-000000f0: 2d75 6e64 6572 3d35 3020 2d2d 636f 762d  -under=50 --cov-
-00000100: 7265 706f 7274 3d74 6572 6d2d 6d69 7373  report=term-miss
-00000110: 696e 670d 0a0d 0a5b 7465 7374 656e 763a  ing....[testenv:
-00000120: 626c 6163 6b5d 0d0a 6465 7073 203d 2062  black]..deps = b
-00000130: 6c61 636b 0d0a 636f 6d6d 616e 6473 203d  lack..commands =
-00000140: 2070 7974 686f 6e20 2d6d 2062 6c61 636b   python -m black
-00000150: 202d 2d63 6865 636b 202e 0d0a 0d0a 5b74   --check .....[t
-00000160: 6573 7465 6e76 3a66 6c61 6b65 385d 0d0a  estenv:flake8]..
-00000170: 6465 7073 203d 2066 6c61 6b65 380d 0a63  deps = flake8..c
-00000180: 6f6d 6d61 6e64 7320 3d20 7079 7468 6f6e  ommands = python
-00000190: 202d 6d20 666c 616b 6538 2073 7263 0d0a   -m flake8 src..
-000001a0: 0d0a 5b74 6573 7465 6e76 3a69 736f 7274  ..[testenv:isort
-000001b0: 5d0d 0a64 6570 7320 3d20 6973 6f72 740d  ]..deps = isort.
-000001c0: 0a63 6f6d 6d61 6e64 7320 3d20 7079 7468  .commands = pyth
-000001d0: 6f6e 202d 6d20 6973 6f72 7420 2d2d 6368  on -m isort --ch
-000001e0: 6563 6b20 7372 630d 0a0d 0a23 5b74 6573  eck src....#[tes
-000001f0: 7465 6e76 3a6d 7970 795d 0d0a 2364 6570  tenv:mypy]..#dep
-00000200: 7320 3d20 6d79 7079 0d0a 2363 6f6d 6d61  s = mypy..#comma
-00000210: 6e64 7320 3d20 7079 7468 6f6e 202d 6d20  nds = python -m 
-00000220: 6d79 7079 2073 7263 0a                   mypy src.
+00000020: 766c 6973 7420 3d20 7079 3331 302c 2070  vlist = py310, p
+00000030: 7933 3131 2c20 7079 3331 322c 2062 6c61  y311, py312, bla
+00000040: 636b 2c20 666c 616b 6538 2c20 6973 6f72  ck, flake8, isor
+00000050: 740d 0a73 6b69 705f 6d69 7373 696e 675f  t..skip_missing_
+00000060: 696e 7465 7270 7265 7465 7273 203d 2054  interpreters = T
+00000070: 7275 650d 0a0d 0a5b 7465 7374 656e 765d  rue....[testenv]
+00000080: 0d0a 6465 7073 203d 0d0a 2020 2020 7079  ..deps =..    py
+00000090: 7465 7374 0d0a 2020 2020 7079 7465 7374  test..    pytest
+000000a0: 2d63 6f76 0d0a 2020 2020 7061 6e64 6173  -cov..    pandas
+000000b0: 0d0a 636f 6d6d 616e 6473 203d 0d0a 2020  ..commands =..  
+000000c0: 2020 7079 7468 6f6e 202d 6d20 7079 7465    python -m pyte
+000000d0: 7374 202d 2d63 6f76 3d63 6861 7274 5f6d  st --cov=chart_m
+000000e0: 6520 2d2d 636f 762d 6661 696c 2d75 6e64  e --cov-fail-und
+000000f0: 6572 3d35 3020 2d2d 636f 762d 7265 706f  er=50 --cov-repo
+00000100: 7274 3d74 6572 6d2d 6d69 7373 696e 670d  rt=term-missing.
+00000110: 0a0d 0a5b 7465 7374 656e 763a 626c 6163  ...[testenv:blac
+00000120: 6b5d 0d0a 6465 7073 203d 2062 6c61 636b  k]..deps = black
+00000130: 0d0a 636f 6d6d 616e 6473 203d 2070 7974  ..commands = pyt
+00000140: 686f 6e20 2d6d 2062 6c61 636b 202d 2d63  hon -m black --c
+00000150: 6865 636b 202e 0d0a 0d0a 5b74 6573 7465  heck .....[teste
+00000160: 6e76 3a66 6c61 6b65 385d 0d0a 6465 7073  nv:flake8]..deps
+00000170: 203d 2066 6c61 6b65 380d 0a63 6f6d 6d61   = flake8..comma
+00000180: 6e64 7320 3d20 7079 7468 6f6e 202d 6d20  nds = python -m 
+00000190: 666c 616b 6538 2073 7263 0d0a 0d0a 5b74  flake8 src....[t
+000001a0: 6573 7465 6e76 3a69 736f 7274 5d0d 0a64  estenv:isort]..d
+000001b0: 6570 7320 3d20 6973 6f72 740d 0a63 6f6d  eps = isort..com
+000001c0: 6d61 6e64 7320 3d20 7079 7468 6f6e 202d  mands = python -
+000001d0: 6d20 6973 6f72 7420 2d2d 6368 6563 6b20  m isort --check 
+000001e0: 7372 630d 0a0d 0a23 5b74 6573 7465 6e76  src....#[testenv
+000001f0: 3a6d 7970 795d 0d0a 2364 6570 7320 3d20  :mypy]..#deps = 
+00000200: 6d79 7079 0d0a 2363 6f6d 6d61 6e64 7320  mypy..#commands 
+00000210: 3d20 7079 7468 6f6e 202d 6d20 6d79 7079  = python -m mypy
+00000220: 2073 7263 0d0a                            src..
```

### Comparing `chart_me-0.1.5/PKG-INFO` & `chart_me-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: chart_me
-Version: 0.1.5
+Version: 0.2.0
 Summary: Charting that keeps you in the EDA flow
 Author-email: Luke Garzia <garzia.luke@gmail.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pandas
 Requires-Dist: altair
 Requires-Dist: typing-extensions
+Requires-Dist: typer
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: myst-nb ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme ; extra == "doc"
 Requires-Dist: sphinx-autoapi ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: vega_datasets ; extra == "test"
 Requires-Dist: notebook ; extra == "test"
```

