# Comparing `tmp/browserxt-0.1.0.tar.gz` & `tmp/browserxt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserxt-0.1.0.tar", last modified: Thu May 30 08:51:22 2024, max compression
+gzip compressed data, was "browserxt-0.1.2.tar", last modified: Sat Jun  1 10:46:47 2024, max compression
```

## Comparing `browserxt-0.1.0.tar` & `browserxt-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    16725 2024-05-30 08:51:07.331211 browserxt-0.1.0/LICENSE
--rw-r--r--   0        0        0     3035 2024-05-30 08:51:07.331211 browserxt-0.1.0/README.md
--rw-r--r--   0        0        0     2296 2024-05-30 08:51:22.431346 browserxt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       72 2024-05-30 08:51:07.335211 browserxt-0.1.0/src/browserxt/__init__.py
--rwxr-xr-x   0        0        0     4677 2024-05-30 08:51:07.335211 browserxt-0.1.0/src/browserxt/browser.py
--rw-r--r--   0        0        0     1124 2024-05-30 08:51:07.335211 browserxt-0.1.0/src/browserxt/cli.py
--rw-r--r--   0        0        0        0 2024-05-30 08:51:07.335211 browserxt-0.1.0/src/browserxt/py.typed
--rw-r--r--   0        0        0     1024 2024-05-30 08:51:07.335211 browserxt-0.1.0/src/browserxt/settings.py
--rwxr-xr-x   0        0        0      589 2024-05-30 08:51:07.339211 browserxt-0.1.0/src/browserxt/utils.py
--rw-r--r--   0        0        0       25 2024-05-30 08:51:07.339211 browserxt-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      448 2024-05-30 08:51:07.339211 browserxt-0.1.0/tests/cli_test.py
--rw-r--r--   0        0        0      136 2024-05-30 08:51:07.339211 browserxt-0.1.0/tests/pkg_test.py
--rw-r--r--   0        0        0      338 2024-05-30 08:51:07.339211 browserxt-0.1.0/tests/settings_test.py
--rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 browserxt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-06-01 10:46:30.857645 browserxt-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3035 2024-06-01 10:46:30.857645 browserxt-0.1.2/README.md
+-rw-r--r--   0        0        0     2296 2024-06-01 10:46:47.317644 browserxt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/__init__.py
+-rwxr-xr-x   0        0        0     3125 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/browser.py
+-rw-r--r--   0        0        0     1197 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/cli.py
+-rw-r--r--   0        0        0        0 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/py.typed
+-rw-r--r--   0        0        0     4537 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/scripts/detect_browsers.ps1
+-rw-r--r--   0        0        0     1024 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/settings.py
+-rwxr-xr-x   0        0        0    10254 2024-06-01 10:46:30.861645 browserxt-0.1.2/src/browserxt/utils.py
+-rw-r--r--   0        0        0       25 2024-06-01 10:46:30.861645 browserxt-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      448 2024-06-01 10:46:30.861645 browserxt-0.1.2/tests/cli_test.py
+-rw-r--r--   0        0        0      136 2024-06-01 10:46:30.861645 browserxt-0.1.2/tests/pkg_test.py
+-rw-r--r--   0        0        0      338 2024-06-01 10:46:30.861645 browserxt-0.1.2/tests/settings_test.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 browserxt-0.1.2/PKG-INFO
```

### Comparing `browserxt-0.1.0/LICENSE` & `browserxt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.0/README.md` & `browserxt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.0/pyproject.toml` & `browserxt-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "full-development-lifecycle",
     "project-template",
     "serious-scaffold",
 ]
 name = "browserxt"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.1.0"
+version = "0.1.2"
 
 [project.license]
 text = "MPL-2.0"
 
 [project.scripts]
 browserxt = "browserxt.cli:app"
```

### Comparing `browserxt-0.1.0/src/browserxt/cli.py` & `browserxt-0.1.2/src/browserxt/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,35 @@
 
 
 @app.command(
     no_args_is_help=True,
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
 )
 def main(
-    browser: list[str] = Option(
+    browser_list: list[str] = Option(
         None,
         "--browser",
         "-b",
         help="Specify the browser(s) to try use in preference order",
     ),
-    wsl: bool = Option(
+    use_wsl: bool = Option(
         False,
         "--wsl",
         help="Force use of WSL browsers (X11 required)",
         hidden=not is_running_in_wsl(),
     ),
     url: str = Argument(..., help="URL to open in the browser"),
     options: list[str] = Argument(
         default=None,
         help="Additional browser options, e.g. `--incognito` for Chrome or `--private-window` for Firefox",
     ),
 ) -> None:
     """Open a browser with specified positional arguments as options."""
-    _browser = Browser(browser or [], options or [], wsl)
-    _browser.open(url)
+    _browser = Browser(browser_list or [], options or [], use_wsl)
+    if not _browser.open(url):
+        raise Exception("No browser detected")
 
 
 typer_click_object = typer_main.get_command(app)
 
 if __name__ == "__main__":
     app()
```

### Comparing `browserxt-0.1.0/src/browserxt/settings.py` & `browserxt-0.1.2/src/browserxt/settings.py`

 * *Files identical despite different names*

### Comparing `browserxt-0.1.0/PKG-INFO` & `browserxt-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserxt
-Version: 0.1.0
+Version: 0.1.2
 Summary: A simple extensible browser runner
 Keywords: copier-template,full-development-lifecycle,project-template,serious-scaffold
 Author-Email: Nick Syntychakis <nsyntych@punkops.dev>
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

