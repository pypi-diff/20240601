# Comparing `tmp/llmail-0.2.4.tar.gz` & `tmp/llmail-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmail-0.2.4.tar", max compression
+gzip compressed data, was "llmail-0.2.5.tar", max compression
```

## Comparing `llmail-0.2.4.tar` & `llmail-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0    34516 2024-04-29 23:29:15.749949 llmail-0.2.4/LICENSE
--rw-r--r--   0        0        0        0 2024-04-29 23:31:53.519788 llmail-0.2.4/llmail/__init__.py
--rw-r--r--   0        0        0    24205 2024-05-18 02:12:51.082069 llmail-0.2.4/llmail/__main__.py
--rw-r--r--   0        0        0        0 2024-04-29 23:49:56.280104 llmail-0.2.4/llmail/utils/__init__.py
--rw-r--r--   0        0        0     6044 2024-05-18 01:33:13.218763 llmail-0.2.4/llmail/utils/cli_args.py
--rw-r--r--   0        0        0      935 2024-05-18 01:33:13.219290 llmail-0.2.4/llmail/utils/utils.py
--rw-r--r--   0        0        0      882 2024-05-18 02:08:30.488272 llmail-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2724 2024-05-12 20:12:58.445880 llmail-0.2.4/README.md
--rw-r--r--   0        0        0     3656 1970-01-01 00:00:00.000000 llmail-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    34516 2024-04-29 23:29:15.749949 llmail-0.2.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-06-01 19:23:33.942223 llmail-0.2.5/llmail/__init__.py
+-rw-r--r--   0        0        0     1452 2024-06-01 20:57:20.554441 llmail-0.2.5/llmail/__main__.py
+-rw-r--r--   0        0        0      217 2024-06-01 20:57:20.555485 llmail-0.2.5/llmail/utils/__init__.py
+-rw-r--r--   0        0        0     6101 2024-06-01 20:57:20.556010 llmail-0.2.5/llmail/utils/cli_args.py
+-rw-r--r--   0        0        0     1048 2024-06-01 20:57:20.557149 llmail-0.2.5/llmail/utils/logging.py
+-rw-r--r--   0        0        0    12481 2024-06-01 20:57:20.557687 llmail-0.2.5/llmail/utils/responding.py
+-rw-r--r--   0        0        0     9562 2024-06-01 20:57:20.558204 llmail-0.2.5/llmail/utils/tracking.py
+-rw-r--r--   0        0        0     1888 2024-06-01 20:57:20.558727 llmail-0.2.5/llmail/utils/utils.py
+-rw-r--r--   0        0        0      882 2024-06-01 20:57:23.115944 llmail-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2836 2024-05-26 21:01:53.908004 llmail-0.2.5/README.md
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 llmail-0.2.5/PKG-INFO
```

### Comparing `llmail-0.2.4/LICENSE` & `llmail-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmail-0.2.4/llmail/utils/cli_args.py` & `llmail-0.2.5/llmail/utils/cli_args.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import argparse
 import os
-import dotenv
 import sys
 from pathlib import Path
 
-argparser = None
+import dotenv
 
 """
 For reference, Gmail's IMAP settings are:
 - Hostname: imap.gmail.com
 - Port: 993
 - Username: Your full Gmail address
 - Password: App token (when using 2FA) or perhaps your regular password (if not using 2FA ?)
 """
 
 
 def set_argparse():
-    global argparser
+    global args
 
     if Path(".env").is_file():
         dotenv.load_dotenv()
         print("Loaded .env file")
     else:
         print("No .env file found")
 
@@ -33,17 +32,15 @@
     # Subcommands
     subparsers = argparser.add_subparsers(
         # Dest means that the current subcommand can be accessed via args.subcommand
         dest="subcommand",
         title="Subcommands",
     )
     # Subcommand: list-folders
-    _ = subparsers.add_parser(
-        "list-folders", help="List all folders in the IMAP account and exit"
-    )
+    _ = subparsers.add_parser("list-folders", help="List all folders in the IMAP account and exit")
     # General arguments
     argparser.add_argument(
         "--log-level",
         "-l",
         help="Log level",
         default=os.getenv("LOG_LEVEL") if os.getenv("LOG_LEVEL") else "INFO",
     )
@@ -62,17 +59,15 @@
         ),
     )
     argparser.add_argument(
         "--watch-interval",
         "-w",
         help="Interval in seconds to check for new emails. If not set, will only check once.",
         type=int,
-        default=(
-            int(os.getenv("WATCH_INTERVAL")) if os.getenv("WATCH_INTERVAL") else None
-        ),
+        default=(int(os.getenv("WATCH_INTERVAL")) if os.getenv("WATCH_INTERVAL") else None),
     )
     # OpenAI-compatible API arguments
     ai_api = argparser.add_argument_group("OpenAI-compatible API")
     ai_api.add_argument(
         "--openai-api-key", help="OpenAI API key", default=os.getenv("OPENAI_API_KEY")
     )
     ai_api.add_argument(
@@ -104,63 +99,51 @@
         default=os.getenv("FOLDER").split(",") if os.getenv("FOLDER") else None,
         action="append",
     )
     email.add_argument(
         "--subject-key",
         "-s",
         help="Emails with this subject will be replied to",
-        default=(
-            os.getenv("SUBJECT_KEY") if os.getenv("SUBJECT_KEY") else "llmail autoreply"
-        ),
+        default=(os.getenv("SUBJECT_KEY") if os.getenv("SUBJECT_KEY") else "llmail autoreply"),
     )
     email.add_argument(
         "--alias",
         help="Name to use in the 'From' in addition to the email address",
         default=os.getenv("ALIAS") if os.getenv("ALIAS") else "LLMail",
     )
     imap = email.add_argument_group("IMAP")
-    imap.add_argument(
-        "--imap-host", help="IMAP server hostname", default=os.getenv("IMAP_HOST")
-    )
-    imap.add_argument(
-        "--imap-port", help="IMAP server port", default=os.getenv("IMAP_PORT")
-    )
+    imap.add_argument("--imap-host", help="IMAP server hostname", default=os.getenv("IMAP_HOST"))
+    imap.add_argument("--imap-port", help="IMAP server port", default=os.getenv("IMAP_PORT"))
     imap.add_argument(
         "--imap-username",
         help="IMAP server username",
         default=os.getenv("IMAP_USERNAME"),
     )
     imap.add_argument(
         "--imap-password",
         help="IMAP server password",
         default=os.getenv("IMAP_PASSWORD"),
     )
     smtp = email.add_argument_group("SMTP")
-    smtp.add_argument(
-        "--smtp-host", help="SMTP server hostname", default=os.getenv("SMTP_HOST")
-    )
-    smtp.add_argument(
-        "--smtp-port", help="SMTP server port", default=os.getenv("SMTP_PORT")
-    )
+    smtp.add_argument("--smtp-host", help="SMTP server hostname", default=os.getenv("SMTP_HOST"))
+    smtp.add_argument("--smtp-port", help="SMTP server port", default=os.getenv("SMTP_PORT"))
     smtp.add_argument(
         "--smtp-username",
         help="SMTP server username",
         default=os.getenv("SMTP_USERNAME"),
     )
     smtp.add_argument(
         "--smtp-password",
         help="SMTP server password",
         default=os.getenv("SMTP_PASSWORD"),
     )
     smtp.add_argument(
         "--message-id-domain",
         help="Domain to use for Message-ID header",
-        default=(
-            os.getenv("MESSAGE_ID_DOMAIN") if os.getenv("MESSAGE_ID_DOMAIN") else None
-        ),
+        default=(os.getenv("MESSAGE_ID_DOMAIN") if os.getenv("MESSAGE_ID_DOMAIN") else None),
     )
 
     check_required_args(
         [
             "imap_host",
             "imap_port",
             "imap_username",
@@ -170,14 +153,18 @@
             "smtp_username",
             "smtp_password",
             "openai_api_key",
             "openai_base_url",
         ],
         argparser,
     )
+    args = argparser.parse_args()
+    # Setting bot_email instead of using imap_username directly in case support is needed for imap_username and bot_email being different
+    global bot_email
+    bot_email = args.imap_username
 
 
 def check_required_args(required_args: list[str], argparser: argparse.ArgumentParser):
     """
     Check if required arguments are set
     Useful if using enviroment variables with argparse as default and required are mutually exclusive
     """
```

### Comparing `llmail-0.2.4/llmail/utils/utils.py` & `llmail-0.2.5/llmail/utils/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import re
-from loguru import logger
 from sys import stderr
 
+from loguru import logger
+
+from llmail.utils.cli_args import args
+
 logging_file = stderr
 
 
 def redact_email_sink(message: str):
     """Custom sink function that redacts email addresses before logging."""
     email_pattern = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b"
     redacted_message = re.sub(email_pattern, "[redacted]", message)
@@ -15,7 +18,10 @@
 def set_primary_logger(log_level, redact_email_addresses):
     """Set up the primary logger with the specified log level. Output to stderr and use the format specified."""
     logger.remove()
     # ^10 is a formatting directive to center with a padding of 10
     logger_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</green> |<level>{level: ^10}</level>| <level>{message}</level>"
     sink = redact_email_sink if redact_email_addresses else stderr
     logger.add(sink=sink, format=logger_format, colorize=True, level=log_level)
+
+
+set_primary_logger(args.log_level, args.redact_email_addresses)
```

### Comparing `llmail-0.2.4/pyproject.toml` & `llmail-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llmail"
-version = "0.2.4"
+version = "0.2.5"
 description = "Interact with LLMs via email"
 authors = ["slashtechno <77907286+slashtechno@users.noreply.github.com>"]
 repository = "https://github.com/slashtechno/llmail"
 keywords = ["llm", "email", "ai", "openai"]
 license = "GNU Affero General Public License v3"
 readme = "README.md"
```

### Comparing `llmail-0.2.4/README.md` & `llmail-0.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # LLMail  
 Interact with Large Language Models (LLMs) via email.
+[![Watch the video](https://img.youtube.com/vi/0YHQaxvxGoI/maxresdefault.jpg)](https://youtu.be/0YHQaxvxGoI)
+
 
 ### Features  
 - Utilize any OpenAI-compatible API with any available model
     - At the time of writing, [OpenRouter](https://openrouter.ai/docs#models) offers free access to specific models with an OpenAI-compatible API
     - [Ollama](https://github.com/ollama/ollama) has an OpenAI-compatible API and allows for easy local deployment of LLMs  
 - Customize the behavior of the LLM with a system prompt
 - Easily run in a Docker container
```

### Comparing `llmail-0.2.4/PKG-INFO` & `llmail-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmail
-Version: 0.2.4
+Version: 0.2.5
 Summary: Interact with LLMs via email
 Home-page: https://github.com/slashtechno/llmail
 License: GNU Affero General Public License v3
 Keywords: llm,email,ai,openai
 Author: slashtechno
 Author-email: 77907286+slashtechno@users.noreply.github.com
 Requires-Python: >=3.10.0,<4.0.0
@@ -21,14 +21,16 @@
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: yagmail[all] (>=0.15.293,<0.16.0)
 Project-URL: Repository, https://github.com/slashtechno/llmail
 Description-Content-Type: text/markdown
 
 # LLMail  
 Interact with Large Language Models (LLMs) via email.
+[![Watch the video](https://img.youtube.com/vi/0YHQaxvxGoI/maxresdefault.jpg)](https://youtu.be/0YHQaxvxGoI)
+
 
 ### Features  
 - Utilize any OpenAI-compatible API with any available model
     - At the time of writing, [OpenRouter](https://openrouter.ai/docs#models) offers free access to specific models with an OpenAI-compatible API
     - [Ollama](https://github.com/ollama/ollama) has an OpenAI-compatible API and allows for easy local deployment of LLMs  
 - Customize the behavior of the LLM with a system prompt
 - Easily run in a Docker container
```

