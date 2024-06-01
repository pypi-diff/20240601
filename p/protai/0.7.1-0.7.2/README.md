# Comparing `tmp/protai-0.7.1.tar.gz` & `tmp/protai-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protai-0.7.1.tar", last modified: Tue May 28 14:27:04 2024, max compression
+gzip compressed data, was "protai-0.7.2.tar", last modified: Sat Jun  1 03:08:26 2024, max compression
```

## Comparing `protai-0.7.1.tar` & `protai-0.7.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 14:27:04.481591 protai-0.7.1/
--rw-rw-rw-   0        0        0     1107 2024-05-23 18:18:24.000000 protai-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     4993 2024-05-28 14:27:04.480591 protai-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     4319 2024-05-26 01:15:37.000000 protai-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 14:27:04.471448 protai-0.7.1/protai/
--rw-rw-rw-   0        0        0        5 2024-05-28 14:23:48.000000 protai-0.7.1/protai/VERSION
--rw-rw-rw-   0        0        0      612 2024-05-28 14:21:45.000000 protai-0.7.1/protai/__init__.py
--rw-rw-rw-   0        0        0     4919 2024-05-25 22:43:02.000000 protai-0.7.1/protai/auth.py
--rw-rw-rw-   0        0        0     2971 2024-05-28 14:24:41.000000 protai-0.7.1/protai/protai.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:27:04.479591 protai-0.7.1/protai.egg-info/
--rw-rw-rw-   0        0        0     4993 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-28 14:27:04.000000 protai-0.7.1/protai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 14:27:04.481591 protai-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     4360 2024-05-28 14:23:28.000000 protai-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:08:26.327018 protai-0.7.2/
+-rw-rw-rw-   0        0        0     1107 2024-05-23 18:18:24.000000 protai-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     4993 2024-06-01 03:08:26.326020 protai-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4319 2024-05-26 01:15:37.000000 protai-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 03:08:26.315502 protai-0.7.2/protai/
+-rw-rw-rw-   0        0        0        5 2024-06-01 02:42:27.000000 protai-0.7.2/protai/VERSION
+-rw-rw-rw-   0        0        0      612 2024-05-28 14:21:45.000000 protai-0.7.2/protai/__init__.py
+-rw-rw-rw-   0        0        0     5109 2024-06-01 02:52:56.000000 protai-0.7.2/protai/auth.py
+-rw-rw-rw-   0        0        0     3581 2024-06-01 02:45:18.000000 protai-0.7.2/protai/protai.py
+-rw-rw-rw-   0        0        0     1464 2024-05-31 18:38:24.000000 protai-0.7.2/protai/texteffects.py
+drwxrwxrwx   0        0        0        0 2024-06-01 03:08:26.325020 protai-0.7.2/protai.egg-info/
+-rw-rw-rw-   0        0        0     4993 2024-06-01 03:08:26.000000 protai-0.7.2/protai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-06-01 03:08:26.000000 protai-0.7.2/protai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 03:08:26.000000 protai-0.7.2/protai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-06-01 03:08:26.000000 protai-0.7.2/protai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-06-01 03:08:26.000000 protai-0.7.2/protai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 03:08:26.000000 protai-0.7.2/protai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 03:08:26.327018 protai-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     4366 2024-06-01 03:08:20.000000 protai-0.7.2/setup.py
```

### Comparing `protai-0.7.1/LICENSE` & `protai-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protai-0.7.1/PKG-INFO` & `protai-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protai
-Version: 0.7.1
+Version: 0.7.2
 Summary: A useful 0-Shot AI in the terminal
 Home-page: https://github.com/protik09/terminal-ai
 Author: Protik Banerji
 Author-email: protik09@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `protai-0.7.1/README.md` & `protai-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `protai-0.7.1/protai/__init__.py` & `protai-0.7.2/protai/__init__.py`

 * *Files identical despite different names*

### Comparing `protai-0.7.1/protai/auth.py` & `protai-0.7.2/protai/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import os
 import re
 import keyring
 import keyring.errors
 
 # This dependancy exists solely so I can give user feedback when typing in a masked password
 from prompt_toolkit import prompt
+from texteffects import printBanner, successString, errorString
 
 KEYRING_SYSTEM: str = "groq"
 KEYRING_USER: str = "api-key"
 API_KEY_MIN_SIZE: int = 30
 API_KEY_MAX_SIZE: int = 1024
 
 
@@ -37,20 +38,20 @@
         exit(1)
     except keyring.errors.KeyringLocked:
         print("[KeyringError]: Keyring is locked.")
         exit(1)
     return keyring_exists
 
 
-def _getApiKeyFromKeyring() -> str:
+def _getApiKeyFromKeyring() -> str | None:
     """Get password from keyring"""
-    password: str = None
+    password: str | None = None
     if _checkKeyringExists():  # If keyring is available
         try:
-            password: str = keyring.get_password(KEYRING_SYSTEM, KEYRING_USER)
+            password = keyring.get_password(KEYRING_SYSTEM, KEYRING_USER)
         except keyring.errors.KeyringError as e:  # If keyring is not available
             print(f"[KeyringError]: {e}")
             exit(1)
     return password
 
 
 def _getApiKeyUser() -> str:
@@ -59,94 +60,99 @@
         api_key = prompt("Enter GROQ API Key: ", is_password=True)
     except KeyboardInterrupt:
         print("KeyboardInterrupt: Exiting...")
         exit(1)
     return api_key
 
 
-def _validateApiKey(api_key: str) -> bool:
+def _validateApiKey(api_key: str | None) -> bool:
     """Validate API key"""
+    if api_key is None:
+        return False
     pattern = re.compile(
         r"^gsk_[a-zA-Z0-9]{"
         + str(API_KEY_MIN_SIZE)
         + r","
         + str(API_KEY_MAX_SIZE)
-        + r"}$"  # ^gsk_[a-zA-Z0-9]{30,1024}$
+        + r"}$"  # regex "^gsk_[a-zA-Z0-9]{30,1024}$"
     )
     return bool(pattern.match(api_key))
 
 
-def _deleteApiKey() -> None:
+def deleteApiKey() -> None:
     """Delete API key from keyring and environment variable"""
     if _checkKeyringExists():  # If keyring is available
         try:
             keyring.delete_password(KEYRING_SYSTEM, KEYRING_USER)
         except keyring.errors.PasswordDeleteError:
-            print("[KeyringError]: Failed to delete password in keyring.")
+            print(errorString("[KeyringError]: No such password in keyring."))
 
         try:
             del os.environ["GROQ_API_KEY"]
         except KeyError:
             #             print(
             #                 "[KeyringError]: Failed to delete password in os.environ. \
-            # It's ok though you can still overwrite it."
-            #             )
+            # It's ok though you can still overwrite it." )
             pass
+        print(successString("API key deleted"))
     else:  # If keyring is not available
-        print("[OsEnvError]: GROQ_API_KEY is not available.")
+        print(errorString("[OsEnvError]: GROQ_API_KEY is not available."))
+
     exit(0)
 
 
 def changeApiKey() -> int:
     """Change API key"""
     error_code = 0
     # Delete key from keyring
-    _deleteApiKey()
+    deleteApiKey()
     # Ask user for password
     api_key = _getApiKeyUser()
 
     if _validateApiKey(api_key):  # Validate API key
         keyring.set_password(
             KEYRING_SYSTEM, KEYRING_USER, api_key
         )  # Store password in keyring
     else:
         error_code = 1  # Invalid API key
 
     return error_code
 
 
-def authGroq() -> str:
+def authGroq() -> str | None:
     """Get API key either from Environment Variable or Keyring"""
     api_key = None
 
     # GET API KEY
     # Check if GROQ API Key exists as an environment variable
     if "GROQ_API_KEY" in os.environ:
         api_key = os.environ["GROQ_API_KEY"]
         print("[DEBUG]: GROQ_API_KEY is set as an environment variable")
         if api_key == "":
             print("GROQ_API_KEY is empty")
             del os.environ["GROQ_API_KEY"]  # Delete key from environment
             api_key = None
     elif _getApiKeyFromKeyring() is None:  # If password is not stored in keyring
+        # Looks like its probably the first time you're running the program
+        printBanner()
         # Get password from user
         api_key = _getApiKeyUser()
         # print(f"[DEBUG]: Entered API key length: {len(api_key)}")  # Debugging info
         try:
             # Store password in keyring
             keyring.set_password(KEYRING_SYSTEM, KEYRING_USER, api_key)
         except keyring.errors.PasswordSetError:
             print("[KeyringError]: Failed to set password in keyring")
     else:  # If password is stored in keyring
-        api_key = _getApiKeyFromKeyring()  # Get password from keyring
+        api_key = _getApiKeyFromKeyring()
 
     # Validate API key
     if not _validateApiKey(api_key):
         print("[KeyError]: Invalid API key. Please check your API key.")
-        _deleteApiKey()  # Delete API key from keyring and environment variable
+        deleteApiKey()
         api_key = None
     else:  # It is a valid API Key
         pass
     return api_key
 
 
 if __name__ == "__main__":
```

### Comparing `protai-0.7.1/protai/protai.py` & `protai-0.7.2/protai/protai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
+from __future__ import annotations
 import sys
-import os
 import argparse
 from rich import print
 from rich.markdown import Markdown
 from groq import Groq, GroqError
-from auth import authGroq, changeApiKey
+from auth import authGroq, changeApiKey, deleteApiKey
 from yaspin import yaspin
-from protai import __version__  # Import the version
+from __init__ import __version__  # noqa: F401
 
 
 # Set your GROQ API endpoint URL
 GROQ_API_URL = "https://api.groq.io/v1/query"
 
 
 def versionHandler() -> None:
@@ -21,65 +21,83 @@
 
 
 def exitHandler(exit_code: int) -> None:
     """TODO: Write more comprehensive exit handler when inspiration strikes."""
     sys.exit(exit_code)
 
 
+def chatCompletionHandler(
+    client: Groq, system_prompt: str, user_input: str
+) -> str | None:
+    """Handle the chat completion request."""
+    # Send the request to the GROQ API
+    chat_completion = client.chat.completions.create(
+        messages=[
+            {"role": "system", "content": system_prompt},
+            {"role": "user", "content": user_input},
+        ],
+        model="llama3-8b-8192",
+    )
+    reply: str | None = chat_completion.choices[0].message.content
+    return reply
+
+
 def main():
     parser = argparse.ArgumentParser(description="protai")
     parser.add_argument("user_input", nargs="*", help="User input")
     parser.add_argument("-v", "--version", action="store_true", help="Show the version")
     parser.add_argument(
         "-c",
         "--change",
         action="store_true",
         help="Change the API key for the GROQ API",
     )
+    parser.add_argument(
+        "-d", "--delete", action="store_true", help="Delete the current API key"
+    )
 
     args = parser.parse_args()
 
     if not args.version and not args.change and len(sys.argv) < 2:
         print("Usage: protai <user input>")
         exitHandler(0)
     elif args.version:
         versionHandler()
+    elif args.delete:
+        deleteApiKey()
     elif args.change:
-        print("Change the API key for the GROQ API")
+        print("\nChange the API key for the GROQ API.\n")
         exitHandler(changeApiKey())
     else:
         user_input = " ".join(args.user_input)
     # print(f"[DEBUG] User input is: {user_input}")
 
     # Set the query parameters
     try:
         client = Groq(api_key=authGroq())
     except GroqError:  # Catch any errors from the Groq class
         print("An error occurred when authenticating with the GROQ API.")
 
-    system_prompt = "You are an AI agent called ProtAI. You will reply succinctly to any input you receive. \
+    system_prompt: str = "You are an AI agent called ProtAI. You will reply succinctly to any input you receive. \
         Your replies will be in the Standard Markdown format. ALWAYS start your replies with '[ProtAI]: ' \
         If providing code snippets, always ensure code highlighting for the appropriate programming language \
         is applied. Always ensure, if sending markdown, that the markdown is sytactically correct."
 
     with yaspin(text="Processing...", color="green") as spinner:
         try:
-            # Send the request to the GROQ API
-            chat_completion = client.chat.completions.create(
-                messages=[
-                    {"role": "system", "content": system_prompt},
-                    {"role": "user", "content": user_input},
-                ],
-                model="llama3-8b-8192",
-            )
-            reply = chat_completion.choices[0].message.content
-            spinner.ok("[✔ ]")  # mark spinner as finished successfully
+            reply: str | None = chatCompletionHandler(client, system_prompt, user_input)
+            spinner.ok("[✔]")  # mark spinner as finished successfully
             # Print the reply in Markdown overwriting the spinner
-            print(Markdown(str("\033[F" + reply)))
+            print(Markdown("\033[F" + str(reply) + "\n"))
+            # print(Markdown(reply))
         except Exception as e:
-            spinner.fail("[✖ ] Processing Failed...")  # mark spinner as failed
-            print(f"An error occurred: {e}")
+            spinner.fail("[✖] Processing Failed...")  # mark spinner as failed
+            print(f"\nAn error occurred: {e}\n")
             exitHandler(1)
 
 
 if __name__ == "__main__":
+    # from time import time_ns
+    # start_time = time_ns()
     main()
+    # end_time = time_ns()
+    # print(f"\n\n\nGROQ Time taken: {(end_time - start_time)/1000000:.4f}ms\n\n\n")
```

### Comparing `protai-0.7.1/protai.egg-info/PKG-INFO` & `protai-0.7.2/protai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protai
-Version: 0.7.1
+Version: 0.7.2
 Summary: A useful 0-Shot AI in the terminal
 Home-page: https://github.com/protik09/terminal-ai
 Author: Protik Banerji
 Author-email: protik09@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `protai-0.7.1/setup.py` & `protai-0.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 VERSION = read_version(version_file_path)
 
 # What packages are required for this module to be executed?
 REQUIRED = requirements
 
 # What packages are optional?
-EXTRAS = {
+EXTRAS: dict = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

