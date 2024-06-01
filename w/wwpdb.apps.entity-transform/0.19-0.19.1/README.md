# Comparing `tmp/wwpdb_apps_entity_transform-0.19.tar.gz` & `tmp/wwpdb_apps_entity_transform-0.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_apps_entity_transform-0.19.tar", last modified: Sun May  5 20:06:48 2024, max compression
+gzip compressed data, was "wwpdb_apps_entity_transform-0.19.1.tar", last modified: Sat Jun  1 12:42:40 2024, max compression
```

## Comparing `wwpdb_apps_entity_transform-0.19.tar` & `wwpdb_apps_entity_transform-0.19.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/
--rw-r--r--   0 vsts      (1001) docker     (127)     1099 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2439 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.499478 wwpdb_apps_entity_transform-0.19/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)     3008 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/DepictBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2941 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/LinkDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8282 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19491 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1905 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11023 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ResultDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15972 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/SeqDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17261 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/StrFormDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11305 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/openeye_util/
--rw-r--r--   0 vsts      (1001) docker     (127)    11226 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/openeye_util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/
--rw-r--r--   0 vsts      (1001) docker     (127)     6367 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/BuildPrd.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7726 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5529 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/CVSCommit.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12737 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/DepictPrd.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12192 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/DepictUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3149 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/HtmlUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13935 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/ReadFormUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4392 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/UpdatePrd.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/
--rw-r--r--   0 vsts      (1001) docker     (127)     7951 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/ChopperHandler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5917 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/CombineCoord.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2337 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/EditPolymer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/MergeLigand.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1225 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/MergePolymer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2335 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/SplitPolymer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7591 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/UpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5386 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/UpdateFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     8180 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/CommandUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3003 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/CompUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6851 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/DownloadFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)      687 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/GetLogMessage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4253 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/ImageGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6104 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/LinkUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2191 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6825 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2748 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3391 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    55983 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/EntityWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6820 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/FormPreProcess.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1099 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2601 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 20:06:36.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      194 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.651370 wwpdb_apps_entity_transform-0.19.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1101 2024-06-01 12:42:40.651370 wwpdb_apps_entity_transform-0.19.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-06-01 12:42:40.651370 wwpdb_apps_entity_transform-0.19.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2439 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.639370 wwpdb_apps_entity_transform-0.19.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.643370 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.643370 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.643370 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3008 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/DepictBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2941 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/LinkDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8270 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19491 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1905 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11023 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/ResultDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15972 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/SeqDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17259 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/StrFormDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11303 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.643370 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/openeye_util/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11226 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/openeye_util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.647370 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6367 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/BuildPrd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7726 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5529 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/CVSCommit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12737 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/DepictPrd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12192 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/DepictUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3149 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/HtmlUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13935 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/ReadFormUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4392 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/UpdatePrd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.647370 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7951 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/ChopperHandler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5916 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/CombineCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2337 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/EditPolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/MergeLigand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1225 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/MergePolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2335 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/SplitPolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7591 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/UpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5386 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/UpdateFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.647370 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8180 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/CommandUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3003 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/CompUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6851 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/DownloadFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      687 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/GetLogMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4253 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/ImageGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6104 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/LinkUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2191 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6825 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2748 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3391 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.651370 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    55983 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/webapp/EntityWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6820 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/webapp/FormPreProcess.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:40:22.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 12:42:40.651370 wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1101 2024-06-01 12:42:40.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2601 2024-06-01 12:42:40.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 12:42:40.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 12:42:25.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      194 2024-06-01 12:42:40.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-06-01 12:42:40.000000 wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/top_level.txt
```

### Comparing `wwpdb_apps_entity_transform-0.19/PKG-INFO` & `wwpdb_apps_entity_transform-0.19.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.entity_transform
-Version: 0.19
+Version: 0.19.1
 Summary: wwPDB entity transformer
 Home-page: https://github.com/rcsb/py-wwpdb_apps_entity_transform
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Dist: wwpdb.utils.config~=0.34
+Requires-Dist: wwpdb.utils.config>=0.34
 Requires-Dist: wwpdb.apps.editormodule>=0.13.1
 Requires-Dist: wwpdb.io
 Requires-Dist: wwpdb.utils.dp
 Requires-Dist: wwpdb.utils.detach
 Requires-Dist: wwpdb.utils.session
 Requires-Dist: wwpdb.utils.wf
 Requires-Dist: wwpdb.utils.oe_util
```

### Comparing `wwpdb_apps_entity_transform-0.19/setup.py` & `wwpdb_apps_entity_transform-0.19.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     #
-    install_requires=['wwpdb.utils.config ~= 0.34', 'wwpdb.apps.editormodule >= 0.13.1',
+    install_requires=['wwpdb.utils.config >= 0.34', 'wwpdb.apps.editormodule >= 0.13.1',
                       'wwpdb.io', 'wwpdb.utils.dp', 'wwpdb.utils.detach',
                       'wwpdb.utils.session', 'wwpdb.utils.wf',
                       'wwpdb.utils.oe_util'],
     packages=find_packages(exclude=['wwpdb.apps.tests-entity_transform',
                                     'mock-data']),
     # Enables Manifest to be used
     # include_package_data = True,
```

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/DepictBase.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/DepictBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/LinkDepict.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/LinkDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,33 +57,33 @@
         #
         text += self.__depiction(self.__data) + '\n'
         #
         text += '<li><a class="fltlft" href="/service/entity/summary_view?' + input_data + '" target="_blank"> Access to split or merge </a></li>\n'
         #
         if self.__splitPolymerResidueFlag:
             text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data + '&type=split" target="_blank"> ' \
-                  + '<span style="color:red;">Split modified residue to standard residue + modification in polymer</span> </a></li>\n'
+                + '<span style="color:red;">Split modified residue to standard residue + modification in polymer</span> </a></li>\n'
         #
         if self.__combResidueFlag:
             text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data + '&type=merge" target="_blank"> ' \
-                  + '<span style="color:red;">Merge standard amino acid residue + modification to modified amino acid residue in polymer</span> </a></li>\n'
+                + '<span style="color:red;">Merge standard amino acid residue + modification to modified amino acid residue in polymer</span> </a></li>\n'
         #
         if self.__matchResultFlag:
             text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data \
-                  + '" target="_blank"> <span style="color:red;">View All Search Result(s)</span> </a></li>\n'
+                + '" target="_blank"> <span style="color:red;">View All Search Result(s)</span> </a></li>\n'
         #
         if self.__graphmatchResultFlag:
             text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data \
-                  + '&type=match" target="_blank"> Update Coordinate File with Match Result(s) </a></li>\n'
+                + '&type=match" target="_blank"> Update Coordinate File with Match Result(s) </a></li>\n'
         #
         text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data \
-              + '&type=input" target="_blank"> Update Coordinate File with Input IDs </a></li>\n'
+            + '&type=input" target="_blank"> Update Coordinate File with Input IDs </a></li>\n'
         #
         text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data + '&type=split_with_input" target="_blank"> ' \
-              + 'Split non standard residue in polymer </a></li>\n'
+            + 'Split non standard residue in polymer </a></li>\n'
         #
         text += '<li><a class="fltlft" href="/service/entity/download_file?' + input_data + '" target="_blank"> Download Files </a></li>\n'
         #
         text += '</ul>\n'
         #
         return text
```

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ResultDepict.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/ResultDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/SeqDepict.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/SeqDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/StrFormDepict.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/StrFormDepict.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         #
         return self._processTemplate('chopper/editor_tmplt.html', myD)
 
     def __processSplitWithChopper(self, myD):
         ciffile = self._identifier + '_model_P1.cif'
         residueId = str(self._reqObj.getValue('split_polymer_residue'))
         if not residueId:
-            residueId = '_'.join([str(self._reqObj.getValue('chain_id')), str(self._reqObj.getValue('res_name')), \
+            residueId = '_'.join([str(self._reqObj.getValue('chain_id')), str(self._reqObj.getValue('res_name')),
                                   str(self._reqObj.getValue('res_num')), str(self._reqObj.getValue('ins_code'))])
         #
         combObj = CombineCoord(reqObj=self._reqObj, instList=[residueId], cifFile=ciffile, verbose=self._verbose, log=self._lfh)
         combObj.processWithCopy(submitValue=self.__submitValue)
         message = combObj.getMessage()
         #
         if message:
```

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         text += '</table>\n'
         return text
 
     def __depictionLigand(self):
         text = '<table>\n'
         text += '<tr>\n'
         text += '<th>Selection/<br/>User Defined Group ID<br/><input id="ligand_select_all" value="Select All" type="button" onClick="select_ligand(' \
-              + "'ligand_select_all'" + ');" /></th>\n'
+            + "'ligand_select_all'" + ');" /></th>\n'
         text += '<th>3 Letter Code</th>\n'
         text += '<th>Chain ID</th>\n'
         text += '<th>ResNum</th>\n'
         text += '<th>InsertCode</th>\n'
         text += '<th>Links</th>\n'
         text += '</tr>\n'
         #
```

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/BuildPrd.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/BuildPrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/CVSCommit.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/CVSCommit.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/DepictPrd.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/DepictPrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/DepictUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/DepictUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/HtmlUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/HtmlUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/ReadFormUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/ReadFormUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/UpdatePrd.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/prd/UpdatePrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/ChopperHandler.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/ChopperHandler.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/CombineCoord.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/CombineCoord.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def processWithCopy(self, submitValue=''):
         #
         self.__submitValue = submitValue
         #
         if self.__submitValue and (len(self.__instList) == 1) and self.__instList[0]:
             pickleFilePath = os.path.join(self.__instancePath, self.__instId + ".pkl")
             if os.access(pickleFilePath, os.F_OK):
-                 os.remove(pickleFilePath)
+                os.remove(pickleFilePath)
             #
             pickleD = {}
             pickleD['residue'] = self.__instList[0]
             pickleD['submit'] = self.__submitValue
             #
             fb = open(pickleFilePath, "wb")
             pickle.dump(pickleD, fb)
```

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/EditPolymer.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/EditPolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/MergeLigand.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/MergeLigand.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/MergePolymer.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/MergePolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/SplitPolymer.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/SplitPolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/UpdateBase.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/UpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/UpdateFile.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/update/UpdateFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/CommandUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/CommandUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/CompUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/CompUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/DownloadFile.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/DownloadFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/GetLogMessage.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/GetLogMessage.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/ImageGenerator.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/ImageGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/LinkUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/LinkUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/mmCIFUtil.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/utils/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/EntityWebApp.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/webapp/EntityWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/FormPreProcess.py` & `wwpdb_apps_entity_transform-0.19.1/wwpdb/apps/entity_transform/webapp/FormPreProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/PKG-INFO` & `wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.entity_transform
-Version: 0.19
+Version: 0.19.1
 Summary: wwPDB entity transformer
 Home-page: https://github.com/rcsb/py-wwpdb_apps_entity_transform
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Requires-Dist: wwpdb.utils.config~=0.34
+Requires-Dist: wwpdb.utils.config>=0.34
 Requires-Dist: wwpdb.apps.editormodule>=0.13.1
 Requires-Dist: wwpdb.io
 Requires-Dist: wwpdb.utils.dp
 Requires-Dist: wwpdb.utils.detach
 Requires-Dist: wwpdb.utils.session
 Requires-Dist: wwpdb.utils.wf
 Requires-Dist: wwpdb.utils.oe_util
```

### Comparing `wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/SOURCES.txt` & `wwpdb_apps_entity_transform-0.19.1/wwpdb.apps.entity_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

