# Comparing `tmp/sim-solps-0.1.2.tar.gz` & `tmp/sim_solps-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sim-solps-0.1.2.tar", last modified: Tue May 24 12:04:19 2022, max compression
+gzip compressed data, was "sim_solps-0.1.3.tar", last modified: Sat Jun  1 12:26:20 2024, max compression
```

## Comparing `sim-solps-0.1.2.tar` & `sim_solps-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.203695 sim-solps-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.195695 sim-solps-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.199695 sim-solps-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-05-24 12:03:56.000000 sim-solps-0.1.2/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-05-24 12:03:56.000000 sim-solps-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-05-24 12:03:56.000000 sim-solps-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-05-24 12:04:19.203695 sim-solps-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-05-24 12:03:56.000000 sim-solps-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.199695 sim-solps-0.1.2/demos/
--rw-r--r--   0 runner    (1001) docker     (121)    55713 2022-05-24 12:03:56.000000 sim-solps-0.1.2/demos/SolpsInterface_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    88357 2022-05-24 12:03:56.000000 sim-solps-0.1.2/demos/ThomsonScattering_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.199695 sim-solps-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.199695 sim-solps-0.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     5433 2022-05-24 12:03:56.000000 sim-solps-0.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-05-24 12:03:56.000000 sim-solps-0.1.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-05-24 12:03:56.000000 sim-solps-0.1.2/docs/source/interface.rst
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-05-24 12:03:56.000000 sim-solps-0.1.2/docs/source/thomson.rst
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-05-24 12:03:56.000000 sim-solps-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-05-24 12:04:19.203695 sim-solps-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-24 12:03:56.000000 sim-solps-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.199695 sim-solps-0.1.2/sim_solps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-05-24 12:04:18.000000 sim-solps-0.1.2/sim_solps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-05-24 12:04:19.000000 sim-solps-0.1.2/sim_solps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-24 12:04:18.000000 sim-solps-0.1.2/sim_solps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-24 12:04:18.000000 sim-solps-0.1.2/sim_solps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-24 12:04:19.000000 sim-solps-0.1.2/sim_solps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.203695 sim-solps-0.1.2/sims/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-05-24 12:03:56.000000 sim-solps-0.1.2/sims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-24 12:04:17.000000 sim-solps-0.1.2/sims/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-24 12:03:56.000000 sim-solps-0.1.2/sims/instruments.py
--rw-r--r--   0 runner    (1001) docker     (121)     8433 2022-05-24 12:03:56.000000 sim-solps-0.1.2/sims/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-24 12:03:56.000000 sim-solps-0.1.2/sims/likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (121)     7290 2022-05-24 12:03:56.000000 sim-solps-0.1.2/sims/thomson.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 12:04:19.203695 sim-solps-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-05-24 12:03:56.000000 sim-solps-0.1.2/tests/test_thomson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.984145 sim_solps-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.976144 sim_solps-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.980144 sim_solps-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-01 12:26:06.000000 sim_solps-0.1.3/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-06-01 12:26:06.000000 sim_solps-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-01 12:26:06.000000 sim_solps-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-06-01 12:26:20.984145 sim_solps-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-06-01 12:26:06.000000 sim_solps-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.980144 sim_solps-0.1.3/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)    55713 2024-06-01 12:26:06.000000 sim_solps-0.1.3/demos/SolpsInterface_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    88357 2024-06-01 12:26:06.000000 sim_solps-0.1.3/demos/ThomsonScattering_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.980144 sim_solps-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-01 12:26:06.000000 sim_solps-0.1.3/docs/docs_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.980144 sim_solps-0.1.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-06-01 12:26:06.000000 sim_solps-0.1.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-06-01 12:26:06.000000 sim_solps-0.1.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-01 12:26:06.000000 sim_solps-0.1.3/docs/source/interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-06-01 12:26:06.000000 sim_solps-0.1.3/docs/source/thomson.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-06-01 12:26:06.000000 sim_solps-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 12:26:20.984145 sim_solps-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 12:26:06.000000 sim_solps-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.984145 sim_solps-0.1.3/sim_solps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-06-01 12:26:20.000000 sim_solps-0.1.3/sim_solps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-01 12:26:20.000000 sim_solps-0.1.3/sim_solps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 12:26:20.000000 sim_solps-0.1.3/sim_solps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-01 12:26:20.000000 sim_solps-0.1.3/sim_solps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 12:26:20.000000 sim_solps-0.1.3/sim_solps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.984145 sim_solps-0.1.3/sims/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-01 12:26:06.000000 sim_solps-0.1.3/sims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 12:26:20.000000 sim_solps-0.1.3/sims/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.984145 sim_solps-0.1.3/sims/instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 12:26:06.000000 sim_solps-0.1.3/sims/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-06-01 12:26:06.000000 sim_solps-0.1.3/sims/instruments/thomson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-06-01 12:26:06.000000 sim_solps-0.1.3/sims/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 12:26:06.000000 sim_solps-0.1.3/sims/likelihoods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 12:26:20.984145 sim_solps-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-01 12:26:06.000000 sim_solps-0.1.3/tests/test_thomson.py
```

### Comparing `sim-solps-0.1.2/.github/workflows/python_publish.yml` & `sim_solps-0.1.3/.github/workflows/python_publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     types: [published]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build twine
       - name: Build package
```

### Comparing `sim-solps-0.1.2/LICENSE` & `sim_solps-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sim-solps-0.1.2/README.md` & `sim_solps-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sim-solps-0.1.2/demos/SolpsInterface_demo.ipynb` & `sim_solps-0.1.3/demos/SolpsInterface_demo.ipynb`

 * *Files identical despite different names*

### Comparing `sim-solps-0.1.2/demos/ThomsonScattering_demo.ipynb` & `sim_solps-0.1.3/demos/ThomsonScattering_demo.ipynb`

 * *Files identical despite different names*

### Comparing `sim-solps-0.1.2/docs/source/conf.py` & `sim_solps-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sim-solps-0.1.2/sim_solps.egg-info/SOURCES.txt` & `sim_solps-0.1.3/sim_solps.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 .readthedocs.yaml
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 .github/workflows/python_publish.yml
 demos/SolpsInterface_demo.ipynb
 demos/ThomsonScattering_demo.ipynb
+docs/docs_requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/interface.rst
 docs/source/thomson.rst
 sim_solps.egg-info/PKG-INFO
 sim_solps.egg-info/SOURCES.txt
 sim_solps.egg-info/dependency_links.txt
 sim_solps.egg-info/requires.txt
 sim_solps.egg-info/top_level.txt
 sims/__init__.py
 sims/_version.py
-sims/instruments.py
 sims/interface.py
 sims/likelihoods.py
-sims/thomson.py
+sims/instruments/__init__.py
+sims/instruments/thomson.py
 tests/test_thomson.py
```

### Comparing `sim-solps-0.1.2/sims/interface.py` & `sim_solps-0.1.3/sims/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,96 @@
-
-from numpy import array, concatenate, zeros, full
+from numpy import array, concatenate, zeros, full, ndarray
 from scipy.io import netcdf
 from tokamesh import TriangularMesh
 from tokamesh.construction import remove_duplicate_vertices
 import matplotlib.pyplot as plt
-from matplotlib.cm import get_cmap
+from matplotlib import colormaps
 
 
-class SolpsInterface(object):
+class SolpsInterface:
     """
     A class which provides an interface to the results of SOLPS-ITER
     simulations stored in a balance.nc file.
 
     The value of a variable at any set of (R, z) positions can be accessed
     using the ``get`` method. A list of available variables can be obtained
     using the ``variables`` method.
 
     :param balance_filepath: \
         A path to a balance.nc file.
     """
+
     def __init__(self, balance_filepath):
-        with netcdf.netcdf_file(balance_filepath, 'r') as solps:
+        with netcdf.netcdf_file(balance_filepath, "r") as solps:
             # TODO - check we're cutting out correct cells from den_n
-            den_i = solps.variables['na'].data.copy()
+            den_i = solps.variables["na"].data.copy()
             trim = (slice(None), slice(None), slice(0, den_i.shape[-1]))
-            den_n = solps.variables['dab2'].data[trim].copy()
-            tab2 = solps.variables['tab2'].data[trim].copy() / 1.602e-19
+            den_n = solps.variables["dab2"].data[trim].copy()
+            tab2 = solps.variables["tab2"].data[trim].copy() / 1.602e-19
 
-            self.ne = solps.variables['ne'].data.copy().flatten()
-            self.te = solps.variables['te'].data.copy().flatten() / 1.602e-19
-            self.ti = solps.variables['ti'].data.copy().flatten() / 1.602e-19
-            self.vol = solps.variables['vol'].data.copy().flatten()
-            self.dmb2 = solps.variables['dmb2'].data[trim].copy().flatten()
-            self.tmb2 = solps.variables['tmb2'].data[trim].copy().flatten() / 1.602e-19
+            self.ne = solps.variables["ne"].data.copy().flatten()
+            self.te = solps.variables["te"].data.copy().flatten() / 1.602e-19
+            self.ti = solps.variables["ti"].data.copy().flatten() / 1.602e-19
+            self.vol = solps.variables["vol"].data.copy().flatten()
+            self.dmb2 = solps.variables["dmb2"].data[trim].copy().flatten()
+            self.tmb2 = solps.variables["tmb2"].data[trim].copy().flatten() / 1.602e-19
 
             self.n_cells = self.ne.size
             self.variable_map = {k: v for k, v in solps_variable_map.items()}
             # process the species data into regular strings
-            species_bytestrings = solps.variables['species'].data.copy()
-            species = [''.join([a.decode('ASCII') for a in s]).strip() for s in species_bytestrings]
+            species_bytestrings = solps.variables["species"].data.copy()
+            species = [
+                "".join([a.decode("ASCII") for a in s]).strip()
+                for s in species_bytestrings
+            ]
             # now separate out the ions from the neutrals
-            ions = [(i, ''.join(s.split('+'))) for i, s in enumerate(species) if '+' in s]
-            self.neutrals = [s for s in species if '+' not in s]
+            ions = [
+                (i, "".join(s.split("+"))) for i, s in enumerate(species) if "+" in s
+            ]
+            self.neutrals = [s for s in species if "+" not in s]
             self.ions = [i[1] for i in ions]
             # set the ion densities
-            [setattr(self, f"n_{ion}", den_i[index, :, :].flatten()) for index, ion in ions]
+            [
+                setattr(self, f"n_{ion}", den_i[index, :, :].flatten())
+                for index, ion in ions
+            ]
             # set the neutral densities and temperatures
             for index, neutral in enumerate(self.neutrals):
                 setattr(self, f"n_{neutral}", den_n[index, :, :].flatten())
                 setattr(self, f"t_{neutral}", tab2[index, :, :].flatten())
 
             # build variable names for the ions and neutrals
             ion_dens = {f"{ion} density": f"n_{ion}" for ion in self.ions}
-            neutral_dens = {f"{neutral} density": f"n_{neutral}" for neutral in self.neutrals}
-            neutral_temp = {f"{neutral} temperature": f"t_{neutral}" for neutral in self.neutrals}
+            neutral_dens = {
+                f"{neutral} density": f"n_{neutral}" for neutral in self.neutrals
+            }
+            neutral_temp = {
+                f"{neutral} temperature": f"t_{neutral}" for neutral in self.neutrals
+            }
             # add them to the variable mapping
-            self.variable_map = {**self.variable_map, **ion_dens, **neutral_dens, **neutral_temp}
+            self.variable_map = {
+                **self.variable_map,
+                **ion_dens,
+                **neutral_dens,
+                **neutral_temp,
+            }
 
             # find the cell centres
-            crx = solps.variables['crx'].data.copy()
-            cry = solps.variables['cry'].data.copy()
+            crx = solps.variables["crx"].data.copy()
+            cry = solps.variables["cry"].data.copy()
             self.cr = crx.mean(axis=0)
             self.cz = cry.mean(axis=0)
             R_sets = [v for v in crx.reshape([4, self.n_cells]).T]
             z_sets = [v for v in cry.reshape([4, self.n_cells]).T]
 
             del den_n, den_i, tab2, species_bytestrings
 
         # build the mesh data by splitting each cell into two triangles
         R, z, triangles = connect_meshes(
-            R_sets,
-            z_sets,
-            [triangles_from_grid([2,2])]*self.n_cells
+            R_sets, z_sets, [triangles_from_grid([2, 2])] * self.n_cells
         )
 
         # now we need to sort the triangles into the same order as the SOLPS cells.
         old_Rc = zeros(2 * self.n_cells)
         old_Rc[0::2] = crx[array([0, 1, 2]), :].mean(axis=0).flatten()
         old_Rc[1::2] = crx[array([1, 2, 3]), :].mean(axis=0).flatten()
 
@@ -87,15 +102,15 @@
         new_zc = z[triangles].mean(axis=1)
 
         inverse_sort = double_argsort(old_Rc, old_zc).argsort()
         descrambler = double_argsort(new_Rc, new_zc)[inverse_sort]
         triangles = triangles[descrambler, :]
         self.mesh = TriangularMesh(R=R, z=z, triangles=triangles)
 
-    def check_variable(self, variable):
+    def check_variable(self, variable: str) -> str:
         if type(variable) is not str:
             raise TypeError(
                 f"""
                 SOLPS variables must be specified as strings, but instead
                 type {type(variable)} was given.
                 """
             )
@@ -106,23 +121,23 @@
                 f"""
                 The given string '{variable}' does not match any SOLPS variables
                 stored by SolpsInterface.
                 """
             )
         return v
 
-    def variables(self):
+    def variables(self) -> list[str]:
         """
         Returns a list containing all available variables.
 
         :return: A list of the available variables.
         """
         return [k for k in self.variable_map]
 
-    def get(self, variable, R, z, outside_value=0):
+    def get(self, variable: str, R: ndarray, z: ndarray, outside_value=0) -> ndarray:
         """
         Returns the value of a chosen variable at a given set of points.
 
         :param variable: \
             A string indicating which variable to retrieve.
 
         :param R: \
@@ -137,55 +152,57 @@
         :return: \
             The values of the variable at the given points as a 1D numpy array.
         """
         v = self.check_variable(variable)
         inds = self.mesh.find_triangle(R, z)
         inside = inds != -1
         values = full(R.shape, fill_value=outside_value, dtype=float)
-        values[inside] = getattr(self, v)[inds//2][inside]
+        values[inside] = getattr(self, v)[inds // 2][inside]
         return values
 
-    def plot(self, variable, draw_mesh=False):
+    def plot(self, variable: str, draw_mesh=False):
         """
         Generate a colour plot of a chosen variable.
 
         :param str variable: A string indicating which variable to plot.
         :param bool draw_mesh: A bool indicating whether to draw the mesh in the plot.
         """
         v = self.check_variable(variable)
-        vals = zeros(2*self.n_cells)
+        vals = zeros(2 * self.n_cells)
         vals[0::2] = getattr(self, v)
         vals[1::2] = getattr(self, v)
-        cmap = get_cmap('viridis')
+        cmap = colormaps["viridis"]
 
         dR = self.mesh.R_limits[1] - self.mesh.R_limits[0]
         dz = self.mesh.z_limits[1] - self.mesh.z_limits[0]
-        fig = plt.figure(figsize=(8*(dR/dz)*1.8, 8))
+        fig = plt.figure(figsize=(8 * (dR / dz) * 1.8, 8))
         ax = fig.add_subplot(111)
-        ax.set_facecolor(cmap(0.))
-        tricol = ax.tripcolor(self.mesh.R, self.mesh.z, self.mesh.triangle_vertices, facecolors=vals)
+        ax.set_facecolor(cmap(0.0))
+        tricol = ax.tripcolor(
+            self.mesh.R, self.mesh.z, self.mesh.triangle_vertices, facecolors=vals
+        )
         plt.colorbar(tricol, ax=ax, aspect=30, pad=0.02, label=variable)
         if draw_mesh:
             self.mesh.draw(ax, lw=0.5)
-        ax.axis('equal')
-        ax.set_xlabel('R (m)')
-        ax.set_ylabel('z (m)')
+        ax.axis("equal")
+        ax.set_xlabel("R (m)")
+        ax.set_ylabel("z (m)")
         fig.subplots_adjust(top=0.95, bottom=0.1)
         plt.show()
 
 
-def triangles_from_grid(grid_shape):
+def triangles_from_grid(grid_shape: tuple[int, int]) -> ndarray:
     triangles = []
     m, n = grid_shape
     for i in range(m - 1):
         for j in range(n - 1):
-            v1 = n*i + j
-            v2 = n*(i+1) + j
-            v3 = n*i + j + 1
-            v4 = n*(i+1) + j + 1
+            v1 = n * i + j
+            v2 = n * (i + 1) + j
+            v3 = n * i + j + 1
+            v4 = n * (i + 1) + j + 1
             triangles.append([v1, v2, v3])
             triangles.append([v2, v3, v4])
     return array(triangles, dtype=int)
 
 
 def double_argsort(R, z):
     z_sorter = z.argsort()
@@ -193,19 +210,21 @@
 
 
 def connect_meshes(R_arrays, z_arrays, triangle_arrays):
     R = concatenate(R_arrays)
     z = concatenate(z_arrays)
     offsets = zeros(len(R_arrays), dtype=int)
     offsets[1:] = array([a.size for a in R_arrays], dtype=int)[:-1].cumsum()
-    triangles = concatenate([tri+off for tri, off in zip(triangle_arrays, offsets)], axis=0, dtype=int)
+    triangles = concatenate(
+        [tri + off for tri, off in zip(triangle_arrays, offsets)], axis=0, dtype=int
+    )
     return remove_duplicate_vertices(R, z, triangles)
 
 
 solps_variable_map = {
     "electron density": "ne",
     "electron temperature": "te",
     "ion temperature": "ti",
     "molecular density": "dmb2",
     "molecular temperature": "tmb2",
-    "cell volume": "vol"
+    "cell volume": "vol",
 }
```

### Comparing `sim-solps-0.1.2/sims/likelihoods.py` & `sim_solps-0.1.3/sims/likelihoods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from numpy import log, exp
 
 
 def gaussian_likelihood(data, errors, prediction):
     z = (data - prediction) / errors
-    return -0.5 * (z ** 2).sum()
+    return -0.5 * (z**2).sum()
 
 
 def cauchy_likelihood(data, errors, prediction):
     z = (data - prediction) / errors
-    return -log(1 + z ** 2).sum()
+    return -log(1 + z**2).sum()
 
 
 def laplace_likelihood(data, errors, prediction):
     z = (data - prediction) / errors
     return -abs(z).sum()
 
 
 def logistic_likelihood(data, errors, prediction):
     z = (prediction - data) / errors
-    f = z + 2*log(1 + exp(-z))
+    f = z + 2 * log(1 + exp(-z))
     return -f.sum()
```

### Comparing `sim-solps-0.1.2/sims/thomson.py` & `sim_solps-0.1.3/sims/instruments/thomson.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-
 from numpy import array, ones, nan, full, ndarray
 from sims.likelihoods import gaussian_likelihood
 
 
-class ThomsonScattering(object):
+class ThomsonScattering:
     """
     Synthetic instrument model for Thomson scattering.
 
     :param R: \
         Radius positions of the sampling points as a 2D numpy array of shape
         ``(num_channels, num_samples)``.
 
@@ -27,14 +26,15 @@
     :param measurements: \
         A dictionary containing Thomson-scattering measurement data to which
         the synthetic instrument predictions will be compared. The data should
         be given as 1D numpy arrays under the keys 'te_data', 'te_err', 'ne_data'
         and 'ne_err'. This keyword argument is required in order to use the
         ``log_likelihood`` method.
     """
+
     def __init__(self, R, z, weights, interface=None, measurements=None):
         self.shape = R.shape
         self.n_channels, self.n_samples = self.shape
         self.R = R
         self.z = z
         self.weights = weights
 
@@ -57,21 +57,21 @@
         self.z_p = None
         if interface is not None:
             self.update_interface(interface)
 
         # attributes for storing experimental data
         if measurements is not None:
             measurements = self.check_measurements(measurements)
-            self.te_data = measurements['te_data']
-            self.te_err = measurements['te_err']
-            self.ne_data = measurements['ne_data']
-            self.ne_err = measurements['ne_err']
+            self.te_data = measurements["te_data"]
+            self.te_err = measurements["te_err"]
+            self.ne_data = measurements["ne_data"]
+            self.ne_err = measurements["ne_err"]
 
     def check_measurements(self, measurements):
-        measurement_keys = ['te_data', 'te_err', 'ne_data', 'ne_err']
+        measurement_keys = ["te_data", "te_err", "ne_data", "ne_err"]
         for key in measurement_keys:
             if key not in measurements:
                 raise KeyError(
                     f"""
                     [ ThomsonScattering error ]
                     >> The dictionary passed via the 'measurements' keyword argument 
                     >> does not contain the required key '{key}'.
@@ -114,21 +114,19 @@
 
         :param interface: \
             An instance of ``SolpsInterface`` from the ``sims.interface`` module.
         """
         self.interface = interface
         # first find out which sample points are actually inside the mesh
         in_mesh = self.interface.mesh.interpolate(
-            self.R,
-            self.z,
-            ones(self.interface.mesh.n_vertices)
+            self.R, self.z, ones(self.interface.mesh.n_vertices)
         )
         # use this to find what total probability of the instrument function
         # is inside the mesh for each channel
-        probs = (in_mesh*self.weights).sum(axis=1)
+        probs = (in_mesh * self.weights).sum(axis=1)
         # only make predictions for channels where over 95%
         # of the probability is inside the mesh
         self.predicted_channels = (probs > 0.95).nonzero()
         # now re-normalise the weights to account of points outside the mesh
         self.p = (in_mesh * self.weights)[self.predicted_channels, :].squeeze()
         self.p = self.p / self.p.sum(axis=1)[:, None]
         # discard sample point data for channels outside mesh
@@ -139,16 +137,16 @@
         """
         Calculate predictions of the electron temperature and density measurements
         made by the instrument for the given SOLPS results.
 
         :return: \
             Predictions of the electron density and temperature as two numpy arrays.
         """
-        te_samples = self.interface.get('electron temperature', self.R_p, self.z_p)
-        ne_samples = self.interface.get('electron density', self.R_p, self.z_p)
+        te_samples = self.interface.get("electron temperature", self.R_p, self.z_p)
+        ne_samples = self.interface.get("electron density", self.R_p, self.z_p)
 
         ne_predictions = (ne_samples * self.p).sum(axis=1)
         te_predictions = (te_samples * ne_samples * self.p).sum(axis=1) / ne_predictions
 
         ne = full(self.n_channels, fill_value=nan)
         ne[self.predicted_channels] = ne_predictions
         te = full(self.n_channels, fill_value=nan)
@@ -168,17 +166,15 @@
 
         :return: The log-likelihood
         """
         ne_prediction, te_prediction = self.predict()
         te_ll = likelihood(
             self.te_data[self.predicted_channels],
             self.te_err[self.predicted_channels],
-            te_prediction[self.predicted_channels]
+            te_prediction[self.predicted_channels],
         )
         ne_ll = likelihood(
             self.ne_data[self.predicted_channels],
             self.ne_err[self.predicted_channels],
-            ne_prediction[self.predicted_channels]
+            ne_prediction[self.predicted_channels],
         )
         return te_ll + ne_ll
-
-
```

### Comparing `sim-solps-0.1.2/tests/test_thomson.py` & `sim_solps-0.1.3/tests/test_thomson.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 from numpy import linspace, exp
-from sims.thomson import ThomsonScattering
+from sims.instruments.thomson import ThomsonScattering
 import pytest
 
+
 @pytest.fixture
 def spatial_data():
-    mu = linspace(1., 1.4, 21)
+    mu = linspace(1.0, 1.4, 21)
     dR = linspace(-0.03, 0.03, 25)
 
     R = mu[:, None] - dR[None, :]
     sigma = 0.01
     z = (R - mu[:, None]) / sigma
-    weights = exp(-0.5*z**2)
+    weights = exp(-0.5 * z**2)
     weights /= weights.sum(axis=1)[:, None]
     return R, z, weights
 
 
 @pytest.fixture
 def measurements():
-    R = linspace(1., 1.4, 21)
-    te = 100 - (R - 1.)*200
-    ne = 1e19 - (R - 1.)*1e19
-    return {
-        "te_data": te,
-        "te_err": te * 0.1,
-        "ne_data": ne,
-        "ne_err": ne * 0.1
-    }
+    R = linspace(1.0, 1.4, 21)
+    te = 100 - (R - 1.0) * 200
+    ne = 1e19 - (R - 1.0) * 1e19
+    return {"te_data": te, "te_err": te * 0.1, "ne_data": ne, "ne_err": ne * 0.1}
 
 
 def test_measurement_parsing(spatial_data, measurements):
     R, z, weights = spatial_data
-    TS = ThomsonScattering(
-        R=R,
-        z=z,
-        weights=weights,
-        measurements=measurements
-    )
+    TS = ThomsonScattering(R=R, z=z, weights=weights, measurements=measurements)
```

