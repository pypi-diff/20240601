# Comparing `tmp/HuggingMouse-0.1.1.tar.gz` & `tmp/HuggingMouse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HuggingMouse-0.1.1.tar", last modified: Sat Jun  1 03:23:23 2024, max compression
+gzip compressed data, was "HuggingMouse-0.2.0.tar", last modified: Sat Jun  1 03:28:18 2024, max compression
```

## Comparing `HuggingMouse-0.1.1.tar` & `HuggingMouse-0.2.0.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.149208 HuggingMouse-0.1.1/
--rw-rw-r--   0 maria     (1000) maria     (1000)     3082 2024-03-21 16:02:48.000000 HuggingMouse-0.1.1/.gitignore
--rw-rw-r--   0 maria     (1000) maria     (1000)      953 2024-03-01 02:48:49.000000 HuggingMouse-0.1.1/.readthedocs.yaml
--rw-rw-r--   0 maria     (1000) maria     (1000)    35149 2024-02-26 19:48:43.000000 HuggingMouse-0.1.1/LICENSE
--rw-r--r--   0 maria     (1000) maria     (1000)      471 2024-06-01 03:23:23.149208 HuggingMouse-0.1.1/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)     6009 2024-06-01 01:28:28.000000 HuggingMouse-0.1.1/README.md
--rw-rw-r--   0 maria     (1000) maria     (1000)    61631 2024-03-22 17:18:08.000000 HuggingMouse-0.1.1/VarExp.png
--rw-rw-r--   0 maria     (1000) maria     (1000)  7344609 2024-03-20 03:35:03.000000 HuggingMouse-0.1.1/calcium_movie.gif
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.097207 HuggingMouse-0.1.1/docs/
--rw-rw-r--   0 maria     (1000) maria     (1000)      634 2024-03-01 01:50:39.000000 HuggingMouse-0.1.1/docs/Makefile
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.097207 HuggingMouse-0.1.1/docs/_build/
--rw-rw-r--   0 maria     (1000) maria     (1000)      230 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.buildinfo
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/allen_api_utilities/
--rw-rw-r--   0 maria     (1000) maria     (1000)    13248 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/custom_exceptions/
--rw-rw-r--   0 maria     (1000) maria     (1000)    12797 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/custom_exceptions/index.doctree
--rw-rw-r--   0 maria     (1000) maria     (1000)     3871 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/make_embeddings/
--rw-rw-r--   0 maria     (1000) maria     (1000)    20957 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/regressors/
--rw-rw-r--   0 maria     (1000) maria     (1000)    13700 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/regressors/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/trial_averaged_data/
--rw-rw-r--   0 maria     (1000) maria     (1000)    10234 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.101207 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/utils/
--rw-rw-r--   0 maria     (1000) maria     (1000)    17337 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/utils/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/visualizers/
--rw-rw-r--   0 maria     (1000) maria     (1000)    10506 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/visualizers/index.doctree
--rw-rw-r--   0 maria     (1000) maria     (1000)     4109 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/index.doctree
--rw-rw-r--   0 maria     (1000) maria     (1000)   321104 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/environment.pickle
--rw-rw-r--   0 maria     (1000) maria     (1000)     5033 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/.doctrees/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/allen_api_utilities/
--rw-rw-r--   0 maria     (1000) maria     (1000)      794 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/custom_exceptions/
--rw-rw-r--   0 maria     (1000) maria     (1000)     1018 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/custom_exceptions/index.rst.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)      341 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/make_embeddings/
--rw-rw-r--   0 maria     (1000) maria     (1000)     1198 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/regressors/
--rw-rw-r--   0 maria     (1000) maria     (1000)     1104 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/regressors/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/trial_averaged_data/
--rw-rw-r--   0 maria     (1000) maria     (1000)      538 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/trial_averaged_data/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/utils/
--rw-rw-r--   0 maria     (1000) maria     (1000)      765 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/utils/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.105208 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/visualizers/
--rw-rw-r--   0 maria     (1000) maria     (1000)      665 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/visualizers/index.rst.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)      249 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_sources/autoapi/index.rst.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.1.1/docs/_build/_sources/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/_static/
--rw-rw-r--   0 maria     (1000) maria     (1000)    11143 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_static/alabaster.css
--rw-rw-r--   0 maria     (1000) maria     (1000)    15096 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_static/basic.css
--rw-rw-r--   0 maria     (1000) maria     (1000)       42 2024-03-20 04:17:52.000000 HuggingMouse-0.1.1/docs/_build/_static/custom.css
--rw-rw-r--   0 maria     (1000) maria     (1000)     4472 2024-03-20 04:18:06.000000 HuggingMouse-0.1.1/docs/_build/_static/doctools.js
--rw-rw-r--   0 maria     (1000) maria     (1000)      328 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_static/documentation_options.js
--rw-rw-r--   0 maria     (1000) maria     (1000)      286 2024-03-20 04:18:06.000000 HuggingMouse-0.1.1/docs/_build/_static/file.png
--rw-rw-r--   0 maria     (1000) maria     (1000)      299 2024-03-20 04:18:06.000000 HuggingMouse-0.1.1/docs/_build/_static/graphviz.css
--rw-rw-r--   0 maria     (1000) maria     (1000)     4758 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_static/language_data.js
--rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-03-20 04:18:06.000000 HuggingMouse-0.1.1/docs/_build/_static/minus.png
--rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-03-20 04:18:06.000000 HuggingMouse-0.1.1/docs/_build/_static/plus.png
--rw-rw-r--   0 maria     (1000) maria     (1000)     5359 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/_static/pygments.css
--rw-rw-r--   0 maria     (1000) maria     (1000)    18732 2024-03-20 04:18:06.000000 HuggingMouse-0.1.1/docs/_build/_static/searchtools.js
--rw-rw-r--   0 maria     (1000) maria     (1000)     5123 2024-03-20 04:18:06.000000 HuggingMouse-0.1.1/docs/_build/_static/sphinx_highlight.js
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/allen_api_utilities/
--rw-rw-r--   0 maria     (1000) maria     (1000)     8255 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/allen_api_utilities/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/custom_exceptions/
--rw-rw-r--   0 maria     (1000) maria     (1000)     9342 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/custom_exceptions/index.html
--rw-rw-r--   0 maria     (1000) maria     (1000)     5593 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/make_embeddings/
--rw-rw-r--   0 maria     (1000) maria     (1000)    11396 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/make_embeddings/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/regressors/
--rw-rw-r--   0 maria     (1000) maria     (1000)     8436 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/regressors/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/trial_averaged_data/
--rw-rw-r--   0 maria     (1000) maria     (1000)     6912 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/trial_averaged_data/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/utils/
--rw-rw-r--   0 maria     (1000) maria     (1000)     9647 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/utils/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.113207 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/visualizers/
--rw-rw-r--   0 maria     (1000) maria     (1000)     6719 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/visualizers/index.html
--rw-rw-r--   0 maria     (1000) maria     (1000)     6009 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/autoapi/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.117208 HuggingMouse-0.1.1/docs/_build/doctrees/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.117208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.117208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.117208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/allen_api_utilities/
--rw-rw-r--   0 maria     (1000) maria     (1000)    11686 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.117208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/analyzer/
--rw-rw-r--   0 maria     (1000) maria     (1000)     4401 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/analyzer/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.117208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/exceptions/
--rw-rw-r--   0 maria     (1000) maria     (1000)     6296 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/exceptions/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.117208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/get_config_params/
--rw-rw-r--   0 maria     (1000) maria     (1000)     8585 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/get_config_params/index.doctree
--rw-rw-r--   0 maria     (1000) maria     (1000)     3949 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.117208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/make_embeddings/
--rw-rw-r--   0 maria     (1000) maria     (1000)    18904 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.121208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/regressors/
--rw-rw-r--   0 maria     (1000) maria     (1000)    10208 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/regressors/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.121208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/trial_averaged_data/
--rw-rw-r--   0 maria     (1000) maria     (1000)     9623 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.121208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/utils/
--rw-rw-r--   0 maria     (1000) maria     (1000)    15134 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/utils/index.doctree
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.121208 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/visualizers/
--rw-rw-r--   0 maria     (1000) maria     (1000)     9439 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/visualizers/index.doctree
--rw-rw-r--   0 maria     (1000) maria     (1000)     4099 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/index.doctree
--rw-rw-r--   0 maria     (1000) maria     (1000)   199562 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 maria     (1000) maria     (1000)     5023 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/doctrees/index.doctree
--rw-rw-r--   0 maria     (1000) maria     (1000)    16500 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/genindex.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.121208 HuggingMouse-0.1.1/docs/_build/html/
--rw-rw-r--   0 maria     (1000) maria     (1000)      230 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/.buildinfo
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/allen_api_utilities/
--rw-rw-r--   0 maria     (1000) maria     (1000)      518 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/analyzer/
--rw-rw-r--   0 maria     (1000) maria     (1000)      173 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/analyzer/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/exceptions/
--rw-rw-r--   0 maria     (1000) maria     (1000)      355 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/exceptions/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/get_config_params/
--rw-rw-r--   0 maria     (1000) maria     (1000)      390 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/get_config_params/index.rst.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)      387 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/make_embeddings/
--rw-rw-r--   0 maria     (1000) maria     (1000)      850 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/regressors/
--rw-rw-r--   0 maria     (1000) maria     (1000)      428 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/regressors/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/trial_averaged_data/
--rw-rw-r--   0 maria     (1000) maria     (1000)      420 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/trial_averaged_data/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/utils/
--rw-rw-r--   0 maria     (1000) maria     (1000)      695 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/utils/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.125208 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/visualizers/
--rw-rw-r--   0 maria     (1000) maria     (1000)      373 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/visualizers/index.rst.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)      249 2024-03-01 09:13:59.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/index.rst.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.1.1/docs/_build/html/_sources/index.rst.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/_static/
--rw-rw-r--   0 maria     (1000) maria     (1000)    11185 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/_static/alabaster.css
--rw-rw-r--   0 maria     (1000) maria     (1000)    15094 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/_static/basic.css
--rw-rw-r--   0 maria     (1000) maria     (1000)       42 2021-01-29 11:59:09.000000 HuggingMouse-0.1.1/docs/_build/html/_static/custom.css
--rw-rw-r--   0 maria     (1000) maria     (1000)     4472 2024-02-29 21:31:27.000000 HuggingMouse-0.1.1/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 maria     (1000) maria     (1000)      328 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 maria     (1000) maria     (1000)      286 2024-02-29 21:31:27.000000 HuggingMouse-0.1.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 maria     (1000) maria     (1000)      299 2024-02-29 21:31:27.000000 HuggingMouse-0.1.1/docs/_build/html/_static/graphviz.css
--rw-rw-r--   0 maria     (1000) maria     (1000)     4758 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-02-29 21:31:27.000000 HuggingMouse-0.1.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-02-29 21:31:27.000000 HuggingMouse-0.1.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 maria     (1000) maria     (1000)     5387 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 maria     (1000) maria     (1000)    18732 2024-02-29 21:31:27.000000 HuggingMouse-0.1.1/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 maria     (1000) maria     (1000)     5123 2024-02-29 21:31:27.000000 HuggingMouse-0.1.1/docs/_build/html/_static/sphinx_highlight.js
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/allen_api_utilities/
--rw-rw-r--   0 maria     (1000) maria     (1000)     7676 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/allen_api_utilities/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/analyzer/
--rw-rw-r--   0 maria     (1000) maria     (1000)     4986 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/analyzer/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/exceptions/
--rw-rw-r--   0 maria     (1000) maria     (1000)     5806 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/exceptions/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/get_config_params/
--rw-rw-r--   0 maria     (1000) maria     (1000)     6483 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/get_config_params/index.html
--rw-rw-r--   0 maria     (1000) maria     (1000)     6106 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/make_embeddings/
--rw-rw-r--   0 maria     (1000) maria     (1000)    10646 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/make_embeddings/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/regressors/
--rw-rw-r--   0 maria     (1000) maria     (1000)     7086 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/regressors/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.133208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/trial_averaged_data/
--rw-rw-r--   0 maria     (1000) maria     (1000)     6821 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/trial_averaged_data/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.137208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/utils/
--rw-rw-r--   0 maria     (1000) maria     (1000)     8887 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/utils/index.html
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.137208 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/visualizers/
--rw-rw-r--   0 maria     (1000) maria     (1000)     6398 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/visualizers/index.html
--rw-rw-r--   0 maria     (1000) maria     (1000)     6540 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/autoapi/index.html
--rw-rw-r--   0 maria     (1000) maria     (1000)    15774 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/genindex.html
--rw-rw-r--   0 maria     (1000) maria     (1000)     4169 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/index.html
--rw-rw-r--   0 maria     (1000) maria     (1000)      998 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/objects.inv
--rw-rw-r--   0 maria     (1000) maria     (1000)     5577 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/py-modindex.html
--rw-rw-r--   0 maria     (1000) maria     (1000)     2940 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/search.html
--rw-rw-r--   0 maria     (1000) maria     (1000)    14472 2024-03-01 09:14:00.000000 HuggingMouse-0.1.1/docs/_build/html/searchindex.js
--rw-rw-r--   0 maria     (1000) maria     (1000)     4062 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/index.html
--rw-rw-r--   0 maria     (1000) maria     (1000)      983 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/objects.inv
--rw-rw-r--   0 maria     (1000) maria     (1000)     4989 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/py-modindex.html
--rw-rw-r--   0 maria     (1000) maria     (1000)     2848 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/search.html
--rw-rw-r--   0 maria     (1000) maria     (1000)    15900 2024-03-21 22:23:00.000000 HuggingMouse-0.1.1/docs/_build/searchindex.js
--rw-rw-r--   0 maria     (1000) maria     (1000)     2430 2024-03-01 02:51:28.000000 HuggingMouse-0.1.1/docs/conf.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.1.1/docs/index.rst
--rw-rw-r--   0 maria     (1000) maria     (1000)      800 2024-03-01 01:50:39.000000 HuggingMouse-0.1.1/docs/make.bat
--rw-rw-r--   0 maria     (1000) maria     (1000)   716060 2024-03-22 17:33:33.000000 HuggingMouse-0.1.1/infogan.png
--rw-rw-r--   0 maria     (1000) maria     (1000)   849292 2024-02-26 19:58:52.000000 HuggingMouse-0.1.1/logo_CC0.jpg
--rw-rw-r--   0 maria     (1000) maria     (1000)  1071744 2024-03-01 06:33:34.000000 HuggingMouse-0.1.1/logo_CC0_attention.jpg
--rw-rw-r--   0 maria     (1000) maria     (1000)      106 2024-03-21 17:54:43.000000 HuggingMouse-0.1.1/pyproject.toml
--rw-rw-r--   0 maria     (1000) maria     (1000)      131 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/requirements.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.137208 HuggingMouse-0.1.1/scripts/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.141208 HuggingMouse-0.1.1/scripts/dev_scripts/
--rw-rw-r--   0 maria     (1000) maria     (1000)       73 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/scripts/dev_scripts/.~lock.merged_data_df.csv#
--rw-rw-r--   0 maria     (1000) maria     (1000)     1658 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/scripts/dev_scripts/hacking_with_labels.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      358 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/scripts/dev_scripts/interleaved.py
--rw-rw-r--   0 maria     (1000) maria     (1000)    63483 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/scripts/dev_scripts/merged_data_df.csv
--rw-rw-r--   0 maria     (1000) maria     (1000)      854 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/scripts/dev_scripts/test.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      283 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/scripts/dev_scripts/test_exp_ids.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     2483 2024-03-22 02:43:14.000000 HuggingMouse-0.1.1/scripts/example_script.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      800 2024-06-01 02:48:04.000000 HuggingMouse-0.1.1/scripts/example_script_pipelines.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     2576 2024-03-21 15:08:54.000000 HuggingMouse-0.1.1/scripts/get_hf_model_downloads_sorted.py
--rw-rw-r--   0 maria     (1000) maria     (1000)   519717 2024-03-03 16:11:41.000000 HuggingMouse-0.1.1/scripts/sorted_models_downloads.json
--rw-rw-r--   0 maria     (1000) maria     (1000)       38 2024-06-01 03:23:23.149208 HuggingMouse-0.1.1/setup.cfg
--rw-rw-r--   0 maria     (1000) maria     (1000)      612 2024-06-01 02:42:10.000000 HuggingMouse-0.1.1/setup.py
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.073207 HuggingMouse-0.1.1/src/
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.145208 HuggingMouse-0.1.1/src/HuggingMouse/
--rw-rw-r--   0 maria     (1000) maria     (1000)       22 2024-06-01 02:53:08.000000 HuggingMouse-0.1.1/src/HuggingMouse/__init__.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     4384 2024-03-21 15:06:01.000000 HuggingMouse-0.1.1/src/HuggingMouse/allen_api_utilities.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      888 2024-03-21 15:08:45.000000 HuggingMouse-0.1.1/src/HuggingMouse/custom_exceptions.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     3703 2024-03-22 02:36:00.000000 HuggingMouse-0.1.1/src/HuggingMouse/make_embeddings.py
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.145208 HuggingMouse-0.1.1/src/HuggingMouse/pipelines/
--rw-rw-r--   0 maria     (1000) maria     (1000)        0 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/src/HuggingMouse/pipelines/__init__.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      128 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/src/HuggingMouse/pipelines/base.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     7988 2024-06-01 02:41:45.000000 HuggingMouse-0.1.1/src/HuggingMouse/pipelines/neuron_prediction.py
--rw-rw-r--   0 maria     (1000) maria     (1000)      333 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/src/HuggingMouse/pipelines/pipeline_tasks.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     3104 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/src/HuggingMouse/pipelines/single_trial_fs.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     6914 2024-03-21 15:22:07.000000 HuggingMouse-0.1.1/src/HuggingMouse/regressors.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     2663 2024-04-26 15:55:46.000000 HuggingMouse-0.1.1/src/HuggingMouse/trial_averaged_data.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     3090 2024-03-21 15:33:11.000000 HuggingMouse-0.1.1/src/HuggingMouse/utils.py
--rw-rw-r--   0 maria     (1000) maria     (1000)     1860 2024-03-22 18:41:54.000000 HuggingMouse-0.1.1/src/HuggingMouse/visualizers.py
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.149208 HuggingMouse-0.1.1/src/HuggingMouse.egg-info/
--rw-r--r--   0 maria     (1000) maria     (1000)      471 2024-06-01 03:23:22.000000 HuggingMouse-0.1.1/src/HuggingMouse.egg-info/PKG-INFO
--rw-rw-r--   0 maria     (1000) maria     (1000)     6728 2024-06-01 03:23:22.000000 HuggingMouse-0.1.1/src/HuggingMouse.egg-info/SOURCES.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)        1 2024-06-01 03:23:22.000000 HuggingMouse-0.1.1/src/HuggingMouse.egg-info/dependency_links.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)      114 2024-06-01 03:23:22.000000 HuggingMouse-0.1.1/src/HuggingMouse.egg-info/requires.txt
--rw-rw-r--   0 maria     (1000) maria     (1000)       13 2024-06-01 03:23:22.000000 HuggingMouse-0.1.1/src/HuggingMouse.egg-info/top_level.txt
-drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:23:23.145208 HuggingMouse-0.1.1/tutorial_notebooks/
--rw-rw-r--   0 maria     (1000) maria     (1000)    18329 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/tutorial_notebooks/clip.ipynb
--rw-rw-r--   0 maria     (1000) maria     (1000)     1725 2024-06-01 01:05:07.000000 HuggingMouse-0.1.1/tutorial_notebooks/top_10.ipynb
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.935675 HuggingMouse-0.2.0/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3082 2024-03-21 16:02:48.000000 HuggingMouse-0.2.0/.gitignore
+-rw-rw-r--   0 maria     (1000) maria     (1000)      953 2024-03-01 02:48:49.000000 HuggingMouse-0.2.0/.readthedocs.yaml
+-rw-rw-r--   0 maria     (1000) maria     (1000)    35149 2024-02-26 19:48:43.000000 HuggingMouse-0.2.0/LICENSE
+-rw-r--r--   0 maria     (1000) maria     (1000)      471 2024-06-01 03:28:18.931676 HuggingMouse-0.2.0/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6009 2024-06-01 01:28:28.000000 HuggingMouse-0.2.0/README.md
+-rw-rw-r--   0 maria     (1000) maria     (1000)    61631 2024-03-22 17:18:08.000000 HuggingMouse-0.2.0/VarExp.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)  7344609 2024-03-20 03:35:03.000000 HuggingMouse-0.2.0/calcium_movie.gif
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.895675 HuggingMouse-0.2.0/docs/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      634 2024-03-01 01:50:39.000000 HuggingMouse-0.2.0/docs/Makefile
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.895675 HuggingMouse-0.2.0/docs/_build/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      230 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.buildinfo
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    13248 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/custom_exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    12797 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/custom_exceptions/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3871 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    20957 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    13700 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/regressors/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    10234 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    17337 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/utils/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    10506 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/visualizers/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4109 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)   321104 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/environment.pickle
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5033 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/.doctrees/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/_sources/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.899675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.903675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      794 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.903675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/custom_exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1018 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/custom_exceptions/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      341 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.903675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1198 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.903675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1104 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/regressors/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.903675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      538 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/trial_averaged_data/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.903675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      765 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/utils/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.903675 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      665 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/visualizers/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      249 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_sources/autoapi/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.2.0/docs/_build/_sources/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/_static/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    11143 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_static/alabaster.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15096 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_static/basic.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)       42 2024-03-20 04:17:52.000000 HuggingMouse-0.2.0/docs/_build/_static/custom.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4472 2024-03-20 04:18:06.000000 HuggingMouse-0.2.0/docs/_build/_static/doctools.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)      328 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_static/documentation_options.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)      286 2024-03-20 04:18:06.000000 HuggingMouse-0.2.0/docs/_build/_static/file.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)      299 2024-03-20 04:18:06.000000 HuggingMouse-0.2.0/docs/_build/_static/graphviz.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4758 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_static/language_data.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-03-20 04:18:06.000000 HuggingMouse-0.2.0/docs/_build/_static/minus.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-03-20 04:18:06.000000 HuggingMouse-0.2.0/docs/_build/_static/plus.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5359 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/_static/pygments.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)    18732 2024-03-20 04:18:06.000000 HuggingMouse-0.2.0/docs/_build/_static/searchtools.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5123 2024-03-20 04:18:06.000000 HuggingMouse-0.2.0/docs/_build/_static/sphinx_highlight.js
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     8255 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/allen_api_utilities/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/custom_exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     9342 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/custom_exceptions/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5593 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    11396 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/make_embeddings/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     8436 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/regressors/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6912 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/trial_averaged_data/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     9647 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/utils/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.907675 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6719 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/visualizers/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6009 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/autoapi/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    11686 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/analyzer/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4401 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/analyzer/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6296 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/exceptions/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/get_config_params/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     8585 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/get_config_params/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3949 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    18904 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    10208 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/regressors/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     9623 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15134 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/utils/index.doctree
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.911675 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     9439 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/visualizers/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4099 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)   199562 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/doctrees/environment.pickle
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5023 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/doctrees/index.doctree
+-rw-rw-r--   0 maria     (1000) maria     (1000)    16500 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/genindex.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      230 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/.buildinfo
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      518 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/analyzer/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      173 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/analyzer/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      355 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/exceptions/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/get_config_params/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      390 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/get_config_params/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      387 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      850 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      428 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/regressors/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      420 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/trial_averaged_data/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      695 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/utils/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.915675 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      373 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/visualizers/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      249 2024-03-01 09:13:59.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/index.rst.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.2.0/docs/_build/html/_sources/index.rst.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.919675 HuggingMouse-0.2.0/docs/_build/html/_static/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    11185 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/_static/alabaster.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15094 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)       42 2021-01-29 11:59:09.000000 HuggingMouse-0.2.0/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4472 2024-02-29 21:31:27.000000 HuggingMouse-0.2.0/docs/_build/html/_static/doctools.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)      328 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)      286 2024-02-29 21:31:27.000000 HuggingMouse-0.2.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)      299 2024-02-29 21:31:27.000000 HuggingMouse-0.2.0/docs/_build/html/_static/graphviz.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4758 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/_static/language_data.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-02-29 21:31:27.000000 HuggingMouse-0.2.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)       90 2024-02-29 21:31:27.000000 HuggingMouse-0.2.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5387 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 maria     (1000) maria     (1000)    18732 2024-02-29 21:31:27.000000 HuggingMouse-0.2.0/docs/_build/html/_static/searchtools.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5123 2024-02-29 21:31:27.000000 HuggingMouse-0.2.0/docs/_build/html/_static/sphinx_highlight.js
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.919675 HuggingMouse-0.2.0/docs/_build/html/autoapi/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.919675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/allen_api_utilities/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     7676 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/allen_api_utilities/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/analyzer/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4986 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/analyzer/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/exceptions/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5806 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/exceptions/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/get_config_params/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6483 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/get_config_params/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6106 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/make_embeddings/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    10646 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/make_embeddings/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/regressors/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     7086 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/regressors/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/trial_averaged_data/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6821 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/trial_averaged_data/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/utils/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     8887 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/utils/index.html
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/visualizers/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6398 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/visualizers/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6540 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/autoapi/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15774 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/genindex.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4169 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)      998 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/objects.inv
+-rw-rw-r--   0 maria     (1000) maria     (1000)     5577 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/py-modindex.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2940 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/search.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)    14472 2024-03-01 09:14:00.000000 HuggingMouse-0.2.0/docs/_build/html/searchindex.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4062 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/index.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)      983 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/objects.inv
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4989 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/py-modindex.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2848 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/search.html
+-rw-rw-r--   0 maria     (1000) maria     (1000)    15900 2024-03-21 22:23:00.000000 HuggingMouse-0.2.0/docs/_build/searchindex.js
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2430 2024-03-01 02:51:28.000000 HuggingMouse-0.2.0/docs/conf.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      452 2024-03-01 01:50:39.000000 HuggingMouse-0.2.0/docs/index.rst
+-rw-rw-r--   0 maria     (1000) maria     (1000)      800 2024-03-01 01:50:39.000000 HuggingMouse-0.2.0/docs/make.bat
+-rw-rw-r--   0 maria     (1000) maria     (1000)   716060 2024-03-22 17:33:33.000000 HuggingMouse-0.2.0/infogan.png
+-rw-rw-r--   0 maria     (1000) maria     (1000)   849292 2024-02-26 19:58:52.000000 HuggingMouse-0.2.0/logo_CC0.jpg
+-rw-rw-r--   0 maria     (1000) maria     (1000)  1071744 2024-03-01 06:33:34.000000 HuggingMouse-0.2.0/logo_CC0_attention.jpg
+-rw-rw-r--   0 maria     (1000) maria     (1000)      106 2024-03-21 17:54:43.000000 HuggingMouse-0.2.0/pyproject.toml
+-rw-rw-r--   0 maria     (1000) maria     (1000)      131 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/requirements.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.923675 HuggingMouse-0.2.0/scripts/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.927675 HuggingMouse-0.2.0/scripts/dev_scripts/
+-rw-rw-r--   0 maria     (1000) maria     (1000)       73 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/scripts/dev_scripts/.~lock.merged_data_df.csv#
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1658 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/scripts/dev_scripts/hacking_with_labels.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      358 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/scripts/dev_scripts/interleaved.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)    63483 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/scripts/dev_scripts/merged_data_df.csv
+-rw-rw-r--   0 maria     (1000) maria     (1000)      854 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/scripts/dev_scripts/test.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      283 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/scripts/dev_scripts/test_exp_ids.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2483 2024-03-22 02:43:14.000000 HuggingMouse-0.2.0/scripts/example_script.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      800 2024-06-01 02:48:04.000000 HuggingMouse-0.2.0/scripts/example_script_pipelines.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2576 2024-03-21 15:08:54.000000 HuggingMouse-0.2.0/scripts/get_hf_model_downloads_sorted.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)   519717 2024-03-03 16:11:41.000000 HuggingMouse-0.2.0/scripts/sorted_models_downloads.json
+-rw-rw-r--   0 maria     (1000) maria     (1000)       38 2024-06-01 03:28:18.935675 HuggingMouse-0.2.0/setup.cfg
+-rw-rw-r--   0 maria     (1000) maria     (1000)      612 2024-06-01 03:27:17.000000 HuggingMouse-0.2.0/setup.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.875675 HuggingMouse-0.2.0/src/
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.927675 HuggingMouse-0.2.0/src/HuggingMouse/
+-rw-rw-r--   0 maria     (1000) maria     (1000)       22 2024-06-01 03:27:26.000000 HuggingMouse-0.2.0/src/HuggingMouse/__init__.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4384 2024-03-21 15:06:01.000000 HuggingMouse-0.2.0/src/HuggingMouse/allen_api_utilities.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      888 2024-03-21 15:08:45.000000 HuggingMouse-0.2.0/src/HuggingMouse/custom_exceptions.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3703 2024-03-22 02:36:00.000000 HuggingMouse-0.2.0/src/HuggingMouse/make_embeddings.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.931676 HuggingMouse-0.2.0/src/HuggingMouse/pipelines/
+-rw-rw-r--   0 maria     (1000) maria     (1000)        0 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/src/HuggingMouse/pipelines/__init__.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      128 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/src/HuggingMouse/pipelines/base.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     7988 2024-06-01 02:41:45.000000 HuggingMouse-0.2.0/src/HuggingMouse/pipelines/neuron_prediction.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      333 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/src/HuggingMouse/pipelines/pipeline_tasks.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3104 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/src/HuggingMouse/pipelines/single_trial_fs.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6914 2024-03-21 15:22:07.000000 HuggingMouse-0.2.0/src/HuggingMouse/regressors.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     2663 2024-04-26 15:55:46.000000 HuggingMouse-0.2.0/src/HuggingMouse/trial_averaged_data.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     3090 2024-03-21 15:33:11.000000 HuggingMouse-0.2.0/src/HuggingMouse/utils.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1860 2024-03-22 18:41:54.000000 HuggingMouse-0.2.0/src/HuggingMouse/visualizers.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.931676 HuggingMouse-0.2.0/src/HuggingMouse.egg-info/
+-rw-r--r--   0 maria     (1000) maria     (1000)      471 2024-06-01 03:28:18.000000 HuggingMouse-0.2.0/src/HuggingMouse.egg-info/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)     6728 2024-06-01 03:28:18.000000 HuggingMouse-0.2.0/src/HuggingMouse.egg-info/SOURCES.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)        1 2024-06-01 03:28:18.000000 HuggingMouse-0.2.0/src/HuggingMouse.egg-info/dependency_links.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)      114 2024-06-01 03:28:18.000000 HuggingMouse-0.2.0/src/HuggingMouse.egg-info/requires.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)       13 2024-06-01 03:28:18.000000 HuggingMouse-0.2.0/src/HuggingMouse.egg-info/top_level.txt
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-06-01 03:28:18.931676 HuggingMouse-0.2.0/tutorial_notebooks/
+-rw-rw-r--   0 maria     (1000) maria     (1000)    18329 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/tutorial_notebooks/clip.ipynb
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1725 2024-06-01 01:05:07.000000 HuggingMouse-0.2.0/tutorial_notebooks/top_10.ipynb
```

### Comparing `HuggingMouse-0.1.1/.gitignore` & `HuggingMouse-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/.readthedocs.yaml` & `HuggingMouse-0.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/LICENSE` & `HuggingMouse-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/README.md` & `HuggingMouse-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/VarExp.png` & `HuggingMouse-0.2.0/VarExp.png`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/calcium_movie.gif` & `HuggingMouse-0.2.0/calcium_movie.gif`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/Makefile` & `HuggingMouse-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/custom_exceptions/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/custom_exceptions/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/regressors/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/regressors/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/utils/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/utils/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/HuggingMouse/visualizers/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/HuggingMouse/visualizers/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/autoapi/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/autoapi/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/environment.pickle` & `HuggingMouse-0.2.0/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/.doctrees/index.doctree` & `HuggingMouse-0.2.0/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/custom_exceptions/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/custom_exceptions/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/regressors/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/regressors/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/trial_averaged_data/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/trial_averaged_data/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/utils/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/utils/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_sources/autoapi/HuggingMouse/visualizers/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/_sources/autoapi/HuggingMouse/visualizers/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_static/alabaster.css` & `HuggingMouse-0.2.0/docs/_build/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_static/basic.css` & `HuggingMouse-0.2.0/docs/_build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_static/doctools.js` & `HuggingMouse-0.2.0/docs/_build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_static/language_data.js` & `HuggingMouse-0.2.0/docs/_build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_static/pygments.css` & `HuggingMouse-0.2.0/docs/_build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_static/searchtools.js` & `HuggingMouse-0.2.0/docs/_build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/_static/sphinx_highlight.js` & `HuggingMouse-0.2.0/docs/_build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/allen_api_utilities/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/allen_api_utilities/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/custom_exceptions/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/custom_exceptions/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/make_embeddings/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/make_embeddings/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/regressors/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/regressors/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/trial_averaged_data/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/trial_averaged_data/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/utils/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/utils/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/HuggingMouse/visualizers/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/HuggingMouse/visualizers/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/autoapi/index.html` & `HuggingMouse-0.2.0/docs/_build/autoapi/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/allen_api_utilities/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/analyzer/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/analyzer/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/exceptions/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/exceptions/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/get_config_params/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/get_config_params/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/make_embeddings/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/regressors/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/regressors/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/trial_averaged_data/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/utils/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/utils/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/HuggingMouse/visualizers/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/HuggingMouse/visualizers/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/autoapi/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/autoapi/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/environment.pickle` & `HuggingMouse-0.2.0/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/doctrees/index.doctree` & `HuggingMouse-0.2.0/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/genindex.html` & `HuggingMouse-0.2.0/docs/_build/genindex.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/allen_api_utilities/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/make_embeddings/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_sources/autoapi/HuggingMouse/utils/index.rst.txt` & `HuggingMouse-0.2.0/docs/_build/html/_sources/autoapi/HuggingMouse/utils/index.rst.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_static/alabaster.css` & `HuggingMouse-0.2.0/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_static/basic.css` & `HuggingMouse-0.2.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_static/doctools.js` & `HuggingMouse-0.2.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_static/language_data.js` & `HuggingMouse-0.2.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_static/pygments.css` & `HuggingMouse-0.2.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_static/searchtools.js` & `HuggingMouse-0.2.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/_static/sphinx_highlight.js` & `HuggingMouse-0.2.0/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/allen_api_utilities/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/allen_api_utilities/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/analyzer/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/analyzer/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/exceptions/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/exceptions/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/get_config_params/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/get_config_params/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/make_embeddings/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/make_embeddings/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/regressors/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/regressors/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/trial_averaged_data/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/trial_averaged_data/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/utils/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/utils/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/HuggingMouse/visualizers/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/HuggingMouse/visualizers/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/autoapi/index.html` & `HuggingMouse-0.2.0/docs/_build/html/autoapi/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/genindex.html` & `HuggingMouse-0.2.0/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/index.html` & `HuggingMouse-0.2.0/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/objects.inv` & `HuggingMouse-0.2.0/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/py-modindex.html` & `HuggingMouse-0.2.0/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/search.html` & `HuggingMouse-0.2.0/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/html/searchindex.js` & `HuggingMouse-0.2.0/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/index.html` & `HuggingMouse-0.2.0/docs/_build/index.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/objects.inv` & `HuggingMouse-0.2.0/docs/_build/objects.inv`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/py-modindex.html` & `HuggingMouse-0.2.0/docs/_build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/search.html` & `HuggingMouse-0.2.0/docs/_build/search.html`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/_build/searchindex.js` & `HuggingMouse-0.2.0/docs/_build/searchindex.js`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/conf.py` & `HuggingMouse-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/docs/make.bat` & `HuggingMouse-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/infogan.png` & `HuggingMouse-0.2.0/infogan.png`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/logo_CC0.jpg` & `HuggingMouse-0.2.0/logo_CC0.jpg`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/logo_CC0_attention.jpg` & `HuggingMouse-0.2.0/logo_CC0_attention.jpg`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/scripts/dev_scripts/hacking_with_labels.py` & `HuggingMouse-0.2.0/scripts/dev_scripts/hacking_with_labels.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/scripts/dev_scripts/merged_data_df.csv` & `HuggingMouse-0.2.0/scripts/dev_scripts/merged_data_df.csv`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/scripts/dev_scripts/test.py` & `HuggingMouse-0.2.0/scripts/dev_scripts/test.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/scripts/example_script.py` & `HuggingMouse-0.2.0/scripts/example_script.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/scripts/example_script_pipelines.py` & `HuggingMouse-0.2.0/scripts/example_script_pipelines.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/scripts/get_hf_model_downloads_sorted.py` & `HuggingMouse-0.2.0/scripts/get_hf_model_downloads_sorted.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/scripts/sorted_models_downloads.json` & `HuggingMouse-0.2.0/scripts/sorted_models_downloads.json`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/setup.py` & `HuggingMouse-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 setup(name='HuggingMouse',
-      version='0.1.1',
+      version='0.2.0',
       description='Data analysis library for Allen Brain Observatory data',
       author='Maria Kesa',
       author_email='mariarosekesa@gmail.com',
       url='https://github.com/mariakesa/HuggingMouse',
       install_requires=[
           'scikit-learn==1.2.2',
           'torch==1.13.1',
```

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/allen_api_utilities.py` & `HuggingMouse-0.2.0/src/HuggingMouse/allen_api_utilities.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/custom_exceptions.py` & `HuggingMouse-0.2.0/src/HuggingMouse/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/make_embeddings.py` & `HuggingMouse-0.2.0/src/HuggingMouse/make_embeddings.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/pipelines/neuron_prediction.py` & `HuggingMouse-0.2.0/src/HuggingMouse/pipelines/neuron_prediction.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/pipelines/single_trial_fs.py` & `HuggingMouse-0.2.0/src/HuggingMouse/pipelines/single_trial_fs.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/regressors.py` & `HuggingMouse-0.2.0/src/HuggingMouse/regressors.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/trial_averaged_data.py` & `HuggingMouse-0.2.0/src/HuggingMouse/trial_averaged_data.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/utils.py` & `HuggingMouse-0.2.0/src/HuggingMouse/utils.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse/visualizers.py` & `HuggingMouse-0.2.0/src/HuggingMouse/visualizers.py`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/src/HuggingMouse.egg-info/SOURCES.txt` & `HuggingMouse-0.2.0/src/HuggingMouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/tutorial_notebooks/clip.ipynb` & `HuggingMouse-0.2.0/tutorial_notebooks/clip.ipynb`

 * *Files identical despite different names*

### Comparing `HuggingMouse-0.1.1/tutorial_notebooks/top_10.ipynb` & `HuggingMouse-0.2.0/tutorial_notebooks/top_10.ipynb`

 * *Files identical despite different names*

