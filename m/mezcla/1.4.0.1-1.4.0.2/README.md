# Comparing `tmp/mezcla-1.4.0.1.tar.gz` & `tmp/mezcla-1.4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.4.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mezcla-1.4.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mezcla-1.4.0.1.tar` & `mezcla-1.4.0.2.tar`

### file list

```diff
@@ -1,236 +1,239 @@
--rw-r--r--   0        0        0      542 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/.coveragerc
--rw-r--r--   0        0        0       67 2024-05-12 06:12:49.213578 mezcla-1.4.0.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      129 2024-05-12 06:12:49.213578 mezcla-1.4.0.1/.github/workflows/act-event.json
--rw-r--r--   0        0        0     3483 2024-05-12 06:12:49.213578 mezcla-1.4.0.1/.github/workflows/act.yml
--rw-r--r--   0        0        0     3955 2024-05-12 06:12:49.217578 mezcla-1.4.0.1/.github/workflows/debug.yml
--rw-r--r--   0        0        0      134 2024-05-12 06:12:49.217578 mezcla-1.4.0.1/.github/workflows/github-event.json
--rw-r--r--   0        0        0     3228 2024-05-12 06:12:49.217578 mezcla-1.4.0.1/.github/workflows/github.yml
--rw-r--r--   0        0        0      137 2024-05-12 06:12:49.217578 mezcla-1.4.0.1/.github/workflows/skip-docker.json
--rw-r--r--   0        0        0      137 2024-05-12 06:12:49.217578 mezcla-1.4.0.1/.github/workflows/use-docker.json
--rw-r--r--   0        0        0     2150 2024-05-12 06:12:49.217578 mezcla-1.4.0.1/.gitignore
--rw-r--r--   0        0        0     7007 2024-05-12 06:12:49.217578 mezcla-1.4.0.1/Dockerfile
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.4.0.1/LICENSE.txt
--rw-r--r--   0        0        0      881 2024-05-14 04:54:27.006918 mezcla-1.4.0.1/README.txt
--rw-r--r--   0        0        0      380 2023-06-01 22:36:35.000000 mezcla-1.4.0.1/TODO.txt
--rw-r--r--   0        0        0      250 2024-05-12 06:12:49.221578 mezcla-1.4.0.1/_temp-user-docker.env
--rw-r--r--   0        0        0      634 2024-05-12 06:13:34.837710 mezcla-1.4.0.1/docs/Makefile
--rw-r--r--   0        0        0     1085 2024-05-12 06:13:34.837710 mezcla-1.4.0.1/docs/conf.py
--rw-r--r--   0        0        0     4062 2024-05-12 06:13:34.837710 mezcla-1.4.0.1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-05-12 06:13:34.837710 mezcla-1.4.0.1/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2024-05-12 06:12:49.221578 mezcla-1.4.0.1/local-workflows.sh -> tools/local-workflows.sh
--rw-r--r--   0        0        0      265 2024-05-12 06:12:49.221578 mezcla-1.4.0.1/mezcla/TODO.md
--rwxr-xr-x   0        0        0     2294 2024-05-17 03:07:30.229237 mezcla-1.4.0.1/mezcla/__init__.py
--rwxr-xr-x   0        0        0     1358 2024-05-12 06:12:49.221578 mezcla-1.4.0.1/mezcla/__main__.py
--rwxr-xr-x   0        0        0        0 2024-05-12 06:13:34.837710 mezcla-1.4.0.1/mezcla/adhoc/__init__.py
--rwxr-xr-x   0        0        0    26129 2024-05-12 06:13:34.837710 mezcla-1.4.0.1/mezcla/adhoc/check_time_tracking.py
--rwxr-xr-x   0        0        0     3740 2024-05-12 06:12:49.221578 mezcla-1.4.0.1/mezcla/adhoc/tests/test_check_time_tracking.py
--rwxr-xr-x   0        0        0    10872 2024-05-12 06:12:49.225578 mezcla-1.4.0.1/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    18007 2024-05-12 06:12:49.225578 mezcla-1.4.0.1/mezcla/audio.py
--rwxr-xr-x   0        0        0     5051 2024-05-12 06:13:34.837710 mezcla-1.4.0.1/mezcla/bash_ast.py
--rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.000000 mezcla-1.4.0.1/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25718 2024-05-12 06:12:49.225578 mezcla-1.4.0.1/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     8307 2024-05-12 06:12:49.225578 mezcla-1.4.0.1/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     9241 2024-05-12 06:12:49.225578 mezcla-1.4.0.1/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14896 2024-05-12 06:12:49.229578 mezcla-1.4.0.1/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0     6040 2024-05-12 06:12:49.229578 mezcla-1.4.0.1/mezcla/convert_emoticons.py
--rwxr-xr-x   0        0        0    23141 2024-05-12 06:13:34.841710 mezcla-1.4.0.1/mezcla/cut.py
--rwxr-xr-x   0        0        0     4795 2024-05-12 06:12:49.229578 mezcla-1.4.0.1/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    52703 2024-05-14 04:54:27.010918 mezcla-1.4.0.1/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0     5033 2024-05-12 06:12:49.233578 mezcla-1.4.0.1/mezcla/evaluate_example_tests.py
--rwxr-xr-x   0        0        0        0 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12874 2024-05-12 06:12:49.233578 mezcla-1.4.0.1/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3644 2024-05-12 06:12:49.233578 mezcla-1.4.0.1/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/examples/download_user_gist.py
--rw-r--r--   0        0        0      118 2024-05-12 06:12:49.233578 mezcla-1.4.0.1/mezcla/examples/dummy-image.png
--rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.000000 mezcla-1.4.0.1/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.000000 mezcla-1.4.0.1/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8811 2024-05-12 06:12:49.233578 mezcla-1.4.0.1/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0    54141 2024-05-12 06:12:49.237578 mezcla-1.4.0.1/mezcla/examples/hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     4660 2024-05-12 06:12:49.237578 mezcla-1.4.0.1/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     6076 2024-05-12 06:13:34.841710 mezcla-1.4.0.1/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.4.0.1/mezcla/examples/iris.csv
--rwxr-xr-x   0        0        0     8645 2024-05-12 06:12:49.237578 mezcla-1.4.0.1/mezcla/examples/matrix_multiply_benchmarking.py
--rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.4.0.1/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.000000 mezcla-1.4.0.1/mezcla/examples/plot_forest_importances.py
--rw-r--r--   0        0        0       20 2024-05-12 06:12:49.237578 mezcla-1.4.0.1/mezcla/examples/resources/translate_es_1.txt
--rw-r--r--   0        0        0     1809 2024-05-12 06:12:49.237578 mezcla-1.4.0.1/mezcla/examples/resources/translate_es_25.txt
--rw-r--r--   0        0        0   105004 2024-05-12 06:12:49.241578 mezcla-1.4.0.1/mezcla/examples/resources/us1.wav
--rw-r--r--   0        0        0    89644 2024-05-12 06:12:49.245578 mezcla-1.4.0.1/mezcla/examples/resources/us10.wav
--rw-r--r--   0        0        0   159725 2024-05-12 06:12:49.245578 mezcla-1.4.0.1/mezcla/examples/sd-spooky-pacman.png
--rwxr-xr-x   0        0        0    13004 2024-05-12 06:12:49.245578 mezcla-1.4.0.1/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     2211 2024-05-12 06:12:49.249578 mezcla-1.4.0.1/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0     5462 2024-05-12 06:12:49.249578 mezcla-1.4.0.1/mezcla/examples/tests/template.py
--rwxr-xr-x   0        0        0    13881 2024-05-12 06:12:49.249578 mezcla-1.4.0.1/mezcla/examples/tests/test_hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     4608 2024-05-12 06:12:49.249578 mezcla-1.4.0.1/mezcla/examples/tests/test_hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     5783 2024-05-12 06:12:49.249578 mezcla-1.4.0.1/mezcla/examples/tests/test_hugging_face_translation.py
--rwxr-xr-x   0        0        0     3199 2024-05-12 06:12:49.249578 mezcla-1.4.0.1/mezcla/examples/tests/test_matrix_multiply_benchmarking.py
--rwxr-xr-x   0        0        0     3873 2024-05-12 06:12:49.249578 mezcla-1.4.0.1/mezcla/examples/tests/test_youtube_transcript.py
--rwxr-xr-x   0        0        0     3617 2024-05-12 06:12:49.249578 mezcla-1.4.0.1/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     3401 2024-05-12 06:12:49.253579 mezcla-1.4.0.1/mezcla/examples/youtube_transcript.py
--rwxr-xr-x   0        0        0     5645 2024-05-12 06:12:49.253579 mezcla-1.4.0.1/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     8648 2024-05-12 06:12:49.253579 mezcla-1.4.0.1/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.4.0.1/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     3073 2024-05-12 06:13:34.841710 mezcla-1.4.0.1/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32976 2024-05-12 06:12:49.253579 mezcla-1.4.0.1/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    42250 2024-05-14 04:54:27.010918 mezcla-1.4.0.1/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0     2231 2024-05-12 06:13:34.845710 mezcla-1.4.0.1/mezcla/gpu_utils.py
--rwxr-xr-x   0        0        0    51212 2024-05-12 06:12:49.257578 mezcla-1.4.0.1/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     5861 2024-05-12 06:12:49.257578 mezcla-1.4.0.1/mezcla/ipython_utils.py
--rwxr-xr-x   0        0        0     5718 2024-05-12 06:12:49.257578 mezcla-1.4.0.1/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17985 2024-05-12 06:12:49.257578 mezcla-1.4.0.1/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    16511 2024-05-14 04:54:27.010918 mezcla-1.4.0.1/mezcla/llm_desktop_search.py
--rwxr-xr-x   0        0        0    52863 2024-05-12 06:13:34.849710 mezcla-1.4.0.1/mezcla/main.py
--rwxr-xr-x   0        0        0     9307 2023-06-01 22:36:35.000000 mezcla-1.4.0.1/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11040 2024-05-12 06:12:49.261578 mezcla-1.4.0.1/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0      608 2024-05-12 06:12:49.261578 mezcla-1.4.0.1/mezcla/mezcla
--rwxr-xr-x   0        0        0    16908 2024-05-12 06:12:49.265578 mezcla-1.4.0.1/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0    10273 2024-05-12 06:12:49.265578 mezcla-1.4.0.1/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    24478 2024-05-12 06:12:49.265578 mezcla-1.4.0.1/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0     1323 2024-05-12 06:12:49.265578 mezcla-1.4.0.1/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31564 2024-05-12 06:12:49.265578 mezcla-1.4.0.1/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      915 2024-05-12 06:12:49.265578 mezcla-1.4.0.1/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     3202 2024-05-12 06:12:49.265578 mezcla-1.4.0.1/mezcla/python_ast.py
--rwxr-xr-x   0        0        0     7337 2024-05-12 06:13:34.849710 mezcla-1.4.0.1/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     9407 2024-05-12 06:13:34.849710 mezcla-1.4.0.1/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40735 2024-05-12 06:12:49.269579 mezcla-1.4.0.1/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39709 2024-05-12 06:12:49.269579 mezcla-1.4.0.1/mezcla/run_bert_classifier.py
--rw-r--r--   0        0        0    24045 2024-05-12 06:12:49.273579 mezcla-1.4.0.1/mezcla/samples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0    17400 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     2930 2024-05-12 06:12:49.273579 mezcla-1.4.0.1/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    22899 2024-05-12 06:12:49.273579 mezcla-1.4.0.1/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     3168 2024-05-12 06:12:49.273579 mezcla-1.4.0.1/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.4.0.1/mezcla/sys_version_info_hack.py
--rwxr-xr-x   0        0        0    56705 2024-05-17 02:55:02.855433 mezcla-1.4.0.1/mezcla/system.py
--rw-r--r--   0        0        0   908397 2024-05-12 06:12:49.289579 mezcla-1.4.0.1/mezcla/temp/compound_CID_3672.xml
--rwxr-xr-x   0        0        0     1124 2024-05-12 06:12:49.289579 mezcla-1.4.0.1/mezcla/temp/plot.py
--rwxr-xr-x   0        0        0    45776 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     6218 2024-05-12 06:12:49.289579 mezcla-1.4.0.1/mezcla/template.py
--rw-r--r--   0        0        0     7418 2024-05-12 06:12:49.289579 mezcla-1.4.0.1/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      140 2024-05-12 06:12:49.289579 mezcla-1.4.0.1/mezcla/tests/README.md
--rw-r--r--   0        0        0      462 2023-06-01 22:36:35.000000 mezcla-1.4.0.1/mezcla/tests/TODO.md
--rw-r--r--   0        0        0     1341 2024-05-12 06:12:49.289579 mezcla-1.4.0.1/mezcla/tests/adhoc-tests.batspp
--rwxr-xr-x   0        0        0     1900 2024-05-12 06:12:49.289579 mezcla-1.4.0.1/mezcla/tests/conftest.py
--rw-r--r--   0        0        0     1306 2024-05-12 06:12:49.293578 mezcla-1.4.0.1/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt
--rw-r--r--   0        0        0    21583 2024-05-12 06:12:49.293578 mezcla-1.4.0.1/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb
--rw-r--r--   0        0        0    28841 2024-05-12 06:12:49.293578 mezcla-1.4.0.1/mezcla/tests/jupyter/test_audio_py.ipynb
--rw-r--r--   0        0        0    44701 2024-05-12 06:12:49.293578 mezcla-1.4.0.1/mezcla/tests/jupyter/test_audio_py_experimental.ipynb
--rw-r--r--   0        0        0    23692 2024-05-12 06:12:49.293578 mezcla-1.4.0.1/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb
--rw-r--r--   0        0        0    29559 2024-05-12 06:12:49.297579 mezcla-1.4.0.1/mezcla/tests/jupyter/test_hugging_face_translation.ipynb
--rw-r--r--   0        0        0    58860 2024-05-12 06:12:49.297579 mezcla-1.4.0.1/mezcla/tests/jupyter/test_template.ipynb
--rw-r--r--   0        0        0     1176 2024-05-12 06:12:49.297579 mezcla-1.4.0.1/mezcla/tests/misc-tests.batspp
--rwxr-xr-x   0        0        0     3898 2024-05-12 06:12:49.297579 mezcla-1.4.0.1/mezcla/tests/misc_doctests.py
--rwxr-xr-x   0        0        0     3722 2024-05-12 06:13:34.853710 mezcla-1.4.0.1/mezcla/tests/misc_tests.py
--rw-r--r--   0        0        0      312 2024-05-12 06:12:49.297579 mezcla-1.4.0.1/mezcla/tests/regression.batspp
--rw-r--r--   0        0        0     1453 2024-05-12 06:12:49.297579 mezcla-1.4.0.1/mezcla/tests/resources/argentinian-attraction-snippets.txt
--rw-r--r--   0        0        0      810 2023-04-30 22:47:21.000000 mezcla-1.4.0.1/mezcla/tests/resources/cars-csv-len-3.txt
--rw-r--r--   0        0        0      113 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      602 2023-04-30 22:47:21.000000 mezcla-1.4.0.1/mezcla/tests/resources/cars-tsv-len-3.txt
--rw-r--r--   0        0        0      659 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      655 2023-04-30 22:47:21.000000 mezcla-1.4.0.1/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0   324207 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/resources/random-10pct-tweet-emotions.tsv
--rw-r--r--   0        0        0     1152 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0      415 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/resources/spell-py-ar.list
--rw-r--r--   0        0        0      391 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/resources/spell-py-en.list
--rw-r--r--   0        0        0      294 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/resources/spell-py-es.list
--rw-r--r--   0        0        0      472 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/resources/spell-py-ru.list
--rw-r--r--   0        0        0     2780 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/resources/test.arpa
--rwxr-xr-x   0        0        0    14631 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/resources/word-POS.freq
--rwxr-xr-x   0        0        0    11479 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/resources/word.freq
--rw-r--r--   0        0        0      254 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     6108 2024-05-14 04:54:27.014918 mezcla-1.4.0.1/mezcla/tests/template.py
--rwxr-xr-x   0        0        0     1766 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/test___init__.py
--rwxr-xr-x   0        0        0     5942 2024-05-12 06:12:49.309579 mezcla-1.4.0.1/mezcla/tests/test_audio.py
--rwxr-xr-x   0        0        0      969 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/test_bert_multi_classification.py
--rwxr-xr-x   0        0        0     2343 2024-05-12 06:12:49.313579 mezcla-1.4.0.1/mezcla/tests/test_bing_search.py
--rwxr-xr-x   0        0        0     7559 2024-05-12 06:12:49.313579 mezcla-1.4.0.1/mezcla/tests/test_compute_tfidf.py
--rwxr-xr-x   0        0        0     4681 2024-05-12 06:12:49.313579 mezcla-1.4.0.1/mezcla/tests/test_convert_emoticons.py
--rwxr-xr-x   0        0        0     2905 2023-04-30 22:47:21.000000 mezcla-1.4.0.1/mezcla/tests/test_cut.py
--rwxr-xr-x   0        0        0     2464 2023-04-30 22:47:21.000000 mezcla-1.4.0.1/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    17872 2024-05-12 06:12:49.313579 mezcla-1.4.0.1/mezcla/tests/test_debug.py
--rwxr-xr-x   0        0        0     2654 2024-05-12 06:12:49.313579 mezcla-1.4.0.1/mezcla/tests/test_evaluate_example_tests.py
--rwxr-xr-x   0        0        0     5469 2024-05-12 06:12:49.313579 mezcla-1.4.0.1/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4429 2023-06-01 22:36:35.000000 mezcla-1.4.0.1/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2939 2023-06-01 22:36:35.000000 mezcla-1.4.0.1/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0    19004 2024-05-12 06:12:49.313579 mezcla-1.4.0.1/mezcla/tests/test_format_profile.py
--rwxr-xr-x   0        0        0     3589 2024-05-12 06:12:49.317579 mezcla-1.4.0.1/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    20109 2024-05-12 06:13:34.853710 mezcla-1.4.0.1/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0     5162 2024-05-12 06:13:34.857710 mezcla-1.4.0.1/mezcla/tests/test_gpu_utils.py
--rwxr-xr-x   0        0        0    14480 2024-05-12 06:12:49.317579 mezcla-1.4.0.1/mezcla/tests/test_html_utils.py
--rwxr-xr-x   0        0        0     2023 2024-05-12 06:12:49.317579 mezcla-1.4.0.1/mezcla/tests/test_ipython_utils.py
--rwxr-xr-x   0        0        0    11821 2024-05-12 06:12:49.317579 mezcla-1.4.0.1/mezcla/tests/test_kenlm_example.py
--rwxr-xr-x   0        0        0     3473 2024-05-12 06:12:49.317579 mezcla-1.4.0.1/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0    10237 2024-05-14 04:54:27.014918 mezcla-1.4.0.1/mezcla/tests/test_llm_desktop_search.py
--rwxr-xr-x   0        0        0    10850 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_main.py
--rwxr-xr-x   0        0        0     2725 2023-06-01 22:36:35.000000 mezcla-1.4.0.1/mezcla/tests/test_merge_files.py
--rwxr-xr-x   0        0        0     1291 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     9528 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     4204 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_my_regex.py
--rwxr-xr-x   0        0        0     5098 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_ngram_tfidf.py
--rwxr-xr-x   0        0        0     1398 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_os_utils.py
--rwxr-xr-x   0        0        0     8297 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_pandas_sklearn.py
--rwxr-xr-x   0        0        0     1183 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_plot_utils.py
--rwxr-xr-x   0        0        0     2156 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_python_ast.py
--rwxr-xr-x   0        0        0     1735 2024-05-12 06:12:49.321579 mezcla-1.4.0.1/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2389 2024-05-12 06:12:49.325579 mezcla-1.4.0.1/mezcla/tests/test_rgb_color_name.py
--rwxr-xr-x   0        0        0      895 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/test_run_albert_classifier.py
--rwxr-xr-x   0        0        0      930 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/test_run_bert_classifier.py
--rwxr-xr-x   0        0        0     1602 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/test_show_bert_representation.py
--rwxr-xr-x   0        0        0     2372 2024-05-12 06:12:49.325579 mezcla-1.4.0.1/mezcla/tests/test_simple_main_example.py
--rwxr-xr-x   0        0        0     5511 2024-05-12 06:12:49.325579 mezcla-1.4.0.1/mezcla/tests/test_spacy_nlp.py
--rwxr-xr-x   0        0        0    13977 2024-05-12 06:12:49.325579 mezcla-1.4.0.1/mezcla/tests/test_spell.py
--rwxr-xr-x   0        0        0      882 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    36834 2024-05-12 06:12:49.325579 mezcla-1.4.0.1/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     2231 2024-05-12 06:12:49.325579 mezcla-1.4.0.1/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     6015 2024-05-12 06:12:49.325579 mezcla-1.4.0.1/mezcla/tests/test_text_categorizer.py
--rwxr-xr-x   0        0        0    11593 2024-05-12 06:13:34.857710 mezcla-1.4.0.1/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7361 2024-05-12 06:12:49.329579 mezcla-1.4.0.1/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    28922 2024-05-12 06:12:49.329579 mezcla-1.4.0.1/mezcla/tests/test_tpo_common.py
--rwxr-xr-x   0        0        0      715 2023-04-30 22:44:00.000000 mezcla-1.4.0.1/mezcla/tests/test_train_language_model.py
--rwxr-xr-x   0        0        0     2041 2024-05-12 06:12:49.329579 mezcla-1.4.0.1/mezcla/tests/test_train_text_categorizer.py
--rwxr-xr-x   0        0        0     4172 2024-05-12 06:12:49.329579 mezcla-1.4.0.1/mezcla/tests/test_transpose_data.py
--rw-r--r--   0        0        0      435 2024-05-12 06:12:49.329579 mezcla-1.4.0.1/mezcla/tests/test_transpose_lines.input
--rwxr-xr-x   0        0        0     7214 2024-05-12 06:13:34.857710 mezcla-1.4.0.1/mezcla/tests/test_unittest_wrapper.py
--rwxr-xr-x   0        0        0     2355 2024-05-12 06:12:49.329579 mezcla-1.4.0.1/mezcla/tests/test_xml_utils.py
--rwxr-xr-x   0        0        0      676 2023-06-17 22:30:28.000000 mezcla-1.4.0.1/mezcla/tests/tfidf/test_corpus.py
--rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.4.0.1/mezcla/tests/tfidf/test_dockeyword.py
--rwxr-xr-x   0        0        0      688 2023-06-17 22:30:28.000000 mezcla-1.4.0.1/mezcla/tests/tfidf/test_document.py
--rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.4.0.1/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    36563 2024-05-12 06:12:49.333579 mezcla-1.4.0.1/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    28563 2024-05-12 06:12:49.333579 mezcla-1.4.0.1/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    13236 2024-05-12 06:12:49.333579 mezcla-1.4.0.1/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2024-05-12 06:12:49.333579 mezcla-1.4.0.1/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0      777 2024-05-12 06:12:49.333579 mezcla-1.4.0.1/mezcla/tfidf/config.py
--rwxr-xr-x   0        0        0    19427 2024-05-12 06:12:49.333579 mezcla-1.4.0.1/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     3146 2024-05-12 06:12:49.333579 mezcla-1.4.0.1/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7925 2024-05-12 06:12:49.337579 mezcla-1.4.0.1/mezcla/tfidf/document.py
--rwxr-xr-x   0        0        0    19704 2024-05-12 06:12:49.337579 mezcla-1.4.0.1/mezcla/tfidf/preprocess.py
--rw-r--r--   0        0        0     3961 2024-05-12 06:12:49.337579 mezcla-1.4.0.1/mezcla/tfidf/tests/misc_test.py
--rwxr-xr-x   0        0        0    60750 2024-05-12 06:12:49.337579 mezcla-1.4.0.1/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5272 2024-05-12 06:12:49.337579 mezcla-1.4.0.1/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5149 2024-05-12 06:12:49.341579 mezcla-1.4.0.1/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6673 2024-05-12 06:12:49.341579 mezcla-1.4.0.1/mezcla/transpose_data.py
--rwxr-xr-x   0        0        0    28787 2024-05-14 04:54:27.014918 mezcla-1.4.0.1/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.4.0.1/mezcla/xml_utils.py
--rw-r--r--   0        0        0      432 2024-05-12 06:12:49.341579 mezcla-1.4.0.1/non-binary-requirements.txt
--rw-r--r--   0        0        0      750 2024-05-12 06:13:34.857710 mezcla-1.4.0.1/packages-required.txt
--rw-r--r--   0        0        0      803 2024-05-17 03:07:30.229237 mezcla-1.4.0.1/pyproject.toml
--rw-r--r--   0        0        0     3936 2024-05-12 06:13:34.861710 mezcla-1.4.0.1/requirements.txt
-lrwxr-xr-x   0        0        0        0 2024-05-12 06:12:49.341579 mezcla-1.4.0.1/run_tests.bash -> tools/run_tests.bash
--rwxr-xr-x   0        0        0     1943 2024-05-17 03:07:30.229237 mezcla-1.4.0.1/setup.py
--rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.000000 mezcla-1.4.0.1/temp/simple_batspp.py
--rw-r--r--   0        0        0     1382 2024-05-12 06:12:49.341579 mezcla-1.4.0.1/tools/_temp_test_settings.bash
--rwxr-xr-x   0        0        0     3002 2024-05-12 06:12:49.345579 mezcla-1.4.0.1/tools/local-workflows.sh
--rwxr-xr-x   0        0        0     3770 2024-05-12 06:12:49.345579 mezcla-1.4.0.1/tools/run_tests.bash
--rw-r--r--   0        0        0      612 2023-06-01 22:36:35.000000 mezcla-1.4.0.1/tox.ini
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 mezcla-1.4.0.1/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/.coveragerc
+-rw-r--r--   0        0        0       67 2024-05-12 06:12:49.213578 mezcla-1.4.0.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      129 2024-05-12 06:12:49.213578 mezcla-1.4.0.2/.github/workflows/act-event.json
+-rw-r--r--   0        0        0     3483 2024-05-12 06:12:49.213578 mezcla-1.4.0.2/.github/workflows/act.yml
+-rw-r--r--   0        0        0     3955 2024-05-12 06:12:49.217578 mezcla-1.4.0.2/.github/workflows/debug.yml
+-rw-r--r--   0        0        0      134 2024-05-12 06:12:49.217578 mezcla-1.4.0.2/.github/workflows/github-event.json
+-rw-r--r--   0        0        0     3228 2024-05-12 06:12:49.217578 mezcla-1.4.0.2/.github/workflows/github.yml
+-rw-r--r--   0        0        0      137 2024-05-12 06:12:49.217578 mezcla-1.4.0.2/.github/workflows/skip-docker.json
+-rw-r--r--   0        0        0      137 2024-05-12 06:12:49.217578 mezcla-1.4.0.2/.github/workflows/use-docker.json
+-rw-r--r--   0        0        0     2150 2024-05-12 06:12:49.217578 mezcla-1.4.0.2/.gitignore
+-rw-r--r--   0        0        0     7007 2024-05-12 06:12:49.217578 mezcla-1.4.0.2/Dockerfile
+-rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.000000 mezcla-1.4.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      881 2024-05-14 04:54:27.006918 mezcla-1.4.0.2/README.txt
+-rw-r--r--   0        0        0      380 2023-06-01 22:36:35.000000 mezcla-1.4.0.2/TODO.txt
+-rw-r--r--   0        0        0      250 2024-05-12 06:12:49.221578 mezcla-1.4.0.2/_temp-user-docker.env
+-rw-r--r--   0        0        0      634 2024-05-12 06:13:34.837710 mezcla-1.4.0.2/docs/Makefile
+-rw-r--r--   0        0        0     1085 2024-05-12 06:13:34.837710 mezcla-1.4.0.2/docs/conf.py
+-rw-r--r--   0        0        0     4062 2024-05-12 06:13:34.837710 mezcla-1.4.0.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-12 06:13:34.837710 mezcla-1.4.0.2/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2024-05-12 06:12:49.221578 mezcla-1.4.0.2/local-workflows.sh -> tools/local-workflows.sh
+-rw-r--r--   0        0        0      458 2024-05-31 10:53:30.979964 mezcla-1.4.0.2/mezcla/TODO.md
+-rwxr-xr-x   0        0        0     2339 2024-06-01 18:34:07.418780 mezcla-1.4.0.2/mezcla/__init__.py
+-rwxr-xr-x   0        0        0     1358 2024-05-12 06:12:49.221578 mezcla-1.4.0.2/mezcla/__main__.py
+-rwxr-xr-x   0        0        0        0 2024-05-12 06:13:34.837710 mezcla-1.4.0.2/mezcla/adhoc/__init__.py
+-rwxr-xr-x   0        0        0    26240 2024-05-26 19:57:29.101506 mezcla-1.4.0.2/mezcla/adhoc/check_time_tracking.py
+-rw-r--r--   0        0        0        0 2024-05-20 04:28:05.690881 mezcla-1.4.0.2/mezcla/adhoc/tests/__init__.py
+-rwxr-xr-x   0        0        0     3772 2024-05-20 04:44:42.349075 mezcla-1.4.0.2/mezcla/adhoc/tests/test_check_time_tracking.py
+-rwxr-xr-x   0        0        0    10872 2024-05-12 06:12:49.225578 mezcla-1.4.0.2/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    18007 2024-05-12 06:12:49.225578 mezcla-1.4.0.2/mezcla/audio.py
+-rwxr-xr-x   0        0        0     5051 2024-05-12 06:13:34.837710 mezcla-1.4.0.2/mezcla/bash_ast.py
+-rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.000000 mezcla-1.4.0.2/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25718 2024-05-12 06:12:49.225578 mezcla-1.4.0.2/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     8307 2024-05-12 06:12:49.225578 mezcla-1.4.0.2/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     9241 2024-05-12 06:12:49.225578 mezcla-1.4.0.2/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14896 2024-05-12 06:12:49.229578 mezcla-1.4.0.2/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0     6040 2024-05-12 06:12:49.229578 mezcla-1.4.0.2/mezcla/convert_emoticons.py
+-rwxr-xr-x   0        0        0    23141 2024-05-12 06:13:34.841710 mezcla-1.4.0.2/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4795 2024-05-12 06:12:49.229578 mezcla-1.4.0.2/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    52703 2024-05-30 20:35:14.365587 mezcla-1.4.0.2/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0     5033 2024-05-12 06:12:49.233578 mezcla-1.4.0.2/mezcla/evaluate_example_tests.py
+-rwxr-xr-x   0        0        0        0 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12874 2024-05-12 06:12:49.233578 mezcla-1.4.0.2/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3644 2024-05-12 06:12:49.233578 mezcla-1.4.0.2/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/examples/download_user_gist.py
+-rw-r--r--   0        0        0      118 2024-05-12 06:12:49.233578 mezcla-1.4.0.2/mezcla/examples/dummy-image.png
+-rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.000000 mezcla-1.4.0.2/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.000000 mezcla-1.4.0.2/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8811 2024-05-12 06:12:49.233578 mezcla-1.4.0.2/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0    54141 2024-05-12 06:12:49.237578 mezcla-1.4.0.2/mezcla/examples/hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     4660 2024-05-12 06:12:49.237578 mezcla-1.4.0.2/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     6076 2024-05-12 06:13:34.841710 mezcla-1.4.0.2/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.4.0.2/mezcla/examples/iris.csv
+-rwxr-xr-x   0        0        0     8645 2024-05-12 06:12:49.237578 mezcla-1.4.0.2/mezcla/examples/matrix_multiply_benchmarking.py
+-rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.4.0.2/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.000000 mezcla-1.4.0.2/mezcla/examples/plot_forest_importances.py
+-rw-r--r--   0        0        0       20 2024-05-12 06:12:49.237578 mezcla-1.4.0.2/mezcla/examples/resources/translate_es_1.txt
+-rw-r--r--   0        0        0     1809 2024-05-12 06:12:49.237578 mezcla-1.4.0.2/mezcla/examples/resources/translate_es_25.txt
+-rw-r--r--   0        0        0   105004 2024-05-12 06:12:49.241578 mezcla-1.4.0.2/mezcla/examples/resources/us1.wav
+-rw-r--r--   0        0        0    89644 2024-05-12 06:12:49.245578 mezcla-1.4.0.2/mezcla/examples/resources/us10.wav
+-rw-r--r--   0        0        0   159725 2024-05-12 06:12:49.245578 mezcla-1.4.0.2/mezcla/examples/sd-spooky-pacman.png
+-rwxr-xr-x   0        0        0    13004 2024-05-12 06:12:49.245578 mezcla-1.4.0.2/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     2211 2024-05-12 06:12:49.249578 mezcla-1.4.0.2/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/examples/tensorflow_matrix_multiply.py
+-rw-r--r--   0        0        0        0 2024-05-20 02:22:11.877351 mezcla-1.4.0.2/mezcla/examples/tests/__init__.py
+-rwxr-xr-x   0        0        0     6126 2024-05-30 20:50:07.276729 mezcla-1.4.0.2/mezcla/examples/tests/template.py
+-rwxr-xr-x   0        0        0    13881 2024-05-12 06:12:49.249578 mezcla-1.4.0.2/mezcla/examples/tests/test_hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     4608 2024-05-12 06:12:49.249578 mezcla-1.4.0.2/mezcla/examples/tests/test_hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     5783 2024-05-12 06:12:49.249578 mezcla-1.4.0.2/mezcla/examples/tests/test_hugging_face_translation.py
+-rwxr-xr-x   0        0        0     3248 2024-05-30 22:59:38.591586 mezcla-1.4.0.2/mezcla/examples/tests/test_matrix_multiply_benchmarking.py
+-rwxr-xr-x   0        0        0     3873 2024-05-12 06:12:49.249578 mezcla-1.4.0.2/mezcla/examples/tests/test_youtube_transcript.py
+-rwxr-xr-x   0        0        0     3617 2024-05-12 06:12:49.249578 mezcla-1.4.0.2/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     3401 2024-05-12 06:12:49.253579 mezcla-1.4.0.2/mezcla/examples/youtube_transcript.py
+-rwxr-xr-x   0        0        0     5645 2024-05-12 06:12:49.253579 mezcla-1.4.0.2/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     8648 2024-05-12 06:12:49.253579 mezcla-1.4.0.2/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.4.0.2/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     3073 2024-05-12 06:13:34.841710 mezcla-1.4.0.2/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32976 2024-05-12 06:12:49.253579 mezcla-1.4.0.2/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    42558 2024-05-30 21:50:27.821644 mezcla-1.4.0.2/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0     2231 2024-05-12 06:13:34.845710 mezcla-1.4.0.2/mezcla/gpu_utils.py
+-rwxr-xr-x   0        0        0    51212 2024-05-12 06:12:49.257578 mezcla-1.4.0.2/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     5861 2024-05-12 06:12:49.257578 mezcla-1.4.0.2/mezcla/ipython_utils.py
+-rwxr-xr-x   0        0        0     5718 2024-05-12 06:12:49.257578 mezcla-1.4.0.2/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17985 2024-05-12 06:12:49.257578 mezcla-1.4.0.2/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    16511 2024-05-14 04:54:27.010918 mezcla-1.4.0.2/mezcla/llm_desktop_search.py
+-rwxr-xr-x   0        0        0    53055 2024-05-30 22:28:07.309002 mezcla-1.4.0.2/mezcla/main.py
+-rwxr-xr-x   0        0        0     9307 2023-06-01 22:36:35.000000 mezcla-1.4.0.2/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11040 2024-05-12 06:12:49.261578 mezcla-1.4.0.2/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0      608 2024-05-12 06:12:49.261578 mezcla-1.4.0.2/mezcla/mezcla
+-rwxr-xr-x   0        0        0    16908 2024-05-12 06:12:49.265578 mezcla-1.4.0.2/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0    10554 2024-05-30 20:41:15.702907 mezcla-1.4.0.2/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    24537 2024-05-18 18:02:24.765459 mezcla-1.4.0.2/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0     1323 2024-05-12 06:12:49.265578 mezcla-1.4.0.2/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31564 2024-05-12 06:12:49.265578 mezcla-1.4.0.2/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      915 2024-05-12 06:12:49.265578 mezcla-1.4.0.2/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     3202 2024-05-12 06:12:49.265578 mezcla-1.4.0.2/mezcla/python_ast.py
+-rwxr-xr-x   0        0        0     7337 2024-05-12 06:13:34.849710 mezcla-1.4.0.2/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     9407 2024-05-12 06:13:34.849710 mezcla-1.4.0.2/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40735 2024-05-12 06:12:49.269579 mezcla-1.4.0.2/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39709 2024-05-12 06:12:49.269579 mezcla-1.4.0.2/mezcla/run_bert_classifier.py
+-rw-r--r--   0        0        0    24045 2024-05-12 06:12:49.273579 mezcla-1.4.0.2/mezcla/samples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0    17400 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     2930 2024-05-12 06:12:49.273579 mezcla-1.4.0.2/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    22899 2024-05-12 06:12:49.273579 mezcla-1.4.0.2/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3168 2024-05-12 06:12:49.273579 mezcla-1.4.0.2/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.4.0.2/mezcla/sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    57638 2024-05-30 21:51:12.953806 mezcla-1.4.0.2/mezcla/system.py
+-rw-r--r--   0        0        0   908397 2024-05-12 06:12:49.289579 mezcla-1.4.0.2/mezcla/temp/compound_CID_3672.xml
+-rwxr-xr-x   0        0        0     1124 2024-05-12 06:12:49.289579 mezcla-1.4.0.2/mezcla/temp/plot.py
+-rwxr-xr-x   0        0        0    45776 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     6191 2024-05-30 21:52:27.730072 mezcla-1.4.0.2/mezcla/template.py
+-rw-r--r--   0        0        0     7418 2024-05-12 06:12:49.289579 mezcla-1.4.0.2/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      140 2024-05-12 06:12:49.289579 mezcla-1.4.0.2/mezcla/tests/README.md
+-rw-r--r--   0        0        0      462 2023-06-01 22:36:35.000000 mezcla-1.4.0.2/mezcla/tests/TODO.md
+-rw-r--r--   0        0        0        0 2024-05-20 04:27:26.070743 mezcla-1.4.0.2/mezcla/tests/__init__.py
+-rw-r--r--   0        0        0     1341 2024-05-12 06:12:49.289579 mezcla-1.4.0.2/mezcla/tests/adhoc-tests.batspp
+-rwxr-xr-x   0        0        0     1900 2024-05-12 06:12:49.289579 mezcla-1.4.0.2/mezcla/tests/conftest.py
+-rw-r--r--   0        0        0     1306 2024-05-12 06:12:49.293578 mezcla-1.4.0.2/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt
+-rw-r--r--   0        0        0    21583 2024-05-12 06:12:49.293578 mezcla-1.4.0.2/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb
+-rw-r--r--   0        0        0    28841 2024-05-12 06:12:49.293578 mezcla-1.4.0.2/mezcla/tests/jupyter/test_audio_py.ipynb
+-rw-r--r--   0        0        0    44701 2024-05-12 06:12:49.293578 mezcla-1.4.0.2/mezcla/tests/jupyter/test_audio_py_experimental.ipynb
+-rw-r--r--   0        0        0    23692 2024-05-12 06:12:49.293578 mezcla-1.4.0.2/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb
+-rw-r--r--   0        0        0    29559 2024-05-12 06:12:49.297579 mezcla-1.4.0.2/mezcla/tests/jupyter/test_hugging_face_translation.ipynb
+-rw-r--r--   0        0        0    58860 2024-05-12 06:12:49.297579 mezcla-1.4.0.2/mezcla/tests/jupyter/test_template.ipynb
+-rw-r--r--   0        0        0     1176 2024-05-12 06:12:49.297579 mezcla-1.4.0.2/mezcla/tests/misc-tests.batspp
+-rwxr-xr-x   0        0        0     3898 2024-05-12 06:12:49.297579 mezcla-1.4.0.2/mezcla/tests/misc_doctests.py
+-rwxr-xr-x   0        0        0     3722 2024-05-12 06:13:34.853710 mezcla-1.4.0.2/mezcla/tests/misc_tests.py
+-rw-r--r--   0        0        0      312 2024-05-12 06:12:49.297579 mezcla-1.4.0.2/mezcla/tests/regression.batspp
+-rw-r--r--   0        0        0     1453 2024-05-12 06:12:49.297579 mezcla-1.4.0.2/mezcla/tests/resources/argentinian-attraction-snippets.txt
+-rw-r--r--   0        0        0      810 2023-04-30 22:47:21.000000 mezcla-1.4.0.2/mezcla/tests/resources/cars-csv-len-3.txt
+-rw-r--r--   0        0        0      113 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      602 2023-04-30 22:47:21.000000 mezcla-1.4.0.2/mezcla/tests/resources/cars-tsv-len-3.txt
+-rw-r--r--   0        0        0      659 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      655 2023-04-30 22:47:21.000000 mezcla-1.4.0.2/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0   324207 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/resources/random-10pct-tweet-emotions.tsv
+-rw-r--r--   0        0        0     1152 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0      415 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/resources/spell-py-ar.list
+-rw-r--r--   0        0        0      391 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/resources/spell-py-en.list
+-rw-r--r--   0        0        0      294 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/resources/spell-py-es.list
+-rw-r--r--   0        0        0      472 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/resources/spell-py-ru.list
+-rw-r--r--   0        0        0     2780 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/resources/test.arpa
+-rwxr-xr-x   0        0        0    14631 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/resources/word-POS.freq
+-rwxr-xr-x   0        0        0    11479 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/resources/word.freq
+-rw-r--r--   0        0        0      254 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     6066 2024-05-31 10:54:07.884092 mezcla-1.4.0.2/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     1766 2024-05-12 06:12:49.309579 mezcla-1.4.0.2/mezcla/tests/test___init__.py
+-rwxr-xr-x   0        0        0     6108 2024-05-31 10:55:57.216472 mezcla-1.4.0.2/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0     2343 2024-05-12 06:12:49.313579 mezcla-1.4.0.2/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     7559 2024-05-12 06:12:49.313579 mezcla-1.4.0.2/mezcla/tests/test_compute_tfidf.py
+-rwxr-xr-x   0        0        0     4681 2024-05-12 06:12:49.313579 mezcla-1.4.0.2/mezcla/tests/test_convert_emoticons.py
+-rwxr-xr-x   0        0        0     2905 2023-04-30 22:47:21.000000 mezcla-1.4.0.2/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2464 2023-04-30 22:47:21.000000 mezcla-1.4.0.2/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    17872 2024-05-12 06:12:49.313579 mezcla-1.4.0.2/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     2654 2024-05-12 06:12:49.313579 mezcla-1.4.0.2/mezcla/tests/test_evaluate_example_tests.py
+-rwxr-xr-x   0        0        0     5469 2024-05-12 06:12:49.313579 mezcla-1.4.0.2/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4429 2023-06-01 22:36:35.000000 mezcla-1.4.0.2/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2939 2023-06-01 22:36:35.000000 mezcla-1.4.0.2/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0    19004 2024-05-12 06:12:49.313579 mezcla-1.4.0.2/mezcla/tests/test_format_profile.py
+-rwxr-xr-x   0        0        0     3589 2024-05-12 06:12:49.317579 mezcla-1.4.0.2/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    20109 2024-05-12 06:13:34.853710 mezcla-1.4.0.2/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0     5162 2024-05-12 06:13:34.857710 mezcla-1.4.0.2/mezcla/tests/test_gpu_utils.py
+-rwxr-xr-x   0        0        0    14480 2024-05-12 06:12:49.317579 mezcla-1.4.0.2/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0     2023 2024-05-12 06:12:49.317579 mezcla-1.4.0.2/mezcla/tests/test_ipython_utils.py
+-rwxr-xr-x   0        0        0    11821 2024-05-12 06:12:49.317579 mezcla-1.4.0.2/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     3473 2024-05-12 06:12:49.317579 mezcla-1.4.0.2/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0    10237 2024-05-14 04:54:27.014918 mezcla-1.4.0.2/mezcla/tests/test_llm_desktop_search.py
+-rwxr-xr-x   0        0        0    10850 2024-05-12 06:12:49.321579 mezcla-1.4.0.2/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2725 2023-06-01 22:36:35.000000 mezcla-1.4.0.2/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     9528 2024-05-12 06:12:49.321579 mezcla-1.4.0.2/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     4204 2024-05-12 06:12:49.321579 mezcla-1.4.0.2/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0     5098 2024-05-12 06:12:49.321579 mezcla-1.4.0.2/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0     1407 2024-05-20 01:30:38.381725 mezcla-1.4.0.2/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8663 2024-05-30 21:56:29.266924 mezcla-1.4.0.2/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0     1183 2024-05-12 06:12:49.321579 mezcla-1.4.0.2/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0     2156 2024-05-12 06:12:49.321579 mezcla-1.4.0.2/mezcla/tests/test_python_ast.py
+-rwxr-xr-x   0        0        0     1735 2024-05-12 06:12:49.321579 mezcla-1.4.0.2/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2389 2024-05-12 06:12:49.325579 mezcla-1.4.0.2/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0     2372 2024-05-12 06:12:49.325579 mezcla-1.4.0.2/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     5511 2024-05-12 06:12:49.325579 mezcla-1.4.0.2/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0    14186 2024-05-31 10:56:10.448518 mezcla-1.4.0.2/mezcla/tests/test_spell.py
+-rwxr-xr-x   0        0        0      882 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    37186 2024-05-18 18:39:51.125549 mezcla-1.4.0.2/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     2231 2024-05-12 06:12:49.325579 mezcla-1.4.0.2/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     6174 2024-05-20 01:31:35.793905 mezcla-1.4.0.2/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0    11767 2024-06-01 18:14:33.079399 mezcla-1.4.0.2/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7361 2024-05-12 06:12:49.329579 mezcla-1.4.0.2/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    28922 2024-05-12 06:12:49.329579 mezcla-1.4.0.2/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2023-04-30 22:44:00.000000 mezcla-1.4.0.2/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0     2041 2024-05-12 06:12:49.329579 mezcla-1.4.0.2/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0     4172 2024-05-12 06:12:49.329579 mezcla-1.4.0.2/mezcla/tests/test_transpose_data.py
+-rw-r--r--   0        0        0      435 2024-05-12 06:12:49.329579 mezcla-1.4.0.2/mezcla/tests/test_transpose_lines.input
+-rwxr-xr-x   0        0        0     9455 2024-05-30 20:48:53.756482 mezcla-1.4.0.2/mezcla/tests/test_unittest_wrapper.py
+-rwxr-xr-x   0        0        0     2355 2024-05-12 06:12:49.329579 mezcla-1.4.0.2/mezcla/tests/test_xml_utils.py
+-rwxr-xr-x   0        0        0      676 2023-06-17 22:30:28.000000 mezcla-1.4.0.2/mezcla/tests/tfidf/test_corpus.py
+-rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.4.0.2/mezcla/tests/tfidf/test_dockeyword.py
+-rwxr-xr-x   0        0        0      688 2023-06-17 22:30:28.000000 mezcla-1.4.0.2/mezcla/tests/tfidf/test_document.py
+-rwxr-xr-x   0        0        0      697 2023-06-17 22:30:28.000000 mezcla-1.4.0.2/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    36563 2024-05-12 06:12:49.333579 mezcla-1.4.0.2/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    28563 2024-05-12 06:12:49.333579 mezcla-1.4.0.2/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    13236 2024-05-12 06:12:49.333579 mezcla-1.4.0.2/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2024-05-12 06:12:49.333579 mezcla-1.4.0.2/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0      777 2024-05-12 06:12:49.333579 mezcla-1.4.0.2/mezcla/tfidf/config.py
+-rwxr-xr-x   0        0        0    19427 2024-05-12 06:12:49.333579 mezcla-1.4.0.2/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     3146 2024-05-12 06:12:49.333579 mezcla-1.4.0.2/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7925 2024-05-12 06:12:49.337579 mezcla-1.4.0.2/mezcla/tfidf/document.py
+-rwxr-xr-x   0        0        0    19704 2024-05-12 06:12:49.337579 mezcla-1.4.0.2/mezcla/tfidf/preprocess.py
+-rw-r--r--   0        0        0     3961 2024-05-12 06:12:49.337579 mezcla-1.4.0.2/mezcla/tfidf/tests/misc_test.py
+-rwxr-xr-x   0        0        0    60750 2024-05-12 06:12:49.337579 mezcla-1.4.0.2/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5272 2024-05-12 06:12:49.337579 mezcla-1.4.0.2/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5149 2024-05-12 06:12:49.341579 mezcla-1.4.0.2/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6673 2024-05-12 06:12:49.341579 mezcla-1.4.0.2/mezcla/transpose_data.py
+-rwxr-xr-x   0        0        0    29330 2024-05-30 21:54:05.406417 mezcla-1.4.0.2/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.4.0.2/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      432 2024-05-12 06:12:49.341579 mezcla-1.4.0.2/non-binary-requirements.txt
+-rw-r--r--   0        0        0      750 2024-05-12 06:13:34.857710 mezcla-1.4.0.2/packages-required.txt
+-rw-r--r--   0        0        0      803 2024-06-01 18:34:07.418780 mezcla-1.4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3948 2024-05-31 10:51:57.791641 mezcla-1.4.0.2/requirements.txt
+lrwxr-xr-x   0        0        0        0 2024-05-12 06:12:49.341579 mezcla-1.4.0.2/run_tests.bash -> tools/run_tests.bash
+-rwxr-xr-x   0        0        0     1943 2024-06-01 18:34:07.418780 mezcla-1.4.0.2/setup.py
+-rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.000000 mezcla-1.4.0.2/temp/simple_batspp.py
+-rw-r--r--   0        0        0     1431 2024-05-20 04:44:21.869023 mezcla-1.4.0.2/tools/_temp_test_settings.bash
+-rwxr-xr-x   0        0        0     3002 2024-05-12 06:12:49.345579 mezcla-1.4.0.2/tools/local-workflows.sh
+-rwxr-xr-x   0        0        0     3770 2024-05-12 06:12:49.345579 mezcla-1.4.0.2/tools/run_tests.bash
+-rw-r--r--   0        0        0      612 2023-06-01 22:36:35.000000 mezcla-1.4.0.2/tox.ini
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 mezcla-1.4.0.2/PKG-INFO
```

### Comparing `mezcla-1.4.0.1/.coveragerc` & `mezcla-1.4.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/.github/workflows/act.yml` & `mezcla-1.4.0.2/.github/workflows/act.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/.github/workflows/debug.yml` & `mezcla-1.4.0.2/.github/workflows/debug.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/.github/workflows/github.yml` & `mezcla-1.4.0.2/.github/workflows/github.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/.gitignore` & `mezcla-1.4.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/Dockerfile` & `mezcla-1.4.0.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/LICENSE.txt` & `mezcla-1.4.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/README.txt` & `mezcla-1.4.0.2/README.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/docs/Makefile` & `mezcla-1.4.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/docs/conf.py` & `mezcla-1.4.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/docs/index.rst` & `mezcla-1.4.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/docs/make.bat` & `mezcla-1.4.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/__init__.py` & `mezcla-1.4.0.2/mezcla/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,21 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-version = "1.4.0.1"
+version = "1.4.0.2"
 __VERSION__ = version
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Note: requires python 3 or higher
 PYTHON3_PLUS = (sys.version_info[0] >= 3)
 assert PYTHON3_PLUS, "Python 3 or higher: ¡por favor!"
 
 # Local modules
 # Define most common imports for causual usage
```

### Comparing `mezcla-1.4.0.1/mezcla/__main__.py` & `mezcla-1.4.0.2/mezcla/__main__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/adhoc/check_time_tracking.py` & `mezcla-1.4.0.2/mezcla/adhoc/check_time_tracking.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                 system.print_stderr("Error: Discrepancy in hours at line {n}: change {spec} => {calc}?".format(n=line_num, spec=specified_hours, calc=hours))
             else:
                 # HACK: pretend user specified tabulated hours (TODO: use 'hours' in weekly_hours update below for clarity)
                 ## OLD: specified_hours = hours
                 pass
             ## OLD: weekly_hours += specified_hours
             weekly_hours += hours
-            debug.assertion((weekday_hours[day_of_week] == ""), "Missing weekly-hours lines?")
+            debug.assertion((weekday_hours[day_of_week] == ""), f"Missing weekly-hours lines (near line {line_num})?")
             ## OLD: weekday_hours[day_of_week] = specified_hours
             ## OLD2: weekday_hours[day_of_week] = hours
             weekday_hours[day_of_week] += ("" if not weekday_hours[day_of_week] else "-or-")
             weekday_hours[day_of_week] += str(hours)
             last_hours = hours
             hours = 0
             debug.trace_fmt(7, "spec_hours={sh} daily_hours={h} weekly_hours={wh} total_hours={th}, weekday_hours={wdh}", 
@@ -306,15 +306,15 @@
         # Check for day of week
         # NOTE: 'day' now stripped above.
         # TODO: make sure 'day' not included in first regex group
         ## if (my_re.search(r"^(\S+)(day)?:\s*$", line)):
         ## OLD: if (my_re.search(r"^(\S+)(day)?:\s*$", line)):
         elif (my_re.search(r"^(\S+)(day)?:\s*$", line)):
             day_of_week = my_re.group(1)
-            debug.assertion(len(day_of_week) == 3)
+            debug.assertion(len(day_of_week) == 3, f"Bad day of week at line {line_num}")
             debug.trace(6, f"day of week check: day={day_of_week}")
             ## TODO: handle Saturday and Wednesday
             ## TODO: day_of_week = re.sub(r"(ur|nes)?day$", "", my_re.group(1))
             if (day_of_week in ALL_WEEKDAYS):
                 if (hours > 0):
                     system.print_stderr("Error: missing 'hours:' line at line {n}".format(n=line_num))
             else:
@@ -383,15 +383,15 @@
                 system.print_stderr("Error: Discrepancy in hours at line {n}: change {spec} => {calc}?".format(n=line_num, spec=specified_hours, calc=hours))
             else:
                 # HACK: pretend user specified tabulated hours (TODO: use 'hours' below for clarify)
                 ## specified_hours = hours
                 pass
             ## OLD: weekly_hours += specified_hours
             weekly_hours += hours
-            debug.assertion(weekday_hours[day_of_week] == "")
+            debug.assertion(weekday_hours[day_of_week] == "", f"Day of week already used at line {line_num}")
             ## OLD: weekday_hours[day_of_week] = specified_hours
             ## OLD2: weekday_hours[day_of_week] = hours
             weekday_hours[day_of_week] += ("" if not weekday_hours[day_of_week] else "-or-")
             weekday_hours[day_of_week] += str(hours)
             last_hours = hours
             hours = 0
             debug.trace_fmt(7, "spec_hours={sh} daily_hours={h} weekly_hours={wh} total_hours={th}, weekday_hours={wdh}",
```

### Comparing `mezcla-1.4.0.1/mezcla/adhoc/tests/test_check_time_tracking.py` & `mezcla-1.4.0.2/mezcla/adhoc/tests/test_check_time_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #    THE_MODULE:                        global module object
 #    TestIt.script_module:              path to file
 try:
     import mezcla.adhoc.check_time_tracking as THE_MODULE
 except:
     debug.assertion(False, "TODO1: FIXME")
     THE_MODULE = None
+debug.trace_expr(5, THE_MODULE)
 #
 # Note: sanity test for customization (TODO: remove if desired)
 if not my_re.search(__file__, r"\btemplate.py$"):
     debug.assertion("mezcla.template" not in str(THE_MODULE))
 
 TEMPLATE = """
     # Time tracking for work Jan 2222
```

### Comparing `mezcla-1.4.0.1/mezcla/analyze_tfidf.py` & `mezcla-1.4.0.2/mezcla/analyze_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/audio.py` & `mezcla-1.4.0.2/mezcla/audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/bash_ast.py` & `mezcla-1.4.0.2/mezcla/bash_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/bert_multi_classification.py` & `mezcla-1.4.0.2/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/bert_text_classification.py` & `mezcla-1.4.0.2/mezcla/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/bing_search.py` & `mezcla-1.4.0.2/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/check_html_javascript.py` & `mezcla-1.4.0.2/mezcla/check_html_javascript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/compute_tfidf.py` & `mezcla-1.4.0.2/mezcla/compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/convert_emoticons.py` & `mezcla-1.4.0.2/mezcla/convert_emoticons.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/cut.py` & `mezcla-1.4.0.2/mezcla/cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/data_utils.py` & `mezcla-1.4.0.2/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/debug.py` & `mezcla-1.4.0.2/mezcla/debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/docs/audio_uml.svg` & `mezcla-1.4.0.2/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/evaluate_example_tests.py` & `mezcla-1.4.0.2/mezcla/evaluate_example_tests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.4.0.2/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.4.0.2/mezcla/examples/brownlee_ml_metrics.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/consume_all_memory.py` & `mezcla-1.4.0.2/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/download_user_gist.py` & `mezcla-1.4.0.2/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/dump_checkpoints.py` & `mezcla-1.4.0.2/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/encoded-iris.csv` & `mezcla-1.4.0.2/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/feature_importance.py` & `mezcla-1.4.0.2/mezcla/examples/feature_importance.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.4.0.2/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/hf_stable_diffusion.py` & `mezcla-1.4.0.2/mezcla/examples/hf_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.4.0.2/mezcla/examples/hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/hugging_face_translation.py` & `mezcla-1.4.0.2/mezcla/examples/hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.4.0.2/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/iris.csv` & `mezcla-1.4.0.2/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/matrix_multiply_benchmarking.py` & `mezcla-1.4.0.2/mezcla/examples/matrix_multiply_benchmarking.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.4.0.2/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/plot_forest_importances.py` & `mezcla-1.4.0.2/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/resources/translate_es_25.txt` & `mezcla-1.4.0.2/mezcla/examples/resources/translate_es_25.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/resources/us1.wav` & `mezcla-1.4.0.2/mezcla/examples/resources/us1.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/resources/us10.wav` & `mezcla-1.4.0.2/mezcla/examples/resources/us10.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/sd-spooky-pacman.png` & `mezcla-1.4.0.2/mezcla/examples/sd-spooky-pacman.png`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.4.0.2/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/template.py` & `mezcla-1.4.0.2/mezcla/examples/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.4.0.2/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/tests/template.py` & `mezcla-1.4.0.2/mezcla/examples/tests/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,25 @@
 # - Fill out TODO's below. Use numbered tests to order (e.g., test_1_usage).
 # - * See test_python_ast.py for simple example of customization.
 # - TODO: If any of the setup/cleanup methods defined, make sure to invoke base
 #   (see examples below for setUp and tearDown).
 # - For debugging the tested script, the ALLOW_SUBCOMMAND_TRACING environment
 #   option shows tracing output normally suppressed by unittest_wrapper.py.
 # - This can be run as follows (e.g., from root of repo):
-#   $ pytest ./mezcla/examples/tests/test_<module>.py
+#   $ pytest ./mezcla/examples/tests/test_<module>.py#
+#
+# Warning:
+# - The use of run_script as in test_01_data_file is an older style of testing.
+#   It is better to directly invoke a helper class in the script that is independent
+#   of the Script class based on Main. (See an example of this, see python_ast.py
+#   and tests/tests_python_ast.py.)
+# - Moreover, debugging tests with run_script is complicated because a separate
+#   process is involved (e.g., with separate environment variables.)
+# - See discussion of SUB_DEBUG_LEVEL in unittest_wrapper.py for more info.
+# - TODO: Feel free to delete this warning as well as the related one below.
 #
 
 ## TODO1: [Warning] Make sure this template adhered to as much as possible. For,
 ## example, only delete todo comments not regular code, unless suggested in tip).
 ## In particular, it is critical that script_module gets initialized properly.
 
 """TODO: Tests for <module> module"""
@@ -35,20 +45,16 @@
 from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:                        global module object
 #    TestIt.script_module:              path to file
 ## TODO (vvv): insert new module name in commented out template teo lines below
 THE_MODULE = None         ## TODO: remove this line: avoids <module> syntax error in next)
- mezcla.
-import 
-## TODO: ## import <module> as THE_MODULE
-import 
+## import mezcla.examples.<module> as THE_MODULE   ## TODO: uncomment this line (<<<)
 ## TODO (^^^): use modified line above
-## TODO1: ## import mezcla.examples.<module> as THE_MODULE
 #
 # Note: sanity test for customization (TODO: remove if desired)
 if not my_re.search(__file__, r"\btemplate.py$"):
     debug.assertion("mezcla.template" not in str(THE_MODULE))
 
 ## TODO:
 ## # Environment options
@@ -89,52 +95,53 @@
     ##     # TODO: debug.trace_current_context(level=debug.QUITE_DETAILED)
     ##     return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     ## DEBUG: @trap_exception            # TODO: remove when debugged
     def test_01_data_file(self):
         """Tests run_script w/ data file"""
+        # Warning: see notes above about potential issues with run_script-based tests.
         debug.trace(4, f"TestIt.test_01_data_file(); self={self}")
         data = ["TODO1", "TODO2"]
         system.write_lines(self.temp_file, data)
         ## TODO: add use_stdin=True to following if no file argument
         output = self.run_script(options="", data_file=self.temp_file)
         self.do_assert(my_re.search(r"TODO-pattern", output.strip()))
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     ## DEBUG: @trap_exception            # TODO: remove when debugged
     def test_02_something_else(self):
         """Test for something_else: TODO..."""
         debug.trace(4, f"TestIt.test_02_something_else(); self={self}")
-        self.do_assert(False)
+        self.do_assert(False, "TODO: implement")
         ## ex: self.do_assert(THE_MODULE.TODO_function() == TODO_value)
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_03_whatever(self):
         """TODO: flesh out test for whatever (capsys-like)"""
-        debug.trace(4, f"TestIt2.test_03_whatever(); self={self}")
+        debug.trace(4, f"TestIt.test_03_whatever(); self={self}")
         THE_MODULE.TODO_whatever()
         captured = self.get_stderr()
         self.do_assert("whatever" in captured, "TODO_whatever trace")
         return
 
     ## TODO: optional cleanup methods
     ##
     ## def tearDown(self):
     ##     debug.trace(6, f"TestIt.tearDown(); self={self}")
-    ##     super().tearDownClass()
+    ##     super().tearDown()
     ##     ...
     ##     return
     ##
     ## @classmethod
     ## def tearDownClass(cls):
     ##     debug.trace(6, f"TestIt.tearDownClass(); cls={cls}")
-    ##     super().tearDown()
+    ##     super().tearDownClass()
     ##     ...
     ##     return
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
```

### Comparing `mezcla-1.4.0.1/mezcla/examples/tests/test_hf_stable_diffusion.py` & `mezcla-1.4.0.2/mezcla/examples/tests/test_hf_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/tests/test_hugging_face_speechrec.py` & `mezcla-1.4.0.2/mezcla/examples/tests/test_hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/tests/test_hugging_face_translation.py` & `mezcla-1.4.0.2/mezcla/examples/tests/test_hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/tests/test_matrix_multiply_benchmarking.py` & `mezcla-1.4.0.2/mezcla/examples/tests/test_matrix_multiply_benchmarking.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,16 +30,19 @@
 ## TODO: from mezcla import glue_helpers as gh
 from mezcla.my_regex import my_re
 from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:                        global module object
 #    TestIt.script_module:              path to file
-## TODO1: import mezcla.test_matrix_multiply_benchmarking as THE_MODULE
-import test_matrix_multiply_benchmarking as THE_MODULE
+try:
+    import mezcla.examples.matrix_multiply_benchmarking as THE_MODULE
+except:
+    THE_MODULE = None
+    system.print_exception_info("matrix_multiply_benchmarking import")
 #
 # Note: sanity test for customization (TODO: remove if desired)
 if not my_re.search(__file__, r"\btemplate.py$"):
     debug.assertion("mezcla.template" not in str(THE_MODULE))
 
 ## TODO:
 ## # Environment options
```

### Comparing `mezcla-1.4.0.1/mezcla/examples/tests/test_youtube_transcript.py` & `mezcla-1.4.0.2/mezcla/examples/tests/test_youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/tracemalloc_display.py` & `mezcla-1.4.0.2/mezcla/examples/tracemalloc_display.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/examples/youtube_transcript.py` & `mezcla-1.4.0.2/mezcla/examples/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/extract_document_text.py` & `mezcla-1.4.0.2/mezcla/extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/file_utils.py` & `mezcla-1.4.0.2/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/filter_random.py` & `mezcla-1.4.0.2/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/format_profile.py` & `mezcla-1.4.0.2/mezcla/format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/gensim_test.py` & `mezcla-1.4.0.2/mezcla/gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/glue_helpers.py` & `mezcla-1.4.0.2/mezcla/glue_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 import inspect
 import os
 import re
 import shutil
 from subprocess import getoutput
 import sys
 import tempfile
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Installed packages
 import textwrap
 
 # Local packages
 from mezcla import debug
 from mezcla import system
 from mezcla import tpo_common as tpo
 ## OLD: from mezcla.tpo_common import debug_format, debug_print, print_stderr, setenv
 from mezcla.tpo_common import debug_format, debug_print
 ## OLD: from mezcla.main import DISABLE_RECURSIVE_DELETE
-## DEBUG: sys.stderr.write(f"{__file__=}\n")
 ## TODO3: debug.trace_expr(6, __file__)
 
 # Constants
 TL = debug.TL
 
 # Environment options
 #
@@ -91,25 +91,23 @@
 TEMP_SUFFIX = ("-")
 NTF_ARGS = {'prefix': TEMP_PREFIX,
             'delete': not debug.detailed_debugging(),
             'suffix': TEMP_SUFFIX}
 TEMP_BASE = system.getenv_value(
     "TEMP_BASE", None,
     description="Override for temporary file basename")
-TEMP_BASE_DIR_DEFAULT = (TEMP_BASE and
-                         (system.is_directory(TEMP_BASE) or TEMP_BASE.endswith("/")))
+USE_TEMP_BASE_DIR_DEFAULT = bool(
+    TEMP_BASE and (system.is_directory(TEMP_BASE) or TEMP_BASE.endswith("/")))
 USE_TEMP_BASE_DIR = system.getenv_bool(
-    "USE_TEMP_BASE_DIR", TEMP_BASE_DIR_DEFAULT,
+    "USE_TEMP_BASE_DIR", USE_TEMP_BASE_DIR_DEFAULT,
     description="Whether TEMP_BASE should be a dir instead of prefix")
 DISABLE_RECURSIVE_DELETE = system.getenv_value(
     "DISABLE_RECURSIVE_DELETE", None,
     description="Disable use of potentially dangerous rm -r style recursive deletions")
-PRESERVE_TEMP_FILE = system.getenv_value(
-    "PRESERVE_TEMP_FILE", None,
-    desc="Retain value of TEMP_FILE even if TEMP_BASE set--see INFER_TEMP_FILE")
+PRESERVE_TEMP_FILE = None
 
 # Globals
 # note:
 # - see init() for main initialization;
 # - these are placeholds until module initialized
 # - os.path.join used to likewise avoid chick-n-egg problems with init
 # - TEMP_FILE is normally None to indicate use of random temp file name
@@ -435,15 +433,18 @@
     if just_issue is None:
         just_issue = False
     save_temp_base = TEMP_BASE
     if TEMP_BASE:
          system.setenv("TEMP_BASE", TEMP_BASE + "_subprocess_")
     save_temp_file = TEMP_FILE
     if TEMP_FILE and (PRESERVE_TEMP_FILE is not True):
-        system.setenv("TEMP_FILE", TEMP_FILE + "_subprocess_")
+        new_TEMP_FILE = TEMP_FILE + "_subprocess_"
+        debug.trace_expr(5, PRESERVE_TEMP_FILE)
+        debug.trace(5, f"Setting TEMP_FILE to {new_TEMP_FILE}")
+        system.setenv("TEMP_FILE", new_TEMP_FILE)
     # Expand the command template
     # TODO: make this optional
     command_line = command
     if re.search("{.*}", command):
         command_line = tpo.format(command_line, indirect_caller=True, ignore_exception=False, **namespace)
     debug_print("issuing: %s" % command_line, trace_level)
     # Run the command
@@ -468,15 +469,16 @@
     result = getoutput(command_line) if wait_for_command else str(os.system(command_line))
     if output:
         print(result)
     # Restore debug level setting in environment
     system.setenv("DEBUG_LEVEL", debug_level_env or "")
     system.setenv("TEMP_BASE", save_temp_base or "")
     if save_temp_file and (PRESERVE_TEMP_FILE is not True):
-        system.setenv("TEMP_FILE", save_temp_file or "")
+        debug.trace(5, f"Resetting TEMP_FILE to {save_temp_file}")
+        system.setenv("TEMP_FILE", save_temp_file)
     debug_print("run(_) => {\n%s\n}" % indent_lines(result), (trace_level + 1))
     return result
 
 
 def run_via_bash(command, trace_level=4, subtrace_level=None, init_file=None,
                  enable_aliases=False,
                  **namespace):
@@ -920,32 +922,39 @@
 else:
 
     def assertion(_condition):
         """Non-debug stub for assertion"""
         return
 
 def init():
-    """Work around for Python quirk"""
+    """Work around for Python quirk
+    Note: This is also used for reinitialize temp-file settings such as for unit tests (e.g., TEMP_FILE from TEMP_BASE)."""
     # See https://stackoverflow.com/questions/1590608/how-do-i-forward-declare-a-function-to-avoid-nameerrors-for-functions-defined
     debug.trace(5, "glue_helpers.init()")
-    global TEMP_FILE
     ## OLD: temp_filename = "temp-file.list"
     temp_filename = f"temp-{PID}.list"
     if USE_TEMP_BASE_DIR and TEMP_BASE:
         full_mkdir(TEMP_BASE)
-    #
-    ## BAD: temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}")
-    ## BAD: temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}" if TEMP_BASE else temp_filename)
-    ## OLD: temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}" if TEMP_BASE else None)
+
+    # Re-initialize flag blocking TEMP_FILE init from TEMP_BASE
+    global PRESERVE_TEMP_FILE
+    PRESERVE_TEMP_FILE = system.getenv_bool(
+        "PRESERVE_TEMP_FILE", None, allow_none=True,
+        desc="Retain value of TEMP_FILE even if TEMP_BASE set--see run and init below as well as unittest_wrapper.py")
+        
     # note: Normally TEMP_FILE gets overriden when TEMP_BASE set. However,
     # this complicates preserving test-specific test files (see unittest_wrapper.py).
+    # Further compications are due to the implicit module loading due to __init__.py.
+    # See tests/test_unittest_wrapper.py for some diagnosis tips.
     temp_file_default = None
     if TEMP_BASE and not PRESERVE_TEMP_FILE:
         temp_file_default = (form_path(TEMP_BASE, temp_filename) if USE_TEMP_BASE_DIR else f"{TEMP_BASE}-{temp_filename}")
+        debug.trace(4, f"FYI: Inferred TEMP_FILE default: {temp_file_default!r}")
     debug.trace_expr(5, system.getenv("TEMP_FILE"))
+    global TEMP_FILE
     TEMP_FILE = system.getenv_value(
         "TEMP_FILE", temp_file_default,
         description="Override for temporary filename")
     debug.trace_expr(5, system.getenv("TEMP_FILE"))
     #
     global TEMP_LOG_FILE
     TEMP_LOG_FILE = system.getenv_text(
```

### Comparing `mezcla-1.4.0.1/mezcla/gpu_utils.py` & `mezcla-1.4.0.2/mezcla/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/html_utils.py` & `mezcla-1.4.0.2/mezcla/html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/ipython_utils.py` & `mezcla-1.4.0.2/mezcla/ipython_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/kenlm_example.py` & `mezcla-1.4.0.2/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/keras_param_search.py` & `mezcla-1.4.0.2/mezcla/keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/llm_desktop_search.py` & `mezcla-1.4.0.2/mezcla/llm_desktop_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/main.py` & `mezcla-1.4.0.2/mezcla/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,23 +79,23 @@
 # Standard packages
 import argparse
 import io
 import os
 import re
 import sys
 import tempfile
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Local packages
 from mezcla import debug
 from mezcla import tpo_common as tpo
 from mezcla import glue_helpers as gh
 from mezcla import system
 from mezcla.my_regex import my_re
 from mezcla.system import getenv_bool
-## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Constants
 HELP_ARG = "--help"
 USAGE_ARG = "--usage"
 VERBOSE_ARG = "verbose"
 USE_PARAGRAPH_MODE_DEFAULT = getenv_bool("USE_PARAGRAPH_MODE", False)
 USE_PARAGRAPH_MODE = getenv_bool("PARAGRAPH_MODE", USE_PARAGRAPH_MODE_DEFAULT,
@@ -148,17 +148,19 @@
 TEMP_FILE = gh.TEMP_FILE
 KEEP_TEMP_FILES = system.getenv_bool("KEEP_TEMP_FILES", debug.detailed_debugging(),
                                      "Retain temporary files")
 INPUT_ERROR_OPTION = "input_error"
 INPUT_ERROR = system.getenv_value(
     INPUT_ERROR_OPTION.upper(), None,
     description="Override for strict input processing error handling")
-DISABLE_RECURSIVE_DELETE = system.getenv_value(
-    "DISABLE_RECURSIVE_DELETE", None,
-    description="Disable use of potentially dangerous rm -r style recursive deletions")
+## OLD:
+## DISABLE_RECURSIVE_DELETE = system.getenv_value(
+##     "DISABLE_RECURSIVE_DELETE", None,
+##     description="Disable use of potentially dangerous rm -r style recursive deletions")
+DISABLE_RECURSIVE_DELETE = gh.DISABLE_RECURSIVE_DELETE
 
 #-------------------------------------------------------------------------------
 
 class Main(object):
     """Class encompassing common script processing"""
     argument_parser = None
     force_unicode = False
@@ -265,15 +267,15 @@
 
         # Check miscellaneous options
         BINARY_INPUT_OPTION = "binary_input"
         PERL_SWITCH_PARSING_OPTION = "perl_switch_parsing"
         bad_options = system.difference(kwargs.keys(), [BINARY_INPUT_OPTION, PERL_SWITCH_PARSING_OPTION, INPUT_ERROR_OPTION])
         debug.assertion(not bad_options, f"Extraneous kwargs: {bad_options}")
         self.binary_input = kwargs.get(BINARY_INPUT_OPTION, False)
-        self.input_error = kwargs.get(INPUT_ERROR_OPTION, INPUT_ERROR)
+        self.input_error_mode = kwargs.get(INPUT_ERROR_OPTION, INPUT_ERROR)
 
         # Setup temporary file and/or base directory
         # Note: Uses NamedTemporaryFile (hence ntf_args)
         # TODO: allow temp_base handling to be overridable by constructor options
         # TODO: reconcile with unittest_wrapper.py.get_temp_dir
         prefix = (FILE_BASE + "-")
         ntf_args = {"prefix": prefix,
@@ -719,25 +721,27 @@
                     debug.trace(3, "Warning: Not opening multiple-valued filename arg")
                     debug.trace_expr(3, self.filename, self.other_filenames)
             else:
                 debug.assertion(isinstance(self.filename, str))
                 if not (self.manual_input and self.skip_input):
                     debug.assertion(os.path.exists(self.filename))
                     mode = ("r" if (not self.binary_input) else "rb")
-                    self.input_stream = system.open_file(self.filename, mode=mode, errors=self.input_error)
+                    self.input_stream = system.open_file(self.filename, mode=mode,
+                                                         errors=self.input_error_mode)
                     debug.assertion(self.input_stream)
         # Optionally reopen stream to change built-in settings
-        error_handling_change = (self.input_error and (self.input_error != self.input_stream.errors))
+        error_handling_change = (self.input_error_mode
+                                 and (self.input_error_mode != self.input_stream.errors))
         reopen_stream = (error_handling_change or self.newlines)
         if reopen_stream:
             if self.newlines:
                 debug.trace(4, f"Changing input stream newlines from {self.input_stream.newlines!r} to {self.newlines!r}")
             if error_handling_change:
-                debug.trace(4, f"Changing input stream error handling from {self.input_stream.errors!r} to {self.input_error!r}")
-            self.input_stream = io.TextIOWrapper(self.input_stream.buffer, encoding=self.input_stream.encoding, errors=self.input_error, newline=self.newlines, line_buffering=self.input_stream.line_buffering, write_through=self.input_stream.write_through)
+                debug.trace(4, f"Changing input stream error handling from {self.input_stream.errors!r} to {self.input_error_mode!r}")
+            self.input_stream = io.TextIOWrapper(self.input_stream.buffer, encoding=self.input_stream.encoding, errors=self.input_error_mode, newline=self.newlines, line_buffering=self.input_stream.line_buffering, write_through=self.input_stream.write_through)
             debug.trace_object(4, self.input_stream)
     
     def run(self):
         """Runner for script processing"""
         tpo.debug_print("Main.run()", 5)
         # TODO: decompose (e.g., isolate input proecessing)
```

### Comparing `mezcla-1.4.0.1/mezcla/merge_files.py` & `mezcla-1.4.0.2/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/merge_notes.py` & `mezcla-1.4.0.2/mezcla/merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/mezcla` & `mezcla-1.4.0.2/mezcla/mezcla`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/misc_utils.py` & `mezcla-1.4.0.2/mezcla/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/my_regex.py` & `mezcla-1.4.0.2/mezcla/my_regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,24 @@
 if RE_ALL:
     ## TODO: __all__ = re.__all__ + ['regex_wrapper', 'my_re']
     __all__ += re.__all__
     pass
 else:
     debug.trace(4, "Omitting use of re __all__")
 
-REGEX_TRACE_LEVEL = system.getenv_int("REGEX_TRACE_LEVEL", debug.QUITE_DETAILED,
-                                      "Trace level for my_regex")
+# Environment options
+## OLD
+## REGEX_TRACE_LEVEL = system.getenv_int("REGEX_TRACE_LEVEL", debug.QUITE_DETAILED,
+##                                       "Trace level for my_regex")
+REGEX_DEBUG_LEVEL = system.getenv_int(
+    "REGEX_TRACE_LEVEL", debug.QUITE_DETAILED,
+    desc="Alias for REGEX_TRACE_LEVEL")
+REGEX_TRACE_LEVEL = system.getenv_int(
+    "REGEX_TRACE_LEVEL", REGEX_DEBUG_LEVEL,
+    desc="Trace level for my_regex")
     
 ## TODO # HACK: make sure regex can be used as plug-in replacement 
 ## from from re import *
 
 ## TEST: Attempts to work around Python enum extension limitation
 ##
 ## OLD: class regex_wrapper(object):
```

### Comparing `mezcla-1.4.0.1/mezcla/ngram_tfidf.py` & `mezcla-1.4.0.2/mezcla/ngram_tfidf.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # Note:
 # - This provides the wrapper class ngram_tfidf_analysis around tfidf for use
 #   in applications like Visual Diff Search (VDS) that use text from external sources.
 # - This incorporates a few optional heuristics, such as filtering overlapping ngrams
 #   and boosting captialized ngrams.
 # - See compute_tfidf.py for computing tfidf over files.
 #
+# TODO1: fix --regular over filename
+#
 # TODO:
 # - Add more optional heuristics: part-of-speech boosting, adjoining ngram filtering,
 #   noun-phrase boosting, etc.
 # - Isolate ngram support into separate module.
 # - Reconcile with compute_tfidf.py (e.g., subsumption here with overlap there).
 #
 
@@ -450,28 +452,29 @@
     SAMPLE_SIZE = 10
     for l in range(num_docs):
         top_ngrams = ngram_analyzer.get_top_terms(l + 1)
         top_ngram_spec = "; ".join([f"{t}: {tpo.round_num(s, 3)}"
                                     for (t, s) in top_ngrams[:SAMPLE_SIZE]])
         print(f"{l}\t{top_ngram_spec}")
     
+
 def main():
     """Entry point for script"""
     debug.trace(4, "main()")
     SIMPLE_TEST_OPT = "simple-test"
     REGULAR_OPT = "regular"
     GOOD_TERMS_OPT = "good-terms"
     BAD_TERMS_OPT = "bad-terms"
     main_app = Main(description=__doc__.format(script=gh.basename(__file__),
                                                options=f"--{REGULAR_OPT}"),
                     boolean_options=[(SIMPLE_TEST_OPT, "Run simple canned test--default"),
                                      (REGULAR_OPT, "Process regular input--not canned test")],
                     text_options=[(GOOD_TERMS_OPT, "Overlap terms for boosting ngrams scores"),
                                   (BAD_TERMS_OPT, "Overlap terms for de-boosting ngrams scores")],
-                    skip_input=False)
+                    skip_input=False, manual_input=True)
     regular = main_app.get_parsed_option(REGULAR_OPT)
     simple_test = main_app.get_parsed_option(SIMPLE_TEST_OPT, not regular)
     good_terms_text = main_app.get_parsed_option(GOOD_TERMS_OPT)
     bad_terms_text = main_app.get_parsed_option(BAD_TERMS_OPT)
     if (simple_test):
         simple_main_test()
     else:
```

### Comparing `mezcla-1.4.0.1/mezcla/os_utils.py` & `mezcla-1.4.0.2/mezcla/os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/pandas_sklearn.py` & `mezcla-1.4.0.2/mezcla/pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/plot_utils.py` & `mezcla-1.4.0.2/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/python_ast.py` & `mezcla-1.4.0.2/mezcla/python_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/randomize_lines.py` & `mezcla-1.4.0.2/mezcla/randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/rgb_color_name.py` & `mezcla-1.4.0.2/mezcla/rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/run_albert_classifier.py` & `mezcla-1.4.0.2/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/run_bert_classifier.py` & `mezcla-1.4.0.2/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/samples/pima-indians-diabetes.csv` & `mezcla-1.4.0.2/mezcla/samples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/show_bert_representation.py` & `mezcla-1.4.0.2/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/simple_main_example.py` & `mezcla-1.4.0.2/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/spacy_nlp.py` & `mezcla-1.4.0.2/mezcla/spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/spell.py` & `mezcla-1.4.0.2/mezcla/spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/sys_version_info_hack.py` & `mezcla-1.4.0.2/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/system.py` & `mezcla-1.4.0.2/mezcla/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 ## OLD: import importlib_metadata
 import inspect
 import os
 import pickle
 import re
 import sys
 import time
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Installed packages
 import six
 
 # Local packages
 from mezcla import debug
 from mezcla.debug import UTF8
 ## TODO3: debug.trace_expr(6, __file__)
-## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Constants
 STRING_TYPES = six.string_types
 MAX_SIZE = six.MAXSIZE
 MAX_INT = MAX_SIZE
 TEMP_DIR = None
 ENCODING = "encoding"
@@ -207,59 +207,73 @@
     debug.trace_fmtd(5, "getenv_value({v!r}, [def={dft!r}], [desc={dsc!r}]]) => {val!r}",
                      v=var, dft=default, dsc=(description or desc), val=value)
     return (value)
 
 
 DEFAULT_GETENV_BOOL = False
 #
-def getenv_bool(var, default=DEFAULT_GETENV_BOOL, description=None, desc=None, update=None):
+def getenv_bool(var, default=DEFAULT_GETENV_BOOL, description=None, desc=None, allow_none=False, update=None):
     """Returns boolean flag based on environment VAR (or DEFAULT value), with optional DESCRIPTION and env. UPDATE
     Note:
     - "0" or "False" is interpreted as False, and any other explicit value as True (e.g., None => None)
     - In general, it is best to use False as default instead of True, because getenv_bool is meant for environment overrides, not defaults.
+    - TODO2: Return is a bool unless ALLOW_NONE; defaults to False.
     """
     # EX: getenv_bool("bad env var", None) => False
+    # EX: getenv_bool("bad env var", None, allow_none=True) => True
     # TODO: * Add debugging sanity checks for type of default to help diagnose when incorrect getenv_xyz variant used (e.g., getenv_int("USE_FUBAR", False) => ... getenv_bool)!
     bool_value = default
     value_text = getenv_value(var, description=description, desc=desc, default=default, update=update)
     if (isinstance(value_text, str) and value_text.strip()):
         bool_value = to_bool(value_text)
+    if not isinstance(bool_value, bool):
+        if (bool_value is None):
+            bool_value = False if (not allow_none) else None
+        else:
+            debug.assertion(bool_value != default, f"Check {var!r} default {default!r}")
+            bool_value = to_bool(bool_value)
+    debug.assertion(isinstance(bool_value, bool) or allow_none)
     debug.trace_fmtd(5, "getenv_bool({v}, {d}) => {r}",
                      v=var, d=default, r=bool_value)
     return (bool_value)
 #
 getenv_boolean = getenv_bool
 
 
-def getenv_number(var, default=-1.0, description=None, desc=None, helper=False, update=None):
-    """Returns number based on environment VAR (or DEFAULT value), with optional DESCRIPTION and env. UPDATE"""
+def getenv_number(var, default=-1.0, description=None, desc=None, helper=False, allow_none=False, update=None):
+    """Returns number based on environment VAR (or DEFAULT value), with optional DESCRIPTION and env. UPDATE
+    Note: Return is a float unless ALLOW_NONE; defaults to -1.0
+    """
+    # EX: getenv_float("?", default=1.5) => 1.5
     # TODO: def getenv_number(...) -> Optional(float):
     # Note: use getenv_int or getenv_float for typed variants
     num_value = default
     value = getenv_value(var, description=description, desc=desc, default=default, update=update)
     if (isinstance(value, str) and value.strip()):
         debug.assertion(is_number(value))
         num_value = to_float(value)
+    if (not ((num_value is None) and allow_none)):
+        num_value = to_float(num_value)
     trace_level = 6 if helper else 5
     debug.trace_fmtd(trace_level, "getenv_number({v}, {d}) => {r}",
                      v=var, d=default, r=num_value)
     return (num_value)
 #
 getenv_float = getenv_number
 
 
-
 def getenv_int(var, default=-1, description=None, desc=None, allow_none=False, update=None):
     """Version of getenv_number for integers, with optional DESCRIPTION and env. UPDATE
-    Note: Return is an integer unless ALLOW_NONE
+    Note: Return is an integer unless ALLOW_NONE; defaults to -1
     """
-    # EX: getenv_int("?", 1.5) => 1
-    value = getenv_number(var, description=description, desc=desc, default=default, helper=True, update=update)
+    # EX: getenv_int("?", default=1.5) => 1
+    value = getenv_number(var, description=description, desc=desc, default=default, allow_none=allow_none, helper=True, update=update)
     if (not isinstance(value, int)):
-        if ((value is not None) or allow_none):
+        ## OLD: if ((value is not None) and (not allow_none)):
+        if (not ((value is None) and allow_none)):
             value = to_int(value)
     debug.trace_fmtd(5, "getenv_int({v}, {d}) => {r}",
                      v=var, d=default, r=value)
     return (value)
 #
 getenv_integer = getenv_int
 
@@ -407,14 +421,15 @@
         errors = 'ignore'
     if kwargs.get(ENCODING) is None:
         kwargs[ENCODING] = encoding
     result = None
     try:
         # pylint: disable=consider-using-with; note: bogus 'Bad option value' warning
         ## BAD: result = open(filename, mode=mode, encoding=encoding, errors=errors, **kwargs)
+        # pylint: disable=unspecified-encoding
         result = open(filename, mode=mode, errors=errors, **kwargs)
     except IOError:
         debug.trace_fmtd(3, "Unable to open {f!r}: {exc}", f=filename, exc=get_exception())
     debug.trace_fmt(5, "open({f}, [{enc}, {err}], kwargs={kw}) => {r}",
                     f=filename, enc=encoding, err=errors, kw=kwargs, r=result)
     return result
 
@@ -567,14 +582,15 @@
     # EX: write_file("/tmp/fu123", "1\n2\n3\n"); read_entire_file("/tmp/fu123") => "1\n2\n3\n"
     data = ""
     try:
         if kwargs.get(ENCODING) is None:
             kwargs[ENCODING] = "UTF-8"
         ## TODO: with open_file(filename, **kwargs) as f:
         ## BAD: with open(filename, encoding="UTF-8", **kwargs) as f:
+        # pylint: disable=unspecified-encoding
         with open(filename, **kwargs) as f:
             data = f.read()
     except (AttributeError, IOError):
         debug.trace_exception(1, "read_entire_file/IOError")
         report_errors = (kwargs.get("errors") != "ignore")
         if report_errors:
             print_stderr("Error: Unable to read file '{f}': {exc}",
```

### Comparing `mezcla-1.4.0.1/mezcla/temp/compound_CID_3672.xml` & `mezcla-1.4.0.2/mezcla/temp/compound_CID_3672.xml`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/temp/plot.py` & `mezcla-1.4.0.2/mezcla/temp/plot.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/temp/simple_batspp.py` & `mezcla-1.4.0.2/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/template.py` & `mezcla-1.4.0.2/mezcla/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 ## TODO: Use helper class for main logic
 ## class Helper:
 ##     """TODO: class for doing ..."""
 ## 
 ##     def __init__(self, ...):
 ##         """Initializer: ..."""
-##         debug.trace_fmtd(TL.VERBOSE, "Helper.__init__(): self={s}", s=self)
+##         debug.trace(TL.VERBOSE, f"Helper.__init__(): self={self}")
 ##         self.TODO = None
 ##         debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
 ## 
 ##     def process(self, ...):
 ##         """TODO: ..."""
 ##         # TODO: flesh out
 ##
@@ -89,15 +89,15 @@
     #
     ## def __init__(self, *args, **kwargs):
     ##     debug.trace_expr(TL.VERBOSE, self, args, kwargs, delim="\n\t", prefix="in {self.__class__.__name__}.__init__({a})")
     ##     super().__init__(*args, **kwargs)
 
     def setup(self):
         """Check results of command line processing"""
-        debug.trace_fmtd(TL.VERBOSE, "Script.setup(): self={s}", s=self)
+        debug.trace(TL.VERBOSE, f"Script.setup(): self={self}")
         ## TODO: extract argument values
         self.todo_arg = self.get_parsed_option(TODO_ARG, self.todo_arg)
         ## TODO:
         ## self.text_arg = self.get_parsed_option(TEXT_ARG, self.text_arg)
         ## self.alt_filename = self.get_parsed_argument(ALT_FILENAME)
         debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
 
@@ -114,15 +114,15 @@
         ##     print("arg2 line: %s" % line)
 
     ## TODO: if no input prococessed, customize run_main_step instead
     ## and specify skip_input below
     ##
     ## def run_main_step(self):
     ##     """Main processing step (n.b., assumes self.manual_input)"""
-    ##     debug.trace_fmtd(5, "Script.run_main_step(): self={s}", s=self)
+    ##     debug.trace(5, f"Script.run_main_step(): self={self}")
     ##
 
     ## TODO:
     ## def wrap_up(self):
     ##     """Do final processing"""
     ##     debug.trace(6, f"Script.wrap_up(); self={self}")
     ##     # ...
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/LICENSE.txt` & `mezcla-1.4.0.2/mezcla/tests/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.4.0.2/mezcla/tests/adhoc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/conftest.py` & `mezcla-1.4.0.2/mezcla/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt` & `mezcla-1.4.0.2/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb` & `mezcla-1.4.0.2/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/jupyter/test_audio_py.ipynb` & `mezcla-1.4.0.2/mezcla/tests/jupyter/test_audio_py.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/jupyter/test_audio_py_experimental.ipynb` & `mezcla-1.4.0.2/mezcla/tests/jupyter/test_audio_py_experimental.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb` & `mezcla-1.4.0.2/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/jupyter/test_hugging_face_translation.ipynb` & `mezcla-1.4.0.2/mezcla/tests/jupyter/test_hugging_face_translation.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/jupyter/test_template.ipynb` & `mezcla-1.4.0.2/mezcla/tests/jupyter/test_template.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/misc-tests.batspp` & `mezcla-1.4.0.2/mezcla/tests/misc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/misc_doctests.py` & `mezcla-1.4.0.2/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/misc_tests.py` & `mezcla-1.4.0.2/mezcla/tests/misc_tests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/argentinian-attraction-snippets.txt` & `mezcla-1.4.0.2/mezcla/tests/resources/argentinian-attraction-snippets.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/cars-csv-len-3.txt` & `mezcla-1.4.0.2/mezcla/tests/resources/cars-csv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/cars-tsv-len-3.txt` & `mezcla-1.4.0.2/mezcla/tests/resources/cars-tsv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/cars.csv` & `mezcla-1.4.0.2/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/cars.tsv` & `mezcla-1.4.0.2/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/example_text.txt` & `mezcla-1.4.0.2/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.4.0.2/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/iris_output.txt` & `mezcla-1.4.0.2/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/random-10pct-tweet-emotions.tsv` & `mezcla-1.4.0.2/mezcla/tests/resources/random-10pct-tweet-emotions.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.4.0.2/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.4.0.2/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.4.0.2/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/test.arpa` & `mezcla-1.4.0.2/mezcla/tests/resources/test.arpa`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/word-POS.freq` & `mezcla-1.4.0.2/mezcla/tests/resources/word-POS.freq`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/resources/word.freq` & `mezcla-1.4.0.2/mezcla/tests/resources/word.freq`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/template.py` & `mezcla-1.4.0.2/mezcla/tests/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,22 @@
 ## TODO: from mezcla import glue_helpers as gh
 from mezcla.my_regex import my_re
 from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:                        global module object
 #    TestIt.script_module:              path to file
-## TODO (vvv): insert new module name in commented out template teo lines below
-THE_MODULE = None         ## TODO: remove this line: avoids <module> syntax error in next)
-## import mezcla.<module> as THE_MODULE   ## TODO: uncomment this line (<<<)
-## TODO (^^^): use modified line above
+THE_MODULE = None
+try:
+    ## TODO: import mezcla.<module> as THE_MODULE
+    pass                                ## TODO: delete
+except:
+    system.print_exception_info("<module> import") 
+## 
+## TODO: make sure import above syntactically valid
 #
 # Note: sanity test for customization (TODO: remove if desired)
 if not my_re.search(__file__, r"\btemplate.py$"):
     debug.assertion("mezcla.template" not in str(THE_MODULE))
 
 ## TODO:
 ## # Environment options
@@ -127,22 +131,22 @@
         self.do_assert("whatever" in captured, "TODO_whatever trace")
         return
 
     ## TODO: optional cleanup methods
     ##
     ## def tearDown(self):
     ##     debug.trace(6, f"TestIt.tearDown(); self={self}")
-    ##     super().tearDownClass()
+    ##     super().tearDown()
     ##     ...
     ##     return
     ##
     ## @classmethod
     ## def tearDownClass(cls):
     ##     debug.trace(6, f"TestIt.tearDownClass(); cls={cls}")
-    ##     super().tearDown()
+    ##     super().tearDownClass()
     ##     ...
     ##     return
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/test___init__.py` & `mezcla-1.4.0.2/mezcla/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_audio.py` & `mezcla-1.4.0.2/mezcla/tests/test_audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 # Notes:
 # - *** All the tests are skipped if the audio packages not installed.
 # - This can be run as follows:
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_audio.py
 # - some tests will take a while.
 #
 ## TODO: solve test execution long times.
+#
+# TODO4:
+# - Reword "this will take a while and this require a valid audio path in AUDIOFILE"
+#   so that just covers RUN_SLOW_TESTS; Check separately for path.
+#
+
 
 
 """Tests for Audio module"""
 
 # Standard packages
 ## NOTE: this is empty for now
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.4.0.2/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_bing_search.py` & `mezcla-1.4.0.2/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.4.0.2/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_convert_emoticons.py` & `mezcla-1.4.0.2/mezcla/tests/test_convert_emoticons.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_cut.py` & `mezcla-1.4.0.2/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_data_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_debug.py` & `mezcla-1.4.0.2/mezcla/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_evaluate_example_tests.py` & `mezcla-1.4.0.2/mezcla/tests/test_evaluate_example_tests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_extract_document_text.py` & `mezcla-1.4.0.2/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_file_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_filter_random.py` & `mezcla-1.4.0.2/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_format_profile.py` & `mezcla-1.4.0.2/mezcla/tests/test_format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_gensim_test.py` & `mezcla-1.4.0.2/mezcla/tests/test_gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_glue_helpers.py` & `mezcla-1.4.0.2/mezcla/tests/test_glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_gpu_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_gpu_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_html_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_ipython_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_ipython_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_kenlm_example.py` & `mezcla-1.4.0.2/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_keras_param_search.py` & `mezcla-1.4.0.2/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_llm_desktop_search.py` & `mezcla-1.4.0.2/mezcla/tests/test_llm_desktop_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_main.py` & `mezcla-1.4.0.2/mezcla/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_merge_files.py` & `mezcla-1.4.0.2/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_merge_notes.py` & `mezcla-1.4.0.2/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_misc_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_my_regex.py` & `mezcla-1.4.0.2/mezcla/tests/test_my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.4.0.2/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_os_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_os_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 """Tests for os_utils module"""
 
 # Standard packages
 ## NOTE: this is empty for now
 
 # Installed packages
-import pytest
+## TODO: import pytest
 
 # Local packages
 from mezcla import debug
 from mezcla import os_utils
 from mezcla.unittest_wrapper import TestWrapper, invoke_tests
 
 # Note: Two references are used for the module to be tested:
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.4.0.2/mezcla/tests/test_pandas_sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,33 @@
     def test_main_without_args(self):
         """Ensure main without args works as expected"""
         debug.trace(4, "test_main_without_args()")
         log_file = gh.get_temp_file()
         self.run_script(data_file='', log_file=log_file)
         assert 'Usage:' in gh.read_file(log_file)
 
+    @pytest.mark.xfail
     def test_normal_usage(self):
         """Ensure normal usage works as expected"""
         debug.trace(4, "test_normal_usage()")
         output = self.run_script(data_file=IRIS_EXAMPLE)
         assert output
 
         # Check line per line avoiding flaky numbers that always change
+        line_num = 0
         for expected_line, actual_line in zip(gh.read_lines(IRIS_OUTPUT), output.splitlines()):
             expected_line = re.sub(r' +', ' ', expected_line)
             actual_line = re.sub(r' +', ' ', actual_line)
+            line_num += 1
+            # note: ignores lines like following
+            #   107          7.3         2.9          6.3         1.8   Iris-virginica
             if re.search(r'[0-9] +[0-9\.]+ +[0-9\.]+ +[0-9\.]+ +[0-9\.]+ +[a-zA-Z]+-[a-zA-Z]+', expected_line):
+                debug.trace(6, f"Ignoring line {line_num} with details: {expected_line}")
                 continue
+            debug.trace_expr(5, line_num, expected_line, actual_line)
             assert actual_line == expected_line
 
     def test_verbose(self):
         """Ensure verbose works as expected"""
         debug.trace(4, "test_normal_usage()")
         output = self.run_script(env_options='VERBOSE=true', data_file=IRIS_EXAMPLE)
         assert 'Development test classification report:' in output
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_plot_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_python_ast.py` & `mezcla-1.4.0.2/mezcla/tests/test_python_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_randomize_lines.py` & `mezcla-1.4.0.2/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.4.0.2/mezcla/tests/test_rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.4.0.2/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.4.0.2/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.4.0.2/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_simple_main_example.py` & `mezcla-1.4.0.2/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.4.0.2/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_spell.py` & `mezcla-1.4.0.2/mezcla/tests/test_spell.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 # - Carefully review tests/template.py.
 # TODO3:
 # - Create test helpers to cut down on all the redundant code.
 #   ex: def check_spelling(self, lang, text, bad):
 #       """Run spelling over TEXT in TEXT looking for BAD words""
 #       output = self.run_script(env_options=f"SPELL_LANG={lang}", data_file=gh.create_temp_file(text))
 #       assert(system.intersection(text.split(), bad.split()))
+# TODO4:
+# - Reword "This test can take some time or may have missing libraries" so that just
+#   covers RUN_SLOW_TESTS; Check separately for missing libraries.
 #
 
 """Tests for spell module"""
 # Standard packages
 ## OLD: import re
 
 # Installed packages
@@ -41,14 +44,15 @@
 #    THE_MODULE:	    global module object
 #    TestIt.script_module:              path to file
 try:
     # note: requires enchant-2 library package under Ubuntu (besides pyenchant)
     import mezcla.spell as THE_MODULE
 except:
     THE_MODULE = None
+    system.print_exception_info("spell import")
 
 # Since importing doesn't work properly, a temporary fix is specifying the path
 # import mezcla.spell as THE_MODULE
 # *** It works fine: please follow the example in test/template.py better! ***
 ## BAD
 ## PATH1 = f'$PWD/mezcla/spell.py'
 ## PATH2 = f'$PWD/spell.py'
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.4.0.2/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_system.py` & `mezcla-1.4.0.2/mezcla/tests/test_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,22 +156,26 @@
     def test_getenv_number(self):
         """Ensure getenv_number works as expected"""
         debug.trace(4, "test_getenv_number()")
         # note: whitespaces is not a typo, is to test strip condition
         self.monkeypatch.setenv('TEST_NUMBER', ' 9.81    ', prepend=False)
         assert THE_MODULE.getenv_number('TEST_NUMBER', default=10) == 9.81
         assert THE_MODULE.getenv_number('BAD_TEST_NUMBER', default=10) == 10
+        assert THE_MODULE.getenv_number('BAD VAR', default=None, allow_none=True) is None
+        assert THE_MODULE.getenv_number('BAD VAR', default=None, allow_none=False) == 0.0
         ## TODO: test helper argument
 
     def test_getenv_int(self):
         """Ensure getenv_int works as expected"""
         debug.trace(4, "test_getenv_int()")
         self.monkeypatch.setenv('TEST_NUMBER', '9.81', prepend=False)
         assert THE_MODULE.getenv_int('TEST_NUMBER', default=20) == 9
         assert THE_MODULE.getenv_int("REALLY FUBAR", 123) == 123
+        assert THE_MODULE.getenv_int('BAD VAR', default=None, allow_none=True) is None
+        assert THE_MODULE.getenv_int('BAD VAR', default=None, allow_none=False) == 0
 
     def test_get_exception(self):
         """Ensure get_exception works as expected"""
         debug.trace(4, "test_get_exception()")
         exception = None
         try:
             raise RuntimeError("testing")
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_template.py` & `mezcla-1.4.0.2/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_text_categorizer.py` & `mezcla-1.4.0.2/mezcla/tests/test_text_categorizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,30 @@
 # Standard packages
 ## OLD: import random
 
 # Installed packages
 import pytest
 
 # Local packages
-from mezcla.unittest_wrapper import TestWrapper, trap_exception
+from mezcla.unittest_wrapper import TestWrapper
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.my_regex import my_re
 from mezcla import system
 from mezcla import misc_utils
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
-system.setenv("USE_XGB", "1")
+## OLD: system.setenv("USE_XGB", "1")
 THE_MODULE = None
 try:
     ## TEMP: fails if xgboost not available (workaround for stupid docker issue)
-    import xgboost
-    debug.trace_expr(5, xgboost.XGBClassifier)
+    ## OLD:
+    ## import xgboost
+    ## debug.trace_expr(5, xgboost.XGBClassifier)
     import mezcla.text_categorizer as THE_MODULE
 except:
     system.print_exception_info("text_categorizer import")
 
 # Environment options
 TEST_TBD = system.getenv_bool("TEST_TBD", False,
                               description="Test features to be designed: TBD")
@@ -133,15 +134,17 @@
 
     @pytest.mark.xfail
     def test_train(self):
         """Make sure training works"""
         debug.trace(4, "test_train()")
         data_file = gh.form_path(self.resources, "random-10pct-tweet-emotions.tsv")
         data = system.read_lines(data_file)
-        tc = THE_MODULE.TextCategorizer(use_xgb=True)
+        ## NOTE: Unfortunately xgboost takes too much disk space under Github actions
+        ## OLD: tc = THE_MODULE.TextCategorizer(use_xgb=True)
+        tc = THE_MODULE.TextCategorizer(use_xgb=False)
         tc.train(data_file)
         num_ok = 0
         num_to_test = 10
         for _i in range(num_to_test):
             ## OLD: case = random.randint(1, len(data) - 1)
             case = misc_utils.random_int(1, len(data) - 1)
             expect_cat, expect_text = data[case].split("\t")
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_text_processing.py` & `mezcla-1.4.0.2/mezcla/tests/test_text_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 from mezcla import system
 from mezcla.my_regex import my_re
 from mezcla.unittest_wrapper import TestWrapper
 from mezcla.unittest_wrapper import trap_exception
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
-import mezcla.text_processing as THE_MODULE
+try:
+    import mezcla.text_processing as THE_MODULE
+except:
+    THE_MODULE = None
+    system.print_exception_info("text_processing import")    
 
 # Constants
 RESOURCES = f'{gh.dir_path(__file__)}/resources'
 TEXT_EXAMPLE = f'{RESOURCES}/example_text.txt'
 TEXT_EXAMPLE_TAGS = f'{RESOURCES}/example_text_tags.txt'
 WORD_POS_FREQ_FILE = f'{RESOURCES}/word-POS.freq'
 WORD_FREQ_FILE = f'{RESOURCES}/word.freq'
 
+@pytest.mark.skipif(not THE_MODULE, reason="Problem loading THE_MODULE")
 class TestTextProcessing(TestWrapper):
     """Class for testcase definition"""
 
     def test_split_sentences(self):
         """Ensure split_sentences works as expected"""
         debug.trace(4, "test_split_sentences()")
         assert THE_MODULE.split_sentences("I came. I saw. I conquered!") == ["I came.", "I saw.", "I conquered!"]
```

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_text_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_tpo_common.py` & `mezcla-1.4.0.2/mezcla/tests/test_tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_train_language_model.py` & `mezcla-1.4.0.2/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.4.0.2/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_transpose_data.py` & `mezcla-1.4.0.2/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/test_xml_utils.py` & `mezcla-1.4.0.2/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.4.0.2/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.4.0.2/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/tfidf/test_document.py` & `mezcla-1.4.0.2/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.4.0.2/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/text_categorizer.py` & `mezcla-1.4.0.2/mezcla/text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/text_processing.py` & `mezcla-1.4.0.2/mezcla/text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/text_utils.py` & `mezcla-1.4.0.2/mezcla/text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tfidf/config.py` & `mezcla-1.4.0.2/mezcla/tfidf/config.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tfidf/corpus.py` & `mezcla-1.4.0.2/mezcla/tfidf/corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tfidf/dockeyword.py` & `mezcla-1.4.0.2/mezcla/tfidf/dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tfidf/document.py` & `mezcla-1.4.0.2/mezcla/tfidf/document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tfidf/preprocess.py` & `mezcla-1.4.0.2/mezcla/tfidf/preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tfidf/tests/misc_test.py` & `mezcla-1.4.0.2/mezcla/tfidf/tests/misc_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/tpo_common.py` & `mezcla-1.4.0.2/mezcla/tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/train_language_model.py` & `mezcla-1.4.0.2/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/train_text_categorizer.py` & `mezcla-1.4.0.2/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/transpose_data.py` & `mezcla-1.4.0.2/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/mezcla/unittest_wrapper.py` & `mezcla-1.4.0.2/mezcla/unittest_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,31 @@
 
 # Standard packages
 import inspect
 import os
 import sys
 import tempfile
 import unittest
+## DEBUG: sys.stderr.write(f"{__file__=}\n")
 
 # Installed packages
 import pytest
 
 # Local packages
-# note: Disables TEMP_FILE default used by in glue_helpers.py.
-os.environ["PRESERVE_TEMP_FILE"] = "1"
+# note: Disables TEMP_FILE default used by glue_helpers.py.
+PRESERVE_TEMP_FILE_LABEL = "PRESERVE_TEMP_FILE"
+if PRESERVE_TEMP_FILE_LABEL not in os.environ:
+    ## DEBUG: 
+    sys.stderr.write(f"Setting {PRESERVE_TEMP_FILE_LABEL}\n")
+    os.environ[PRESERVE_TEMP_FILE_LABEL] = "1"
 import mezcla
 from mezcla import debug
 from mezcla import glue_helpers as gh
-from mezcla.main import DISABLE_RECURSIVE_DELETE
+## BAD: from mezcla.main import DISABLE_RECURSIVE_DELETE
+DISABLE_RECURSIVE_DELETE = gh.DISABLE_RECURSIVE_DELETE
 from mezcla.misc_utils import string_diff
 from mezcla.my_regex import my_re
 from mezcla import system
 ## DEBUG: debug.trace_expr(6, __file__)
 
 # Constants (e.g., environment options)
 
@@ -173,37 +179,45 @@
         """Wrapper around unary function f(x)"""   ## TODO: {function.__name__}
         debug.trace(7, f"in wrapper: x={x}")
         return function(x)
     #
     debug.trace(7, f"pytest_fixture_wrapper() => {gh.elide(wrapper)}")
     return wrapper
 
+
 def invoke_tests(filename: str, via_unittest: bool = VIA_UNITTEST):
     """Invoke TESTS defined in FILENAME, optionally VIA_UNITTEST"""
     if via_unittest:
         unittest.main()
     else:
         pytest.main([filename])
 
+
+def init_temp_settings():
+    """Initialize settings related to temp-file names"""
+    ok = True
+    # Re-initalize glue helper temp file settings
+    ## TODO?: system.setenv("PRESERVE_TEMP_FILE", "1")
+    debug.trace_expr(4, os.environ.get(PRESERVE_TEMP_FILE_LABEL))
+    ## TEST: os.environ["PRESERVE_TEMP_FILE"] = "1"
+    if not system.getenv(PRESERVE_TEMP_FILE_LABEL):
+        system.setenv(PRESERVE_TEMP_FILE_LABEL, "1")
+    gh.init()
+    debug.trace_expr(4, os.environ.get(PRESERVE_TEMP_FILE_LABEL))
+    return ok
+        
 #-------------------------------------------------------------------------------
 
 class TestWrapper(unittest.TestCase):
     """Class for testcase definition
     Note:
     - script_module should be overriden to specify the module instance, such as via get_testing_module_name (see test/template.py)
     - set it to None to avoid command-line invocation checks
     """
-
-    # Re-initalize glue helper temp file settings
-    ## TODO?: system.setenv("PRESERVE_TEMP_FILE", "1")
-    debug.trace_expr(4, os.environ.get("PRESERVE_TEMP_FILE"))
-    ## TEST: os.environ["PRESERVE_TEMP_FILE"] = "1"
-    system.setenv("PRESERVE_TEMP_FILE", "1")
-    gh.init()
-    debug.trace_expr(4, os.environ.get("PRESERVE_TEMP_FILE"))
+    init_ok = init_temp_settings()
 
     script_file = TODO_FILE             # path for invocation via 'python -m coverage run ...' (n.b., usually set via get_module_file_path)
     script_module = TODO_MODULE         # name for invocation via 'python -m' (n.b., usually set via derive_tested_module_name)
     temp_base = system.getenv_text(
         "TEMP_BASE", tempfile.NamedTemporaryFile().name,
         desc="Override for basename of temporary files")
     check_coverage = system.getenv_bool(
@@ -342,15 +356,15 @@
         """Per-test initializations
         Notes:
         - Disables tracing scripts invoked via run() unless ALLOW_SUBCOMMAND_TRACING
         - Initializes temp file name (With override from environment)."""
         # Note: By default, each test gets its own temp file.
         debug.trace(5, "TestWrapper.setUp()")
         if not self.class_setup:
-            debug.trace(4, "Warning: invoking setUpClass in setUp")
+            debug.trace(3, "Warning: invoking setUpClass in setUp; make sure seUpClass calls parent")
             TestWrapper.setUpClass(self.__class__)
         if not gh.ALLOW_SUBCOMMAND_TRACING:
             gh.disable_subcommand_tracing()
         # The temp file is an extension of temp-base file by default.
         # Optionally, if can be a file in temp-base subdrectory.
         if self.use_temp_base_dir:
             default_temp_file = gh.form_path(self.temp_base, "test-")
```

### Comparing `mezcla-1.4.0.1/mezcla/xml_utils.py` & `mezcla-1.4.0.2/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/packages-required.txt` & `mezcla-1.4.0.2/packages-required.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/pyproject.toml` & `mezcla-1.4.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## TODO: eliminate redundancy
 
 [tool.poetry]
 name = "mezcla"
-version = "1.4.0.1"
+version = "1.4.0.2"
 description = "Miscellaneous Python scripts developed over the course of several independent consulting projects. [Mezcla is Spanish for mixture.]"
 authors = ["Tom O'Hara <tomasohara@gmail.com>"]
 license = "LGPLv3"
 ## TODO:
 ## packages = ['mezcla', 'mezcla.tfidf']
 
 [tool.poetry.dependencies]
```

### Comparing `mezcla-1.4.0.1/requirements.txt` & `mezcla-1.4.0.2/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 #opt# flit
 #opt# gensim
 #opt# ibm-watson
 #opt# ibm_cloud_sdk_core
 #opt# ipython
 #opt# jupyter
 #opt# librosa
+#opt# numba
 #opt# pocketsphinx
 #opt# pylint
 #opt# pyyaml
 #opt# scispacy
 #opt# selenium
 #opt# Sphinx
 #
```

### Comparing `mezcla-1.4.0.1/setup.py` & `mezcla-1.4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla', 'mezcla.tfidf'],
       module="mezcla",
       ## TODO2: import mezcla; version=mezcla.VERSION
-      version="1.4.0.1",
+      version="1.4.0.2",
       ## BAD: description-file="README.txt",
       description_file="README.txt",
       ## BAD: dist-name="Mezcla",
       dist_name="Mezcla",
       author="Tom O'Hara",
       # TODO3: find out which email key is preferred
       email="tomasohara@gmail.com",
```

### Comparing `mezcla-1.4.0.1/temp/simple_batspp.py` & `mezcla-1.4.0.2/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/tools/_temp_test_settings.bash` & `mezcla-1.4.0.2/tools/_temp_test_settings.bash`

 * *Files 5% similar despite different names*

```diff
@@ -22,13 +22,14 @@
 # 2. For other Github Actions env. vars, see https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/environment-variables-full-list-github-actions
 MIN_DEBUG_LEVEL=2
 if [ "$DEPLOYMENT_BASEPATH" == "/opt/runner" ]; then
     MIN_DEBUG_LEVEL=4
 fi
 DEBUG_LEVEL="${DEBUG_LEVEL:-0}"
 if [ "$DEBUG_LEVEL" -lt "$MIN_DEBUG_LEVEL" ]; then
-    export DEBUG_LEVEL=MIN_DEBUG_LEVEL
+    export DEBUG_LEVEL=$MIN_DEBUG_LEVEL
 fi
 if [ "$DEBUG_LEVEL" -ge 4 ]; then
     export PYTEST_OPTIONS="-v -s"
 fi
-export TEST_REGEX=unittest_wrapper
+## BAD: export TEST_REGEX=unittest_wrapper
+export FILTER_REGEX='tests/template.py'
```

### Comparing `mezcla-1.4.0.1/tools/local-workflows.sh` & `mezcla-1.4.0.2/tools/local-workflows.sh`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/tools/run_tests.bash` & `mezcla-1.4.0.2/tools/run_tests.bash`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/tox.ini` & `mezcla-1.4.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `mezcla-1.4.0.1/PKG-INFO` & `mezcla-1.4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mezcla
-Version: 1.4.0.1
+Version: 1.4.0.2
 Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
 Home-page: https://github.com/tomasohara/mezcla
 License: LGPLv3
 Author: Tomás O'Hara
 Author-email: tomasohara@gmail.com
 Description-Content-Type: text/plain
```

