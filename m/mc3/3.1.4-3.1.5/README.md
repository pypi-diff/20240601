# Comparing `tmp/mc3-3.1.4.tar.gz` & `tmp/mc3-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc3-3.1.4.tar", last modified: Thu May 30 15:04:12 2024, max compression
+gzip compressed data, was "mc3-3.1.5.tar", last modified: Sat Jun  1 05:53:15 2024, max compression
```

## Comparing `mc3-3.1.4.tar` & `mc3-3.1.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.344791 mc3-3.1.4/
--rw-r--r--   0 pato       (501) staff       (20)      123 2024-05-30 15:02:31.000000 mc3-3.1.4/.readthedocs.yml
--rw-r--r--   0 pato       (501) staff       (20)     2943 2021-03-08 22:07:25.000000 mc3-3.1.4/CONTRIBUTING.md
--rw-r--r--   0 pato       (501) staff       (20)     1085 2024-05-30 15:02:31.000000 mc3-3.1.4/LICENSE
--rw-r--r--   0 pato       (501) staff       (20)      365 2024-05-30 15:03:29.000000 mc3-3.1.4/MANIFEST.in
--rw-r--r--   0 pato       (501) staff       (20)     3486 2024-05-30 15:04:12.344506 mc3-3.1.4/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1779 2024-05-30 15:02:31.000000 mc3-3.1.4/README.md
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.329627 mc3-3.1.4/docs/
--rw-r--r--   0 pato       (501) staff       (20)     7657 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/Makefile
--rw-r--r--   0 pato       (501) staff       (20)    62757 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/api.rst
--rw-r--r--   0 pato       (501) staff       (20)    11541 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/conf.py
--rw-r--r--   0 pato       (501) staff       (20)     2970 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/contributing.rst
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.332649 mc3-3.1.4/docs/figures/
--rw-r--r--   0 pato       (501) staff       (20)    32125 2021-03-26 16:00:15.000000 mc3-3.1.4/docs/figures/quad_bestfit.png
--rw-r--r--   0 pato       (501) staff       (20)    34319 2021-03-26 16:00:15.000000 mc3-3.1.4/docs/figures/quad_fitting.png
--rw-r--r--   0 pato       (501) staff       (20)    46027 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/figures/quad_hist.png
--rw-r--r--   0 pato       (501) staff       (20)   242288 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/figures/quad_pairwise.png
--rw-r--r--   0 pato       (501) staff       (20)   211712 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/figures/quad_trace.png
--rw-r--r--   0 pato       (501) staff       (20)    48970 2021-03-26 16:00:15.000000 mc3-3.1.4/docs/figures/rms-vs-binsize.png
--rw-r--r--   0 pato       (501) staff       (20)     8854 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/fit_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)     6737 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/get_started.rst
--rw-r--r--   0 pato       (501) staff       (20)     4370 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/index.rst
--rw-r--r--   0 pato       (501) staff       (20)     1140 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/license.rst
--rw-r--r--   0 pato       (501) staff       (20)     7243 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/make.bat
--rw-r--r--   0 pato       (501) staff       (20)    28030 2024-05-30 15:02:31.000000 mc3-3.1.4/docs/mcmc_tutorial.rst
--rw-r--r--   0 pato       (501) staff       (20)     1691 2021-03-08 22:07:25.000000 mc3-3.1.4/docs/references.rst
--rw-r--r--   0 pato       (501) staff       (20)     1333 2021-03-26 16:00:15.000000 mc3-3.1.4/docs/time_averaging.rst
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.335390 mc3-3.1.4/examples/
--rw-r--r--   0 pato       (501) staff       (20)     1650 2024-05-30 15:02:31.000000 mc3-3.1.4/examples/get_started.py
--rw-r--r--   0 pato       (501) staff       (20)     1556 2021-03-08 22:07:25.000000 mc3-3.1.4/examples/timeavg.py
--rw-r--r--   0 pato       (501) staff       (20)     2792 2024-05-30 15:02:31.000000 mc3-3.1.4/examples/tutorial.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.336823 mc3-3.1.4/mc3/
--rw-r--r--   0 pato       (501) staff       (20)      688 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    10897 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/__main__.py
--rw-r--r--   0 pato       (501) staff       (20)    13086 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/chain.py
--rw-r--r--   0 pato       (501) staff       (20)     9288 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/fit_driver.py
--rw-r--r--   0 pato       (501) staff       (20)    13642 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/mcmc_driver.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.340205 mc3-3.1.4/mc3/plots/
--rw-r--r--   0 pato       (501) staff       (20)      604 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/plots/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     5594 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/plots/colors.py
--rw-r--r--   0 pato       (501) staff       (20)    10671 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/plots/plot_functions.py
--rw-r--r--   0 pato       (501) staff       (20)    39119 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/plots/posterior.py
--rw-r--r--   0 pato       (501) staff       (20)    23046 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/sampler_driver.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.341333 mc3-3.1.4/mc3/stats/
--rw-r--r--   0 pato       (501) staff       (20)      638 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     2674 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/gelman.py
--rw-r--r--   0 pato       (501) staff       (20)      811 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/prayer.py
--rw-r--r--   0 pato       (501) staff       (20)    36306 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/stats.py
--rw-r--r--   0 pato       (501) staff       (20)     1589 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/stats/time_averaging.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.341772 mc3-3.1.4/mc3/utils/
--rw-r--r--   0 pato       (501) staff       (20)      529 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/utils/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)     7119 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/utils/log.py
--rw-r--r--   0 pato       (501) staff       (20)    13722 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/utils/utils.py
--rw-r--r--   0 pato       (501) staff       (20)      275 2024-05-30 15:02:31.000000 mc3-3.1.4/mc3/version.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.344111 mc3-3.1.4/mc3.egg-info/
--rw-r--r--   0 pato       (501) staff       (20)     3486 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1373 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/SOURCES.txt
--rw-r--r--   0 pato       (501) staff       (20)        1 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/dependency_links.txt
--rw-r--r--   0 pato       (501) staff       (20)       42 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/entry_points.txt
--rw-r--r--   0 pato       (501) staff       (20)       65 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/requires.txt
--rw-r--r--   0 pato       (501) staff       (20)        4 2024-05-30 15:04:12.000000 mc3-3.1.4/mc3.egg-info/top_level.txt
--rw-r--r--   0 pato       (501) staff       (20)     1075 2024-05-30 15:02:31.000000 mc3-3.1.4/pyproject.toml
--rw-r--r--   0 pato       (501) staff       (20)      150 2021-03-08 22:07:25.000000 mc3-3.1.4/pytest.ini
--rw-r--r--   0 pato       (501) staff       (20)       57 2024-05-30 15:02:31.000000 mc3-3.1.4/requirements.txt
--rw-r--r--   0 pato       (501) staff       (20)       38 2024-05-30 15:04:12.344832 mc3-3.1.4/setup.cfg
--rw-r--r--   0 pato       (501) staff       (20)      833 2024-05-30 15:02:31.000000 mc3-3.1.4/setup.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.342362 mc3-3.1.4/src_c/
--rw-r--r--   0 pato       (501) staff       (20)     3973 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/_binarray.c
--rw-r--r--   0 pato       (501) staff       (20)     7667 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/_chisq.c
--rw-r--r--   0 pato       (501) staff       (20)    10514 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/_dwt.c
--rw-r--r--   0 pato       (501) staff       (20)     6902 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/_time_averaging.c
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.342827 mc3-3.1.4/src_c/include/
--rw-r--r--   0 pato       (501) staff       (20)      522 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/include/ind.h
--rw-r--r--   0 pato       (501) staff       (20)     6646 2024-05-30 15:02:31.000000 mc3-3.1.4/src_c/include/stats.h
--rw-r--r--   0 pato       (501) staff       (20)     4185 2024-05-30 15:02:32.000000 mc3-3.1.4/src_c/include/wavelet.h
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-05-30 15:04:12.343894 mc3-3.1.4/tests/
--rw-r--r--   0 pato       (501) staff       (20)     3988 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_fit.py
--rw-r--r--   0 pato       (501) staff       (20)     2281 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_logging.py
--rw-r--r--   0 pato       (501) staff       (20)    15975 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_mcmc.py
--rw-r--r--   0 pato       (501) staff       (20)     3790 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_plots.py
--rw-r--r--   0 pato       (501) staff       (20)    14911 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_stats.py
--rw-r--r--   0 pato       (501) staff       (20)     8937 2024-05-30 15:02:32.000000 mc3-3.1.4/tests/test_utils.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.858306 mc3-3.1.5/
+-rw-r--r--   0 pato       (501) staff       (20)      302 2024-06-01 05:51:25.000000 mc3-3.1.5/.readthedocs.yml
+-rw-r--r--   0 pato       (501) staff       (20)     2943 2021-03-08 22:07:25.000000 mc3-3.1.5/CONTRIBUTING.md
+-rw-r--r--   0 pato       (501) staff       (20)     1085 2024-05-30 15:02:31.000000 mc3-3.1.5/LICENSE
+-rw-r--r--   0 pato       (501) staff       (20)      365 2024-05-30 15:03:29.000000 mc3-3.1.5/MANIFEST.in
+-rw-r--r--   0 pato       (501) staff       (20)     3486 2024-06-01 05:53:15.856896 mc3-3.1.5/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1779 2024-05-30 15:02:31.000000 mc3-3.1.5/README.md
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.827561 mc3-3.1.5/docs/
+-rw-r--r--   0 pato       (501) staff       (20)     7657 2021-03-08 22:07:25.000000 mc3-3.1.5/docs/Makefile
+-rw-r--r--   0 pato       (501) staff       (20)    62757 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/api.rst
+-rw-r--r--   0 pato       (501) staff       (20)    11636 2024-06-01 05:51:25.000000 mc3-3.1.5/docs/conf.py
+-rw-r--r--   0 pato       (501) staff       (20)     2970 2021-03-08 22:07:25.000000 mc3-3.1.5/docs/contributing.rst
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.831284 mc3-3.1.5/docs/figures/
+-rw-r--r--   0 pato       (501) staff       (20)    32125 2021-03-26 16:00:15.000000 mc3-3.1.5/docs/figures/quad_bestfit.png
+-rw-r--r--   0 pato       (501) staff       (20)    34319 2021-03-26 16:00:15.000000 mc3-3.1.5/docs/figures/quad_fitting.png
+-rw-r--r--   0 pato       (501) staff       (20)    46027 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/figures/quad_hist.png
+-rw-r--r--   0 pato       (501) staff       (20)   242288 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/figures/quad_pairwise.png
+-rw-r--r--   0 pato       (501) staff       (20)   211712 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/figures/quad_trace.png
+-rw-r--r--   0 pato       (501) staff       (20)    48970 2021-03-26 16:00:15.000000 mc3-3.1.5/docs/figures/rms-vs-binsize.png
+-rw-r--r--   0 pato       (501) staff       (20)     8854 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/fit_tutorial.rst
+-rw-r--r--   0 pato       (501) staff       (20)     6737 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/get_started.rst
+-rw-r--r--   0 pato       (501) staff       (20)     4370 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/index.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1140 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/license.rst
+-rw-r--r--   0 pato       (501) staff       (20)     7243 2021-03-08 22:07:25.000000 mc3-3.1.5/docs/make.bat
+-rw-r--r--   0 pato       (501) staff       (20)    28030 2024-05-30 15:02:31.000000 mc3-3.1.5/docs/mcmc_tutorial.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1691 2021-03-08 22:07:25.000000 mc3-3.1.5/docs/references.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1333 2021-03-26 16:00:15.000000 mc3-3.1.5/docs/time_averaging.rst
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.834110 mc3-3.1.5/examples/
+-rw-r--r--   0 pato       (501) staff       (20)     1650 2024-05-30 15:02:31.000000 mc3-3.1.5/examples/get_started.py
+-rw-r--r--   0 pato       (501) staff       (20)     1556 2021-03-08 22:07:25.000000 mc3-3.1.5/examples/timeavg.py
+-rw-r--r--   0 pato       (501) staff       (20)     2792 2024-05-30 15:02:31.000000 mc3-3.1.5/examples/tutorial.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.840144 mc3-3.1.5/mc3/
+-rw-r--r--   0 pato       (501) staff       (20)      688 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    10897 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/__main__.py
+-rw-r--r--   0 pato       (501) staff       (20)    13086 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/chain.py
+-rw-r--r--   0 pato       (501) staff       (20)     9288 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/fit_driver.py
+-rw-r--r--   0 pato       (501) staff       (20)    13642 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/mcmc_driver.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.849816 mc3-3.1.5/mc3/plots/
+-rw-r--r--   0 pato       (501) staff       (20)      604 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/plots/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     5594 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/plots/colors.py
+-rw-r--r--   0 pato       (501) staff       (20)    10671 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/plots/plot_functions.py
+-rw-r--r--   0 pato       (501) staff       (20)    39119 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/plots/posterior.py
+-rw-r--r--   0 pato       (501) staff       (20)    23046 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/sampler_driver.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.851718 mc3-3.1.5/mc3/stats/
+-rw-r--r--   0 pato       (501) staff       (20)      638 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/stats/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     2674 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/stats/gelman.py
+-rw-r--r--   0 pato       (501) staff       (20)      811 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/stats/prayer.py
+-rw-r--r--   0 pato       (501) staff       (20)    36306 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/stats/stats.py
+-rw-r--r--   0 pato       (501) staff       (20)     1589 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/stats/time_averaging.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.852238 mc3-3.1.5/mc3/utils/
+-rw-r--r--   0 pato       (501) staff       (20)      529 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/utils/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)     7119 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/utils/log.py
+-rw-r--r--   0 pato       (501) staff       (20)    13722 2024-05-30 15:02:31.000000 mc3-3.1.5/mc3/utils/utils.py
+-rw-r--r--   0 pato       (501) staff       (20)      275 2024-06-01 05:51:25.000000 mc3-3.1.5/mc3/version.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.855152 mc3-3.1.5/mc3.egg-info/
+-rw-r--r--   0 pato       (501) staff       (20)     3486 2024-06-01 05:53:15.000000 mc3-3.1.5/mc3.egg-info/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1373 2024-06-01 05:53:15.000000 mc3-3.1.5/mc3.egg-info/SOURCES.txt
+-rw-r--r--   0 pato       (501) staff       (20)        1 2024-06-01 05:53:15.000000 mc3-3.1.5/mc3.egg-info/dependency_links.txt
+-rw-r--r--   0 pato       (501) staff       (20)       42 2024-06-01 05:53:15.000000 mc3-3.1.5/mc3.egg-info/entry_points.txt
+-rw-r--r--   0 pato       (501) staff       (20)       65 2024-06-01 05:53:15.000000 mc3-3.1.5/mc3.egg-info/requires.txt
+-rw-r--r--   0 pato       (501) staff       (20)        4 2024-06-01 05:53:15.000000 mc3-3.1.5/mc3.egg-info/top_level.txt
+-rw-r--r--   0 pato       (501) staff       (20)     1075 2024-05-30 15:02:31.000000 mc3-3.1.5/pyproject.toml
+-rw-r--r--   0 pato       (501) staff       (20)      150 2021-03-08 22:07:25.000000 mc3-3.1.5/pytest.ini
+-rw-r--r--   0 pato       (501) staff       (20)       57 2024-05-30 15:02:31.000000 mc3-3.1.5/requirements.txt
+-rw-r--r--   0 pato       (501) staff       (20)       38 2024-06-01 05:53:15.858521 mc3-3.1.5/setup.cfg
+-rw-r--r--   0 pato       (501) staff       (20)      845 2024-06-01 05:51:25.000000 mc3-3.1.5/setup.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.853230 mc3-3.1.5/src_c/
+-rw-r--r--   0 pato       (501) staff       (20)     3973 2024-05-30 15:02:31.000000 mc3-3.1.5/src_c/_binarray.c
+-rw-r--r--   0 pato       (501) staff       (20)     7667 2024-05-30 15:02:31.000000 mc3-3.1.5/src_c/_chisq.c
+-rw-r--r--   0 pato       (501) staff       (20)    10514 2024-05-30 15:02:31.000000 mc3-3.1.5/src_c/_dwt.c
+-rw-r--r--   0 pato       (501) staff       (20)     6902 2024-05-30 15:02:31.000000 mc3-3.1.5/src_c/_time_averaging.c
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.853659 mc3-3.1.5/src_c/include/
+-rw-r--r--   0 pato       (501) staff       (20)      522 2024-05-30 15:02:31.000000 mc3-3.1.5/src_c/include/ind.h
+-rw-r--r--   0 pato       (501) staff       (20)     6646 2024-05-30 15:02:31.000000 mc3-3.1.5/src_c/include/stats.h
+-rw-r--r--   0 pato       (501) staff       (20)     4185 2024-05-30 15:02:32.000000 mc3-3.1.5/src_c/include/wavelet.h
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2024-06-01 05:53:15.854884 mc3-3.1.5/tests/
+-rw-r--r--   0 pato       (501) staff       (20)     3988 2024-05-30 15:02:32.000000 mc3-3.1.5/tests/test_fit.py
+-rw-r--r--   0 pato       (501) staff       (20)     2281 2024-05-30 15:02:32.000000 mc3-3.1.5/tests/test_logging.py
+-rw-r--r--   0 pato       (501) staff       (20)    15975 2024-05-30 15:02:32.000000 mc3-3.1.5/tests/test_mcmc.py
+-rw-r--r--   0 pato       (501) staff       (20)     3790 2024-05-30 15:02:32.000000 mc3-3.1.5/tests/test_plots.py
+-rw-r--r--   0 pato       (501) staff       (20)    14911 2024-05-30 15:02:32.000000 mc3-3.1.5/tests/test_stats.py
+-rw-r--r--   0 pato       (501) staff       (20)     8937 2024-05-30 15:02:32.000000 mc3-3.1.5/tests/test_utils.py
```

### Comparing `mc3-3.1.4/CONTRIBUTING.md` & `mc3-3.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/LICENSE` & `mc3-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/PKG-INFO` & `mc3-3.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mc3
-Version: 3.1.4
+Version: 3.1.5
 Summary: Multi-core Markov-chain Monte Carlo package
 Author-email: Patricio Cubillos <patricio.cubillos@oeaw.ac.at>
 License: Copyright (c) 2015-2022 Patricio Cubillos and contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mc3-3.1.4/README.md` & `mc3-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/Makefile` & `mc3-3.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/api.rst` & `mc3-3.1.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/conf.py` & `mc3-3.1.5/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.mathjax',
     'sphinx.ext.viewcode',
+    'IPython.sphinxext.ipython_console_highlighting',
+    'nbsphinx',
+    "sphinx_copybutton",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -68,15 +71,15 @@
 release = mc3.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
```

### Comparing `mc3-3.1.4/docs/contributing.rst` & `mc3-3.1.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/figures/quad_bestfit.png` & `mc3-3.1.5/docs/figures/quad_bestfit.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/figures/quad_fitting.png` & `mc3-3.1.5/docs/figures/quad_fitting.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/figures/quad_hist.png` & `mc3-3.1.5/docs/figures/quad_hist.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/figures/quad_pairwise.png` & `mc3-3.1.5/docs/figures/quad_pairwise.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/figures/quad_trace.png` & `mc3-3.1.5/docs/figures/quad_trace.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/figures/rms-vs-binsize.png` & `mc3-3.1.5/docs/figures/rms-vs-binsize.png`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/fit_tutorial.rst` & `mc3-3.1.5/docs/fit_tutorial.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/get_started.rst` & `mc3-3.1.5/docs/get_started.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/index.rst` & `mc3-3.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/license.rst` & `mc3-3.1.5/docs/license.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/make.bat` & `mc3-3.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/mcmc_tutorial.rst` & `mc3-3.1.5/docs/mcmc_tutorial.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/references.rst` & `mc3-3.1.5/docs/references.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/docs/time_averaging.rst` & `mc3-3.1.5/docs/time_averaging.rst`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/examples/get_started.py` & `mc3-3.1.5/examples/get_started.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/examples/timeavg.py` & `mc3-3.1.5/examples/timeavg.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/examples/tutorial.py` & `mc3-3.1.5/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/__init__.py` & `mc3-3.1.5/mc3/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/__main__.py` & `mc3-3.1.5/mc3/__main__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/chain.py` & `mc3-3.1.5/mc3/chain.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/fit_driver.py` & `mc3-3.1.5/mc3/fit_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/mcmc_driver.py` & `mc3-3.1.5/mc3/mcmc_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/plots/__init__.py` & `mc3-3.1.5/mc3/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/plots/colors.py` & `mc3-3.1.5/mc3/plots/colors.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/plots/plot_functions.py` & `mc3-3.1.5/mc3/plots/plot_functions.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/plots/posterior.py` & `mc3-3.1.5/mc3/plots/posterior.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/sampler_driver.py` & `mc3-3.1.5/mc3/sampler_driver.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/stats/__init__.py` & `mc3-3.1.5/mc3/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/stats/gelman.py` & `mc3-3.1.5/mc3/stats/gelman.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/stats/prayer.py` & `mc3-3.1.5/mc3/stats/prayer.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/stats/stats.py` & `mc3-3.1.5/mc3/stats/stats.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/stats/time_averaging.py` & `mc3-3.1.5/mc3/stats/time_averaging.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/utils/__init__.py` & `mc3-3.1.5/mc3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/utils/log.py` & `mc3-3.1.5/mc3/utils/log.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3/utils/utils.py` & `mc3-3.1.5/mc3/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/mc3.egg-info/PKG-INFO` & `mc3-3.1.5/mc3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mc3
-Version: 3.1.4
+Version: 3.1.5
 Summary: Multi-core Markov-chain Monte Carlo package
 Author-email: Patricio Cubillos <patricio.cubillos@oeaw.ac.at>
 License: Copyright (c) 2015-2022 Patricio Cubillos and contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mc3-3.1.4/mc3.egg-info/SOURCES.txt` & `mc3-3.1.5/mc3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/pyproject.toml` & `mc3-3.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/setup.py` & `mc3-3.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 incdir = 'src_c/include/'
 
 cfiles = os.listdir(srcdir)
 cfiles = list(filter(lambda x: re.search('.+[.]c$', x), cfiles))
 cfiles = list(filter(lambda x: not re.search('[.#].+[.]c$', x), cfiles))
 
 inc = [get_include(), incdir]
-eca = ['-O3', '-ffast-math']
-ela = []
+eca = ['-lm', '-O3', '-ffast-math']
+ela = ['-lm']
 
 extensions = [
     Extension(
         'mc3.lib.' + cfile.rstrip('.c'),
         sources=[f'{srcdir}{cfile}'],
         include_dirs=inc,
         extra_compile_args=eca,
```

### Comparing `mc3-3.1.4/src_c/_binarray.c` & `mc3-3.1.5/src_c/_binarray.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/src_c/_chisq.c` & `mc3-3.1.5/src_c/_chisq.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/src_c/_dwt.c` & `mc3-3.1.5/src_c/_dwt.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/src_c/_time_averaging.c` & `mc3-3.1.5/src_c/_time_averaging.c`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/src_c/include/ind.h` & `mc3-3.1.5/src_c/include/ind.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/src_c/include/stats.h` & `mc3-3.1.5/src_c/include/stats.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/src_c/include/wavelet.h` & `mc3-3.1.5/src_c/include/wavelet.h`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/tests/test_fit.py` & `mc3-3.1.5/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/tests/test_logging.py` & `mc3-3.1.5/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/tests/test_mcmc.py` & `mc3-3.1.5/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/tests/test_plots.py` & `mc3-3.1.5/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/tests/test_stats.py` & `mc3-3.1.5/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `mc3-3.1.4/tests/test_utils.py` & `mc3-3.1.5/tests/test_utils.py`

 * *Files identical despite different names*

