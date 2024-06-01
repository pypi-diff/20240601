# Comparing `tmp/fs_dropboxfs-1.0.2.tar.gz` & `tmp/fs_dropboxfs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_dropboxfs-1.0.2.tar", max compression
+gzip compressed data, was "fs_dropboxfs-1.0.3.tar", max compression
```

## Comparing `fs_dropboxfs-1.0.2.tar` & `fs_dropboxfs-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2022-11-26 02:07:10.069629 fs_dropboxfs-1.0.2/LICENSE
--rw-r--r--   0        0        0     1266 2023-11-20 05:31:26.424923 fs_dropboxfs-1.0.2/README.md
--rw-r--r--   0        0        0      184 2023-09-27 04:40:59.303625 fs_dropboxfs-1.0.2/fs/dropboxfs/__init__.py
--rw-r--r--   0        0        0    11119 2023-11-20 06:03:54.981338 fs_dropboxfs-1.0.2/fs/dropboxfs/dropboxfs.py
--rw-r--r--   0        0        0      707 2023-09-27 04:40:59.303990 fs_dropboxfs-1.0.2/fs/dropboxfs/opener.py
--rw-r--r--   0        0        0     1703 2023-11-20 05:58:14.992937 fs_dropboxfs-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 fs_dropboxfs-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-11-26 02:07:10.069629 fs_dropboxfs-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1266 2023-11-20 05:31:26.424923 fs_dropboxfs-1.0.3/README.md
+-rw-r--r--   0        0        0      184 2023-09-27 04:40:59.303625 fs_dropboxfs-1.0.3/fs/dropboxfs/__init__.py
+-rw-r--r--   0        0        0    11340 2024-06-01 01:32:10.523822 fs_dropboxfs-1.0.3/fs/dropboxfs/dropboxfs.py
+-rw-r--r--   0        0        0      707 2023-09-27 04:40:59.303990 fs_dropboxfs-1.0.3/fs/dropboxfs/opener.py
+-rw-r--r--   0        0        0     1727 2024-06-01 01:33:15.741573 fs_dropboxfs-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 fs_dropboxfs-1.0.3/PKG-INFO
```

### Comparing `fs_dropboxfs-1.0.2/LICENSE` & `fs_dropboxfs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fs_dropboxfs-1.0.2/README.md` & `fs_dropboxfs-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fs_dropboxfs-1.0.2/fs/dropboxfs/dropboxfs.py` & `fs_dropboxfs-1.0.3/fs/dropboxfs/dropboxfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,15 +284,19 @@
 	def scandir(self, path, namespaces=None, page=None):
 		_logger.info(f'scandir({path}, {namespaces}, {page})')
 		path = self.validatepath(path)
 		with self._lock:
 			# get all the avaliable metadata since it's cheap
 			# TODO - this call has a recursive flag so we can either use that and cache OR override walk
 			try:
-				result = self.dropbox.files_list_folder(path)
+				effective_path = path
+				if path == '/':
+					# Error in call to API function "files/list_folder": request body: path: Specify the root folder as an empty string rather than as "/"
+					effective_path = ''
+				result = self.dropbox.files_list_folder(effective_path)
 			except ApiError as e:
 				assert isinstance(e.error, ListFolderError), 'Unexpected Dropbox error thrown'
 				if e.error.is_path() is False:
 					raise FSError from e
 				lookupError = e.error.get_path()
 				if lookupError.is_not_found():
 					raise ResourceNotFound(path=path) from e
```

### Comparing `fs_dropboxfs-1.0.2/fs/dropboxfs/opener.py` & `fs_dropboxfs-1.0.3/fs/dropboxfs/opener.py`

 * *Files identical despite different names*

### Comparing `fs_dropboxfs-1.0.2/pyproject.toml` & `fs_dropboxfs-1.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fs.dropboxfs"
-version = "1.0.2"
+version = "1.0.3"
 description = "Pyfilesystem2 implementation for Dropbox"
 authors = ["Rehan Khwaja <rehan@khwaja.name>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "fs"}]
 homepage = "https://github.com/rkhwaja/fs.dropboxfs"
 keywords = ["filesystem", "Pyfilesystem2", "dropbox"]
@@ -26,38 +26,38 @@
 setuptools = "<67" # 67 broke something to do with pyfilesystem openers
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.2.0"
 pyperclip = ">=1.8.2"
 poethepoet = ">=0.16.4"
 pytest-xdist = ">=3.2.1"
-ruff = ">=0.0.291"
+ruff = ">=0.4.4"
 
 [tool.poetry.plugins] # Optional super table
 
 [tool.poetry.plugins."fs.opener"]
 "dropbox" = "fs.dropboxfs.opener:DropboxOpener"
 
 [tool.poe.tasks]
-lint = "ruff fs/dropboxfs/ tests/"
+lint = "ruff check fs/dropboxfs/ tests/"
 
 [tool.poe.tasks.test]
 shell = """
 pytest -n 8 || exit 1
 """
 
 [tool.ruff]
 line-length = 1000
-ignore = ["ANN", "B011", "COM812", "D", "DTZ", "EM", "ERA001", "FBT002", "FIX", "G004", "I", "N802", "N806", "N815", "N816", "PLR0913", "PTH", "S101", "T201", "TD", "TRY003", "W191"]
-select = ["ALL"]
+lint.ignore = ["ANN", "B011", "COM812", "D", "DTZ", "EM", "ERA001", "FBT002", "FIX", "G004", "I", "N802", "N806", "N815", "N816", "PLR0913", "PTH", "S101", "T201", "TD", "TRY003", "W191"]
+lint.select = ["ALL"]
 target-version = "py38"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "fs/**" = ["PT"]
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "single"
 multiline-quotes = "single"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fs_dropboxfs-1.0.2/PKG-INFO` & `fs_dropboxfs-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs.dropboxfs
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pyfilesystem2 implementation for Dropbox
 Home-page: https://github.com/rkhwaja/fs.dropboxfs
 License: MIT
 Keywords: filesystem,Pyfilesystem2,dropbox
 Author: Rehan Khwaja
 Author-email: rehan@khwaja.name
 Requires-Python: >=3.8
```

