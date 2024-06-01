# Comparing `tmp/minecraft_script-0.2.0.tar.gz` & `tmp/minecraft_script-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.2.0.tar", last modified: Sun May 12 12:02:50 2024, max compression
+gzip compressed data, was "minecraft_script-0.2.1.tar", last modified: Sat Jun  1 10:32:28 2024, max compression
```

## Comparing `minecraft_script-0.2.0.tar` & `minecraft_script-0.2.1.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.814597 minecraft_script-0.2.0/
--rw-rw-rw-   0        0        0     2670 2024-05-12 12:02:50.813596 minecraft_script-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.714612 minecraft_script-0.2.0/minecraft_script/
--rw-rw-rw-   0        0        0     1169 2024-05-12 10:23:12.000000 minecraft_script-0.2.0/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      171 2024-05-10 15:07:03.000000 minecraft_script-0.2.0/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0      575 2024-05-09 19:42:35.000000 minecraft_script-0.2.0/minecraft_script/common.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.744746 minecraft_script-0.2.0/minecraft_script/compiler/
--rw-rw-rw-   0        0        0      223 2024-05-09 18:22:05.000000 minecraft_script-0.2.0/minecraft_script/compiler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.747749 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.759784 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/
--rw-rw-rw-   0        0        0        7 2024-03-23 20:02:41.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/command.mcfunction
--rw-rw-rw-   0        0        0       40 2024-05-05 13:37:43.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/give_item.mcfunction
--rw-rw-rw-   0        0        0      266 2024-03-25 19:24:47.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/log.mcfunction
--rw-rw-rw-   0        0        0       33 2024-03-28 19:55:27.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/builtins/set_block.mcfunction
--rw-rw-rw-   0        0        0       41 2023-08-30 16:13:30.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/function_tags.json
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.776980 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/
--rw-rw-rw-   0        0        0      115 2024-03-17 10:01:01.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/add.mcfunction
--rw-rw-rw-   0        0        0      115 2024-03-17 10:01:01.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/divide.mcfunction
--rw-rw-rw-   0        0        0      125 2024-03-23 17:55:14.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/equals.mcfunction
--rw-rw-rw-   0        0        0      126 2024-03-23 18:00:46.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/greater_equals_than.mcfunction
--rw-rw-rw-   0        0        0      125 2024-03-23 17:57:51.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/greater_than.mcfunction
--rw-rw-rw-   0        0        0      126 2024-03-23 17:58:24.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/less_equals_than.mcfunction
--rw-rw-rw-   0        0        0      125 2024-03-23 17:57:13.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/less_than.mcfunction
--rw-rw-rw-   0        0        0      115 2024-03-17 10:03:02.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/modulus.mcfunction
--rw-rw-rw-   0        0        0      115 2024-03-17 10:01:01.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/multiply.mcfunction
--rw-rw-rw-   0        0        0      115 2024-03-17 10:01:01.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/math/subtract.mcfunction
--rw-rw-rw-   0        0        0      140 2024-05-05 12:13:11.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0      487 2024-02-11 19:12:12.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/pack.png
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.702881 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/tags/
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.779982 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/tags/blocks/
--rw-rw-rw-   0        0        0      248 2024-03-29 21:11:25.000000 minecraft_script-0.2.0/minecraft_script/compiler/build_templates/tags/blocks/no_collision.json
--rw-rw-rw-   0        0        0    17022 2024-05-11 21:25:07.000000 minecraft_script-0.2.0/minecraft_script/compiler/builtin_functions.py
--rw-rw-rw-   0        0        0    21509 2024-05-11 17:21:20.000000 minecraft_script-0.2.0/minecraft_script/compiler/compile_interpreter.py
--rw-rw-rw-   0        0        0     4874 2024-05-09 10:44:09.000000 minecraft_script-0.2.0/minecraft_script/compiler/compile_types.py
--rw-rw-rw-   0        0        0     9822 2024-05-11 19:24:42.000000 minecraft_script-0.2.0/minecraft_script/compiler/compiler.py
--rw-rw-rw-   0        0        0       21 2024-05-09 20:04:29.000000 minecraft_script-0.2.0/minecraft_script/config.json
--rw-rw-rw-   0        0        0      954 2024-03-20 20:07:01.000000 minecraft_script-0.2.0/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.796579 minecraft_script-0.2.0/minecraft_script/interpreter/
--rw-rw-rw-   0        0        0        0 2024-03-17 11:19:20.000000 minecraft_script-0.2.0/minecraft_script/interpreter/__init__.py
--rw-rw-rw-   0        0        0     9127 2024-05-12 10:29:42.000000 minecraft_script-0.2.0/minecraft_script/interpreter/builtin_functions.py
--rw-rw-rw-   0        0        0    12773 2024-03-27 19:37:34.000000 minecraft_script-0.2.0/minecraft_script/interpreter/interpreter.py
--rw-rw-rw-   0        0        0    10427 2024-03-20 20:31:18.000000 minecraft_script-0.2.0/minecraft_script/interpreter/types.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.799583 minecraft_script-0.2.0/minecraft_script/lexer/
--rw-rw-rw-   0        0        0        0 2024-03-17 11:19:09.000000 minecraft_script-0.2.0/minecraft_script/lexer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.801585 minecraft_script-0.2.0/minecraft_script/lexer/grammar/
--rw-rw-rw-   0        0        0      427 2024-01-28 16:27:27.000000 minecraft_script-0.2.0/minecraft_script/lexer/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0     2489 2024-03-27 19:31:59.000000 minecraft_script-0.2.0/minecraft_script/lexer/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     5954 2024-03-27 19:15:41.000000 minecraft_script-0.2.0/minecraft_script/lexer/lexer.py
--rw-rw-rw-   0        0        0      929 2024-03-17 11:32:14.000000 minecraft_script-0.2.0/minecraft_script/lexer/tokens.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.811594 minecraft_script-0.2.0/minecraft_script/parser/
--rw-rw-rw-   0        0        0        0 2024-03-17 11:19:14.000000 minecraft_script-0.2.0/minecraft_script/parser/__init__.py
--rw-rw-rw-   0        0        0    11327 2024-03-27 19:33:03.000000 minecraft_script-0.2.0/minecraft_script/parser/nodes.py
--rw-rw-rw-   0        0        0    20952 2024-05-12 11:25:10.000000 minecraft_script-0.2.0/minecraft_script/parser/parser.py
--rw-rw-rw-   0        0        0     3882 2024-05-10 15:07:03.000000 minecraft_script-0.2.0/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-08-30 16:13:30.000000 minecraft_script-0.2.0/minecraft_script/text_additions.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:02:50.812594 minecraft_script-0.2.0/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     2670 2024-05-12 12:02:50.000000 minecraft_script-0.2.0/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2024-05-12 12:02:50.000000 minecraft_script-0.2.0/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 12:02:50.000000 minecraft_script-0.2.0/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 12:02:50.000000 minecraft_script-0.2.0/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 12:02:50.814597 minecraft_script-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1201 2024-05-12 12:02:09.000000 minecraft_script-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.396565 minecraft_script-0.2.1/
+-rw-rw-rw-   0        0        0     2681 2024-06-01 10:32:28.395564 minecraft_script-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.275708 minecraft_script-0.2.1/minecraft_script/
+-rw-rw-rw-   0        0        0     1169 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      171 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0      348 2024-05-31 21:09:56.000000 minecraft_script-0.2.1/minecraft_script/common.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.314138 minecraft_script-0.2.1/minecraft_script/compiler/
+-rw-rw-rw-   0        0        0      223 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.323943 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.337957 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/builtins/
+-rw-rw-rw-   0        0        0        7 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/builtins/command.mcfunction
+-rw-rw-rw-   0        0        0       40 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/builtins/give_item.mcfunction
+-rw-rw-rw-   0        0        0      266 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/builtins/log.mcfunction
+-rw-rw-rw-   0        0        0       33 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/builtins/set_block.mcfunction
+-rw-rw-rw-   0        0        0       41 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/function_tags.json
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.379730 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/
+-rw-rw-rw-   0        0        0      115 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/add.mcfunction
+-rw-rw-rw-   0        0        0      115 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/divide.mcfunction
+-rw-rw-rw-   0        0        0      125 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/equals.mcfunction
+-rw-rw-rw-   0        0        0      126 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/greater_equals_than.mcfunction
+-rw-rw-rw-   0        0        0      125 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/greater_than.mcfunction
+-rw-rw-rw-   0        0        0      126 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/less_equals_than.mcfunction
+-rw-rw-rw-   0        0        0      125 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/less_than.mcfunction
+-rw-rw-rw-   0        0        0      115 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/modulus.mcfunction
+-rw-rw-rw-   0        0        0      115 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/multiply.mcfunction
+-rw-rw-rw-   0        0        0      115 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/subtract.mcfunction
+-rw-rw-rw-   0        0        0       56 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/u_add.mcfunction
+-rw-rw-rw-   0        0        0      278 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/u_not.mcfunction
+-rw-rw-rw-   0        0        0      154 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/math/u_subtract.mcfunction
+-rw-rw-rw-   0        0        0      140 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0      487 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/pack.png
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.249185 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/tags/
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.383749 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/tags/blocks/
+-rw-rw-rw-   0        0        0      248 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/build_templates/tags/blocks/no_collision.json
+-rw-rw-rw-   0        0        0    16986 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/builtin_functions.py
+-rw-rw-rw-   0        0        0    23650 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/compile_interpreter.py
+-rw-rw-rw-   0        0        0     4874 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/compile_types.py
+-rw-rw-rw-   0        0        0     9814 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/compiler/compiler.py
+-rw-rw-rw-   0        0        0       52 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/config.json
+-rw-rw-rw-   0        0        0     1045 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/config_utils.py
+-rw-rw-rw-   0        0        0      954 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.386752 minecraft_script-0.2.1/minecraft_script/interpreter/
+-rw-rw-rw-   0        0        0        0 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/interpreter/__init__.py
+-rw-rw-rw-   0        0        0     9127 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/interpreter/builtin_functions.py
+-rw-rw-rw-   0        0        0    12773 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/interpreter/interpreter.py
+-rw-rw-rw-   0        0        0    10427 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/interpreter/types.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.389756 minecraft_script-0.2.1/minecraft_script/lexer/
+-rw-rw-rw-   0        0        0        0 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/lexer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.391560 minecraft_script-0.2.1/minecraft_script/lexer/grammar/
+-rw-rw-rw-   0        0        0      427 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/lexer/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0     2489 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/lexer/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     7165 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/lexer/lexer.py
+-rw-rw-rw-   0        0        0      929 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/lexer/tokens.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.393563 minecraft_script-0.2.1/minecraft_script/parser/
+-rw-rw-rw-   0        0        0        0 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/parser/__init__.py
+-rw-rw-rw-   0        0        0    11327 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/parser/nodes.py
+-rw-rw-rw-   0        0        0    20408 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/parser/parser.py
+-rw-rw-rw-   0        0        0     4029 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/minecraft_script/text_additions.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:32:28.394564 minecraft_script-0.2.1/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     2681 2024-06-01 10:32:28.000000 minecraft_script-0.2.1/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2500 2024-06-01 10:32:28.000000 minecraft_script-0.2.1/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 10:32:28.000000 minecraft_script-0.2.1/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-06-01 10:32:28.000000 minecraft_script-0.2.1/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 10:32:28.396565 minecraft_script-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-05-31 20:30:17.000000 minecraft_script-0.2.1/setup.py
```

### Comparing `minecraft_script-0.2.0/PKG-INFO` & `minecraft_script-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.2.0
+Version: 0.2.1
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <christophe@dronne.fr>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -35,32 +35,32 @@
 
 
 ## Using Minecraft Script to make Datapacks
 ### Debugging your program
 To debug your program, you can first run your file like any other programming language.
 To do this, use the following command:
 ```commandline
-python -m minecraft_script run [file]
+python -m minecraft_script debug <path>
 ```
-_where [file] is a relative or absolute path to your mcs file_
+_where <path> is a relative or absolute path to your mcs file_
 
 ### Building your datapack
 To actually build your minecraft datapack, which you can then simply drag & drop into your
 minecraft worlds, use the following command:
 ```commandline
-python -m minecraft_script build [file]
+python -m minecraft_script compile <path>
 ```
-_where [file] is a relative or absolute path to your mcs file_
+_where <path> is a relative or absolute path to your mcs file_
 
 ### More info
 For a list of all shell commands, you can use the following command:
 ```commandline
 python -m minecraft_script help
 ```
-If you want to simplify the usage of shell commands, you can check out [the installations page in the documentation](https://github.com/Bard-Gaming/Minecraft-Script/blob/main/documentation/installations.md).
+If you want to simplify the usage of shell commands, you can check out [the installations page in the documentation](https://github.com/Bard-Gaming/Minecraft-Script/blob/main/documentation/custom-installations.md).
 
 ## GitHub
 [**Link to GitHub Repository**](https://github.com/Bard-Gaming/Minecraft-Script)
 
 Source code, documentation, and examples, can all be found on the GitHub.
 
 ## Compatibility
```

### Comparing `minecraft_script-0.2.0/minecraft_script/__init__.py` & `minecraft_script-0.2.1/minecraft_script/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/compiler/builtin_functions.py` & `minecraft_script-0.2.1/minecraft_script/compiler/builtin_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .compile_types import *
-from ..common import COMMON_CONFIG
 
 function_output = tuple[tuple[str, ...], mcs_type]  # [commands, return value]
 
 
 def log(interpreter, args, context) -> function_output:
     max_length = 5
```

### Comparing `minecraft_script-0.2.0/minecraft_script/compiler/compile_interpreter.py` & `minecraft_script-0.2.1/minecraft_script/compiler/compile_interpreter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 from .builtin_functions import builtin_functions
 from .compile_types import *
+from ..common import COMMON_CONFIG
+
+
+def add_comment(commands: tuple, comment: str) -> tuple:
+    if COMMON_CONFIG["debug_comments"] is False:
+        return commands
+
+    return (f"\n# {comment}",) + commands
 
 
 class CompileSymbols:
     def __init__(self, parent: "CompileSymbols" = None, *, load_builtins: bool = False):
         self.symbols: dict[str, mcs_type] = {}
         self.parent = parent
 
@@ -188,15 +196,15 @@
 
         result = CompileResult(mcs_obj)
         return result
 
     def visit_BooleanNode(self, node, context: CompileContext) -> CompileResult:
         boolean: bool = node.get_value()
         mcs_obj = MCSBoolean(context)
-        value = "1b" if boolean is True else "0b"
+        value = "1" if boolean is True else "0"
 
         # add value creation command to compiled commands
         self.add_command(context.mcfunction_name, mcs_obj.save_to_storage_cmd(value))
 
         result = CompileResult(mcs_obj)
         return result
 
@@ -224,16 +232,15 @@
         if variable_value is None:
             context.declare(variable_name, MCSNull(context))
             return CompileResult()
 
         variable_value = self.visit(variable_value, context).get_value()
 
         commands = [
-            variable_value.set_to_current_cmd(context),
-            f"data modify storage mcs_{context.uuid} variable.{variable_name} set from storage mcs_{context.uuid} current"  # NOQA
+            f"data modify storage mcs_{context.uuid} variable.{variable_name} set from storage {variable_value.get_storage()} {variable_value.get_nbt()}",
         ]
         # garbage collect variable_value if it's not a variable (was only used to define current variable):
         if not isinstance(variable_value, MCSVariable):
             commands.append(variable_value.delete_from_storage_cmd())
         self.add_commands(context.mcfunction_name, commands)  # actually put the commands in the context file
 
         variable = MCSVariable(variable_name, context)  # create variable object to save in context
@@ -250,19 +257,16 @@
 
     def visit_VariableSetNode(self, node, context: CompileContext) -> CompileResult:
         var_name = node.get_name()
         new_value: mcs_type = self.visit(node.get_value(), context).get_value()
 
         owner_context = context.get_context_ownership(var_name)
 
-        commands = (
-            new_value.set_to_current_cmd(context),
-            f"data modify storage mcs_{owner_context.uuid} variable.{var_name} set from storage mcs_{context.uuid} current",  # NOQA
-        )
-        self.add_commands(context.mcfunction_name, commands)
+        command = f"data modify storage mcs_{owner_context.uuid} variable.{var_name} set from storage {new_value.get_storage()} {new_value.get_nbt()}"
+        self.add_command(context.mcfunction_name, command)
 
         return CompileResult()
 
     def visit_GetKeyNode(self, node, context: CompileContext) -> CompileResult:
         atom: mcs_type = self.visit(node.get_atom(), context).get_value()
         key: MCSNumber = self.visit(node.get_key(), context).get_value()
 
@@ -275,72 +279,84 @@
         )
 
         commands = (
             f"data modify storage mcs_{context.uuid} current set value " "{}",
             f"data modify storage mcs_{context.uuid} current.index set from storage {key.get_storage()} {key.get_nbt()}",
             f"function {self.datapack_id}:{local_context.mcfunction_name} with storage mcs_{context.uuid} current"
         )
+        commands = add_comment(commands, f"Get key (from {atom.get_nbt() !r})")
         self.add_commands(context.mcfunction_name, commands)
 
         return CompileResult(result)
 
     # ------------------ conditions & loops ------------------ :
     def visit_IfConditionNode(self, node, context: CompileContext) -> CompileResult:
         conditions: list[dict] = node.get_conditions()
+        local_context = CompileContext(parent=context)
+
+        init_commands = (
+            f"function {self.datapack_id}:{local_context.mcfunction_name}",  # runs the function with all conditional logic
+        )
+        init_commands = add_comment(init_commands, "If condition block")
+        self.add_commands(context.mcfunction_name, init_commands)
 
         for condition in conditions:
-            if condition.get('type') == 'if':
-                # create local context with all parent variables and create all body commands there
-                local_context = CompileContext(parent=context)
-                out: CompileResult = self.visit(condition.get('body'), local_context)
+            # create local context with all parent variables and create all body commands there
+            sublocal_context = CompileContext(parent=local_context)
+            out: CompileResult = self.visit(condition.get('body'), sublocal_context)
 
+            if condition.get('type') == 'if':
                 expression: MCSNumber = self.visit(condition.get('expression'), context).get_value()
                 commands = (
-                    expression.set_to_current_cmd(context),
-                    f"execute store result score .out mcs_math run data get storage mcs_{context.uuid} current 1",
-                    f"data modify storage mcs_{local_context.uuid} variable set from storage mcs_{context.uuid} variable",
-                    f"execute if score .out mcs_math matches 1 run function {self.datapack_id}:{local_context.mcfunction_name}"  # NOQA
+                    f"execute store result score .out mcs_math run data get storage {expression.get_storage()} {expression.get_nbt()} 1",
+                    f"data modify storage mcs_{sublocal_context.uuid} variable set from storage mcs_{context.uuid} variable",
+                    f"execute if score .out mcs_math matches 1 run function {self.datapack_id}:{sublocal_context.mcfunction_name}",
+                    f"execute if score .out mcs_math matches 1 run return 0",
                 )
-                self.add_commands(context.mcfunction_name, commands)
-
-                if out.get_return() is not None:
-                    return out
+                commands = add_comment(commands, "If condition:")
+                self.add_commands(local_context.mcfunction_name, commands)
 
             else:
-                out: CompileResult = self.visit(condition.get('body'), context)
-                if out.get_return() is not None:
-                    return out
+                commands = (
+                    f"function {self.datapack_id}:{sublocal_context.mcfunction_name}",
+                )
+                commands = add_comment(commands, "Else condition:")
+                self.add_commands(local_context.mcfunction_name, commands)
+
+            if out.get_return() is not None:
+                return out
 
         return CompileResult()
 
     def visit_ForLoopNode(self, node, context: CompileContext) -> CompileResult:
         iterable: MCSList = self.visit(node.get_iterable(), context).get_value()
         element_name: str = node.get_child_name()
         body = node.get_body()
 
         local_context = CompileContext(parent=context)
         macro_context = CompileContext(parent=context)
         loop_id = f"{generate_uuid()}"
 
         init_commands = (
             f"scoreboard players set .loop_iter_{loop_id} mcs_math 0",
-            iterable.set_to_current_cmd(context),
-            f"execute store result score .loop_end_{loop_id} mcs_math run data get storage mcs_{context.uuid} current.length 1",  # NOQA
+            f"execute store result score .loop_end_{loop_id} mcs_math run data get storage {iterable.get_storage()} {iterable.get_nbt()}.length 1",
             f"function {self.datapack_id}:{local_context.mcfunction_name}",
-            f"scoreboard players reset .loop_iter_{loop_id} mcs_math",  # remove to avoid clutter
+            # remove scoreboard values to avoid clutter:
+            f"scoreboard players reset .loop_iter_{loop_id} mcs_math",
             f"scoreboard players reset .loop_end_{loop_id} mcs_math",
         )
+        init_commands = add_comment(init_commands, f"For loop (variable {element_name !r})")
         self.add_commands(context.mcfunction_name, init_commands)
 
-        macro_cmd = f"$data modify storage mcs_{local_context.uuid} variable.{element_name} set from storage {iterable.get_storage()} {iterable.get_nbt()}.$(index)"  # NOQA
+        macro_cmd = f"$data modify storage mcs_{local_context.uuid} variable.{element_name} set from storage {iterable.get_storage()} {iterable.get_nbt()}.$(index)"
         self.add_command(macro_context.mcfunction_name, macro_cmd)
 
         loop_init_commands = (
-            f"execute store result storage mcs_{local_context.uuid} current.index int 1 run scoreboard players get .loop_iter_{loop_id} mcs_math",  # NOQA
-            f"function {self.datapack_id}:{macro_context.mcfunction_name} with storage mcs_{local_context.uuid} current",  # NOQA
+            f"execute store result storage mcs_{local_context.uuid} current.index int 1 run scoreboard players get .loop_iter_{loop_id} mcs_math",
+            f"function {self.datapack_id}:{macro_context.mcfunction_name} with storage mcs_{local_context.uuid} current",
         )
         self.add_commands(local_context.mcfunction_name, loop_init_commands)
         local_context.declare(element_name, MCSVariable(element_name, local_context))
 
         out: CompileResult = self.visit(body, local_context)  # add commands to code block
 
         loop_end_commands = (
@@ -353,26 +369,31 @@
             return out
 
         return CompileResult()
 
     def visit_WhileLoopNode(self, node, context: CompileContext) -> CompileResult:
         loop_context = CompileContext(parent=context)
 
-        out: CompileResult = self.visit(node.get_body(), loop_context)  # add commands to loop context file
+        # Start loop:
+        init_cmd = f"function {self.datapack_id}:{loop_context.mcfunction_name}"
+        if COMMON_CONFIG["debug_comments"] is True:
+            init_cmd = f"# Initialize while loop:\n{init_cmd}"
+        self.add_command(context.mcfunction_name, init_cmd)
 
+        # Add visit while loop body inside local context:
+        out: CompileResult = self.visit(node.get_body(), loop_context)
         condition: mcs_type = self.visit(node.get_condition(), loop_context).get_value()
+
         loop_commands = (
-            condition.set_to_current_cmd(loop_context),
-            f"execute store result score .out mcs_math run data get storage mcs_{loop_context.uuid} current 1",
-            f"execute if score .out mcs_math matches 1 run function {self.datapack_id}:{loop_context.mcfunction_name}",  # NOQA
+            f"execute store result score .out mcs_math run data get storage {condition.get_storage()} {condition.get_nbt()} 1",
+            f"execute if score .out mcs_math matches 1 run function {self.datapack_id}:{loop_context.mcfunction_name}",
         )
+        loop_commands = add_comment(loop_commands, f"While loop:")
         self.add_commands(loop_context.mcfunction_name, loop_commands)
 
-        self.add_command(context.mcfunction_name, f"function {self.datapack_id}:{loop_context.mcfunction_name}")  # NOQA
-
         return out if out.get_return() is not None else CompileResult()
 
     # ------------------ scope nodes ------------------ :
     def visit_MultilineCodeNode(self, node, context: CompileContext) -> CompileResult:
         for statement in node.get_nodes():
             return_value: CompileResult = self.visit(statement, context)
 
@@ -387,25 +408,27 @@
         return_value: CompileResult = self.visit(node.get_body(), local_context)
 
         # import parent context's variables and execute code block:
         commands = (
             f"data modify storage mcs_{local_context.uuid} variable set from storage mcs_{context.uuid} variable",
             f"function {self.datapack_id}:{local_context.mcfunction_name}"
         )
+        commands = add_comment(commands, f"Code block (parent: {context.mcfunction_name !r})")
         self.add_commands(context.mcfunction_name, commands)  # add commands to parent context
 
         return return_value
 
     def visit_FunctionCallNode(self, node, context: CompileContext) -> CompileResult:
         fnc: MCSFunction = self.visit(node.get_root(), context).get_value()
         arguments: tuple[mcs_type, ...] = tuple(map(lambda x: self.visit(x, context).get_value(), node.get_arguments()))
 
         commands, return_value = fnc.call(self, arguments, context)
 
         if commands is not None:
+            commands = add_comment(tuple(commands), "Function call")
             self.add_commands(context.mcfunction_name, commands)
 
         return CompileResult(return_value)
 
     # ------------------ minecraft stuff ------------------ :
     def visit_EntitySelectorNode(self, node, context: CompileContext) -> CompileResult:
         selector: str = node.get_selector()
@@ -413,37 +436,54 @@
 
         out: CompileResult = self.visit(node.get_statement(), local_context)  # add commands to local context
 
         setup_commands = (
             f"data modify storage mcs_{local_context.uuid} variable set from storage mcs_{context.uuid} variable",
             f"execute as @{selector} at @s run function {self.datapack_id}:{local_context.mcfunction_name}",  # NOQA
         )
+        commands = add_comment(setup_commands, f"Entity selector {selector !r}")
         self.add_commands(context.mcfunction_name, setup_commands)
 
         return out if out.get_return() is not None else CompileResult()
 
-    # ------------------ miscellaneous ------------------ :
+    # ------------------ Operations ------------------ :
     def visit_BinaryOperationNode(self, node, context: CompileContext) -> CompileResult:
         left_value: mcs_type = self.visit(node.get_left_node(), context).get_value()
         right_value: mcs_type = self.visit(node.get_right_node(), context).get_value()
         operation: str = node.get_operator().variant.lower()  # 'add', 'subtract', etc...
         result: mcs_type = MCSNumber(context)
 
         commands = (
-            left_value.set_to_current_cmd(context),
-            f"execute store result score .a mcs_math run data get storage mcs_{context.uuid} current",
-            right_value.set_to_current_cmd(context),
-            f"execute store result score .b mcs_math run data get storage mcs_{context.uuid} current",
+            f"execute store result score .a mcs_math run data get storage {left_value.get_storage()} {left_value.get_nbt()}",
+            f"execute store result score .b mcs_math run data get storage {right_value.get_storage()} {right_value.get_nbt()}",
             f"function {self.datapack_id}:math/{operation}",
-            f"execute store result storage mcs_{context.uuid} {result.get_nbt()} int 1 run scoreboard players get .out mcs_math",  # NOQA
+            f"execute store result storage mcs_{context.uuid} {result.get_nbt()} int 1 run scoreboard players get .out mcs_math",
         )
+        commands = add_comment(commands, f"Binary Operation {operation !r}")
         self.add_commands(context.mcfunction_name, commands)
 
         return CompileResult(result)
 
+    def visit_UnaryOperationNode(self, node, context: CompileContext) -> CompileResult:
+        operation = f"u_{node.get_operator()}"
+        root: mcs_type = self.visit(node.get_root(), context).get_value()
+
+        result = MCSBoolean(context)
+
+        commands = (
+            f"execute store result score .a mcs_math run data get storage {root.get_storage()} {root.get_nbt()}",
+            f"function {self.datapack_id}:math/{operation}",
+            f"execute store result storage {result.get_storage()} {result.get_nbt()} int 1 run scoreboard players get .out mcs_math",
+        )
+        commands = add_comment(commands, f"Unary Operation {operation !r}")
+        self.add_commands(context.mcfunction_name, commands)
+
+        return CompileResult(result)
+
+    # ------------------ miscellaneous ------------------ :
     @staticmethod
     def visit_unknown(node, context):
         raise ValueError(f'Unknown node {node !r}')
 
     def __repr__(self) -> str:
         return "CompileInterpreter()"
```

### Comparing `minecraft_script-0.2.0/minecraft_script/compiler/compile_types.py` & `minecraft_script-0.2.1/minecraft_script/compiler/compile_types.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/compiler/compiler.py` & `minecraft_script-0.2.1/minecraft_script/compiler/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
         self.import_builtins_files()
         if verbose:
             print('\rBuilding built-in functions... 83%', end="")
 
         self.make_click_item_check_file()
         if verbose:
-            print('\rBuilding builtin-in functions... Done!', end="")
+            print('\rBuilding builtin-in functions... Done!')
 
     def build(self, verbose: bool = True):
         start_time = time()  # keep track of start time
 
         if verbose:
             print(f'Building with name "{self.datapack_name}" (id: "{self.datapack_id}")')
```

### Comparing `minecraft_script-0.2.0/minecraft_script/errors.py` & `minecraft_script-0.2.1/minecraft_script/errors.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/interpreter/builtin_functions.py` & `minecraft_script-0.2.1/minecraft_script/interpreter/builtin_functions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/interpreter/interpreter.py` & `minecraft_script-0.2.1/minecraft_script/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/interpreter/types.py` & `minecraft_script-0.2.1/minecraft_script/interpreter/types.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/lexer/grammar/LANG_TOKENS.json` & `minecraft_script-0.2.1/minecraft_script/lexer/grammar/LANG_TOKENS.json`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/lexer/lexer.py` & `minecraft_script-0.2.1/minecraft_script/lexer/lexer.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         else:
             self.position_x += 1
 
     @property
     def next_char(self) -> str | None:
         return self.code_input[self.current_index + 1] if self.current_index < len(self.code_input) - 2 else None
 
+    # ---------------- Special cases ---------------- :
     def make_number(self) -> Token:
         number = self.current_char
         position = (self.position_x, self.position_y)
         self.advance()
 
         while self.current_char in token_type_chars['TT_NUMBER']:
             number += self.current_char
@@ -91,14 +92,40 @@
 
         if self.current_char is None:
             raise MCSSyntaxError(f'Unmatched string starting at line {position[1]}, {position[0]}')
         self.advance()  # skip closing string quote
 
         return Token(string, 'TT_STRING', position)
 
+    def make_entity_selector(self) -> Token:
+        selector = self.current_char  # should be "@" char
+        self.advance()
+
+        position = self.position_x, self.position_y
+        depth = 0
+
+        while self.current_char is not None and not (depth == 0 and self.current_char == ' '):
+            if self.current_char == '[':
+                depth += 1
+            elif self.current_char == ']':
+                depth -= 1
+
+            if depth < 0:
+                raise MCSSyntaxError(f'Malformed entity selector at line {position[1]}, {position[0]}')
+
+            selector += self.current_char
+            self.advance()
+
+        if self.current_char is None:
+            raise MCSSyntaxError(f'Malformed entity selector at line {position[1]}, {position[0]}')
+        self.advance()  # skip space (is going to get skipped anyway)
+
+        return Token(selector, 'TT_SELECTOR', position)
+
+    # ---------------- Main implementation (turning code into tokens) ---------------- :
     def default_tokenize_treatment(self) -> None:
         position = (self.position_x, self.position_y)
 
         advance_needed = True if self.next_char is not None else False  # If token is composed, advance is needed
         token_value = self.current_char + self.next_char if self.next_char is not None else self.current_char
         token_type = token_lookup_table.get(token_value)  # try with composed token first (priority to composed tokens)
 
@@ -137,14 +164,17 @@
 
             elif self.current_char in token_type_chars['TT_NAME']:
                 self.__token_list.append(self.make_name())
 
             elif self.current_char in token_type_chars['TT_QUOTE']:
                 self.__token_list.append(self.make_string())
 
+            elif self.current_char in token_type_chars['TT_AT']:
+                self.__token_list.append(self.make_entity_selector())
+
             elif self.next_char is not None and self.current_char + self.next_char in token_type_chars['TT_COMMENT']:
                 self.advance()  # skip second "/" (self.next_char)
                 while self.current_char is not None and self.current_char != "\n":
                     self.advance()  # skip everything until newline (it's a comment)
 
             else:
                 self.default_tokenize_treatment()
```

### Comparing `minecraft_script-0.2.0/minecraft_script/lexer/tokens.py` & `minecraft_script-0.2.1/minecraft_script/lexer/tokens.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/parser/nodes.py` & `minecraft_script-0.2.1/minecraft_script/parser/nodes.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script/parser/parser.py` & `minecraft_script-0.2.1/minecraft_script/parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
         elif self.current_token.matches('TT_WHILE_LOOP'):
             return self.while_loop()
 
         elif self.current_token.matches('TT_FOR_LOOP'):
             return self.for_loop()
 
-        elif self.current_token.matches('TT_AT'):
+        elif self.current_token.matches('TT_SELECTOR'):
             return self.entity_selector()
 
         return self.code_block_statement()
 
     def multiline_code(self, *, expect_end: bool = False) -> MultilineCodeNode:
         position = self.current_token.get_position()
 
@@ -507,26 +507,13 @@
             self.raise_error(f"Expected name, got {self.current_token.value !r}")
         name = self.current_token
 
         self.advance()
         return AttributeGetNode(root, name)
 
     def entity_selector(self) -> EntitySelectorNode:
-        position = self.current_token.get_position()
-        self.advance()  # skip '@'
-
-        if not self.current_token.matches('TT_NAME'):
-            self.raise_error(f"Expected name, got {self.current_token.value !r}")
-        selector = self.current_token.value  # save string, not token
+        selector_token = self.current_token
         self.advance()
 
-        if self.current_token.matches('TT_BRACKET', 'LEFT'):
-            while not self.current_token.matches('TT_BRACKET', 'RIGHT'):
-                selector += self.current_token.value
-                self.advance()
-
-            selector += self.current_token.value  # add "]" to selector
-            self.advance()
-
         statement = self.statement()
 
-        return EntitySelectorNode(selector, statement, position)
+        return EntitySelectorNode(selector_token.value, statement, selector_token.get_position())
```

### Comparing `minecraft_script-0.2.0/minecraft_script/shell_commands.py` & `minecraft_script-0.2.1/minecraft_script/shell_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from . import debug_code
 from .compiler import build_datapack
-from .common import COMMON_CONFIG, update_config, version
+from .common import COMMON_CONFIG, version
+from .config_utils import update_config
 
 
 def handle_arguments(arguments: list):
     if not arguments:
         sh_default()
 
     function_name = arguments.pop(0)
@@ -77,16 +78,23 @@
     )
     verbose: bool = (
         True
         if arg_count < 3 else
         args[2].lower() == 'true'
     )
 
-    with open(path, 'rt', encoding='utf-8') as file:
-        code = file.read()
+    try:
+        file = open(path, 'rt', encoding='utf-8')
+
+    except FileNotFoundError:
+        print(f"Error: Could not find file at {path !r}")
+        exit(-1)
+
+    code = file.read()
+    file.close()
 
     build_datapack(code, datapack_name, verbose)
 
 
 def sh_config(*args):
     arg_count = len(args)
     args = list(args)
@@ -111,33 +119,35 @@
     value = args[1]
 
     if setting not in COMMON_CONFIG.keys():
         print(f"Unknown setting {setting !r}.")
         exit()
 
     update_config(setting, value)
-    print(f"Updated setting {setting !r} to value {value !r}")
+    print(f"Updated setting {setting !r} to value {value}")
 
 
 def sh_config_get(args: list):
     if len(args) < 1:
         print("Minecraft Script configuration:")
         for setting, value in COMMON_CONFIG.items():
-            print(f"- {setting}: {value !r}")
+            print(f"- {setting}: {value}")
         exit()
 
     setting = args[0]
-    value = COMMON_CONFIG.get(setting)
-    if value is not None:
-        print(
-            f"Setting {setting !r} has the following value: \n"
-            f"{value !r}"
-        )
-    else:
+    value: any = COMMON_CONFIG.get(setting)
+
+    if value is None:
         print(f"Unknown setting {setting !r}.")
+        exit()
+
+    print(
+        f"Setting {setting !r} has the following value: \n"
+        f"{value !r}"
+    )
 
 
 shell_functions = {
     'help': sh_help,
     'debug': sh_debug,
     'compile': sh_compile,
     'config': sh_config,
```

### Comparing `minecraft_script-0.2.0/minecraft_script/text_additions.py` & `minecraft_script-0.2.1/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.2.0/minecraft_script.egg-info/PKG-INFO` & `minecraft_script-0.2.1/minecraft_script.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.2.0
+Version: 0.2.1
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <christophe@dronne.fr>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -35,32 +35,32 @@
 
 
 ## Using Minecraft Script to make Datapacks
 ### Debugging your program
 To debug your program, you can first run your file like any other programming language.
 To do this, use the following command:
 ```commandline
-python -m minecraft_script run [file]
+python -m minecraft_script debug <path>
 ```
-_where [file] is a relative or absolute path to your mcs file_
+_where <path> is a relative or absolute path to your mcs file_
 
 ### Building your datapack
 To actually build your minecraft datapack, which you can then simply drag & drop into your
 minecraft worlds, use the following command:
 ```commandline
-python -m minecraft_script build [file]
+python -m minecraft_script compile <path>
 ```
-_where [file] is a relative or absolute path to your mcs file_
+_where <path> is a relative or absolute path to your mcs file_
 
 ### More info
 For a list of all shell commands, you can use the following command:
 ```commandline
 python -m minecraft_script help
 ```
-If you want to simplify the usage of shell commands, you can check out [the installations page in the documentation](https://github.com/Bard-Gaming/Minecraft-Script/blob/main/documentation/installations.md).
+If you want to simplify the usage of shell commands, you can check out [the installations page in the documentation](https://github.com/Bard-Gaming/Minecraft-Script/blob/main/documentation/custom-installations.md).
 
 ## GitHub
 [**Link to GitHub Repository**](https://github.com/Bard-Gaming/Minecraft-Script)
 
 Source code, documentation, and examples, can all be found on the GitHub.
 
 ## Compatibility
```

### Comparing `minecraft_script-0.2.0/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.2.1/minecraft_script.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 setup.py
 minecraft_script/__init__.py
 minecraft_script/__main__.py
 minecraft_script/common.py
 minecraft_script/config.json
+minecraft_script/config_utils.py
 minecraft_script/errors.py
 minecraft_script/shell_commands.py
 minecraft_script/text_additions.py
 minecraft_script.egg-info/PKG-INFO
 minecraft_script.egg-info/SOURCES.txt
 minecraft_script.egg-info/dependency_links.txt
 minecraft_script.egg-info/top_level.txt
@@ -28,14 +29,17 @@
 minecraft_script/compiler/build_templates/math/greater_equals_than.mcfunction
 minecraft_script/compiler/build_templates/math/greater_than.mcfunction
 minecraft_script/compiler/build_templates/math/less_equals_than.mcfunction
 minecraft_script/compiler/build_templates/math/less_than.mcfunction
 minecraft_script/compiler/build_templates/math/modulus.mcfunction
 minecraft_script/compiler/build_templates/math/multiply.mcfunction
 minecraft_script/compiler/build_templates/math/subtract.mcfunction
+minecraft_script/compiler/build_templates/math/u_add.mcfunction
+minecraft_script/compiler/build_templates/math/u_not.mcfunction
+minecraft_script/compiler/build_templates/math/u_subtract.mcfunction
 minecraft_script/compiler/build_templates/tags/blocks/no_collision.json
 minecraft_script/interpreter/__init__.py
 minecraft_script/interpreter/builtin_functions.py
 minecraft_script/interpreter/interpreter.py
 minecraft_script/interpreter/types.py
 minecraft_script/lexer/__init__.py
 minecraft_script/lexer/lexer.py
```

### Comparing `minecraft_script-0.2.0/setup.py` & `minecraft_script-0.2.1/setup.py`

 * *Files identical despite different names*

