# Comparing `tmp/wwpdb_apps_releasemodule-0.31.4.tar.gz` & `tmp/wwpdb_apps_releasemodule-0.31.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_apps_releasemodule-0.31.4.tar", last modified: Sun May  5 19:51:21 2024, max compression
+gzip compressed data, was "wwpdb_apps_releasemodule-0.31.5.tar", last modified: Fri May 31 22:45:09 2024, max compression
```

## Comparing `wwpdb_apps_releasemodule-0.31.4.tar` & `wwpdb_apps_releasemodule-0.31.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.580123 wwpdb_apps_releasemodule-0.31.4/
--rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-05-05 19:51:21.580123 wwpdb_apps_releasemodule-0.31.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       52 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-05 19:51:21.580123 wwpdb_apps_releasemodule-0.31.4/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2539 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.556123 wwpdb_apps_releasemodule-0.31.4/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.556123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.560123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.564123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/
--rw-r--r--   0 vsts      (1001) docker     (127)    10466 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/Analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/CheckResult.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15867 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/CitationFinder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5284 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchMP.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35275 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchResultParser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4490 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MatchMP.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2569 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MatchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8181 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14457 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6962 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/RisCitationParser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5050 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchMP.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchResultParser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3216 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/StringUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.568123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)     2904 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19491 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19597 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7582 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4158 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4437 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6443 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictRequest.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14638 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      894 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/test_DepictCitation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.572123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/
--rw-r--r--   0 vsts      (1001) docker     (127)    12660 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/AutoReRelease.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12851 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13786 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EmReleaseUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3069 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2611 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryPullProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25384 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryUpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25079 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3574 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/InputFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18623 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4828 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/NmrDataGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21730 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23671 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/ReleaseUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3479 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3773 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22156 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateFormParser.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13024 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.576123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)    24098 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/CombineDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22431 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/ContentDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7405 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/JournalAbbrev.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6429 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/MessageBaseClass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9550 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1574 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/MultiProcLimit.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6170 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3456 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12760 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/Utility.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.576123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    47983 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.580123 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 19:51:00.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      252 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.725173 wwpdb_apps_releasemodule-0.31.5/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-05-31 22:45:09.725173 wwpdb_apps_releasemodule-0.31.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       52 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-31 22:45:09.725173 wwpdb_apps_releasemodule-0.31.5/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2539 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.713173 wwpdb_apps_releasemodule-0.31.5/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.717173 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.717173 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.717173 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10466 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/Analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/CheckResult.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15867 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/CitationFinder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5284 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/FetchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35275 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/FetchResultParser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4490 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/FetchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/MatchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2569 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/MatchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8181 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14457 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6962 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/RisCitationParser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5050 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/SearchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/SearchResultParser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3216 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/SearchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/StringUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.721173 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2904 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19491 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19597 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7582 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4158 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4437 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6443 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14638 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      894 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/test_DepictCitation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.721173 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/
+-rw-r--r--   0 vsts      (1001) docker     (127)    12660 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/AutoReRelease.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12851 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13786 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EmReleaseUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3069 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2611 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EntryPullProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25384 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EntryUpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25079 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3574 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/InputFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18623 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4828 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/NmrDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21730 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23671 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/ReleaseUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3479 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3773 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/UpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22156 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/UpdateFormParser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13024 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.725173 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)    24098 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/CombineDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22431 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/ContentDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7405 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/JournalAbbrev.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6429 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/MessageBaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9550 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1574 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/MultiProcLimit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6170 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3456 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12760 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/Utility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.725173 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    47983 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 22:43:26.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:45:09.725173 wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-05-31 22:45:09.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-05-31 22:45:09.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-31 22:45:09.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-31 22:44:51.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      252 2024-05-31 22:45:09.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-31 22:45:09.000000 wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/top_level.txt
```

### Comparing `wwpdb_apps_releasemodule-0.31.4/PKG-INFO` & `wwpdb_apps_releasemodule-0.31.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.releasemodule
-Version: 0.31.4
+Version: 0.31.5
 Summary: wwPDB sequence module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_releasemodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: mmcif
 Requires-Dist: wwpdb.apps.msgmodule
 Requires-Dist: wwpdb.apps.wf_engine
 Requires-Dist: wwpdb.io
-Requires-Dist: wwpdb.utils.config~=0.24
+Requires-Dist: wwpdb.utils.config>=0.24
 Requires-Dist: wwpdb.utils.dp~=0.48
 Requires-Dist: wwpdb.utils.emdb~=1.0
 Requires-Dist: wwpdb.utils.session
 Requires-Dist: wwpdb.utils.wf
 Requires-Dist: mmcif.utils
 Requires-Dist: wwpdb.utils.db>=0.8
 Requires-Dist: rcsb.utils.multiproc
```

### Comparing `wwpdb_apps_releasemodule-0.31.4/setup.cfg` & `wwpdb_apps_releasemodule-0.31.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/setup.py` & `wwpdb_apps_releasemodule-0.31.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     #
     install_requires=['mmcif', 'wwpdb.apps.msgmodule', 'wwpdb.apps.wf_engine',
-                      'wwpdb.io', 'wwpdb.utils.config ~= 0.24',
+                      'wwpdb.io', 'wwpdb.utils.config >= 0.24',
                       'wwpdb.utils.dp ~= 0.48',
                       'wwpdb.utils.emdb ~= 1.0', 'wwpdb.utils.session',
                       'wwpdb.utils.wf', 'mmcif.utils', 'wwpdb.utils.db >= 0.8',
                       'rcsb.utils.multiproc'],
     packages=find_packages(exclude=['wwpdb.apps.tests-releasemodule',
                                     'mock-data']),
     # Enables Manifest to be used
```

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/Analysis.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/Analysis.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/CheckResult.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/CheckResult.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/CitationFinder.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/CitationFinder.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchMP.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/FetchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchResultParser.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/FetchResultParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/FetchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MatchMP.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/MatchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MatchUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/MatchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/RisCitationParser.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/RisCitationParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchMP.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/SearchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchResultParser.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/SearchResultParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/SearchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/StringUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/citation/StringUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictBase.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictRequest.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/DepictRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/test_DepictCitation.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/depict/test_DepictCitation.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/AutoReRelease.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/AutoReRelease.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EmReleaseUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EmReleaseUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryPullProcess.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EntryPullProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryUpdateBase.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EntryUpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/InputFormParser_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/InputFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/NmrDataGenerator.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/NmrDataGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/ReleaseUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/ReleaseUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateBase.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/UpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateFormParser.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/UpdateFormParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/CombineDbApi.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/CombineDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/ContentDbApi.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/ContentDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/DbApiUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/JournalAbbrev.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/JournalAbbrev.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/MessageBaseClass.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/MessageBaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/MultiProcLimit.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/MultiProcLimit.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/TimeUtil.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/Utility.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/utils/Utility.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py` & `wwpdb_apps_releasemodule-0.31.5/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/PKG-INFO` & `wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.releasemodule
-Version: 0.31.4
+Version: 0.31.5
 Summary: wwPDB sequence module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_releasemodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: mmcif
 Requires-Dist: wwpdb.apps.msgmodule
 Requires-Dist: wwpdb.apps.wf_engine
 Requires-Dist: wwpdb.io
-Requires-Dist: wwpdb.utils.config~=0.24
+Requires-Dist: wwpdb.utils.config>=0.24
 Requires-Dist: wwpdb.utils.dp~=0.48
 Requires-Dist: wwpdb.utils.emdb~=1.0
 Requires-Dist: wwpdb.utils.session
 Requires-Dist: wwpdb.utils.wf
 Requires-Dist: mmcif.utils
 Requires-Dist: wwpdb.utils.db>=0.8
 Requires-Dist: rcsb.utils.multiproc
```

### Comparing `wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/SOURCES.txt` & `wwpdb_apps_releasemodule-0.31.5/wwpdb.apps.releasemodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

