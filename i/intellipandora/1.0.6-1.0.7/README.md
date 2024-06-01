# Comparing `tmp/intellipandora-1.0.6-py3-none-any.whl.zip` & `tmp/intellipandora-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,49 +1,76 @@
-Zip file size: 63738 bytes, number of entries: 92
--rwxr-xr-x  2.0 unx      173 b- defN 24-May-04 14:02 intellipandora-1.0.6.data/scripts/runner.py
--rw-r--r--  2.0 unx      652 b- defN 24-May-05 07:15 ipandora/CHANGELOG
+Zip file size: 97070 bytes, number of entries: 123
+-rwxr-xr-x  2.0 unx      173 b- defN 24-May-04 14:02 intellipandora-1.0.7.data/scripts/runner.py
+-rw-r--r--  2.0 unx      893 b- defN 24-Jun-01 13:36 ipandora/CHANGELOG
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 02:43 ipandora/__init__.py
 -rw-r--r--  2.0 unx      643 b- defN 24-Apr-20 11:39 ipandora/version.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 02:43 ipandora/common/__init__.py
--rw-r--r--  2.0 unx     1399 b- defN 24-May-04 14:02 ipandora/common/fileaction.py
--rw-r--r--  2.0 unx     4580 b- defN 24-May-04 14:03 ipandora/common/filewriter.py
--rw-r--r--  2.0 unx     2613 b- defN 24-May-02 13:17 ipandora/common/mysqlaction.py
--rw-r--r--  2.0 unx     3150 b- defN 24-May-04 14:04 ipandora/common/systeminfo.py
+-rw-r--r--  2.0 unx      826 b- defN 24-May-22 06:33 ipandora/common/dictutils.py
+-rw-r--r--  2.0 unx     3008 b- defN 24-Jun-01 13:16 ipandora/common/mysqlaction.py
+-rw-r--r--  2.0 unx     3605 b- defN 24-May-22 07:02 ipandora/common/stringaction.py
+-rw-r--r--  2.0 unx     3304 b- defN 24-Jun-01 13:16 ipandora/common/systeminfo.py
+-rw-r--r--  2.0 unx     4218 b- defN 24-May-21 01:15 ipandora/common/timeutils.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 02:43 ipandora/conf/__init__.py
--rw-r--r--  2.0 unx      465 b- defN 24-May-04 14:10 ipandora/core/__init__.py
--rw-r--r--  2.0 unx     2251 b- defN 24-Apr-29 02:43 ipandora/core/log.py
+-rw-r--r--  2.0 unx      396 b- defN 24-Jun-01 13:13 ipandora/core/__init__.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 10:33 ipandora/core/base/__init__.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 10:35 ipandora/core/base/classwrap/__init__.py
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-24 23:26 ipandora/core/base/classwrap/attrvaluesplit.py
 -rw-r--r--  2.0 unx     1487 b- defN 24-Apr-20 11:52 ipandora/core/base/classwrap/classproperty.py
 -rw-r--r--  2.0 unx     2787 b- defN 24-May-04 14:02 ipandora/core/base/classwrap/multihandle.py
 -rw-r--r--  2.0 unx      608 b- defN 24-Apr-20 11:49 ipandora/core/base/classwrap/singleton.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:52 ipandora/core/base/data/__init__.py
 -rw-r--r--  2.0 unx     1155 b- defN 24-Apr-19 04:30 ipandora/core/base/data/markdata.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 10:39 ipandora/core/base/loglib/__init__.py
 -rw-r--r--  2.0 unx      995 b- defN 24-May-05 01:23 ipandora/core/base/loglib/log.py
+-rw-r--r--  2.0 unx       95 b- defN 24-May-23 02:07 ipandora/core/base/repository/__init__.py
+-rw-r--r--  2.0 unx     4691 b- defN 24-Jun-01 13:46 ipandora/core/base/repository/baserepository.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:53 ipandora/core/engine/__init__.py
--rw-r--r--  2.0 unx      734 b- defN 24-May-03 14:22 ipandora/core/engine/generator/__init__.py
--rw-r--r--  2.0 unx      286 b- defN 24-Apr-29 08:26 ipandora/core/engine/generator/model/__init__.py
+-rw-r--r--  2.0 unx       95 b- defN 24-May-21 16:13 ipandora/core/engine/crypto/__init__.py
+-rw-r--r--  2.0 unx     3997 b- defN 24-Jun-01 13:19 ipandora/core/engine/crypto/aescryptographer.py
+-rw-r--r--  2.0 unx     2229 b- defN 24-Jun-01 13:19 ipandora/core/engine/crypto/crypto.py
+-rw-r--r--  2.0 unx      285 b- defN 24-May-22 07:18 ipandora/core/engine/crypto/cryptoabc.py
+-rw-r--r--  2.0 unx     2804 b- defN 24-Jun-01 13:19 ipandora/core/engine/crypto/fercryptographer.py
+-rw-r--r--  2.0 unx     3898 b- defN 24-Jun-01 13:19 ipandora/core/engine/crypto/rsacryptographer.py
+-rw-r--r--  2.0 unx      733 b- defN 24-Jun-01 13:16 ipandora/core/engine/generator/__init__.py
+-rw-r--r--  2.0 unx      497 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/model/__init__.py
 -rw-r--r--  2.0 unx       94 b- defN 24-Apr-29 08:25 ipandora/core/engine/generator/model/data/__init__.py
+-rw-r--r--  2.0 unx       94 b- defN 24-May-24 16:46 ipandora/core/engine/generator/model/data/moduledata.py
 -rw-r--r--  2.0 unx     1969 b- defN 24-May-03 01:38 ipandora/core/engine/generator/model/data/robotcase.py
--rw-r--r--  2.0 unx     8774 b- defN 24-May-03 01:53 ipandora/core/engine/generator/model/data/robotsuite.py
+-rw-r--r--  2.0 unx     3078 b- defN 24-May-24 00:47 ipandora/core/engine/generator/model/data/robotcaselegacy.py
+-rw-r--r--  2.0 unx      798 b- defN 24-May-25 05:33 ipandora/core/engine/generator/model/data/robotsuite.py
+-rw-r--r--  2.0 unx     8941 b- defN 24-Jun-01 13:20 ipandora/core/engine/generator/model/data/robotsuitelegacy.py
+-rw-r--r--  2.0 unx     4105 b- defN 24-Jun-01 01:07 ipandora/core/engine/generator/model/data/testcase.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-28 09:00 ipandora/core/engine/generator/model/handler/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-03 01:21 ipandora/core/engine/generator/model/handler/robotrenderer.py
+-rw-r--r--  2.0 unx     3412 b- defN 24-Jun-01 13:21 ipandora/core/engine/generator/model/handler/robotrenderer.py
+-rw-r--r--  2.0 unx     1932 b- defN 24-Jun-01 13:21 ipandora/core/engine/generator/model/handler/robotrendererlegacy.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-28 09:00 ipandora/core/engine/generator/provider/__init__.py
 -rw-r--r--  2.0 unx      825 b- defN 24-May-02 12:33 ipandora/core/engine/generator/provider/caseprovider.py
--rw-r--r--  2.0 unx     2315 b- defN 24-May-03 01:17 ipandora/core/engine/generator/provider/robotprovider.py
+-rw-r--r--  2.0 unx      838 b- defN 24-May-23 02:02 ipandora/core/engine/generator/provider/robotbaseprovider.py
+-rw-r--r--  2.0 unx     2854 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/provider/robotprovider.py
+-rw-r--r--  2.0 unx       95 b- defN 24-May-22 09:30 ipandora/core/engine/generator/repository/__init__.py
+-rw-r--r--  2.0 unx     1418 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/modulerepository.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/projectrepository.py
+-rw-r--r--  2.0 unx     1708 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/submodulerepository.py
+-rw-r--r--  2.0 unx     2450 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/tagcategoryrepository.py
+-rw-r--r--  2.0 unx     3131 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/tagrepository.py
+-rw-r--r--  2.0 unx    12370 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/testcaserepository.py
+-rw-r--r--  2.0 unx     2788 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/testcasetagsrepository.py
+-rw-r--r--  2.0 unx     2568 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/repository/teststeprepository.py
+-rw-r--r--  2.0 unx       95 b- defN 24-May-24 01:36 ipandora/core/engine/generator/service/__init__.py
+-rw-r--r--  2.0 unx     2813 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/service/robotcaseservice.py
+-rw-r--r--  2.0 unx     9692 b- defN 24-Jun-01 13:24 ipandora/core/engine/generator/service/testcaseserivce.py
 -rw-r--r--  2.0 unx      314 b- defN 24-May-04 14:02 ipandora/core/plugin/__init__.py
 -rw-r--r--  2.0 unx     1038 b- defN 24-May-04 14:26 ipandora/core/plugin/innerplugin.py
 -rw-r--r--  2.0 unx     1169 b- defN 24-May-04 14:02 ipandora/core/plugin/pluginmanager.py
 -rw-r--r--  2.0 unx     3045 b- defN 24-May-04 14:02 ipandora/core/plugin/specificationsbuilder.py
 -rw-r--r--  2.0 unx      411 b- defN 24-May-04 14:02 ipandora/core/plugin/interface/__init__.py
 -rw-r--r--  2.0 unx      231 b- defN 24-May-04 14:02 ipandora/core/plugin/interface/endpointsinterface.py
 -rw-r--r--  2.0 unx      235 b- defN 24-May-04 14:02 ipandora/core/plugin/interface/httpregisterinterface.py
 -rw-r--r--  2.0 unx      859 b- defN 24-May-05 01:36 ipandora/core/plugin/interface/plugininterface.py
--rw-r--r--  2.0 unx       95 b- defN 24-May-04 14:10 ipandora/core/protocol/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 24-Jun-01 13:14 ipandora/core/protocol/__init__.py
 -rw-r--r--  2.0 unx      585 b- defN 24-May-05 01:17 ipandora/core/protocol/http/__init__.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:53 ipandora/core/protocol/http/model/__init__.py
 -rw-r--r--  2.0 unx     2227 b- defN 24-May-04 14:23 ipandora/core/protocol/http/model/httpmodel.py
 -rw-r--r--  2.0 unx      374 b- defN 24-May-04 14:24 ipandora/core/protocol/http/model/sessionmodel.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:53 ipandora/core/protocol/http/model/data/__init__.py
 -rw-r--r--  2.0 unx     1226 b- defN 24-May-05 01:23 ipandora/core/protocol/http/model/data/baseobject.py
 -rw-r--r--  2.0 unx     4323 b- defN 24-May-04 14:23 ipandora/core/protocol/http/model/data/requestobject.py
@@ -58,37 +85,41 @@
 -rw-r--r--  2.0 unx     1009 b- defN 24-May-04 14:02 ipandora/core/protocol/http/model/option/apioption.py
 -rw-r--r--  2.0 unx      236 b- defN 24-May-04 14:10 ipandora/core/protocol/http/model/option/httpontion.py
 -rw-r--r--  2.0 unx      256 b- defN 24-May-04 14:23 ipandora/core/protocol/http/provider/__init__.py
 -rw-r--r--  2.0 unx     2835 b- defN 24-May-04 14:02 ipandora/core/protocol/http/provider/baseprovider.py
 -rw-r--r--  2.0 unx      914 b- defN 24-May-04 14:18 ipandora/core/protocol/http/provider/httpprovider.py
 -rw-r--r--  2.0 unx     1637 b- defN 24-May-04 14:02 ipandora/core/protocol/http/provider/markprovider.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:54 ipandora/core/schedule/__init__.py
--rw-r--r--  2.0 unx     4649 b- defN 24-May-04 14:02 ipandora/core/schedule/runtime.py
--rw-r--r--  2.0 unx     2713 b- defN 24-Apr-20 11:54 ipandora/core/schedule/session.py
+-rw-r--r--  2.0 unx     8448 b- defN 24-Jun-01 13:46 ipandora/core/schedule/runtime.py
+-rw-r--r--  2.0 unx     2712 b- defN 24-Jun-01 13:14 ipandora/core/schedule/session.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:54 ipandora/core/wrapper/__init__.py
 -rw-r--r--  2.0 unx     2103 b- defN 24-May-04 14:02 ipandora/core/wrapper/basewrapper.py
 -rw-r--r--  2.0 unx     2793 b- defN 24-May-04 14:24 ipandora/core/wrapper/requestwrapper.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-20 11:54 ipandora/core/wrapper/interface/__init__.py
 -rw-r--r--  2.0 unx      535 b- defN 24-Apr-20 11:54 ipandora/core/wrapper/interface/requestinterface.py
 -rw-r--r--  2.0 unx      196 b- defN 24-May-04 14:02 ipandora/run/__init__.py
 -rw-r--r--  2.0 unx     1106 b- defN 24-May-04 14:02 ipandora/run/cmd.py
 -rw-r--r--  2.0 unx     1393 b- defN 24-Apr-20 11:49 ipandora/run/commandbase.py
 -rw-r--r--  2.0 unx     2115 b- defN 24-May-04 14:02 ipandora/run/commandmanager.py
 -rw-r--r--  2.0 unx     6447 b- defN 24-May-04 14:02 ipandora/run/ipandoracommand.py
 -rw-r--r--  2.0 unx      173 b- defN 24-May-04 14:02 ipandora/run/runner.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-20 12:10 ipandora/run/commands/__init__.py
 -rw-r--r--  2.0 unx     1867 b- defN 24-May-04 14:02 ipandora/run/commands/project.py
 -rw-r--r--  2.0 unx       93 b- defN 24-Apr-17 03:12 ipandora/utils/__init__.py
--rw-r--r--  2.0 unx     1386 b- defN 24-Apr-30 00:37 ipandora/utils/error.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-Jun-01 13:17 ipandora/utils/error.py
+-rw-r--r--  2.0 unx     1413 b- defN 24-Jun-01 13:16 ipandora/utils/fileload.py
+-rw-r--r--  2.0 unx     5133 b- defN 24-Jun-01 13:16 ipandora/utils/filewriter.py
 -rw-r--r--  2.0 unx     1805 b- defN 24-May-04 14:02 ipandora/utils/importpath.py
--rw-r--r--  2.0 unx     1080 b- defN 24-May-04 14:02 ipandora/utils/log.py
+-rw-r--r--  2.0 unx     3269 b- defN 24-Jun-01 13:12 ipandora/utils/log.py
 -rw-r--r--  2.0 unx     2408 b- defN 24-Apr-17 03:25 ipandora/utils/match.py
 -rw-r--r--  2.0 unx      521 b- defN 24-Apr-17 05:38 ipandora/utils/niceline.py
+-rw-r--r--  2.0 unx     3650 b- defN 24-Jun-01 13:16 ipandora/utils/pathutils.py
+-rw-r--r--  2.0 unx     4769 b- defN 24-Jun-01 13:16 ipandora/utils/robotlogparser.py
 -rw-r--r--  2.0 unx     2183 b- defN 24-Apr-19 14:34 ipandora/utils/variable.py
--rw-r--r--  2.0 unx      479 b- defN 24-May-05 07:15 intellipandora-1.0.6.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx    11342 b- defN 24-May-05 07:15 intellipandora-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2572 b- defN 24-May-05 07:15 intellipandora-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-05 07:15 intellipandora-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 24-May-05 07:15 intellipandora-1.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-05 07:15 intellipandora-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8801 b- defN 24-May-05 07:15 intellipandora-1.0.6.dist-info/RECORD
-92 files, 141435 bytes uncompressed, 49356 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx      479 b- defN 24-Jun-01 13:47 intellipandora-1.0.7.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx    11342 b- defN 24-Jun-01 13:47 intellipandora-1.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3471 b- defN 24-Jun-01 13:47 intellipandora-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 13:47 intellipandora-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-Jun-01 13:47 intellipandora-1.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Jun-01 13:47 intellipandora-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    12147 b- defN 24-Jun-01 13:47 intellipandora-1.0.7.dist-info/RECORD
+123 files, 241686 bytes uncompressed, 77150 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,49 +1,52 @@
-Filename: intellipandora-1.0.6.data/scripts/runner.py
+Filename: intellipandora-1.0.7.data/scripts/runner.py
 Comment: 
 
 Filename: ipandora/CHANGELOG
 Comment: 
 
 Filename: ipandora/__init__.py
 Comment: 
 
 Filename: ipandora/version.py
 Comment: 
 
 Filename: ipandora/common/__init__.py
 Comment: 
 
-Filename: ipandora/common/fileaction.py
+Filename: ipandora/common/dictutils.py
 Comment: 
 
-Filename: ipandora/common/filewriter.py
+Filename: ipandora/common/mysqlaction.py
 Comment: 
 
-Filename: ipandora/common/mysqlaction.py
+Filename: ipandora/common/stringaction.py
 Comment: 
 
 Filename: ipandora/common/systeminfo.py
 Comment: 
 
-Filename: ipandora/conf/__init__.py
+Filename: ipandora/common/timeutils.py
 Comment: 
 
-Filename: ipandora/core/__init__.py
+Filename: ipandora/conf/__init__.py
 Comment: 
 
-Filename: ipandora/core/log.py
+Filename: ipandora/core/__init__.py
 Comment: 
 
 Filename: ipandora/core/base/__init__.py
 Comment: 
 
 Filename: ipandora/core/base/classwrap/__init__.py
 Comment: 
 
+Filename: ipandora/core/base/classwrap/attrvaluesplit.py
+Comment: 
+
 Filename: ipandora/core/base/classwrap/classproperty.py
 Comment: 
 
 Filename: ipandora/core/base/classwrap/multihandle.py
 Comment: 
 
 Filename: ipandora/core/base/classwrap/singleton.py
@@ -57,47 +60,125 @@
 
 Filename: ipandora/core/base/loglib/__init__.py
 Comment: 
 
 Filename: ipandora/core/base/loglib/log.py
 Comment: 
 
+Filename: ipandora/core/base/repository/__init__.py
+Comment: 
+
+Filename: ipandora/core/base/repository/baserepository.py
+Comment: 
+
 Filename: ipandora/core/engine/__init__.py
 Comment: 
 
+Filename: ipandora/core/engine/crypto/__init__.py
+Comment: 
+
+Filename: ipandora/core/engine/crypto/aescryptographer.py
+Comment: 
+
+Filename: ipandora/core/engine/crypto/crypto.py
+Comment: 
+
+Filename: ipandora/core/engine/crypto/cryptoabc.py
+Comment: 
+
+Filename: ipandora/core/engine/crypto/fercryptographer.py
+Comment: 
+
+Filename: ipandora/core/engine/crypto/rsacryptographer.py
+Comment: 
+
 Filename: ipandora/core/engine/generator/__init__.py
 Comment: 
 
 Filename: ipandora/core/engine/generator/model/__init__.py
 Comment: 
 
 Filename: ipandora/core/engine/generator/model/data/__init__.py
 Comment: 
 
+Filename: ipandora/core/engine/generator/model/data/moduledata.py
+Comment: 
+
 Filename: ipandora/core/engine/generator/model/data/robotcase.py
 Comment: 
 
+Filename: ipandora/core/engine/generator/model/data/robotcaselegacy.py
+Comment: 
+
 Filename: ipandora/core/engine/generator/model/data/robotsuite.py
 Comment: 
 
+Filename: ipandora/core/engine/generator/model/data/robotsuitelegacy.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/model/data/testcase.py
+Comment: 
+
 Filename: ipandora/core/engine/generator/model/handler/__init__.py
 Comment: 
 
 Filename: ipandora/core/engine/generator/model/handler/robotrenderer.py
 Comment: 
 
+Filename: ipandora/core/engine/generator/model/handler/robotrendererlegacy.py
+Comment: 
+
 Filename: ipandora/core/engine/generator/provider/__init__.py
 Comment: 
 
 Filename: ipandora/core/engine/generator/provider/caseprovider.py
 Comment: 
 
+Filename: ipandora/core/engine/generator/provider/robotbaseprovider.py
+Comment: 
+
 Filename: ipandora/core/engine/generator/provider/robotprovider.py
 Comment: 
 
+Filename: ipandora/core/engine/generator/repository/__init__.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/repository/modulerepository.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/repository/projectrepository.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/repository/submodulerepository.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/repository/tagcategoryrepository.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/repository/tagrepository.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/repository/testcaserepository.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/repository/testcasetagsrepository.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/repository/teststeprepository.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/service/__init__.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/service/robotcaseservice.py
+Comment: 
+
+Filename: ipandora/core/engine/generator/service/testcaseserivce.py
+Comment: 
+
 Filename: ipandora/core/plugin/__init__.py
 Comment: 
 
 Filename: ipandora/core/plugin/innerplugin.py
 Comment: 
 
 Filename: ipandora/core/plugin/pluginmanager.py
@@ -234,44 +315,56 @@
 
 Filename: ipandora/utils/__init__.py
 Comment: 
 
 Filename: ipandora/utils/error.py
 Comment: 
 
+Filename: ipandora/utils/fileload.py
+Comment: 
+
+Filename: ipandora/utils/filewriter.py
+Comment: 
+
 Filename: ipandora/utils/importpath.py
 Comment: 
 
 Filename: ipandora/utils/log.py
 Comment: 
 
 Filename: ipandora/utils/match.py
 Comment: 
 
 Filename: ipandora/utils/niceline.py
 Comment: 
 
+Filename: ipandora/utils/pathutils.py
+Comment: 
+
+Filename: ipandora/utils/robotlogparser.py
+Comment: 
+
 Filename: ipandora/utils/variable.py
 Comment: 
 
-Filename: intellipandora-1.0.6.dist-info/AUTHORS.rst
+Filename: intellipandora-1.0.7.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: intellipandora-1.0.6.dist-info/LICENSE
+Filename: intellipandora-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: intellipandora-1.0.6.dist-info/METADATA
+Filename: intellipandora-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: intellipandora-1.0.6.dist-info/WHEEL
+Filename: intellipandora-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: intellipandora-1.0.6.dist-info/entry_points.txt
+Filename: intellipandora-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: intellipandora-1.0.6.dist-info/top_level.txt
+Filename: intellipandora-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: intellipandora-1.0.6.dist-info/RECORD
+Filename: intellipandora-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipandora/CHANGELOG

```diff
@@ -1,7 +1,14 @@
+v1.0.7
+==============
+* add common libraries -- timeutils, fileutils, stringutils
+* add utils -- pathutils, robotlogparser, fileload, filewrite
+* add core.engine -- crypto
+* add core.engine -- generator, repository and service for testcase
+
 v1.0.6
 ==============
 * rename src/intellipandora to src/ipandora
 * add common libraries
 * split the core/engine into engine and protocol
 
 v1.0.4
```

## ipandora/common/mysqlaction.py

```diff
@@ -3,44 +3,54 @@
 @Author: Shao Feng
 @File  : mysqlaction.py
 @Time  : 2024-05-02
 """
 import pymysql
 import pymysql.cursors
 from pymysql.err import MySQLError
-from pandoragt.core import logger
+from ipandora.utils.log import logger
 
 
 class MysqlAction(object):
-    def __init__(self, host, user, password, database):
+    def __init__(self, host, username, password, database, port = 3306):
         self.connection = None
         self.host = host
-        self.user = user
+        self.user = username
         self.password = password
         self.database = database
+        self.port = port
+
+    def __enter__(self):
+        self.connect()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
 
     def connect(self):
         """
         Connect to MySQL database, only connect if there is no active connection.
         :return:
         """
         if self.connection is not None:
             logger.warn("Connection already established.")
             return self.connection
-        try:
-            self.connection = pymysql.connect(
-                host=self.host,
-                user=self.user,
-                password=self.password,
-                database=self.database,
-                cursorclass=pymysql.cursors.DictCursor
-            )
-            logger.info("Database connection established.")
-        except MySQLError as e:
-            raise MySQLError(f"Error connecting to MySQL Platform: {e}")
+        else:
+            try:
+                self.connection = pymysql.connect(
+                    host=self.host,
+                    user=self.user,
+                    password=self.password,
+                    database=self.database,
+                    cursorclass=pymysql.cursors.DictCursor
+                )
+                logger.info("Database connection established.")
+                return self
+            except MySQLError as e:
+                raise MySQLError(f"Error connecting to MySQL Platform: {e}")
 
     def execute_query(self, query):
         """
         Execute SQL query and handle possible exceptions.
         :param query:
         :return:
         """
@@ -63,16 +73,18 @@
         """
         if self.connection is None:
             logger.warn("No connection to the database.")
             return
         try:
             with self.connection.cursor() as cursor:
                 cursor.execute(query)
+                affected_rows = cursor.rowcount
                 self.connection.commit()
-                logger.info("Transaction committed.")
+                logger.info(f"Transaction committed. {affected_rows} rows affected.")
+                return affected_rows
         except MySQLError as e:
             logger.warn(f"Error during transaction, rolling back: {e}")
             self.connection.rollback()
 
     def close(self):
         """
         close the database connection.
```

## ipandora/common/systeminfo.py

```diff
@@ -4,22 +4,27 @@
 @File  : systeminfo.py
 @Time  : 2024-04-24
 """
 import platform
 import socket
 import psutil
 import os
-from ipandora.core import logger
+import getpass
+from ipandora.utils.log import logger
 
 
 class SystemInfo(object):
     def __init__(self):
         pass
 
     @property
+    def user(self):
+        return getpass.getuser()
+
+    @property
     def host(self):
         return self.get_host()
 
     @property
     def host_name(self):
         return self.get_host_name()
 
@@ -52,15 +57,15 @@
         return self.get_parent_pid()
 
     @staticmethod
     def get_memory_info():
         return psutil.virtual_memory()
 
     @staticmethod
-    def get_host_name(self):
+    def get_host_name():
         return socket.gethostname()
 
     @staticmethod
     def get_host():
         interfaces = psutil.net_if_addrs()
         for interface_name, interface_addresses in interfaces.items():
             for address in interface_addresses:
@@ -108,11 +113,13 @@
         except psutil.AccessDenied:
             logger.warning(f"Permission denied to terminate process {pid}.")
         except Exception as e:
             logger.warning(f"Error terminating process {pid}: {e}")
 
 
 if __name__ == '__main__':
-    pids = (SystemInfo().get_pids_by_name('python', 'remote', 'stop'))
-    for p in pids:
-        SystemInfo().kill_process(p)
+    print(SystemInfo().get_host())
+    print(SystemInfo().user)
+    # pids = (SystemInfo().get_pids_by_name('python', 'remote', 'stop'))
+    # for p in pids:
+    #     SystemInfo().kill_process(p)
```

## ipandora/core/__init__.py

```diff
@@ -1,22 +1,18 @@
 # -*- coding: utf-8 -*-
 # @Author: Shao Feng
 # @File  : __init__.py.py
 # @Time  : 2024-04-17
-import logging
 import os
 import sys
 from ipandora.core.schedule.runtime import Runtime
-from ipandora.core.protocol.http import Api
-from ipandora.core.log import logger
-
-
+from ipandora.core.protocol import Api
 api = Api()
 
 
 def init(product=''):
     sys.path.append(
         os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir)))
     Runtime.product = product
 
 
-__all__ = ['api', 'init', 'logger']
+__all__ = ['api', 'init']
```

## ipandora/core/engine/generator/__init__.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : __init__.py.py
 @Time  : 2024-04-28
 """
-from pandoragt.core.engine.generator.provider.robotprovider import (RobotSuiteProvider,
+from ipandora.core.engine.generator.provider.robotprovider import (RobotSuiteProvider,
                                                                     RobotCaseProvider)
 __all__ = ['RobotSuiteProvider', 'RobotCaseProvider', 'GeneratorApi']
 
 
 class GeneratorApi(object):
     def __init__(self, config):
         self.config = config
```

## ipandora/core/engine/generator/model/__init__.py

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : __init__.py.py
 @Time  : 2024-04-28
 """
-from pandoragt.core.engine.generator.model.data.robotsuite import RobotSuite
-from pandoragt.core.engine.generator.model.data.robotcase import RobotCase
+from ipandora.core.engine.generator.model.data.robotsuite import RobotSuite
+from ipandora.core.engine.generator.model.data.robotcase import RobotCase
+from ipandora.core.engine.generator.model.data.robotsuitelegacy import RobotSuiteLegacy
+from ipandora.core.engine.generator.model.data.robotcaselegacy import RobotCaseLegacy
 
-__all__ = ["RobotSuite", "RobotCase"]
+__all__ = ["RobotSuiteLegacy", "RobotCaseLegacy", "RobotSuite", "RobotCase"]
```

## ipandora/core/engine/generator/model/data/robotsuite.py

```diff
@@ -1,276 +1,37 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : robotsuite.py
-@Time  : 2024-04-29
+@Time  : 2024-05-24
 """
-from pandoragt.core import logger
-from pandoragt.core.engine.generator.model.data.robotcase import RobotCase, TypeCheck
-from pandoragt.utils.error import VariableError
-from typing import Union, List
+from typing import List, Optional
+from dataclasses import dataclass
 
 
-class RobotSuite(object):
-    def __init__(self, name, setup=None, teardown=None):
-        self._name = name
-        self._setup = setup
-        self._teardown = teardown
-        self._cases = []
-        self._case_obj = None
-        self._setting = self.init_setting()
-
-    def init_setting(self):
-        _setting = {}
-        if self._setup:
-            _setting.update({"Suite Setup": self._setup})
-        if self._teardown:
-            _setting.update({"Suite Teardown": self._teardown})
-        return _setting
-
-    @property
-    def content(self):
-        return {
-            "name": self._name,
-            "setting": self._setting,
-            "cases": self._cases,
-        }
-
-    @property
-    def name(self):
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        self._name = name
-
-    @property
-    def setting(self):
-        return self._setting
-
-    @setting.setter
-    def setting(self, setting):
-        if not isinstance(setting, dict):
-            raise VariableError("Setting must be a dictionary.")
-        for k, v in setting.items():
-            if k.lower() in ["suite setup", "suite teardown", "test template",
-                             "library", "resource"]:
-                self._setting.update({k: v})
-            elif k.lower() == "setup":
-                self.setup = v
-            elif k.lower() == "teardown":
-                self.teardown = v
-            else:
-                continue
-
-    @property
-    def setup(self):
-        return self._setting.get("Suite Setup")
-
-    @setup.setter
-    def setup(self, setup: str):
-        if not isinstance(setup, str):
-            raise VariableError("Suite Setup must be a string.")
-        if setup:
-            self._setting.update({"Suite Setup": setup})
-        else:
-            logger.warn("Suite Setup is empty.")
-
-    @property
-    def teardown(self):
-        return self._setting.get("Suite Teardown")
-
-    @teardown.setter
-    def teardown(self, teardown: str):
-        if not isinstance(teardown, str):
-            raise VariableError("Suite Teardown must be a string.")
-        if teardown:
-            self._setting.update({"Suite Teardown": teardown})
-        else:
-            logger.warn("Suite Teardown is empty.")
-
-    @property
-    def test_setup(self):
-        return self._setting.get("Test Setup")
-
-    @test_setup.setter
-    def test_setup(self, testsetup: str):
-        if not isinstance(testsetup, str):
-            raise VariableError("Test Setup must be a string.")
-        if testsetup:
-            self._setting.update({"Test Setup": testsetup})
-        else:
-            logger.warn("Test Setup is empty.")
-
-    @property
-    def test_teardown(self):
-        return self._setting.get("Test Teardown")
-
-    @test_teardown.setter
-    def test_teardown(self, test_teardown: str):
-        if not isinstance(test_teardown, str):
-            raise VariableError("Test Teardown must be a string.")
-        if test_teardown:
-            self._setting.update({"Test Teardown": test_teardown})
-        else:
-            logger.warn("Test Teardown is empty.")
-
-    @property
-    def tags(self):
-        return self._setting.get("Test Tags") or []
-
-    @tags.setter
-    def tags(self, tags):
-        _tag_list = self.tags
-        if isinstance(tags, list):
-            _tag_list.extend(tags)
-        else:
-            _tag_list.append(tags)
-        self._setting.update({"Test Tags": _tag_list})
-
-    @property
-    def resource(self):
-        return self._setting.get("Resource") or []
-
-    @resource.setter
-    def resource(self, resource):
-        _resource_list = self.resource
-        if isinstance(resource, list):
-            _resource_list.extend(resource)
-        else:
-            _resource_list.append(resource)
-        self._setting.update({"Resource": _resource_list})
-
-    @property
-    def library(self):
-        return self.setting.get("Library") or []
-
-    @library.setter
-    def library(self, library):
-        _library_list = self.library
-        if isinstance(library, list):
-            _library_list.extend(library)
-        else:
-            _library_list.append(library)
-        self._setting.update({"Library": _library_list})
-
-    @property
-    def template(self):
-        return self._setting.get("Test Template")
-
-    @template.setter
-    def template(self, template):
-        self._setting.update({"Test Template": template})
-
-    @property
-    def cases(self):
-        return self._cases
-
-    @cases.setter
-    def cases(self, case_objects: Union[RobotCase, List[RobotCase]]):
-        if isinstance(case_objects, list):
-            self._cases.extend(case_objects)
-        else:
-            self._cases.append(case_objects)
-
-    @property
-    def case_name(self):
-        return self._case_obj.name
-
-    @case_name.setter
-    def case_name(self, case_name):
-        # create new case object and attached to the suite
-        self._case_obj = RobotCase(case_name)
-        self._cases.append(self._case_obj)
-
-    @property
-    def case_setup(self):
-        return self._case_obj.setup
-
-    @case_setup.setter
-    def case_setup(self, case_setup: str):
-        if not self._case_obj and isinstance(self._case_obj, RobotCase):
-            raise VariableError("Case object not found. Please add a case first.")
-        if not isinstance(case_setup, str):
-            raise VariableError("Case Setup must be a string.")
-        self._case_obj.setup = case_setup
-
-    @property
-    def case_teardown(self):
-        return self._case_obj.teardown
-
-    @case_teardown.setter
-    def case_teardown(self, case_teardown: str):
-        if not isinstance(case_teardown, str):
-            raise VariableError("Case Teardown must be a string.")
-        if not self._case_obj and isinstance(self._case_obj, RobotCase):
-            raise VariableError("Case object not found. Please add a case first.")
-        self._case_obj.teardown = case_teardown
-
-    @property
-    def steps(self):
-        return self._case_obj.steps
-
-    @steps.setter
-    def steps(self, step):
-        if not self._case_obj:
-            raise VariableError("Case object not found. Please add a case first.")
-        self._case_obj.steps = step
-
-    def add_case(self, case_name, case_steps, case_setup=None, case_teardown=None):
-        self._case_obj = RobotCase(case_name, case_setup, case_teardown)
-        if isinstance(case_steps, list):
-            for step in case_steps:
-                self._case_obj.steps = step
-        else:
-            self._case_obj.steps = case_steps
-        self._cases.append(self._case_obj)
-
-    def add_config(self, resource=None, library=None, template=None):
-        self.resource = resource
-        self.library = library
-        self._setting.update({
-            "Resource": self.resource,
-            "Library": self.library,
-            "Test Template": template
-        })
-
-    def __str__(self):
-        return f"RobotSuite(name={self.name}, cases={self.cases}, setting={self.setting})"
-
-    def __repr__(self):
-        return f"RobotSuite({self.name!r}, {self.cases!r}, setting={self.setting!r})"
-
-
-if __name__ == '__main__':
-    _suite_obj = RobotSuite('test_suite_demo', 'Suite Setup', 'Suite Teardown')
-    _suite_obj.setup = "Suite Setup update"
-    _suite_obj.library = "SSHLibrary"
-    _suite_obj.resource = "resource.robot"
-    _suite_obj.add_config('resource_of_template.robot', 'Collections', 'Keyword As Template New')
-
-    # set cases and steps
-    _suite_obj.case_name = "Test Case 1"
-    _suite_obj.case_setup = "Case Setup"
-    _suite_obj.case_teardown = "Case Teardown"
-    _suite_obj.steps = "Step 1 for Case 1"
-    _suite_obj.steps = "Step 2 for Case 1"
-
-    _suite_obj.case_name = "Test Case 2"
-    _suite_obj.steps = "Step 1 for Case 2"
-    _suite_obj.steps = "Step 2 for Case 2"
-
-    _case_obj_3 = RobotCase("Test Case 3333", 'Case Setup 3333',
-                            'Case Teardown 3333')
-    _case_obj_3.steps = ["Step 300 for Case 3333", "Step 301 for Case 3333",
-                         "Step 302 for Case 3333", "Step 303 for Case 3333"]
-    _case_obj_4 = RobotCase("Test Case 444", 'Case Setup 444',
-                            'Case Teardown 444')
-    _suite_obj.cases = [_case_obj_4, _case_obj_3]
-
-    print(_suite_obj)
-
-    from pandoragt.core.engine.generator.model.handler.robotrenderer import RobotRenderer
-    _content = RobotRenderer(_suite_obj).content()
-    print(_content)
-    # from pandoragt.common.filewriter import RobotFileWriter
-    # RobotFileWriter("test.robot", _content)
+@dataclass
+class RobotSettings:
+    suite_setup: Optional[str] = None
+    suite_teardown: Optional[str] = None
+    test_setup: Optional[str] = None
+    test_teardown: Optional[str] = None
+    test_template: Optional[str] = None
+    resource: List[str] = None
+    library: List[str] = None
+    force_tag: List[str] = None
+
+
+@dataclass
+class RobotCase:
+    name: str
+    steps: List[str] = None
+    setup: Optional[str] = None
+    teardown: Optional[str] = None
+    documentation: Optional[str] = None
+    tags: List[str] = None
+
+
+@dataclass
+class RobotSuite:
+    name: str
+    settings: RobotSettings
+    cases: List[RobotCase] = None
```

## ipandora/core/engine/generator/model/handler/robotrenderer.py

```diff
@@ -1,51 +1,109 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : robotrenderer.py
-@Time  : 2024-04-28
+@Time  : 2024-05-25
 """
-from pandoragt.core.engine.generator.model import RobotSuite
+from ipandora.core.engine.generator.model.data.robotsuite import (RobotSuite, RobotSettings,
+                                                                  RobotCase)
 
 
-class RobotRenderer(object):
-    def __init__(self, suite: RobotSuite):
-        self.suite = suite
+class RobotRenderer:
+    def __init__(self, _robot_suite: RobotSuite):
+        self.robot_suite = _robot_suite
 
-    def content(self):
+    def content(self) -> str:
         content = ""
         content += self.render_setting()
         content += self.render_case()
         return content
 
-    def render_setting(self):
-        content = f"*** Settings ***\n"
-        max_key_length = max(len(key) for key in self.suite.setting) + 4
-        for _key, _value in self.suite.setting.items():
-            if isinstance(_value, list) and (_key == "Library" or _key == "Resource"):
-                for _v in _value:
-                    content += f"{_key:<{max_key_length}}{_v}\n"
-            elif isinstance(_value, list) and (_key == "Test Tags"):
-                _value = "    ".join(_value)
-                content += f"{_key:<{max_key_length}}{_value}\n"
-            else:
-                content += f"{_key:<{max_key_length}}{_value}\n"
+    def render_setting(self) -> str:
+        _settings = self.robot_suite.settings
+        content = "*** Settings ***\n"
+
+        setting_fields = {
+            "suite_setup": "Suite Setup",
+            "suite_teardown": "Suite Teardown",
+            "test_setup": "Test Setup",
+            "test_teardown": "Test Teardown",
+            "test_template": "Test Template",
+            "resource": "Resource",
+            "library": "Library",
+            "force_tag": "Force Tags"
+        }
+        for attr, keyword in setting_fields.items():
+            value = getattr(_settings, attr)
+            if isinstance(value, list):
+                for item in value:
+                    content += f"{keyword}    {item}\n"
+            elif value:
+                content += f"{keyword}    {value}\n"
         content += "\n"
         return content
 
-    def render_case(self):
-        content = f"*** Test Cases ***\n"
-        for _case_obj in self.suite.cases:
-            content += f"{_case_obj.name}\n"
-            if _case_obj.setup:
-                content += f"    [Setup]    {_case_obj.setup}\n"
-            for _step in _case_obj.steps:
-                content += f"    {_step}\n"
-            if _case_obj.teardown:
-                content += f"    [Teardown]    {_case_obj.teardown}\n"
+    def render_case(self) -> str:
+        content = "*** Test Cases ***\n"
+        case_fields = {
+            "documentation": "Documentation",
+            "setup": "Setup",
+            "teardown": "Teardown",
+            "tags": "Tags",
+            "steps": "Steps"
+        }
+
+        for case in self.robot_suite.cases:
+            content += f"{case.name}\n"
+            for attr, keyword in case_fields.items():
+                value = getattr(case, attr)
+                if isinstance(value, list) and keyword == "Steps":
+                    for step in value:
+                        content += f"    {step}\n"
+                elif isinstance(value, list):
+                    content += f"    [{keyword}]    {'    '.join(value)}\n"
+                elif value:
+                    content += f"    [{keyword}]    {value}\n"
             content += "\n"
         return content
 
 
 if __name__ == '__main__':
-    pass
-
+    # 示例用法
+    settings = RobotSettings(
+        suite_setup="Setup Suite 012",
+        suite_teardown="Teardown Suite 012",
+        test_setup="Setup Test 012",
+        test_teardown="Teardown Test 012",
+        test_template="Test Template 012",
+        resource=["Resource1", "Resource2"],
+        library=["Library1", "Library2"],
+        force_tag=["Tag1", "Tag2"]
+    )
+
+    cases = [
+        RobotCase(
+            name="Test Case 1",
+            steps=["Step 1", "Step 2"],
+            setup="Setup Case 1",
+            teardown="Teardown Case 1",
+            documentation="Documentation Case 1",
+            tags=["Tag1", "Tag2"]
+        ),
+        RobotCase(
+            name="Test Case 2",
+            steps=["Step 1", "Step 2", "Step 3"],
+            setup="Setup Case 2",
+            teardown="Teardown Case 2",
+            documentation="Documentation Case 2",
+            tags=["Tag3", "Tag4"]
+        )
+    ]
+
+    suite = RobotSuite(
+        name="Test Suite",
+        settings=settings,
+        cases=cases
+    )
+    print(suite)
+    renderer = RobotRenderer(suite)
+    print(renderer.content())
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## ipandora/core/engine/generator/provider/robotprovider.py

```diff
@@ -1,56 +1,68 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : robotprovider.py
 @Time  : 2024-04-29
 """
 from typing import List, Union
-from pandoragt.core.engine.generator.model.data.robotcase import RobotCase
-from pandoragt.core.engine.generator.model.data.robotsuite import RobotSuite
-from pandoragt.common.filewriter import RobotFileWriter
-from pandoragt.core.engine.generator.model.handler.robotrenderer import RobotRenderer
-from pandoragt.core.engine.generator.provider.caseprovider import ICaseProvider, ISuiteProvider
+from ipandora.core.engine.generator.model.data.robotcaselegacy import RobotCaseLegacy
+from ipandora.core.engine.generator.model.data.robotsuitelegacy import RobotSuiteLegacy
+from ipandora.utils.filewriter import RobotFileWriter
+from ipandora.core.engine.generator.model.handler.robotrendererlegacy import RobotRendererLegacy
+from ipandora.core.engine.generator.provider.robotbaseprovider import ICaseProvider, ISuiteProvider
 
 
 class RobotCaseProvider(ICaseProvider):
-    def create_case(self, steps: List[str]) -> RobotCase:
-        _case_object = RobotCase(self.name, self.setup, self.teardown)
-        for step in steps:
-            _case_object.steps = step
+    def create_case(self, steps: Union[str, List[str]]) -> RobotCaseLegacy:
+        _case_object = RobotCaseLegacy(self.name, self.setup, self.teardown)
+        _case_object.steps = steps
         return _case_object
 
 
 class RobotSuiteProvider(ISuiteProvider):
-    def create_suite(self, case_objects: Union[RobotCase, List[RobotCase]]) -> RobotSuite:
-        self.suite_object = RobotSuite(self.name, self.setup, self.teardown)
-        self.suite_object.cases = case_objects
+    def create_suite(self, case_objects: Union[RobotCaseLegacy, List[RobotCaseLegacy], None] = None):
+        self.suite_object = RobotSuiteLegacy(self.name, self.setup, self.teardown)
+        if case_objects:
+            self.suite_object.cases = case_objects
         return self.suite_object
 
-    def add_case_to_suite(self, suite:RobotSuite, case):
-        suite.cases = case
+    def add_case_to_suite(self, case):
+        if not self.suite_object:
+            self.create_suite()
+        self.suite_object.cases = case
+
+    def add_setting_to_suite(self, setting: dict):
+        if not self.suite_object:
+            self.create_suite()
+        self.suite_object.setting = setting
 
     def generate(self, directory: str = ''):
-        RobotFileWriter(self.suite_object.name, RobotRenderer(self.suite_object).content(),
+        RobotFileWriter(self.suite_object.name, RobotRendererLegacy(self.suite_object).content(),
                         directory)
 
 
 if __name__ == '__main__':
     # generate a robot file, suite and cases
     # create case object
     _c1 = RobotCaseProvider('testcase_001').create_case(['step 01 of case 001', 'step 02 of case 001'])
     _c1.steps = 'step extra of case 001'
+    _c1.documentation = 'this is a test case 001 documentation'
+    _c1.tags = ['tag1111', 'tag22222']
+    _c1.setup = 'setup of case 001'
+    _c1.teardown = 'teardown of case 001'
     _c2 = RobotCaseProvider('testcase_002', 'setup_case2', 'teardown_case2').create_case(
         ['step 01 of case 002', 'step 02 of case 002', 'step 03 of case 002'])
     # create suite object and attach case to suite.
     _sp = RobotSuiteProvider('testsuite_001', 'setup of suite 001', 'teardown of suite 001')
     _suite_obj = _sp.create_suite([_c1, _c2])
     _suite_obj.test_setup = 'test setup of suite 001'
     _suite_obj.test_teardown = 'test teardown of suite 001'
     _suite_obj.tags = ['tag1', 'tag2']
     _suite_obj.tags = 'smoke'
     _suite_obj.library = ['SSHLibrary', 'Collections']
     _suite_obj.resource = ['GT_resource.robot']
     print(_suite_obj)
+    print(RobotRendererLegacy(_suite_obj).content())
 
     # generate file
-    _sp.generate('/Users/shaofeng/Repos/logtemp')
+    # _sp.generate('/Users/shaofeng/Repos/logtemp')
```

## ipandora/core/protocol/__init__.py

```diff
@@ -1,6 +1,24 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : __init__.py.py
 @Time  : 2024-05-04
 """
+from ipandora.core.protocol.http.provider import Http, Mark
+from ipandora.core.plugin import PluginManager
+from ipandora.core.base.classwrap.multihandle import init as exit_init
+from ipandora.core.protocol.http.model.interface.responseinterface import HttpResponseInterface
+
+# init plugin manager
+PluginManager.init()
+
+# init exit
+exit_init()
+
+
+class Api(object):
+    http = Http()
+    mark = Mark
+    # socket = Socket()
+    # data object
+    response = None  # type:HttpResponseInterface
```

## ipandora/core/schedule/runtime.py

```diff
@@ -1,22 +1,176 @@
 # -*- coding: utf-8 -*-
 """
 @Author: Shao Feng
 @File  : runtime.py
 @Time  : 2024-04-19
 """
+import os
 import socket
 from typing import Union
+
+from ipandora.common.dictutils import DictUtils
+from ipandora.common.stringaction import StringAction
+from ipandora.common.systeminfo import SystemInfo
 from ipandora.core.base.classwrap.classproperty import classproperty, ClassPropertyMeta
+from ipandora.core.engine.crypto.crypto import CryptoFactory
+from ipandora.utils.fileload import FileLoad
+from ipandora.utils.pathutils import PathUtils
 
 
 class Runtime(object):
 	exc_info = ''
 	product = ''
-	settings = {}  # type:dict
+	settings = FileLoad(
+		os.path.join(PathUtils().pandora_path, 'conf/config.yaml')).load_yaml()  # type:dict
+
+	class User(metaclass=ClassPropertyMeta):
+		_user = ''
+
+		@classproperty
+		def user(self):
+			if not self._user:
+				self._user = SystemInfo().user
+			return self._user
+
+		@user.set
+		def user(self, value):
+			self._user = value
+
+	class Mysql(metaclass=ClassPropertyMeta):
+		_host = ''
+		_username = ''
+		_password = ''
+		_port = 3306
+		_database = ''
+
+		@classproperty
+		def host(self):
+			if not self._host:
+				self._host = DictUtils.safe_get(Runtime.settings, 'mysql', 'host')
+			return self._host
+
+		@host.set
+		def host(self, value):
+			self._host = value
+
+		@classproperty
+		def username(self):
+			if not self._username:
+				self._username = DictUtils.safe_get(Runtime.settings, 'mysql', 'username')
+			return self._username
+
+		@username.set
+		def username(self, value):
+			self._username = value
+
+		@classproperty
+		def password(self):
+			if not self._password:
+				self._password = DictUtils.safe_get(Runtime.settings, 'mysql', 'password')
+				if self._password and StringAction.is_base64_encoded(self._password):
+					self._password = CryptoFactory().aes.decrypt(self._password)
+			return self._password
+
+		@password.set
+		def password(self, value):
+			self._password = value
+
+		@classproperty
+		def port(self):
+			if not self._port:
+				self._port = DictUtils.safe_get(Runtime.settings, 'mysql', 'port')
+			return self._port
+
+		@port.set
+		def port(self, value):
+			self._port = value
+
+		@classproperty
+		def database(self):
+			if not self._database:
+				self._database = DictUtils.safe_get(Runtime.settings, 'mysql', 'database')
+			return self._database
+
+		@database.set
+		def database(self, value):
+			self._database = value
+
+	class Email(metaclass=ClassPropertyMeta):
+		_host = ''
+		_username = ''
+		_password = ''
+		_port = 465
+		_recipients = []
+
+		@classproperty
+		def host(self):
+			if not self._host:
+				self._host = DictUtils.safe_get(Runtime.settings, 'email', 'host')
+			return self._host
+
+		@host.set
+		def host(self, value):
+			self._host = value
+
+		@classproperty
+		def username(self):
+			if not self._username:
+				self._username = DictUtils.safe_get(Runtime.settings, 'email', 'username')
+			return self._username
+
+		@username.set
+		def username(self, value):
+			self._username = value
+
+		@classproperty
+		def password(self):
+			if not self._password:
+				self._password = DictUtils.safe_get(Runtime.settings, 'email', 'password')
+			if self._password and StringAction.is_base64_encoded(self._password):
+				self._password = CryptoFactory().aes.decrypt(self._password)
+			return self._password
+
+		@password.set
+		def password(self, value):
+			self._password = value
+
+		@classproperty
+		def port(self):
+			if not self._port:
+				self._port = DictUtils.safe_get(Runtime.settings, 'email', 'port')
+			return self._port
+
+		@port.set
+		def port(self, value):
+			self._port = value
+
+		@classproperty
+		def recipients(self):
+			if not self._recipients:
+				_tmp = DictUtils.safe_get(Runtime.settings, 'addressesTo', 'recipients')
+				self._recipients = _tmp if _tmp else []
+			return self._recipients
+
+		@recipients.set
+		def recipients(self, value):
+			self._recipients = value
+
+	class Path(metaclass=ClassPropertyMeta):
+		_pandora_path = ''
+
+		@classproperty
+		def pandora_path(self):
+			if not self._pandora_path:
+				self._pandora_path = PathUtils().pandora_path
+			return self._pandora_path
+
+		@pandora_path.set
+		def pandora_path(self, value):
+			self._pandora_path = value
 
 	class Device(metaclass=ClassPropertyMeta):
 
 		ip = socket.gethostbyname(socket.gethostname())
 
 	class Host(metaclass=ClassPropertyMeta):
```

## ipandora/core/schedule/session.py

```diff
@@ -3,15 +3,14 @@
 @Author: Shao Feng
 @File  : session.py
 @Time  : 2024-04-19
 """
 import logging
 from threading import current_thread, RLock
 from typing import Dict
-
 import requests
 from requests.structures import CaseInsensitiveDict
 from requests.utils import default_headers
 
 logger = logging.getLogger(__name__)
```

## ipandora/utils/error.py

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 # @Author: Shao Feng
 # @File  : error.py
 # @Time  : 2024-04-17
-class PandoraGTError(Exception):
+class PandoraError(Exception):
     """Base class for FusionPandora Framework errors.
 
     Do not raise this method but use more specific errors instead.
     """
 
     def __init__(self, message='', details=''):
         super().__init__(message)
         self.details = details
 
     @property
     def message(self):
         return str(self)
 
 
-class FrameworkError(PandoraGTError):
+class FrameworkError(PandoraError):
     """Can be used when the core framework goes to unexpected state.
 
     It is good to explicitly raise a FrameworkError if some framework
     component is used incorrectly. This is pretty much same as
     'Internal Error' and should of course never happen.
     """
 
 
-class DataError(PandoraGTError):
+class DataError(PandoraError):
     """Used when the provided test data is invalid.
 
     DataErrors are not caught by keywords that run other keywords
     (e.g. `Run Keyword And Expect Error`).
     """
 
 
@@ -48,7 +48,13 @@
     VariableErrors are caught by keywords that run other keywords
     (e.g. `Run Keyword And Expect Error`).
     """
 
 
 class CommandError(Exception):
     pass
+
+
+class CryptoError(PandoraError):
+    """
+    Used when exception occurred while Encryption and decryption.
+    """
```

## ipandora/utils/log.py

```diff
@@ -1,14 +1,79 @@
 # -*- coding: utf-8 -*-
 # @Author: Shao Feng
 # @File  : log.py
 # @Time  : 2024-04-17
+import sys
 import logging
+import json
+from robot.api import logger as rf_logger
 
-logger = logging.getLogger("ipandora.log")
+
+class RobotFrameworkLoggingHandler(logging.Handler):
+    def emit(self, record):
+        try:
+            msg = self.format(record)
+            level = record.levelno
+            if level >= logging.CRITICAL:
+                rf_logger.error(msg)
+            elif level >= logging.ERROR:
+                rf_logger.error(msg)
+            elif level >= logging.WARNING:
+                rf_logger.warn(msg)
+            elif level >= logging.INFO:
+                rf_logger.info(msg)
+            else:
+                rf_logger.debug(msg)
+        except Exception:
+            self.handleError(record)
+
+
+class SmartJsonFormatter(logging.Formatter):
+    def format(self, record):
+        self.formatTime(record, self.datefmt)
+        message = record.getMessage()
+        try:
+            json_object = json.loads(message)
+            return json.dumps(json_object, indent=4)
+        except json.JSONDecodeError as e:
+            if "Expecting property name enclosed in double quotes" in str(e):
+                message = message.replace("'", '"')
+                try:
+                    json_object = json.loads(message)
+                    return json.dumps(json_object, indent=4)
+                except json.JSONDecodeError as e:
+                    pass
+            else:
+                pass
+        return super().format(record)
+
+
+def setup_logger():
+    # set logger level
+    _logger = logging.getLogger(__name__)
+    _logger.setLevel(logging.DEBUG)
+
+    # Robot Framework handler
+    rf_handler = RobotFrameworkLoggingHandler()
+    rf_handler.setLevel(logging.DEBUG)
+    rf_formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+    rf_handler.setFormatter(rf_formatter)
+    _logger.addHandler(rf_handler)
+
+    # Console handler
+    # formatter = logging.Formatter('[%(asctime)s](%(levelname)s)(%(name)s): %(message)s')
+    formatter = SmartJsonFormatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+    console_handler = logging.StreamHandler(sys.stdout)
+    console_handler.setLevel(logging.INFO)
+    console_handler.setFormatter(formatter)
+    _logger.addHandler(console_handler)
+    return _logger
+
+
+logger = setup_logger()
 
 
 class Log(object):
     name = 'default'
     END = '\033[0m'
 
     # color sequences
@@ -37,14 +102,15 @@
         cls.format(msg=msg)
 
     @classmethod
     def red(cls, msg=None):
         cls.format(color=cls.RED, msg=msg)
 
     @classmethod
-    def redInfo(cls, msg=None):
+    def red_info(cls, msg=None):
         return cls.RED + msg + cls.END
 
     @classmethod
     def format(cls, color=None, msg=None):
         _msg = color + msg + cls.END if color is not None else msg
-        logger.info(_msg)
+        logger.info(_msg)
+
```

## Comparing `ipandora/common/filewriter.py` & `ipandora/utils/filewriter.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @File  : filewriter.py
 @Time  : 2024-04-28
 """
 import csv
 import json
 import yaml
 import os
-from ipandora.core import logger
+from ipandora.utils.log import logger
 from ipandora.utils.error import FileError, DataError
 
 
 class FileWriter(object):
     def __init__(self, filename, content, directory=''):
         self.filename = filename
         self.content = content
@@ -36,14 +36,15 @@
         self._handle_write()
 
     def _handle_base_path(self):
         if not os.path.isabs(self.filename):
             if os.path.isabs(self.directory):
                 self.filename = os.path.join(self.directory, self.filename)
             else:
+                logger.warning(f"The <{self.directory}> is not exist. files will be stored <home>")
                 self.filename = os.path.join(os.path.expanduser('~'), self.filename)
         _dir_name = os.path.dirname(self.filename)
         # check directory exists and create if not
         if not os.path.exists(_dir_name):
             os.makedirs(_dir_name)
 
     def _handle_write(self):
@@ -130,22 +131,37 @@
     def extension(self):
         return '.yaml'
 
 
 class RobotFileWriter(FileWriter):
     """
     RobotFileWriter is a class that writes.
-    Content should be a string. which has be rendered by RobotRenderer.
+    Content should be a string. which has be rendered by RobotRendererLegacy.
     The file will be created in the home directory if filename is not the absolute path.
     """
     def _write(self):
         with open(self.filename, 'w', encoding='utf-8') as file:
             file.write(self.content)
 
     @property
     def extension(self):
         return '.robot'
 
 
+class HtmlFileWriter(FileWriter):
+    """
+    HtmlFileWriter is a class that writes.
+    Content should be a string. which has be rendered by HtmlRenderer.
+    The file will be created in the home directory if filename is not the absolute path.
+    """
+    def _write(self):
+        with open(self.filename, 'w', encoding='utf-8') as file:
+            file.write(self.content)
+
+    @property
+    def extension(self):
+        return '.html'
+
+
 if __name__ == '__main__':
     resp = YAMLFileWriter("test", {"name": "test"}, directory='/Users/shaofeng/temp_file/')
     print(resp)
```

## Comparing `intellipandora-1.0.6.dist-info/LICENSE` & `intellipandora-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intellipandora-1.0.6.dist-info/METADATA` & `intellipandora-1.0.7.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: intellipandora
-Version: 1.0.6
+Version: 1.0.7
 Summary: Generic automation framework for system testing and model evaluation
-Home-page: https://www.python.org/doc/
+Home-page: https://github.com/Conan-Shao/IntelliPandora
 Author: Shao Feng
 Author-email: just.shao.007@gmail.com
 License: Apache License 2.0
 Keywords: intellipandora
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -34,23 +34,25 @@
 Requires-Dist: six
 Requires-Dist: pendulum
 Requires-Dist: tabulate
 Requires-Dist: retrying
 Requires-Dist: assertpy
 Requires-Dist: bs4
 Requires-Dist: pluggy
-Requires-Dist: pyyaml
-Requires-Dist: pycryptodome
+Requires-Dist: PyYAML
+Requires-Dist: cryptography
 Requires-Dist: urllib3
 Requires-Dist: requests
-Requires-Dist: httpretty
 Requires-Dist: websockets
+Requires-Dist: httpretty
 Requires-Dist: pytest
 Requires-Dist: robotframework
 Requires-Dist: psutil
+Requires-Dist: Jinja2
+Requires-Dist: pymysql
 
 # IntelliPandora
 
 ## 一、概要
 
 > IntelliPandora 是Python开发以提供通用能力测试框架
 >
@@ -80,9 +82,24 @@
 ### 使用手册(待添加)
 > 包含了框架使用，例如http如何调用，用于接口自动化测试
 * [IntelliPandora使用手册](docs/usr/user_guider.md)
 
 
 ## 三、开发
 * [IntelliPandora开发说明](docs/dev/IntelliPandora_Dev.md)
+* 
+### **3.1 框架结构介绍**
+> 代码都在***src/intellipandora***
+* **core**: 提供自动化核心能力接口。
+  * **base**: 基础类(基类)，如SingletonClass、BaseRepository等
+  * **protocol**: 提供协议能力，支持与被测对象交互/通信。如http、grpc、websocket等
+  * **engine**: 提供执行引擎，提供框架核心功能，如自动生成、加密、分布式执行处理等
+* **common**: 基础方法封装，支持自动化测试断言、数据准备、数据处理等
+* **run**: 框架的命令行模块
+* **utils**: 框架基础功能，如log、error...
+* **conf**: 配置文件
+
 
+## GitHub Feature
 
+1. You can use Readme\_XXX.md to support different languages, such as Readme\_en.md, Readme\_zh.md
+2. Explore open source project [IntelliPandora](https://github.com/Conan-Shao/IntelliPandora)
```

## Comparing `intellipandora-1.0.6.dist-info/RECORD` & `intellipandora-1.0.7.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,75 @@
-intellipandora-1.0.6.data/scripts/runner.py,sha256=PY1i5YDyMo6NpEajxWwGfO3NlvP47NcAVP-lgI2cigY,173
-ipandora/CHANGELOG,sha256=Bgnj5uo99GUTZdepodWt82Dc-Qg4Up5z-YsYUH6XVoY,652
+intellipandora-1.0.7.data/scripts/runner.py,sha256=PY1i5YDyMo6NpEajxWwGfO3NlvP47NcAVP-lgI2cigY,173
+ipandora/CHANGELOG,sha256=7BNGNsg9_5VJ3IdZ2K7h9Qo5N3q6tJBm11tEnAWJbwU,893
 ipandora/__init__.py,sha256=E5O_DsKDHoEyLVSq0z28FbuviMrBGUxHYLcZwAa_mrQ,93
 ipandora/version.py,sha256=sH31l0BYCiRZ137xEQIoFhJbEhocRHJoTPq9uNNlwt0,643
 ipandora/common/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
-ipandora/common/fileaction.py,sha256=xcuktwp_todw7UGDAELODrXxgFk6s3arDQV7vuaRIuo,1399
-ipandora/common/filewriter.py,sha256=955SGQtKaZzpon1uKNfngzx8mZWxaNCV4R7AlT4He7E,4580
-ipandora/common/mysqlaction.py,sha256=q4TDAzklQpqc6qWFv0eXqB0J9CGc1tBzlspalQFooCQ,2613
-ipandora/common/systeminfo.py,sha256=3dbu1x7VmWWYP03tyxokn9n7K0-2atF24Hd9zLCFU78,3150
+ipandora/common/dictutils.py,sha256=A-aIFawYvwCI52tA9Xd3ddesJdereKm44OS0_WVaAes,826
+ipandora/common/mysqlaction.py,sha256=VCCs09TusSRGUfDO5bVMfInJKzcqhgWUAw4ihCvy94Q,3008
+ipandora/common/stringaction.py,sha256=Nc33hzabwO7fHHlYjh2RiE_TWSdr0iFVk0Je2RwUkRI,3605
+ipandora/common/systeminfo.py,sha256=0-fYqK_pkiK2MWcksuB0GLGxmdsD80RPsICjj1eyAY4,3304
+ipandora/common/timeutils.py,sha256=EW4h7KQRkEBvmbjOBtLybMPjoSdUEMrMF0oYnmI7_pc,4218
 ipandora/conf/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
-ipandora/core/__init__.py,sha256=-bV2CrT82WTpezUF83DduQvJ3NpO69HWqJceEPi9U3c,465
-ipandora/core/log.py,sha256=PEp_jNlBltTd8xotfI2yJ6n_4nvPY0zMa0gre3OfMxk,2251
+ipandora/core/__init__.py,sha256=vZgX0fLc3ju1z_Whmg8qz3-dwuziz_wbCkRGfufTgKQ,396
 ipandora/core/base/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
 ipandora/core/base/classwrap/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
+ipandora/core/base/classwrap/attrvaluesplit.py,sha256=Vsjh-x65LUZEd9ogQjjr6DxR1XkNHNAwSIQlTz00xnY,1061
 ipandora/core/base/classwrap/classproperty.py,sha256=24A6bnry6nC8bcpKG2X2so6bOUSB7oYNHvYrRrIO5qA,1487
 ipandora/core/base/classwrap/multihandle.py,sha256=WHoVK8TjspPjJ6tdWfrdwOL6ON-wounfdYQcjBPDLEY,2787
 ipandora/core/base/classwrap/singleton.py,sha256=r_1SWj0cFzUiUrXRfX3h-2-rTulE1ube3lW8I2637bs,608
 ipandora/core/base/data/__init__.py,sha256=kN56eO5g7PvMHmcdhzuKA2UuzaQBf2ZbCBzmp0WYPI4,95
 ipandora/core/base/data/markdata.py,sha256=NPJCf5KkH5is6TwLCS8fZu1Osx2xA1IZOZY_k-9z-ts,1155
 ipandora/core/base/loglib/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
 ipandora/core/base/loglib/log.py,sha256=8FxKjE4skqXPudjLM8v6-WkZPJC1dXdDUV4c_E90MsA,995
+ipandora/core/base/repository/__init__.py,sha256=pB_MW2OvHVyHaGalZCbpk1xJVi_E04t9bFeXp2-pRCk,95
+ipandora/core/base/repository/baserepository.py,sha256=o8c_I0iMI4MHpFDKthS_5LiLOAvVBDl6eRNiqULO940,4691
 ipandora/core/engine/__init__.py,sha256=wNPK4pG-Zhm5GaohCQcLVHbCfzzFaaqc0AnZNvi0eYQ,95
-ipandora/core/engine/generator/__init__.py,sha256=E3W_xykDmkzTMtJy559LUogPdbuOIGokwYxoBsGaT8E,734
-ipandora/core/engine/generator/model/__init__.py,sha256=B4JU9LD3_k2Bzrr-emKvvn86tkm3NvPgSnwD0nUOVLo,286
+ipandora/core/engine/crypto/__init__.py,sha256=blbxfw0bVwgaNND_ck7NednAuFmPJ29r8_kGc2_d94w,95
+ipandora/core/engine/crypto/aescryptographer.py,sha256=rFA46PAqbKjx45wilLjO3kUrRrn7oI7Lkksaaugv70E,3997
+ipandora/core/engine/crypto/crypto.py,sha256=5LN57O3XbSr2DN-Q659XusMbMI3clA2xJVQGEyv5UAA,2229
+ipandora/core/engine/crypto/cryptoabc.py,sha256=KHRoWs1Ic2n3kixJrxkLEhKdLll_Pz27GB15G7PWBNA,285
+ipandora/core/engine/crypto/fercryptographer.py,sha256=N3uOoTgx6buf9hMJwB7gFyvX1Eu5w9w7uF85Xbfg1Sk,2804
+ipandora/core/engine/crypto/rsacryptographer.py,sha256=Kb75XlrGztQdqufaSQl0CCTyAbE28s5gezFE3odUzrQ,3898
+ipandora/core/engine/generator/__init__.py,sha256=F8A_m8EVcA1_hkfjR6027QYp13KitZVRhpeBTNGvb4I,733
+ipandora/core/engine/generator/model/__init__.py,sha256=TTddEo3r12HZYiUTYZzWWd_sIyWBe9fWMSk07shH7A8,497
 ipandora/core/engine/generator/model/data/__init__.py,sha256=w0FTd9iMJpAQoYC1z8tLi8_5WUdv2BT-kqq163bAglU,94
+ipandora/core/engine/generator/model/data/moduledata.py,sha256=9w35IZ0amhJsWgG5gGBiiBHTQ0ja7qlT9Zvay2R07c0,94
 ipandora/core/engine/generator/model/data/robotcase.py,sha256=8Gc1NJW4NucJLKjdjekKvjqodhhl_gAmg_O6mdSH2To,1969
-ipandora/core/engine/generator/model/data/robotsuite.py,sha256=R9kPcPSUxLhK00WRokFMHe1Cc_03D_6HG64jGDMzXaI,8774
+ipandora/core/engine/generator/model/data/robotcaselegacy.py,sha256=c2aT7vjDFHpZFo983zjo7tFPi61h5l0vNinbnh-VS1c,3078
+ipandora/core/engine/generator/model/data/robotsuite.py,sha256=h1lsowZZ58NXwQO88h0vhcOIioYBouxgGpQX1jjpsLY,798
+ipandora/core/engine/generator/model/data/robotsuitelegacy.py,sha256=mjyMYlTHD1DCpE7iaWabsG8SHDMMQiOyuUOc9gpra-w,8941
+ipandora/core/engine/generator/model/data/testcase.py,sha256=jk9Qzfj1M-oT_9jTGdfrMiw7hlaZjEdtjjQdzuMMQxI,4105
 ipandora/core/engine/generator/model/handler/__init__.py,sha256=DvEZBI8XxHtdB6HDWo_cw8KdMoQtyRx0G9PgWdTJkUI,95
-ipandora/core/engine/generator/model/handler/robotrenderer.py,sha256=JHGW7OYmjLnAQ852JBroDTvOzZSqDFux_Ata7eWV-T4,1638
+ipandora/core/engine/generator/model/handler/robotrenderer.py,sha256=20nReXjdLh6yoyO9oumroAwrNBEx5Z6MLhQn_PsYKEI,3412
+ipandora/core/engine/generator/model/handler/robotrendererlegacy.py,sha256=RT0BohHmN8MHCHqSxpytqhOV56lVmNc2bpDClttVRaE,1932
 ipandora/core/engine/generator/provider/__init__.py,sha256=DvEZBI8XxHtdB6HDWo_cw8KdMoQtyRx0G9PgWdTJkUI,95
 ipandora/core/engine/generator/provider/caseprovider.py,sha256=4RKSJxbMUO1jFnGTOpMY9PdDJ7YekDnWv1b-PNX3UfQ,825
-ipandora/core/engine/generator/provider/robotprovider.py,sha256=hE4jW4WCTQkCQAhuAN4PaM239Hi66HpHFX586h0h16c,2315
+ipandora/core/engine/generator/provider/robotbaseprovider.py,sha256=HCVSuo1NHf7toI-Uo4h2qtj6oUoLB4iKo-5rjijOjYs,838
+ipandora/core/engine/generator/provider/robotprovider.py,sha256=eHUIyjVZFRnwG500zclftbDXTxxcjWtEGaPgSLP8UfM,2854
+ipandora/core/engine/generator/repository/__init__.py,sha256=blbxfw0bVwgaNND_ck7NednAuFmPJ29r8_kGc2_d94w,95
+ipandora/core/engine/generator/repository/modulerepository.py,sha256=6LAALSz-sg7JRu-qY001LDxBaJLZqYIcwy4FXgzPjRY,1418
+ipandora/core/engine/generator/repository/projectrepository.py,sha256=zg_AbsEx2kmLc38p7Xz7CYY-EzBTK47j_S6bJqQzsgg,1496
+ipandora/core/engine/generator/repository/submodulerepository.py,sha256=crdEyA6n3dS3mQAde48I-3eGOLiw1YzKC28GHh8YlkM,1708
+ipandora/core/engine/generator/repository/tagcategoryrepository.py,sha256=VCGIvlAZyyQqYwFV7AnCY7S1KxPd_W8QQALHEoPzupU,2450
+ipandora/core/engine/generator/repository/tagrepository.py,sha256=oXzub_vQS5KQndCTA9ZlJv_eBP20GjbhC_e6fQ0wWeY,3131
+ipandora/core/engine/generator/repository/testcaserepository.py,sha256=VgQzqkSFZo5m1XjfI9pIjnuBnhOIUQcbDA6P6SZRwAI,12370
+ipandora/core/engine/generator/repository/testcasetagsrepository.py,sha256=MHNO-1BA6efoZZaBLC-2ftEFNEC59Q26520AYPUAJl8,2788
+ipandora/core/engine/generator/repository/teststeprepository.py,sha256=mIUYyBdQ6xuqKm0Vi0vKk2pzsjd9k7DvfgIvm4aEEYg,2568
+ipandora/core/engine/generator/service/__init__.py,sha256=5qpoXr2BaGPd7DpBvjlVAA8oDIZU2S2YHYY0mcPbaCg,95
+ipandora/core/engine/generator/service/robotcaseservice.py,sha256=YKaD1m5hQQg0eVZGn0zLtsnAFDLlxGyyiUGqdEcliZg,2813
+ipandora/core/engine/generator/service/testcaseserivce.py,sha256=_OroZQk3AStAk2286Q7-4zxHAQIvbyH_ez3CxzC981Q,9692
 ipandora/core/plugin/__init__.py,sha256=tHpWtfnDG64k3GDFQYRPuVM7u6gswbdLFl_6mKVvao8,314
 ipandora/core/plugin/innerplugin.py,sha256=5jMV_85IvmSQ0btaeD8DzN2hH7_v9WxZ31V01wTOoAA,1038
 ipandora/core/plugin/pluginmanager.py,sha256=zQ8sNJLVweG7gkLJASG8Ryvcan5eSSIcoHXLFhGvQEc,1169
 ipandora/core/plugin/specificationsbuilder.py,sha256=B0n76SmST6GyRVNusGqEshAW2N9uMCpW0lOD85kASFg,3045
 ipandora/core/plugin/interface/__init__.py,sha256=7C65JZ9J_-KseBNo8MQF9mtQwiFRRxXIZDynxyWOIsw,411
 ipandora/core/plugin/interface/endpointsinterface.py,sha256=jf2Adn2GyaVxs_64ro5oTgK2MF2rJhYOdww2L32T06E,231
 ipandora/core/plugin/interface/httpregisterinterface.py,sha256=btfN6z_MIf4BHoIb9bWZiS_dFFjZexaFKHAWsq0-DNI,235
 ipandora/core/plugin/interface/plugininterface.py,sha256=fOn70ZEeVDZ6vwm42M6B1mapmUOI8VCDdg03f9LgFyY,859
-ipandora/core/protocol/__init__.py,sha256=KUqvsIVNtHN9sQPz7xt0ggb6iNcM955xaKPY1JskBCQ,95
+ipandora/core/protocol/__init__.py,sha256=t_Abm0XgU049G8VjdKRuNTZSaBDy8DdjR_sf0szB2aw,585
 ipandora/core/protocol/http/__init__.py,sha256=GCXY7zfHctmVXwbpZ3uuhgKuIuqOd84C8RHGbdjqLzk,585
 ipandora/core/protocol/http/model/__init__.py,sha256=wNPK4pG-Zhm5GaohCQcLVHbCfzzFaaqc0AnZNvi0eYQ,95
 ipandora/core/protocol/http/model/httpmodel.py,sha256=vXv1IiCR0O0iIK6nqGgmrkvPvBor9k6sEtEMguI__0U,2227
 ipandora/core/protocol/http/model/sessionmodel.py,sha256=SYcf_h-D-NPYfIxCMPvERBpchMNOA1XOeUXm0fF2rbk,374
 ipandora/core/protocol/http/model/data/__init__.py,sha256=wNPK4pG-Zhm5GaohCQcLVHbCfzzFaaqc0AnZNvi0eYQ,95
 ipandora/core/protocol/http/model/data/baseobject.py,sha256=qAa_6-LNuPBqlC7QuN0W3pAHwcnh-SOJ4k-qzhU-eZc,1226
 ipandora/core/protocol/http/model/data/requestobject.py,sha256=_59Av21DnHdhfJQSUSg5xGVA7HxanvzTgZCaAd1Tgis,4323
@@ -57,36 +84,40 @@
 ipandora/core/protocol/http/model/option/apioption.py,sha256=gzI0g-KSXVTKGnvqYjT39G2xsnGJqES1CKWN0HpfJvo,1009
 ipandora/core/protocol/http/model/option/httpontion.py,sha256=HmYE39ow6AapfmDtDybxkLx1fxYTppSm5IJP5GuNQ34,236
 ipandora/core/protocol/http/provider/__init__.py,sha256=-MO0Pctdkxpdz8JFeigMq8EVShc5mJr2ZkV9Vzd1_zM,256
 ipandora/core/protocol/http/provider/baseprovider.py,sha256=g9aw5F8qdNF4rQqEKYlFRpRZGNWi92gMJt3NWkMaQsY,2835
 ipandora/core/protocol/http/provider/httpprovider.py,sha256=7-Yh7iZ0TSdF2_ihNr_fSGkNwAm7KuzfoyQ71Cla7JQ,914
 ipandora/core/protocol/http/provider/markprovider.py,sha256=LaycnyOMtBKKgvHu4tOmUitVGoJv_38Zp6nxsOhiXHc,1637
 ipandora/core/schedule/__init__.py,sha256=wNPK4pG-Zhm5GaohCQcLVHbCfzzFaaqc0AnZNvi0eYQ,95
-ipandora/core/schedule/runtime.py,sha256=YlcDHadPm855dSvO8U_XLVE7dtP-KaM9IV9XDAxT_Cw,4649
-ipandora/core/schedule/session.py,sha256=UuGi0xYVHbW0gLngWhJd_jtnFvBR6C8GxvYlMFECbRo,2713
+ipandora/core/schedule/runtime.py,sha256=608DmAXar_BqhoEBcp84dTpfdqmSMySVYolefZNaUO4,8448
+ipandora/core/schedule/session.py,sha256=LSD-HQkT3Sml4MKJMkQelAOIa8m3sTVVRex8F8dSXHQ,2712
 ipandora/core/wrapper/__init__.py,sha256=wNPK4pG-Zhm5GaohCQcLVHbCfzzFaaqc0AnZNvi0eYQ,95
 ipandora/core/wrapper/basewrapper.py,sha256=6mE8RsIx63mEgS_uZD2tQCjyty_BgumRM5QL_vy6-Lg,2103
 ipandora/core/wrapper/requestwrapper.py,sha256=z4mX2gBsgoUnRC1MnVaGTG4MAe6XHceQ_dOU0KNzL5o,2793
 ipandora/core/wrapper/interface/__init__.py,sha256=wNPK4pG-Zhm5GaohCQcLVHbCfzzFaaqc0AnZNvi0eYQ,95
 ipandora/core/wrapper/interface/requestinterface.py,sha256=NRgotfPCQXJSC_dzZ2DqSTHAlp9VRAwy_9KYdaqkmUs,535
 ipandora/run/__init__.py,sha256=p-y1lhpp8-lmxsHhQYj51fhH1YdTvt7v1Yuik87BEbM,196
 ipandora/run/cmd.py,sha256=Byg6yzTto-5Kx_f4oUb50aPyceYZauK9ofc4VOmFDdM,1106
 ipandora/run/commandbase.py,sha256=bztIeQlzyAtvOUGhrbCU5TfHepkvYtuTxtqkeLgt_-g,1393
 ipandora/run/commandmanager.py,sha256=bX3xZNZrNgcbgF8GrCXM6G6Psc6aDFRXT93VHqwl1qY,2115
 ipandora/run/ipandoracommand.py,sha256=O0yAoEsqSRQE4AiwUMm_VrDBBEHY0H0RT34OpPFwOaE,6447
 ipandora/run/runner.py,sha256=PY1i5YDyMo6NpEajxWwGfO3NlvP47NcAVP-lgI2cigY,173
 ipandora/run/commands/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
 ipandora/run/commands/project.py,sha256=eP1TE9675OiBSnR0xaHGTQO95H8Jue1guZHIQIAM3Yo,1867
 ipandora/utils/__init__.py,sha256=Y5poEhdll69EYWO4FC-FkPA_0bRJhWCojeOiEOuTugw,93
-ipandora/utils/error.py,sha256=I9s3soTJ4ikkuYat-taDccyM4WVHUDutFjwCCprD-y4,1386
+ipandora/utils/error.py,sha256=cyNp57P4rAopczIOS_LmELeXrTyEGA8lrH0wIK8-AVc,1496
+ipandora/utils/fileload.py,sha256=MFQ4uw15tKV2m6NL32ubqZ9TLCcKiUj6q60sVVebnLc,1413
+ipandora/utils/filewriter.py,sha256=S_Ju4dGJkhXKtrl2dibM_2RXdHzP1hjPHfoQhHTa4kw,5133
 ipandora/utils/importpath.py,sha256=8yDKTlVjwxGETrLmBC6Jccoyirx-JUTy6-5Wp7zhCkk,1805
-ipandora/utils/log.py,sha256=dho7A2foCkCEmxmbeyiWq7bbdEClKcvwbdOZ8BuI2UQ,1080
+ipandora/utils/log.py,sha256=eWhReua7bBuSEbnfRQM1WADjO8YUbHmC-9hbama2jHI,3269
 ipandora/utils/match.py,sha256=42mLplqpxF_NFDPSGxhztBow3WaVbPWnVQ9LJGQhPdI,2408
 ipandora/utils/niceline.py,sha256=w_VIC_i6rmC0r5uaE_lxef0kEy9mfkYUn7wqYBzQkFY,521
+ipandora/utils/pathutils.py,sha256=GpmnARi_OiqdQQQRopiikLRHkhAuVplDDrRwv7NmA5k,3650
+ipandora/utils/robotlogparser.py,sha256=ybqwG0vVEu9Vf6yDDbBDt7RyTVVvTk_HTC-pxK8ToqE,4769
 ipandora/utils/variable.py,sha256=DPGdOa2Zf8aZJgXZBv0yETfjgqMe7UI8I_4BYToqv8M,2183
-intellipandora-1.0.6.dist-info/AUTHORS.rst,sha256=FKR3o3pakwdsG63888OhufBDR4E-GKQmpVDsL7HOCdw,479
-intellipandora-1.0.6.dist-info/LICENSE,sha256=t-0geih-ExGDCpCpE0YPuwA8pqA3vDt7l76v0jXiGo4,11342
-intellipandora-1.0.6.dist-info/METADATA,sha256=zNWc_TJ5xVsMY89m5-7XAq21n4hjGBcea7JXJHllDiE,2572
-intellipandora-1.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-intellipandora-1.0.6.dist-info/entry_points.txt,sha256=pw27C7OcHWLb7to_EkzyC9uc3Fdg8_pUrjjQ1kNQtfE,55
-intellipandora-1.0.6.dist-info/top_level.txt,sha256=bTT1b-jSKiifyEy34Li89A7IZQ3Q8oYjxB3bRGi9i0g,9
-intellipandora-1.0.6.dist-info/RECORD,,
+intellipandora-1.0.7.dist-info/AUTHORS.rst,sha256=FKR3o3pakwdsG63888OhufBDR4E-GKQmpVDsL7HOCdw,479
+intellipandora-1.0.7.dist-info/LICENSE,sha256=t-0geih-ExGDCpCpE0YPuwA8pqA3vDt7l76v0jXiGo4,11342
+intellipandora-1.0.7.dist-info/METADATA,sha256=66QRkjYFBAsHNYay7qUhIBt8X1YUbSZqOqPxC-nQqNw,3471
+intellipandora-1.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+intellipandora-1.0.7.dist-info/entry_points.txt,sha256=pw27C7OcHWLb7to_EkzyC9uc3Fdg8_pUrjjQ1kNQtfE,55
+intellipandora-1.0.7.dist-info/top_level.txt,sha256=bTT1b-jSKiifyEy34Li89A7IZQ3Q8oYjxB3bRGi9i0g,9
+intellipandora-1.0.7.dist-info/RECORD,,
```

