# Comparing `tmp/kwldn_bot-1.3.1.tar.gz` & `tmp/kwldn_bot-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwldn_bot-1.3.1.tar", last modified: Tue May 21 13:48:11 2024, max compression
+gzip compressed data, was "kwldn_bot-1.3.5.tar", last modified: Sat Jun  1 13:09:13 2024, max compression
```

## Comparing `kwldn_bot-1.3.1.tar` & `kwldn_bot-1.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:48:11.978912 kwldn_bot-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-21 13:48:11.978912 kwldn_bot-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:48:11.978912 kwldn_bot-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:48:11.974912 kwldn_bot-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:48:11.974912 kwldn_bot-1.3.1/src/kwldn_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:48:11.974912 kwldn_bot-1.3.1/src/kwldn_bot/database/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/database/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:48:11.978912 kwldn_bot-1.3.1/src/kwldn_bot/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/modules/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/modules/state_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-21 13:48:07.000000 kwldn_bot-1.3.1/src/kwldn_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:48:11.978912 kwldn_bot-1.3.1/src/kwldn_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-21 13:48:11.000000 kwldn_bot-1.3.1/src/kwldn_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-21 13:48:11.000000 kwldn_bot-1.3.1/src/kwldn_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:48:11.000000 kwldn_bot-1.3.1/src/kwldn_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:48:11.000000 kwldn_bot-1.3.1/src/kwldn_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 13:48:11.000000 kwldn_bot-1.3.1/src/kwldn_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:09:13.327135 kwldn_bot-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-06-01 13:09:13.327135 kwldn_bot-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:09:13.327135 kwldn_bot-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:09:13.323135 kwldn_bot-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:09:13.323135 kwldn_bot-1.3.5/src/kwldn_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:09:13.323135 kwldn_bot-1.3.5/src/kwldn_bot/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/database/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:09:13.323135 kwldn_bot-1.3.5/src/kwldn_bot/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/modules/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/modules/state_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-06-01 13:09:08.000000 kwldn_bot-1.3.5/src/kwldn_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:09:13.327135 kwldn_bot-1.3.5/src/kwldn_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-06-01 13:09:13.000000 kwldn_bot-1.3.5/src/kwldn_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-01 13:09:13.000000 kwldn_bot-1.3.5/src/kwldn_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:09:13.000000 kwldn_bot-1.3.5/src/kwldn_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 13:09:13.000000 kwldn_bot-1.3.5/src/kwldn_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 13:09:13.000000 kwldn_bot-1.3.5/src/kwldn_bot.egg-info/top_level.txt
```

### Comparing `kwldn_bot-1.3.1/pyproject.toml` & `kwldn_bot-1.3.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kwldn_bot"
-version = "1.3.1"
+version = "1.3.5"
 description = "Universal aiogram bot library"
 readme = "README.md"
 authors = [{ name = "kewldan", email = "kewldanil1@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["bot", "telegram"]
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 dependencies = [
-    "aiogram", "aiohttp", "pydantic", "motor", "beanie"
+    "aiogram~=3.7.0", "aiohttp~=3.9.5", "pydantic~=2.7.2", "motor~=3.4.0", "beanie~=1.26.0"
 ]
 
 [project.urls]
 Homepage = "https://github.com/kewldan/xbot"
```

### Comparing `kwldn_bot-1.3.1/src/kwldn_bot/bot.py` & `kwldn_bot-1.3.5/src/kwldn_bot/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import random
 import string
 
 from aiogram import Dispatcher, Router, Bot
+from aiogram.client.default import DefaultBotProperties
 from aiogram.client.session.aiohttp import AiohttpSession
 from aiogram.enums import ParseMode
 from aiogram.exceptions import TelegramUnauthorizedError
 from aiogram.types import User
 from aiogram.webhook.aiohttp_server import SimpleRequestHandler, setup_application, TokenBasedRequestHandler
 from aiohttp import web
 
@@ -15,15 +16,18 @@
     def __init__(self, token: str):
         self.token = token
 
         self.router = Router()
         self.dispatcher = Dispatcher()
         self.dispatcher.include_router(self.router)
 
-        self._bot_settings = {"session": AiohttpSession(), "parse_mode": ParseMode.HTML}
+        self._bot_settings = {
+            'session': AiohttpSession(),
+            'default': DefaultBotProperties(parse_mode=ParseMode.HTML)
+        }
         self.main_bot = Bot(self.token, **self._bot_settings)
 
     async def start(self) -> None:
         pass
 
 
 class XBot(BaseBot):
```

### Comparing `kwldn_bot-1.3.1/src/kwldn_bot/config.py` & `kwldn_bot-1.3.5/src/kwldn_bot/config.py`

 * *Files identical despite different names*

### Comparing `kwldn_bot-1.3.1/src/kwldn_bot/modules/error_handler.py` & `kwldn_bot-1.3.5/src/kwldn_bot/modules/error_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,22 +43,22 @@
             pass
 
 
 def add_to_router(main_router: Router, main_bot: Bot, owners: list[int], url: str):
     error_handler_router = Router()
 
     @error_handler_router.error(F.update.message.as_("message"))
-    async def error_handler(exception: ErrorEvent, message: Message):
+    async def error_handler(_exception: ErrorEvent, message: Message):
         await message.reply('❌ Похоже, что-то пошло не так, репорт отправлен', reply_markup=get_support_markup(url))
 
         await report(main_bot, owners, 'сообщения', message.text, message.from_user.username,
                      message.from_user.id,
                      message.from_user.url)
 
     @error_handler_router.error(F.update.callback_query.as_("query"))
-    async def error_handler(exception: ErrorEvent, query: CallbackQuery):
+    async def error_handler(_exception: ErrorEvent, query: CallbackQuery):
         await query.answer('❌ Похоже, что-то пошло не так, репорт отправлен', show_alert=True)
 
         await report(main_bot, owners, 'кнопки', query.data, query.from_user.username, query.from_user.id,
                      query.from_user.url)
 
     main_router.include_router(error_handler_router)
```

### Comparing `kwldn_bot-1.3.1/src/kwldn_bot/modules/state_clear.py` & `kwldn_bot-1.3.5/src/kwldn_bot/modules/state_clear.py`

 * *Files identical despite different names*

### Comparing `kwldn_bot-1.3.1/src/kwldn_bot/utils.py` & `kwldn_bot-1.3.5/src/kwldn_bot/utils.py`

 * *Files identical despite different names*

