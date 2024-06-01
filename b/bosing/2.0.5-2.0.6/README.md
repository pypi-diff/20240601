# Comparing `tmp/bosing-2.0.5.tar.gz` & `tmp/bosing-2.0.6.tar.gz`

## Comparing `bosing-2.0.5.tar` & `bosing-2.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 bosing-2.0.5/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-05-23 09:57:54.000000 bosing-2.0.5/.github/dependabot.yml
--rw-r--r--   0     1001      127      690 2024-05-23 09:57:54.000000 bosing-2.0.5/.github/workflows/auto-dep.yml
--rw-r--r--   0     1001      127     6323 2024-05-23 09:57:54.000000 bosing-2.0.5/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-05-23 09:57:54.000000 bosing-2.0.5/.gitignore
--rw-r--r--   0     1001      127      972 2024-05-23 09:57:54.000000 bosing-2.0.5/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-05-23 09:57:54.000000 bosing-2.0.5/LICENSE.txt
--rw-r--r--   0     1001      127     1360 2024-05-23 09:57:54.000000 bosing-2.0.5/README.md
--rw-r--r--   0     1001      127    10767 2024-05-23 09:57:54.000000 bosing-2.0.5/bosing.pyi
--rw-r--r--   0     1001      127       78 2024-05-23 09:57:54.000000 bosing-2.0.5/clippy.toml
--rw-r--r--   0     1001      127      634 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/conf.py
--rw-r--r--   0     1001      127     1258 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/index.rst
--rw-r--r--   0     1001      127     1716 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/quickstart.rst
--rw-r--r--   0     1001      127       22 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-05-23 09:57:54.000000 bosing-2.0.5/docs/schedule.rst
--rw-r--r--   0     1001      127     1171 2024-05-23 09:57:54.000000 bosing-2.0.5/example/flexible.py
--rw-r--r--   0     1001      127      533 2024-05-23 09:57:54.000000 bosing-2.0.5/example/hann.py
--rw-r--r--   0     1001      127      788 2024-05-23 09:57:54.000000 bosing-2.0.5/example/interp.py
--rw-r--r--   0     1001      127      696 2024-05-23 09:57:54.000000 bosing-2.0.5/example/overlap.py
--rw-r--r--   0     1001      127     2074 2024-05-23 09:57:54.000000 bosing-2.0.5/example/schedule.py
--rw-r--r--   0     1001      127     2362 2024-05-23 09:57:54.000000 bosing-2.0.5/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-05-23 09:57:54.000000 bosing-2.0.5/ruff_defaults.toml
--rw-r--r--   0     1001      127    11370 2024-05-23 09:57:54.000000 bosing-2.0.5/src/executor.rs
--rw-r--r--   0     1001      127    62682 2024-05-23 09:57:54.000000 bosing-2.0.5/src/lib.rs
--rw-r--r--   0     1001      127    17863 2024-05-23 09:57:54.000000 bosing-2.0.5/src/pulse.rs
--rw-r--r--   0     1001      127     7540 2024-05-23 09:57:54.000000 bosing-2.0.5/src/quant.rs
--rw-r--r--   0     1001      127     2367 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     9689 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule/grid/helper.rs
--rw-r--r--   0     1001      127     6941 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3145 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule/play.rs
--rw-r--r--   0     1001      127     2010 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     3577 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule/simple.rs
--rw-r--r--   0     1001      127     3132 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule/stack/helper.rs
--rw-r--r--   0     1001      127     7464 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule/stack.rs
--rw-r--r--   0     1001      127     7859 2024-05-23 09:57:54.000000 bosing-2.0.5/src/schedule.rs
--rw-r--r--   0     1001      127     7677 2024-05-23 09:57:54.000000 bosing-2.0.5/src/shape.rs
--rw-r--r--   0     1001      127       14 2024-05-23 09:57:54.000000 bosing-2.0.5/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-05-23 09:57:54.000000 bosing-2.0.5/tests/__init__.py
--rw-r--r--   0     1001      127     1291 2024-05-23 09:57:54.000000 bosing-2.0.5/tests/test_basic.py
--rw-r--r--   0     1001      127    22677 2024-05-23 09:58:06.000000 bosing-2.0.5/Cargo.lock
--rw-r--r--   0     1001      127     1863 2024-05-23 09:57:54.000000 bosing-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 bosing-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bosing-2.0.6/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-06-01 12:01:49.000000 bosing-2.0.6/.github/dependabot.yml
+-rw-r--r--   0     1001      127      690 2024-06-01 12:01:49.000000 bosing-2.0.6/.github/workflows/auto-dep.yml
+-rw-r--r--   0     1001      127     6538 2024-06-01 12:01:49.000000 bosing-2.0.6/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-06-01 12:01:49.000000 bosing-2.0.6/.gitignore
+-rw-r--r--   0     1001      127      971 2024-06-01 12:01:49.000000 bosing-2.0.6/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-06-01 12:01:49.000000 bosing-2.0.6/LICENSE.txt
+-rw-r--r--   0     1001      127     1360 2024-06-01 12:01:49.000000 bosing-2.0.6/README.md
+-rw-r--r--   0     1001      127    10767 2024-06-01 12:01:49.000000 bosing-2.0.6/bosing.pyi
+-rw-r--r--   0     1001      127       78 2024-06-01 12:01:49.000000 bosing-2.0.6/clippy.toml
+-rw-r--r--   0     1001      127      634 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/api.rst
+-rw-r--r--   0     1001      127     1478 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/quickstart.rst
+-rw-r--r--   0     1001      127     5534 2024-06-01 12:01:49.000000 bosing-2.0.6/docs/schedule.rst
+-rw-r--r--   0     1001      127     1171 2024-06-01 12:01:49.000000 bosing-2.0.6/example/flexible.py
+-rw-r--r--   0     1001      127      533 2024-06-01 12:01:49.000000 bosing-2.0.6/example/hann.py
+-rw-r--r--   0     1001      127      788 2024-06-01 12:01:49.000000 bosing-2.0.6/example/interp.py
+-rw-r--r--   0     1001      127      696 2024-06-01 12:01:49.000000 bosing-2.0.6/example/overlap.py
+-rw-r--r--   0     1001      127     2074 2024-06-01 12:01:49.000000 bosing-2.0.6/example/schedule.py
+-rw-r--r--   0     1001      127     2362 2024-06-01 12:01:49.000000 bosing-2.0.6/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6327 2024-06-01 12:01:49.000000 bosing-2.0.6/ruff_defaults.toml
+-rw-r--r--   0     1001      127    11370 2024-06-01 12:01:49.000000 bosing-2.0.6/src/executor.rs
+-rw-r--r--   0     1001      127    62682 2024-06-01 12:01:49.000000 bosing-2.0.6/src/lib.rs
+-rw-r--r--   0     1001      127     7861 2024-06-01 12:01:49.000000 bosing-2.0.6/src/pulse/iir.rs
+-rw-r--r--   0     1001      127    17055 2024-06-01 12:01:49.000000 bosing-2.0.6/src/pulse.rs
+-rw-r--r--   0     1001      127     7540 2024-06-01 12:01:49.000000 bosing-2.0.6/src/quant.rs
+-rw-r--r--   0     1001      127     2367 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     9689 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule/grid/helper.rs
+-rw-r--r--   0     1001      127     6941 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3145 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2010 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3577 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     3132 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule/stack/helper.rs
+-rw-r--r--   0     1001      127     7464 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule/stack.rs
+-rw-r--r--   0     1001      127     7859 2024-06-01 12:01:49.000000 bosing-2.0.6/src/schedule.rs
+-rw-r--r--   0     1001      127     7677 2024-06-01 12:01:49.000000 bosing-2.0.6/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-06-01 12:01:49.000000 bosing-2.0.6/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-06-01 12:01:49.000000 bosing-2.0.6/tests/__init__.py
+-rw-r--r--   0     1001      127     1291 2024-06-01 12:01:49.000000 bosing-2.0.6/tests/test_basic.py
+-rw-r--r--   0     1001      127    22248 2024-06-01 12:02:02.000000 bosing-2.0.6/Cargo.lock
+-rw-r--r--   0     1001      127     1840 2024-06-01 12:01:49.000000 bosing-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2419 1970-01-01 00:00:00.000000 bosing-2.0.6/PKG-INFO
```

### Comparing `bosing-2.0.5/Cargo.toml` & `bosing-2.0.6/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [package]
 name = "bosing"
-version = "2.0.5"
+version = "2.0.6"
 edition = "2021"
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "bosing"
 crate-type = ["cdylib"]
 
 [dependencies]
 anyhow = "1.0.82"
-biquad = "0.4.2"
 bspline = "1.1.0"
 cached = "0.50.0"
 float-cmp = "0.9.0"
 hashbrown = { version = "0.14.5", features = ["rayon"] }
 indoc = "2.0.5"
 itertools = "0.12.1"
 ndarray = { version = "0.15.6", features = ["rayon"] }
```

### Comparing `bosing-2.0.5/.github/workflows/auto-dep.yml` & `bosing-2.0.6/.github/workflows/auto-dep.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/.github/workflows/ci.yml` & `bosing-2.0.6/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,27 @@
 
     steps:
       - uses: actions/checkout@v4
       - name: Cargo build
         run: cargo build --verbose
       - name: Cargo test
         run: cargo test --verbose
+      - name: Cargo fmt
+        run: cargo fmt --check
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
-      - name: Install hatch
-        run: |
-          python -m pip install --upgrade pip
-          pip install hatch
+      - name: Install Hatch
+        uses: pypa/hatch@a3c83ab3d481fbc2dc91dd0088628817488dd1d5
+        with:
+          version: 1.11.1
       - name: Test
-        run: hatch run test:run
+        run: hatch test --all
+      - name: Lint
+        run: hatch fmt --check
       - name: Stubtest
         run: hatch run stubcheck
 
   # Should run on every push and PR, but only run semantic-release on push
   release:
     name: Run semantic-release
     runs-on: ubuntu-latest
@@ -58,15 +62,15 @@
       pull-requests: write
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Semantic Release
-        uses: codfish/semantic-release-action@v3
+        uses: docker://ghcr.io/codfish/semantic-release-action@sha256:71048986f7e28f024cbad0ef106a7ef20b9b0d322f3a8aa51d89f1c424e75061 # v3.3.0
         # Only run on push events
         if: github.event_name == 'push'
         id: semantic-release
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           plugins: |
```

### Comparing `bosing-2.0.5/.gitignore` & `bosing-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/.readthedocs.yaml` & `bosing-2.0.6/.readthedocs.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -25,10 +25,11 @@
 #    - epub
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
   install:
-    - requirements: docs/requirements.txt
     - method: pip
       path: .
+      extra_requirements:
+        - docs
```

### Comparing `bosing-2.0.5/LICENSE.txt` & `bosing-2.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/README.md` & `bosing-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/bosing.pyi` & `bosing-2.0.6/bosing.pyi`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/docs/Makefile` & `bosing-2.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/docs/_templates/autosummary/module.rst` & `bosing-2.0.6/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/docs/conf.py` & `bosing-2.0.6/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "bosing"
-copyright = "2023, Jiahao Yuan"
+copyright = "2023, Jiahao Yuan"  # noqa: A001
 author = "Jiahao Yuan"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.viewcode",
```

### Comparing `bosing-2.0.5/docs/index.rst` & `bosing-2.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/docs/instruction.rst` & `bosing-2.0.6/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/docs/make.bat` & `bosing-2.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/docs/schedule.rst` & `bosing-2.0.6/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/example/flexible.py` & `bosing-2.0.6/example/flexible.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/example/hann.py` & `bosing-2.0.6/example/hann.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/example/interp.py` & `bosing-2.0.6/example/interp.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/example/overlap.py` & `bosing-2.0.6/example/overlap.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/example/schedule.py` & `bosing-2.0.6/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/example/schedule_stress.py` & `bosing-2.0.6/example/schedule_stress.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/ruff_defaults.toml` & `bosing-2.0.6/ruff_defaults.toml`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,15 @@
   "B028",
   "B029",
   "B030",
   "B031",
   "B032",
   "B033",
   "B034",
+  "B035",
   "B904",
   "B905",
   "BLE001",
   "C400",
   "C401",
   "C402",
   "C403",
@@ -79,15 +80,14 @@
   "DTZ006",
   "DTZ007",
   "DTZ011",
   "DTZ012",
   "E101",
   "E401",
   "E402",
-  "E501",
   "E701",
   "E702",
   "E703",
   "E711",
   "E712",
   "E713",
   "E714",
@@ -169,14 +169,18 @@
   "ICN002",
   "ICN003",
   "INP001",
   "INT001",
   "INT002",
   "INT003",
   "ISC003",
+  "LOG001",
+  "LOG002",
+  "LOG007",
+  "LOG009",
   "N801",
   "N802",
   "N803",
   "N804",
   "N805",
   "N806",
   "N807",
@@ -189,16 +193,14 @@
   "N817",
   "N818",
   "N999",
   "PERF101",
   "PERF102",
   "PERF401",
   "PERF402",
-  "PGH001",
-  "PGH002",
   "PGH005",
   "PIE790",
   "PIE794",
   "PIE796",
   "PIE800",
   "PIE804",
   "PIE807",
@@ -212,14 +214,15 @@
   "PLC0414",
   "PLC3002",
   "PLE0100",
   "PLE0101",
   "PLE0116",
   "PLE0117",
   "PLE0118",
+  "PLE0237",
   "PLE0241",
   "PLE0302",
   "PLE0307",
   "PLE0604",
   "PLE0605",
   "PLE1142",
   "PLE1205",
@@ -326,14 +329,15 @@
   "PYI050",
   "PYI051",
   "PYI052",
   "PYI053",
   "PYI054",
   "PYI055",
   "PYI056",
+  "PYI058",
   "RET503",
   "RET504",
   "RET505",
   "RET506",
   "RET507",
   "RET508",
   "RSE102",
@@ -342,32 +346,36 @@
   "RUF003",
   "RUF005",
   "RUF006",
   "RUF007",
   "RUF008",
   "RUF009",
   "RUF010",
-  "RUF011",
   "RUF012",
   "RUF013",
   "RUF015",
   "RUF016",
+  "RUF017",
+  "RUF018",
+  "RUF019",
+  "RUF020",
   "RUF100",
-  "RUF200",
   "S101",
   "S102",
   "S103",
   "S104",
   "S105",
   "S106",
   "S107",
   "S108",
   "S110",
   "S112",
   "S113",
+  "S201",
+  "S202",
   "S301",
   "S302",
   "S303",
   "S304",
   "S305",
   "S306",
   "S307",
@@ -383,36 +391,44 @@
   "S318",
   "S319",
   "S320",
   "S321",
   "S323",
   "S324",
   "S501",
+  "S502",
+  "S503",
+  "S504",
+  "S505",
   "S506",
+  "S507",
   "S508",
   "S509",
   "S601",
   "S602",
   "S604",
   "S605",
   "S606",
   "S607",
   "S608",
   "S609",
+  "S611",
   "S612",
   "S701",
+  "S702",
   "SIM101",
   "SIM102",
   "SIM103",
   "SIM105",
   "SIM107",
   "SIM108",
   "SIM109",
   "SIM110",
   "SIM112",
+  "SIM113",
   "SIM114",
   "SIM115",
   "SIM116",
   "SIM117",
   "SIM118",
   "SIM201",
   "SIM202",
@@ -422,37 +438,43 @@
   "SIM212",
   "SIM220",
   "SIM221",
   "SIM222",
   "SIM223",
   "SIM300",
   "SIM910",
+  "SIM911",
   "SLF001",
   "SLOT000",
   "SLOT001",
   "SLOT002",
   "T100",
   "T201",
   "T203",
   "TCH001",
   "TCH002",
   "TCH003",
   "TCH004",
   "TCH005",
+  "TCH010",
   "TD004",
   "TD005",
   "TD006",
   "TD007",
   "TID251",
   "TID252",
   "TID253",
+  "TRIO100",
+  "TRIO105",
+  "TRIO109",
+  "TRIO110",
+  "TRIO115",
   "TRY002",
   "TRY003",
   "TRY004",
-  "TRY200",
   "TRY201",
   "TRY300",
   "TRY301",
   "TRY302",
   "TRY400",
   "TRY401",
   "UP001",
@@ -489,14 +511,15 @@
   "UP034",
   "UP035",
   "UP036",
   "UP037",
   "UP038",
   "UP039",
   "UP040",
+  "UP041",
   "W291",
   "W292",
   "W293",
   "W505",
   "W605",
   "YTT101",
   "YTT102",
```

### Comparing `bosing-2.0.5/src/executor.rs` & `bosing-2.0.6/src/executor.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/lib.rs` & `bosing-2.0.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/pulse.rs` & `bosing-2.0.6/src/pulse.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+mod iir;
+
 use std::{
     ops::{Add, Mul},
     sync::Arc,
 };
 
 use anyhow::{bail, Context, Result};
-use biquad::Biquad as _;
 use cached::proc_macro::cached;
 use float_cmp::approx_eq;
 use hashbrown::HashMap;
 use itertools::{izip, Itertools};
 use ndarray::{azip, s, ArrayView1, ArrayView2, ArrayViewMut2, Axis};
 use numpy::Complex64;
 use pulp::{Arch, Simd, WithSimd};
@@ -476,42 +477,15 @@
 
 pub(crate) fn apply_offset_inplace(waveform: &mut ArrayViewMut2<f64>, offset: ArrayView1<f64>) {
     assert!(waveform.shape()[0] == offset.len());
     azip!((mut row in waveform.axis_iter_mut(Axis(0)), &offset in &offset) row += offset);
 }
 
 pub(crate) fn apply_iir_inplace(waveform: &mut ArrayViewMut2<f64>, sos: ArrayView2<f64>) {
-    let mut biquads: Vec<_> = sos
-        .axis_iter(Axis(0))
-        .map(|row| {
-            let b0 = row[0];
-            let b1 = row[1];
-            let b2 = row[2];
-            let a1 = row[4];
-            let a2 = row[5];
-            let coef = biquad::Coefficients { b0, a1, a2, b1, b2 };
-            biquad::DirectForm2Transposed::<f64>::new(coef)
-        })
-        .collect();
-    for mut row in waveform.axis_iter_mut(Axis(0)) {
-        apply_iir_inplace_1d(row.as_slice_mut().unwrap(), &mut biquads);
-    }
-}
-
-fn apply_iir_inplace_1d(waveform: &mut [f64], biquads: &mut [biquad::DirectForm2Transposed<f64>]) {
-    for biquad in biquads.iter_mut() {
-        biquad.reset_state();
-    }
-    for y in waveform.iter_mut() {
-        let mut x = *y;
-        for biquad in biquads.iter_mut() {
-            x = biquad.run(x);
-        }
-        *y = x;
-    }
+    self::iir::iir_filter_inplace(waveform.view_mut(), sos).unwrap()
 }
 
 pub(crate) fn apply_fir_inplace(waveform: &mut ArrayViewMut2<f64>, taps: ArrayView1<f64>) {
     let arch = Arch::new();
     arch.dispatch(ApplyFirInplace {
         waveform: waveform.view_mut(),
         taps,
```

### Comparing `bosing-2.0.5/src/quant.rs` & `bosing-2.0.6/src/quant.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule/absolute.rs` & `bosing-2.0.6/src/schedule/absolute.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule/grid/helper.rs` & `bosing-2.0.6/src/schedule/grid/helper.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule/grid.rs` & `bosing-2.0.6/src/schedule/grid.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule/play.rs` & `bosing-2.0.6/src/schedule/play.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule/repeat.rs` & `bosing-2.0.6/src/schedule/repeat.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule/simple.rs` & `bosing-2.0.6/src/schedule/simple.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule/stack/helper.rs` & `bosing-2.0.6/src/schedule/stack/helper.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule/stack.rs` & `bosing-2.0.6/src/schedule/stack.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/schedule.rs` & `bosing-2.0.6/src/schedule.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/src/shape.rs` & `bosing-2.0.6/src/shape.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/tests/test_basic.py` & `bosing-2.0.6/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.5/Cargo.lock` & `bosing-2.0.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -35,34 +35,24 @@
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
-name = "biquad"
-version = "0.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "820524f5e3e3add696ddf69f79575772e152c0e78e9f0370b56990a7e808ec3e"
-dependencies = [
- "libm 0.1.4",
-]
-
-[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.5"
+version = "2.0.6"
 dependencies = [
  "anyhow",
- "biquad",
  "bspline",
  "cached",
  "float-cmp",
  "hashbrown",
  "indoc",
  "itertools",
  "mockall",
@@ -282,20 +272,14 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libm"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fc7aa29613bd6a620df431842069224d8bc9011086b1db4c0e0cd47fa03ec9a"
-
-[[package]]
-name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
@@ -539,15 +523,15 @@
 [[package]]
 name = "pulp"
 version = "0.18.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "762ad20f6b65f5a33874de3b7506d6cf6631d37fb9c0c6ee0e310d7210a167d9"
 dependencies = [
  "bytemuck",
- "libm 0.2.8",
+ "libm",
  "num-complex",
  "reborrow",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
```

### Comparing `bosing-2.0.5/pyproject.toml` & `bosing-2.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,56 +15,51 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
 ]
-dependencies = ["numpy", "scipy"]
+dependencies = ["numpy >= 1.16.0"]
+
+[project.optional-dependencies]
+docs = ["sphinx", "furo", "matplotlib", "scipy"]
 
 [project.urls]
 Documentation = "https://bosing.readthedocs.io"
 Issues = "https://github.com/kahojyun/Bosing/issues"
 Source = "https://github.com/kahojyun/Bosing"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [tool.hatch.envs.default]
+features = ["docs"]
 dependencies = [
     "maturin>=1.5,<2.0",
-    "matplotlib",
     "ipython",
-    "sphinx",
-    "furo",
     "mypy",
 ]
 
 [tool.hatch.envs.default.scripts]
 mip = "maturin develop && ipython"
 stubcheck = "maturin develop && stubtest bosing --allowlist stubtest-allowlist.txt"
 build_docs = "maturin develop && sphinx-build -M html docs docs/_build {args}"
 clean_docs = "rm -rf docs/_build docs/generated"
 
 [tool.hatch.envs.default.overrides]
 platform.windows.scripts = [
     'clean_docs=rmdir /s /q docs\\_build docs\\generated',
 ]
 
-[tool.hatch.envs.test]
-dependencies = ["pytest"]
-
-[[tool.hatch.envs.test.matrix]]
+[[tool.hatch.envs.hatch-test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
-[tool.hatch.envs.test.scripts]
-run = "pytest {args}"
-
-[tool.pytest.ini_options]
-addopts = ["--import-mode=importlib"]
-testpaths = ["tests"]
-
 [tool.hatch.envs.hatch-static-analysis]
 config-path = "ruff_defaults.toml"
 
 [tool.ruff]
 extend = "ruff_defaults.toml"
+
+[tool.ruff.lint.extend-per-file-ignores]
+"docs/conf.py" = ["INP001"]
+"example/*" = ["INP001", "T201"]
```

### Comparing `bosing-2.0.5/PKG-INFO` & `bosing-2.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.5
+Version: 2.0.6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: numpy
-Requires-Dist: scipy
+Requires-Dist: numpy >=1.16.0
+Requires-Dist: sphinx ; extra == 'docs'
+Requires-Dist: furo ; extra == 'docs'
+Requires-Dist: matplotlib ; extra == 'docs'
+Requires-Dist: scipy ; extra == 'docs'
+Provides-Extra: docs
 License-File: LICENSE.txt
 Summary: Waveform generator for pulse sequences in quantum computing
 Keywords: 
 Author-email: kaho <kaho0769@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

