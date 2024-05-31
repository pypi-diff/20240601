# Comparing `tmp/ros_introspect-0.2.0.tar.gz` & `tmp/ros_introspect-0.2.1.tar.gz`

## Comparing `ros_introspect-0.2.0.tar` & `ros_introspect-0.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/.coveragerc
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/.gitattributes
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/.yamllint.yaml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/setup.cfg
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/.github/workflows/publish_pip.yaml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/_version.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/finder.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/package.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/ros_resources.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/util.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/cmake.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/documentation.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/dynamic_reconfig.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/launch.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/misc_config.py
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/package_xml.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/param_config.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/plugin_xml.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/ros_interface.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/rviz_config.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/setup_cfg.py
--rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/setup_py.py
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/source_code.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/src/ros_introspect/components/urdf.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test/test_components.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test/test_finder.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test/test_packages.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test/test_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/README.md
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/eeaao/package.xml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/hibachi/CMakeLists.txt
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/hibachi/package.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/hibachi/src/lib.cpp
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/hibachi/src/main.cpp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/kungfu/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/kungfu/ignore_file.yaml~
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/kungfu/package.xml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/kungfu/test_file.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/kungfu/.hidden_folder/pinata.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/kungfu/.svn/very_important_svn_file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/kungfu/scripts/pinky.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/eleanor/kungfu/scripts/pinky.py~
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/fake_git_root/chad/package.xml
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/fake_git_root/racacoonie/package.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/jobu/kpop/COLCON_IGNORE
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/jobu/kpop/package.xml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/waymond/package.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/waymond/random_file
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/waymond/action/Laundry.action
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/waymond/action/Taxes.action
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/waymond/msg/FannyPack.msg
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/test_data/waymond/srv/BeKind.srv
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/LICENSE
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/README.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 ros_introspect-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/.coveragerc
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/.gitattributes
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/.yamllint.yaml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/setup.cfg
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/.github/workflows/publish_pip.yaml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/_version.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/finder.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/package.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/ros_resources.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/util.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/cmake.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/documentation.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/dynamic_reconfig.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/launch.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/misc_config.py
+-rw-r--r--   0        0        0    12593 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/package_xml.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/param_config.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/plugin_xml.py
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/ros_interface.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/rviz_config.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/setup_cfg.py
+-rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/setup_py.py
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/source_code.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/src/ros_introspect/components/urdf.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test/test_components.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test/test_finder.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test/test_packages.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test/test_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/README.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/eeaao/package.xml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/hibachi/CMakeLists.txt
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/hibachi/package.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/hibachi/src/lib.cpp
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/hibachi/src/main.cpp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/kungfu/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/kungfu/ignore_file.yaml~
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/kungfu/package.xml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/kungfu/test_file.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/kungfu/.hidden_folder/pinata.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/kungfu/.svn/very_important_svn_file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/kungfu/scripts/pinky.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/eleanor/kungfu/scripts/pinky.py~
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/fake_git_root/chad/package.xml
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/fake_git_root/racacoonie/package.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/jobu/kpop/COLCON_IGNORE
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/jobu/kpop/package.xml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/waymond/package.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/waymond/random_file
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/waymond/action/Laundry.action
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/waymond/action/Taxes.action
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/waymond/msg/FannyPack.msg
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/test_data/waymond/srv/BeKind.srv
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/README.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 ros_introspect-0.2.1/PKG-INFO
```

### Comparing `ros_introspect-0.2.0/.pre-commit-config.yaml` & `ros_introspect-0.2.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -22,27 +22,27 @@
   - id: codespell
     args:
     - --write-changes
   rev: v2.2.6
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
 - repo: https://github.com/adrienverge/yamllint
   hooks:
   - id: yamllint
     args:
     - --format
     - parsable
     - --strict
-  rev: v1.33.0
+  rev: v1.35.1
 - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
   hooks:
   - id: yamlfmt
     args:
     - --width
     - '120'
     - --implicit_start
```

### Comparing `ros_introspect-0.2.0/.yamllint.yaml` & `ros_introspect-0.2.1/.yamllint.yaml`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/.github/workflows/main.yaml` & `ros_introspect-0.2.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/.github/workflows/publish_pip.yaml` & `ros_introspect-0.2.1/.github/workflows/publish_pip.yaml`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/__init__.py` & `ros_introspect-0.2.1/src/ros_introspect/__init__.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/finder.py` & `ros_introspect-0.2.1/src/ros_introspect/finder.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,22 +50,32 @@
     for subfolder in parent_path.iterdir():
         if not subfolder.is_dir():
             continue
         if is_package_root(subfolder) and subfolder != package_folder:
             yield subfolder
 
 
-def walk(root, include_hidden=True):
+def is_hidden(path, check_all=True):
+    parts = path.parts
+    if not check_all:
+        parts = parts[-1:]
+    for part in parts:
+        if part.startswith('.'):
+            return True
+    return False
+
+
+def walk(root, include_hidden=False):
     """Yield the paths of all the "valid" files in a directory, relative to the directory"""
 
     queue = [root]
     while queue:
         folder = queue.pop(0)
         for subpath in folder.iterdir():
-            if not include_hidden and subpath.name.startswith('.'):
+            if not include_hidden and is_hidden(subpath, check_all=False):
                 # Ignore hidden files and directories
                 continue
 
             if subpath.is_dir():
                 # Folder
                 if not is_repo_marker(subpath):
                     queue.append(subpath)
```

### Comparing `ros_introspect-0.2.0/src/ros_introspect/package.py` & `ros_introspect-0.2.1/src/ros_introspect/package.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/ros_resources.py` & `ros_introspect-0.2.1/src/ros_introspect/ros_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             cls.instance.actions = set()
         return cls.instance
 
     @classmethod
     def get(cls):
         return cls()
 
-    def load_from_ros(self):
+    def load_from_ros(self):  # pragma: no cover
         self.packages |= get_package_names()
         for interface in list_interfaces():
             self.add_interface(interface)
 
     def add_interface(self, interface):
         if interface.type == 'msg':
             self.messages.add(interface)
```

### Comparing `ros_introspect-0.2.0/src/ros_introspect/util.py` & `ros_introspect-0.2.1/src/ros_introspect/util.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/cmake.py` & `ros_introspect-0.2.1/src/ros_introspect/components/cmake.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/launch.py` & `ros_introspect-0.2.1/src/ros_introspect/components/launch.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/package_xml.py` & `ros_introspect-0.2.1/src/ros_introspect/components/package_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,22 +194,30 @@
             keys.append('test_depend')
 
         pkgs = set()
         for key in keys:
             pkgs |= self.get_packages_by_tag(key)
         return pkgs
 
-    def get_people(self):
+    def get_people_by_tag(self, tag):
         people = []
-        for el in self.get_elements_by_tags(PEOPLE_TAGS):
+        for el in self.root.getElementsByTagName(tag):
             name = el.childNodes[0].nodeValue
             email = el.getAttribute('email')
             people.append(Person(name, email))
         return people
 
+    def get_people(self):
+        people = []
+        for tag in PEOPLE_TAGS:
+            for person in self.get_people_by_tag(tag):
+                if person not in people:
+                    people.append(person)
+        return people
+
     def get_license_element(self):
         els = self.root.getElementsByTagName('license')
         if els:
             return els[0]
 
     def get_license(self):
         el = self.get_license_element()
```

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/param_config.py` & `ros_introspect-0.2.1/src/ros_introspect/components/param_config.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/plugin_xml.py` & `ros_introspect-0.2.1/src/ros_introspect/components/plugin_xml.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/ros_interface.py` & `ros_introspect-0.2.1/src/ros_introspect/components/ros_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,16 @@
             return deps
 
         for section in self.sections:
             for field in section.fields:
                 if '/' not in field.type:
                     continue
                 package = field.type.split('/')[0]
+                if package == self.package.name:
+                    continue
                 deps.add(package)
 
         return deps
 
     def regenerate_contents(self):
         return '---\n'.join(map(str, self.sections))
```

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/rviz_config.py` & `ros_introspect-0.2.1/src/ros_introspect/components/rviz_config.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/setup_py.py` & `ros_introspect-0.2.1/src/ros_introspect/components/setup_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Version-Dependent AST operations
 if sys.version_info.major == 3 and sys.version_info.minor >= 8:
     def is_constant(el):
         return isinstance(el.value, ast.Constant)
 
     get_source_segment = ast.get_source_segment
-else:
+else:  # pragma: no cover
     def is_constant(el):
         return isinstance(el.value, ast.Str)
 
     def get_source_segment(source, node):
         """Get source code segment of the *source* that generated *node*.
         If some location information (`lineno`, `end_lineno`, `col_offset`,
         or `end_col_offset`) is missing, return None.
@@ -241,14 +241,21 @@
                     for keyword in el.value.keywords:
                         self.args[keyword.arg] = ast_to_python(keyword.value)
 
             elif isinstance(el, ast.Expr) and self.helper_variable is None:
                 for keyword in el.value.keywords:
                     self.args[keyword.arg] = ast_to_python(keyword.value)
 
+    def set_arg(self, key, value):
+        f_value = repr(value)
+        if self.args.get(key) == f_value:
+            return
+        self.args[key] = f_value
+        self.changed = True
+
     def get_share_path(self, rel_fn=None):
         if str(rel_fn) == 'resource':
             return "'share/ament_index/resource_index/packages'"
 
         if self.declare_package_name:
             base_folder = "'share/' + package_name"
         else:
@@ -280,18 +287,18 @@
                 if m:
                     glob_pattern = m.group(1)
                     existing_files = []
                     root = self.full_path.parent
                     for subpath in root.glob(glob_pattern):
                         existing_files.append(quote_string(str(subpath).replace(str(root) + '/', '')))
 
-            if not isinstance(existing_files, list):
+            if not isinstance(existing_files, list):  # pragma: no cover
                 raise RuntimeError('Trouble understanding the install data_files bit of the setup.py')
 
-        if folder == 'resource' and self.declare_package_name and "'resource/' + package_name" in existing_files:
+        if str(folder) == 'resource' and self.declare_package_name and "'resource/' + package_name" in existing_files:
             paths.remove(self.package.name)
 
         for fn in paths:
             if folder:
                 resolved = quote_string(folder / fn)
             else:
                 resolved = quote_string(fn)
@@ -345,15 +352,15 @@
 
 def create_setup_py(package):
     if package.setup_py:
         return
     package.add_file(SetupPy(package.root / 'setup.py', package))
 
 
-if __name__ == '__main__':
+if __name__ == '__main__':  # pragma: no coverage
     output_dir = pathlib.Path('output_data')
     output_dir.mkdir(exist_ok=True)
 
     rows = []
     for filename in sorted(pathlib.Path('test_data').glob('*py')):
         spy = SetupPy('TEST_PACKAGE_NAME', filename)
```

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/source_code.py` & `ros_introspect-0.2.1/src/ros_introspect/components/source_code.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/src/ros_introspect/components/urdf.py` & `ros_introspect-0.2.1/src/ros_introspect/components/urdf.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/test/test_components.py` & `ros_introspect-0.2.1/test/test_components.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/test/test_finder.py` & `ros_introspect-0.2.1/test/test_finder.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,9 +32,9 @@
     assert len(e_sibs) == 2
     names = [sib.name for sib in e_sibs]
     assert 'kungfu' in names
 
 
 def test_walk():
     folder = TEST_DATA_FOLDER / 'eleanor' / 'kungfu'
-    assert len(list(walk(folder))) == 5
+    assert len(list(walk(folder, include_hidden=True))) == 5
     assert len(list(walk(folder, include_hidden=False))) == 4
```

### Comparing `ros_introspect-0.2.0/test/test_packages.py` & `ros_introspect-0.2.1/test/test_packages.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/test/test_util.py` & `ros_introspect-0.2.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/LICENSE` & `ros_introspect-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/README.md` & `ros_introspect-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/pyproject.toml` & `ros_introspect-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ros_introspect-0.2.0/PKG-INFO` & `ros_introspect-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ros_introspect
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pure Python library for working with the files in ROS packages
 Project-URL: Homepage, https://github.com/MetroRobots/ros_introspect
 Project-URL: Bug Tracker, https://github.com/MetroRobots/ros_introspect/issues
 Author-email: "David V. Lu!!" <davidvlu@gmail.com>
 Maintainer-email: "David V. Lu!!" <davidvlu@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

