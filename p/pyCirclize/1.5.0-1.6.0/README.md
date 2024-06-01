# Comparing `tmp/pycirclize-1.5.0.tar.gz` & `tmp/pycirclize-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycirclize-1.5.0.tar", max compression
+gzip compressed data, was "pycirclize-1.6.0.tar", max compression
```

## Comparing `pycirclize-1.5.0.tar` & `pycirclize-1.6.0.tar`

### file list

```diff
@@ -1,48 +1,26 @@
--rw-r--r--   0        0        0     1062 2024-05-18 05:08:28.097730 pycirclize-1.5.0/LICENSE
--rw-r--r--   0        0        0     9304 2024-05-18 05:08:28.101730 pycirclize-1.5.0/README.md
--rw-r--r--   0        0        0     2088 2024-05-18 05:08:28.245730 pycirclize-1.5.0/pyproject.toml
--rw-r--r--   0        0        0       89 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/__init__.py
--rw-r--r--   0        0        0    46248 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/circos.py
--rw-r--r--   0        0        0     3078 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/config.py
--rw-r--r--   0        0        0      337 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/__init__.py
--rw-r--r--   0        0        0     1684 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/bed.py
--rw-r--r--   0        0        0    16026 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/genbank.py
--rw-r--r--   0        0        0    17540 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/gff.py
--rw-r--r--   0        0        0     8157 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/matrix.py
--rw-r--r--   0        0        0     6182 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/parser/table.py
--rw-r--r--   0        0        0    16391 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/patches.py
--rw-r--r--   0        0        0    17309 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/sector.py
--rw-r--r--   0        0        0    52377 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/track.py
--rw-r--r--   0        0        0    25330 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/tree.py
--rw-r--r--   0        0        0      533 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/__init__.py
--rw-r--r--   0        0        0     7829 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/dataset.py
--rw-r--r--   0        0        0     9955 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/images/python_logo.png
--rw-r--r--   0        0        0      565 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/alphabet.nwk
--rw-r--r--   0        0        0     7112 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/large_example.nwk
--rw-r--r--   0        0        0      778 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/medium_example.nwk
--rw-r--r--   0        0        0      227 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/small_example.nwk
--rw-r--r--   0        0        0     3870 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/helper.py
--rw-r--r--   0        0        0     2314 2024-05-18 05:08:28.245730 pycirclize-1.5.0/src/pycirclize/utils/plot.py
--rw-r--r--   0        0        0        0 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0     2601 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/parser/__init__.py
--rw-r--r--   0        0        0     2639 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/parser/test_genbank.py
--rw-r--r--   0        0        0     1827 2024-05-18 05:08:28.245730 pycirclize-1.5.0/tests/parser/test_gff.py
--rw-r--r--   0        0        0     4351 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/parser/test_matrix.py
--rw-r--r--   0        0        0     3700 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/parser/test_table.py
--rw-r--r--   0        0        0     2962 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/test_circos.py
--rw-r--r--   0        0        0    25203 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/test_plot.py
--rw-r--r--   0        0        0     2885 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/test_sector.py
--rw-r--r--   0        0        0      988 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/test_track.py
--rw-r--r--   0        0        0      755 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
--rw-r--r--   0        0        0    30808 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
--rw-r--r--   0        0        0   283582 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
--rw-r--r--   0        0        0   148834 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
--rw-r--r--   0        0        0    36204 2024-05-18 05:08:28.249730 pycirclize-1.5.0/tests/testdata/prokaryote/enterobacteria_phage.gff
--rw-r--r--   0        0        0   580710 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
--rw-r--r--   0        0        0    58530 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
--rw-r--r--   0        0        0    57946 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/testdata/prokaryote/mycoplasma_alvi_nocomment.gff.gz
--rw-r--r--   0        0        0        0 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1851 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/utils/test_dataset.py
--rw-r--r--   0        0        0     1839 2024-05-18 05:08:28.253730 pycirclize-1.5.0/tests/utils/test_helper.py
--rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 pycirclize-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-06-01 05:16:13.994844 pycirclize-1.6.0/LICENSE
+-rw-r--r--   0        0        0     9304 2024-06-01 05:16:13.994844 pycirclize-1.6.0/README.md
+-rw-r--r--   0        0        0     2068 2024-06-01 05:16:14.138844 pycirclize-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/__init__.py
+-rw-r--r--   0        0        0    47205 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/circos.py
+-rw-r--r--   0        0        0     3078 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/config.py
+-rw-r--r--   0        0        0      337 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/parser/__init__.py
+-rw-r--r--   0        0        0     1684 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/parser/bed.py
+-rw-r--r--   0        0        0    16052 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/parser/genbank.py
+-rw-r--r--   0        0        0    17730 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/parser/gff.py
+-rw-r--r--   0        0        0     8169 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/parser/matrix.py
+-rw-r--r--   0        0        0     6182 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/parser/table.py
+-rw-r--r--   0        0        0    16391 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/patches.py
+-rw-r--r--   0        0        0    17309 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/sector.py
+-rw-r--r--   0        0        0    52389 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/track.py
+-rw-r--r--   0        0        0    25334 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/tree.py
+-rw-r--r--   0        0        0      577 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/__init__.py
+-rw-r--r--   0        0        0     7844 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/dataset.py
+-rw-r--r--   0        0        0     9955 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/example_data/images/python_logo.png
+-rw-r--r--   0        0        0      565 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/example_data/trees/alphabet.nwk
+-rw-r--r--   0        0        0     7112 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/example_data/trees/large_example.nwk
+-rw-r--r--   0        0        0      778 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/example_data/trees/medium_example.nwk
+-rw-r--r--   0        0        0      227 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/example_data/trees/small_example.nwk
+-rw-r--r--   0        0        0     4295 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/helper.py
+-rw-r--r--   0        0        0     2314 2024-06-01 05:16:14.138844 pycirclize-1.6.0/src/pycirclize/utils/plot.py
+-rw-r--r--   0        0        0    10315 1970-01-01 00:00:00.000000 pycirclize-1.6.0/PKG-INFO
```

### Comparing `pycirclize-1.5.0/LICENSE` & `pycirclize-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/README.md` & `pycirclize-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/pyproject.toml` & `pycirclize-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyCirclize"
-version = "1.5.0"
+version = "1.6.0"
 description = "Circular visualization in Python"
 authors = ["moshi4"]
 license = "MIT"
 homepage = "https://moshi4.github.io/pyCirclize/"
 repository = "https://github.com/moshi4/pyCirclize/"
 readme = "README.md"
 keywords = [
@@ -15,15 +15,14 @@
     "chord-diagram",
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Framework :: Matplotlib",
 ]
-include = ["tests"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov=src --tb=long -vv --cov-report=xml --cov-report=term"
 testpaths = ["tests"]
 
 [tool.ruff]
```

### Comparing `pycirclize-1.5.0/src/pycirclize/circos.py` & `pycirclize-1.6.0/src/pycirclize/circos.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,20 @@
 from pycirclize.track import Track
 from pycirclize.tree import TreeViz
 
 
 class Circos:
     """Circos Visualization Class"""
 
+    # By default, after saving a figure using the `savefig()` method, figure object is
+    # automatically deleted to avoid memory leaks (no display on jupyter notebook)
+    # If you want to display the figure on jupyter notebook using `savefig()` method,
+    # set clear_savefig=False.
+    clear_savefig: bool = True
+
     def __init__(
         self,
         sectors: Mapping[str, int | float | tuple[float, float]],
         start: float = 0,
         end: float = 360,
         *,
         space: float | list[float] = 0,
@@ -518,16 +524,18 @@
         label_formatter : Callable[[str], str] | None, optional
             User-defined label text format function to change plot label text content.
             For example, if you want to change underscore of the label to space,
             set `lambda t: t.replace("_", " ")`.
 
         Returns
         -------
-        circos, tv : tuple[Circos, TreeViz]
-            Circos & TreeViz instances initialized from tree
+        circos : Circos
+            Circos instance
+        tv : TreeViz
+            TreeViz instance
         """
         # Initialize circos sector with tree size
         tree = TreeViz.load_tree(tree_data, format=format)
         leaf_num = tree.count_terminals()
         circos = Circos(dict(tree=leaf_num), start=start, end=end)
         sector = circos.sectors[0]
 
@@ -942,15 +950,17 @@
         self,
         bounds: tuple[float, float, float, float] = (1.02, 0.3, 0.02, 0.4),
         *,
         vmin: float = 0,
         vmax: float = 1,
         cmap: str | Colormap = "bwr",
         orientation: str = "vertical",
+        label: str | None = None,
         colorbar_kws: dict[str, Any] | None = None,
+        label_kws: dict[str, Any] | None = None,
         tick_kws: dict[str, Any] | None = None,
     ) -> None:
         """Plot colorbar
 
         Parameters
         ----------
         bounds : tuple[float, float, float, float], optional
@@ -960,35 +970,43 @@
         vmax : float, optional
             Colorbar max value
         cmap : str | Colormap, optional
             Colormap (e.g. `viridis`, `Spectral`, `Reds`, `Greys`)
             <https://matplotlib.org/stable/tutorials/colors/colormaps.html>
         orientation : str, optional
             Colorbar orientation (`vertical`|`horizontal`)
+        label : str | None, optional
+            Colorbar label. If None, no label shown.
         colorbar_kws : dict[str, Any] | None, optional
-            Colorbar properties (e.g. `dict(label="name", format="%.1f", ...)`)
+            Colorbar properties (e.g. `dict(format="%.1f", ...)`)
             <https://matplotlib.org/stable/api/colorbar_api.html>
+        label_kws : dict[str, Any] | None, optional
+            Text properties (e.g. `dict(size=15, color="red", ...)`)
+            <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         tick_kws : dict[str, Any] | None, optional
             Axes.tick_params properties (e.g. `dict(labelsize=12, colors="red", ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.tick_params.html>
         """
         colorbar_kws = {} if colorbar_kws is None else deepcopy(colorbar_kws)
+        label_kws = {} if label_kws is None else deepcopy(label_kws)
         tick_kws = {} if tick_kws is None else deepcopy(tick_kws)
 
         def plot_colorbar(ax: PolarAxes) -> None:
             axin: Axes = ax.inset_axes(bounds)
             norm = Normalize(vmin=vmin, vmax=vmax)
-            Colorbar(
+            cb = Colorbar(
                 axin,
                 cmap=cmap,  # type: ignore
                 norm=norm,
                 orientation=orientation,  # type: ignore
                 **colorbar_kws,
             )
             axin.tick_params(**tick_kws)
+            if label:
+                cb.set_label(label, **label_kws)
 
         self._plot_funcs.append(plot_colorbar)
 
     def plotfig(
         self,
         dpi: int = 100,
         *,
@@ -1051,38 +1069,41 @@
         *,
         dpi: int = 100,
         figsize: tuple[float, float] = (8, 8),
         pad_inches: float = 0.5,
     ) -> None:
         """Save figure to file
 
-        `circos.savefig("result.png")` is alias for
-        `circos.plotfig().savefig("result.png")`
-
         Parameters
         ----------
         savefile : str | Path
             Save file (`*.png`|`*.jpg`|`*.svg`|`*.pdf`)
         dpi : int, optional
             DPI
         figsize : tuple[float, float], optional
             Figure size
         pad_inches : float, optional
             Padding inches
+
+        Warnings
+        --------
+        To plot a figure that settings a user-defined legend, subtracks, or annotations,
+        call `fig.savefig()` instead of `gv.savefig()`.
         """
         fig = self.plotfig(dpi=dpi, figsize=figsize)
         fig.savefig(
             fname=savefile,  # type: ignore
             dpi=dpi,
             pad_inches=pad_inches,
             bbox_inches="tight",
         )
         # Clear & close figure to suppress memory leak
-        fig.clear()
-        plt.close(fig)
+        if self.clear_savefig:
+            fig.clear()
+            plt.close(fig)
 
     ############################################################
     # Private Method
     ############################################################
 
     def _check_degree_range(self, start: float, end: float) -> None:
         """Check start-end degree range (`-360 <= start < end <= 360`)
@@ -1132,16 +1153,18 @@
         figsize : tuple[float, float], optional
             Figure size
         dpi : int, optional
             Figure DPI
 
         Returns
         -------
-        fig, ax : tuple[Figure, PolarAxes]
-            Figure, PolarAxes
+        fig : Figure
+            Figure
+        ax : PolarAxes
+            PolarAxes
         """
         fig = plt.figure(figsize=figsize, dpi=dpi, tight_layout=True)
         ax = fig.add_subplot(projection="polar")
         return fig, ax
 
     def _initialize_polar_axes(self, ax: PolarAxes) -> None:
         """Initialize polar axes params
```

### Comparing `pycirclize-1.5.0/src/pycirclize/config.py` & `pycirclize-1.6.0/src/pycirclize/config.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/parser/bed.py` & `pycirclize-1.6.0/src/pycirclize/parser/bed.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/parser/genbank.py` & `pycirclize-1.6.0/src/pycirclize/parser/genbank.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,18 @@
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
         seq : str | None, optional
             Sequence for GCskew calculation (Default: `self.genome_seq`)
 
         Returns
         -------
-        gc_skew_result_tuple : tuple[NDArray[np.int64], NDArray[np.float64]]
-            Position list & GC skew list
+        pos_list : NDArray[np.int64]
+            Position list
+        gc_skew_list : NDArray[np.float64]
+            GC skew list
         """
         pos_list, gc_skew_list = [], []
         seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
             step_size = int(len(seq) / 1000)
@@ -196,16 +198,18 @@
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
         seq : str | None, optional
             Sequence for GC content calculation (Default: `self.genome_seq`)
 
         Returns
         -------
-        gc_content_result_tuple : tuple[NDArray[np.int64], NDArray[np.float64]]
-            Position list & GC content list
+        pos_list : NDArray[np.int64]
+            Position list
+        gc_content_list : NDArray[np.float64]
+            GC content list
         """
         pos_list, gc_content_list = [], []
         seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
             step_size = int(len(seq) / 1000)
```

### Comparing `pycirclize-1.5.0/src/pycirclize/parser/gff.py` & `pycirclize-1.6.0/src/pycirclize/parser/gff.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,20 @@
         gff_file : str | Path
             GFF file
         target_seqid : str | None
             Target seqid to be extracted
 
         Returns
         -------
-        gff_records, start, end : tuple[list[GffRecord], int, int]
-            GFF record list, start, end
+        gff_records : list[GffRecord]
+            GFF record list
+        start : int
+            Start position of target_seqid record
+        end : int
+            End position of target_seqid record
         """
         gff_file = Path(gff_file)
         if gff_file.suffix == ".gz":
             with gzip.open(gff_file, mode="rt") as f:
                 gff_records, start, end = self._parse_gff_textio(f, target_seqid)
         elif gff_file.suffix == ".bz2":
             with bz2.open(gff_file, mode="rt") as f:
@@ -304,16 +308,20 @@
         handle : TextIO
             GFF TextIO handle
         target_seqid : str | None, optional
             GFF target seqid
 
         Returns
         -------
-        gff_records, start, end : tuple[list[GffRecord], int, int]
-            GFF record list, start, end
+        gff_records : list[GffRecord]
+            GFF record list
+        start : int
+            Start position of target_seqid record
+        end : int
+            End position of target_seqid record
         """
         # Parse GFF lines
         gff_all_lines = handle.read().splitlines()
         gff_record_lines = filter(GffRecord.is_gff_line, gff_all_lines)
         gff_records = list(map(GffRecord.parse_gff_line, gff_record_lines))
         if len(gff_records) == 0:
             err_msg = f"Failed to parse '{self._gff_file}' as GFF file "
```

### Comparing `pycirclize-1.5.0/src/pycirclize/parser/matrix.py` & `pycirclize-1.6.0/src/pycirclize/parser/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,24 +198,27 @@
         return sectors
 
     def to_links(
         self,
     ) -> list[tuple[tuple[str, float, float], tuple[str, float, float]]]:
         """Convert matrix to links data for `circos.link()` method
 
-        >>> # Example usage
+        Returns
+        -------
+        link_target1 : tuple[str, float, float]
+            name1, start1, end1
+        link_target2 : tuple[str, float, float]
+            name2, start2, end2
+
+        Examples
+        --------
         >>> matrix = Matrix(matrix_file)
         >>> circos = Circos(matrix.to_sectors())
         >>> for link in matrix.to_links():
         >>>    circos.link(*link)
-
-        Returns
-        -------
-        links : list[tuple[tuple[str, float, float], tuple[str, float, float]]]
-            List of link `((name1, start1, end1), (name2, end2, start2))`
         """
         return self._links
 
     def to_fromto_table(self) -> pd.DataFrame:
         """Convert matrix to from-to table dataframe
 
         Returns
```

### Comparing `pycirclize-1.5.0/src/pycirclize/parser/table.py` & `pycirclize-1.6.0/src/pycirclize/parser/table.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/patches.py` & `pycirclize-1.6.0/src/pycirclize/patches.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/sector.py` & `pycirclize-1.6.0/src/pycirclize/sector.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/track.py` & `pycirclize-1.6.0/src/pycirclize/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -1314,16 +1314,18 @@
         rad : list[float] | np.ndarray
             Radian list
         r : list[float] | np.ndarray
             Radius list
 
         Returns
         -------
-        arc_rad, arc_r : tuple[list[float], list[float]]
-            Arc radian list, Ard radius list
+        arc_rad : list[float]
+            Arc radian list
+        arc_r : list[float]
+            Arc radius list
         """
         all_arc_rad, all_arc_r = [], []
         for i in range(len(rad) - 1):
             rad1, rad2, r1, r2 = rad[i], rad[i + 1], r[i], r[i + 1]
             if rad1 == rad2:
                 all_arc_rad.extend([rad1, rad2])
                 all_arc_r.extend([r1, r2])
```

### Comparing `pycirclize-1.5.0/src/pycirclize/tree.py` & `pycirclize-1.6.0/src/pycirclize/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,16 +438,18 @@
         Parameters
         ----------
         tree : Tree
             Tree object
 
         Returns
         -------
-        tree, uniq_node_names: tuple[Tree, list[str]]
-            Unique node name set tree object & set unique node names
+        tree : Tree
+            Tree (set unique node names)
+        uniq_node_names : list[str]
+            Unique node names
         """
         tree = deepcopy(tree)
         uniq_innode_names: list[str] = []
         for idx, node in enumerate(tree.get_nonterminals(), 1):
             uniq_innode_name = f"N_{idx}"
             if node.name is None:
                 node.name = uniq_innode_name
```

### Comparing `pycirclize-1.5.0/src/pycirclize/utils/__init__.py` & `pycirclize-1.6.0/src/pycirclize/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from pycirclize.utils.dataset import (
     fetch_genbank_by_accid,
     load_eukaryote_example_dataset,
     load_example_image_file,
     load_example_tree_file,
     load_prokaryote_example_file,
 )
-from pycirclize.utils.helper import ColorCycler, calc_group_spaces
+from pycirclize.utils.helper import ColorCycler, calc_group_spaces, is_pseudo_feature
 
 __all__ = [
     "plot",
     "fetch_genbank_by_accid",
     "load_eukaryote_example_dataset",
     "load_prokaryote_example_file",
     "load_example_image_file",
     "load_example_tree_file",
     "ColorCycler",
     "calc_group_spaces",
+    "is_pseudo_feature",
 ]
```

### Comparing `pycirclize-1.5.0/src/pycirclize/utils/dataset.py` & `pycirclize-1.6.0/src/pycirclize/utils/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,16 +92,20 @@
         Output cache directory (Default: `~/.cache/pycirclize/`)
     overwrite_cache : bool
         If True, overwrite cache dataset.
         Assumed to be used when cache dataset is corrupt.
 
     Returns
     -------
-    chr_bed_file, cytoband_file, chr_links : tuple[Path, Path, list[ChrLink]]
-        BED file, Cytoband file, Chromosome links
+    chr_bed_file : Path
+        BED file
+    cytoband_file : Path
+        Cytoband file
+    chr_links : list[ChrLink]
+        Chromosome links
     """
     # Check specified name dataset exists or not
     if name not in config.EUKARYOTE_DATASET:
         available_dataset = list(config.EUKARYOTE_DATASET.keys())
         raise ValueError(f"{name=} dataset not found.\n{available_dataset=}")
 
     # Dataset cache local directory
```

### Comparing `pycirclize-1.5.0/src/pycirclize/utils/example_data/images/python_logo.png` & `pycirclize-1.6.0/src/pycirclize/utils/example_data/images/python_logo.png`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/alphabet.nwk` & `pycirclize-1.6.0/src/pycirclize/utils/example_data/trees/alphabet.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/large_example.nwk` & `pycirclize-1.6.0/src/pycirclize/utils/example_data/trees/large_example.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/utils/example_data/trees/medium_example.nwk` & `pycirclize-1.6.0/src/pycirclize/utils/example_data/trees/medium_example.nwk`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/src/pycirclize/utils/helper.py` & `pycirclize-1.6.0/src/pycirclize/utils/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import matplotlib as mpl
 import numpy as np
+from Bio.SeqFeature import SeqFeature
 from matplotlib.colors import Colormap, to_hex
 
 
 class ColorCycler:
     """Color Cycler Class"""
 
     counter = 0
@@ -125,7 +126,24 @@
             group_spaces = [space_in_group] * (group_num - 1)
             group_spaces.extend([space_bw_group])
             spaces.extend(group_spaces)
     if endspace:
         return spaces
     else:
         return spaces[:-1]
+
+
+def is_pseudo_feature(feature: SeqFeature) -> bool:
+    """Check target feature is pseudo or not from qualifiers tag
+
+    Parameters
+    ----------
+    feature : SeqFeature
+        Target feature
+
+    Returns
+    -------
+    check_result : bool
+        pseudo check result
+    """
+    quals = feature.qualifiers
+    return True if "pseudo" in quals or "pseudogene" in quals else False
```

### Comparing `pycirclize-1.5.0/src/pycirclize/utils/plot.py` & `pycirclize-1.6.0/src/pycirclize/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycirclize-1.5.0/PKG-INFO` & `pycirclize-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCirclize
-Version: 1.5.0
+Version: 1.6.0
 Summary: Circular visualization in Python
 Home-page: https://moshi4.github.io/pyCirclize/
 License: MIT
 Keywords: matplotlib,visualization,bioinformatics,circos,chord-diagram
 Author: moshi4
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Matplotlib
```

