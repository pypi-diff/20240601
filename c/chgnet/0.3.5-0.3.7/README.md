# Comparing `tmp/chgnet-0.3.5.tar.gz` & `tmp/chgnet-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chgnet-0.3.5.tar", last modified: Mon Mar 11 15:42:35 2024, max compression
+gzip compressed data, was "chgnet-0.3.7.tar", last modified: Sat Jun  1 01:06:31 2024, max compression
```

## Comparing `chgnet-0.3.5.tar` & `chgnet-0.3.7.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.426643 chgnet-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-11 15:42:29.000000 chgnet-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-03-11 15:42:35.426643 chgnet-0.3.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    15042 2024-03-11 15:42:29.000000 chgnet-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.406643 chgnet-0.3.5/chgnet/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.410643 chgnet-0.3.5/chgnet/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31587 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.410643 chgnet-0.3.5/chgnet/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/graph/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/graph/crystalgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/graph/cygraph.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/graph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.410643 chgnet-0.3.5/chgnet/model/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/model/basis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/model/composition_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    35216 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/model/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/model/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    35963 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.406643 chgnet-0.3.5/chgnet/pretrained/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.410643 chgnet-0.3.5/chgnet/pretrained/0.2.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1765 2024-03-11 15:42:29.000000 chgnet-0.3.5/chgnet/pretrained/0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  4639235 2024-03-11 15:42:30.000000 chgnet-0.3.5/chgnet/pretrained/0.2.0/chgnet_0.2.0_e30f77s348m32.pth.tar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.418643 chgnet-0.3.5/chgnet/pretrained/0.3.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1872 2024-03-11 15:42:30.000000 chgnet-0.3.5/chgnet/pretrained/0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  4863221 2024-03-11 15:42:30.000000 chgnet-0.3.5/chgnet/pretrained/0.3.0/chgnet_0.3.0_e29f68s314m37.pth.tar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.422643 chgnet-0.3.5/chgnet/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-11 15:42:30.000000 chgnet-0.3.5/chgnet/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27841 2024-03-11 15:42:30.000000 chgnet-0.3.5/chgnet/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.422643 chgnet-0.3.5/chgnet/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-11 15:42:30.000000 chgnet-0.3.5/chgnet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-11 15:42:30.000000 chgnet-0.3.5/chgnet/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-03-11 15:42:30.000000 chgnet-0.3.5/chgnet/utils/vasp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.426643 chgnet-0.3.5/chgnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-03-11 15:42:35.000000 chgnet-0.3.5/chgnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-11 15:42:35.000000 chgnet-0.3.5/chgnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 15:42:35.000000 chgnet-0.3.5/chgnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-11 15:42:35.000000 chgnet-0.3.5/chgnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 15:42:35.000000 chgnet-0.3.5/chgnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-03-11 15:42:30.000000 chgnet-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 15:42:35.426643 chgnet-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-11 15:42:30.000000 chgnet-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 15:42:35.426643 chgnet-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_crystal_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_relaxation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-11 15:42:30.000000 chgnet-0.3.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.454275 chgnet-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-06-01 01:06:26.000000 chgnet-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-06-01 01:06:31.454275 chgnet-0.3.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15042 2024-06-01 01:06:26.000000 chgnet-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.434275 chgnet-0.3.7/chgnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.434275 chgnet-0.3.7/chgnet/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34415 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.434275 chgnet-0.3.7/chgnet/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/graph/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/graph/crystalgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/graph/cygraph.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/graph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.438275 chgnet-0.3.7/chgnet/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/model/basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/model/composition_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34952 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/model/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/model/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35941 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.430275 chgnet-0.3.7/chgnet/pretrained/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.438275 chgnet-0.3.7/chgnet/pretrained/0.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1765 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/pretrained/0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  4639235 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/pretrained/0.2.0/chgnet_0.2.0_e30f77s348m32.pth.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.442275 chgnet-0.3.7/chgnet/pretrained/0.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1872 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/pretrained/0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  4863221 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/pretrained/0.3.0/chgnet_0.3.0_e29f68s314m37.pth.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.450275 chgnet-0.3.7/chgnet/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27831 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.450275 chgnet-0.3.7/chgnet/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-06-01 01:06:26.000000 chgnet-0.3.7/chgnet/utils/vasp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.450275 chgnet-0.3.7/chgnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-06-01 01:06:31.000000 chgnet-0.3.7/chgnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-06-01 01:06:31.000000 chgnet-0.3.7/chgnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:06:31.000000 chgnet-0.3.7/chgnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-06-01 01:06:31.000000 chgnet-0.3.7/chgnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 01:06:31.000000 chgnet-0.3.7/chgnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-06-01 01:06:26.000000 chgnet-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:06:31.454275 chgnet-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-01 01:06:26.000000 chgnet-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:06:31.450275 chgnet-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_crystal_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-06-01 01:06:26.000000 chgnet-0.3.7/tests/test_vasp_utils.py
```

### Comparing `chgnet-0.3.5/LICENSE` & `chgnet-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/PKG-INFO` & `chgnet-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chgnet
-Version: 0.3.5
+Version: 0.3.7
 Summary: Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling
 Author-email: Bowen Deng <bowendeng@berkeley.edu>
 License: Modified BSD
 Project-URL: Source, https://github.com/CederGroupHub/chgnet
 Project-URL: Package, https://pypi.org/project/chgnet
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -15,28 +15,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ase
+Requires-Dist: ase>=3.23.0
 Requires-Dist: cython>=0.29.26
-Requires-Dist: numpy>=1.21.6
+Requires-Dist: numpy>=1.26
 Requires-Dist: nvidia-ml-py3>=7.352.0
 Requires-Dist: pymatgen>=2023.10.11
 Requires-Dist: torch>=1.11.0
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-cov>=4; extra == "test"
+Requires-Dist: pytest>=8; extra == "test"
 Provides-Extra: examples
-Requires-Dist: crystal-toolkit; extra == "examples"
-Requires-Dist: pandas; extra == "examples"
+Requires-Dist: crystal-toolkit>=2023.11.3; extra == "examples"
+Requires-Dist: pandas>=2.2; extra == "examples"
 Provides-Extra: docs
-Requires-Dist: lazydocs; extra == "docs"
+Requires-Dist: lazydocs>=0.4; extra == "docs"
 
 <h1 align="center">CHGNet</h1>
 
 <h4 align="center">
 
 [![Tests](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e3bdcea0382a495d96408e4f84408e85)](https://app.codacy.com/gh/CederGroupHub/chgnet/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
```

### Comparing `chgnet-0.3.5/README.md` & `chgnet-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/chgnet/data/dataset.py` & `chgnet-0.3.7/chgnet/data/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,61 +29,115 @@
     """A simple torch Dataset of structures."""
 
     def __init__(
         self,
         structures: list[Structure],
         energies: list[float],
         forces: list[Sequence[Sequence[float]]],
+        *,
         stresses: list[Sequence[Sequence[float]]] | None = None,
         magmoms: list[Sequence[Sequence[float]]] | None = None,
-        structure_ids: list[str] | None = None,
+        structure_ids: list | None = None,
         graph_converter: CrystalGraphConverter | None = None,
+        shuffle: bool = True,
     ) -> None:
         """Initialize the dataset.
 
         Args:
             structures (list[dict]): pymatgen Structure objects.
             energies (list[float]): [data_size, 1]
             forces (list[list[float]]): [data_size, n_atoms, 3]
             stresses (list[list[float]], optional): [data_size, 3, 3]
+                Default = None
             magmoms (list[list[float]], optional): [data_size, n_atoms, 1]
-            structure_ids (list[str], optional): a list of ids to track the structures
+                Default = None
+            structure_ids (list, optional): a list of ids to track the structures
+                Default = None
             graph_converter (CrystalGraphConverter, optional): Converts the structures
                 to graphs. If None, it will be set to CHGNet 0.3.0 converter
                 with AtomGraph cutoff = 6A.
+            shuffle (bool): whether to shuffle the sequence of dataset
+                Default = True
 
         Raises:
             RuntimeError: if the length of structures and labels (energies, forces,
                 stresses, magmoms) are not equal.
         """
         for idx, struct in enumerate(structures):
             if not isinstance(struct, Structure):
-                raise ValueError(f"{idx} is not a pymatgen Structure object: {struct}")
+                raise TypeError(f"{idx} is not a pymatgen Structure object: {struct}")
         for name in "energies forces stresses magmoms structure_ids".split():
             labels = locals()[name]
             if labels is not None and len(labels) != len(structures):
                 raise RuntimeError(
                     f"Inconsistent number of structures and labels: "
                     f"{len(structures)=}, len({name})={len(labels)}"
                 )
         self.structures = structures
         self.energies = energies
         self.forces = forces
         self.stresses = stresses
         self.magmoms = magmoms
         self.structure_ids = structure_ids
         self.keys = np.arange(len(structures))
-        random.shuffle(self.keys)
-        print(f"{len(structures)} structures imported")
+        if shuffle:
+            random.shuffle(self.keys)
+        print(f"{type(self).__name__} imported {len(structures):,} structures")
         self.graph_converter = graph_converter or CrystalGraphConverter(
             atom_graph_cutoff=6, bond_graph_cutoff=3
         )
         self.failed_idx: list[int] = []
         self.failed_graph_id: dict[str, str] = {}
 
+    @classmethod
+    def from_vasp(
+        cls,
+        file_root: str,
+        *,
+        check_electronic_convergence: bool = True,
+        save_path: str | None = None,
+        graph_converter: CrystalGraphConverter | None = None,
+        shuffle: bool = True,
+    ) -> StructureData:
+        """Parse VASP output files into structures and labels and feed into the dataset.
+
+        Args:
+            file_root (str): the directory of the VASP calculation outputs
+            check_electronic_convergence (bool): if set to True, this function will
+                raise Exception to VASP calculation that did not achieve
+                electronic convergence.
+                Default = True
+            save_path (str): path to save the parsed VASP labels
+                Default = None
+            graph_converter (CrystalGraphConverter, optional): Converts the structures
+                to graphs. If None, it will be set to CHGNet 0.3.0 converter
+                with AtomGraph cutoff = 6A.
+            shuffle (bool): whether to shuffle the sequence of dataset
+                Default = True
+        """
+        result_dict = utils.parse_vasp_dir(
+            base_dir=file_root,
+            check_electronic_convergence=check_electronic_convergence,
+            save_path=save_path,
+        )
+        return cls(
+            structures=result_dict["structure"],
+            energies=result_dict["energy_per_atom"],
+            forces=result_dict["force"],
+            stresses=None
+            if result_dict["stress"] in [None, []]
+            else result_dict["stress"],
+            magmoms=None
+            if result_dict["magmom"] in [None, []]
+            else result_dict["magmom"],
+            structure_ids=np.arange(len(result_dict["structure"])),
+            graph_converter=graph_converter,
+            shuffle=shuffle,
+        )
+
     def __len__(self) -> int:
         """Get the number of structures in this dataset."""
         return len(self.keys)
 
     @functools.cache  # Cache loaded structures
     def __getitem__(self, idx: int) -> tuple[CrystalGraph, dict]:
         """Get one graph for a structure in this dataset.
@@ -140,45 +194,50 @@
 
 class CIFData(Dataset):
     """A dataset from CIFs."""
 
     def __init__(
         self,
         cif_path: str,
+        *,
         labels: str | dict = "labels.json",
         targets: TrainTask = "efsm",
         graph_converter: CrystalGraphConverter | None = None,
         energy_key: str = "energy_per_atom",
         force_key: str = "force",
         stress_key: str = "stress",
         magmom_key: str = "magmom",
+        shuffle: bool = True,
     ) -> None:
         """Initialize the dataset from a directory containing CIFs.
 
         Args:
             cif_path (str): path that contain all the graphs, labels.json
             labels (str, dict): the path or dictionary of labels
             targets ("ef" | "efs" | "efm" | "efsm"): The training targets.
                 Default = "efsm"
             graph_converter (CrystalGraphConverter, optional): Converts the structures
                 to graphs. If None, it will be set to CHGNet 0.3.0 converter
                 with AtomGraph cutoff = 6A.
             energy_key (str, optional): the key of energy in the labels.
-                Default = "energy_per_atom".
+                Default = "energy_per_atom"
             force_key (str, optional): the key of force in the labels.
-                Default = "force".
+                Default = "force"
             stress_key (str, optional): the key of stress in the labels.
-                Default = "stress".
+                Default = "stress"
             magmom_key (str, optional): the key of magmom in the labels.
-                Default = "magmom".
+                Default = "magmom"
+            shuffle (bool): whether to shuffle the sequence of dataset
+                Default = True
         """
         self.data_dir = cif_path
         self.data = utils.read_json(os.path.join(cif_path, labels))
         self.cif_ids = list(self.data)
-        random.shuffle(self.cif_ids)
+        if shuffle:
+            random.shuffle(self.cif_ids)
         print(f"{cif_path}: {len(self.cif_ids):,} structures imported")
         self.graph_converter = graph_converter or CrystalGraphConverter(
             atom_graph_cutoff=6, bond_graph_cutoff=3
         )
 
         self.energy_key = energy_key
         self.force_key = force_key
@@ -251,40 +310,44 @@
     """A dataset of graphs. This is compatible with the graph.pt documents made by
     make_graphs.py. We recommend you to use the dataset to avoid graph conversion steps.
     """
 
     def __init__(
         self,
         graph_path: str,
+        *,
         labels: str | dict = "labels.json",
         targets: TrainTask = "efsm",
         exclude: str | list | None = None,
         energy_key: str = "energy_per_atom",
         force_key: str = "force",
         stress_key: str = "stress",
         magmom_key: str = "magmom",
+        shuffle: bool = True,
     ) -> None:
         """Initialize the dataset from a directory containing saved crystal graphs.
 
         Args:
             graph_path (str): path that contain all the graphs, labels.json
             labels (str, dict): the path or dictionary of labels.
                 Default = "labels.json"
             targets ("ef" | "efs" | "efm" | "efsm"): The training targets.
                 Default = "efsm"
             exclude (str, list | None): the path or list of excluded graphs.
                 Default = None
             energy_key (str, optional): the key of energy in the labels.
-                Default = "energy_per_atom".
+                Default = "energy_per_atom"
             force_key (str, optional): the key of force in the labels.
-                Default = "force".
+                Default = "force"
             stress_key (str, optional): the key of stress in the labels.
-                Default = "stress".
+                Default = "stress"
             magmom_key (str, optional): the key of magmom in the labels.
-                Default = "magmom".
+                Default = "magmom"
+            shuffle (bool): whether to shuffle the sequence of dataset
+                Default = True
         """
         self.graph_path = graph_path
         if isinstance(labels, str):
             labels = os.path.join(graph_path, labels)
             print(f"Importing: {labels}")
             self.labels = utils.read_json(labels)
         elif isinstance(labels, dict):
@@ -296,15 +359,16 @@
             self.excluded_graph = exclude
         else:
             self.excluded_graph = []
 
         self.keys = [
             (mp_id, graph_id) for mp_id, dic in self.labels.items() for graph_id in dic
         ]
-        random.shuffle(self.keys)
+        if shuffle:
+            random.shuffle(self.keys)
         print(f"{len(self.labels)} mp_ids, {len(self)} frames imported")
         if self.excluded_graph is not None:
             print(f"{len(self.excluded_graph)} graphs are pre-excluded")
 
         self.energy_key = energy_key
         self.force_key = force_key
         self.stress_key = stress_key
@@ -365,14 +429,15 @@
             idx = random.randint(0, len(self) - 1)
             return self.__getitem__(idx)
 
     def get_train_val_test_loader(
         self,
         train_ratio: float = 0.8,
         val_ratio: float = 0.1,
+        *,
         train_key: list[str] | None = None,
         val_key: list[str] | None = None,
         test_key: list[str] | None = None,
         batch_size=32,
         num_workers=0,
         pin_memory=True,
     ) -> tuple[DataLoader, DataLoader, DataLoader]:
@@ -477,72 +542,77 @@
     This class is used to load the MPtrj dataset.
     """
 
     def __init__(
         self,
         data: str | dict,
         graph_converter: CrystalGraphConverter,
+        *,
         targets: TrainTask = "efsm",
         energy_key: str = "energy_per_atom",
         force_key: str = "force",
         stress_key: str = "stress",
         magmom_key: str = "magmom",
+        shuffle: bool = True,
     ) -> None:
         """Initialize the dataset by reading JSON files.
 
         Args:
             data (str | dict): file path or dir name that contain all the JSONs
             graph_converter (CrystalGraphConverter): Converts pymatgen.core.Structure
                 to CrystalGraph object.
             targets ("ef" | "efs" | "efm" | "efsm"): The training targets.
                 Default = "efsm"
             energy_key (str, optional): the key of energy in the labels.
-                Default = "energy_per_atom".
+                Default = "energy_per_atom"
             force_key (str, optional): the key of force in the labels.
-                Default = "force".
+                Default = "force"
             stress_key (str, optional): the key of stress in the labels.
-                Default = "stress".
+                Default = "stress"
             magmom_key (str, optional): the key of magmom in the labels.
-                Default = "magmom".
+                Default = "magmom"
+            shuffle (bool): whether to shuffle the sequence of dataset
+                Default = True
         """
         if isinstance(data, str):
             self.data = {}
             if os.path.isdir(data):
                 for json_path in os.listdir(data):
                     if json_path.endswith(".json"):
                         print(f"Importing: {json_path}")
                         self.data.update(utils.read_json(os.path.join(data, json_path)))
             else:
                 print(f"Importing: {data}")
                 self.data.update(utils.read_json(data))
         elif isinstance(data, dict):
             self.data = data
         else:
-            raise ValueError(f"data must be JSON path or dictionary, got {type(data)}")
+            raise TypeError(f"data must be JSON path or dictionary, got {type(data)}")
 
         self.keys = [
             (mp_id, graph_id) for mp_id, dct in self.data.items() for graph_id in dct
         ]
-        random.shuffle(self.keys)
-        print(f"{len(self.data)} mp_ids, {len(self)} structures imported")
+        if shuffle:
+            random.shuffle(self.keys)
+        print(f"{len(self.data)} MP IDs, {len(self)} structures imported")
         self.graph_converter = graph_converter
         self.energy_key = energy_key
         self.force_key = force_key
         self.stress_key = stress_key
         self.magmom_key = magmom_key
         self.targets = targets
         self.failed_idx: list[int] = []
         self.failed_graph_id: dict[str, str] = {}
 
     def __len__(self) -> int:
         """Get the number of structures with targets in the dataset."""
         return len(self.keys)
 
     @functools.cache  # Cache loaded structures
-    def __getitem__(self, idx):
+    def __getitem__(self, idx: int) -> tuple[CrystalGraph, dict[str, Tensor]]:
         """Get one item in the dataset.
 
         Returns:
             crystal_graph (CrystalGraph): graph of the crystal structure
             targets (dict): dictionary of targets. i.e. energy, force, stress, magmom
         """
         if idx not in self.failed_idx:
@@ -586,14 +656,15 @@
             idx = random.randint(0, len(self) - 1)
             return self.__getitem__(idx)
 
     def get_train_val_test_loader(
         self,
         train_ratio: float = 0.8,
         val_ratio: float = 0.1,
+        *,
         train_key: list[str] | None = None,
         val_key: list[str] | None = None,
         test_key: list[str] | None = None,
         batch_size=32,
         num_workers=0,
         pin_memory=True,
     ) -> tuple[DataLoader, DataLoader, DataLoader]:
@@ -679,15 +750,15 @@
                 pin_memory=pin_memory,
             )
         else:
             test_loader = None
         return train_loader, val_loader, test_loader
 
 
-def collate_graphs(batch_data: list):
+def collate_graphs(batch_data: list) -> tuple[list[CrystalGraph], dict[str, Tensor]]:
     """Collate of list of (graph, target) into batch data.
 
     Args:
         batch_data (list): list of (graph, target(dict))
 
     Returns:
         graphs (List): a list of graphs
@@ -709,21 +780,22 @@
                 all_targets[target].append(value)
 
     return graphs, all_targets
 
 
 def get_train_val_test_loader(
     dataset: Dataset,
+    *,
     batch_size: int = 64,
     train_ratio: float = 0.8,
     val_ratio: float = 0.1,
     return_test: bool = True,
     num_workers: int = 0,
     pin_memory: bool = True,
-):
+) -> tuple[DataLoader, DataLoader, DataLoader]:
     """Randomly partition a dataset into train, val, test loaders.
 
     Args:
         dataset (Dataset): The dataset to partition.
         batch_size (int): The batch size for the data loaders
             Default = 64
         train_ratio (float): The ratio of the dataset to use for training
@@ -774,15 +846,17 @@
             num_workers=num_workers,
             pin_memory=pin_memory,
         )
         return train_loader, val_loader, test_loader
     return train_loader, val_loader
 
 
-def get_loader(dataset, batch_size=64, num_workers=0, pin_memory=True):
+def get_loader(
+    dataset, *, batch_size: int = 64, num_workers: int = 0, pin_memory: bool = True
+) -> DataLoader:
     """Get a dataloader from a dataset.
 
     Args:
         dataset (Dataset): The dataset to partition.
         batch_size (int): The batch size for the data loaders
             Default = 64
         num_workers (int): The number of worker processes for loading the data
```

### Comparing `chgnet-0.3.5/chgnet/graph/converter.py` & `chgnet-0.3.7/chgnet/graph/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     gradients like force and stress can be calculated through back-propagation later.
     """
 
     make_graph = None
 
     def __init__(
         self,
+        *,
         atom_graph_cutoff: float = 6,
         bond_graph_cutoff: float = 3,
         algorithm: Literal["legacy", "fast"] = "fast",
         on_isolated_atoms: Literal["ignore", "warn", "error"] = "error",
         verbose: bool = False,
     ) -> None:
         """Initialize the Crystal Graph Converter.
@@ -270,15 +271,14 @@
                 with isolated atoms.
                 Default = 'error'.
 
         Returns:
             None
         """
         self.on_isolated_atoms = on_isolated_atoms
-        return
 
     def as_dict(self) -> dict[str, str | float]:
         """Save the args of the graph converter."""
         return {
             "atom_graph_cutoff": self.atom_graph_cutoff,
             "bond_graph_cutoff": self.bond_graph_cutoff,
             "algorithm": self.algorithm,
```

### Comparing `chgnet-0.3.5/chgnet/graph/crystalgraph.py` & `chgnet-0.3.7/chgnet/graph/crystalgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         bond_graph_len = len(self.bond_graph)
         return (
             f"CrystalGraph({composition=}, {atom_graph_cutoff=}, {bond_graph_cutoff=}, "
             f"{n_atoms=}, {atom_graph_len=}, {bond_graph_len=})"
         )
 
     @property
-    def num_isolated_atoms(self):
+    def num_isolated_atoms(self) -> int:
         """Number of isolated atoms given the atom graph cutoff
         Isolated atoms are disconnected nodes in the atom graph
         that will not get updated in CHGNet.
         These atoms will always have calculated force equal to zero.
 
         With the default CHGNet atom graph cutoff radius, only ~ 0.1% of MPtrj dataset
         structures has isolated atoms.
```

### Comparing `chgnet-0.3.5/chgnet/graph/cygraph.pyx` & `chgnet-0.3.7/chgnet/graph/cygraph.pyx`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/chgnet/graph/graph.py` & `chgnet-0.3.7/chgnet/graph/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             index (int): the index of this node
             info (dict, optional): any additional information about this node.
         """
         self.index = index
         self.info = info
         self.neighbors: dict[int, list[DirectedEdge | UndirectedEdge]] = {}
 
-    def add_neighbor(self, index, edge):
+    def add_neighbor(self, index, edge) -> None:
         """Draw an directed edge between self and the node specified by index.
 
         Args:
             index (int): the index of neighboring node
             edge (DirectedEdge): an DirectedEdge object pointing from self to the node.
         """
         if index not in self.neighbors:
@@ -40,15 +40,15 @@
         self, nodes: list, index: int | None = None, info: dict | None = None
     ) -> None:
         """Initialize an Edge."""
         self.nodes = nodes
         self.index = index
         self.info = info
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """String representation of this edge."""
         nodes, index, info = self.nodes, self.index, self.info
         return f"{type(self).__name__}({nodes=}, {index=}, {info=})"
 
     def __hash__(self) -> int:
         """Hash this edge."""
         img = (self.info or {}).get("image")
@@ -62,15 +62,15 @@
 
 
 class UndirectedEdge(Edge):
     """An undirected/bi-directed edge in a graph."""
 
     __hash__ = Edge.__hash__
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         """Check if two undirected edges are equal."""
         return set(self.nodes) == set(other.nodes) and self.info == other.info
 
 
 class DirectedEdge(Edge):
     """A directed edge in a graph."""
 
@@ -174,24 +174,24 @@
             for undirected_edge in self.undirected_edges[tmp]:
                 if (
                     abs(undirected_edge.info["distance"] - distance) < 1e-6
                     and len(undirected_edge.info["directed_edge_index"]) == 1
                 ):
                     # There is an undirected edge with similar length and only one of
                     # the directed edges associated has been added
-                    added_DE = self.directed_edges_list[
+                    added_dir_edge = self.directed_edges_list[
                         undirected_edge.info["directed_edge_index"][0]
                     ]
 
                     # See if the DE that's associated to this UDE
                     # is the reverse of our DE
-                    if added_DE == this_directed_edge:
+                    if added_dir_edge == this_directed_edge:
                         # Add UDE index to this DE
                         this_directed_edge.info["undirected_edge_index"] = (
-                            added_DE.info["undirected_edge_index"]
+                            added_dir_edge.info["undirected_edge_index"]
                         )
 
                         # At the center node, draw edge with this DE
                         self.nodes[center_index].add_neighbor(
                             neighbor_index, this_directed_edge
                         )
 
@@ -213,15 +213,15 @@
                 info={"directed_edge_index": [directed_edge_index]},
             )
             self.undirected_edges[tmp].append(this_undirected_edge)
             self.undirected_edges_list.append(this_undirected_edge)
             self.nodes[center_index].add_neighbor(neighbor_index, this_directed_edge)
             self.directed_edges_list.append(this_directed_edge)
 
-    def adjacency_list(self):
+    def adjacency_list(self) -> tuple[list[list[int]], list[int]]:
         """Get the adjacency list
         Return:
             graph: the adjacency list
                 [[0, 1],
                  [0, 2],
                  ...
                  [5, 2]
@@ -236,15 +236,15 @@
         """
         graph = [edge.nodes for edge in self.directed_edges_list]
         directed2undirected = [
             edge.info["undirected_edge_index"] for edge in self.directed_edges_list
         ]
         return graph, directed2undirected
 
-    def line_graph_adjacency_list(self, cutoff):
+    def line_graph_adjacency_list(self, cutoff) -> tuple[list[list[int]], list[int]]:
         """Get the line graph adjacency list.
 
         Args:
             cutoff (float): a float to indicate the maximum edge length to be included
                 in constructing the line graph, this is used to decrease computation
                 complexity
 
@@ -260,19 +260,20 @@
                 the fourth column specifies 2nd undirected edge(right bond) index,
                 the fifth column specifies 2nd directed edge(right bond) index,.
             undirected2directed:
                 [32, 45, ...]
                 a list of length = num_undirected_edge that
                 maps the undirected edge index to one of its directed edges indices
         """
-        assert len(self.directed_edges_list) == 2 * len(self.undirected_edges_list), (
-            f"Error: number of directed edges={len(self.directed_edges_list)} != 2 * "
-            f"number of undirected edges={len(self.directed_edges_list)}!"
-            f"This indicates directed edges are not complete"
-        )
+        if len(self.directed_edges_list) != 2 * len(self.undirected_edges_list):
+            raise ValueError(
+                f"Error: number of directed edges={len(self.directed_edges_list)} != 2 "
+                f"* number of undirected edges={len(self.directed_edges_list)}!"
+                f"This indicates directed edges are not complete"
+            )
         line_graph = []
         undirected2directed = []
 
         # Loop through all the undirected edges(UDE)
         for u_edge in self.undirected_edges_list:
             # Create the mapping from the UDE index to one of its DE index
             undirected2directed.append(u_edge.info["directed_edge_index"][0])
@@ -281,66 +282,69 @@
             if u_edge.info["distance"] > cutoff:
                 continue
 
             # Assert if the UDE is valid
             # if encountered exception,
             # it means after Atom_Graph creation, the UDE has only 1 DE associated
             # This exception is not encountered from the develop team's experience
-            assert len(u_edge.info["directed_edge_index"]) == 2, (
-                "Did not find 2 Directed_edges !!!"
-                f"undirected edge {u_edge} has:"
-                f"edge.info['directed_edge_index'] = "
-                f"{u_edge.info['directed_edge_index']}"
-                f"len directed_edges_list = {len(self.directed_edges_list)}"
-                f"len undirected_edges_list = {len(self.undirected_edges_list)}"
-            )
+            if len(u_edge.info["directed_edge_index"]) != 2:
+                raise ValueError(
+                    "Did not find 2 Directed_edges !!!"
+                    f"undirected edge {u_edge} has:"
+                    f"edge.info['directed_edge_index'] = "
+                    f"{u_edge.info['directed_edge_index']}"
+                    f"len directed_edges_list = {len(self.directed_edges_list)}"
+                    f"len undirected_edges_list = {len(self.undirected_edges_list)}"
+                )
 
             # This UDE is valid to be considered as a node in Bond_Graph
 
             # Get the two ends (centers) and the two DE associated with this UDE
             # DE1 should have center=center1 and DE2 should have center=center2
             # We will need to find directed edges with center = center1
             # and create angles with DE1, then do the same for center2 and DE2
-            for center, DE in zip(u_edge.nodes, u_edge.info["directed_edge_index"]):
+            for center, dir_edge in zip(
+                u_edge.nodes, u_edge.info["directed_edge_index"]
+            ):
                 for directed_edges in self.nodes[center].neighbors.values():
                     for directed_edge in directed_edges:
-                        if directed_edge.index == DE:
+                        if directed_edge.index == dir_edge:
                             continue
                         if directed_edge.info["distance"] < cutoff:
                             line_graph.append(
                                 [
                                     center,
                                     u_edge.index,
-                                    DE,
+                                    dir_edge,
                                     directed_edge.info["undirected_edge_index"],
                                     directed_edge.index,
                                 ]
                             )
         return line_graph, undirected2directed
 
-    def undirected2directed(self):
+    def undirected2directed(self) -> list[int]:
         """The index map from undirected_edge index to one of its directed_edge
         index.
         """
         return [
             undirected_edge.info["directed_edge_index"][0]
             for undirected_edge in self.undirected_edges_list
         ]
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         """Return dictionary serialization of a Graph."""
         return {
             "nodes": self.nodes,
             "directed_edges": self.directed_edges,
             "directed_edges_list": self.directed_edges_list,
             "undirected_edges": self.undirected_edges,
             "undirected_edges_list": self.undirected_edges_list,
         }
 
-    def to(self, filename="graph.json"):
+    def to(self, filename="graph.json") -> None:
         """Save graph dictionary to file."""
         write_json(self.as_dict(), filename)
 
     def __repr__(self) -> str:
         """Return string representation of the Graph."""
         num_nodes = len(self.nodes)
         num_directed_edges = len(self.directed_edges_list)
```

### Comparing `chgnet-0.3.5/chgnet/model/basis.py` & `chgnet-0.3.7/chgnet/model/basis.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch
 from torch import Tensor, nn
 
 
 class Fourier(nn.Module):
     """Fourier Expansion for angle features."""
 
-    def __init__(self, order: int = 5, learnable: bool = False) -> None:
+    def __init__(self, *, order: int = 5, learnable: bool = False) -> None:
         """Initialize the Fourier expansion.
 
         Args:
             order (int): the maximum order, refer to the N in eq 1 in CHGNet paper
                 Default = 5
             learnable (bool): whether to set the frequencies as learnable parameters
                 Default = False
@@ -43,14 +43,15 @@
 class RadialBessel(torch.nn.Module):
     """1D Bessel Basis
     from: https://github.com/TUM-DAML/gemnet_pytorch/.
     """
 
     def __init__(
         self,
+        *,
         num_radial: int = 9,
         cutoff: float = 5,
         learnable: bool = False,
         smooth_cutoff: int = 5,
     ) -> None:
         """Initialize the SmoothRBF function.
 
@@ -86,15 +87,15 @@
             self.smooth_cutoff = CutoffPolynomial(
                 cutoff=cutoff, cutoff_coeff=smooth_cutoff
             )
         else:
             self.smooth_cutoff = None
 
     def forward(
-        self, dist: Tensor, return_smooth_factor: bool = False
+        self, dist: Tensor, *, return_smooth_factor: bool = False
     ) -> Tensor | tuple[Tensor, Tensor]:
         """Apply Bessel expansion to a feature Tensor.
 
         Args:
             dist (Tensor): tensor of distances [n, 1]
             return_smooth_factor (bool): whether to return the smooth factor
                 Default = False
@@ -118,31 +119,33 @@
 class GaussianExpansion(nn.Module):
     """Expands the distance by Gaussian basis.
     Unit: angstrom.
     """
 
     def __init__(
         self,
-        min: float = 0,
-        max: float = 5,
+        min: float = 0,  # noqa: A002
+        max: float = 5,  # noqa: A002
         step: float = 0.5,
         var: float | None = None,
     ) -> None:
         """Gaussian Expansion
         expand a scalar feature to a soft-one-hot feature vector.
 
         Args:
             min (float): minimum Gaussian center value
             max (float): maximum Gaussian center value
             step (float): Step size between the Gaussian centers
             var (float): variance in gaussian filter, default to step
         """
         super().__init__()
-        assert min < max
-        assert max - min > step
+        if min >= max:
+            raise ValueError(f"{min=} must be less than {max=}")
+        if max - min <= step:
+            raise ValueError(f"{max - min=} must be greater than {step=}")
         self.register_buffer("gaussian_centers", torch.arange(min, max + step, step))
         self.var = var or step
         if self.var <= 0:
             raise ValueError(f"{var=} must be positive")
 
     def expand(self, features: Tensor) -> Tensor:
         """Apply Gaussian filter to a feature Tensor.
```

### Comparing `chgnet-0.3.5/chgnet/model/composition_model.py` & `chgnet-0.3.7/chgnet/model/composition_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 from pymatgen.core import Structure
 from torch import Tensor, nn
 
 from chgnet.model.functions import GatedMLP, find_activation
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
+    from pathlib import Path
 
     from chgnet.graph.crystalgraph import CrystalGraph
 
 
 class CompositionModel(nn.Module):
     """A simple FC model that takes in a chemical composition (no structure info)
     and outputs energy.
     """
 
     def __init__(
         self,
+        *,
         atom_fea_dim: int = 64,
         activation: str = "silu",
         is_intensive: bool = True,
         max_num_elements: int = 94,
     ) -> None:
         """Initialize a CompositionModel."""
         super().__init__()
@@ -57,15 +59,15 @@
         return self.fc2(composition_feas).view(-1)
 
     def forward(self, graphs: list[CrystalGraph]) -> Tensor:
         """Get the energy of a list of CrystalGraphs as Tensor."""
         composition_feas = self._assemble_graphs(graphs)
         return self._get_energy(composition_feas)
 
-    def _assemble_graphs(self, graphs: list[CrystalGraph]):
+    def _assemble_graphs(self, graphs: list[CrystalGraph]) -> Tensor:
         """Assemble a list of graphs into one-hot composition encodings.
 
         Args:
             graphs (list[CrystalGraph]): a list of CrystalGraphs
 
         Returns:
             assembled batch_graph that contains all information for model.
@@ -83,32 +85,35 @@
 
 
 class AtomRef(nn.Module):
     """A linear regression for elemental energy.
     From: https://github.com/materialsvirtuallab/m3gnet/.
     """
 
-    def __init__(self, is_intensive: bool = True, max_num_elements: int = 94) -> None:
+    def __init__(
+        self, *, is_intensive: bool = True, max_num_elements: int = 94
+    ) -> None:
         """Initialize an AtomRef model."""
         super().__init__()
         self.is_intensive = is_intensive
         self.max_num_elements = max_num_elements
         self.fc = nn.Linear(max_num_elements, 1, bias=False)
         self.fitted = False
 
-    def forward(self, graphs: list[CrystalGraph]):
+    def forward(self, graphs: list[CrystalGraph]) -> Tensor:
         """Get the energy of a list of CrystalGraphs.
 
         Args:
             graphs (List(CrystalGraph)): a list of Crystal Graph to compute
 
         Returns:
             energy (tensor)
         """
-        assert self.fitted is True, "composition model need to be fitted first!"
+        if not self.fitted:
+            raise ValueError("composition model needs to be fitted first!")
         composition_feas = self._assemble_graphs(graphs)
         return self._get_energy(composition_feas)
 
     def _get_energy(self, composition_feas: Tensor) -> Tensor:
         """Predict the energy given composition encoding.
 
         Args:
@@ -163,15 +168,15 @@
             @ self.feature_matrix.T
             @ self.energies
         )
         state_dict["weight"] = torch.tensor(weight).view(1, 94)
         self.fc.load_state_dict(state_dict)
         self.fitted = True
 
-    def _assemble_graphs(self, graphs: list[CrystalGraph]):
+    def _assemble_graphs(self, graphs: list[CrystalGraph]) -> Tensor:
         """Assemble a list of graphs into one-hot composition encodings
         Args:
             graphs (list[Tensor]): a list of CrystalGraphs
         Returns:
             assembled batch_graph that contains all information for model.
         """
         composition_feas = []
@@ -181,38 +186,38 @@
             )
             if self.is_intensive:
                 n_atom = graph.atomic_number.shape[0]
                 composition_fea = composition_fea / n_atom
             composition_feas.append(composition_fea)
         return torch.stack(composition_feas, dim=0).float()
 
-    def get_site_energies(self, graphs: list[CrystalGraph]):
+    def get_site_energies(self, graphs: list[CrystalGraph]) -> list[Tensor]:
         """Predict the site energies given a list of CrystalGraphs.
 
         Args:
             graphs (List(CrystalGraph)): a list of Crystal Graph to compute
 
         Returns:
             a list of tensors corresponding to site energies of each graph [batchsize].
         """
         return [
             self.fc.state_dict()["weight"][0, graph.atomic_number - 1]
             for graph in graphs
         ]
 
-    def initialize_from(self, dataset: str):
+    def initialize_from(self, dataset: str) -> None:
         """Initialize pre-fitted weights from a dataset."""
-        if dataset in ["MPtrj", "MPtrj_e"]:
+        if dataset in {"MPtrj", "MPtrj_e"}:
             self.initialize_from_MPtrj()
         elif dataset == "MPF":
             self.initialize_from_MPF()
         else:
             raise NotImplementedError(f"{dataset=} not supported yet")
 
-    def initialize_from_MPtrj(self):
+    def initialize_from_MPtrj(self) -> None:  # noqa: N802
         """Initialize pre-fitted weights from MPtrj dataset."""
         state_dict = collections.OrderedDict()
         state_dict["weight"] = torch.tensor(
             [
                 -3.4431,
                 -0.1279,
                 -2.8300,
@@ -309,15 +314,15 @@
                 -14.2530,
             ]
         ).view([1, 94])
         self.fc.load_state_dict(state_dict)
         self.is_intensive = True
         self.fitted = True
 
-    def initialize_from_MPF(self):
+    def initialize_from_MPF(self) -> None:  # noqa: N802
         """Initialize pre-fitted weights from MPF dataset."""
         state_dict = collections.OrderedDict()
         state_dict["weight"] = torch.tensor(
             [
                 -3.4654e00,
                 -6.2617e-01,
                 -3.4622e00,
@@ -414,15 +419,15 @@
                 -1.5473e01,
             ]
         ).view([1, 94])
         self.fc.load_state_dict(state_dict)
         self.is_intensive = False
         self.fitted = True
 
-    def initialize_from_numpy(self, file_name):
+    def initialize_from_numpy(self, file_name: str | Path) -> None:
         """Initialize pre-fitted weights from numpy file."""
         atom_ref_np = np.load(file_name)
         state_dict = collections.OrderedDict()
         state_dict["weight"] = torch.tensor(atom_ref_np).view([1, 94])
         self.fc.load_state_dict(state_dict)
         self.is_intensive = False
         self.fitted = True
```

### Comparing `chgnet-0.3.5/chgnet/model/dynamics.py` & `chgnet-0.3.7/chgnet/model/dynamics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
 import contextlib
 import inspect
 import io
-import os
 import pickle
 import sys
 from typing import TYPE_CHECKING, Literal
 
 import numpy as np
-import torch
 from ase import Atoms, units
 from ase.calculators.calculator import Calculator, all_changes, all_properties
 from ase.md.npt import NPT
 from ase.md.nptberendsen import Inhomogeneous_NPTBerendsen, NPTBerendsen
 from ase.md.nvtberendsen import NVTBerendsen
 from ase.md.velocitydistribution import MaxwellBoltzmannDistribution, Stationary
 from ase.md.verlet import VelocityVerlet
@@ -24,15 +22,15 @@
 from ase.optimize.mdmin import MDMin
 from ase.optimize.sciopt import SciPyFminBFGS, SciPyFminCG
 from pymatgen.analysis.eos import BirchMurnaghan
 from pymatgen.core.structure import Molecule, Structure
 from pymatgen.io.ase import AseAtomsAdaptor
 
 from chgnet.model.model import CHGNet
-from chgnet.utils import cuda_devices_sorted_by_free_mem
+from chgnet.utils import determine_device
 
 if TYPE_CHECKING:
     from ase.io import Trajectory
     from ase.optimize.optimize import Optimizer
 
 # We would like to thank M3GNet develop team for this module
 # source: https://github.com/materialsvirtuallab/m3gnet
@@ -53,53 +51,63 @@
     """CHGNet Calculator for ASE applications."""
 
     implemented_properties = ("energy", "forces", "stress", "magmoms")
 
     def __init__(
         self,
         model: CHGNet | None = None,
+        *,
         use_device: str | None = None,
+        check_cuda_mem: bool = True,
         stress_weight: float | None = 1 / 160.21766208,
         on_isolated_atoms: Literal["ignore", "warn", "error"] = "warn",
         **kwargs,
     ) -> None:
         """Provide a CHGNet instance to calculate various atomic properties using ASE.
 
         Args:
             model (CHGNet): instance of a chgnet model. If set to None,
                 the pretrained CHGNet is loaded.
                 Default = None
             use_device (str, optional): The device to be used for predictions,
                 either "cpu", "cuda", or "mps". If not specified, the default device is
                 automatically selected based on the available options.
                 Default = None
+            check_cuda_mem (bool): Whether to use cuda with most available memory
+                Default = True
             stress_weight (float): the conversion factor to convert GPa to eV/A^3.
                 Default = 1/160.21
             on_isolated_atoms ('ignore' | 'warn' | 'error'): how to handle Structures
                 with isolated atoms.
                 Default = 'warn'
             **kwargs: Passed to the Calculator parent class.
         """
         super().__init__(**kwargs)
 
         # Determine the device to use
-        use_device = use_device or os.getenv("CHGNET_DEVICE")
-        if use_device in ("mps", None) and torch.backends.mps.is_available():
-            self.device = "mps"
-        else:
-            self.device = use_device or ("cuda" if torch.cuda.is_available() else "cpu")
-            if self.device == "cuda":
-                self.device = f"cuda:{cuda_devices_sorted_by_free_mem()[-1]}"
+        device = determine_device(use_device=use_device, check_cuda_mem=check_cuda_mem)
+        self.device = device
 
         # Move the model to the specified device
         self.model = (model or CHGNet.load(verbose=False)).to(self.device)
         self.model.graph_converter.set_isolated_atom_response(on_isolated_atoms)
         self.stress_weight = stress_weight
         print(f"CHGNet will run on {self.device}")
 
+    @classmethod
+    def from_file(
+        cls, path: str, use_device: str | None = None, **kwargs
+    ) -> CHGNetCalculator:
+        """Load a user's CHGNet model and initialize the Calculator."""
+        return CHGNetCalculator(
+            model=CHGNet.from_file(path),
+            use_device=use_device,
+            **kwargs,
+        )
+
     @property
     def version(self) -> str | None:
         """The version of CHGNet."""
         return self.model.version
 
     @property
     def n_params(self) -> int:
@@ -206,14 +214,15 @@
     def n_params(self) -> int:
         """The number of parameters in CHGNet."""
         return self.calculator.model.n_params
 
     def relax(
         self,
         atoms: Structure | Atoms,
+        *,
         fmax: float | None = 0.1,
         steps: int | None = 500,
         relax_cell: bool | None = True,
         ase_filter: str | None = "FrechetCellFilter",
         save_path: str | None = None,
         loginterval: int | None = 1,
         crystal_feas_save_path: str | None = None,
@@ -229,58 +238,46 @@
                 Default = 0.1
             steps (int | None): The maximum number of steps for relaxation.
                 Default = 500
             relax_cell (bool | None): Whether to relax the cell as well.
                 Default = True
             ase_filter (str | ase.filters.Filter): The filter to apply to the atoms
                 object for relaxation. Default = FrechetCellFilter
-                Used to default to ExpCellFilter but was removed due to bug reported in
-                https://gitlab.com/ase/ase/-/issues/1321 and fixed in
+                Default used to be ExpCellFilter which was removed due to bug reported
+                in https://gitlab.com/ase/ase/-/issues/1321 and fixed in
                 https://gitlab.com/ase/ase/-/merge_requests/3024.
             save_path (str | None): The path to save the trajectory.
                 Default = None
-            loginterval (int | None): Interval for logging trajectory and crystal feas
-                Default = 1
+            loginterval (int | None): Interval for logging trajectory and crystal
+                features. Default = 1
             crystal_feas_save_path (str | None): Path to save crystal feature vectors
                 which are logged at a loginterval rage
                 Default = None
             verbose (bool): Whether to print the output of the ASE optimizer.
                 Default = True
             assign_magmoms (bool): Whether to assign magnetic moments to the final
                 structure. Default = True
             **kwargs: Additional parameters for the optimizer.
 
         Returns:
             dict[str, Structure | TrajectoryObserver]:
                 A dictionary with 'final_structure' and 'trajectory'.
         """
-        try:
-            import ase.filters as filter_classes
-            from ase.filters import Filter
-
-        except ImportWarning:
-            import ase.constraints as filter_classes
-            from ase.constraints import Filter
-
-            if ase_filter == "FrechetCellFilter":
-                ase_filter = "ExpCellFilter"
-            print(
-                "Failed to import ase.filters. Default filter to ExpCellFilter. "
-                "For better relaxation accuracy with the new FrechetCellFilter, "
-                "run pip install git+https://gitlab.com/ase/ase"
-            )
+        import ase.filters as filters
+        from ase.filters import Filter
+
         valid_filter_names = [
             name
-            for name, cls in inspect.getmembers(filter_classes, inspect.isclass)
+            for name, cls in inspect.getmembers(filters, inspect.isclass)
             if issubclass(cls, Filter)
         ]
 
         if isinstance(ase_filter, str):
             if ase_filter in valid_filter_names:
-                ase_filter = getattr(filter_classes, ase_filter)
+                ase_filter = getattr(filters, ase_filter)
             else:
                 raise ValueError(
                     f"Invalid {ase_filter=}, must be one of {valid_filter_names}. "
                 )
 
         if isinstance(atoms, Structure):
             atoms = AseAtomsAdaptor().get_atoms(atoms)
@@ -391,15 +388,15 @@
     def __init__(self, atoms: Atoms) -> None:
         """Create a CrystalFeasObserver from an Atoms object."""
         self.atoms = atoms
         self.crystal_feature_vectors: list[np.ndarray] = []
 
     def __call__(self) -> None:
         """Record Atoms crystal feature vectors after an MD/relaxation step."""
-        self.crystal_feature_vectors.append(self.atoms._calc.results["crystal_fea"])
+        self.crystal_feature_vectors.append(self.atoms._calc.results["crystal_fea"])  # noqa: SLF001
 
     def __len__(self) -> int:
         """Number of recorded steps."""
         return len(self.crystal_feature_vectors)
 
     def save(self, filename: str) -> None:
         """Save the crystal feature vectors to filename in pickle format."""
@@ -410,14 +407,15 @@
 
 class MolecularDynamics:
     """Molecular dynamics class."""
 
     def __init__(
         self,
         atoms: Atoms | Structure,
+        *,
         model: CHGNet | CHGNetCalculator | None = None,
         ensemble: str = "nvt",
         thermostat: str = "Berendsen_inhomogeneous",
         temperature: int = 300,
         starting_temperature: int | None = None,
         timestep: float = 2.0,
         pressure: float = 1.01325e-4,
@@ -720,24 +718,24 @@
             atoms (Atoms): new atoms for running MD
         """
         calculator = self.atoms.calc
         self.atoms = atoms
         self.dyn.atoms = atoms
         self.dyn.atoms.calc = calculator
 
-    def upper_triangular_cell(self, verbose: bool | None = False) -> None:
+    def upper_triangular_cell(self, *, verbose: bool | None = False) -> None:
         """Transform to upper-triangular cell.
         ASE Nose-Hoover implementation only supports upper-triangular cell
         while ASE's canonical description is lower-triangular cell.
 
         Args:
             verbose (bool): Whether to notify user about upper-triangular cell
                 transformation. Default = False
         """
-        if not NPT._isuppertriangular(self.atoms.get_cell()):
+        if not NPT._isuppertriangular(self.atoms.get_cell()):  # noqa: SLF001
             a, b, c, alpha, beta, gamma = self.atoms.cell.cellpar()
             angles = np.radians((alpha, beta, gamma))
             sin_a, sin_b, _sin_g = np.sin(angles)
             cos_a, cos_b, cos_g = np.cos(angles)
             cos_p = (cos_g - cos_a * cos_b) / (sin_a * sin_b)
             cos_p = np.clip(cos_p, -1, 1)
             sin_p = (1 - cos_p**2) ** 0.5
@@ -790,14 +788,15 @@
             on_isolated_atoms=on_isolated_atoms,
         )
         self.fitted = False
 
     def fit(
         self,
         atoms: Structure | Atoms,
+        *,
         n_points: int = 11,
         fmax: float | None = 0.1,
         steps: int | None = 500,
         verbose: bool | None = False,
         **kwargs,
     ) -> None:
         """Relax the Structure/Atoms and fit the Birch-Murnaghan equation of state.
@@ -881,10 +880,10 @@
             raise ValueError(
                 "Equation of state needs to be fitted first through self.fit()"
             )
         if unit == "A^3/eV":
             return 1 / self.bm.b0
         if unit == "GPa^-1":
             return 1 / self.bm.b0_GPa
-        if unit in ("Pa^-1", "m^2/N"):
+        if unit in {"Pa^-1", "m^2/N"}:
             return 1 / (self.bm.b0_GPa * 1e9)
         raise NotImplementedError("unit has to be one of A^3/eV, GPa^-1 Pa^-1 or m^2/N")
```

### Comparing `chgnet-0.3.5/chgnet/model/encoders.py` & `chgnet-0.3.7/chgnet/model/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 class BondEncoder(nn.Module):
     """Encode a chemical bond given the positions of two atoms using Gaussian
     distance.
     """
 
     def __init__(
         self,
+        *,
         atom_graph_cutoff: float = 5,
         bond_graph_cutoff: float = 3,
         num_radial: int = 9,
         cutoff_coeff: int = 5,
         learnable: bool = False,
     ) -> None:
         """Initialize the bond encoder.
@@ -109,15 +110,15 @@
         bond_basis_bg = self.rbf_expansion_bg(undirected_bond_lengths)
         return bond_basis_ag, bond_basis_bg, bond_vectors
 
 
 class AngleEncoder(nn.Module):
     """Encode an angle given the two bond vectors using Fourier Expansion."""
 
-    def __init__(self, num_angular: int = 9, learnable: bool = True) -> None:
+    def __init__(self, *, num_angular: int = 9, learnable: bool = True) -> None:
         """Initialize the angle encoder.
 
         Args:
             num_angular (int): number of angular basis to use. Must be an odd integer.
             learnable (bool): whether to set the frequencies of the Fourier expansion
                 as learnable parameters. Default = False
         """
```

### Comparing `chgnet-0.3.5/chgnet/model/functions.py` & `chgnet-0.3.7/chgnet/model/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import Sequence
 
 import torch
 from torch import Tensor, nn
 
 
-def aggregate(data: Tensor, owners: Tensor, average=True, num_owner=None) -> Tensor:
+def aggregate(data: Tensor, owners: Tensor, *, average=True, num_owner=None) -> Tensor:
     """Aggregate rows in data by specifying the owners.
 
     Args:
         data (Tensor): data tensor to aggregate [n_row, feature_dim]
         owners (Tensor): specify the owner of each row [n_row, 1]
         average (bool): if True, average the rows, if False, sum the rows.
             Default = True
@@ -41,14 +41,15 @@
 
 class MLP(nn.Module):
     """Multi-Layer Perceptron used for non-linear regression."""
 
     def __init__(
         self,
         input_dim: int,
+        *,
         output_dim: int = 1,
         hidden_dim: int | Sequence[int] | None = (64, 64),
         dropout: float = 0,
         activation: str = "silu",
         bias: bool = True,
     ) -> None:
         """Initialize the MLP.
@@ -63,15 +64,15 @@
             activation (str, optional): The name of the activation function to use
                 in the gated MLP. Must be one of "relu", "silu", "tanh", or "gelu".
                 Default = "silu"
             bias (bool): whether to use bias in each Linear layers.
                 Default = True
         """
         super().__init__()
-        if hidden_dim in (None, 0):
+        if hidden_dim is None or hidden_dim == 0:
             layers = [nn.Dropout(dropout), nn.Linear(input_dim, output_dim, bias=bias)]
         elif isinstance(hidden_dim, int):
             layers = [
                 nn.Linear(input_dim, hidden_dim, bias=bias),
                 find_activation(activation),
                 nn.Dropout(dropout),
                 nn.Linear(hidden_dim, output_dim, bias=bias),
@@ -89,35 +90,36 @@
             layers.append(nn.Linear(hidden_dim[-1], output_dim, bias=bias))
         else:
             raise TypeError(
                 f"{hidden_dim=} must be an integer, a list of integers, or None."
             )
         self.layers = nn.Sequential(*layers)
 
-    def forward(self, X: Tensor) -> Tensor:
+    def forward(self, x: Tensor) -> Tensor:
         """Performs a forward pass through the MLP.
 
         Args:
-            X (Tensor): a tensor of shape (batch_size, input_dim)
+            x (Tensor): a tensor of shape (batch_size, input_dim)
 
         Returns:
             Tensor: a tensor of shape (batch_size, output_dim)
         """
-        return self.layers(X)
+        return self.layers(x)
 
 
 class GatedMLP(nn.Module):
     """Gated MLP
     similar model structure is used in CGCNN and M3GNet.
     """
 
     def __init__(
         self,
         input_dim: int,
         output_dim: int,
+        *,
         hidden_dim: int | list[int] | None = None,
         dropout: float = 0,
         activation: str = "silu",
         norm: str = "batch",
         bias: bool = True,
     ) -> None:
         """Initialize a gated MLP.
@@ -158,29 +160,29 @@
         )
         self.activation = find_activation(activation)
         self.sigmoid = nn.Sigmoid()
         self.norm = norm
         self.bn1 = find_normalization(name=norm, dim=output_dim)
         self.bn2 = find_normalization(name=norm, dim=output_dim)
 
-    def forward(self, X: Tensor) -> Tensor:
+    def forward(self, x: Tensor) -> Tensor:
         """Performs a forward pass through the MLP.
 
         Args:
-            X (Tensor): a tensor of shape (batch_size, input_dim)
+            x (Tensor): a tensor of shape (batch_size, input_dim)
 
         Returns:
             Tensor: a tensor of shape (batch_size, output_dim)
         """
         if self.norm is None:
-            core = self.activation(self.mlp_core(X))
-            gate = self.sigmoid(self.mlp_gate(X))
+            core = self.activation(self.mlp_core(x))
+            gate = self.sigmoid(self.mlp_gate(x))
         else:
-            core = self.activation(self.bn1(self.mlp_core(X)))
-            gate = self.sigmoid(self.bn2(self.mlp_gate(X)))
+            core = self.activation(self.bn1(self.mlp_core(x)))
+            gate = self.sigmoid(self.bn2(self.mlp_gate(x)))
         return core * gate
 
 
 class ScaledSiLU(torch.nn.Module):
     """Scaled Sigmoid Linear Unit."""
 
     def __init__(self) -> None:
```

### Comparing `chgnet-0.3.5/chgnet/model/layers.py` & `chgnet-0.3.7/chgnet/model/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 
 
 class AtomConv(nn.Module):
     """A convolution Layer to update atom features."""
 
     def __init__(
         self,
+        *,
         atom_fea_dim: int,
         bond_fea_dim: int,
         hidden_dim: int = 64,
         dropout: float = 0,
         activation: str = "silu",
         norm: str | None = None,
         use_mlp_out: bool = True,
         mlp_out_bias: bool = False,
         resnet: bool = True,
-        gMLP_norm: str | None = None,
+        gMLP_norm: str | None = None,  # noqa: N803
     ) -> None:
         """Initialize the AtomConv layer.
 
         Args:
             atom_fea_dim (int): The dimensionality of the input atom features.
             bond_fea_dim (int): The dimensionality of the input bond features.
             hidden_dim (int, optional): The dimensionality of the hidden layers in the
@@ -140,22 +141,23 @@
     """A convolution Layer to update bond features."""
 
     def __init__(
         self,
         atom_fea_dim: int,
         bond_fea_dim: int,
         angle_fea_dim: int,
+        *,
         hidden_dim: int = 64,
         dropout: float = 0,
         activation: str = "silu",
         norm: str | None = None,
         use_mlp_out: bool = True,
         mlp_out_bias: bool = False,
         resnet=True,
-        gMLP_norm: str | None = None,
+        gMLP_norm: str | None = None,  # noqa: N803
     ) -> None:
         """Initialize the BondConv layer.
 
         Args:
             atom_fea_dim (int): The dimensionality of the input atom features.
             bond_fea_dim (int): The dimensionality of the input bond features.
             angle_fea_dim (int): The dimensionality of the input angle features.
@@ -267,20 +269,21 @@
     """Update angle features."""
 
     def __init__(
         self,
         atom_fea_dim: int,
         bond_fea_dim: int,
         angle_fea_dim: int,
+        *,
         hidden_dim: int = 0,
         dropout: float = 0,
         activation: str = "silu",
         norm: str | None = None,
         resnet: bool = True,
-        gMLP_norm: str | None = None,
+        gMLP_norm: str | None = None,  # noqa: N803
     ) -> None:
         """Initialize the AngleUpdate layer.
 
         Args:
             atom_fea_dim (int): The dimensionality of the input atom features.
             bond_fea_dim (int): The dimensionality of the input bond features.
             angle_fea_dim (int): The dimensionality of the input angle features.
@@ -359,15 +362,15 @@
             new_angle_feas = self.angle_norm(new_angle_feas)
         return new_angle_feas
 
 
 class GraphPooling(nn.Module):
     """Pooling the sub-graphs in the batched graph."""
 
-    def __init__(self, average: bool = False) -> None:
+    def __init__(self, *, average: bool = False) -> None:
         """Args:
         average (bool): whether to average the features.
         """
         super().__init__()
         self.average = average
 
     def forward(self, atom_feas: Tensor, atom_owner: Tensor) -> Tensor:
@@ -388,15 +391,20 @@
 
 class GraphAttentionReadOut(nn.Module):
     """Multi Head Attention Read Out Layer
     merge the information from atom_feas to crystal_fea.
     """
 
     def __init__(
-        self, atom_fea_dim: int, num_head: int = 3, hidden_dim: int = 32, average=False
+        self,
+        atom_fea_dim: int,
+        num_head: int = 3,
+        hidden_dim: int = 32,
+        *,
+        average=False,
     ) -> None:
         """Initialize the layer.
 
         Args:
             atom_fea_dim (int): atom feature dimension
             num_head (int): number of attention heads used
             hidden_dim (int): dimension of hidden layer
```

### Comparing `chgnet-0.3.5/chgnet/model/model.py` & `chgnet-0.3.7/chgnet/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,30 @@
 from chgnet.model.layers import (
     AngleUpdate,
     AtomConv,
     BondConv,
     GraphAttentionReadOut,
     GraphPooling,
 )
-from chgnet.utils import cuda_devices_sorted_by_free_mem
+from chgnet.utils import determine_device
 
 if TYPE_CHECKING:
     from chgnet import PredTask
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 
 
 class CHGNet(nn.Module):
     """Crystal Hamiltonian Graph neural Network
     A model that takes in a crystal graph and output energy, force, magmom, stress.
     """
 
     def __init__(
         self,
+        *,
         atom_fea_dim: int = 64,
         bond_fea_dim: int = 64,
         angle_fea_dim: int = 64,
         composition_model: str | nn.Module = "MPtrj",
         num_radial: int = 31,
         num_angular: int = 31,
         n_conv: int = 4,
@@ -57,15 +58,15 @@
         is_intensive: bool = True,
         non_linearity: Literal["silu", "relu", "tanh", "gelu"] = "silu",
         atom_graph_cutoff: float = 6,
         bond_graph_cutoff: float = 3,
         graph_converter_algorithm: Literal["legacy", "fast"] = "fast",
         cutoff_coeff: int = 8,
         learnable_rbf: bool = True,
-        gMLP_norm: str | None = "layer",
+        gMLP_norm: str | None = "layer",  # noqa: N803
         readout_norm: str | None = "layer",
         version: str | None = None,
         **kwargs,
     ) -> None:
         """Initialize CHGNet.
 
         Args:
@@ -146,17 +147,17 @@
             readout_norm (str): normalization layer to use before readout layer
                 Default = 'layer'
             version (str): Pretrained checkpoint version.
             **kwargs: Additional keyword arguments
         """
         # Store model args for reconstruction
         self.model_args = {
-            k: v
-            for k, v in locals().items()
-            if k not in ["self", "__class__", "kwargs"]
+            key: val
+            for key, val in locals().items()
+            if key not in {"self", "__class__", "kwargs"}
         }
         self.model_args.update(kwargs)
         if version:
             self.model_args["version"] = version
 
         super().__init__()
         self.atom_fea_dim = atom_fea_dim
@@ -275,26 +276,26 @@
         self.site_wise = nn.Linear(atom_fea_dim, 1)
         self.readout_norm = find_normalization(readout_norm, dim=atom_fea_dim)
         self.mlp_first = mlp_first
         if mlp_first:
             self.read_out_type = "sum"
             input_dim = atom_fea_dim
             self.pooling = GraphPooling(average=False)
-        elif read_out in ["attn", "weighted"]:
+        elif read_out in {"attn", "weighted"}:
             self.read_out_type = "attn"
             num_heads = kwargs.pop("num_heads", 3)
             self.pooling = GraphAttentionReadOut(
                 atom_fea_dim, num_head=num_heads, average=True
             )
             input_dim = atom_fea_dim * num_heads
         else:
             self.read_out_type = "ave"
             input_dim = atom_fea_dim
             self.pooling = GraphPooling(average=True)
-        if kwargs.pop("final_mlp", "MLP") in ["normal", "MLP"]:
+        if kwargs.pop("final_mlp", "MLP") in {"normal", "MLP"}:
             self.mlp = MLP(
                 input_dim=input_dim,
                 hidden_dim=mlp_hidden_dims,
                 output_dim=1,
                 dropout=mlp_dropout,
                 activation=non_linearity,
             )
@@ -323,14 +324,15 @@
     def n_params(self) -> int:
         """Return the number of parameters in the model."""
         return sum(p.numel() for p in self.parameters())
 
     def forward(
         self,
         graphs: Sequence[CrystalGraph],
+        *,
         task: PredTask = "e",
         return_site_energies: bool = False,
         return_atom_feas: bool = False,
         return_crystal_feas: bool = False,
     ) -> dict[str, Tensor]:
         """Get prediction associated with input graphs
         Args:
@@ -377,15 +379,16 @@
             prediction["site_energies"] = [
                 i + j for i, j in zip(prediction["site_energies"], site_energy_shifts)
             ]
         return prediction
 
     def _compute(
         self,
-        g,
+        g: BatchedGraph,
+        *,
         compute_force: bool = False,
         compute_stress: bool = False,
         compute_magmom: bool = False,
         return_site_energies: bool = False,
         return_atom_feas: bool = False,
         return_crystal_feas: bool = False,
     ) -> dict:
@@ -526,14 +529,15 @@
         prediction["e"] = energy
 
         return prediction
 
     def predict_structure(
         self,
         structure: Structure | Sequence[Structure],
+        *,
         task: PredTask = "efsm",
         return_site_energies: bool = False,
         return_atom_feas: bool = False,
         return_crystal_feas: bool = False,
         batch_size: int = 16,
     ) -> dict[str, Tensor] | list[dict[str, Tensor]]:
         """Predict from pymatgen.core.Structure.
@@ -574,14 +578,15 @@
             return_crystal_feas=return_crystal_feas,
             batch_size=batch_size,
         )
 
     def predict_graph(
         self,
         graph: CrystalGraph | Sequence[CrystalGraph],
+        *,
         task: PredTask = "efsm",
         return_site_energies: bool = False,
         return_atom_feas: bool = False,
         return_crystal_feas: bool = False,
         batch_size: int = 16,
     ) -> dict[str, Tensor] | list[dict[str, Tensor]]:
         """Predict from CrustalGraph.
@@ -604,15 +609,15 @@
                 e (Tensor) : energy of structures float in eV/atom
                 f (Tensor) : force on atoms [num_atoms, 3] in eV/A
                 s (Tensor) : stress of structure [3, 3] in GPa
                 m (Tensor) : magnetic moments of sites [num_atoms, 3] in Bohr
                     magneton mu_B
         """
         if not isinstance(graph, (CrystalGraph, Sequence)):
-            raise ValueError(
+            raise TypeError(
                 f"{type(graph)=} must be CrystalGraph or list of CrystalGraphs"
             )
 
         model_device = next(self.parameters()).device
 
         graphs = [graph] if isinstance(graph, CrystalGraph) else graph
         self.eval()
@@ -659,35 +664,39 @@
     def from_dict(cls, dct: dict, **kwargs) -> CHGNet:
         """Build a CHGNet from a saved dictionary."""
         chgnet = CHGNet(**dct["model_args"], **kwargs)
         chgnet.load_state_dict(dct["state_dict"])
         return chgnet
 
     @classmethod
-    def from_file(cls, path, **kwargs) -> CHGNet:
+    def from_file(cls, path: str, **kwargs) -> CHGNet:
         """Build a CHGNet from a saved file."""
         state = torch.load(path, map_location=torch.device("cpu"))
         return CHGNet.from_dict(state["model"], **kwargs)
 
     @classmethod
     def load(
         cls,
-        model_name="0.3.0",
+        *,
+        model_name: str = "0.3.0",
         use_device: str | None = None,
+        check_cuda_mem: bool = True,
         verbose: bool = True,
     ) -> CHGNet:
         """Load pretrained CHGNet model.
 
         Args:
             model_name (str, optional):
                 Default = "0.3.0".
             use_device (str, optional): The device to be used for predictions,
                 either "cpu", "cuda", or "mps". If not specified, the default device is
                 automatically selected based on the available options.
                 Default = None
+            check_cuda_mem (bool): Whether to use cuda with most available memory
+                Default = True
             verbose (bool): whether to print model device information
                 Default = True
         Raises:
             ValueError: On unknown model_name.
         """
         checkpoint_path = {
             "0.3.0": "../pretrained/0.3.0/chgnet_0.3.0_e29f68s314m37.pth.tar",
@@ -703,21 +712,15 @@
             # cases causes unphysical jumps in bonding energy. see
             # https://github.com/CederGroupHub/chgnet/issues/79
             mlp_out_bias=model_name == "0.2.0",
             version=model_name,
         )
 
         # Determine the device to use
-        use_device = use_device or os.getenv("CHGNET_DEVICE")
-        if use_device in ("mps", None) and torch.backends.mps.is_available():
-            device = "mps"
-        else:
-            device = use_device or ("cuda" if torch.cuda.is_available() else "cpu")
-            if device == "cuda":
-                device = f"cuda:{cuda_devices_sorted_by_free_mem()[-1]}"
+        device = determine_device(use_device=use_device, check_cuda_mem=check_cuda_mem)
 
         # Move the model to the specified device
         model = model.to(device)
         if verbose:
             print(f"CHGNet will run on {device}")
         return model
 
@@ -768,14 +771,15 @@
 
     @classmethod
     def from_graphs(
         cls,
         graphs: Sequence[CrystalGraph],
         bond_basis_expansion: nn.Module,
         angle_basis_expansion: nn.Module,
+        *,
         compute_stress: bool = False,
     ) -> BatchedGraph:
         """Featurize and assemble a list of graphs.
 
         Args:
             graphs (list[Tensor]): a list of CrystalGraphs
             bond_basis_expansion (nn.Module): bond basis expansion layer in CHGNet
```

### Comparing `chgnet-0.3.5/chgnet/pretrained/0.2.0/README.md` & `chgnet-0.3.7/chgnet/pretrained/0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/chgnet/pretrained/0.2.0/chgnet_0.2.0_e30f77s348m32.pth.tar` & `chgnet-0.3.7/chgnet/pretrained/0.2.0/chgnet_0.2.0_e30f77s348m32.pth.tar`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/chgnet/pretrained/0.3.0/README.md` & `chgnet-0.3.7/chgnet/pretrained/0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/chgnet/pretrained/0.3.0/chgnet_0.3.0_e29f68s314m37.pth.tar` & `chgnet-0.3.7/chgnet/pretrained/0.3.0/chgnet_0.3.0_e29f68s314m37.pth.tar`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/chgnet/trainer/trainer.py` & `chgnet-0.3.7/chgnet/trainer/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,29 @@
     CosineAnnealingLR,
     CosineAnnealingWarmRestarts,
     ExponentialLR,
     MultiStepLR,
 )
 
 from chgnet.model.model import CHGNet
-from chgnet.utils import AverageMeter, cuda_devices_sorted_by_free_mem, mae, write_json
+from chgnet.utils import AverageMeter, determine_device, mae, write_json
 
 if TYPE_CHECKING:
     from torch.utils.data import DataLoader
 
     from chgnet import TrainTask
 
 
 class Trainer:
     """A trainer to train CHGNet using energy, force, stress and magmom."""
 
     def __init__(
         self,
         model: CHGNet | None = None,
+        *,
         targets: TrainTask = "ef",
         energy_loss_ratio: float = 1,
         force_loss_ratio: float = 1,
         stress_loss_ratio: float = 0.1,
         mag_loss_ratio: float = 0.1,
         optimizer: str = "Adam",
         scheduler: str = "CosLR",
@@ -44,14 +45,15 @@
         epochs: int = 50,
         starting_epoch: int = 0,
         learning_rate: float = 1e-3,
         print_freq: int = 100,
         torch_seed: int | None = None,
         data_seed: int | None = None,
         use_device: str | None = None,
+        check_cuda_mem: bool = True,
         **kwargs,
     ) -> None:
         """Initialize all hyper-parameters for trainer.
 
         Args:
             model (nn.Module): a CHGNet model
             targets ("ef" | "efs" | "efsm"): The training targets. Default = "ef"
@@ -76,24 +78,27 @@
                 Default = 1e-3
             print_freq (int): frequency to print training output
                 Default = 100
             torch_seed (int): random seed for torch
                 Default = None
             data_seed (int): random seed for random
                 Default = None
-            use_device (str, optional): device name to train the CHGNet.
-                Can be "cuda", "cpu"
+            use_device (str, optional): The device to be used for predictions,
+                either "cpu", "cuda", or "mps". If not specified, the default device is
+                automatically selected based on the available options.
                 Default = None
+            check_cuda_mem (bool): Whether to use cuda with most available memory
+                Default = True
             **kwargs (dict): additional hyper-params for optimizer, scheduler, etc.
         """
         # Store trainer args for reproducibility
         self.trainer_args = {
             k: v
             for k, v in locals().items()
-            if k not in ["self", "__class__", "model", "kwargs"]
+            if k not in {"self", "__class__", "model", "kwargs"}
         }
         self.trainer_args.update(kwargs)
 
         self.model = model
         self.targets = targets
 
         if torch_seed is not None:
@@ -124,29 +129,29 @@
         elif optimizer == "RAdam":
             weight_decay = kwargs.pop("weight_decay", 0)
             self.optimizer = torch.optim.RAdam(
                 model.parameters(), learning_rate, weight_decay=weight_decay
             )
 
         # Define learning rate scheduler
-        if scheduler in ["MultiStepLR", "multistep"]:
+        if scheduler in {"MultiStepLR", "multistep"}:
             scheduler_params = kwargs.pop(
                 "scheduler_params",
                 {
                     "milestones": [4 * epochs, 6 * epochs, 8 * epochs, 9 * epochs],
                     "gamma": 0.3,
                 },
             )
             self.scheduler = MultiStepLR(self.optimizer, **scheduler_params)
             self.scheduler_type = "multistep"
-        elif scheduler in ["ExponentialLR", "Exp", "Exponential"]:
+        elif scheduler in {"ExponentialLR", "Exp", "Exponential"}:
             scheduler_params = kwargs.pop("scheduler_params", {"gamma": 0.98})
             self.scheduler = ExponentialLR(self.optimizer, **scheduler_params)
             self.scheduler_type = "exp"
-        elif scheduler in ["CosineAnnealingLR", "CosLR", "Cos", "cos"]:
+        elif scheduler in {"CosineAnnealingLR", "CosLR", "Cos", "cos"}:
             scheduler_params = kwargs.pop("scheduler_params", {"decay_fraction": 1e-2})
             decay_fraction = scheduler_params.pop("decay_fraction")
             self.scheduler = CosineAnnealingLR(
                 self.optimizer,
                 T_max=10 * epochs,  # Maximum number of iterations.
                 eta_min=decay_fraction * learning_rate,
             )
@@ -176,36 +181,30 @@
             mag_loss_ratio=mag_loss_ratio,
             **kwargs,
         )
         self.epochs = epochs
         self.starting_epoch = starting_epoch
 
         # Determine the device to use
-        if use_device is not None:
-            self.device = use_device
-        elif torch.cuda.is_available():
-            self.device = "cuda"
-        else:
-            self.device = "cpu"
-        if self.device == "cuda":
-            # Determine cuda device with most available memory
-            device_with_most_available_memory = cuda_devices_sorted_by_free_mem()[-1]
-            self.device = f"cuda:{device_with_most_available_memory}"
+        self.device = determine_device(
+            use_device=use_device, check_cuda_mem=check_cuda_mem
+        )
 
         self.print_freq = print_freq
         self.training_history: dict[
             str, dict[Literal["train", "val", "test"], list[float]]
         ] = {key: {"train": [], "val": [], "test": []} for key in self.targets}
         self.best_model = None
 
     def train(
         self,
         train_loader: DataLoader,
         val_loader: DataLoader,
         test_loader: DataLoader | None = None,
+        *,
         save_dir: str | None = None,
         save_test_result: bool = False,
         train_composition_model: bool = False,
     ) -> None:
         """Train the model using torch data_loaders.
 
         Args:
@@ -352,14 +351,15 @@
                     )
                 print(message)
         return {key: round(err.avg, 6) for key, err in mae_errors.items()}
 
     def _validate(
         self,
         val_loader: DataLoader,
+        *,
         is_test: bool = False,
         test_result_save_path: str | None = None,
     ) -> dict:
         """Validation or test step.
 
         Args:
             val_loader (DataLoader): val loader to test accuracy after each epoch
@@ -471,24 +471,24 @@
         print(message)
         return {k: round(mae_error.avg, 6) for k, mae_error in mae_errors.items()}
 
     def get_best_model(self) -> CHGNet:
         """Get best model recorded in the trainer."""
         if self.best_model is None:
             raise RuntimeError("the model needs to be trained first")
-        MAE = min(self.training_history["e"]["val"])
+        MAE = min(self.training_history["e"]["val"])  # noqa: N806
         print(f"Best model has val {MAE =:.4}")
         return self.best_model
 
     @property
     def _init_keys(self) -> list[str]:
         return [
             key
             for key in list(inspect.signature(Trainer.__init__).parameters)
-            if key not in (["self", "model", "kwargs"])
+            if key not in {"self", "model", "kwargs"}
         ]
 
     def save(self, filename: str = "training_result.pth.tar") -> None:
         """Save the model, graph_converter, etc."""
         state = {
             "model": self.model.as_dict(),
             "optimizer": self.optimizer.state_dict(),
@@ -571,14 +571,15 @@
 
 
 class CombinedLoss(nn.Module):
     """A combined loss function of energy, force, stress and magmom."""
 
     def __init__(
         self,
+        *,
         target_str: str = "ef",
         criterion: str = "MSE",
         is_intensive: bool = True,
         energy_loss_ratio: float = 1,
         force_loss_ratio: float = 1,
         stress_loss_ratio: float = 0.1,
         mag_loss_ratio: float = 0.1,
@@ -601,17 +602,17 @@
                 Default = 0.1
             mag_loss_ratio (float): magmom loss ratio in loss function
                 Default = 0.1
             delta (float): delta for torch.nn.HuberLoss. Default = 0.1
         """
         super().__init__()
         # Define loss criterion
-        if criterion in ["MSE", "mse"]:
+        if criterion in {"MSE", "mse"}:
             self.criterion = nn.MSELoss()
-        elif criterion in ["MAE", "mae", "l1"]:
+        elif criterion in {"MAE", "mae", "l1"}:
             self.criterion = nn.L1Loss()
         elif criterion == "Huber":
             self.criterion = nn.HuberLoss(delta=delta)
         else:
             raise NotImplementedError
         self.target_str = target_str
         self.is_intensive = is_intensive
```

### Comparing `chgnet-0.3.5/chgnet/utils/common_utils.py` & `chgnet-0.3.7/chgnet/utils/common_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,39 @@
 import os
 
 import nvidia_smi
 import torch
 from torch import Tensor
 
 
+def determine_device(
+    use_device: str | None = None,
+    *,
+    check_cuda_mem: bool = True,
+) -> str:
+    """Determine the device to use for torch model.
+
+    Args:
+        use_device (str): User specify device name
+        check_cuda_mem (bool): Whether to return cuda with most available memory
+
+    Returns:
+        device (str): device name to be passed to model.to(device)
+    """
+    use_device = use_device or os.getenv("CHGNET_DEVICE")
+    if use_device in {"mps", None} and torch.backends.mps.is_available():
+        device = "mps"
+    else:
+        device = use_device or ("cuda" if torch.cuda.is_available() else "cpu")
+        if device == "cuda" and check_cuda_mem:
+            device = f"cuda:{cuda_devices_sorted_by_free_mem()[-1]}"
+
+    return device
+
+
 def cuda_devices_sorted_by_free_mem() -> list[int]:
     """List available CUDA devices sorted by increasing available memory.
 
     To get the device with the most free memory, use the last list item.
     """
     if not torch.cuda.is_available():
         return []
```

### Comparing `chgnet-0.3.5/chgnet/utils/vasp_utils.py` & `chgnet-0.3.7/chgnet/utils/vasp_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 from __future__ import annotations
 
+import os.path
 import re
 from typing import TYPE_CHECKING
 
 from monty.io import reverse_readfile
+from monty.os.path import zpath
 from pymatgen.io.vasp.outputs import Oszicar, Vasprun
 
+from chgnet.utils import write_json
+
 if TYPE_CHECKING:
     from pymatgen.core import Structure
 
 
 def parse_vasp_dir(
-    file_root: str, check_electronic_convergence: bool = True
+    base_dir: str,
+    *,
+    check_electronic_convergence: bool = True,
+    save_path: str | None = None,
 ) -> dict[str, list]:
     """Parse VASP output files into structures and labels
     By default, the magnetization is read from mag_x from VASP,
     plz modify the code if magnetization is for (y) and (z).
 
     Args:
-        file_root (str): the directory of the VASP calculation outputs
+        base_dir (str): the directory of the VASP calculation outputs
         check_electronic_convergence (bool): if set to True, this function will raise
             Exception to VASP calculation that did not achieve electronic convergence.
+            Default = True
+        save_path (str): path to save the parsed VASP labels
     """
-    try:
-        oszicar = Oszicar(f"{file_root}/OSZICAR")
-        vasprun_orig = Vasprun(
-            f"{file_root}/vasprun.xml",
-            parse_dos=False,
-            parse_eigen=False,
-            parse_projected_eigen=False,
-            parse_potcar_file=False,
-            exception_on_bad_xml=False,
-        )
-        outcar_filename = f"{file_root}/OUTCAR"
-    except Exception:
-        oszicar = Oszicar(f"{file_root}/OSZICAR.gz")
-        vasprun_orig = Vasprun(
-            f"{file_root}/vasprun.xml.gz",
-            parse_dos=False,
-            parse_eigen=False,
-            parse_projected_eigen=False,
-            parse_potcar_file=False,
-            exception_on_bad_xml=False,
-        )
-        outcar_filename = f"{file_root}/OUTCAR.gz"
-
-    charge = []
-    mag_x = []
-    mag_y = []
-    mag_z = []
-    header = []
-    all_lines = []
+    if os.path.isdir(base_dir) is False:
+        raise FileNotFoundError(f"{base_dir=} is not a directory")
+
+    oszicar_path = zpath(f"{base_dir}/OSZICAR")
+    vasprun_path = zpath(f"{base_dir}/vasprun.xml")
+    outcar_path = zpath(f"{base_dir}/OUTCAR")
+    if not os.path.exists(oszicar_path) or not os.path.exists(vasprun_path):
+        raise RuntimeError(f"No data parsed from {base_dir}!")
+
+    oszicar = Oszicar(oszicar_path)
+    vasprun_orig = Vasprun(
+        vasprun_path,
+        parse_dos=False,
+        parse_eigen=False,
+        parse_projected_eigen=False,
+        parse_potcar_file=False,
+        exception_on_bad_xml=False,
+    )
+
+    charge, mag_x, mag_y, mag_z, header, all_lines = [], [], [], [], [], []
 
-    for line in reverse_readfile(outcar_filename):
+    for line in reverse_readfile(outcar_path):
         clean = line.strip()
         all_lines.append(clean)
 
     all_lines.reverse()
     # For single atom systems, VASP doesn't print a total line, so
     # reverse parsing is very difficult
-    read_charge = False
-    read_mag_x = False
-    read_mag_y = False  # for SOC calculations only
-    read_mag_z = False
+    # for SOC calculations only
+    read_charge = read_mag_x = read_mag_y = read_mag_z = False
     mag_x_all = []
     ion_step_count = 0
 
     for clean in all_lines:
         if "magnetization (x)" in clean:
             ion_step_count += 1
         if read_charge or read_mag_x or read_mag_y or read_mag_z:
@@ -85,40 +83,32 @@
                     elif read_mag_y:
                         mag_y.append(dict(zip(header, tokens)))
                     elif read_mag_z:
                         mag_z.append(dict(zip(header, tokens)))
                 elif clean.startswith("tot"):
                     if ion_step_count == (len(mag_x_all) + 1):
                         mag_x_all.append(mag_x)
-                    read_charge = False
-                    read_mag_x = False
-                    read_mag_y = False
-                    read_mag_z = False
+                    read_charge = read_mag_x = read_mag_y = read_mag_z = False
         if clean == "total charge":
             read_charge = True
-            read_mag_x, read_mag_y, read_mag_z = False, False, False
+            read_mag_x = read_mag_y = read_mag_z = False
         elif clean == "magnetization (x)":
             mag_x = []
             read_mag_x = True
-            read_charge, read_mag_y, read_mag_z = False, False, False
+            read_charge = read_mag_y = read_mag_z = False
         elif clean == "magnetization (y)":
             mag_y = []
             read_mag_y = True
-            read_charge, read_mag_x, read_mag_z = False, False, False
+            read_charge = read_mag_x = read_mag_z = False
         elif clean == "magnetization (z)":
             mag_z = []
             read_mag_z = True
-            read_charge, read_mag_x, read_mag_y = False, False, False
+            read_charge = read_mag_x = read_mag_y = False
         elif re.search("electrostatic", clean):
-            read_charge, read_mag_x, read_mag_y, read_mag_z = (
-                False,
-                False,
-                False,
-                False,
-            )
+            read_charge = read_mag_x = read_mag_y = read_mag_z = False
 
     if len(oszicar.ionic_steps) == len(mag_x_all):  # unfinished VASP job
         print("Unfinished OUTCAR")
     elif len(oszicar.ionic_steps) == (len(mag_x_all) - 1):  # finished job
         mag_x_all.pop(-1)
 
     n_atoms = len(vasprun_orig.ionic_steps[0]["structure"])
@@ -128,32 +118,37 @@
         "uncorrected_total_energy": [],
         "energy_per_atom": [],
         "force": [],
         "magmom": [],
         "stress": None if "stress" not in vasprun_orig.ionic_steps[0] else [],
     }
 
-    for ionic_step, mag_step in zip(vasprun_orig.ionic_steps, mag_x_all):
+    for index, ionic_step in enumerate(vasprun_orig.ionic_steps):
         if (
             check_electronic_convergence
             and len(ionic_step["electronic_steps"]) >= vasprun_orig.parameters["NELM"]
         ):
             continue
 
         dataset["structure"].append(ionic_step["structure"])
         dataset["uncorrected_total_energy"].append(ionic_step["e_0_energy"])
         dataset["energy_per_atom"].append(ionic_step["e_0_energy"] / n_atoms)
         dataset["force"].append(ionic_step["forces"])
-        dataset["magmom"].append([site["tot"] for site in mag_step])
+        if mag_x_all != []:
+            dataset["magmom"].append([site["tot"] for site in mag_x_all[index]])
         if "stress" in ionic_step:
             dataset["stress"].append(ionic_step["stress"])
 
     if dataset["uncorrected_total_energy"] == []:
-        raise RuntimeError(f"No data parsed from {file_root}!")
+        raise RuntimeError(f"No data parsed from {base_dir}!")
 
+    if save_path is not None:
+        save_dict = dataset.copy()
+        save_dict["structure"] = [struct.as_dict() for struct in dataset["structure"]]
+        write_json(save_dict, save_path)
     return dataset
 
 
 def solve_charge_by_mag(
     structure: Structure,
     default_ox: dict[str, float] | None = None,
     ox_ranges: dict[str, dict[tuple[float, float], int]] | None = None,
```

### Comparing `chgnet-0.3.5/chgnet.egg-info/PKG-INFO` & `chgnet-0.3.7/chgnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chgnet
-Version: 0.3.5
+Version: 0.3.7
 Summary: Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling
 Author-email: Bowen Deng <bowendeng@berkeley.edu>
 License: Modified BSD
 Project-URL: Source, https://github.com/CederGroupHub/chgnet
 Project-URL: Package, https://pypi.org/project/chgnet
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -15,28 +15,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ase
+Requires-Dist: ase>=3.23.0
 Requires-Dist: cython>=0.29.26
-Requires-Dist: numpy>=1.21.6
+Requires-Dist: numpy>=1.26
 Requires-Dist: nvidia-ml-py3>=7.352.0
 Requires-Dist: pymatgen>=2023.10.11
 Requires-Dist: torch>=1.11.0
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-cov>=4; extra == "test"
+Requires-Dist: pytest>=8; extra == "test"
 Provides-Extra: examples
-Requires-Dist: crystal-toolkit; extra == "examples"
-Requires-Dist: pandas; extra == "examples"
+Requires-Dist: crystal-toolkit>=2023.11.3; extra == "examples"
+Requires-Dist: pandas>=2.2; extra == "examples"
 Provides-Extra: docs
-Requires-Dist: lazydocs; extra == "docs"
+Requires-Dist: lazydocs>=0.4; extra == "docs"
 
 <h1 align="center">CHGNet</h1>
 
 <h4 align="center">
 
 [![Tests](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml/badge.svg)](https://github.com/CederGroupHub/chgnet/actions/workflows/test.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/e3bdcea0382a495d96408e4f84408e85)](https://app.codacy.com/gh/CederGroupHub/chgnet/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
```

### Comparing `chgnet-0.3.5/chgnet.egg-info/SOURCES.txt` & `chgnet-0.3.7/chgnet.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 tests/test_dataset.py
 tests/test_encoders.py
 tests/test_graph.py
 tests/test_md.py
 tests/test_model.py
 tests/test_relaxation.py
 tests/test_trainer.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_vasp_utils.py
```

### Comparing `chgnet-0.3.5/pyproject.toml` & `chgnet-0.3.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-[build-system]
-requires = ["Cython", "setuptools>=65.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "chgnet"
-version = "0.3.5"
+version = "0.3.7"
 description = "Pretrained Universal Neural Network Potential for Charge-informed Atomistic Modeling"
 authors = [{ name = "Bowen Deng", email = "bowendeng@berkeley.edu" }]
 requires-python = ">=3.9"
 readme = "README.md"
 license = { text = "Modified BSD" }
 dependencies = [
-    "ase",
+    "ase>=3.23.0",
     "cython>=0.29.26",
-    "numpy>=1.21.6",
+    "numpy>=1.26",
     "nvidia-ml-py3>=7.352.0",
     "pymatgen>=2023.10.11",
     "torch>=1.11.0",
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
@@ -28,107 +24,86 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 [project.optional-dependencies]
-test = ["pytest", "pytest-cov"]
+test = ["pytest-cov>=4", "pytest>=8"]
 # needed to run interactive example notebooks
-examples = ["crystal-toolkit", "pandas"]
-docs = ["lazydocs"]
+examples = ["crystal-toolkit>=2023.11.3", "pandas>=2.2"]
+docs = ["lazydocs>=0.4"]
 
 [project.urls]
 Source = "https://github.com/CederGroupHub/chgnet"
 Package = "https://pypi.org/project/chgnet"
 
 [tool.setuptools.packages]
 find = { include = ["chgnet*"], exclude = ["tests", "tests*"] }
 
 [tool.setuptools.package-data]
 "chgnet" = ["*.json"]
 "chgnet.pretrained" = ["*", "**/*"]
 
+[build-system]
+requires = ["Cython", "setuptools>=65.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
 [tool.ruff]
 target-version = "py39"
-include = ["**/pyproject.toml", "*.ipynb", "*.py", "*.pyi"]
+extend-include = ["*.ipynb"]
+
 [tool.ruff.lint]
-select = [
-    "B",    # flake8-bugbear
-    "C4",   # flake8-comprehensions
-    "D",    # pydocstyle
-    "E",    # pycodestyle error
-    "EXE",  # flake8-executable
-    "F",    # pyflakes
-    "FA",   # flake8-future-annotations
-    "FLY",  # flynt
-    "I",    # isort
-    "ICN",  # flake8-import-conventions
-    "ISC",  # flake8-implicit-str-concat
-    "PD",   # pandas-vet
-    "PERF", # perflint
-    "PIE",  # flake8-pie
-    "PL",   # pylint
-    "PT",   # flake8-pytest-style
-    "PYI",  # flakes8-pyi
-    "Q",    # flake8-quotes
-    "RET",  # flake8-return
-    "RSE",  # flake8-raise
-    "RUF",  # Ruff-specific rules
-    "SIM",  # flake8-simplify
-    "SLOT", # flakes8-slot
-    "T201",
-    "TCH",  # flake8-type-checking
-    "TID",  # tidy imports
-    "TID",  # flake8-tidy-imports
-    "UP",   # pyupgrade
-    "W",    # pycodestyle warning
-    "YTT",  # flake8-2020
-]
+select = ["ALL"]
 ignore = [
     "ANN001",  # TODO add missing type annotations
     "ANN003",
+    "ANN101",
+    "ANN102",
     "B019",    # Use of functools.lru_cache on methods can lead to memory leaks
     "BLE001",
     "C408",    # unnecessary-collection-call
     "C901",    # function is too complex
     "COM812",  # trailing comma missing
     "D100",    # Missing docstring in public module
     "D104",    # Missing docstring in public package
     "D205",    # 1 blank line required between summary line and description
     "DTZ005",  # use of datetime.now() without timezone
     "E731",    # do not assign a lambda expression, use a def
     "EM",
     "ERA001",  # found commented out code
-    "FBT001",  # Boolean positional argument in function
-    "FBT002",  # Boolean keyword argument in function
     "ISC001",
     "NPY002",  # TODO replace legacy np.random.seed
     "PLR",     # pylint refactor
     "PLW2901", # Outer for loop variable overwritten by inner assignment target
     "PT006",   # pytest-parametrize-names-wrong-type
     "PT011",   # pytest-raises-too-broad
     "PT013",   # pytest-incorrect-pytest-import
     "PT019",   # pytest-fixture-param-without-value
     "PTH",     # prefer Path to os.path
+    "S108",
     "S301",    # pickle can be unsafe
     "S310",
+    "S311",
     "TRY003",
+    "TRY300",
 ]
 pydocstyle.convention = "google"
 isort.required-imports = ["from __future__ import annotations"]
 isort.split-on-trailing-comma = false
 
+[tool.ruff.format]
+docstring-code-format = true
+
 [tool.ruff.lint.per-file-ignores]
 "site/*" = ["INP001", "S602"]
-"tests/*" = ["ANN201", "D103", "INP001", "S101"]
+"tests/*" = ["ANN201", "D100", "D103", "FBT001", "FBT002", "INP001", "S101"]
 # E402 Module level import not at top of file
 "examples/*" = ["E402", "I002", "INP001", "N816", "S101", "T201"]
 "chgnet/**/*" = ["T201"]
 "__init__.py" = ["F401"]
 
-
 [tool.coverage.run]
 source = ["chgnet"]
 
 [tool.coverage.report]
 omit = ["tests/*"]
```

### Comparing `chgnet-0.3.5/tests/test_converter.py` & `chgnet-0.3.7/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/tests/test_crystal_graph.py` & `chgnet-0.3.7/tests/test_crystal_graph.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/tests/test_dataset.py` & `chgnet-0.3.7/tests/test_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import random
+
 import numpy as np
 import pytest
 import torch
 from pymatgen.core import Lattice, Structure
 
 from chgnet.data.dataset import StructureData, get_train_val_test_loader
 from chgnet.graph import CrystalGraph
@@ -13,45 +15,47 @@
 coords = [[0, 0, 0], [0.5, 0.5, 0.5]]
 NaCl = Structure(lattice, species, coords)
 
 
 @pytest.fixture()
 def structure_data() -> StructureData:
     """Create a graph with 3 nodes and 3 directed edges."""
+    random.seed(42)
     structures, energies, forces, stresses, magmoms, structure_ids = (
         [],
         [],
         [],
         [],
         [],
         [],
     )
-    for _ in range(100):
+    for index in range(100):
         struct = NaCl.copy()
         struct.perturb(0.1)
         structures.append(struct)
         energies.append(np.random.random(1))
         forces.append(np.random.random([2, 3]))
         stresses.append(np.random.random([3, 3]))
         magmoms.append(np.random.random([2, 1]))
-        structure_ids.append("tmp_id")
+        structure_ids.append(index)
     return StructureData(
         structures=structures,
         energies=energies,
         forces=forces,
         stresses=stresses,
         magmoms=magmoms,
         structure_ids=structure_ids,
     )
 
 
 def test_structure_data(structure_data: StructureData) -> None:
     get_one = structure_data[0]
     assert isinstance(get_one[0], CrystalGraph)
-    assert get_one[0].mp_id == "tmp_id"
+    assert isinstance(get_one[0].mp_id, int)
+    assert get_one[0].mp_id == 42
     assert isinstance(get_one[1], dict)
     assert isinstance(get_one[1]["e"], torch.Tensor)
     assert isinstance(get_one[1]["f"], torch.Tensor)
     assert isinstance(get_one[1]["s"], torch.Tensor)
     assert isinstance(get_one[1]["m"], torch.Tensor)
 
 
@@ -81,7 +85,25 @@
         StructureData(structures=structures, energies=energies, forces=forces)
 
     assert (
         str(exc.value)
         == f"Inconsistent number of structures and labels: {len(structures)=}, "
         f"{len(forces)=}"
     )
+
+
+def test_dataset_no_shuffling():
+    n_samples = 100
+    structure_ids = list(range(n_samples))
+
+    structure_data = StructureData(
+        structures=[NaCl.copy() for _ in range(n_samples)],
+        energies=np.random.random(n_samples),
+        forces=np.random.random([n_samples, 2, 3]),
+        stresses=np.random.random([n_samples, 3, 3]),
+        magmoms=np.random.random([n_samples, 2, 1]),
+        structure_ids=structure_ids,
+        shuffle=False,
+    )
+    sample_ids = [data[0].mp_id for data in structure_data]
+    # shuffle=False means structure_ids should be in order
+    assert sample_ids == structure_ids
```

### Comparing `chgnet-0.3.5/tests/test_encoders.py` & `chgnet-0.3.7/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/tests/test_graph.py` & `chgnet-0.3.7/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/tests/test_md.py` & `chgnet-0.3.7/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/tests/test_model.py` & `chgnet-0.3.7/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,27 +224,30 @@
     capsys: pytest.CaptureFixture, monkeypatch: pytest.MonkeyPatch
 ) -> None:
     model = CHGNet.load(use_device="cpu")
     v030_key, v030_params = "0.3.0", 412_525
     assert model.version == v030_key
     assert model.n_params == v030_params
     stdout, stderr = capsys.readouterr()
-    expected_stdout = lambda version, params: (
-        f"CHGNet v{version} initialized with {params:,} parameters\n"
+
+    assert stdout == (
+        f"CHGNet v{v030_key} initialized with {v030_params:,} parameters\n"
         "CHGNet will run on cpu\n"
     )
-    assert stdout == expected_stdout(v030_key, v030_params)
     assert stderr == ""
 
     v020_key, v020_params = "0.2.0", 400_438
     model = CHGNet.load(model_name=v020_key, use_device="cpu")
     assert model.version == v020_key
     assert model.n_params == v020_params
     stdout, stderr = capsys.readouterr()
-    assert stdout == expected_stdout(v020_key, v020_params)
+    assert stdout == (
+        f"CHGNet v{v020_key} initialized with {v020_params:,} parameters\n"
+        "CHGNet will run on cpu\n"
+    )
     assert stderr == ""
 
     model_name = "0.1.0"  # invalid
     with pytest.raises(ValueError, match=f"Unknown {model_name=}"):
         CHGNet.load(model_name=model_name)
 
     #     # set CHGNET_DEVICE to "cuda" and test
```

### Comparing `chgnet-0.3.5/tests/test_relaxation.py` & `chgnet-0.3.7/tests/test_relaxation.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/tests/test_trainer.py` & `chgnet-0.3.7/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `chgnet-0.3.5/tests/test_utils.py` & `chgnet-0.3.7/tests/test_utils.py`

 * *Files identical despite different names*

