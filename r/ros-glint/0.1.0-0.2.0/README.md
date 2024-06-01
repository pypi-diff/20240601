# Comparing `tmp/ros_glint-0.1.0.tar.gz` & `tmp/ros_glint-0.2.0.tar.gz`

## Comparing `ros_glint-0.1.0.tar` & `ros_glint-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.coveragerc
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.gitattributes
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.yamllint.yaml
--rw-r--r--   0        0        0   959635 2020-02-02 00:00:00.000000 ros_glint-0.1.0/logo.gif
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ros_glint-0.1.0/setup.cfg
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.github/workflows/publish_pip.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/_version.py
--rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/cmake_ordering.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/config.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/core.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/diff.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glint_hook.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/main.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/python_types.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/terminal.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/util.py
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/data/cmake.ignore
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/data/cmake_patterns.ignore
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/data/package.ignore
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/data/package_patterns.ignore
--rw-r--r--   0        0        0    13996 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/data/rviz_class_defaults.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/data/rviz_generic_defaults.yaml
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/data/rviz_global_defaults.yaml
--rw-r--r--   0        0        0    16523 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/cmake.py
--rw-r--r--   0        0        0    14463 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/cmake_installs.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/cmake_pretty.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/cmake_sorting.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/misc.py
--rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/package_xml.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/plugins.py
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/python_setup.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/ros_interfaces.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 ros_glint-0.1.0/src/ros_glint/glinters/rviz_config.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 ros_glint-0.1.0/test/test_from_zip.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ros_glint-0.1.0/test/zip_interface.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ros_glint-0.1.0/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ros_glint-0.1.0/LICENSE
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 ros_glint-0.1.0/README.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 ros_glint-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 ros_glint-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.coveragerc
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.gitattributes
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.yamllint.yaml
+-rw-r--r--   0        0        0   959635 2020-02-02 00:00:00.000000 ros_glint-0.2.0/logo.gif
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ros_glint-0.2.0/setup.cfg
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.github/workflows/publish_pip.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/_version.py
+-rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/cmake_ordering.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/config.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/core.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/diff.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glint_hook.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/main.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/python_types.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/terminal.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/util.py
+-rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/data/cmake.ignore
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/data/cmake_patterns.ignore
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/data/package.ignore
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/data/package_patterns.ignore
+-rw-r--r--   0        0        0    13996 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/data/rviz_class_defaults.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/data/rviz_generic_defaults.yaml
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/data/rviz_global_defaults.yaml
+-rw-r--r--   0        0        0    16556 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/cmake.py
+-rw-r--r--   0        0        0    14447 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/cmake_installs.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/cmake_pretty.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/cmake_sorting.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/misc.py
+-rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/package_xml.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/plugins.py
+-rw-r--r--   0        0        0     9476 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/python_setup.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/ros_interfaces.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 ros_glint-0.2.0/src/ros_glint/glinters/rviz_config.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 ros_glint-0.2.0/test/test_from_zip.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 ros_glint-0.2.0/test/zip_interface.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ros_glint-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ros_glint-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 ros_glint-0.2.0/README.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 ros_glint-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 ros_glint-0.2.0/PKG-INFO
```

### Comparing `ros_glint-0.1.0/.pre-commit-config.yaml` & `ros_glint-0.2.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -11,30 +11,30 @@
   - id: destroyed-symlinks
   - id: check-symlinks
   - id: check-case-conflict
   - id: check-yaml
   - id: check-ast
   - id: double-quote-string-fixer
   - id: requirements-txt-fixer
-  rev: v4.4.0
+  rev: v4.5.0
 - repo: https://github.com/codespell-project/codespell
   hooks:
   - id: codespell
     args:
     - --write-changes
     - --skip=src/ros_glint/data/*ignore
   rev: v2.2.6
 - repo: https://github.com/adrienverge/yamllint
   hooks:
   - id: yamllint
     args:
     - --format
     - parsable
     - --strict
-  rev: v1.32.0
+  rev: v1.35.1
 - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
   hooks:
   - id: yamlfmt
     args:
     - --width
     - '120'
     - --implicit_start
@@ -46,14 +46,14 @@
     - --offset
     - '0'
     exclude: ^.pre-commit-hooks.yaml
   rev: 0.2.3
 - repo: https://github.com/hhatto/autopep8
   hooks:
   - id: autopep8
-  rev: v2.0.4
+  rev: v2.1.0
 - repo: https://github.com/PyCQA/flake8
   hooks:
   - id: flake8
-  rev: 6.1.0
+  rev: 7.0.0
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `ros_glint-0.1.0/.pre-commit-hooks.yaml` & `ros_glint-0.2.0/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/.yamllint.yaml` & `ros_glint-0.2.0/.yamllint.yaml`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/logo.gif` & `ros_glint-0.2.0/logo.gif`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/.github/workflows/main.yaml` & `ros_glint-0.2.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/.github/workflows/publish_pip.yaml` & `ros_glint-0.2.0/.github/workflows/publish_pip.yaml`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/cmake_ordering.py` & `ros_glint-0.2.0/src/ros_glint/cmake_ordering.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/glint_hook.py` & `ros_glint-0.2.0/src/ros_glint/glint_hook.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/main.py` & `ros_glint-0.2.0/src/ros_glint/main.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/terminal.py` & `ros_glint-0.2.0/src/ros_glint/terminal.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/util.py` & `ros_glint-0.2.0/src/ros_glint/util.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/data/cmake.ignore` & `ros_glint-0.2.0/src/ros_glint/data/cmake.ignore`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/data/cmake_patterns.ignore` & `ros_glint-0.2.0/src/ros_glint/data/cmake_patterns.ignore`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/data/package.ignore` & `ros_glint-0.2.0/src/ros_glint/data/package.ignore`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/data/rviz_class_defaults.yaml` & `ros_glint-0.2.0/src/ros_glint/data/rviz_class_defaults.yaml`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/data/rviz_global_defaults.yaml` & `ros_glint-0.2.0/src/ros_glint/data/rviz_global_defaults.yaml`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/cmake.py` & `ros_glint-0.2.0/src/ros_glint/glinters/cmake.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,16 @@
             remove_cmake_comments_helper(content.contents, ignorables, replacement)
     cmake.contents = remove_empty_strings(cmake.contents)
 
 
 @glinter
 def remove_empty_cmake_lines(package):
     cmake = package.cmake
+    if not cmake:
+        return
     for i, content in enumerate(cmake.contents[:-2]):
         if str(content)[-1] == '\n' and cmake.contents[i + 1] == '\n' and cmake.contents[i + 2] == '\n':
             cmake.contents[i + 1] = ''
             cmake.mark_changed()
     cmake.contents = remove_empty_strings(cmake.contents)
```

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/cmake_installs.py` & `ros_glint-0.2.0/src/ros_glint/glinters/cmake_installs.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                 cmd.add_section('', ['include'])
                 insert_in_order(cmake, cmd)
             install_section_check(cmake, ['include/'], InstallType.HEADERS, package.ros_version, directory=True)
 
 
 @glinter
 def export_cplusplus_libraries(package):
-    if package.ros_version == 1:
+    if package.ros_version == 1 or not package.cmake:
         return
     libraries = package.cmake.get_libraries()
     if not libraries:
         return
 
     export_targets = []
     cmds = get_commands_by_type(package.cmake, InstallType.LIBRARY)
@@ -304,16 +304,15 @@
         build_tools = package.package_xml.get_packages_by_tag('buildtool_depend')
         if acp not in build_tools:
             package.package_xml.insert_new_packages('buildtool_depend', [acp])
             package.build_type = acp
 
         install_cmake_dependencies(package, {acp})
 
-    if package.setup_py is None:
-        create_setup_py(package)
+    create_setup_py(package)
 
 
 @glinter
 def update_misc_installs(package):
     extra_files_by_folder = collections.defaultdict(list)
 
     for rel_fn, package_file in sorted(package.components_by_name.items()):
```

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/cmake_pretty.py` & `ros_glint-0.2.0/src/ros_glint/glinters/cmake_pretty.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/cmake_sorting.py` & `ros_glint-0.2.0/src/ros_glint/glinters/cmake_sorting.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/misc.py` & `ros_glint-0.2.0/src/ros_glint/glinters/misc.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/package_xml.py` & `ros_glint-0.2.0/src/ros_glint/glinters/package_xml.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/plugins.py` & `ros_glint-0.2.0/src/ros_glint/glinters/plugins.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/python_setup.py` & `ros_glint-0.2.0/src/ros_glint/glinters/python_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from stylish_cmake_parser import Command, SectionStyle
 from ros_introspect.package import MiscPackageFile
+from ros_introspect.components.package_xml import PEOPLE_TAGS
 from ros_introspect.components.setup_py import create_setup_py, contains_quoted_string, quote_string, unquote_string
 from ros_introspect.components.setup_cfg import SetupCFG
 from ros_introspect.components.source_code import SourceCode
 from ..core import glinter
 from ..cmake_ordering import insert_in_order
 from ..python_types import get_python_usage, PythonUsage
 from .cmake import section_check
@@ -69,31 +70,36 @@
 
 
 @glinter
 def sync_package_xml_and_setup_py(package):
     if package.setup_py is None and package.build_type != 'ament_python':
         return
 
-    if package.setup_py is None:
-        create_setup_py(package)
+    create_setup_py(package)  # If needed
 
+    setup_py = package.setup_py
     for tag in ['version', 'description', 'license']:
-        tags = package.manifest.get_elements_by_tags([tag])
+        tags = package.package_xml.get_elements_by_tags([tag])
         if not tags:
             continue
-        value = tags[0].childNodes[0].nodeValue
-        package.setup_py.args[tag] = repr(value)
+        setup_py.set_arg(tag, tags[0].childNodes[0].nodeValue)
 
-    for maintainer in package.manifest.get_elements_by_tags(['maintainer']):
-        # TODO: Expand for author
-        # TODO: Joint multiple people?
-        package.setup_py.args['maintainer'] = repr(maintainer.childNodes[0].nodeValue)
-        package.setup_py.args['maintainer_email'] = repr(maintainer.getAttribute('email'))
-
-    package.setup_py.changed = True
+    for tag_name in PEOPLE_TAGS:
+        names = []
+        emails = []
+        for person in package.package_xml.get_people_by_tag(tag_name):
+            if person.name:
+                names.append(person.name)
+            if person.email:
+                emails.append(person.email)
+
+        if names:
+            setup_py.set_arg(tag_name, ', '.join(names))
+        if emails:
+            setup_py.set_arg(f'{tag_name}_email', ', '.join(emails))
 
 
 def has_python_library(package_name, py_src):
     for source in py_src:
         parts = source.rel_fn.parts
         if len(parts) > 1 and parts[0] == 'src' and parts[1] == package_name:
             return True
```

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/ros_interfaces.py` & `ros_glint-0.2.0/src/ros_glint/glinters/ros_interfaces.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/src/ros_glint/glinters/rviz_config.py` & `ros_glint-0.2.0/src/ros_glint/glinters/rviz_config.py`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/test/test_from_zip.py` & `ros_glint-0.2.0/test/test_from_zip.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from ros_introspect import Package, ROSResources
 
 URL_TEMPLATE = 'https://github.com/DLu/roscompile_test_data/raw/{}/test_data.zip'
 TEST_DATA = [
     # (branch, known_hash)
     ('ros1', '84bf97b92d2ceb8d4369ed0d6fd8a01fabaf3006034fb7710d448b8cfe9885d9'),
-    ('ros2', 'cf23d832e0cf56c8e160c0178af81e865c615fb330fb26604ddf031fc51a280a'),
+    ('ros2', '5cfbd9c39ee239674d5c9e79f759f72655f869f43a0d0562dcc187cba7cc8efa'),
 ]
 
 linters = get_linters()
 
 
 def run_case(test_config, cases):
     resources = ROSResources.get()
```

### Comparing `ros_glint-0.1.0/test/zip_interface.py` & `ros_glint-0.2.0/test/zip_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import collections
 import os
 import pathlib
 import tempfile
 import yaml
 import zipfile
 
-from ros_introspect.finder import walk
+from ros_introspect.finder import walk, is_hidden
 from ros_glint.util import set_executable
 
 
 class ROSCompilePackageFiles:
     def __init__(self, package_name, pkg_files, executables):
         self.package_name = package_name
         self.is_written = False
@@ -30,21 +30,24 @@
 
     def __exit__(self, a_type, value, traceback):
         self.is_written = False
         self.root = None
         self.tempdir = None
 
     def get_filenames(self):
+        the_files = []
         if self.is_written:
-            the_files = []
             for subpath in walk(self.root):
                 the_files.append(subpath)
-            return set(the_files)
         else:
-            return set(self.pkg_files.keys())
+            for subpath in self.pkg_files.keys():
+                if is_hidden(subpath):
+                    continue
+                the_files.append(subpath)
+        return set(the_files)
 
     def get_contents(self, filename):
         if self.is_written:
             full_path = self.root / filename
             if full_path.exists():
                 return open(full_path).read().replace('\r\n', '\n')
         elif filename in self.pkg_files:
```

### Comparing `ros_glint-0.1.0/LICENSE` & `ros_glint-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/README.md` & `ros_glint-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 ![ROS Glint animated logo](logo.gif)
 
 ### Make your ROS code sparkle!
 
 ROS Glint is a linter for ROS 1 and ROS 2 packages.
 It is a pure Python version of the ROS 1 package [roscompile](https://github.com/DLu/roscompile/blob/main/roscompile/README.md).
 
+# Installation
+
+[![PyPI version](https://badge.fury.io/py/ros-glint.svg)](https://badge.fury.io/py/ros-glint)
+
+    sudo pip3 install ros-glint
+
 # Running from the Command Line
 
 Installing the Python package installs the `glint_ros` command. (Note: There's 5 million commands that start with `ros`. [citation needed] The command is `glint_ros` for ease of access/tab completion)
 
 The command will find all ROS packages in a the current directory and attempt to run the "glinters" on them all.
 
 ```
```

### Comparing `ros_glint-0.1.0/pyproject.toml` & `ros_glint-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ros_glint-0.1.0/PKG-INFO` & `ros_glint-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ros_glint
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pure Python library for linting ROS packages
 Project-URL: Homepage, https://github.com/MetroRobots/ros_glint
 Project-URL: Bug Tracker, https://github.com/MetroRobots/ros_glint/issues
 Author-email: "David V. Lu!!" <davidvlu@gmail.com>
 Maintainer-email: "David V. Lu!!" <davidvlu@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,20 @@
 ![ROS Glint animated logo](logo.gif)
 
 ### Make your ROS code sparkle!
 
 ROS Glint is a linter for ROS 1 and ROS 2 packages.
 It is a pure Python version of the ROS 1 package [roscompile](https://github.com/DLu/roscompile/blob/main/roscompile/README.md).
 
+# Installation
+
+[![PyPI version](https://badge.fury.io/py/ros-glint.svg)](https://badge.fury.io/py/ros-glint)
+
+    sudo pip3 install ros-glint
+
 # Running from the Command Line
 
 Installing the Python package installs the `glint_ros` command. (Note: There's 5 million commands that start with `ros`. [citation needed] The command is `glint_ros` for ease of access/tab completion)
 
 The command will find all ROS packages in a the current directory and attempt to run the "glinters" on them all.
 
 ```
```

