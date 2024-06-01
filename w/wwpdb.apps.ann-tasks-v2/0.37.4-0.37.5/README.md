# Comparing `tmp/wwpdb_apps_ann_tasks_v2-0.37.4.tar.gz` & `tmp/wwpdb_apps_ann_tasks_v2-0.37.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_apps_ann_tasks_v2-0.37.4.tar", last modified: Sun May  5 19:37:31 2024, max compression
+gzip compressed data, was "wwpdb_apps_ann_tasks_v2-0.37.5.tar", last modified: Sat Jun  1 13:10:06 2024, max compression
```

## Comparing `wwpdb_apps_ann_tasks_v2-0.37.4.tar` & `wwpdb_apps_ann_tasks_v2-0.37.5.tar`

### file list

```diff
@@ -1,151 +1,152 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2540 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.502959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/
--rw-r--r--   0 vsts      (1001) docker     (127)    39726 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46849 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/
--rw-r--r--   0 vsts      (1001) docker     (127)     5712 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/Check.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4344 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3138 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6865 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/
--rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33977 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16936 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/density/
--rw-r--r--   0 vsts      (1001) docker     (127)      998 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/density/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)     3945 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/
--rw-r--r--   0 vsts      (1001) docker     (127)     2573 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4448 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4053 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19613 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5646 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/
--rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14499 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2942 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3345 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12364 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12679 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/
--rw-r--r--   0 vsts      (1001) docker     (127)    10620 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12969 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18806 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11248 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/
--rw-r--r--   0 vsts      (1001) docker     (127)    15912 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9923 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/link/
--rw-r--r--   0 vsts      (1001) docker     (127)     3057 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/link/Link.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/link/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/
--rw-r--r--   0 vsts      (1001) docker     (127)     3231 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4323 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4763 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5394 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4764 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3305 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3716 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3561 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nafeatures/
--rw-r--r--   0 vsts      (1001) docker     (127)     2610 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/
--rw-r--r--   0 vsts      (1001) docker     (127)    21849 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8475 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3526 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/
--rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2010 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/Related.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/
--rw-r--r--   0 vsts      (1001) docker     (127)     8902 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25640 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/
--rw-r--r--   0 vsts      (1001) docker     (127)     8612 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1983 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/LinksReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    79069 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34873 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/secstruct/
--rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/site/
--rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/site/Site.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/site/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/solvent/
--rw-r--r--   0 vsts      (1001) docker     (127)     3037 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/status/
--rw-r--r--   0 vsts      (1001) docker     (127)    33282 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/status/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/transformCoord/
--rw-r--r--   0 vsts      (1001) docker     (127)     3759 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     6619 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6242 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1509 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3451 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4026 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8388 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3396 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4790 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3021 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4071 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3062 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3053 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/validate/
--rw-r--r--   0 vsts      (1001) docker     (127)    10304 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/validate/Validate.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/validate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/view3d/
--rw-r--r--   0 vsts      (1001) docker     (127)     5085 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)     5627 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46092 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)   179598 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15321 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65098 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16955 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5590 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 19:36:48.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.636595 wwpdb_apps_ann_tasks_v2-0.37.5/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-06-01 13:10:06.636595 wwpdb_apps_ann_tasks_v2-0.37.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-06-01 13:10:06.636595 wwpdb_apps_ann_tasks_v2-0.37.5/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2540 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.620594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.620594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.620594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.620594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/assembly/
+-rw-r--r--   0 vsts      (1001) docker     (127)    39726 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46849 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.624594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5711 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/Check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4344 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3138 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6864 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.624594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/correspnd/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34397 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16936 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.624594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/density/
+-rw-r--r--   0 vsts      (1001) docker     (127)      998 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/density/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.624594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3945 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.624594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2573 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4448 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4053 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19613 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5646 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.624594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14498 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2942 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3345 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12363 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12678 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.628594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11212 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12969 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18806 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11248 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.628594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15910 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9923 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.628594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/link/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3057 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/link/Link.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/link/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.628594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3231 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4323 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4763 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5394 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4764 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3305 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3716 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3561 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.628594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nafeatures/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2610 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.628594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21849 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8475 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3526 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.628594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/related/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2010 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/related/Related.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/related/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.628594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9738 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25923 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8612 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1805 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/LinksReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    79069 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43133 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/PdbxEmExtensionCategoryStyle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36705 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/secstruct/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/site/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/site/Site.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/site/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/solvent/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3037 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/status/
+-rw-r--r--   0 vsts      (1001) docker     (127)    33282 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/status/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/transformCoord/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3759 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6619 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6242 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1509 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3451 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4026 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8387 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3396 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4790 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3021 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4071 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3062 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3053 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/validate/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10304 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/validate/Validate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/validate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.632594 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/view3d/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5085 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.636595 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5627 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46092 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   180943 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15464 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65460 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16955 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 13:07:34.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 13:10:06.636595 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-06-01 13:10:06.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5660 2024-06-01 13:10:06.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 13:10:06.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 13:09:22.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-06-01 13:10:06.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-06-01 13:10:06.000000 wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/PKG-INFO` & `wwpdb_apps_ann_tasks_v2-0.37.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann_tasks_v2
-Version: 0.37.4
+Version: 0.37.5
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
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
-Requires-Dist: wwpdb.utils.config~=0.37
+Requires-Dist: wwpdb.utils.config>=0.37
 Requires-Dist: wwpdb.apps.wf_engine
 Requires-Dist: wwpdb.io
 Requires-Dist: wwpdb.utils.db>=0.6
 Requires-Dist: wwpdb.utils.emdb~=1.0
 Requires-Dist: wwpdb.utils.wf~=0.13
 Requires-Dist: wwpdb.utils.session
 Requires-Dist: mmcif>=0.25
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/setup.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     #
     install_requires=[
-        "wwpdb.utils.config ~= 0.37",
+        "wwpdb.utils.config >= 0.37",
         "wwpdb.apps.wf_engine",
         "wwpdb.io",
         "wwpdb.utils.db >= 0.6",
         "wwpdb.utils.emdb ~= 1.0",
         "wwpdb.utils.wf ~= 0.13",
         "wwpdb.utils.session",
         "mmcif >= 0.25",
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/Check.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/Check.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import inspect
 
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 from wwpdb.apps.ann_tasks_v2.utils.PublicPdbxFile import PublicPdbxFile
 
 
 class Check(PublicPdbxFile):
-
     """
     Encapsulates dictioanry-level PDBx/mmCIF checking.
 
     Operations are performed in the current session context defined in the input
     reqObj().
 
     """
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import inspect
 
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 from wwpdb.apps.ann_tasks_v2.utils.PublicPdbxFile import PublicPdbxFile
 
 
 class XmlCheck(PublicPdbxFile):
-
     """
     Encapsulates PDBML/XML checking.
     """
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
         super(XmlCheck, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
         self.__reportPath = None
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,15 +509,18 @@
         enc = self.__getEncourage()
         myD["letter_encourage"] = "\n\n" + enc if enc else ""
 
         myD["major"] = self.__letterTemplateMap["major"]
         myD["major_release"] = self.__letterTemplateMap["major_release"]
         myD["major_minor_addition"] = self.__letterTemplateMap["major_minor_addition"]
         myD["minor"] = self.__letterTemplateMap["minor"]
-        myD["minor_release"] = self.__getRelaseInfo()
+        myD["minor_release"], is_repl_rel = self.__getRelaseInfo()
+        if is_repl_rel:
+            myD["major_release"] = self.__letterTemplateMap["release_repl_rel"]
+        #
         myD["letter_footer"] = self.__letterTemplateMap["signature"]
         myD["slection_text"] = self.__getSlectionText(selectD, additionalD)
         myD["text_map"] = self.__javascript_text_mapping
         if self.__EmMapOnly:
             # For map only deposition, encouragement is in the header already.
             myD["full_text"] = myD["letter_header"]
         elif major_text != "":
@@ -707,33 +710,40 @@
                 return None
 
         # Not EM and not NMR -- Xray
         return self.__letterTemplateMap["encourage_xray"]
 
     def __getRelaseInfo(self):
         text = ""
+        is_repl_rel = False
+        #
         author_release_status_code = self.__corresInfo["author_release_status_code"]
         #
         if author_release_status_code == "HOLD":
             text += self.__letterTemplateMap["release_hold"] % self.__corresInfo
         elif author_release_status_code == "HPUB":
             text += self.__letterTemplateMap["release_hpub"]
         elif author_release_status_code == "REL":
             text += self.__letterTemplateMap["release_rel"]
+        elif author_release_status_code == "REPL_REL":
+            text += self.__letterTemplateMap["release_repl_rel"]
+            is_repl_rel = True
         else:
             text += self.__letterTemplateMap["release_unknown"]
         #
-        text += "\n\n"
-        sequence_code = self.__corresInfo["author_release_sequence_code"]
-        if sequence_code == "RELEASE NOW":
-            text += self.__letterTemplateMap["pre_release_yes"]
-        else:
-            text += self.__letterTemplateMap["pre_release_no"]
+        if author_release_status_code != "REPL_REL":
+            text += "\n\n"
+            sequence_code = self.__corresInfo["author_release_sequence_code"]
+            if sequence_code == "RELEASE NOW":
+                text += self.__letterTemplateMap["pre_release_yes"]
+            else:
+                text += self.__letterTemplateMap["pre_release_no"]
+            #
         #
-        return text
+        return text, is_repl_rel
 
     def __getTableContext(self, count):
         text = ""
         for ldir in self.__ligandInfo:
             label = "ID: " + ldir["id"]
             if "original_id" in ldir:
                 label += " &nbsp; &nbsp; ( Original ID: " + ldir["original_id"] + " )"
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 from wwpdb.io.locator.PathInfo import PathInfo
 from wwpdb.io.locator.DataReference import ReferenceFileComponents
 from wwpdb.apps.ann_tasks_v2.utils.SessionWebDownloadUtils import SessionWebDownloadUtils
 
 
 class EmEditUtils(SessionWebDownloadUtils):
-
     """
     Edit volume data file header records and related data stored in model files.
 
     """
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
         super(EmEditUtils, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from mmcif_utils.style.PdbxEmExtensionCategoryStyle import PdbxEmExtensionCategoryStyle
 from mmcif.io.IoAdapterCore import IoAdapterCore
 
 #
 
 
 class EmModelUtils(PdbxStyleIoUtil):
-
     """
     Manage map header updates in model file -
 
     Here are the model data items with direct correspondences with binary map header -
 
 
         The following items are exported in JSON object from the one of the various mapfix applications -
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 import matplotlib.pyplot as plt  # noqa: E402
 
 import pygal  # noqa: E402
 from pygal.style import LightGreenStyle  # noqa: E402
 
 
 class EmUtils(SessionWebDownloadUtils):
-
     """
     Manages mapfix (view and edit) and em2m operations.
 
     """
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
         super(EmUtils, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,24 +90,29 @@
         self.__sessionPath = self.__sObj.getPath()
         self.__status = "none"
         #
         self.__mtzLogPath = os.path.join(self.__sessionPath, "mtzdmp.log")
         self.__htmlPath = os.path.join(self.__sessionPath, "get_mtz_infor.html")
         self.__sfInfoPath = os.path.join(self.__sessionPath, "sf_information.cif")
 
-    def __bashSetting(self):
+    def __bashSetting(self, html=False):
         setting = (
             " PACKAGE_DIR="
             + self.__packagePath
             + "; export PACKAGE_DIR; "
             + " SF_PATH=${PACKAGE_DIR}/sf-valid; export SF_PATH; "
             + " CCP4_PATH=${PACKAGE_DIR}/ccp4; export CCP4_PATH; "
             + " PHENIX_PATH=${PACKAGE_DIR}/phenix; export PHENIX_PATH; "
-            + " source ${CCP4_PATH}/bin/ccp4.setup.sh; source ${PHENIX_PATH}/phenix_env.sh; ${SF_PATH}/bin/sf_convert "
+            + " source ${CCP4_PATH}/bin/ccp4.setup.sh; source ${PHENIX_PATH}/phenix_env.sh; "
         )
+
+        if html:
+            setting += "${SF_PATH}/bin/sf_convert_html "
+        else:
+            setting += "${SF_PATH}/bin/sf_convert "
         return setting
 
     def __generateInputForm(self, logPath):
         """ """
         options = (
             " -mtz_man_html "
             + self.__mtzDataSet
@@ -117,15 +122,15 @@
             + self.__topSessionPath
             + " -cgi_bin  /cgi-bin/ -sf "
             + self.__mtzFileName
             + " > "
             + logPath
             + " 2>&1 ; "
         )
-        self.__runCmd(options)
+        self.__runCmd(options, html=True)
         #
         if os.access(self.__mtzLogPath, os.R_OK) and os.access(self.__htmlPath, os.R_OK):
             cmd = "cat " + self.__mtzLogPath + " >> " + logPath + " ; "
             os.system(cmd)
             self.addDownloadPath(logPath)
             #
             self.__readHtmlText()
@@ -161,17 +166,19 @@
             #
             self.__status = "ok"
             return True
         #
         self.__status = "error"
         return False
 
-    def __runCmd(self, options):
+    def __runCmd(self, options, html=False):
         """ """
-        cmd = "cd " + self.__sessionPath + " ; " + self.__bashSetting() + options
+        cmd = "cd " + self.__sessionPath + " ; " + self.__bashSetting(html) + options
+        if self.__verbose:
+            self.__lfh.write("MtzTommCIF command: %s\n" % cmd)
         os.system(cmd)
 
     def __readHtmlText(self):
         """ """
         try:
             ofh = open(self.__htmlPath, "r")
             data = ofh.read()
@@ -208,15 +215,15 @@
     def __parseSemiAutoForm(self):
         """ """
         tokenNameList = [
             ["fp", " 'FP=%s', "],
             ["sigfp", " 'SIGFP=%s', "],
             ["i", " 'I=%s', "],
             ["sigi", " 'SIGI=%s', "],
-            ["free", " 'FREE=%s', "],
+            ["free", " 'FreeR_flag=%s', "],  # Gemmi will instantiate pdbx_r_free_flag as well. Undocumented feature
             ["phib", " 'PHIB=%s', "],
             ["fom", " 'FOM=%s', "],
             ["fc", " 'FC=%s', "],
             ["phic", " 'PHIC=%s', "],
             ["hla", " 'HLA=%s', "],
             ["hlb", " 'HLB=%s', "],
             ["hlc", " 'HLC=%s', "],
@@ -231,30 +238,38 @@
             ["sigfneg", " 'SIGF(-)=%s', "],
             ["dp", " 'DP=%s', "],
             ["sigdp", " 'SIGDP=%s', "],
             ["fwt", " 'FWT=%s', "],
             ["phwt", " 'PHWT=%s', "],
             ["delfwt", " 'DELFWT=%s', "],
             ["delphwt", " 'DELPHWT=%s', "],
-            ["freer", " -FREER %s , "],
+            ["freer", " -freer %s "],
         ]
         #
         items = ""
+        lastitem = None
         for i in range(self.__intDataSet):
             if (i > 0) and items:
                 items += " : "
             #
             for tokenName in tokenNameList:
                 value = self.__reqObj.getValue(tokenName[0] + "_" + str(i + 1))
                 if not value:
                     continue
                 #
-                items += tokenName[1] % value
+                # This limits us to a single rfree across multiple sets.
+                if tokenName[0] == "freer":
+                    lastitem = tokenName[1] % value
+                else:
+                    items += tokenName[1] % value
             #
         #
+        if lastitem:
+            items += lastitem
+
         return items
 
     def __getPdbId(self):
         """ """
         pdbid = "xxxx"
         try:
             modelFileName = self.__reqObj.getValue("entryfilename")
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 from mmcif.io.IoAdapterPy import IoAdapterPy
 
 # from mmcif.api.PdbxContainers import *
 
 
 class PdbxFileIo(object):
-
     """Read PDBx data files and package content as PDBx container object or container object list
     Write PDBx data using source PDBx container object list source content.
 
     PDBx container object represents
     """
 
     def __init__(self, ioObj=IoAdapterPy(), verbose=True, log=sys.stderr):
@@ -76,15 +75,14 @@
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 traceback.print_exc(file=self.__lfh)
             return False
 
 
 class ModelFileIo(object):
-
     """
     Assemble sample and coordinate sequence details from model coordinate data file.
 
     """
 
     def __init__(self, dataContainer=None, verbose=True, log=sys.stderr):
         self.__currentContainer = dataContainer
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/PisaReader.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/io/PisaReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/link/Link.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/link/Link.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/Related.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/related/Related.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 __version__ = "V0.01"
 
 import os
 import shutil
 import sys
 import traceback
 
-from wwpdb.apps.ann_tasks_v2.report.styles.PdbxIo import PdbxReportIo, PdbxGeometryReportIo, PdbxXrayExpReportIo, PdbxLinksReportIo
+from wwpdb.apps.ann_tasks_v2.report.styles.PdbxIo import PdbxReportIo, PdbxGeometryReportIo, PdbxXrayExpReportIo, PdbxLinksReportIo, EmInfoReportIo
 from mmcif_utils.style.PdbxGeometryReportCategoryStyle import PdbxGeometryReportCategoryStyle
 
 from wwpdb.apps.ann_tasks_v2.report.PdbxReportDepictBootstrap import PdbxReportDepictBootstrap
 from wwpdb.apps.ann_tasks_v2.report.styles.DCCReport import PdbxXrayExpReportCategoryStyle
 from wwpdb.apps.ann_tasks_v2.report.styles.ModelReport import PdbxReportCategoryStyle
 from wwpdb.apps.ann_tasks_v2.report.styles.LinksReport import PdbxLinksReportCategoryStyle
+from wwpdb.apps.ann_tasks_v2.report.styles.PdbxEmExtensionCategoryStyle import PdbxEmExtensionCategoryStyle
 
 
 class PdbxReport(object):
     """PDBx report generator functions."""
 
     def __init__(self, reqObj, verbose=False, log=sys.stderr):
         """PRD report generator.
@@ -106,21 +107,27 @@
                 oL = rdd.render(dd, style=layout, leadingHtmlL=leadingHtmlL, trailingHtmlL=trailingHtmlL)
 
             if contentType in ["geometry-check-report"]:
                 self.setFilePath(filePath, fileFormat=fileFormat, idCode=idCode)
                 dd = self.doReport(contentType)
                 rdd = PdbxReportDepictBootstrap(styleObject=PdbxGeometryReportCategoryStyle(), includePath=includePath, verbose=self.__verbose, log=self.__lfh)
                 oL = rdd.render(dd, style=layout, leadingHtmlL=leadingHtmlL, trailingHtmlL=trailingHtmlL)
-            
+
             if contentType in ["links-report"]:
                 self.setFilePath(filePath, fileFormat=fileFormat, idCode=idCode)
                 dd = self.doReport(contentType)
                 rdd = PdbxReportDepictBootstrap(styleObject=PdbxLinksReportCategoryStyle(), includePath=includePath, verbose=self.__verbose, log=self.__lfh)
                 oL = rdd.render(dd, style=layout, leadingHtmlL=leadingHtmlL, trailingHtmlL=trailingHtmlL)
 
+            if contentType in ["em-map-info-report"]:
+                self.setFilePath(filePath, fileFormat=fileFormat, idCode=idCode)
+                dd = self.doReport(contentType)
+                rdd = PdbxReportDepictBootstrap(styleObject=PdbxEmExtensionCategoryStyle(), includePath=includePath, verbose=self.__verbose, log=self.__lfh)
+                oL = rdd.render(dd, style=layout, leadingHtmlL=leadingHtmlL, trailingHtmlL=trailingHtmlL)
+
             if self.__debug:
                 self.__lfh.write("+PdbxReport.makeTabularReport - generated HTML \n%s\n" % "\n".join(oL))
 
         return oL
 
     def setFilePath(self, filePath, fileFormat="cif", idCode=None):
         self.__filePath = filePath
@@ -178,14 +185,19 @@
                 pdbxR = PdbxReportIo(verbose=self.__verbose, log=self.__lfh)
             elif contentType == "geometry-check-report":
                 pdbxR = PdbxGeometryReportIo(verbose=self.__verbose, log=self.__lfh)
             elif contentType == "dcc-report":
                 pdbxR = PdbxXrayExpReportIo(verbose=self.__verbose, log=self.__lfh)
             elif contentType == "links-report":
                 pdbxR = PdbxLinksReportIo(verbose=self.__verbose, log=self.__lfh)
+            elif contentType == "em-map-info-report":
+                pdbxR = EmInfoReportIo(verbose=self.__verbose, log=self.__lfh)
+            else:
+                self.__lfh.write("+PdbxReport.doReport() - unknown contentType %s\n" % contentType)
+                return oD
 
             pdbxR.setFilePath(localPath, idCode=None)
             pdbxR.get()
             oD["blockId"] = pdbxR.getCurrentContainerId()
             if self.__verbose:
                 self.__lfh.write("+PdbxReport.doReport() - category name list %r \n" % pdbxR.getCurrentCategoryNameList())
             for catName in pdbxR.getCurrentCategoryNameList():
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 class PdbxReportDepictBootstrap(PdbxDepictBootstrapBase):
     """Create tabular HTML reports from PDBx data files.
 
     This version uses Bootstrap CSS framework constructs.
 
     """
+
     MAX_LINES = 12
 
     def __init__(self, styleObject=None, includePath=None, verbose=False, log=sys.stderr):
         """
         :param `styleObject`:  object containing report data and formatting details.
         :param `includePath`:  path to web application html include files.
         :param `verbose`:      boolean flag to activate verbose logging.
@@ -132,14 +133,20 @@
                 ("pdbx_validate_polymer_linkage", "Polymer linkages", "row-wise"),
                 ("pdbx_validate_chiral", "Chirality exceptions", "row-wise"),
             ]
         elif self.__st.getStyleId() in ["PDBX_LINKS_REPORT_V1"]:
             self.__reportCategories = [
                 ("struct_conn", "", "row-wise"),
             ]
+        elif self.__st.getStyleId() in ["PDBX_STYLE_EmExtension_V1"]:
+            self.__reportCategories = [
+                ("em_map", "", "row-wise"),
+            ]
+        else:
+            self.__lfh.write("Error: PdbxReportDepict.__setup unknown style %s\n" % self.__st.getStyleId())
 
     def render(self, eD, style="tabs", leadingHtmlL=None, trailingHtmlL=None):
         """ """
         if style in ["tabs"]:
             return self.__doRenderTabs(eD)
         elif style in ["accordion", "multiaccordion"]:
             return self.__doRenderAccordion(eD)
@@ -534,15 +541,15 @@
             if itemName in rD:
                 itemValue = rD[itemName]
                 if len(itemValue) >= 3:
                     rD[itemName] = '<a target="_blank" href="http://ligand-expo.rcsb.org/pyapps/ldHandler.py?formid=cc-index-search&operation=ccid&target=%s">%s</a>' % (
                         itemValue,
                         itemValue,
                     )
-        
+
         if catName == "struct_conn":
             itemName = "_struct_conn.id"
             if itemName in rD:
                 itemValue = rD[itemName]
                 rD[itemName] = '<a href="#" onclick="inspect(\'%s\'); return false;">%s</button>' % (
                     itemValue.strip(),
                     itemValue,
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/LinksReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/LinksReport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 Report style details for PDBx struct_conn category.
 
 """
 
-
 from mmcif_utils.style.PdbxCategoryStyleBase import PdbxCategoryStyleBase
 
 
 class PdbxLinksReportCategoryStyle(PdbxCategoryStyleBase):
     _styleId = "PDBX_LINKS_REPORT_V1"
     _categoryInfo = [
         ("struct_conn", "table"),
     ]
     _cDict = {
         "struct_conn": [
-            ('_struct_conn.id', '%s', 'str', ''),
+            ("_struct_conn.id", "%s", "str", ""),
             ("_struct_conn.pdbx_leaving_atom_flag", "%s", "str", ""),
             ("_struct_conn.ptnr1_auth_asym_id", "%s", "str", ""),
             ("_struct_conn.ptnr1_auth_comp_id", "%s", "str", ""),
             ("_struct_conn.ptnr1_auth_seq_id", "%s", "str", ""),
             ("_struct_conn.ptnr1_symmetry", "%s", "str", ""),
             ("_struct_conn.pdbx_ptnr1_label_alt_id", "%s", "str", ""),
             ("_struct_conn.pdbx_ptnr1_PDB_ins_code", "%s", "str", ""),
@@ -32,12 +31,14 @@
         ],
     }
     _excludeList = []
     _suppressList = []
     #
 
     def __init__(self):
-        super(PdbxLinksReportCategoryStyle, self).__init__(styleId=PdbxLinksReportCategoryStyle._styleId,
-                                                              catFormatL=PdbxLinksReportCategoryStyle._categoryInfo,
-                                                              catItemD=PdbxLinksReportCategoryStyle._cDict,
-                                                              excludeList=PdbxLinksReportCategoryStyle._excludeList,
-                                                              suppressList=PdbxLinksReportCategoryStyle._suppressList)
+        super(PdbxLinksReportCategoryStyle, self).__init__(
+            styleId=PdbxLinksReportCategoryStyle._styleId,
+            catFormatL=PdbxLinksReportCategoryStyle._categoryInfo,
+            catItemD=PdbxLinksReportCategoryStyle._cDict,
+            excludeList=PdbxLinksReportCategoryStyle._excludeList,
+            suppressList=PdbxLinksReportCategoryStyle._suppressList,
+        )
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 # from mmcif_utils.style.PdbxXrayExpReportCategoryStyle import PdbxXrayExpReportCategoryStyle
 from wwpdb.apps.ann_tasks_v2.report.styles.DCCReport import PdbxXrayExpReportCategoryStyle
 
 # from mmcif_utils.style.PdbxReportCategoryStyle import PdbxReportCategoryStyle
 from wwpdb.apps.ann_tasks_v2.report.styles.ModelReport import PdbxReportCategoryStyle
 from wwpdb.apps.ann_tasks_v2.report.styles.LinksReport import PdbxLinksReportCategoryStyle
+from wwpdb.apps.ann_tasks_v2.report.styles.PdbxEmExtensionCategoryStyle import PdbxEmExtensionCategoryStyle
 
 logger = logging.getLogger()
 
 
 class PdbxReportIo(PdbxStyleIoUtil):
     """Methods for reading PDBx data files for reporting applications including style details."""
 
@@ -850,14 +851,69 @@
         else:
             return False
 
     def get(self):
         """
         Check for a valid current data container.
 
+        Returns True for success or False otherwise.
+        """
+        return self.getCurrentContainerId() is not None
+
+    def complyStyle(self):
+        return self.testStyleComplete(self.__lfh)
+
+    def setBlock(self, blockId):
+        return self.setContainer(containerName=blockId)
+
+    def newBlock(self, blockId):
+        return self.newContainer(containerName=blockId)
+
+    def update(self, catName, attributeName, value, iRow=0):
+        return self.updateAttribute(catName, attributeName, value, iRow=iRow)
+
+    def write(self, filePath):
+        return self.writeFile(filePath)
+
+
+class EmInfoReportIo(PdbxStyleIoUtil):
+    """Methods for reading EM information details."""
+
+    def __init__(self, verbose=True, log=sys.stderr):
+        super(EmInfoReportIo, self).__init__(styleObject=PdbxEmExtensionCategoryStyle(), verbose=verbose, log=log)
+
+        # self.__verbose = verbose
+        # self.__debug = False
+        self.__lfh = log
+        #
+        self.__filePath = None
+
+        self.__idCode = None
+
+    def getCategory(self, catName="entity"):
+        return self.getItemDictList(catName)
+
+    def setFilePath(self, filePath, idCode=None):
+        """Specify the file path for the target and optionally provide an identifier
+        for the data section within the file.
+        """
+        self.__filePath = filePath
+        self.__idCode = idCode
+        if self.readFile(self.__filePath):
+            if self.__idCode is not None:
+                return self.setContainer(containerName=self.__idCode)
+            else:
+                return self.setContainer(containerIndex=0)
+        else:
+            return False
+
+    def get(self):
+        """
+        Check for a valid current data container.
+
         Returns True for success or False otherwise.
         """
         return self.getCurrentContainerId() is not None
 
     def complyStyle(self):
         return self.testStyleComplete(self.__lfh)
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/site/Site.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/site/Site.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 import logging
 
 logger = logging.getLogger()
 
 
 class StatusUpdate(object):
-
     """Update release status items."""
 
     def __init__(self, reqObj, IoAdapter=IoAdapterCore(), verbose=False, log=sys.stderr):
         """
         :param `verbose`:  boolean flag to activate verbose logging.
         :param `log`:      stream for logging.
 
@@ -256,15 +255,15 @@
             "obsoleted_date",
             "details",
             "last_update",
             "map_release_date",
             "map_hold_date",
             "header_release_date",
             "replace_existing_entry_flag",
-            "title"
+            "title",
             # Do not add process_site here.  Handled internally below
         ]
 
         depuiAttributeNameList = ["depositor_hold_instructions"]
 
         try:
             dcObj = cObj.getObj("pdbx_database_status")
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import traceback
 
 from wwpdb.io.locator.PathInfo import PathInfo
 from wwpdb.io.locator.DataReference import ReferenceFileComponents
 
 
 class SessionDownloadUtils(object):
-
     """Common methods for managing download operations for project files within the session context."""
 
     #
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
         """Input request object is used to determine session context."""
         self.__verbose = verbose
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/validate/Validate.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/validate/Validate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -2110,14 +2110,15 @@
             "dict-check-report",
             "dict-check-report-r4",
             "dict-check-report-next",
             "xml-check-report",
             "special-position-report",
             "emd-xml-header-report",
             "em-map-check-report",
+            "em-map-info-report",
             "downloads",
         ]:
             myD[ky] = None
         myD["entry-info"] = {
             "pdb_id": "",
             "struct_title": "",
             "my_entry_id": entryId,
@@ -2293,14 +2294,37 @@
                 ok = du.fetchId(entryId, contentType="em-map-check-report", formatType="txt", fileSource=fileSource, instance=instance)
                 if ok:
                     downloadPath = du.getDownloadPath()
                     aTagList.append(du.getAnchorTag())
                     myD[cT] = self.__getFileTextWithMarkup(downloadPath)
                 else:
                     myD[cT] = self.__getMessageTextWithMarkup("")
+            elif cT == "em-map-info-report":
+                if useModelFileVersion:
+                    versionId = "latest"
+                else:
+                    versionId = "none"
+
+                # Try to avoid fetch if not needed
+                downloadPath = du.getFilePath(entryId, contentType="model", formatType="pdbx", fileSource=fileSource, instance=instance, versionId=versionId)
+                if downloadPath is None or not os.path.exists(downloadPath):
+                    ok = du.fetchId(entryId, contentType="model", formatType="pdbx", fileSource=fileSource, instance=instance, versionId=versionId)
+                    downloadPath = du.getDownloadPath()
+                else:
+                    ok = True
+                if ok:
+                    aTagList.append(du.getAnchorTag())
+                    myD[cT] = "\n".join(pR.makeTabularReport(filePath=downloadPath, contentType="em-map-info-report", idCode=entryId, layout=layout))
+                else:
+                    myD[cT] = self.__getMessageTextWithMarkup("None")
+            elif cT == "downloads":
+                # We call this a "report type" - might not be correct...
+                pass
+            else:
+                self._lfh.write("+CommonTasksWebAppWorker._renderCheckReports() unknown report %r\n" % cT)
 
         # downloads
 
         for data_file in (
             ("model", "pdbx"),
             ("model", "pdb"),
             ("structure-factors", "pdbx"),
@@ -2696,15 +2720,15 @@
                 "check-geometry",
                 "check-special-position",
                 "check-sf",
                 "check-emd-xml",
                 "check-em-map",
             ]
             aTagList = self._makeCheckReports([entryId], operationList=opList, fileSource=fileSource, useFileVersions=useFileVersions)
-            cTList = ["model"]
+            cTList = ["model", "em-map-info-report"]
             cTList.extend(sorted(opCtD.values()))
             if self._verbose:
                 self._lfh.write("+ReviewDataWebAppWorker._reviewDataInlineIdOps() content type list %r\n" % cTList)
             myD = self._renderCheckReports(entryId, fileSource="session-download", instance=None, contentTypeList=cTList, useModelFileVersion=useFileVersions)
             rC.setHtmlTextFromTemplate(templateFilePath=templateFilePath, webIncludePath=webIncludePath, parameterDict=myD, insertContext=True)
             rC.setStatus(statusMsg="Check reports completed")
         else:
@@ -3723,31 +3747,29 @@
 
         if self._verbose:
             self._lfh.write("+CommonTasksWebAppWorker._launchFromIdcodeOp() completed for identifier %s\n" % identifier)
         #
         return rC
 
     def _autoProcessNmrCombinedDataFile(self, identifier):
-        """
-        """
+        """ """
         if self._verbose:
             self._lfh.write("+CommonTasksWebAppWorker._autoProcessNmrCombinedDataFile() starting with identifier %s\n" % identifier)
         #
         try:
             csUtil = NmrChemShiftProcessUtils(siteId=self._siteId, verbose=self._verbose, log=self._lfh)
             csUtil.setWorkingDirPath(dirPath=self._sessionPath)
             csUtil.setIdentifier(identifier=identifier)
             csUtil.runNefProcess(identifier=identifier)
         except:  # noqa: E722 pylint: disable=bare-except
             traceback.print_exc(file=self._lfh)
         #
 
     def _autoProcessNmrChemShifts(self, identifier):
-        """
-        """
+        """ """
         try:
             csUtil = NmrChemShiftProcessUtils(siteId=self._siteId, verbose=self._verbose, log=self._lfh)
             csUtil.setWorkingDirPath(dirPath=self._sessionPath)
             csUtil.setIdentifier(identifier=identifier, nmrDataFlag=False)
             csUtil.run()
         except:  # noqa: E722 pylint: disable=bare-except
             traceback.print_exc(file=self._lfh)
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
             self._lfh.write("+ReviewDataWebAppWorker._updateAndReportFileOps() starting with op %s\n" % operation)
 
         isFile = False
 
         rC = ResponseContent(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
         rC.setReturnFormat("json")
 
+        contentType = contentFormat = partitionNumber = None
         if self._isFileUpload():
             # make a copy of the file in the session directory and set 'fileName'
             self._uploadFile()
             fileName = self._reqObj.getValue("fileName")
             filePath = os.path.join(self._sessionPath, fileName)
             (_rootName, _ext) = os.path.splitext(fileName)
             isFile = True
@@ -145,14 +146,15 @@
         if not isFile or fileName is None or len(fileName) < 1:
             rC.setError(errMsg="File upload failed.")
 
         elif operation in ["report"]:
             #
             pR = PdbxReport(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
             aTagList.append(du.getAnchorTag())
+            downloadPath = du.getDownloadPath()
             layout = "multiaccordion"
             htmlList.extend(pR.makeTabularReport(filePath=downloadPath, contentType=contentType, idCode=idCode, layout=layout))
             if len(aTagList) > 0:
                 rC.setHtmlLinkText('<span class="url-list">Download: %s</span>' % ",".join(aTagList))
                 rC.setHtmlList(htmlList)
                 rC.setStatus(statusMsg="Reports completed")
             else:
@@ -336,14 +338,15 @@
             "misc-check-report",
             "format-check-report",
             "dict-check-report",
             "xml-check-report",
             # 'model-pdb',
             "emd-xml-header-report",
             "em-map-check-report",
+            "em-map-info-report",
             "downloads",
         ]
         reportD = self._renderCheckReports(idCode, fileSource=fileSource, instance=instance, contentTypeList=cTL)
         #
         reportD["sessionid"] = self._reqObj.getSessionId()
         reportD["entryid"] = idCode
         #
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,20 @@
             postRelStatusCode = sUD["postRelStatus"]
 
             if self._verbose:
                 self._lfh.write(
                     "\n+%s.%s starting with identifier %s statusCode %r authRelCode %r annotatorId %r\n"
                     % (self.__class__.__name__, inspect.currentframe().f_code.co_name, identifier, statusCode, authRelCode, annotatorId)
                 )
+        else:
+            self._lfh.write("\n+%s.%s ERROR failing to fetchId %s\n"
+                            % (self.__class__.__name__, inspect.currentframe().f_code.co_name, identifier))
+            rC = ResponseContent(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
+            rC.setError("Unable to decipher identifier")
+            return rC
 
         # Prepare the Startup data items
         myD = {}
         myD["entryid"] = identifier
         myD["sessionid"] = self._sessionId
         myD["annotatorid"] = annotatorId
         myD["startannotator"] = origAnnotator
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann_tasks_v2
-Version: 0.37.4
+Version: 0.37.5
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
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
-Requires-Dist: wwpdb.utils.config~=0.37
+Requires-Dist: wwpdb.utils.config>=0.37
 Requires-Dist: wwpdb.apps.wf_engine
 Requires-Dist: wwpdb.io
 Requires-Dist: wwpdb.utils.db>=0.6
 Requires-Dist: wwpdb.utils.emdb~=1.0
 Requires-Dist: wwpdb.utils.wf~=0.13
 Requires-Dist: wwpdb.utils.session
 Requires-Dist: mmcif>=0.25
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt` & `wwpdb_apps_ann_tasks_v2-0.37.5/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 wwpdb/apps/ann_tasks_v2/related/__init__.py
 wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
 wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
 wwpdb/apps/ann_tasks_v2/report/__init__.py
 wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
 wwpdb/apps/ann_tasks_v2/report/styles/LinksReport.py
 wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
+wwpdb/apps/ann_tasks_v2/report/styles/PdbxEmExtensionCategoryStyle.py
 wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
 wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
 wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
 wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
 wwpdb/apps/ann_tasks_v2/site/Site.py
 wwpdb/apps/ann_tasks_v2/site/__init__.py
 wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
```

