# Comparing `tmp/aiogram_cli-1.0.3.tar.gz` & `tmp/aiogram_cli-1.1.0.tar.gz`

## Comparing `aiogram_cli-1.0.3.tar` & `aiogram_cli-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/.coveragerc
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/Makefile
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/.github/workflows/pypi-release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/__main__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/main.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/resolver.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/version.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/wraps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/develop/__init__.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/develop/_dispatcher.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/develop/_polling.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/develop/_resolver.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/develop/_webhook.py
--rw-r--r--   0        0        0     8411 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/aiogram_cli/develop/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/README.md
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 aiogram_cli-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/.coveragerc
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/Makefile
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/__main__.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/main.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/resolver.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/wraps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/develop/__init__.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/develop/_bot.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/develop/_dispatcher.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/develop/_polling.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/develop/_resolver.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/develop/_server_address.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/develop/_webhook.py
+-rw-r--r--   0        0        0    10910 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/aiogram_cli/develop/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/README.md
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 aiogram_cli-1.1.0/PKG-INFO
```

### Comparing `aiogram_cli-1.0.3/Makefile` & `aiogram_cli-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `aiogram_cli-1.0.3/.github/workflows/pypi-release.yml` & `aiogram_cli-1.1.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `aiogram_cli-1.0.3/aiogram_cli/main.py` & `aiogram_cli-1.1.0/aiogram_cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 
 from aiogram_cli import __version__
 from aiogram_cli.resolver import iter_entry_points
 
 
 @with_plugins(iter_entry_points("aiogram_cli.plugins"))
 @click.group(
-    context_settings={"help_option_names": ["-h", "--help"]},
+    context_settings={
+        "help_option_names": ["-h", "--help"],
+        "show_default": True,
+    },
 )
 @click.version_option(version=__version__, prog_name="aiogram-cli", message="%(version)s")
 def cli():
     pass
 
 
 @cli.command("version")
```

### Comparing `aiogram_cli-1.0.3/aiogram_cli/develop/_dispatcher.py` & `aiogram_cli-1.1.0/aiogram_cli/develop/_dispatcher.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,29 +26,15 @@
     if not isinstance(dispatcher, Dispatcher):
         msg = f"Dispatcher must be instance of aiogram.Dispatcher, got: {type(dispatcher)}"
         raise ValueError(msg)
 
     if skip_updates:
         dispatcher.startup.register(do_skip_updates)
 
-    _add_status_watcher(dispatcher)
-
-    return dispatcher
-
-
-def simplified_prepare_dispatcher(*, dispatcher: Any, skip_updates: bool) -> Dispatcher:
-    if callable(dispatcher):
-        dispatcher = dispatcher()
-
-    if not isinstance(dispatcher, Dispatcher):
-        msg = f"Dispatcher must be instance of aiogram.Dispatcher, got: {type(dispatcher)}"
-        raise ValueError(msg)
-
-    if skip_updates:
-        dispatcher.startup.register(do_skip_updates)
+    dispatcher.startup.register(debug_info)
 
     _add_status_watcher(dispatcher)
 
     return dispatcher
 
 
 def _add_status_watcher(dispatcher: Dispatcher):
@@ -61,7 +47,11 @@
 
 async def startup_completed_callback():
     click.echo("Application started")
 
 
 async def shutdown_completed_callback():
     click.echo("Application stopped")
+
+
+async def debug_info(bot: Bot):
+    logger.debug("Bot defaults: %s", bot.default)
```

### Comparing `aiogram_cli-1.0.3/aiogram_cli/develop/_resolver.py` & `aiogram_cli-1.1.0/aiogram_cli/develop/_resolver.py`

 * *Files identical despite different names*

### Comparing `aiogram_cli-1.0.3/aiogram_cli/develop/_webhook.py` & `aiogram_cli-1.1.0/aiogram_cli/develop/_webhook.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import logging
 import ssl
 import sys
 from logging import basicConfig
 from pathlib import Path
+from typing import Any
 
 import aiogram
 import click
 from aiogram import Bot
-from aiogram.enums import ParseMode
+from aiogram.client.default import DefaultBotProperties
 from aiogram.types import FSInputFile
 from aiogram.webhook.aiohttp_server import SimpleRequestHandler, setup_application
 from aiohttp.web import Application, run_app
 
-from aiogram_cli.develop._dispatcher import resolve_dispatcher, simplified_prepare_dispatcher
+from aiogram_cli.develop._bot import create_bot
+from aiogram_cli.develop._dispatcher import prepare_dispatcher, resolve_dispatcher
 from aiogram_cli.develop._resolver import LoadError
 
 logger = logging.getLogger(__name__)
 
 
 def start_webhook(
     *,
@@ -25,18 +27,17 @@
     port: int,
     path: str,
     webhook_address: str | None,
     webhook_secret: str | None,
     ssl_certificate: Path | None,
     ssl_private_key: Path | None,
     token: str,
-    parse_mode: ParseMode,
-    disable_web_page_preview: bool,
-    protect_content: bool,
+    defaults: DefaultBotProperties,
     skip_updates: bool,
+    api_address: str,
     log_level: str,
     log_format: str,
 ) -> int:
     if log_level:
         basicConfig(level=log_level, format=log_format)
 
     click.echo("=" * 80)
@@ -45,46 +46,67 @@
     click.echo("Loading application...")
     try:
         dispatcher = resolve_dispatcher(target=target)
     except LoadError as e:
         click.echo(str(e), err=True)
         sys.exit(2)
 
-    dispatcher = simplified_prepare_dispatcher(dispatcher=dispatcher, skip_updates=skip_updates)
-    bot = Bot(
-        token=token,
-        parse_mode=parse_mode,
-        disable_web_page_preview=disable_web_page_preview,
-        protect_content=protect_content,
-    )
+    bot = create_bot(token=token, default=defaults, api_address=api_address)
     click.echo("Start webhook")
 
-    app = Application()
-    setup_application(app, dispatcher, bot=bot)
-    SimpleRequestHandler(dispatcher=dispatcher, bot=bot).register(app, path=path)
-
-    async def _setup_webhook():
-        logger.info("Setting up webhook to %s", webhook_address)
-        if ssl_certificate:
-            certificate = FSInputFile(ssl_certificate)
-        else:
-            certificate = None
-        await bot.set_webhook(url=webhook_address, secret_token=webhook_secret, certificate=certificate)
-
-    if webhook_address:
-        dispatcher.startup.register(_setup_webhook)
-
     if ssl_certificate and ssl_private_key:
         context = ssl.SSLContext(ssl.PROTOCOL_TLSv1_2)
         context.load_cert_chain(ssl_certificate, ssl_private_key)
     else:
         context = None
 
     logger.info("Starting web application on %s:%s", host, port)
     run_app(
-        app,
+        _create_app(
+            bot=bot,
+            dispatcher=dispatcher,
+            path=path,
+            webhook_address=webhook_address,
+            webhook_secret=webhook_secret,
+            ssl_certificate=ssl_certificate,
+            skip_updates=skip_updates,
+        ),
         host=host,
         port=port,
         ssl_context=context,
         print=logging.getLogger("aiohttp.server").info,
     )
     return 0
+
+
+async def _create_app(
+    *,
+    bot: Bot,
+    dispatcher: Any,
+    path: str,
+    webhook_address: str | None,
+    webhook_secret: str | None,
+    ssl_certificate: Path | None,
+    skip_updates: bool,
+) -> Application:
+    app = Application()
+    try:
+        dispatcher = await prepare_dispatcher(dispatcher=dispatcher, skip_updates=skip_updates)
+        setup_application(app, dispatcher, bot=bot)
+    except Exception as e:
+        click.echo(f"Application startup failed - {type(e).__name__}: {e}", err=True)
+        raise
+
+    SimpleRequestHandler(dispatcher=dispatcher, bot=bot, secret_token=webhook_secret).register(app, path=path)
+
+    async def _setup_webhook():
+        logger.info("Setting up webhook to %s", webhook_address)
+        if ssl_certificate:
+            certificate = FSInputFile(ssl_certificate)
+        else:
+            certificate = None
+        await bot.set_webhook(url=webhook_address, secret_token=webhook_secret, certificate=certificate)
+
+    if webhook_address:
+        dispatcher.startup.register(_setup_webhook)
+
+    return app
```

### Comparing `aiogram_cli-1.0.3/LICENSE.txt` & `aiogram_cli-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiogram_cli-1.0.3/README.md` & `aiogram_cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aiogram_cli-1.0.3/pyproject.toml` & `aiogram_cli-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Environment :: Plugins",
     "Topic :: Utilities",
 ]
 dependencies = [
     "click~=8.1.7",
     "click-plugins~=1.1.1",
     "colorama~=0.4.6",
-    "aiogram~=3.0",
+    "aiogram>=3.7.0,<4.0.0",
     "watchfiles~=0.20.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/aiogram/cli#readme"
 Issues = "https://github.com/aiogram/cli/issues"
 Source = "https://github.com/aiogram/cli"
@@ -97,27 +97,28 @@
 [tool.black]
 target-version = ["py37"]
 line-length = 120
 
 [tool.ruff]
 target-version = "py37"
 line-length = 120
+
+[tool.ruff.lint]
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
     "E",
     "EM",
     "F",
     "FBT",
     "I",
     "ICN",
-    "ISC",
     "N",
     "PLC",
     "PLE",
     "PLR",
     "PLW",
     "Q",
     "RUF",
@@ -139,21 +140,21 @@
     "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
 unfixable = [
     # Don't touch unused imports
     "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["cli"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source_pkgs = ["cli", "tests"]
 branch = true
 parallel = true
```

### Comparing `aiogram_cli-1.0.3/PKG-INFO` & `aiogram_cli-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aiogram_cli
-Version: 1.0.3
+Version: 1.1.0
 Project-URL: Documentation, https://github.com/aiogram/cli#readme
 Project-URL: Issues, https://github.com/aiogram/cli/issues
 Project-URL: Source, https://github.com/aiogram/cli
 Author-email: Alex Root Junior <jroot.junior@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
-Requires-Dist: aiogram~=3.0
+Requires-Dist: aiogram<4.0.0,>=3.7.0
 Requires-Dist: click-plugins~=1.1.1
 Requires-Dist: click~=8.1.7
 Requires-Dist: colorama~=0.4.6
 Requires-Dist: watchfiles~=0.20.0
 Description-Content-Type: text/markdown
 
 # aiogram-cli (PoC)
```

