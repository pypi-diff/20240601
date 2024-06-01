# Comparing `tmp/salve_ipc-0.2.2.tar.gz` & `tmp/salve_ipc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salve_ipc-0.2.2.tar", last modified: Thu May 30 05:28:34 2024, max compression
+gzip compressed data, was "salve_ipc-0.3.0.tar", last modified: Sat Jun  1 11:04:58 2024, max compression
```

## Comparing `salve_ipc-0.2.2.tar` & `salve_ipc-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:28:34.127036 salve_ipc-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-05-30 05:28:34.127036 salve_ipc-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:28:34.123036 salve_ipc-0.2.2/salve_ipc/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/salve_ipc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:28:34.127036 salve_ipc-0.2.2/salve_ipc/highlight/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/salve_ipc/highlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/salve_ipc/highlight/highlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/salve_ipc/ipc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/salve_ipc/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/salve_ipc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/salve_ipc/server_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:28:34.127036 salve_ipc-0.2.2/salve_ipc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-05-30 05:28:34.000000 salve_ipc-0.2.2/salve_ipc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 05:28:34.000000 salve_ipc-0.2.2/salve_ipc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:28:34.000000 salve_ipc-0.2.2/salve_ipc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 05:28:34.000000 salve_ipc-0.2.2/salve_ipc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 05:28:34.000000 salve_ipc-0.2.2/salve_ipc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:28:34.127036 salve_ipc-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-30 05:28:23.000000 salve_ipc-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/salve_ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/salve_ipc/highlight/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/highlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/highlight/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/salve_ipc/server_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/salve_ipc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 11:04:58.000000 salve_ipc-0.3.0/salve_ipc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 11:04:58.831773 salve_ipc-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-06-01 11:04:51.000000 salve_ipc-0.3.0/setup.py
```

### Comparing `salve_ipc-0.2.2/LICENSE` & `salve_ipc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.2.2/PKG-INFO` & `salve_ipc-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salve_ipc
-Version: 0.2.2
+Version: 0.3.0
 Summary: A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor
 Home-page: https://github.com/Moosems/salve
 Author: Moosems
 Author-email: moosems.j@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,18 @@
 
 # Installation
 
 In the Command Line, paste the following: `pip install salve_ipc`
 
 ## Description
 
-Salve is an IPC library that can be used by code editors to get autocompletions, replacements, and syntax highlighting.
+Salve is an IPC library that can be used by code editors to easily get autocompletions, replacements, and syntax highlighting.
+
+> **Note**
+> The first time that the system is loaded or a new server needs to be started it will take a fair bit longer than if it is simply kept alive by pinging regularly.
 
 ## Documentation
 
 ### `COMMANDS`
 
 The `COMMANDS` list contains all valid commands to request server output from. If multiple requests of different commands are made they will be kept and held seperately and can be retrieved seperately. Current commands are as follows:
 
@@ -37,87 +40,72 @@
 - "replacements"
 - "highlight"
 
 ### `generic_tokens`
 
 The `generic_tokens` list is a list of strings that define all of the generic token types returned by the server which can be mapped to colors for syntax highlighting.
 
-### `Request` and `Response` TypedDict classes
-
-The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
-
 ### `Token` dataclass
 
 The `Token` dataclass gives easy type checking for tokens returned from the highlight command.
 
+### `hidden_chars`
+
+The `hidden_chars` (`dict[str, str]`) dictionary holds a bunch of hidden (zero width) characters as keys and then names for them as values. `Token`'s of type "Hidden_Char" give the index to hidden characters and allow the user to display hidden characters to them that they may not see. These characters appear in code posted on forums or blogs by those hoping to prevent others from simply copy-pasting their code along with many other places.
+
+### `Response` TypedDict classes
+
+The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
+
 ### `is_unicode_letter(char: str) -> bool`
 
 The `is_unicode_letter()` function returns a boolean if a given word is a unicode letter (includes "\_" as special case) which can be useful when trying to find the current word being typed to hand to the IPC for autocompletion.
 
-### `tokens_from_result(result: list[str]) -> list[Token]`
+### `tokens_from_result(result: list[tuple[tuple[int, int], int, str]) -> list[Token]`
 
-The `tokens_from_result()` function takes the results from a `highlight` commands results output and returns a list `Token` types from it to be used for highlighting.
+The `tokens_from_result()` function takes the results from a `highlight` commands output and returns a list `Token` types from it to be used for highlighting. The mapping of the result to `Token` is very simple however and this step can be skipped if one understands how to read the return values.
 
 ### `IPC` Class
 
-| Method              | Description                                                                                                                                                                                                                                                                                          | Arguments                                                                                                                                                                         |
-| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                             | None                                                                                                                                                                              |
-| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                             | `command`: str                                                                                                                                                                    |
-| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                        | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
-| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                              | `command`: str                                                                                                                                                                    |
-| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                    | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
-| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash. | `filename`: str                                                                                                                                                                   |
-| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                  | None                                                                                                                                                                              |
+| Method              | Description                                                                                                                                                                                                                                                                                                                                               | Arguments                                                                                                                                                                         |
+| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                                                                                  | None                                                                                                                                                                              |
+| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                                                                                  | `command`: str                                                                                                                                                                    |
+| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                                                                             | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
+| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                                                                                   | `command`: str                                                                                                                                                                    |
+| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                                                                         | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
+| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash (`Request`'s go after `Notification`'s and `Ping`'s). | `filename`: str                                                                                                                                                                   |
+| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                                                                       | None                                                                                                                                                                              |
 
 ### Basic Usage:
 
 ```python
-from os import set_blocking
-from selectors import EVENT_READ, DefaultSelector
-from sys import stdin, stdout
-
-from salve_ipc import IPC, Response
-
-autocompleter = IPC()
-
-set_blocking(stdin.fileno(), False)
-set_blocking(stdin.fileno(), False)
-selector = DefaultSelector()
-selector.register(stdin, EVENT_READ)
-
-stdout.write("Code: \n")
-stdout.flush()
-
-while True:
-    # Keep IPC alive
-    autocompleter.ping()
-
-    # Add file
-    autocompleter.add_file("test", "")
-
-    # Check input
-    events = selector.select(0.025)
-    if events:
-        # Make requests
-        for line in stdin:
-            autocompleter.update_file("test", line)
-            autocompleter.request(
-                "autocomplete",
-                expected_keywords=[],
-                full_text=line,
-                current_word=line[-2],
-            )
-
-    # Check output
-    output: Response | None = autocompleter.get_response()
-    if not output:
-        continue
-    stdout.write(str(output) + "\n")
-    stdout.flush()
+from time import sleep
+
+from salve_ipc import IPC, Response, tokens_from_result
+
+context = IPC()
+
+context.update_file(
+    "test",
+    open(__file__, "r+").read(),
+)
+
+context.request(
+    "autocomplete",
+    file="test",
+    expected_keywords=[],
+    current_word="t",
+)
+
+sleep(1)
+
+output: Response = context.get_response("autocomplete")  # type: ignore
+print(tokens_from_result(output["result"]))  # type: ignore
+context.kill_IPC()
 ```
 
 ## How to run and contribute
 
 ### Running
 
 To run the example, move `examples/example_usage.py` to the root directory and run with python.
```

### Comparing `salve_ipc-0.2.2/README.md` & `salve_ipc-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 # Installation
 
 In the Command Line, paste the following: `pip install salve_ipc`
 
 ## Description
 
-Salve is an IPC library that can be used by code editors to get autocompletions, replacements, and syntax highlighting.
+Salve is an IPC library that can be used by code editors to easily get autocompletions, replacements, and syntax highlighting.
+
+> **Note**
+> The first time that the system is loaded or a new server needs to be started it will take a fair bit longer than if it is simply kept alive by pinging regularly.
 
 ## Documentation
 
 ### `COMMANDS`
 
 The `COMMANDS` list contains all valid commands to request server output from. If multiple requests of different commands are made they will be kept and held seperately and can be retrieved seperately. Current commands are as follows:
 
@@ -21,87 +24,72 @@
 - "replacements"
 - "highlight"
 
 ### `generic_tokens`
 
 The `generic_tokens` list is a list of strings that define all of the generic token types returned by the server which can be mapped to colors for syntax highlighting.
 
-### `Request` and `Response` TypedDict classes
-
-The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
-
 ### `Token` dataclass
 
 The `Token` dataclass gives easy type checking for tokens returned from the highlight command.
 
+### `hidden_chars`
+
+The `hidden_chars` (`dict[str, str]`) dictionary holds a bunch of hidden (zero width) characters as keys and then names for them as values. `Token`'s of type "Hidden_Char" give the index to hidden characters and allow the user to display hidden characters to them that they may not see. These characters appear in code posted on forums or blogs by those hoping to prevent others from simply copy-pasting their code along with many other places.
+
+### `Response` TypedDict classes
+
+The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
+
 ### `is_unicode_letter(char: str) -> bool`
 
 The `is_unicode_letter()` function returns a boolean if a given word is a unicode letter (includes "\_" as special case) which can be useful when trying to find the current word being typed to hand to the IPC for autocompletion.
 
-### `tokens_from_result(result: list[str]) -> list[Token]`
+### `tokens_from_result(result: list[tuple[tuple[int, int], int, str]) -> list[Token]`
 
-The `tokens_from_result()` function takes the results from a `highlight` commands results output and returns a list `Token` types from it to be used for highlighting.
+The `tokens_from_result()` function takes the results from a `highlight` commands output and returns a list `Token` types from it to be used for highlighting. The mapping of the result to `Token` is very simple however and this step can be skipped if one understands how to read the return values.
 
 ### `IPC` Class
 
-| Method              | Description                                                                                                                                                                                                                                                                                          | Arguments                                                                                                                                                                         |
-| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                             | None                                                                                                                                                                              |
-| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                             | `command`: str                                                                                                                                                                    |
-| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                        | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
-| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                              | `command`: str                                                                                                                                                                    |
-| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                    | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
-| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash. | `filename`: str                                                                                                                                                                   |
-| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                  | None                                                                                                                                                                              |
+| Method              | Description                                                                                                                                                                                                                                                                                                                                               | Arguments                                                                                                                                                                         |
+| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                                                                                  | None                                                                                                                                                                              |
+| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                                                                                  | `command`: str                                                                                                                                                                    |
+| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                                                                             | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
+| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                                                                                   | `command`: str                                                                                                                                                                    |
+| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                                                                         | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
+| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash (`Request`'s go after `Notification`'s and `Ping`'s). | `filename`: str                                                                                                                                                                   |
+| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                                                                       | None                                                                                                                                                                              |
 
 ### Basic Usage:
 
 ```python
-from os import set_blocking
-from selectors import EVENT_READ, DefaultSelector
-from sys import stdin, stdout
-
-from salve_ipc import IPC, Response
-
-autocompleter = IPC()
-
-set_blocking(stdin.fileno(), False)
-set_blocking(stdin.fileno(), False)
-selector = DefaultSelector()
-selector.register(stdin, EVENT_READ)
-
-stdout.write("Code: \n")
-stdout.flush()
-
-while True:
-    # Keep IPC alive
-    autocompleter.ping()
-
-    # Add file
-    autocompleter.add_file("test", "")
-
-    # Check input
-    events = selector.select(0.025)
-    if events:
-        # Make requests
-        for line in stdin:
-            autocompleter.update_file("test", line)
-            autocompleter.request(
-                "autocomplete",
-                expected_keywords=[],
-                full_text=line,
-                current_word=line[-2],
-            )
-
-    # Check output
-    output: Response | None = autocompleter.get_response()
-    if not output:
-        continue
-    stdout.write(str(output) + "\n")
-    stdout.flush()
+from time import sleep
+
+from salve_ipc import IPC, Response, tokens_from_result
+
+context = IPC()
+
+context.update_file(
+    "test",
+    open(__file__, "r+").read(),
+)
+
+context.request(
+    "autocomplete",
+    file="test",
+    expected_keywords=[],
+    current_word="t",
+)
+
+sleep(1)
+
+output: Response = context.get_response("autocomplete")  # type: ignore
+print(tokens_from_result(output["result"]))  # type: ignore
+context.kill_IPC()
 ```
 
 ## How to run and contribute
 
 ### Running
 
 To run the example, move `examples/example_usage.py` to the root directory and run with python.
```

### Comparing `salve_ipc-0.2.2/salve_ipc/ipc.py` & `salve_ipc-0.3.0/salve_ipc/ipc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-from difflib import ndiff
 from json import dumps, loads
-from os import set_blocking
+from os import remove, set_blocking
 from pathlib import Path
 from random import randint
 from subprocess import PIPE, Popen
+from tempfile import NamedTemporaryFile, _TemporaryFileWrapper
 from typing import IO
 
-from .misc import COMMANDS, Message, Notification, Ping, Request, Response
+from .misc import (
+    COMMANDS,
+    Details,
+    Message,
+    Notification,
+    Ping,
+    Request,
+    Response,
+)
 
 
 class IPC:
     """The IPC class is used to talk to the server and run commands ("autocomplete", "replacements", and "highlight"). The public API includes the following methods:
     - IPC.ping()
     - IPC.request()
     - IPC.cancel_request()
     - IPC.update_file()
     - IPC.remove_file()
     - IPC.kill_IPC()
     """
 
     def __init__(self, id_max: int = 15_000) -> None:
-        self.used_ids: list[int] = []
+        self.all_ids: dict[int, str] = {}  # id, tempfile path
         self.id_max = id_max
         self.current_ids: dict[str, int] = {}
         self.newest_responses: dict[str, Response | None] = {}
         for command in COMMANDS:
             self.current_ids[command] = 0
             self.newest_responses[command] = None
 
@@ -40,71 +48,86 @@
         set_blocking(server.stdout.fileno(), False)  # type: ignore
         set_blocking(server.stdin.fileno(), False)  # type: ignore
         self.main_server = server
 
         files_copy = self.files.copy()
         self.files = {}
         for filename, data in files_copy.items():
-            self.add_file(filename, data)
+            self.update_file(filename, data)
 
     def check_server(self) -> None:
         """Checks that the main_server is alive - internal API"""
         if self.main_server.poll() is not None:
             self.create_server()
 
     def get_server_file(self, file: str) -> IO:
         """Returns the main_server stdin/stdout based on the argument provided ("stdin"/"stdout") - internal API"""
         self.check_server()
         if file == "stdout":
             return self.main_server.stdout  # type: ignore
         return self.main_server.stdin  # type: ignore
 
+    def write_tmp_file(self, details: Details, tmp_path: str) -> None:
+        with open(tmp_path, "r+") as file:
+            file.write(dumps(details))
+
     def send_message(self, message: Message) -> None:
         """Sends a Message to the main_server as provided by the argument message - internal API"""
         json_request: str = dumps(message)
 
         server_stdin = self.get_server_file("stdin")
         server_stdin.write(f"{json_request}\n".encode())
         server_stdin.flush()
 
     def create_message(self, type: str, **kwargs) -> None:
         """Creates a Message based on the args and kwawrgs provided. Highly flexible. - internal API"""
         id = randint(1, self.id_max)  # 0 is reserved for the empty case
-        while id in self.used_ids:
+        while id in list(self.all_ids.keys()):
             id = randint(1, self.id_max)
 
-        self.used_ids.append(id)
+        tmp: _TemporaryFileWrapper[str] = NamedTemporaryFile(
+            prefix="salve_ipc", suffix=".tmp", delete=False, mode="r+"
+        )
+        self.all_ids[id] = tmp.name
         match type:
             case "ping":
-                ping: Ping = {"id": id, "type": "ping"}
+                ping: Ping = {"id": id, "type": "ping", "tmp_file": tmp.name}
                 self.send_message(ping)
             case "request":
                 command = kwargs.get("command", "")
                 self.current_ids[command] = id
-                request: Request = {
-                    "id": id,
-                    "type": type,
+                request_details: Request = {
                     "command": command,
                     "file": kwargs.get("file"),
                     "expected_keywords": kwargs.get("expected_keywords"),
                     "current_word": kwargs.get("current_word"),
                     "language": kwargs.get("language"),
                 }  # type: ignore
+                request: Message = {
+                    "id": id,
+                    "type": type,
+                    "tmp_file": tmp.name,
+                }
+                self.write_tmp_file(request_details, tmp.name)
                 self.send_message(request)
             case "notification":
-                notification: Notification = {
+                notification_details: Notification = {
+                    "remove": kwargs.get("remove", False),
+                    "file": kwargs.get("filename", ""),
+                    "contents": kwargs.get("contents", ""),
+                }
+                notification: Message = {
                     "id": id,
                     "type": type,
-                    "remove": kwargs.get("remove", False),
-                    "filename": kwargs.get("filename", ""),
-                    "diff": kwargs.get("diff", ""),
+                    "tmp_file": tmp.name,
                 }
+                self.write_tmp_file(notification_details, tmp.name)
                 self.send_message(notification)
             case _:
-                ping: Ping = {"id": id, "type": "ping"}
+                ping: Ping = {"id": id, "type": "ping", "tmp_file": tmp.name}
                 self.send_message(ping)
 
     def ping(self) -> None:
         """Pings the main_server to keep it alive - external API"""
         self.create_message("ping")
 
     def request(
@@ -118,14 +141,18 @@
         """Sends the main_server a request of type command with given kwargs - external API"""
         if command not in COMMANDS:
             self.kill_IPC()
             raise Exception(
                 f"Command {command} not in builtin commands. Those are {COMMANDS}!"
             )
 
+        if file not in self.files:
+            self.kill_IPC()
+            raise Exception(f"File {file} does not exist in system!")
+
         self.create_message(
             type="request",
             command=command,
             file=file,
             expected_keywords=expected_keywords,
             current_word=current_word,
             language=language,
@@ -139,27 +166,29 @@
                 f"Cannot cancel command {command}, valid commands are {COMMANDS}"
             )
 
         self.current_ids[command] = 0
 
     def parse_line(self, line: str) -> None:
         """Parses main_server output line and discards useless responses - internal API"""
-        response_json: Response = loads(line)
+        response_json: Message = loads(line)
+        details: Response = loads(open(response_json["tmp_file"], "r+").read())
         id = response_json["id"]
-        self.used_ids.remove(id)
+        self.all_ids.pop(id)
+        remove(response_json["tmp_file"])
 
-        if "command" not in response_json:
+        if "command" not in details:
             return
 
-        command = response_json["command"]
+        command = details["command"]
         if id != self.current_ids[command]:
             return
 
         self.current_ids[command] = 0
-        self.newest_responses[command] = response_json
+        self.newest_responses[command] = details
 
     def check_responses(self) -> None:
         """Checks all main_server output by calling IPC.parse_line() on each response - internal API"""
         server_stdout: IO = self.get_server_file("stdout")
 
         for line in server_stdout:  # type: ignore
             self.parse_line(line)
@@ -175,38 +204,22 @@
         self.check_responses()
         response: Response | None = self.newest_responses[command]
         if response is None:
             return None
         self.newest_responses[command] = None
         return response
 
-    def add_file(self, filename: str, current_state: str) -> None:
-        """Adds a file to the main_server's file list - internal API"""
-        if filename in self.files.keys():
-            return
-
-        self.files[filename] = current_state
-
-        diff = "".join(ndiff([""], current_state.splitlines(keepends=True)))
-
-        self.create_message("notification", filename=filename, diff=diff)
-
     def update_file(self, filename: str, current_state: str) -> None:
-        """Updates files if they are already in the system or adds them if not - external API"""
-        self.add_file(filename, current_state)
+        """Updates files in the system - external API"""
 
         self.files[filename] = current_state
 
-        diff = "".join(
-            ndiff(
-                self.files[filename].splitlines(keepends=True),
-                current_state.splitlines(keepends=True),
-            )
+        self.create_message(
+            "notification", filename=filename, contents=current_state
         )
-        self.create_message("notification", filename=filename, diff=diff)
 
     def remove_file(self, filename: str) -> None:
         """Removes a file from the main_server - external API"""
         if filename not in list(self.files.keys()):
             self.kill_IPC()
             raise Exception(
                 f"Cannot remove file {filename} as file is not in file database!"
```

### Comparing `salve_ipc-0.2.2/salve_ipc/misc.py` & `salve_ipc-0.3.0/salve_ipc/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,47 @@
 COMMANDS: list[str] = ["autocomplete", "replacements", "highlight"]
 
 
 class Message(TypedDict):
     """Base class for messages in and out of the server"""
 
     id: int
-    type: str  # Can be "ping", "request", "response", "cancelled", "notification"
+    type: str  # Can be "ping", "request", "response", "notification"
+    tmp_file: str  # Not checked on pings
 
 
-class Request(Message):
+class Ping(Message):
+    """Not really different from a standard Message but the Ping type allows for nice differentiation"""
+
+    ...
+
+
+class Details(TypedDict):
+    """These are the details held by the tmp_file"""
+
+    ...
+
+
+class Request(Details):
     """Request results/output from the server with command specific input"""
 
     command: str  # Can only be commands in COMMANDS
     file: str
     expected_keywords: NotRequired[list[str]]  # autocomplete, replacements
     current_word: NotRequired[str]  # autocomplete, replacements
     language: NotRequired[str]  # highlight
 
 
-class Ping(Message):
-    """Not really different from a standard Message but the Ping type allows for nice differentiation"""
-
-    ...
-
-
-class Notification(Message):
+class Notification(Details):
     """Notifies the server to add/update/remove a file for usage in fulfilling commands"""
 
-    filename: str
+    file: str
     remove: bool
-    diff: NotRequired[str]
+    contents: NotRequired[str]
 
 
-class Response(Message):
+class Response(Details):
     """Server responses to requests, notifications, and pings"""
 
     cancelled: bool
     command: NotRequired[str]
-    result: NotRequired[list[str]]
+    result: NotRequired[list[str | tuple[tuple[int, int], int, str]]]
```

### Comparing `salve_ipc-0.2.2/salve_ipc/server.py` & `salve_ipc-0.3.0/salve_ipc/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,90 +1,104 @@
-from difflib import restore
 from json import dumps, loads
 from os import set_blocking
 from selectors import EVENT_READ, DefaultSelector
 from sys import exit, stdin, stdout
 from time import time
 
 from highlight import Token, get_highlights
-from misc import COMMANDS, Message, Request, Response
+from misc import COMMANDS, Details, Message, Notification, Request, Response
 from server_functions import find_autocompletions, get_replacements
 
 
 class Handler:
     """Handles input from the user and returns output from special functions designed to make the job easy. Not an external API."""
 
     def __init__(self) -> None:
         set_blocking(stdin.fileno(), False)
         set_blocking(stdout.fileno(), False)
         self.selector = DefaultSelector()
         self.selector.register(stdin, EVENT_READ)
 
-        self.id_list: list[int] = []
+        self.all_ids: dict[int, str] = {}  # id, tmp path
         self.newest_ids: dict[str, int] = {}
         self.newest_requests: dict[str, Request | None] = {}
         for command in COMMANDS:
             self.newest_ids[command] = 0
             self.newest_requests[command] = None
 
         self.files: dict[str, str] = {}
 
         self.old_time = time()
 
-    def write_response(self, response: Response) -> None:
-        stdout.write(dumps(response) + "\n")
+    def write_tmp_file(self, details: Details, tmp_path: str) -> None:
+        with open(tmp_path, "r+") as file:
+            file.truncate()
+            file.write(dumps(details))
+            file.flush()
+
+    def write_message(self, message: Message) -> None:
+        stdout.write(dumps(message) + "\n")
         stdout.flush()
 
-    def cancel_id(self, id: int) -> None:
-        response: Response = {"id": id, "type": "response", "cancelled": True}
-        self.write_response(response)
+    def simple_id_response(
+        self, id: int, tmp_path: str, cancelled: bool = True
+    ) -> None:
+        response_details: Response = {
+            "cancelled": cancelled,
+        }
+        response: Message = {
+            "id": id,
+            "type": "response",
+            "tmp_file": tmp_path,
+        }
+        self.write_tmp_file(response_details, tmp_path)
+        self.write_message(response)
 
     def parse_line(self, line: str) -> None:
         json_input: Message = loads(line)
         id: int = json_input["id"]
         match json_input["type"]:
             case "ping":
-                self.cancel_id(id)
+                self.simple_id_response(id, json_input["tmp_file"], False)
             case "notification":
-                filename: str = json_input["filename"]  # type: ignore
-                if json_input["remove"]:  # type: ignore
+                notification_details: Notification = loads(
+                    open(json_input["tmp_file"], "r+").read()
+                )
+                filename: str = notification_details["file"]
+                if notification_details["remove"]:
                     self.files.pop(filename)
                     return
-                diff: list[str] = json_input["diff"].splitlines()  # type: ignore
-                self.files[filename] = "".join(restore(diff, 2))  # type: ignore
+                contents: str = notification_details["contents"]  # type: ignore
+                self.files[filename] = contents
+                self.simple_id_response(id, json_input["tmp_file"], False)
             case _:
-                self.id_list.append(id)
-                command: str = json_input["command"]  # type: ignore
+                request_details: Request = loads(
+                    open(json_input["tmp_file"], "r+").read()
+                )
+                self.all_ids[id] = json_input["tmp_file"]
+                command: str = request_details["command"]  # type: ignore
                 self.newest_ids[command] = id
-                self.newest_requests[command] = json_input  # type: ignore
+                self.newest_requests[command] = request_details  # type: ignore
 
     def cancel_all_ids_except_newest(self) -> None:
-        for id in self.id_list:
+        for id in list(self.all_ids.keys()):
             if id in list(self.newest_ids.values()):
                 continue
-            self.cancel_id(id)
+            self.simple_id_response(id, self.all_ids.pop(id))
 
     def handle_request(self, request: Request) -> None:
-        file: str = request["file"]
-        result: list[str] = []
         command: str = request["command"]
+        id: int = self.newest_ids[command]
+        file: str = request["file"]
+        result: list[str | tuple[tuple[int, int], int, str]] = []
         cancelled: bool = False
-
-        if file not in self.files:
-            response: Response = {
-                "id": request["id"],
-                "type": "response",
-                "cancelled": True,
-                "command": command,
-                "result": result,
-            }
+        tmp_file: str = self.all_ids.pop(id)
 
         match request["command"]:
             case "autocomplete":
-                result: list[str] = []
                 result = find_autocompletions(
                     full_text=self.files[file],
                     expected_keywords=request["expected_keywords"],  # type: ignore
                     current_word=request["current_word"],  # type: ignore
                 )
             case "replacements":
                 result = get_replacements(
@@ -92,27 +106,30 @@
                     expected_keywords=request["expected_keywords"],  # type: ignore
                     replaceable_word=request["current_word"],  # type: ignore
                 )
             case "highlight":
                 pre_refined_result: list[Token] = get_highlights(
                     full_text=self.files[file], language=request["language"]  # type: ignore
                 )
-                result = []
-                result += [str(token) for token in pre_refined_result]
+                result += [token.to_tuple() for token in pre_refined_result]  # type: ignore
             case _:
                 cancelled = True
 
-        response: Response = {
-            "id": request["id"],
-            "type": "response",
+        response_details: Response = {
             "cancelled": cancelled,
             "command": command,
-            "result": result,
+            "result": result,  # type: ignore
         }
-        self.write_response(response)
+        response_message: Message = {
+            "id": id,
+            "type": "response",
+            "tmp_file": tmp_file,
+        }
+        self.write_tmp_file(response_details, response_message["tmp_file"])
+        self.write_message(response_message)
         self.newest_ids[command] = 0
 
     def run_tasks(self) -> None:
         current_time = time()
         if current_time - self.old_time > 5:
             exit(0)
 
@@ -138,14 +155,12 @@
         for request in list(self.newest_requests.values()):
             if request is None:
                 continue
             self.handle_request(request)
             command: str = request["command"]
             self.newest_requests[command] = None
 
-        self.id_list = []
-
 
 if __name__ == "__main__":
     handler = Handler()
     while True:
         handler.run_tasks()
```

### Comparing `salve_ipc-0.2.2/salve_ipc/server_functions.py` & `salve_ipc-0.3.0/salve_ipc/server_functions.py`

 * *Files identical despite different names*

### Comparing `salve_ipc-0.2.2/salve_ipc.egg-info/PKG-INFO` & `salve_ipc-0.3.0/salve_ipc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salve-ipc
-Version: 0.2.2
+Version: 0.3.0
 Summary: A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor
 Home-page: https://github.com/Moosems/salve
 Author: Moosems
 Author-email: moosems.j@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,18 @@
 
 # Installation
 
 In the Command Line, paste the following: `pip install salve_ipc`
 
 ## Description
 
-Salve is an IPC library that can be used by code editors to get autocompletions, replacements, and syntax highlighting.
+Salve is an IPC library that can be used by code editors to easily get autocompletions, replacements, and syntax highlighting.
+
+> **Note**
+> The first time that the system is loaded or a new server needs to be started it will take a fair bit longer than if it is simply kept alive by pinging regularly.
 
 ## Documentation
 
 ### `COMMANDS`
 
 The `COMMANDS` list contains all valid commands to request server output from. If multiple requests of different commands are made they will be kept and held seperately and can be retrieved seperately. Current commands are as follows:
 
@@ -37,87 +40,72 @@
 - "replacements"
 - "highlight"
 
 ### `generic_tokens`
 
 The `generic_tokens` list is a list of strings that define all of the generic token types returned by the server which can be mapped to colors for syntax highlighting.
 
-### `Request` and `Response` TypedDict classes
-
-The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
-
 ### `Token` dataclass
 
 The `Token` dataclass gives easy type checking for tokens returned from the highlight command.
 
+### `hidden_chars`
+
+The `hidden_chars` (`dict[str, str]`) dictionary holds a bunch of hidden (zero width) characters as keys and then names for them as values. `Token`'s of type "Hidden_Char" give the index to hidden characters and allow the user to display hidden characters to them that they may not see. These characters appear in code posted on forums or blogs by those hoping to prevent others from simply copy-pasting their code along with many other places.
+
+### `Response` TypedDict classes
+
+The `Request` and `Response` TypedDict classes allow for type checking when handling output from salve_ipc.
+
 ### `is_unicode_letter(char: str) -> bool`
 
 The `is_unicode_letter()` function returns a boolean if a given word is a unicode letter (includes "\_" as special case) which can be useful when trying to find the current word being typed to hand to the IPC for autocompletion.
 
-### `tokens_from_result(result: list[str]) -> list[Token]`
+### `tokens_from_result(result: list[tuple[tuple[int, int], int, str]) -> list[Token]`
 
-The `tokens_from_result()` function takes the results from a `highlight` commands results output and returns a list `Token` types from it to be used for highlighting.
+The `tokens_from_result()` function takes the results from a `highlight` commands output and returns a list `Token` types from it to be used for highlighting. The mapping of the result to `Token` is very simple however and this step can be skipped if one understands how to read the return values.
 
 ### `IPC` Class
 
-| Method              | Description                                                                                                                                                                                                                                                                                          | Arguments                                                                                                                                                                         |
-| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                             | None                                                                                                                                                                              |
-| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                             | `command`: str                                                                                                                                                                    |
-| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                        | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
-| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                              | `command`: str                                                                                                                                                                    |
-| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                    | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
-| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash. | `filename`: str                                                                                                                                                                   |
-| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                  | None                                                                                                                                                                              |
+| Method              | Description                                                                                                                                                                                                                                                                                                                                               | Arguments                                                                                                                                                                         |
+| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `.ping()`           | Pings the server. After five seconds the server closes if not pinged so it is better for performance to keep it alive but it will be reopened either way                                                                                                                                                                                                  | None                                                                                                                                                                              |
+| `.get_response()`   | Gets a response of the requested command                                                                                                                                                                                                                                                                                                                  | `command`: str                                                                                                                                                                    |
+| `.request()`        | Makes a request to the server                                                                                                                                                                                                                                                                                                                             | `command`: str, `file`: str, `expected_keywords`: list[str] ("autocomple" or "replacements"), `current_word`: str ("autocomple" or "replacements"), `language`: str ("highlight") |
+| `.cancel_request()` | Cancels request of command type and removes reponse if it was recieved. Must be called before `.get_response()` to work                                                                                                                                                                                                                                   | `command`: str                                                                                                                                                                    |
+| `.update_file()`    | Updates files stored on the server that are used to get responses                                                                                                                                                                                                                                                                                         | `filename`: str, `current_state`: str (just the text of the file)                                                                                                                 |
+| `.remove_file()`    | Removes a file of the name given if any exists. Note that a file should only be removed when sure that all other requests using the file are completed. If you delete a file right after a request you run the risk of it removing the file before the task could be run and causing a server crash (`Request`'s go after `Notification`'s and `Ping`'s). | `filename`: str                                                                                                                                                                   |
+| `.kill_IPC()`       | This kills the IPC process and acts as a precaution against wasted CPU when the main thread no longer needs the IPC                                                                                                                                                                                                                                       | None                                                                                                                                                                              |
 
 ### Basic Usage:
 
 ```python
-from os import set_blocking
-from selectors import EVENT_READ, DefaultSelector
-from sys import stdin, stdout
-
-from salve_ipc import IPC, Response
-
-autocompleter = IPC()
-
-set_blocking(stdin.fileno(), False)
-set_blocking(stdin.fileno(), False)
-selector = DefaultSelector()
-selector.register(stdin, EVENT_READ)
-
-stdout.write("Code: \n")
-stdout.flush()
-
-while True:
-    # Keep IPC alive
-    autocompleter.ping()
-
-    # Add file
-    autocompleter.add_file("test", "")
-
-    # Check input
-    events = selector.select(0.025)
-    if events:
-        # Make requests
-        for line in stdin:
-            autocompleter.update_file("test", line)
-            autocompleter.request(
-                "autocomplete",
-                expected_keywords=[],
-                full_text=line,
-                current_word=line[-2],
-            )
-
-    # Check output
-    output: Response | None = autocompleter.get_response()
-    if not output:
-        continue
-    stdout.write(str(output) + "\n")
-    stdout.flush()
+from time import sleep
+
+from salve_ipc import IPC, Response, tokens_from_result
+
+context = IPC()
+
+context.update_file(
+    "test",
+    open(__file__, "r+").read(),
+)
+
+context.request(
+    "autocomplete",
+    file="test",
+    expected_keywords=[],
+    current_word="t",
+)
+
+sleep(1)
+
+output: Response = context.get_response("autocomplete")  # type: ignore
+print(tokens_from_result(output["result"]))  # type: ignore
+context.kill_IPC()
 ```
 
 ## How to run and contribute
 
 ### Running
 
 To run the example, move `examples/example_usage.py` to the root directory and run with python.
```

### Comparing `salve_ipc-0.2.2/setup.py` & `salve_ipc-0.3.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 setup(
     name="salve_ipc",
-    version="0.2.2",
+    version="0.3.0",
     description="A module that makes easily provides autocompletions, replacement suggestions, and syntax highlighting to your code editor",
     author="Moosems",
     author_email="moosems.j@gmail.com",
     url="https://github.com/Moosems/salve",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["pygments"],
+    install_requires=[line for line in open("requirements.txt").readlines()],
     python_requires=">=3.9",
     license="MIT license",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Typing :: Typed",
     ],
     packages=["salve_ipc"],
-    package_data={"salve_ipc": ["./*", "./highlight/*"]},
+    package_data={
+        "salve_ipc": ["./*", "./highlight/*"],
+        "./": ["requirements.txt"],
+    },
 )
```

