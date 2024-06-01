# Comparing `tmp/plex-api-client-0.7.0.tar.gz` & `tmp/plex-api-client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-api-client-0.7.0.tar", last modified: Thu May 23 15:59:01 2024, max compression
+gzip compressed data, was "plex-api-client-0.8.0.tar", last modified: Sat Jun  1 01:24:49 2024, max compression
```

## Comparing `plex-api-client-0.7.0.tar` & `plex-api-client-0.8.0.tar`

### file list

```diff
@@ -1,171 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    20824 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.749991 plex-api-client-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.753991 plex-api-client-0.7.0/src/plex_api/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.753991 plex-api-client-0.7.0/src/plex_api/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    18356 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/hubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38654 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.753991 plex-api-client-0.7.0/src/plex_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.753991 plex-api-client-0.7.0/src/plex_api/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.761991 plex-api-client-0.7.0/src/plex_api/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/uploadplaylist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.761991 plex-api-client-0.7.0/src/plex_api/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/src/plex_api/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/searchlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/uploadplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    34579 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    28675 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/src/plex_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/src/plex_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20824 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.530963 plex-api-client-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-06-01 01:24:49.530963 plex-api-client-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:24:49.530963 plex-api-client-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.506963 plex-api-client-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.506963 plex-api-client-0.8.0/src/plex_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.510963 plex-api-client-0.8.0/src/plex_api/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18356 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/hubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44220 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.510963 plex-api-client-0.8.0/src/plex_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.510963 plex-api-client-0.8.0/src/plex_api/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.518963 plex-api-client-0.8.0/src/plex_api/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getlibraryitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/searchlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/errors/uploadplaylist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.518963 plex-api-client-0.8.0/src/plex_api/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.530963 plex-api-client-0.8.0/src/plex_api/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18874 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getlibraryitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/searchlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/models/operations/uploadplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34579 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28675 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.530963 plex-api-client-0.8.0/src/plex_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-06-01 01:24:37.000000 plex-api-client-0.8.0/src/plex_api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:24:49.530963 plex-api-client-0.8.0/src/plex_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-06-01 01:24:49.000000 plex-api-client-0.8.0/src/plex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-06-01 01:24:49.000000 plex-api-client-0.8.0/src/plex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:24:49.000000 plex-api-client-0.8.0/src/plex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-06-01 01:24:49.000000 plex-api-client-0.8.0/src/plex_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 01:24:49.000000 plex-api-client-0.8.0/src/plex_api_client.egg-info/top_level.txt
```

### Comparing `plex-api-client-0.7.0/LICENSE.md` & `plex-api-client-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/PKG-INFO` & `plex-api-client-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
@@ -31,14 +31,15 @@
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -96,14 +97,15 @@
         ### [library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md)
         
         * [get_file_hash](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_file_hash) - Get Hash Value
         * [get_recently_added](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_recently_added) - Get Recently Added
         * [get_libraries](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_libraries) - Get All Libraries
         * [get_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_library) - Get Library Details
         * [delete_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#delete_library) - Delete Library Section
+        * [get_library_items](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_library_items) - Get Library Items
         * [refresh_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#refresh_library) - Refresh Library
         * [search_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#search_library) - Search Library
         * [get_metadata](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata) - Get Items Metadata
         * [get_metadata_children](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata_children) - Get Items Children
         * [get_on_deck](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_on_deck) - Get On Deck
         
         ### [log](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/log/README.md)
@@ -172,14 +174,15 @@
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
         res = None
         try:
             res = s.server.get_server_capabilities()
+        
         except errors.GetServerCapabilitiesResponseBody as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -208,14 +211,15 @@
         
         s = plex_api.PlexAPI(
             server_idx=0,
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -235,14 +239,15 @@
         
         s = plex_api.PlexAPI(
             server_url="{protocol}://{ip}:{port}",
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -253,14 +258,15 @@
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2")
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -298,14 +304,15 @@
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -336,14 +343,15 @@
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.7.0 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.8.0 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
@@ -71,15 +71,17 @@
 //github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_recently_added) - Get Recently Added * [get_libraries](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_libraries) - Get All Libraries * [get_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_library) - Get Library Details * [delete_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
-README.md#delete_library) - Delete Library Section * [refresh_library](https://
+README.md#delete_library) - Delete Library Section * [get_library_items](https:
+//github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
+README.md#get_library_items) - Get Library Items * [refresh_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#refresh_library) - Refresh Library * [search_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#search_library) - Search Library * [get_metadata](https://github.com/
 LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata) - Get
 Items Metadata * [get_metadata_children](https://github.com/LukeHagar/plexpy/
 blob/master/docs/sdks/library/README.md#get_metadata_children) - Get Items
```

### Comparing `plex-api-client-0.7.0/README.md` & `plex-api-client-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import plex_api
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
+
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -89,14 +90,15 @@
 ### [library](docs/sdks/library/README.md)
 
 * [get_file_hash](docs/sdks/library/README.md#get_file_hash) - Get Hash Value
 * [get_recently_added](docs/sdks/library/README.md#get_recently_added) - Get Recently Added
 * [get_libraries](docs/sdks/library/README.md#get_libraries) - Get All Libraries
 * [get_library](docs/sdks/library/README.md#get_library) - Get Library Details
 * [delete_library](docs/sdks/library/README.md#delete_library) - Delete Library Section
+* [get_library_items](docs/sdks/library/README.md#get_library_items) - Get Library Items
 * [refresh_library](docs/sdks/library/README.md#refresh_library) - Refresh Library
 * [search_library](docs/sdks/library/README.md#search_library) - Search Library
 * [get_metadata](docs/sdks/library/README.md#get_metadata) - Get Items Metadata
 * [get_metadata_children](docs/sdks/library/README.md#get_metadata_children) - Get Items Children
 * [get_on_deck](docs/sdks/library/README.md#get_on_deck) - Get On Deck
 
 ### [log](docs/sdks/log/README.md)
@@ -165,14 +167,15 @@
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
 res = None
 try:
     res = s.server.get_server_capabilities()
+
 except errors.GetServerCapabilitiesResponseBody as e:
     # handle exception
     raise(e)
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
@@ -201,14 +204,15 @@
 
 s = plex_api.PlexAPI(
     server_idx=0,
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
+
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -228,14 +232,15 @@
 
 s = plex_api.PlexAPI(
     server_url="{protocol}://{ip}:{port}",
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
+
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -246,14 +251,15 @@
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     x_plex_client_identifier='Postman',
 )
 
+
 res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2")
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -291,14 +297,15 @@
 import plex_api
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
+
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -329,14 +336,15 @@
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     x_plex_client_identifier='Postman',
 )
 
+
 res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
```

#### html2text {}

```diff
@@ -44,34 +44,35 @@
 [get_search_results](docs/sdks/search/README.md#get_search_results) - Get
 Search Results ### [library](docs/sdks/library/README.md) * [get_file_hash]
 (docs/sdks/library/README.md#get_file_hash) - Get Hash Value *
 [get_recently_added](docs/sdks/library/README.md#get_recently_added) - Get
 Recently Added * [get_libraries](docs/sdks/library/README.md#get_libraries) -
 Get All Libraries * [get_library](docs/sdks/library/README.md#get_library) -
 Get Library Details * [delete_library](docs/sdks/library/
-README.md#delete_library) - Delete Library Section * [refresh_library](docs/
-sdks/library/README.md#refresh_library) - Refresh Library * [search_library]
-(docs/sdks/library/README.md#search_library) - Search Library * [get_metadata]
-(docs/sdks/library/README.md#get_metadata) - Get Items Metadata *
-[get_metadata_children](docs/sdks/library/README.md#get_metadata_children) -
-Get Items Children * [get_on_deck](docs/sdks/library/README.md#get_on_deck) -
-Get On Deck ### [log](docs/sdks/log/README.md) * [log_line](docs/sdks/log/
-README.md#log_line) - Logging a single line message. * [log_multi_line](docs/
-sdks/log/README.md#log_multi_line) - Logging a multi-line message *
-[enable_paper_trail](docs/sdks/log/README.md#enable_paper_trail) - Enabling
-Papertrail ### [plex](docs/sdks/plex/README.md) * [get_pin](docs/sdks/plex/
-README.md#get_pin) - Get a Pin * [get_token](docs/sdks/plex/
-README.md#get_token) - Get Access Token ### [playlists](docs/sdks/playlists/
-README.md) * [create_playlist](docs/sdks/playlists/README.md#create_playlist) -
-Create a Playlist * [get_playlists](docs/sdks/playlists/
-README.md#get_playlists) - Get All Playlists * [get_playlist](docs/sdks/
-playlists/README.md#get_playlist) - Retrieve Playlist * [delete_playlist](docs/
-sdks/playlists/README.md#delete_playlist) - Deletes a Playlist *
-[update_playlist](docs/sdks/playlists/README.md#update_playlist) - Update a
-Playlist * [get_playlist_contents](docs/sdks/playlists/
+README.md#delete_library) - Delete Library Section * [get_library_items](docs/
+sdks/library/README.md#get_library_items) - Get Library Items *
+[refresh_library](docs/sdks/library/README.md#refresh_library) - Refresh
+Library * [search_library](docs/sdks/library/README.md#search_library) - Search
+Library * [get_metadata](docs/sdks/library/README.md#get_metadata) - Get Items
+Metadata * [get_metadata_children](docs/sdks/library/
+README.md#get_metadata_children) - Get Items Children * [get_on_deck](docs/
+sdks/library/README.md#get_on_deck) - Get On Deck ### [log](docs/sdks/log/
+README.md) * [log_line](docs/sdks/log/README.md#log_line) - Logging a single
+line message. * [log_multi_line](docs/sdks/log/README.md#log_multi_line) -
+Logging a multi-line message * [enable_paper_trail](docs/sdks/log/
+README.md#enable_paper_trail) - Enabling Papertrail ### [plex](docs/sdks/plex/
+README.md) * [get_pin](docs/sdks/plex/README.md#get_pin) - Get a Pin *
+[get_token](docs/sdks/plex/README.md#get_token) - Get Access Token ###
+[playlists](docs/sdks/playlists/README.md) * [create_playlist](docs/sdks/
+playlists/README.md#create_playlist) - Create a Playlist * [get_playlists]
+(docs/sdks/playlists/README.md#get_playlists) - Get All Playlists *
+[get_playlist](docs/sdks/playlists/README.md#get_playlist) - Retrieve Playlist
+* [delete_playlist](docs/sdks/playlists/README.md#delete_playlist) - Deletes a
+Playlist * [update_playlist](docs/sdks/playlists/README.md#update_playlist) -
+Update a Playlist * [get_playlist_contents](docs/sdks/playlists/
 README.md#get_playlist_contents) - Retrieve Playlist Contents *
 [clear_playlist_contents](docs/sdks/playlists/
 README.md#clear_playlist_contents) - Delete Playlist Contents *
 [add_playlist_contents](docs/sdks/playlists/README.md#add_playlist_contents) -
 Adding to a Playlist * [upload_playlist](docs/sdks/playlists/
 README.md#upload_playlist) - Upload Playlist ### [authentication](docs/sdks/
 authentication/README.md) * [get_transient_token](docs/sdks/authentication/
```

### Comparing `plex-api-client-0.7.0/setup.py` & `plex-api-client-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='plex-api-client',
-    version='0.7.0',
+    version='0.8.0',
     author='LukeHagar',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/LukeHagar/plexpy.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `plex-api-client-0.7.0/src/plex_api/_hooks/registration.py` & `plex-api-client-0.8.0/src/plex_api/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/_hooks/sdkhooks.py` & `plex-api-client-0.8.0/src/plex_api/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/_hooks/types.py` & `plex-api-client-0.8.0/src/plex_api/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/activities.py` & `plex-api-client-0.8.0/src/plex_api/activities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/authentication.py` & `plex-api-client-0.8.0/src/plex_api/authentication.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/butler.py` & `plex-api-client-0.8.0/src/plex_api/butler.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/hubs.py` & `plex-api-client-0.8.0/src/plex_api/hubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/library.py` & `plex-api-client-0.8.0/src/plex_api/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,14 +389,104 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
+    def get_library_items(self, section_id: int, tag: operations.Tag) -> operations.GetLibraryItemsResponse:
+        r"""Get Library Items
+        Fetches details from a specific section of the library identified by a section key and a tag. The tag parameter accepts the following values:
+        - `all`: All items in the section.
+        - `unwatched`: Items that have not been played.
+        - `newest`: Items that are recently released.
+        - `recentlyAdded`: Items that are recently added to the library.
+        - `recentlyViewed`: Items that were recently viewed.
+        - `onDeck`: Items to continue watching.
+        - `collection`: Items categorized by collection.
+        - `edition`: Items categorized by edition.
+        - `genre`: Items categorized by genre.
+        - `year`: Items categorized by year of release.
+        - `decade`: Items categorized by decade.
+        - `director`: Items categorized by director.
+        - `actor`: Items categorized by starring actor.
+        - `country`: Items categorized by country of origin.
+        - `contentRating`: Items categorized by content rating.
+        - `rating`: Items categorized by rating.
+        - `resolution`: Items categorized by resolution.
+        - `firstCharacter`: Items categorized by the first letter.
+        - `folder`: Items categorized by folder.
+        """
+        hook_ctx = HookContext(operation_id='getLibraryItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetLibraryItemsRequest(
+            section_id=section_id,
+            tag=tag,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/library/sections/{sectionId}/{tag}', request)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        res = operations.GetLibraryItemsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibraryItemsResponseBody])
+                res.object = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.GetLibraryItemsResponseBody)
+                out.raw_response = http_res
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
     def refresh_library(self, section_id: float) -> operations.RefreshLibraryResponse:
         r"""Refresh Library
         This endpoint Refreshes the library.
         """
         hook_ctx = HookContext(operation_id='refreshLibrary', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.RefreshLibraryRequest(
             section_id=section_id,
@@ -503,15 +593,15 @@
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+        if utils.match_status_codes(['400','401','4XX','5XX'], http_res.status_code):
             result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
             if e is not None:
                 raise e
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
@@ -524,16 +614,25 @@
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchLibraryResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+        elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.SearchLibraryResponseBody)
+                out.raw_response = http_res
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `plex-api-client-0.7.0/src/plex_api/log.py` & `plex-api-client-0.8.0/src/plex_api/log.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/media.py` & `plex-api-client-0.8.0/src/plex_api/media.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/__init__.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .getbutlertasks import *
 from .getdevices import *
 from .getfilehash import *
 from .getglobalhubs import *
 from .getlibraries import *
 from .getlibrary import *
 from .getlibraryhubs import *
+from .getlibraryitems import *
 from .getmetadata import *
 from .getmetadatachildren import *
 from .getmyplexaccount import *
 from .getondeck import *
 from .getpin import *
 from .getplaylist import *
 from .getplaylistcontents import *
@@ -46,18 +47,19 @@
 from .logmultiline import *
 from .markplayed import *
 from .markunplayed import *
 from .performsearch import *
 from .performvoicesearch import *
 from .refreshlibrary import *
 from .sdkerror import *
+from .searchlibrary import *
 from .startalltasks import *
 from .starttask import *
 from .startuniversaltranscode import *
 from .stopalltasks import *
 from .stoptask import *
 from .stoptranscodesession import *
 from .updateplaylist import *
 from .updateplayprogress import *
 from .uploadplaylist import *
 
-__all__ = ["AddPlaylistContentsErrors","AddPlaylistContentsResponseBody","ApplyUpdatesErrors","ApplyUpdatesResponseBody","CancelServerActivitiesErrors","CancelServerActivitiesResponseBody","CheckForUpdatesErrors","CheckForUpdatesResponseBody","ClearPlaylistContentsErrors","ClearPlaylistContentsResponseBody","CreatePlaylistErrors","CreatePlaylistResponseBody","DeleteLibraryErrors","DeleteLibraryResponseBody","DeletePlaylistErrors","DeletePlaylistResponseBody","EnablePaperTrailErrors","EnablePaperTrailResponseBody","Errors","GetAvailableClientsErrors","GetAvailableClientsResponseBody","GetButlerTasksErrors","GetButlerTasksResponseBody","GetDevicesErrors","GetDevicesResponseBody","GetFileHashErrors","GetFileHashResponseBody","GetGlobalHubsErrors","GetGlobalHubsResponseBody","GetLibrariesErrors","GetLibrariesResponseBody","GetLibraryErrors","GetLibraryHubsErrors","GetLibraryHubsResponseBody","GetLibraryResponseBody","GetMetadataChildrenErrors","GetMetadataChildrenResponseBody","GetMetadataErrors","GetMetadataResponseBody","GetMyPlexAccountErrors","GetMyPlexAccountResponseBody","GetOnDeckErrors","GetOnDeckResponseBody","GetPinErrors","GetPinResponseBody","GetPlaylistContentsErrors","GetPlaylistContentsResponseBody","GetPlaylistErrors","GetPlaylistResponseBody","GetPlaylistsErrors","GetPlaylistsResponseBody","GetRecentlyAddedErrors","GetRecentlyAddedResponseBody","GetResizedPhotoErrors","GetResizedPhotoResponseBody","GetSearchResultsErrors","GetSearchResultsResponseBody","GetServerActivitiesErrors","GetServerActivitiesResponseBody","GetServerCapabilitiesResponseBody","GetServerIdentityErrors","GetServerIdentityResponseBody","GetServerListErrors","GetServerListResponseBody","GetServerPreferencesErrors","GetServerPreferencesResponseBody","GetSessionHistoryErrors","GetSessionHistoryResponseBody","GetSessionsErrors","GetSessionsResponseBody","GetSourceConnectionInformationErrors","GetSourceConnectionInformationResponseBody","GetStatisticsErrors","GetStatisticsResponseBody","GetTimelineErrors","GetTimelineResponseBody","GetTokenErrors","GetTokenResponseBody","GetTranscodeSessionsErrors","GetTranscodeSessionsResponseBody","GetTransientTokenErrors","GetTransientTokenResponseBody","GetUpdateStatusErrors","GetUpdateStatusResponseBody","LogLineErrors","LogLineResponseBody","LogMultiLineErrors","LogMultiLineResponseBody","MarkPlayedErrors","MarkPlayedResponseBody","MarkUnplayedErrors","MarkUnplayedResponseBody","PerformSearchErrors","PerformSearchResponseBody","PerformVoiceSearchErrors","PerformVoiceSearchResponseBody","RefreshLibraryErrors","RefreshLibraryResponseBody","SDKError","StartAllTasksErrors","StartAllTasksResponseBody","StartTaskErrors","StartTaskResponseBody","StartUniversalTranscodeErrors","StartUniversalTranscodeResponseBody","StopAllTasksErrors","StopAllTasksResponseBody","StopTaskErrors","StopTaskResponseBody","StopTranscodeSessionErrors","StopTranscodeSessionResponseBody","UpdatePlayProgressErrors","UpdatePlayProgressResponseBody","UpdatePlaylistErrors","UpdatePlaylistResponseBody","UploadPlaylistErrors","UploadPlaylistResponseBody"]
+__all__ = ["AddPlaylistContentsErrors","AddPlaylistContentsResponseBody","ApplyUpdatesErrors","ApplyUpdatesResponseBody","CancelServerActivitiesErrors","CancelServerActivitiesResponseBody","CheckForUpdatesErrors","CheckForUpdatesResponseBody","ClearPlaylistContentsErrors","ClearPlaylistContentsResponseBody","CreatePlaylistErrors","CreatePlaylistResponseBody","DeleteLibraryErrors","DeleteLibraryResponseBody","DeletePlaylistErrors","DeletePlaylistResponseBody","EnablePaperTrailErrors","EnablePaperTrailResponseBody","Errors","GetAvailableClientsErrors","GetAvailableClientsResponseBody","GetButlerTasksErrors","GetButlerTasksResponseBody","GetDevicesErrors","GetDevicesResponseBody","GetFileHashErrors","GetFileHashResponseBody","GetGlobalHubsErrors","GetGlobalHubsResponseBody","GetLibrariesErrors","GetLibrariesResponseBody","GetLibraryErrors","GetLibraryHubsErrors","GetLibraryHubsResponseBody","GetLibraryItemsErrors","GetLibraryItemsResponseBody","GetLibraryResponseBody","GetMetadataChildrenErrors","GetMetadataChildrenResponseBody","GetMetadataErrors","GetMetadataResponseBody","GetMyPlexAccountErrors","GetMyPlexAccountResponseBody","GetOnDeckErrors","GetOnDeckResponseBody","GetPinErrors","GetPinResponseBody","GetPlaylistContentsErrors","GetPlaylistContentsResponseBody","GetPlaylistErrors","GetPlaylistResponseBody","GetPlaylistsErrors","GetPlaylistsResponseBody","GetRecentlyAddedErrors","GetRecentlyAddedResponseBody","GetResizedPhotoErrors","GetResizedPhotoResponseBody","GetSearchResultsErrors","GetSearchResultsResponseBody","GetServerActivitiesErrors","GetServerActivitiesResponseBody","GetServerCapabilitiesResponseBody","GetServerIdentityErrors","GetServerIdentityResponseBody","GetServerListErrors","GetServerListResponseBody","GetServerPreferencesErrors","GetServerPreferencesResponseBody","GetSessionHistoryErrors","GetSessionHistoryResponseBody","GetSessionsErrors","GetSessionsResponseBody","GetSourceConnectionInformationErrors","GetSourceConnectionInformationResponseBody","GetStatisticsErrors","GetStatisticsResponseBody","GetTimelineErrors","GetTimelineResponseBody","GetTokenErrors","GetTokenResponseBody","GetTranscodeSessionsErrors","GetTranscodeSessionsResponseBody","GetTransientTokenErrors","GetTransientTokenResponseBody","GetUpdateStatusErrors","GetUpdateStatusResponseBody","LogLineErrors","LogLineResponseBody","LogMultiLineErrors","LogMultiLineResponseBody","MarkPlayedErrors","MarkPlayedResponseBody","MarkUnplayedErrors","MarkUnplayedResponseBody","PerformSearchErrors","PerformSearchResponseBody","PerformVoiceSearchErrors","PerformVoiceSearchResponseBody","RefreshLibraryErrors","RefreshLibraryResponseBody","SDKError","SearchLibraryErrors","SearchLibraryResponseBody","StartAllTasksErrors","StartAllTasksResponseBody","StartTaskErrors","StartTaskResponseBody","StartUniversalTranscodeErrors","StartUniversalTranscodeResponseBody","StopAllTasksErrors","StopAllTasksResponseBody","StopTaskErrors","StopTaskResponseBody","StopTranscodeSessionErrors","StopTranscodeSessionResponseBody","UpdatePlayProgressErrors","UpdatePlayProgressResponseBody","UpdatePlaylistErrors","UpdatePlaylistResponseBody","UploadPlaylistErrors","UploadPlaylistResponseBody"]
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/addplaylistcontents.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/applyupdates.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/cancelserveractivities.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/checkforupdates.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/clearplaylistcontents.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/createplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/deletelibrary.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/deleteplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/enablepapertrail.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getavailableclients.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getbutlertasks.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getdevices.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getfilehash.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getglobalhubs.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getlibraries.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getlibrary.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getlibraryhubs.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getmetadata.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getmetadatachildren.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getmyplexaccount.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getondeck.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getpin.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getplaylistcontents.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getplaylists.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getrecentlyadded.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getresizedphoto.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getsearchresults.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getserveractivities.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getservercapabilities.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getserveridentity.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getserverlist.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getserverpreferences.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getsessionhistory.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getsessions.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getsourceconnectioninformation.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getstatistics.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/gettimeline.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/gettoken.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/gettranscodesessions.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/gettransienttoken.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/getupdatestatus.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/logline.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/logmultiline.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/markplayed.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/markunplayed.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/performsearch.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/performvoicesearch.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/refreshlibrary.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/sdkerror.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/startalltasks.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/starttask.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/startuniversaltranscode.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/stopalltasks.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/stoptask.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/stoptranscodesession.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/updateplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/updateplayprogress.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/errors/uploadplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/errors/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/internal/globals.py` & `plex-api-client-0.8.0/src/plex_api/models/internal/globals.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/__init__.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .getbutlertasks import *
 from .getdevices import *
 from .getfilehash import *
 from .getglobalhubs import *
 from .getlibraries import *
 from .getlibrary import *
 from .getlibraryhubs import *
+from .getlibraryitems import *
 from .getmetadata import *
 from .getmetadatachildren import *
 from .getmyplexaccount import *
 from .getondeck import *
 from .getpin import *
 from .getplaylist import *
 from .getplaylistcontents import *
@@ -56,8 +57,8 @@
 from .stopalltasks import *
 from .stoptask import *
 from .stoptranscodesession import *
 from .updateplaylist import *
 from .updateplayprogress import *
 from .uploadplaylist import *
 
-__all__ = ["Account","Activity","AddPlaylistContentsMediaContainer","AddPlaylistContentsMetadata","AddPlaylistContentsRequest","AddPlaylistContentsResponse","AddPlaylistContentsResponseBody","ApplyUpdatesRequest","ApplyUpdatesResponse","ButlerTask","ButlerTasks","CancelServerActivitiesRequest","CancelServerActivitiesResponse","CheckForUpdatesRequest","CheckForUpdatesResponse","ClearPlaylistContentsRequest","ClearPlaylistContentsResponse","Context","Country","CreatePlaylistMediaContainer","CreatePlaylistMetadata","CreatePlaylistRequest","CreatePlaylistResponse","CreatePlaylistResponseBody","DeleteLibraryRequest","DeleteLibraryResponse","DeletePlaylistRequest","DeletePlaylistResponse","Device","Director","Directory","Download","EnablePaperTrailResponse","Field","FieldType","Filter","Force","GET_PIN_SERVERS","GET_TOKEN_SERVERS","Genre","GetAvailableClientsMediaContainer","GetAvailableClientsResponse","GetAvailableClientsResponseBody","GetButlerTasksResponse","GetButlerTasksResponseBody","GetDevicesMediaContainer","GetDevicesResponse","GetDevicesResponseBody","GetFileHashRequest","GetFileHashResponse","GetGlobalHubsMediaContainer","GetGlobalHubsMetadata","GetGlobalHubsRequest","GetGlobalHubsResponse","GetGlobalHubsResponseBody","GetLibrariesDirectory","GetLibrariesLocation","GetLibrariesMediaContainer","GetLibrariesResponse","GetLibrariesResponseBody","GetLibraryDirectory","GetLibraryHubsCountry","GetLibraryHubsDirector","GetLibraryHubsGenre","GetLibraryHubsHub","GetLibraryHubsMedia","GetLibraryHubsMediaContainer","GetLibraryHubsMetadata","GetLibraryHubsPart","GetLibraryHubsRequest","GetLibraryHubsResponse","GetLibraryHubsResponseBody","GetLibraryHubsRole","GetLibraryHubsWriter","GetLibraryMediaContainer","GetLibraryRequest","GetLibraryResponse","GetLibraryResponseBody","GetLibraryType","GetMetadataChildrenDirectory","GetMetadataChildrenMediaContainer","GetMetadataChildrenMetadata","GetMetadataChildrenRequest","GetMetadataChildrenResponse","GetMetadataChildrenResponseBody","GetMetadataCountry","GetMetadataDirector","GetMetadataGenre","GetMetadataMedia","GetMetadataMediaContainer","GetMetadataMetadata","GetMetadataPart","GetMetadataRequest","GetMetadataResponse","GetMetadataResponseBody","GetMetadataRole","GetMetadataWriter","GetMyPlexAccountResponse","GetMyPlexAccountResponseBody","GetOnDeckGuids","GetOnDeckMedia","GetOnDeckMediaContainer","GetOnDeckMetadata","GetOnDeckPart","GetOnDeckResponse","GetOnDeckResponseBody","GetOnDeckStream","GetPinGlobals","GetPinRequest","GetPinResponse","GetPinResponseBody","GetPlaylistContentsCountry","GetPlaylistContentsDirector","GetPlaylistContentsGenre","GetPlaylistContentsMedia","GetPlaylistContentsMediaContainer","GetPlaylistContentsMetadata","GetPlaylistContentsPart","GetPlaylistContentsRequest","GetPlaylistContentsResponse","GetPlaylistContentsResponseBody","GetPlaylistContentsRole","GetPlaylistContentsWriter","GetPlaylistMediaContainer","GetPlaylistMetadata","GetPlaylistRequest","GetPlaylistResponse","GetPlaylistResponseBody","GetPlaylistsMediaContainer","GetPlaylistsMetadata","GetPlaylistsRequest","GetPlaylistsResponse","GetPlaylistsResponseBody","GetRecentlyAddedMediaContainer","GetRecentlyAddedResponse","GetRecentlyAddedResponseBody","GetResizedPhotoRequest","GetResizedPhotoResponse","GetSearchResultsCountry","GetSearchResultsDirector","GetSearchResultsGenre","GetSearchResultsMedia","GetSearchResultsMediaContainer","GetSearchResultsMetadata","GetSearchResultsPart","GetSearchResultsRequest","GetSearchResultsResponse","GetSearchResultsResponseBody","GetSearchResultsRole","GetSearchResultsWriter","GetServerActivitiesMediaContainer","GetServerActivitiesResponse","GetServerActivitiesResponseBody","GetServerCapabilitiesResponse","GetServerCapabilitiesResponseBody","GetServerIdentityMediaContainer","GetServerIdentityResponse","GetServerIdentityResponseBody","GetServerListMediaContainer","GetServerListResponse","GetServerListResponseBody","GetServerListServer","GetServerPreferencesMediaContainer","GetServerPreferencesResponse","GetServerPreferencesResponseBody","GetSessionHistoryMediaContainer","GetSessionHistoryMetadata","GetSessionHistoryResponse","GetSessionHistoryResponseBody","GetSessionsMedia","GetSessionsMediaContainer","GetSessionsMetadata","GetSessionsPart","GetSessionsResponse","GetSessionsResponseBody","GetSessionsStream","GetSourceConnectionInformationRequest","GetSourceConnectionInformationResponse","GetStatisticsDevice","GetStatisticsMediaContainer","GetStatisticsRequest","GetStatisticsResponse","GetStatisticsResponseBody","GetTimelineRequest","GetTimelineResponse","GetTokenGlobals","GetTokenRequest","GetTokenResponse","GetTranscodeSessionsMediaContainer","GetTranscodeSessionsResponse","GetTranscodeSessionsResponseBody","GetTransientTokenQueryParamType","GetTransientTokenRequest","GetTransientTokenResponse","GetUpdateStatusMediaContainer","GetUpdateStatusResponse","GetUpdateStatusResponseBody","Guids","Hub","IncludeDetails","Level","Location","LogLineRequest","LogLineResponse","LogMultiLineResponse","MarkPlayedRequest","MarkPlayedResponse","MarkUnplayedRequest","MarkUnplayedResponse","Media","MediaContainer","Metadata","MinSize","MyPlex","OnlyTransient","Operator","Part","PathParamTaskName","PerformSearchRequest","PerformSearchResponse","PerformVoiceSearchRequest","PerformVoiceSearchResponse","Player","PlaylistType","Producer","Provider","QueryParamOnlyTransient","QueryParamSmart","QueryParamType","Ratings","RefreshLibraryRequest","RefreshLibraryResponse","Release","Role","Scope","SearchLibraryMediaContainer","SearchLibraryMetadata","SearchLibraryRequest","SearchLibraryResponse","SearchLibraryResponseBody","Server","Session","Setting","Skip","Smart","Sort","StartAllTasksResponse","StartTaskRequest","StartTaskResponse","StartUniversalTranscodeRequest","StartUniversalTranscodeResponse","State","StatisticsMedia","StopAllTasksResponse","StopTaskRequest","StopTaskResponse","StopTranscodeSessionRequest","StopTranscodeSessionResponse","Stream","TaskName","Tonight","TranscodeSession","Type","UpdatePlayProgressRequest","UpdatePlayProgressResponse","UpdatePlaylistRequest","UpdatePlaylistResponse","UploadPlaylistRequest","UploadPlaylistResponse","Upscale","User","Writer"]
+__all__ = ["Account","Activity","AddPlaylistContentsMediaContainer","AddPlaylistContentsMetadata","AddPlaylistContentsRequest","AddPlaylistContentsResponse","AddPlaylistContentsResponseBody","ApplyUpdatesRequest","ApplyUpdatesResponse","ButlerTask","ButlerTasks","CancelServerActivitiesRequest","CancelServerActivitiesResponse","CheckForUpdatesRequest","CheckForUpdatesResponse","ClearPlaylistContentsRequest","ClearPlaylistContentsResponse","Context","Country","CreatePlaylistMediaContainer","CreatePlaylistMetadata","CreatePlaylistRequest","CreatePlaylistResponse","CreatePlaylistResponseBody","DeleteLibraryRequest","DeleteLibraryResponse","DeletePlaylistRequest","DeletePlaylistResponse","Device","Director","Directory","Download","EnablePaperTrailResponse","Field","FieldType","Filter","Force","GET_PIN_SERVERS","GET_TOKEN_SERVERS","Genre","GetAvailableClientsMediaContainer","GetAvailableClientsResponse","GetAvailableClientsResponseBody","GetButlerTasksResponse","GetButlerTasksResponseBody","GetDevicesMediaContainer","GetDevicesResponse","GetDevicesResponseBody","GetFileHashRequest","GetFileHashResponse","GetGlobalHubsMediaContainer","GetGlobalHubsMetadata","GetGlobalHubsRequest","GetGlobalHubsResponse","GetGlobalHubsResponseBody","GetLibrariesDirectory","GetLibrariesLocation","GetLibrariesMediaContainer","GetLibrariesResponse","GetLibrariesResponseBody","GetLibraryDirectory","GetLibraryHubsCountry","GetLibraryHubsDirector","GetLibraryHubsGenre","GetLibraryHubsHub","GetLibraryHubsMedia","GetLibraryHubsMediaContainer","GetLibraryHubsMetadata","GetLibraryHubsPart","GetLibraryHubsRequest","GetLibraryHubsResponse","GetLibraryHubsResponseBody","GetLibraryHubsRole","GetLibraryHubsWriter","GetLibraryItemsCountry","GetLibraryItemsDirector","GetLibraryItemsGenre","GetLibraryItemsMedia","GetLibraryItemsMediaContainer","GetLibraryItemsMetadata","GetLibraryItemsPart","GetLibraryItemsRequest","GetLibraryItemsResponse","GetLibraryItemsResponseBody","GetLibraryItemsRole","GetLibraryItemsWriter","GetLibraryMediaContainer","GetLibraryRequest","GetLibraryResponse","GetLibraryResponseBody","GetLibraryType","GetMetadataChildrenDirectory","GetMetadataChildrenMediaContainer","GetMetadataChildrenMetadata","GetMetadataChildrenRequest","GetMetadataChildrenResponse","GetMetadataChildrenResponseBody","GetMetadataCountry","GetMetadataDirector","GetMetadataGenre","GetMetadataMedia","GetMetadataMediaContainer","GetMetadataMetadata","GetMetadataPart","GetMetadataRequest","GetMetadataResponse","GetMetadataResponseBody","GetMetadataRole","GetMetadataWriter","GetMyPlexAccountResponse","GetMyPlexAccountResponseBody","GetOnDeckGuids","GetOnDeckMedia","GetOnDeckMediaContainer","GetOnDeckMetadata","GetOnDeckPart","GetOnDeckResponse","GetOnDeckResponseBody","GetOnDeckStream","GetPinGlobals","GetPinRequest","GetPinResponse","GetPinResponseBody","GetPlaylistContentsCountry","GetPlaylistContentsDirector","GetPlaylistContentsGenre","GetPlaylistContentsMedia","GetPlaylistContentsMediaContainer","GetPlaylistContentsMetadata","GetPlaylistContentsPart","GetPlaylistContentsRequest","GetPlaylistContentsResponse","GetPlaylistContentsResponseBody","GetPlaylistContentsRole","GetPlaylistContentsWriter","GetPlaylistMediaContainer","GetPlaylistMetadata","GetPlaylistRequest","GetPlaylistResponse","GetPlaylistResponseBody","GetPlaylistsMediaContainer","GetPlaylistsMetadata","GetPlaylistsRequest","GetPlaylistsResponse","GetPlaylistsResponseBody","GetRecentlyAddedMediaContainer","GetRecentlyAddedResponse","GetRecentlyAddedResponseBody","GetResizedPhotoRequest","GetResizedPhotoResponse","GetSearchResultsCountry","GetSearchResultsDirector","GetSearchResultsGenre","GetSearchResultsMedia","GetSearchResultsMediaContainer","GetSearchResultsMetadata","GetSearchResultsPart","GetSearchResultsRequest","GetSearchResultsResponse","GetSearchResultsResponseBody","GetSearchResultsRole","GetSearchResultsWriter","GetServerActivitiesMediaContainer","GetServerActivitiesResponse","GetServerActivitiesResponseBody","GetServerCapabilitiesResponse","GetServerCapabilitiesResponseBody","GetServerIdentityMediaContainer","GetServerIdentityResponse","GetServerIdentityResponseBody","GetServerListMediaContainer","GetServerListResponse","GetServerListResponseBody","GetServerListServer","GetServerPreferencesMediaContainer","GetServerPreferencesResponse","GetServerPreferencesResponseBody","GetSessionHistoryMediaContainer","GetSessionHistoryMetadata","GetSessionHistoryResponse","GetSessionHistoryResponseBody","GetSessionsMedia","GetSessionsMediaContainer","GetSessionsMetadata","GetSessionsPart","GetSessionsResponse","GetSessionsResponseBody","GetSessionsStream","GetSourceConnectionInformationRequest","GetSourceConnectionInformationResponse","GetStatisticsDevice","GetStatisticsMediaContainer","GetStatisticsRequest","GetStatisticsResponse","GetStatisticsResponseBody","GetTimelineRequest","GetTimelineResponse","GetTokenGlobals","GetTokenRequest","GetTokenResponse","GetTranscodeSessionsMediaContainer","GetTranscodeSessionsResponse","GetTranscodeSessionsResponseBody","GetTransientTokenQueryParamType","GetTransientTokenRequest","GetTransientTokenResponse","GetUpdateStatusMediaContainer","GetUpdateStatusResponse","GetUpdateStatusResponseBody","Guids","Hub","IncludeDetails","Level","Location","LogLineRequest","LogLineResponse","LogMultiLineResponse","MarkPlayedRequest","MarkPlayedResponse","MarkUnplayedRequest","MarkUnplayedResponse","Media","MediaContainer","Metadata","MinSize","MyPlex","OnlyTransient","Operator","Part","PathParamTaskName","PerformSearchRequest","PerformSearchResponse","PerformVoiceSearchRequest","PerformVoiceSearchResponse","Player","PlaylistType","Producer","Provider","QueryParamOnlyTransient","QueryParamSmart","QueryParamType","Ratings","RefreshLibraryRequest","RefreshLibraryResponse","Release","Role","Scope","SearchLibraryMediaContainer","SearchLibraryMetadata","SearchLibraryRequest","SearchLibraryResponse","SearchLibraryResponseBody","Server","Session","Setting","Skip","Smart","Sort","StartAllTasksResponse","StartTaskRequest","StartTaskResponse","StartUniversalTranscodeRequest","StartUniversalTranscodeResponse","State","StatisticsMedia","StopAllTasksResponse","StopTaskRequest","StopTaskResponse","StopTranscodeSessionRequest","StopTranscodeSessionResponse","Stream","Tag","TaskName","Tonight","TranscodeSession","Type","UpdatePlayProgressRequest","UpdatePlayProgressResponse","UpdatePlaylistRequest","UpdatePlaylistResponse","UploadPlaylistRequest","UploadPlaylistResponse","Upscale","User","Writer"]
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/addplaylistcontents.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/applyupdates.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/applyupdates.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 from typing import Optional
 
+
 class Tonight(int, Enum):
     r"""Indicate that you want the update to run during the next Butler execution. Omitting this or setting it to false indicates that the update should install"""
     ZERO = 0
     ONE = 1
 
+
 class Skip(int, Enum):
     r"""Indicate that the latest version should be marked as skipped. The <Release> entry for this version will have the `state` set to `skipped`."""
     ZERO = 0
     ONE = 1
 
 
 @dataclasses.dataclass
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/cancelserveractivities.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/checkforupdates.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/checkforupdates.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 from typing import Optional
 
+
 class Download(int, Enum):
     r"""Indicate that you want to start download any updates found."""
     ZERO = 0
     ONE = 1
 
 
 @dataclasses.dataclass
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/clearplaylistcontents.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/createplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/createplaylist.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import dataclasses
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from plex_api import utils
 from typing import List, Optional
 
+
 class QueryParamType(str, Enum):
     r"""type of playlist to create"""
     AUDIO = 'audio'
     VIDEO = 'video'
     PHOTO = 'photo'
 
+
 class Smart(int, Enum):
     r"""whether the playlist is smart or not"""
     ZERO = 0
     ONE = 1
 
 
 @dataclasses.dataclass
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/deletelibrary.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/deleteplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/enablepapertrail.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getavailableclients.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getbutlertasks.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getdevices.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getfilehash.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getglobalhubs.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getglobalhubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dataclasses
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from plex_api import utils
 from typing import List, Optional
 
+
 class OnlyTransient(int, Enum):
     r"""Only return hubs which are \\"transient\\", meaning those which are prone to changing after media playback or addition (e.g. On Deck, or Recently Added)."""
     ZERO = 0
     ONE = 1
 
 
 @dataclasses.dataclass
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getlibraries.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getlibrary.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getlibrary.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dataclasses
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from plex_api import utils
 from typing import List, Optional
 
+
 class IncludeDetails(int, Enum):
     r"""Whether or not to include details for a section (types, filters, and sorts).
     Only exists for backwards compatibility, media providers other than the server libraries have it on always.
     """
     ZERO = 0
     ONE = 1
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getlibraryhubs.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getlibraryhubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from datetime import date
 from enum import Enum
 from plex_api import utils
 from typing import List, Optional
 
+
 class QueryParamOnlyTransient(int, Enum):
     r"""Only return hubs which are \\"transient\\", meaning those which are prone to changing after media playback or addition (e.g. On Deck, or Recently Added)."""
     ZERO = 0
     ONE = 1
 
 
 @dataclasses.dataclass
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getmetadata.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getmetadatachildren.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getmyplexaccount.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getondeck.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getpin.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getplaylistcontents.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getplaylists.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getplaylists.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import dataclasses
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from plex_api import utils
 from typing import List, Optional
 
+
 class PlaylistType(str, Enum):
     r"""limit to a type of playlist."""
     AUDIO = 'audio'
     VIDEO = 'video'
     PHOTO = 'photo'
 
+
 class QueryParamSmart(int, Enum):
     r"""type of playlists to return (default is all)."""
     ZERO = 0
     ONE = 1
 
 
 @dataclasses.dataclass
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getrecentlyadded.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getresizedphoto.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getresizedphoto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 
+
 class MinSize(int, Enum):
     r"""images are always scaled proportionally. A value of '1' in minSize will make the smaller native dimension the dimension resized against."""
     ZERO = 0
     ONE = 1
 
+
 class Upscale(int, Enum):
     r"""allow images to be resized beyond native dimensions."""
     ZERO = 0
     ONE = 1
 
 
 @dataclasses.dataclass
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getsearchresults.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getserveractivities.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getservercapabilities.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getserveridentity.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getserverlist.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getserverpreferences.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getsessionhistory.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getsessions.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getsourceconnectioninformation.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getstatistics.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/gettimeline.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/gettimeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 
+
 class State(str, Enum):
     r"""The state of the media item"""
     PLAYING = 'playing'
     PAUSED = 'paused'
     STOPPED = 'stopped'
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/gettoken.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/gettranscodesessions.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/gettransienttoken.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/gettransienttoken.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 
+
 class GetTransientTokenQueryParamType(str, Enum):
     r"""`delegation` - This is the only supported `type` parameter."""
     DELEGATION = 'delegation'
 
+
 class Scope(str, Enum):
     r"""`all` - This is the only supported `scope` parameter."""
     ALL = 'all'
 
 
 @dataclasses.dataclass
 class GetTransientTokenRequest:
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/getupdatestatus.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/logline.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/logline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 
+
 class Level(int, Enum):
     r"""An integer log level to write to the PMS log with.
     0: Error  
     1: Warning  
     2: Info  
     3: Debug  
     4: Verbose
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/logmultiline.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/markplayed.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/markunplayed.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/performsearch.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/performvoicesearch.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/refreshlibrary.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/searchlibrary.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/searchlibrary.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dataclasses
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from plex_api import utils
 from typing import List, Optional
 
+
 class Type(int, Enum):
     r"""Plex content type to search for"""
     ONE = 1
     TWO = 2
     THREE = 3
     FOUR = 4
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/startalltasks.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/starttask.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/starttask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 
+
 class TaskName(str, Enum):
     r"""the name of the task to be started."""
     BACKUP_DATABASE = 'BackupDatabase'
     BUILD_GRACENOTE_COLLECTIONS = 'BuildGracenoteCollections'
     CHECK_FOR_UPDATES = 'CheckForUpdates'
     CLEAN_OLD_BUNDLES = 'CleanOldBundles'
     CLEAN_OLD_CACHE_FILES = 'CleanOldCacheFiles'
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/startuniversaltranscode.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/stopalltasks.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/stoptask.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/stoptask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 
+
 class PathParamTaskName(str, Enum):
     r"""The name of the task to be started."""
     BACKUP_DATABASE = 'BackupDatabase'
     BUILD_GRACENOTE_COLLECTIONS = 'BuildGracenoteCollections'
     CHECK_FOR_UPDATES = 'CheckForUpdates'
     CLEAN_OLD_BUNDLES = 'CleanOldBundles'
     CLEAN_OLD_CACHE_FILES = 'CleanOldCacheFiles'
```

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/stoptranscodesession.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/updateplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/updateplayprogress.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/models/operations/uploadplaylist.py` & `plex-api-client-0.8.0/src/plex_api/models/operations/uploadplaylist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from enum import Enum
 
+
 class Force(int, Enum):
     r"""Force overwriting of duplicate playlists.
     By default, a playlist file uploaded with the same path will overwrite the existing playlist. 
     The `force` argument is used to disable overwriting.  
     If the `force` argument is set to 0, a new playlist will be created suffixed with the date and time that the duplicate was uploaded.
     """
     ZERO = 0
```

### Comparing `plex-api-client-0.7.0/src/plex_api/playlists.py` & `plex-api-client-0.8.0/src/plex_api/playlists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/plex.py` & `plex-api-client-0.8.0/src/plex_api/plex.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/sdk.py` & `plex-api-client-0.8.0/src/plex_api/sdk.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/sdkconfiguration.py` & `plex-api-client-0.8.0/src/plex_api/sdkconfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 SERVERS = [
     '{protocol}://{ip}:{port}',
     # The full address of your Plex Server
 ]
 """Contains the list of servers available to the SDK"""
 
+
 class ServerProtocol(str, Enum):
     r"""The protocol to use when connecting to your plex server."""
     HTTP = 'http'
     HTTPS = 'https'
 
 
 @dataclass
@@ -29,17 +30,17 @@
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     server_defaults: List[Dict[str, str]] = field(default_factory=List)
     language: str = 'python'
     openapi_doc_version: str = '0.0.3'
-    sdk_version: str = '0.7.0'
-    gen_version: str = '2.326.3'
-    user_agent: str = 'speakeasy-sdk/python 0.7.0 2.326.3 0.0.3 plex-api-client'
+    sdk_version: str = '0.8.0'
+    gen_version: str = '2.335.5'
+    user_agent: str = 'speakeasy-sdk/python 0.8.0 2.335.5 0.0.3 plex-api-client'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `plex-api-client-0.7.0/src/plex_api/search.py` & `plex-api-client-0.8.0/src/plex_api/search.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/server.py` & `plex-api-client-0.8.0/src/plex_api/server.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/sessions.py` & `plex-api-client-0.8.0/src/plex_api/sessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/statistics.py` & `plex-api-client-0.8.0/src/plex_api/statistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/updater.py` & `plex-api-client-0.8.0/src/plex_api/updater.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/utils/retries.py` & `plex-api-client-0.8.0/src/plex_api/utils/retries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api/utils/utils.py` & `plex-api-client-0.8.0/src/plex_api/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,19 +814,19 @@
             return ",".join(items)
     else:
         return f"{_val_to_string(obj)}"
 
     return ""
 
 
-def unmarshal_json(data, typ, decoder=None):
+def unmarshal_json(data, typ, decoder=None, infer_missing=False):
     unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
-        out = unmarshal.from_dict({"res": json_dict})
+        out = unmarshal.from_dict({"res": json_dict}, infer_missing=infer_missing)
     except AttributeError as attr_err:
         raise AttributeError(
             f"unable to unmarshal {data} as {typ} - {attr_err}"
         ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
```

### Comparing `plex-api-client-0.7.0/src/plex_api/video.py` & `plex-api-client-0.8.0/src/plex_api/video.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.7.0/src/plex_api_client.egg-info/PKG-INFO` & `plex-api-client-0.8.0/src/plex_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
@@ -31,14 +31,15 @@
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -96,14 +97,15 @@
         ### [library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md)
         
         * [get_file_hash](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_file_hash) - Get Hash Value
         * [get_recently_added](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_recently_added) - Get Recently Added
         * [get_libraries](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_libraries) - Get All Libraries
         * [get_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_library) - Get Library Details
         * [delete_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#delete_library) - Delete Library Section
+        * [get_library_items](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_library_items) - Get Library Items
         * [refresh_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#refresh_library) - Refresh Library
         * [search_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#search_library) - Search Library
         * [get_metadata](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata) - Get Items Metadata
         * [get_metadata_children](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata_children) - Get Items Children
         * [get_on_deck](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_on_deck) - Get On Deck
         
         ### [log](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/log/README.md)
@@ -172,14 +174,15 @@
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
         res = None
         try:
             res = s.server.get_server_capabilities()
+        
         except errors.GetServerCapabilitiesResponseBody as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -208,14 +211,15 @@
         
         s = plex_api.PlexAPI(
             server_idx=0,
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -235,14 +239,15 @@
         
         s = plex_api.PlexAPI(
             server_url="{protocol}://{ip}:{port}",
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -253,14 +258,15 @@
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2")
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -298,14 +304,15 @@
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -336,14 +343,15 @@
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             x_plex_client_identifier='Postman',
         )
         
+        
         res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.7.0 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.8.0 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
@@ -71,15 +71,17 @@
 //github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_recently_added) - Get Recently Added * [get_libraries](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_libraries) - Get All Libraries * [get_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_library) - Get Library Details * [delete_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
-README.md#delete_library) - Delete Library Section * [refresh_library](https://
+README.md#delete_library) - Delete Library Section * [get_library_items](https:
+//github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
+README.md#get_library_items) - Get Library Items * [refresh_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#refresh_library) - Refresh Library * [search_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#search_library) - Search Library * [get_metadata](https://github.com/
 LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata) - Get
 Items Metadata * [get_metadata_children](https://github.com/LukeHagar/plexpy/
 blob/master/docs/sdks/library/README.md#get_metadata_children) - Get Items
```

### Comparing `plex-api-client-0.7.0/src/plex_api_client.egg-info/SOURCES.txt` & `plex-api-client-0.8.0/src/plex_api_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 src/plex_api/models/errors/getbutlertasks.py
 src/plex_api/models/errors/getdevices.py
 src/plex_api/models/errors/getfilehash.py
 src/plex_api/models/errors/getglobalhubs.py
 src/plex_api/models/errors/getlibraries.py
 src/plex_api/models/errors/getlibrary.py
 src/plex_api/models/errors/getlibraryhubs.py
+src/plex_api/models/errors/getlibraryitems.py
 src/plex_api/models/errors/getmetadata.py
 src/plex_api/models/errors/getmetadatachildren.py
 src/plex_api/models/errors/getmyplexaccount.py
 src/plex_api/models/errors/getondeck.py
 src/plex_api/models/errors/getpin.py
 src/plex_api/models/errors/getplaylist.py
 src/plex_api/models/errors/getplaylistcontents.py
@@ -73,14 +74,15 @@
 src/plex_api/models/errors/logmultiline.py
 src/plex_api/models/errors/markplayed.py
 src/plex_api/models/errors/markunplayed.py
 src/plex_api/models/errors/performsearch.py
 src/plex_api/models/errors/performvoicesearch.py
 src/plex_api/models/errors/refreshlibrary.py
 src/plex_api/models/errors/sdkerror.py
+src/plex_api/models/errors/searchlibrary.py
 src/plex_api/models/errors/startalltasks.py
 src/plex_api/models/errors/starttask.py
 src/plex_api/models/errors/startuniversaltranscode.py
 src/plex_api/models/errors/stopalltasks.py
 src/plex_api/models/errors/stoptask.py
 src/plex_api/models/errors/stoptranscodesession.py
 src/plex_api/models/errors/updateplaylist.py
@@ -102,14 +104,15 @@
 src/plex_api/models/operations/getbutlertasks.py
 src/plex_api/models/operations/getdevices.py
 src/plex_api/models/operations/getfilehash.py
 src/plex_api/models/operations/getglobalhubs.py
 src/plex_api/models/operations/getlibraries.py
 src/plex_api/models/operations/getlibrary.py
 src/plex_api/models/operations/getlibraryhubs.py
+src/plex_api/models/operations/getlibraryitems.py
 src/plex_api/models/operations/getmetadata.py
 src/plex_api/models/operations/getmetadatachildren.py
 src/plex_api/models/operations/getmyplexaccount.py
 src/plex_api/models/operations/getondeck.py
 src/plex_api/models/operations/getpin.py
 src/plex_api/models/operations/getplaylist.py
 src/plex_api/models/operations/getplaylistcontents.py
```

