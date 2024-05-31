# Comparing `tmp/lpath_md-1.0.2.tar.gz` & `tmp/lpath_md-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpath_md-1.0.2.tar", last modified: Tue May 21 19:37:22 2024, max compression
+gzip compressed data, was "lpath_md-1.0.3.tar", last modified: Fri May 31 22:48:36 2024, max compression
```

## Comparing `lpath_md-1.0.2.tar` & `lpath_md-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.082848 lpath_md-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-21 19:37:17.000000 lpath_md-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-21 19:37:17.000000 lpath_md-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-21 19:37:17.000000 lpath_md-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-21 19:37:22.082848 lpath_md-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-21 19:37:17.000000 lpath_md-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.078848 lpath_md-1.0.2/lpath/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    37269 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.074848 lpath_md-1.0.2/lpath/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.078848 lpath_md-1.0.2/lpath/data/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/data/styles/default.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/extloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    44451 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/extract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3669 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/lpath.py
--rw-r--r--   0 runner    (1001) docker     (127)    36321 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/match.py
--rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.078848 lpath_md-1.0.2/lpath/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_lpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.078848 lpath_md-1.0.2/lpath_md.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:37:21.000000 lpath_md-1.0.2/lpath_md.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-21 19:37:17.000000 lpath_md-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-21 19:37:22.082848 lpath_md-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:48:36.182231 lpath_md-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-31 22:48:31.000000 lpath_md-1.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-31 22:48:31.000000 lpath_md-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 22:48:31.000000 lpath_md-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-31 22:48:36.182231 lpath_md-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-31 22:48:31.000000 lpath_md-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:48:36.178230 lpath_md-1.0.3/lpath/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 22:48:36.000000 lpath_md-1.0.3/lpath/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37269 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:48:36.174230 lpath_md-1.0.3/lpath/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:48:36.178230 lpath_md-1.0.3/lpath/data/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/data/styles/default.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/extloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44451 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3669 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/lpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36321 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22808 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:48:36.182231 lpath_md-1.0.3/lpath/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/tests/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/tests/test_discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/tests/test_lpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-31 22:48:31.000000 lpath_md-1.0.3/lpath/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:48:36.182231 lpath_md-1.0.3/lpath_md.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-31 22:48:36.000000 lpath_md-1.0.3/lpath_md.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-31 22:48:36.000000 lpath_md-1.0.3/lpath_md.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:48:36.000000 lpath_md-1.0.3/lpath_md.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 22:48:36.000000 lpath_md-1.0.3/lpath_md.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:48:35.000000 lpath_md-1.0.3/lpath_md.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 22:48:36.000000 lpath_md-1.0.3/lpath_md.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 22:48:36.000000 lpath_md-1.0.3/lpath_md.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-31 22:48:31.000000 lpath_md-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-31 22:48:36.182231 lpath_md-1.0.3/setup.cfg
```

### Comparing `lpath_md-1.0.2/CODE_OF_CONDUCT.md` & `lpath_md-1.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/LICENSE` & `lpath_md-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/PKG-INFO` & `lpath_md-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpath-md
-Version: 1.0.2
+Version: 1.0.3
 Summary: A user-friendly, Python tool for clustering pathways from molecular dynamics simulations.
 Author-email: Anthony Bogetti <atb43@pitt.edu>, Jeremy Leung <jml230@pitt.edu>, Lillian Chong <lchong@pitt.edu>
 Maintainer-email: Jeremy Leung <jml230@pitt.edu>
 License: MIT
 Project-URL: Source, https://github.com/chonglab-pitt/lpath/
 Project-URL: Documentation, https://lpath.readthedocs.io/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lpath_md-1.0.2/README.md` & `lpath_md-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/_logger.py` & `lpath_md-1.0.3/lpath/_logger.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/argparser.py` & `lpath_md-1.0.3/lpath/argparser.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/discretize.py` & `lpath_md-1.0.3/lpath/discretize.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/extloader.py` & `lpath_md-1.0.3/lpath/extloader.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/extract.py` & `lpath_md-1.0.3/lpath/extract.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/io.py` & `lpath_md-1.0.3/lpath/io.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/lpath.py` & `lpath_md-1.0.3/lpath/lpath.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/match.py` & `lpath_md-1.0.3/lpath/match.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/plot.py` & `lpath_md-1.0.3/lpath/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         # Report number of pathways.
         self.n_pathways = len(self.pathways)
         log.info(f'There are {self.n_pathways} pathways.')
 
         for pathway in self.pathways:
             non_zero = pathway[numpy.nonzero(pathway[:, 0])]  # Removing padding frames...
             weights.append(non_zero[-1, -1])
-            durations.append(len(non_zero))
+            durations.append(len(non_zero) / arguments.stride)
             target_iter.append(non_zero[-1][0])
             iter_num += [frame[0] for frame in non_zero]
             states.append(pathway[:, 2])
 
         for cluster in set(self.cluster_labels):
             path_indices.append(numpy.where(self.cluster_labels == cluster)[0])
 
@@ -165,14 +165,15 @@
         self.weights = numpy.asarray(weights)
         self.durations = numpy.asarray(durations)
         self.states = numpy.asarray(states, dtype=object)
         self.path_indices = path_indices
         self.num_iter = numpy.asarray(iter_num, dtype=object)
         self.target_iter = numpy.asarray(target_iter)
         self.num_clusters = len(path_indices)
+        self.stride = arguments.stride
 
         # weighted_counts = [numpy.sum(self.weights[self.states == i]) for i in range(self.num_clusters)]
         # self.weighted_counts = numpy.array(weighted_counts, dtype=float)
 
         self.min_iter = min(self.num_iter)
         self.max_iter = max(self.num_iter)
         self.interval = 25 if self.max_iter - self.min_iter > 50 else 5
@@ -188,14 +189,17 @@
 
         # Set up dummy variables for the plots!
         self.fig = None
         self.ax = None
         self.show_fig = arguments.dendrogram_show
         self.ax_idx = 0
 
+        if not self.show_fig:
+            matplotlib.use('agg')
+
     def plt_config(self, ax_idx=None, separate=None):
         """
         Process matplotlib arguments and append fig/axis objects to class.
 
         ax_idx = list or int
             Index or list of indic
```

### Comparing `lpath_md-1.0.2/lpath/tests/conftest.py` & `lpath_md-1.0.3/lpath/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/tests/test_argparser.py` & `lpath_md-1.0.3/lpath/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/tests/test_extract.py` & `lpath_md-1.0.3/lpath/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath/tests/test_match.py` & `lpath_md-1.0.3/lpath/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/lpath_md.egg-info/PKG-INFO` & `lpath_md-1.0.3/lpath_md.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpath-md
-Version: 1.0.2
+Version: 1.0.3
 Summary: A user-friendly, Python tool for clustering pathways from molecular dynamics simulations.
 Author-email: Anthony Bogetti <atb43@pitt.edu>, Jeremy Leung <jml230@pitt.edu>, Lillian Chong <lchong@pitt.edu>
 Maintainer-email: Jeremy Leung <jml230@pitt.edu>
 License: MIT
 Project-URL: Source, https://github.com/chonglab-pitt/lpath/
 Project-URL: Documentation, https://lpath.readthedocs.io/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lpath_md-1.0.2/lpath_md.egg-info/SOURCES.txt` & `lpath_md-1.0.3/lpath_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lpath_md-1.0.2/pyproject.toml` & `lpath_md-1.0.3/pyproject.toml`

 * *Files identical despite different names*

