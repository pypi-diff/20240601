# Comparing `tmp/HuggingMouse-0.0.2.tar.gz` & `tmp/HuggingMouse-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HuggingMouse-0.0.2.tar", last modified: Fri Mar 22 02:45:51 2024, max compression
+gzip compressed data, was "HuggingMouse-0.1.0.tar", last modified: Sat Jun  1 01:31:36 2024, max compression
```

## Comparing `HuggingMouse-0.0.2.tar` & `HuggingMouse-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,231 @@
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-03-22 02:45:51.302662 HuggingMouse-0.0.2/
--rw-rw-r--   0 maria     (1000) maria     (1000)    35149 2024-02-26 19:48:43.000000 HuggingMouse-0.0.2/LICENSE
--rw-rw-r--   0 maria     (1000) maria     (1000)      297 2024-03-22 02:45:51.302662 HuggingMouse-0.0.2/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)     3484 2024-03-22 02:43:53.000000 HuggingMouse-0.0.2/README.md
--rw-rw-r--   0 maria     (1000) maria     (1000)      106 2024-03-21 17:54:43.000000 HuggingMouse-0.0.2/pyproject.toml
--rw-rw-r--   0 maria     (1000) maria     (1000)       38 2024-03-22 02:45:51.302662 HuggingMouse-0.0.2/setup.cfg
--rw-rw-r--   0 maria     (1000) maria     (1000)      585 2024-03-22 02:45:19.000000 HuggingMouse-0.0.2/setup.py
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-03-22 02:45:51.298662 HuggingMouse-0.0.2/src/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-03-22 02:45:51.302662 HuggingMouse-0.0.2/src/HuggingMouse/
--rw-rw-r--   0 maria     (1000) maria     (1000)        0 2024-03-01 03:09:15.000000 HuggingMouse-0.0.2/src/HuggingMouse/__init__.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     4384 2024-03-21 15:06:01.000000 HuggingMouse-0.0.2/src/HuggingMouse/allen_api_utilities.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      888 2024-03-21 15:08:45.000000 HuggingMouse-0.0.2/src/HuggingMouse/custom_exceptions.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     3703 2024-03-22 02:36:00.000000 HuggingMouse-0.0.2/src/HuggingMouse/make_embeddings.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     6914 2024-03-21 15:22:07.000000 HuggingMouse-0.0.2/src/HuggingMouse/regressors.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     2663 2024-03-22 02:26:54.000000 HuggingMouse-0.0.2/src/HuggingMouse/trial_averaged_data.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     3090 2024-03-21 15:33:11.000000 HuggingMouse-0.0.2/src/HuggingMouse/utils.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     1860 2024-03-21 18:18:33.000000 HuggingMouse-0.0.2/src/HuggingMouse/visualizers.py
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-03-22 02:45:51.302662 HuggingMouse-0.0.2/src/HuggingMouse.egg-info/
--rw-r--r--   0 maria     (1000) maria     (1000)      297 2024-03-22 02:45:51.000000 HuggingMouse-0.0.2/src/HuggingMouse.egg-info/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)      512 2024-03-22 02:45:51.000000 HuggingMouse-0.0.2/src/HuggingMouse.egg-info/SOURCES.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)        1 2024-03-22 02:45:51.000000 HuggingMouse-0.0.2/src/HuggingMouse.egg-info/dependency_links.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)      100 2024-03-22 02:45:51.000000 HuggingMouse-0.0.2/src/HuggingMouse.egg-info/requires.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)       13 2024-03-22 02:45:51.000000 HuggingMouse-0.0.2/src/HuggingMouse.egg-info/top_level.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.640608 HuggingMouse-0.1.0/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3082 2024-03-21 16:02:48.000000 HuggingMouse-0.1.0/.gitignore
+-rw-rw-r--   0 maria     (1000) maria     (1000)      953 2024-03-01 02:48:49.000000 HuggingMouse-0.1.0/.readthedocs.yaml
+-rw-rw-r--   0 maria     (1000) maria     (1000)    35149 2024-02-26 19:48:43.000000 HuggingMouse-0.1.0/LICENSE
+-rw-r--r--   0 maria     (1000) maria     (1000)      471 2024-06-01 01:31:36.640608 HuggingMouse-0.1.0/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6009 2024-06-01 01:28:28.000000 HuggingMouse-0.1.0/README.md
+-rw-rw-r--   0 maria     (1000) maria     (1000)    61631 2024-03-22 17:18:08.000000 HuggingMouse-0.1.0/VarExp.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)  7344609 2024-03-20 03:35:03.000000 HuggingMouse-0.1.0/calcium_movie.gif
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.600608 HuggingMouse-0.1.0/docs/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      634 2024-03-01 01:50:39.000000 HuggingMouse-0.1.0/docs/Makefile
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.604608 HuggingMouse-0.1.0/docs/_build/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      230 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.buildinfo
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.604608 HuggingMouse-0.1.0/docs/_build/.doctrees/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.604608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.604608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.604608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    13248 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.604608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/custom_exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    12797 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/custom_exceptions/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3871 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.604608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    20957 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.604608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    13700 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/regressors/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    10234 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    17337 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/utils/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    10506 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/HuggingMouse/visualizers/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4109 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/autoapi/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)   321104 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/environment.pickle
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5033 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/.doctrees/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      794 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/custom_exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1018 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/custom_exceptions/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      341 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1198 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1104 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/regressors/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      538 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/trial_averaged_data/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      765 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/utils/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.608608 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      665 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/HuggingMouse/visualizers/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      249 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_sources/autoapi/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.1.0/docs/_build/_sources/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.612608 HuggingMouse-0.1.0/docs/_build/_static/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    11143 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_static/alabaster.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15096 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_static/basic.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)       42 2024-03-20 04:17:52.000000 HuggingMouse-0.1.0/docs/_build/_static/custom.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4472 2024-03-20 04:18:06.000000 HuggingMouse-0.1.0/docs/_build/_static/doctools.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)      328 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_static/documentation_options.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)      286 2024-03-20 04:18:06.000000 HuggingMouse-0.1.0/docs/_build/_static/file.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)      299 2024-03-20 04:18:06.000000 HuggingMouse-0.1.0/docs/_build/_static/graphviz.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4758 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_static/language_data.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-03-20 04:18:06.000000 HuggingMouse-0.1.0/docs/_build/_static/minus.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-03-20 04:18:06.000000 HuggingMouse-0.1.0/docs/_build/_static/plus.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5359 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/_static/pygments.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)    18732 2024-03-20 04:18:06.000000 HuggingMouse-0.1.0/docs/_build/_static/searchtools.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5123 2024-03-20 04:18:06.000000 HuggingMouse-0.1.0/docs/_build/_static/sphinx_highlight.js
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.612608 HuggingMouse-0.1.0/docs/_build/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.612608 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.612608 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     8255 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/allen_api_utilities/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.612608 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/custom_exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     9342 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/custom_exceptions/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5593 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.612608 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    11396 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/make_embeddings/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     8436 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/regressors/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6912 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/trial_averaged_data/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     9647 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/utils/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6719 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/HuggingMouse/visualizers/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6009 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/autoapi/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    11686 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/analyzer/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4401 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/analyzer/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6296 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/exceptions/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/get_config_params/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     8585 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/get_config_params/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3949 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    18904 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    10208 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/regressors/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     9623 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.616608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15134 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/utils/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.620608 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     9439 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/HuggingMouse/visualizers/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4099 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/autoapi/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)   199562 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/doctrees/environment.pickle
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5023 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/doctrees/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)    16500 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/genindex.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.620608 HuggingMouse-0.1.0/docs/_build/html/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      230 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/.buildinfo
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.620608 HuggingMouse-0.1.0/docs/_build/html/_sources/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.620608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.620608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.620608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      518 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.620608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/analyzer/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      173 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/analyzer/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.624608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      355 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/exceptions/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.624608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/get_config_params/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      390 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/get_config_params/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      387 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.624608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      850 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.624608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      428 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/regressors/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.624608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      420 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/trial_averaged_data/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.624608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      695 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/utils/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.624608 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      373 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/HuggingMouse/visualizers/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      249 2024-03-01 09:13:59.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/autoapi/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.1.0/docs/_build/html/_sources/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/_static/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    11185 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/_static/alabaster.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15094 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)       42 2021-01-29 11:59:09.000000 HuggingMouse-0.1.0/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4472 2024-02-29 21:31:27.000000 HuggingMouse-0.1.0/docs/_build/html/_static/doctools.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)      328 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)      286 2024-02-29 21:31:27.000000 HuggingMouse-0.1.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)      299 2024-02-29 21:31:27.000000 HuggingMouse-0.1.0/docs/_build/html/_static/graphviz.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4758 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/_static/language_data.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-02-29 21:31:27.000000 HuggingMouse-0.1.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-02-29 21:31:27.000000 HuggingMouse-0.1.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5387 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)    18732 2024-02-29 21:31:27.000000 HuggingMouse-0.1.0/docs/_build/html/_static/searchtools.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5123 2024-02-29 21:31:27.000000 HuggingMouse-0.1.0/docs/_build/html/_static/sphinx_highlight.js
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     7676 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/allen_api_utilities/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/analyzer/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4986 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/analyzer/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5806 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/exceptions/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/get_config_params/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6483 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/get_config_params/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6106 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    10646 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/make_embeddings/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     7086 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/regressors/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.628608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6821 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/trial_averaged_data/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.632608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     8887 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/utils/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.632608 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6398 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/HuggingMouse/visualizers/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6540 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/autoapi/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15774 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/genindex.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4169 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)      998 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/objects.inv
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5577 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/py-modindex.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2940 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/search.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)    14472 2024-03-01 09:14:00.000000 HuggingMouse-0.1.0/docs/_build/html/searchindex.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4062 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)      983 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/objects.inv
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4989 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/py-modindex.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2848 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/search.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15900 2024-03-21 22:23:00.000000 HuggingMouse-0.1.0/docs/_build/searchindex.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2430 2024-03-01 02:51:28.000000 HuggingMouse-0.1.0/docs/conf.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.1.0/docs/index.rst
+-rw-rw-r--   0 maria     (1000) maria     (1000)      800 2024-03-01 01:50:39.000000 HuggingMouse-0.1.0/docs/make.bat
+-rw-rw-r--   0 maria     (1000) maria     (1000)   716060 2024-03-22 17:33:33.000000 HuggingMouse-0.1.0/infogan.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)   849292 2024-02-26 19:58:52.000000 HuggingMouse-0.1.0/logo_CC0.jpg
+-rw-rw-r--   0 maria     (1000) maria     (1000)  1071744 2024-03-01 06:33:34.000000 HuggingMouse-0.1.0/logo_CC0_attention.jpg
+-rw-rw-r--   0 maria     (1000) maria     (1000)      106 2024-03-21 17:54:43.000000 HuggingMouse-0.1.0/pyproject.toml
+-rw-rw-r--   0 maria     (1000) maria     (1000)      131 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/requirements.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.632608 HuggingMouse-0.1.0/scripts/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.636608 HuggingMouse-0.1.0/scripts/dev_scripts/
+-rw-rw-r--   0 maria     (1000) maria     (1000)       73 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/scripts/dev_scripts/.~lock.merged_data_df.csv#
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1658 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/scripts/dev_scripts/hacking_with_labels.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      358 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/scripts/dev_scripts/interleaved.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)    63483 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/scripts/dev_scripts/merged_data_df.csv
+-rw-rw-r--   0 maria     (1000) maria     (1000)      854 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/scripts/dev_scripts/test.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      283 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/scripts/dev_scripts/test_exp_ids.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2483 2024-03-22 02:43:14.000000 HuggingMouse-0.1.0/scripts/example_script.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      710 2024-06-01 01:23:35.000000 HuggingMouse-0.1.0/scripts/example_script_pipelines.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2576 2024-03-21 15:08:54.000000 HuggingMouse-0.1.0/scripts/get_hf_model_downloads_sorted.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)   519717 2024-03-03 16:11:41.000000 HuggingMouse-0.1.0/scripts/sorted_models_downloads.json
+-rw-rw-r--   0 maria     (1000) maria     (1000)       38 2024-06-01 01:31:36.640608 HuggingMouse-0.1.0/setup.cfg
+-rw-rw-r--   0 maria     (1000) maria     (1000)      612 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/setup.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.580608 HuggingMouse-0.1.0/src/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.636608 HuggingMouse-0.1.0/src/HuggingMouse/
+-rw-rw-r--   0 maria     (1000) maria     (1000)       22 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/src/HuggingMouse/__init__.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4384 2024-03-21 15:06:01.000000 HuggingMouse-0.1.0/src/HuggingMouse/allen_api_utilities.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      888 2024-03-21 15:08:45.000000 HuggingMouse-0.1.0/src/HuggingMouse/custom_exceptions.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3703 2024-03-22 02:36:00.000000 HuggingMouse-0.1.0/src/HuggingMouse/make_embeddings.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.640608 HuggingMouse-0.1.0/src/HuggingMouse/pipelines/
+-rw-rw-r--   0 maria     (1000) maria     (1000)        0 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/src/HuggingMouse/pipelines/__init__.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      128 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/src/HuggingMouse/pipelines/base.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     7869 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/src/HuggingMouse/pipelines/neuron_prediction.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      333 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/src/HuggingMouse/pipelines/pipeline_tasks.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3104 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/src/HuggingMouse/pipelines/single_trial_fs.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6914 2024-03-21 15:22:07.000000 HuggingMouse-0.1.0/src/HuggingMouse/regressors.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2663 2024-04-26 15:55:46.000000 HuggingMouse-0.1.0/src/HuggingMouse/trial_averaged_data.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3090 2024-03-21 15:33:11.000000 HuggingMouse-0.1.0/src/HuggingMouse/utils.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1860 2024-03-22 18:41:54.000000 HuggingMouse-0.1.0/src/HuggingMouse/visualizers.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.640608 HuggingMouse-0.1.0/src/HuggingMouse.egg-info/
+-rw-r--r--   0 maria     (1000) maria     (1000)      471 2024-06-01 01:31:36.000000 HuggingMouse-0.1.0/src/HuggingMouse.egg-info/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6728 2024-06-01 01:31:36.000000 HuggingMouse-0.1.0/src/HuggingMouse.egg-info/SOURCES.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)        1 2024-06-01 01:31:36.000000 HuggingMouse-0.1.0/src/HuggingMouse.egg-info/dependency_links.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      114 2024-06-01 01:31:36.000000 HuggingMouse-0.1.0/src/HuggingMouse.egg-info/requires.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)       13 2024-06-01 01:31:36.000000 HuggingMouse-0.1.0/src/HuggingMouse.egg-info/top_level.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 01:31:36.640608 HuggingMouse-0.1.0/tutorial_notebooks/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    18329 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/tutorial_notebooks/clip.ipynb
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1725 2024-06-01 01:05:07.000000 HuggingMouse-0.1.0/tutorial_notebooks/top_10.ipynb
```

### Comparing `HuggingMouse-0.0.2/LICENSE` & `HuggingMouse-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.0.2/setup.py` & `HuggingMouse-0.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(name='HuggingMouse',
-      version='0.0.2',
+      version='0.1.0',
       description='Data analysis library for Allen Brain Observatory data',
       author='Maria Kesa',
       author_email='mariarosekesa@gmail.com',
       url='https://github.com/mariakesa/HuggingMouse',
       install_requires=[
           'scikit-learn==1.2.2',
           'torch==1.13.1',
           'pandas==1.5.3',
           'numpy==1.23.5',
           'transformers==4.31.0',
-          'allensdk==2.16.2'
+          'allensdk==2.16.2',
+          'plotly==5.9.0'
       ],
       packages=find_packages("src"),
       package_dir={"": "src"}
       )
```

### Comparing `HuggingMouse-0.0.2/src/HuggingMouse/allen_api_utilities.py` & `HuggingMouse-0.1.0/src/HuggingMouse/allen_api_utilities.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.0.2/src/HuggingMouse/custom_exceptions.py` & `HuggingMouse-0.1.0/src/HuggingMouse/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.0.2/src/HuggingMouse/make_embeddings.py` & `HuggingMouse-0.1.0/src/HuggingMouse/make_embeddings.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.0.2/src/HuggingMouse/regressors.py` & `HuggingMouse-0.1.0/src/HuggingMouse/regressors.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.0.2/src/HuggingMouse/trial_averaged_data.py` & `HuggingMouse-0.1.0/src/HuggingMouse/trial_averaged_data.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.0.2/src/HuggingMouse/utils.py` & `HuggingMouse-0.1.0/src/HuggingMouse/utils.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.0.2/src/HuggingMouse/visualizers.py` & `HuggingMouse-0.1.0/src/HuggingMouse/visualizers.py`

 * *Files identical despite different names*

