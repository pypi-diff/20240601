# Comparing `tmp/starred-astro-1.4.2.tar.gz` & `tmp/starred_astro-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred-astro-1.4.2.tar", last modified: Fri May 24 00:58:58 2024, max compression
+gzip compressed data, was "starred_astro-1.4.3.tar", last modified: Sat Jun  1 17:47:08 2024, max compression
```

## Comparing `starred-astro-1.4.2.tar` & `starred_astro-1.4.3.tar`

### file list

```diff
@@ -1,45 +1,71 @@
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.125914 starred-astro-1.4.2/
--rw-r--r--   0 fred      (1000) fred      (1000)      847 2023-09-03 03:28:55.000000 starred-astro-1.4.2/AUTHORS.md
--rw-r--r--   0 fred      (1000) fred      (1000)    35143 2023-08-24 20:35:25.000000 starred-astro-1.4.2/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)     5961 2024-05-24 00:58:58.125914 starred-astro-1.4.2/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)     5441 2024-05-06 20:44:40.000000 starred-astro-1.4.2/README.md
--rw-r--r--   0 fred      (1000) fred      (1000)       38 2024-05-24 00:58:58.125914 starred-astro-1.4.2/setup.cfg
--rw-r--r--   0 fred      (1000) fred      (1000)     1212 2024-05-24 00:54:57.000000 starred-astro-1.4.2/setup.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.122581 starred-astro-1.4.2/starred/
--rw-r--r--   0 fred      (1000) fred      (1000)      352 2023-08-24 20:35:25.000000 starred-astro-1.4.2/starred/__init__.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.122581 starred-astro-1.4.2/starred/deconvolution/
--rw-r--r--   0 fred      (1000) fred      (1000)      112 2023-09-04 14:18:38.000000 starred-astro-1.4.2/starred/deconvolution/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)    39953 2024-03-13 00:55:55.000000 starred-astro-1.4.2/starred/deconvolution/deconvolution.py
--rw-r--r--   0 fred      (1000) fred      (1000)    14267 2024-05-23 14:27:41.000000 starred-astro-1.4.2/starred/deconvolution/loss.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4391 2023-11-08 20:15:24.000000 starred-astro-1.4.2/starred/deconvolution/parameters.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.122581 starred-astro-1.4.2/starred/optim/
--rw-r--r--   0 fred      (1000) fred      (1000)      128 2024-03-11 19:32:35.000000 starred-astro-1.4.2/starred/optim/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7098 2024-05-23 14:27:41.000000 starred-astro-1.4.2/starred/optim/inference_base.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9557 2023-12-20 13:59:25.000000 starred-astro-1.4.2/starred/optim/optimization.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2577 2023-12-20 13:59:25.000000 starred-astro-1.4.2/starred/optim/sampling.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.125914 starred-astro-1.4.2/starred/plots/
--rw-r--r--   0 fred      (1000) fred      (1000)       89 2023-08-24 20:35:25.000000 starred-astro-1.4.2/starred/plots/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4797 2024-05-23 14:27:41.000000 starred-astro-1.4.2/starred/plots/f2n.py
--rw-r--r--   0 fred      (1000) fred      (1000)    23752 2024-05-23 21:47:02.000000 starred-astro-1.4.2/starred/plots/plot_function.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.125914 starred-astro-1.4.2/starred/procedures/
--rw-r--r--   0 fred      (1000) fred      (1000)      287 2023-12-20 13:59:25.000000 starred-astro-1.4.2/starred/procedures/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9374 2024-05-06 20:44:40.000000 starred-astro-1.4.2/starred/procedures/deconvolution_routines.py
--rw-r--r--   0 fred      (1000) fred      (1000)    26070 2024-05-23 21:47:02.000000 starred-astro-1.4.2/starred/procedures/psf_routines.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.125914 starred-astro-1.4.2/starred/psf/
--rw-r--r--   0 fred      (1000) fred      (1000)      103 2023-09-04 14:18:27.000000 starred-astro-1.4.2/starred/psf/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11298 2024-05-23 21:47:02.000000 starred-astro-1.4.2/starred/psf/loss.py
--rw-r--r--   0 fred      (1000) fred      (1000)     5373 2024-05-23 14:27:41.000000 starred-astro-1.4.2/starred/psf/parameters.py
--rw-r--r--   0 fred      (1000) fred      (1000)    39162 2024-05-23 21:57:11.000000 starred-astro-1.4.2/starred/psf/psf.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.125914 starred-astro-1.4.2/starred/utils/
--rw-r--r--   0 fred      (1000) fred      (1000)      178 2023-12-20 13:59:25.000000 starred-astro-1.4.2/starred/utils/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2379 2023-09-01 15:33:20.000000 starred-astro-1.4.2/starred/utils/ds9reg.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11588 2024-03-04 18:09:29.000000 starred-astro-1.4.2/starred/utils/generic_utils.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6200 2024-05-23 14:27:41.000000 starred-astro-1.4.2/starred/utils/jax_utils.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4331 2023-11-08 20:15:24.000000 starred-astro-1.4.2/starred/utils/light_profile_analytical.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9730 2024-05-23 14:27:41.000000 starred-astro-1.4.2/starred/utils/noise_utils.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11087 2023-12-20 13:59:25.000000 starred-astro-1.4.2/starred/utils/parameters.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-05-24 00:58:58.125914 starred-astro-1.4.2/starred_astro.egg-info/
--rw-r--r--   0 fred      (1000) fred      (1000)     5961 2024-05-24 00:58:58.000000 starred-astro-1.4.2/starred_astro.egg-info/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)      943 2024-05-24 00:58:58.000000 starred-astro-1.4.2/starred_astro.egg-info/SOURCES.txt
--rw-r--r--   0 fred      (1000) fred      (1000)        1 2024-05-24 00:58:58.000000 starred-astro-1.4.2/starred_astro.egg-info/dependency_links.txt
--rw-r--r--   0 fred      (1000) fred      (1000)        8 2024-05-24 00:58:58.000000 starred-astro-1.4.2/starred_astro.egg-info/top_level.txt
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.364911 starred_astro-1.4.3/
+-rw-r--r--   0 fred      (1000) fred      (1000)      847 2024-06-01 17:40:26.000000 starred_astro-1.4.3/AUTHORS.md
+-rw-r--r--   0 fred      (1000) fred      (1000)    35143 2024-06-01 17:40:26.000000 starred_astro-1.4.3/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)     6790 2024-06-01 17:47:08.364911 starred_astro-1.4.3/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)     5441 2024-06-01 17:40:26.000000 starred_astro-1.4.3/README.md
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.361578 starred_astro-1.4.3/docs/
+-rw-r--r--   0 fred      (1000) fred      (1000)     4519 2024-06-01 17:40:26.000000 starred_astro-1.4.3/docs/conf.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1354 2024-06-01 17:47:03.000000 starred_astro-1.4.3/pyproject.toml
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.361578 starred_astro-1.4.3/scripts/
+-rw-r--r--   0 fred      (1000) fred      (1000)    11882 2024-06-01 17:40:26.000000 starred_astro-1.4.3/scripts/1_generate_psf.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    12081 2024-06-01 17:40:26.000000 starred_astro-1.4.3/scripts/2_deconvolve.py
+-rw-r--r--   0 fred      (1000) fred      (1000)       38 2024-06-01 17:47:08.364911 starred_astro-1.4.3/setup.cfg
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.361578 starred_astro-1.4.3/starred/
+-rw-r--r--   0 fred      (1000) fred      (1000)      352 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/__init__.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.361578 starred_astro-1.4.3/starred/deconvolution/
+-rw-r--r--   0 fred      (1000) fred      (1000)      112 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/deconvolution/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    39953 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/deconvolution/deconvolution.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    14267 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/deconvolution/loss.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4391 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/deconvolution/parameters.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.361578 starred_astro-1.4.3/starred/optim/
+-rw-r--r--   0 fred      (1000) fred      (1000)      128 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/optim/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7098 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/optim/inference_base.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9557 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/optim/optimization.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2577 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/optim/sampling.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.361578 starred_astro-1.4.3/starred/plots/
+-rw-r--r--   0 fred      (1000) fred      (1000)       89 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/plots/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4797 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/plots/f2n.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    23752 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/plots/plot_function.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.361578 starred_astro-1.4.3/starred/procedures/
+-rw-r--r--   0 fred      (1000) fred      (1000)      287 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/procedures/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9374 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/procedures/deconvolution_routines.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    27521 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/procedures/psf_routines.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.361578 starred_astro-1.4.3/starred/psf/
+-rw-r--r--   0 fred      (1000) fred      (1000)      103 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/psf/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11298 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/psf/loss.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     5373 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/psf/parameters.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    39162 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/psf/psf.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.364911 starred_astro-1.4.3/starred/utils/
+-rw-r--r--   0 fred      (1000) fred      (1000)      178 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/utils/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2379 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/utils/ds9reg.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    12671 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/utils/generic_utils.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6200 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/utils/jax_utils.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4331 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/utils/light_profile_analytical.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9730 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/utils/noise_utils.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11087 2024-06-01 17:40:26.000000 starred_astro-1.4.3/starred/utils/parameters.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.364911 starred_astro-1.4.3/starred_astro.egg-info/
+-rw-r--r--   0 fred      (1000) fred      (1000)     6790 2024-06-01 17:47:08.000000 starred_astro-1.4.3/starred_astro.egg-info/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)     1510 2024-06-01 17:47:08.000000 starred_astro-1.4.3/starred_astro.egg-info/SOURCES.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)        1 2024-06-01 17:47:08.000000 starred_astro-1.4.3/starred_astro.egg-info/dependency_links.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)      227 2024-06-01 17:47:08.000000 starred_astro-1.4.3/starred_astro.egg-info/requires.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)       57 2024-06-01 17:47:08.000000 starred_astro-1.4.3/starred_astro.egg-info/top_level.txt
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.364911 starred_astro-1.4.3/tests/
+-rw-r--r--   0 fred      (1000) fred      (1000)      166 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/__init__.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.364911 starred_astro-1.4.3/tests/test_deconv/
+-rw-r--r--   0 fred      (1000) fred      (1000)        0 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_deconv/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    10615 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_deconv/test_deconv.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4105 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_deconv/test_deconv_sersic.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.364911 starred_astro-1.4.3/tests/test_plots/
+-rw-r--r--   0 fred      (1000) fred      (1000)        0 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_plots/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3504 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_plots/test_plots.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.364911 starred_astro-1.4.3/tests/test_psf/
+-rw-r--r--   0 fred      (1000) fred      (1000)        0 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_psf/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9974 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_psf/test_convolution.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1325 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_psf/test_distortion.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    13878 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_psf/test_psf.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2024-06-01 17:47:08.364911 starred_astro-1.4.3/tests/test_utils/
+-rw-r--r--   0 fred      (1000) fred      (1000)        0 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_utils/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1290 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_utils/test_jax_utils.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4655 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_utils/test_noise.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3238 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_utils/test_params.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     5453 2024-06-01 17:40:26.000000 starred_astro-1.4.3/tests/test_utils/test_utils.py
```

### Comparing `starred-astro-1.4.2/AUTHORS.md` & `starred_astro-1.4.3/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/LICENSE` & `starred_astro-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/PKG-INFO` & `starred_astro-1.4.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: starred-astro
-Version: 1.4.2
-Summary: A two-channel deconvolution method with Starlet regularization
-Author: Kevin Michalewicz, Martin Millon, Fred Dux
-Author-email: kevinmicha@hotmail.com
-Requires: astropy
-Requires: dill
-Requires: jax
-Requires: jaxlib
-Requires: jaxopt
-Requires: matplotlib
-Requires: numpy
-Requires: scipy
-Requires: optax
-Requires: tqdm
-Requires: emcee
-Requires: pyregion
-Requires: h5py
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-
 # STARRED: STARlet REgularized Deconvolution 
 
 [![pipeline status](https://gitlab.com/cosmograil/starred/badges/main/pipeline.svg)](https://gitlab.com/cosmograil/starred/commits/main)
 [![coverage report](https://gitlab.com/cosmograil/starred/badges/main/coverage.svg)](https://cosmograil.gitlab.io/starred/coverage/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05340/status.svg)](https://doi.org/10.21105/joss.05340)
```

### Comparing `starred-astro-1.4.2/README.md` & `starred_astro-1.4.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: starred-astro
+Version: 1.4.3
+Summary: A two-channel deconvolution method with Starlet regularization
+Author: Martin Millon, Frédéric Dux
+Author-email: Kevin Michalewicz <kevinmicha@hotmail.com>
+Project-URL: homepage, https://starred-astro.github.io
+Project-URL: repository, https://github.com/starred/starred-astro
+Keywords: deconvolution,astronomy,starlet,image processing
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: astropy>=5.0.4
+Requires-Dist: dill>=0.3.5.1
+Requires-Dist: jax>=0.4.13
+Requires-Dist: jaxlib>=0.4.13
+Requires-Dist: matplotlib>=3.4.2
+Requires-Dist: numpy>=1.21.2
+Requires-Dist: scipy>=1.10.0
+Requires-Dist: optax>=0.1.7
+Requires-Dist: jaxopt>=0.8
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: h5py>=3.9.0
+Provides-Extra: opt
+Requires-Dist: emcee>=3.1.4; extra == "opt"
+Requires-Dist: mclmc>=0.2.6; extra == "opt"
+Requires-Dist: pyregion>=2.2.0; extra == "opt"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+
 # STARRED: STARlet REgularized Deconvolution 
 
 [![pipeline status](https://gitlab.com/cosmograil/starred/badges/main/pipeline.svg)](https://gitlab.com/cosmograil/starred/commits/main)
 [![coverage report](https://gitlab.com/cosmograil/starred/badges/main/coverage.svg)](https://cosmograil.gitlab.io/starred/coverage/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05340/status.svg)](https://doi.org/10.21105/joss.05340)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `starred-astro-1.4.2/starred/deconvolution/deconvolution.py` & `starred_astro-1.4.3/starred/deconvolution/deconvolution.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/deconvolution/loss.py` & `starred_astro-1.4.3/starred/deconvolution/loss.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/deconvolution/parameters.py` & `starred_astro-1.4.3/starred/deconvolution/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/optim/inference_base.py` & `starred_astro-1.4.3/starred/optim/inference_base.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/optim/optimization.py` & `starred_astro-1.4.3/starred/optim/optimization.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/optim/sampling.py` & `starred_astro-1.4.3/starred/optim/sampling.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/plots/f2n.py` & `starred_astro-1.4.3/starred/plots/f2n.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/plots/plot_function.py` & `starred_astro-1.4.3/starred/plots/plot_function.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/procedures/deconvolution_routines.py` & `starred_astro-1.4.3/starred/procedures/deconvolution_routines.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/procedures/psf_routines.py` & `starred_astro-1.4.3/starred/procedures/psf_routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import warnings
 
 from starred.psf.psf import PSF
 from starred.psf.loss import Loss, Prior
 from starred.optim.optimization import Optimizer
 from starred.psf.parameters import ParametersPSF
 from starred.utils.noise_utils import propagate_noise
+from starred.plots import plot_function as pltf
+import matplotlib.pyplot as plt
 
 
 def build_psf(image, noisemap, subsampling_factor,
               masks=None,
               n_iter_analytic=40, n_iter_adabelief=2000,
               guess_method_star_position='barycenter', guess_fwhm_pixels=3.,
               field_distortion=False, stamp_coordinates=None):
@@ -349,32 +351,38 @@
 
 def update_PSF(kernel_old, data, sigma_2, masks=None,
                lambda_scales=2., lambda_hf=2., lambda_positivity=0.,
                subsampling_factor=2.,
                optim_list=None,
                kwargs_optim_list=None,
                method_noise='MC',
-               verbose=True, normalise_data=True):
+               verbose=True, normalise_data=True, show_plots=False):
     """
     Update the PSF model from a provided kernel. It will not use the Moffat and the PSF will entirely be described
-    by the grid of pixel. This function is called in the PSF fitting routine of lenstronomy.
+    by the grid of pixel.
 
     :param kernel_old: array containing the first guess of the kernel (should be the narrow PSF ideally...)
     :param data: arrays containing the observations. Dimension (Nstar x Npix x Npix)
     :param sigma_2: arrays containing the noise maps. Dimension (Nstar x Npix x Npix)
     :param masks: array containing the masks for the PSF (if given)
     :param lambda_scales: Lagrange parameter that weights intermediate scales in the transformed domain.
     :param lambda_hf: Lagrange parameter weighting the highest frequency scale
     :param lambda_positivity: Lagrange parameter weighting the positivity of the full PSF. 0 means no positivity constraint (recommended).
     :param subsampling_factor: int, by how much we supersample the PSF pixel grid compare to data.
     :param optim_list: List of 3 optimisers, one for each step of the fit. Default: ['l-bfgd-b', 'adabelief', 'adabelief']
     :param kwargs_optim_list: List of 3 dictionaries, containing the setting for the different optimiser. Default: None
     :param method_noise: method for noise propagation. Choose 'MC' for an empirical propagation of the noise or 'SLIT' for analytical propagation. Default: 'MC'
     :param verbose: bool, if True, print the progress of the fit. Default: True
     :param normalise_data: bool, if True, renormalise the data before running the fit. Default: True
+    :param show_plots: bool, if True, show the plots of the fit. Default: False
+
+    :return kernel_new: array containing the new full PSF
+    :return narrow_psf: array containing the narrow PSF
+    :return psf_kernel_list: list of arrays containing the PSF kernels fitted to the data
+    :return starred_output: list containing the model, parameters, loss, kwargs_partial_list, LogL_list, loss_history_list, norm
 
     """
     if normalise_data:
         norm = data[0].max()
         data /= norm
         sigma_2 /= norm ** 2
     else:
@@ -404,15 +412,15 @@
     model = PSF(image_size=image_size, number_of_sources=N,
                 upsampling_factor=subsampling_factor,
                 convolution_method='scipy',
                 include_moffat=False)
 
     # Parameter initialization.
     kwargs_init, kwargs_fixed, kwargs_up, kwargs_down = model.smart_guess(data, fixed_background=True,
-                                                                          guess_method='max')
+                                                                          guess_method='center')
     # Fix the background to the previous kernel
     kwargs_init['kwargs_background']['background'] = np.ravel(kernel_old) / np.sum(kernel_old)
     kwargs_fixed['kwargs_background']['background'] = np.ravel(kernel_old) / np.sum(kernel_old)
     parameters = ParametersPSF(kwargs_init, kwargs_fixed, kwargs_up=kwargs_up, kwargs_down=kwargs_down,
                                include_moffat=False)
 
     # Align images (keep background fixed)
@@ -433,18 +441,20 @@
         print('Overall Reduced Chi2 : ', loss.reduced_chi2(kwargs_partial))
 
     # compute noise propagation
     W = propagate_noise(model, np.sqrt(sigma_2), kwargs_partial, masks=masks, wavelet_type_list=['starlet'],
                         method=method_noise, num_samples=500,
                         seed=1, likelihood_type='chi2', verbose=False, upsampling_factor=subsampling_factor)[0]
 
-    # release background, fix positions
+    # release background, fix positions and amplitudes
     kwargs_fixed['kwargs_background'] = {}
     kwargs_fixed['kwargs_gaussian']['x0'] = kwargs_partial['kwargs_gaussian']['x0']
     kwargs_fixed['kwargs_gaussian']['y0'] = kwargs_partial['kwargs_gaussian']['y0']
+    kwargs_fixed['kwargs_gaussian']['a'] = kwargs_partial['kwargs_gaussian']['a']
+
     parameters = ParametersPSF(kwargs_partial, kwargs_fixed, kwargs_up=kwargs_up, kwargs_down=kwargs_down,
                                include_moffat=False)
 
     loss = Loss(data, model, parameters, sigma_2, N, regularization_terms='l1_starlet',
                 regularization_strength_scales=lambda_scales, regularization_strength_hf=lambda_hf,
                 regularization_strength_positivity=lambda_positivity, W=W, regularize_full_psf=False,
                 masks=masks)
@@ -459,26 +469,30 @@
         print('Step 2/3 took %2.f seconds' % (runtime))
         print('Kwargs partial at step 2/3:', kwargs_partial)
         print('LogL : ', logL_best_fit)
         print('Overall Reduced Chi2 : ', loss.reduced_chi2(kwargs_partial))
 
     # Release everything
     kwargs_fixed['kwargs_gaussian'] = {}
-    # Add prior on position to avoid full degeneracy between background and position
-    prior_astrom = Prior(prior_gaussian=[['x0', kwargs_partial['kwargs_gaussian']['x0'], 1.],
-                                         ['y0', kwargs_partial['kwargs_gaussian']['x0'], 1.]],
+    # Add prior on position and photometry to avoid full degeneracy between background and position
+    prior_astrom_photom = Prior(prior_gaussian=[['x0', kwargs_partial['kwargs_gaussian']['x0'], 1.],
+                                                ['y0', kwargs_partial['kwargs_gaussian']['x0'], 1.],
+                                                ['a', kwargs_partial['kwargs_gaussian']['a'],
+                                                 0.1 * kwargs_partial['kwargs_gaussian']['a']],
+                                                ],
                          prior_background=None, prior_moffat=None)
 
+    print('Applying priors on position to avoid degeneracy between background and position')
     parameters = ParametersPSF(kwargs_partial, kwargs_fixed, kwargs_up=kwargs_up, kwargs_down=kwargs_down,
                                include_moffat=False)
 
     loss = Loss(data, model, parameters, sigma_2, N, regularization_terms='l1_starlet',
                 regularization_strength_scales=lambda_scales, regularization_strength_hf=lambda_hf,
                 regularization_strength_positivity=lambda_positivity, W=W, regularize_full_psf=False,
-                masks=masks, prior=prior_astrom)
+                masks=masks, prior=prior_astrom_photom)
     optim = Optimizer(loss, parameters, method=optim_list[2])
     best_fit, logL_best_fit, extra_fields, runtime = optim.minimize(**kwargs_optim_list[2])
 
     kwargs_final = parameters.args2kwargs(best_fit)
     kwargs_partial_list.append(kwargs_final)
     loss_history_list.append(extra_fields['loss_history'])
     LogL_list.append(logL_best_fit)
@@ -487,9 +501,20 @@
         print('Kwargs partial at step 3/3:', kwargs_final)
         print('LogL : ', logL_best_fit)
         print('Overall Reduced Chi2 : ', loss.reduced_chi2(kwargs_final))
 
     starred_output = [model, parameters, loss, kwargs_partial_list, LogL_list, loss_history_list, norm]
     kernel_new = model.get_full_psf(**kwargs_final, norm=True, high_res=True)
     narrow_psf = model.get_narrow_psf(**kwargs_final, norm=True)
+    psf_kernel_list = model.model(**kwargs_final, high_res=False)
+
+    if show_plots:
+        print('Initial data:')
+        fig0 = pltf.display_data(data, sigma_2=sigma_2, masks=masks, units='e-')
+        for i, kwargs_partial in enumerate(kwargs_partial_list):
+            print('Step %i' % i)
+            print(kwargs_partial)
+            fig1 = pltf.multiple_PSF_plot(model, data, sigma_2, kwargs_partial, masks=masks, units='e-')
+            fig_loss1 = pltf.plot_loss(loss_history_list[i])
+            plt.show()
 
-    return kernel_new, narrow_psf, starred_output
+    return kernel_new, narrow_psf, psf_kernel_list, starred_output
```

### Comparing `starred-astro-1.4.2/starred/psf/loss.py` & `starred_astro-1.4.3/starred/psf/loss.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/psf/parameters.py` & `starred_astro-1.4.3/starred/psf/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/psf/psf.py` & `starred_astro-1.4.3/starred/psf/psf.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/utils/ds9reg.py` & `starred_astro-1.4.3/starred/utils/ds9reg.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/utils/generic_utils.py` & `starred_astro-1.4.3/starred/utils/generic_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import jax.scipy.signal
 import numpy as np
 from astropy.io import fits
 from jax import lax, jit
 from jax.numpy.fft import fft2, ifft2
 from functools import partial
 from copy import deepcopy
+import scipy.ndimage
 
 
 def timer_func(func):
     """
     This function shows the execution time of the provided function object.
 
     """
@@ -93,14 +94,47 @@
     m, n = fr.shape
     cc = jnp.real(ifft2(fr * fr2))
     cc = jnp.roll(cc, int(-m / 2), axis=0)
     cc = jnp.roll(cc, int(-n / 2), axis=1)
     return cc
 
 
+def fourier_division(a, b):
+    """
+    Divides two arrays in Fourier space. Work much better with even kernel.
+    To obtain the narrow PSF, a should be the full PSF and b a gaussian with 2pix FWHM.
+    This function makes use of scipy if the kernel are even, and is not yet jaxified
+
+    :param a: first array
+    :param b: second array
+    """
+    assert a.shape == b.shape, "Arrays must have the same shape."
+    assert a.shape[0] == a.shape[1], "Array must be square."
+
+    padding = False  # array must have odd number of pixel
+    if a.shape[0] % 2 == 0:
+        a = jnp.pad(a, ((0, 1), (0, 1)), mode='constant')
+        b = jnp.pad(b, ((0, 1), (0, 1)), mode='constant')
+        padding = True
+
+    A = fft2(a)
+    B = fft2(b)
+    C = A / B
+    cc = jnp.real(ifft2(C))
+    m, n = C.shape
+    cc = jnp.roll(cc, int(-m / 2) - 1, axis=0)
+    cc = jnp.roll(cc, int(-n / 2) - 1, axis=1)
+
+    if padding:
+        # todo: jaxified that if jax.scipy.ndimage.shift is available one day
+        cc = scipy.ndimage.shift(cc, (-0.5, -0.5))[:-1, :-1]
+
+    return cc
+
+
 @jit
 def scipy_convolve(data, kernel):
     """
     FFT-based Scipy convolution.
 
     :param data: first array 
     :param kernel: second array
```

### Comparing `starred-astro-1.4.2/starred/utils/jax_utils.py` & `starred_astro-1.4.3/starred/utils/jax_utils.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/utils/light_profile_analytical.py` & `starred_astro-1.4.3/starred/utils/light_profile_analytical.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/utils/noise_utils.py` & `starred_astro-1.4.3/starred/utils/noise_utils.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred/utils/parameters.py` & `starred_astro-1.4.3/starred/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `starred-astro-1.4.2/starred_astro.egg-info/PKG-INFO` & `starred_astro-1.4.3/starred_astro.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 Metadata-Version: 2.1
 Name: starred-astro
-Version: 1.4.2
+Version: 1.4.3
 Summary: A two-channel deconvolution method with Starlet regularization
-Author: Kevin Michalewicz, Martin Millon, Fred Dux
-Author-email: kevinmicha@hotmail.com
-Requires: astropy
-Requires: dill
-Requires: jax
-Requires: jaxlib
-Requires: jaxopt
-Requires: matplotlib
-Requires: numpy
-Requires: scipy
-Requires: optax
-Requires: tqdm
-Requires: emcee
-Requires: pyregion
-Requires: h5py
+Author: Martin Millon, Frédéric Dux
+Author-email: Kevin Michalewicz <kevinmicha@hotmail.com>
+Project-URL: homepage, https://starred-astro.github.io
+Project-URL: repository, https://github.com/starred/starred-astro
+Keywords: deconvolution,astronomy,starlet,image processing
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
+Requires-Dist: astropy>=5.0.4
+Requires-Dist: dill>=0.3.5.1
+Requires-Dist: jax>=0.4.13
+Requires-Dist: jaxlib>=0.4.13
+Requires-Dist: matplotlib>=3.4.2
+Requires-Dist: numpy>=1.21.2
+Requires-Dist: scipy>=1.10.0
+Requires-Dist: optax>=0.1.7
+Requires-Dist: jaxopt>=0.8
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: h5py>=3.9.0
+Provides-Extra: opt
+Requires-Dist: emcee>=3.1.4; extra == "opt"
+Requires-Dist: mclmc>=0.2.6; extra == "opt"
+Requires-Dist: pyregion>=2.2.0; extra == "opt"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 # STARRED: STARlet REgularized Deconvolution 
 
 [![pipeline status](https://gitlab.com/cosmograil/starred/badges/main/pipeline.svg)](https://gitlab.com/cosmograil/starred/commits/main)
 [![coverage report](https://gitlab.com/cosmograil/starred/badges/main/coverage.svg)](https://cosmograil.gitlab.io/starred/coverage/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `starred-astro-1.4.2/starred_astro.egg-info/SOURCES.txt` & `starred_astro-1.4.3/starred_astro.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 AUTHORS.md
 LICENSE
 README.md
-setup.py
+pyproject.toml
+docs/conf.py
+scripts/1_generate_psf.py
+scripts/2_deconvolve.py
 starred/__init__.py
 starred/deconvolution/__init__.py
 starred/deconvolution/deconvolution.py
 starred/deconvolution/loss.py
 starred/deconvolution/parameters.py
 starred/optim/__init__.py
 starred/optim/inference_base.py
@@ -27,8 +30,24 @@
 starred/utils/jax_utils.py
 starred/utils/light_profile_analytical.py
 starred/utils/noise_utils.py
 starred/utils/parameters.py
 starred_astro.egg-info/PKG-INFO
 starred_astro.egg-info/SOURCES.txt
 starred_astro.egg-info/dependency_links.txt
-starred_astro.egg-info/top_level.txt
+starred_astro.egg-info/requires.txt
+starred_astro.egg-info/top_level.txt
+tests/__init__.py
+tests/test_deconv/__init__.py
+tests/test_deconv/test_deconv.py
+tests/test_deconv/test_deconv_sersic.py
+tests/test_plots/__init__.py
+tests/test_plots/test_plots.py
+tests/test_psf/__init__.py
+tests/test_psf/test_convolution.py
+tests/test_psf/test_distortion.py
+tests/test_psf/test_psf.py
+tests/test_utils/__init__.py
+tests/test_utils/test_jax_utils.py
+tests/test_utils/test_noise.py
+tests/test_utils/test_params.py
+tests/test_utils/test_utils.py
```

