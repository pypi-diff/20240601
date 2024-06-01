# Comparing `tmp/wwpdb_utils_wf-0.35.4.tar.gz` & `tmp/wwpdb_utils_wf-0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_utils_wf-0.35.4.tar", last modified: Thu May  9 20:24:05 2024, max compression
+gzip compressed data, was "wwpdb_utils_wf-0.36.tar", last modified: Sat Jun  1 09:49:19 2024, max compression
```

## Comparing `wwpdb_utils_wf-0.35.4.tar` & `wwpdb_utils_wf-0.36.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      485 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2103 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.484543 wwpdb_utils_wf-0.35.4/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.488543 wwpdb_utils_wf-0.35.4/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.488543 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/
--rw-r--r--   0 vsts      (1001) docker     (127)     3229 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/DataSelector.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4658 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/DataValueContainer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3661 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/WfDataObject.py
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.488543 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/
--rw-r--r--   0 vsts      (1001) docker     (127)     6846 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16002 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbCommand.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbConnection.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1946 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/LocalDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3018 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/StatusDbApi.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1281 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WFEtime.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47456 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WfDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4251 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WfTracking.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11637 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/dbAPI.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.492544 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/
--rw-r--r--   0 vsts      (1001) docker     (127)    65854 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/AnnotationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11876 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ChemCompUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/DictUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4666 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/DpUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18242 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6275 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/FileUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13301 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/FormatUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50817 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/NmrUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18848 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/PdbxUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3840 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/PrdSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3427 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5580 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SFConvert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5698 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SeqStatsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11212 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SeqdbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1456 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/UtilsBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27740 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ValidationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/
--rw-r--r--   0 vsts      (1001) docker     (127)    15843 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ActionRegistry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7456 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ActionRegistryIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11325 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ProcessRunner.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/
--rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/WfSchemaMap.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11697 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/database_descriptions.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      233 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/mandatory_items.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1724 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 20:23:48.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      132 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.605676 wwpdb_utils_wf-0.36/
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1015 2024-06-01 09:49:19.605676 wwpdb_utils_wf-0.36/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      485 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-06-01 09:49:19.605676 wwpdb_utils_wf-0.36/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2103 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.597676 wwpdb_utils_wf-0.36/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.597676 wwpdb_utils_wf-0.36/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.597676 wwpdb_utils_wf-0.36/wwpdb/utils/wf/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3229 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/DataSelector.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4658 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/DataValueContainer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3661 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/WfDataObject.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.601676 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6846 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16002 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/DbCommand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/DbConnection.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1946 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/LocalDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3018 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/StatusDbApi.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1281 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/WFEtime.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47489 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/WfDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4251 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/WfTracking.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11637 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/dbAPI.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.605676 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (127)    65854 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/AnnotationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11876 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/ChemCompUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/DictUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4666 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/DpUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18242 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6275 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/FileUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13301 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/FormatUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50953 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/NmrUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18891 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/PdbxUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3840 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/PrdSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3427 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5580 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/SFConvert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5698 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/SeqStatsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11212 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/SeqdbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1456 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/UtilsBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27740 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/ValidationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.605676 wwpdb_utils_wf-0.36/wwpdb/utils/wf/process/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15843 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/process/ActionRegistry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7456 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/process/ActionRegistryIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11325 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/process/ProcessRunner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/process/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.605676 wwpdb_utils_wf-0.36/wwpdb/utils/wf/schema/
+-rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/schema/WfSchemaMap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/schema/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11697 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/schema/database_descriptions.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      233 2024-06-01 09:48:01.000000 wwpdb_utils_wf-0.36/wwpdb/utils/wf/schema/mandatory_items.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 09:49:19.605676 wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1015 2024-06-01 09:49:19.000000 wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1724 2024-06-01 09:49:19.000000 wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 09:49:19.000000 wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 09:49:04.000000 wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      132 2024-06-01 09:49:19.000000 wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-06-01 09:49:19.000000 wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/top_level.txt
```

### Comparing `wwpdb_utils_wf-0.35.4/LICENSE` & `wwpdb_utils_wf-0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/PKG-INFO` & `wwpdb_utils_wf-0.36/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.35.4
+Version: 0.36
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_wf-0.35.4/setup.py` & `wwpdb_utils_wf-0.36/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/DataSelector.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/DataSelector.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/DataValueContainer.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/DataValueContainer.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/WfDataObject.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/WfDataObject.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbApiUtil.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbCommand.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/DbCommand.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbConnection.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/DbConnection.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/LocalDbApi.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/LocalDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/StatusDbApi.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/StatusDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WFEtime.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/WFEtime.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WfDbApi.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/WfDbApi.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,14 +598,16 @@
         """
 
         existObj = False
         depId = None
         classId = None
         instId = None
         taskId = None
+        rd = {}
+
         if len(dataObj) == 0:
             existObj = False
         else:
             if self.__idList[3] in dataObj.keys():
                 taskId = dataObj[self.__idList[3]]
             if self.__idList[2] in dataObj.keys():
                 instId = dataObj[self.__idList[2]]
@@ -614,18 +616,18 @@
             if self.__idList[0] in dataObj.keys():
                 depId = dataObj[self.__idList[0]]
             if depId is None and classId is None and instId is None and taskId is None:
                 existObj = False
             else:
                 rd = self.getObject(depId, classId, instId, taskId)
 
-            if len(rd) > 0:
-                existObj = True
-            else:
-                existObj = False
+                if len(rd) > 0:
+                    existObj = True
+                else:
+                    existObj = False
 
         return existObj
 
     def getTableDef(self, dataObj):
         """
         Determine which table to use in the database
```

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WfTracking.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/WfTracking.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/dbAPI.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/dbapi/dbAPI.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/AnnotationUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/AnnotationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ChemCompUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/ChemCompUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/DictUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/DictUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/DpUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/DpUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/EmUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/EmUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/FileUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/FileUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/FormatUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/FormatUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/NmrUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/NmrUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,16 +483,14 @@
                                 elif save_pattern.match(line):
                                     has_save = True
                                 elif loop_pattern.match(line):
                                     has_loop = True
                                 elif stop_pattern.match(line):
                                     has_stop = True
 
-                            ifp.close()
-
                         if has_datablock or has_anonymous_saveframe or has_save or has_loop or has_stop:  # NMR-STAR or NEF (DAOTHER-6830)
                             mrPathList.append(mr_file)
                         else:
                             arPathList.append({"file_name": mr_file, "file_type": mr_file_type, "original_file_name": mr_orig_file})
             #
             cifInpPath = inpObjD["src3"].getFilePathReference()
             prcInpPath = inpObjD["prc3"].getFilePathReference()
@@ -586,28 +584,31 @@
                     if mr_file_type.startswith("nm-res") or mr_file_type.startswith("nm-aux") or mr_file_type.startswith("nm-pea"):
                         has_datablock = False
                         has_anonymous_saveframe = False
                         has_save = False
                         has_loop = False
                         has_stop = False
 
-                        with open(mr_file, "r") as ifp:
-                            for line in ifp:
-                                if datablock_pattern.match(line):
-                                    has_datablock = True
-                                elif sf_anonymous_pattern.match(line):
-                                    has_anonymous_saveframe = True
-                                elif save_pattern.match(line):
-                                    has_save = True
-                                elif loop_pattern.match(line):
-                                    has_loop = True
-                                elif stop_pattern.match(line):
-                                    has_stop = True
+                        try:
+
+                            with open(mr_file, "r") as ifp:
+                                for line in ifp:
+                                    if datablock_pattern.match(line):
+                                        has_datablock = True
+                                    elif sf_anonymous_pattern.match(line):
+                                        has_anonymous_saveframe = True
+                                    elif save_pattern.match(line):
+                                        has_save = True
+                                    elif loop_pattern.match(line):
+                                        has_loop = True
+                                    elif stop_pattern.match(line):
+                                        has_stop = True
 
-                            ifp.close()
+                        except UnicodeDecodeError:  # catch exception due to binary format (DAOTHER-9425)
+                            pass
 
                         if has_datablock or has_anonymous_saveframe or has_save or has_loop or has_stop:  # NMR-STAR or NEF (DAOTHER-6830)
                             mrPathList.append(mr_file)
                         else:
                             arPathList.append({"file_name": mr_file, "file_type": mr_file_type, "original_file_name": mr_orig_file})
             #
             cifInpPath = inpObjD["src4"].getFilePathReference()
```

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/PdbxUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/PdbxUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,24 +241,24 @@
             else:
                 return False
             #
             yes_no_value = self.__getAnnModAutoCompleteFlag()
             if outObjD["dst2"].getContainerTypeName() == "value":
                 outObjD["dst2"].setValue(yes_no_value)
             elif outObjD["dst2"].getContainerTypeName() == "list":
-                outObjD["dst2"].setValue([ yes_no_value ])
+                outObjD["dst2"].setValue([yes_no_value])
             else:
                 return False
             #
             cI = ConfigInfo()
             siteName = cI.get("SITE_NAME")
             if outObjD["dst3"].getContainerTypeName() == "value":
                 outObjD["dst3"].setValue(siteName)
             elif outObjD["dst3"].getContainerTypeName() == "list":
-                outObjD["dst3"].setValue([ siteName ])
+                outObjD["dst3"].setValue([siteName])
             else:
                 return False
             #
             return True
         except Exception as _e:  # noqa: F841
             if self._verbose:
                 traceback.print_exc(file=self._lfh)
@@ -465,21 +465,21 @@
                         #
                     #
                 #
             #
             if ret == "NO":
                 return ret
             #
-            assemblyCategories = { "pdbx_struct_assembly": [ "id", "details" ], \
-                                   "pdbx_struct_assembly_gen": [ "assembly_id", "oper_expression", "asym_id_list" ], \
-                                   "pdbx_struct_oper_list": [ "id", "matrix[1][1]", "matrix[1][2]", "matrix[1][3]", \
-                                   "vector[1]", "matrix[2][1]", "matrix[2][2]", "matrix[2][3]", "vector[2]", "matrix[3][1]", \
-                                   "matrix[3][2]", "matrix[3][3]", "vector[3]" ] }
+            assemblyCategories = {"pdbx_struct_assembly": ["id", "details"],
+                                  "pdbx_struct_assembly_gen": ["assembly_id", "oper_expression", "asym_id_list"],
+                                  "pdbx_struct_oper_list": ["id", "matrix[1][1]", "matrix[1][2]", "matrix[1][3]",
+                                                            "vector[1]", "matrix[2][1]", "matrix[2][2]", "matrix[2][3]", "vector[2]", "matrix[3][1]",
+                                                            "matrix[3][2]", "matrix[3][3]", "vector[3]"]}
             #
-            for cate,items in assemblyCategories.items():
+            for cate, items in assemblyCategories.items():
                 if self.__block.IsTablePresent(cate):
                     table = self.__block.GetTable(cate)
                     if table and (table.GetNumRows() > 0):
                         valList = []
                         for item in items:
                             if table.IsColumnPresent(item):
                                 val = table(0, item)
@@ -498,11 +498,11 @@
                     ret = "NO"
                 #
                 if ret == "NO":
                     return ret
                 #
             #
             return ret
-        except Exception as _e:
+        except Exception as _e:  # noqa: F841
             traceback.print_exc(file=sys.stderr)
             return "NO"
         #
```

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/PrdSearchUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/PrdSearchUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ReportUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/ReportUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SFConvert.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/SFConvert.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SeqStatsUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/SeqStatsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SeqdbUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/SeqdbUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/UtilsBase.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/UtilsBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ValidationUtils.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/plugins/ValidationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ActionRegistry.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/process/ActionRegistry.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ActionRegistryIo.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/process/ActionRegistryIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ProcessRunner.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/process/ProcessRunner.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/WfSchemaMap.py` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/schema/WfSchemaMap.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/database_descriptions.txt` & `wwpdb_utils_wf-0.36/wwpdb/utils/wf/schema/database_descriptions.txt`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/PKG-INFO` & `wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.35.4
+Version: 0.36
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/SOURCES.txt` & `wwpdb_utils_wf-0.36/wwpdb.utils.wf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

