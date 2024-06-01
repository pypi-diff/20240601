# Comparing `tmp/custom_json_diff-0.4.0.tar.gz` & `tmp/custom_json_diff-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_json_diff-0.4.0.tar", last modified: Fri May 24 05:32:16 2024, max compression
+gzip compressed data, was "custom_json_diff-0.5.0.tar", last modified: Sat Jun  1 06:45:02 2024, max compression
```

## Comparing `custom_json_diff-0.4.0.tar` & `custom_json_diff-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:32:16.687142 custom_json_diff-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 05:32:12.000000 custom_json_diff-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-24 05:32:16.687142 custom_json_diff-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-24 05:32:12.000000 custom_json_diff-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:32:16.687142 custom_json_diff-0.4.0/custom_json_diff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 05:32:12.000000 custom_json_diff-0.4.0/custom_json_diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-24 05:32:12.000000 custom_json_diff-0.4.0/custom_json_diff/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-05-24 05:32:12.000000 custom_json_diff-0.4.0/custom_json_diff/custom_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:32:16.687142 custom_json_diff-0.4.0/custom_json_diff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-24 05:32:16.000000 custom_json_diff-0.4.0/custom_json_diff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-24 05:32:16.000000 custom_json_diff-0.4.0/custom_json_diff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 05:32:16.000000 custom_json_diff-0.4.0/custom_json_diff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 05:32:16.000000 custom_json_diff-0.4.0/custom_json_diff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 05:32:16.000000 custom_json_diff-0.4.0/custom_json_diff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 05:32:16.000000 custom_json_diff-0.4.0/custom_json_diff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-24 05:32:12.000000 custom_json_diff-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 05:32:16.687142 custom_json_diff-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:32:16.687142 custom_json_diff-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)   255317 2024-05-24 05:32:12.000000 custom_json_diff-0.4.0/test/test_custom_json_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/custom_json_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/custom_json_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/custom_json_diff/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/custom_json_diff/custom_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/custom_json_diff/custom_diff_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/custom_json_diff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-01 06:45:02.000000 custom_json_diff-0.5.0/custom_json_diff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:02.021921 custom_json_diff-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/test/test_bom_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 06:44:53.000000 custom_json_diff-0.5.0/test/test_custom_json_diff.py
```

### Comparing `custom_json_diff-0.4.0/LICENSE` & `custom_json_diff-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_json_diff-0.4.0/PKG-INFO` & `custom_json_diff-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-json-diff
-Version: 0.4.0
+Version: 0.5.0
 Summary: Custom JSON diffing and comparison tool.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/custom-json-diff
 Project-URL: Bug Tracker, https://github.com/appthreat/custom-json-diff/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,14 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: json-flatten>=0.3
+Requires-Dist: semver>=3.0.0
 Requires-Dist: toml>=0.10
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # custom-json-diff
 
@@ -33,27 +34,30 @@
 
 
 ## Installation
 `pip install custom-json-diff`
 
 ## CLI Usage
 ```
-usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen})
+usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] [-b] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended})
 
 options:
   -h, --help            show this help message and exit
   -i INPUT INPUT, --input INPUT INPUT
-                        Two JSON files to compare
+                        Two JSON files to compare.
   -o OUTPUT, --output OUTPUT
-                        Export JSON of differences to this file
+                        Export JSON of differences to this file.
+  -a, --allow-new-versions
+                        Allow new versions in BOM comparison.
+  -b, --bom-diff        Produce a comparison of CycloneDX BOMs.
   -c CONFIG, --config-file CONFIG
-                        Import TOML configuration file
+                        Import TOML configuration file.
   -x EXCLUDE [EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...]
-                        Exclude field(s) from comparison
-  -p {cdxgen}, --preset {cdxgen}
+                        Exclude field(s) from comparison.
+  -p {cdxgen,cdxgen-extended}, --preset {cdxgen,cdxgen-extended}
                         Preset to use
 
 ```
 
 ## Specifying fields to exclude
 
 To exclude fields from comparison, use the `-x` or `--exclude` flag and specify the field name(s) 
@@ -79,25 +83,27 @@
     "field1.field3.[0].b": "val2",
     "field1.field3.[1].a": "val3",
     "field1.field3.[1].b": "val4"
 }
 ```
 
 To exclude field2, you would specify `field1.field2`. To exclude the `a` field in the array of 
-objects, you would specify `field1.field3.[].a`. custom-json-diff will create a regex which will 
-account for the array index in the field name. Multiple fields may be specified separated by a 
-space. To better understand what your fields should be, check out json-flatten, which is the 
-package used for this function.
+objects, you would specify `field1.field3.[].a` (do NOT include the array index, just do `[]`). 
+Multiple fields may be specified separated by a space. To better understand what your fields should
+be, check out json-flatten, which is the package used for this function.
 
 ## Sorting
 
 custom-json-diff will sort the imported JSON alphabetically. If your JSON document contains arrays 
 of objects, you will need to specify any keys you want to sort by in a toml file or use a preset.
 The first key located from the provided keys that is present in the object will be used for sorting.
 
 ## TOML config file example
 
 ```toml
 [settings]
 excluded_fields = ["serialNumber", "metadata.timestamp"]
 sort_keys = ["url", "content", "ref", "name", "value"]
+
+[bom_diff]
+allow_new_versions = false
 ```
```

### Comparing `custom_json_diff-0.4.0/README.md` & `custom_json_diff-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 
 
 ## Installation
 `pip install custom-json-diff`
 
 ## CLI Usage
 ```
-usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen})
+usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] [-b] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended})
 
 options:
   -h, --help            show this help message and exit
   -i INPUT INPUT, --input INPUT INPUT
-                        Two JSON files to compare
+                        Two JSON files to compare.
   -o OUTPUT, --output OUTPUT
-                        Export JSON of differences to this file
+                        Export JSON of differences to this file.
+  -a, --allow-new-versions
+                        Allow new versions in BOM comparison.
+  -b, --bom-diff        Produce a comparison of CycloneDX BOMs.
   -c CONFIG, --config-file CONFIG
-                        Import TOML configuration file
+                        Import TOML configuration file.
   -x EXCLUDE [EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...]
-                        Exclude field(s) from comparison
-  -p {cdxgen}, --preset {cdxgen}
+                        Exclude field(s) from comparison.
+  -p {cdxgen,cdxgen-extended}, --preset {cdxgen,cdxgen-extended}
                         Preset to use
 
 ```
 
 ## Specifying fields to exclude
 
 To exclude fields from comparison, use the `-x` or `--exclude` flag and specify the field name(s) 
@@ -54,25 +57,27 @@
     "field1.field3.[0].b": "val2",
     "field1.field3.[1].a": "val3",
     "field1.field3.[1].b": "val4"
 }
 ```
 
 To exclude field2, you would specify `field1.field2`. To exclude the `a` field in the array of 
-objects, you would specify `field1.field3.[].a`. custom-json-diff will create a regex which will 
-account for the array index in the field name. Multiple fields may be specified separated by a 
-space. To better understand what your fields should be, check out json-flatten, which is the 
-package used for this function.
+objects, you would specify `field1.field3.[].a` (do NOT include the array index, just do `[]`). 
+Multiple fields may be specified separated by a space. To better understand what your fields should
+be, check out json-flatten, which is the package used for this function.
 
 ## Sorting
 
 custom-json-diff will sort the imported JSON alphabetically. If your JSON document contains arrays 
 of objects, you will need to specify any keys you want to sort by in a toml file or use a preset.
 The first key located from the provided keys that is present in the object will be used for sorting.
 
 ## TOML config file example
 
 ```toml
 [settings]
 excluded_fields = ["serialNumber", "metadata.timestamp"]
 sort_keys = ["url", "content", "ref", "name", "value"]
+
+[bom_diff]
+allow_new_versions = false
 ```
```

### Comparing `custom_json_diff-0.4.0/custom_json_diff/cli.py` & `custom_json_diff-0.5.0/custom_json_diff/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import argparse
 
 from custom_json_diff.custom_diff import (
-    compare_dicts,
-    get_common,
-    get_diffs,
-    perform_bom_diff,
-    report_results
+    compare_dicts, get_diff, perform_bom_diff, report_results
 )
 
 
 def build_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-i",
@@ -23,20 +19,21 @@
     parser.add_argument(
         "-o",
         "--output",
         action="store",
         help="Export JSON of differences to this file.",
         dest="output",
     )
-    # parser.add_argument(
-    #     "--common",
-    #      action="store_true",
-    #      help="Include common elements as well as differences",
-    #      dest="common",
-    # )
+    parser.add_argument(
+        "-a",
+        "--allow-new-versions",
+        action="store_true",
+        help="Allow new versions in BOM comparison.",
+        dest="allow_new_versions",
+    )
     parser.add_argument(
         "-b",
         "--bom-diff",
          action="store_true",
          help="Produce a comparison of CycloneDX BOMs.",
          dest="bom_diff",
     )
@@ -66,18 +63,19 @@
         dest="preset",
     )
     return parser.parse_args()
 
 
 def main():
     args = build_args()
-    result, j1, j2 = compare_dicts(args.input[0], args.input[1], args.preset, args.exclude, args.config)
-    diffs = get_diffs(args.input[0], args.input[1], j1, j2)
+    settings = args.preset or args.config or args.exclude
+    result, j1, j2 = compare_dicts(args.input[0], args.input[1], settings, args.bom_diff, args.allow_new_versions)
+
     if args.bom_diff:
-        common = get_common(j1, j2)
-        perform_bom_diff(result, diffs, common, args.input[0], args.input[1], args.output)
+        result_summary = perform_bom_diff(j1, j2)
     else:
-        report_results(result, diffs, args.output)
+        result_summary = get_diff(args.input[0], args.input[1], j1, j2)
+    report_results(result, result_summary, args.output)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `custom_json_diff-0.4.0/custom_json_diff/custom_diff.py` & `custom_json_diff-0.5.0/custom_json_diff/custom_diff_classes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,107 @@
-import json
-import logging
+import contextlib
 import re
-import sys
-from pathlib import Path
 from typing import Dict, List, Set, Tuple
 
-import toml
-from json_flatten import flatten, unflatten  # type: ignore
+import semver
+from json_flatten import unflatten  # type: ignore
 
 
-DELIM = "|>"
+class BomComponent:
+    def __init__(self, comp: Dict, allow_new_versions: bool, component_type: str):
+        self.version = set_version(comp.get("version", ""), allow_new_versions)
+        self.search_key = create_comp_key(comp, allow_new_versions, component_type)
+        self.allow_new_versions = allow_new_versions
+        self.original_data = comp
+        self.component_type = comp.get("type", "")
 
+    def __eq__(self, other):
+        if self.allow_new_versions:
+            return self.search_key == other.search_key and self.version >= other.version
+        else:
+            return self.search_key == other.search_key
+
+    def __ne__(self, other):
+        return not self == other
 
-class FlatDicts:
-    def __init__(self, elements):
-        self.data, self.search_keys = import_flat_dict(elements)
+
+class BomDependency:
+    def __init__(self, dep: Dict, allow_new_versions: bool):
+        self.ref, self.deps = import_bom_dependency(dep, allow_new_versions)
+        self.original_data = dep
 
     def __eq__(self, other):
-        return all(i in other.data for i in self.data)
+        return self.ref == other.ref and self.deps == other.deps
 
     def __ne__(self, other):
         return not self == other
 
+
+class BomDicts:
+    def __init__(self, allow_new_versions: bool, filename: str, data: Dict | None = None,
+                 metadata: Dict | None = None, components: List | None = None,
+                 services: List | None = None, dependencies: List | None = None):
+        self.data, self.components, self.services, self.dependencies = import_bom_dict(
+            allow_new_versions, data, metadata, components, services, dependencies)
+        self.filename = filename
+        self.allow_new_versions = allow_new_versions
+
+    def __eq__(self, other):
+        return (self.data == other.data and self.components == other.components and
+                self.services == other.services)
+
+    def __ne__(self, other):
+        return not self == other
+
+
+class FlatDicts:
+
+    def __init__(self, elements: Dict | List):
+        self.data = import_flat_dict(elements)
+
+    def __eq__(self, other) -> bool:
+        return all(i in other.data for i in self.data) and all(i in self.data for i in other.data)
+
+    def __ne__(self, other) -> bool:
+        return not self == other
+
+    def __iadd__(self, other):
+        to_add = [i for i in other.data if i not in self.data]
+        self.data.extend(to_add)
+        return self
+
+    def __isub__(self, other):
+        kept_items = [i for i in self.data if i not in other.data]
+        self.data = kept_items
+        return self
+
+    def __add__(self, other):
+        to_add = self.data
+        for i in other.data:
+            if i not in self.data:
+                to_add.append(i)
+        return FlatDicts(to_add)
+
     def __sub__(self, other):
-        missing = [i for i in self.data if i not in other.data]
-        return {i.key: i.value for i in missing}
-        # new_flat_dict = {}
-        # for i in missing:
-        #     for j in self.data:
-        #         if i == j.search_key:
-        #             new_flat_dict[j.key] = j.value
-        # return new_flat_dict
+        to_add = [i for i in self.data if i not in other.data]
+        return FlatDicts(to_add)
 
-    def to_dict(self, unflat: bool = False):
+    def to_dict(self, unflat: bool = False) -> Dict:
         result = {i.key: i.value for i in self.data}
         if unflat:
             result = unflatten(result)
         return result
 
-    def intersection(self, other):
-        intersection = {}
-        for i in self.data:
-            if i.search_key in other.search_keys:
-                intersection[i.key] = i.value
-        return intersection
-
-    def filter_out_keys(self, exclude_keys):
-        filtered_data = []
-        for i in self.data:
-            if check_key(i.search_key, exclude_keys):
-                filtered_data.append(i)
+    def intersection(self, other: "FlatDicts") -> "FlatDicts":
+        """Returns the intersection of two FlatDicts as a new FlatDicts"""
+        intersection = [i for i in self.data if i in other.data]
+        return FlatDicts(intersection)
+
+    def filter_out_keys(self, exclude_keys: Set[str]) -> "FlatDicts":
+        filtered_data = [i for i in self.data if check_key(i.search_key, exclude_keys)]
         self.data = filtered_data
         return self
 
 
 class FlatElement:
     def __init__(self, key, value):
         self.key = key
@@ -64,179 +112,78 @@
         return self.search_key == other.search_key
 
 
 def check_key(key: str, exclude_keys: Set[str]) -> bool:
     return not any(key.startswith(k) for k in exclude_keys)
 
 
-def check_regex(regex_keys: Set[re.Pattern], key: str) -> bool:
-    return any(regex.match(key) for regex in regex_keys)
-
-
-def compare_dicts(
-        json1: str, json2: str, preset: str | None = None,
-        excluded: List[str] | None = None, config: str | None = None
-) -> Tuple[int, FlatDicts, FlatDicts]:
-    if preset:
-        exclude_keys, sort_keys = set_excluded_fields(preset)
-    elif config:
-        exclude_keys, sort_keys = import_toml(config)
-    else:
-        exclude_keys, sort_keys = set(excluded), []  # type: ignore
-    json_1_data = load_json(json1, exclude_keys, sort_keys)
-    json_2_data = load_json(json2, exclude_keys, sort_keys)
-    if json_1_data.data == json_2_data.data:
-        return 0, json_1_data, json_2_data
-    else:
-        return 1, json_1_data, json_2_data
-
-
 def create_search_key(key: str, value: str) -> str:
     combined_key = re.sub(r"(?<=\[)[0-9]+(?=])", "", key)
     combined_key += f"|>{value}"
     return combined_key
 
 
-def export_results(outfile: str, diffs: Dict) -> None:
-    with open(outfile, "w", encoding="utf-8") as f:
-        f.write(json.dumps(diffs, indent=2))
-
-
-def filter_dict(data: Dict, exclude_keys: Set[str], sort_keys: List[str]) -> FlatDicts:
-    data = flatten(sort_dict(data, sort_keys))
-    return FlatDicts(data).filter_out_keys(exclude_keys)
-
-
-def filter_simple(flattened_data: Dict, exclude_keys: Set[str]) -> Dict:
-    return {
-        key: value
-        for key, value in flattened_data.items()
-        if check_key(key, exclude_keys)
-    }
-
-
-def get_common(json_1_data: FlatDicts, json_2_data: FlatDicts) -> Dict:
-    return unflatten(json_1_data.intersection(json_2_data))
-
-
-def get_diffs(f1: str | Path, f2: str | Path, j1: FlatDicts, j2: FlatDicts) -> Dict:
-    diff_1 = unflatten(j1 - j2)
-    diff_2 = unflatten(j2 - j1)
-    return {str(f1): diff_1, str(f2): diff_2}
-
-
-def get_sort_key(data: Dict, sort_keys: List[str]) -> str | bool:
-    return next((i for i in sort_keys if i in data), False)
-
-
-def handle_results(outfile: str, diffs: Dict) -> None:
-    if outfile:
-        export_results(outfile, diffs)
-    else:
-        print("Differences found:")
-        print(json.dumps(diffs, indent=2))
-
-
-def import_flat_dict(my_dict: Dict) -> Tuple[List[FlatElement], Set[str]]:
-    searchable = []
-    search_keys = set()
-    for key, value in my_dict.items():
+def create_comp_key(comp: Dict, allow_new_versions: bool, component_type: str) -> str:
+    if allow_new_versions:
+        if component_type == "components":
+            return f"{comp.get('name', '')}|{comp.get('type', '')}|{comp.get('group', '')}|{comp.get('publisher', '')}"
+        return f"{comp.get('name', '')}|{comp.get('group', '')}"
+    if component_type == "components":
+        return f"{comp.get('bom-ref', '')}|{comp.get('name', '')}|{comp.get('purl', '')}|{comp.get('type', '')}|{comp.get('group', '')}|{comp.get('version', '')}|{comp.get('publisher', '')}"
+    return f"{comp.get('bom-ref', '')}|{comp.get('name', '')}|{comp.get('group', '')}|{comp.get('version', '')}"
+
+
+def import_bom_dependency(data: Dict, allow_new_versions: bool):
+    ref = data.get("ref", "")
+    deps = data.get("dependencies", [])
+    if allow_new_versions:
+        ref = ref.split("@")[0]
+        deps = [i.split("@")[0] for i in deps]
+    return ref, set(deps)
+
+
+def import_bom_dict(
+        allow_new_versions: bool, data: Dict | None = None, metadata: Dict | None = None,
+        components: List | None = None, services: List | None = None,
+        dependencies: List | None = None) -> Tuple[FlatDicts, List, List, List]:
+    if data:
+        metadata, components, services, dependencies = parse_bom_dict(data, allow_new_versions)
+    return FlatDicts(metadata), components, services, dependencies  # type: ignore
+
+
+def import_flat_dict(data: Dict | List) -> List[FlatElement]:
+    if isinstance(data, list):
+        return data
+    flat_dicts = []
+    for key, value in data.items():
         ele = FlatElement(key, value)
-        searchable.append(ele)
-        search_keys.add(ele.search_key)
-    return searchable, search_keys
-
-
-def import_toml(toml_file_path: str) -> Tuple[Set[str], List[str]]:
-    with open(toml_file_path, "r", encoding="utf-8") as f:
-        try:
-            toml_data = toml.load(f)
-        except toml.TomlDecodeError:
-            logging.error("Invalid TOML.")
-            sys.exit(1)
-    try:
-        return toml_data["settings"]["excluded_fields"], toml_data["settings"]["sort_keys"]
-    except KeyError:
-        logging.error("Invalid TOML.")
-        sys.exit(1)
-
-
-def load_json(json_file: str, exclude_keys: Set[str], sort_keys: List[str]) -> FlatDicts:
-    try:
-        with open(json_file, "r", encoding="utf-8") as f:
-            data = json.load(f)
-    except FileNotFoundError:
-        logging.error("File not found: %s", json_file)
-        sys.exit(1)
-    except json.JSONDecodeError:
-        logging.error("Invalid JSON: %s", json_file)
-        sys.exit(1)
-    return filter_dict(data, exclude_keys, sort_keys)
-
-
-def perform_bom_diff(status: int, diff: Dict, commons: Dict, f1: str, f2: str, outfile: str):
-    diff_elements = produce_bom_diff(diff, commons, f1, f2)
-    handle_results(outfile, diff_elements)
-
-
-def populate_bom_diff(diff: Dict) -> Dict:
-    if not diff:
-        return {"components": [], "services": []}
-    return {
-            "components": [i.get("purl") for i in diff.get("components", []) if i.get("purl")],
-            "services": [i.get("bom-ref") for i in diff.get("services", []) if i.get("bom-ref")],
-    }
-
-
-def produce_bom_diff(diff: Dict, common: Dict, f1: str, f2: str) -> Dict:
-    diff_summary = {f1: populate_bom_diff(diff.get(f1, {})), f2: populate_bom_diff(diff.get(f2, {}))}
-    if common:
-        diff_summary["common"] = populate_bom_diff(common)
-    return diff_summary
-
-
-def report_results(status: int, diffs: Dict, outfile: str):
-    if status == 0:
-        print("No differences found.")
-    else:
-        handle_results(outfile, diffs)
-
-
-def set_excluded_fields(preset: str) -> Tuple[Set[str], List[str]]:
-    excluded = []
-    sort_fields = []
-    if preset.startswith("cdxgen"):
-        excluded.extend(["metadata.timestamp", "serialNumber",
-                         "metadata.tools.components.[].version",
-                         "metadata.tools.components.[].purl",
-                         "metadata.tools.components.[].bom-ref",
-                         "components.[].properties",
-                         "components.[].evidence"
-                         ])
-        if preset == "cdxgen-extended":
-            excluded.append("components.[].licenses")
-        sort_fields.extend(["url", "content", "ref", "name", "value"])
-    return set(excluded), sort_fields
-
-
-def sort_dict(result: Dict, sort_keys: List[str]) -> Dict:
-    """Sorts a dictionary"""
-    for k, v in result.items():
-        if isinstance(v, dict):
-            result[k] = sort_dict(v, sort_keys)
-        elif isinstance(v, list) and len(v) >= 2:
-            result[k] = sort_list(v, sort_keys)
-        else:
-            result[k] = v
-    return result
+        flat_dicts.append(ele)
+    return flat_dicts
 
 
-def sort_list(lst: List, sort_keys: List[str]) -> List:
-    """Sorts a list"""
-    if isinstance(lst[0], dict):
-        if sort_key := get_sort_key(lst[0], sort_keys):
-            return sorted(lst, key=lambda x: x[sort_key])
-        logging.debug("No key(s) specified for sorting. Cannot sort list of dictionaries.")
-        return lst
-    if isinstance(lst[0], (str, int)):
-        lst.sort()
-    return lst
+def parse_bom_dict(data: Dict, allow_new_versions: bool):
+    metadata = []
+    components = []
+    services = []
+    dependencies = []
+    for key, value in data.items():
+        if key not in {"components", "dependencies", "services"}:
+            ele = FlatElement(key, value)
+            metadata.append(ele)
+            continue
+        if key == "components":
+            for i in value:
+                components.append(BomComponent(i, allow_new_versions, "component"))
+        elif key == "services":
+            for i in value:
+                services.append(BomComponent(i, allow_new_versions, "service"))
+        elif key == "dependencies":
+            for i in value:
+                dependencies.append(BomDependency(i, allow_new_versions, ))
+    return metadata, components, services, dependencies
+
+
+def set_version(version: str, allow_new_versions: bool = False) -> semver.Version | str:
+    with contextlib.suppress(ValueError):
+        if allow_new_versions and version:
+            return semver.Version.parse(version, True)
+    return version
```

### Comparing `custom_json_diff-0.4.0/custom_json_diff.egg-info/PKG-INFO` & `custom_json_diff-0.5.0/custom_json_diff.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-json-diff
-Version: 0.4.0
+Version: 0.5.0
 Summary: Custom JSON diffing and comparison tool.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/custom-json-diff
 Project-URL: Bug Tracker, https://github.com/appthreat/custom-json-diff/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,14 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: json-flatten>=0.3
+Requires-Dist: semver>=3.0.0
 Requires-Dist: toml>=0.10
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # custom-json-diff
 
@@ -33,27 +34,30 @@
 
 
 ## Installation
 `pip install custom-json-diff`
 
 ## CLI Usage
 ```
-usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen})
+usage: cjd [-h] -i INPUT INPUT [-o OUTPUT] [-b] (-c CONFIG | -x EXCLUDE [EXCLUDE ...] | -p {cdxgen,cdxgen-extended})
 
 options:
   -h, --help            show this help message and exit
   -i INPUT INPUT, --input INPUT INPUT
-                        Two JSON files to compare
+                        Two JSON files to compare.
   -o OUTPUT, --output OUTPUT
-                        Export JSON of differences to this file
+                        Export JSON of differences to this file.
+  -a, --allow-new-versions
+                        Allow new versions in BOM comparison.
+  -b, --bom-diff        Produce a comparison of CycloneDX BOMs.
   -c CONFIG, --config-file CONFIG
-                        Import TOML configuration file
+                        Import TOML configuration file.
   -x EXCLUDE [EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...]
-                        Exclude field(s) from comparison
-  -p {cdxgen}, --preset {cdxgen}
+                        Exclude field(s) from comparison.
+  -p {cdxgen,cdxgen-extended}, --preset {cdxgen,cdxgen-extended}
                         Preset to use
 
 ```
 
 ## Specifying fields to exclude
 
 To exclude fields from comparison, use the `-x` or `--exclude` flag and specify the field name(s) 
@@ -79,25 +83,27 @@
     "field1.field3.[0].b": "val2",
     "field1.field3.[1].a": "val3",
     "field1.field3.[1].b": "val4"
 }
 ```
 
 To exclude field2, you would specify `field1.field2`. To exclude the `a` field in the array of 
-objects, you would specify `field1.field3.[].a`. custom-json-diff will create a regex which will 
-account for the array index in the field name. Multiple fields may be specified separated by a 
-space. To better understand what your fields should be, check out json-flatten, which is the 
-package used for this function.
+objects, you would specify `field1.field3.[].a` (do NOT include the array index, just do `[]`). 
+Multiple fields may be specified separated by a space. To better understand what your fields should
+be, check out json-flatten, which is the package used for this function.
 
 ## Sorting
 
 custom-json-diff will sort the imported JSON alphabetically. If your JSON document contains arrays 
 of objects, you will need to specify any keys you want to sort by in a toml file or use a preset.
 The first key located from the provided keys that is present in the object will be used for sorting.
 
 ## TOML config file example
 
 ```toml
 [settings]
 excluded_fields = ["serialNumber", "metadata.timestamp"]
 sort_keys = ["url", "content", "ref", "name", "value"]
+
+[bom_diff]
+allow_new_versions = false
 ```
```

### Comparing `custom_json_diff-0.4.0/pyproject.toml` & `custom_json_diff-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "custom-json-diff"
-version = "0.4.0"
+version = "0.5.0"
 description = "Custom JSON diffing and comparison tool."
 authors = [
   { name = "Caroline Russell", email = "caroline@appthreat.dev" },
 ]
-dependencies = ["json-flatten>=0.3", "toml>=0.10"]
+dependencies = ["json-flatten>=0.3", "semver >= 3.0.0", "toml>=0.10"]
 license = { text = "Apache-2.0" }
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
```

