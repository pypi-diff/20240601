# Comparing `tmp/django_typer-1.1.2.tar.gz` & `tmp/django_typer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_typer-1.1.2.tar", max compression
+gzip compressed data, was "django_typer-2.0.0.tar", max compression
```

## Comparing `django_typer-1.1.2.tar` & `django_typer-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,95 @@
--rw-r--r--   0        0        0     1068 2024-03-14 23:09:15.471852 django_typer-1.1.2/LICENSE
--rw-r--r--   0        0        0     8170 2024-04-11 18:48:40.869937 django_typer-1.1.2/README.md
--rw-r--r--   0        0        0    81845 2024-04-22 20:59:04.110791 django_typer-1.1.2/django_typer/__init__.py
--rw-r--r--   0        0        0     3374 2024-04-11 18:48:40.871353 django_typer-1.1.2/django_typer/apps.py
--rw-r--r--   0        0        0    16547 2024-03-14 23:09:15.472439 django_typer-1.1.2/django_typer/completers.py
--rw-r--r--   0        0        0        0 2024-03-14 23:09:15.474628 django_typer-1.1.2/django_typer/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 23:09:15.474707 django_typer-1.1.2/django_typer/management/commands/__init__.py
--rw-r--r--   0        0        0    26891 2024-04-03 18:21:16.067895 django_typer-1.1.2/django_typer/management/commands/shellcompletion.py
--rw-r--r--   0        0        0     7195 2024-03-14 23:09:15.474929 django_typer-1.1.2/django_typer/parsers.py
--rw-r--r--   0        0        0     5659 2024-04-03 18:21:16.068517 django_typer-1.1.2/django_typer/patch.py
--rw-r--r--   0        0        0        0 2024-03-14 23:09:15.475040 django_typer-1.1.2/django_typer/py.typed
--rw-r--r--   0        0        0     6055 2024-03-14 23:09:15.487659 django_typer-1.1.2/django_typer/types.py
--rw-r--r--   0        0        0     2828 2024-03-18 04:57:08.074572 django_typer-1.1.2/django_typer/utils.py
--rw-r--r--   0        0        0     5626 2024-04-22 20:59:04.112873 django_typer-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     9974 1970-01-01 00:00:00.000000 django_typer-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-10-24 04:20:22.142156 django_typer-2.0.0/LICENSE
+-rw-r--r--   0        0        0    11879 2024-05-30 15:54:12.104764 django_typer-2.0.0/README.md
+-rw-r--r--   0        0        0   127370 2024-06-01 00:35:51.255668 django_typer-2.0.0/django_typer/__init__.py
+-rw-r--r--   0        0        0     3344 2024-05-15 04:36:56.651523 django_typer-2.0.0/django_typer/apps.py
+-rw-r--r--   0        0        0    24715 2024-06-01 00:35:51.256316 django_typer-2.0.0/django_typer/completers.py
+-rw-r--r--   0        0        0        0 2024-01-14 22:24:15.916200 django_typer-2.0.0/django_typer/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-14 22:25:15.612846 django_typer-2.0.0/django_typer/management/commands/__init__.py
+-rw-r--r--   0        0        0    26904 2024-05-30 04:36:55.696471 django_typer-2.0.0/django_typer/management/commands/shellcompletion.py
+-rw-r--r--   0        0        0     7655 2024-05-15 04:36:56.655851 django_typer-2.0.0/django_typer/parsers.py
+-rw-r--r--   0        0        0     5669 2024-05-15 04:36:56.656294 django_typer-2.0.0/django_typer/patch.py
+-rw-r--r--   0        0        0        0 2024-03-04 21:09:02.017478 django_typer-2.0.0/django_typer/py.typed
+-rw-r--r--   0        0        0     6209 2024-05-15 04:36:56.681201 django_typer-2.0.0/django_typer/types.py
+-rw-r--r--   0        0        0     6757 2024-06-01 00:35:51.265077 django_typer-2.0.0/django_typer/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 06:14:15.937093 django_typer-2.0.0/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.657535 django_typer-2.0.0/examples/basic/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-22 05:48:46.639465 django_typer-2.0.0/examples/basic/apps.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.657673 django_typer-2.0.0/examples/basic/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.657741 django_typer-2.0.0/examples/basic/management/commands/__init__.py
+-rw-r--r--   0        0        0      211 2024-02-22 09:12:43.593968 django_typer-2.0.0/examples/basic/management/commands/basic.py
+-rw-r--r--   0        0        0     1343 2024-05-15 04:36:56.653212 django_typer-2.0.0/examples/basic/management/commands/hierarchy.py
+-rw-r--r--   0        0        0      657 2024-05-22 18:17:52.664385 django_typer-2.0.0/examples/basic/management/commands/multi.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.270252 django_typer-2.0.0/examples/completers/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.270286 django_typer-2.0.0/examples/completers/apps.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.270346 django_typer-2.0.0/examples/completers/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.270407 django_typer-2.0.0/examples/completers/management/commands/__init__.py
+-rw-r--r--   0        0        0     1016 2024-06-01 00:35:51.270472 django_typer-2.0.0/examples/completers/management/commands/app_labels.py
+-rw-r--r--   0        0        0      932 2024-06-01 00:35:51.270530 django_typer-2.0.0/examples/completers/management/commands/app_labels_typer.py
+-rw-r--r--   0        0        0    25568 2024-04-04 03:07:57.238591 django_typer-2.0.0/examples/helps/basic.svg
+-rw-r--r--   0        0        0    22121 2024-04-04 03:07:57.239091 django_typer-2.0.0/examples/helps/hierarchy.svg
+-rw-r--r--   0        0        0    12138 2024-04-04 03:07:57.239677 django_typer-2.0.0/examples/helps/hierarchy_math.svg
+-rw-r--r--   0        0        0    12358 2024-04-04 03:07:57.240181 django_typer-2.0.0/examples/helps/hierarchy_math_divide.svg
+-rw-r--r--   0        0        0    10121 2024-04-04 03:07:57.240473 django_typer-2.0.0/examples/helps/hierarchy_math_multiply.svg
+-rw-r--r--   0        0        0    22963 2024-05-15 04:36:56.652828 django_typer-2.0.0/examples/helps/multi.svg
+-rw-r--r--   0        0        0    10147 2024-04-04 03:07:57.241722 django_typer-2.0.0/examples/helps/multi_create.svg
+-rw-r--r--   0        0        0    10130 2024-04-04 03:07:57.241918 django_typer-2.0.0/examples/helps/multi_delete.svg
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.270588 django_typer-2.0.0/examples/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.270652 django_typer-2.0.0/examples/plugins/backup/__init__.py
+-rw-r--r--   0        0        0      163 2024-06-01 00:35:51.270711 django_typer-2.0.0/examples/plugins/backup/apps.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.270772 django_typer-2.0.0/examples/plugins/backup/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.270849 django_typer-2.0.0/examples/plugins/backup/management/commands/__init__.py
+-rw-r--r--   0        0        0     4260 2024-06-01 00:35:51.270970 django_typer-2.0.0/examples/plugins/backup/management/commands/backup.py
+-rw-r--r--   0        0        0     3820 2024-06-01 00:35:51.271032 django_typer-2.0.0/examples/plugins/backup/management/commands/backup_typer.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.271089 django_typer-2.0.0/examples/plugins/media1/__init__.py
+-rw-r--r--   0        0        0      162 2024-06-01 00:35:51.271154 django_typer-2.0.0/examples/plugins/media1/apps.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.271219 django_typer-2.0.0/examples/plugins/media1/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.271291 django_typer-2.0.0/examples/plugins/media1/management/commands/__init__.py
+-rw-r--r--   0        0        0     1129 2024-06-01 00:35:51.271372 django_typer-2.0.0/examples/plugins/media1/management/commands/backup.py
+-rw-r--r--   0        0        0     1083 2024-06-01 00:35:51.271443 django_typer-2.0.0/examples/plugins/media1/management/commands/backup_typer.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.271504 django_typer-2.0.0/examples/plugins/media2/__init__.py
+-rw-r--r--   0        0        0      324 2024-06-01 00:35:51.271561 django_typer-2.0.0/examples/plugins/media2/apps.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.271617 django_typer-2.0.0/examples/plugins/media2/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.271682 django_typer-2.0.0/examples/plugins/media2/management/plugins/__init__.py
+-rw-r--r--   0        0        0     1128 2024-06-01 00:35:51.271750 django_typer-2.0.0/examples/plugins/media2/management/plugins/backup.py
+-rw-r--r--   0        0        0     1063 2024-06-01 00:35:51.271818 django_typer-2.0.0/examples/plugins/media2/management/plugins/backup_typer.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.271885 django_typer-2.0.0/examples/plugins/my_app/__init__.py
+-rw-r--r--   0        0        0      324 2024-06-01 00:35:51.271952 django_typer-2.0.0/examples/plugins/my_app/apps.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.272010 django_typer-2.0.0/examples/plugins/my_app/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:35:51.272074 django_typer-2.0.0/examples/plugins/my_app/management/plugins/__init__.py
+-rw-r--r--   0        0        0     1123 2024-06-01 00:35:51.272144 django_typer-2.0.0/examples/plugins/my_app/management/plugins/backup.py
+-rw-r--r--   0        0        0     1131 2024-06-01 00:35:51.272199 django_typer-2.0.0/examples/plugins/my_app/management/plugins/backup_typer.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.657922 django_typer-2.0.0/examples/polls/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-15 04:36:56.658186 django_typer-2.0.0/examples/polls/admin.py
+-rw-r--r--   0        0        0      153 2024-05-22 05:10:20.670503 django_typer-2.0.0/examples/polls/apps.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.658307 django_typer-2.0.0/examples/polls/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.658388 django_typer-2.0.0/examples/polls/management/commands/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-22 05:11:40.475666 django_typer-2.0.0/examples/polls/management/commands/add_polls.py
+-rw-r--r--   0        0        0      983 2024-05-22 18:17:52.664149 django_typer-2.0.0/examples/polls/management/commands/closepoll.py
+-rw-r--r--   0        0        0     1020 2024-05-22 05:12:02.802283 django_typer-2.0.0/examples/polls/management/commands/closepoll_django.py
+-rw-r--r--   0        0        0      811 2024-05-22 05:11:08.676314 django_typer-2.0.0/examples/polls/management/commands/closepoll_t1.py
+-rw-r--r--   0        0        0      729 2024-05-30 04:36:55.708879 django_typer-2.0.0/examples/polls/management/commands/closepoll_t1_typer.py
+-rw-r--r--   0        0        0     1101 2024-05-30 04:36:55.709002 django_typer-2.0.0/examples/polls/management/commands/closepoll_t2.py
+-rw-r--r--   0        0        0      999 2024-05-30 04:36:55.709058 django_typer-2.0.0/examples/polls/management/commands/closepoll_t2_typer.py
+-rw-r--r--   0        0        0     1644 2024-05-30 05:22:22.823183 django_typer-2.0.0/examples/polls/management/commands/closepoll_t3.py
+-rw-r--r--   0        0        0     1498 2024-05-30 05:24:10.723694 django_typer-2.0.0/examples/polls/management/commands/closepoll_t3_typer.py
+-rw-r--r--   0        0        0     1282 2024-05-30 04:36:55.709341 django_typer-2.0.0/examples/polls/management/commands/closepoll_t4.py
+-rw-r--r--   0        0        0     1104 2024-05-30 04:36:55.709411 django_typer-2.0.0/examples/polls/management/commands/closepoll_t4_typer.py
+-rw-r--r--   0        0        0     1413 2024-05-30 04:36:55.709525 django_typer-2.0.0/examples/polls/management/commands/closepoll_t5.py
+-rw-r--r--   0        0        0     1276 2024-05-30 04:36:55.709591 django_typer-2.0.0/examples/polls/management/commands/closepoll_t5_typer.py
+-rw-r--r--   0        0        0     1007 2024-05-30 04:36:55.709706 django_typer-2.0.0/examples/polls/management/commands/closepoll_t6.py
+-rw-r--r--   0        0        0      906 2024-05-30 04:36:55.709779 django_typer-2.0.0/examples/polls/management/commands/closepoll_t6_typer.py
+-rw-r--r--   0        0        0      867 2024-05-30 04:36:55.709836 django_typer-2.0.0/examples/polls/management/commands/closepoll_typer.py
+-rw-r--r--   0        0        0     1004 2024-05-22 05:12:11.920891 django_typer-2.0.0/examples/polls/management/commands/poll_as_option.py
+-rw-r--r--   0        0        0     1842 2024-05-22 18:53:14.366965 django_typer-2.0.0/examples/polls/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.659034 django_typer-2.0.0/examples/polls/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2024-05-22 18:52:27.170246 django_typer-2.0.0/examples/polls/models.py
+-rw-r--r--   0        0        0       17 2024-05-15 04:36:56.659473 django_typer-2.0.0/examples/polls/urls.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.675678 django_typer-2.0.0/examples/typer/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-22 04:55:20.452780 django_typer-2.0.0/examples/typer/apps.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.675808 django_typer-2.0.0/examples/typer/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:36:56.675872 django_typer-2.0.0/examples/typer/management/commands/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-15 04:36:56.654739 django_typer-2.0.0/examples/typer/management/commands/basic.py
+-rw-r--r--   0        0        0     1238 2024-05-22 18:17:52.664469 django_typer-2.0.0/examples/typer/management/commands/hierarchy.py
+-rw-r--r--   0        0        0      507 2024-05-22 18:17:52.664332 django_typer-2.0.0/examples/typer/management/commands/multi.py
+-rw-r--r--   0        0        0     5621 2024-05-30 04:36:55.710334 django_typer-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13683 1970-01-01 00:00:00.000000 django_typer-2.0.0/PKG-INFO
```

### Comparing `django_typer-1.1.2/LICENSE` & `django_typer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_typer-1.1.2/README.md` & `django_typer-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # django-typer
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI version](https://badge.fury.io/py/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
 [![PyPI djversions](https://img.shields.io/pypi/djversions/django-typer.svg)](https://pypi.org/project/django-typer/)
 [![PyPI status](https://img.shields.io/pypi/status/django-typer.svg)](https://pypi.python.org/pypi/django-typer)
 [![Documentation Status](https://readthedocs.org/projects/django-typer/badge/?version=latest)](http://django-typer.readthedocs.io/?badge=latest/)
 [![Code Cov](https://codecov.io/gh/bckohan/django-typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://codecov.io/gh/bckohan/django-typer)
 [![Test Status](https://github.com/bckohan/django-typer/workflows/test/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/test.yml)
 [![Lint Status](https://github.com/bckohan/django-typer/workflows/lint/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/lint.yml)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Use [Typer](https://typer.tiangolo.com/) to define the CLI for your [Django](https://www.djangoproject.com/) management commands. Provides a TyperCommand class that inherits from [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) and allows typer-style annotated parameter types. All of the BaseCommand functionality is preserved, so that TyperCommand can be a drop-in replacement.
+Use static typing to define the CLI for your [Django](https://www.djangoproject.com/) management commands with [Typer](https://typer.tiangolo.com/). Optionally use the provided [TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) class that inherits from [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand). This class maps the [Typer](https://typer.tiangolo.com/) interface onto a class based interface that Django developers will be familiar with. All of the [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) functionality is preserved, so that [TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) can be a drop in replacement.
 
 **django-typer makes it easy to:**
 
-- Define your command CLI interface in a clear, DRY, and safe way using type hints.
-- Create subcommand and group command hierarchies.
-- Use the full power of Typer's parameter types to validate and parse command line inputs.
-- Create beautiful and information dense help outputs.
-- Configure the rendering of exception stack traces using rich.
-- [Install shell tab-completion support](https://django-typer.readthedocs.io/en/latest/shell_completion.html) for TyperCommands and normal Django commands for [bash](https://www.gnu.org/software/bash/), [zsh](https://www.zsh.org/), [fish](https://fishshell.com/), and [powershell](https://learn.microsoft.com/en-us/powershell/scripting/overview).
-- [Create custom and portable shell tab-completions for your CLI parameters.](https://django-typer.readthedocs.io/en/latest/shell_completion.html#defining-custom-completions)
-- Refactor existing management commands into TyperCommands because TyperCommand is interface compatible with BaseCommand.
+   * Define your command CLI interface in a clear, DRY and safe way using type hints
+   * Create subcommands and hierarchical groups of commands.
+   * Use the full power of [Typer](https://typer.tiangolo.com/)'s parameter types to validate and parse command line inputs.
+   * Create beautiful and information dense help outputs.
+   * Configure the rendering of exception stack traces using [rich](https://rich.readthedocs.io/en/latest/).
+   * [Install shell tab-completion support](https://django-typer.readthedocs.io/en/latest/shell_completion.html) for [bash](https://www.gnu.org/software/bash/), [zsh](https://www.zsh.org/), [fish](https://fishshell.com/), and [powershell](https://learn.microsoft.com/en-us/powershell/scripting/overview).
+   * [Create custom and portable shell tab-completions for your CLI parameters.](https://django-typer.readthedocs.io/en/latest/shell_completion.html#defining-custom-completions)
+   * Port existing commands ([TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) is interface compatible with [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand)).
+   * Use either a Django-style class-based interface or the Typer-style interface to define commands.
+   * Add plugins to upstream commands.
 
 Please refer to the [full documentation](https://django-typer.readthedocs.io/) for more information.
 
 ![django-typer example](https://raw.githubusercontent.com/bckohan/django-typer/main/doc/source/_static/img/closepoll_example.gif)
 
 ## Installation
 
@@ -39,39 +41,53 @@
 
    [rich](https://rich.readthedocs.io/en/latest/) is a powerful library for rich text and beautiful formatting in the terminal. It is not required but highly recommended for the best experience:
 
    ```bash
    pip install "django-typer[rich]"
    ```
 
-2. Add `django_typer` to your `INSTALLED_APPS` setting:
+2. Optionally add `django_typer` to your `INSTALLED_APPS` setting:
 
    ```python
    INSTALLED_APPS = [
        ...
        'django_typer',
    ]
    ```
 
 *You only need to install django_typer as an app if you want to use the shell completion command to enable tab-completion or if you would like django-typer to install [rich traceback rendering](https://django-typer.readthedocs.io/en/latest/howto.html#configure-rich-stack-traces) for you - which it does by default if rich is also installed.*
 
 ## Basic Example
 
-For example, TyperCommands can be a very simple drop-in replacement for BaseCommands. All of the documented features of [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) work!
+[TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) is a very simple drop in replacement for [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand). All of the documented features of [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) work the same way!
 
 ```python
 from django_typer import TyperCommand
 
 class Command(TyperCommand):
     def handle(self, arg1: str, arg2: str, arg3: float = 0.5, arg4: int = 1):
         """
         A basic command that uses Typer
         """
 ```
 
+Or, you may also use an interface identical to [Typer](https://typer.tiangolo.com/)'s. Simply import [Typer](https://typer.tiangolo.com/) from django_typer instead of typer.
+
+```python
+from django_typer import Typer
+
+app = Typer()
+
+@app.command()
+def main(arg1: str, arg2: str, arg3: float = 0.5, arg4: int = 1):
+   """
+   A basic command that uses Typer
+   """
+```
+
 ![Basic Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/basic.svg)
 
 ## Multiple Subcommands Example
 
 
 
 Commands with multiple subcommands can be defined:
@@ -105,27 +121,57 @@
       ):
          """
          Delete an object.
          """
 
 ```
 
+Or using the typer-style interface this could be written:
+
+```python
+from django_typer import Typer
+import typing as t
+
+from django.utils.translation import gettext_lazy as _
+from typer import Argument
+
+app = Typer(help="A command that defines subcommands.")
+
+@app.command()
+def create(
+   name: t.Annotated[str, Argument(help=_("The name of the object to create."))],
+):
+   """
+   Create an object.
+   """
+
+@app.command()
+def delete(
+   id: t.Annotated[int, Argument(help=_("The id of the object to delete."))]
+):
+   """
+   Delete an object.
+   """
+```
+
 ![Multiple Subcommands Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi.svg)
 ![Multiple Subcommands Example - create](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_create.svg)
 ![Multiple Subcommands Example - delete](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_delete.svg)
 
 ## Grouping and Hierarchies Example
 
 More complex groups and subcommand hierarchies can be defined. For example, this command defines a group of commands called math, with subcommands divide and multiply. The group has a common initializer that optionally sets a float precision value. We would invoke this command like so:
 
 ```bash
 ./manage.py hierarchy math --precision 5 divide 10 2.1
 ./manage.py hierarchy math multiply 10 2
 ```
 
+Using the class-based interface we could define the command like this:
+
 ```python
    import typing as t
    from functools import reduce
 
    from django.utils.translation import gettext_lazy as _
    from typer import Argument, Option
 
@@ -143,23 +189,26 @@
          self,
          precision: t.Annotated[
             int, Option(help=_("The number of decimal places to output."))
          ] = precision,
       ):
          self.precision = precision
 
+      # helps can be passed to the decorators
       @math.command(help=_("Multiply the given numbers."))
       def multiply(
          self,
          numbers: t.Annotated[
             t.List[float], Argument(help=_("The numbers to multiply"))
          ],
       ):
          return f"{reduce(lambda x, y: x * y, [1, *numbers]):.{self.precision}f}"
 
+      # or if no help is supplied to the decorators, the docstring if present
+      # will be used!
       @math.command()
       def divide(
          self,
          numerator: t.Annotated[float, Argument(help=_("The numerator"))],
          denominator: t.Annotated[float, Argument(help=_("The denominator"))],
          floor: t.Annotated[bool, Option(help=_("Use floor division"))] = False,
       ):
@@ -168,11 +217,65 @@
          """
          if floor:
                return str(numerator // denominator)
          return f"{numerator / denominator:.{self.precision}f}"
 
 ```
 
+The typer-style interface builds a [TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) class for us **that allows you to optionally accept the self argument in your commands.** We could define the above command using the typer interface like this:
+
+```python
+
+import typing as t
+from functools import reduce
+
+from django.utils.translation import gettext_lazy as _
+from typer import Argument, Option
+
+from django_typer import Typer
+
+
+app = Typer(help=_("A more complex command that defines a hierarchy of subcommands."))
+
+
+math_grp = Typer(help=_("Do some math at the given precision."))
+
+app.add_typer(math_grp)
+
+@math_grp.callback()
+def math(
+   self,
+   precision: t.Annotated[
+      int, Option(help=_("The number of decimal places to output."))
+   ] = 2,
+):
+   self.precision = precision
+
+
+@math_grp.command(help=_("Multiply the given numbers."))
+def multiply(
+   self,
+   numbers: t.Annotated[
+      t.List[float], Argument(help=_("The numbers to multiply"))
+   ],
+):
+   return f"{reduce(lambda x, y: x * y, [1, *numbers]):.{self.precision}f}"
+
+@math_grp.command()
+def divide(
+   self,
+   numerator: t.Annotated[float, Argument(help=_("The numerator"))],
+   denominator: t.Annotated[float, Argument(help=_("The denominator"))],
+   floor: t.Annotated[bool, Option(help=_("Use floor division"))] = False,
+):
+   """
+   Divide the given numbers.
+   """
+   if floor:
+         return str(numerator // denominator)
+   return f"{numerator / denominator:.{self.precision}f}"
+```
+
 ![Grouping and Hierarchies Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy.svg)
 ![Grouping and Hierarchies Example - math](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math.svg)
 ![Grouping and Hierarchies Example - math multiply](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_multiply.svg)
 ![Grouping and Hierarchies Example - math divide](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_divide.svg)
```

### Comparing `django_typer-1.1.2/django_typer/__init__.py` & `django_typer-2.0.0/django_typer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 r"""
 ::
 
-      ___ _                           _____                       
-     /   (_) __ _ _ __   __ _  ___   /__   \_   _ _ __   ___ _ __ 
+      ___ _                           _____
+     /   (_) __ _ _ __   __ _  ___   /__   \_   _ _ __   ___ _ __
     / /\ / |/ _` | '_ \ / _` |/ _ \    / /\/ | | | '_ \ / _ \ '__|
-   / /_//| | (_| | | | | (_| | (_) |  / /  | |_| | |_) |  __/ |   
-  /___,'_/ |\__,_|_| |_|\__, |\___/   \/    \__, | .__/ \___|_|   
-       |__/             |___/               |___/|_|              
+   / /_//| | (_| | | | | (_| | (_) |  / /  | |_| | |_) |  __/ |
+  /___,'_/ |\__,_|_| |_|\__, |\___/   \/    \__, | .__/ \___|_|
+       |__/             |___/               |___/|_|
 
 
-django-typer_ provides an extension class, :class:`~django_typer.TyperCommand`, to the 
+django-typer_ provides an extension class, :class:`~django_typer.TyperCommand`, to the
 BaseCommand_ class that melds the Typer_/click_ infrastructure with
 the Django_ infrastructure. The result is all the ease of specifying commands, groups
 and options and arguments using Typer_ and click_ in a way that feels like and is
 interface compatible with Django_'s BaseCommand_ This should enable a smooth transition
 for existing Django_ commands and an intuitive feel for implementing new commands.
 
 django-typer_ also supports shell completion for bash_, zsh_, fish_ and powershell_ and
@@ -21,19 +21,20 @@
 
 
 The goal of django-typer_ is to provide full Typer_ style functionality while maintaining
 compatibility with the Django management command system. This means that the BaseCommand_
 interface is preserved and the Typer_ interface is added on top of it. This means that
 this code base is more robust to changes in the Django management command system - because
 most of the base class functionality is preserved but many Typer_ and click_ internals are
-used directly to achieve this. We rely on robust CI to catch breaking changes upstream.
+used directly to achieve this. We rely on robust CI to catch breaking changes upstream and
+keep a tight version lock on Typer.
 """
 
 # During development of django-typer_ I've wrestled with a number of encumbrances in the
-# aging django management command design. I detail them here mostly to keep track of them
+# old django management command design. I detail them here mostly to keep track of them
 # for possible future refactors of core Django.
 
 # 1) BaseCommand::execute() prints results to stdout without attempting to convert them
 # to strings. This means you've gotta do weird stuff to get a return object out of
 # call_command()
 
 # 2) call_command() converts arguments to strings. There is no official way to pass
@@ -58,38 +59,55 @@
 # 5) There is an awkwardness to how parse_args flattens all the arguments and options
 # into a single dictionary. This means that when mapping a library like Typer onto the
 # BaseCommand interface you cannot allow arguments at different levels
 # (e.g. in initialize()) or group() functions above the command to have the same names as
 # the command's options. You can work around this by using a different name for the
 # option in the command and supplying the desired name in the annotation, but its an odd
 # quirk imposed by the base class for users to be aware of.
+# ruff: noqa: E402
 
+# This file has lots of interdependent code that would be difficult to break out into
+# smaller files. Most of the book keeping complexity is induced by the necessity of
+# figuring out if and where django's base command line parameters should be attached
+# and how to bind a method function to a class that may not been created yet. To do
+# this commands and Typer instances (groups in click/django-typer parlance) need to
+# be able to access the django command class they are attached to. The length of this
+# file is largely a result of wrapping Typer.command, Typer.callback and
+# Typer.add_typer in many different contexts to achieve the nice interface we would
+# like and also because we list out each parameter for developer experience
+#
+# The other complexity comes from the fact that we pull in methods into the typer
+# infrastructure before classes are created so we have to do some bookkeeping to make sure
+# methods are bound to the right objects when called
 
 import inspect
 import sys
 import typing as t
+from collections import deque
 from copy import copy, deepcopy
+from functools import cached_property
 from importlib import import_module
 from pathlib import Path
 from types import MethodType, SimpleNamespace
 
 import click
 from click.shell_completion import CompletionItem
 from django.core.management import get_commands
 from django.core.management.base import BaseCommand, CommandError
 from django.core.management.base import OutputWrapper as BaseOutputWrapper
 from django.core.management.color import Style as ColorStyle
 from django.db.models import Model
+from django.utils.functional import classproperty
 from django.utils.translation import gettext as _
 
 from django_typer import patch
 
 patch.apply()
 
-from typer import Typer
+import typer
 from typer.core import MarkupMode
 from typer.core import TyperCommand as CoreTyperCommand
 from typer.core import TyperGroup as CoreTyperGroup
 from typer.main import get_command as get_typer_command
 from typer.main import get_params_convertors_ctx_param_name_from_function
 from typer.models import Context as TyperContext
 from typer.models import Default, DefaultPlaceholder
@@ -102,43 +120,84 @@
     PythonPath,
     Settings,
     SkipChecks,
     Traceback,
     Verbosity,
     Version,
 )
-from .utils import _command_context, get_usage_script, traceback_config, with_typehint
+from .utils import (
+    _command_context,
+    _load_command_plugins,
+    called_from_command_definition,
+    called_from_module,
+    get_usage_script,
+    is_method,
+    traceback_config,
+    with_typehint,
+)
 
 if sys.version_info < (3, 10):
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec
 
 
-VERSION = (1, 1, 2)
+VERSION = (2, 0, 0)
 
 __title__ = "Django Typer"
 __version__ = ".".join(str(i) for i in VERSION)
 __author__ = "Brian Kohan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023-2024 Brian Kohan"
 
 
 __all__ = [
     "TyperCommand",
+    "CommandNode",
+    "Typer",
+    "DjangoTyperMixin",
+    "DTCommand",
+    "DTGroup",
     "Context",
     "initialize",
     "command",
     "group",
     "get_command",
     "model_parser_completer",
 ]
 
 P = ParamSpec("P")
+P2 = ParamSpec("P2")
 R = t.TypeVar("R")
+R2 = t.TypeVar("R2")
+C = t.TypeVar("C", bound=BaseCommand)
+
+_CACHE_KEY = "_register_typer"
+
+
+if sys.version_info < (3, 10):
+    # todo - remove this when support for <3.10 is dropped
+    class static_factory(type):
+        def __call__(self, *args, **kwargs):
+            assert args
+            if type(args[0]).__name__ == "staticmethod":
+                return args[0]
+            return super().__call__(*args, **kwargs)
+
+    class staticmethod(t.Generic[P, R], metaclass=static_factory):
+        __func__: t.Callable[P, R]
+
+        def __init__(self, func: t.Callable[P, R]):
+            self.__func__ = func
+
+        def __getattr__(self, name):
+            return getattr(self.__func__, name)
+
+        def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
+            return self.__func__(*args, **kwargs)
 
 
 def model_parser_completer(
     model_cls: t.Type[Model],
     lookup_field: t.Optional[str] = None,
     case_insensitive: bool = False,
     help_field: t.Optional[str] = ModelObjectCompleter.help_field,
@@ -197,22 +256,60 @@
             query=query,
             limit=limit,
             distinct=distinct,
         ),
     }
 
 
+@t.overload  # pragma: no cover
+def get_command(  # type: ignore[overload-overlap]
+    command_name: str,
+    stdout: t.Optional[t.IO[str]] = None,
+    stderr: t.Optional[t.IO[str]] = None,
+    no_color: bool = False,
+    force_color: bool = False,
+    **kwargs,
+) -> BaseCommand: ...
+
+
+@t.overload  # pragma: no cover
+# mypy seems to break on this one, but this is correct
+def get_command(
+    command_name: str,
+    cmd_type: t.Type[C],
+    stdout: t.Optional[t.IO[str]] = None,
+    stderr: t.Optional[t.IO[str]] = None,
+    no_color: bool = False,
+    force_color: bool = False,
+    **kwargs,
+) -> C: ...
+
+
+@t.overload  # pragma: no cover
 def get_command(
     command_name: str,
-    *subcommand: str,
+    path0: str,
+    *path: str,
     stdout: t.Optional[t.IO[str]] = None,
     stderr: t.Optional[t.IO[str]] = None,
     no_color: bool = False,
     force_color: bool = False,
-) -> t.Union[BaseCommand, MethodType]:
+    **kwargs,
+) -> MethodType: ...
+
+
+def get_command(
+    command_name,
+    *path,
+    stdout=None,
+    stderr=None,
+    no_color: bool = False,
+    force_color: bool = False,
+    **kwargs,
+):
     """
     Get a Django_ command by its name and instantiate it with the provided options. This
     will work for subclasses of BaseCommand_ as well as for :class:`~django_typer.TyperCommand`
     subclasses. If subcommands are listed for a :class:`~django_typer.TyperCommand`, the
     method that corresponds to the command name will be returned. This method may then be
     invoked directly. If no subcommands are listed the command instance will be returned.
 
@@ -237,32 +334,59 @@
     Subcommands may be retrieved by passing the subcommand names as additional arguments:
 
     .. code-block:: python
 
         divide = get_command('hierarchy', 'math', 'divide')
         result = divide(10, 2)
 
+    When fetching an entire TyperCommand (i.e. no group or subcommand path), you may supply
+    the type of the expected TyperCommand as the second argument. This will allow the type
+    system to infer the correct return type:
+
+    .. code-block:: python
+
+        from myapp.management.commands import Command as Hierarchy
+        hierarchy: Hierarchy = get_command('hierarchy', Hierarchy)
+
+    .. note::
+
+        If get_command fetches a BaseCommand that does not implement __call__ get_command will
+        make the command callable by adding a __call__ method that calls the handle method of
+        the BaseCommand. This allows you to call the command like get_command("command")() with
+        confidence.
+
     :param command_name: the name of the command to get
-    :param subcommand: the subcommand to get if any
+    :param path: the path walking down the group/command tree
     :param stdout: the stdout stream to use
     :param stderr: the stderr stream to use
     :param no_color: whether to disable color
     :param force_color: whether to force color
+    :param kwargs: t.Any other parameters to pass through to the command constructor
     :raises ModuleNotFoundError: if the command is not found
     :raises LookupError: if the subcommand is not found
     """
     module = import_module(
         f"{get_commands()[command_name]}.management.commands.{command_name}"
     )
-    cmd = module.Command(
-        stdout=stdout, stderr=stderr, no_color=no_color, force_color=force_color
+    cmd: BaseCommand = module.Command(
+        stdout=stdout,
+        stderr=stderr,
+        no_color=no_color,
+        force_color=force_color,
+        **kwargs,
     )
-    if subcommand:
-        method = cmd.get_subcommand(*subcommand).click_command._callback.__wrapped__
-        return MethodType(method, cmd)  # return the bound method
+    if path and (isinstance(path[0], str) or len(path) > 1):
+        return t.cast(TyperCommand, cmd).get_subcommand(*path).callback
+
+    if not hasattr(cmd, "__call__"):
+        setattr(
+            cmd.__class__,
+            "__call__",
+            lambda self, *args, **options: self.handle(*args, **options),
+        )
 
     return cmd
 
 
 def _common_options(
     version: Version = False,
     verbosity: Verbosity = 1,
@@ -377,23 +501,39 @@
             supplied=list(self.supplied_params.keys()),
         )
         self.children = []
         if parent:
             parent.children.append(self)
 
 
-class _DjangoAdapterMixin(with_typehint(CoreTyperGroup)):  # type: ignore[misc]
+class DjangoTyperMixin(with_typehint(CoreTyperGroup)):  # type: ignore[misc]
     """
     A mixin we use to add additional needed contextual awareness to click Commands
     and Groups.
     """
 
     context_class: t.Type[click.Context] = Context
     django_command: "TyperCommand"
-    callback_is_method: bool = True
+    _callback: t.Optional[t.Callable[..., t.Any]] = None
+    _callback_is_method: t.Optional[bool] = None
+    common_init: bool = False
+
+    @property
+    def no_callback(self) -> bool:
+        """Returns false if no callback was registered at the root django command."""
+        return bool(
+            getattr(self, "django_command", None)
+            and not self.django_command.typer_app.registered_callback
+        )
+
+    @property
+    def is_method(self) -> t.Optional[bool]:
+        if self._callback_is_method is None:
+            self._callback_is_method = is_method(self._callback)
+        return self._callback_is_method
 
     class Converter:
         """
         Because of the way the BaseCommand forces parsing to be done in a separate
         first step, type casting of input strings to the correct types will have
         sometimes happened already. We use this class to avoid double type casting.
 
@@ -439,33 +579,47 @@
             completions = super().shell_complete(
                 ctx, min(getattr(ctx, "_opt_prefixes", [""]))
             )
         return completions
 
     def common_params(self) -> t.Sequence[t.Union[click.Argument, click.Option]]:
         """
-        Get the django common options that should be included in this click command.
-        These will very depending on how the base class command is specified so look
-        to individual implementations for details.
+        Add the common parameters to this group only if this group is the root
+        command's user specified initialize callback.
         """
-        return []
+        suppressed = getattr(self.django_command, "suppressed_base_arguments", None)
+        return (
+            [
+                param
+                for param in _get_common_params()
+                if param.name
+                and param.name
+                not in (
+                    {arg.lstrip("--").replace("-", "_") for arg in suppressed or []}
+                )
+            ]
+            if self.common_init or self.no_callback
+            else []
+        )
 
     def __init__(
         self,
         *args,
-        callback: t.Callable[..., t.Any],
+        callback: t.Optional[t.Callable[..., t.Any]],
         params: t.Optional[t.List[click.Parameter]] = None,
         **kwargs,
     ):
         params = params or []
         self._callback = callback
-        expected = [param.name for param in params[1:] if param.name]
-        self_arg = params[0].name if params and params[0].name else "self"
+        expected = [
+            param.name for param in params[1 if self.is_method else 0 :] if param.name
+        ]
 
         def call_with_self(*args, **kwargs):
+            assert callback
             ctx = t.cast(Context, click.get_current_context())
             return callback(
                 *args,
                 **{
                     # we could call param.process_value() here to allow named
                     # parameters to be passed as their unparsed string values,
                     # we don't because this forces some weird idempotency on custom
@@ -474,164 +628,504 @@
                     # which expect the parsed values to be passed by name. Unparsed values can
                     # always be passed as argument strings.
                     param: val
                     for param, val in kwargs.items()
                     if param in expected
                 },
                 **(
-                    {self_arg: getattr(ctx, "django_command", None)}
-                    if self.callback_is_method
+                    {str(params[0].name): getattr(ctx, "django_command", None)}
+                    if self.is_method
                     else {}
                 ),
             )
 
         super().__init__(
             *args,
             params=[
-                *(params[1:] if self.callback_is_method else params),
+                *(params[1:] if self.is_method else params),
                 *[
                     param
                     for param in self.common_params()
                     if param.name not in expected
                 ],
             ],
             callback=call_with_self,
             **kwargs,
         )
 
 
-class TyperCommandWrapper(_DjangoAdapterMixin, CoreTyperCommand):
+class DTCommand(DjangoTyperMixin, CoreTyperCommand):
     """
-    This class extends the TyperCommand class to work with the django-typer
-    interfaces. If you need to add functionality to the command class - which
-    you should not - you should inherit from this class.
+    This class extends the TyperCommand class to work with the django-typer interfaces.
+    If you need to add functionality to the command class - you should inherit from
+    this class. You can then pass your custom class to the command() decorators
+    using the cls parameter.
+
+    .. code-block:: python
+
+        from django_typer import TyperCommand, DTCommand, command
+
+        class CustomCommand(DTCommand):
+            ...
+
+        class Command(TyperCommand):
+
+            @command(cls=CustomCommand)
+            def handle(self):
+                ...
     """
 
-    def common_params(self) -> t.Sequence[t.Union[click.Argument, click.Option]]:
-        """
-        Return the common django params that are not suppressed only if the django
-        command has a single command and no callback or other groups. When there are
-        multiple commands and groups - the command parameters are added to a global
-        initialization callback. See the meta class for details.
-        """
-        if (
-            hasattr(self, "django_command")
-            and self.django_command._num_commands < 2
-            and not self.django_command._has_callback
-            and not self.django_command._root_groups
-        ):
-            return [
-                param
-                for param in _get_common_params()
-                if param.name
-                and param.name
-                not in (self.django_command.suppressed_base_arguments or [])
-            ]
-        return super().common_params()
+
+class DTGroup(DjangoTyperMixin, CoreTyperGroup):
+    """
+    This class extends the TyperGroup class to work with the django-typer interfaces.
+    If you need to add functionality to the group class you should inherit from this
+    class. You can then pass your custom class to the command() decorators using the
+    cls parameter.
+
+    .. code-block:: python
+
+        from django_typer import TyperCommand, DTGroup, group
+
+        class CustomGroup(DTGroup):
+            ...
+
+        class Command(TyperCommand):
+
+            @group(cls=CustomGroup)
+            def grp(self):
+                ...
+    """
+
+
+# staticmethod objects are not picklable which causes problems with deepcopy
+# hence the following mishegoss
 
 
-class TyperGroupWrapper(_DjangoAdapterMixin, CoreTyperGroup):
+@t.overload  # pragma: no cover
+def _check_static(
+    func: typer.models.CommandFunctionType,
+) -> typer.models.CommandFunctionType: ...
+
+
+@t.overload  # pragma: no cover
+def _check_static(func: None) -> None: ...
+
+
+def _check_static(func):
     """
-    This class extends the TyperGroup class to work with the django-typer
-    interfaces. If you need to add functionality to the group class - which
-    you should not - you should inherit from this class.
+    Check if a function is a staticmethod and return it if it is otherwise make
+    it static if it should be but isn't.
     """
+    if func and not is_method(func) and not isinstance(func, staticmethod):
+        return staticmethod(func)
+    return func
 
-    def common_params(self) -> t.Sequence[t.Union[click.Argument, click.Option]]:
-        """
-        Add the common parameters to this group only if this group is the root
-        command's user specified initialize callback.
-        """
-        if (
-            hasattr(self, "django_command") and self.django_command._has_callback
-        ) or getattr(self, "common_init", False):
-            return [
-                param
-                for param in _get_common_params()
-                if param.name
-                if param.name
-                not in (self.django_command.suppressed_base_arguments or [])
-            ]
-        return super().common_params()
+
+@t.overload  # pragma: no cover
+def _strip_static(func: t.Callable[P, R]) -> t.Callable[P, R]: ...
+
+
+@t.overload  # pragma: no cover
+def _strip_static(func: None) -> None: ...
+
+
+def _strip_static(func: t.Optional[t.Callable[P, R]]) -> t.Optional[t.Callable[P, R]]:
+    """
+    Strip the staticmethod wrapper from a function if it is present.
+    """
+    ret = getattr(func, "__func__", func)
+    return ret
+
+
+def _cache_initializer(
+    callback: t.Callable[..., t.Any],
+    common_init: bool,
+    name: t.Optional[str] = Default(None),
+    help: t.Optional[str] = Default(None),
+    cls: t.Type[DTGroup] = DTGroup,
+    **kwargs,
+):
+    def register(
+        cmd: "TyperCommand",
+        _name: t.Optional[str] = Default(None),
+        _help: t.Optional[str] = Default(None),
+        **extra,
+    ):
+        return cmd.typer_app.callback(
+            name=name or _name,
+            cls=type(
+                "_Initializer",
+                (cls,),
+                {"django_command": cmd, "common_init": common_init},
+            ),
+            help=cmd.typer_app.info.help or help or _help,
+            **kwargs,
+            **extra,
+        )(_strip_static(callback))
+
+    setattr(callback, _CACHE_KEY, register)
+
+
+def _cache_command(
+    callback: t.Callable[..., t.Any],
+    name: t.Optional[str] = None,
+    help: t.Optional[str] = None,
+    cls: t.Type[DTCommand] = DTCommand,
+    **kwargs,
+):
+    def register(
+        cmd: "TyperCommand",
+        _name: t.Optional[str] = None,
+        _help: t.Optional[str] = None,
+        **extra,
+    ):
+        return cmd.typer_app.command(
+            name=name or _name,
+            cls=type("_Command", (cls,), {"django_command": cmd}),
+            help=help or _help or None,
+            **kwargs,
+            **extra,
+        )(_strip_static(callback))
+
+    setattr(callback, _CACHE_KEY, register)
+
+
+TyperFunction = t.Union[
+    "Typer[P, R]",
+    typer.models.CommandInfo,
+    typer.models.TyperInfo,
+    t.Callable[..., t.Any],
+]
+
+
+def _get_direct_function(
+    obj: "TyperCommand",
+    app_node: TyperFunction,
+):
+    """
+    Get a direct callable function bound to the given object if it is not static held by the given
+    Typer instance or TyperInfo instance.
+    """
+    if isinstance(app_node, Typer):
+        method = app_node.is_method
+        cb = getattr(app_node.registered_callback, "callback", app_node.info.callback)
+    elif cb := getattr(app_node, "callback", None):
+        method = is_method(cb)
+    else:
+        assert callable(app_node)
+        cb = app_node
+        method = is_method(cb)
+    assert cb
+    return MethodType(cb, obj) if method else staticmethod(cb)
+
+
+class AppFactory(type):
+    """
+    A metaclass used to define/set Command classes into the defining module when
+    the Typer-like functional interface is used.
+    """
+
+    def __call__(self, *args, **kwargs) -> "Typer":
+        if called_from_module():
+            frame = inspect.currentframe()
+            cmd_module = inspect.getmodule(frame.f_back) if frame else None
+            if cmd_module and not hasattr(cmd_module, "Command"):
+
+                class Command(
+                    TyperCommand,
+                    name=kwargs.pop("name", None) or cmd_module.__name__.split(".")[-1],
+                    **kwargs,
+                    typer_app=args[0] if args else None,
+                ):
+                    pass
+
+                # spoof it so hard
+                Command.__module__ = cmd_module.__name__
+                Command.__qualname__ = f"{cmd_module.__name__}.Command"
+                setattr(cmd_module, "Command", Command)
+                return Command.typer_app
+            else:
+                return Typer(**kwargs)
+
+        if sys.version_info < (3, 9):
+            # this is a workaround for a bug in python 3.8 that causes multiple
+            # values for cls error. 3.8 support is sun setting soon so we just punt
+            # on this one - REMOVE when 3.8 support is dropped
+            kwargs.pop("cls", None)
+        return super().__call__(*args, **kwargs)
 
 
-class GroupFunction(Typer):
+class Typer(typer.Typer, t.Generic[P, R], metaclass=AppFactory):
     """
     Typer_ adds additional groups of commands by adding Typer_ apps to parent
     Typer_ apps. This class extends the ``typer.Typer`` class so that we can add
     the additional information necessary to attach this app to the root app
     and other groups specified on the django command.
+
+    :param name: the name of the class being created
+    :param bases: the base classes of the class being created
+    :param attrs: the attributes of the class being created
+    :param cls: The class to use as the core typer group wrapper
+    :param invoke_without_command: whether to invoke the group callback if no command
+        was specified.
+    :param no_args_is_help: whether to show the help if no arguments are provided
+    :param subcommand_metavar: the metavar to use for subcommands in the help output
+    :param chain: whether to chain commands, this allows multiple commands from the group
+        to be specified and run in order sequentially in one call from the command line.
+    :param result_callback: a callback to invoke with the result of the command
+    :param context_settings: the click context settings to use - see
+        `click docs <https://click.palletsprojects.com/api/#context>`_.
+    :param help: the help string to use, defaults to the function docstring, if you need
+        to translate the help you should use the help kwarg instead because docstrings
+        will not be translated.
+    :param epilog: the epilog to use in the help output
+    :param short_help: the short help to use in the help output
+    :param options_metavar: the metavar to use for options in the help output
+    :param add_help_option: whether to add the help option to the command
+    :param hidden: whether to hide this group from the help output
+    :param deprecated: show a deprecation warning
+    :param rich_markup_mode: the rich markup mode to use - if rich is installed
+        this can be used to enable rich markup or Markdown in the help output. Can
+        be "markdown", "rich" or None to disable markup rendering.
+    :param rich_help_panel: the rich help panel to use - if rich is installed
+        this can be used to group commands into panels in the help output.
+    :param pretty_exceptions_enable: whether to enable pretty exceptions - if rich is
+        installed this can be used to enable pretty exception rendering. This will
+        default to on if the traceback configuration settings installs the rich
+        traceback handler. This allows tracebacks to be configured by the user on a
+        per deployment basis in the settings file. We therefore do not advise
+        hardcoding this value.
+    :param pretty_exceptions_show_locals: whether to show local variables in pretty
+        exceptions - if rich is installed. This will default to the 'show_locals'
+        setting in the traceback configuration setting (on by default). This allows
+        tracebacks to be configured by the user on a per deployment basis in the
+        settings file. We therefore do not advise hardcoding this value.
+    :param pretty_exceptions_short: whether to show short tracebacks in pretty
+        exceptions - if rich is installed. This will default to the 'short' setting
+        in the traceback configuration setting (off by default). This allows tracebacks
+        to be configured by the user on a per deployment basis in the settings file. We
+        therefore do not advise hardcoding this value.
     """
 
-    bound: bool = False
-    django_command_cls: t.Type["TyperCommand"]
-    _callback: t.Callable[..., t.Any]
-
-    def __get__(
-        self, obj: t.Optional["TyperCommand"], _=None
-    ) -> t.Union["GroupFunction", MethodType]:
+    parent: t.Optional["Typer"] = None
+
+    name: t.Optional[str] = None
+
+    _django_command: t.Optional[t.Type["TyperCommand"]] = None
+
+    # these aren't defined on the super class which messes up __getattr__
+    registered_groups: t.List[typer.models.TyperInfo] = []
+    registered_commands: t.List[typer.models.CommandInfo] = []
+    registered_callback: t.Optional[typer.models.TyperInfo] = None
+
+    is_method: t.Optional[bool] = None
+    top_level: bool = False
+
+    @property
+    def django_command(self) -> t.Optional[t.Type["TyperCommand"]]:
+        return self._django_command or getattr(self.parent, "django_command", None)
+
+    @django_command.setter
+    def django_command(self, cmd: t.Optional[t.Type["TyperCommand"]]):
+        self._django_command = cmd
+
+    # todo - this results in type hinting expecting self to be passed explicitly
+    # when this is called as a callable
+    # https://github.com/bckohan/django-typer/issues/73
+    def __get__(self, obj, _=None) -> "Typer[P, R]":
         """
         Our Typer app wrapper also doubles as a descriptor, so when
         it is accessed on the instance, we return the wrapped function
         so it may be called directly - but when accessed on the class
         the app itself is returned so it can modified by other decorators
         on the class and subclasses.
         """
-        if obj is None:
-            return self
-        return MethodType(self._callback, obj)
+        if isinstance(obj, TyperCommand):
+            return t.cast(Typer[P, R], BoundProxy(obj, self))
+        return self
 
-    def __init__(self, *args, **kwargs):
-        self._callback = kwargs["callback"]
-        super().__init__(*args, **kwargs)
-
-    def bind(self, django_command_cls: t.Type["TyperCommand"]):
-        """
-        Bind this typer app to the given django command class. Only groups at
-        root need to be bound - and will be done so by the meta class, this will
-        happen automatically (See group()) when groups are added to other groups.
-        """
-        self.django_command_cls = django_command_cls
-        # the deepcopy is necessary for instances where classes derive
-        # from Command classes and replace/extend commands on groups
-        # defined in the base class - this avoids the extending class
-        # polluting the base class's command tree
-        self.django_command_cls.typer_app.add_typer(deepcopy(self))
-
-    def callback(self, *args, **kwargs):
-        """
-        callback is not supported because we've adapted the typer interface to be more
-        intuitive for django users. The callback for a group is the function decorated
-        by group().
-        """
-        raise NotImplementedError(
-            _(
-                "callback is not supported - the function decorated by group() is the "
-                "callback."
+    def __getattr__(self, name: str) -> t.Any:
+        for cmd in self.registered_commands:
+            assert cmd.callback
+            if name in _names(cmd):
+                return cmd
+        for grp in self.registered_groups:
+            cmd_grp = t.cast(Typer, grp.typer_instance)
+            assert cmd_grp
+            if name in _names(cmd_grp):
+                return cmd_grp
+        raise AttributeError(
+            "{cls} object has no attribute {name}".format(
+                cls=self.__class__.__name__, name=name
             )
         )
 
+    def __init__(
+        self,
+        *args,
+        name: t.Optional[str] = Default(None),
+        cls: t.Optional[t.Type[DTGroup]] = DTGroup,
+        invoke_without_command: bool = Default(False),
+        no_args_is_help: bool = Default(False),
+        subcommand_metavar: t.Optional[str] = Default(None),
+        chain: bool = Default(False),
+        result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
+        # Command
+        context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
+        callback: t.Optional[t.Callable[P, R]] = Default(None),
+        help: t.Optional[str] = Default(None),
+        epilog: t.Optional[str] = Default(None),
+        short_help: t.Optional[str] = Default(None),
+        options_metavar: str = Default("[OPTIONS]"),
+        add_help_option: bool = Default(True),
+        hidden: bool = Default(False),
+        deprecated: bool = Default(False),
+        add_completion: bool = True,
+        # Rich settings
+        rich_markup_mode: MarkupMode = None,
+        rich_help_panel: t.Union[str, None] = Default(None),
+        pretty_exceptions_enable: bool = True,
+        pretty_exceptions_show_locals: bool = True,
+        pretty_exceptions_short: bool = True,
+        parent: t.Optional["Typer"] = None,
+        django_command: t.Optional[t.Type["TyperCommand"]] = None,
+        **kwargs,
+    ):
+        assert not args  # should have been removed by metaclass
+        self.parent = parent
+        self._django_command = django_command
+        self.top_level = kwargs.pop("top_level", False)
+        typer_app = kwargs.pop("typer_app", None)
+        callback = _strip_static(callback)
+        if callback:
+            self.name = callback.__name__
+            self.is_method = is_method(callback)
+        super().__init__(
+            name=name,
+            cls=type(
+                "_DTGroup", (cls or DTGroup,), {"django_command": self.django_command}
+            ),
+            invoke_without_command=invoke_without_command,
+            no_args_is_help=no_args_is_help,
+            subcommand_metavar=subcommand_metavar,
+            chain=chain,
+            result_callback=result_callback,
+            context_settings=context_settings,
+            callback=callback,
+            help=help,
+            epilog=epilog,
+            short_help=short_help,
+            options_metavar=options_metavar,
+            add_help_option=add_help_option,
+            hidden=hidden,
+            deprecated=deprecated,
+            add_completion=add_completion,
+            rich_markup_mode=rich_markup_mode,
+            rich_help_panel=rich_help_panel,
+            pretty_exceptions_enable=pretty_exceptions_enable,
+            pretty_exceptions_show_locals=pretty_exceptions_show_locals,
+            pretty_exceptions_short=pretty_exceptions_short,
+            **kwargs,
+        )
+        # if we're copying a supplied typer app, pull in the hierarchy and options
+        if typer_app:
+            self.registered_callback = typer_app.registered_callback
+            self.registered_commands = copy(typer_app.registered_commands)
+            self.registered_groups = deepcopy(typer_app.registered_groups)
+            self.rich_help_panel = (
+                typer_app.rich_help_panel
+                if isinstance(self.rich_help_panel, DefaultPlaceholder)
+                else self.rich_help_panel
+            )
+            for param, cfg in vars(self.info).items():
+                if isinstance(cfg, DefaultPlaceholder):
+                    setattr(self.info, param, getattr(typer_app.info, param))
+
+    def callback(  # type: ignore
+        self,
+        name: t.Optional[str] = Default(None),
+        *,
+        cls: t.Type[DTGroup] = DTGroup,
+        invoke_without_command: bool = Default(False),
+        no_args_is_help: bool = Default(False),
+        subcommand_metavar: t.Optional[str] = Default(None),
+        chain: bool = Default(False),
+        result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
+        # Command
+        context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
+        help: t.Optional[str] = Default(None),
+        epilog: t.Optional[str] = Default(None),
+        short_help: t.Optional[str] = Default(None),
+        options_metavar: str = Default("[OPTIONS]"),
+        add_help_option: bool = Default(True),
+        hidden: bool = Default(False),
+        deprecated: bool = Default(False),
+        # Rich settings
+        rich_help_panel: t.Union[str, None] = Default(None),
+        **kwargs,
+    ) -> t.Callable[
+        [typer.models.CommandFunctionType], typer.models.CommandFunctionType
+    ]:
+        def make_callback(
+            func: typer.models.CommandFunctionType,
+        ) -> typer.models.CommandFunctionType:
+            self.is_method = is_method(func)
+            self.name = func.__name__
+            self.registered_callback = typer.models.TyperInfo(
+                name=name,
+                cls=type(
+                    "_Initializer",
+                    (cls,),
+                    {
+                        "django_command": self.django_command,
+                        "common_init": self.parent is None,
+                    },
+                ),
+                invoke_without_command=invoke_without_command,
+                no_args_is_help=no_args_is_help,
+                subcommand_metavar=subcommand_metavar,
+                chain=chain,
+                result_callback=result_callback,
+                context_settings=context_settings,
+                callback=func,
+                help=help,
+                epilog=epilog,
+                short_help=short_help,
+                options_metavar=options_metavar,
+                add_help_option=add_help_option,
+                hidden=hidden,
+                deprecated=deprecated,
+                rich_help_panel=rich_help_panel,
+                **kwargs,
+            )
+            return _check_static(func)
+
+        return make_callback
+
+    initialize = callback  # allow initialize as an alias for callback
+
     def command(  # type: ignore
         self,
         name: t.Optional[str] = None,
         *,
-        cls: t.Type[CoreTyperCommand] = TyperCommandWrapper,
+        cls: t.Type[DTCommand] = DTCommand,
         context_settings: t.Optional[t.Dict[t.Any, t.Any]] = None,
-        help: t.Optional[str] = None,  # pylint: disable=redefined-builtin
+        help: t.Optional[str] = None,
         epilog: t.Optional[str] = None,
         short_help: t.Optional[str] = None,
         options_metavar: str = "[OPTIONS]",
         add_help_option: bool = True,
         no_args_is_help: bool = False,
         hidden: bool = False,
         deprecated: bool = False,
         # Rich settings
         rich_help_panel: t.Union[str, None] = Default(None),
-        **kwargs: t.Dict[str, t.Any],
-    ) -> t.Callable[[t.Callable[P, R]], t.Callable[P, R]]:
+        **kwargs,
+    ) -> t.Callable[[t.Callable[P2, R2]], t.Callable[P2, R2]]:
         """
         A function decorator that creates a new command and attaches it to this group.
         This is a passthrough to Typer.command() and the options are the same, except
         we swap the default command class for our wrapper.
 
         The decorated function is the command function. It may also be invoked directly
         as a method from an instance of the django command class.
@@ -670,41 +1164,93 @@
         :param no_args_is_help: whether to show the help if no arguments are provided
         :param hidden: whether to hide the command from help output
         :param deprecated: show a deprecation warning
         :param rich_help_panel: the rich help panel to use - if rich is installed
             this can be used to group commands into panels in the help output.
         """
 
-        def decorator(f: t.Callable[P, R]) -> t.Callable[P, R]:
-            return super(  # pylint: disable=super-with-arguments
-                GroupFunction, self
-            ).command(
-                name=name,
-                cls=cls,
-                context_settings=context_settings,
-                help=help,
-                epilog=epilog,
-                short_help=short_help,
-                options_metavar=options_metavar,
-                add_help_option=add_help_option,
-                no_args_is_help=no_args_is_help,
-                hidden=hidden,
-                deprecated=deprecated,
-                rich_help_panel=rich_help_panel,
-                **kwargs,
-            )(
-                f
+        def make_command(func: t.Callable[P2, R2]) -> t.Callable[P2, R2]:
+            return _check_static(
+                super(  # pylint: disable=super-with-arguments
+                    Typer, self
+                ).command(
+                    name=name,
+                    cls=type(
+                        "_Command", (cls,), {"django_command": self.django_command}
+                    ),
+                    context_settings=context_settings,
+                    help=help,
+                    epilog=epilog,
+                    short_help=short_help,
+                    options_metavar=options_metavar,
+                    add_help_option=add_help_option,
+                    no_args_is_help=no_args_is_help,
+                    hidden=hidden,
+                    deprecated=deprecated,
+                    rich_help_panel=rich_help_panel,
+                    **kwargs,
+                )(_strip_static(func))
             )
 
-        return decorator
+        return make_command
+
+    def add_typer(  # type: ignore
+        self,
+        typer_instance: "Typer",
+        *,
+        name: t.Optional[str] = Default(None),
+        cls: t.Type[DTGroup] = DTGroup,
+        invoke_without_command: bool = Default(False),
+        no_args_is_help: bool = Default(False),
+        subcommand_metavar: t.Optional[str] = Default(None),
+        chain: bool = Default(False),
+        result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
+        # Command
+        context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
+        callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
+        help: t.Optional[str] = Default(None),
+        epilog: t.Optional[str] = Default(None),
+        short_help: t.Optional[str] = Default(None),
+        options_metavar: str = Default("[OPTIONS]"),
+        add_help_option: bool = Default(True),
+        hidden: bool = Default(False),
+        deprecated: bool = Default(False),
+        # Rich settings
+        rich_help_panel: t.Union[str, None] = Default(None),
+        **kwargs,
+    ) -> None:
+        typer_instance.parent = self
+        typer_instance.django_command = self.django_command
+
+        return super().add_typer(
+            typer_instance=typer_instance,
+            name=name,
+            cls=type("_DTGroup", (cls,), {"django_command": self.django_command}),
+            invoke_without_command=invoke_without_command,
+            no_args_is_help=no_args_is_help,
+            subcommand_metavar=subcommand_metavar,
+            chain=chain,
+            result_callback=result_callback,
+            context_settings=context_settings,
+            callback=_strip_static(callback),
+            help=help,
+            epilog=epilog,
+            short_help=short_help,
+            options_metavar=options_metavar,
+            add_help_option=add_help_option,
+            hidden=hidden,
+            deprecated=deprecated,
+            rich_help_panel=rich_help_panel,
+            **kwargs,
+        )
 
     def group(
         self,
         name: t.Optional[str] = Default(None),
-        cls: t.Type[CoreTyperGroup] = TyperGroupWrapper,
+        cls: t.Type[DTGroup] = DTGroup,
         invoke_without_command: bool = Default(False),
         no_args_is_help: bool = Default(False),
         subcommand_metavar: t.Optional[str] = Default(None),
         chain: bool = Default(False),
         result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
         # Command
         context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
@@ -713,16 +1259,16 @@
         short_help: t.Optional[str] = Default(None),
         options_metavar: str = Default("[OPTIONS]"),
         add_help_option: bool = Default(True),
         hidden: bool = Default(False),
         deprecated: bool = Default(False),
         # Rich settings
         rich_help_panel: t.Union[str, None] = Default(None),
-        **kwargs: t.Dict[str, t.Any],
-    ) -> t.Callable[[t.Callable[..., t.Any]], "GroupFunction"]:
+        **kwargs,
+    ) -> t.Callable[[t.Callable[P2, R2]], "Typer[P2, R2]"]:
         """
         Create a new subgroup and attach it to this group. This is like creating a new
         Typer app and adding it to a parent Typer app. The kwargs are passed through
         to the Typer() constructor.
 
         .. code-block:: python
 
@@ -761,18 +1307,18 @@
         :param add_help_option: whether to add the help option to the command
         :param hidden: whether to hide this group from the help output
         :param deprecated: show a deprecation warning
         :param rich_help_panel: the rich help panel to use - if rich is installed
             this can be used to group commands into panels in the help output.
         """
 
-        def create_app(func: t.Callable[..., t.Any]) -> GroupFunction:
-            grp = GroupFunction(  # type: ignore
+        def create_app(func: t.Callable[P2, R2]) -> Typer[P2, R2]:
+            grp: Typer[P2, R2] = Typer(  # pyright: ignore[reportAssignmentType]
                 name=name,
-                cls=cls,
+                cls=type("_DTGroup", (cls,), {"django_command": self.django_command}),
                 invoke_without_command=invoke_without_command,
                 no_args_is_help=no_args_is_help,
                 subcommand_metavar=subcommand_metavar,
                 chain=chain,
                 result_callback=result_callback,
                 callback=func,
                 context_settings=context_settings,
@@ -780,27 +1326,69 @@
                 epilog=epilog,
                 short_help=short_help,
                 options_metavar=options_metavar,
                 add_help_option=add_help_option,
                 hidden=hidden,
                 deprecated=deprecated,
                 rich_help_panel=rich_help_panel,
+                parent=self,
                 **kwargs,
             )
             self.add_typer(grp)
-            grp.bound = True
             return grp
 
         return create_app
 
 
+class BoundProxy(t.Generic[P, R]):
+    """
+    A helper class that proxies the Typer or command objects and binds them
+    to the django command instance.
+    """
+
+    command: "TyperCommand"
+    proxied: TyperFunction
+
+    def __init__(self, command: "TyperCommand", proxied: TyperFunction):
+        self.command = command
+        self.proxied = proxied
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
+        if isinstance(self.proxied, Typer) and not self.proxied.parent:
+            # if we're calling a top level Typer app we need invoke Typer's call
+            return self.proxied(*args, **kwargs)
+        return _get_direct_function(self.command, self.proxied)(*args, **kwargs)
+
+    def __getattr__(self, name: str) -> t.Any:
+        """
+        If our proxied object __getattr__ returns a Typer or Command object we
+        wrap it in a BoundProxy so that it can be called directly as a method
+        on the django command instance.
+        """
+        if hasattr(self.proxied, name):
+            attr = getattr(self.proxied, name)
+            # want to avoid recursive binding
+            if isinstance(attr, (Typer, typer.models.CommandInfo)):
+                return BoundProxy(self.command, attr)
+            return attr
+
+        raise AttributeError(
+            "{cls} object has no attribute {name}".format(
+                cls=self.__class__.__name__, name=name
+            )
+        )
+
+    # def __repr__(self) -> str:
+    #     return f'<{self.__class__.__module__}.{self.__class__.__name__} for {repr(self.proxied)}>'
+
+
 def initialize(
     name: t.Optional[str] = Default(None),
     *,
-    cls: t.Type[TyperGroupWrapper] = TyperGroupWrapper,
+    cls: t.Type[DTGroup] = DTGroup,
     invoke_without_command: bool = Default(False),
     no_args_is_help: bool = Default(False),
     subcommand_metavar: t.Optional[str] = Default(None),
     chain: bool = Default(False),
     result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
     # Command
     context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
@@ -809,16 +1397,16 @@
     short_help: t.Optional[str] = Default(None),
     options_metavar: str = Default("[OPTIONS]"),
     add_help_option: bool = Default(True),
     hidden: bool = Default(False),
     deprecated: bool = Default(False),
     # Rich settings
     rich_help_panel: t.Union[str, None] = Default(None),
-    **kwargs: t.Dict[str, t.Any],
-) -> t.Callable[[t.Callable[P, R]], t.Callable[P, R]]:
+    **kwargs,
+) -> t.Callable[[t.Callable[P2, R2]], t.Callable[P2, R2]]:
     """
     A function decorator that creates a Typer_
     `callback <https://typer.tiangolo.com/tutorial/commands/callback/>`_. This
     decorator wraps the
     `Typer.callback() <https://typer.tiangolo.com/tutorial/commands/callback/>`_
     functionality. We've renamed it to ``initialize()`` because ``callback()`` is
     to general and not intuitive. Callbacks in Typer_ are functions that are invoked
@@ -903,64 +1491,61 @@
     :param add_help_option: whether to add the help option to the command
     :param hidden: whether to hide this group from the help output
     :param deprecated: show a deprecation warning
     :param rich_help_panel: the rich help panel to use - if rich is installed
         this can be used to group commands into panels in the help output.
     """
 
-    def decorator(func: t.Callable[P, R]) -> t.Callable[P, R]:
-        setattr(
+    def make_initializer(func: t.Callable[P2, R2]) -> t.Callable[P2, R2]:
+        func = _check_static(func)
+        _cache_initializer(
             func,
-            "_typer_callback_",
-            lambda cmd, _name=None, _help=Default(
-                None
-            ), **extra: cmd.typer_app.callback(
-                name=name or _name,
-                cls=type("_AdaptedCallback", (cls,), {"django_command": cmd}),
-                invoke_without_command=invoke_without_command,
-                subcommand_metavar=subcommand_metavar,
-                chain=chain,
-                result_callback=result_callback,
-                context_settings=context_settings,
-                help=cmd.typer_app.info.help or help or _help,
-                epilog=epilog,
-                short_help=short_help,
-                options_metavar=options_metavar,
-                add_help_option=add_help_option,
-                no_args_is_help=no_args_is_help,
-                hidden=hidden,
-                deprecated=deprecated,
-                rich_help_panel=rich_help_panel,
-                **kwargs,
-                **extra,
-            )(
-                func
-            ),
+            common_init=True,
+            name=name,
+            cls=cls,
+            invoke_without_command=invoke_without_command,
+            subcommand_metavar=subcommand_metavar,
+            chain=chain,
+            result_callback=result_callback,
+            context_settings=context_settings,
+            help=help,
+            epilog=epilog,
+            short_help=short_help,
+            options_metavar=options_metavar,
+            add_help_option=add_help_option,
+            no_args_is_help=no_args_is_help,
+            hidden=hidden,
+            deprecated=deprecated,
+            rich_help_panel=rich_help_panel,
+            **kwargs,
         )
         return func
 
-    return decorator
+    return make_initializer
+
+
+callback = initialize  # allow callback as an alias
 
 
 def command(  # pylint: disable=keyword-arg-before-vararg
     name: t.Optional[str] = None,
     *,
-    cls: t.Type[TyperCommandWrapper] = TyperCommandWrapper,
+    cls: t.Type[DTCommand] = DTCommand,
     context_settings: t.Optional[t.Dict[t.Any, t.Any]] = None,
     help: t.Optional[str] = None,  # pylint: disable=redefined-builtin
     epilog: t.Optional[str] = None,
     short_help: t.Optional[str] = None,
     options_metavar: str = "[OPTIONS]",
     add_help_option: bool = True,
     no_args_is_help: bool = False,
     hidden: bool = False,
     deprecated: bool = False,
     # Rich settings
     rich_help_panel: t.Union[str, None] = Default(None),
-    **kwargs: t.Dict[str, t.Any],
+    **kwargs,
 ) -> t.Callable[[t.Callable[P, R]], t.Callable[P, R]]:
     """
     A function decorator that creates a new command and attaches it to the root
     command group. This is a passthrough to
     `Typer.command() <https://typer.tiangolo.com/tutorial/commands/>`_ and the
     options are the same, except we swap the default command class for our wrapper.
 
@@ -1010,44 +1595,41 @@
     :param no_args_is_help: whether to show the help if no arguments are provided
     :param hidden: whether to hide the command from help output
     :param deprecated: show a deprecation warning
     :param rich_help_panel: the rich help panel to use - if rich is installed
         this can be used to group commands into panels in the help output.
     """
 
-    def decorator(func: t.Callable[P, R]) -> t.Callable[P, R]:
-        setattr(
+    def make_command(func: t.Callable[P, R]) -> t.Callable[P, R]:
+        func = _check_static(func)
+        _cache_command(
             func,
-            "_typer_command_",
-            lambda cmd, _name=None, _help=None, **extra: cmd.typer_app.command(
-                name=name or _name,
-                cls=type("_AdaptedCommand", (cls,), {"django_command": cmd}),
-                context_settings=context_settings,
-                help=help or _help,
-                epilog=epilog,
-                short_help=short_help,
-                options_metavar=options_metavar,
-                add_help_option=add_help_option,
-                no_args_is_help=no_args_is_help,
-                hidden=hidden,
-                deprecated=deprecated,
-                # Rich settings
-                rich_help_panel=rich_help_panel,
-                **kwargs,
-                **extra,
-            )(func),
+            name=name,
+            cls=cls,
+            context_settings=context_settings,
+            help=help,
+            epilog=epilog,
+            short_help=short_help,
+            options_metavar=options_metavar,
+            add_help_option=add_help_option,
+            no_args_is_help=no_args_is_help,
+            hidden=hidden,
+            deprecated=deprecated,
+            # Rich settings
+            rich_help_panel=rich_help_panel,
+            **kwargs,
         )
         return func
 
-    return decorator
+    return make_command
 
 
 def group(
     name: t.Optional[str] = Default(None),
-    cls: t.Type[TyperGroupWrapper] = TyperGroupWrapper,
+    cls: t.Type[DTGroup] = DTGroup,
     invoke_without_command: bool = Default(False),
     no_args_is_help: bool = Default(False),
     subcommand_metavar: t.Optional[str] = Default(None),
     chain: bool = Default(False),
     result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
     # Command
     context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
@@ -1056,16 +1638,16 @@
     short_help: t.Optional[str] = Default(None),
     options_metavar: str = Default("[OPTIONS]"),
     add_help_option: bool = Default(True),
     hidden: bool = Default(False),
     deprecated: bool = Default(False),
     # Rich settings
     rich_help_panel: t.Union[str, None] = Default(None),
-    **kwargs: t.Dict[str, t.Any],
-) -> t.Callable[[t.Callable[..., t.Any]], GroupFunction]:
+    **kwargs,
+) -> t.Callable[[t.Callable[P, R]], Typer[P, R]]:
     """
     A function decorator that creates a new subgroup and attaches it to the root
     command group. This is like creating a new Typer_ app and adding it to a parent
     Typer app. The kwargs are passed through to the Typer() constructor. The group()
     functions work like :func:`~django_typer.initialize` functions for their command
     groups.
 
@@ -1122,16 +1704,16 @@
     :param add_help_option: whether to add the help option to the command
     :param hidden: whether to hide this group from the help output
     :param deprecated: show a deprecation warning
     :param rich_help_panel: the rich help panel to use - if rich is installed
         this can be used to group commands into panels in the help output.
     """
 
-    def create_app(func: t.Callable[..., t.Any]) -> GroupFunction:
-        grp = GroupFunction(  # type: ignore
+    def create_app(func: t.Callable[P, R]) -> Typer[P, R]:
+        grp = Typer(
             name=name,
             cls=cls,
             invoke_without_command=invoke_without_command,
             no_args_is_help=no_args_is_help,
             subcommand_metavar=subcommand_metavar,
             chain=chain,
             result_callback=result_callback,
@@ -1141,21 +1723,151 @@
             epilog=epilog,
             short_help=short_help,
             options_metavar=options_metavar,
             add_help_option=add_help_option,
             hidden=hidden,
             deprecated=deprecated,
             rich_help_panel=rich_help_panel,
+            parent=None,
+            top_level=True,
             **kwargs,
         )
         return grp
 
     return create_app
 
 
+def _add_common_initializer(
+    cmd: t.Union["TyperCommandMeta", t.Type["TyperCommand"], "TyperCommand"],
+) -> t.Optional[typer.models.TyperInfo]:
+    """
+    Add a callback to the typer app that will add the unsuppressed
+    common django base command parameters to the CLI if the command
+    is a compound command and no existing callback is registered.
+
+    :param cmd: The command class or instance.
+    :return: The callback that was/is registered on the command
+    """
+    if cmd.is_compound_command and not cmd.typer_app.registered_callback:
+        cmd.typer_app.callback(
+            cls=type(
+                "_Initializer",
+                (DTGroup,),
+                {
+                    "django_command": cmd,
+                    "_callback_is_method": False,
+                    "common_init": True,
+                },
+            )
+        )(lambda: None)
+    return cmd.typer_app.registered_callback
+
+
+def _resolve_help(dj_cmd: "TyperCommand"):
+    """
+    If no help string would be rendered for the root level command and a class docstring is
+    present, use it as the help string.
+
+    :param dj_cmd: The TyperCommand to resolve the help string for.
+    """
+    hlp = None
+    for cmd_cls in [
+        c
+        for c in dj_cmd.__class__.__mro__
+        if issubclass(c, TyperCommand) and c is not TyperCommand
+    ]:
+        hlp = cmd_cls.__doc__
+        if hlp:
+            break
+    if hlp:
+        if dj_cmd.typer_app.registered_callback:
+            cb = dj_cmd.typer_app.registered_callback
+            if not cb.help and not cb.callback.__doc__:
+                cb.help = hlp
+        else:
+            cmd = (
+                dj_cmd.typer_app.registered_commands[0]
+                if dj_cmd.typer_app.registered_commands
+                else None
+            )
+            if cmd and not cmd.help and not cmd.callback.__doc__:
+                cmd.help = hlp
+            elif not dj_cmd.typer_app.info.help:
+                dj_cmd.typer_app.info.help = hlp
+
+
+def _names(tc: t.Union[typer.models.CommandInfo, Typer]) -> t.List[str]:
+    """
+    For a command or group, get a list of attribute name and its CLI name.
+
+    This annoyingly lives in difference places depending on how the command
+    or group was defined. This logic is sensitive to typer internals.
+    """
+    names = []
+    if isinstance(tc, typer.models.CommandInfo):
+        assert tc.callback
+        names.append(tc.callback.__name__)
+        if tc.name and tc.name != tc.callback.__name__:
+            names.append(tc.name)
+    else:
+        if tc.name:
+            names.append(tc.name)
+        if tc.info.name and tc.info.name != tc.name:
+            names.append(tc.info.name)
+    return names
+
+
+def _bfs_match(
+    app: Typer, name: str
+) -> t.Optional[t.Union[typer.models.CommandInfo, Typer]]:
+    """
+    Perform a breadth first search for a command or group by name.
+
+    :param app: The Typer app to search.
+    :param name: The name of the command or group to search for.
+    :return: The command or group if found, otherwise None.
+    """
+
+    def find_at_level(
+        lvl: Typer,
+    ) -> t.Optional[t.Union[typer.models.CommandInfo, Typer]]:
+        for cmd in reversed(lvl.registered_commands):
+            if name in _names(cmd):
+                return cmd
+        if name in _names(lvl):
+            return lvl
+        return None
+
+    # fast exit out if at top level (most searches - avoid building BFS)
+    if found := find_at_level(app):
+        return found
+
+    bfs_order: t.List[Typer] = []
+    queue = deque([app])
+
+    while queue:
+        grp = queue.popleft()
+        bfs_order.append(grp)
+        # if names conflict, only pick the first the others have been
+        # overridden - avoids walking down stale branches
+        seen = []
+        for child_grp in reversed(grp.registered_groups):
+            child_app = t.cast(Typer, child_grp.typer_instance)
+            assert child_app
+            if child_app.name not in seen:
+                seen.extend(_names(child_app))
+                queue.append(child_app)
+
+    for grp in bfs_order[1:]:
+        found = find_at_level(grp)
+        if found:
+            return found
+    return None
+
+
 class TyperCommandMeta(type):
     """
     The metaclass used to build the TyperCommand class. This metaclass is responsible
     for building Typer app using the arguments supplied to the TyperCommand constructor.
     It also discovers if handle() was supplied as the single command implementation.
 
     .. warning::
@@ -1213,25 +1925,28 @@
     stdout: BaseOutputWrapper
     stderr: BaseOutputWrapper
     requires_system_checks: t.Union[t.Sequence[str], str]
     suppressed_base_arguments: t.Optional[t.Iterable[str]]
     typer_app: Typer
     no_color: bool
     force_color: bool
-    _num_commands: int = 0
-    _has_callback: bool = False
-    _root_groups: int = 0
+    is_compound_command: bool
     _handle: t.Optional[t.Callable[..., t.Any]]
 
+    # this holds the Typer app commands and groups defined directly on the class
+    # and its parents.
+    _defined_groups: t.Dict[str, Typer] = {}
+
     def __new__(
         mcs,
-        name,
+        cls_name,
         bases,
         attrs,
-        cls: t.Optional[t.Type[CoreTyperGroup]] = TyperGroupWrapper,
+        name: t.Optional[str] = Default(None),
+        # cls: t.Optional[t.Type[DTGroup]] = DTGroup,
         invoke_without_command: bool = Default(False),
         no_args_is_help: bool = Default(False),
         subcommand_metavar: t.Optional[str] = Default(None),
         chain: bool = Default(False),
         result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
         context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
         callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
@@ -1245,14 +1960,15 @@
         rich_markup_mode: MarkupMode = None,
         rich_help_panel: t.Union[str, None] = Default(None),
         pretty_exceptions_enable: t.Union[DefaultPlaceholder, bool] = Default(True),
         pretty_exceptions_show_locals: t.Union[DefaultPlaceholder, bool] = Default(
             True
         ),
         pretty_exceptions_short: t.Union[DefaultPlaceholder, bool] = Default(True),
+        **kwargs,
     ):
         """
         This method is called when a new class is created.
         """
         try:
             # avoid unnecessary work creating the TyperCommand class
             # is there a less weird way to do this?
@@ -1273,18 +1989,31 @@
                     "show_locals", pretty_exceptions_show_locals
                 )
             if isinstance(pretty_exceptions_short, DefaultPlaceholder):
                 pretty_exceptions_short = tb_config.get(
                     "short", pretty_exceptions_short
                 )
 
+            attr_help = attrs.get("help", Default(None))
+            if not help:
+                for base in [base for base in bases if issubclass(base, TyperCommand)]:
+                    if isinstance(help, DefaultPlaceholder):
+                        help = base._help_kwarg  # type: ignore[unreachable]
+                    if isinstance(attr_help, DefaultPlaceholder):
+                        attr_help = base.help
+
+            def command_bases() -> t.Generator[t.Type[TyperCommand], None, None]:
+                for base in reversed(bases):
+                    if issubclass(base, TyperCommand) and base is not TyperCommand:
+                        yield base
+
             typer_app = Typer(
-                name=mcs.__module__.rsplit(".", maxsplit=1)[-1],
-                cls=cls,
-                help=help or attrs.get("help", Default(None)),
+                name=name or attrs.get("__module__", "").rsplit(".", maxsplit=1)[-1],
+                cls=kwargs.pop("cls", DTGroup),
+                help=help or attr_help,  # pyright: ignore[reportArgumentType]
                 invoke_without_command=invoke_without_command,
                 no_args_is_help=no_args_is_help,
                 subcommand_metavar=subcommand_metavar,
                 chain=chain,
                 result_callback=result_callback,
                 context_settings=context_settings,
                 callback=callback,
@@ -1298,94 +2027,128 @@
                 rich_markup_mode=rich_markup_mode,
                 rich_help_panel=rich_help_panel,
                 pretty_exceptions_enable=pretty_exceptions_enable,
                 pretty_exceptions_show_locals=t.cast(
                     bool, pretty_exceptions_show_locals
                 ),
                 pretty_exceptions_short=t.cast(bool, pretty_exceptions_short),
+                **kwargs,
             )
 
+            # move up here
+            def get_ctor(attr: t.Any) -> t.Optional[t.Callable[..., t.Any]]:
+                return getattr(attr, _CACHE_KEY, None)
+
+            # because we're mapping a non-class based interface onto a class based
+            # interface, we have to handle this class mro stuff manually here
+            handle = None  # there can be only one or none
+            _defined_groups: t.Dict[str, Typer] = {}
+            to_remove = []
+            to_register = []
+            local_handle = attrs.pop("handle", None)
+            for cmd_cls, cls_attrs in [
+                *[(base, vars(base)) for base in command_bases()],
+                (None, attrs),
+            ]:
+                for name, attr in list(cls_attrs.items()):
+                    if name == "_handle":
+                        continue
+                    if name == "_defined_groups":
+                        _defined_groups = {**_defined_groups, **attr}
+                        continue
+                    if name != "typer_app" and isinstance(attr, Typer):
+                        assert name
+                        to_remove.append(name)
+                        _defined_groups[name] = attr
+                    elif register := get_ctor(attr):
+                        to_register.append(register)
+
+                handle = getattr(cmd_cls, "_handle", handle)
+
+            handle = local_handle or handle
+
+            for grp in set(_defined_groups.values()):
+                if grp.top_level:
+                    cpy = deepcopy(grp)
+                    cpy.parent = typer_app
+                    typer_app.add_typer(cpy)
+
+            # remove the groups from the class to allow __getattr__ to control
+            # which group instance is returned based on call context
+            for name in to_remove:
+                attrs.pop(name)
+
+            attrs["_defined_groups"] = _defined_groups
+
+            if handle:
+                ctor = get_ctor(handle)
+                if ctor:
+                    to_register.append(
+                        lambda cmd_cls: ctor(
+                            cmd_cls,
+                            _name=typer_app.info.name,
+                            _help=attrs.get("help", Default(None)),
+                        )
+                    )
+                else:
+                    to_register.append(
+                        lambda _: typer_app.command(
+                            typer_app.info.name,
+                            help=typer_app.info.help or None,
+                        )(handle)
+                    )
+
             attrs = {
-                "_handle": attrs.pop("handle", None),
                 **attrs,
+                "_handle": handle,
+                "_to_register": to_register,
                 "typer_app": typer_app,
             }
 
-        return super().__new__(mcs, name, bases, attrs)
+        else:
+            # we do this to avoid typing complaints on handle overrides
+            attrs["handle"] = attrs.pop("_run")
+
+        if help:
+            attrs["_help_kwarg"] = help
+
+        return super().__new__(mcs, cls_name, bases, attrs)
 
-    def __init__(cls, name, bases, attrs, **kwargs):
+    def __init__(cls, cls_name, bases, attrs, **kwargs):
         """
         This method is called after a new class is created.
         """
+        cls = t.cast(t.Type["TyperCommand"], cls)
         if getattr(cls, "typer_app", None):
-            cls.typer_app.info.name = cls.__module__.rsplit(".", maxsplit=1)[-1]
-            cls.suppressed_base_arguments = {
-                arg.lstrip("--").replace("-", "_")
-                for arg in cls.suppressed_base_arguments or []
-            }  # per django docs - allow these to be specified by either the option or param name
-
-            def get_ctor(attr: t.Any) -> t.Optional[t.Callable[..., t.Any]]:
-                return getattr(
-                    attr, "_typer_command_", getattr(attr, "_typer_callback_", None)
-                )
-
-            # because we're mapping a non-class based interface onto a class based
-            # interface, we have to handle this class mro stuff manually here
-            for cmd_cls, cls_attrs in [
-                *[(base, vars(base)) for base in reversed(bases)],
-                (cls, attrs),
-            ]:
-                if not issubclass(cmd_cls, TyperCommand) or cmd_cls is TyperCommand:
-                    continue
-                for attr in [*cls_attrs.values(), cls._handle]:
-                    cls._num_commands += hasattr(attr, "_typer_command_")
-                    cls._has_callback |= hasattr(attr, "_typer_callback_")
-                    if isinstance(attr, GroupFunction) and not attr.bound:
-                        attr.bind(cls)  # type: ignore
-                        cls._root_groups += 1
-
-                if cmd_cls._handle:
-                    ctor = get_ctor(cmd_cls._handle)
-                    if ctor:
-                        ctor(
-                            cls,
-                            _name=cls.typer_app.info.name,
-                            _help=getattr(cls, "help", None),
-                        )
-                    else:
-                        cls._num_commands += 1
-                        cls.typer_app.command(
-                            cls.typer_app.info.name,
-                            cls=type(
-                                "_AdaptedCommand",
-                                (TyperCommandWrapper,),
-                                {"django_command": cls},
-                            ),
-                            help=cls.typer_app.info.help or None,
-                        )(cmd_cls._handle)
+            cls.typer_app.django_command = cls
+            cls.typer_app.info.name = (
+                cls.typer_app.info.name or cls.__module__.rsplit(".", maxsplit=1)[-1]
+            )
+            for cmd in getattr(cls, "_to_register", []):
+                cmd(cls)
 
-                for attr in cls_attrs.values():
-                    (get_ctor(attr) or (lambda _: None))(cls)
+            _add_common_initializer(cls)
 
-            if (
-                cls._num_commands > 1 or cls._root_groups > 0
-            ) and not cls.typer_app.registered_callback:
-                cls.typer_app.callback(
-                    cls=type(
-                        "_AdaptedCallback",
-                        (TyperGroupWrapper,),
-                        {
-                            "django_command": cls,
-                            "callback_is_method": False,
-                            "common_init": True,
-                        },
-                    )
-                )(lambda: None)
+        super().__init__(cls_name, bases, attrs, **kwargs)
 
-        super().__init__(name, bases, attrs, **kwargs)
+    def __getattr__(cls, name: str) -> t.Any:
+        """
+        Fall back breadth first search of the typer app tree to resolve attribute accesses of the type:
+            Command.sub_grp or Command.sub_cmd
+        """
+        if name != "typer_app":
+            if called_from_command_definition():
+                if name in cls._defined_groups:
+                    return cls._defined_groups[name]
+            found = _bfs_match(cls.typer_app, name)
+            if found:
+                return found
+        raise AttributeError(
+            "{cls} object has no attribute {name}".format(cls=cls.__name__, name=name)
+        )
 
 
 class CommandNode:
     """
     A tree node that represents a command in the command tree. This is used to
     walk the click command hierarchy and produce helps and map command paths
     to command functions. The command tree is built on TyperCommand initialization.
@@ -1394,34 +2157,77 @@
     :param click_command: the click command object
     :param context: the click context object
     :param django_command: the django command instance
     :param parent: the parent node or None if this is a root node
     """
 
     name: str
-    click_command: click.Command
-    context: TyperContext
+    """
+    The name of the group or command that this node represents.
+    """
+
+    click_command: DjangoTyperMixin
+    """
+    The click command object that this node represents.
+    """
+
+    context: Context
+    """
+    The Typer context object used to run this command.
+    """
+
     django_command: "TyperCommand"
-    parent: t.Optional["CommandNode"] = None
-    children: t.Dict[str, "CommandNode"]
+    """
+    Back reference to the django command instance that this command belongs to.
+    """
+
+    @cached_property
+    def children(self) -> t.Dict[str, "CommandNode"]:
+        """
+        The child group and command nodes of this command node.
+        """
+        return {
+            name: CommandNode(name, cmd, self.django_command, parent=self.context)
+            for name, cmd in getattr(
+                self.context.command,
+                "commands",
+                {
+                    name: self.context.command.get_command(self.context, name)  # type: ignore[attr-defined]
+                    for name in (
+                        self.context.command.list_commands(self.context)
+                        if isinstance(self.context.command, click.MultiCommand)
+                        else []
+                    )
+                },
+            ).items()
+        }
+
+    @property
+    def callback(self) -> t.Callable[..., t.Any]:
+        """Get the function for this command or group"""
+        return _get_direct_function(
+            self.django_command, getattr(self.click_command._callback, "__wrapped__")
+        )
 
     def __init__(
         self,
         name: str,
-        click_command: click.Command,
-        context: TyperContext,
+        click_command: DjangoTyperMixin,
         django_command: "TyperCommand",
-        parent: t.Optional["CommandNode"] = None,
+        parent: t.Optional[Context] = None,
     ):
         self.name = name
         self.click_command = click_command
-        self.context = context
         self.django_command = django_command
-        self.parent = parent
-        self.children = {}
+        self.context = Context(
+            self.click_command,
+            info_name=name,
+            django_command=django_command,
+            parent=parent,
+        )
 
     def print_help(self) -> t.Optional[str]:
         """
         Prints the help for this command to stdout of the django command.
         """
         # if rich is installed this prints the help, if it is not it
         # returns the help as a string - we deal with this higher on the
@@ -1429,25 +2235,35 @@
         return self.click_command.get_help(self.context)
 
     def get_command(self, *command_path: str) -> "CommandNode":
         """
         Return the command node for the given command path at or below
         this node.
 
-        :param command_path: the path(s) to the command to retrieve
-        :return: the command node at the given path
+        :param command_path: the parent group names followed by the name of the command
+            or group to retrieve
+        :return: the command node at the given group/subcommand path
         :raises LookupError: if the command path does not exist
         """
         if not command_path:
             return self
         try:
             return self.children[command_path[0]].get_command(*command_path[1:])
         except KeyError as err:
             raise LookupError(f'No such command "{command_path[0]}"') from err
 
+    def __call__(self, *args, **kwargs) -> t.Any:
+        """
+        Call this command or group directly.
+
+        :param args: the arguments to pass to the command or group callback
+        :param kwargs: the named parameters to pass to the command or group callback
+        """
+        return self.callback(*args, **kwargs)
+
 
 class TyperParser:
     """
     A class that conforms to the argparse.ArgumentParser interface that the django
     base class works with that is returned by BaseCommand.create_parser(). This class
     does not strictly conform to the argparse interface but does just enough to
     satisfy the django base class.
@@ -1484,47 +2300,49 @@
             The number of arguments consumed by this parameter or 0 if it is a flag.
             """
             return 0 if getattr(self.param, "is_flag", False) else self.param.nargs
 
         @property
         def option_strings(self) -> t.List[str]:
             """
-            The list of allowable command line option strings for this parameter.
+            call_command uses this to determine a mapping of supplied options to function
+            arguments. I.e. it will remap option_string: dest. We don't want this because
+            we'd rather have supplied parameters line up with their function arguments to
+            allow deconfliction when CLI options share the same name.
             """
-            return list(self.param.opts) if isinstance(self.param, click.Option) else []
+            return []
 
     _actions: t.List[t.Any]
     _mutually_exclusive_groups: t.List[t.Any] = []
 
     django_command: "TyperCommand"
     prog_name: str
     subcommand: str
 
     def __init__(self, django_command: "TyperCommand", prog_name, subcommand):
         self._actions = []
         self.django_command = django_command
         self.prog_name = prog_name
         self.subcommand = subcommand
+        self.tree = self.django_command.command_tree
+        self.tree.context.info_name = f"{self.prog_name} {self.subcommand}"
 
         def populate_params(node: CommandNode) -> None:
             for param in node.click_command.params:
                 self._actions.append(self.Action(param))
             for child in node.children.values():
                 populate_params(child)
 
-        populate_params(self.django_command.command_tree)
+        populate_params(self.tree)
 
     def print_help(self, *command_path: str):
         """
         Print the help for the given command path to stdout of the django command.
         """
-        self.django_command.command_tree.context.info_name = (
-            f"{self.prog_name} {self.subcommand}"
-        )
-        command_node = self.django_command.get_subcommand(*command_path)
+        command_node = self.tree.get_command(*command_path)
         hlp = command_node.print_help()
         if hlp:
             self.django_command.stdout.write(
                 hlp, style_func=lambda msg: msg, ending="\n\n"
             )
 
     def parse_args(self, args=None, namespace=None) -> _ParsedArgs:
@@ -1665,15 +2483,15 @@
           markdown rendering in help output.
         - Using the chain parameter to enable `command chaining
           <https://click.palletsprojects.com/commands/#multi-command-chaining>`_.
 
 
     We can see that our help renders like so:
 
-    .. typer:: django_typer.tests.test_app.management.commands.chain.Command:typer_app
+    .. typer:: django_typer.tests.apps.test_app.management.commands.chain.Command:typer_app
         :prog: ./manage.py chain
         :width: 80
         :convert-png: latex
 
 
     And we can see the chain behavior by calling our command(s) like so:
 
@@ -1712,21 +2530,368 @@
     suppressed_base_arguments = {"verbosity"}
 
     missing_args_message = "Missing parameter: {parameter}"
 
     typer_app: Typer
     no_color: bool = False
     force_color: bool = False
-    _num_commands: int = 0
-    _has_callback: bool = False
-    _root_groups: int = 0
     _handle: t.Callable[..., t.Any]
     _traceback: bool = False
+    _help_kwarg: t.Optional[str] = Default(None)
+    _defined_groups: t.Dict[str, Typer] = {}
+
+    help: t.Optional[t.Union[DefaultPlaceholder, str]] = Default(None)  # type: ignore
+
+    # allow deriving commands to override handle() from BaseCommand
+    # without triggering static type checking complaints
+    handle = None  # type: ignore
+
+    @property
+    def command_tree(self) -> CommandNode:
+        """
+        Get the root CommandNode for this command. Allows easy traversal of the command
+        tree.
+        """
+        return CommandNode(
+            f"{sys.argv[0]} {self._name}",
+            click_command=t.cast(DjangoTyperMixin, get_typer_command(self.typer_app)),
+            django_command=self,
+        )
+
+    @classmethod
+    def initialize(
+        cmd,  # pyright: ignore[reportSelfClsParameterName]
+        name: t.Optional[str] = Default(None),
+        *,
+        cls: t.Type[DTGroup] = DTGroup,
+        invoke_without_command: bool = Default(False),
+        no_args_is_help: bool = Default(False),
+        subcommand_metavar: t.Optional[str] = Default(None),
+        chain: bool = Default(False),
+        result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
+        # Command
+        context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
+        help: t.Optional[str] = Default(None),  # pylint: disable=redefined-builtin
+        epilog: t.Optional[str] = Default(None),
+        short_help: t.Optional[str] = Default(None),
+        options_metavar: str = Default("[OPTIONS]"),
+        add_help_option: bool = Default(True),
+        hidden: bool = Default(False),
+        deprecated: bool = Default(False),
+        # Rich settings
+        rich_help_panel: t.Union[str, None] = Default(None),
+        **kwargs,
+    ) -> t.Callable[[t.Callable[P, R]], t.Callable[P, R]]:
+        """
+        Override the initializer for this command class after it has been defined.
+
+        .. note::
+            See :ref:`plugins` for details on when you might want to use this extension
+            pattern.
+
+        .. code-block:: python
+
+            from your_app.management.commands.your_command import Command as YourCommand
+
+            @YourCommand.initialize()
+            def init(self, ...):
+                # implement your command initialization logic here
+
+        :param name: the name of the callback (defaults to the name of the decorated
+            function)
+        :param cls: the command class to use - (the initialize() function is technically
+            the root command group)
+        :param invoke_without_command: whether to invoke the callback if no command was
+            specified.
+        :param no_args_is_help: whether to show the help if no arguments are provided
+        :param subcommand_metavar: the metavar to use for subcommands in the help output
+        :param chain: whether to chain commands, this allows multiple commands from the group
+            to be specified and run in order sequentially in one call from the command line.
+        :param result_callback: a callback to invoke with the result of the command
+        :param context_settings: the click context settings to use - see
+            `click docs <https://click.palletsprojects.com/api/#context>`_.
+        :param help: the help string to use, defaults to the function docstring, if you need
+            to translate the help you should use the help kwarg instead because docstrings
+            will not be translated.
+        :param epilog: the epilog to use in the help output
+        :param short_help: the short help to use in the help output
+        :param options_metavar: the metavar to use for options in the help output
+        :param add_help_option: whether to add the help option to the command
+        :param hidden: whether to hide this group from the help output
+        :param deprecated: show a deprecation warning
+        :param rich_help_panel: the rich help panel to use - if rich is installed
+            this can be used to group commands into panels in the help output.
+        """
+        if called_from_command_definition():
+            return initialize(
+                name=name,
+                cls=cls,
+                context_settings=context_settings,
+                help=help,
+                epilog=epilog,
+                short_help=short_help,
+                options_metavar=options_metavar,
+                add_help_option=add_help_option,
+                invoke_without_command=invoke_without_command,
+                no_args_is_help=no_args_is_help,
+                subcommand_metavar=subcommand_metavar,
+                chain=chain,
+                result_callback=result_callback,
+                hidden=hidden,
+                deprecated=deprecated,
+                # Rich settings
+                rich_help_panel=rich_help_panel,
+                **kwargs,
+            )
+
+        def make_initializer(func: t.Callable[P, R]) -> t.Callable[P, R]:
+            # we might have to override a method defined in the base class
+            setattr(cmd, func.__name__, func)
+            cmd.typer_app.callback(
+                name=name,
+                cls=type("_Initializer", (cls,), {"django_command": cmd}),
+                context_settings=context_settings,
+                help=help,
+                epilog=epilog,
+                short_help=short_help,
+                options_metavar=options_metavar,
+                add_help_option=add_help_option,
+                invoke_without_command=invoke_without_command,
+                no_args_is_help=no_args_is_help,
+                subcommand_metavar=subcommand_metavar,
+                chain=chain,
+                result_callback=result_callback,
+                hidden=hidden,
+                deprecated=deprecated,
+                # Rich settings
+                rich_help_panel=rich_help_panel,
+                **kwargs,
+            )(_strip_static(func))
+            return func
+
+        return make_initializer
+
+    callback = initialize
+
+    @classmethod
+    def command(
+        cmd,  # pyright: ignore[reportSelfClsParameterName]
+        name: t.Optional[str] = None,
+        *,
+        cls: t.Type[DTCommand] = DTCommand,
+        context_settings: t.Optional[t.Dict[t.Any, t.Any]] = None,
+        help: t.Optional[str] = None,  # pylint: disable=redefined-builtin
+        epilog: t.Optional[str] = None,
+        short_help: t.Optional[str] = None,
+        options_metavar: str = "[OPTIONS]",
+        add_help_option: bool = True,
+        no_args_is_help: bool = False,
+        hidden: bool = False,
+        deprecated: bool = False,
+        # Rich settings
+        rich_help_panel: t.Union[str, None] = Default(None),
+        **kwargs,
+    ) -> t.Callable[[t.Callable[P, R]], t.Callable[P, R]]:
+        """
+        Add a command to this command class after it has been defined. You can
+        use this decorator to add commands to a root command from other Django apps.
+
+        .. note::
+            See :ref:`plugins` for details on when you might want to use this extension
+            pattern.
+
+        .. code-block:: python
+
+            from your_app.management.commands.your_command import Command as YourCommand
 
-    command_tree: CommandNode
+            @YourCommand.command()
+            def new_command(self, ...):
+                # implement your additional command here
+
+        :param name: the name of the command (defaults to the name of the decorated
+            function)
+        :param cls: the command class to use
+        :param context_settings: the context settings to use - see
+            `click docs <https://click.palletsprojects.com/api/#context>`_.
+        :param help: the help string to use, defaults to the function docstring, if
+            you need the help to be translated you should use the help kwarg instead
+            because docstrings will not be translated.
+        :param epilog: the epilog to use in the help output
+        :param short_help: the short help to use in the help output
+        :param options_metavar: the metavar to use for options in the help output
+        :param add_help_option: whether to add the help option to the command
+        :param no_args_is_help: whether to show the help if no arguments are provided
+        :param hidden: whether to hide the command from help output
+        :param deprecated: show a deprecation warning
+        :param rich_help_panel: the rich help panel to use - if rich is installed
+            this can be used to group commands into panels in the help output.
+        """
+        if called_from_command_definition():
+            return command(
+                name=name,
+                cls=cls,
+                context_settings=context_settings,
+                help=help,
+                epilog=epilog,
+                short_help=short_help,
+                options_metavar=options_metavar,
+                add_help_option=add_help_option,
+                no_args_is_help=no_args_is_help,
+                hidden=hidden,
+                deprecated=deprecated,
+                # Rich settings
+                rich_help_panel=rich_help_panel,
+                **kwargs,
+            )
+
+        def make_command(func: t.Callable[P, R]) -> t.Callable[P, R]:
+            # we might have to override a method defined in the base class
+            setattr(cmd, func.__name__, func)
+            cmd.typer_app.command(
+                name=name,
+                cls=type("_Command", (cls,), {"django_command": cmd}),
+                context_settings=context_settings,
+                help=help,
+                epilog=epilog,
+                short_help=short_help,
+                options_metavar=options_metavar,
+                add_help_option=add_help_option,
+                no_args_is_help=no_args_is_help,
+                hidden=hidden,
+                deprecated=deprecated,
+                # Rich settings
+                rich_help_panel=rich_help_panel,
+                **kwargs,
+            )(_strip_static(func))
+            return func
+
+        return make_command
+
+    @classmethod
+    def group(
+        cmd,  # pyright: ignore[reportSelfClsParameterName]
+        name: t.Optional[str] = Default(None),
+        cls: t.Type[DTGroup] = DTGroup,
+        invoke_without_command: bool = Default(False),
+        no_args_is_help: bool = Default(False),
+        subcommand_metavar: t.Optional[str] = Default(None),
+        chain: bool = Default(False),
+        result_callback: t.Optional[t.Callable[..., t.Any]] = Default(None),
+        # Command
+        context_settings: t.Optional[t.Dict[t.Any, t.Any]] = Default(None),
+        help: t.Optional[str] = Default(None),  # pylint: disable=redefined-builtin
+        epilog: t.Optional[str] = Default(None),
+        short_help: t.Optional[str] = Default(None),
+        options_metavar: str = Default("[OPTIONS]"),
+        add_help_option: bool = Default(True),
+        hidden: bool = Default(False),
+        deprecated: bool = Default(False),
+        # Rich settings
+        rich_help_panel: t.Union[str, None] = Default(None),
+        **kwargs,
+    ) -> t.Callable[[t.Callable[P, R]], Typer[P, R]]:
+        """
+        Add a group to this command class after it has been defined. You can
+        use this decorator to add groups to a root command from other Django apps.
+
+        .. note::
+            See :ref:`plugins` for details on when you might want to use this extension
+            pattern.
+
+        .. code-block:: python
+
+            from your_app.management.commands.your_command import Command as YourCommand
+
+            @YourCommand.group()
+            def new_group(self, ...):
+                # implement your group initializer here
+
+            @new_group.command()
+            def grp_command(self, ...):
+                # implement group subcommand here
+
+        :param name: the name of the group (defaults to the name of the decorated function)
+        :param cls: the group class to use
+        :param invoke_without_command: whether to invoke the group callback if no command
+            was specified.
+        :param no_args_is_help: whether to show the help if no arguments are provided
+        :param subcommand_metavar: the metavar to use for subcommands in the help output
+        :param chain: whether to chain commands, this allows multiple commands from the group
+            to be specified and run in order sequentially in one call from the command line.
+        :param result_callback: a callback to invoke with the result of the command
+        :param context_settings: the click context settings to use - see
+            `click docs <https://click.palletsprojects.com/api/#context>`_.
+        :param help: the help string to use, defaults to the function docstring, if you need
+            to translate the help you should use the help kwarg instead because docstrings
+            will not be translated.
+        :param epilog: the epilog to use in the help output
+        :param short_help: the short help to use in the help output
+        :param options_metavar: the metavar to use for options in the help output
+        :param add_help_option: whether to add the help option to the command
+        :param hidden: whether to hide this group from the help output
+        :param deprecated: show a deprecation warning
+        :param rich_help_panel: the rich help panel to use - if rich is installed
+            this can be used to group commands into panels in the help output.
+        """
+        if called_from_command_definition():
+            return group(
+                name=name,
+                cls=cls,
+                invoke_without_command=invoke_without_command,
+                no_args_is_help=no_args_is_help,
+                subcommand_metavar=subcommand_metavar,
+                chain=chain,
+                result_callback=result_callback,
+                context_settings=context_settings,
+                help=help,
+                epilog=epilog,
+                short_help=short_help,
+                options_metavar=options_metavar,
+                add_help_option=add_help_option,
+                hidden=hidden,
+                deprecated=deprecated,
+                rich_help_panel=rich_help_panel,
+                **kwargs,
+            )
+
+        def create_app(func: t.Callable[P, R]) -> Typer[P, R]:
+            grp: Typer[P, R] = Typer(
+                name=name,
+                cls=cls,
+                invoke_without_command=invoke_without_command,
+                no_args_is_help=no_args_is_help,
+                subcommand_metavar=subcommand_metavar,
+                chain=chain,
+                result_callback=result_callback,
+                callback=func,
+                context_settings=context_settings,
+                help=help,
+                epilog=epilog,
+                short_help=short_help,
+                options_metavar=options_metavar,
+                add_help_option=add_help_option,
+                hidden=hidden,
+                deprecated=deprecated,
+                rich_help_panel=rich_help_panel,
+                parent=None,
+                **kwargs,
+            )
+            cmd.typer_app.add_typer(grp)
+            return grp
+
+        return create_app
+
+    @classproperty
+    def is_compound_command(cls) -> bool:
+        """Return True if this command has more than a single executable block."""
+        return bool(
+            cls.typer_app.registered_groups
+            or len(cls.typer_app.registered_commands) > 1
+            or cls.typer_app.registered_callback
+        )
 
     @property
     def _name(self) -> str:
         """The name of the django command"""
         return self.typer_app.info.name or self.__module__.rsplit(".", maxsplit=1)[-1]
 
     def __enter__(self):
@@ -1765,16 +2930,21 @@
 
     def __init__(
         self,
         stdout: t.Optional[t.TextIO] = None,
         stderr: t.Optional[t.TextIO] = None,
         no_color: bool = no_color,
         force_color: bool = force_color,
-        **kwargs: t.Dict[str, t.Any],
+        **kwargs,
     ):
+        assert self.typer_app.info.name
+        _load_command_plugins(self.typer_app.info.name)
+        _add_common_initializer(self)
+        _resolve_help(self)
+
         self.force_color = force_color
         self.no_color = no_color
         with self:
             super().__init__(
                 stdout=stdout,
                 stderr=stderr,
                 no_color=no_color,
@@ -1785,79 +2955,33 @@
             # exceptions when strings are returned from command functions
             stdout_style_func = self.stdout.style_func
             stderr_style_func = self.stderr.style_func
             self.stdout = OutputWrapper(stdout or sys.stdout)
             self.stderr = OutputWrapper(stderr or sys.stderr)
             self.stdout.style_func = stdout_style_func
             self.stderr.style_func = stderr_style_func
-            self.command_tree = self._build_cmd_tree(get_typer_command(self.typer_app))
+            try:
+                assert get_typer_command(self.typer_app)
+            except RuntimeError as rerr:
+                raise NotImplementedError(
+                    _(
+                        "No commands or command groups were registered on {command}"
+                    ).format(command=self._name)
+                ) from rerr
 
     def get_subcommand(self, *command_path: str) -> CommandNode:
-        """Get the CommandNode"""
-        return self.command_tree.get_command(*command_path)
-
-    def _filter_commands(
-        self, ctx: TyperContext, cmd_filter: t.Optional[t.List[str]] = None
-    ):
-        """
-        Fetch subcommand names. Given a click context, return the list of commands
-        that are valid return the list of commands that are valid for the given
-        context.
-
-        :param ctx: the click context
-        :param cmd_filter: a list of command names to filter by, if None no subcommands
-            will be filtered out
-        :return: the list of command names that are valid for the given context
         """
-        return sorted(
-            [
-                cmd
-                for name, cmd in getattr(
-                    ctx.command,
-                    "commands",
-                    {
-                        name: ctx.command.get_command(ctx, name)  # type: ignore[attr-defined]
-                        for name in (
-                            ctx.command.list_commands(ctx)
-                            if isinstance(ctx.command, click.MultiCommand)
-                            else []
-                        )
-                    },
-                ).items()
-                if not cmd_filter or name in cmd_filter
-            ],
-            key=lambda item: item.name,
-        )
+        Retrieve a :class:`~django_typer.CommandNode` at the given command path.
 
-    def _build_cmd_tree(
-        self,
-        cmd: click.Command,
-        parent: t.Optional[Context] = None,
-        info_name: t.Optional[str] = None,
-        node: t.Optional[CommandNode] = None,
-    ):
+        :param command_path: the path to the command to retrieve, where each argument
+            is the string name in order of a group or command in the hierarchy.
+        :return: the command node at the given path
+        :raises LookupError: if no group or command exists at the given path
         """
-        Recursively build the CommandNode tree used to walk the click command
-        hierarchy.
-
-        :param cmd: the click command to build the tree from
-        :param parent: the parent click context
-        :param info_name: the name of the command
-        :param node: the parent node or None if this is a root node
-        """
-        assert cmd.name
-        ctx = Context(cmd, info_name=info_name, parent=parent, django_command=self)
-        current = CommandNode(cmd.name, cmd, ctx, self, parent=node)
-        if node:
-            node.children[cmd.name] = current
-        for sub_cmd in self._filter_commands(ctx):
-            self._build_cmd_tree(
-                sub_cmd, parent=ctx, info_name=sub_cmd.name, node=current
-            )
-        return current
+        return self.command_tree.get_command(*command_path)
 
     def __init_subclass__(cls, **_):
         """Avoid passing typer arguments up the subclass init chain"""
         return super().__init_subclass__()
 
     def create_parser(  # pyright: ignore[reportIncompatibleMethodOverride]
         self, prog_name: str, subcommand: str, **_
@@ -1875,15 +2999,14 @@
                 script = get_usage_script(prog_name)
                 if isinstance(script, Path):
                     prog_name = str(script)
                     if not str(prog_name).startswith(("..", "/", ".")):
                         prog_name = f"./{prog_name}"
                 else:
                     prog_name = str(script)
-
             return TyperParser(self, prog_name, subcommand)
 
     def print_help(self, prog_name: str, subcommand: str, *cmd_path: str):
         """
         Print the help message for this command to stdout of the django command.
 
         :param prog_name: the name of the manage script that invoked the command
@@ -1891,14 +3014,36 @@
         :param cmd_path: the path to the command to print the help for. This is
             an extension to the pase class print_help() interface, required because
             typer/click have different helps for each subgroup or subcommand.
         """
         with self:
             self.create_parser(prog_name, subcommand).print_help(*cmd_path)
 
+    def __getattr__(self, name: str) -> t.Any:
+        """
+        Do a breadth first search of the typer app tree to find a command or group
+        and return that command or group if the attribute name matches the command/group
+        function OR its registered CLI name.
+        """
+        init = getattr(
+            self.typer_app.registered_callback,
+            "callback",
+            self.typer_app.info.callback,
+        )
+        if init and init and name == init.__name__:
+            return BoundProxy(self, init)
+        found = _bfs_match(self.typer_app, name)
+        if found:
+            return BoundProxy(self, found)
+        raise AttributeError(
+            "{cls} object has no attribute {name}".format(
+                cls=self.__class__.__name__, name=name
+            )
+        )
+
     def __call__(self, *args, **kwargs):
         """
         Call this command's derived class handle() implementation directly. Note this
         does not call the handle() function below - but the handle() function that
         was implemented on the deriving class if one exists.
 
         When simple commands are implemented using only the handle() function we may
@@ -1922,34 +3067,40 @@
             multiple commands and groups are not required to implement handle() and
             for those commands the functions should be invoked directly.
 
         :param args: the arguments to directly pass to handle()
         :param kwargs: the options to directly pass to handle()
         """
         with self:
-            if getattr(self, "_handle", None) and callable(self._handle):
-                return self._handle(*args, **kwargs)
+            handle = getattr(self, "_handle", None) or getattr(
+                self.typer_app,
+                "handle",
+                None,  # registered dynamically
+            )
+            if callable(handle):
+                return handle(*args, **kwargs)
             raise NotImplementedError(
                 _(
                     "{cls} does not implement handle(), you must call the other command "
                     "functions directly."
                 ).format(cls=self.__class__)
             )
 
-    def handle(self, *args, **options):
+    @t.no_type_check
+    def _run(self, *args, **options):
         """
         Invoke the underlying Typer app with the given arguments and parameters.
 
         :param args: the arguments to pass to the command, may be strings needing
             to be parsed, or already resolved object types the argument ultimately
             resolves to. TODO - check this is true
         :param options: the options to pass to the command, may be strings needing
             to be parsed, or already resolved object types the option ultimately
             resolves to.
-        :return: Any object returned by the Typer app
+        :return: t.Any object returned by the Typer app
         """
         with self:
             return self.typer_app(
                 args=args,
                 standalone_mode=False,
                 supplied_params=options,
                 django_command=self,
@@ -1977,21 +3128,66 @@
         below this call may use get_current_command() to get a reference
         to the command instance.
 
         args and options are passed to handle().
 
         :param args: the arguments to pass to the command
         :param options: the options to pass to the command
-        :return: Any object returned by the command
+        :return: t.Any object returned by the command
         """
         no_color = self.no_color
         force_color = self.force_color
         if options.get("no_color", None) is not None:
             self.no_color = options["no_color"]
         if options.get("force_color", None) is not None:
             self.force_color = options["force_color"]
         try:
             with self:
                 return super().execute(*args, **options)
         finally:
             self.no_color = no_color
             self.force_color = force_color
+
+    def echo(
+        self, message: t.Optional[t.Any] = None, nl: bool = True, err: bool = False
+    ):
+        """
+        A wrapper for `typer.echo() <https://typer.tiangolo.com/tutorial/printing/#typer-echo>`_
+        that response --no-color and --force-color flags, and writes to the command's stdout.
+
+        :param message: The string or bytes to output. Other objects are
+            converted to strings.
+        :param err: Write to ``stderr`` instead of ``stdout``.
+        :param nl: Print a newline after the message. Enabled by default.
+        """
+
+        return typer.echo(
+            message=message,
+            file=t.cast(t.IO[str], self.stderr._out if err else self.stdout._out),
+            nl=nl,
+            color=False if self.no_color else True if self.force_color else None,
+        )
+
+    def secho(
+        self,
+        message: t.Optional[t.Any] = None,
+        nl: bool = True,
+        err: bool = False,
+        **styles: t.Any,
+    ):
+        """
+        A wrapper for `typer.secho() <https://typer.tiangolo.com/tutorial/printing/#typersecho-style-and-print>`_
+        that response --no-color and --force-color flags, and writes to the command's stdout.
+
+        :param message: The string or bytes to output. Other objects are
+            converted to strings.
+        :param err: Write to ``stderr`` instead of ``stdout``.
+        :param nl: Print a newline after the message. Enabled by default.
+        :param styles: Styles to apply to the output
+        """
+        return typer.secho(
+            message=message,
+            file=t.cast(t.IO[str], self.stderr._out if err else self.stdout._out),
+            nl=nl,
+            color=False if self.no_color else True if self.force_color else None,
+            **styles,
+        )
```

### Comparing `django_typer-1.1.2/django_typer/apps.py` & `django_typer-2.0.0/django_typer/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 import inspect
 import os
 import typing as t
 from types import ModuleType
 
 from django.apps import AppConfig
 from django.conf import settings
-from django.core.checks import CheckMessage
+from django.core.checks import CheckMessage, register
 from django.core.checks import Warning as CheckWarning
-from django.core.checks import register
 from django.utils.translation import gettext as _
 
 from django_typer import patch
 from django_typer.utils import traceback_config
 
 patch.apply()
```

### Comparing `django_typer-1.1.2/django_typer/management/commands/shellcompletion.py` & `django_typer-2.0.0/django_typer/management/commands/shellcompletion.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,18 @@
 )
 from django.core.management import CommandError, ManagementUtility
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
 from shellingham import ShellDetectionFailure, detect_shell
 from typer import Argument, Option, echo
-from typer.completion import Shells  # type: ignore
-from typer.completion import completion_init  # type: ignore
+from typer.completion import (  # type: ignore
+    Shells,  # pyright: ignore[reportPrivateImportUsage]
+    completion_init,  # pyright: ignore[reportPrivateImportUsage]
+)
 
 from django_typer import TyperCommand, command, get_command
 from django_typer.utils import get_usage_script
 
 DETECTED_SHELL = None
 
 try:
@@ -249,17 +251,15 @@
                 f"{self.manage_script} {DJANGO_COMMAND} complete",
                 [1, 2],
             )
         else:
             assert shell in [
                 Shells.pwsh,
                 Shells.powershell,
-            ], gettext(
-                "Unsupported shell: {shell}"
-            ).format(shell=shell.value)
+            ], gettext("Unsupported shell: {shell}").format(shell=shell.value)
             script = replace(
                 typer_scripts.COMPLETION_SCRIPT_POWER_SHELL,
                 "%(prog_name)s",
                 f"{self.manage_script} {DJANGO_COMMAND} complete",
                 [0],
             )
             typer_scripts._completion_scripts[Shells.powershell.value] = script
@@ -585,15 +585,15 @@
                         # if we're here a user is probably trying to debug a completion
                         # notify them that the command is not recognized
                         raise CommandError(
                             gettext('Unrecognized command: "{cmd_str}"').format(
                                 cmd_str=cmd_str
                             )
                         ) from err
-                    raise  # otherwise nowhere to go - just error out
+                    return  # otherwise nowhere to go
 
                 if isinstance(cmd, TyperCommand):  # type: ignore[unreachable]
                     # this will exit out so no return is needed here
                     cmd.typer_app(
                         args=args[cmd_idx + 1 :],
                         standalone_mode=True,
                         django_command=cmd,
```

### Comparing `django_typer-1.1.2/django_typer/parsers.py` & `django_typer-2.0.0/django_typer/parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 import typing as t
 from uuid import UUID
 
 from click import Context, Parameter, ParamType
 from django.apps import AppConfig, apps
 from django.core.management import CommandError
-from django.db.models import Field, ForeignObjectRel, Model, UUIDField
+from django.db import models
 from django.utils.translation import gettext as _
 
 from django_typer.completers import ModelObjectCompleter
 
 
 class ModelObjectParser(ParamType):
     """
@@ -66,54 +66,65 @@
     :param lookup_field: The field to use for lookup. Defaults to 'pk'.
     :param on_error: A callable that will be called if the lookup fails.
         The callable should accept three arguments: the model class, the
         value that failed to lookup, and the exception that was raised.
         If not provided, a CommandError will be raised.
     """
 
-    error_handler = t.Callable[[t.Type[Model], str, Exception], None]
+    error_handler = t.Callable[[t.Type[models.Model], str, Exception], None]
 
-    model_cls: t.Type[Model]
+    model_cls: t.Type[models.Model]
     lookup_field: str
     case_insensitive: bool = False
     on_error: t.Optional[error_handler] = None
 
     _lookup: str = ""
-    _field: Field
+    _field: models.Field
     _completer: ModelObjectCompleter
 
     __name__: str = "MODEL"  # typer internals expect this
 
+    def _get_metavar(self) -> str:
+        if isinstance(self._field, models.IntegerField):
+            return "INT"
+        elif isinstance(self._field, models.EmailField):
+            return "EMAIL"
+        elif isinstance(self._field, models.URLField):
+            return "URL"
+        elif isinstance(self._field, models.GenericIPAddressField):
+            return "[IPv4|IPv6]"
+        elif isinstance(self._field, models.UUIDField):
+            return "UUID"
+        elif isinstance(self._field, (models.FloatField, models.DecimalField)):
+            return "FLOAT"
+        return "TXT"
+
     def __init__(
         self,
-        model_cls: t.Type[Model],
+        model_cls: t.Type[models.Model],
         lookup_field: t.Optional[str] = None,
         case_insensitive: bool = case_insensitive,
         on_error: t.Optional[error_handler] = on_error,
     ):
         from django.contrib.contenttypes.fields import GenericForeignKey
 
         self.model_cls = model_cls
         self.lookup_field = str(
             lookup_field or getattr(self.model_cls._meta.pk, "name", "id")
         )
         self.on_error = on_error
         self.case_insensitive = case_insensitive
         field = self.model_cls._meta.get_field(self.lookup_field)
-        assert not isinstance(field, (ForeignObjectRel, GenericForeignKey)), _(
+        assert not isinstance(field, (models.ForeignObjectRel, GenericForeignKey)), _(
             "{cls} is not a supported lookup field."
         ).format(cls=self._field.__class__.__name__)
         self._field = field
         if self.case_insensitive and "iexact" in self._field.get_lookups():
             self._lookup = "__iexact"
-        self.__name__ = (
-            str(self.model_cls._meta.verbose_name)
-            if self.model_cls._meta.verbose_name
-            else self.model_cls.__name__
-        )
+        self.__name__ = self._get_metavar()
 
     def convert(
         self, value: t.Any, param: t.Optional[Parameter], ctx: t.Optional[Context]
     ):
         """
         Invoke the parsing action on the given string. If the value is
         already a model instance of the expected type the value will
@@ -126,15 +137,15 @@
         :param ctx: The context of the command.
         :raises CommandError: If the lookup fails and no error handler is
             provided.
         """
         try:
             if isinstance(value, self.model_cls):
                 return value
-            if isinstance(self._field, UUIDField):
+            if isinstance(self._field, models.UUIDField):
                 uuid = ""
                 for char in value:
                     if char.isalnum():
                         uuid += char
                 value = UUID(uuid)
             return self.model_cls.objects.get(
                 **{f"{self.lookup_field}{self._lookup}": value}
```

### Comparing `django_typer-1.1.2/django_typer/patch.py` & `django_typer-2.0.0/django_typer/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Mostly because typer does not allow direct access to the rich console objects it
 creates we need to do some monkey patching to get the desired behavior when
 --no-color options or --force-color options are specified
 
 apply() needs to be called before any imports from Typer
 
 .. todo::
-    
+
     Revisit this if Typer exposes control of the console objects.
 
 To achieve expected --force-color and --no-color behavior there are 3 different
 console objects installed when rich is used:
 
 - The first is the global exception handler installed by rich - see apps.py
 - The second is the command exception handler console installed by typer - see below
@@ -125,15 +125,15 @@
     # but this is the easiest
     from click import _compat
 
     strip_ansi = _compat.strip_ansi
     _compat.strip_ansi = lambda value: strip_ansi(str(value))
 
 
-from typer import __version__ as typer_version
+from typer import __version__ as typer_version  # noqa: E402
 
 if (0, 4, 0) <= tuple(int(v) for v in typer_version.split(".")) < (0, 13, 0):
     from typer import main as typer_main
     from typer.models import ParamMeta
 
     upstream_get_click_param = typer_main.get_click_param
```

### Comparing `django_typer-1.1.2/django_typer/types.py` & `django_typer-2.0.0/django_typer/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 else:
     from typing import Annotated
 
 from django.core.management import CommandError
 from django.utils.translation import gettext_lazy as _
 from typer import Option
 
+from .completers import complete_directory, complete_import_path
+
 COMMON_PANEL = "Django"
 
 
 def print_version(context, _, value):
     """
     A callback to run the get_version() routine of the
     command when --version is specified.
@@ -108,14 +110,15 @@
             _(
                 "The Python path to a settings module, e.g. "
                 '"myproject.settings.main". If this isn\'t provided, the '
                 "DJANGO_SETTINGS_MODULE environment variable will be used."
             ),
         ),
         rich_help_panel=COMMON_PANEL,
+        shell_complete=complete_import_path,
     ),
 ]
 """
 The type hint for the 
 `Django --settings option <https://docs.djangoproject.com/en/stable/ref/django-admin/#cmdoption-settings>`_.
 
 The --settings option is included by default and behaves the same as on BaseCommand_ use it to
@@ -130,14 +133,15 @@
             str,
             _(
                 "A directory to add to the Python path, e.g. "
                 '"/home/djangoprojects/myproject".'
             ),
         ),
         rich_help_panel=COMMON_PANEL,
+        shell_complete=complete_directory,
     ),
 ]
 """
 The type hint for the 
 `Django --pythonpath option <https://docs.djangoproject.com/en/stable/ref/django-admin/#cmdoption-pythonpath>`_.
 
 The --pythonpath option is included by default and behaves the same as on BaseCommand_ use it to
```

### Comparing `django_typer-1.1.2/pyproject.toml` & `django_typer-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-typer"
-version = "1.1.2"
+version = "2.0.0"
 description = "Use Typer to define the CLI for your Django management commands."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bckohan/django-typer"
 homepage = "https://django-typer.readthedocs.io"
 keywords = ["django", "CLI", "management", "Typer", "commands"]
@@ -58,41 +58,42 @@
 # we need this on 3.8 for Annotated types and 3.9 for ParamSpec
 typing-extensions = { version = ">=3.7.4.3", markers = "python_version < '3.10'" }
 
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.13"
 pytest-django = "^4.7.0"
-isort = "^5.13.0"
 pytest-cov = "^4.1.0"
 Sphinx = [
     { version = "^7.2.0", markers = "python_version > '3.8'" },
     { version = "^7.0.0", markers = "python_version <= '3.8'" },
 ]
 sphinx-rtd-theme = "^2.0.0"
 mypy = "^1.0"
 pylint = "^3.0"
-black = ">=23.12"
 doc8 = "^1.1.1"
 aiohttp = "^3.9.1"
 readme-renderer = {extras = ["md"], version = ">=42,<44"}
-sphinxcontrib-typer = {extras = ["html", "pdf", "png"], version = "^0.2.0"}
+sphinxcontrib-typer = {extras = ["html", "pdf", "png"], version = "^0.2.5", markers="python_version >= '3.9'"}
 scikit-learn = "^1.0.0"
 pytest-env = "^1.0.0"
 numpy = [
     { version = ">=1.26", markers = "python_version > '3.8'" },
     { version = "<=1.24", markers = "python_version <= '3.8'" },
 ]
 scipy = [
     { version = ">=1.11", markers = "python_version > '3.8'" },
     { version = "<=1.10", markers = "python_version <= '3.8'" },
 ]
 django-stubs = "^4.2.7"
 pexpect = "^4.9.0"
 pyright = "^1.1.357"
+ruff = "^0.4.1"
+graphviz = "^0.20.3"
+sphinx-tabs = "^3.4.5"
 
 [tool.poetry.extras]
 rich = ["rich"]
 
 [tool.mypy]
 # The mypy configurations: http://bit.ly/2zEl9WI
 allow_redefinition = false
@@ -109,68 +110,53 @@
 local_partial_types = true
 no_implicit_optional = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 warn_unused_configs = true
 warn_unreachable = true
 warn_no_return = true
-exclude = [
-    "tests",
-    "examples"
-]
+exclude = ["tests"]
 
 
 # todo doc8 configuration here is not being picked up and doesnt seem to be working
 # as expected - for now pass these parameters manually
 [tool.doc8]
 max-line-length = 100
 sphinx = true
 
-[tool.isort]
-profile = "black"
-
-
 [tool.pytest.ini_options]
 # py.test options:
-DJANGO_SETTINGS_MODULE = "django_typer.tests.settings"
-python_files = "tests.py"
-norecursedirs = "*.egg .eggs dist build docs .tox .git __pycache__"
+DJANGO_SETTINGS_MODULE = "django_typer.tests.settings.base"
+python_files = "test_*.py"
+norecursedirs = "*.egg .eggs dist build docs .tox .git __pycache__ shellcompletion"
 env = [
     "TERMINAL_WIDTH=80",
 ]
 
 addopts = [
   "--strict-markers",
   "--cov=django_typer",
   "--cov-branch",
   "--cov-report=term-missing:skip-covered"
 ]
 
 [tool.coverage.run]
-omit = [
-  "django_typer/tests/**/*.py",
-  "django_typer/examples/**/*.py"
-]
+omit = ["django_typer/tests/**/*.py"]
 branch = true
 source = ["django_typer"]
 concurrency = ["multiprocessing"]
 parallel = true
 relative_files = true
 command_line = "-m pytest --cov=django_typer"
 
 [tool.coverage.paths]
 source = [
     "django_typer"
 ]
 
-
-[tool.black]
-target-version = ["py38", "py39", "py310", "py311", "py312"]
-include = '\.pyi?$'
-
 [pylint]
 output-format = "colorized"
 max-line-length = 88
 
 [tool.pylint.'DESIGN']
 max-args=30
 max-locals=30  # there are lots of options!
@@ -189,14 +175,24 @@
     'C0415', # imports outside top level. I put them where they need to be!
     'C0413', # wrong import order. I put them where they need to be!
     'C0411', # wrong import order. I put them where they need to be!
     'W0603', # Using the global statement
 ]
 
 [tool.pyright]
-exclude = [
-    "django_typer/tests/**/*",
-    "django_typer/examples/**/*"
-]
+exclude = ["django_typer/tests/**/*"]
 include = [
     "django_typer"
 ]
+
+[tool.ruff]
+line-length = 88
+exclude = [
+    "doc",
+    "dist",
+    "examples"
+]
+
+[tool.ruff.lint]
+exclude = [
+    "django_typer/tests/**/*"
+]
```

### Comparing `django_typer-1.1.2/PKG-INFO` & `django_typer-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typer
-Version: 1.1.2
+Version: 2.0.0
 Summary: Use Typer to define the CLI for your Django management commands.
 Home-page: https://django-typer.readthedocs.io
 License: MIT
 Keywords: django,CLI,management,Typer,commands
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -41,36 +41,38 @@
 Project-URL: Repository, https://github.com/bckohan/django-typer
 Description-Content-Type: text/markdown
 
 # django-typer
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI version](https://badge.fury.io/py/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
 [![PyPI djversions](https://img.shields.io/pypi/djversions/django-typer.svg)](https://pypi.org/project/django-typer/)
 [![PyPI status](https://img.shields.io/pypi/status/django-typer.svg)](https://pypi.python.org/pypi/django-typer)
 [![Documentation Status](https://readthedocs.org/projects/django-typer/badge/?version=latest)](http://django-typer.readthedocs.io/?badge=latest/)
 [![Code Cov](https://codecov.io/gh/bckohan/django-typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://codecov.io/gh/bckohan/django-typer)
 [![Test Status](https://github.com/bckohan/django-typer/workflows/test/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/test.yml)
 [![Lint Status](https://github.com/bckohan/django-typer/workflows/lint/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/lint.yml)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Use [Typer](https://typer.tiangolo.com/) to define the CLI for your [Django](https://www.djangoproject.com/) management commands. Provides a TyperCommand class that inherits from [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) and allows typer-style annotated parameter types. All of the BaseCommand functionality is preserved, so that TyperCommand can be a drop-in replacement.
+Use static typing to define the CLI for your [Django](https://www.djangoproject.com/) management commands with [Typer](https://typer.tiangolo.com/). Optionally use the provided [TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) class that inherits from [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand). This class maps the [Typer](https://typer.tiangolo.com/) interface onto a class based interface that Django developers will be familiar with. All of the [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) functionality is preserved, so that [TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) can be a drop in replacement.
 
 **django-typer makes it easy to:**
 
-- Define your command CLI interface in a clear, DRY, and safe way using type hints.
-- Create subcommand and group command hierarchies.
-- Use the full power of Typer's parameter types to validate and parse command line inputs.
-- Create beautiful and information dense help outputs.
-- Configure the rendering of exception stack traces using rich.
-- [Install shell tab-completion support](https://django-typer.readthedocs.io/en/latest/shell_completion.html) for TyperCommands and normal Django commands for [bash](https://www.gnu.org/software/bash/), [zsh](https://www.zsh.org/), [fish](https://fishshell.com/), and [powershell](https://learn.microsoft.com/en-us/powershell/scripting/overview).
-- [Create custom and portable shell tab-completions for your CLI parameters.](https://django-typer.readthedocs.io/en/latest/shell_completion.html#defining-custom-completions)
-- Refactor existing management commands into TyperCommands because TyperCommand is interface compatible with BaseCommand.
+   * Define your command CLI interface in a clear, DRY and safe way using type hints
+   * Create subcommands and hierarchical groups of commands.
+   * Use the full power of [Typer](https://typer.tiangolo.com/)'s parameter types to validate and parse command line inputs.
+   * Create beautiful and information dense help outputs.
+   * Configure the rendering of exception stack traces using [rich](https://rich.readthedocs.io/en/latest/).
+   * [Install shell tab-completion support](https://django-typer.readthedocs.io/en/latest/shell_completion.html) for [bash](https://www.gnu.org/software/bash/), [zsh](https://www.zsh.org/), [fish](https://fishshell.com/), and [powershell](https://learn.microsoft.com/en-us/powershell/scripting/overview).
+   * [Create custom and portable shell tab-completions for your CLI parameters.](https://django-typer.readthedocs.io/en/latest/shell_completion.html#defining-custom-completions)
+   * Port existing commands ([TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) is interface compatible with [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand)).
+   * Use either a Django-style class-based interface or the Typer-style interface to define commands.
+   * Add plugins to upstream commands.
 
 Please refer to the [full documentation](https://django-typer.readthedocs.io/) for more information.
 
 ![django-typer example](https://raw.githubusercontent.com/bckohan/django-typer/main/doc/source/_static/img/closepoll_example.gif)
 
 ## Installation
 
@@ -82,39 +84,53 @@
 
    [rich](https://rich.readthedocs.io/en/latest/) is a powerful library for rich text and beautiful formatting in the terminal. It is not required but highly recommended for the best experience:
 
    ```bash
    pip install "django-typer[rich]"
    ```
 
-2. Add `django_typer` to your `INSTALLED_APPS` setting:
+2. Optionally add `django_typer` to your `INSTALLED_APPS` setting:
 
    ```python
    INSTALLED_APPS = [
        ...
        'django_typer',
    ]
    ```
 
 *You only need to install django_typer as an app if you want to use the shell completion command to enable tab-completion or if you would like django-typer to install [rich traceback rendering](https://django-typer.readthedocs.io/en/latest/howto.html#configure-rich-stack-traces) for you - which it does by default if rich is also installed.*
 
 ## Basic Example
 
-For example, TyperCommands can be a very simple drop-in replacement for BaseCommands. All of the documented features of [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) work!
+[TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) is a very simple drop in replacement for [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand). All of the documented features of [BaseCommand](https://docs.djangoproject.com/en/stable/howto/custom-management-commands/#django.core.management.BaseCommand) work the same way!
 
 ```python
 from django_typer import TyperCommand
 
 class Command(TyperCommand):
     def handle(self, arg1: str, arg2: str, arg3: float = 0.5, arg4: int = 1):
         """
         A basic command that uses Typer
         """
 ```
 
+Or, you may also use an interface identical to [Typer](https://typer.tiangolo.com/)'s. Simply import [Typer](https://typer.tiangolo.com/) from django_typer instead of typer.
+
+```python
+from django_typer import Typer
+
+app = Typer()
+
+@app.command()
+def main(arg1: str, arg2: str, arg3: float = 0.5, arg4: int = 1):
+   """
+   A basic command that uses Typer
+   """
+```
+
 ![Basic Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/basic.svg)
 
 ## Multiple Subcommands Example
 
 
 
 Commands with multiple subcommands can be defined:
@@ -148,27 +164,57 @@
       ):
          """
          Delete an object.
          """
 
 ```
 
+Or using the typer-style interface this could be written:
+
+```python
+from django_typer import Typer
+import typing as t
+
+from django.utils.translation import gettext_lazy as _
+from typer import Argument
+
+app = Typer(help="A command that defines subcommands.")
+
+@app.command()
+def create(
+   name: t.Annotated[str, Argument(help=_("The name of the object to create."))],
+):
+   """
+   Create an object.
+   """
+
+@app.command()
+def delete(
+   id: t.Annotated[int, Argument(help=_("The id of the object to delete."))]
+):
+   """
+   Delete an object.
+   """
+```
+
 ![Multiple Subcommands Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi.svg)
 ![Multiple Subcommands Example - create](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_create.svg)
 ![Multiple Subcommands Example - delete](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/multi_delete.svg)
 
 ## Grouping and Hierarchies Example
 
 More complex groups and subcommand hierarchies can be defined. For example, this command defines a group of commands called math, with subcommands divide and multiply. The group has a common initializer that optionally sets a float precision value. We would invoke this command like so:
 
 ```bash
 ./manage.py hierarchy math --precision 5 divide 10 2.1
 ./manage.py hierarchy math multiply 10 2
 ```
 
+Using the class-based interface we could define the command like this:
+
 ```python
    import typing as t
    from functools import reduce
 
    from django.utils.translation import gettext_lazy as _
    from typer import Argument, Option
 
@@ -186,23 +232,26 @@
          self,
          precision: t.Annotated[
             int, Option(help=_("The number of decimal places to output."))
          ] = precision,
       ):
          self.precision = precision
 
+      # helps can be passed to the decorators
       @math.command(help=_("Multiply the given numbers."))
       def multiply(
          self,
          numbers: t.Annotated[
             t.List[float], Argument(help=_("The numbers to multiply"))
          ],
       ):
          return f"{reduce(lambda x, y: x * y, [1, *numbers]):.{self.precision}f}"
 
+      # or if no help is supplied to the decorators, the docstring if present
+      # will be used!
       @math.command()
       def divide(
          self,
          numerator: t.Annotated[float, Argument(help=_("The numerator"))],
          denominator: t.Annotated[float, Argument(help=_("The denominator"))],
          floor: t.Annotated[bool, Option(help=_("Use floor division"))] = False,
       ):
@@ -211,12 +260,66 @@
          """
          if floor:
                return str(numerator // denominator)
          return f"{numerator / denominator:.{self.precision}f}"
 
 ```
 
+The typer-style interface builds a [TyperCommand](https://django-typer.readthedocs.io/en/latest/reference.html#django_typer.TyperCommand) class for us **that allows you to optionally accept the self argument in your commands.** We could define the above command using the typer interface like this:
+
+```python
+
+import typing as t
+from functools import reduce
+
+from django.utils.translation import gettext_lazy as _
+from typer import Argument, Option
+
+from django_typer import Typer
+
+
+app = Typer(help=_("A more complex command that defines a hierarchy of subcommands."))
+
+
+math_grp = Typer(help=_("Do some math at the given precision."))
+
+app.add_typer(math_grp)
+
+@math_grp.callback()
+def math(
+   self,
+   precision: t.Annotated[
+      int, Option(help=_("The number of decimal places to output."))
+   ] = 2,
+):
+   self.precision = precision
+
+
+@math_grp.command(help=_("Multiply the given numbers."))
+def multiply(
+   self,
+   numbers: t.Annotated[
+      t.List[float], Argument(help=_("The numbers to multiply"))
+   ],
+):
+   return f"{reduce(lambda x, y: x * y, [1, *numbers]):.{self.precision}f}"
+
+@math_grp.command()
+def divide(
+   self,
+   numerator: t.Annotated[float, Argument(help=_("The numerator"))],
+   denominator: t.Annotated[float, Argument(help=_("The denominator"))],
+   floor: t.Annotated[bool, Option(help=_("Use floor division"))] = False,
+):
+   """
+   Divide the given numbers.
+   """
+   if floor:
+         return str(numerator // denominator)
+   return f"{numerator / denominator:.{self.precision}f}"
+```
+
 ![Grouping and Hierarchies Example](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy.svg)
 ![Grouping and Hierarchies Example - math](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math.svg)
 ![Grouping and Hierarchies Example - math multiply](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_multiply.svg)
 ![Grouping and Hierarchies Example - math divide](https://raw.githubusercontent.com/bckohan/django-typer/main/django_typer/examples/helps/hierarchy_math_divide.svg)
```

