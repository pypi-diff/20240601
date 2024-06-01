# Comparing `tmp/mobase-stubs-2.5.0.dev8.tar.gz` & `tmp/mobase-stubs-2.5.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobase-stubs-2.5.0.dev8.tar", last modified: Thu May  5 16:27:33 2022, max compression
+gzip compressed data, was "mobase-stubs-2.5.0.dev9.tar", last modified: Sat May  7 12:00:14 2022, max compression
```

## Comparing `mobase-stubs-2.5.0.dev8.tar` & `mobase-stubs-2.5.0.dev9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 16:27:33.886835 mobase-stubs-2.5.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-05 16:27:26.000000 mobase-stubs-2.5.0.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-05-05 16:27:33.886835 mobase-stubs-2.5.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-05-05 16:27:26.000000 mobase-stubs-2.5.0.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 16:27:33.886835 mobase-stubs-2.5.0.dev8/mobase-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)   150325 2022-05-05 16:27:33.000000 mobase-stubs-2.5.0.dev8/mobase-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 16:27:33.886835 mobase-stubs-2.5.0.dev8/mobase-stubs/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-05-05 16:27:33.000000 mobase-stubs-2.5.0.dev8/mobase-stubs/widgets/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 16:27:33.886835 mobase-stubs-2.5.0.dev8/mobase_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-05-05 16:27:33.000000 mobase-stubs-2.5.0.dev8/mobase_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-05-05 16:27:33.000000 mobase-stubs-2.5.0.dev8/mobase_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 16:27:33.000000 mobase-stubs-2.5.0.dev8/mobase_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-05 16:27:33.000000 mobase-stubs-2.5.0.dev8/mobase_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-05 16:27:33.886835 mobase-stubs-2.5.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-05-05 16:27:26.000000 mobase-stubs-2.5.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 12:00:14.947543 mobase-stubs-2.5.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-07 11:59:58.000000 mobase-stubs-2.5.0.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-05-07 12:00:14.947543 mobase-stubs-2.5.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2022-05-07 11:59:58.000000 mobase-stubs-2.5.0.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 12:00:14.947543 mobase-stubs-2.5.0.dev9/mobase-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)   151071 2022-05-07 12:00:13.000000 mobase-stubs-2.5.0.dev9/mobase-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 12:00:14.947543 mobase-stubs-2.5.0.dev9/mobase-stubs/widgets/
+-rw-r--r--   0 runner    (1001) docker     (121)     5010 2022-05-07 12:00:13.000000 mobase-stubs-2.5.0.dev9/mobase-stubs/widgets/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 12:00:14.947543 mobase-stubs-2.5.0.dev9/mobase_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-05-07 12:00:14.000000 mobase-stubs-2.5.0.dev9/mobase_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-05-07 12:00:14.000000 mobase-stubs-2.5.0.dev9/mobase_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-07 12:00:14.000000 mobase-stubs-2.5.0.dev9/mobase_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-07 12:00:14.000000 mobase-stubs-2.5.0.dev9/mobase_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-07 12:00:14.947543 mobase-stubs-2.5.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-05-07 11:59:58.000000 mobase-stubs-2.5.0.dev9/setup.py
```

### Comparing `mobase-stubs-2.5.0.dev8/LICENSE` & `mobase-stubs-2.5.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `mobase-stubs-2.5.0.dev8/PKG-INFO` & `mobase-stubs-2.5.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobase-stubs
-Version: 2.5.0.dev8
+Version: 2.5.0.dev9
 Summary: PEP561 stub files for the mobase python API
 Home-page: https://github.com/ModOrganizer2/mo2-pystubs-generation
 Author: Holt59
 Author-email: capelle.mikael@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mobase-stubs-2.5.0.dev8/README.md` & `mobase-stubs-2.5.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `mobase-stubs-2.5.0.dev8/mobase-stubs/__init__.pyi` & `mobase-stubs-2.5.0.dev9/mobase-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
-__version__ = "v2.5.0.dev8"
+__version__ = "v2.5.0.dev9"
 
 import abc
+import os
 from enum import Enum
-from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Optional,
@@ -21,44 +21,46 @@
     overload,
 )
 
 import PyQt6.QtCore
 import PyQt6.QtGui
 import PyQt6.QtWidgets
 
-MoVariant = Union[None, bool, int, str, list[Any], dict[str, Any]]
-FileWrapper = Union[str, PyQt6.QtCore.QFileInfo, Path]
-DirectoryWrapper = Union[str, PyQt6.QtCore.QDir, Path]
 GameFeatureType = TypeVar("GameFeatureType")
+MoVariant = None | bool | int | str | list[object] | dict[str, object]
 
-def getFileVersion(filepath: FileWrapper) -> str:
+def getFileVersion(filepath: Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]) -> str:
     """
     Retrieve the file version of the given executable.
 
     Args:
         filepath: Absolute path to the executable.
 
     Returns:
         The file version, or an empty string if the file version could not be retrieved.
     """
     ...
 
-def getIconForExecutable(executable: FileWrapper) -> PyQt6.QtGui.QIcon:
+def getIconForExecutable(
+    executable: Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]
+) -> PyQt6.QtGui.QIcon:
     """
     Retrieve the icon of an executable. Currently this always extracts the biggest icon.
 
     Args:
         executable: Absolute path to the executable.
 
     Returns:
         The icon for this executable, if any.
     """
     ...
 
-def getProductVersion(executable: FileWrapper) -> str:
+def getProductVersion(
+    executable: Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]
+) -> str:
     """
     Retrieve the product version of the given executable.
 
     Args:
         executable: Absolute path to the executable.
 
     Returns:
@@ -339,26 +341,30 @@
         self: ExecutableForcedLoadSetting, enabled: bool
     ) -> ExecutableForcedLoadSetting: ...
     def withForced(
         self: ExecutableForcedLoadSetting, forced: bool
     ) -> ExecutableForcedLoadSetting: ...
 
 class ExecutableInfo:
-    def __init__(self: ExecutableInfo, title: str, binary: FileWrapper): ...
+    def __init__(
+        self: ExecutableInfo,
+        title: str,
+        binary: Union[str, os.PathLike, PyQt6.QtCore.QFileInfo],
+    ): ...
     def arguments(self: ExecutableInfo) -> Sequence[str]: ...
     def asCustom(self: ExecutableInfo) -> ExecutableInfo: ...
     def binary(self: ExecutableInfo) -> PyQt6.QtCore.QFileInfo: ...
     def isCustom(self: ExecutableInfo) -> bool: ...
     def isValid(self: ExecutableInfo) -> bool: ...
     def steamAppID(self: ExecutableInfo) -> str: ...
     def title(self: ExecutableInfo) -> str: ...
     def withArgument(self: ExecutableInfo, argument: str) -> ExecutableInfo: ...
     def withSteamAppId(self: ExecutableInfo, app_id: str) -> ExecutableInfo: ...
     def withWorkingDirectory(
-        self: ExecutableInfo, directory: DirectoryWrapper
+        self: ExecutableInfo, directory: Union[str, os.PathLike, PyQt6.QtCore.QDir]
     ) -> ExecutableInfo: ...
     def workingDirectory(self: ExecutableInfo) -> PyQt6.QtCore.QDir: ...
 
 class FileInfo:
     """
     Information about a virtualized file
     """
@@ -1276,15 +1282,15 @@
         Returns:
             The extensions of archives supported by this installation manager.
         """
         ...
     def installArchive(
         self: IInstallationManager,
         mod_name: GuessedString,
-        archive: FileWrapper,
+        archive: Union[str, os.PathLike, PyQt6.QtCore.QFileInfo],
         mod_id: int = 0,
     ) -> Tuple[InstallResult, str, int]:
         """
         Install the given archive.
 
         Args:
             mod_name: Suggested name of the mod.
@@ -1941,60 +1947,66 @@
     def downloadsPath(self: IOrganizer) -> str:
         """
         Returns:
             The absolute path to the download directory.
         """
         ...
     def findFileInfos(
-        self: IOrganizer, path: DirectoryWrapper, filter: Callable[[FileInfo], bool]
+        self: IOrganizer,
+        path: Union[str, os.PathLike, PyQt6.QtCore.QDir],
+        filter: Callable[[FileInfo], bool],
     ) -> Sequence[FileInfo]:
         """
         Find files in the virtual directory matching the specified filter.
 
         Args:
             path: The path to search in (relative to the 'data' folder).
             filter: The function to use to filter files. Should return True for the files to keep.
 
         Returns:
             The list of `QFileInfo` corresponding to the matching files.
         """
         ...
     @overload
     def findFiles(
-        self: IOrganizer, path: DirectoryWrapper, filter: Callable[[str], bool]
+        self: IOrganizer,
+        path: Union[str, os.PathLike, PyQt6.QtCore.QDir],
+        filter: Callable[[str], bool],
     ) -> Sequence[str]:
         """
         Find files in the given folder that matches the given filter.
 
         Args:
             path: The path to search in (relative to the 'data' folder).
             filter: The function to use to filter files. Should return True for the files to keep.
 
         Returns:
             The list of matching files.
         """
         ...
     @overload
     def findFiles(
-        self: IOrganizer, path: DirectoryWrapper, patterns: Sequence[str]
+        self: IOrganizer,
+        path: Union[str, os.PathLike, PyQt6.QtCore.QDir],
+        patterns: Sequence[str],
     ) -> Sequence[str]:
         """
         Find files in the given folder that matches one of the given glob patterns.
 
         Args:
             path: The path to search in (relative to the 'data' folder).
             patterns: List of glob patterns to match against.
 
         Returns:
             The list of matching files.
         """
         ...
     @overload
     def findFiles(
-        self: IOrganizer, path: DirectoryWrapper, pattern: str
+        self: IOrganizer, path: Union[str, os.PathLike, PyQt6.QtCore.QDir], pattern: str
     ) -> Sequence[str]:
         """
         Find files in the given folder that matches the given glob pattern.
 
         Args:
             path: The path to search in (relative to the 'data' folder).
             pattern: The glob pattern to use to filter files.
@@ -2032,15 +2044,17 @@
     def getPluginDataPath() -> str:
         """
         Returns:
             The directory for plugin data, typically plugins/data.
         """
         ...
     def installMod(
-        self: IOrganizer, filename: FileWrapper, name_suggestion: str = ""
+        self: IOrganizer,
+        filename: Union[str, os.PathLike, PyQt6.QtCore.QFileInfo],
+        name_suggestion: str = "",
     ) -> IModInterface:
         """
         Install a mod archive at the specified location.
 
         Args:
             filename: Absolute filepath to the archive to install.
             name_suggestion: Suggested name for this mod. This can still be changed by the user.
@@ -2346,15 +2360,17 @@
         The main part of the refresh of the mods file structure, mod list and plugin list is done
         asynchronously, so you should not expect them to be up-to-date when this function returns.
 
         Args:
             save_changes: If True, the relevant profile information is saved first (enabled mods and order of mods).
         """
         ...
-    def resolvePath(self: IOrganizer, filename: FileWrapper) -> str:
+    def resolvePath(
+        self: IOrganizer, filename: Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]
+    ) -> str:
         """
         Resolves a path relative to the virtual data directory to its absolute real path.
 
         Args:
             filename: Path to resolve.
 
         Returns:
@@ -2394,17 +2410,17 @@
                 really good reason to access data of another mod AND if you can verify that plugin is actually installed.
             key: Identifier of the setting.
             value: New value for the setting.
         """
         ...
     def startApplication(
         self: IOrganizer,
-        executable: FileWrapper,
+        executable: Union[str, os.PathLike, PyQt6.QtCore.QFileInfo],
         args: Sequence[str] = [],
-        cwd: DirectoryWrapper = "",
+        cwd: Union[str, os.PathLike, PyQt6.QtCore.QDir] = "",
         profile: str = "",
         forcedCustomOverwrite: str = "",
         ignoreCustomOverwrite: bool = False,
     ) -> int:
         """
         Starts an application with virtual filesystem active.
 
@@ -3706,15 +3722,17 @@
 
 class ISaveGame:
     """
     Base class for information about what is in a save game.
     """
 
     def __init__(self: ISaveGame): ...
-    def allFiles(self: ISaveGame) -> Sequence[str]:
+    def allFiles(
+        self: ISaveGame,
+    ) -> Sequence[Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]]:
         """
         Returns:
             The list of all files related to this save.
         """
         ...
     def getCreationTime(self: ISaveGame) -> PyQt6.QtCore.QDateTime:
         """
@@ -3723,15 +3741,15 @@
         The creation time of a save is not always the same as the creation time of
         the file containing the save.
 
         Returns:
             The creation time of the save.
         """
         ...
-    def getFilepath(self: ISaveGame) -> str:
+    def getFilepath(self: ISaveGame) -> Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]:
         """
         Returns:
             The path name to the (main) file or folder for the save.
         """
         ...
     def getName(self: ISaveGame) -> str:
         """
@@ -4231,28 +4249,21 @@
             A SaveGameInfoWidget to display information about save game.
         """
         ...
 
 class ScriptExtender(abc.ABC):
     def __init__(self: ScriptExtender): ...
     @abc.abstractmethod
-    def BinaryName(self: ScriptExtender) -> str:
+    def binaryName(self: ScriptExtender) -> str:
         """
         Returns:
             The name of the script extender binary.
         """
         ...
     @abc.abstractmethod
-    def PluginPath(self: ScriptExtender) -> str:
-        """
-        Returns:
-            The script extender plugin path, relative to the data folder.
-        """
-        ...
-    @abc.abstractmethod
     def getArch(self: ScriptExtender) -> int:
         """
         Returns:
             The CPU platform of the extender.
         """
         ...
     @abc.abstractmethod
@@ -4273,21 +4284,30 @@
     def loaderName(self: ScriptExtender) -> str:
         """
         Returns:
             The loader to use to ensure the game runs with the script extender.
         """
         ...
     @abc.abstractmethod
-    def loaderPath(self: ScriptExtender) -> str:
+    def loaderPath(
+        self: ScriptExtender,
+    ) -> Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]:
         """
         Returns:
             The full path to the script extender loader.
         """
         ...
     @abc.abstractmethod
+    def pluginPath(self: ScriptExtender) -> Union[str, os.PathLike, PyQt6.QtCore.QDir]:
+        """
+        Returns:
+            The script extender plugin path, relative to the data folder.
+        """
+        ...
+    @abc.abstractmethod
     def savegameExtension(self: ScriptExtender) -> str:
         """
         Retrieve the extension of script extender save files.
 
         Returns:
             The extension of script extender save files (e.g. "skse").
         """
@@ -4316,30 +4336,34 @@
             official_only: Retrieve only unmanaged official mods.
 
         Returns:
             The list of unmanaged mods (internal names).
         """
         ...
     @abc.abstractmethod
-    def referenceFile(self: UnmanagedMods, mod_name: str) -> PyQt6.QtCore.QFileInfo:
+    def referenceFile(
+        self: UnmanagedMods, mod_name: str
+    ) -> Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]:
         """
         Retrieve the reference file for the requested mod.
 
         Example: For Bethesda games, the reference file may be the main
         plugin (esp or esm) for the game or a DLCs.
 
         Args:
             mod_name: Internal name of the mod.
 
         Returns:
             The reference file (absolute path) for the requested mod.
         """
         ...
     @abc.abstractmethod
-    def secondaryFiles(self: UnmanagedMods, mod_name: str) -> Sequence[str]:
+    def secondaryFiles(
+        self: UnmanagedMods, mod_name: str
+    ) -> Sequence[Union[str, os.PathLike, PyQt6.QtCore.QFileInfo]]:
         """
         Retrieve the secondary files for the requested mod.
 
         Example: For Bethesda games, the secondary files may be the archives
         corresponding to the reference file.
 
         Args:
```

### Comparing `mobase-stubs-2.5.0.dev8/mobase_stubs.egg-info/PKG-INFO` & `mobase-stubs-2.5.0.dev9/mobase_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobase-stubs
-Version: 2.5.0.dev8
+Version: 2.5.0.dev9
 Summary: PEP561 stub files for the mobase python API
 Home-page: https://github.com/ModOrganizer2/mo2-pystubs-generation
 Author: Holt59
 Author-email: capelle.mikael@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mobase-stubs-2.5.0.dev8/setup.py` & `mobase-stubs-2.5.0.dev9/setup.py`

 * *Files identical despite different names*

