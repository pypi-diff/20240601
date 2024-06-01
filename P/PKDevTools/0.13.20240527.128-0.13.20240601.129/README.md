# Comparing `tmp/PKDevTools-0.13.20240527.128.tar.gz` & `tmp/PKDevTools-0.13.20240601.129.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240527.128.tar", last modified: Mon May 27 20:59:35 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240601.129.tar", last modified: Sat Jun  1 08:12:44 2024, max compression
```

## Comparing `PKDevTools-0.13.20240527.128.tar` & `PKDevTools-0.13.20240601.129.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 20:59:35.330645 PKDevTools-0.13.20240527.128/
--rw-rw-rw-   0        0        0     1086 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-27 20:59:35.315019 PKDevTools-0.13.20240527.128/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:59:35.330645 PKDevTools-0.13.20240527.128/PKDevTools/classes/
--rw-rw-rw-   0        0        0     4960 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6376 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2608 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/FunctionTimeouts.py
--rw-rw-rw-   0        0        0    11963 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     5261 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/NSEMarketStatus.py
--rw-rw-rw-   0        0        0     2860 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    16509 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5243 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    12875 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-27 20:59:30.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:59:35.315019 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1199 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-27 20:59:29.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      189 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-27 20:59:35.330645 PKDevTools-0.13.20240527.128/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/README.md
--rw-rw-rw-   0        0        0       86 2024-05-27 20:59:35.330645 PKDevTools-0.13.20240527.128/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:12:44.803027 PKDevTools-0.13.20240601.129/
+-rw-rw-rw-   0        0        0     1086 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/LICENSE
+drwxrwxrwx   0        0        0        0 2024-06-01 08:12:44.787402 PKDevTools-0.13.20240601.129/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:12:44.803027 PKDevTools-0.13.20240601.129/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     4960 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2608 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/FunctionTimeouts.py
+-rw-rw-rw-   0        0        0    11963 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     5261 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/NSEMarketStatus.py
+-rw-rw-rw-   0        0        0     2860 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    16509 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5243 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    12875 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11306 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-06-01 08:12:39.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:12:44.787402 PKDevTools-0.13.20240601.129/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-06-01 08:12:44.000000 PKDevTools-0.13.20240601.129/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1199 2024-06-01 08:12:44.000000 PKDevTools-0.13.20240601.129/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 08:12:44.000000 PKDevTools-0.13.20240601.129/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-06-01 08:12:44.000000 PKDevTools-0.13.20240601.129/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-06-01 08:12:38.000000 PKDevTools-0.13.20240601.129/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      201 2024-06-01 08:12:44.000000 PKDevTools-0.13.20240601.129/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 08:12:44.000000 PKDevTools-0.13.20240601.129/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-06-01 08:12:44.803027 PKDevTools-0.13.20240601.129/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/README.md
+-rw-rw-rw-   0        0        0       86 2024-06-01 08:12:44.803027 PKDevTools-0.13.20240601.129/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-06-01 08:11:40.000000 PKDevTools-0.13.20240601.129/setup.py
```

### Comparing `PKDevTools-0.13.20240527.128/LICENSE` & `PKDevTools-0.13.20240601.129/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/__init__.py` & `PKDevTools-0.13.20240601.129/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/FunctionTimeouts.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/FunctionTimeouts.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/NSEMarketStatus.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/NSEMarketStatus.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/Telegram.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Get from telegram
 # See tutorial https://www.siteguarding.com/en/how-to-get-telegram-bot-api-token
 
 import requests
 from dotenv import dotenv_values
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.OutputControls import OutputControls
-from telegram.constants import ParseMode
+from telegram.constants import PARSEMODE_HTML
 
 # from io import BytesIO
 # from PIL import Image
 
 
 # URL_TELE = f"https://api.telegram.org/bot{TOKEN}/getUpdates"
 # **DOCU**
@@ -108,18 +108,18 @@
 
 def send_exception(ex, extra_mes=""):
     extra_mes + "   ** Exception **" + str(ex)
     if not is_token_telegram_configured():
         return
 
 
-def send_message(message, userID=None, parse_type=ParseMode.HTML, list_png=None, retrial=False):
+def send_message(message, userID=None, parse_type=PARSEMODE_HTML, list_png=None, retrial=False):
     initTelegram()
-    # botsUrl = f"https://api.telegram.org/bot{TOKEN}"  # + "/sendMessage?chat_id={}&text={}".format(chat_idLUISL, message_aler, parse_mode=ParseMode.HTML)
-    # url = botsUrl + "/sendMessage?chat_id={}&text={}&parse_mode={parse_mode}".format(chat_idLUISL, message_aler,parse_mode=ParseMode.MARKDOWN_V2)
+    # botsUrl = f"https://api.telegram.org/bot{TOKEN}"  # + "/sendMessage?chat_id={}&text={}".format(chat_idLUISL, message_aler, parse_mode=PARSEMODE_HTML)
+    # url = botsUrl + "/sendMessage?chat_id={}&text={}&parse_mode={parse_mode}".format(chat_idLUISL, message_aler,parse_mode=PARSEMODE_MARKDOWN_V2)
     if not is_token_telegram_configured():
         return
     global chat_idADMIN, botsUrl, Channel_Id, LIST_PEOPLE_IDS_CHAT, TOKEN
     if userID is not None and userID !="":
         LIST_PEOPLE_IDS_CHAT = [int(str(userID).replace("\"",""))]
     if list_png is None or any(elem is None for elem in list_png):
         resp = None
@@ -159,22 +159,22 @@
     method = "/sendPhoto"
     global chat_idADMIN, botsUrl, Channel_Id, LIST_PEOPLE_IDS_CHAT, TOKEN
     photo = open(photoFilePath, "rb")
     if message_id is not None:
         params = {
             "chat_id": (userID if userID is not None else Channel_Id),
             "caption": message,
-            "parse_mode": ParseMode.HTML,
+            "parse_mode": PARSEMODE_HTML,
             "reply_to_message_id": message_id,
         }
     else:
         params = {
             "chat_id": (userID if userID is not None else Channel_Id),
             "caption": message,
-            "parse_mode": ParseMode.HTML,
+            "parse_mode": PARSEMODE_HTML,
         }
     files = {"photo": photo}
     resp = None
     try:
         resp = requests.post(
             botsUrl + method,
             params,
@@ -198,22 +198,22 @@
         return
     document = open(documentFilePath, "rb")
     global chat_idADMIN, botsUrl, Channel_Id, LIST_PEOPLE_IDS_CHAT, TOKEN
     if message_id is not None:
         params = {
             "chat_id": (userID if userID is not None else Channel_Id),
             "caption": message,
-            "parse_mode": ParseMode.HTML,
+            "parse_mode": PARSEMODE_HTML,
             "reply_to_message_id": message_id,
         }
     else:
         params = {
             "chat_id": (userID if userID is not None else Channel_Id),
             "caption": message,
-            "parse_mode": ParseMode.HTML,
+            "parse_mode": PARSEMODE_HTML,
         }
     files = {"document": document}
     method = "/sendDocument"
     resp = None
     try:
         resp = requests.post(
             botsUrl + method,
@@ -258,13 +258,13 @@
 #                 img.save(output, format='PNG')
 #                 output.seek(0)
 #                 name = f'photo{i}'
 #                 files[name] = output.read()
 #                 # a list of InputMediaPhoto. attach refers to the name of the file in the files dict
 #                 media.append(dict(type='photo', media=f'attach://{name}'))
 #         media[0]['caption'] = caption
-#         media[0]['parse_mode'] = ParseMode.HTML
+#         media[0]['parse_mode'] = PARSEMODE_HTML
 #         return requests.post(SEND_MEDIA_GROUP, data={'chat_id': chat_id, 'media': json.dumps(media),
 #                                                     'reply_to_message_id': reply_to_message_id }, files=files )
 
 initTelegram()
 is_token_telegram_configured()
```

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240601.129/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240601.129/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240527.128
+Version: 0.13.20240601.129
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240527.128.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240601.129.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240527.128/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240601.129/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/PKG-INFO` & `PKDevTools-0.13.20240601.129/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240527.128
+Version: 0.13.20240601.129
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240527.128.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240601.129.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240527.128/README.md` & `PKDevTools-0.13.20240601.129/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240527.128/setup.py` & `PKDevTools-0.13.20240601.129/setup.py`

 * *Files identical despite different names*

