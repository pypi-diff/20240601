# Comparing `tmp/mkdocs_include_markdown_plugin-6.0.7.tar.gz` & `tmp/mkdocs_include_markdown_plugin-6.1.0.tar.gz`

## Comparing `mkdocs_include_markdown_plugin-6.0.7.tar` & `mkdocs_include_markdown_plugin-6.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/__init__.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/cache.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/config.py
--rw-r--r--   0        0        0     8134 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/directive.py
--rw-r--r--   0        0        0    24484 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/event.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/files_watcher.py
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/plugin.py
--rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/py.typed
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/.gitignore
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/LICENSE
--rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/README.md
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/pyproject.toml
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.0.7/PKG-INFO
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/__init__.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/cache.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/config.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/directive.py
+-rw-r--r--   0        0        0    24416 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/event.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/files_watcher.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/plugin.py
+-rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/py.typed
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/.gitignore
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/LICENSE
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/README.md
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11389 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-6.1.0/PKG-INFO
```

### Comparing `mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/cache.py` & `mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/cache.py`

 * *Files identical despite different names*

### Comparing `mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/config.py` & `mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,7 +20,8 @@
     comments = MkType(bool, default=True)
     rewrite_relative_urls = MkType(bool, default=True)
     heading_offset = MkType(int, default=0)
     start = Optional(MkType(str))
     end = Optional(MkType(str))
     exclude = ListOfItems(MkType(str), default=[])
     cache = MkType(int, default=0)
+    recursive = MkType(bool, default=True)
```

### Comparing `mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/directive.py` & `mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/directive.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             'encoding': str,
             'preserve-includer-indent': bool,
             'dedent': bool,
             'trailing-newlines': bool,
             'comments': bool,
             'rewrite-relative-urls': bool,
             'heading-offset': int,
+            'recursive': bool,
             'start': str | None,
             'end': str | None,
         },
     )
 
 
 GLOB_FLAGS = glob.NEGATE | glob.EXTGLOB | glob.GLOBSTAR | glob.BRACE
@@ -92,14 +93,15 @@
 
     # bool
     'comments': arg('comments'),
     'preserve-includer-indent': arg('preserve-includer-indent'),
     'dedent': arg('dedent'),
     'trailing-newlines': arg('trailing-newlines'),
     'rewrite-relative-urls': arg('rewrite-relative-urls'),
+    'recursive': arg('recursive'),
 
     # int
     'heading-offset': arg('heading-offset'),
 }
 
 
 def parse_filename_argument(
```

### Comparing `mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/event.py` & `mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,30 @@
         defaults: DefaultValues,
         settings: Settings,
         cumulative_heading_offset: int = 0,
         files_watcher: FilesWatcher | None = None,
         http_cache: Cache | None = None,
 ) -> str:
     """Return the content of the file to include."""
+    settings_ignore_paths = []
+    if settings.exclude is not None:
+        for path in glob.glob(
+                [
+                    os.path.join(docs_dir, fp)
+                    if not os.path.isabs(fp)
+                    else fp for fp in settings.exclude
+                ],
+                flags=GLOB_FLAGS,
+                root_dir=docs_dir,
+        ):
+            if path not in settings_ignore_paths:
+                settings_ignore_paths.append(path)
+        if page_src_path in settings_ignore_paths:
+            return markdown
+
     def found_include_tag(  # noqa: PLR0912, PLR0915
             match: re.Match[str],
     ) -> str:
         directive_match_start = match.start()
 
         includer_indent = match['_includer_indent']
 
@@ -121,48 +137,35 @@
                 ' directive at'
                 f' {file_lineno_message(page_src_path, docs_dir, lineno)}',
             )
 
         arguments_string = match['arguments']
 
         exclude_match = ARGUMENT_REGEXES['exclude'].search(arguments_string)
-        ignore_paths = []
-        if settings.exclude:
-            ignore_paths.extend(
-                glob.glob(
-                    [
-                        os.path.join(docs_dir, fp)
-                        if not os.path.isabs(fp)
-                        else fp for fp in settings.exclude
-                    ],
-                    flags=GLOB_FLAGS,
-                    root_dir=docs_dir,
-                ),
-            )
+        ignore_paths = [*settings_ignore_paths]
         if exclude_match is not None:
             exclude_string = parse_string_argument(exclude_match)
             if exclude_string is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
                 raise PluginError(
                     "Invalid empty 'exclude' argument in 'include'"
                     ' directive at'
                     f' {file_lineno_message(page_src_path, docs_dir, lineno)}',
                 )
 
-            ignore_paths.extend(
-                resolve_file_paths_to_exclude(
+            for path in resolve_file_paths_to_exclude(
                     exclude_string,
                     page_src_path,
                     docs_dir,
-                ),
-            )
-        ignore_paths = list(set(ignore_paths))
+            ):
+                if path not in ignore_paths:
+                    ignore_paths.append(path)
 
         file_paths_to_include, is_url = resolve_file_paths_to_include(
             filename,
             page_src_path,
             docs_dir,
             ignore_paths,
         )
@@ -177,15 +180,16 @@
                 f' {file_lineno_message(page_src_path, docs_dir, lineno)}',
             )
 
         if files_watcher is not None and not is_url:
             files_watcher.included_files.extend(file_paths_to_include)
 
         bool_options, invalid_bool_args = parse_bool_options(
-            ['preserve-includer-indent', 'dedent', 'trailing-newlines'],
+            ['preserve-includer-indent', 'dedent',
+                'trailing-newlines', 'recursive'],
             defaults,
             arguments_string,
         )
         if invalid_bool_args:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
@@ -260,24 +264,25 @@
                     )
                 )
                 for i in range(2):
                     if expected_but_any_found[i] and not expected_not_found[i]:
                         expected_but_any_found[i] = False
 
             # nested includes
-            new_text_to_include = get_file_content(
-                new_text_to_include,
-                file_path,
-                docs_dir,
-                tags,
-                defaults,
-                settings,
-                files_watcher=files_watcher,
-                http_cache=http_cache,
-            )
+            if bool_options['recursive'].value:
+                new_text_to_include = get_file_content(
+                    new_text_to_include,
+                    file_path,
+                    docs_dir,
+                    tags,
+                    defaults,
+                    settings,
+                    files_watcher=files_watcher,
+                    http_cache=http_cache,
+                )
 
             # trailing newlines right stripping
             if not bool_options['trailing-newlines'].value:
                 new_text_to_include = process.rstrip_trailing_newlines(
                     new_text_to_include,
                 )
 
@@ -345,47 +350,34 @@
                 f' directive at'
                 f' {file_lineno_message(page_src_path, docs_dir, lineno)}',
             )
 
         arguments_string = match['arguments']
 
         exclude_match = ARGUMENT_REGEXES['exclude'].search(arguments_string)
-        ignore_paths = []
-        if settings.exclude is not None:
-            ignore_paths.extend(
-                glob.glob(
-                    [
-                        os.path.join(docs_dir, fp)
-                        if not os.path.isabs(fp)
-                        else fp for fp in settings.exclude
-                    ],
-                    flags=GLOB_FLAGS,
-                    root_dir=docs_dir,
-                ),
-            )
+        ignore_paths = [*settings_ignore_paths]
         if exclude_match is not None:
             exclude_string = parse_string_argument(exclude_match)
             if exclude_string is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
                 raise PluginError(
                     "Invalid empty 'exclude' argument in 'include-markdown'"
                     f' directive at'
                     f' {file_lineno_message(page_src_path, docs_dir, lineno)}',
                 )
-            ignore_paths.extend(
-                resolve_file_paths_to_exclude(
+            for path in resolve_file_paths_to_exclude(
                     exclude_string,
                     page_src_path,
                     docs_dir,
-                ),
-            )
-        ignore_paths = list(set(ignore_paths))
+            ):
+                if path not in ignore_paths:
+                    ignore_paths.append(path)
 
         file_paths_to_include, is_url = resolve_file_paths_to_include(
             filename,
             page_src_path,
             docs_dir,
             ignore_paths,
         )
@@ -663,14 +655,15 @@
             'encoding': config.encoding,
             'preserve-includer-indent': config.preserve_includer_indent,
             'dedent': config.dedent,
             'trailing-newlines': config.trailing_newlines,
             'comments': config.comments,
             'rewrite-relative-urls': config.rewrite_relative_urls,
             'heading-offset': config.heading_offset,
+            'recursive': config.recursive,
             'start': config.start,
             'end': config.end,
         },
         Settings(
             exclude=config.exclude,
         ),
         files_watcher=plugin._files_watcher,
```

### Comparing `mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/plugin.py` & `mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_include_markdown_plugin-6.0.7/src/mkdocs_include_markdown_plugin/process.py` & `mkdocs_include_markdown_plugin-6.1.0/src/mkdocs_include_markdown_plugin/process.py`

 * *Files identical despite different names*

### Comparing `mkdocs_include_markdown_plugin-6.0.7/LICENSE` & `mkdocs_include_markdown_plugin-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_include_markdown_plugin-6.0.7/README.md` & `mkdocs_include_markdown_plugin-6.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
       dedent: false
       trailing_newlines: true
       comments: true
       rewrite_relative_urls: true
       heading_offset: 0
       start: <!--start-->
       end: <!--end-->
+      recursive: true
 ```
 
 #### `opening_tag` and `closing_tag`
 
 Default opening and closing tags. When not specified they are `{%` and `%}`.
 
 ```yaml
@@ -241,14 +242,17 @@
   when passing globs to include multiple files.
 - <a name="include_trailing-newlines" href="#include_trailing-newlines">#</a>
   **trailing-newlines** (_true_): When this option is disabled, the trailing newlines
   found in the content to include are stripped. Possible values are `true` and `false`.
 - <a name="include_encoding" href="#include_encoding">#</a>
   **encoding** (_utf-8_): Specify the encoding of the included file.
   If not defined `utf-8` will be used.
+- <a name="recursive" href="#include_recursive">#</a>
+  **recursive** (_true_): When this option is disabled, included files are not
+  processed for recursive includes. Possible values are `true` and `false`.
 
 ##### Examples
 
 ```jinja
 ~~~yaml
 {% include "../examples/github-minimal.yml" %}
 ~~~
```

### Comparing `mkdocs_include_markdown_plugin-6.0.7/pyproject.toml` & `mkdocs_include_markdown_plugin-6.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-include-markdown-plugin"
-version = "6.0.7"
+version = "6.1.0"
 description = "Mkdocs Markdown includer plugin."
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Operating System :: OS Independent",
```

### Comparing `mkdocs_include_markdown_plugin-6.0.7/PKG-INFO` & `mkdocs_include_markdown_plugin-6.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mkdocs-include-markdown-plugin
-Version: 6.0.7
+Version: 6.1.0
 Summary: Mkdocs Markdown includer plugin.
 Project-URL: Source, https://github.com/mondeja/mkdocs-include-markdown-plugin
 Project-URL: Documentation, https://github.com/mondeja/mkdocs-include-markdown-plugin#documentation
 Project-URL: Bug tracker, https://github.com/mondeja/mkdocs-include-markdown-plugin/issues
 Project-URL: Changelog, https://github.com/mondeja/mkdocs-include-markdown-plugin/releases
 Author: Joe Rickerby
 Author-email: Álvaro Mondéjar Rubio <mondejar1994@gmail.com>
@@ -90,14 +90,15 @@
       dedent: false
       trailing_newlines: true
       comments: true
       rewrite_relative_urls: true
       heading_offset: 0
       start: <!--start-->
       end: <!--end-->
+      recursive: true
 ```
 
 #### `opening_tag` and `closing_tag`
 
 Default opening and closing tags. When not specified they are `{%` and `%}`.
 
 ```yaml
@@ -276,14 +277,17 @@
   when passing globs to include multiple files.
 - <a name="include_trailing-newlines" href="#include_trailing-newlines">#</a>
   **trailing-newlines** (_true_): When this option is disabled, the trailing newlines
   found in the content to include are stripped. Possible values are `true` and `false`.
 - <a name="include_encoding" href="#include_encoding">#</a>
   **encoding** (_utf-8_): Specify the encoding of the included file.
   If not defined `utf-8` will be used.
+- <a name="recursive" href="#include_recursive">#</a>
+  **recursive** (_true_): When this option is disabled, included files are not
+  processed for recursive includes. Possible values are `true` and `false`.
 
 ##### Examples
 
 ```jinja
 ~~~yaml
 {% include "../examples/github-minimal.yml" %}
 ~~~
```

