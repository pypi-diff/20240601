# Comparing `tmp/browserxt-0.1.2.tar.gz` & `tmp/browserxt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserxt-0.1.2.tar", last modified: Sat Jun  1 10:46:47 2024, max compression
+gzip compressed data, was "browserxt-0.1.4.tar", last modified: Sat Jun  1 12:53:39 2024, max compression
```

## Comparing `browserxt-0.1.2.tar` & `browserxt-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    16725 2024-06-01 10:46:30.857645 browserxt-0.1.2/LICENSE
--rw-r--r--   0        0        0     3035 2024-06-01 10:46:30.857645 browserxt-0.1.2/README.md
--rw-r--r--   0        0        0     2296 2024-06-01 10:46:47.317644 browserxt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       72 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/__init__.py
--rwxr-xr-x   0        0        0     3125 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/browser.py
--rw-r--r--   0        0        0     1197 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/cli.py
--rw-r--r--   0        0        0        0 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/py.typed
--rw-r--r--   0        0        0     4537 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/scripts/detect_browsers.ps1
--rw-r--r--   0        0        0     1024 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/settings.py
--rwxr-xr-x   0        0        0    10254 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/utils.py
--rw-r--r--   0        0        0       25 2024-06-01 10:46:30.861645 browserxt-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      448 2024-06-01 10:46:30.861645 browserxt-0.1.2/tests/cli_test.py
--rw-r--r--   0        0        0      136 2024-06-01 10:46:30.861645 browserxt-0.1.2/tests/pkg_test.py
--rw-r--r--   0        0        0      338 2024-06-01 10:46:30.861645 browserxt-0.1.2/tests/settings_test.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 browserxt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-06-01 12:53:19.649266 browserxt-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3035 2024-06-01 12:53:19.649266 browserxt-0.1.4/README.md
+-rw-r--r--   0        0        0     2296 2024-06-01 12:53:39.477321 browserxt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-06-01 12:53:19.653266 browserxt-0.1.4/src/browserxt/__init__.py
+-rwxr-xr-x   0        0        0     4823 2024-06-01 12:53:19.653266 browserxt-0.1.4/src/browserxt/browser.py
+-rw-r--r--   0        0        0     1324 2024-06-01 12:53:19.653266 browserxt-0.1.4/src/browserxt/cli.py
+-rw-r--r--   0        0        0        0 2024-06-01 12:53:19.653266 browserxt-0.1.4/src/browserxt/py.typed
+-rw-r--r--   0        0        0     4946 2024-06-01 12:53:19.653266 browserxt-0.1.4/src/browserxt/scripts/detect_browsers.ps1
+-rw-r--r--   0        0        0     1024 2024-06-01 12:53:19.653266 browserxt-0.1.4/src/browserxt/settings.py
+-rwxr-xr-x   0        0        0    10912 2024-06-01 12:53:19.653266 browserxt-0.1.4/src/browserxt/utils.py
+-rw-r--r--   0        0        0       25 2024-06-01 12:53:19.653266 browserxt-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      448 2024-06-01 12:53:19.653266 browserxt-0.1.4/tests/cli_test.py
+-rw-r--r--   0        0        0      136 2024-06-01 12:53:19.653266 browserxt-0.1.4/tests/pkg_test.py
+-rw-r--r--   0        0        0      338 2024-06-01 12:53:19.653266 browserxt-0.1.4/tests/settings_test.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 browserxt-0.1.4/PKG-INFO
```

### Comparing `browserxt-0.1.2/LICENSE` & `browserxt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.2/README.md` & `browserxt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.2/pyproject.toml` & `browserxt-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "full-development-lifecycle",
     "project-template",
     "serious-scaffold",
 ]
 name = "browserxt"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.1.2"
+version = "0.1.4"
 
 [project.license]
 text = "MPL-2.0"
 
 [project.scripts]
 browserxt = "browserxt.cli:app"
```

### Comparing `browserxt-0.1.2/src/browserxt/cli.py` & `browserxt-0.1.4/src/browserxt/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,22 +20,25 @@
     ),
     use_wsl: bool = Option(
         False,
         "--wsl",
         help="Force use of WSL browsers (X11 required)",
         hidden=not is_running_in_wsl(),
     ),
+    ignore_default: bool = Option(
+        False, "--ignore-default", help="Ignore the default browser"
+    ),
     url: str = Argument(..., help="URL to open in the browser"),
     options: list[str] = Argument(
         default=None,
         help="Additional browser options, e.g. `--incognito` for Chrome or `--private-window` for Firefox",
     ),
 ) -> None:
     """Open a browser with specified positional arguments as options."""
-    _browser = Browser(browser_list or [], options or [], use_wsl)
+    _browser = Browser(browser_list or [], options or [], use_wsl, ignore_default)
     if not _browser.open(url):
         raise Exception("No browser detected")
 
 
 typer_click_object = typer_main.get_command(app)
 
 if __name__ == "__main__":
```

### Comparing `browserxt-0.1.2/src/browserxt/scripts/detect_browsers.ps1` & `browserxt-0.1.4/src/browserxt/scripts/detect_browsers.ps1`

 * *Files 8% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 $bravePossiblePaths = @(
     "$env:ProgramFiles\BraveSoftware\Brave-Browser\Application\brave.exe",
     "$env:ProgramFiles (x86)\BraveSoftware\Brave-Browser\Application\brave.exe",
     "$env:LocalAppData\BraveSoftware\Brave-Browser\Application\brave.exe"
 )
 
 $operaPossiblePaths = @(
-    "$env:ProgramFiles\Opera\launcher.exe",
-    "$env:ProgramFiles (x86)\Opera\launcher.exe",
-    "$env:LocalAppData\Programs\Opera\launcher.exe"
+    "$env:ProgramFiles\Opera\opera.exe",
+    "$env:ProgramFiles (x86)\Opera\opera.exe",
+    "$env:LocalAppData\Programs\Opera\opera.exe"
 )
 
 function Find-BrowserPath {
     param (
         [string[]]$registryPaths,
         [string[]]$possiblePaths
     )
@@ -103,39 +103,49 @@
 
 $browsers = @{}
 $defaultBrowser = Get-DefaultBrowser
 
 # Find Chrome paths
 $chromePaths = Find-BrowserPath -registryPaths $chromeRegistryPaths -possiblePaths $chromePossiblePaths
 if ($chromePaths.Count -gt 0) {
-    $browsers["chrome"] = $chromePaths
+    $browsers["chrome"] = @{}
+    $browsers["chrome"]["path"] = $chromePaths
+    $browsers["chrome"]["family"] = "chromium"
 }
 
 # Find Firefox paths
 $firefoxPaths = Find-BrowserPath -registryPaths $firefoxRegistryPaths -possiblePaths $firefoxPossiblePaths
 if ($firefoxPaths.Count -gt 0) {
-    $browsers["firefox"] = $firefoxPaths
+    $browsers["firefox"] = @{}
+    $browsers["firefox"]["path"] = $firefoxPaths
+    $browsers["firefox"]["family"] = "firefox"
 }
 
 # Find Edge paths
 $edgePaths = Find-BrowserPath -registryPaths $edgeRegistryPaths -possiblePaths $edgePossiblePaths
 if ($edgePaths.Count -gt 0) {
-    $browsers["edge"] = $edgePaths
+    $browsers["edge"] = @{}
+    $browsers["edge"]["path"] = $edgePaths
+    $browsers["edge"]["family"] = "chromium"
 }
 
 # Find Brave paths
 $bravePaths = Find-BrowserPath -registryPaths $braveRegistryPaths -possiblePaths $bravePossiblePaths
 if ($bravePaths.Count -gt 0) {
-    $browsers["brave"] = $bravePaths
+    $browsers["brave"] = @{}
+    $browsers["brave"]["path"] = $bravePaths
+    $browsers["brave"]["family"] = "chromium"
 }
 
 # Find Opera paths
 $operaPaths = Find-BrowserPath -registryPaths $operaRegistryPaths -possiblePaths $operaPossiblePaths
 if ($operaPaths.Count -gt 0) {
-    $browsers["opera"] = $operaPaths
+    $browsers["opera"] = @{}
+    $browsers["opera"]["path"] = $operaPaths
+    $browsers["opera"]["family"] = "chromium"
 }
 
 # Add default browser to the output
 $output = @{
     default = $defaultBrowser
     browsers = $browsers
 }
```

### Comparing `browserxt-0.1.2/src/browserxt/settings.py` & `browserxt-0.1.4/src/browserxt/settings.py`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.2/src/browserxt/utils.py` & `browserxt-0.1.4/src/browserxt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,41 +2,62 @@
 import sys
 import json
 import shutil
 import platform
 import subprocess
 import configparser
 
-
-POSIX_BROWSER_PATHS = {
-    "chrome": [
-        "google-chrome",
-        "google-chrome-stable",
-        "chrome",
-        "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
-    ],
-    "firefox": ["firefox", "/Applications/Firefox.app/Contents/MacOS/firefox"],
-    "chromium": [
-        "chromium",
-        "chromium-browser",
-        "/Applications/Chromium.app/Contents/MacOS/Chromium",
-    ],
-    "opera": ["opera", "/Applications/Opera.app/Contents/MacOS/Opera"],
-    "brave": [
-        "brave",
-        "brave-browser",
-        "/Applications/Brave Browser.app/Contents/MacOS/Brave Browser",
-    ],
-    "edge": [
-        "microsoft-edge",
-        "microsoft-edge-stable",
-        "edge",
-        "msedge",
-        "/Applications/Microsoft Edge.app/Contents/MacOS/Microsoft Edge",
-    ],
+POSIX_BROWSERS = {
+    "chrome": {
+        "paths": [
+            "google-chrome",
+            "google-chrome-stable",
+            "chrome",
+            "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
+        ],
+        "family": "chromium",
+    },
+    "firefox": {
+        "paths": [
+            "firefox",
+            "firefox-bin",
+            "/Applications/Firefox.app/Contents/MacOS/firefox",
+        ],
+        "family": "firefox",
+    },
+    "chromium": {
+        "paths": [
+            "chromium",
+            "chromium-browser",
+            "/Applications/Chromium.app/Contents/MacOS/Chromium",
+        ],
+        "family": "chromium",
+    },
+    "opera": {
+        "paths": ["opera", "/Applications/Opera.app/Contents/MacOS/Opera"],
+        "family": "chromium",
+    },
+    "brave": {
+        "paths": [
+            "brave",
+            "brave-browser",
+            "/Applications/Brave Browser.app/Contents/MacOS/Brave Browser",
+        ],
+        "family": "chromium",
+    },
+    "edge": {
+        "paths": [
+            "microsoft-edge",
+            "microsoft-edge-stable",
+            "edge",
+            "msedge",
+            "/Applications/Microsoft Edge.app/Contents/MacOS/Microsoft Edge",
+        ],
+        "family": "chromium",
+    },
 }
 
 
 def get_posix_default_browser() -> str | None:
     # Check xdg-settings (Linux)
     try:
         result = subprocess.run(
@@ -230,49 +251,51 @@
 
     return None
 
 
 def get_posix_browser_name(path: str | None) -> str:
     if not path:
         return ""
-    for browser_type, binaries in POSIX_BROWSER_PATHS.items():
-        for binary in binaries:
+    for name, browser in POSIX_BROWSERS.items():
+        for binary in browser.get("paths", []):
             if binary in path:
-                return browser_type
+                return name
     return ""
 
 
 def get_default_from_env_vars() -> str:
     browser = os.getenv("BROWSER") or os.getenv("DEFAULT_BROWSER")
     if browser:
         return browser
     return ""
 
 
 # Function to check if a browser is installed and map its name
-def detect_posix() -> tuple[str, dict[str, str]]:
-    installed_browsers = {}
-    for name, binaries in POSIX_BROWSER_PATHS.items():
-        for binary in binaries:
+def detect_posix() -> tuple[str, dict[str, dict[str, str]]]:
+    installed_browsers: dict[str, dict[str, str]] = {}
+    for name, browser in POSIX_BROWSERS.items():
+        for binary in browser.get("paths", []):
             path = shutil.which(binary)
             if path:
-                installed_browsers[name] = path
+                installed_browsers[name] = {}
+                installed_browsers[name]["path"] = path
+                installed_browsers[name]["family"] = str(browser.get("family", ""))
                 break  # Stop at the first detected binary for a browser
 
     default_browser = get_default_from_env_vars()
     if default_browser in installed_browsers:
         return default_browser, installed_browsers
 
     default_browser = get_posix_browser_name(
         get_binary_path_from_desktop_entry(get_posix_default_browser())
     )
     return default_browser, installed_browsers
 
 
-def detect_nt() -> tuple[str, dict[str, str]]:
+def detect_nt() -> tuple[str, dict[str, dict[str, str]]]:
     # Path to the PowerShell script
     powershell_script_path = os.path.join(
         os.path.dirname(__file__), "scripts/detect_browsers.ps1"
     )
     try:
         # Run the PowerShell script
         result = subprocess.run(
```

### Comparing `browserxt-0.1.2/PKG-INFO` & `browserxt-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserxt
-Version: 0.1.2
+Version: 0.1.4
 Summary: A simple extensible browser runner
 Keywords: copier-template,full-development-lifecycle,project-template,serious-scaffold
 Author-Email: Nick Syntychakis <nsyntych@punkops.dev>
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

