# Comparing `tmp/pytest_topo-0.0.4.tar.gz` & `tmp/pytest_topo-1.0.0.tar.gz`

## Comparing `pytest_topo-0.0.4.tar` & `pytest_topo-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/DEVNOTES.md
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/src/pytest_topo/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/src/pytest_topo/plugin.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/src/pytest_topo/topo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/test_extendable.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/test_ordering.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/tests/test_skipping.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/LICENSE
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/README.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pytest_topo-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/DEVNOTES.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/src/pytest_topo/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/src/pytest_topo/plugin.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/src/pytest_topo/topo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/tests/test_extendable.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/tests/test_ordering.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/tests/test_skipping.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/README.md
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pytest_topo-1.0.0/PKG-INFO
```

### Comparing `pytest_topo-0.0.4/.github/workflows/deploy.yml` & `pytest_topo-1.0.0/.github/workflows/deploy.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,72 @@
-name: Publish package
-
-on: 
-  push:
-    branches:
-      - main
-
-jobs:
-  test:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-
-      - name: Set up Python
-        uses: actions/setup-python@v5
-        with:
-          python-version: "3.11"
-
-      - name: Install dependencies
-        run: pip install .[test]
-
-      - name: Check linter
-        run: ruff check
-
-      - name: Run tests
-        run: pytest
-
-  build:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-
-      - name: Set up Python
-        uses: actions/setup-python@v5
-        with:
-          python-version: "3.11"
-
-      - name: Install dependencies
-        run: pip install --upgrade build
-      
-      - name: Build package
-        run: python -m build
-
-      - name: Store package
-        uses: actions/upload-artifact@v4
-        with:
-          name: package
-          path: dist/
-
-  publish:
-    runs-on: ubuntu-latest
-    needs: [build, test]
-    permissions:
-      id-token: write
-    steps:
-      - uses: actions/download-artifact@v4
-        with:
-          name: package
-          path: dist/
-
-      - name: Publish package to TestPyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          repository-url: https://test.pypi.org/legacy/
+name: Publish package
+
+on: 
+  push:
+    branches:
+      - main
+
+jobs:
+  test:
+    runs-on: ubuntu-latest
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
+    steps:
+      - uses: actions/checkout@v4
+
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Install dependencies
+        run: pip install .[test]
+
+      - name: Check linter
+        run: ruff check
+
+      - name: Run tests
+        run: pytest
+
+  build:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.12"
+
+      - name: Install dependencies
+        run: pip install --upgrade build
+      
+      - name: Build package
+        run: python -m build
+
+      - name: Store package
+        uses: actions/upload-artifact@v4
+        with:
+          name: package
+          path: dist/
+
+  publish:
+    runs-on: ubuntu-latest
+    needs: [build, test]
+    permissions:
+      id-token: write
+    steps:
+      - uses: actions/download-artifact@v4
+        with:
+          name: package
+          path: dist/
+
+      - name: Publish package to TestPyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          repository-url: https://test.pypi.org/legacy/
+
+      - name: Publish package to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+
```

### Comparing `pytest_topo-0.0.4/src/pytest_topo/topo.py` & `pytest_topo-1.0.0/src/pytest_topo/topo.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from typing import Dict, List
-
-from pytest import Item
-
-failures = set()
-func_name_map = {}
-
-
-def order_by_dependency(items: List[Item]) -> None:
-    for item in items:
-        mark = item.get_closest_marker("dependency")
-        if not mark:
-            continue
-        for name in mark.args:
-            assert name not in func_name_map, f"Duplicate dependency name found: {name}"
-            func_name_map[name] = item.nodeid
-
-    dependencies = {}
-    for item in items:
-        dependencies[item.nodeid] = []
-        mark = item.get_closest_marker("depends_on")
-        if not mark:
-            continue
-        for dep in mark.args:
-            func_name = func_name_map[dep]
-            dependencies[item.nodeid].append(func_name)
-
-    new_order = list(topological_sort(dependencies))
-
-    new_items = []
-    for func_name in new_order:
-        new_items.extend([item for item in items if item.nodeid == func_name])
-
-    items[:] = new_items
-
-
-def topological_sort(source: Dict[str, List[Item]]):
-    # This is blatantly stolen from stack overflow
-    # copy deps so we can modify set in-place
-    pending = [(name, set(deps)) for name, deps in source.items()]
-    emitted = []
-    while pending:
-        next_pending = []
-        next_emitted = []
-        for entry in pending:
-            name, deps = entry
-            deps.difference_update(emitted)  # remove deps we emitted last pass
-            # still has deps? recheck during next pass
-            if deps:
-                next_pending.append(entry)
-            else:
-                yield name
-                # not required, but helps preserve original ordering
-                emitted.append(name)
-                # remember what we emitted for difference_update() in next pass
-                next_emitted.append(name)
-
-        # all entries have unmet deps, one of two things is wrong...
-        if not next_emitted:
-            raise ValueError(f"cyclic or missing dependancy detected: {next_pending!r}")
-        pending = next_pending
-        emitted = next_emitted
-
-
-def mark_as_failure(item: Item):
-    failures.add(item.nodeid)
-
-
-def should_skip(item: Item) -> bool:
-    mark = item.get_closest_marker("depends_on")
-    if not mark:
-        return False
-    for name in mark.args:
-        func_name = func_name_map[name]
-        if func_name in failures:
-            return True
-    return False
+from typing import Dict, List
+
+from pytest import Item
+
+failures = set()
+func_name_map = {}
+
+
+def order_by_dependency(items: List[Item]) -> None:
+    for item in items:
+        mark = item.get_closest_marker("dependency")
+        if not mark:
+            continue
+        for name in mark.args:
+            assert name not in func_name_map, f"Duplicate dependency name found: {name}"
+            func_name_map[name] = item.nodeid
+
+    dependencies = {}
+    for item in items:
+        dependencies[item.nodeid] = []
+        mark = item.get_closest_marker("depends_on")
+        if not mark:
+            continue
+        for dep in mark.args:
+            func_name = func_name_map[dep]
+            dependencies[item.nodeid].append(func_name)
+
+    new_order = list(topological_sort(dependencies))
+
+    new_items = []
+    for func_name in new_order:
+        new_items.extend([item for item in items if item.nodeid == func_name])
+
+    items[:] = new_items
+
+
+def topological_sort(source: Dict[str, List[Item]]):
+    # This is blatantly stolen from stack overflow
+    # copy deps so we can modify set in-place
+    pending = [(name, set(deps)) for name, deps in source.items()]
+    emitted = []
+    while pending:
+        next_pending = []
+        next_emitted = []
+        for entry in pending:
+            name, deps = entry
+            deps.difference_update(emitted)  # remove deps we emitted last pass
+            # still has deps? recheck during next pass
+            if deps:
+                next_pending.append(entry)
+            else:
+                yield name
+                # not required, but helps preserve original ordering
+                emitted.append(name)
+                # remember what we emitted for difference_update() in next pass
+                next_emitted.append(name)
+
+        # all entries have unmet deps, one of two things is wrong...
+        if not next_emitted:
+            raise ValueError(f"cyclic or missing dependancy detected: {next_pending!r}")
+        pending = next_pending
+        emitted = next_emitted
+
+
+def mark_as_failure(item: Item):
+    failures.add(item.nodeid)
+
+
+def should_skip(item: Item) -> bool:
+    mark = item.get_closest_marker("depends_on")
+    if not mark:
+        return False
+    for name in mark.args:
+        func_name = func_name_map[name]
+        if func_name in failures:
+            return True
+    return False
```

### Comparing `pytest_topo-0.0.4/LICENSE` & `pytest_topo-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pytest_topo-0.0.4/README.md` & `pytest_topo-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,78 @@
-## Install
-```bash
-pip install pytest-topo
-```
-The pytest-topo library offers a topological ordering feature for pytest tests, ensuring that dependent tests are run in the correct sequence. This is particularly useful for integration testing libraries that use pytest for orchestration. 
-
-Please note that this library is not recommended for unit tests, as unit tests should ideally be independent of each other.
-
-## Usage Examples
-To sequence your tests, apply the `dependency` and `depends_on` markers.
-
-```python
-import pytest
-
-@pytest.mark.dependency("One")
-def test_one():
-    # This test is executed first
-
-@pytest.mark.depends_on("Two")
-def test_three():
-    # This test is executed third
-
-@pytest.mark.depends_on("One")
-@pytest.mark.dependency("Two")
-def test_two():
-    # This test is executed second
-```
-
-If any of the dependent tests do not pass, they will not be skipped. This will also skip any fixture creation, if there are no remaining tests that need to use them.
-
-```python
-import pytest
-
-@pytest.mark.dependency("DoesntPass")
-def test_one():
-    assert False  # force a failure
-
-@pytest.fixture(scope="function")
-def my_fixture():
-    # This fixture is never created
-
-@pytest.mark.depends_on("DoesntPass")
-def test_two(my_fixture):
-    # This test will be skipped
-
-```
-
-## Motivation
-Consider software where customers register with an `account` API, and submit purchases to a `purchases` API. These are two services with API tests that could look like this:
-
-```
-tests
-  - account
-    - test_create_and_delete
-    - ...
-  - purchases
-    - test_make_purchase
-    - ...
-```
-
-The `purchases` tests may run a pre-test setup to create an account, execute tests, then run a post-test teardown. If there is an issue in the account creation or deletion, all these tests will error. By adding dependency links, the `purchases` tests will be skipped, reducing test failure noise.
+Metadata-Version: 2.3
+Name: pytest-topo
+Version: 1.0.0
+Summary: Topological sorting for pytest
+Project-URL: Homepage, https://github.com/Nick-Sullivan/pytest-topo
+Project-URL: Issues, https://github.com/Nick-Sullivan/pytest-topo/issues
+Author-email: Nick Sullivan <nick.dave.sullivan@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: pytest>=7.0.0
+Provides-Extra: test
+Requires-Dist: ruff>=0.4.6; extra == 'test'
+Description-Content-Type: text/markdown
+
+## Install
+```bash
+pip install pytest-topo
+```
+The pytest-topo library offers a topological ordering feature for pytest tests, ensuring that dependent tests are run in the correct sequence. This is particularly useful for integration testing libraries that use pytest for orchestration. 
+
+Please note that this library is not recommended for unit tests, as unit tests should ideally be independent of each other.
+
+## Usage Examples
+To sequence your tests, apply the `dependency` and `depends_on` markers.
+
+```python
+import pytest
+
+@pytest.mark.dependency("One")
+def test_one():
+    # This test is executed first
+
+@pytest.mark.depends_on("Two")
+def test_three():
+    # This test is executed third
+
+@pytest.mark.depends_on("One")
+@pytest.mark.dependency("Two")
+def test_two():
+    # This test is executed second
+```
+
+If any of the dependent tests do not pass, they will not be skipped. This will also skip any fixture creation, if there are no remaining tests that need to use them.
+
+```python
+import pytest
+
+@pytest.mark.dependency("DoesntPass")
+def test_one():
+    assert False  # force a failure
+
+@pytest.fixture(scope="function")
+def my_fixture():
+    # This fixture is never created
+
+@pytest.mark.depends_on("DoesntPass")
+def test_two(my_fixture):
+    # This test will be skipped
+
+```
+
+## Motivation
+Consider software where customers register with an `account` API, and submit purchases to a `purchases` API. These are two services with API tests that could look like this:
+
+```
+tests
+  - account
+    - test_create_and_delete
+    - ...
+  - purchases
+    - test_make_purchase
+    - ...
+```
+
+The `purchases` tests may run a pre-test setup to create an account, execute tests, then run a post-test teardown. If there is an issue in the account creation or deletion, all these tests will error. By adding dependency links, the `purchases` tests will be skipped, reducing test failure noise.
```

### Comparing `pytest_topo-0.0.4/pyproject.toml` & `pytest_topo-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-[project]
-name = "pytest-topo"
-version = "0.0.4"
-authors = [
-  { name="Nick Sullivan", email="nick.dave.sullivan@gmail.com" },
-]
-description = "Topological sorting for pytest"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "pytest>=8.2.1",
-]
-
-[project.optional-dependencies]
-test = [
-    "ruff==0.4.6",
-]
-
-[project.urls]
-Homepage = "https://github.com/Nick-Sullivan/pytest-topo"
-Issues = "https://github.com/Nick-Sullivan/pytest-topo/issues"
-
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.pytest.ini_options]
-pythonpath = "src"
-markers = [
-    "dependency",
-    "depends_on",
-]
-
-[project.entry-points.pytest11]
-pytest_topo = "pytest_topo.plugin"
-
-[tool.ruff.lint]
-select = [
-    # pycodestyle
-    "E",
-    # Pyflakes
-    "F",
-    # pyupgrade
-    "UP",
-    # flake8-bugbear
-    "B",
-    # flake8-simplify
-    "SIM",
-    # isort
-    "I",
-]
+[project]
+name = "pytest-topo"
+version = "1.0.0"
+authors = [
+  { name="Nick Sullivan", email="nick.dave.sullivan@gmail.com" },
+]
+description = "Topological sorting for pytest"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "pytest>=7.0.0",
+]
+
+[project.optional-dependencies]
+test = [
+    "ruff>=0.4.6",
+]
+
+[project.urls]
+Homepage = "https://github.com/Nick-Sullivan/pytest-topo"
+Issues = "https://github.com/Nick-Sullivan/pytest-topo/issues"
+
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.pytest.ini_options]
+pythonpath = "src"
+markers = [
+    "dependency",
+    "depends_on",
+]
+
+[project.entry-points.pytest11]
+pytest_topo = "pytest_topo.plugin"
+
+[tool.ruff.lint]
+select = [
+    # pycodestyle
+    "E",
+    # Pyflakes
+    "F",
+    # pyupgrade
+    "UP",
+    # flake8-bugbear
+    "B",
+    # flake8-simplify
+    "SIM",
+    # isort
+    "I",
+]
```

### Comparing `pytest_topo-0.0.4/PKG-INFO` & `pytest_topo-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.3
-Name: pytest-topo
-Version: 0.0.4
-Summary: Topological sorting for pytest
-Project-URL: Homepage, https://github.com/Nick-Sullivan/pytest-topo
-Project-URL: Issues, https://github.com/Nick-Sullivan/pytest-topo/issues
-Author-email: Nick Sullivan <nick.dave.sullivan@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: pytest>=8.2.1
-Provides-Extra: test
-Requires-Dist: ruff==0.4.6; extra == 'test'
-Description-Content-Type: text/markdown
-
 ## Install
 ```bash
 pip install pytest-topo
 ```
 The pytest-topo library offers a topological ordering feature for pytest tests, ensuring that dependent tests are run in the correct sequence. This is particularly useful for integration testing libraries that use pytest for orchestration. 
 
 Please note that this library is not recommended for unit tests, as unit tests should ideally be independent of each other.
```

