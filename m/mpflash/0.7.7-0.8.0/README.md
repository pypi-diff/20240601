# Comparing `tmp/mpflash-0.7.7.tar.gz` & `tmp/mpflash-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpflash-0.7.7.tar", max compression
+gzip compressed data, was "mpflash-0.8.0.tar", max compression
```

## Comparing `mpflash-0.7.7.tar` & `mpflash-0.8.0.tar`

### file list

```diff
@@ -1,42 +1,46 @@
--rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.7/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.7/mpflash/__init__.py
--rw-r--r--   0        0        0     9459 2024-05-07 20:07:54.692259 mpflash-0.7.7/mpflash/ask_input.py
--rw-r--r--   0        0        0     3623 2024-05-07 20:07:54.695005 mpflash-0.7.7/mpflash/cli_download.py
--rw-r--r--   0        0        0     6133 2024-05-07 20:07:54.697239 mpflash-0.7.7/mpflash/cli_flash.py
--rw-r--r--   0        0        0     2424 2024-05-07 20:25:23.483181 mpflash-0.7.7/mpflash/cli_group.py
--rw-r--r--   0        0        0     1024 2024-04-29 18:55:09.408806 mpflash-0.7.7/mpflash/cli_list.py
--rw-r--r--   0        0        0      796 2024-05-07 20:07:54.699465 mpflash-0.7.7/mpflash/cli_main.py
--rw-r--r--   0        0        0     1049 2024-04-29 18:55:09.409821 mpflash-0.7.7/mpflash/common.py
--rw-r--r--   0        0        0      495 2024-05-07 20:25:16.221241 mpflash-0.7.7/mpflash/config.py
--rw-r--r--   0        0        0    11120 2024-05-03 13:05:36.160916 mpflash-0.7.7/mpflash/download.py
--rw-r--r--   0        0        0     3803 2024-04-29 18:55:09.412110 mpflash-0.7.7/mpflash/downloaded.py
--rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.7.7/mpflash/errors.py
--rw-r--r--   0        0        0     2490 2024-04-29 18:55:09.414103 mpflash-0.7.7/mpflash/flash.py
--rw-r--r--   0        0        0     2314 2024-05-03 13:05:36.160916 mpflash-0.7.7/mpflash/flash_esp.py
--rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.7.7/mpflash/flash_stm32.py
--rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.7.7/mpflash/flash_stm32_cube.py
--rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.7.7/mpflash/flash_stm32_dfu.py
--rw-r--r--   0        0        0     2441 2024-05-07 20:28:07.108289 mpflash-0.7.7/mpflash/flash_uf2.py
--rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.7/mpflash/flash_uf2_boardid.py
--rw-r--r--   0        0        0     4049 2024-05-07 20:20:22.285175 mpflash-0.7.7/mpflash/flash_uf2_linux.py
--rw-r--r--   0        0        0     2740 2024-05-07 20:17:40.591356 mpflash-0.7.7/mpflash/flash_uf2_macos.py
--rw-r--r--   0        0        0     1093 2024-05-03 13:05:36.160916 mpflash-0.7.7/mpflash/flash_uf2_windows.py
--rw-r--r--   0        0        0     4713 2024-05-03 13:05:36.167441 mpflash-0.7.7/mpflash/list.py
--rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.7/mpflash/logger.py
--rw-r--r--   0        0        0     3621 2024-05-03 13:05:36.168458 mpflash-0.7.7/mpflash/mpboard_id/__init__.py
--rw-r--r--   0        0        0     2592 2024-05-07 20:07:47.160190 mpflash-0.7.7/mpflash/mpboard_id/board_id.py
--rw-r--r--   0        0        0    96983 2024-05-07 20:07:47.163202 mpflash-0.7.7/mpflash/mpboard_id/board_info.csv
--rw-r--r--   0        0        0   674442 2024-05-07 08:36:27.021683 mpflash-0.7.7/mpflash/mpboard_id/board_info.json
--rw-r--r--   0        0        0    15759 2024-05-07 10:08:07.568299 mpflash-0.7.7/mpflash/mpboard_id/Untitled-1.ipynb
--rw-r--r--   0        0        0     7683 2024-05-07 20:07:54.702473 mpflash-0.7.7/mpflash/mpremoteboard/__init__.py
--rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.7/mpflash/mpremoteboard/mpy_fw_info.py
--rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.7.7/mpflash/mpremoteboard/runner.py
--rw-r--r--   0        0        0      298 2024-05-07 20:17:27.989525 mpflash-0.7.7/mpflash/uf2disk.py
--rw-r--r--   0        0        0     5739 2024-04-29 18:55:09.422436 mpflash-0.7.7/mpflash/vendor/dfu.py
--rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.7.7/mpflash/vendor/pydfu.py
--rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.7.7/mpflash/vendor/readme.md
--rw-r--r--   0        0        0     3629 2024-05-07 20:07:47.167675 mpflash-0.7.7/mpflash/vendor/versions.py
--rw-r--r--   0        0        0     5297 2024-05-03 13:05:36.171762 mpflash-0.7.7/mpflash/worklist.py
--rw-r--r--   0        0        0     1666 2024-05-07 20:33:36.178933 mpflash-0.7.7/pyproject.toml
--rw-r--r--   0        0        0    13159 2024-04-29 21:19:09.956495 mpflash-0.7.7/README.md
--rw-r--r--   0        0        0    14671 1970-01-01 00:00:00.000000 mpflash-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.8.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.8.0/mpflash/__init__.py
+-rw-r--r--   0        0        0     3435 2024-05-22 21:29:21.517582 mpflash-0.8.0/mpflash/add_firmware.py
+-rw-r--r--   0        0        0     8496 2024-05-27 21:07:02.040121 mpflash-0.8.0/mpflash/ask_input.py
+-rw-r--r--   0        0        0     3645 2024-05-27 21:03:47.978786 mpflash-0.8.0/mpflash/cli_download.py
+-rw-r--r--   0        0        0     7074 2024-05-27 21:24:52.546385 mpflash-0.8.0/mpflash/cli_flash.py
+-rw-r--r--   0        0        0     1974 2024-05-27 21:03:47.983988 mpflash-0.8.0/mpflash/cli_group.py
+-rw-r--r--   0        0        0     1997 2024-05-27 21:03:47.983988 mpflash-0.8.0/mpflash/cli_list.py
+-rw-r--r--   0        0        0     1030 2024-06-01 12:56:07.150733 mpflash-0.8.0/mpflash/cli_main.py
+-rw-r--r--   0        0        0     5594 2024-06-01 11:40:47.253016 mpflash-0.8.0/mpflash/common.py
+-rw-r--r--   0        0        0      495 2024-05-27 21:03:47.991712 mpflash-0.8.0/mpflash/config.py
+-rw-r--r--   0        0        0     3029 2024-05-27 21:03:47.992049 mpflash-0.8.0/mpflash/connected.py
+-rw-r--r--   0        0        0    11421 2024-06-01 11:29:24.977288 mpflash-0.8.0/mpflash/download.py
+-rw-r--r--   0        0        0     3804 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/downloaded.py
+-rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.8.0/mpflash/errors.py
+-rw-r--r--   0        0        0     2468 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/flash.py
+-rw-r--r--   0        0        0     2311 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/flash_esp.py
+-rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.8.0/mpflash/flash_stm32.py
+-rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.8.0/mpflash/flash_stm32_cube.py
+-rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.8.0/mpflash/flash_stm32_dfu.py
+-rw-r--r--   0        0        0     2508 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/flash_uf2.py
+-rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.8.0/mpflash/flash_uf2_boardid.py
+-rw-r--r--   0        0        0     4055 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/flash_uf2_linux.py
+-rw-r--r--   0        0        0     2696 2024-05-27 21:03:48.002459 mpflash-0.8.0/mpflash/flash_uf2_macos.py
+-rw-r--r--   0        0        0     1093 2024-05-03 13:05:36.160916 mpflash-0.8.0/mpflash/flash_uf2_windows.py
+-rw-r--r--   0        0        0     2963 2024-05-27 21:03:48.002459 mpflash-0.8.0/mpflash/list.py
+-rw-r--r--   0        0        0     1098 2024-05-09 18:26:02.794085 mpflash-0.8.0/mpflash/logger.py
+-rw-r--r--   0        0        0     3576 2024-06-01 12:35:35.666067 mpflash-0.8.0/mpflash/mpboard_id/__init__.py
+-rw-r--r--   0        0        0     9684 2024-06-01 13:17:03.471049 mpflash-0.8.0/mpflash/mpboard_id/add_boards.py
+-rw-r--r--   0        0        0     1151 2024-06-01 12:35:24.218389 mpflash-0.8.0/mpflash/mpboard_id/board.py
+-rw-r--r--   0        0        0     2489 2024-06-01 12:32:47.930044 mpflash-0.8.0/mpflash/mpboard_id/board_id.py
+-rw-r--r--   0        0        0    19759 2024-06-01 13:17:49.539026 mpflash-0.8.0/mpflash/mpboard_id/board_info.zip
+-rw-r--r--   0        0        0     1462 2024-06-01 12:41:26.069251 mpflash-0.8.0/mpflash/mpboard_id/store.py
+-rw-r--r--   0        0        0     7683 2024-05-10 21:00:04.227607 mpflash-0.8.0/mpflash/mpremoteboard/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.8.0/mpflash/mpremoteboard/mpy_fw_info.py
+-rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.8.0/mpflash/mpremoteboard/runner.py
+-rw-r--r--   0        0        0      298 2024-05-27 21:03:48.006614 mpflash-0.8.0/mpflash/uf2disk.py
+-rw-r--r--   0        0        0     9545 2024-05-27 21:03:57.348737 mpflash-0.8.0/mpflash/vendor/basicgit.py
+-rw-r--r--   0        0        0     5755 2024-05-27 21:03:48.006614 mpflash-0.8.0/mpflash/vendor/dfu.py
+-rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.8.0/mpflash/vendor/pydfu.py
+-rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.8.0/mpflash/vendor/readme.md
+-rw-r--r--   0        0        0     3783 2024-05-27 21:06:13.964512 mpflash-0.8.0/mpflash/vendor/versions.py
+-rw-r--r--   0        0        0     5962 2024-06-01 12:14:29.624478 mpflash-0.8.0/mpflash/worklist.py
+-rw-r--r--   0        0        0     1651 2024-06-01 13:22:52.017074 mpflash-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13680 2024-05-27 21:03:47.974599 mpflash-0.8.0/README.md
+-rw-r--r--   0        0        0    15224 1970-01-01 00:00:00.000000 mpflash-0.8.0/PKG-INFO
```

### Comparing `mpflash-0.7.7/LICENSE` & `mpflash-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/ask_input.py` & `mpflash-0.8.0/mpflash/ask_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,158 +1,132 @@
 """
 Interactive input for mpflash.
 
 Note: The prompts can use "{version}" and "{action}" to insert the version and action in the prompt without needing an f-string.
 The values are provided from the answers dictionary.
 """
 
-from dataclasses import dataclass, field
-from pathlib import Path
-from typing import Dict, List, Sequence, Tuple, Union
+from typing import List, Sequence, Tuple, Union
 
 from loguru import logger as log
 
-from mpflash.config import config
-from mpflash.mpboard_id import get_known_boards_for_port, get_known_ports, known_stored_boards
-from mpflash.mpremoteboard import MPRemoteBoard
-from mpflash.vendor.versions import micropython_versions
-
-
-@dataclass
-class Params:
-    ports: List[str] = field(default_factory=list)
-    boards: List[str] = field(default_factory=list)
-    versions: List[str] = field(default_factory=list)
-    fw_folder: Path = Path()
-
-
-@dataclass
-class DownloadParams(Params):
-    clean: bool = False
-    force: bool = False
-
-
-@dataclass
-class FlashParams(Params):
-    # TODO: Should Serial port be a list?
-    serial: str = ""
-    erase: bool = True
-    bootloader: bool = True
-    cpu: str = ""
-
-
-ParamType = Union[DownloadParams, FlashParams]
+from .common import DownloadParams, FlashParams, ParamType
+from .config import config
+from .mpboard_id import get_known_boards_for_port, get_known_ports, known_stored_boards
+from .mpremoteboard import MPRemoteBoard
+from .vendor.versions import micropython_versions
 
 
 def ask_missing_params(
     params: ParamType,
-    # action: str = "download",
 ) -> ParamType:
     """
     Asks the user for parameters that have not been supplied on the commandline and returns the updated params.
 
     Args:
         params (ParamType): The parameters to be updated.
-        action (str, optional): The action to be performed. Defaults to "download".
 
     Returns:
         ParamType: The updated parameters.
     """
+    import inquirer
+
+    log.trace(f"ask_missing_params: {params}")
+
     # if action flash,  single input
     # if action download, multiple input
     multi_select = isinstance(params, DownloadParams)
     action = "download" if isinstance(params, DownloadParams) else "flash"
     if not config.interactive:
         # no interactivity allowed
         return params
-    # import only when needed to reduce load time
-    import inquirer
 
     questions = []
-    answers = {"action": "download" if isinstance(params, DownloadParams) else "flash"}
+    answers: dict[str, Union[str, List]] = {"action": action}
     if not multi_select:
         if not params.serial or "?" in params.serial:
-            ask_serialport(questions)
+            questions.append(ask_serialport(multi_select=False, bluetooth=False))
         else:
             answers["serial"] = params.serial
 
-    if not params.versions or "?" in params.versions:
-        ask_versions(questions, multi_select=multi_select, action=action)
+    if params.versions == [] or "?" in params.versions:
+        questions.append(ask_mp_version(multi_select=multi_select, action=action))
     else:
         # versions is used to show only the boards for the selected versions
         answers["versions"] = params.versions  # type: ignore
 
     if not params.boards or "?" in params.boards:
-        ask_port_board(questions, multi_select=multi_select, action=action)
+        questions.extend(ask_port_board(multi_select=multi_select, action=action))
     if questions:
-        answers = inquirer.prompt(questions, answers=answers)
+        answers = inquirer.prompt(questions, answers=answers)  # type: ignore
     if not answers:
         # input cancelled by user
         return []  # type: ignore
-    # print(repr(answers))
+    log.trace(f"answers: {answers}")
     if isinstance(params, FlashParams) and "serial" in answers:
-        params.serial = answers["serial"].split()[0]  # split to remove the description
+        if isinstance(answers["serial"], str):
+            answers["serial"] = [answers["serial"]]
+        params.serial = [s.split()[0] for s in answers["serial"]]  # split to remove the description
     if "port" in answers:
         params.ports = [p for p in params.ports if p != "?"]  # remove the "?" if present
-        params.ports.append(answers["port"])
+        params.ports.extend(answers["port"])
     if "boards" in answers:
         params.boards = [b for b in params.boards if b != "?"]  # remove the "?" if present
         params.boards.extend(answers["boards"] if isinstance(answers["boards"], list) else [answers["boards"]])
     if "versions" in answers:
         params.versions = [v for v in params.versions if v != "?"]  # remove the "?" if present
         # make sure it is a list
         if isinstance(answers["versions"], (list, tuple)):
             params.versions.extend(answers["versions"])
         else:
             params.versions.append(answers["versions"])
     # remove duplicates
     params.ports = list(set(params.ports))
     params.boards = list(set(params.boards))
     params.versions = list(set(params.versions))
-    log.debug(repr(params))
+    log.trace(f"ask_missing_params returns: {params}")
 
     return params
 
 
 def filter_matching_boards(answers: dict) -> Sequence[Tuple[str, str]]:
     """
     Filters the known boards based on the selected versions and returns the filtered boards.
 
     Args:
         answers (dict): The user's answers.
 
     Returns:
         Sequence[Tuple[str, str]]: The filtered boards.
     """
+    versions = None
     # if version is not asked ; then need to get the version from the inputs
     if "versions" in answers:
-        _versions = list(answers["versions"])
-        if "stable" in _versions:
-            _versions.remove("stable")
-            _versions.append(micropython_versions()[-2])  # latest stable
-        if "preview" in _versions:
-            _versions.remove("preview")
-            _versions.extend((micropython_versions()[-1], micropython_versions()[-2]))  # latest preview and stable
+        versions = list(answers["versions"])
+        if "stable" in versions:
+            versions.remove("stable")
+            versions.append(micropython_versions()[-2])  # latest stable
+        elif "preview" in versions:
+            versions.remove("preview")
+            versions.extend((micropython_versions()[-1], micropython_versions()[-2]))  # latest preview and stable
 
-        some_boards = known_stored_boards(answers["port"], _versions)  #    or known_mp_boards(answers["port"])
-    else:
-        some_boards = known_stored_boards(answers["port"])
+    some_boards = known_stored_boards(answers["port"], versions)  #    or known_mp_boards(answers["port"])
 
     if some_boards:
         # Create a dictionary where the keys are the second elements of the tuples
         # This will automatically remove duplicates because dictionaries cannot have duplicate keys
         unique_dict = {item[1]: item for item in some_boards}
         # Get the values of the dictionary, which are the unique items from the original list
         some_boards = list(unique_dict.values())
     else:
-        some_boards = [(f"No {answers['port']} boards found for version(s) {_versions}", "")]
+        some_boards = [(f"No {answers['port']} boards found for version(s) {versions}", "")]
     return some_boards
 
 
-def ask_port_board(questions: list, *, multi_select: bool, action: str):
+def ask_port_board(*, multi_select: bool, action: str):
     """
     Asks the user for the port and board selection.
 
     Args:
         questions (list): The list of questions to be asked.
         action (str): The action to be performed.
 
@@ -161,103 +135,92 @@
     """
     # import only when needed to reduce load time
     import inquirer
 
     # if action flash,  single input
     # if action download, multiple input
     inquirer_ux = inquirer.Checkbox if multi_select else inquirer.List
-    questions.extend(
-        (
-            inquirer.List(
-                "port",
-                message="Which port do you want to {action} " + "to {serial} ?" if action == "flash" else "?",
-                choices=get_known_ports(),
-                autocomplete=True,
-            ),
-            inquirer_ux(
-                "boards",
-                message=(
-                    "Which {port} board firmware do you want to {action} " + "to {serial} ?"
-                    if action == "flash"
-                    else "?"
-                ),
-                choices=filter_matching_boards,
-                validate=lambda _, x: True if x else "Please select at least one board",  # type: ignore
+    return [
+        inquirer.List(
+            "port",
+            message="Which port do you want to {action} " + "to {serial} ?" if action == "flash" else "?",
+            choices=get_known_ports(),
+            # autocomplete=True,
+        ),
+        inquirer_ux(
+            "boards",
+            message=(
+                "Which {port} board firmware do you want to {action} " + "to {serial} ?" if action == "flash" else "?"
             ),
-        )
-    )
+            choices=filter_matching_boards,
+            validate=lambda _, x: True if x else "Please select at least one board",  # type: ignore
+        ),
+    ]
 
 
-def ask_versions(questions: list, *, multi_select: bool, action: str):
+def ask_mp_version(multi_select: bool, action: str):
     """
     Asks the user for the version selection.
 
     Args:
         questions (list): The list of questions to be asked.
         action (str): The action to be performed.
 
     Returns:
-        None
+
     """
     # import only when needed to reduce load time
     import inquirer
     import inquirer.errors
 
     input_ux = inquirer.Checkbox if multi_select else inquirer.List
+
     mp_versions: List[str] = micropython_versions()
-    mp_versions = [v for v in mp_versions if "preview" not in v]
+    mp_versions.reverse()  # newest first
 
     # remove the versions for which there are no known boards in the board_info.json
     # todo: this may be a little slow
-    mp_versions = [v for v in mp_versions if get_known_boards_for_port("stm32", [v])]
-
-    mp_versions.append("preview")
-    mp_versions.reverse()  # newest first
+    mp_versions = [v for v in mp_versions if "preview" in v or get_known_boards_for_port("stm32", [v])]
 
     def at_least_one_validation(answers, current) -> bool:
         if not current:
             raise inquirer.errors.ValidationError("", reason="Please select at least one version")
-        if isinstance(current, list):
-            if not any(current):
-                raise inquirer.errors.ValidationError("", reason="Please select at least one version")
+        if isinstance(current, list) and not any(current):
+            raise inquirer.errors.ValidationError("", reason="Please select at least one version")
         return True
 
-    questions.append(
-        input_ux(
-            # inquirer.List(
-            "versions",
-            message="Which version(s) do you want to {action} " + ("to {serial} ?" if action == "flash" else "?"),
-            # Hints would be nice , but needs a hint for each and every option
-            # hints=["Use space to select multiple options"],
-            choices=mp_versions,
-            autocomplete=True,
-            validate=at_least_one_validation,  # type: ignore
-        )
+    message = "Which version(s) do you want to {action} " + ("to {serial} ?" if action == "flash" else "?")
+    q = input_ux(
+        # inquirer.List(
+        "versions",
+        message=message,
+        # Hints would be nice , but needs a hint for each and every option
+        # hints=["Use space to select multiple options"],
+        choices=mp_versions,
+        autocomplete=True,
+        validate=at_least_one_validation,  # type: ignore
     )
+    return q
 
 
-def ask_serialport(questions: list, *, multi_select: bool = False, bluetooth: bool = False):
+def ask_serialport(*, multi_select: bool = False, bluetooth: bool = False):
     """
     Asks the user for the serial port selection.
 
     Args:
         questions (list): The list of questions to be asked.
         action (str): The action to be performed.
 
     Returns:
         None
     """
     # import only when needed to reduce load time
     import inquirer
 
     comports = MPRemoteBoard.connected_boards(bluetooth=bluetooth, description=True)
-    questions.append(
-        inquirer.List(
-            "serial",
-            message="Which serial port do you want to {action} ?",
-            choices=comports,
-            other=True,
-            validate=lambda _, x: True if x else "Please select or enter a serial port",  # type: ignore
-        )
+    return inquirer.List(
+        "serial",
+        message="Which serial port do you want to {action} ?",
+        choices=comports,
+        other=True,
+        validate=lambda _, x: True if x else "Please select or enter a serial port",  # type: ignore
     )
-
-    return questions
```

### Comparing `mpflash-0.7.7/mpflash/cli_download.py` & `mpflash-0.8.0/mpflash/cli_download.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """CLI to Download MicroPython firmware for specific ports, boards and versions."""
 
 from pathlib import Path
-from typing import List, Tuple
 
 import rich_click as click
 from loguru import logger as log
 
+from mpflash.connected import connected_ports_boards
 from mpflash.errors import MPFlashError
 from mpflash.mpboard_id import find_known_board
 from mpflash.vendor.versions import clean_version
 
-from .ask_input import DownloadParams, ask_missing_params
+from .ask_input import ask_missing_params
 from .cli_group import cli
-from .cli_list import list_mcus
+from .common import DownloadParams
 from .config import config
 from .download import download
 
 
 @cli.command(
     "download",
     help="Download MicroPython firmware for specific ports, boards and versions.",
@@ -47,14 +47,36 @@
     multiple=True,
     default=[],
     show_default=True,
     help="The board(s) to download the firmware for.",
     metavar="BOARD_ID or ?",
 )
 @click.option(
+    "--serial",
+    "--serial-port",
+    "-s",
+    "serial",
+    default=["*"],
+    show_default=True,
+    multiple=True,
+    help="Which serial port(s) to flash",
+    metavar="SERIALPORT",
+)
+@click.option(
+    "--ignore",
+    "-i",
+    is_eager=True,
+    help="Serial port(s) to ignore. Defaults to MPFLASH_IGNORE.",
+    multiple=True,
+    default=[],
+    envvar="MPFLASH_IGNORE",
+    show_default=True,
+    metavar="SERIALPORT",
+)
+@click.option(
     "--clean/--no-clean",
     default=True,
     show_default=True,
     help="""Remove dates and hashes from the downloaded firmware filenames.""",
 )
 @click.option(
     "--force",
@@ -63,27 +85,31 @@
     show_default=True,
     help="""Force download of firmware even if it already exists.""",
 )
 def cli_download(**kwargs) -> int:
     params = DownloadParams(**kwargs)
     params.versions = list(params.versions)
     params.boards = list(params.boards)
+    params.serial = list(params.serial)
+    params.ignore = list(params.ignore)
+
+    # all_boards: List[MPRemoteBoard] = []
     if params.boards:
         if not params.ports:
             # no ports specified - resolve ports from specified boards by resolving board IDs
             for board in params.boards:
                 if board != "?":
                     try:
                         board_ = find_known_board(board)
-                        params.ports.append(board_["port"])
+                        params.ports.append(board_.port)
                     except MPFlashError as e:
                         log.error(f"{e}")
     else:
         # no boards specified - detect connected ports and boards
-        params.ports, params.boards = connected_ports_boards()
+        params.ports, params.boards, _ = connected_ports_boards(include=params.serial, ignore=params.ignore)
 
     params = ask_missing_params(params)
     if not params:  # Cancelled by user
         return 2
     params.versions = [clean_version(v, drop_v=True) for v in params.versions]
     assert isinstance(params, DownloadParams)
 
@@ -96,23 +122,7 @@
             params.force,
             params.clean,
         )
         return 0
     except MPFlashError as e:
         log.error(f"{e}")
         return 1
-
-
-def connected_ports_boards() -> Tuple[List[str], List[str]]:
-    """
-    Returns a tuple containing lists of unique ports and boards from the connected MCUs.
-    Boards that are physically connected, but give no tangible response are ignored.
-
-    Returns:
-        A tuple containing two lists:
-            - A list of unique ports where MCUs are connected.
-            - A list of unique board names of the connected MCUs.
-    """
-    mpr_boards = [b for b in list_mcus() if b.connected]
-    ports = list({b.port for b in mpr_boards})
-    boards = list({b.board for b in mpr_boards})
-    return ports, boards
```

### Comparing `mpflash-0.7.7/mpflash/cli_flash.py` & `mpflash-0.8.0/mpflash/cli_flash.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from pathlib import Path
+from typing import List
 
 import rich_click as click
 from loguru import logger as log
 
+# from mpflash.common import filtered_comports
 from mpflash.errors import MPFlashError
 from mpflash.mpboard_id import find_known_board
+from mpflash.mpremoteboard import MPRemoteBoard
 from mpflash.vendor.versions import clean_version
 
-from .ask_input import FlashParams, ask_missing_params
+from .ask_input import ask_missing_params
 from .cli_download import connected_ports_boards
 from .cli_group import cli
 from .cli_list import show_mcus
+from .common import FlashParams
 from .config import config
 from .flash import flash_list
-from .worklist import MPRemoteBoard, WorkList, full_auto_worklist, manual_worklist, single_auto_worklist
+from .worklist import WorkList, full_auto_worklist, manual_worklist, single_auto_worklist
 
 # #########################################################################################################
 # CLI
 # #########################################################################################################
 
 
 @cli.command(
@@ -44,18 +48,30 @@
     metavar="SEMVER, 'stable', 'preview' or '?'",
 )
 @click.option(
     "--serial",
     "--serial-port",
     "-s",
     "serial",
-    default="auto",
+    default=["*"],
+    multiple=True,
     show_default=True,
     help="Which serial port(s) to flash",
-    metavar="SERIAL_PORT",
+    metavar="SERIALPORT",
+)
+@click.option(
+    "--ignore",
+    "-i",
+    is_eager=True,
+    help="Serial port(s) to ignore. Defaults to MPFLASH_IGNORE.",
+    multiple=True,
+    default=[],
+    envvar="MPFLASH_IGNORE",
+    show_default=True,
+    metavar="SERIALPORT",
 )
 @click.option(
     "--port",
     "-p",
     "ports",
     help="The MicroPython port to flash",
     metavar="PORT",
@@ -97,77 +113,75 @@
     if kwargs["board"] is None:
         kwargs["boards"] = []
         kwargs.pop("board")
     else:
         kwargs["boards"] = [kwargs.pop("board")]
 
     params = FlashParams(**kwargs)
-
-    # make it simple for the user to flash one board
-    # by asking for the serial port if not specified
-    if params.boards == ["?"] and params.serial == "auto":
-        params.serial = "?"
+    params.versions = list(params.versions)
+    params.boards = list(params.boards)
+    params.serial = list(params.serial)
+    params.ignore = list(params.ignore)
+
+    # make it simple for the user to flash one board by asking for the serial port if not specified
+    if params.boards == ["?"] and params.serial == "*":
+        params.serial = ["?"]
 
     # Detect connected boards if not specified,
     # and ask for input if boards cannot be detected
+    all_boards: List[MPRemoteBoard] = []
     if not params.boards or params.boards == []:
         # nothing specified - detect connected boards
-        params.ports, params.boards = connected_ports_boards()
+        params.ports, params.boards, all_boards = connected_ports_boards(include=params.ports, ignore=params.ignore)
         if params.boards == []:
             # No MicroPython boards detected, but it could be unflashed or not in bootloader mode
             # Ask for serial port and board_id to flash
-            params.serial = "?"
+            params.serial = ["?"]
             params.boards = ["?"]
     else:
-        for board_id in params.boards:
-            if board_id == "":
-                params.boards.remove(board_id)
-                continue
-            if " " in board_id:
-                try:
-                    info = find_known_board(board_id)
-                    if info:
-                        log.info(f"Resolved board description: {info['board']}")
-                        params.boards.remove(board_id)
-                        params.boards.append(info["board"])
-                except Exception as e:
-                    log.warning(f"unable to resolve board description: {e}")
+        resolve_board_ids(params)
 
     # Ask for missing input if needed
     params = ask_missing_params(params)
     if not params:  # Cancelled by user
         return 2
     # TODO: Just in time Download of firmware
 
     assert isinstance(params, FlashParams)
 
     if len(params.versions) > 1:
         log.error(f"Only one version can be flashed at a time, not {params.versions}")
         raise MPFlashError("Only one version can be flashed at a time")
-    # if len(params.boards) > 1:
-    #     log.error(f"Only one board can be flashed at a time, not {params.boards}")
-    #     raise MPFlashError("Only one board can be flashed at a time")
 
     params.versions = [clean_version(v) for v in params.versions]
     worklist: WorkList = []
     # if serial port == auto and there are one or more specified/detected boards
-    if params.serial == "auto" and params.boards:
-        worklist = full_auto_worklist(version=params.versions[0], fw_folder=params.fw_folder)
+    if params.serial == ["*"] and params.boards:
+        if not all_boards:
+            log.trace("No boards detected yet, scanning for connected boards")
+            _, _, all_boards = connected_ports_boards(include=params.ports, ignore=params.ignore)
+        worklist = full_auto_worklist(
+            all_boards=all_boards,
+            version=params.versions[0],
+            fw_folder=params.fw_folder,
+            include=params.serial,
+            ignore=params.ignore,
+        )
     elif params.versions[0] and params.boards[0] and params.serial:
-        # A single serial port including the board / variant
+        # A one or more  serial port including the board / variant
         worklist = manual_worklist(
-            params.versions[0],
-            params.fw_folder,
-            params.serial,
-            params.boards[0],
+            params.serial[0],
+            board_id=params.boards[0],
+            version=params.versions[0],
+            fw_folder=params.fw_folder,
         )
     else:
         # just this serial port on auto
         worklist = single_auto_worklist(
-            serial_port=params.serial,
+            serial=params.serial[0],
             version=params.versions[0],
             fw_folder=params.fw_folder,
         )
 
     if flashed := flash_list(
         worklist,
         params.fw_folder,
@@ -176,7 +190,23 @@
     ):
         log.info(f"Flashed {len(flashed)} boards")
         show_mcus(flashed, title="Updated boards after flashing")
         return 0
     else:
         log.error("No boards were flashed")
         return 1
+
+
+def resolve_board_ids(params):
+    """Resolve board descriptions to board_id, and remove empty strings from list of boards"""
+    for board_id in params.boards:
+        if board_id == "":
+            params.boards.remove(board_id)
+            continue
+        if " " in board_id:
+            try:
+                if info := find_known_board(board_id):
+                    log.info(f"Resolved board description: {info.board_id}")
+                    params.boards.remove(board_id)
+                    params.boards.append(info.board_id)
+            except Exception as e:
+                log.warning(f"Unable to resolve board description: {e}")
```

### Comparing `mpflash-0.7.7/mpflash/cli_group.py` & `mpflash-0.8.0/mpflash/cli_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 """
 Main entry point for the CLI group.
 Additional comands are added in the submodules.
 """
 
-import sys
-
 import rich_click as click
 
 from .config import config
 from .logger import make_quiet, set_loglevel
 
 
 def cb_verbose(ctx, param, value):
     """Callback to set the log level to DEBUG if verbose is set"""
     if value and not config.quiet:
-        set_loglevel("DEBUG")
         config.verbose = True
+        if value > 1:
+            set_loglevel("TRACE")
+        else:
+            set_loglevel("DEBUG")
     else:
         set_loglevel("INFO")
         config.verbose = False
     return value
 
 
-def cb_ignore(ctx, param, value):
-    if value:
-        config.ignore_ports = list(value)
-        if sys.platform == "win32":
-            config.ignore_ports = [port.upper() for port in config.ignore_ports]
-    return value
-
-
 def cb_interactive(ctx, param, value):
     if value:
         config.interactive = value
     return value
 
 
 def cb_test(ctx, param, value):
@@ -70,31 +63,19 @@
     default=True,
     show_default=True,
 )
 @click.option(
     "-V",
     "--verbose",
     is_eager=True,
-    is_flag=True,
+    count=True,
     help="Enables verbose mode.",
     callback=cb_verbose,
 )
 @click.option(
-    "--ignore",
-    "-i",
-    is_eager=True,
-    help="Serial port(s) to ignore. Defaults to MPFLASH_IGNORE.",
-    callback=cb_ignore,
-    multiple=True,
-    default=[],
-    envvar="MPFLASH_IGNORE",
-    show_default=True,
-    metavar="SERIALPORT",
-)
-@click.option(
     "--test",
     is_eager=True,
     help="test a specific feature",
     callback=cb_test,
     multiple=True,
     default=[],
     envvar="MPFLASH_TEST",
```

### Comparing `mpflash-0.7.7/mpflash/cli_main.py` & `mpflash-0.8.0/mpflash/cli_main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 """mpflash is a CLI to download and flash MicroPython firmware to various boards."""
 
 # import rich_click as click
 
+import os
+
 import click
 from loguru import logger as log
 
 from .cli_download import cli_download
 from .cli_flash import cli_flash_board
 from .cli_group import cli
 from .cli_list import cli_list_mcus
 
 
 def mpflash():
-    cli.add_command(cli_flash_board)
     cli.add_command(cli_list_mcus)
     cli.add_command(cli_download)
+    cli.add_command(cli_flash_board)
+
     # cli(auto_envvar_prefix="MPFLASH")
-    try:
+    if False and os.environ.get("COMPUTERNAME") == "JOSVERL-S4":
+        # intentional less error suppression on dev machine
         result = cli(standalone_mode=False)
-        exit(result)
-    except AttributeError as e:
-        log.error(f"Error: {e}")
-        exit(-1)
-    except click.exceptions.ClickException as e:
-        log.error(f"Error: {e}")
-        exit(-2)
+    else:
+        try:
+            result = cli(standalone_mode=False)
+            exit(result)
+        except AttributeError as e:
+            log.error(f"Error: {e}")
+            exit(-1)
+        except click.exceptions.ClickException as e:
+            log.error(f"Error: {e}")
+            exit(-2)
 
 
 if __name__ == "__main__":
     mpflash()
```

### Comparing `mpflash-0.7.7/mpflash/download.py` & `mpflash-0.8.0/mpflash/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 # make sure that jsonlines does not mistake the MicroPython ujson for the CPython ujson
 import jsonlines
 import requests
 from bs4 import BeautifulSoup
 from loguru import logger as log
 from rich.progress import track
 
-from mpflash.common import PORT_FWTYPES
+from mpflash.common import PORT_FWTYPES, FWInfo
 from mpflash.errors import MPFlashError
 from mpflash.mpboard_id import get_known_ports
 
+# avoid conflict with the ujson used by MicroPython
 jsonlines.ujson = None  # type: ignore
 # #########################################################################################################
 
 
 MICROPYTHON_ORG_URL = "https://micropython.org/"
 
 # Regexes to remove dates and hashes in the filename that just get in the way
@@ -47,14 +48,18 @@
 def get_board_urls(page_url: str) -> List[Dict[str, str]]:
     """
     Get the urls to all the board pages listed on this page.
     Assumes that all links to firmware  have "class": "board-card"
 
     Args:
         page_url (str): The url of the page to get the board urls from.
+
+    Returns:
+        List[Dict[str, str]]: A list of dictionaries containing the board name and url.
+
     """
     downloads_html = get_page(page_url)
     soup = BeautifulSoup(downloads_html, "html.parser")
     tags = soup.findAll("a", recursive=True, attrs={"class": "board-card"})
     # assumes that all links are relative to the page url
     boards = [tag.get("href") for tag in tags]
     if "?" in page_url:
@@ -85,84 +90,89 @@
     )
     if "?" in base_url:
         base_url = base_url.split("?")[0]
     links: List = [urljoin(base_url, tag.get("href")) for tag in tags]
     return links
 
 
-# type alias for the firmware info
-FirmwareInfo = Dict[str, str]
-
-
 # boards we are interested in ( this avoids getting a lot of boards we don't care about)
 # The first run takes ~60 seconds to run for 4 ports , all boards
 # so it makes sense to cache the results and skip boards as soon as possible
-def get_boards(ports: List[str], boards: List[str], clean: bool) -> List[FirmwareInfo]:
+def get_boards(ports: List[str], boards: List[str], clean: bool) -> List[FWInfo]:
     """
     Retrieves a list of firmware information for the specified ports and boards.
 
     Args:
         ports (List[str]): The list of ports to check for firmware.
         boards (List[str]): The list of boards to retrieve firmware information for.
         clean (bool): A flag indicating whether to perform a clean retrieval.
 
     Returns:
-        List[FirmwareInfo]: A list of firmware information for the specified ports and boards.
+        List[FWInfo]: A list of firmware information for the specified ports and boards.
 
     """
-    board_urls: List[FirmwareInfo] = []
+    board_urls: List[FWInfo] = []
     if ports is None:
         ports = get_known_ports()
     for port in ports:
         download_page_url = f"{MICROPYTHON_ORG_URL}download/?port={port}"
-        _urls = get_board_urls(download_page_url)
+        urls = get_board_urls(download_page_url)
         # filter out boards we don't care about
-        _urls = [board for board in _urls if board["board"] in boards]
+        urls = [board for board in urls if board["board"] in boards]
         # add the port to the board urls
-        for board in _urls:
+        for board in urls:
             board["port"] = port
 
-        for board in track(_urls, description=f"Checking {port} download pages", transient=True,refresh_per_second=2):
+        for board in track(urls, description=f"Checking {port} download pages", transient=True, refresh_per_second=2):
             # add a board to the list for each firmware found
-            firmwares = []
+            firmware_urls: List[str] = []
             for ext in PORT_FWTYPES[port]:
-                firmwares += board_firmware_urls(board["url"], MICROPYTHON_ORG_URL, ext)
-
-            for _url in firmwares:
+                firmware_urls += board_firmware_urls(board["url"], MICROPYTHON_ORG_URL, ext)
+            for _url in firmware_urls:
                 board["firmware"] = _url
-                board["preview"] = "preview" in _url  # type: ignore
-                if ver_match := re.search(RE_VERSION_PREVIEW, _url):
-                    board["version"] = ver_match[1]
-                else:
-                    board["version"] = ""
-                if "preview." in board["version"]:
-                    board["build"] = board["version"].split("preview.")[-1]
-                else:
-                    board["build"] = "0"
                 fname = Path(board["firmware"]).name
                 if clean:
                     # remove date from firmware name
                     fname = re.sub(RE_DATE, "-", fname)
                     # remove hash from firmware name
                     fname = re.sub(RE_HASH, ".", fname)
-                board["filename"] = fname
-                board["ext"] = Path(board["firmware"]).suffix
-                board["variant"] = board["filename"].split("-v")[0] if "-v" in board["filename"] else ""
-                board_urls.append(board.copy())
+                fw_info = FWInfo(
+                    filename=fname,
+                    port=port,
+                    board=board["board"],
+                    preview="preview" in _url,
+                    firmware=_url,
+                    version="",
+                )
+                # board["firmware"] = _url
+                # board["preview"] = "preview" in _url  # type: ignore
+                if ver_match := re.search(RE_VERSION_PREVIEW, _url):
+                    fw_info.version = ver_match[1]
+                # else:
+                #     board.$1= ""
+                if "preview." in fw_info.version:
+                    fw_info.build = fw_info.version.split("preview.")[-1]
+                else:
+                    fw_info.build = "0"
+
+                fw_info.ext = Path(fw_info.firmware).suffix
+                fw_info.variant = fw_info.filename.split("-v")[0] if "-v" in fw_info.filename else ""
+
+                board_urls.append(fw_info)
     return board_urls
 
 
-def key_fw_ver_pre_ext_bld(x: FirmwareInfo):
+def key_fw_ver_pre_ext_bld(x: FWInfo):
     "sorting key for the retrieved board urls"
-    return x["variant"], x["version"], x["preview"], x["ext"], x["build"]
+    return x.variant, x.version, x.preview, x.ext, x.build
 
 
-def key_fw_var_pre_ext(x: FirmwareInfo):
+def key_fw_var_pre_ext(x: FWInfo):
     "Grouping key for the retrieved board urls"
-    return x["variant"], x["preview"], x["ext"]
+    return x.variant, x.preview, x.ext
 
 
 def download_firmwares(
     firmware_folder: Path,
     ports: List[str],
     boards: List[str],
     versions: Optional[List[str]] = None,
@@ -173,40 +183,40 @@
     skipped = downloaded = 0
     if versions is None:
         versions = []
 
     unique_boards = get_firmware_list(ports, boards, versions, clean)
 
     for b in unique_boards:
-        log.debug(b["filename"])
+        log.debug(b.filename)
     # relevant
 
     log.info(f"Found {len(unique_boards)} relevant unique firmwares")
 
     firmware_folder.mkdir(exist_ok=True)
 
     with jsonlines.open(firmware_folder / "firmware.jsonl", "a") as writer:
         for board in unique_boards:
-            filename = firmware_folder / board["port"] / board["filename"]
+            filename = firmware_folder / board.port / board.filename
             filename.parent.mkdir(exist_ok=True)
             if filename.exists() and not force:
                 skipped += 1
                 log.debug(f" {filename} already exists, skip download")
                 continue
-            log.info(f"Downloading {board['firmware']}")
+            log.info(f"Downloading {board.firmware}")
             log.info(f"         to {filename}")
             try:
-                r = requests.get(board["firmware"], allow_redirects=True)
+                r = requests.get(board.firmware, allow_redirects=True)
                 with open(filename, "wb") as fw:
                     fw.write(r.content)
-                board["filename"] = str(filename.relative_to(firmware_folder))
+                board.filename = str(filename.relative_to(firmware_folder))
             except requests.RequestException as e:
                 log.exception(e)
                 continue
-            writer.write(board)
+            writer.write(board.to_dict())
             downloaded += 1
     log.info(f"Downloaded {downloaded} firmwares, skipped {skipped} existing files.")
     return downloaded + skipped
 
 
 def get_firmware_list(ports: List[str], boards: List[str], versions: List[str], clean: bool):
     """
@@ -215,32 +225,32 @@
     Args:
         ports : The list of ports to check for firmware.
         boards : The list of boards to filter the firmware by.
         versions : The list of versions to filter the firmware by.
         clean : A flag indicating whether to perform a clean check.
 
     Returns:
-        List[FirmwareInfo]: A list of unique firmware information.
+        List[FWInfo]: A list of unique firmware information.
 
     """
 
     log.trace("Checking MicroPython download pages")
     preview = "preview" in versions
     board_urls = sorted(get_boards(ports, boards, clean), key=key_fw_ver_pre_ext_bld)
 
     log.debug(f"Total {len(board_urls)} firmwares")
     relevant = [
         board
         for board in board_urls
-        if board["board"] in boards and (board["version"] in versions or board["preview"] and preview)
+        if board.board in boards and (board.version in versions or board.preview and preview)
         # and b["port"] in ["esp32", "rp2"]
     ]
     log.debug(f"Matching firmwares: {len(relevant)}")
     # select the unique boards
-    unique_boards: List[FirmwareInfo] = []
+    unique_boards: List[FWInfo] = []
     for _, g in itertools.groupby(relevant, key=key_fw_var_pre_ext):
         # list is aleady sorted by build so we can just get the last item
         sub_list = list(g)
         unique_boards.append(sub_list[-1])
     log.debug(f"Last preview only: {len(unique_boards)}")
     return unique_boards
```

### Comparing `mpflash-0.7.7/mpflash/downloaded.py` & `mpflash-0.8.0/mpflash/downloaded.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 # #########################################################################################################
 def downloaded_firmwares(fw_folder: Path) -> List[FWInfo]:
     """Load a list of locally downloaded firmwares from the jsonl file"""
     firmwares: List[FWInfo] = []
     try:
         with jsonlines.open(fw_folder / "firmware.jsonl") as reader:
-            firmwares.extend(iter(reader))
+            firmwares = [FWInfo.from_dict(item) for item in reader]
     except FileNotFoundError:
         log.error(f"No firmware.jsonl found in {fw_folder}")
     # sort by filename
-    firmwares.sort(key=lambda x: x["filename"])
+    firmwares.sort(key=lambda x: x.filename)
     return firmwares
 
 
 def find_downloaded_firmware(
     *,
     board_id: str,
     version: str = "",
@@ -64,15 +64,15 @@
             version=version,
             port=port,
             trie=trie + 1,
             selector=selector,
         )
         # hope we have a match now for the board
     # sort by filename
-    fw_list.sort(key=lambda x: x["filename"])
+    fw_list.sort(key=lambda x: x.filename)
     return fw_list
 
 
 def filter_downloaded_fwlist(
     fw_list: List[FWInfo],
     board_id: str,
     version: str,
@@ -80,29 +80,29 @@
     # preview: bool,
     variants: bool,
     selector: dict,
 ) -> List[FWInfo]:
     """Filter the downloaded firmware list based on the provided parameters"""
     if "preview" in version:
         # never get a preview for an older version
-        fw_list = [fw for fw in fw_list if fw["preview"]]
+        fw_list = [fw for fw in fw_list if fw.preview]
     else:
-        fw_list = [fw for fw in fw_list if fw["version"] == version]
+        fw_list = [fw for fw in fw_list if fw.version == version]
 
     # filter by port
     if port:
-        fw_list = [fw for fw in fw_list if fw["port"] == port]
+        fw_list = [fw for fw in fw_list if fw.port == port]
 
     if board_id:
         if variants:
             # any variant of this board_id
-            fw_list = [fw for fw in fw_list if fw["board"] == board_id]
+            fw_list = [fw for fw in fw_list if fw.board == board_id]
         else:
             # the firmware variant should match exactly the board_id
-            fw_list = [fw for fw in fw_list if fw["variant"] == board_id]
+            fw_list = [fw for fw in fw_list if fw.variant == board_id]
     if selector and port in selector:
-        fw_list = [fw for fw in fw_list if fw["filename"].endswith(selector[port])]
+        fw_list = [fw for fw in fw_list if fw.filename.endswith(selector[port])]
     return fw_list
 
 
 # #########################################################################################################
 #
```

### Comparing `mpflash-0.7.7/mpflash/flash.py` & `mpflash-0.8.0/mpflash/flash.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     fw_folder: Path,
     erase: bool,
     bootloader: bool,
 ):
     """Flash a list of boards with the specified firmware."""
     flashed = []
     for mcu, fw_info in todo:
-        fw_file = fw_folder / fw_info["filename"]  # type: ignore
+        fw_file = fw_folder / fw_info.filename
         if not fw_file.exists():
             log.error(f"File {fw_file} does not exist, skipping {mcu.board} on {mcu.serialport}")
             continue
-        log.info(f"Updating {mcu.board} on {mcu.serialport} to {fw_info['version']}")
+        log.info(f"Updating {mcu.board} on {mcu.serialport} to {fw_info.version}")
         updated = None
         # try:
         if mcu.port in [port for port, exts in PORT_FWTYPES.items() if ".uf2" in exts] and fw_file.suffix == ".uf2":
             # any .uf2 port ["samd", "rp2", "nrf"]:
             if bootloader:
                 enter_bootloader(mcu)
             updated = flash_uf2(mcu, fw_file=fw_file, erase=erase)
```

### Comparing `mpflash-0.7.7/mpflash/flash_esp.py` & `mpflash-0.8.0/mpflash/flash_esp.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     if mcu.port not in ["esp32", "esp8266"] or mcu.board in ["ARDUINO_NANO_ESP32"]:
         log.error(f"esptool not supported for {mcu.port} {mcu.board} on {mcu.serialport}")
         return None
 
     log.info(f"Flashing {fw_file} on {mcu.board} on {mcu.serialport}")
     if not mcu.cpu:
         # Lookup CPU based on the board name
-        mcu.cpu = find_known_board(mcu.board)["cpu"]
+        mcu.cpu = find_known_board(mcu.board).cpu
 
     cmds: List[List[str]] = []
     if erase:
         cmds.append(f"esptool --chip {mcu.cpu} --port {mcu.serialport} erase_flash".split())
 
     if mcu.cpu.upper().startswith("ESP32"):
         baud_rate = str(921_600)
```

### Comparing `mpflash-0.7.7/mpflash/flash_stm32.py` & `mpflash-0.8.0/mpflash/flash_stm32.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/flash_stm32_cube.py` & `mpflash-0.8.0/mpflash/flash_stm32_cube.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/flash_stm32_dfu.py` & `mpflash-0.8.0/mpflash/flash_stm32_dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/flash_uf2.py` & `mpflash-0.8.0/mpflash/flash_uf2.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 from loguru import logger as log
 from rich.progress import track
 
 from mpflash.mpremoteboard import MPRemoteBoard
 
 from .common import PORT_FWTYPES
 from .config import config
-from .flash_uf2_linux import dismount_uf2, wait_for_UF2_linux
+from .flash_uf2_linux import dismount_uf2_linux, wait_for_UF2_linux
 from .flash_uf2_macos import wait_for_UF2_macos
 from .flash_uf2_windows import wait_for_UF2_windows
 
 
 def flash_uf2(mcu: MPRemoteBoard, fw_file: Path, erase: bool) -> Optional[MPRemoteBoard]:
     """
     Flash .UF2 devices via bootloader and filecopy
     - mpremote bootloader
     - Wait for the device to mount as a drive (up to 5s)
     - detect new drive with INFO_UF2.TXT
     - copy the firmware file to the drive
     - wait for the device to restart (5s)
 
-    for Lunix :
-    pmount and pumount are used to mount and unmount the drive
-    as this is not done automatically by the OS in headless mode.
+    for Linux - to support headless operation ( GH Actions ) :
+        pmount and pumount are used to mount and unmount the drive
+        as this is not done automatically by the OS in headless mode.
     """
     if ".uf2" not in PORT_FWTYPES[mcu.port]:
         log.error(f"UF2 not supported on {mcu.board} on {mcu.serialport}")
         return None
     if erase:
         log.info("Erasing not yet implemented for UF2 flashing.")
 
@@ -59,11 +59,11 @@
         return None
 
     log.info("Board is in bootloader mode")
     log.info(f"Copying {fw_file} to {destination}.")
     shutil.copy(fw_file, destination)
     log.success("Done copying, resetting the board and wait for it to restart")
     if sys.platform in ["linux"]:
-        dismount_uf2()
+        dismount_uf2_linux()
     for _ in track(range(5 + 2), description="Waiting for the board to restart", transient=True, refresh_per_second=2):
         time.sleep(1)  # 5 secs to short on linux
     return mcu
```

### Comparing `mpflash-0.7.7/mpflash/flash_uf2_linux.py` & `mpflash-0.8.0/mpflash/flash_uf2_linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         subprocess.run(["pumount", disk.mountpoint])  # ), f"/media/{disk.label}"])
         log.info(f"Unmounted {disk.label} from {disk.mountpoint}")
         disk.mountpoint = f""
     else:
         log.warning(f"{disk.label} already dismounted")
 
 
-def dismount_uf2():
+def dismount_uf2_linux():
     global glb_dismount_me
     for disk in glb_dismount_me:
         pumount(disk)
     glb_dismount_me = []
 
 
 def wait_for_UF2_linux(s_max: int = 10):
```

### Comparing `mpflash-0.7.7/mpflash/flash_uf2_macos.py` & `mpflash-0.8.0/mpflash/flash_uf2_macos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """ Flashing UF2 based MCU on macos"""
 
 # sourcery skip: snake-case-functions
 from __future__ import annotations
 
-import subprocess
 import sys
 import time
 from pathlib import Path
-from typing import List
 
 from loguru import logger as log
 from rich.progress import track
 
 from .flash_uf2_boardid import get_board_id
 from .uf2disk import UF2Disk
```

### Comparing `mpflash-0.7.7/mpflash/flash_uf2_windows.py` & `mpflash-0.8.0/mpflash/flash_uf2_windows.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/logger.py` & `mpflash-0.8.0/mpflash/logger.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/mpboard_id/__init__.py` & `mpflash-0.8.0/mpflash/mpboard_id/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,89 @@
 """
 Access to the micropython port and board information that is stored in the board_info.json file 
 that is included in the module.
 
 """
 
-import json
 from functools import lru_cache
-from pathlib import Path
-from typing import List, Optional, Tuple, TypedDict, Union
+from typing import List, Optional, Tuple
 
-from mpflash.common import PORT_FWTYPES
 from mpflash.errors import MPFlashError
+from mpflash.mpboard_id.board import Board
+from mpflash.mpboard_id.store import read_known_boardinfo
 from mpflash.vendor.versions import clean_version
 
 # KNOWN ports and boards are sourced from the micropython repo,
 # this info is stored in the board_info.json file
 
 
-# Board  based on the dataclass Board but changed to TypedDict
-# - source : get_boardnames.py
-class Board(TypedDict):
-    """MicroPython Board definition"""
-
-    description: str
-    port: str
-    board: str
-    board_name: str
-    mcu_name: str
-    path: Union[Path, str]
-    version: str
-    cpu: str
-
-
-@lru_cache(maxsize=None)
-def read_known_boardinfo() -> List[Board]:
-    """Reads the board_info.json file and returns the data as a list of Board objects"""
-    with open(Path(__file__).parent / "board_info.json", "r") as file:
-        return json.load(file)
-
-
 def get_known_ports() -> List[str]:
     # TODO: Filter for Version
     mp_boards = read_known_boardinfo()
     # select the unique ports from info
-    ports = set({board["port"] for board in mp_boards if board["port"] in PORT_FWTYPES.keys()})
+    ports = set({board.port for board in mp_boards if board.port})
     return sorted(list(ports))
 
 
-def get_known_boards_for_port(port: str, versions: Optional[List[str]] = None):
+def get_known_boards_for_port(port: Optional[str] = "", versions: Optional[List[str]] = None) -> List[Board]:
     """
     Returns a list of boards for the given port and version(s)
 
-    port : str : The Micropython port to filter for
-    versions : List[str] : The Micropython versions to filter for (actual versions required)"""
+    port: The Micropython port to filter for
+    versions:  Optional, The Micropython versions to filter for (actual versions required)
+    """
     mp_boards = read_known_boardinfo()
+    if versions:
+        preview_or_stable = "preview" in versions or "stable" in versions
+    else:
+        preview_or_stable = False
 
     # filter for 'preview' as they are not in the board_info.json
     # instead use stable version
     versions = versions or []
     if "preview" in versions:
         versions.remove("preview")
         versions.append("stable")
     if versions:
         # make sure of the v prefix
         versions = [clean_version(v) for v in versions]
         # filter for the version(s)
-        mp_boards = [board for board in mp_boards if board["version"] in versions]
+        mp_boards = [board for board in mp_boards if board.version in versions]
+        if not mp_boards and preview_or_stable:
+            # nothing found - perhaps there is a newer version for which we do not have the board info yet
+            # use the latest known version from the board info
+            mp_boards = read_known_boardinfo()
+            last_known_version = sorted({b.version for b in mp_boards})[-1]
+            mp_boards = [board for board in mp_boards if board.version == last_known_version]
+
     # filter for the port
-    mp_boards = [board for board in mp_boards if board["port"] == port]
+    if port:
+        mp_boards = [board for board in mp_boards if board.port == port]
     return mp_boards
 
 
 def known_stored_boards(port: str, versions: Optional[List[str]] = None) -> List[Tuple[str, str]]:
     """
     Returns a list of tuples with the description and board name for the given port and version
 
     port : str : The Micropython port to filter for
     versions : List[str] : The Micropython versions to filter for (actual versions required)
     """
     mp_boards = get_known_boards_for_port(port, versions)
 
-    boards = set({(f'{board["version"]} {board["description"]}', board["board"]) for board in mp_boards})
+    boards = set({(f"{board.version} {board.description}", board.board_id) for board in mp_boards})
     return sorted(list(boards))
 
 
 @lru_cache(maxsize=20)
 def find_known_board(board_id: str) -> Board:
     """Find the board for the given BOARD_ID or 'board description' and return the board info as a Board object"""
     info = read_known_boardinfo()
     for board_info in info:
-        if board_id in (board_info["board"], board_info["description"]):
-            if "cpu" not in board_info or not board_info["cpu"]:
-                if " with " in board_info["description"]:
-                    board_info["cpu"] = board_info["description"].split(" with ")[-1]
+        if board_id in (board_info.board_id, board_info.description):
+            if not board_info.cpu:
+                if " with " in board_info.description:
+                    board_info.cpu = board_info.description.split(" with ")[-1]
                 else:
-                    board_info["cpu"] = board_info["port"]
+                    board_info.cpu = board_info.port
             return board_info
     raise MPFlashError(f"Board {board_id} not found")
```

### Comparing `mpflash-0.7.7/mpflash/mpboard_id/board_id.py` & `mpflash-0.8.0/mpflash/mpboard_id/board_id.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """
 Translate board description to board designator
 """
 
 import functools
-import json
 from pathlib import Path
 from typing import Optional
 
 from mpflash.errors import MPFlashError
+from mpflash.logger import log
+from mpflash.mpboard_id.store import read_known_boardinfo
 from mpflash.vendor.versions import clean_version, get_stable_mp_version
 
-###############################################################################################
-HERE = Path(__file__).parent
-###############################################################################################
-
 
 def find_board_id_by_description(
     descr: str,
     short_descr: str,
     *,
     version: str,
     board_info: Optional[Path] = None,
@@ -27,49 +24,47 @@
     try:
         boards = _find_board_id_by_description(
             descr=descr,
             short_descr=short_descr,
             board_info=board_info,
             version=clean_version(version) if version else None,
         )
-        return boards[-1]["board"]
+        return boards[-1].board_id
     except MPFlashError:
         return "UNKNOWN_BOARD"
 
 
 @functools.lru_cache(maxsize=20)
 def _find_board_id_by_description(
-    *, descr: str, short_descr: str, version: Optional[str] = None, board_info: Optional[Path] = None
+    *,
+    descr: str,
+    short_descr: str,
+    version: Optional[str] = None,
+    board_info: Optional[Path] = None,
 ):
     """
     Find the MicroPython BOARD_ID based on the description in the firmware
     using the pre-built board_info.json file
     """
-    if not board_info:
-        board_info = HERE / "board_info.json"
-    if not board_info.exists():
-        raise FileNotFoundError(f"Board info file not found: {board_info}")
 
-    candidate_boards = _read_board_info(board_info)
+    candidate_boards = read_known_boardinfo(board_info)
 
     if version:
         # filter for matching version
         if version in ("preview", "stable"):
             # match last stable
             version = get_stable_mp_version()
-        version_matches = [b for b in candidate_boards if b["version"].startswith(version)]
+        known_versions = sorted({b.version for b in candidate_boards})
+        if version not in known_versions:
+            # FIXME if latest stable is newer than the last version in the boardlist this will fail
+            log.trace(f"Version {version} not found in board info, using latest known version {known_versions[-1]}")
+            version = known_versions[-1]
+        version_matches = [b for b in candidate_boards if b.version.startswith(version)]
         if not version_matches:
             raise MPFlashError(f"No board info found for version {version}")
         candidate_boards = version_matches
-    matches = [b for b in candidate_boards if b["description"] == descr]
+    matches = [b for b in candidate_boards if b.description == descr]
     if not matches and short_descr:
-        matches = [b for b in candidate_boards if b["description"] == short_descr]
+        matches = [b for b in candidate_boards if b.description == short_descr]
     if not matches:
         raise MPFlashError(f"No board info found for description '{descr}' or '{short_descr}'")
-    return sorted(matches, key=lambda x: x["version"])
-
-
-@functools.lru_cache(maxsize=20)
-def _read_board_info(board_info):
-    with open(board_info, "r") as file:
-        info = json.load(file)
-    return info
+    return sorted(matches, key=lambda x: x.version)
```

### Comparing `mpflash-0.7.7/mpflash/mpremoteboard/__init__.py` & `mpflash-0.8.0/mpflash/mpremoteboard/__init__.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/mpremoteboard/mpy_fw_info.py` & `mpflash-0.8.0/mpflash/mpremoteboard/mpy_fw_info.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/mpremoteboard/runner.py` & `mpflash-0.8.0/mpflash/mpremoteboard/runner.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/vendor/dfu.py` & `mpflash-0.8.0/mpflash/vendor/dfu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # sourcery skip: require-parameter-annotation
 # sourcery skip: replace-interpolation-with-fstring
+# type: ignore
 #!/usr/bin/python
 
 # Written by Antonio Galea - 2010/11/18
 # Distributed under Gnu LGPL 3.0
 # see http://www.gnu.org/licenses/lgpl-3.0.txt
 
 import os
```

### Comparing `mpflash-0.7.7/mpflash/vendor/pydfu.py` & `mpflash-0.8.0/mpflash/vendor/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.7/mpflash/vendor/versions.py` & `mpflash-0.8.0/mpflash/vendor/versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 """
 
 from functools import lru_cache
 
 from loguru import logger as log
 from packaging.version import parse
 
+from mpflash.common import GH_CLIENT
+
 V_PREVIEW = "preview"
 "Latest preview version"
 
 SET_PREVIEW = {"preview", "latest", "master"}
 
 
 def clean_version(
@@ -63,20 +65,20 @@
         version = "v" + version
     if version in SET_PREVIEW:
         version = V_PREVIEW
     return version
 
 
 @lru_cache(maxsize=10)
-def micropython_versions(minver: str = "v1.20"):
+def micropython_versions(minver: str = "v1.20", reverse: bool = False):
     """Get the list of micropython versions from github tags"""
     try:
         gh_client = GH_CLIENT
         repo = gh_client.get_repo("micropython/micropython")
-        versions = [tag.name for tag in repo.get_tags() if parse(tag.name) >= parse(minver)]
+        versions = [tag.name for tag in repo.get_tags()]
     except Exception:
         versions = [
             "v9.99.9-preview",
             "v1.22.2",
             "v1.22.1",
             "v1.22.0",
             "v1.21.1",
@@ -90,15 +92,17 @@
             "v1.15",
             "v1.14",
             "v1.13",
             "v1.12",
             "v1.11",
             "v1.10",
         ]
-        versions = [v for v in versions if parse(v) >= parse(minver)]
+    versions = [v for v in versions if parse(v) >= parse(minver)]
+    # remove all but the most recent (preview) version
+    versions = versions[:1] + [v for v in versions if "preview" not in v]
     return sorted(versions)
 
 
 def get_stable_mp_version() -> str:
     # read the versions from the git tags
     all_versions = micropython_versions(minver="v1.17")
     return [v for v in all_versions if not v.endswith(V_PREVIEW)][-1]
```

### Comparing `mpflash-0.7.7/mpflash/worklist.py` & `mpflash-0.8.0/mpflash/worklist.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 from loguru import logger as log
 
-from mpflash.common import FWInfo
+from mpflash.common import FWInfo, filtered_comports
 from mpflash.errors import MPFlashError
 
-from .config import config
 from .downloaded import find_downloaded_firmware
 from .list import show_mcus
 from .mpboard_id import find_known_board
 from .mpremoteboard import MPRemoteBoard
 
 # #########################################################################################################
 WorkList = List[Tuple[MPRemoteBoard, FWInfo]]
@@ -56,92 +55,116 @@
             log.error(f"No {target_version} firmware found for {mcu.board} on {mcu.serialport}.")
             continue
         if len(board_firmwares) > 1:
             log.debug(f"Multiple {target_version} firmwares found for {mcu.board} on {mcu.serialport}.")
 
         # just use the last firmware
         fw_info = board_firmwares[-1]
-        log.info(f"Found {target_version} firmware {fw_info['filename']} for {mcu.board} on {mcu.serialport}.")
+        log.info(f"Found {target_version} firmware {fw_info.filename} for {mcu.board} on {mcu.serialport}.")
         wl.append((mcu, fw_info))
     return wl
 
 
+def manual_worklist(
+    serial: str,
+    *,
+    board_id: str,
+    version: str,
+    fw_folder: Path,
+) -> WorkList:
+    """Create a worklist for a single board specified manually.
+
+    Args:
+        serial (str): Serial port of the board
+        board (str): Board_ID
+        version (str): Firmware version
+        fw_folder (Path): Path to the firmware folder
+
+    Returns:
+        WorkList: List of boards and firmware information to update
+    """
+    log.trace(f"Manual updating {serial} to {board_id} {version}")
+    mcu = MPRemoteBoard(serial)
+    # Lookup the matching port and cpu in board_info based in the board name
+    try:
+        info = find_known_board(board_id)
+        mcu.port = info.port
+        # need the CPU type for the esptool
+        mcu.cpu = info.cpu
+    except (LookupError, MPFlashError) as e:
+        log.error(f"Board {board_id} not found in board_info.zip")
+        log.exception(e)
+        return []
+    mcu.board = board_id
+    firmwares = find_downloaded_firmware(fw_folder=fw_folder, board_id=board_id, version=version, port=mcu.port)
+    if not firmwares:
+        log.error(f"No firmware found for {mcu.port} {board_id} version {version}")
+        return []
+    # use the most recent matching firmware
+    return [(mcu, firmwares[-1])]  # type: ignore
+
+
 def single_auto_worklist(
+    serial: str,
     *,
-    serial_port: str,
     version: str,
     fw_folder: Path,
 ) -> WorkList:
     """Create a worklist for a single serial-port.
 
     Args:
         serial_port (str): Serial port of the board
         version (str): Firmware version
         fw_folder (Path): Path to the firmware folder
 
     Returns:
         WorkList: List of boards and firmware information to update
     """
-    conn_boards = [MPRemoteBoard(serial_port)]
+    log.trace(f"Auto updating {serial} to {version}")
+    conn_boards = [MPRemoteBoard(serial)]
     todo = auto_update(conn_boards, version, fw_folder)  # type: ignore # List / list
     show_mcus(conn_boards)  # type: ignore
     return todo
 
 
-def full_auto_worklist(*, version: str, fw_folder: Path) -> WorkList:
+def full_auto_worklist(
+    all_boards: List[MPRemoteBoard], *, include: List[str], ignore: List[str], version: str, fw_folder: Path
+) -> WorkList:
     """
     Create a worklist for all connected micropython boards based on the information retrieved from the board.
     This allows the firmware version of one or moae boards to be changed without needing to specify the port or board_id manually.
 
     Args:
         version (str): Firmware version
         fw_folder (Path): Path to the firmware folder
 
     Returns:
         WorkList: List of boards and firmware information to update
     """
-    try:
-        conn_boards = [
-            MPRemoteBoard(sp, update=True) for sp in MPRemoteBoard.connected_boards() if sp not in config.ignore_ports
-        ]
-    except ConnectionError as e:
-        log.error(f"Error connecting to boards: {e}")
+    log.trace(f"Auto updating all boards to {version}")
+    if selected_boards := filter_boards(all_boards, include=include, ignore=ignore):
+        return auto_update(selected_boards, version, fw_folder)
+    else:
         return []
-    return auto_update(conn_boards, version, fw_folder)  # type: ignore
-
-
-def manual_worklist(
-    version: str,
-    fw_folder: Path,
-    serial_port: str,
-    board: str,
-    # port: str,
-) -> WorkList:
-    """Create a worklist for a single board specified manually.
 
-    Args:
-        version (str): Firmware version
-        fw_folder (Path): Path to the firmware folder
-        serial_port (str): Serial port of the board
-        board (str): Board name
 
-    Returns:
-        WorkList: List of boards and firmware information to update
-    """
-    mcu = MPRemoteBoard(serial_port)
-    # TODO : Find a way to avoid needing to specify the port
-    # Lookup the matching port and cpu in board_info based in the board name
+def filter_boards(
+    all_boards: List[MPRemoteBoard],
+    *,
+    include: List[str],
+    ignore: List[str],
+):
     try:
-        info = find_known_board(board)
-        mcu.port = info["port"]
-        # need the CPU type for the esptool
-        mcu.cpu = info["cpu"]
-    except (LookupError, MPFlashError) as e:
-        log.error(f"Board {board} not found in board_info.json")
-        return []
-    mcu.board = board
-    firmwares = find_downloaded_firmware(fw_folder=fw_folder, board_id=board, version=version, port=mcu.port)
-    if not firmwares:
-        log.error(f"No firmware found for {mcu.port} {board} version {version}")
+        comports = [
+            p.device
+            for p in filtered_comports(
+                ignore=ignore,
+                include=include,
+                bluetooth=False,
+            )
+        ]
+        selected_boards = [b for b in all_boards if b.serialport in comports]
+        # [MPRemoteBoard(port.device, update=True) for port in comports]
+    except ConnectionError as e:
+        log.error(f"Error connecting to boards: {e}")
         return []
-        # use the most recent matching firmware
-    return [(mcu, firmwares[-1])]  # type: ignore
+    return selected_boards  # type: ignore
```

### Comparing `mpflash-0.7.7/pyproject.toml` & `mpflash-0.8.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpflash"
-version = "0.7.7"
+version = "0.8.0"
 description = "Flash and download tool for MicroPython firmwares"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["MicroPython", "firmware", "flash", "download", "UF2", "esptool"]
 homepage = "https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md"
 repository = "https://github.com/Josverl/micropython-stubber"
@@ -14,46 +14,47 @@
     "Topic :: Software Development :: Build Tools",
 ]
 
 [tool.poetry.scripts]
 mpflash = "mpflash.cli_main:mpflash"
 
 [tool.poetry.dependencies]
-python =  ">=3.8.1,<4.0"
-requests = "^2.31.0"
 beautifulsoup4 = "^4.12.3"
-loguru = "^0.7.2"
+bincopy = "^20.0.0"
+blkinfo = "^0.2.0"
+cachetools = "^5.3.0"
 esptool = "^4.7.0"
+inquirer = "^3.2.4"
 jsonlines = "^4.0.0"
-bincopy = "^20.0.0"
-# strip-ansi = "^0.1.1"
-rich-click = "^1.7.3"
+jsons = "^1.6.3"
+libusb = {version = "^1.0.27", platform = "win32"}
+loguru = "^0.7.2"
+mpremote = "^1.22.0"
+packaging = "23.2"
+platformdirs = "^4.2.0"
 psutil = "^5.9.8"
-blkinfo = "^0.2.0"
 pygithub = "^2.1.1"
-platformdirs = "^4.2.0"
+python =  ">=3.8.1,<4.0"
 pyusb = "^1.2.1"
-packaging = "23.2"
+requests = "^2.31.0"
+rich-click = "^1.8.1"
 tenacity = "8.2.3"
-mpremote = "^1.22.0"
-inquirer = "^3.2.4"
-libusb = {version = "^1.0.27", platform = "win32"}
-jsons = "^1.6.3"
+
 
 [tool.poetry.group.test]
 optional = true
 [tool.poetry.group.test.dependencies]
-coverage = ">=6.4.3,<8.0.0"
 pytest = "^7.1.2"
 pytest-github-actions-annotate-failures = ">=0.1.7,<0.3.0"
 pytest-json-report = "^1.5.0"
 pytest-metadata = ">=2.0.2,<4.0.0"
 pytest-mock = "^3.10.0"
-mock = "^4.0.3"
+#
+coverage = ">=6.4.3,<8.0.0"
 distro = "^1.8.0"
 fasteners = "^0.19"
-jsons = "^1.6.3"
+mock = "^4.0.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mpflash-0.7.7/README.md` & `mpflash-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 # MPFLASH
+  [![pypi version](https://badgen.net/pypi/v/mpflash)](https://pypi.org/project/mpflash/)
+  [![python versions](https://badgen.net/pypi/python/mpflash)](https://badgen.net/pypi/python/mpflash)
+[![Downloads](https://static.pepy.tech/badge/mpflash)](https://pepy.tech/project/mpflash)
+
 
 `mpflash` is a command-line tool for working with MicroPython firmware. It provides features to help you flash and update Micropython on one or more .
 
-This tool was initially created to be used in a CI/CD pipeline to automate the process of downloading and flashing MicroPython firmware to multiple boards, but it has been extend with a TUI to me be used for manual downloadig, flashing and development.
+This tool was initially created to be used in a CI/CD pipeline to automate the process of downloading and flashing MicroPython firmware to multiple boards, but it has been extend with a TUI to be used for manual downloadig, flashing and development.
 
-`mpflash` has been tested on Windows x64, Linux X64, but not (yet) macOS.
-Tested ports: `rp2`, `samd`, `esp32`, `esp32s3`, `esp32c3`, `esp8266` and `stm32`
+`mpflash` has been tested on:  
+ - OS: Windows x64, Linux X64, but not (yet) macOS.
+ - Micropython (hardware) ports: 
+    - `rp2`, using `.uf2`, using filecopy (macos not tested yet)
+    - `samd`, using ` .uf2`, using filecopy (macos not tested yet)
+    - `esp32`, using `.bin`, using esptool,
+    - `esp8266`, using `.bin`, using esptool
+    - `stm32`, using ` .dfu`, using pydfu
 
+Not yet implemented: `nrf`, `cc3200`, `mimxrt`
+ 
 ## Features
  1. List the connected boards including their firmware details, in a tabular or json format
  2. Download MicroPython firmware for versions, and matching a specified board or matches your current attached board.
  3. Flash one or all connected MicroPython boards with a specific firmware or version.  
  
 ## Installation
 To install mpflash, you can use pip: `pip install mpflash`
@@ -30,16 +42,15 @@
 On Windows this will not be an issue, but on Linux you can use  udev rules to give non-root users access to the USB devices.
 [See the stm32_permissions documentation](./stm32_udev_rules.md) for more information.
 
 
 ## Detailed usage
 You can list the connected boards using the following command:
 ```bash
-$ mpflash list
-D:\MyPython\micropython-stubber> mpflash list
+$> mpflash list
                                                Connected boards
 ┏━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━┓
 ┃ Serial  ┃Family       ┃Port  ┃Board                                      ┃CPU     ┃Version          ┃build ┃
 ┡━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━┩
 │ COM21   │micropython  │rp2   │RPI_PICO                                   │RP2040  │v1.23.0-preview  │  236 │
 │         │             │      │Raspberry Pi Pico with RP2040              │        │                 │      │
 │ COM23   │micropython  │rp2   │RPI_PICO_W                                 │RP2040  │v1.23.0-preview  │  176 │
```

### Comparing `mpflash-0.7.7/PKG-INFO` & `mpflash-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpflash
-Version: 0.7.7
+Version: 0.8.0
 Summary: Flash and download tool for MicroPython firmwares
 Home-page: https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md
 License: MIT
 Keywords: MicroPython,firmware,flash,download,UF2,esptool
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -15,41 +15,54 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: bincopy (>=20.0.0,<21.0.0)
 Requires-Dist: blkinfo (>=0.2.0,<0.3.0)
+Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: esptool (>=4.7.0,<5.0.0)
 Requires-Dist: inquirer (>=3.2.4,<4.0.0)
 Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
 Requires-Dist: jsons (>=1.6.3,<2.0.0)
 Requires-Dist: libusb (>=1.0.27,<2.0.0) ; sys_platform == "win32"
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: mpremote (>=1.22.0,<2.0.0)
 Requires-Dist: packaging (==23.2)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pygithub (>=2.1.1,<3.0.0)
 Requires-Dist: pyusb (>=1.2.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich-click (>=1.7.3,<2.0.0)
+Requires-Dist: rich-click (>=1.8.1,<2.0.0)
 Requires-Dist: tenacity (==8.2.3)
 Project-URL: Repository, https://github.com/Josverl/micropython-stubber
 Description-Content-Type: text/markdown
 
 # MPFLASH
+  [![pypi version](https://badgen.net/pypi/v/mpflash)](https://pypi.org/project/mpflash/)
+  [![python versions](https://badgen.net/pypi/python/mpflash)](https://badgen.net/pypi/python/mpflash)
+[![Downloads](https://static.pepy.tech/badge/mpflash)](https://pepy.tech/project/mpflash)
+
 
 `mpflash` is a command-line tool for working with MicroPython firmware. It provides features to help you flash and update Micropython on one or more .
 
-This tool was initially created to be used in a CI/CD pipeline to automate the process of downloading and flashing MicroPython firmware to multiple boards, but it has been extend with a TUI to me be used for manual downloadig, flashing and development.
+This tool was initially created to be used in a CI/CD pipeline to automate the process of downloading and flashing MicroPython firmware to multiple boards, but it has been extend with a TUI to be used for manual downloadig, flashing and development.
 
-`mpflash` has been tested on Windows x64, Linux X64, but not (yet) macOS.
-Tested ports: `rp2`, `samd`, `esp32`, `esp32s3`, `esp32c3`, `esp8266` and `stm32`
+`mpflash` has been tested on:  
+ - OS: Windows x64, Linux X64, but not (yet) macOS.
+ - Micropython (hardware) ports: 
+    - `rp2`, using `.uf2`, using filecopy (macos not tested yet)
+    - `samd`, using ` .uf2`, using filecopy (macos not tested yet)
+    - `esp32`, using `.bin`, using esptool,
+    - `esp8266`, using `.bin`, using esptool
+    - `stm32`, using ` .dfu`, using pydfu
 
+Not yet implemented: `nrf`, `cc3200`, `mimxrt`
+ 
 ## Features
  1. List the connected boards including their firmware details, in a tabular or json format
  2. Download MicroPython firmware for versions, and matching a specified board or matches your current attached board.
  3. Flash one or all connected MicroPython boards with a specific firmware or version.  
  
 ## Installation
 To install mpflash, you can use pip: `pip install mpflash`
@@ -69,16 +82,15 @@
 On Windows this will not be an issue, but on Linux you can use  udev rules to give non-root users access to the USB devices.
 [See the stm32_permissions documentation](./stm32_udev_rules.md) for more information.
 
 
 ## Detailed usage
 You can list the connected boards using the following command:
 ```bash
-$ mpflash list
-D:\MyPython\micropython-stubber> mpflash list
+$> mpflash list
                                                Connected boards
 ┏━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━┓
 ┃ Serial  ┃Family       ┃Port  ┃Board                                      ┃CPU     ┃Version          ┃build ┃
 ┡━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━┩
 │ COM21   │micropython  │rp2   │RPI_PICO                                   │RP2040  │v1.23.0-preview  │  236 │
 │         │             │      │Raspberry Pi Pico with RP2040              │        │                 │      │
 │ COM23   │micropython  │rp2   │RPI_PICO_W                                 │RP2040  │v1.23.0-preview  │  176 │
```

