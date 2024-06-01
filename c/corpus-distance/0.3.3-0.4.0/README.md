# Comparing `tmp/corpus_distance-0.3.3.tar.gz` & `tmp/corpus_distance-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_distance-0.3.3.tar", last modified: Sat Jun  1 00:05:05 2024, max compression
+gzip compressed data, was "corpus_distance-0.4.0.tar", last modified: Sat Jun  1 13:49:01 2024, max compression
```

## Comparing `corpus_distance-0.3.3.tar` & `corpus_distance-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:05.234455 corpus_distance-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-06-01 00:05:05.234455 corpus_distance-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:05:05.234455 corpus_distance-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:05.230455 corpus_distance-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:05.230455 corpus_distance-0.3.3/src/corpus_distance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/cdutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:05.234455 corpus_distance-0.3.3/src/corpus_distance/clusterisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/clusterisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/clusterisation/clusterisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/clusterisation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:05.234455 corpus_distance-0.3.3/src/corpus_distance/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data/data_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)   267685 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data/gospels.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:05.234455 corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/data_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/frequency_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/shingle_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/topic_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/vectorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:05.234455 corpus_distance-0.3.3/src/corpus_distance/distance_measurement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/distance_measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/distance_measurement/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/distance_measurement/frequency_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/distance_measurement/hybridisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/distance_measurement/metrics_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/distance_measurement/string_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-06-01 00:05:01.000000 corpus_distance-0.3.3/src/corpus_distance/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:05:05.234455 corpus_distance-0.3.3/src/corpus_distance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-06-01 00:05:05.000000 corpus_distance-0.3.3/src/corpus_distance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-06-01 00:05:05.000000 corpus_distance-0.3.3/src/corpus_distance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:05:05.000000 corpus_distance-0.3.3/src/corpus_distance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-01 00:05:05.000000 corpus_distance-0.3.3/src/corpus_distance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 00:05:05.000000 corpus_distance-0.3.3/src/corpus_distance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.854416 corpus_distance-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-06-01 13:49:01.854416 corpus_distance-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:49:01.854416 corpus_distance-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.850416 corpus_distance-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.850416 corpus_distance-0.4.0/src/corpus_distance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/cdutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.850416 corpus_distance-0.4.0/src/corpus_distance/clusterisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/clusterisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/clusterisation/clusterisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/clusterisation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.850416 corpus_distance-0.4.0/src/corpus_distance/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data/data_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267685 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data/gospels.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.854416 corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/frequency_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/shingle_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/topic_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/vectorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.854416 corpus_distance-0.4.0/src/corpus_distance/distance_measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/distance_measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/distance_measurement/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/distance_measurement/frequency_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/distance_measurement/hybridisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/distance_measurement/metrics_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/distance_measurement/string_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/src/corpus_distance/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.854416 corpus_distance-0.4.0/src/corpus_distance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-06-01 13:49:01.000000 corpus_distance-0.4.0/src/corpus_distance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-06-01 13:49:01.000000 corpus_distance-0.4.0/src/corpus_distance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:49:01.000000 corpus_distance-0.4.0/src/corpus_distance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-01 13:49:01.000000 corpus_distance-0.4.0/src/corpus_distance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 13:49:01.000000 corpus_distance-0.4.0/src/corpus_distance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:01.854416 corpus_distance-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-01 13:48:56.000000 corpus_distance-0.4.0/tests/test_placeholder.py
```

### Comparing `corpus_distance-0.3.3/LICENSE` & `corpus_distance-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/PKG-INFO` & `corpus_distance-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corpus_distance
-Version: 0.3.3
+Version: 0.4.0
 Summary: Python package for measuring distance between the lects represented by small raw corpora
 Author-email: Ilia Afanasev <szrnamerg@gmail.com>
 Project-URL: Homepage, https://github.com/The-One-Who-Speaks-and-Depicts/corpus_distance
 Project-URL: Issues, https://github.com/The-One-Who-Speaks-and-Depicts/corpus_distance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -20,44 +20,70 @@
 Requires-Dist: pandas==2.1.1
 Requires-Dist: pyjarowinkler==1.8
 Requires-Dist: scipy==1.11.4
 Requires-Dist: tqdm==4.66.4
 Requires-Dist: packaging==21.3
 
 # Python package for measuring distance between the lects represented by small raw corpora
-![pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11395683.svg)](https://doi.org/10.5281/zenodo.11395683)
 
+![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
+![pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)
+
 # What is it?
 
 corpus_distance is a Python package that allows to measure distance between the lects that are presented only by small (down to extremely small, <1000 tokens) raw (without any kind of morhological tagging, lemmatisation, or dependency parsing) corpora, and classify them. It joins frequency-based metrics and string similarity measurements into a hybrid distance scorer.
 
 corpus_distance operates with 3-shingles, a sequences of 3 symbols, by which words are split. This helps to spot more intricate patterns and correspondences within raw data, as well as to enhance the dataset size.
 
 ## NB!
 
-The classification is going to be only (and extemely) preliminary, as it is by default language-agnostic and does not use preliminary expert judgements or linguistic information. Basically, the more effort is put into the actual data, the more reliable are final results. 
+The classification is going to be only (and extremely) preliminary, as it is by default language-agnostic and does not use preliminary expert judgements or linguistic information. Basically, the more effort is put into the actual data, the more reliable are final results. 
 
-In addition, the results may not be used as a proof of language relationship (external classification), only as a supporting evidence for tree topology (internal classification), as it is with any kind of phylogenetic methods in historical comparative studies.
+In addition, the results may not be used as a proof of language relationship (external classification), only as a supporting evidence for a tree topology (internal classification), as it is with any kind of phylogenetic methods in historical comparative studies.
 
-One more important notion is that one should be very careful with using this package for a distantly related lects. As it is with any kind of language-agnostic methods, they lose precision with the increase of distance between analysed groups. 
+One more important notion is that one should be very careful with using this package for a distantly related lects. As it is with any kind of language-agnostic methods, it loses precision with the increase of distance between analysed groups (Holman et al., 2008). 
 
 # How to install
 
 ## From TestPyPI (development version; requires manual installation of dependencies; may contain bugs)
 
 ```
 pip install biopython
 pip install Levenshtein
 pip install gensim
 pip install pyjarowinkler
 
 python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps --force-reinstall corpus_distance
 ```
 
+## From PyPI (release version)
+
+```
+pip install corpus_distance
+```
+
+## From Docker
+
+1. Clone repository.
+```
+git clone https://github.com/The-One-Who-Speaks-and-Depicts/corpus_distance.git
+```
+2. Cd to the repository root directory.
+3. (optionally) Add your data and configuration file (see How to use/Preparation below), put both into the repository directory.
+4. Create Docker image.
+```
+sudo docker build --tag IMAGE_NAME .
+```
+IMAGE_NAME is a name of the docker image of your choice
+5. Run Docker image.
+```
+sudo docker run -i -t IMAGE_NAME /bin/bash
+```
+
 # How to use
 
 ## Preparation
 
 1. Create a virtual environment with `python3 -m venv ENV`, where `ENV` is a name of your virtual environment.
 2. Install package, following the instructions above.
 3. Create a folder for your data.
@@ -119,31 +145,33 @@
             "outgroup": "Slovak",
             "metrics": "default_metrics_name",
             "classification_method": "upgma",
             "store_path": "default"
         }
     }
 ```
+7. In case you are using Docker, do not forget to put your data and configuration file into the repository directory before creating Docker image. 
+
 ## Running the code
 
 There are two ways of running the code: with prepared Jupyter Notebook, or independently.
 
 ### Ready-made Jupyter Notebook
 
 In the folder `example`, there is a tutorial notebook that outlines the inner workings of the package.
 
-### Using your own file
+### Using your own file (or from Docker console)
 
 After data and configuration are ready, open Python interpreter:
 
 ```
 python
 ```
 
 Run the following commands:
 
 ```
 from corpus_distance.pipeline import perform_clusterisation
 perform_clusterisation(PATH_TO_CONFIG)
 ```
 
-PATH_TO_CONFIG here is a path to `config.json`.
+`PATH_TO_CONFIG` here is a path to `config.json`. This parameter may be empty, then the model performs clusterisation with default dataset (Modern Standard Slavic Gospels of John: Croatian, Slovak, Slovenian) and default parameters.
```

### Comparing `corpus_distance-0.3.3/README.md` & `corpus_distance-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,64 @@
 # Python package for measuring distance between the lects represented by small raw corpora
-![pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11395683.svg)](https://doi.org/10.5281/zenodo.11395683)
 
+![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
+![pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)
+
 # What is it?
 
 corpus_distance is a Python package that allows to measure distance between the lects that are presented only by small (down to extremely small, <1000 tokens) raw (without any kind of morhological tagging, lemmatisation, or dependency parsing) corpora, and classify them. It joins frequency-based metrics and string similarity measurements into a hybrid distance scorer.
 
 corpus_distance operates with 3-shingles, a sequences of 3 symbols, by which words are split. This helps to spot more intricate patterns and correspondences within raw data, as well as to enhance the dataset size.
 
 ## NB!
 
-The classification is going to be only (and extemely) preliminary, as it is by default language-agnostic and does not use preliminary expert judgements or linguistic information. Basically, the more effort is put into the actual data, the more reliable are final results. 
+The classification is going to be only (and extremely) preliminary, as it is by default language-agnostic and does not use preliminary expert judgements or linguistic information. Basically, the more effort is put into the actual data, the more reliable are final results. 
 
-In addition, the results may not be used as a proof of language relationship (external classification), only as a supporting evidence for tree topology (internal classification), as it is with any kind of phylogenetic methods in historical comparative studies.
+In addition, the results may not be used as a proof of language relationship (external classification), only as a supporting evidence for a tree topology (internal classification), as it is with any kind of phylogenetic methods in historical comparative studies.
 
-One more important notion is that one should be very careful with using this package for a distantly related lects. As it is with any kind of language-agnostic methods, they lose precision with the increase of distance between analysed groups. 
+One more important notion is that one should be very careful with using this package for a distantly related lects. As it is with any kind of language-agnostic methods, it loses precision with the increase of distance between analysed groups (Holman et al., 2008). 
 
 # How to install
 
 ## From TestPyPI (development version; requires manual installation of dependencies; may contain bugs)
 
 ```
 pip install biopython
 pip install Levenshtein
 pip install gensim
 pip install pyjarowinkler
 
 python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps --force-reinstall corpus_distance
 ```
 
+## From PyPI (release version)
+
+```
+pip install corpus_distance
+```
+
+## From Docker
+
+1. Clone repository.
+```
+git clone https://github.com/The-One-Who-Speaks-and-Depicts/corpus_distance.git
+```
+2. Cd to the repository root directory.
+3. (optionally) Add your data and configuration file (see How to use/Preparation below), put both into the repository directory.
+4. Create Docker image.
+```
+sudo docker build --tag IMAGE_NAME .
+```
+IMAGE_NAME is a name of the docker image of your choice
+5. Run Docker image.
+```
+sudo docker run -i -t IMAGE_NAME /bin/bash
+```
+
 # How to use
 
 ## Preparation
 
 1. Create a virtual environment with `python3 -m venv ENV`, where `ENV` is a name of your virtual environment.
 2. Install package, following the instructions above.
 3. Create a folder for your data.
@@ -94,31 +120,33 @@
             "outgroup": "Slovak",
             "metrics": "default_metrics_name",
             "classification_method": "upgma",
             "store_path": "default"
         }
     }
 ```
+7. In case you are using Docker, do not forget to put your data and configuration file into the repository directory before creating Docker image. 
+
 ## Running the code
 
 There are two ways of running the code: with prepared Jupyter Notebook, or independently.
 
 ### Ready-made Jupyter Notebook
 
 In the folder `example`, there is a tutorial notebook that outlines the inner workings of the package.
 
-### Using your own file
+### Using your own file (or from Docker console)
 
 After data and configuration are ready, open Python interpreter:
 
 ```
 python
 ```
 
 Run the following commands:
 
 ```
 from corpus_distance.pipeline import perform_clusterisation
 perform_clusterisation(PATH_TO_CONFIG)
 ```
 
-PATH_TO_CONFIG here is a path to `config.json`.
+`PATH_TO_CONFIG` here is a path to `config.json`. This parameter may be empty, then the model performs clusterisation with default dataset (Modern Standard Slavic Gospels of John: Croatian, Slovak, Slovenian) and default parameters.
```

### Comparing `corpus_distance-0.3.3/pyproject.toml` & `corpus_distance-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.7.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "corpus_distance"
-version = "0.3.3"
+version = "0.4.0"
 authors = [
   { name="Ilia Afanasev", email="szrnamerg@gmail.com" },
 ]
 description = "Python package for measuring distance between the lects represented by small raw corpora"
 readme = "README.md"
 requires-python = ">=3.10.12"
 classifiers = [
```

### Comparing `corpus_distance-0.3.3/src/corpus_distance/cdutils.py` & `corpus_distance-0.4.0/src/corpus_distance/cdutils.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/clusterisation/clusterisation.py` & `corpus_distance-0.4.0/src/corpus_distance/clusterisation/clusterisation.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/clusterisation/utils.py` & `corpus_distance-0.4.0/src/corpus_distance/clusterisation/utils.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/data/config.json` & `corpus_distance-0.4.0/src/corpus_distance/data/config.json`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/data/gospels.csv` & `corpus_distance-0.4.0/src/corpus_distance/data/gospels.csv`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/data_loading.py` & `corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/data_loading.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/data_pipeline.py` & `corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/frequency_scoring.py` & `corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/frequency_scoring.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/shingle_processing.py` & `corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/shingle_processing.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/topic_modelling.py` & `corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/topic_modelling.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/data_preprocessing/vectorisation.py` & `corpus_distance-0.4.0/src/corpus_distance/data_preprocessing/vectorisation.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/distance_measurement/analysis.py` & `corpus_distance-0.4.0/src/corpus_distance/distance_measurement/analysis.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/distance_measurement/frequency_metrics.py` & `corpus_distance-0.4.0/src/corpus_distance/distance_measurement/frequency_metrics.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/distance_measurement/hybridisation.py` & `corpus_distance-0.4.0/src/corpus_distance/distance_measurement/hybridisation.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/distance_measurement/metrics_pipeline.py` & `corpus_distance-0.4.0/src/corpus_distance/distance_measurement/metrics_pipeline.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/distance_measurement/string_similarity.py` & `corpus_distance-0.4.0/src/corpus_distance/distance_measurement/string_similarity.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance/pipeline.py` & `corpus_distance-0.4.0/src/corpus_distance/pipeline.py`

 * *Files identical despite different names*

### Comparing `corpus_distance-0.3.3/src/corpus_distance.egg-info/PKG-INFO` & `corpus_distance-0.4.0/src/corpus_distance.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corpus_distance
-Version: 0.3.3
+Version: 0.4.0
 Summary: Python package for measuring distance between the lects represented by small raw corpora
 Author-email: Ilia Afanasev <szrnamerg@gmail.com>
 Project-URL: Homepage, https://github.com/The-One-Who-Speaks-and-Depicts/corpus_distance
 Project-URL: Issues, https://github.com/The-One-Who-Speaks-and-Depicts/corpus_distance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -20,44 +20,70 @@
 Requires-Dist: pandas==2.1.1
 Requires-Dist: pyjarowinkler==1.8
 Requires-Dist: scipy==1.11.4
 Requires-Dist: tqdm==4.66.4
 Requires-Dist: packaging==21.3
 
 # Python package for measuring distance between the lects represented by small raw corpora
-![pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11395683.svg)](https://doi.org/10.5281/zenodo.11395683)
 
+![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
+![pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)
+
 # What is it?
 
 corpus_distance is a Python package that allows to measure distance between the lects that are presented only by small (down to extremely small, <1000 tokens) raw (without any kind of morhological tagging, lemmatisation, or dependency parsing) corpora, and classify them. It joins frequency-based metrics and string similarity measurements into a hybrid distance scorer.
 
 corpus_distance operates with 3-shingles, a sequences of 3 symbols, by which words are split. This helps to spot more intricate patterns and correspondences within raw data, as well as to enhance the dataset size.
 
 ## NB!
 
-The classification is going to be only (and extemely) preliminary, as it is by default language-agnostic and does not use preliminary expert judgements or linguistic information. Basically, the more effort is put into the actual data, the more reliable are final results. 
+The classification is going to be only (and extremely) preliminary, as it is by default language-agnostic and does not use preliminary expert judgements or linguistic information. Basically, the more effort is put into the actual data, the more reliable are final results. 
 
-In addition, the results may not be used as a proof of language relationship (external classification), only as a supporting evidence for tree topology (internal classification), as it is with any kind of phylogenetic methods in historical comparative studies.
+In addition, the results may not be used as a proof of language relationship (external classification), only as a supporting evidence for a tree topology (internal classification), as it is with any kind of phylogenetic methods in historical comparative studies.
 
-One more important notion is that one should be very careful with using this package for a distantly related lects. As it is with any kind of language-agnostic methods, they lose precision with the increase of distance between analysed groups. 
+One more important notion is that one should be very careful with using this package for a distantly related lects. As it is with any kind of language-agnostic methods, it loses precision with the increase of distance between analysed groups (Holman et al., 2008). 
 
 # How to install
 
 ## From TestPyPI (development version; requires manual installation of dependencies; may contain bugs)
 
 ```
 pip install biopython
 pip install Levenshtein
 pip install gensim
 pip install pyjarowinkler
 
 python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps --force-reinstall corpus_distance
 ```
 
+## From PyPI (release version)
+
+```
+pip install corpus_distance
+```
+
+## From Docker
+
+1. Clone repository.
+```
+git clone https://github.com/The-One-Who-Speaks-and-Depicts/corpus_distance.git
+```
+2. Cd to the repository root directory.
+3. (optionally) Add your data and configuration file (see How to use/Preparation below), put both into the repository directory.
+4. Create Docker image.
+```
+sudo docker build --tag IMAGE_NAME .
+```
+IMAGE_NAME is a name of the docker image of your choice
+5. Run Docker image.
+```
+sudo docker run -i -t IMAGE_NAME /bin/bash
+```
+
 # How to use
 
 ## Preparation
 
 1. Create a virtual environment with `python3 -m venv ENV`, where `ENV` is a name of your virtual environment.
 2. Install package, following the instructions above.
 3. Create a folder for your data.
@@ -119,31 +145,33 @@
             "outgroup": "Slovak",
             "metrics": "default_metrics_name",
             "classification_method": "upgma",
             "store_path": "default"
         }
     }
 ```
+7. In case you are using Docker, do not forget to put your data and configuration file into the repository directory before creating Docker image. 
+
 ## Running the code
 
 There are two ways of running the code: with prepared Jupyter Notebook, or independently.
 
 ### Ready-made Jupyter Notebook
 
 In the folder `example`, there is a tutorial notebook that outlines the inner workings of the package.
 
-### Using your own file
+### Using your own file (or from Docker console)
 
 After data and configuration are ready, open Python interpreter:
 
 ```
 python
 ```
 
 Run the following commands:
 
 ```
 from corpus_distance.pipeline import perform_clusterisation
 perform_clusterisation(PATH_TO_CONFIG)
 ```
 
-PATH_TO_CONFIG here is a path to `config.json`.
+`PATH_TO_CONFIG` here is a path to `config.json`. This parameter may be empty, then the model performs clusterisation with default dataset (Modern Standard Slavic Gospels of John: Croatian, Slovak, Slovenian) and default parameters.
```

### Comparing `corpus_distance-0.3.3/src/corpus_distance.egg-info/SOURCES.txt` & `corpus_distance-0.4.0/src/corpus_distance.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 src/corpus_distance/data_preprocessing/topic_modelling.py
 src/corpus_distance/data_preprocessing/vectorisation.py
 src/corpus_distance/distance_measurement/__init__.py
 src/corpus_distance/distance_measurement/analysis.py
 src/corpus_distance/distance_measurement/frequency_metrics.py
 src/corpus_distance/distance_measurement/hybridisation.py
 src/corpus_distance/distance_measurement/metrics_pipeline.py
-src/corpus_distance/distance_measurement/string_similarity.py
+src/corpus_distance/distance_measurement/string_similarity.py
+tests/test_placeholder.py
```

