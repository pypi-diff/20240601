# Comparing `tmp/airbyte-source-rki-covid-0.1.2.tar.gz` & `tmp/airbyte_source_rki_covid-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-rki-covid-0.1.2.tar", last modified: Wed Jan 31 16:38:41 2024, max compression
+gzip compressed data, was "airbyte_source_rki_covid-0.1.3.tar", max compression
```

## Comparing `airbyte-source-rki-covid-0.1.2.tar` & `airbyte_source_rki_covid-0.1.3.tar`

### file list

```diff
@@ -1,64 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:38:41.395913 airbyte-source-rki-covid-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     6108 2024-01-31 16:38:41.395913 airbyte-source-rki-covid-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6151 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:38:41.395913 airbyte-source-rki-covid-0.1.2/airbyte_source_rki_covid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6108 2024-01-31 16:38:41.000000 airbyte-source-rki-covid-0.1.2/airbyte_source_rki_covid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2432 2024-01-31 16:38:41.000000 airbyte-source-rki-covid-0.1.2/airbyte_source_rki_covid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 16:38:41.000000 airbyte-source-rki-covid-0.1.2/airbyte_source_rki_covid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-01-31 16:38:41.000000 airbyte-source-rki-covid-0.1.2/airbyte_source_rki_covid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-01-31 16:38:41.000000 airbyte-source-rki-covid-0.1.2/airbyte_source_rki_covid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-01-31 16:38:41.000000 airbyte-source-rki-covid-0.1.2/airbyte_source_rki_covid.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:38:41.387913 airbyte-source-rki-covid-0.1.2/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)    26710 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       31 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       33 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      424 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5977 2024-01-31 16:38:41.399913 airbyte-source-rki-covid-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      925 2024-01-31 16:38:39.000000 airbyte-source-rki-covid-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:38:41.387913 airbyte-source-rki-covid-0.1.2/source_rki_covid/
--rw-r--r--   0 root         (0) root         (0)      128 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/__init__.py
--rw-r--r--   0 root         (0) root         (0)      237 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:38:41.391913 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/
--rw-r--r--   0 root         (0) root         (0)      217 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/german_history_deaths.json
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/german_history_frozen_incidence.json
--rw-r--r--   0 root         (0) root         (0)     1342 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/german_history_hospitalization.json
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/german_history_incidence.json
--rw-r--r--   0 root         (0) root         (0)      223 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/german_history_recovered.json
--rw-r--r--   0 root         (0) root         (0)     2624 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany.json
--rw-r--r--   0 root         (0) root         (0)     8490 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany_age_groups.json
--rw-r--r--   0 root         (0) root         (0)      215 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany_history_cases.json
--rw-r--r--   0 root         (0) root         (0)     1863 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany_states.json
--rw-r--r--   0 root         (0) root         (0)     8582 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany_states_age_groups.json
--rw-r--r--   0 root         (0) root         (0)      375 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/states_history_cases.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/states_history_deaths.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/states_history_frozen_incidence.json
--rw-r--r--   0 root         (0) root         (0)     1490 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/states_history_hospitalization.json
--rw-r--r--   0 root         (0) root         (0)      390 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/states_history_incidence.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/states_history_recovered.json
--rw-r--r--   0 root         (0) root         (0)    24292 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/source.py
--rw-r--r--   0 root         (0) root         (0)      540 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/source_rki_covid/spec.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:38:41.395913 airbyte-source-rki-covid-0.1.2/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       64 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_cached_stream_state.py
--rw-r--r--   0 root         (0) root         (0)     1828 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_incremental_germanhistorycases.py
--rw-r--r--   0 root         (0) root         (0)     2283 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_incremental_germanhistorydeaths.py
--rw-r--r--   0 root         (0) root         (0)     2422 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_incremental_germanhistoryfrozenIncidence.py
--rw-r--r--   0 root         (0) root         (0)     2427 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_incremental_germanhistoryhospitalization.py
--rw-r--r--   0 root         (0) root         (0)     2331 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_incremental_germanhistoryincidence.py
--rw-r--r--   0 root         (0) root         (0)     2331 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_incremental_germanhistoryrecovered.py
--rw-r--r--   0 root         (0) root         (0)     1825 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_incremental_streams.py
--rw-r--r--   0 root         (0) root         (0)      564 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)      808 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stateshistorycases.py
--rw-r--r--   0 root         (0) root         (0)      814 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stateshistorydeaths.py
--rw-r--r--   0 root         (0) root         (0)      869 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stateshistoryfrozenincidence.py
--rw-r--r--   0 root         (0) root         (0)      868 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stateshistoryhospitalization.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stateshistoryincidence.py
--rw-r--r--   0 root         (0) root         (0)      832 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stateshistoryrecovered.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stream_agegroup.py
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stream_germany.py
--rw-r--r--   0 root         (0) root         (0)      483 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_stream_germany_states.py
--rw-r--r--   0 root         (0) root         (0)     2063 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_streams.py
--rw-r--r--   0 root         (0) root         (0)      512 2024-01-31 16:34:25.000000 airbyte-source-rki-covid-0.1.2/unit_tests/test_streams_states_agegroup.py
+-rw-r--r--   0        0        0     4550 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/README.md
+-rw-r--r--   0        0        0      761 2024-05-31 22:24:38.071380 airbyte_source_rki_covid-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/run.py
+-rw-r--r--   0        0        0     1650 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/TODO.md
+-rw-r--r--   0        0        0      217 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/german_history_deaths.json
+-rw-r--r--   0        0        0      230 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/german_history_frozen_incidence.json
+-rw-r--r--   0        0        0     1342 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/german_history_hospitalization.json
+-rw-r--r--   0        0        0      230 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/german_history_incidence.json
+-rw-r--r--   0        0        0      223 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/german_history_recovered.json
+-rw-r--r--   0        0        0     2624 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany.json
+-rw-r--r--   0        0        0     8490 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany_age_groups.json
+-rw-r--r--   0        0        0      215 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany_history_cases.json
+-rw-r--r--   0        0        0     1863 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany_states.json
+-rw-r--r--   0        0        0     8582 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany_states_age_groups.json
+-rw-r--r--   0        0        0      375 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/states_history_cases.json
+-rw-r--r--   0        0        0      377 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/states_history_deaths.json
+-rw-r--r--   0        0        0      464 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/states_history_frozen_incidence.json
+-rw-r--r--   0        0        0     1490 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/states_history_hospitalization.json
+-rw-r--r--   0        0        0      390 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/states_history_incidence.json
+-rw-r--r--   0        0        0      383 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/states_history_recovered.json
+-rw-r--r--   0        0        0    24292 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/source.py
+-rw-r--r--   0        0        0      540 2024-05-31 22:08:13.000000 airbyte_source_rki_covid-0.1.3/source_rki_covid/spec.json
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 airbyte_source_rki_covid-0.1.3/PKG-INFO
```

### Comparing `airbyte-source-rki-covid-0.1.2/PKG-INFO` & `airbyte_source_rki_covid-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-rki-covid
-Version: 0.1.2
+Version: 0.1.3
 Summary: Source implementation for Rki Covid.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/rki-covid
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-Requires-Dist: airbyte-cdk; extra == "tests"
 
-# RKI Covid Source
+# Rki-Covid source connector
 
-This is the repository for the RkI (Robert Koch-Institut - von Marlon Lückert) Covid-19 source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/rki-covid).
 
-```
-Germany:
-1. /germany
-2. /germany/age-groups
-3. /germany/history/cases/:days
-4. /germany/history/incidence/:days
-5. /germany/history/deaths/:days
-6. /germany/history/recovered/:days
-7. /germany/history/frozen-incidence/:days
-8. /germany/history/hospitalization/:days
-9. /germany/states
-10. /germany/states/age-groups
-11. /germany/states/history/cases/:days
-12. /germany/states/history/incidence/:days
-13. /germany/states/history/frozen-incidence/:days
-14. /germany/states/history/deaths/:days
-15. /germany/states/history/recovered/:days
-16. /germany/states/history/hospitalization/:days
-```
+This is the repository for the Rki-Covid source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/rki-covid).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/rki-covid)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_rki_covid/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/rki-covid)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_rki_covid/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source rki-covid test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-rki-covid spec
+poetry run source-rki-covid check --config secrets/config.json
+poetry run source-rki-covid discover --config secrets/config.json
+poetry run source-rki-covid read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-rki-covid build
 ```
 
-An image will be built with the tag `airbyte/source-rki-covid:dev`.
+An image will be available on your host with the tag `airbyte/source-rki-covid:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-rki-covid:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-rki-covid:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-rki-covid:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-rki-covid:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-rki-covid:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-rki-covid test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-rki-covid test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/rki-covid.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/rki-covid.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/german_history_hospitalization.json` & `airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/german_history_hospitalization.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany.json` & `airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany_age_groups.json` & `airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany_age_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany_states.json` & `airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany_states.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/germany_states_age_groups.json` & `airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/germany_states_age_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-rki-covid-0.1.2/source_rki_covid/schemas/states_history_hospitalization.json` & `airbyte_source_rki_covid-0.1.3/source_rki_covid/schemas/states_history_hospitalization.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-rki-covid-0.1.2/source_rki_covid/source.py` & `airbyte_source_rki_covid-0.1.3/source_rki_covid/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-rki-covid-0.1.2/source_rki_covid/spec.json` & `airbyte_source_rki_covid-0.1.3/source_rki_covid/spec.json`

 * *Files identical despite different names*

