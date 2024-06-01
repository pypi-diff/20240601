# Comparing `tmp/PyAibote-1.5.1.tar.gz` & `tmp/PyAibote-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAibote-1.5.1.tar", last modified: Sat May 25 08:59:31 2024, max compression
+gzip compressed data, was "PyAibote-1.5.2.tar", last modified: Sat Jun  1 02:28:17 2024, max compression
```

## Comparing `PyAibote-1.5.1.tar` & `PyAibote-1.5.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 08:59:31.121026 PyAibote-1.5.1/
--rw-rw-rw-   0        0        0     1089 2024-05-25 08:59:31.120026 PyAibote-1.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-25 08:59:30.634883 PyAibote-1.5.1/PyAibote/
--rw-rw-rw-   0        0        0     2679 2024-05-25 01:54:49.000000 PyAibote-1.5.1/PyAibote/AndroidBot.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:59:30.789136 PyAibote-1.5.1/PyAibote/AndroidBotModel/
--rw-rw-rw-   0        0        0     7584 2024-04-22 14:02:06.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
--rw-rw-rw-   0        0        0     2381 2024-04-22 13:58:45.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/AndroidLoadWait.py
--rw-rw-rw-   0        0        0     2924 2024-04-22 14:05:12.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/ColorFindingOperation.py
--rw-rw-rw-   0        0        0     6178 2024-05-14 09:14:47.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/Control.py
--rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/CoordinateOperation.py
--rw-rw-rw-   0        0        0    12733 2024-04-22 14:05:28.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0    17545 2024-04-22 14:05:53.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/EquipmentOperation.py
--rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/FileTransfer.py
--rw-rw-rw-   0        0        0     8092 2024-04-22 14:06:01.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/MapFindingOperation.py
--rw-rw-rw-   0        0        0     9064 2024-04-22 14:06:06.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/OcrCorrelation.py
--rw-rw-rw-   0        0        0      949 2024-04-22 14:06:12.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
--rw-rw-rw-   0        0        0     9217 2024-04-22 14:06:16.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/ScreenshotOperation.py
--rw-rw-rw-   0        0        0     1926 2024-04-22 14:06:20.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/UrlRequest.py
--rw-rw-rw-   0        0        0     4218 2024-04-22 14:06:28.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     1781 2024-04-22 14:06:33.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/YoloService.py
--rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.5.1/PyAibote/AndroidBotModel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:59:30.795097 PyAibote-1.5.1/PyAibote/CommonUse/
--rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.5.1/PyAibote/CommonUse/ChatGenerative.py
--rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.5.1/PyAibote/CommonUse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:59:30.874000 PyAibote-1.5.1/PyAibote/Tool/
--rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.5.1/PyAibote/Tool/DatabaseFunc.py
--rw-rw-rw-   0        0        0     2188 2024-04-30 01:29:58.000000 PyAibote-1.5.1/PyAibote/Tool/DebugStartDriver.py
--rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.5.1/PyAibote/Tool/Logger.py
--rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.5.1/PyAibote/Tool/LoggerFunc.py
--rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.5.1/PyAibote/Tool/SendTcpData.py
--rw-rw-rw-   0        0        0     1090 2024-05-25 02:00:00.000000 PyAibote-1.5.1/PyAibote/Tool/SocketServer.py
--rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.5.1/PyAibote/Tool/Sqlite3DataBase.py
--rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.5.1/PyAibote/Tool/UniversalFunction.py
--rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.5.1/PyAibote/Tool/WriteReadFileFunc.py
--rw-rw-rw-   0        0        0      550 2024-05-25 01:55:35.000000 PyAibote-1.5.1/PyAibote/Tool/__init__.py
--rw-rw-rw-   0        0        0     2024 2024-05-18 03:36:32.000000 PyAibote-1.5.1/PyAibote/WebBot.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:59:30.990025 PyAibote-1.5.1/PyAibote/WebBotModel/
--rw-rw-rw-   0        0        0     3465 2024-04-22 14:07:39.000000 PyAibote-1.5.1/PyAibote/WebBotModel/CookiesOperation.py
--rw-rw-rw-   0        0        0     1356 2024-05-11 08:59:42.000000 PyAibote-1.5.1/PyAibote/WebBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    11034 2024-04-22 14:07:57.000000 PyAibote-1.5.1/PyAibote/WebBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.5.1/PyAibote/WebBotModel/IframeOperation.py
--rw-rw-rw-   0        0        0      804 2024-04-22 14:08:02.000000 PyAibote-1.5.1/PyAibote/WebBotModel/JSinjection.py
--rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.5.1/PyAibote/WebBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     3649 2024-04-22 14:08:09.000000 PyAibote-1.5.1/PyAibote/WebBotModel/PagesAndNavigation.py
--rw-rw-rw-   0        0        0     1005 2024-04-22 14:02:29.000000 PyAibote-1.5.1/PyAibote/WebBotModel/PopUpWindow.py
--rw-rw-rw-   0        0        0     3421 2024-04-22 07:22:21.000000 PyAibote-1.5.1/PyAibote/WebBotModel/WebLoadWait.py
--rw-rw-rw-   0        0        0     5548 2024-04-24 07:42:11.000000 PyAibote-1.5.1/PyAibote/WebBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0      718 2024-05-18 03:36:16.000000 PyAibote-1.5.1/PyAibote/WebBotModel/__init__.py
--rw-rw-rw-   0        0        0     4186 2024-05-25 01:54:28.000000 PyAibote-1.5.1/PyAibote/WindowsBot.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:59:31.116043 PyAibote-1.5.1/PyAibote/WindowsBotModel/
--rw-rw-rw-   0        0        0    19762 2024-04-22 14:08:25.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/ColorOperation.py
--rw-rw-rw-   0        0        0    23558 2024-05-14 08:46:42.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/DigitalHumanOperation.py
--rw-rw-rw-   0        0        0     2221 2024-05-11 08:52:11.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    13246 2024-04-22 14:08:33.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0     4863 2024-04-22 14:03:06.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/ExcelOperation.py
--rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     8223 2024-04-22 14:03:16.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/OcrOperation.py
--rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/OtherOperations.py
--rw-rw-rw-   0        0        0     2293 2024-04-22 14:03:22.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/SystemOperation.py
--rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     6058 2024-04-22 14:03:35.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/VoiceService.py
--rw-rw-rw-   0        0        0     7427 2024-04-22 14:03:52.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/WinHidCorrelation.py
--rw-rw-rw-   0        0        0     2412 2024-04-22 07:22:40.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/WinLoadWait.py
--rw-rw-rw-   0        0        0     8331 2024-04-22 14:08:39.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0     2764 2024-04-22 14:03:57.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/YoloOperation.py
--rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.5.1/PyAibote/WindowsBotModel/__init__.py
--rw-rw-rw-   0        0        0      277 2024-05-25 08:58:53.000000 PyAibote-1.5.1/PyAibote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:59:30.661886 PyAibote-1.5.1/PyAibote.egg-info/
--rw-rw-rw-   0        0        0     1089 2024-05-25 08:59:30.000000 PyAibote-1.5.1/PyAibote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2024-05-25 08:59:30.000000 PyAibote-1.5.1/PyAibote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 08:59:30.000000 PyAibote-1.5.1/PyAibote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-25 08:59:30.000000 PyAibote-1.5.1/PyAibote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 08:59:30.000000 PyAibote-1.5.1/PyAibote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10966 2024-05-11 08:33:55.000000 PyAibote-1.5.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 08:59:31.122022 PyAibote-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1425 2024-05-25 08:59:13.000000 PyAibote-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:28:17.747203 PyAibote-1.5.2/
+-rw-rw-rw-   0        0        0     1089 2024-06-01 02:28:17.700207 PyAibote-1.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 02:28:16.935808 PyAibote-1.5.2/PyAibote/
+-rw-rw-rw-   0        0        0     2679 2024-05-25 01:54:49.000000 PyAibote-1.5.2/PyAibote/AndroidBot.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:28:17.319203 PyAibote-1.5.2/PyAibote/AndroidBotModel/
+-rw-rw-rw-   0        0        0     7584 2024-04-22 14:02:06.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
+-rw-rw-rw-   0        0        0     2415 2024-06-01 02:23:34.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/AndroidLoadWait.py
+-rw-rw-rw-   0        0        0     2924 2024-04-22 14:05:12.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/ColorFindingOperation.py
+-rw-rw-rw-   0        0        0     6178 2024-05-14 09:14:47.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/Control.py
+-rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/CoordinateOperation.py
+-rw-rw-rw-   0        0        0    12733 2024-04-22 14:05:28.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0    17545 2024-04-22 14:05:53.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/EquipmentOperation.py
+-rw-rw-rw-   0        0        0     3128 2024-06-01 02:24:45.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/FileTransfer.py
+-rw-rw-rw-   0        0        0     8092 2024-04-22 14:06:01.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/MapFindingOperation.py
+-rw-rw-rw-   0        0        0     9064 2024-04-22 14:06:06.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/OcrCorrelation.py
+-rw-rw-rw-   0        0        0      949 2024-04-22 14:06:12.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
+-rw-rw-rw-   0        0        0     9251 2024-06-01 02:24:51.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/ScreenshotOperation.py
+-rw-rw-rw-   0        0        0     1926 2024-04-22 14:06:20.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/UrlRequest.py
+-rw-rw-rw-   0        0        0     4218 2024-04-22 14:06:28.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     1781 2024-04-22 14:06:33.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/YoloService.py
+-rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.5.2/PyAibote/AndroidBotModel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:28:17.342203 PyAibote-1.5.2/PyAibote/CommonUse/
+-rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.5.2/PyAibote/CommonUse/ChatGenerative.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.5.2/PyAibote/CommonUse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:28:17.424208 PyAibote-1.5.2/PyAibote/Tool/
+-rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.5.2/PyAibote/Tool/DatabaseFunc.py
+-rw-rw-rw-   0        0        0     2188 2024-04-30 01:29:58.000000 PyAibote-1.5.2/PyAibote/Tool/DebugStartDriver.py
+-rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.5.2/PyAibote/Tool/Logger.py
+-rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.5.2/PyAibote/Tool/LoggerFunc.py
+-rw-rw-rw-   0        0        0      946 2024-06-01 02:23:52.000000 PyAibote-1.5.2/PyAibote/Tool/SendTcpData.py
+-rw-rw-rw-   0        0        0     1090 2024-05-25 02:00:00.000000 PyAibote-1.5.2/PyAibote/Tool/SocketServer.py
+-rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.5.2/PyAibote/Tool/Sqlite3DataBase.py
+-rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.5.2/PyAibote/Tool/UniversalFunction.py
+-rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.5.2/PyAibote/Tool/WriteReadFileFunc.py
+-rw-rw-rw-   0        0        0      550 2024-05-25 01:55:35.000000 PyAibote-1.5.2/PyAibote/Tool/__init__.py
+-rw-rw-rw-   0        0        0     2024 2024-05-18 03:36:32.000000 PyAibote-1.5.2/PyAibote/WebBot.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:28:17.541206 PyAibote-1.5.2/PyAibote/WebBotModel/
+-rw-rw-rw-   0        0        0     3465 2024-04-22 14:07:39.000000 PyAibote-1.5.2/PyAibote/WebBotModel/CookiesOperation.py
+-rw-rw-rw-   0        0        0     1356 2024-05-11 08:59:42.000000 PyAibote-1.5.2/PyAibote/WebBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    11034 2024-04-22 14:07:57.000000 PyAibote-1.5.2/PyAibote/WebBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.5.2/PyAibote/WebBotModel/IframeOperation.py
+-rw-rw-rw-   0        0        0      804 2024-04-22 14:08:02.000000 PyAibote-1.5.2/PyAibote/WebBotModel/JSinjection.py
+-rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.5.2/PyAibote/WebBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     3649 2024-04-22 14:08:09.000000 PyAibote-1.5.2/PyAibote/WebBotModel/PagesAndNavigation.py
+-rw-rw-rw-   0        0        0     1005 2024-04-22 14:02:29.000000 PyAibote-1.5.2/PyAibote/WebBotModel/PopUpWindow.py
+-rw-rw-rw-   0        0        0     3531 2024-06-01 02:25:20.000000 PyAibote-1.5.2/PyAibote/WebBotModel/WebLoadWait.py
+-rw-rw-rw-   0        0        0     5548 2024-04-24 07:42:11.000000 PyAibote-1.5.2/PyAibote/WebBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0      718 2024-05-18 03:36:16.000000 PyAibote-1.5.2/PyAibote/WebBotModel/__init__.py
+-rw-rw-rw-   0        0        0     4186 2024-05-25 01:54:28.000000 PyAibote-1.5.2/PyAibote/WindowsBot.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:28:17.697205 PyAibote-1.5.2/PyAibote/WindowsBotModel/
+-rw-rw-rw-   0        0        0    19762 2024-04-22 14:08:25.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/ColorOperation.py
+-rw-rw-rw-   0        0        0    23558 2024-05-14 08:46:42.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/DigitalHumanOperation.py
+-rw-rw-rw-   0        0        0     2221 2024-05-11 08:52:11.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    13246 2024-04-22 14:08:33.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0     4863 2024-04-22 14:03:06.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/ExcelOperation.py
+-rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     8223 2024-04-22 14:03:16.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/OcrOperation.py
+-rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/OtherOperations.py
+-rw-rw-rw-   0        0        0     2293 2024-04-22 14:03:22.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/SystemOperation.py
+-rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     6058 2024-04-22 14:03:35.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/VoiceService.py
+-rw-rw-rw-   0        0        0     7427 2024-04-22 14:03:52.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/WinHidCorrelation.py
+-rw-rw-rw-   0        0        0     2490 2024-06-01 02:23:15.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/WinLoadWait.py
+-rw-rw-rw-   0        0        0     8331 2024-04-22 14:08:39.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0     2764 2024-04-22 14:03:57.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/YoloOperation.py
+-rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.5.2/PyAibote/WindowsBotModel/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-05-25 08:58:53.000000 PyAibote-1.5.2/PyAibote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:28:16.988587 PyAibote-1.5.2/PyAibote.egg-info/
+-rw-rw-rw-   0        0        0     1089 2024-06-01 02:28:16.000000 PyAibote-1.5.2/PyAibote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2493 2024-06-01 02:28:16.000000 PyAibote-1.5.2/PyAibote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 02:28:16.000000 PyAibote-1.5.2/PyAibote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-06-01 02:28:16.000000 PyAibote-1.5.2/PyAibote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 02:28:16.000000 PyAibote-1.5.2/PyAibote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10966 2024-05-11 08:33:55.000000 PyAibote-1.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 02:28:17.748206 PyAibote-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2024-06-01 02:27:20.000000 PyAibote-1.5.2/setup.py
```

### Comparing `PyAibote-1.5.1/PKG-INFO` & `PyAibote-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.5.1
+Version: 1.5.2
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.5,<4.0
```

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBot.py` & `PyAibote-1.5.2/PyAibote/AndroidBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/AndroidHidCorrelation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/AndroidHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/AndroidLoadWait.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/AndroidLoadWait.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             self.debug(rf"->>> {data[:100]}......")
         else:
             self.debug(rf"->>> {data}")
 
         self.request.sendall(data)
         response = self.request.recv(87654)
         if response == b"":
+            self.request.close()
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} Client disconnects")
         data_length, data = response.split(b"/", 1)
         while int(data_length) > len(data):
             data += self.request.recv(87654)
             
         response = data.decode('UTF-8')
         if len(response) > 10000:
```

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/ColorFindingOperation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/ColorFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/Control.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/Control.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/CoordinateOperation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/CoordinateOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/ElementOperation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/EquipmentOperation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/EquipmentOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/FileTransfer.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/FileTransfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             argv = str(argv)
             args_text += argv
             args_len += str(len(bytes(argv, 'utf8'))) + "/"
         data = (args_len.strip("/") + "\n" + args_text).encode("utf8")
         self.request.sendall(data)
         response = self.request.recv(65535)
         if response == b"":
+            self.request.close()
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} 客户端断开链接")
         data_length, data = response.split(b"/", 1)
         while int(data_length) > len(data):
             data += self.request.recv(65535)
         return data
 
     def push_file(self, origin_path: str, to_path: str) -> bool:
```

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/MapFindingOperation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/MapFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/OcrCorrelation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/OcrCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/ScreenProjectionOperation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/ScreenProjectionOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/ScreenshotOperation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/ScreenshotOperation.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self.request.sendall(data)
         response = self.request.recv(65535)
         if len(response) > 10000:
             self.debug(rf"<-<- {response[:100]}......")
         else:
             self.debug(rf"<-<- {response}")
         if response == b"":
+            self.request.close()
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} 客户端断开链接")
         data_length, data = response.split(b"/", 1)
         while int(data_length) > len(data):
             data += self.request.recv(65535)
         return data
 
     def save_screenshot(self, image_name: str, region: tuple = (0,0,0,0), algorithm: tuple = (0,0,0)) -> str:
```

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/UrlRequest.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/UrlRequest.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/VerificationCodeOperation.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/YoloService.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/YoloService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/AndroidBotModel/__init__.py` & `PyAibote-1.5.2/PyAibote/AndroidBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/CommonUse/ChatGenerative.py` & `PyAibote-1.5.2/PyAibote/CommonUse/ChatGenerative.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/DatabaseFunc.py` & `PyAibote-1.5.2/PyAibote/Tool/DatabaseFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/DebugStartDriver.py` & `PyAibote-1.5.2/PyAibote/Tool/DebugStartDriver.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/Logger.py` & `PyAibote-1.5.2/PyAibote/Tool/Logger.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/LoggerFunc.py` & `PyAibote-1.5.2/PyAibote/Tool/LoggerFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/SendTcpData.py` & `PyAibote-1.5.2/PyAibote/Tool/SendTcpData.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,9 +21,10 @@
             args_text += argv
             args_len += str(len(bytes(argv, 'utf8'))) + "/"
         data = (args_len.strip("/") + "\n" + args_text).encode("utf8")
         try:
             response = self.StarLoadWait(data)
             return response
         except Exception as e:
+            self.request.close()
             self.error("send/read tcp data error: " + str(traceback.format_exc()))
             raise e
```

### Comparing `PyAibote-1.5.1/PyAibote/Tool/SocketServer.py` & `PyAibote-1.5.2/PyAibote/Tool/SocketServer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/Sqlite3DataBase.py` & `PyAibote-1.5.2/PyAibote/Tool/Sqlite3DataBase.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/UniversalFunction.py` & `PyAibote-1.5.2/PyAibote/Tool/UniversalFunction.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/WriteReadFileFunc.py` & `PyAibote-1.5.2/PyAibote/Tool/WriteReadFileFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/Tool/__init__.py` & `PyAibote-1.5.2/PyAibote/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBot.py` & `PyAibote-1.5.2/PyAibote/WebBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/CookiesOperation.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/CookiesOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/DrivingOperation.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/ElementOperation.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/IframeOperation.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/IframeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/JSinjection.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/JSinjection.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/KeymouseOperation.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/PagesAndNavigation.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/PagesAndNavigation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/PopUpWindow.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/PopUpWindow.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/WebLoadWait.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/WebLoadWait.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 
     def _Send(self,data):
         self.debug(rf"->>> {data}")
 
         self.request.sendall(data)
         response = self.request.recv(87654)
         if response == b"":
+            self.request.close()
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} Client disconnects")
         data_length, data = response.split(b"/", 1)
         while int(data_length) > len(data):
             data += self.request.recv(87654)
 
         response = data.decode('UTF-8')
         if len(response) > 10000:
             self.debug(rf"<-<- {response[:100]}......")
         else:
             self.debug(rf"<-<- {response}")
         if response == b"":
+            self.request.close()
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} Client disconnects")
         return response
 
     def StarLoadWait(self, data):
         response = self._Send(data)
         start_time = time.time()
         if 'false' in response or 'webdriver error' in response:
@@ -48,14 +50,15 @@
                     if "domain" in response or "path" in response or "secure" in response or "httpOnly" in response:
                         break
                     time.sleep(self.Implicit_Waiting_Frequency)
                 except Exception as e:
                     time.sleep(self.Implicit_Waiting_Frequency)
             if self.Implicit_Waiting_Throwing:
                 if 'false' in response or 'webdriver error' in response:
+                    self.request.close()
                     raise "Unable to find the specified element"
         return response
 
     def StartShowWait(self, Time: int, RotationTime: int, ThrowException: bool):
         """
             进行隐式等待和显示等待模式的切换
             Switch between implicit waiting and display waiting modes.
```

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/WindowOperation.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WebBotModel/__init__.py` & `PyAibote-1.5.2/PyAibote/WebBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBot.py` & `PyAibote-1.5.2/PyAibote/WindowsBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/ColorOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/ColorOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/DigitalHumanOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/DigitalHumanOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/DrivingOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/ElementOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/ExcelOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/ExcelOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/KeymouseOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/OcrOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/OcrOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/OtherOperations.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/OtherOperations.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/SystemOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/SystemOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/VerificationCodeOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/VoiceService.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/VoiceService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/WinHidCorrelation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/WinHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/WinLoadWait.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/WinLoadWait.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,26 +16,29 @@
     Show_Waiting_Throwing = False
 
     def _Send(self,data):
         self.debug(rf"->>> {data}")
 
         self.request.sendall(data)
         response = self.request.recv(87654)
+        
         if response == b"":
+            self.request.close()
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} Client disconnects")
         data_length, data = response.split(b"/", 1)
         while int(data_length) > len(data):
             data += self.request.recv(87654)
 
         response = data.decode('UTF-8')
         if len(response) > 10000:
             self.debug(rf"<-<- {response[:100]}......")
         else:
             self.debug(rf"<-<- {response}")
         if response == b"":
+            self.request.close()
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} Client disconnects")
         
         return response
 
     def StarLoadWait(self, data):
         response = self._Send(data)
         return response
```

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/WindowOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/YoloOperation.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/YoloOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote/WindowsBotModel/__init__.py` & `PyAibote-1.5.2/PyAibote/WindowsBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/PyAibote.egg-info/PKG-INFO` & `PyAibote-1.5.2/PyAibote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.5.1
+Version: 1.5.2
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.5,<4.0
```

### Comparing `PyAibote-1.5.1/PyAibote.egg-info/SOURCES.txt` & `PyAibote-1.5.2/PyAibote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/README.md` & `PyAibote-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `PyAibote-1.5.1/setup.py` & `PyAibote-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Pillow",
     "requests",
     "pymysql"
 ]
 
 setup(
     name="PyAibote", 
-    version="1.5.1", 
+    version="1.5.2", 
     author="Riven", 
     author_email="pyaibote@163.com", 
     description="A pure code RPA office automation framework, which supports Android, Browser and Windows", 
     long_description="Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium", # 加载read_me的内容
     long_description_content_type="text/markdown", 
     url="https://www.pyaibote.com",  
     packages=packages,
```

