# Comparing `tmp/ParticlePhaseSpace-0.5.5.tar.gz` & `tmp/particlephasespace-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParticlePhaseSpace-0.5.5.tar", last modified: Wed Aug 30 03:33:25 2023, max compression
+gzip compressed data, was "particlephasespace-0.6.0.tar", last modified: Sat Jun  1 03:27:53 2024, max compression
```

## Comparing `ParticlePhaseSpace-0.5.5.tar` & `particlephasespace-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 03:33:25.815778 ParticlePhaseSpace-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (999)    35149 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     2846 2023-08-30 03:33:25.815778 ParticlePhaseSpace-0.5.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 03:33:25.815778 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/
--rw-r--r--   0 runner    (1001) docker     (999)    12310 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/DataExporters.py
--rw-r--r--   0 runner    (1001) docker     (999)    29377 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/DataLoaders.py
--rw-r--r--   0 runner    (1001) docker     (999)    82041 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/_ParticlePhaseSpace.py
--rw-r--r--   0 runner    (1001) docker     (999)      229 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2275 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/__particle_config__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5268 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/__phase_space_config__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6537 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/__unit_config__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2755 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 03:33:25.815778 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2846 2023-08-30 03:33:25.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      768 2023-08-30 03:33:25.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 03:33:25.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       42 2023-08-30 03:33:25.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       19 2023-08-30 03:33:25.000000 ParticlePhaseSpace-0.5.5/ParticlePhaseSpace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     2256 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       93 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      811 2023-08-30 03:33:25.815778 ParticlePhaseSpace-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 03:33:25.815778 ParticlePhaseSpace-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (999)    17389 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/tests/test_ParticlePhaseSpace.py
--rw-r--r--   0 runner    (1001) docker     (999)     4500 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (999)     4959 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (999)     1064 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/tests/test_notebooks_run.py
--rw-r--r--   0 runner    (1001) docker     (999)     1427 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/tests/test_phase_space_config.py
--rw-r--r--   0 runner    (1001) docker     (999)     1166 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/tests/test_supported_particles.py
--rw-r--r--   0 runner    (1001) docker     (999)     5382 2023-08-30 03:33:14.000000 ParticlePhaseSpace-0.5.5/tests/test_unit_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:27:53.431003 particlephasespace-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-06-01 03:27:53.431003 particlephasespace-0.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:27:53.431003 particlephasespace-0.6.0/ParticlePhaseSpace/
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/ParticlePhaseSpace/DataExporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29385 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/ParticlePhaseSpace/DataLoaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82041 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/ParticlePhaseSpace/_ParticlePhaseSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/ParticlePhaseSpace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/ParticlePhaseSpace/__particle_config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/ParticlePhaseSpace/__phase_space_config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/ParticlePhaseSpace/__unit_config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/ParticlePhaseSpace/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:27:53.431003 particlephasespace-0.6.0/ParticlePhaseSpace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-06-01 03:27:53.000000 particlephasespace-0.6.0/ParticlePhaseSpace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-06-01 03:27:53.000000 particlephasespace-0.6.0/ParticlePhaseSpace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:27:53.000000 particlephasespace-0.6.0/ParticlePhaseSpace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-01 03:27:53.000000 particlephasespace-0.6.0/ParticlePhaseSpace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 03:27:53.000000 particlephasespace-0.6.0/ParticlePhaseSpace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-06-01 03:27:53.435003 particlephasespace-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:27:53.431003 particlephasespace-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17389 2024-06-01 03:27:48.000000 particlephasespace-0.6.0/tests/test_ParticlePhaseSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-06-01 03:27:49.000000 particlephasespace-0.6.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-06-01 03:27:49.000000 particlephasespace-0.6.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-01 03:27:49.000000 particlephasespace-0.6.0/tests/test_notebooks_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-06-01 03:27:49.000000 particlephasespace-0.6.0/tests/test_phase_space_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-06-01 03:27:49.000000 particlephasespace-0.6.0/tests/test_supported_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-06-01 03:27:49.000000 particlephasespace-0.6.0/tests/test_unit_conversions.py
```

### Comparing `ParticlePhaseSpace-0.5.5/LICENSE` & `particlephasespace-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/PKG-INFO` & `particlephasespace-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: ParticlePhaseSpace
-Version: 0.5.5
+Version: 0.6.0
 Summary: Import, analyze, manipulate, and export particle phase space data
 Home-page: https://github.com/bwheelz36/ParticlePhaseSpace
 Author: Brendan Whelan
 Author-email: bwheelz36@gmail.com
 Project-URL: Bug Tracker, https://github.com/bwheelz36/ParticlePhaseSpace/issues
 Project-URL: Documentation, https://bwheelz36.github.io/ParticlePhaseSpace
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: topas2numpy
+Requires-Dist: scipy
 
 # ParticlePhaseSpace
 
 ![tests](https://github.com/bwheelz36/ParticlePhaseSpace/actions/workflows/run_tests.yml/badge.svg)![tests](https://github.com/bwheelz36/ParticlePhaseSpace/actions/workflows/build_docs.yml/badge.svg)[![codecov](https://codecov.io/gh/bwheelz36/ParticlePhaseSpace/branch/main/graph/badge.svg?token=T44KBJ7INR)](https://codecov.io/gh/bwheelz36/ParticlePhaseSpace)[![PyPI version](https://badge.fury.io/py/ParticlePhaseSpace.svg)](https://badge.fury.io/py/ParticlePhaseSpace)
 
 Common library for dealing with particle phase spaces, revolving around the simple workflow of `import`, `analyse`, `export`. If you have a data format that we can't already work with, extension mechanisms are provided for writing new `DataLoaders` and `DataExporters`.
```

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/DataExporters.py` & `particlephasespace-0.6.0/ParticlePhaseSpace/DataExporters.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/DataLoaders.py` & `particlephasespace-0.6.0/ParticlePhaseSpace/DataLoaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     :param input_data: location of file to read, or data to read
     :param particle_type: optional parameter if phase space format does not specify particle.
         particle type is a string matching a particle name from particle config
     :param units:  optionally specify units by passing a unit set
     """
 
-    def __init__(self, input_data: (str, Path), particle_type:str=None, units:UnitSet=units('mm_MeV')):
+    def __init__(self, input_data: (str, Path), particle_type:(str, None)=None, units:UnitSet=units('mm_MeV')):
 
         self.data = pd.DataFrame()
         if not isinstance(units, UnitSet):
             raise TypeError('units must be an instance of articlePhaseSpace.__unit_config__._UnitSet.'
                             'UnitSets are accessed through the ParticlePhaseSpaceUnits class')
         self._units = units
         self._columns = ps_cfg.get_all_column_names(self._units)
```

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/_ParticlePhaseSpace.py` & `particlephasespace-0.6.0/ParticlePhaseSpace/_ParticlePhaseSpace.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/__particle_config__.py` & `particlephasespace-0.6.0/ParticlePhaseSpace/__particle_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/__phase_space_config__.py` & `particlephasespace-0.6.0/ParticlePhaseSpace/__phase_space_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/__unit_config__.py` & `particlephasespace-0.6.0/ParticlePhaseSpace/__unit_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace/utilities.py` & `particlephasespace-0.6.0/ParticlePhaseSpace/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import numpy as np
 import ParticlePhaseSpace.__phase_space_config__ as ps_cfg
 import ParticlePhaseSpace.__particle_config__ as particle_cfg
 from ParticlePhaseSpace import ParticlePhaseSpaceUnits
 from ParticlePhaseSpace import UnitSet
+import numpy as np
 
 def _check_particle_types(pdg_codes):
     """
     check that the particle types in the phase space are known particle types
     """
+
+
     for code in pdg_codes:
+
         try:
+            assert isinstance(code, (int, np.integer))
             test = particle_cfg.particle_properties[code]
         except:
             raise AttributeError(f'unknown particle type {particle_cfg.particle_properties[code]["name"]}')
 
 
 def get_rest_masses_from_pdg_codes(pdg_codes):
     """
```

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace.egg-info/PKG-INFO` & `particlephasespace-0.6.0/ParticlePhaseSpace.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: ParticlePhaseSpace
-Version: 0.5.5
+Version: 0.6.0
 Summary: Import, analyze, manipulate, and export particle phase space data
 Home-page: https://github.com/bwheelz36/ParticlePhaseSpace
 Author: Brendan Whelan
 Author-email: bwheelz36@gmail.com
 Project-URL: Bug Tracker, https://github.com/bwheelz36/ParticlePhaseSpace/issues
 Project-URL: Documentation, https://bwheelz36.github.io/ParticlePhaseSpace
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: topas2numpy
+Requires-Dist: scipy
 
 # ParticlePhaseSpace
 
 ![tests](https://github.com/bwheelz36/ParticlePhaseSpace/actions/workflows/run_tests.yml/badge.svg)![tests](https://github.com/bwheelz36/ParticlePhaseSpace/actions/workflows/build_docs.yml/badge.svg)[![codecov](https://codecov.io/gh/bwheelz36/ParticlePhaseSpace/branch/main/graph/badge.svg?token=T44KBJ7INR)](https://codecov.io/gh/bwheelz36/ParticlePhaseSpace)[![PyPI version](https://badge.fury.io/py/ParticlePhaseSpace.svg)](https://badge.fury.io/py/ParticlePhaseSpace)
 
 Common library for dealing with particle phase spaces, revolving around the simple workflow of `import`, `analyse`, `export`. If you have a data format that we can't already work with, extension mechanisms are provided for writing new `DataLoaders` and `DataExporters`.
```

### Comparing `ParticlePhaseSpace-0.5.5/ParticlePhaseSpace.egg-info/SOURCES.txt` & `particlephasespace-0.6.0/ParticlePhaseSpace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/README.md` & `particlephasespace-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/setup.cfg` & `particlephasespace-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/tests/test_ParticlePhaseSpace.py` & `particlephasespace-0.6.0/tests/test_ParticlePhaseSpace.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/tests/test_export.py` & `particlephasespace-0.6.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/tests/test_import.py` & `particlephasespace-0.6.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/tests/test_notebooks_run.py` & `particlephasespace-0.6.0/tests/test_notebooks_run.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/tests/test_phase_space_config.py` & `particlephasespace-0.6.0/tests/test_phase_space_config.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/tests/test_supported_particles.py` & `particlephasespace-0.6.0/tests/test_supported_particles.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.5/tests/test_unit_conversions.py` & `particlephasespace-0.6.0/tests/test_unit_conversions.py`

 * *Files identical despite different names*

