# Comparing `tmp/wwpdb_apps_editormodule-0.18.1.tar.gz` & `tmp/wwpdb_apps_editormodule-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_apps_editormodule-0.18.1.tar", last modified: Mon Apr 15 23:53:40 2024, max compression
+gzip compressed data, was "wwpdb_apps_editormodule-0.19.tar", last modified: Sat Jun  1 13:12:55 2024, max compression
```

## Comparing `wwpdb_apps_editormodule-0.18.1.tar` & `wwpdb_apps_editormodule-0.19.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.225452 wwpdb_apps_editormodule-0.18.1/
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/LICENSE
--rwxr-xr-x   0 vsts      (1001) docker     (127)      110 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-15 23:53:40.225452 wwpdb_apps_editormodule-0.18.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-15 23:53:40.225452 wwpdb_apps_editormodule-0.18.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2209 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.217451 wwpdb_apps_editormodule-0.18.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.217451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.217451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.217451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/
--rw-r--r--   0 vsts      (1001) docker     (127)      290 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7864 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/EditorConfig.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)   144958 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
--rw-r--r--   0 vsts      (1001) docker     (127)   216804 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/depict/
--rwxr-xr-x   0 vsts      (1001) docker     (127)    52449 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/depict/EditorDepict.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/
--rw-r--r--   0 vsts      (1001) docker     (127)     4873 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/EditorDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (127)   163711 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxDataIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8061 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1616 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/
--rw-r--r--   0 vsts      (1001) docker     (127)     6211 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
--rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (127)    13947 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (127)    17945 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
--rw-r--r--   0 vsts      (1001) docker     (127)    15904 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
--rw-r--r--   0 vsts      (1001) docker     (127)     3502 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_prototyping.html
--rw-r--r--   0 vsts      (1001) docker     (127)     2470 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    79034 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/EditorWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)    10750 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/WebRequest.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1637 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-15 23:53:25.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.244025 wwpdb_apps_editormodule-0.19/
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/LICENSE
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      110 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-06-01 13:12:55.244025 wwpdb_apps_editormodule-0.19/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-06-01 13:12:55.244025 wwpdb_apps_editormodule-0.19/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2209 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.240024 wwpdb_apps_editormodule-0.19/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.240024 wwpdb_apps_editormodule-0.19/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.240024 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.240024 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/
+-rw-r--r--   0 vsts      (1001) docker     (127)      290 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7864 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/EditorConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   144958 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
+-rw-r--r--   0 vsts      (1001) docker     (127)   216804 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.240024 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/depict/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    52449 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/depict/EditorDepict.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.244025 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4873 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/EditorDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   164042 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/PdbxDataIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8061 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1616 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.244025 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6211 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    13947 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    17945 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    15904 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     3502 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_prototyping.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     2470 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.244025 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    79288 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/webapp/EditorWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    10750 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/webapp/WebRequest.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:11:44.000000 wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:12:55.244025 wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-06-01 13:12:55.000000 wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1637 2024-06-01 13:12:55.000000 wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 13:12:55.000000 wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 13:12:42.000000 wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-06-01 13:12:55.000000 wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-06-01 13:12:55.000000 wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/top_level.txt
```

### Comparing `wwpdb_apps_editormodule-0.18.1/LICENSE` & `wwpdb_apps_editormodule-0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/PKG-INFO` & `wwpdb_apps_editormodule-0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.18.1
+Version: 0.19
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 License-File: LICENSE
 Requires-Dist: mmcif
 Requires-Dist: mmcif.utils
 Requires-Dist: wwpdb.utils.wf
 Requires-Dist: wwpdb.utils.db
 Requires-Dist: wwpdb.utils.session
 Requires-Dist: wwpdb.io
-Requires-Dist: wwpdb.utils.config~=0.24
+Requires-Dist: wwpdb.utils.config>=0.24
 Requires-Dist: wwpdb.utils.dp~=0.45
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 See:  README.md
```

### Comparing `wwpdb_apps_editormodule-0.18.1/setup.py` & `wwpdb_apps_editormodule-0.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     #
-    install_requires=["mmcif", "mmcif.utils", "wwpdb.utils.wf", "wwpdb.utils.db", "wwpdb.utils.session", "wwpdb.io", "wwpdb.utils.config ~= 0.24", "wwpdb.utils.dp ~= 0.45"],
+    install_requires=["mmcif", "mmcif.utils", "wwpdb.utils.wf", "wwpdb.utils.db", "wwpdb.utils.session", "wwpdb.io", "wwpdb.utils.config >= 0.24", "wwpdb.utils.dp ~= 0.45"],
     packages=find_packages(exclude=["wwpdb.apps.tests-editormodule"]),
     # Enables Manifest to be used
     include_package_data=True,
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         "": ["*.md", "*.rst", "*.txt", "*.cfg", "*.html", "*.cif"],
     },
```

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/EditorConfig.py` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/EditorConfig.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif`

 * *Files 0% similar despite different names*

```diff
@@ -364,17 +364,17 @@
 loop_
 _pdbx_display_view_item_info.category_display_name
 _pdbx_display_view_item_info.item_name
 _pdbx_display_view_item_info.item_display_name
 _pdbx_display_view_item_info.read_only_flag
 em_admin                           '_em_admin.entry_id'                                          id                                               Y
 em_admin                           '_em_admin.title'                                             'entry title'                                    N
-em_admin                           '_em_admin.current_status'                                    'current status'                                 N
-em_admin                           '_em_admin.map_release_date'                                  'map release date'                               N
-em_admin                           '_em_admin.obsoleted_date'                                    'obsoleted date'                                 N
+em_admin                           '_em_admin.current_status'                                    'current status'                                 Y
+em_admin                           '_em_admin.map_release_date'                                  'map release date'                               Y
+em_admin                           '_em_admin.obsoleted_date'                                    'obsoleted date'                                 Y
 em_admin                           '_em_admin.replace_existing_entry_flag'                       'replace existing entry flag'                    N
 
 data_EM1B
 loop_
 _pdbx_display_view_category_info.category_menu_display_name
 _pdbx_display_view_category_info.category_name
 _pdbx_display_view_category_info.category_group_display_name
```

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/depict/EditorDepict.py` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/depict/EditorDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/EditorDataImport.py` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/EditorDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxDataIo.py` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/PdbxDataIo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1595,14 +1595,16 @@
             #
             for attributeNm in attributeList:
 
                 if attributeNm == "task_name":
                     valueToSupply = "solvent position" if p_task == "solventpos" else p_task
                 elif attributeNm == "status":
                     valueToSupply = "skip"
+                else:
+                    valueToSupply = "None"
                 #
                 rowToAdd.append(valueToSupply)
 
             #
             if self.__verbose:
                 logger.info("-- About to update category '%s' with new row as %r", cifCtgryNm, rowToAdd)
             #
@@ -2583,14 +2585,16 @@
         #
         if p_ctgryName == "audit_author":
             targetAttributeNm = "pdbx_ordinal"
         elif p_ctgryName == "citation_author":
             targetAttributeNm = "ordinal"
         elif p_ctgryName == "em_author_list":
             targetAttributeNm = "ordinal"
+        else:
+            targetAttributeNm = "None"  # Will cause an error
 
         ctgryObj = p_myPersist.fetchOneObject(self.__dbFilePath, self.__dataBlockName, p_ctgryName)
         #
         if ctgryObj:
             rowList = ctgryObj.getRowList()
             #
             attributeList = ctgryObj.getAttributeList()
@@ -2616,28 +2620,32 @@
             if self.__verbose:
                 logger.info("'%s' category not found in data.", p_ctgryName)
 
         return bSuccess
 
     def propagateTitle(self, p_targetCtgry):
         """copy title to/from citation from/to struct"""
-        if os.access(self.__dbFilePath, os.R_OK):
 
-            origTitleValue = None
+        origTitleValue = None
+        bSuccess = False
+
+        if os.access(self.__dbFilePath, os.R_OK):
             bSuccess = True
             myPersist = PdbxPersist(self.__verbose, self.__lfh)
 
             if not self.__pdbxDictStore:
                 self.__pdbxDictStore = PdbxDictionaryInfoStore(verbose=self.__verbose, log=self.__lfh)
             #
             targetAttributeNm = "title"
             if p_targetCtgry == "struct":
                 srcCtgry = "citation"
             elif p_targetCtgry == "citation":
                 srcCtgry = "struct"
+            else:
+                srcCtgry = "None"  # Error - but what can you do
 
             srcCtgryObj = myPersist.fetchOneObject(self.__dbFilePath, self.__dataBlockName, srcCtgry)
             targetCtgryObj = myPersist.fetchOneObject(self.__dbFilePath, self.__dataBlockName, p_targetCtgry)
             #
             if srcCtgryObj:
                 srcRowList = srcCtgryObj.getRowList()
                 #
@@ -2649,14 +2657,15 @@
                     if attributeNm == targetAttributeNm:
                         indxSrcTitle = iNdx
                     if srcCtgry == "citation":
                         if attributeNm == "id":
                             indxSrcId = iNdx
 
                 if indxSrcTitle >= 0:
+                    srcTitleValue = None
                     for _rowNum, row in enumerate(srcRowList):
                         if indxSrcId >= 0:
                             if row[indxSrcId] == "primary":
                                 srcTitleValue = row[indxSrcTitle]
                         else:
                             srcTitleValue = row[indxSrcTitle]
 
@@ -2666,14 +2675,15 @@
                     targetRowList = targetCtgryObj.getRowList()
                     #
                     targetAttributeList = targetCtgryObj.getAttributeList()
                     #
                     idxTargetTitle = -1
                     idxTargetId = -1
                     targetRowNmbr = 0
+                    targetTitleValue = None
                     for idx, attribNm in enumerate(targetAttributeList):
                         if attribNm == targetAttributeNm:
                             idxTargetTitle = idx
                         if p_targetCtgry == "citation":
                             if attribNm == "id":
                                 idxTargetId = idx
```

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_prototyping.html` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_prototyping.html`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/EditorWebApp.py` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/webapp/EditorWebApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,14 +324,18 @@
         subject = str(self.__reqObj.getValue("subject"))
         depId = str(self.__reqObj.getValue("dep_id")) if self.__reqObj.getValue("suffix") is not None else ""
         feedback = str(self.__reqObj.getValue("feedback"))
         #
         haveUploadFile = False
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
         #
+        # Keep pylint happy - define variable - only needed if haveUploadFile is True
+        encodedContent = None
+        uploadFlMimeTyp = None
+        uploadFlName = None
         #
         if self.__isFileUpload():
             haveUploadFile = self.__uploadFeedbackFile()
             if haveUploadFile:
                 uploadFlPth = self.__reqObj.getValue("filePath")
                 uploadFlName = self.__reqObj.getValue("uploadFileName")
                 uploadFlMimeTyp = self.__reqObj.getValue("mimeType")
@@ -1222,14 +1226,16 @@
         cloneItems = self.__reqObj.getValue("clone_items")
         #
         if self.__verbose:
             logger.info("-- cifctgry is:%s", cifCtgry)
             logger.info("-- editActnIndx is:%s", editActnIndx)
             logger.info("-- action is:%s", action)
             #
+
+        numRows = None  # Not really needed as only delrow will need variable
         if action == "delrow" or action == "insert":
             rowIdx = self.__reqObj.getValue("row_idx")
             numRows = int(self.__reqObj.getValue("num_rows")) if self.__reqObj.getValue("num_rows") else None
             logger.info(" -- rowIdx is:%s", rowIdx)
             rowIdx = int(rowIdx.replace("row_", ""))  # remove prefix so that can be used by PdbxDataIo
 
             if context == "editorconfig" and action == "insert":
```

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/WebRequest.py` & `wwpdb_apps_editormodule-0.19/wwpdb/apps/editormodule/webapp/WebRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/PKG-INFO` & `wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.18.1
+Version: 0.19
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 License-File: LICENSE
 Requires-Dist: mmcif
 Requires-Dist: mmcif.utils
 Requires-Dist: wwpdb.utils.wf
 Requires-Dist: wwpdb.utils.db
 Requires-Dist: wwpdb.utils.session
 Requires-Dist: wwpdb.io
-Requires-Dist: wwpdb.utils.config~=0.24
+Requires-Dist: wwpdb.utils.config>=0.24
 Requires-Dist: wwpdb.utils.dp~=0.45
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 See:  README.md
```

### Comparing `wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/SOURCES.txt` & `wwpdb_apps_editormodule-0.19/wwpdb.apps.editormodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

