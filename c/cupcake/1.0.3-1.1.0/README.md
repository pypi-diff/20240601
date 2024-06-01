# Comparing `tmp/cupcake-1.0.3.tar.gz` & `tmp/cupcake-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake-1.0.3.tar", max compression
+gzip compressed data, was "cupcake-1.1.0.tar", max compression
```

## Comparing `cupcake-1.0.3.tar` & `cupcake-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.0.3/LICENSE
--rw-r--r--   0        0        0      594 2024-05-07 13:12:26.668058 cupcake-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.0.3/src/cupcake/__init__.py
--rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.0.3/src/cupcake/cascade.py
--rw-r--r--   0        0        0    10186 2024-05-07 04:36:31.961880 cupcake-1.0.3/src/cupcake/confee.py
--rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.0.3/src/cupcake/data/cmake_names.py
--rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.0.3/src/cupcake/data/new/.gitignore
--rw-r--r--   0        0        0     1031 2024-04-30 21:17:59.470632 cupcake-1.0.3/src/cupcake/data/new/CMakeLists.txt
--rw-r--r--   0        0        0     2477 2024-04-29 20:21:28.383431 cupcake-1.0.3/src/cupcake/data/new/conanfile.py
--rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.0.3/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
--rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.0.3/src/cupcake/data/new/src/lib{{name}}.cpp
--rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.0.3/src/cupcake/data/new/src/{{name}}.cpp
--rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-1.0.3/src/cupcake/data/new/tests/CMakeLists.txt
--rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.0.3/src/cupcake/data/new/tests/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.0.3/src/cupcake/data/query/CMakeLists.txt
--rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.0.3/src/cupcake/expression.py
--rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.0.3/src/cupcake/functional.py
--rw-r--r--   0        0        0    56076 2024-05-07 13:09:21.595122 cupcake-1.0.3/src/cupcake/main.py
--rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.0.3/src/cupcake/transformations.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 cupcake-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.1.0/LICENSE
+-rw-r--r--   0        0        0      612 2024-06-01 04:01:54.329876 cupcake-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.1.0/src/cupcake/__init__.py
+-rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.1.0/src/cupcake/cascade.py
+-rw-r--r--   0        0        0    10126 2024-06-01 03:11:31.727585 cupcake-1.1.0/src/cupcake/confee.py
+-rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.1.0/src/cupcake/data/cmake_names.py
+-rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.1.0/src/cupcake/data/new/.gitignore
+-rw-r--r--   0        0        0     1339 2024-05-31 04:30:52.889552 cupcake-1.1.0/src/cupcake/data/new/CMakeLists.txt
+-rw-r--r--   0        0        0     3301 2024-05-31 04:30:52.889552 cupcake-1.1.0/src/cupcake/data/new/conanfile.py
+-rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.1.0/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
+-rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.1.0/src/cupcake/data/new/src/lib{{name}}.cpp
+-rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.1.0/src/cupcake/data/new/src/{{name}}.cpp
+-rw-r--r--   0        0        0      469 2024-05-31 03:14:56.556911 cupcake-1.1.0/src/cupcake/data/new/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.1.0/src/cupcake/data/new/tests/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.1.0/src/cupcake/data/query/CMakeLists.txt
+-rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.1.0/src/cupcake/expression.py
+-rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.1.0/src/cupcake/functional.py
+-rw-r--r--   0        0        0    61628 2024-06-01 03:15:07.109670 cupcake-1.1.0/src/cupcake/main.py
+-rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.1.0/src/cupcake/transformations.py
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 cupcake-1.1.0/PKG-INFO
```

### Comparing `cupcake-1.0.3/LICENSE` & `cupcake-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.3/pyproject.toml` & `cupcake-1.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "cupcake"
-version = "1.0.3"
+version = "1.1.0"
 description = "Make C++ a piece of cake."
 authors = ["John Freeman <jfreeman08@gmail.com>"]
 packages = [{include = "cupcake", from = "src"}]
 
 [tool.poetry.scripts]
 cupcake = 'cupcake.main:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.0.4"
 click-option-group = "^0.5.3"
 tomlkit = "^0.10.1"
 jinja2 = "^3.1.1"
 psutil = "^5.9.8"
+semver = "^3.0.2"
 
 [tool.poetry.group.dev.dependencies]
 shush = "^0.3.2"
 pytest = "^7.0.1"
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.2.1"
```

### Comparing `cupcake-1.0.3/src/cupcake/cascade.py` & `cupcake-1.1.0/src/cupcake/cascade.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.3/src/cupcake/confee.py` & `cupcake-1.1.0/src/cupcake/confee.py`

 * *Files 7% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         return tomlkit.table()
 
 class JsonType:
     def read(self, file):
         return json.load(file)
     def write(self, file, value):
         json.dump(value, file, indent=2)
+        file.write('\n')
     def root(self):
         return {}
     def object(self):
         return {}
 
 def read(pathlike, typ=None):
     path = pathlib.Path(pathlike)
@@ -329,12 +330,11 @@
     set(proxy, items + type(items)([item]))
 
 def filter(proxies, pred):
     for proxy in proxies:
         if evaluate(pred, proxy()):
             yield proxy
 
-def remove_if(proxies, pred):
-    # Collect everything to remove before removing anything.
-    chosen = [proxy for proxy in proxies if evaluate(pred, proxy())]
-    for proxy in chosen:
+def remove(proxies):
+    # Collect all proxies before deleting any.
+    for proxy in list(proxies):
         delete(proxy)
```

### Comparing `cupcake-1.0.3/src/cupcake/data/cmake_names.py` & `cupcake-1.1.0/src/cupcake/data/cmake_names.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.3/src/cupcake/data/new/CMakeLists.txt` & `cupcake-1.1.0/src/cupcake/data/new/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 cmake_minimum_required(VERSION 3.21)
 
-project({{ name }}
-  VERSION 0.1.0
-  {% if github %}
-  HOMEPAGE_URL https://github.com/{{ github }}/{{ name }}
+{% if special %}
+file(READ cupcake.json metadata)
+string(JSON name GET "${metadata}" project name)
+string(JSON version GET "${metadata}" project version)
+string(JSON url ERROR_VARIABLE ignored GET "${metadata}" project url)
+{% else %}
+set(name {{ name }})
+set(version 0.1.0)
+{% if url %}
+set(url {{ url }})
+{% endif %}
+{% endif %}
+
+project(
+  ${name}
+  VERSION ${version}
+  {% if special or url %}
+  HOMEPAGE_URL ${url}
   {% endif %}
   LANGUAGES CXX
 )
 
 find_package(cupcake.cmake REQUIRED)
 
 cupcake_project()
 
 {% if special %}
 cupcake_find_packages(main)
 cupcake_link_libraries(${PROJECT_NAME}.imports.main INTERFACE main)
 cupcake_find_packages(tool PRIVATE)
-{% endif %}
 
+{% endif %}
 {% if with_library %}
 {% if special %}
 cupcake_add_libraries()
 {% else %}
 cupcake_add_library({{ name }})
 target_link_libraries(${this} PUBLIC ${PROJECT_NAME}.imports.main)
 {% endif %}
@@ -29,15 +43,15 @@
 {% endif %}
 {% if with_executable %}
 {% if special %}
 cupcake_add_executables()
 {% else %}
 cupcake_add_executable({{ name }})
 {% if with_library %}
-target_link_libraries(${this} PRIVATE ${PROJECT_NAME}.lib{{ name }})
+target_link_libraries(${this} PRIVATE ${PROJECT_NAME}.l.{{ name }})
 {% else %}
 target_link_libraries(${this} PRIVATE ${PROJECT_NAME}.imports.main)
 {% endif %}
 {% endif %}
 
 {% endif %}
 {% if with_tests %}
```

### Comparing `cupcake-1.0.3/src/cupcake/expression.py` & `cupcake-1.1.0/src/cupcake/expression.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.3/src/cupcake/main.py` & `cupcake-1.1.0/src/cupcake/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import json
 import locale
 import operator
 import os
 import pathlib
 import psutil
 import re
+import semver
 import shlex
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
 import typing as t
@@ -103,14 +104,15 @@
         return y if compare(x, y) < 0 else x
     return function
 
 # Build flavor is selected at build time.
 # Configuration commands take a set of possible flavors.
 
 # Map from friendly Cupcake name to Conan/CMake name.
+# TODO: Unalias flavor names before saving in `config_`.
 FLAVORS = {
     'd': 'Debug',
     'debug': 'Debug',
     'minsizerel': 'MinSizeRel',
     'msr': 'MinSizeRel',
     'r': 'Release',
     'rd': 'RelWithDebInfo',
@@ -246,20 +248,25 @@
         del requirements[i:i+1]
     after = f(before)
     if after is not None:
         requirements.append(after)
     requirements.sort(key=lambda item: item['name'])
     metadata.imports = requirements
 
-def expand(reference):
-    if reference.startswith('lib'):
-        return ('libraries', reference[len('lib'):])
-    if reference.startswith('test.'):
-        return ('tests', reference[len('test.'):])
-    return ('executables', reference)
+DEFAULT_TO_KIND = {
+    'library': 'libraries',
+    'executable': 'executables',
+}
+
+KIND_TO_DEFAULT = { v: k for k, v in DEFAULT_TO_KIND.items() }
+
+KIND_ALIASES = {
+    k: v for kind in ['libraries', 'executables', 'tests', 'imports']
+    for k, v in { kind: kind, kind[0]: kind }.items()
+}
 
 class SearchResult:
     """Representation for a Conan package search result."""
 
     key = functools.cmp_to_key(lambda a, b: a.__cmp__(b))
 
     def __init__(self, remote, reference):
@@ -913,26 +920,43 @@
             command.extend(['--target', target])
         with (log_dir_ / 'build').open('wb') as stream:
             tee(command, stream=stream)
         return cmake
 
     @cascade.command()
     @cascade.argument('executable', required=False)
-    # TODO: No way to pass arguments to default executable.
     @cascade.argument('arguments', nargs=-1)
     def exe(self, CMAKE, cmake_dir_, flavor_, cmake, executable, arguments):
         """Execute an executable."""
         target = 'execute'
-        if executable is not None:
+        if executable is not None and executable != '.':
             target += '.' + executable
         command = [CMAKE, '--build', cmake_dir_, '--target', target]
         if cmake.multiConfig():
             command.extend(['--config', FLAVORS[flavor_]])
         env = os.environ.copy()
-        escape = lambda arg: arg.replace(';', '\\;')
+        escape = lambda arg: '"' + arg.replace(';', '\\;') + '"'
+        env['CUPCAKE_EXE_ARGUMENTS'] = ';'.join(map(escape, arguments))
+        run(command, env=env)
+
+    @cascade.command()
+    @cascade.argument('executable', required=False)
+    @cascade.argument('arguments', nargs=-1)
+    def debug(self, CMAKE, cmake_dir_, flavor_, cmake, executable, arguments):
+        """Debug an executable."""
+        if flavor_ != 'debug':
+            raise SystemExit('must select debug flavor')
+        target = 'debug'
+        if executable is not None and executable != '.':
+            target += '.' + executable
+        command = [CMAKE, '--build', cmake_dir_, '--target', target]
+        if cmake.multiConfig():
+            command.extend(['--config', FLAVORS[flavor_]])
+        env = os.environ.copy()
+        escape = lambda arg: '"' + arg.replace(';', '\\;') + '"'
         env['CUPCAKE_EXE_ARGUMENTS'] = ';'.join(map(escape, arguments))
         run(command, env=env)
 
     @cascade.command()
     def install(self, CMAKE, cmake_dir_, flavor_, build, prefix_):
         """Install the selected flavor."""
         run([
@@ -989,15 +1013,15 @@
         jenv.filters['pascal'] = pascal
         jenv.filters['snake'] = snake
         return jenv
 
     @cascade.command()
     @cascade.argument('path', required=False, default='.')
     @cascade.option(
-        '--version', help='Version of requirement cupcake.cmake@github/thejohnfreeman.', default='1.0.2',
+        '--version', help='Version of requirement cupcake.cmake@github/thejohnfreeman.', default='1.1.0',
     )
     @cascade.option(
         '--special/--general', help='Whether to enable special commands.', default=True,
     )
     @cascade.option(
         '--library/--no-library', help='Whether to export a library.', default=True,
     )
@@ -1058,25 +1082,28 @@
             author = f'{username} <{email}>'
 
         prefix = pathlib.Path(path).resolve()
         if not force and prefix.exists() and any(prefix.iterdir()):
             raise SystemExit('directory is not empty')
         if name is None:
             name = prefix.name
+        url = None if github is None else f'https://github.com/{github}/{name}'
 
         # TODO: Take default license and github from user config.
+        # TODO: Write LICENSE file from template.
         context = dict(
             version=version,
             special=special,
             with_library=library,
             with_executable=executable,
             with_tests=tests,
             license=license,
             author=author,
             github=github,
+            url=url,
         )
 
         tnames = [
             n for n in jenv.list_templates()
             if (library or not n.startswith('include/'))
             or (library or not n.startswith('src/lib'))
             or (executable or not (n.startswith('src/') and not n.startswith('src/lib')))
@@ -1084,22 +1111,25 @@
         ]
         self.generate_(jenv, prefix, tnames, name, context)
 
         # Assemble and write cupcake.json.
         if special:
             metadata = confee.read(prefix / 'cupcake.json')
             metadata.project.name = name
+            metadata.project.version = '0.1.0'
+            if url is not None:
+                metadata.project.url = url
             if library:
                 metadata.libraries = [
                     {'name': name, 'links': ['${PROJECT_NAME}.imports.main'] }
                 ]
             if executable:
                 links = ['${PROJECT_NAME}.imports.main']
                 if library:
-                    links.append(f'{name}.lib{name}')
+                    links.append(f'{name}.library')
                 exe = {'name': name, 'links': links}
                 metadata.executables = [exe]
             if tests:
                 metadata.imports = [
                     {
                         'name': 'doctest',
                         'version': '2.4.8',
@@ -1107,15 +1137,15 @@
                         'file': 'doctest',
                         'targets': ['doctest::doctest'],
                         'groups': ['test'],
                     }
                 ]
                 links = ['${PROJECT_NAME}.imports.test']
                 if library:
-                    links.append(f'{name}.lib{name}')
+                    links.append(f'{name}.library')
                 test = {'name': name, 'links': links }
                 metadata.tests = [test]
             confee.write(metadata)
 
 
     def generate_(self, jenv, prefix, tnames, name, context):
         assert_legal_name(name)
@@ -1148,62 +1178,63 @@
 
     @cascade.command()
     # TODO: Mutually exclusive option group to choose requirement group.
     @cascade.option(
         '--group', '-g', metavar='GROUP', multiple=True, default=('main',),
         help='Requirement groups, e.g. "main" or "test".',
     )
-    @cascade.argument('query')
-    def add(self, CONAN, source_dir_, conanfile_path_, group, query):
-        """Add a requirement."""
+    @cascade.argument('queries', required=True, nargs=-1)
+    def add(self, CONAN, source_dir_, conanfile_path_, group, queries):
+        """Add one or more requirements."""
         # TODO: Support conanfile.txt.
         if conanfile_path_.name != 'conanfile.py':
             raise SystemExit('missing conanfile.py')
 
-        # Parse reference into name/version@user/channel
-        # with optional version, user, and channel.
-        match = re.match('([^/@]+)(?:/([^/@]+))?(?:@([^/@]+)/([^/@]+))?', query)
-        if not match:
-            raise SystemExit(f'not a reference pattern: "{query}"')
-        name, version, user, channel = match.groups()
-
-        if version is None:
-            subquery = f'{name}/*'
-            if user is not None:
-                subquery += f'@{user}/{channel}'
-            results = CONAN.search(subquery)
-            if len(results) < 1:
-                raise SystemExit('no matches found')
-            version = results[0].version
-
-        reference = f'{name}/{version}'
-        if user is not None:
-            reference += f'@{user}/{channel}'
-
-        # Find the CMake names.
-        names = CONAN.get_cmake_names(reference)
-
         # Find the cupcake.json.
         path = source_dir_ / 'cupcake.json'
         metadata = confee.read(path)
 
-        # Add or update the requirement.
-        def add_requirement(before):
-            if before is not None:
-                # TODO: Add --upgrade option.
-                raise SystemExit(f'{name} already in imports')
-            return {
-                'name': name,
-                'version': version,
-                'reference': reference,
-                'file': names['file'],
-                'targets': names['targets'],
-                'groups': group,
-            }
-        update_requirement(metadata, name, add_requirement)
+        for query in queries:
+            # Parse reference into name/version@user/channel
+            # with optional version, user, and channel.
+            match = re.match('([^/@]+)(?:/([^/@]+))?(?:@([^/@]+)/([^/@]+))?', query)
+            if not match:
+                raise SystemExit(f'not a reference pattern: "{query}"')
+            name, version, user, channel = match.groups()
+
+            if version is None:
+                subquery = f'{name}/*'
+                if user is not None:
+                    subquery += f'@{user}/{channel}'
+                results = CONAN.search(subquery)
+                if len(results) < 1:
+                    raise SystemExit('no matches found')
+                version = results[0].version
+
+            reference = f'{name}/{version}'
+            if user is not None:
+                reference += f'@{user}/{channel}'
+
+            # Find the CMake names.
+            names = CONAN.get_cmake_names(reference)
+
+            # Add or update the requirement.
+            def add_requirement(before):
+                if before is not None:
+                    # TODO: Add --upgrade option.
+                    raise SystemExit(f'{name} already in imports')
+                return {
+                    'name': name,
+                    'version': version,
+                    'reference': reference,
+                    'file': names['file'],
+                    'targets': names['targets'],
+                    'groups': group,
+                }
+            update_requirement(metadata, name, add_requirement)
 
         # Update cupcake.json.
         confee.write(metadata)
 
     @cascade.command()
     @cascade.argument('name')
     def remove(self, conanfile_path_, source_dir_, name):
@@ -1223,116 +1254,206 @@
         update_requirement(metadata, name, const(None))
         confee.write(metadata)
 
     @cascade.command()
     def list(self, source_dir_):
         """List targets and their links."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        kinds = [
-            ('libraries', 'lib'),
-            ('executables', ''),
-            ('tests', 'test.'),
-        ]
-        for kind, prefix in kinds:
+        for kind in ('libraries', 'executables', 'tests'):
             for item in metadata[kind][:]:
-                line = f'{prefix}{item.name()}'
+                line = f'.{kind[0]}.{item.name()}'
                 links = item.links([])
                 if links:
                     line += ' -> ' + ', '.join(links)
                 print(line)
 
     @cascade.command()
     @cascade.argument('downstream', required=True)
     @cascade.argument('upstreams', required=True, nargs=-1)
     def link(self, source_dir_, downstream, upstreams):
-        """Link a downstream target to upstream libraries."""
+        """Link a target to one or more libraries."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
         pname = metadata.project.name()
 
-        def unprefix(reference):
-            for prefix in (pname + '.', '${PROJECT_NAME}.'):
-                if reference.startswith(prefix):
-                    return reference[len(prefix):]
-            return reference
+        # Linked internal targets _must_ be qualified by their project name,
+        # even if it is the default library or the libraries group.
+        # In other words, you cannot link to root project targets,
+        # e.g. `library` or `l.<name>` or `libraries`.
+        # Those targets are provided for convenience on the command-line.
+        #
+        # We cannot assume anything about the format of external targets,
+        # even though they typically contain double colon (`::`).
+        # We cannot assume any aliases for them.
+        #
+        # We _can_ assume that this project is a special Cupcake project.
+        # We _can_ assume that all upstream targets are libraries.
+        # Therefore, upstream internal targets will start with either
+        # `<project-name>.` or `${PROJECT_NAME}.`.
+        # For convenience, we let callers abbreviate the prefix to just `.`.
+        #
+        # Internal targets _may_ not be declared in the metadata.
+        # We cannot assume that they appear there.
+        # We _can_ assume their aliases and verify that
+        # they are not directly linked more than once by the same target.
+        #
+        # If a target has one of the three recognized project prefixes,
+        # then assume it is an internal Cupcake target
+        # and generate all of its known aliases.
+        # Otherwise, assume it is an external target and generate no aliases.
+        #
+        # The upstream target _must_ be an internal target,
+        # i.e. library or executable target with prefixed name,
+        # and it _must_ appear in the metadata.
+        # Resolve its target to its kind and name to find it in the metadata.
+
+        def unalias(target):
+            # Take the prefix up to the first dot (.).
+            # If it does not exist, or does not match a known prefix,
+            # then assume it is an external target and return nothing.
+            parts = target.split('.')
+            if parts[0] not in ('', pname, '${PROJECT_NAME}'):
+                return (None, None)
+            try:
+                if parts[1] in DEFAULT_TO_KIND:
+                    assert(len(parts) == 2)
+                    return (DEFAULT_TO_KIND[parts[1]], pname)
+                if parts[1] in KIND_ALIASES:
+                    assert(parts[2])
+                    return (KIND_ALIASES[parts[1]], parts[2])
+            except:
+                pass
+            raise SystemExit(f'malformed reference: {target}')
 
         def find(reference):
-            kind, name = expand(reference)
+            kind, name = unalias(reference)
+            if kind is None:
+                raise SystemExit(f'not an internal target: {reference}')
             items = confee.filter(metadata[kind][:], subject['name'] == name)
             items = list(items)
             if len(items) > 1:
                 raise SystemExit(f'ambiguous reference: {reference}')
             if len(items) < 1:
                 raise SystemExit(f'unknown reference: {reference}')
             return items[0]
 
-        downstream = unprefix(downstream)
+        def expand(reference):
+            kind, name = unalias(reference)
+            if kind is None:
+                return [reference]
+            suffixes = [f'{kind}.{name}', f'{kind[0]}.{name}']
+            if name == pname:
+                suffixes += [KIND_TO_DEFAULT[kind]]
+            return [
+                prefix + '.' + suffix
+                for suffix in suffixes
+                for prefix in ['${PROJECT_NAME}', pname]
+            ]
+
+        # Find the downstream target in the metadata.
+        # It must be a special internal target.
         dproxy = find(downstream)
 
         for upstream in upstreams:
-            upstream = unprefix(upstream)
-            if upstream.startswith('lib'):
-                uproxy = find(upstream)
-                if uproxy == dproxy:
-                    raise SystemExit(f'cannot link to self')
-            elif not re.match(f'^imports.\\w+$', upstream):
-                raise SystemExit(f'upstream is not a library: {upstream}')
-
-            link1 = '${PROJECT_NAME}.' + upstream
-            link2 = pname + '.' + upstream
-
+            # TODO: Check for cycles, including through aliases.
+            aliases = expand(upstream)
             existing = confee.filter(dproxy.links[:], (
-                (subject == link1) | (subject == link2) |
-                (subject['target'] == link1) | (subject['target'] == link2)
+                contains(aliases, subject) |
+                contains(aliases, subject['target'])
             ))
             existing = list(existing)
+            # Skip duplicates.
+            if len(existing) > 1:
+                # Duplicate links were _already_ present.
+                raise SystemExit(f'duplicate links found: {existing}')
             if len(existing) > 0:
-                raise SystemExit('already linked')
-            confee.add(dproxy.links, link1)
+                # TODO: If verbose, print a warning.
+                continue
+            confee.add(dproxy.links, aliases[0])
 
         confee.write(metadata)
 
+    @cascade.command('version')
+    @cascade.argument('version', required=False)
+    def version_(self, source_dir_, version):
+        """Print or change the package version."""
+        metadata = confee.read(source_dir_ / 'cupcake.json')
+        before = metadata.project.version()
+        if version is None:
+            return print(before)
+        if version in ('major', 'minor', 'patch'):
+            before = semver.Version.parse(before)
+            method = f'bump_{version}'
+            after = getattr(before, method)()
+            metadata.project.version = after
+        else:
+            # Assert that it can be parsed.
+            semver.Version.parse(version)
+            metadata.project.version = version
+        confee.write(metadata)
+
     @cascade.command()
     @cascade.argument('downstream', required=True)
     @cascade.argument('upstreams', required=True, nargs=-1)
     def unlink(self, source_dir_, downstream, upstreams):
-        """Unlink a downstream target from upstream libraries."""
+        """Unlink a target from one or more libraries."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
         pname = metadata.project.name()
 
-        def unprefix(reference):
-            for prefix in (pname + '.', '${PROJECT_NAME}.'):
-                if reference.startswith(prefix):
-                    return reference[len(prefix):]
-            return reference
+        def unalias(target):
+            # Take the prefix up to the first dot (.).
+            # If it does not exist, or does not match a known prefix,
+            # then assume it is an external target and return nothing.
+            parts = target.split('.')
+            if parts[0] not in ('', pname, '${PROJECT_NAME}'):
+                return (None, None)
+            try:
+                if parts[1] in DEFAULT_TO_KIND:
+                    assert(len(parts) == 2)
+                    return (DEFAULT_TO_KIND[parts[1]], pname)
+                if parts[1] in KIND_ALIASES:
+                    assert(parts[2])
+                    return (KIND_ALIASES[parts[1]], parts[2])
+            except:
+                pass
+            raise SystemExit(f'malformed reference: {target}')
 
         def find(reference):
-            kind, name = expand(reference)
+            kind, name = unalias(reference)
+            if kind is None:
+                raise SystemExit(f'not an internal target: {reference}')
             items = confee.filter(metadata[kind][:], subject['name'] == name)
             items = list(items)
             if len(items) > 1:
                 raise SystemExit(f'ambiguous reference: {reference}')
             if len(items) < 1:
                 raise SystemExit(f'unknown reference: {reference}')
             return items[0]
 
-        downstream = unprefix(downstream)
+        def expand(reference):
+            kind, name = unalias(reference)
+            if kind is None:
+                return [reference]
+            suffixes = [f'{kind}.{name}', f'{kind[0]}.{name}']
+            if name == pname:
+                suffixes += [KIND_TO_DEFAULT[kind]]
+            return [
+                prefix + '.' + suffix
+                for suffix in suffixes
+                for prefix in [pname, '${PROJECT_NAME}']
+            ]
+
         dproxy = find(downstream)
 
         for upstream in upstreams:
-            upstream = unprefix(upstream)
-            # We don't need to check that upstream is a library.
-            # All we care is whether it appears in the links.
-
-            link1 = '${PROJECT_NAME}.' + upstream
-            link2 = pname + '.' + upstream
-
-            confee.remove_if(dproxy.links[:], (
-                (subject == link1) | (subject == link2) |
-                (subject['target'] == link1) | (subject['target'] == link2)
+            aliases = expand(upstream)
+            existing = confee.filter(dproxy.links[:], (
+                contains(aliases, subject) |
+                contains(aliases, subject['target'])
             ))
+            confee.remove(existing)
 
         confee.write(metadata)
 
     @cascade.command('add:lib')
     @cascade.option('--public/--private', is_flag=True, default=True, help='Whether to export the library.')
     @cascade.option('--header-only', is_flag=True, help='Whether to create a source file.')
     @cascade.argument('names', required=True, nargs=-1)
```

### Comparing `cupcake-1.0.3/src/cupcake/transformations.py` & `cupcake-1.1.0/src/cupcake/transformations.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.3/PKG-INFO` & `cupcake-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: cupcake
-Version: 1.0.3
+Version: 1.1.0
 Summary: Make C++ a piece of cake.
 Author: John Freeman
 Author-email: jfreeman08@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.3,<0.6.0)
 Requires-Dist: jinja2 (>=3.1.1,<4.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
+Requires-Dist: semver (>=3.0.2,<4.0.0)
 Requires-Dist: tomlkit (>=0.10.1,<0.11.0)
```

