# Comparing `tmp/sourmash_plugin_betterplot-0.3.2.tar.gz` & `tmp/sourmash_plugin_betterplot-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_betterplot-0.3.2.tar", last modified: Mon May 20 01:11:15 2024, max compression
+gzip compressed data, was "sourmash_plugin_betterplot-0.3.3.tar", last modified: Sat Jun  1 13:32:42 2024, max compression
```

## Comparing `sourmash_plugin_betterplot-0.3.2.tar` & `sourmash_plugin_betterplot-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-20 01:11:15.145065 sourmash_plugin_betterplot-0.3.2/
--rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3.2/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     7364 2024-05-20 01:11:15.144832 sourmash_plugin_betterplot-0.3.2/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     6978 2024-05-20 01:04:58.000000 sourmash_plugin_betterplot-0.3.2/README.md
--rw-r--r--   0 t          (502) staff       (20)      797 2024-05-20 01:09:54.000000 sourmash_plugin_betterplot-0.3.2/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2024-05-20 01:11:15.145112 sourmash_plugin_betterplot-0.3.2/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-20 01:11:15.142813 sourmash_plugin_betterplot-0.3.2/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-20 01:11:15.144565 sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     7364 2024-05-20 01:11:15.000000 sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      422 2024-05-20 01:11:15.000000 sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2024-05-20 01:11:15.000000 sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)      396 2024-05-20 01:11:15.000000 sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       63 2024-05-20 01:11:15.000000 sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       27 2024-05-20 01:11:15.000000 sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)    26933 2024-05-20 01:04:58.000000 sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-20 01:11:15.144234 sourmash_plugin_betterplot-0.3.2/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3.2/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-06-01 13:32:42.082226 sourmash_plugin_betterplot-0.3.3/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3.3/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     7364 2024-06-01 13:32:42.082029 sourmash_plugin_betterplot-0.3.3/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     6978 2024-05-20 01:04:58.000000 sourmash_plugin_betterplot-0.3.3/README.md
+-rw-r--r--   0 t          (502) staff       (20)      797 2024-06-01 13:31:57.000000 sourmash_plugin_betterplot-0.3.3/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2024-06-01 13:32:42.082260 sourmash_plugin_betterplot-0.3.3/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-06-01 13:32:42.080265 sourmash_plugin_betterplot-0.3.3/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-06-01 13:32:42.081758 sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     7364 2024-06-01 13:32:42.000000 sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      422 2024-06-01 13:32:42.000000 sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2024-06-01 13:32:42.000000 sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      396 2024-06-01 13:32:42.000000 sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       63 2024-06-01 13:32:42.000000 sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       27 2024-06-01 13:32:42.000000 sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)    28621 2024-06-01 13:31:57.000000 sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-06-01 13:32:42.081453 sourmash_plugin_betterplot-0.3.3/tests/
+-rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3.3/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_betterplot-0.3.2/LICENSE` & `sourmash_plugin_betterplot-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_betterplot-0.3.2/PKG-INFO` & `sourmash_plugin_betterplot-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_betterplot
-Version: 0.3.2
+Version: 0.3.3
 Summary: sourmash plugin for improved plotting/viz and cluster examination.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sourmash<5,>=4.8.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
```

### Comparing `sourmash_plugin_betterplot-0.3.2/README.md` & `sourmash_plugin_betterplot-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_betterplot-0.3.2/pyproject.toml` & `sourmash_plugin_betterplot-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "sourmash_plugin_betterplot"
 description = "sourmash plugin for improved plotting/viz and cluster examination."
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.3.2"
+version = "0.3.3"
 
 dependencies = ["sourmash>=4.8.8,<5",
                 "matplotlib", "numpy", "scipy", "scikit-learn", "seaborn"]
 
 [metadata]
 license = { text = "BSD 3-Clause License" }
```

### Comparing `sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.egg-info/PKG-INFO` & `sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_betterplot
-Version: 0.3.2
+Version: 0.3.3
 Summary: sourmash plugin for improved plotting/viz and cluster examination.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sourmash<5,>=4.8.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
```

### Comparing `sourmash_plugin_betterplot-0.3.2/src/sourmash_plugin_betterplot.py` & `sourmash_plugin_betterplot-0.3.3/src/sourmash_plugin_betterplot.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,56 +21,67 @@
 from matplotlib.lines import Line2D
 import seaborn as sns
 
 from sourmash.logging import debug_literal, error, notify, print_results
 from sourmash.plugins import CommandLinePlugin
 
 
-###
-
+### utility functions
 
 def load_labelinfo_csv(filename):
+    "Load file output by 'sourmash compare --labels-to'"
     with sourmash_args.FileInputCSV(filename) as r:
         labelinfo = list(r)
 
     labelinfo.sort(key=lambda row: int(row["sort_order"]))
     return labelinfo
 
 
 def load_categories_csv(filename, labelinfo):
+    "Load categories file, integrate with labelinfo => colors"
     with sourmash_args.FileInputCSV(filename) as r:
         categories = list(r)
 
     category_map = {}
     colors = None
     if categories:
+        # first, figure out which column is matching between labelinfo
+        # and categories file.
         assert labelinfo
         keys = set(categories[0].keys())
         keys -= {"category"}
 
         key = None
         for k in keys:
             if k in labelinfo[0].keys():
                 notify(f"found category key: {k}")
                 key = k
                 break
 
+        # found one? awesome. load in all the categories & assign colors.
+
         if key:
-            category_values = list(set([row["category"] for row in categories]))
-            category_values.sort()
+            # get distinct categories
+            category_values = set([row["category"] for row in categories])
+            category_values = list(sorted(category_values))
 
+            # map to colormap colors
             cat_colors = list(map(plt.cm.tab10, range(len(category_values))))
+
+            # build map of category => color
             category_map = {}
             for v, color in zip(category_values, cat_colors):
                 category_map[v] = color
 
+            # build map of key => color
             category_map2 = {}
             for row in categories:
                 category_map2[row[key]] = category_map[row["category"]]
 
+            # build list of colors
             colors = []
             for row in labelinfo:
                 value = row[key]
                 color = category_map2[value]
                 colors.append(color)
 
         else:
@@ -78,55 +89,60 @@
     else:
         notify(f"nothing in categories file '{filename}'?!")
 
     return category_map, colors
 
 
 def load_categories_csv_for_labels(filename, queries):
-    "Load a categories CSV that must use label name."
+    "Load a categories CSV that uses the 'label' column."
     with sourmash_args.FileInputCSV(filename) as r:
         categories = list(r)
 
     category_map = {}
     colors = None
     if categories:
         key = "label"
 
+        # load distinct categories
         category_values = list(set([row["category"] for row in categories]))
         category_values.sort()
 
+        # map categories to color
         cat_colors = list(map(plt.cm.tab10, range(len(category_values))))
         category_map = {}
         for v, color in zip(category_values, cat_colors):
             category_map[v] = color
 
+        # map label to color
         category_map2 = {}
         for row in categories:
             label = row[key]
             cat = row["category"]
             category_map2[label] = category_map[cat]
 
+        # build list of colors
         colors = []
         for label, idx in queries:
             color = category_map2[label]
             colors.append(color)
     else:
         notify(f"nothing in categories file '{filename}'?!")
 
     return category_map, colors
 
 
 #
-# CLI plugin - supports 'sourmash scripts plot2'
+# CLI plugin code
 #
 
-
 class Command_Plot2(CommandLinePlugin):
     command = "plot2"  # 'scripts <command>'
-    description = "plot a distance matrix produced by 'sourmash compare'"  # output with -h
+    description = (
+        "plot a distance matrix produced by 'sourmash compare'"  # output with -h
+    )
     usage = "sourmash scripts plot <matrix> <labels_csv> -o <output.png>"  # output with no args/bad args as well as -h
     epilog = epilog  # output with -h
     formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
 
     def __init__(self, subparser):
         super().__init__(subparser)
         subparser.add_argument("distances", help='output from "sourmash compare"')
@@ -241,19 +257,20 @@
     Z1 = sch.dendrogram(
         Y,
         orientation="left",
         labels=labeltext,
         no_labels=not show_labels,
         get_leaves=True,
     )
-    # ax1.set_xticks([])
 
+    # draw cut point
     if cut_point is not None:
         ax1.axvline(x=cut_point, c="red", linestyle="dashed")
 
+    # draw matrix
     xstart = 0.45
     width = 0.45
     if not show_labels:
         xstart = 0.315
     scale_xstart = xstart + width + 0.01
 
     idx1 = Z1["leaves"]
@@ -412,63 +429,63 @@
 
     def __init__(self, subparser):
         super().__init__(subparser)
 
         subparser.add_argument(
             "pairwise_csv", help="output from 'sourmash scripts pairwise'"
         )
-        subparser.add_argument('-o', '--output-matrix', required=True)
-        subparser.add_argument('--labels-to')
+        subparser.add_argument("-o", "--output-matrix", required=True)
+        subparser.add_argument("--labels-to")
 
     def main(self, args):
         super().main(args)
 
         with sourmash_args.FileInputCSV(args.pairwise_csv) as r:
             rows = list(r)
 
         # pick out all the distinct queries/matches.
         print(f"loaded {len(rows)} rows from '{args.pairwise_csv}'")
-        queries = set( [ row['query_name'] for row in rows ] )
-        queries.update(set( [ row['match_name'] for row in rows ] ))
+        queries = set([row["query_name"] for row in rows])
+        queries.update(set([row["match_name"] for row in rows]))
         print(f"loaded {len(queries)} total elements")
 
         queries = list(sorted(queries))
 
         sample_d = {}
         for n, sample_name in enumerate(queries):
             sample_d[sample_name] = n
 
         assert n == len(queries) - 1
 
         mat = numpy.zeros((len(queries), len(queries)))
 
         for row in rows:
             # get unique indices for each query/match pair.
-            q = row['query_name']
+            q = row["query_name"]
             qi = sample_d[q]
-            m = row['match_name']
+            m = row["match_name"]
             mi = sample_d[m]
-            jaccard = float(row['jaccard'])
+            jaccard = float(row["jaccard"])
 
             mat[qi, mi] = jaccard
             mat[mi, qi] = jaccard
 
         numpy.fill_diagonal(mat, 1)
 
-        with open(args.output_matrix, 'wb') as fp:
+        with open(args.output_matrix, "wb") as fp:
             numpy.save(fp, mat)
 
-        with open(args.output_matrix + '.labels.txt', 'wt') as fp:
+        with open(args.output_matrix + ".labels.txt", "wt") as fp:
             for label, n in sample_d.items():
                 fp.write(label + "\n")
 
         if args.labels_to:
-            with open(args.labels_to, 'w', newline="") as fp:
+            with open(args.labels_to, "w", newline="") as fp:
                 w = csv.writer(fp)
-                w.writerow(['sort_order', 'label'])
+                w.writerow(["sort_order", "label"])
                 for label, n in sample_d.items():
                     w.writerow([n, label])
 
 
 class Command_MDS2(CommandLinePlugin):
     command = "mds2"  # 'scripts <command>'
     description = "plot a 2-D multidimensional scaling plot from branchwater plugin's 'pairwise' output"  # output with -h
@@ -491,54 +508,56 @@
         super().main(args)
 
         with sourmash_args.FileInputCSV(args.pairwise_csv) as r:
             rows = list(r)
 
         # pick out all the distinct queries/matches.
         print(f"loaded {len(rows)} rows from '{args.pairwise_csv}'")
-        queries = set( [ row['query_name'] for row in rows ] )
-        queries.update(set( [ row['match_name'] for row in rows ] ))
+        queries = set([row["query_name"] for row in rows])
+        queries.update(set([row["match_name"] for row in rows]))
         print(f"loaded {len(queries)} total elements")
 
         queries = list(sorted(queries))
 
         sample_d = {}
         for n, sample_name in enumerate(queries):
             sample_d[sample_name] = n
 
         assert n == len(queries) - 1
 
         mat = numpy.zeros((len(queries), len(queries)))
 
         for row in rows:
             # get unique indices for each query/match pair.
-            q = row['query_name']
+            q = row["query_name"]
             qi = sample_d[q]
-            m = row['match_name']
+            m = row["match_name"]
             mi = sample_d[m]
-            jaccard = float(row['jaccard'])
+            jaccard = float(row["jaccard"])
 
             mat[qi, mi] = jaccard
             mat[mi, qi] = jaccard
 
         numpy.fill_diagonal(mat, 1)
 
         # load categories?
         category_map = None
         colors = None
         if args.categories_csv:
-            category_map, colors = load_categories_csv_for_labels(args.categories_csv, sample_d.items())
+            category_map, colors = load_categories_csv_for_labels(
+                args.categories_csv, sample_d.items()
+            )
 
         dissim = 1 - mat
         plot_mds(dissim, colors=colors, category_map=category_map)
 
         plt.savefig(args.output_figure)
 
 
-#@CTB unused again...
+# @CTB unused code for sparse matrix foo. Revisit!
 def create_sparse_dissimilarity_matrix(tuples, num_objects):
     # Initialize matrix in LIL format for efficient setup
     similarity_matrix = lil_matrix((num_objects, num_objects))
 
     for obj1, obj2, similarity in tuples:
         similarity_matrix[obj1, obj2] = 1 - similarity
         if obj1 != obj2:
@@ -565,15 +584,17 @@
         for k, v in category_map.items():
             legend_elements.append(Line2D([0], [0], color=v, label=k, marker="o", lw=0))
         plt.legend(handles=legend_elements)
 
 
 class Command_Plot3(CommandLinePlugin):
     command = "plot3"  # 'scripts <command>'
-    description = "plot a distance matrix produced by 'sourmash compare'"  # output with -h
+    description = (
+        "plot a distance matrix produced by 'sourmash compare'"  # output with -h
+    )
     usage = "sourmash scripts plot <matrix> <labels_csv> -o <output.png>"  # output with no args/bad args as well as -h
     epilog = epilog  # output with -h
     formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
 
     def __init__(self, subparser):
         super().__init__(subparser)
         subparser.add_argument("distances", help='output from "sourmash compare"')
@@ -609,14 +630,18 @@
         )
         subparser.add_argument(
             "-o", "--output-figure", help="output figure to this file", required=True
         )
         subparser.add_argument(
             "-C", "--categories-csv", help="CSV mapping label columns to categories"
         )
+        subparser.add_argument(
+            "--no-labels", action="store_true",
+            help="disable X & Y axis labels"
+        )
 
     def main(self, args):
         super().main(args)
         D_filename = args.distances
 
         notify(f"loading comparison matrix from {D_filename}...")
         with open(D_filename, "rb") as f:
@@ -645,35 +670,42 @@
             sample_idx = sample_idx[: args.subsample]
 
             np_idx = numpy.array(sample_idx)
             D = D[numpy.ix_(np_idx, np_idx)]
             labelinfo = [labelinfo[idx] for idx in sample_idx]
 
         # turn into dissimilarity matrix
-        #dissim = 1 - D
-        #numpy.fill_diagonal(dissim, 1)
+        # dissim = 1 - D
+        # numpy.fill_diagonal(dissim, 1)
         dissim = D
 
-        #plot!
+        if args.no_labels:
+            yticklabels=[]
+        else:
+            yticklabels=[x["label"].split(" ")[0] for x in labelinfo],
+
+        # plot!
         fig = sns.clustermap(
             dissim,
             figsize=(args.figsize_x, args.figsize_y),
             vmin=args.vmin,
             vmax=args.vmax,
             col_colors=colors,
-            yticklabels=[ x["label"].split(' ')[0] for x in labelinfo ],
+            yticklabels=yticklabels,
             xticklabels=[],
             cmap="flare",
         )
 
         if colors and category_map:
             # create a custom legend of just the categories
             legend_elements = []
             for k, v in category_map.items():
-                legend_elements.append(Line2D([0], [0], color=v, label=k, marker="o", lw=0))
+                legend_elements.append(
+                    Line2D([0], [0], color=v, label=k, marker="o", lw=0)
+                )
             fig.ax_col_dendrogram.legend(handles=legend_elements)
 
         # turn off column dendrogram
         fig.ax_row_dendrogram.set_visible(False)
 
         fig.savefig(args.output_figure, bbox_inches="tight")
         notify(f"wrote plot to: {args.output_figure}")
@@ -704,33 +736,46 @@
         )
         subparser.add_argument("--figsize-x", type=int, default=11)
         subparser.add_argument("--figsize-y", type=int, default=8)
         subparser.add_argument(
             "-o", "--output-figure", help="output figure to this file", required=True
         )
         subparser.add_argument(
-            "-R", "--row-categories-csv", help="CSV mapping labels @CTB query or against? to categories"
+            "-R",
+            "--row-categories-csv",
+            help="CSV mapping labels @CTB query or against? to categories",
         )
         subparser.add_argument(
-            "-C", "--col-categories-csv", help="CSV mapping labels @CTB query or against? to categories"
+            "-C",
+            "--col-categories-csv",
+            help="CSV mapping labels @CTB query or against? to categories",
+        )
+        subparser.add_argument(
+            "-u",
+            "--use-column",
+            default="jaccard",
+            help="column name to use in matrix (default: jaccard)",
+        )
+        subparser.add_argument(
+            "--boolean", action="store_true", help="convert values into 0/1"
+        )
+        subparser.add_argument(
+            "--no-labels", action="store_true",
+            help="disable X & Y axis labels"
         )
-        subparser.add_argument('-u', '--use-column', default='jaccard',
-                               help='column name to use in matrix (default: jaccard)')
-        subparser.add_argument('--boolean', action='store_true',
-                               help='convert values into 0/1')
 
     def main(self, args):
         super().main(args)
         with sourmash_args.FileInputCSV(args.manysearch_csv) as r:
             rows = list(r)
 
         # pick out all the distinct queries/matches.
         print(f"loaded {len(rows)} rows from '{args.manysearch_csv}'")
-        queries = set( [ row['query_name'] for row in rows ] )
-        against = set( [ row['match_name'] for row in rows ] )
+        queries = set([row["query_name"] for row in rows])
+        against = set([row["match_name"] for row in rows])
         print(f"loaded {len(queries)} x {len(against)} total elements")
 
         queries = list(sorted(queries))
         against = list(sorted(against))
 
         query_d = {}
         for n, query_name in enumerate(queries):
@@ -745,61 +790,81 @@
 
         mat = numpy.zeros((len(queries), len(against)))
 
         colname = args.use_column
         print(f"using column '{colname}'")
         make_bool = args.boolean
         if make_bool:
-            print(f"forcing values to 0 / 1")
+            print(f"forcing values to 0 / 1 and disabling color barbecause of --boolean")
 
         for row in rows:
-            q = row['query_name']
+            q = row["query_name"]
             qi = query_d[q]
-            m = row['match_name']
+            m = row["match_name"]
             mi = against_d[m]
             value = float(row[colname])
             if make_bool:
                 value = 1 if value else 0
 
             mat[qi, mi] = value
 
         # load categories?
         row_category_map = None
         row_colors = None
         if args.row_categories_csv:
-            row_category_map, row_colors = load_categories_csv_for_labels(args.row_categories_csv, query_d.items())
+            row_category_map, row_colors = load_categories_csv_for_labels(
+                args.row_categories_csv, query_d.items()
+            )
 
         col_category_map = None
         col_colors = None
         if args.col_categories_csv:
-            col_category_map, col_colors = load_categories_csv_for_labels(args.col_categories_csv, against_d.items())
+            col_category_map, col_colors = load_categories_csv_for_labels(
+                args.col_categories_csv, against_d.items()
+            )
+
+        kw_args = {}
+        if args.boolean:        # turn off colorbar if boolean.
+            kw_args['cbar_pos'] = None
+
+        if args.no_labels:
+            xticklabels=[]
+            yticklabels=[]
+        else:
+            yticklabels=[q.split()[0] for q, _ in query_d_items],
+            xticklabels=[a.split()[0] for a, _ in against_d_items],
 
         # turn into dissimilarity matrix
         # plot!
         fig = sns.clustermap(
             mat,
             figsize=(args.figsize_x, args.figsize_y),
             vmin=args.vmin,
             vmax=args.vmax,
             col_colors=col_colors,
             row_colors=row_colors,
-            yticklabels=[ q.split()[0] for q, _ in query_d_items ],
-            xticklabels=[ a.split()[0] for a, _ in against_d_items ],
+            yticklabels=xticklabels,
+            xticklabels=yticklabels,
             cmap="flare",
+            **kw_args
         )
 
         if col_colors and col_category_map:
             # create a custom legend of just the categories
             legend_elements = []
             for k, v in col_category_map.items():
-                legend_elements.append(Line2D([0], [0], color=v, label=k, marker="o", lw=0))
+                legend_elements.append(
+                    Line2D([0], [0], color=v, label=k, marker="o", lw=0)
+                )
             fig.ax_col_dendrogram.legend(handles=legend_elements)
 
         if row_colors and row_category_map:
             # create a custom legend of just the categories
             legend_elements = []
             for k, v in row_category_map.items():
-                legend_elements.append(Line2D([0], [0], color=v, label=k, marker="o", lw=0))
+                legend_elements.append(
+                    Line2D([0], [0], color=v, label=k, marker="o", lw=0)
+                )
             fig.ax_row_dendrogram.legend(handles=legend_elements)
 
         fig.savefig(args.output_figure, bbox_inches="tight")
         notify(f"wrote plot to: {args.output_figure}")
```

