# Comparing `tmp/damply-0.4.0.tar.gz` & `tmp/damply-0.4.1.tar.gz`

## Comparing `damply-0.4.0.tar` & `damply-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.4.0/pixi.lock
--rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.4.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 damply-0.4.0/config/coverage.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 damply-0.4.0/config/hatch.toml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.4.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 damply-0.4.0/config/releaserc.toml
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 damply-0.4.0/config/ruff.toml
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 damply-0.4.0/devnotes/pixi-hatch-build.md
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 damply-0.4.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.4.0/docs/about.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/__init__.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/cli.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/metadata.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/utils/byte_size.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/utils/whose.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.4.0/tests/test_general.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 damply-0.4.0/tests/test_metadata.py
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/invalid_.md
--rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/README_gcsi.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file9.txt
--rwxr-xr-x   0        0        0     1210 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/kallisto/README_kallisto.md
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/README_simple.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file9.txt
--rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/README_vanderijn.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file9.txt
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 damply-0.4.0/.gitignore
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 damply-0.4.0/README.md
--rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 damply-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 damply-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.4.1/pixi.lock
+-rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.4.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 damply-0.4.1/config/coverage.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 damply-0.4.1/config/hatch.toml
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 damply-0.4.1/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 damply-0.4.1/config/releaserc.toml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 damply-0.4.1/config/ruff.toml
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 damply-0.4.1/devnotes/pixi-hatch-build.md
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 damply-0.4.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.4.1/docs/about.md
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 damply-0.4.1/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 damply-0.4.1/src/damply/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 damply-0.4.1/src/damply/cli.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 damply-0.4.1/src/damply/metadata.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 damply-0.4.1/src/damply/utils/byte_size.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 damply-0.4.1/src/damply/utils/whose.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.4.1/tests/test_general.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 damply-0.4.1/tests/test_metadata.py
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/invalid_.md
+-rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/README_gcsi.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/gcsi/test_dir_1/file9.txt
+-rwxr-xr-x   0        0        0     1210 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/kallisto/README_kallisto.md
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/README_simple.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/simple/test_dir_1/file9.txt
+-rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/README_vanderijn.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.1/tests/examples/vanderijn/test_dir_1/file9.txt
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 damply-0.4.1/.gitignore
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 damply-0.4.1/README.md
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 damply-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 damply-0.4.1/PKG-INFO
```

### Comparing `damply-0.4.0/pixi.lock` & `damply-0.4.1/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2853,17 +2853,17 @@
   license_family: BSD
   purls:
   - pkg:pypi/cryptography?source=conda-forge-mapping
   size: 1978679
   timestamp: 1715044173081
 - kind: pypi
   name: damply
-  version: 0.4.0
+  version: 0.4.1
   path: .
-  sha256: b2811d5009d9ac733800bddaa30d3d134178741e59d03d7a9083f3ed7df25897
+  sha256: 8e280c77e10e972c3842e7eef671e018b6aebfa61042a893ddc619c6400647d4
   requires_dist:
   - rich
   - rich-click
   - pydantic
   - textual
   - trogon
   - dataclasses-json
@@ -5812,40 +5812,48 @@
   purls:
   - pkg:pypi/pydantic?source=conda-forge-mapping
   size: 282316
   timestamp: 1716962269411
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
+  url: https://files.pythonhosted.org/packages/94/bc/e5d1938f36cad75525e923ecfef6f544970d4f14800716728ea5555fc574/pydantic_core-2.18.3-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 0bee9bb305a562f8b9271855afb6ce00223f545de3d68560b3c1649c7c5295e9
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.3
   url: https://files.pythonhosted.org/packages/e3/5c/477dac00c0d6d34921fec2507ae6aea2cd7c84072eab1dca5bcbbf86c4a2/pydantic_core-2.18.3-cp312-none-win_amd64.whl
   sha256: 2c8333f6e934733483c7eddffdb094c143b9463d2af7e6bd85ebcb2d4a1b82c6
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/77/72/3ce28b58f3d9c9a8bb59984d810be3eabba4455e92de806a4edacd4e5c0b/pydantic_core-2.18.3-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: f0928cde2ae416a2d1ebe6dee324709c6f73e93494d8c7aea92df99aab1fc40f
+  url: https://files.pythonhosted.org/packages/c2/9f/e2f17d24aee5406a8e8e57784fa737abde9ac538d18028b523268796bcce/pydantic_core-2.18.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 24b214b7ee3bd3b865e963dbed0f8bc5375f49449d70e8d407b567af3222aae4
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/94/bc/e5d1938f36cad75525e923ecfef6f544970d4f14800716728ea5555fc574/pydantic_core-2.18.3-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 0bee9bb305a562f8b9271855afb6ce00223f545de3d68560b3c1649c7c5295e9
+  url: https://files.pythonhosted.org/packages/77/72/3ce28b58f3d9c9a8bb59984d810be3eabba4455e92de806a4edacd4e5c0b/pydantic_core-2.18.3-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: f0928cde2ae416a2d1ebe6dee324709c6f73e93494d8c7aea92df99aab1fc40f
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/c2/9f/e2f17d24aee5406a8e8e57784fa737abde9ac538d18028b523268796bcce/pydantic_core-2.18.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 24b214b7ee3bd3b865e963dbed0f8bc5375f49449d70e8d407b567af3222aae4
+  url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
+  sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
   url: https://files.pythonhosted.org/packages/a0/27/aeade6d7b2f2bcc8fc835bdf6aa705f6f34508da380f170e13cd37477dd4/pydantic_core-2.18.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
@@ -5868,38 +5876,30 @@
   sha256: 45e4ffbae34f7ae30d0047697e724e534a7ec0a82ef9994b7913a412c21462a0
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
-  sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
+  url: https://files.pythonhosted.org/packages/d2/c7/e01cb2017c4b7b274258694f73e8bbbb0988a28b49802e569d1d9bfd51cb/pydantic_core-2.18.3-cp311-none-win_amd64.whl
+  sha256: 58ff8631dbab6c7c982e6425da8347108449321f61fe427c52ddfadd66642af7
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
   url: https://files.pythonhosted.org/packages/0c/84/a14457b3cb1ec1f5d1567395abe11ab420dd76733bc79dd0124a874e9eac/pydantic_core-2.18.3-cp311-cp311-macosx_11_0_arm64.whl
   sha256: b8e20e15d18bf7dbb453be78a2d858f946f5cdf06c5072453dace00ab652e2b2
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/d2/c7/e01cb2017c4b7b274258694f73e8bbbb0988a28b49802e569d1d9bfd51cb/pydantic_core-2.18.3-cp311-none-win_amd64.whl
-  sha256: 58ff8631dbab6c7c982e6425da8347108449321f61fe427c52ddfadd66642af7
-  requires_dist:
-  - typing-extensions>=4.6.0,!=4.7.0
-  requires_python: '>=3.8'
-- kind: pypi
-  name: pydantic-core
-  version: 2.18.3
   url: https://files.pythonhosted.org/packages/4a/cf/2847167bab3e7676ba6f0b49963ba04112b1e4281d8c70e302c2fd29e08c/pydantic_core-2.18.3-cp311-cp311-macosx_10_12_x86_64.whl
   sha256: b9ebe8231726c49518b16b237b9fe0d7d361dd221302af511a83d4ada01183ab
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
```

### Comparing `damply-0.4.0/.github/workflows/main.yaml` & `damply-0.4.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/config/mkdocs.yaml` & `damply-0.4.1/config/mkdocs.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -19,13 +19,12 @@
 remote_branch: gh-pages
 
 # Address when using 'mkdocs serve', format is 'address:port'
 dev_addr: 127.0.0.1:8000
 
 # The layout of the navigation links
 nav:
-  - Home: ../README.md
   - Home: index.md
   - About: about.md
   - Changelog: CHANGELOG.md
 
 theme: readthedocs
```

### Comparing `damply-0.4.0/config/releaserc.toml` & `damply-0.4.1/config/releaserc.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [semantic_release]
-version_variables = ["src/damply/__init__.py:version"]
+version_variables = ["src/damply/__init__.py:__version__"]
 version_toml = [
   "pyproject.toml:project.version",
   "pyproject.toml:tool.pixi.version",
 ]
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
```

### Comparing `damply-0.4.0/config/ruff.toml` & `damply-0.4.1/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/devnotes/pixi-hatch-build.md` & `damply-0.4.1/devnotes/pixi-hatch-build.md`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/docs/CHANGELOG.md` & `damply-0.4.1/docs/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v0.4.1 (2024-05-31)
+
+### Chore
+
+* chore: Update navigation links in mkdocs.yaml ([`931524b`](https://github.com/jjjermiah/damply/commit/931524b39f8ca9edb971c8a43b84dc858b4a2de8))
+
+### Fix
+
+* fix: Update metadata table title in cli.py ([`a63c36b`](https://github.com/jjjermiah/damply/commit/a63c36bba26d880abf433cf06690faecb1537d3d))
+
+* fix: version ([`ecefaaf`](https://github.com/jjjermiah/damply/commit/ecefaafab444f70ace8a8185240d6577fe4db0a3))
+
+* fix: format ([`e153b30`](https://github.com/jjjermiah/damply/commit/e153b30f32108b0a9750f1a4b0c7e0b00116c152))
+
+
 ## v0.4.0 (2024-05-31)
 
 ### Feature
 
 * feat: add cli whose ([`b15ec32`](https://github.com/jjjermiah/damply/commit/b15ec32b551533aab892b3b3227e2091c643dfe1))
 
 * feat: Update CLI help messages and add &#39;whose&#39; command ([`620f209`](https://github.com/jjjermiah/damply/commit/620f209656ab91d5f8ae4e11608eaa6aef05e3f9))
```

### Comparing `damply-0.4.0/docs/about.md` & `damply-0.4.1/docs/about.md`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/src/damply/cli.py` & `damply-0.4.1/src/damply/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,115 +4,113 @@
 import rich_click as click
 from rich import print
 
 from damply.metadata import DMPMetadata
 from damply.utils import whose as whose_util
 
 click.rich_click.OPTION_GROUPS = {
-    "damply": [
+    'damply': [
         {
-            "name": "Basic options",
-            "options": ["--help"],
+            'name': 'Basic options',
+            'options': ['--help'],
         },
     ]
 }
 
 click.rich_click.COMMAND_GROUPS = {
-    "damply": [
+    'damply': [
         {
-            "name": "Subcommands",
-            "commands": ["version", "view", "whose"],
+            'name': 'Subcommands',
+            'commands': ['version', 'view', 'whose'],
         }
     ]
 }
 
 help_config = click.RichHelpConfiguration(
     show_arguments=True,
-    option_groups={"damply": [{"name": "Arguments", "panel_styles": {"box": "ASCII"}}]},
+    option_groups={'damply': [{'name': 'Arguments', 'panel_styles': {'box': 'ASCII'}}]},
 )
 
 
-@click.group(name="damply", context_settings={"help_option_names": ["-h", "--help"]})
+@click.group(name='damply', context_settings={'help_option_names': ['-h', '--help']})
 def cli() -> None:
     """A tool to interact with systems implementing the Data Management Plan (DMP) standard."""
     pass
 
 
 @cli.command()
 def version() -> None:
     """Print the version of damply."""
     from . import __version__ as ver
 
-    print(f"damply version {ver}")
+    print(f'damply version {ver}')
 
 
-@cli.command(context_settings={"help_option_names": ["-h", "--help"]})
+@cli.command(context_settings={'help_option_names': ['-h', '--help']})
 @click.argument(
-    "directory",
+    'directory',
     type=click.Path(
         exists=True,
         path_type=Path,
         file_okay=False,
         dir_okay=True,
         readable=True,
     ),
     default=Path().cwd(),
 )
 @click.rich_config(help_config=help_config)
 def view(directory: Path) -> None:
     """View the DMP Metadata of a valid DMP Directory."""
-    readmes = [f for f in directory.glob("README*") if f.is_file()]
+    readmes = [f for f in directory.glob('README*') if f.is_file()]
 
     if len(readmes) == 0:
-        print("No README file found.")
+        print('No README file found.')
         return
     elif len(readmes) > 1:
-        print("Multiple README files found. Using the first one.")
+        print('Multiple README files found. Using the first one.')
         readme = readmes[0]
     else:
         readme = readmes[0]
 
     metadata = DMPMetadata.from_path(readme)
 
     from rich.console import Console
     from rich.markdown import Markdown
     from rich.table import Table
 
     console = Console()
 
     table = Table.grid(padding=1, pad_edge=True, expand=True)
-    table.title = f"[bold]Metadata for {metadata.path.name}[/bold]"
-    table.add_column("Field", justify="right", style="cyan")
-    table.add_column("Value", style="yellow")
+    table.title = f'[bold]Metadata for {metadata.path.absolute()}[/bold]'
+    table.add_column('Field', justify='right', style='cyan')
+    table.add_column('Value', style='yellow')
 
     for field, value in metadata.fields.items():
         table.add_row(field, value)
 
     console.print(table)
     console.print(Markdown(metadata.content))
-    console.print(Markdown("\n".join(metadata.logs)))
+    console.print(Markdown('\n'.join(metadata.logs)))
 
 
-@cli.command(context_settings={"help_option_names": ["-h", "--help"]})
+@cli.command(context_settings={'help_option_names': ['-h', '--help']})
 @click.argument(
-    "path",
+    'path',
     type=click.Path(
         exists=True,
         path_type=Path,
         file_okay=True,
         dir_okay=True,
         readable=True,
     ),
     default=Path().cwd(),
 )
 @click.rich_config(help_config=help_config)
 def whose(path: Path) -> None:
     """Print the owner of the file or directory."""
     result = whose_util.get_file_owner_full_name(path)
 
-    print(
-        f"The owner of [bold magenta]{path}[/bold magenta] is [bold cyan]{result}[/bold cyan]"
-    )
+    print(f'The owner of [bold magenta]{path}[/bold magenta] is [bold cyan]{result}[/bold cyan]')
 
 
-def hello() -> Literal["Hello, World!"]:
-    return "Hello, World!"
+def hello() -> Literal['Hello, World!']:
+    return 'Hello, World!'
```

### Comparing `damply-0.4.0/src/damply/metadata.py` & `damply-0.4.1/src/damply/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,181 +4,181 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Type
 
 import rich.repr
 from rich import print
 
+
 def is_file_writable(file_path: Path) -> bool:
     import os
 
     return file_path.exists() and os.access(file_path, os.W_OK)
 
 
 @dataclass
 class DMPMetadata:
     fields: dict = field(default_factory=dict)
     content: str = field(default_factory=str, repr=False)
     path: Path = field(default=Path().cwd())
-    permissions: str = field(default="---------")
+    permissions: str = field(default='---------')
     logs: list = field(default_factory=list, repr=True)
 
     @classmethod
-    def from_path(cls: Type["DMPMetadata"], path: Path) -> "DMPMetadata":
-        if "README" not in path.stem.upper():
-            raise ValueError("The file is not a README file.")
+    def from_path(cls: Type['DMPMetadata'], path: Path) -> 'DMPMetadata':
+        if 'README' not in path.stem.upper():
+            raise ValueError('The file is not a README file.')
 
         metadata = cls()
         metadata.path = path
         metadata.permissions = cls.evaluate_permissions(path)
 
         if not metadata.is_readable():
-            raise PermissionError(f"{path} is not readable: {metadata.permissions}")
+            raise PermissionError(f'{path} is not readable: {metadata.permissions}')
 
         metadata.fields = cls._parse_readme(path)
 
         # remove the content field from the fields dict
-        metadata.content = metadata.fields.pop("content", "")
+        metadata.content = metadata.fields.pop('content', '')
 
         return metadata
 
     def log_change(self, description: str) -> None:
-        timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M")
-        self.logs.append(f"{timestamp}: {description}")
+        timestamp = datetime.datetime.now().strftime('%Y-%m-%d %H:%M')
+        self.logs.append(f'{timestamp}: {description}')
 
     def write_to_file(self, newpath: Path | None = None) -> None:
-        newpath = newpath or self.path.with_name(self.path.stem + ".dmp")
+        newpath = newpath or self.path.with_name(self.path.stem + '.dmp')
 
         if not is_file_writable(newpath):
-            raise PermissionError(f"{newpath} is not writable: {self.permissions}")
+            raise PermissionError(f'{newpath} is not writable: {self.permissions}')
 
         # with newpath.open(mode='w') as file:
-        file = newpath.open(mode="w")
+        file = newpath.open(mode='w')
         for fld, value in self.fields.items():
-            line = f"#{fld}: {value}"
+            line = f'#{fld}: {value}'
             if len(line) > 80:
                 # If the line length exceeds 80,
                 # split it into multiple lines without breaking words
                 words = line.split()
                 lines = []
-                current_line = ""
+                current_line = ''
                 for word in words:
                     if len(current_line) + len(word) + 1 <= 80:
-                        current_line += word + " "
+                        current_line += word + ' '
                     else:
                         lines.append(current_line.strip())
-                        current_line = word + " "
+                        current_line = word + ' '
                 if current_line:
                     lines.append(current_line.strip())
-                file.write("\n".join(lines))
+                file.write('\n'.join(lines))
             else:
                 file.write(line)
-            file.write("\n\n")
+            file.write('\n\n')
         if self.content:
-            file.write(f"\n{self.content}")
+            file.write(f'\n{self.content}')
         if self.logs:
-            file.write("\n\n\n")
+            file.write('\n\n\n')
             for log in self.logs:
-                file.write(f"\n{log}")
+                file.write(f'\n{log}')
         file.close()
 
     @classmethod
     def _parse_readme(
-        cls: Type["DMPMetadata"],
+        cls: Type['DMPMetadata'],
         readme: Path,
-        pattern: re.Pattern[str] = re.compile(r"^#([A-Z]+): (.+)$"),
+        pattern: re.Pattern[str] = re.compile(r'^#([A-Z]+): (.+)$'),
     ) -> dict:
         current_field = None
         current_value = []
         content_lines = []
         metadata = {}
-        with readme.open(mode="r") as file:
+        with readme.open(mode='r') as file:
             for line in file:
-                if line.strip() == "" and current_field:
+                if line.strip() == '' and current_field:
                     # End current field on double newline
-                    metadata[current_field] = " ".join(current_value).strip()
+                    metadata[current_field] = ' '.join(current_value).strip()
                     current_field = None
                     current_value = []
                 else:
                     match = pattern.match(line.strip())
                     if match:
                         if current_field:
-                            metadata[current_field] = " ".join(current_value).strip()
+                            metadata[current_field] = ' '.join(current_value).strip()
                         current_field, current_value = (
                             match.groups()[0],
                             [match.groups()[1]],
                         )
                     elif current_field:
                         current_value.append(line.strip())
                     else:
                         content_lines.append(line.strip())
 
             if current_field:
-                metadata[current_field] = " ".join(current_value).strip()
+                metadata[current_field] = ' '.join(current_value).strip()
 
-        metadata["content"] = "\n".join(content_lines).strip()
+        metadata['content'] = '\n'.join(content_lines).strip()
         return metadata
 
     def __getitem__(self, item: str) -> str:
         return self.fields.get(item, None)
 
     def __setitem__(self, key: str, value: str) -> None:
         self.fields[key] = value
 
     @staticmethod
     def evaluate_permissions(path: Path) -> str:
         permissions = path.stat().st_mode
-        is_dir = "d" if stat.S_ISDIR(permissions) else "-"
+        is_dir = 'd' if stat.S_ISDIR(permissions) else '-'
         perm_bits = [
-            (permissions & stat.S_IRUSR, "r"),
-            (permissions & stat.S_IWUSR, "w"),
-            (permissions & stat.S_IXUSR, "x"),
-            (permissions & stat.S_IRGRP, "r"),
-            (permissions & stat.S_IWGRP, "w"),
-            (permissions & stat.S_IXGRP, "x"),
-            (permissions & stat.S_IROTH, "r"),
-            (permissions & stat.S_IWOTH, "w"),
-            (permissions & stat.S_IXOTH, "x"),
+            (permissions & stat.S_IRUSR, 'r'),
+            (permissions & stat.S_IWUSR, 'w'),
+            (permissions & stat.S_IXUSR, 'x'),
+            (permissions & stat.S_IRGRP, 'r'),
+            (permissions & stat.S_IWGRP, 'w'),
+            (permissions & stat.S_IXGRP, 'x'),
+            (permissions & stat.S_IROTH, 'r'),
+            (permissions & stat.S_IWOTH, 'w'),
+            (permissions & stat.S_IXOTH, 'x'),
         ]
-        formatted_permissions = is_dir + "".join(
-            bit[1] if bit[0] else "-" for bit in perm_bits
-        )
+        formatted_permissions = is_dir + ''.join(bit[1] if bit[0] else '-' for bit in perm_bits)
         return formatted_permissions
 
     def get_permissions(self) -> str:
         if not self.permissions:
-            return "No permissions set."
+            return 'No permissions set.'
         return self.permissions
 
     def is_writeable(self) -> bool:
-        return "w" in self.permissions
+        return 'w' in self.permissions
 
     def is_readable(self) -> bool:
-        return "r" in self.permissions
+        return 'r' in self.permissions
 
     def __rich_repr__(self) -> rich.repr.Result:
-        yield "path", self.path
-        yield "fields", self.fields
-        yield "content", self.content
-        yield "permissions", self.permissions
-        yield "logs", self.logs
+        yield 'path', self.path
+        yield 'fields', self.fields
+        yield 'content', self.content
+        yield 'permissions', self.permissions
+        yield 'logs', self.logs
+
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     # test the function
     cwd = Path.cwd()
-    readme_example_dir = cwd / "tests" / "examples"
+    readme_example_dir = cwd / 'tests' / 'examples'
 
-    all_dirs = list(readme_example_dir.glob("*"))
+    all_dirs = list(readme_example_dir.glob('*'))
 
-    all_files = [file for directoru in all_dirs for file in directoru.glob("README*")]
+    all_files = [file for directoru in all_dirs for file in directoru.glob('README*')]
 
     dmps = []
     for file in all_files:
         dmp = DMPMetadata.from_path(file)
         print()
         dmps.append(dmp)
 
     print(dmps[3])
-    dmps[3].log_change("Added a log entry.")
-    dmps[3].log_change("Added another log entry.")
+    dmps[3].log_change('Added a log entry.')
+    dmps[3].log_change('Added another log entry.')
     print(dmps[3])
     dmps[3].write_to_file()
```

### Comparing `damply-0.4.0/src/damply/utils/byte_size.py` & `damply-0.4.1/src/damply/utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/src/damply/utils/whose.py` & `damply-0.4.1/src/damply/utils/whose.py`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/tests/test_metadata.py` & `damply-0.4.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/tests/examples/gcsi/README_gcsi.md` & `damply-0.4.1/tests/examples/gcsi/README_gcsi.md`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/tests/examples/kallisto/README_kallisto.md` & `damply-0.4.1/tests/examples/kallisto/README_kallisto.md`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/tests/examples/vanderijn/README_vanderijn.md` & `damply-0.4.1/tests/examples/vanderijn/README_vanderijn.md`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/.gitignore` & `damply-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/README.md` & `damply-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `damply-0.4.0/pyproject.toml` & `damply-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "damply"
-version = "0.4.0"
+version = "0.4.1"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["damply", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
@@ -123,24 +123,24 @@
 # Available tasks: doc-build, doc-serve, doc-deploy
 # See config/mkdocs.yaml for the configuration
 [tool.pixi.feature.docs.dependencies]
 mkdocs = "*"
 
 [tool.pixi.feature.docs.tasks.doc-build]
 cmd = "mkdocs build -f config/mkdocs.yaml"
-inputs = ["docs"]
+inputs = ["docs", "config/mkdocs.yaml"]
 outputs = ["site"]
 
 [tool.pixi.feature.docs.tasks.doc-serve]
 cmd = "mkdocs serve -f config/mkdocs.yaml"
-inputs = ["docs"]
+inputs = ["docs", "config/mkdocs.yaml"]
 
 [tool.pixi.feature.docs.tasks.doc-deploy]
 cmd = "mkdocs gh-deploy -f config/mkdocs.yaml --force"
-inputs = ["docs"]
+inputs = ["docs", "config/mkdocs.yaml"]
 
 #################################### RELEASE & BUILD ###############################################
 [tool.pixi.feature.release.dependencies]
 python-semantic-release = ">=8.5.1"
 
 [tool.pixi.feature.release.tasks]
 # Semver task will only work on the main or dev/develop branch (see releaserc.toml:branches)
```

### Comparing `damply-0.4.0/PKG-INFO` & `damply-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: damply
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/damply
 Project-URL: repository, https://github.com/jjjermiah/damply
 Project-URL: documentation, https://jjjermiah.github.io/damply/
 Project-URL: changelog, https://github.com/jjjermiah/damply/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/damply/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

