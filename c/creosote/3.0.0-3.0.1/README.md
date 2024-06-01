# Comparing `tmp/creosote-3.0.0-py3-none-any.whl.zip` & `tmp/creosote-3.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16036 bytes, number of entries: 14
+Zip file size: 16142 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 creosote/__about__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 creosote/__init__.py
 -rw-r--r--  2.0 unx       72 b- defN 20-Feb-02 00:00 creosote/__main__.py
 -rw-r--r--  2.0 unx     2015 b- defN 20-Feb-02 00:00 creosote/cli.py
--rw-r--r--  2.0 unx     5703 b- defN 20-Feb-02 00:00 creosote/config.py
+-rw-r--r--  2.0 unx     5689 b- defN 20-Feb-02 00:00 creosote/config.py
 -rw-r--r--  2.0 unx     1109 b- defN 20-Feb-02 00:00 creosote/formatters.py
 -rw-r--r--  2.0 unx      523 b- defN 20-Feb-02 00:00 creosote/models.py
 -rw-r--r--  2.0 unx     9523 b- defN 20-Feb-02 00:00 creosote/parsers.py
--rw-r--r--  2.0 unx     9397 b- defN 20-Feb-02 00:00 creosote/resolvers.py
-?rw-r--r--  2.0 unx    14683 b- defN 20-Feb-02 00:00 creosote-3.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-3.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-3.0.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-3.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1083 b- defN 20-Feb-02 00:00 creosote-3.0.0.dist-info/RECORD
-14 files, 45336 bytes uncompressed, 14250 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx     9549 b- defN 20-Feb-02 00:00 creosote/resolvers.py
+?rw-r--r--  2.0 unx    15130 b- defN 20-Feb-02 00:00 creosote-3.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-3.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-3.0.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-3.0.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1083 b- defN 20-Feb-02 00:00 creosote-3.0.1.dist-info/RECORD
+14 files, 45921 bytes uncompressed, 14356 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: creosote/parsers.py
 Comment: 
 
 Filename: creosote/resolvers.py
 Comment: 
 
-Filename: creosote-3.0.0.dist-info/METADATA
+Filename: creosote-3.0.1.dist-info/METADATA
 Comment: 
 
-Filename: creosote-3.0.0.dist-info/WHEEL
+Filename: creosote-3.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: creosote-3.0.0.dist-info/entry_points.txt
+Filename: creosote-3.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: creosote-3.0.0.dist-info/licenses/LICENSE
+Filename: creosote-3.0.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: creosote-3.0.0.dist-info/RECORD
+Filename: creosote-3.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## creosote/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "3.0.0"
+__version__ = "3.0.1"
```

## creosote/config.py

```diff
@@ -16,15 +16,15 @@
 class Config:
     """Structured configuration data.
 
     It is important that these attributes exactly match
     the ``dest`` specified in ``add_argument``.
     """
 
-    format: Literal["default", "no-color", "porcelain"] = "default"  # noqa: A003
+    format: Literal["default", "no-color", "porcelain"] = "default"
     paths: List[str] = field(default_factory=lambda: ["src"])
     sections: List[str] = field(default_factory=lambda: ["project.dependencies"])
     exclude_deps: List[str] = field(default_factory=list)
     deps_file: str = "pyproject.toml"
     venvs: List[str] = field(
         default_factory=lambda: [os.environ.get("VIRTUAL_ENV", ".venv")]
     )
```

## creosote/resolvers.py

```diff
@@ -19,17 +19,17 @@
         self.imports: List[ImportInfo] = imports
         self.dependencies: List[DependencyInfo] = [
             DependencyInfo(name=dep) for dep in dependency_names
         ]
         self.venvs: List[str] = venvs
 
         self.top_level_txt_pattern = re.compile(
-            r"\/([\w]*).[\d\.]*.dist-info\/top_level.txt"
+            r"\/([\w\.]*).[\d\.]*.dist-info\/top_level.txt"
         )
-        self.record_pattern = re.compile(r"\/([\w]*).[\d\.]*.dist-info\/RECORD")
+        self.record_pattern = re.compile(r"\/([\w\.]*).[\d\.]*.dist-info\/RECORD")
 
         self.top_level_filepaths: List[pathlib.Path] = []
         self.record_filepaths: List[pathlib.Path] = []
         self.unused_deps: List[DependencyInfo] = []
 
     @staticmethod
     def canonicalize_module_name(module_name: str) -> str:
@@ -95,21 +95,24 @@
                         f"via top_level.txt: {import_names} ⭐️"
                     )
                     return True
         logger.debug(f"[{dep_info.name}] did not find top_level.txt in venv")
         return False
 
     def map_dep_to_import_via_record_file(self, dep_info: DependencyInfo) -> bool:
-        dep_name = self.canonicalize_module_name(dep_info.name)
+        dep_name_canonicalized = self.canonicalize_module_name(dep_info.name)
 
         for record_filepath in self.record_filepaths:
             normalized_record_filepath = record_filepath.as_posix()
             matches = self.record_pattern.findall(normalized_record_filepath)
             for import_name_from_record in matches:
-                if import_name_from_record.lower() == dep_name.lower():
+                if (
+                    import_name_from_record.lower() == dep_name_canonicalized.lower()
+                    or import_name_from_record.lower() == dep_info.name.lower()
+                ):
                     with open(record_filepath, "r", encoding="utf-8") as infile:
                         lines = infile.readlines()
 
                     import_names_found = []
                     for line in lines:
                         candidate, _hash, _size = line.split(",")
                         if candidate.endswith(".py") and "__init__" in candidate:
```

## Comparing `creosote-3.0.0.dist-info/METADATA` & `creosote-3.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: creosote
-Version: 3.0.0
+Version: 3.0.1
 Summary: Identify unused dependencies and avoid a bloated virtual environment.
 Project-URL: Source, https://github.com/fredrikaverpil/creosote
 Project-URL: Tracker, https://github.com/fredrikaverpil/creosote/issues
 Author-email: Fredrik Averpil <fredrik.averpil@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -18,18 +18,23 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: dotty-dict<1.4,>=1.3.1
 Requires-Dist: loguru<0.8,>=0.6.0
 Requires-Dist: pip-requirements-parser<33.1,>=32.0.1
 Requires-Dist: toml<0.11,>=0.10.2
 Provides-Extra: dev
-Requires-Dist: creosote[lint,test,types]; extra == 'dev'
+Requires-Dist: coverage; extra == 'dev'
+Requires-Dist: loguru-mypy; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-mock; extra == 'dev'
+Requires-Dist: ruff<0.5,>=0.4.7; extra == 'dev'
+Requires-Dist: types-toml; extra == 'dev'
 Provides-Extra: lint
-Requires-Dist: black; extra == 'lint'
-Requires-Dist: ruff==0.0.290; extra == 'lint'
+Requires-Dist: ruff<0.5,>=0.4.7; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-mock; extra == 'test'
 Provides-Extra: types
 Requires-Dist: loguru-mypy; extra == 'types'
 Requires-Dist: mypy; extra == 'types'
@@ -270,11 +275,20 @@
 
 # Creosote build from PR #123
 $ pipx install --suffix=@123 --force git+https://github.com/fredrikaverpil/creosote.git@refs/pull/123/head
 $ creosote@123 --venv .venv ...
 $ pipx uninstall creosote@123
 ```
 
+You can also clone down the repo and run creosote from the git repo:
+
+```bash
+$ python -m venv .venv
+$ source .venv/bin/activate  # linux/macOS syntax
+$ pip install -e '.[dev]'  # install the dependencies group 'dev'
+$ creosote -venv .venv ...
+```
+
 ### 🚀 Releasing
 
 1. Bump version in `src/creosote/__about__.py` and `.pre-commit-config.yaml`.
 2. GitHub Action will run automatically on creating [a release](https://github.com/fredrikaverpil/creosote/releases) and deploy the release onto PyPi.
```

## Comparing `creosote-3.0.0.dist-info/licenses/LICENSE` & `creosote-3.0.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `creosote-3.0.0.dist-info/RECORD` & `creosote-3.0.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-creosote/__about__.py,sha256=EPmgXOdWKks5S__ZMH7Nu6xpAeVrZpfxaFy4pykuyeI,22
+creosote/__about__.py,sha256=E3P6AbnCwaWk6ndR1zNqlOTVebX9z5rv9voltc71dos,22
 creosote/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 creosote/__main__.py,sha256=jLAVZ1gLnCRXjnsiGtjeaIPvlni7xCpM5PHp95P4uFw,72
 creosote/cli.py,sha256=8yFpz5ktUfTDEfY5JaE13Zn3vPHxlnysp9FJF4Dd5PM,2015
-creosote/config.py,sha256=w0SDPkSCIUIVUPEdowWL5fciXQuM2NXuqvWcwljICtY,5703
+creosote/config.py,sha256=dkTgB06GGChJN2EMF-2KfR9_Exh15qpXdo_G2smkEbU,5689
 creosote/formatters.py,sha256=KaQhieJcUynXI7p24sbO4c08CaBzl_PfV_OyPF9tgOk,1109
 creosote/models.py,sha256=zwLjGtrHDjyRBHi3HLylmxrlUssEYuzoFNsx4trkexQ,523
 creosote/parsers.py,sha256=hWuFA7j-6CdZPz8ZG7_ap8nRsKmd96N3Slh89CCugXQ,9523
-creosote/resolvers.py,sha256=mthlHJAiM5YtWslFCXi780rIqhojT4V8QaXGYFSWCUE,9397
-creosote-3.0.0.dist-info/METADATA,sha256=K5nu6hHH_tcDeNndsgLArukvMZDzhrz7VDtk3l4ulfU,14683
-creosote-3.0.0.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-creosote-3.0.0.dist-info/entry_points.txt,sha256=1WdMKnsMdlsTqCkVmpuvYDayaGWihV0Yf5qJJOa1u1o,47
-creosote-3.0.0.dist-info/licenses/LICENSE,sha256=_hQiru1DnmKFV7ndyrHSYBPcq9g5dMUxzxRqfvyxyvQ,1072
-creosote-3.0.0.dist-info/RECORD,,
+creosote/resolvers.py,sha256=TclKhF-mj5uYX__DhafDKFlmEV9amYrLFVLAu8fC53c,9549
+creosote-3.0.1.dist-info/METADATA,sha256=m3g9T49oM4QRBu0szA7UhWCWF_BaaQSJmuoltqmvIIM,15130
+creosote-3.0.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+creosote-3.0.1.dist-info/entry_points.txt,sha256=1WdMKnsMdlsTqCkVmpuvYDayaGWihV0Yf5qJJOa1u1o,47
+creosote-3.0.1.dist-info/licenses/LICENSE,sha256=_hQiru1DnmKFV7ndyrHSYBPcq9g5dMUxzxRqfvyxyvQ,1072
+creosote-3.0.1.dist-info/RECORD,,
```

